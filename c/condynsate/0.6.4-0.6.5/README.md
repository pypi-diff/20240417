# Comparing `tmp/condynsate-0.6.4.tar.gz` & `tmp/condynsate-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "condynsate-0.6.4.tar", last modified: Fri Apr 12 20:04:34 2024, max compression
+gzip compressed data, was "condynsate-0.6.5.tar", last modified: Wed Apr 17 17:08:03 2024, max compression
```

## Comparing `condynsate-0.6.4.tar` & `condynsate-0.6.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 20:04:34.760053 condynsate-0.6.4/
--rw-rw-rw-   0        0        0     1092 2023-11-24 19:50:22.000000 condynsate-0.6.4/LICENSE
--rw-rw-rw-   0        0        0     4875 2024-04-12 20:04:34.744441 condynsate-0.6.4/PKG-INFO
--rw-rw-rw-   0        0        0     2391 2024-03-21 21:05:21.000000 condynsate-0.6.4/README.md
--rw-rw-rw-   0        0        0     1439 2024-04-12 20:03:40.000000 condynsate-0.6.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 20:04:34.760053 condynsate-0.6.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-12 20:04:34.665519 condynsate-0.6.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-12 20:04:34.681931 condynsate-0.6.4/src/condynsate/
-drwxrwxrwx   0        0        0        0 2024-04-12 20:04:34.744441 condynsate-0.6.4/src/condynsate/__assets__/
--rw-rw-rw-   0        0        0    36584 2023-11-24 19:50:22.000000 condynsate-0.6.4/src/condynsate/__assets__/arrow_ccw.stl
--rw-rw-rw-   0        0        0    36584 2023-11-24 19:50:22.000000 condynsate-0.6.4/src/condynsate/__assets__/arrow_cw.stl
--rw-rw-rw-   0        0        0     6784 2023-11-24 19:50:22.000000 condynsate-0.6.4/src/condynsate/__assets__/arrow_lin.stl
--rw-rw-rw-   0        0        0     6379 2023-11-24 19:50:22.000000 condynsate-0.6.4/src/condynsate/__assets__/check.png
--rw-rw-rw-   0        0        0      684 2023-11-24 19:50:22.000000 condynsate-0.6.4/src/condynsate/__assets__/cube.stl
--rw-rw-rw-   0        0        0    12684 2023-12-12 22:20:42.000000 condynsate-0.6.4/src/condynsate/__assets__/cylinder.stl
--rw-rw-rw-   0        0        0    12684 2023-12-12 22:33:34.000000 condynsate-0.6.4/src/condynsate/__assets__/cylinder_lower_origin.stl
--rw-rw-rw-   0        0        0    11484 2024-01-05 02:07:25.000000 condynsate-0.6.4/src/condynsate/__assets__/gate_med.stl
--rw-rw-rw-   0        0        0     4084 2024-01-05 02:03:45.000000 condynsate-0.6.4/src/condynsate/__assets__/gate_short.stl
--rw-rw-rw-   0        0        0    11484 2024-01-05 02:08:19.000000 condynsate-0.6.4/src/condynsate/__assets__/gate_tall.stl
--rw-rw-rw-   0        0        0      344 2023-11-24 19:50:22.000000 condynsate-0.6.4/src/condynsate/__assets__/plane_big.obj
--rw-rw-rw-   0        0        0      332 2023-11-24 19:50:22.000000 condynsate-0.6.4/src/condynsate/__assets__/plane_med.obj
--rw-rw-rw-   0        0        0      320 2023-11-24 19:50:22.000000 condynsate-0.6.4/src/condynsate/__assets__/plane_small.obj
--rw-rw-rw-   0        0        0      384 2023-11-24 19:50:22.000000 condynsate-0.6.4/src/condynsate/__assets__/pyramid.stl
--rw-rw-rw-   0        0        0    61284 2023-11-24 19:50:22.000000 condynsate-0.6.4/src/condynsate/__assets__/sphere.stl
--rw-rw-rw-   0        0        0      153 2024-04-12 20:03:30.000000 condynsate-0.6.4/src/condynsate/__init__.py
--rw-rw-rw-   0        0        0    44652 2023-12-15 21:36:13.000000 condynsate-0.6.4/src/condynsate/animator.py
--rw-rw-rw-   0        0        0     8209 2024-02-06 15:55:34.000000 condynsate-0.6.4/src/condynsate/keyboard.py
--rw-rw-rw-   0        0        0   145453 2024-04-12 19:30:44.000000 condynsate-0.6.4/src/condynsate/simulator.py
--rw-rw-rw-   0        0        0    10805 2024-04-12 19:31:07.000000 condynsate-0.6.4/src/condynsate/utils.py
--rw-rw-rw-   0        0        0    23281 2024-04-12 17:33:51.000000 condynsate-0.6.4/src/condynsate/visualizer.py
-drwxrwxrwx   0        0        0        0 2024-04-12 20:04:34.744441 condynsate-0.6.4/src/condynsate.egg-info/
--rw-rw-rw-   0        0        0     4875 2024-04-12 20:04:34.000000 condynsate-0.6.4/src/condynsate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      981 2024-04-12 20:04:34.000000 condynsate-0.6.4/src/condynsate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 20:04:34.000000 condynsate-0.6.4/src/condynsate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-04-12 20:04:34.000000 condynsate-0.6.4/src/condynsate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-12 20:04:34.000000 condynsate-0.6.4/src/condynsate.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 17:08:03.713805 condynsate-0.6.5/
+-rw-rw-rw-   0        0        0     1092 2023-11-24 19:50:22.000000 condynsate-0.6.5/LICENSE
+-rw-rw-rw-   0        0        0     4875 2024-04-17 17:08:03.711805 condynsate-0.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2391 2024-03-21 21:05:21.000000 condynsate-0.6.5/README.md
+-rw-rw-rw-   0        0        0     1439 2024-04-17 17:07:18.000000 condynsate-0.6.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-17 17:08:03.713805 condynsate-0.6.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 17:08:03.639212 condynsate-0.6.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-17 17:08:03.655216 condynsate-0.6.5/src/condynsate/
+drwxrwxrwx   0        0        0        0 2024-04-17 17:08:03.709805 condynsate-0.6.5/src/condynsate/__assets__/
+-rw-rw-rw-   0        0        0    36584 2023-11-24 19:50:22.000000 condynsate-0.6.5/src/condynsate/__assets__/arrow_ccw.stl
+-rw-rw-rw-   0        0        0    36584 2023-11-24 19:50:22.000000 condynsate-0.6.5/src/condynsate/__assets__/arrow_cw.stl
+-rw-rw-rw-   0        0        0     6784 2023-11-24 19:50:22.000000 condynsate-0.6.5/src/condynsate/__assets__/arrow_lin.stl
+-rw-rw-rw-   0        0        0     6379 2023-11-24 19:50:22.000000 condynsate-0.6.5/src/condynsate/__assets__/check.png
+-rw-rw-rw-   0        0        0      684 2023-11-24 19:50:22.000000 condynsate-0.6.5/src/condynsate/__assets__/cube.stl
+-rw-rw-rw-   0        0        0    12684 2023-12-12 22:20:42.000000 condynsate-0.6.5/src/condynsate/__assets__/cylinder.stl
+-rw-rw-rw-   0        0        0    12684 2023-12-12 22:33:34.000000 condynsate-0.6.5/src/condynsate/__assets__/cylinder_lower_origin.stl
+-rw-rw-rw-   0        0        0    11484 2024-01-05 02:07:25.000000 condynsate-0.6.5/src/condynsate/__assets__/gate_med.stl
+-rw-rw-rw-   0        0        0     4084 2024-01-05 02:03:45.000000 condynsate-0.6.5/src/condynsate/__assets__/gate_short.stl
+-rw-rw-rw-   0        0        0    11484 2024-01-05 02:08:19.000000 condynsate-0.6.5/src/condynsate/__assets__/gate_tall.stl
+-rw-rw-rw-   0        0        0      344 2023-11-24 19:50:22.000000 condynsate-0.6.5/src/condynsate/__assets__/plane_big.obj
+-rw-rw-rw-   0        0        0      332 2023-11-24 19:50:22.000000 condynsate-0.6.5/src/condynsate/__assets__/plane_med.obj
+-rw-rw-rw-   0        0        0      320 2023-11-24 19:50:22.000000 condynsate-0.6.5/src/condynsate/__assets__/plane_small.obj
+-rw-rw-rw-   0        0        0      384 2023-11-24 19:50:22.000000 condynsate-0.6.5/src/condynsate/__assets__/pyramid.stl
+-rw-rw-rw-   0        0        0    61284 2023-11-24 19:50:22.000000 condynsate-0.6.5/src/condynsate/__assets__/sphere.stl
+-rw-rw-rw-   0        0        0      153 2024-04-17 17:07:18.000000 condynsate-0.6.5/src/condynsate/__init__.py
+-rw-rw-rw-   0        0        0    44652 2023-12-15 21:36:13.000000 condynsate-0.6.5/src/condynsate/animator.py
+-rw-rw-rw-   0        0        0     8681 2024-04-17 16:50:25.000000 condynsate-0.6.5/src/condynsate/keyboard.py
+-rw-rw-rw-   0        0        0   151710 2024-04-17 17:03:11.000000 condynsate-0.6.5/src/condynsate/simulator.py
+-rw-rw-rw-   0        0        0    10805 2024-04-12 19:31:07.000000 condynsate-0.6.5/src/condynsate/utils.py
+-rw-rw-rw-   0        0        0    22871 2024-04-15 16:06:31.000000 condynsate-0.6.5/src/condynsate/visualizer.py
+drwxrwxrwx   0        0        0        0 2024-04-17 17:08:03.710805 condynsate-0.6.5/src/condynsate.egg-info/
+-rw-rw-rw-   0        0        0     4875 2024-04-17 17:08:03.000000 condynsate-0.6.5/src/condynsate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      981 2024-04-17 17:08:03.000000 condynsate-0.6.5/src/condynsate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 17:08:03.000000 condynsate-0.6.5/src/condynsate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-04-17 17:08:03.000000 condynsate-0.6.5/src/condynsate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-17 17:08:03.000000 condynsate-0.6.5/src/condynsate.egg-info/top_level.txt
```

### Comparing `condynsate-0.6.4/LICENSE` & `condynsate-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.4/PKG-INFO` & `condynsate-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: condynsate
-Version: 0.6.4
+Version: 0.6.5
 Summary: Simulates and visualizes articulated systems in real time
 Author-email: Grayson Schaer <gschaer2@illinois.edu>
 License: MIT License
         
         Copyright (c) 2023 Grayson Schaer
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `condynsate-0.6.4/README.md` & `condynsate-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.4/pyproject.toml` & `condynsate-0.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "condynsate"
-version = "0.6.4"
+version = "0.6.5"
 description = "Simulates and visualizes articulated systems in real time"
 readme = "README.md"
 authors = [{ name = "Grayson Schaer", email = "gschaer2@illinois.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `condynsate-0.6.4/src/condynsate/__assets__/arrow_ccw.stl` & `condynsate-0.6.5/src/condynsate/__assets__/arrow_ccw.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.4/src/condynsate/__assets__/arrow_cw.stl` & `condynsate-0.6.5/src/condynsate/__assets__/arrow_cw.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.4/src/condynsate/__assets__/arrow_lin.stl` & `condynsate-0.6.5/src/condynsate/__assets__/arrow_lin.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.4/src/condynsate/__assets__/check.png` & `condynsate-0.6.5/src/condynsate/__assets__/check.png`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.4/src/condynsate/__assets__/cylinder.stl` & `condynsate-0.6.5/src/condynsate/__assets__/cylinder.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.4/src/condynsate/__assets__/cylinder_lower_origin.stl` & `condynsate-0.6.5/src/condynsate/__assets__/cylinder_lower_origin.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.4/src/condynsate/__assets__/gate_med.stl` & `condynsate-0.6.5/src/condynsate/__assets__/gate_med.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.4/src/condynsate/__assets__/gate_short.stl` & `condynsate-0.6.5/src/condynsate/__assets__/gate_short.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.4/src/condynsate/__assets__/gate_tall.stl` & `condynsate-0.6.5/src/condynsate/__assets__/gate_tall.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.4/src/condynsate/__assets__/sphere.stl` & `condynsate-0.6.5/src/condynsate/__assets__/sphere.stl`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.4/src/condynsate/animator.py` & `condynsate-0.6.5/src/condynsate/animator.py`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.4/src/condynsate/keyboard.py` & `condynsate-0.6.5/src/condynsate/keyboard.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,14 +31,16 @@
         None.
 
         """
         # Set that no key is down
         self.down = False
         self.key_buffer = []
         self.mod_key_buffer = []
+        self.len_key_buffer = 0
+        self.len_mod_key_buffer = 0
         
         # Asynch listen for script exit
         signal.signal(signal.SIGTERM, self._signal_handler)
         signal.signal(signal.SIGINT, self._signal_handler)
         
         # Start the keyboard listener
         self.listener = keyboard.Listener(on_press=self._on_press,
@@ -121,32 +123,36 @@
     
     def _add_to_buffer(self,
                        key_str):
         # Handle modifiers
         if key_str=="shift+" or key_str=="ctrl+" or key_str=="alt+":
             if key_str not in self.mod_key_buffer:
                 self.mod_key_buffer.append(key_str)
+                self.len_mod_key_buffer = self.len_mod_key_buffer + 1
             
         # Handle other keys
         else:
             if key_str not in self.key_buffer:
                 self.key_buffer.append(key_str)
+                self.len_key_buffer = self.len_key_buffer + 1
     
     
     def _remove_from_buffer(self,
                             key_str):
         # Handle modifiers
         if key_str=="shift+" or key_str=="ctrl+" or key_str=="alt+":
             if key_str in self.mod_key_buffer:
                 self.mod_key_buffer.pop(self.mod_key_buffer.index(key_str))
+                self.len_mod_key_buffer = self.len_mod_key_buffer - 1
             
         # Handle other keys
         else:
             if key_str in self.key_buffer:
                 self.key_buffer.pop(self.key_buffer.index(key_str))
+                self.len_key_buffer = self.len_key_buffer - 1
             
 
 
     def _on_press(self,
                   key):
         """
         Takes place on a key down event. Stores the pressed key as a unique
@@ -194,15 +200,15 @@
         # Determine if it's time to stop listening
         leave = key_str == "esc"
         
         # Remove the released key from the key buffer
         self._remove_from_buffer(key_str)
         
         # If the buffer is empty, note that no keys are down
-        if len(self.key_buffer) == 0 and len(self.mod_key_buffer):
+        if self.len_key_buffer == 0 and self.len_mod_key_buffer == 0:
             self.down = False
         
         # Stop the listener gracefully
         if leave:
             # Wait for 0.5 seconds before leaving
             time.sleep(0.5)
             print("Termination command detected. " + 
@@ -240,31 +246,35 @@
         -------
         bool
             A boolean flag to indicate whether the desired key is pressed.
 
         """
         key = key_str
         mods = []
+        len_mods = 0
         
         # Disambiguate mods from keys
         if ("shift+" in key):
             key = key.replace('shift+','')
             mods.append('shift+')
+            len_mods = len_mods + 1
         if ("ctrl+" in key):
             key = key.replace('ctrl+','')
             mods.append('ctrl+')
+            len_mods = len_mods + 1
         if ("alt+" in key):
             key = key.replace('alt+','')
             mods.append('alt+')
+            len_mods = len_mods + 1
             
         # Determine if correct key is down
         key_is_down = key in self.key_buffer
         
         # Determine if correct mods are down
-        if len(mods) == 0:
-            mods_are_down = len(self.mod_key_buffer)==0
+        if len_mods == 0:
+            mods_are_down = self.len_mod_key_buffer==0
         else:
             mods_are_down = all([mod in self.mod_key_buffer for mod in mods])
         
         # Return whether the proper keys and modifiers are pressed
         return key_is_down and mods_are_down
```

### Comparing `condynsate-0.6.4/src/condynsate/simulator.py` & `condynsate-0.6.5/src/condynsate/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,21 +51,44 @@
             by the visualizer each time step.
             
         Returns
         -------
         None.
 
         """
+        # Identification number
         self.urdf_id = urdf_id
+        
+        # Maps that link a link name to the parent joint id num or link id num
         self.joint_map = joint_map
-        self.link_map = link_map     
+        self.link_map = link_map
+        
+        # Boolean flag that indicates whether or not this urdf is
+        # visually dynamic (True) or visually static (False)
         self.update_vis = update_vis
+        
+        # A list of initial conditions of the URDF. URDF reset to this 
+        # state when the simulator is reset
         self.initial_conds = {}
+        
+        # Lists that contain the visual geometrys and textures of the URDF
+        # in order of link id. One per link
         self.geometries = []
         self.textures = []
+        
+        # Structure that contains a bool to indicate if the stored
+        # CoM is valid (True) or stale (needs to be recalculated) (False)
+        # as well as the stored CoM
+        self.center_of_mass = [False, np.array([0., 0., 0.])]
+        
+        # Structure that contains bools to indicate if the stored
+        # world and body base state valid (True) or stale
+        # (needs to be recalculated) (False) as well as the stored base state
+        # in world coords and body coords
+        self.base_state = [False, {}, False, {}]
 
 
 ###############################################################################
 #SIMULATOR CLASS
 ###############################################################################
 class Simulator:
     """
@@ -496,14 +519,33 @@
                                                   forces=[0])
             
             
     def _set_max_joint_vel(self,
                             urdf_obj,
                             joint_name,
                             max_vel=1000.):
+        """
+        Sets the maximum joint velocity of a specific joint on a given URDF.
+
+        Parameters
+        ----------
+        urdf_obj : URDF_Obj
+            A URDF_Obj that contains that joint whose max velocity is set
+        joint_name : string
+            The name of the joint whose max velocity is set. The
+            joint name is specified in the .urdf file.
+        max_vel : float, optional
+            The maximum joint velocity. For angular joints in rad/sec.
+            The default is 1000..
+
+        Returns
+        -------
+        None.
+
+        """
         # Gather information from urdf_obj
         urdf_id = urdf_obj.urdf_id
         joint_map = urdf_obj.joint_map
         
         # Set the max joint velocity
         if joint_name in joint_map:
             joint_id = joint_map[joint_name]
@@ -861,21 +903,32 @@
                 mode = self.engine.POSITION_CONTROL
                 position = [position]
                 self.engine.setJointMotorControlArray(urdf_id,
                                                       joint_id,
                                                       mode,
                                                       forces=[100.],
                                                       targetPositions=position)
+                
+                # Note that CoM and base state is no longer valid
+                urdf_obj.center_of_mass[0] = False
+                urdf_obj.base_state[0] = False
+                urdf_obj.base_state[2] = False
+                
             # Reset joint position
             else:
                 self.engine.resetJointState(bodyUniqueId=urdf_id,
                                             jointIndex=joint_id[0],
                                             targetValue=position,
                                             targetVelocity=0.0)
                 
+                # Note that CoM and base state is no longer valid
+                urdf_obj.center_of_mass[0] = False
+                urdf_obj.base_state[0] = False
+                urdf_obj.base_state[2] = False
+                
             # Update the initial conditions
             if initial_cond:
                 urdf_obj.initial_conds[joint_id[0]]['position'] = position
            
             # Color the link based on the position
             if color and min_pos!=None and max_pos!=None:
                 self.set_color_from_pos(urdf_obj=urdf_obj,
@@ -953,24 +1006,32 @@
                 target = [velocity]
                 self.engine.setJointMotorControlArray(urdf_id,
                                                       joint_id,
                                                       mode,
                                                       forces=[1000.],
                                                       targetVelocities=target)
                 
+                # Note that base state is no longer valid
+                urdf_obj.base_state[0] = False
+                urdf_obj.base_state[2] = False
+                
             # Set the velocity without physics
             else:
                 state = self.get_joint_state(urdf_obj=urdf_obj,
                                              joint_name=joint_name)
                 curr_pos = state['position']
                 self.engine.resetJointState(bodyUniqueId=urdf_id,
                                             jointIndex=joint_id[0],
                                             targetValue=curr_pos,
                                             targetVelocity=velocity)
                 
+                # Note that base state is no longer valid
+                urdf_obj.base_state[0] = False
+                urdf_obj.base_state[2] = False
+                
             if initial_cond:
                 urdf_obj.initial_conds[joint_id[0]]['velocity'] = velocity
                 
             # Color the link based on the velocity
             if color:
                 self.set_color_from_vel(urdf_obj=urdf_obj,
                                         joint_name=joint_name,
@@ -1251,14 +1312,17 @@
         link_map = urdf_obj.link_map
         
         # Set the link mass
         if link_name in link_map:
             joint_id = link_map[link_name]
             self.engine.changeDynamics(urdf_id, joint_id, mass=mass)
             
+            # Note that CoM is no longer valid
+            urdf_obj.center_of_mass[0] = False
+            
             # Color the link based on the position
             if color and min_mass!=None and max_mass!=None:
                 self.set_color_from_mass(urdf_obj=urdf_obj,
                                          link_name=link_name,
                                          min_mass=min_mass, 
                                          max_mass=max_mass)
                 
@@ -1450,14 +1514,19 @@
             xyzw_ori = self.engine.getQuaternionFromEuler(euler_angles)
         
         # Set the base position and orientation
         self.engine.resetBasePositionAndOrientation(bodyUniqueId=i,
                                                     posObj=position,
                                                     ornObj=xyzw_ori)
         
+        # Note that CoM and base states is no longer valid
+        urdf_obj.center_of_mass[0] = False
+        urdf_obj.base_state[0] = False
+        urdf_obj.base_state[2] = False
+        
         # Return the set position and orientation
         return position, xyzw_ori
     
     
     def _set_base_vel(self,
                       urdf_obj,
                       velocity,
@@ -1506,14 +1575,18 @@
             w_inW = np.array(ang_velocity)
             
         # Set the base velocity and angular velocity
         self.engine.resetBaseVelocity(objectUniqueId=i,
                                       linearVelocity=v_inW,
                                       angularVelocity=w_inW)
         
+        # Note that base state is no longer valid
+        urdf_obj.base_state[0] = False
+        urdf_obj.base_state[2] = False
+        
         # Return the set velocities
         return v_inW, w_inW
     
     
     def set_base_state(self,
                        urdf_obj,
                        position=None,
@@ -1693,14 +1766,20 @@
                 written in world coordinates, exactly equal to the roll rate,
                 the pitch rate, and the yaw rate.
 
         """
         # Get object id
         urdf_id = urdf_obj.urdf_id
         
+        # Check if the base state is cached
+        if (not body_coords) and urdf_obj.base_state[0]:
+            return urdf_obj.base_state[1]
+        elif body_coords and urdf_obj.base_state[2]:
+            return urdf_obj.base_state[3]
+        
         # Retrieve position and orientation in world coordinates
         O, Q = self.engine.getBasePositionAndOrientation(urdf_id)
         O_inW = O
         xyzw_ori = Q
         
         # Convert the orientation quaternion the Euler angles
         rpy = self.engine.getEulerFromQuaternion(xyzw_ori)
@@ -1735,25 +1814,37 @@
             state = {'position' : O_inW,
                      'roll' : rpy[0],
                      'pitch' : rpy[1],
                      'yaw' : rpy[2],
                      'R of world in body' : R_ofW_inB,
                      'velocity' : vel_inB,
                      'angular velocity' : ang_vel_inB}
+            
+            # Update cached state
+            urdf_obj.base_state[2] = True
+            urdf_obj.base_state[3] = state
+            
+            # Return body fixed state
             return state
         
         else:
             # Make the dictionary in world coords and return the base state
             state = {'position' : O_inW,
                      'roll' : rpy[0],
                      'pitch' : rpy[1],
                      'yaw' : rpy[2],
                      'R of world in body' : R_ofW_inB,
                      'velocity' : vel_inW,
                      'angular velocity' : ang_vel_inW}
+            
+            # Update cached state
+            urdf_obj.base_state[0] = True
+            urdf_obj.base_state[1] = state
+            
+            # Return world fixed state
             return state
     
     
     def get_center_of_mass(self,
                            urdf_obj):
         """
         Get the center of mass of a body .
@@ -1766,14 +1857,18 @@
         Returns
         -------
         com : array-like, shape(3,)
             The cartesian coordinates of the center of mass of the body in
             world coordinates.
 
         """
+        # If the current CoM is not stale, just return that
+        if urdf_obj.center_of_mass[0]:
+            return urdf_obj.center_of_mass[1]
+        
         # Gather information from urdf_obj
         urdf_id = urdf_obj.urdf_id
         link_map = urdf_obj.link_map
         
         # Get all link ids
         link_ids = list(link_map.values())
         base=False
@@ -1801,14 +1896,20 @@
             link_poss.append(link_state[0])
         
         # Get the CoM
         if total_mass == 0:
             com=np.array([0., 0., 0.])
         else:
             com = np.dot(masses, link_poss) / total_mass
+            
+        # Update the caches CoM value
+        urdf_obj.center_of_mass[0] = True
+        urdf_obj.center_of_mass[1] = com
+        
+        # Return the calculated CoM
         return com
     
     
     ###########################################################################
     #EXTERNAL FORCE AND TORQUE APPLICATION
     ###########################################################################   
     def apply_force_to_link(self,
@@ -2115,21 +2216,27 @@
         
         # Check the current status of the arrow
         arr_exists = urdf_force in self.lin_arr_map
   
         # If show_arrow is set to false, and the visualizer and associated
         # force arrow exist, set the arrows visibility to false
         if (not show_arrow) and arr_exists:
-            arr_name = str(self.lin_arr_map[urdf_force])
-            self.vis.set_link_color(urdf_name = "Force Arrows",
-                                    link_name = arr_name,
-                                    link_geometry = self.lin_geom, 
-                                    color = [0, 0, 0],
-                                    transparent = True,
-                                    opacity = 0.0)
+            # Check if the arrow is currently set to visible
+            arr_visible = self.lin_arr_map[urdf_force]['visible']
+            
+            # If the arrow is visible make changes, if not visible, do nothing
+            if arr_visible:
+                self.lin_arr_map[urdf_force]['visible'] = False
+                arr_name = self.lin_arr_map[urdf_force]['name']
+                self.vis.set_link_color(urdf_name = "Force Arrows",
+                                        link_name = arr_name,
+                                        link_geometry = self.lin_geom, 
+                                        color = [0, 0, 0],
+                                        transparent = True,
+                                        opacity = 0.0)
         
         # If show arrow is set to True and the visualizer exists, draw the
         # arrow at the position and orientation listed.
         if show_arrow:
             
             # Get the direction in which the force is applied
             f_inW_norm = np.linalg.norm(f_inW)
@@ -2146,39 +2253,45 @@
             # Get the scale of the arrow based on the magnitude of the force
             scale = arr_scale*np.linalg.norm(f_inW)*np.array([1., 1., 1.])
             scale = scale.tolist()
             
             # If the arrow already exists, only update its position and ori
             if arr_exists:
                 # Get the arrow's name
-                arr_name = str(self.lin_arr_map[urdf_force])
+                arr_name = self.lin_arr_map[urdf_force]['name']
                 
-                # Set the visibility of the arrow to True
-                self.vis.set_link_color(urdf_name = "Force Arrows",
-                                        link_name = arr_name,
-                                        link_geometry = self.lin_geom, 
-                                        color = [0, 0, 0],
-                                        transparent = False,
-                                        opacity = 1.0)
+                # Check if the arrow is currently set to visible
+                arr_visible = self.lin_arr_map[urdf_force]['visible']
+                
+                # Set the visibility of the arrow to True if False
+                if not arr_visible:
+                    self.lin_arr_map[urdf_force]['visible'] = True
+                    self.vis.set_link_color(urdf_name = "Force Arrows",
+                                            link_name = arr_name,
+                                            link_geometry = self.lin_geom, 
+                                            color = [0, 0, 0],
+                                            transparent = False,
+                                            opacity = 1.0)
                 
                 # Set the position and orientation of the arrow
                 self.vis.apply_transform(urdf_name="Force Arrows",
                                          link_name=arr_name,
                                          scale=scale,
                                          translate=arr_pos_inW,
                                          wxyz_quaternion=arr_wxyz_inW)
             
             
             # If the arrow is not already created, add it to the visualizer
             else:
                 # Add the arrow to the linear arrow map
-                self.lin_arr_map[urdf_force] = force_name
+                self.lin_arr_map[urdf_force] = {'name' : force_name,
+                                                 'visible' : True}
                 
                 # Get the arrow's name
-                arr_name = self.lin_arr_map[urdf_force]
+                arr_name = self.lin_arr_map[urdf_force]['name']
                 
                 # Get the path to the arrow asset
                 arr_path = Path(__file__).parents[0]
                 arr_path = arr_path.absolute().as_posix()
                 arr_path = arr_path + "/__assets__/arrow_lin.stl"
                 
                 # Add an arrow to the visualizer
@@ -2244,22 +2357,28 @@
         
         # Check the current status of the arrow
         arr_exists = urdf_torque in self.ccw_arr_map
         
         # If show_arrow is set to false, and the visualizer and associated
         # torque arrow exist, set the arrows visibility to false
         if (not show_arrow) and arr_exists:
-            arr_name = str(self.ccw_arr_map[urdf_torque])
-            self.vis.set_link_color(urdf_name = "Torque Arrows",
-                                    link_name = arr_name,
-                                    link_geometry = self.ccw_geom, 
-                                    color = [0, 0, 0],
-                                    transparent = True,
-                                    opacity = 0.0)
-        
+            # Check if the arrow is currently set to visible
+            arr_visible = self.ccw_arr_map[urdf_torque]['visible']
+            
+            # If the arrow is visible make changes, if not visible, do nothing
+            if arr_visible:
+                self.ccw_arr_map[urdf_torque]['visible'] = False
+                arr_name = self.ccw_arr_map[urdf_torque]['name']
+                self.vis.set_link_color(urdf_name = "Torque Arrows",
+                                        link_name = arr_name,
+                                        link_geometry = self.ccw_geom, 
+                                        color = [0, 0, 0],
+                                        transparent = True,
+                                        opacity = 0.0)
+                
         # If show arrow is set to True and the visualizer exists, draw the
         # arrow at the position and orientation listed.
         if show_arrow:
             
             # Get the direction in which the torque is applied
             t_inW_norm = np.linalg.norm(t_inW)
             if t_inW_norm != 0:
@@ -2275,39 +2394,45 @@
             # Get the scale of the arrow based on the magnitude of the torque
             scale = arr_scale*np.linalg.norm(t_inW)*np.array([1., 1., 0.05])
             scale = scale.tolist()
             
             # If the arrow already exists, only update its position and ori
             if arr_exists:
                 # Get the arrow's name
-                arr_name = str(self.ccw_arr_map[urdf_torque])
+                arr_name = self.ccw_arr_map[urdf_torque]['name']
                 
-                # Set the visibility of the arrow to True
-                self.vis.set_link_color(urdf_name = "Torque Arrows",
-                                        link_name = arr_name,
-                                        link_geometry = self.ccw_geom, 
-                                        color = [0, 0, 0],
-                                        transparent = False,
-                                        opacity = 1.0)
+                # Check if the arrow is currently set to visible
+                arr_visible = self.ccw_arr_map[urdf_torque]['visible']
+                
+                # Set the visibility of the arrow to True if False
+                if not arr_visible:
+                    self.ccw_arr_map[urdf_torque]['visible'] = True
+                    self.vis.set_link_color(urdf_name = "Torque Arrows",
+                                            link_name = arr_name,
+                                            link_geometry = self.ccw_geom, 
+                                            color = [0, 0, 0],
+                                            transparent = False,
+                                            opacity = 1.0)
                 
                 # Set the position and orientation of the arrow
                 self.vis.apply_transform(urdf_name="Torque Arrows",
                                          link_name=arr_name,
                                          scale=scale,
                                          translate=arr_pos_inW,
                                          wxyz_quaternion=arr_wxyz_inW)
             
             
             # If the arrow is not already created, add it to the visualizer
             else:
                 # Add the arrow to the linear arrow map
-                self.ccw_arr_map[urdf_torque] = torque_name
+                self.ccw_arr_map[urdf_torque] = {'name' : torque_name,
+                                                 'visible' : True}
                 
                 # Get the arrow's name
-                arr_name = self.ccw_arr_map[urdf_torque]
+                arr_name = self.ccw_arr_map[urdf_torque]['name']
                 
                 # Get the path to the arrow asset
                 arr_path = Path(__file__).parents[0]
                 arr_path = arr_path.absolute().as_posix()
                 arr_path = arr_path + "/__assets__/arrow_ccw.stl"
                 
                 # Add an arrow to the visualizer
@@ -3418,16 +3543,19 @@
                     print("QUITTING...")
                     return
                 
                 # Start condition
                 if self.is_pressed(key):
                     print("CONTINUING...")
                     return
+                
+                # Add a sleep to reduce CPU usage
+                time.sleep(0.05)
             
-        # If there is not a keyboard, wait 1 second then return
+        # If there is not a keyboard, wait 1.0 seconds then return
         else:
             start_time = time.time()
             while (time.time() - start_time) < 1.0:
                 # Ensure so the GUI remains interactive
                 if self.animation:
                     self.ani.flush_events()
                 time.sleep(0.05)
@@ -3475,29 +3603,33 @@
             The iterated value.
 
         """
         # Do nothing if the simulation is paused
         if self.paused:
             return curr_val
 
+        # Determine which keys are pressed
+        is_down_key = self.is_pressed(down_key)
+        is_up_key = self.is_pressed(up_key)
+
         # Do nothing if both up and down keys are pressed
-        if self.is_pressed(down_key) and self.is_pressed(up_key):
+        if is_down_key and is_up_key:
             return curr_val
 
         # Set the new val to the current value
         new_val = curr_val
 
         # Listen to see if the down key is pressed
-        if self.is_pressed(up_key):
+        if is_up_key:
             new_val = curr_val + iter_val
             if new_val > max_val:
                 new_val = max_val
     
         # Listen to see if the up key is pressed
-        elif self.is_pressed(down_key):
+        elif is_down_key:
             new_val = curr_val - iter_val
             if new_val < min_val:
                 new_val = min_val
     
         # Return the updated target value
         return new_val
       
@@ -3537,14 +3669,21 @@
             p = urdf_obj.initial_conds['position']
             o = urdf_obj.initial_conds['orientation']
             v = urdf_obj.initial_conds['velocity']
             w = urdf_obj.initial_conds['angular velocity']
             self.engine.resetBasePositionAndOrientation(bodyUniqueId=i,
                                                         posObj=p,
                                                         ornObj=o)
+            
+            # Note that CoM and base state is no longer valid
+            urdf_obj.center_of_mass[0] = False
+            urdf_obj.base_state[0] = False
+            urdf_obj.base_state[2] = False
+            
+            # Reset the base velocities for all urdfs
             self.engine.resetBaseVelocity(objectUniqueId=i,
                                           linearVelocity=v,
                                           angularVelocity=w)
             
             # Reset each joint
             for joint_name in urdf_obj.joint_map.keys():
                 
@@ -3556,14 +3695,17 @@
                     pos = urdf_obj.initial_conds[joint_id]['position']
                     vel = urdf_obj.initial_conds[joint_id]['velocity']
                     self.engine.resetJointState(bodyUniqueId=urdf_obj.urdf_id,
                                                 jointIndex=joint_id,
                                                 targetValue=pos,
                                                 targetVelocity=vel)
                     
+                    # Note that CoM is no longer valid
+                    urdf_obj.center_of_mass[0] = False
+                    
                     # Set the joint torque to 0
                     self.set_joint_torque(urdf_obj,
                                           joint_name,
                                           torque=0.,
                                           show_arrow=False,
                                           color=False,)
         
@@ -3649,15 +3791,21 @@
         if self.start_epoch == -1.0:
             self.start_epoch = time.time()
         current_time = time.time() - self.start_epoch - self.pause_elapsed_time
 
         # Step the physics engine
         self.engine.stepSimulation()
         self.time = self.time + self.dt
-    
+        
+        # Invalidate all center of masses and base states
+        for urdf_obj in self.urdf_objs:
+            urdf_obj.center_of_mass[0] = False
+            urdf_obj.base_state[0] = False
+            urdf_obj.base_state[2] = False
+            
         # Based on the visualizer frame rate, determine if it is time to 
         # frame update
         frame_cond_1 = current_time >= self.frame_time_target
         frame_cond_2 = self.prev_frame_time < self.frame_time_target
         frame_cond_3 = self.prev_frame_time >= self.frame_time_target
         self.vis_time_okay = (frame_cond_1 and frame_cond_2) or frame_cond_3
```

### Comparing `condynsate-0.6.4/src/condynsate/utils.py` & `condynsate-0.6.5/src/condynsate/utils.py`

 * *Files identical despite different names*

### Comparing `condynsate-0.6.4/src/condynsate/visualizer.py` & `condynsate-0.6.5/src/condynsate/visualizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,49 +248,50 @@
             The default is [1., 0., 0., 0.].
 
         Returns
         -------
         transform : array-like, size (4,4)
             The resultant 4x4 3D affine transformation matrix.
 
-        """
-        # Get the scaling matrix based on the scale vector
-        scale_matrix = np.array([[scale[0], 0.0,      0.0,      0.0],
-                                 [0.0,      scale[1], 0.0,      0.0],
-                                 [0.0,      0.0,      scale[2], 0.0],
-                                 [0.0,      0.0,      0.0,      1.0]])
-        
-        # Get the translation matrix based on the translation vector
-        translate_matrix = np.array([[1.0, 0.0, 0.0, translate[0]],
-                                     [0.0, 1.0, 0.0, translate[1]],
-                                     [0.0, 0.0, 1.0, translate[2]],
-                                     [0.0, 0.0, 0.0, 1.0]])
-        
-        # Get the rotation matrix based on the wxyz quaternion
+        """      
+        # Extract rotation data
         w = wxyz_quaternion[0]
         x = wxyz_quaternion[1]
         y = wxyz_quaternion[2]
         z = wxyz_quaternion[3]
+        
+        # Perform calculations used to transform quaternion to rotation matrix
         xx = 2.*x*x
         xy = 2.*x*y
         xz = 2.*x*z
         yy = 2.*y*y
         yz = 2.*y*z
         zz = 2.*z*z
         wx = 2.*w*x
         wy = 2.*w*y
         wz = 2.*w*z
-        rotation_matrix = np.array([[1.-yy-zz, xy-wz, xz+wy, 0.],
-                                    [xy+wz, 1.-xx-zz, yz-wx, 0.],
-                                    [xz-wy, yz+wx, 1.-xx-yy, 0.],
-                                    [0., 0., 0., 1.]])
         
-        # Calculate and return the total transformation matrix
-        transform =  translate_matrix @ rotation_matrix @ scale_matrix
-        return transform
+        # Extract scale data
+        s1 = scale[0]
+        s2 = scale[1]
+        s3 = scale[2]
+        
+        # Extract translate data
+        t1 = translate[0]
+        t2 = translate[1]
+        t3 = translate[2]
+        
+        # Directly build the transform matrix
+        H = np.array([[s1*(1.-yy-zz), s2*(xy-wz),    s3*(xz+wy),    t1],
+                      [s1*(xy+wz),    s2*(1.-xx-zz), s3*(yz-wx),    t2],
+                      [s1*(xz-wy),    s2*(yz+wx),    s3*(1.-xx-yy), t3],
+                      [0.,            0.,            0.,            1.]])
+        
+        # Return the translation matrix
+        return H
 
 
     def apply_transform(self,
                         urdf_name,
                         link_name,
                         scale=[1., 1., 1.],
                         translate=[0., 0., 0.],
```

### Comparing `condynsate-0.6.4/src/condynsate.egg-info/PKG-INFO` & `condynsate-0.6.5/src/condynsate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: condynsate
-Version: 0.6.4
+Version: 0.6.5
 Summary: Simulates and visualizes articulated systems in real time
 Author-email: Grayson Schaer <gschaer2@illinois.edu>
 License: MIT License
         
         Copyright (c) 2023 Grayson Schaer
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `condynsate-0.6.4/src/condynsate.egg-info/SOURCES.txt` & `condynsate-0.6.5/src/condynsate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

