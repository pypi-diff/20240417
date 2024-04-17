# Comparing `tmp/dorado-scheduling-0.1.0.tar.gz` & `tmp/dorado_scheduling-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dorado-scheduling-0.1.0.tar", last modified: Wed Feb  3 03:59:22 2021, max compression
+gzip compressed data, was "dorado_scheduling-0.2.0.tar", max compression
```

## Comparing `dorado-scheduling-0.1.0.tar` & `dorado_scheduling-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,54 @@
--rw-r--r--   0        0        0    12550 2021-02-03 03:59:09.323286 dorado-scheduling-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0        0 2021-02-03 03:59:09.323789 dorado-scheduling-0.1.0/dorado/scheduling/__init__.py
--rw-r--r--   0        0        0     1267 2021-02-03 03:59:09.324084 dorado-scheduling-0.1.0/dorado/scheduling/constraints/__init__.py
--rw-r--r--   0        0        0     1192 2021-02-03 03:59:09.324303 dorado-scheduling-0.1.0/dorado/scheduling/constraints/earth_limb.py
--rw-r--r--   0        0        0     1150 2021-02-03 03:59:09.324494 dorado-scheduling-0.1.0/dorado/scheduling/constraints/orbit_night.py
--rw-r--r--   0        0        0     1804 2021-02-03 03:59:09.324674 dorado-scheduling-0.1.0/dorado/scheduling/constraints/saa.py
--rw-r--r--   0        0        0      574 2021-02-03 03:59:09.324899 dorado-scheduling-0.1.0/dorado/scheduling/data/L_SAA_2008198.03
--rw-r--r--   0        0        0      303 2021-02-03 03:59:09.325067 dorado-scheduling-0.1.0/dorado/scheduling/data/README.md
--rw-r--r--   0        0        0        0 2021-02-03 03:59:09.325154 dorado-scheduling-0.1.0/dorado/scheduling/data/__init__.py
--rw-r--r--   0        0        0      164 2021-02-03 03:59:09.325308 dorado-scheduling-0.1.0/dorado/scheduling/data/orbits.txt
--rw-r--r--   0        0        0     2324 2021-02-03 03:59:09.325499 dorado-scheduling-0.1.0/dorado/scheduling/orbit.py
--rw-r--r--   0        0        0      876 2021-02-03 03:59:09.325679 dorado-scheduling-0.1.0/dorado/scheduling/regard.py
--rw-r--r--   0        0        0        0 2021-02-03 03:59:09.325924 dorado-scheduling-0.1.0/dorado/scheduling/scripts/__init__.py
--rw-r--r--   0        0        0     7216 2021-02-03 03:59:09.326200 dorado-scheduling-0.1.0/dorado/scheduling/scripts/animate.py
--rw-r--r--   0        0        0     5913 2021-02-03 03:59:09.326427 dorado-scheduling-0.1.0/dorado/scheduling/scripts/main.py
--rw-r--r--   0        0        0     3037 2021-02-03 03:59:09.326668 dorado-scheduling-0.1.0/dorado/scheduling/skygrid.py
--rw-r--r--   0        0        0        0 2021-02-03 03:59:09.327154 dorado-scheduling-0.1.0/dorado/scheduling/tests/__init__.py
--rw-r--r--   0        0        0     2944 2021-02-03 03:59:09.327356 dorado-scheduling-0.1.0/dorado/scheduling/tests/test_earth_limb.py
--rw-r--r--   0        0        0     1018 2021-02-03 03:59:09.362414 dorado-scheduling-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1166 2021-02-03 03:59:22.129100 dorado-scheduling-0.1.0/setup.py
--rw-r--r--   0        0        0      697 2021-02-03 03:59:22.129350 dorado-scheduling-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    12550 2024-04-17 20:56:11.015625 dorado_scheduling-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2787 2024-04-17 20:56:11.015625 dorado_scheduling-0.2.0/README.md
+-rw-r--r--   0        0        0      423 2024-04-17 20:56:11.015625 dorado_scheduling-0.2.0/dorado/scheduling/__init__.py
+-rw-r--r--   0        0        0     2569 2024-04-17 20:56:11.015625 dorado_scheduling-0.2.0/dorado/scheduling/_slew.py
+-rw-r--r--   0        0        0     1989 2024-04-17 20:56:11.015625 dorado_scheduling-0.2.0/dorado/scheduling/constraints/__init__.py
+-rw-r--r--   0        0        0     1298 2024-04-17 20:56:11.015625 dorado_scheduling-0.2.0/dorado/scheduling/constraints/bright_earth_limb.py
+-rw-r--r--   0        0        0     1198 2024-04-17 20:56:11.015625 dorado_scheduling-0.2.0/dorado/scheduling/constraints/earth_limb.py
+-rw-r--r--   0        0        0     1156 2024-04-17 20:56:11.015625 dorado_scheduling-0.2.0/dorado/scheduling/constraints/orbit_night.py
+-rw-r--r--   0        0        0     1279 2024-04-17 20:56:11.015625 dorado_scheduling-0.2.0/dorado/scheduling/constraints/radiation.py
+-rw-r--r--   0        0        0      701 2024-04-17 20:56:11.015625 dorado_scheduling-0.2.0/dorado/scheduling/data/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 20:56:11.015625 dorado_scheduling-0.2.0/dorado/scheduling/data/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-17 20:56:11.015625 dorado_scheduling-0.2.0/dorado/scheduling/data/dorado-510km-31inc.tle
+-rw-r--r--   0        0        0      140 2024-04-17 20:56:11.015625 dorado_scheduling-0.2.0/dorado/scheduling/data/dorado-510km-60inc.tle
+-rw-r--r--   0        0        0      140 2024-04-17 20:56:11.015625 dorado_scheduling-0.2.0/dorado/scheduling/data/dorado-510km-sunsync.tle
+-rw-r--r--   0        0        0      140 2024-04-17 20:56:11.015625 dorado_scheduling-0.2.0/dorado/scheduling/data/dorado-625km-31inc.tle
+-rw-r--r--   0        0        0      140 2024-04-17 20:56:11.015625 dorado_scheduling-0.2.0/dorado/scheduling/data/dorado-625km-60inc.tle
+-rw-r--r--   0        0        0      140 2024-04-17 20:56:11.015625 dorado_scheduling-0.2.0/dorado/scheduling/data/dorado-625km-sunsync.tle
+-rw-r--r--   0        0        0      168 2024-04-17 20:56:11.015625 dorado_scheduling-0.2.0/dorado/scheduling/data/goes17.tle
+-rw-r--r--   0        0        0     2418 2024-04-17 20:56:11.015625 dorado_scheduling-0.2.0/dorado/scheduling/dust.py
+-rw-r--r--   0        0        0     5751 2024-04-17 20:56:11.015625 dorado_scheduling-0.2.0/dorado/scheduling/fov.py
+-rw-r--r--   0        0        0        0 2024-04-17 20:56:11.015625 dorado_scheduling-0.2.0/dorado/scheduling/metrics/__init__.py
+-rw-r--r--   0        0        0     6325 2024-04-17 20:56:11.015625 dorado_scheduling-0.2.0/dorado/scheduling/metrics/kne.py
+-rw-r--r--   0        0        0     6704 2024-04-17 20:56:11.015625 dorado_scheduling-0.2.0/dorado/scheduling/mission.py
+-rw-r--r--   0        0        0      387 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/orbit/__init__.py
+-rw-r--r--   0        0        0     1596 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/orbit/base.py
+-rw-r--r--   0        0        0     2567 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/orbit/spice.py
+-rw-r--r--   0        0        0     3312 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/orbit/tle.py
+-rw-r--r--   0        0        0     3747 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/schedulers/__init__.py
+-rw-r--r--   0        0        0     8264 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/schedulers/continuous_time_slew.py
+-rw-r--r--   0        0        0     4519 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/schedulers/discrete_time.py
+-rw-r--r--   0        0        0        0 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/scripts/__init__.py
+-rw-r--r--   0        0        0     8392 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/scripts/animate.py
+-rw-r--r--   0        0        0     3631 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/scripts/animate_skymaps.py
+-rw-r--r--   0        0        0     9612 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/scripts/animate_survey.py
+-rw-r--r--   0        0        0     6350 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/scripts/main.py
+-rw-r--r--   0        0        0     6176 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/scripts/metrics.py
+-rw-r--r--   0        0        0    23962 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/scripts/simsurvey.py
+-rw-r--r--   0        0        0     1292 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/scripts/skygrid.py
+-rw-r--r--   0        0        0     9570 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/scripts/survey_slicer.py
+-rw-r--r--   0        0        0     3176 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/skygrid/__init__.py
+-rw-r--r--   0        0        0     4766 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/skygrid/_geodesic.py
+-rw-r--r--   0        0        0     1107 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/skygrid/_healpix.py
+-rw-r--r--   0        0        0     1824 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/skygrid/_sinusoidal.py
+-rw-r--r--   0        0        0     1293 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/skygrid/_spiral.py
+-rw-r--r--   0        0        0        0 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/tests/__init__.py
+-rw-r--r--   0        0        0     2811 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/tests/test_earth_limb.py
+-rw-r--r--   0        0        0     1836 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/tests/test_orbit.py
+-rw-r--r--   0        0        0     1050 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/tests/test_skygrid.py
+-rw-r--r--   0        0        0      992 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/units/__init__.py
+-rw-r--r--   0        0        0      642 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/units/equivalencies.py
+-rw-r--r--   0        0        0      590 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/units/orbital.py
+-rw-r--r--   0        0        0     1586 2024-04-17 20:56:11.019625 dorado_scheduling-0.2.0/dorado/scheduling/utils.py
+-rw-r--r--   0        0        0     2831 2024-04-17 20:56:11.035626 dorado_scheduling-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4630 1970-01-01 00:00:00.000000 dorado_scheduling-0.2.0/PKG-INFO
```

### Comparing `dorado-scheduling-0.1.0/LICENSE.txt` & `dorado_scheduling-0.2.0/LICENSE.txt`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
    the Subject Software information on how to obtain the source code
    in a reasonable manner on or through a medium customarily used for
    software exchange.
 
 B. Each Recipient must ensure that the following copyright notice
 appears prominently in the Subject Software:
 
-Copyright © 2020 United States Government as represented by the Administrator
+Copyright © 2021 United States Government as represented by the Administrator
 of the National Aeronautics and Space Administration. No copyright is claimed
 in the United States under Title 17, U.S. Code. All Other Rights Reserved.
 
 C. Each Contributor must characterize its alteration of the Subject
 Software as a Modification and must identify itself as the originator
 of its Modification in a manner that reasonably allows subsequent
 Recipients to identify the originator of the Modification.  In
```

### Comparing `dorado-scheduling-0.1.0/dorado/scheduling/constraints/earth_limb.py` & `dorado_scheduling-0.2.0/dorado/scheduling/constraints/earth_limb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright © 2020 United States Government as represented by the Administrator
+# Copyright © 2021 United States Government as represented by the Administrator
 # of the National Aeronautics and Space Administration. No copyright is claimed
 # in the United States under Title 17, U.S. Code. All Other Rights Reserved.
 #
 # SPDX-License-Identifier: NASA-1.3
 #
 from astroplan.constraints import Constraint, _get_altaz
 from astropy.constants import R_earth
@@ -14,15 +14,15 @@
 
 class EarthLimbConstraint(Constraint):
     """
     Constrain the angle from the Earth limb.
 
     Parameters
     ----------
-    min : `~astropy.units.Quantity`
+    min : :class:`astropy.units.Quantity`
         Minimum angular separation from the Earth's limb.
 
     Notes
     -----
     This constraint assumes a spherical Earth, so it is only accurate to about
     a degree for observers in very low Earth orbit (height of 100 km).
     """
```

### Comparing `dorado-scheduling-0.1.0/dorado/scheduling/constraints/orbit_night.py` & `dorado_scheduling-0.2.0/dorado/scheduling/constraints/orbit_night.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright © 2020 United States Government as represented by the Administrator
+# Copyright © 2021 United States Government as represented by the Administrator
 # of the National Aeronautics and Space Administration. No copyright is claimed
 # in the United States under Title 17, U.S. Code. All Other Rights Reserved.
 #
 # SPDX-License-Identifier: NASA-1.3
 #
 from astropy.coordinates import get_sun
 from astropy import units as u
@@ -16,15 +16,15 @@
 
 class OrbitNightConstraint(EarthLimbConstraint):
     """
     Constrain the angle of the Sun from the Earth limb.
 
     Parameters
     ----------
-    min : `~astropy.units.Quantity`
+    min : :class:`astropy.units.Quantity`
         Minimum angle of the edge of the sun's disc from the Earth's limb.
 
     Notes
     -----
     This constraint assumes a spherical Earth, so it is only accurate to about
     a degree for observers in very low Earth orbit (height of 100 km).
     """
```

### Comparing `dorado-scheduling-0.1.0/dorado/scheduling/scripts/animate.py` & `dorado_scheduling-0.2.0/dorado/scheduling/scripts/animate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,89 +1,119 @@
 #
-# Copyright © 2020 United States Government as represented by the Administrator
+# Copyright © 2021 United States Government as represented by the Administrator
 # of the National Aeronautics and Space Administration. No copyright is claimed
 # in the United States under Title 17, U.S. Code. All Other Rights Reserved.
 #
 # SPDX-License-Identifier: NASA-1.3
 #
-"""Plot an observing plan."""
+"""Render an animation of an observing plan."""
 import logging
 
+from astropy import units as u
 from ligo.skymap.tool import ArgumentParser, FileType
 
+from .. import mission as _mission
+from ..units import equivalencies
+
 log = logging.getLogger(__name__)
 
 
 def parser():
-    p = ArgumentParser()
-    p.add_argument('skymap', metavar='FILE.fits[.gz]',
-                   type=FileType('rb'), help='Input sky map')
-    p.add_argument('schedule', metavar='SCHEDULE.ecsv',
-                   type=FileType('rb'), default='-',
-                   help='Schedule filename')
-    p.add_argument('output', metavar='MOVIE.gif', type=FileType('wb'),
-                   help='Output filename')
+    p = ArgumentParser(prog='dorado-scheduling-animate')
+
+    group = p.add_argument_group(
+        'problem setup options',
+        'Options that control the problem setup')
+    group.add_argument(
+        '--mission', choices=set(_mission.__all__) - {'Mission'},
+        default='dorado', help='Mission configuration')
+    group.add_argument(
+        '--delay', type=u.Quantity, default='30 min',
+        help='Delay after event time to start observing (any time units)')
+    group.add_argument(
+        '--duration', type=u.Quantity, default='1 orbit',
+        help='Duration of observing plan (any time units)')
+
+    group = p.add_argument_group(
+        'discretization options',
+        'Options that control the discretization of decision variables')
+    group.add_argument(
+        '--time-step', type=u.Quantity, default='1 min',
+        help='Model time step')
+
+    p.add_argument(
+        '--nside', type=int, default=32, help='HEALPix sampling resolution')
+    p.add_argument(
+        'skymap', metavar='FILE.fits[.gz]', type=FileType('rb'),
+        help='Input sky map')
+    p.add_argument(
+        'schedule', metavar='SCHEDULE.ecsv', type=FileType('rb'), default='-',
+        help='Schedule filename')
+    p.add_argument(
+        'output', metavar='MOVIE.gif', type=FileType('wb'),
+        help='Output filename')
+
     return p
 
 
 def main(args=None):
     args = parser().parse_args(args)
 
     # Late imports
-    from astropy_healpix import HEALPix, nside_to_level, npix_to_nside
+    from astropy.coordinates import ICRS
+    from astropy_healpix import HEALPix
     from astropy.io import fits
     from astropy.time import Time
     from astropy.table import QTable
-    from astropy import units as u
     from ligo.skymap.io import read_sky_map
     from ligo.skymap.bayestar import rasterize
     from ligo.skymap import plot
     from ligo.skymap.postprocess import find_greedy_credible_levels
     from matplotlib import pyplot as plt
     from matplotlib.animation import FuncAnimation, PillowWriter
     from matplotlib.ticker import FormatStrFormatter
     import numpy as np
     import seaborn
     from tqdm import tqdm
 
-    from .. import orbit
-    from .. import skygrid
-    from ..regard import get_field_of_regard
+    mission = getattr(_mission, args.mission)()
+    healpix = HEALPix(args.nside, order='nested', frame=ICRS())
 
     log.info('reading sky map')
 
     # Read multi-order sky map and rasterize to working resolution
     start_time = Time(fits.getval(args.skymap, 'DATE-OBS', ext=1))
     skymap = read_sky_map(args.skymap, moc=True)['UNIQ', 'PROBDENSITY']
     skymap_hires = rasterize(skymap)['PROB']
-    healpix_hires = HEALPix(npix_to_nside(len(skymap_hires)))
-    skymap = rasterize(skymap, nside_to_level(skygrid.healpix.nside))['PROB']
-    nest = skygrid.healpix.order == 'nested'
-    if not nest:
-        skymap = skymap[skygrid.healpix.ring_to_nested(np.arange(len(skymap)))]
-        skymap_hires = skymap[healpix_hires.ring_to_nested(np.arange(
-            len(skymap_hires)))]
+    skymap = rasterize(skymap, healpix.level)['PROB']
 
     cls = find_greedy_credible_levels(skymap_hires)
 
-    times = np.arange(orbit.time_steps) * orbit.time_step_duration + start_time
+    with u.add_enabled_equivalencies(equivalencies.orbital(mission.orbit)):
+        times = start_time + args.delay + np.arange(
+            0, args.duration.to_value(u.s),
+            args.time_step.to_value(u.s)) * u.s
 
     log.info('reading observing schedule')
     schedule = QTable.read(args.schedule.name, format='ascii.ecsv')
 
     log.info('calculating field of regard')
-    field_of_regard = get_field_of_regard(times)
+    field_of_regard = mission.get_field_of_regard(
+        healpix.healpix_to_skycoord(np.arange(healpix.npix)), times)
 
     orbit_field_of_regard = np.logical_or.reduce(field_of_regard)
-    # continuous_viewing_zone = np.logical_and.reduce(field_of_regard)
+    continuous_viewing_zone = np.logical_and.reduce(field_of_regard)
+    has_continuous_viewing_zone = np.any(continuous_viewing_zone)
 
     t = (times - times[0]).to(u.minute).value
 
-    instantaneous_color, orbit_color, _, skymap_color, _, footprint_color = \
-        seaborn.color_palette('Paired', n_colors=6)
+    (
+        instantaneous_color, orbit_color, continuous_color, skymap_color,
+        _, footprint_color
+    ) = seaborn.color_palette('Paired', n_colors=6)
 
     fig = plt.figure(figsize=(8, 8))
     gs_sky, gs_time, gs_prob = plt.GridSpec(
         3, 1, height_ratios=[2, 1, 1], hspace=0.1)
 
     ax_time = fig.add_subplot(gs_time)
     ax_time.set_xlim(t[0], t[-1])
@@ -94,82 +124,88 @@
     twin.set_ylim(0, 4 * 180**2 / np.pi * 1e-4)
     twin.set_ylabel('Area ($10^4$ deg$^2$)')
     plt.setp(ax_time.get_xticklabels(), visible=False)
 
     indices = np.asarray([], dtype=np.intp)
     prob = []
     for row in schedule:
-        new_indices = skygrid.get_footprint_healpix(row['center'], row['roll'])
+        new_indices = mission.fov.footprint_healpix(
+            healpix, row['center'], row['roll'])
         indices = np.unique(np.concatenate((indices, new_indices)))
         prob.append(100 * skymap[indices].sum())
 
     ax_prob = fig.add_subplot(gs_prob, sharex=ax_time, sharey=ax_time)
     start = (schedule['time'] - times[0]).to_value(u.minute).tolist()
     ax_prob.plot(
         [t[0] - 1] + start + [t[-1] + 1], [0] + prob + [100], '-o',
         drawstyle='steps-post', color='black')
     ax_prob.set_xlabel(f'Time since {start_time.iso} (minutes)')
     ax_prob.set_ylabel('Integrated prob.')
 
-    # y = continuous_viewing_zone.sum() / skygrid.healpix.npix * 100
-    # ax_time.axhline(
-    #     continuous_viewing_zone.sum() / skygrid.healpix.npix,
-    #     color=continuous_color, zorder=2.1)
+    if has_continuous_viewing_zone:
+        y = continuous_viewing_zone.sum() / healpix.npix * 100
+        ax_time.axhline(y, color=continuous_color, zorder=2.1)
 
-    y = field_of_regard.sum(1) / skygrid.healpix.npix * 100
+    y = field_of_regard.sum(1) / healpix.npix * 100
     ax_time.fill_between(
         t, y, np.repeat(100, len(y)), color=instantaneous_color, zorder=2.2)
 
-    y = orbit_field_of_regard.sum() / skygrid.healpix.npix * 100
+    y = orbit_field_of_regard.sum() / healpix.npix * 100
     ax_time.axhspan(y, 100, color=orbit_color, zorder=2.3)
 
     ax_sky = fig.add_subplot(gs_sky, projection='astro hours mollweide')
     ax_sky.grid()
+    colors = [continuous_color, orbit_color, instantaneous_color]
+    labels = ['Continuous', 'Orbit-averaged', 'Instantaneous']
+    if not has_continuous_viewing_zone:
+        colors = colors[1:]
+        labels = labels[1:]
     ax_sky.add_artist(ax_sky.legend(
         [plt.Rectangle((0, 0), 0, 0, edgecolor='none', facecolor=color)
-         for color in [orbit_color, instantaneous_color]],
-        ['Orbit-averaged', 'Instantaneous'], title='Outside field of regard',
+         for color in colors],
+        labels, title='Outside field of regard',
         bbox_to_anchor=[-0.05, -0.3, 1.1, 1.6], loc='upper right'))
     ax_sky.legend(
         [plt.Rectangle((0, 0), 0, 0, edgecolor=color, facecolor='none')
          for color in [skymap_color, footprint_color]],
         ['Localization', 'Observations'],
         bbox_to_anchor=[-0.05, -0.3, 1.1, 1.6], loc='upper left')
 
-    ax_sky.contour_hpx(cls, levels=[0.9], colors=[skymap_color], nested=nest)
-    # ax_sky.contourf_hpx(continuous_viewing_zone.astype(float),
-    #                     levels=[0, 0.5], colors=[continuous_color],
-    #                     nested=nest, zorder=0.4)
+    ax_sky.contour_hpx(cls, levels=[0.9], colors=[skymap_color], nested=True)
+    if has_continuous_viewing_zone:
+        ax_sky.contourf_hpx(continuous_viewing_zone.astype(float),
+                            levels=[0, 0.5], colors=[continuous_color],
+                            nested=True, zorder=0.3)
     ax_sky.contourf_hpx(orbit_field_of_regard.astype(float), levels=[0, 0.5],
-                        colors=[orbit_color], nested=nest, zorder=0.5)
+                        colors=[orbit_color], nested=True, zorder=0.5)
 
     old_artists = []
 
     log.info('rendering animation frames')
     with tqdm(total=len(field_of_regard)) as progress:
 
         def animate(i):
             for artist in old_artists:
                 artist.remove()
             del old_artists[:]
             for row in schedule:
                 if times[i] >= row['time']:
-                    poly = skygrid.get_footprint_polygon(
-                        row['center'], row['roll'])
+                    poly = mission.fov.footprint(
+                        row['center'], row['roll']).icrs
                     vertices = np.column_stack((poly.ra.rad, poly.dec.rad))
                     for cut_vertices in plot.cut_prime_meridian(vertices):
                         patch = plt.Polygon(
                             np.rad2deg(cut_vertices),
                             transform=ax_sky.get_transform('world'),
                             facecolor='none', edgecolor=footprint_color)
                         old_artists.append(ax_sky.add_patch(patch))
             old_artists.extend(ax_sky.contourf_hpx(
                 field_of_regard[i].astype(float), levels=[0, 0.5],
-                colors=[instantaneous_color], nested=nest,
-                zorder=0.2).collections)
+                colors=[instantaneous_color], nested=True,
+                zorder=0.4).collections)
             old_artists.append(ax_prob.axvline(t[i], color='gray', zorder=10))
             old_artists.append(ax_time.axvline(t[i], color='gray', zorder=10))
             progress.update()
 
         ani = FuncAnimation(fig, animate, frames=range(len(field_of_regard)))
         ani.save(args.output.name, writer=PillowWriter())
```

### Comparing `dorado-scheduling-0.1.0/dorado/scheduling/tests/test_earth_limb.py` & `dorado_scheduling-0.2.0/dorado/scheduling/tests/test_earth_limb.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 #
-# Copyright © 2020 United States Government as represented by the Administrator
+# Copyright © 2021 United States Government as represented by the Administrator
 # of the National Aeronautics and Space Administration. No copyright is claimed
 # in the United States under Title 17, U.S. Code. All Other Rights Reserved.
 #
 # SPDX-License-Identifier: NASA-1.3
 #
 from astroplan import FixedTarget, Observer
 from astropy.coordinates import EarthLocation, SkyCoord
 from astropy.time import Time
 from astropy import units as u
 from hypothesis import given, settings
 from hypothesis.strategies import floats
 
 from ..constraints.earth_limb import EarthLimbConstraint
 
+givens = given(
+    lon=floats(-180, 180, allow_subnormal=False),
+    lat=floats(-90, 90, allow_subnormal=False),
+    ra=floats(0, 360, allow_subnormal=False),
+    dec=floats(-90, 90, allow_subnormal=False),
+    time=floats(51544.5, 51909.75, allow_subnormal=False),
+    min=floats(-90, 90, allow_subnormal=False)
+)
 
-@given(lon=floats(-180, 180), lat=floats(-90, 90),
-       ra=floats(0, 360), dec=floats(-90, 90),
-       time=floats(51544.5, 51909.75), min=floats(-90, 90))
+
+@givens
 @settings(deadline=None)
 def test_observer_on_surface(lon, lat, ra, dec, time, min):
     """Test an obsever on the surface of the Earth."""
     obstime = Time(time, format='mjd')
     location = EarthLocation.from_geodetic(lon*u.deg, lat*u.deg)
     observer = Observer(location)
     target = FixedTarget(SkyCoord(ra*u.deg, dec*u.deg))
@@ -31,17 +38,15 @@
 
     if alt > (min + 1) * u.deg:
         assert observable
     elif alt < (min - 1) * u.deg:
         assert not observable
 
 
-@given(lon=floats(-180, 180), lat=floats(-90, 90),
-       ra=floats(0, 360), dec=floats(-90, 90),
-       time=floats(51544.5, 51909.75), min=floats(-90, 90))
+@givens
 @settings(deadline=None)
 def test_low_earth_orbit(lon, lat, ra, dec, time, min):
     """Test an observer in low Earth orbit."""
     obstime = Time(time, format='mjd')
     location = EarthLocation.from_geodetic(lon*u.deg, lat*u.deg, 550 * u.km)
     observer = Observer(location)
     target = FixedTarget(SkyCoord(ra*u.deg, dec*u.deg))
@@ -51,17 +56,15 @@
 
     if alt > (min - 22.5) * u.deg:
         assert observable
     elif alt < (min - 23.5) * u.deg:
         assert not observable
 
 
-@given(lon=floats(-180, 180), lat=floats(-90, 90),
-       ra=floats(0, 360), dec=floats(-90, 90),
-       time=floats(51544.5, 51909.75), min=floats(-90, 90))
+@givens
 @settings(deadline=None)
 def test_distant_obsever(lon, lat, ra, dec, time, min):
     """Test a very distant observer."""
     obstime = Time(time, format='mjd')
     location = EarthLocation.from_geodetic(lon*u.deg, lat*u.deg, 1*u.au)
     observer = Observer(location)
     target = FixedTarget(SkyCoord(ra*u.deg, dec*u.deg))
```

