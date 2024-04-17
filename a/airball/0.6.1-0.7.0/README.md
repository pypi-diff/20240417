# Comparing `tmp/airball-0.6.1.tar.gz` & `tmp/airball-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airball-0.6.1.tar", last modified: Fri Dec 15 06:38:41 2023, max compression
+gzip compressed data, was "airball-0.7.0.tar", last modified: Wed Apr 17 19:46:05 2024, max compression
```

## Comparing `airball-0.6.1.tar` & `airball-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 06:38:41.043823 airball-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-12-15 06:38:33.000000 airball-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2023-12-15 06:38:41.043823 airball-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2023-12-15 06:38:33.000000 airball-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-12-15 06:38:33.000000 airball-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-15 06:38:41.043823 airball-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      930 2023-12-15 06:38:33.000000 airball-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 06:38:41.039823 airball-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 06:38:41.043823 airball-0.6.1/src/airball/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2023-12-15 06:38:33.000000 airball-0.6.1/src/airball/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25138 2023-12-15 06:38:33.000000 airball-0.6.1/src/airball/analytic.py
--rw-r--r--   0 runner    (1001) docker     (127)    42997 2023-12-15 06:38:33.000000 airball-0.6.1/src/airball/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    29110 2023-12-15 06:38:33.000000 airball-0.6.1/src/airball/environments.py
--rw-r--r--   0 runner    (1001) docker     (127)    16252 2023-12-15 06:38:33.000000 airball-0.6.1/src/airball/imf.py
--rw-r--r--   0 runner    (1001) docker     (127)    41692 2023-12-15 06:38:33.000000 airball-0.6.1/src/airball/stars.py
--rw-r--r--   0 runner    (1001) docker     (127)    26076 2023-12-15 06:38:33.000000 airball-0.6.1/src/airball/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2023-12-15 06:38:33.000000 airball-0.6.1/src/airball/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 06:38:41.043823 airball-0.6.1/src/airball.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2023-12-15 06:38:41.000000 airball-0.6.1/src/airball.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2023-12-15 06:38:41.000000 airball-0.6.1/src/airball.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 06:38:41.000000 airball-0.6.1/src/airball.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-15 06:38:41.000000 airball-0.6.1/src/airball.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-15 06:38:41.000000 airball-0.6.1/src/airball.egg-info/top_level.txt
+drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2024-04-17 19:46:05.216738 airball-0.7.0/
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    35149 2022-05-02 19:30:08.000000 airball-0.7.0/LICENSE
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     3261 2024-04-17 19:46:05.216559 airball-0.7.0/PKG-INFO
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     2592 2023-10-11 05:11:21.000000 airball-0.7.0/README.md
+-rw-r--r--   0 zyrxvo     (501) staff       (20)       85 2023-12-11 15:38:51.000000 airball-0.7.0/pyproject.toml
+-rw-r--r--   0 zyrxvo     (501) staff       (20)       38 2024-04-17 19:46:05.216774 airball-0.7.0/setup.cfg
+-rw-r--r--   0 zyrxvo     (501) staff       (20)      930 2024-04-17 19:44:38.000000 airball-0.7.0/setup.py
+drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2024-04-17 19:46:05.213464 airball-0.7.0/src/
+drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2024-04-17 19:46:05.215619 airball-0.7.0/src/airball/
+-rw-r--r--   0 zyrxvo     (501) staff       (20)      639 2024-04-17 19:44:56.000000 airball-0.7.0/src/airball/__init__.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    31576 2024-04-11 20:48:41.000000 airball-0.7.0/src/airball/analytic.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    43194 2024-04-17 18:42:00.000000 airball-0.7.0/src/airball/core.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    29017 2024-03-07 15:29:46.000000 airball-0.7.0/src/airball/environments.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    16366 2024-04-12 21:11:30.000000 airball-0.7.0/src/airball/imf.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    42685 2024-02-02 19:59:31.000000 airball-0.7.0/src/airball/stars.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)    32730 2024-04-17 18:41:31.000000 airball-0.7.0/src/airball/tools.py
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     7407 2023-12-17 07:19:28.000000 airball-0.7.0/src/airball/units.py
+drwxr-xr-x   0 zyrxvo     (501) staff       (20)        0 2024-04-17 19:46:05.216366 airball-0.7.0/src/airball.egg-info/
+-rw-r--r--   0 zyrxvo     (501) staff       (20)     3261 2024-04-17 19:46:05.000000 airball-0.7.0/src/airball.egg-info/PKG-INFO
+-rw-r--r--   0 zyrxvo     (501) staff       (20)      393 2024-04-17 19:46:05.000000 airball-0.7.0/src/airball.egg-info/SOURCES.txt
+-rw-r--r--   0 zyrxvo     (501) staff       (20)        1 2024-04-17 19:46:05.000000 airball-0.7.0/src/airball.egg-info/dependency_links.txt
+-rw-r--r--   0 zyrxvo     (501) staff       (20)       42 2024-04-17 19:46:05.000000 airball-0.7.0/src/airball.egg-info/requires.txt
+-rw-r--r--   0 zyrxvo     (501) staff       (20)        8 2024-04-17 19:46:05.000000 airball-0.7.0/src/airball.egg-info/top_level.txt
```

### Comparing `airball-0.6.1/LICENSE` & `airball-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `airball-0.6.1/PKG-INFO` & `airball-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airball
-Version: 0.6.1
+Version: 0.7.0
 Summary: A package for running and managing flybys using REBOUND
 Home-page: https://github.com/zyrxvo/airball/
 Author: Garett Brown
 Author-email: garett.brown@mail.utoronto.ca
 Project-URL: Bug Tracker, https://github.com/zyrxvo/airball/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `airball-0.6.1/README.md` & `airball-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `airball-0.6.1/setup.py` & `airball-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="airball",
-    version="0.6.1",
+    version="0.7.0",
     author="Garett Brown",
     author_email="garett.brown@mail.utoronto.ca",
     description="A package for running and managing flybys using REBOUND",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zyrxvo/airball/",
     project_urls={
```

### Comparing `airball-0.6.1/src/airball/__init__.py` & `airball-0.7.0/src/airball/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 from .core import (add_star_to_sim, flyby, flybys, hybrid_flyby, hybrid_flybys, successive_flybys, concurrent_flybys)
 from .environments import (StellarEnvironment, LocalNeighborhood, OpenCluster, GlobularCluster, GalacticBulge, GalacticCore)
 from .analytic import (relative_energy_change, energy_change_adiabatic_estimate, eccentricity_change_adiabatic_estimate, inclination_change_adiabatic_estimate)
 from .imf import (IMF)
 from .stars import (Star, Stars)
 from .units import (UnitSet)
 
-__version__ = 'v0.6.1'
+__version__ = 'v0.7.0'
```

### Comparing `airball-0.6.1/src/airball/analytic.py` & `airball-0.7.0/src/airball/analytic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as _np
 import joblib as _joblib
+import warnings as _warnings
 from scipy.special import j0 as _j0,jv as _jv
 
 from . import tools as _tools
 from . import units as _u
 from .core import add_star_to_sim, _rotate_into_plane
 
 ############################################################
@@ -29,17 +30,20 @@
         sim.add(m=1.)
         sim.add(m=5e-5, a=30., e=0.1, inc=0.1)
         energy = airball.analytic.binary_energy(sim)
         ```
     """
     index = int(particle_index)
     unit_set = _tools.rebound_units(sim)
-    G = (sim.G * unit_set['length']**3 / unit_set['mass'] / unit_set['time']**2)
+    G = (sim.G * unit_set.length**3 / unit_set.mass / unit_set.time**2)
     p = sim.particles
-    return (-G * p[0].m * unit_set['mass'] * p[index].m * unit_set['mass'] / (2. * p[index].a * unit_set['length'])).decompose(list(unit_set.values()))
+    if p[index].m == 0:
+        message = "Planet has zero mass therefore the binary energy is zero. This may cause divide by zero error when calculating the relative change in energy."
+        _warnings.warn(message, RuntimeWarning)
+    return (-G * p[0].m * unit_set.mass * p[index].m * unit_set.mass / (2. * p[index].a * unit_set['length'])).decompose(list(unit_set.values()))
     
 def energy_change_adiabatic_estimate(sim, star, averaged=False, particle_index=1):
     """
     An analytical estimate for the change in energy of a binary system due to a stellar flyby.
 
     This function is based on the conclusions of [Roy & Haddow (2003)](https://ui.adsabs.harvard.edu/abs/2003CeMDA..87..411R/abstract) and [Heggie (2006)](https://ui.adsabs.harvard.edu/abs/2006fbp..book...20H/abstract). The orbital element angles of the flyby star are determined with respect to the plane defined by the binary orbit.
 
@@ -60,32 +64,32 @@
         sim.add(m=1.)
         sim.add(m=5e-5, a=30., e=0.1, inc=0.1)
         star = airball.Star(m=1., b=500, v=5)
         energy_change = airball.energy_change_adiabatic_estimate(sim, star)
         ```
     """
     index = int(particle_index)
-    unit_set = _tools.rebound_units(sim)
-    t0 = 0*unit_set['time']
-    G = (sim.G * unit_set['length']**3 / unit_set['mass'] / unit_set['time']**2)
+    units = _tools.rebound_units(sim)
+    t0 = 0*units.time
+    G = (sim.G * units.length**3 / units.mass / units.time**2)
 
     sim = sim.copy()
     _rotate_into_plane(sim, plane=index)
     # add_star_to_sim(sim, star, hash='flybystar', rmax=0) # Initialize Star at perihelion
     sim.move_to_hel()
     
     p = sim.particles
-    m1, m2, m3 = p[0].m * unit_set['mass'], p[index].m * unit_set['mass'], star.mass # redefine the masses for convenience
+    m1, m2, m3 = p[0].m * units.mass, p[index].m * units.mass, star.mass # redefine the masses for convenience
     M12 = m1 + m2 # total mass of the binary system
     M123 = m1 + m2 + m3 # total mass of all the objects involved
     
-    mu = G * (_tools.system_mass(sim)  * unit_set['mass'] + m3)
-    es = _tools.vinf_and_b_to_e(mu=mu, star_b=star.b, star_v=star.v)
+    mu = G * (_tools.system_mass(sim)  * units.mass + m3)
+    es = _tools.calculate_eccentricity(sim, star)
     
-    a, e = p[index].a * unit_set['length'], p[index].e # redefine the orbital elements of the planet for convenience
+    a, e = p[index].a * units.length, p[index].e # redefine the orbital elements of the planet for convenience
     # Case: Non-circular Binary
 
     n = _np.sqrt(G*M12/a**3) # compute the mean motion of the planet
     
     w, W, i = star.omega, star.Omega, star.inc # redefine the orientation elements of the flyby star for convenience
     V = star.v
     # GM123 = G*M123 
@@ -108,29 +112,29 @@
     prefactor = (-_np.sqrt(_np.pi)/8.0) * ((G*m1*m2*m3)/M12) * ((a*a)/(q*q*q)) * f1 * k**(2.5) * _np.exp((-2.0*k/3.0)*f2)
     with _u.set_enabled_equivalencies(_u.dimensionless_angles()):
         term1 = e1 * ( _np.sin(2.0*w + n*t0)*_np.cos(2.0*i - 1.0)- _np.sin(2.0*w + n*t0)*_np.cos(2.0*i)*_np.cos(2.0*W) - 3.0*_np.sin(n*t0 + 2.0*w)*_np.cos(2.0*W) - 4.0*_np.sin(2.0*W)*_np.cos(2.0*w + n*t0)*_np.cos(i) )
         term2 = e2 * (1.0 - e*e) * ( _np.sin(2.0*w + n*t0)*(1.0-_np.cos(2.0*i)) - _np.sin(2.0*w + n*t0)*_np.cos(2.0*i)*_np.cos(2.0*W) - 3.0*_np.sin(n*t0 +2.0*w)*_np.cos(2.0*W) - 4.0*_np.cos(n*t0 + 2.0*w)*_np.sin(2.0*W)*_np.cos(i) )
         term3 = e4 * _np.sqrt(1.0 - e*e) * (-2.0*_np.cos(2.0*i)*_np.cos(2.0*w + n*t0)*_np.sin(2.0*W) - 6.0*_np.cos(2.0*w + n*t0)*_np.sin(2.0*W) - 8.0*_np.cos(2.0*W)*_np.sin(2.0*w + n*t0)*_np.cos(i) )
     
     noncircular_result = None
-    if averaged: noncircular_result = (prefactor * (e1 + e2 * (1 - e*e) + 2 * e4 * _np.sqrt(1 - e*e))).decompose(list(unit_set.values()))
-    else: noncircular_result = (prefactor * ( term1 + term2 + term3)).decompose(list(unit_set.values()))
+    if averaged: noncircular_result = (prefactor * (e1 + e2 * (1 - e*e) + 2 * e4 * _np.sqrt(1 - e*e))).decompose(list(units.values()))
+    else: noncircular_result = (prefactor * ( term1 + term2 + term3)).decompose(list(units.values()))
 
     # Case: Circular Binary
 
     # Compute the prefactor and terms of the calculation done by Roy & Haddow (2003)
     prefactor = (-_np.sqrt(_np.pi)/8.0) * ((G*m1*m2*m3)/M12) * ((a*a*a)/(q*q*q*q)) * f1 * k**(3.5) * _np.exp((-2.0*k/3.0)*f2) * (m2/M12 - m1/M12)
     with _u.set_enabled_equivalencies(_u.dimensionless_angles()):
         term1 = (1.0 + _np.cos(i)) * _np.sin(i)**2.0
         term2 = ( (_np.cos(w)**3.0) - 3.0 * (_np.sin(w)**2.0) * _np.cos(w) ) * _np.sin(n*t0)
         term3 = ( 3.0 * (_np.cos(w)**2.0) * _np.sin(w) - (_np.sin(w)**3.0)) * _np.cos(n*t0)
     
     circular_result = None
-    if averaged: circular_result = (prefactor / _np.pi).decompose(list(unit_set.values()))
-    else: circular_result = (prefactor * term1 * (term2 + term3)).decompose(list(unit_set.values()))
+    if averaged: circular_result = (prefactor / _np.pi).decompose(list(units.values()))
+    else: circular_result = (prefactor * term1 * (term2 + term3)).decompose(list(units.values()))
 
     return circular_result + noncircular_result
 
 def energy_change_close_encounter_estimate(sim, star, particle_index=1):
     '''
     An analytical estimate for the change in energy of a binary system due to a flyby star. From Equation (4.7) of [Heggie (1975)](https://ui.adsabs.harvard.edu/abs/1975MNRAS.173..729H/abstract). The orbital element angles of the flyby star are determined with respect to the plane defined by the binary orbit.
 
@@ -150,41 +154,73 @@
         sim.add(m=1.)
         sim.add(m=5e-5, a=30., e=0.1, inc=0.1)
         star = Star(m=1., b=100, v=5)
         energy_change = airball.analytic.energy_change_close_encounter_estimate(sim, star)
         ```
     '''
     index = int(particle_index)
-    s = sim.copy()
-    _rotate_into_plane(s, plane=index)
-    add_star_to_sim(s, star, hash='flybystar', rmax=0) # Initialize Star at perihelion
-    s.move_to_hel()
-    p = s.particles
-
     units = _tools.rebound_units(sim)
-    G = (s.G * units.length**3 / units.mass / units.time**2) # Newton's Gravitational constant
+    
+    def process_star(this_sim, this_star, this_index):
+        s = this_sim.copy()
+        add_star_to_sim(s, this_star, hash='flybystar', rmax=0, plane=this_index) # Initialize Star at perihelion
+        return _tools.unit_vector(s.particles['flybystar'].xyz << units.length)
+    
+    if star.N == 1:
+        x,y,z = process_star(sim, star, index)
+    else:
+        x,y,z = _np.asarray(_joblib.Parallel(n_jobs=-1)(_joblib.delayed(process_star)(sim, this_star, index) for this_star in star)).T
+    c = _tools.cartesian_elements(sim, star, rmax=0)
+    dat = _np.array([c['x'].value, c['y'].value, c['z'].value]).T << units.length
+    G = (sim.G * units.length**3 / units.mass / units.time**2) # Newton's Gravitational constant
 
-    m1, m2 = p[0].m * units.mass, p[index].m * units.mass # redefine the masses for convenience
+    m1, m2 = sim.particles[0].m * units.mass, sim.particles[index].m * units.mass # redefine the masses for convenience
     m3 = star.m
     M12 = m1 + m2 # total mass of the binary system
     M23 = m2 + m3 # total mass of the second and third bodies
 
     V = star.v # velocity of the star
 
-    x,y,z = _tools.unit_vector(p['flybystar'].xyz << units.length)
-    vx,vy,vz = p[index].vxyz << (units.length/units.time)
+    
+    vx,vy,vz = sim.particles[index].vxyz << (units.length/units.time)
 
     with _u.set_enabled_equivalencies(_u.dimensionless_angles()):
         cosϕ = 1.0/_np.sqrt(1.0 + (((star.b**2.0)*(V**4.0))/((G*M23)**2.0)).decompose())
     
     prefactor = (-2.0 * m1 * m2 * m3)/(M12 * M23) * V * cosϕ
     t1 = -(x*vx + y*vy + z*vz)
     t2 = (m3 * V * cosϕ)/M23
     return (prefactor * (t1 + t2)).decompose(units.values())
 
+def relative_energy_change_close_encounter_estimate(sim, star, particle_index=1):
+    '''
+     A convenience function for computing the analytical estimate for the relative change in energy of a binary system due to a close encounter with a flyby star. Combines [`energy_change_close_encounter_estimate`][airball.analytic.energy_change_close_encounter_estimate] and [`binary_energy`][airball.analytic.binary_energy] functions.
+
+    Args:
+        sim (Simulation): The simulation with two bodies, a central star and a planet.
+        star (Star or Stars): The star or stars used to estimate the change in energy of a binary due to the flyby star
+        particle_index (int, optional): The index of the particle in the simulation to calculate the energy for. Default is 1.
+
+    Returns:
+        energy_change (Quantity): The relative change in energy of the binary system.
+
+    Example:
+        ```python
+        import rebound
+        import airball
+        sim = rebound.Simulation()
+        sim.add(m=1.)
+        sim.add(m=5e-5, a=30., e=0.1, inc=0.1)
+        star = airball.Star(m=1., b=500, v=5)
+        energy_change = airball.analytic.relative_energy_change_close_encounter_estimate(sim, star)
+        ```
+
+    '''
+    return energy_change_close_encounter_estimate(sim, star, particle_index=particle_index)/binary_energy(sim, particle_index=particle_index)
+
 def relative_energy_change(sim, star, averaged=False, particle_index=1):
     '''
      A convenience function for computing the analytical estimate for the relative change in energy of a binary system due to a flyby star. Combines [`energy_change_adiabatic_estimate`][airball.analytic.energy_change_adiabatic_estimate] and [`binary_energy`][airball.analytic.binary_energy] functions.
 
     Args:
         sim (Simulation): The simulation with two bodies, a central star and a planet.
         star (Star or Stars): The star or stars used to estimate the change in energy of a binary due to the flyby star
@@ -202,15 +238,30 @@
         sim.add(m=1.)
         sim.add(m=5e-5, a=30., e=0.1, inc=0.1)
         star = airball.Star(m=1., b=500, v=5)
         energy_change = airball.analytic.relative_energy_change(sim, star)
         ```
 
     '''
-    return energy_change_adiabatic_estimate(sim=sim, star=star, averaged=averaged, particle_index=particle_index)/binary_energy(sim, particle_index=particle_index)
+    unit_set = _tools.rebound_units(sim)
+    qs = star.q(sim)/(sim.particles[particle_index].a * unit_set.length)
+    q_crit = 2**(2/3)
+    if star.N == 1:
+        if qs < q_crit: return energy_change_close_encounter_estimate(sim, star, particle_index=particle_index)/binary_energy(sim, particle_index=particle_index)
+        else: return energy_change_adiabatic_estimate(sim, star, averaged=averaged, particle_index=particle_index)/binary_energy(sim, particle_index=particle_index)
+    else:
+        de_close = energy_change_close_encounter_estimate(sim, star, particle_index=particle_index)/binary_energy(sim, particle_index=particle_index)
+        de = energy_change_adiabatic_estimate(sim, star, averaged=averaged, particle_index=particle_index)/binary_energy(sim, particle_index=particle_index)
+        close_inds = qs < q_crit
+        far_inds = ~close_inds
+        results = _np.zeros(star.N)
+        results[close_inds] = de_close[close_inds]
+        results[far_inds] = de[far_inds]
+        return results
+    # return energy_change_adiabatic_estimate(sim=sim, star=star, averaged=averaged, particle_index=particle_index)/binary_energy(sim, particle_index=particle_index)
 
 def parallel_relative_energy_change(sims, stars, averaged=False, particle_index=1):
     '''
         A convenience function for computing the analytical estimate for the relative change in energy of a binary system due to a flyby star. Combines [`energy_change_adiabatic_estimate`][airball.analytic.energy_change_adiabatic_estimate] and [`binary_energy`][airball.analytic.binary_energy] functions parallelized over the input parameters.
 
         Args:
             sims (list of Simulations): The simulation with two bodies, a central star and a planet.
@@ -231,21 +282,56 @@
                 sim.add(m=5e-5, a=30., e=0.1, f='uniform')
                 return sim
             stars = airball.Star(m=1., b=500, v=5, size=10)
             sims = [setup() for _ in range(stars.N)]
             energy_change = airball.analytic.parallel_relative_energy_change(sims, stars)
             ```
     '''
-    return _joblib.Parallel(n_jobs=-1)(_joblib.delayed(relative_energy_change)(sim=sims[i], star=stars[i], averaged=averaged, particle_index=particle_index) for i in range(stars.N))
+    unit_set = _tools.rebound_units(sims[0])
+    qs = stars.q(sims[0])
+    de = _np.array(_joblib.Parallel(n_jobs=-1)(_joblib.delayed(relative_energy_change)(sim=sims[i], star=stars[i], averaged=averaged, particle_index=particle_index) for i in range(stars.N)))
+    de_close = _np.array(_joblib.Parallel(n_jobs=-1)(_joblib.delayed(relative_energy_change_close_encounter_estimate)(sim=sims[i], star=stars[i], particle_index=particle_index) for i in range(stars.N)))
+    close_inds = qs/(sims[0].particles[particle_index].a * unit_set.length) < 2**(2/3)
+    far_inds = ~close_inds
+    results = _np.zeros(stars.N)
+    results[close_inds] = de_close[close_inds]
+    results[far_inds] = de[far_inds]
+    return results
 
 
 ############################################################
 ################ Eccentricity Estimates ####################
 ############################################################
 
+
+def eccentricity_change_close_encounter_estimate(sim, star, particle_index=1):
+    '''
+    An analytical estimate for the change in eccentricity of a binary system due to a flyby star. From Equation A1 of [Spurzem et al. (2009)](https://ui.adsabs.harvard.edu/abs/2009MNRAS.393..457S/abstract). The orbital element angles of the flyby star are determined with respect to the plane defined by the binary orbit.
+    '''
+
+    index = int(particle_index)
+    unit_set = _tools.rebound_units(sim)
+
+    p = sim.particles
+    m1, m2, m3 = p[0].m * unit_set.mass, p[index].m * unit_set.mass, star.mass # redefine the masses for convenience
+    M12 = m1 + m2 # total mass of the binary system
+    M123 = m1 + m2 + m3 # total mass of all the objects involved
+
+    q = star.q(sim) # compute the periapsis of the flyby star
+    AB = _tools.hyperbolic_plane(sim, star)
+    A,B = AB['A'], AB['B']
+    ahat, bhat = [1,0,0], [0,1,0]
+
+    # mu = G * (_tools.system_mass(sim)  * unit_set.mass + m3)
+    # es = _tools.vinf_and_b_to_e(mu=mu, star_b=star.b, star_v=star.v)
+
+    a, e = p[index].a * unit_set.length, p[index].e # redefine the orbital elements of the planet for convenience
+
+    return ( ((-15.0*_np.pi*m3) / _np.sqrt(32.0 * M12*M123)) * ((a/q)**1.5) * (e * _np.sqrt(1.0 - e*e)) * ( (ahat @ A) * (bhat @ A) + (ahat @ B) * (bhat @ B) ) ).decompose(list(unit_set.values()))
+
 def eccentricity_change_adiabatic_estimate(sim, star, averaged=False, particle_index=1, rmax=1e5*_u.au):
     '''
         An analytical estimate for the change in eccentricity of a binary system due to a flyby star. From Equations (7, 9, & 12) of Heggie & Rasio [(1996)](https://ui.adsabs.harvard.edu/abs/1996MNRAS.282.1064H/abstract). The orbital element angles of the flyby star are determined with respect to the plane defined by the binary orbit.
 
         Args:
             sim (Simulation): The simulation with two bodies, a central star and a planet.
             star (Star): The star used to estimate the change in energy of a binary due to the flyby star
@@ -267,33 +353,34 @@
             eccentricity_change = airball.analytic.eccentricity_change_adiabatic_estimate(sim, star)
             ```
     '''
 
     index = int(particle_index)
 
     unit_set = _tools.rebound_units(sim)
-    t0 = sim.t * unit_set['time']
-    G = (sim.G * unit_set['length']**3 / unit_set['mass'] / unit_set['time']**2)
+
+    t0 = sim.t * unit_set.time
+    G = (sim.G * unit_set.length**3 / unit_set.mass / unit_set.time**2)
     
     p = sim.particles
-    m1, m2, m3 = p[0].m * unit_set['mass'], p[index].m * unit_set['mass'], star.mass # redefine the masses for convenience
+    m1, m2, m3 = p[0].m * unit_set.mass, p[index].m * unit_set.mass, star.mass # redefine the masses for convenience
     M12 = m1 + m2 # total mass of the binary system
     M123 = m1 + m2 + m3 # total mass of all the objects involved
     
-    mu = G * (_tools.system_mass(sim)  * unit_set['mass'] + m3)
+    mu = G * (_tools.system_mass(sim)  * unit_set.mass + m3)
     es = _tools.vinf_and_b_to_e(mu=mu, star_b=star.b, star_v=star.v)
     
-    a, e = p[index].a * unit_set['length'], p[index].e # redefine the orbital elements of the planet for convenience
+    a, e = p[index].a * unit_set.length, p[index].e # redefine the orbital elements of the planet for convenience
     # n = _np.sqrt(G*M12/a**3) # compute the mean motion of the planet
     
     w, W, i = star.omega, star.Omega, star.inc # redefine the orientation elements of the flyby star for convenience
 
     star_params = _tools.hyperbolic_elements(sim, star, rmax)
     tperi = star_params['T']
-    Mperi = p[index].M + (p[index].n/unit_set['time']) * (tperi - t0) # get the Mean anomaly when the flyby star is at perihelion
+    Mperi = p[index].M + (p[index].n/unit_set.time) * (tperi - t0) # get the Mean anomaly when the flyby star is at perihelion
     f = _tools.M_to_f(p[index].e, Mperi.value) << _u.rad # get the true anomaly when the flyby star is at perihelion
     Wp = W + f
     V = star.v
     q = (- mu + _np.sqrt( mu**2. + star.b**2. * V**4.))/V**2. # compute the periapsis of the flyby star
 
     # Case: Non-Circular Binary
 
@@ -331,14 +418,15 @@
         i2 = i/2.0
         exponential = -_np.sqrt(M12/M123) * ((q/a)**1.5) * ((_np.sqrt(es*es - 1.0) - _np.arccos(1.0/es)) / ((es - 1.0)**1.5))
         angles = (_np.cos(i2)**2.0) * _np.sqrt((_np.cos(i2)**4.0) + ((4.0/9.0)*_np.sin(i2)**4.0) + ((4.0/3.0)*(_np.cos(i2)**2.0)*(_np.sin(i2)**2.0)*_np.cos(4.0*w + 2.0*Wp)))
 
     if averaged: exponential_result = prefactor * _np.exp(exponential)
     else: exponential_result = prefactor * _np.exp(exponential) * angles
 
+    # Add the ABS together, deliberately choose a norm.
     return (_np.nan_to_num(circular_result) + _np.nan_to_num(noncircular_result) + _np.nan_to_num(exponential_result)).decompose()
 
 def parallel_eccentricity_change_adiabatic_estimate(sims, stars, averaged=False, particle_index=1, rmax=1e5*_u.au):
     """
     An analytical estimate for the changes in eccentricity of binary systems due to a flyby stars.
 
     Args:
@@ -366,14 +454,19 @@
         ```
     """
     return _joblib.Parallel(n_jobs=-1)(_joblib.delayed(eccentricity_change_adiabatic_estimate)(sim=sims[i], star=stars[i], averaged=averaged, particle_index=particle_index, rmax=rmax) for i in range(stars.N))
 
 def eccentricity_change_impulsive_estimate(sim, star, particle_index=1):
     '''
     An analytical estimate for the change in eccentricity of an eccentric binary system due to a flyby star. From Equation (28) of [Heggie & Rasio (1996)](https://ui.adsabs.harvard.edu/abs/1996MNRAS.282.1064H/abstract). The orbital element angles of the flyby star are determined with respect to the plane defined by the binary orbit.
+    
+    The base assumptions are that the flyby is coplanar, $q_\star \gg a$, and $v_\star \gg v_\mathrm{planet}$. It may work outside of this regime, but it is not guaranteed.
+    
+    TODO:
+        Make sure that the time of perihelion is calculated correctly and that the phase of the planet is correct.
 
     Args:
         sim (Simulation): The simulation with two bodies, a central star and a planet.
         star (Star): The star used to estimate the change in energy of a binary due to the flyby star
         particle_index (int, optional): The index of the particle in the simulation to calculate the energy for. Default is 1.
 
     Returns:
@@ -388,34 +481,58 @@
         sim.add(m=5e-5, a=30., e=0.1, inc=0.1)
         star = airball.Star(m=1., b=500, v=5)
         eccentricity_change = airball.analytic.eccentricity_change_impulsive_estimate(sim, star)
         ```
     '''
 
     index = int(particle_index)
-
-    unit_set = _tools.rebound_units(sim)
-    G = (sim.G * unit_set['length']**3 / unit_set['mass'] / unit_set['time']**2)
-    sim = sim.copy()
-    _rotate_into_plane(sim, plane=index)
-    add_star_to_sim(sim, star, hash='flybystar', rmax=0) # Initialize Star at perihelion
+    units = _tools.rebound_units(sim)
+    G = (sim.G * units.length**3 / units.mass / units.time**2)
 
     p = sim.particles
-    m1, m2, m3 = p[0].m * unit_set['mass'], p[index].m * unit_set['mass'], star.mass # redefine the masses for convenience
+    m1, m2, m3 = p[0].m * units.mass, p[index].m * units.mass, star.mass # redefine the masses for convenience
     M12 = m1 + m2 # total mass of the binary system
     
-    a = p[index].a * unit_set['length'] # redefine the orbital elements of the planet for convenience
+    a = p[index].a * units.length # redefine the orbital elements of the planet for convenience
     V = star.v
-    mu = G * (_tools.system_mass(sim)  * unit_set['mass'] + m3)
-    q = (- mu + _np.sqrt( mu**2. + star.b**2. * V**4.))/V**2. # compute the periapsis of the flyby star
-
-    theta = _tools.angle_between(p[index].xyz, p['flybystar'].xyz)
+    q = star.q(sim) # compute the periapsis of the flyby star
+    c = _tools.cartesian_elements(sim, star, rmax=0) # Get the heliocentric coordinates of the flyby star at periapsis
+    dat = _np.array([c['x'].value, c['y'].value, c['z'].value]).T << units.length
+    theta = _tools.angle_between(p[index].xyz, dat)
 
+    # print(f"{G=}, {M12=}, {m3=}, {V=}, {a=}, {q=}, {theta=}")
     return ((2.0 * _np.sqrt(G/M12) * (m3/V) * _np.sqrt(a*a*a) / (q*q)) * _np.abs(_np.cos(theta)) * _np.sqrt((_np.cos(theta)**2.0) + (4.0 * _np.sin(theta)**2.0))).decompose()
 
+def parallel_eccentricity_change_impulsive_estimate(sims, stars, particle_index=1):
+    """
+    An analytical estimate for the changes in eccentricity of binary systems due to a flyby stars.
+
+    Args:
+        sims (list of Simulations): the simulation with two bodies, a central star and a planet.
+        stars (Stars): the star or stars used to estimate the change in energy of a binary due to the flyby star
+        particle_index (int, optional): the index of the particle in the simulation to calculate the energy for. Default is 1.
+
+    Returns:
+        results (list of Quantities): The changes in eccentricity of the binary systems.
+
+    Example:
+        ```python
+        import rebound
+        import airball
+        def setup():
+            sim = rebound.Simulation()
+            sim.add(m=1.)
+            sim.add(m=5e-5, a=30., e=0.1, f='uniform')
+            return sim
+        stars = airball.Star(m=1., b=500, v=5, size=10)
+        sims = [setup() for _ in range(stars.N)]
+        eccentricity_changes = airball.analytic.parallel_eccentricity_change_impulsive_estimate(sims, stars)
+        ```
+    """
+    return _joblib.Parallel(n_jobs=-1)(_joblib.delayed(eccentricity_change_impulsive_estimate)(sim=sims[i], star=stars[i], particle_index=particle_index) for i in range(stars.N))
 
 ############################################################
 ################ Inclination Estimate ######################
 ############################################################
 
 def inclination_change_adiabatic_estimate(sim, star, averaged=False, particle_index=1):
     '''
@@ -450,15 +567,15 @@
     
     p = sim.particles
     m1, m2, m3 = p[0].m * unit_set['mass'], p[index].m * unit_set['mass'], star.mass # redefine the masses for convenience
     M12 = m1 + m2 # total mass of the binary system
     M123 = m1 + m2 + m3 # total mass of all the objects involved
     
     mu = G * (_tools.system_mass(sim)  * unit_set['mass'] + m3)
-    es = _tools.vinf_and_b_to_e(mu=mu, star_b=star.b, star_v=star.v)
+    es = _tools.calculate_eccentricity(sim, star)
     
     a, e = p[index].a * unit_set['length'], p[index].e # redefine the orbital elements of the planet for convenience
     
     w, W, i = star.omega, star.Omega, star.inc # redefine the orientation elements of the flyby star for convenience
 
     V = star.v
     q = (- mu + _np.sqrt( mu**2. + star.b**2. * V**4.))/V**2. # compute the periapsis of the flyby star
```

### Comparing `airball-0.6.1/src/airball/core.py` & `airball-0.7.0/src/airball/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     Simulate a stellar flyby to a REBOUND simulation.
 
     Because REBOUND Simulations are C structs underneath the Python, this function can pass the simulation by reference. Meaning, any changes made inside this function to the REBOUND simulation are permanent. This can be avoided by specifying `overwrite=False`. If any pointers have been assigned to the simulation, then the default `overwrite=True` is recommended.
 
     Args:
         sim (Simulation): The simulation (star and planets) that will experience the flyby star.
         star (Star): The star that will flyby the given REBOUND simulation.
-    
+
     Keyword Args:
         hybrid (bool, optional): Determines whether or not to use the hybrid method. Default is False. If True, then any kwargs for `hybrid_flyby` will be passed to that function.
         rmax (float, optional): The starting distance of the flyby star in units of AU. Default is $10^5$ AU.
         overwrite (bool, optional): Determines whether or not to return a copy of sim (`overwrite=False`) or integrate using the original sim (`overwrite=True`). Default is True. If any pointers have been assigned to the simulation, then `overwrite=True` is recommended.
         plane (str or int, optional): The plane defining the orientation of the star, None, 'invariable', 'ecliptic', or int. Default is None.
         hash (str, optional): The name for the flyby star. Default is `'flybystar'`.
 
@@ -44,15 +44,16 @@
     """
     if kwargs.get('hybrid', False): return hybrid_flyby(sim, star, **kwargs)
     else:
         if sim.integrator == 'whfast': _warnings.warn("Did you intend to use the hybrid method with WHFast? WHFast may not correctly resolve close encounters.", RuntimeWarning)
         overwrite = kwargs.get('overwrite', True)
         if not overwrite: sim = sim.copy()
         hash = kwargs.get('hash', 'flybystar')
-        add_star_to_sim(sim, star, hash, rmax=kwargs.get('rmax', 1e5*_u.au), plane=kwargs.get('plane'))
+        if 'hash' in kwargs: del kwargs['hash']
+        add_star_to_sim(sim, star, hash, **kwargs)
         tperi = sim.particles[hash].T - sim.t # Compute the time to periapsis for the flyby star from the current time.
         sim.integrate(sim.t + 2*tperi)
         remove_star_from_sim(sim, hash)
         return sim
 
 def flybys(sims, stars, **kwargs):
     '''
@@ -150,15 +151,15 @@
 
         Keyword Args:
             rmax (float, optional): The starting distance of the flyby star in units of the REBOUND Simulation. Default is $10^5$ AU.
             crossoverFactor (float, optional): The value for when to switch to IAS15 as a multiple of sim.particles[particle_index].a. Default is 30x, i.e. 30 times the semi-major axis of particle at particle_index.
             particle_index (int, optional): The particle index to consider for the crossoverFactor. Default is 1.
             overwrite (boolean, optional): Determines whether or not to return a copy of sim (`overwrite=False`) or integrate using the original sim (`overwrite=True`). Default is True. `overwrite=True` is recommended if any pointers have been assigned to the simulation.
             plane (str or int, optional): The plane defining the orientation of the star, None, 'invariable', 'ecliptic', or int. Default is None.
-        
+
         Returns:
             sim (Simulation): The simulation after the flyby. This is the same object as the input sim if overwrite=True.
 
         Example:
             ```python
             import rebound
             import airball
@@ -171,15 +172,16 @@
     '''
 
     overwrite = kwargs.get('overwrite', True)
     if not overwrite: sim = sim.copy()
     hash = kwargs.get('hash', 'flybystar')
     sim_units = _tools.rebound_units(sim)
 
-    star_vars = add_star_to_sim(sim, star, rmax=kwargs.get('rmax', 1e5*_u.au), plane=kwargs.get('plane'), hash=hash)
+    if 'hash' in kwargs: del kwargs['hash']
+    star_vars = add_star_to_sim(sim, star, hash, **kwargs)
 
     tperi = sim.particles[hash].T - sim.t # Compute the time to periapsis for the flyby star from the current time.
 
     # Integrate the flyby. Start at the current time and go to twice the time to periapsis.
     switch, tIAS15 = _time_to_periapsis_from_crossover_point(sim, sim_units, crossoverFactor=kwargs.get('crossoverFactor', 30), index=kwargs.get('particle_index', 1), star_elements=star_vars)
     if switch:
         t_switch = sim.t + tperi - tIAS15.value
@@ -323,15 +325,16 @@
     '''
 
     # Do not overwrite given sim.
     overwrite = kwargs.get('overwrite', True)
     if overwrite == False: sim = sim.copy()
     hashes = kwargs.get('hashes', [f'flybystar{i}' for i in range(stars.N)])
     saveSnapshots = kwargs.get('snapshots', False)
-    if saveSnapshots: snapshots = [sim.copy()]
+    snapshots = []
+    if saveSnapshots: snapshots.append(sim.copy())
     for i,star in enumerate(stars):
         if overwrite == True: flyby(sim, star, hash=hashes[i], **kwargs)
         else:  sim = flyby(sim, star, hash=hashes[i], **kwargs)
         if saveSnapshots: snapshots.append(sim.copy())
     if saveSnapshots: return snapshots
     else: return sim
 
@@ -351,15 +354,15 @@
             start_times (list): An array of times for the stars to be added to the sim.
 
         Keyword Args:
             overwrite (boolean, optional): Sets whether or not to return new simulation objects or overwrite the given ones. Default is True, meaning the same simulation objects will be returned. This keeps all original pointers attached to it.
             hashes (list of str, optional): A list of hash values for adding and removing stars from simulations. Default is ['flybystar0', 'flybystar1', ...].
             rmax (float, optional): The starting distance of the flyby object (in units of the REBOUND Simulation). Default is $10^5$.
             plane (str or int, optional): The plane defining the orientation of the star, None, 'invariable', 'ecliptic', or Int. Default is None.
-        
+
         Example:
             ```python
             import rebound
             import airball
             sim = rebound.Simulation()
             sim.add(m=1)
             sim.add(m=5e-5, a=30)
@@ -385,23 +388,23 @@
     # Using the sim and the start times, compute the end times for the flyby stars.
     all_times = _np.zeros((stars.N, 2))
     for star_number, star in enumerate(stars):
         tmp_sim = sim.copy()
         hash = hashes[star_number]
         add_star_to_sim(tmp_sim, star, hash=hash, rmax=rmax, plane=plane)
         # Compute the time to periapsis for the flyby star from the current simulation time.
-        tperi = tmp_sim.particles[hash].T - tmp_sim.t 
+        tperi = tmp_sim.particles[hash].T - tmp_sim.t
         end_time = start_times[star_number] + tmp_sim.t + 2*tperi
         all_times[star_number] = [start_times[star_number], end_time]
 
     # Sort the event times sequentially.
     all_times = all_times.flatten()
     event_order = _np.argsort(all_times)
     max_event_number = len(all_times)
-    
+
     # Integrate the flybys, adding and removing them at the appropriate times.
     event_number = 0
     while event_number < max_event_number:
         event_index = event_order[event_number]
         star_number = event_index//2
         sim.integrate(all_times[event_index])
         if event_index%2 == 0: add_star_to_sim(sim, stars[star_number], hash=hashes[star_number], rmax=rmax, plane=plane)
@@ -413,22 +416,23 @@
 ############################################################
 ################# Flyby Helper Functions ###################
 ############################################################
 
 def _rotate_into_plane(sim, plane):
     '''
     Rotates the simulation into the specified plane.
-    
+
     Args:
         sim (Simulation): The REBOUND Simulation containing the star and planets that will experience a flyby.
         plane (str, int): The plane defining the orientation of the star: None, 'invariable', 'ecliptic', or int.
-    
+
     Returns:
         rotation (Rotation): The rotation that was applied to the simulation.
     '''
+    _warnings.warn("This function is deprecated and will be removed in a future version. Use the `airball.tools.rotate_into_plane` function instead.", DeprecationWarning)
     int_types = (int, _np.integer)
     rotation = _rebound.Rotation.to_new_axes(newz=[0,0,1])
     if plane is not None:
         # Move the system into the chosen plane of reference. TODO: Make sure the angular momentum calculations don't include other flyby stars.
         if plane == 'invariable': rotation = _rebound.Rotation.to_new_axes(newz=sim.angular_momentum())
         elif plane == 'ecliptic': rotation = _rebound.Rotation.to_new_axes(newz=_tools.calculate_angular_momentum(sim)[3]) # Assumes Earth is particle 3. 0-Sun, 1-Mecury, 2-Venus, 3-Earth, ...
         elif isinstance(plane, int_types):
@@ -469,15 +473,16 @@
     units = _tools.rebound_units(sim)
     rmax = _tools.verify_unit(kwargs.get('rmax', 1e5*_u.au), units['length'])
     stellar_elements = _tools.hyperbolic_elements(sim, star, rmax, values_only=True)
 
     plane = kwargs.get('plane')
     if plane is not None: rotation = _rotate_into_plane(sim, plane)
 
-    sim.add(**stellar_elements, hash=hash, primary=sim.particles[0])
+    if kwargs.get('helio', False): sim.add(**stellar_elements, hash=hash, primary=sim.particles[0])
+    else: sim.add(**stellar_elements, hash=hash)
     # Because a new particle was added, we need to tell REBOUND to recalculate the coordinates if WHFast is being used.
     if sim.integrator == 'whfast': sim.ri_whfast.recalculate_coordinates_this_timestep = 1
     sim.integrator_synchronize() # For good measure.
 
     if plane is not None: sim.rotate(rotation.inverse())
     sim.move_to_com()
 
@@ -506,15 +511,15 @@
 
         Args:
             sim (Simulation): The REBOUND Simulation containing the star and planets that will experience a flyby.
             sim_units (dict): The units of the REBOUND Simulation.
             crossoverFactor (float): The value for when to switch to IAS15 as a multiple of sim.particles[index].a.
             index (int): The simulation particle index to define the crossoverFactor with respect to.
             star_elements (dict): The initial conditions of the star in the REBOUND simulation. `m`, `a`, `e`, `l` are the mass, semi-major axis, eccentricity, and semilatus rectum of the star, respectively.
-        
+
         Returns:
             switch (bool): Whether or not to switch to IAS15.
             tIAS15 (float): The time to periapsis from the crossover point. None if switch=False.
     '''
     rCrossOver = crossoverFactor * sim.particles[index].a * sim_units['length'] # This is the distance to switch integrators
     q = star_elements['a'] * (1 - star_elements['e'])
     if q < rCrossOver:
@@ -531,15 +536,15 @@
     else: return False, None
 
 # old signature flyby(sim, star=None, m=0.3, b=1000, v=40,  e=None, inc='uniform', omega='uniform', Omega='uniform', rmax=2.5e5, hybrid=True, crossoverFactor=30, overwrite=False):
 
 def _integrate_with_ias15(sim, tmax):
     '''
         Integrate a REBOUND simulation with IAS15.
-        
+
         Args:
             sim (Simulation): A REBOUND Simulation.
             tmax (float): The time to integrate to.
     '''
     sim.integrator = 'ias15'
     sim.gravity = 'basic'
     sim.integrate(tmax)
@@ -760,24 +765,24 @@
     if verbose:
         tmpdic = {0 : f'ADD', 1 : f'start IAS15', 2 : f'end IAS15', 3 : f'REMOVE'}
         print([f'{tmpdic[i%4]} {i//4}' for i in event_order[:max_event_number]])
 
     useIAS15 = _np.array([False] * stars.N)
     def startUsingIAS15(i, IAS15_array): IAS15_array[i//4] = True
     def stopUsingIAS15(i, IAS15_array): IAS15_array[i//4] = False
-    
+
     def function_map( i, v, sim, star, IAS15_array, plane, hash):
-        if not _np.isnan(v): 
+        if not _np.isnan(v):
             map_i = i%4
             if map_i == 0: add_star_to_sim(sim, star, plane=plane, hash=hash)
             elif map_i == 1: startUsingIAS15(i, IAS15_array)
             elif map_i == 2: stopUsingIAS15(i, IAS15_array)
             elif map_i == 3: remove_star_from_sim(sim, hash=hash)
             else: pass
-    
+
     output = None
     event_number = 0
     dt = sim.dt
     dt_frac = sim.dt/sim.particles[1].P
     with _tempfile.NamedTemporaryFile() as tmp:
         sim.simulationarchive_snapshot(tmp.name, deletefile=True)
         while event_number < max_event_number:
```

### Comparing `airball-0.6.1/src/airball/environments.py` & `airball-0.7.0/src/airball/environments.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,23 +28,23 @@
       mass_function (callable, optional): A function that defines the mass distribution of stars. Default is None.
       maximum_impact_parameter (float, optional): The maximum impact parameter defining the outer limit of the sphere of influence around a stellar system. If not provided, AIRBALL attempts to estimate a reasonable one. Default is None.
       name (str, optional): The name of the environment. Default is None.
       UNIT_SYSTEM (list, optional): The unit system used in the environment. Default is an empty list.
       units (airball.units.UnitSet, optional): The units used in the environment. Default is None.
       object_name (str, optional): The name of the object in the environment. Default is None.
       seed (int, optional): The seed fixing the random star generator. Default is None so it's always random.
-      
+
     Example:
       ```python
       import airball
       my_env = airball.StellarEnvironment(stellar_density=10, velocity_dispersion=20, lower_mass_limit=0.08, upper_mass_limit=8, name='My Environment')
       my_star = my_env.random_star()
-      ```  
+      ```
 
-    If a `maximum_impact_parameter` is not given, AIRBALL attempts to estimate a reasonable one. 
+    If a `maximum_impact_parameter` is not given, AIRBALL attempts to estimate a reasonable one.
     The Maximum Impact Parameter is radius defining the outer limit of the sphere of influence around a stellar system.
     There are predefined subclasses for the LocalNeighborhood, a generic OpenCluster, a generic GlobularCluster, and the Milky Way center GalacticBulge and GalacticCore.
   '''
   def __init__(self, stellar_density, velocity_dispersion, lower_mass_limit, upper_mass_limit, mass_function=None, maximum_impact_parameter=None, name=None, UNIT_SYSTEM=[], units=None, object_name=None, seed=None, number_imf_samples=100):
     # Check to see if an stars object unit is defined in the given UNIT_SYSTEM and if the user defined a different name for the objects.
     self.units = units if isinstance(units, _u.UnitSet) else _u.UnitSet(UNIT_SYSTEM)
     objectUnit = [this for this in UNIT_SYSTEM if this.is_equivalent(_u.stars)]
@@ -64,24 +64,24 @@
     self.name = name if name is not None else 'Stellar Environment'
     self.short_name = self.name.replace(' ', '')
     self.seed = seed if seed is not None else None #_np.random.randint(0, int(2**32 - 1))
 
   def random_stars(self, size=1, **kwargs):
     '''
       Computes a random star from a stellar environment.
-      
+
       Args:
         size (int or tuple): The number of stars to generate. If size is a tuple, it is interpreted as array dimensions. Default: 1.
-      
+
       Keyword Args:
         include_orientation (bool, optional): If True, the orientation of the star is randomly generated. Otherwise, the orientation of the stars are zero. Default: True.
         maximum_impact_parameter (float, optional): The maximum impact parameter of the star. If None, the maximum impact parameter is estimated. Default: None.
         seed (int, optional): The random seed to use. If None is given then it is random every time. Default: None.
 
-      Returns: 
+      Returns:
         stars (Star or Stars): A Star object or Stars object (if size > 1) with the randomly generated masses, impact parameters, velocities, and orientations in a heliocentric model.
 
       Example:
         ```python
         import airball
         my_env = airball.StellarEnvironment(stellar_density=10, velocity_dispersion=20, lower_mass_limit=0.08, upper_mass_limit=8, name='My Environment')
         my_stars = my_env.random_stars(10)
@@ -134,15 +134,15 @@
 
   def copy(self):
     '''
     Returns a deep copy of the current Stellar Environment.
     '''
     kwargs = {'stellar_density':self.density, 'velocity_dispersion':self.velocity_dispersion, 'lower_mass_limit':self.lower_mass_limit, 'upper_mass_limit':self.upper_mass_limit, 'mass_function':self.IMF.initial_mass_function, 'maximum_impact_parameter':self.maximum_impact_parameter, 'name':self.name, 'UNIT_SYSTEM':self.UNIT_SYSTEM, 'object_name':self.object_name, 'seed':self.seed, 'number_imf_samples':self.IMF.number_samples}
     return type(self)(**kwargs)
-  
+
   def __eq__(self, other):
     # Overrides the default implementation
     if isinstance(other, StellarEnvironment):
         return (self.density == other.density and self.velocity_dispersion == other.velocity_dispersion and self.lower_mass_limit == other.lower_mass_limit and self.upper_mass_limit == other.upper_mass_limit and self.IMF == other.IMF and self.maximum_impact_parameter == other.maximum_impact_parameter and self.name == self.name and self.units == other.units and self.object_name == other.object_name and self.seed == other.seed)
     else:
       return NotImplemented
 
@@ -152,45 +152,45 @@
     for d in sorted(self.__dict__.items()):
         try: data.append((d[0], tuple(d[1])))
         except: data.append(d)
     data = tuple(data)
     return hash(data)
 
   def summary(self, returned=False):
-    ''' 
+    '''
     Prints a compact summary of the current stats of the Stellar Environment object.
     '''
     s = f"<{self.__module__}.{type(self).__name__} object at {hex(id(self))}"
     s += f", n= {self.density:1.4g}"
     s += f", v= {self.velocity_dispersion:,.1f}"
     s += f", m= {self.lower_mass_limit.value:,.2f}-{self.upper_mass_limit.value:,.1f} {self.units['mass']}"
     s += ">"
     if returned: return s
     else: print(s)
-  
+
   def __str__(self):
     return self.summary(returned=True)
-  
+
   def __repr__(self):
     return self.summary(returned=True)
 
 
   @property
   def object_unit(self):
     '''The unit of the object (star) in the environment.'''
     return self.units['object']
-  
+
   @property
   def object_name(self):
     '''
     Args:
       value (str): The name of the object (star) in the environment.
     '''
     return self.units['object'].to_string()
-  
+
   @object_name.setter
   def object_name(self, value):
     self.units.object = _u.def_unit(value, _u.stars)
 
   @property
   def UNIT_SYSTEM(self):
       '''
@@ -322,16 +322,16 @@
 
         - n : stellar number density. Default units: $\\rm{pc}^{-3}$
         - σ : interaction cross section. Default units: $\\rm{AU}^2$
         - v : velocity dispersion. Default units: $\\rm{km/s}$
 
         The interaction cross section $σ = πb^2$ considers gravitational focussing where $b = q \\sqrt(1 + \\frac{2GM}{q v_∞^2})$ determined by the median mass of the environment, the maximum impact parameter, and the relative velocity at infinity derived from the velocity dispersion.
     '''
-    return _tools.encounter_rate(self._density, _tools.maxwell_boltzmann_mean_from_dispersion(self.velocity_dispersion), self._maximum_impact_parameter, self.median_mass, unit_set=self.units).to(self.units['object']/self.units['time'])
-  
+    return _tools.encounter_rate(self._density, self.velocity_mean, self._maximum_impact_parameter, self.median_mass, unit_set=self.units).to(self.units['object']/self.units['time'])
+
   def cumulative_encounter_times(self, size):
     '''
     Returns the cumulative time from t=0 for when to expect the next flyby encounters.
     This function assumes a Poisson Process and uses an Exponential distribution with the encounter rate.
 
     Args:
         size (int or tuple): The shape of the returned array. If size is an integer, it is treated as the length of the array. If size is a tuple, it is treated as the shape of the array.
@@ -342,25 +342,25 @@
     Example:
         ```python
         import airball
         my_env = airball.StellarEnvironment(stellar_density=10, velocity_dispersion=20, lower_mass_limit=0.08, upper_mass_limit=8, name='My Environment')
         my_env.cumulative_encounter_times(10) # returns an array of 10 cumulative encounter times.
         ```
     '''
-    if isinstance(size, tuple): 
+    if isinstance(size, tuple):
       size = tuple([int(i) for i in size])
       result = _np.cumsum(_exponential.rvs(scale=1/self.encounter_rate, size=size), axis=1) << self.units['time']
       result -= result[:, 0][:, None]
       return result
     else:
       size = int(size)
       result = _np.cumsum(_exponential.rvs(scale=1/self.encounter_rate, size=size)) << self.units['time']
       result -= result[0]
       return result
-  
+
   def encounter_times(self, size):
     '''
     Returns the time between encounters for when to the expect the next flyby encounters.
     Assumes a Poisson Process and uses an Exponential distribution with the encounter rate.
 
     Args:
         size (int or tuple): The shape of the returned array. If size is an integer, it is treated as the length of the array. If size is a tuple, it is treated as the shape of the array.
@@ -371,15 +371,15 @@
     Example:
         ```python
         import airball
         my_env = airball.StellarEnvironment(stellar_density=10, velocity_dispersion=20, lower_mass_limit=0.08, upper_mass_limit=8, name='My Environment')
         my_env.encounter_times(10) # returns an array of 10 encounter times.
         ```
     '''
-    if isinstance(size, tuple): 
+    if isinstance(size, tuple):
       size = tuple([int(i) for i in size])
       return _exponential.rvs(scale=1/self.encounter_rate, size=size) << self.units['time']
     else:
       size = int(size)
       return _exponential.rvs(scale=1/self.encounter_rate, size=size) << self.units['time']
 
   def time_to_next_encounter(self):
@@ -402,15 +402,15 @@
 
 
 class LocalNeighborhood(StellarEnvironment):
   '''
     This is a `StellarEnvironment` subclass for the Local Neighborhood.
     It encapsulates the relevant data for a static stellar environment representing the local neighborhood of the solar system.
 
-    The stellar density is 0.14 $\\rm{pc}^{-3}$ defined by [Bovy (2017)](https://ui.adsabs.harvard.edu/abs/2017MNRAS.470.1360B/abstract). 
+    The stellar density is 0.14 $\\rm{pc}^{-3}$ defined by [Bovy (2017)](https://ui.adsabs.harvard.edu/abs/2017MNRAS.470.1360B/abstract).
     The velocity distribution is defined using a Maxwell-Boltzmann distribution where the velocity dispersion is 20 km/s, defined by [Binnery & Tremaine (2008)](https://ui.adsabs.harvard.edu/abs/2008gady.book.....B/abstract) where the $v_\\rm{rms} \\sim 50$ km/s and [Bailer-Jones et al. (2018)](https://ui.adsabs.harvard.edu/abs/2018A%26A...616A..37B/abstract) so that 90% of stars have v < 100 km/s with an encounter rate of ~20 stars/Myr within 1 pc. However, a more accurate representation of the velocity distribution in the solar neighborhood is a triaxial Gaussian distribution, but that has not been implemented here.
     The mass limits is defined to between 0.08-8 solar masses using Equation (17) from [Chabrier (2003)](https://ui.adsabs.harvard.edu/abs/2003PASP..115..763C/abstract) for single stars when m < 1 and a power-law model from [Bovy (2017)](https://ui.adsabs.harvard.edu/abs/2017MNRAS.470.1360B/abstract) for stars m ≥ 1 to account for depleted stars due to stellar evolution.
 
     Example:
       ```python
       import airball
       my_local = airball.LocalNeighborhood()
```

### Comparing `airball-0.6.1/src/airball/imf.py` & `airball-0.7.0/src/airball/imf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,41 @@
 import numpy as _np
 import types as _types
 from scipy.integrate import quad as _quad
 from . import units as _u
 from . import tools as _tools
 
 class Distribution():
-  def __init__(self, mass_function, **kwargs):
+  '''
+  Base class for defining a probability distribution function.
+  This class is used to wrap a probability distribution function and its parameters into a single object.
+
+  Args:
+    mass_function (function): Probability distribution function.
+    args (list): List of arguments for the probability distribution function.
+
+  Returns:
+    pdf (float or ndarray): Probability density at the given mass value(s).
+  
+  Example:
+    ```python
+    import airball
+    mf = airball.imf.Distribution(lambda x, A: A * x, [1])
+    imf = airball.IMF(0.1, 100, mass_function=mf)
+    imf.random_mass()
+    ```
+
+  '''
+
+  def __init__(self, mass_function, args):
     self.mass_function = mass_function
-    self.params = kwargs
+    self.params = args
   
   def __call__(self, x):
-    return self.mass_function(x, **self.params)
+    return self.mass_function(x, *self.params)
 
 class chabrier_2003_single(Distribution):
   """
   Chabrier 2003 IMF for single stars.
   This function calculates the probability density for a given mass value (x) based on Equation (17) of Chabrier 2003 for an IMF for single stars.
 
   $$PDF(x) = \\frac{A}{x} \\exp\\left[-\\frac{(\\log_{10}(x) - \\log_{10}(0.079))^2 }{ 2 \\cdot 0.69^2}\\right]$$
@@ -29,16 +50,15 @@
     ```python
     import airball
     imf = airball.IMF(0.1, 100, mass_function=airball.imf.chabrier_2003_single(A=0.158))
     imf.random_mass()
     ```
   """
   def __init__(self, A=0.158):
-    kwargs = {k: v for k, v in locals().items() if k not in ('self', '__class__')}
-    super().__init__(self._chabrier_2003_single, **kwargs)
+    super().__init__(self._chabrier_2003_single, [A])
   
   def _chabrier_2003_single(self, x, A=0.158):
     return (A / x) * _np.exp(-((_np.log10(x) - _np.log10(0.079)) ** 2) / (2 * 0.69 ** 2))
 
 class salpeter_1955(Distribution):
   """
   Salpeter 1955 IMF for single stars.
@@ -56,16 +76,15 @@
     ```python
     import airball
     imf = airball.IMF(0.1, 100, mass_function=airball.imf.salpeter_1955(A=1))
     imf.random_mass()
     ```
   """
   def __init__(self, A):
-    kwargs = {k: v for k, v in locals().items() if k not in ('self', '__class__')}
-    super().__init__(self._salpeter_1955, **kwargs)
+    super().__init__(self._salpeter_1955, [A])
   
   def _salpeter_1955(self, x, A):
     return A * x ** -2.3
 
 class default_mass_function(Distribution):
   '''
   Default mass function for an IMF. This function is a piecewise function that uses the IMF for single stars from Chabrier 2003 for masses less than 1 solar mass and the Salpeter 1955 IMF for masses greater than 1 solar mass.
@@ -80,15 +99,15 @@
     ```python
     import airball
     imf = airball.IMF(0.1, 100, mass_function=airball.imf.default_mass_function())
     imf.random_mass()
     ```
   '''
   def __init__(self):
-    super().__init__(self._default_mass_function)
+    super().__init__(self._default_mass_function, [])
   
   def _default_mass_function(self, x):
     chabrier03 = chabrier_2003_single(A=0.158)
     salpeter55 = salpeter_1955(A=chabrier03(1))
     return _np.where(x < 1, chabrier03(x), salpeter55(x))
 
 class uniform(Distribution):
@@ -115,16 +134,15 @@
     alpha (float): Power law index.
     A (float): Normalization factor.
 
   Returns:
     pdf (float or ndarray): Probability density at the given mass value(s).
   '''
   def __init__(self, alpha, A):
-    kwargs = {k: v for k, v in locals().items() if k not in ('self', '__class__')}
-    super().__init__(self._power_law, **kwargs)
+    super().__init__(self._power_law, [alpha, A])
   
   def _power_law(self, x, alpha, A):
     return A * x ** alpha
 
 class broken_power_law(Distribution):
   '''
   Broken power law IMF.
@@ -138,16 +156,15 @@
     A (float): Normalization factor.
     x_0 (float): Break point between the two power laws.
     
   Returns:
     pdf (float or ndarray): Probability density at the given mass value(s).
   '''
   def __init__(self, alpha, beta, A, x_0):
-    kwargs = {k: v for k, v in locals().items() if k not in ('self', '__class__')}
-    super().__init__(self._broken_power_law, **kwargs)
+    super().__init__(self._broken_power_law, [alpha, beta, A, x_0])
 
   def _broken_power_law(self, x, alpha, beta, A, x_0):
     return _np.where(x < x_0, A * x ** alpha, A * x_0 ** (beta - alpha) * x ** beta)
 
 class lognormal(Distribution):
   '''
   Lognormal IMF.
@@ -160,16 +177,15 @@
     sigma (float): Standard deviation of the lognormal distribution.
     A (float): Normalization factor.
     
   Returns:
     pdf (float or ndarray): Probability density at the given mass value(s).
   '''
   def __init__(self, mu, sigma, A):
-    kwargs = {k: v for k, v in locals().items() if k not in ('self', '__class__')}
-    super().__init__(self._lognormal, **kwargs)
+    super().__init__(self._lognormal, [mu, sigma, A])
   
   def _lognormal(self, x, mu, sigma, A):
     return A * _np.exp(-(x - mu) ** 2 / (2 * sigma ** 2))
 
 class loguniform(Distribution):
   '''
   Loguniform IMF.
@@ -180,16 +196,15 @@
   Args:
     A (float): Normalization factor.
     
   Returns:
     pdf (float or ndarray): Probability density at the given mass value(s).
   '''
   def __init__(self, A):
-    kwargs = {k: v for k, v in locals().items() if k not in ('self', '__class__')}
-    super().__init__(self._loguniform, **kwargs)
+    super().__init__(self._loguniform, [A])
 
   def _loguniform(self, x, A):
     return A / x
 
 class IMF():
   """
   Class representing an Initial Mass Function (IMF).
```

### Comparing `airball-0.6.1/src/airball/stars.py` & `airball-0.7.0/src/airball/stars.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,14 +323,26 @@
     if filename is not None and isinstance(filename, str):
       try:
         loaded = Stars._load(filename)
         self.__dict__ = loaded.__dict__
       except: raise Exception('Invalid filename.')
       return
     
+    # If nothing is specified, return an empty Stars object.
+    if not kwargs: 
+      self._m = _np.array([]) << self.units['mass']
+      self._b = _np.array([]) << self.units['length']
+      self._v = _np.array([]) << self.units['velocity']
+      self._inc = _np.array([]) << self.units['angle']
+      self._omega = _np.array([]) << self.units['angle']
+      self._Omega = _np.array([]) << self.units['angle']
+      self._shape = (0,)
+      self.environment = None
+      return
+
     # Determine the number of stars to generate.
     self._shape = (0,)
     for key in kwargs:
       try:
         if isinstance(kwargs[key], _u.Quantity):
             shape = kwargs[key].shape
             N = 0
@@ -347,15 +359,15 @@
 
     if 'size' in kwargs and self.N != 0: raise OverspecifiedParametersException('If lists are given then size cannot be specified.')
     elif 'size' in kwargs:
       if isinstance(kwargs['size'], tuple): 
         self._shape = tuple([int(i) for i in kwargs['size']])
       else: self._shape = (int(kwargs['size']),)
     elif self.N == 0: raise UnspecifiedParameterException('If no lists of parameters are given then size must be specified.')
-    else: pass
+    else: pass # No errors or issues, continue.
 
 
     # Initialize Stars from environment.
     self.environment = kwargs.get('environment', None)
     if (('environment' in kwargs or 'env' in kwargs) or  isinstance(filename, _env.StellarEnvironment)) and 'size' in kwargs:
       if self.N <= 1: raise InvalidValueForKeyException("If a generating environment is given then size must be greater than 1.")
       if 'environment' in kwargs:
@@ -696,17 +708,17 @@
 
     Returns:
       eccentricity (ndarray): The eccentricity of the Stars.
     '''
     return self.e(sim)
 
   def e(self, sim):
-    sim_units = _tools.rebound_units(sim)
-    G = (sim.G * sim_units['length']**3 / sim_units['mass'] / sim_units['time']**2)
-    mu = G * (_tools.system_mass(sim) * sim_units['mass'] + self.m)
+    units = _tools.rebound_units(sim)
+    G = (sim.G * units.length**3 / units.mass / units.time**2)
+    mu = G * (_tools.system_mass(sim) * units.mass + self.m)
 
     numerator = self.b * self.v*self.v
     return _np.sqrt(1 + (numerator/mu)**2.)
   
   def periastron(self, sim):
     '''
     The periastron of the Stars, alias for `q(sim)`.
@@ -833,15 +845,15 @@
       ```
     """
     if not isinstance(filename, str): raise ValueError('Filename must be a string.')
     with open(filename, 'wb') as pfile:
       _pickle.dump(self, pfile, protocol=_pickle.HIGHEST_PROTOCOL)
 
   @classmethod
-  def _load(self, filename, init=False):
+  def _load(cls, filename, init=False):
     """
     Load an instance of the Stars class from a file using pickle.
 
     Args:
       filename (str): The name of the file to load the instance from. The file should be in binary format, pickled.
 
     Returns:
@@ -859,17 +871,17 @@
   def stats(self, returned=False):
     '''
     Prints a summary of the current stats of the Stars object.
     The stats are returned as a string if `returned=True`.
     '''
     s = f"<{self.__module__}.{type(self).__name__} object at {hex(id(self))}, "
     s += f"N={f'{self.N:,.0f}' if len(self.shape) == 1 else self.shape}"
-    s += f", m= {_np.min(self.m.value):,.2f}-{_np.max(self.m.value):,.2f} {self.units['mass']}"
-    s += f", b= {_np.min(self.b.value):,.0f}-{_np.max(self.b.value):,.0f} {self.units['length']}"
-    s += f", v= {_np.min(self.v.value):,.0f}-{_np.max(self.v.value):,.0f} {self.units['velocity']}"
+    if self.N > 0: s += f", m= {_np.min(self.m.value):,.2f}-{_np.max(self.m.value):,.2f} {self.units['mass']}"
+    if self.N > 0: s += f", b= {_np.min(self.b.value):,.0f}-{_np.max(self.b.value):,.0f} {self.units['length']}"
+    if self.N > 0: s += f", v= {_np.min(self.v.value):,.0f}-{_np.max(self.v.value):,.0f} {self.units['velocity']}"
     s += f"{f', Environment={self.environment.name}' if self.environment is not None else ''}"
     s += ">"
     if returned: return s
     else: print(s)
   
   def __str__(self):
     return self.stats(returned=True)
@@ -956,14 +968,20 @@
     data = []
     for d in sorted(self.__dict__.items()):
         try: data.append((d[0], tuple(d[1])))
         except: data.append(d)
     data = tuple(data)
     return hash(data)
   
+  def __add__(self, other):
+    # Overrides the default implementation
+    if isinstance(other, Stars):
+      if self.N == 0 and other.N == 0: return Stars()
+      else: return Stars(m=_np.concatenate((self.m, other.m)), b=_np.concatenate((self.b, other.b)), v=_np.concatenate((self.v, other.v)), inc=_np.concatenate((self.inc, other.inc)), omega=_np.concatenate((self.omega, other.omega)), Omega=_np.concatenate((self.Omega, other.Omega)))
+    return NotImplemented
 
 ################################
 ###### Custom Exceptions #######
 ################################
 
 class InvalidStarException(Exception):
   def __init__(self): super().__init__('Object is not a valid airball.Star object.')
```

### Comparing `airball-0.6.1/src/airball/tools.py` & `airball-0.7.0/src/airball/tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,47 @@
 import numpy as _np
+import rebound as _rebound
 import joblib as _joblib
 import warnings as _warnings
-from scipy.stats import maxwell
 from .units import UnitSet as _UnitSet
 from . import units as _u
+from mpmath import mp as _mp
+
+# Set the precision
+_mp.dps = 50  # 50 digits of precision
 
 twopi = 2.*_np.pi
 
 ############################################################
 ################### Helper Functions #######################
 ############################################################
 
+def rotate_into_plane(sim, plane):
+    '''
+    Rotates the simulation into the specified plane.
+
+    Args:
+        sim (Simulation): The REBOUND Simulation containing the star and planets that will experience a flyby.
+        plane (str, int): The plane defining the orientation of the star: None, 'invariable', 'ecliptic', or int.
+
+    Returns:
+        rotation (Rotation): The rotation that was applied to the simulation.
+    '''
+    int_types = (int, _np.integer)
+    rotation = _rebound.Rotation.to_new_axes(newz=[0,0,1])
+    if plane is not None:
+        # Move the system into the chosen plane of reference. TODO: Make sure the angular momentum calculations don't include other flyby stars.
+        if plane == 'invariable': rotation = _rebound.Rotation.to_new_axes(newz=sim.angular_momentum())
+        elif plane == 'ecliptic': rotation = _rebound.Rotation.to_new_axes(newz=calculate_angular_momentum(sim)[3]) # Assumes Earth is particle 3. 0-Sun, 1-Mecury, 2-Venus, 3-Earth, ...
+        elif isinstance(plane, int_types):
+            p = sim.particles[int(plane)]
+            rotation = (_rebound.Rotation.orbit(Omega=p.Omega, inc=p.inc, omega=p.omega)).inverse()
+    sim.rotate(rotation)
+    return rotation
+
 # Implemented from StackOverflow: https://stackoverflow.com/a/14314054
 def moving_average(a, n=3, method=None) :
     '''
     Compute the moving average of an array of numbers using the nearest n elements.
     Adapted from [StackOverflow](https://stackoverflow.com/a/14314054).
     
     The options for handling NaN values are: `'nn'` (nearest neighbor), `'nan'` (ignore NaNs), and `None`. The default is `None` which uses `numpy.cumsum`. The `'nn'` method is slower than `'nan'` but attempts to replace the NaN values with the average of the adjacent values. Thus, if the adjacent values are NaN, then it will also return NaN.
@@ -172,37 +199,49 @@
     x = geometric_means(b)
     w = wfac * x*_np.mean((x[1:] - x[:-1])/x[:-1])
     
     if normalize: return x, y/_np.trapz(y,x), w
     else: return x,y,w
 
 def unit_vector(vector):
-    """ Returns the unit vector of the vector."""
-    return vector / _np.linalg.norm(vector)
+    """ 
+    Returns the unit vector of the vector.
+    Fails if the vector is a list of Quantity objects.
+    
+    Args:
+      vector (array): The vector to convert to a unit vector.
+
+    Returns:
+      vector (array): The unit vector of the vector.
+    """
+    try:
+        if len(vector.shape) > 1: return vector / _np.linalg.norm(vector, axis=1)[:,None]
+        else: return vector / _np.linalg.norm(vector)
+    except AttributeError: return vector / _np.linalg.norm(vector)
 
 def angle_between(v1, v2):
     """ Returns the angle in radians between vectors 'v1' and 'v2'. Implemented from [StackOverflow](https://stackoverflow.com/a/13849249/71522).
 
     Args:
       v1 (array): The first vector.
       v2 (array): The second vector.
     
     Returns:
-      theta (float): The angle between the two vectors in radians.
+      theta (float): The angle between the two vectors in units of radians.
     
     Example:
       ```python
       angle_between((1, 0, 0), (0, 1, 0)) # 1.5707963267948966
       angle_between((1, 0, 0), (1, 0, 0)) # 0.0
       angle_between((1, 0, 0), (-1, 0, 0)) # 3.141592653589793
       ```
     """
     v1_u = unit_vector(v1)
     v2_u = unit_vector(v2)
-    return _np.arccos(_np.clip(_np.dot(v1_u, v2_u), -1.0, 1.0))
+    return _np.arccos(_np.dot(v1_u, v2_u.T))
 
 def mod2pi(f):
     '''Converts an angle to the range [0, 2pi). Implemented from REBOUND using Numpy to handle vectorization.'''
     return _np.mod(twopi + _np.mod(f, twopi), twopi)
 
 def M_to_E(e, M):
   '''Converts mean anomaly to eccentric anomaly. Implemented from REBOUND using Numpy to handle vectorization.'''
@@ -232,15 +271,14 @@
   else: return mod2pi(2.*_np.arctan(_np.sqrt((1.+e)/(1.-e))*_np.tan(0.5*E)))
 
 def M_to_f(e, M):
   '''Converts mean anomaly to true anomaly. Implemented from REBOUND using Numpy to handle vectorization.'''
   E = M_to_E(e, M)
   return E_to_f(e, E)
 
-
 ############################################################
 ############### Properties and Elements ####################
 ############################################################
 
 def calculate_angular_momentum(sim):
     '''
         Calculates the angular momentum of the system and of each particle in the system.
@@ -359,20 +397,20 @@
         star_mass (Quantity): The mass of the flyby star to calculate the gravitational parameter of.
       
       Returns:
         mu (Quantity): The gravitational parameter of the system.
     '''
     # Convert the units of the REBOUND Simulation into Astropy Units.
     units = rebound_units(sim)
-    G = (sim.G * units['length']**3 / units['mass'] / units['time']**2)
+    G = (sim.G * units.length**3 / units.mass / units.time**2)
     if star is not None and star_mass is not None: raise Exception('Cannot define both star and star_mass.')
-    elif star is not None and star_mass is None: star_mass = verify_unit(star.mass, units['mass'])
-    elif star is None and star_mass is not None: star_mass = verify_unit(star_mass, units['mass'])
+    elif star is not None and star_mass is None: star_mass = verify_unit(star.mass, units.mass)
+    elif star is None and star_mass is not None: star_mass = verify_unit(star_mass, units.mass)
     else: raise Exception('Either star or star_mass must be defined.')
-    return G * (system_mass(sim)  * units['mass'] + star_mass)
+    return G * (system_mass(sim) * units.mass + star_mass)
 
 def calculate_periastron(sim, star):
     '''
         Using the impact parameter and the relative velocity at infinity between the two stars convert to the periastron of the flyby star.
 
         Args:
           sim (Simulation): The REBOUND Simulation to calculate the periastron with respect to.
@@ -434,15 +472,15 @@
       ```
     """
     e = calculate_eccentricity(sim, star)
     a = -star.b/_np.sqrt(e**2. - 1.) # Compute the semi-major axis of the flyby star
     l = semilatus_rectum(a=a, e=e) # Compute the semi-latus rectum of the hyperbolic orbit to get the true anomaly
 
     rmax = verify_unit(rmax, _u.au)
-    if star.N > 1: rmax = _np.array(star.N * [rmax.value]) << rmax.unit
+    if star.N > 1 and not isList(rmax): rmax = _np.array(star.N * [rmax.value]) << rmax.unit
     with _warnings.catch_warnings():
       _warnings.simplefilter("error")
       # Make sure that the value for rmax is sufficiently large.
       div = (_np.divide(l, rmax, out=_np.full_like(rmax, 0), where=rmax!=0) - 1.0)/e # if rmax is 0, then set f=0. Catch divide by zero warning.
       try:
         if star.N > 1:
           if _np.any(rmax[rmax != 0] < star.b[rmax != 0]): raise RuntimeWarning()
@@ -459,23 +497,129 @@
         E = _np.arccosh((_np.cos(f)+e)/(1.+e*_np.cos(f))) # Compute the eccentric anomaly
         M = e * _np.sinh(E)-E # Compute the mean anomaly
     Tperi = M/_np.sqrt(mu/(-a*a*a))
 
     if values_only: return {'m':star.m.value, 'a':a.value, 'e':e.value, 'inc':star.inc.value, 'omega':star.omega.value, 'Omega':star.Omega.value, 'f':-f.value}
     return {'m':star.m, 'a':a, 'e':e, 'inc':star.inc, 'omega':star.omega, 'Omega':star.Omega, 'f':-f, 'T':Tperi}
 
+def hyperbolic_plane(sim, star):
+    '''
+      Calculate the plane of the hyperbolic orbit of the flyby star using the position and velocity vectors of the flyby star when the star is a perihelion.
+      
+      Args:
+        sim (Simulation): The simulation with two bodies, a central star and a planet.
+        star (Star): The star that is flying by.
+
+      Returns:
+        AB (dict): The normalized vectors defining the plane of the hyperbolic orbit. The vectors are `A` and `B` which are unit vectors in the direction of the perihelion and the ascending node, respectively.
+    '''
+    e = calculate_eccentricity(sim, star)
+    
+    cO = _np.cos(star.Omega)
+    sO = _np.sin(star.Omega)
+    co = _np.cos(star.omega)
+    so = _np.sin(star.omega)
+    ci = _np.cos(star.inc)
+    si = _np.sin(star.inc)
+
+    cf = _np.cos(0)
+    sf = _np.sin(0)
+    A = unit_vector([(cO*(co*cf-so*sf) - sO*(so*cf+co*sf)*ci), (sO*(co*cf-so*sf) + cO*(so*cf+co*sf)*ci), (so*cf+co*sf)*si])
+    B = unit_vector([((e+cf)*(-ci*co*sO - cO*so) - sf*(co*cO - ci*so*sO)), ((e+cf)*(ci*co*cO - sO*so)  - sf*(co*sO + ci*so*cO)), ((e+cf)*co*si - sf*si*so)])
+    
+    return {'A': A, 'B': B}
+
+def cartesian_elements(sim, star, rmax, values_only=False):
+    '''
+      Returns the Cartesian elements in the Heliocentric frame, based on the total mass of the REBOUND Simulation.
+      Implemented from REBOUND using Numpy to handle vectorization.
+
+      Args:
+      sim (Simulation): The simulation with two bodies, a central star and a planet.
+      star (Star): The star that is flying by.
+      rmax (float): The starting distance of the flyby star. Defaults to units of AU.
+      values_only (bool): Whether to return only the values of the hyperbolic orbital elements. If True, then the results can be used to add a new particle to a REBOUND Simulation. Defaults to False.
+
+    Returns:
+      elements (dict): A dictionary containing the hyperbolic orbital elements: `{m, a, e, inc, omega, Omega, f, T}`.
+      values_only (dict): A dictionary containing the hyperbolic orbital elements: `m`, `a`, `e`, `inc`, `omega`, `Omega`, `f`.
+
+    Raises:
+      RuntimeError: If the value for `rmax` is smaller than the impact parameter, `b`.
+
+    Example:
+      ```python
+      import rebound
+      import airball
+      sim = rebound.Simulation()
+      sim.add(m=1)
+      sim.add(m=5e-5, a=30)
+      star = airball.Star(m=1, b=500, v=5)
+      elements = hyperbolic_elements(sim, star, rmax=100)
+      ```
+    '''
+    units = rebound_units(sim)
+    G = (sim.G * units.length**3 / units.mass / units.time**2)
+
+    sim.move_to_hel()
+    primary = sim.com()
+    sim.move_to_com()
+    elements = hyperbolic_elements(sim, star, rmax=rmax, values_only=False)
+    m,a,e,inc,omega,Omega,f = elements['m'], elements['a'], elements['e'], elements['inc'], elements['omega'], elements['Omega'], elements['f']
+    if _np.any(e < 0.): raise ValueError('Eccentricity must be greater than or equal to zero.')
+    if _np.any(e > 1.):
+        if _np.any(a > 0.):
+            raise ValueError('Bound orbit (a > 0) must have e < 1.')
+    else:
+        if _np.any(a < 0.):
+            raise ValueError('Unbound orbit (a < 0) must have e > 1.')
+    if _np.any(e*_np.cos(f) < -1.):
+        raise ValueError('Unbound orbit can\'t have f set beyond the range allowed by the asymptotes set by the parabola.')
+    if primary.m < 1e-15:
+        raise ValueError('Primary has no mass.')
+
+    r = a*(1-e*e)/(1 + e*_np.cos(f))
+    v0 = _np.sqrt(G*(m + primary.m*units.mass)/a/(1.-e*e))  # in this form it works for elliptical and hyperbolic orbits
+
+    cO = _np.cos(Omega)
+    sO = _np.sin(Omega)
+    co = _np.cos(omega)
+    so = _np.sin(omega)
+    cf = _np.cos(f)
+    sf = _np.sin(f)
+    ci = _np.cos(inc)
+    si = _np.sin(inc)
+
+    # Murray & Dermott Eq 2.122
+    x = primary.x * units.length + r*(cO*(co*cf-so*sf) - sO*(so*cf+co*sf)*ci)
+    y = primary.y * units.length + r*(sO*(co*cf-so*sf) + cO*(so*cf+co*sf)*ci)
+    z = primary.z * units.length + r*(so*cf+co*sf)*si
+
+    # Murray & Dermott Eq. 2.36 after applying the 3 rotation matrices from Sec. 2.8 to the velocities in the orbital plane
+    vx = primary.vx * units.length/units.time + v0*((e+cf)*(-ci*co*sO - cO*so) - sf*(co*cO - ci*so*sO))
+    vy = primary.vy * units.length/units.time + v0*((e+cf)*(ci*co*cO - sO*so)  - sf*(co*sO + ci*so*cO))
+    vz = primary.vz * units.length/units.time + v0*((e+cf)*co*si - sf*si*so)
+
+    if values_only: return {'m':m.value, 'x':x.value, 'y':y.value, 'z':z.value, 'vx':vx.value, 'vy':vy.value, 'vz':vz.value}
+    return {'m':m, 'x':x, 'y':y, 'z':z, 'vx':vx, 'vy':vy, 'vz':vz, 'T':elements['T']}
+
 def impulse_gradient(star):
     '''Calculate the impulse gradient for a flyby star, $\\frac{2 G M}{v b^2}$.'''
     G = (1 * _u.au**3 / _u.solMass / _u.yr2pi**2)
     return ((2.0 * G * star.m) / (star.v * star.b**2.0)).to(_u.km/_u.s/_u.au)
 
 ############################################################
 ############# Stellar Environment Functions ################
 ############################################################
 
+def maxwell_boltzmann_dispersion_from_scale(scale):
+    '''
+        Converts velocity dispersion (variance) $\\sigma$ to scale factor $a$ for [Maxwell-Boltzmann distributions](https://en.wikipedia.org/wiki/Maxwell-Boltzmann_distribution), $\\sigma = a \\sqrt{\\frac{(3\\pi - 8)}{\\pi}}$.
+    '''
+    return scale * _np.sqrt((3.0*_np.pi - 8.0)/(_np.pi))
 
 def maxwell_boltzmann_scale_from_dispersion(sigma):
     '''
         Converts velocity dispersion (variance) $\\sigma$ to scale factor $a$ for [Maxwell-Boltzmann distributions](https://en.wikipedia.org/wiki/Maxwell-Boltzmann_distribution), $a = \\sqrt{\\frac{\\pi\\sigma^2}{3\\pi - 8}}$.
     '''
     return _np.sqrt((_np.pi*_np.square(sigma))/(3.0*_np.pi - 8.0))
```

### Comparing `airball-0.6.1/src/airball/units.py` & `airball-0.7.0/src/airball/units.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import astropy.units as _u
 from astropy.units import *
 twopi = 6.28318530717958623199592693708837032318115234375
-yrtwopi = def_unit('yrtwopi', _u.yr/twopi, format={'latex': r'(yr/2\pi)'})
-yr2pi = def_unit('yr2pi', _u.yr/twopi, format={'latex': r'(yr/2\pi)'})
-stars = def_unit('stars')
-add_enabled_units([yr2pi, yrtwopi])
-add_enabled_aliases({'msun': _u.solMass})
+yrtwopi = _u.def_unit('yrtwopi', _u.yr/twopi, format={'latex': r'(yr/2\pi)'})
+yr2pi = _u.def_unit('yr2pi', _u.yr/twopi, format={'latex': r'(yr/2\pi)'})
+stars = _u.def_unit('stars')
+_u.add_enabled_units([yr2pi, yrtwopi])
+_u.add_enabled_aliases({'msun': _u.solMass})
 
 
 def isUnit(var):
     '''Determines if an object is an Astropy Quantity. Used for Stellar Environment initializations.'''
     return isinstance(var, (_u.core.IrreducibleUnit, _u.core.CompositeUnit, _u.Unit))
 
 class UnitSet():
@@ -53,61 +53,61 @@
   @property
   def units(self):
     return self._units
 
   @property
   def UNIT_SYSTEM(self):
     return self._UNIT_SYSTEM
-  
+
   def __getitem__(self, key):
     if isinstance(key, str): return self.units[key]
-    else: raise InvalidKeyException() 
-  
+    else: raise InvalidKeyException()
+
   def __setitem__(self, key, value):
     if isinstance(key, str):
       if isUnit(value): self.units[key] = value
-      else: raise InvalidUnitException() 
-    else: raise InvalidKeyException() 
+      else: raise InvalidUnitException()
+    else: raise InvalidKeyException()
 
   def __str__(self):
     s = '{'
     for key in self.units:
        s += f'{key}: {self.units[key].to_string()}, '
     s = s[:-2] + '}'
     return s
-  
+
   def __repr__(self):
     s = '{'
     for key in self.units:
        s += f'{key}: {self.units[key].to_string()},\n'
     s = s[:-2] + '}'
     return s
-  
+
   def __iter__(self):
     for k in self.units:
       yield self.units[k]
-  
+
   def __eq__(self, other):
     # Determines if the string representations of the units in each UnitSets are identical.
     if isinstance(other, UnitSet):
         result = True
         for u1,u2 in zip(self, other):
             result = result and (u1.to_string() == u2.to_string())
         return result
     return NotImplemented
-  
+
   def __hash__(self):
     # Overrides the default implementation
     data = []
     for d in sorted(self.__dict__.items()):
         try: data.append((d[0], tuple(d[1])))
         except: data.append(d)
     data = tuple(data)
     return hash(data)
-  
+
   def values(self):
     return self.units.values()
 
   @property
   def length(self):
     return self._units['length']
 
@@ -183,28 +183,27 @@
       self._units['angle'] = angleUnit[0] if angleUnit != [] else self._units['angle']
 
       objectUnit = [this for this in UNIT_SYSTEM if this.is_equivalent(stars)]
       self._units['object'] = objectUnit[0] if objectUnit != [] else stars
 
       densityUnit = [this for this in UNIT_SYSTEM if this.is_equivalent(stars/_u.m**3)]
       densityUnit2 = [this for this in UNIT_SYSTEM if this.is_equivalent(1/_u.m**3)]
-      if densityUnit == [] and densityUnit2 != []: 
+      if densityUnit == [] and densityUnit2 != []:
         densityUnit = [self._units['object'] * densityUnit2[0]]
-      elif densityUnit == [] and objectUnit != [] and lengthUnit != []: 
+      elif densityUnit == [] and objectUnit != [] and lengthUnit != []:
         densityUnit = [self._units['object']/self._units['length']**3]
       elif densityUnit == [] and densityUnit2 == [] and objectUnit != []:
          densityLength = [this for this in self._units['density'].bases if this.is_equivalent(_u.m)][0]
          densityUnit = [self._units['object']/densityLength**3]
       self._units['density'] = densityUnit[0] if densityUnit != [] else self._units['density']
-    
+
     self._UNIT_SYSTEM = list(self._units.values())
 
 ############################################################
 ###################### Exceptions ##########################
 ############################################################
 
 class InvalidKeyException(Exception):
   def __init__(self): super().__init__('Invalid key type.')
 
 class InvalidUnitException(Exception):
   def __init__(self): super().__init__('Value is not a valid unit type.')
-
```

### Comparing `airball-0.6.1/src/airball.egg-info/PKG-INFO` & `airball-0.7.0/src/airball.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airball
-Version: 0.6.1
+Version: 0.7.0
 Summary: A package for running and managing flybys using REBOUND
 Home-page: https://github.com/zyrxvo/airball/
 Author: Garett Brown
 Author-email: garett.brown@mail.utoronto.ca
 Project-URL: Bug Tracker, https://github.com/zyrxvo/airball/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

