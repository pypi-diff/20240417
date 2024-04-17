# Comparing `tmp/dsptoolbox-0.3.4.tar.gz` & `tmp/dsptoolbox-0.3.5.tar.gz`

## Comparing `dsptoolbox-0.3.4.tar` & `dsptoolbox-0.3.5.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/.gitattributes
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/.readthedocs.yaml
--rw-r--r--   0        0        0    17782 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/CHANGELOG.rst
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/requirements.txt
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/docs/Makefile
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/docs/__rdme.rst
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/docs/classes.rst
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/docs/conf.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/docs/index.rst
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/docs/make.bat
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/docs/modules.rst
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/docs/readme.rst
--rw-r--r--   0        0        0   262622 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/docs/logo/logo.png
--rw-r--r--   0        0        0   262793 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/docs/logo/logo2.png
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/docs/modules/dsptoolbox.audio_io.rst
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/docs/modules/dsptoolbox.beamforming.rst
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/docs/modules/dsptoolbox.distances.rst
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/docs/modules/dsptoolbox.effects.rst
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/docs/modules/dsptoolbox.filterbanks.rst
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/docs/modules/dsptoolbox.generators.rst
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/docs/modules/dsptoolbox.plots.rst
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/docs/modules/dsptoolbox.room_acoustics.rst
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/docs/modules/dsptoolbox.standard_functions.rst
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/docs/modules/dsptoolbox.transfer_functions.rst
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/docs/modules/dsptoolbox.transforms.rst
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/__init__.py
--rw-r--r--   0        0        0    36760 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/_general_helpers.py
--rw-r--r--   0        0        0    35393 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/_standard.py
--rw-r--r--   0        0        0    46331 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/standard_functions.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/audio_io/__init__.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/audio_io/_audio_io.py
--rw-r--r--   0        0        0    14939 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/audio_io/audio_io.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/beamforming/__init__.py
--rw-r--r--   0        0        0     9865 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/beamforming/_beamforming.py
--rw-r--r--   0        0        0    62886 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/beamforming/beamforming.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/classes/__init__.py
--rw-r--r--   0        0        0    20948 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/classes/_filter.py
--rw-r--r--   0        0        0    13843 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/classes/_lattice_ladder_filter.py
--rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/classes/_phaseLinearizer.py
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/classes/_plots.py
--rw-r--r--   0        0        0     8389 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/classes/_svfilter.py
--rw-r--r--   0        0        0    32846 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/classes/filter_class.py
--rw-r--r--   0        0        0    29479 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/classes/filterbank.py
--rw-r--r--   0        0        0    16030 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/classes/multibandsignal.py
--rw-r--r--   0        0        0    57438 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/classes/signal_class.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/distances/__init__.py
--rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/distances/_distances.py
--rw-r--r--   0        0        0    13049 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/distances/distances.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/effects/__init__.py
--rw-r--r--   0        0        0    18619 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/effects/_effects.py
--rw-r--r--   0        0        0    58609 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/effects/effects.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/filterbanks/__init__.py
--rw-r--r--   0        0        0    48939 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/filterbanks/_filterbank.py
--rw-r--r--   0        0        0    16152 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/filterbanks/filterbanks.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/generators/__init__.py
--rw-r--r--   0        0        0    18264 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/generators/generators.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/plots/__init__.py
--rw-r--r--   0        0        0    10165 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/plots/plots.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/room_acoustics/__init__.py
--rw-r--r--   0        0        0    43524 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/room_acoustics/_room_acoustics.py
--rw-r--r--   0        0        0    26111 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/room_acoustics/room_acoustics.py
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/transfer_functions/__init__.py
--rw-r--r--   0        0        0    10926 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/transfer_functions/_transfer_functions.py
--rw-r--r--   0        0        0    54061 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/transfer_functions/transfer_functions.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/transforms/__init__.py
--rw-r--r--   0        0        0    11056 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/transforms/_transforms.py
--rw-r--r--   0        0        0    29980 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/dsptoolbox/transforms/transforms.py
--rw-r--r--   0        0        0    46390 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/examples/audio_io_module.ipynb
--rw-r--r--   0        0        0   369566 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/examples/beamforming_module.ipynb
--rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/examples/distances_module.ipynb
--rw-r--r--   0        0        0   409017 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/examples/filterbanks_module.ipynb
--rw-r--r--   0        0        0  1013477 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/examples/general.ipynb
--rw-r--r--   0        0        0   244031 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/examples/generators_module.ipynb
--rw-r--r--   0        0        0   180489 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/examples/room_acoustics_module.ipynb
--rw-r--r--   0        0        0    94731 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/examples/standard_module.ipynb
--rw-r--r--   0        0        0   208870 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/examples/transfer_function_module.ipynb
--rw-r--r--   0        0        0  1248737 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/examples/transforms_module.ipynb
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/examples/data/array.xml
--rw-r--r--   0        0        0   384044 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/examples/data/chirp.wav
--rw-r--r--   0        0        0   384044 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/examples/data/chirp_mono.wav
--rw-r--r--   0        0        0   768044 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/examples/data/chirp_stereo.wav
--rw-r--r--   0        0        0  1766444 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/examples/data/fuer_elise.wav
--rw-r--r--   0        0        0    96044 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/examples/data/rir.wav
--rw-r--r--   0        0        0   187792 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/examples/data/speech.flac
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/tests/test_audio_io.py
--rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/tests/test_beamforming.py
--rw-r--r--   0        0        0    34160 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/tests/test_classes.py
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/tests/test_distances.py
--rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/tests/test_filterbanks.py
--rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/tests/test_fx.py
--rw-r--r--   0        0        0     7614 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/tests/test_generators.py
--rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/tests/test_room_acoustics.py
--rw-r--r--   0        0        0    12974 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/tests/test_standard.py
--rw-r--r--   0        0        0    17635 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/tests/test_transfer_functions.py
--rw-r--r--   0        0        0     5930 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/tests/test_transforms.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/LICENSE
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/README.rst
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 dsptoolbox-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/.gitattributes
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/.readthedocs.yaml
+-rw-r--r--   0        0        0    18324 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/CHANGELOG.rst
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/requirements.txt
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/Makefile
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/__rdme.rst
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/classes.rst
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/conf.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/index.rst
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/make.bat
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/modules.rst
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/readme.rst
+-rw-r--r--   0        0        0   262622 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/logo/logo.png
+-rw-r--r--   0        0        0   262793 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/logo/logo2.png
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/modules/dsptoolbox.audio_io.rst
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/modules/dsptoolbox.beamforming.rst
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/modules/dsptoolbox.distances.rst
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/modules/dsptoolbox.effects.rst
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/modules/dsptoolbox.filterbanks.rst
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/modules/dsptoolbox.generators.rst
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/modules/dsptoolbox.plots.rst
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/modules/dsptoolbox.room_acoustics.rst
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/modules/dsptoolbox.standard_functions.rst
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/modules/dsptoolbox.transfer_functions.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/docs/modules/dsptoolbox.transforms.rst
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/__init__.py
+-rw-r--r--   0        0        0    37498 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/_general_helpers.py
+-rw-r--r--   0        0        0    36355 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/_standard.py
+-rw-r--r--   0        0        0    46103 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/standard_functions.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/audio_io/__init__.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/audio_io/_audio_io.py
+-rw-r--r--   0        0        0    14939 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/audio_io/audio_io.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/beamforming/__init__.py
+-rw-r--r--   0        0        0     9865 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/beamforming/_beamforming.py
+-rw-r--r--   0        0        0    62886 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/beamforming/beamforming.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/classes/__init__.py
+-rw-r--r--   0        0        0    20948 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/classes/_filter.py
+-rw-r--r--   0        0        0    13843 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/classes/_lattice_ladder_filter.py
+-rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/classes/_phaseLinearizer.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/classes/_plots.py
+-rw-r--r--   0        0        0     8389 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/classes/_svfilter.py
+-rw-r--r--   0        0        0    32846 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/classes/filter_class.py
+-rw-r--r--   0        0        0    29479 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/classes/filterbank.py
+-rw-r--r--   0        0        0    16030 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/classes/multibandsignal.py
+-rw-r--r--   0        0        0    57889 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/classes/signal_class.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/distances/__init__.py
+-rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/distances/_distances.py
+-rw-r--r--   0        0        0    13049 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/distances/distances.py
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/effects/__init__.py
+-rw-r--r--   0        0        0    18619 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/effects/_effects.py
+-rw-r--r--   0        0        0    58609 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/effects/effects.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/filterbanks/__init__.py
+-rw-r--r--   0        0        0    48939 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/filterbanks/_filterbank.py
+-rw-r--r--   0        0        0    16152 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/filterbanks/filterbanks.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/generators/__init__.py
+-rw-r--r--   0        0        0    18264 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/generators/generators.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/plots/__init__.py
+-rw-r--r--   0        0        0    10165 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/plots/plots.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/room_acoustics/__init__.py
+-rw-r--r--   0        0        0    43582 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/room_acoustics/_room_acoustics.py
+-rw-r--r--   0        0        0    25842 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/room_acoustics/room_acoustics.py
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/transfer_functions/__init__.py
+-rw-r--r--   0        0        0    10926 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/transfer_functions/_transfer_functions.py
+-rw-r--r--   0        0        0    60900 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/transfer_functions/transfer_functions.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/transforms/__init__.py
+-rw-r--r--   0        0        0    11056 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/transforms/_transforms.py
+-rw-r--r--   0        0        0    30334 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/dsptoolbox/transforms/transforms.py
+-rw-r--r--   0        0        0    46390 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/audio_io_module.ipynb
+-rw-r--r--   0        0        0   369566 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/beamforming_module.ipynb
+-rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/distances_module.ipynb
+-rw-r--r--   0        0        0   409017 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/filterbanks_module.ipynb
+-rw-r--r--   0        0        0  1013477 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/general.ipynb
+-rw-r--r--   0        0        0   244031 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/generators_module.ipynb
+-rw-r--r--   0        0        0   180489 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/room_acoustics_module.ipynb
+-rw-r--r--   0        0        0    94731 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/standard_module.ipynb
+-rw-r--r--   0        0        0   208870 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/transfer_function_module.ipynb
+-rw-r--r--   0        0        0  1248737 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/transforms_module.ipynb
+-rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/data/array.xml
+-rw-r--r--   0        0        0   384044 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/data/chirp.wav
+-rw-r--r--   0        0        0   384044 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/data/chirp_mono.wav
+-rw-r--r--   0        0        0   768044 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/data/chirp_stereo.wav
+-rw-r--r--   0        0        0  1766444 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/data/fuer_elise.wav
+-rw-r--r--   0        0        0    96044 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/data/rir.wav
+-rw-r--r--   0        0        0   187792 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/examples/data/speech.flac
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/tests/test_audio_io.py
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/tests/test_beamforming.py
+-rw-r--r--   0        0        0    34170 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/tests/test_classes.py
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/tests/test_distances.py
+-rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/tests/test_filterbanks.py
+-rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/tests/test_fx.py
+-rw-r--r--   0        0        0     7614 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/tests/test_generators.py
+-rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/tests/test_room_acoustics.py
+-rw-r--r--   0        0        0    13083 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/tests/test_standard.py
+-rw-r--r--   0        0        0    17635 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/tests/test_transfer_functions.py
+-rw-r--r--   0        0        0     5930 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/tests/test_transforms.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/LICENSE
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/README.rst
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 dsptoolbox-0.3.5/PKG-INFO
```

### Comparing `dsptoolbox-0.3.4/.readthedocs.yaml` & `dsptoolbox-0.3.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/CHANGELOG.rst` & `dsptoolbox-0.3.5/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,34 @@
 
 `To Do's for future releases`_
 ------------------------------
 
 - Validation for results from tests in every module (so far many tests are
   only regarding functionality)
 
+`0.3.5 <https://pypi.org/project/dsptoolbox/0.3.5>`_ - 
+---------------------
+
+Added
+~~~~~~~
+- `harmonic_distortion_analysis` in ``transfer_functions``
+- added possibility of scaling the spectrogram
+- calibration using any dBSPL value
+
+Bugfix
+~~~~~~~
+- `reverb_time` now uses indices of peaks instead of -20 dBFS threshold since
+  it delivers more accurate results
+- now scaling a spectrum of a signal with a window is done correctly (taking
+  the window into account)
+
+Misc
+~~~~~~
+- general documentation and small performance improvements
+
 `0.3.4 <https://pypi.org/project/dsptoolbox/0.3.4>`_ - 
 ---------------------
 
 Added
 ~~~~~~~
 - added support for `MultiBandSignal` in `hilbert` in module ``transforms``
 - plot momentary spl added in `Signal`
```

### Comparing `dsptoolbox-0.3.4/docs/Makefile` & `dsptoolbox-0.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/docs/classes.rst` & `dsptoolbox-0.3.5/docs/classes.rst`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/docs/conf.py` & `dsptoolbox-0.3.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/docs/index.rst` & `dsptoolbox-0.3.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/docs/make.bat` & `dsptoolbox-0.3.5/docs/make.bat`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-@ECHO OFF
-
-pushd %~dp0
-
-REM Command file for Sphinx documentation
-
-if "%SPHINXBUILD%" == "" (
-	set SPHINXBUILD=python -msphinx
-)
-set SOURCEDIR=.
-set BUILDDIR=_build
-set SPHINXPROJ=dsptools
-
-%SPHINXBUILD% >NUL 2>NUL
-if errorlevel 9009 (
-	echo.
-	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
-	echo.installed, then set the SPHINXBUILD environment variable to point
-	echo.to the full path of the 'sphinx-build' executable. Alternatively you
-	echo.may add the Sphinx directory to PATH.
-	echo.
-	echo.If you don't have Sphinx installed, grab it from
-	echo.https://www.sphinx-doc.org/
-	exit /b 1
-)
-
-if "%1" == "" goto help
-
-%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
-goto end
-
-:help
-%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
-
-:end
-popd
+@ECHO OFF
+
+pushd %~dp0
+
+REM Command file for Sphinx documentation
+
+if "%SPHINXBUILD%" == "" (
+	set SPHINXBUILD=python -msphinx
+)
+set SOURCEDIR=.
+set BUILDDIR=_build
+set SPHINXPROJ=dsptools
+
+%SPHINXBUILD% >NUL 2>NUL
+if errorlevel 9009 (
+	echo.
+	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
+	echo.installed, then set the SPHINXBUILD environment variable to point
+	echo.to the full path of the 'sphinx-build' executable. Alternatively you
+	echo.may add the Sphinx directory to PATH.
+	echo.
+	echo.If you don't have Sphinx installed, grab it from
+	echo.https://www.sphinx-doc.org/
+	exit /b 1
+)
+
+if "%1" == "" goto help
+
+%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
+goto end
+
+:help
+%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
+
+:end
+popd
```

### Comparing `dsptoolbox-0.3.4/docs/modules.rst` & `dsptoolbox-0.3.5/docs/modules.rst`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/docs/readme.rst` & `dsptoolbox-0.3.5/docs/readme.rst`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/docs/logo/logo.png` & `dsptoolbox-0.3.5/docs/logo/logo.png`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/docs/logo/logo2.png` & `dsptoolbox-0.3.5/docs/logo/logo2.png`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/__init__.py` & `dsptoolbox-0.3.5/dsptoolbox/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,8 +69,8 @@
     "filterbanks",
     "transforms",
     "audio_io",
     "beamforming",
     "effects",
 ]
 
-__version__ = "0.3.4"
+__version__ = "0.3.5"
```

### Comparing `dsptoolbox-0.3.4/dsptoolbox/_general_helpers.py` & `dsptoolbox-0.3.5/dsptoolbox/_general_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         window_full = 1 - window_full
     return window_full
 
 
 def _get_normalized_spectrum(
     f,
     spectra: np.ndarray,
-    mode="standard",
+    scaling: str = "amplitude",
     f_range_hz=[20, 20000],
     normalize: str | None = None,
     smoothe: int = 0,
     phase=False,
     calibrated_data: bool = False,
 ) -> tuple[np.ndarray, np.ndarray] | tuple[np.ndarray, np.ndarray, np.ndarray]:
     """This function gives a normalized magnitude spectrum in dB with frequency
@@ -119,30 +119,31 @@
 
     Parameters
     ----------
     f : `np.ndarray`
         Frequency vector.
     spectra : `np.ndarray`
         Spectrum matrix.
-    mode : str, optional
-        Mode of spectrum, needed for factor in dB respresentation.
-        Choose from `'standard'` or `'welch'`. Default: `'standard'`.
+    scaling : str, optional
+        Information about whether the spectrum is scaled as an amplitude or
+        power. Choose from `'amplitude'` or `'power'`. Default: `'amplitude'`.
     f_range_hz : array-like with length 2
         Range of frequencies to get the normalized spectrum back.
         Default: [20, 20e3].
     normalize : str, optional
         Normalize spectrum (per channel). Choose from `'1k'` (for 1 kHz),
         `'max'` (maximum value) or `None` for no normalization. The
         normalization for 1 kHz uses a linear interpolation for getting the
         value at 1 kHz regardless of the frequency resolution. Default: `None`.
     smoothe : int, optional
         1/smoothe-fractional octave band smoothing for magnitude spectra. Pass
         `0` for no smoothing. Default: 0.
     phase : bool, optional
-        When `True`, phase spectra are also returned. Default: `False`.
+        When `True`, phase spectra are also returned. Smoothing is also
+        applied to the unwrapped phase. Default: `False`.
     calibrated_data : bool, optional
         When `True`, it is assumed that the time data has been calibrated
         to be in Pascal so that it is scaled by p0=20e-6 Pa. Default: `False`.
 
     Returns
     -------
     f : `np.ndarray`
@@ -172,23 +173,24 @@
     # Check for complex spectrum if phase is required
     if phase:
         assert np.iscomplexobj(spectra), (
             "Phase computation is not "
             + "possible since the spectra are not complex"
         )
     # Factor
-    if mode == "standard":
+    if scaling == "amplitude":
         scale_factor = 20e-6 if calibrated_data and normalize is None else 1
         factor = 20
-    elif mode == "welch":
+    elif scaling == "power":
         scale_factor = 4e-10 if calibrated_data and normalize is None else 1
         factor = 10
     else:
         raise ValueError(
-            f"{mode} is not supported. Please select standard " "or welch"
+            f"{scaling} is not supported. Please select amplitude or "
+            + "power scaling"
         )
 
     if f_range_hz is not None:
         assert len(f_range_hz) == 2, (
             "Frequency range must have only " + "a lower and an upper bound"
         )
         f_range_hz = np.sort(f_range_hz)
@@ -200,32 +202,31 @@
         id2 = len(f)
 
     spectra = spectra[id1:id2]
     f = f[id1:id2]
 
     mag_spectra = np.abs(spectra)
 
-    if smoothe != 0 and mode == "standard":
-        if mode == "standard":
+    if smoothe != 0:
+        if scaling == "amplitude":
             mag_spectra = _fractional_octave_smoothing(mag_spectra, smoothe)
-        else:  # Welch
+        else:  # Smoothing always in amplitude representation
             mag_spectra = (
                 _fractional_octave_smoothing(mag_spectra**0.5, smoothe) ** 2
             )
 
-    epsilon = 10 ** (-400 / 10)
+    epsilon = 10 ** (-800 / 10)
     mag_spectra = factor * np.log10(
         np.clip(mag_spectra, a_min=epsilon, a_max=None) / scale_factor
     )
 
     if normalize is not None:
         for i in range(spectra.shape[1]):
             if normalize == "1k":
-                gain = _get_exact_gain_1khz(f, mag_spectra[:, i])
-                mag_spectra[:, i] -= gain
+                mag_spectra[:, i] -= _get_exact_gain_1khz(f, mag_spectra[:, i])
             else:
                 mag_spectra[:, i] -= np.max(mag_spectra[:, i])
 
     if phase:
         phase_spectra = np.angle(spectra)
         if smoothe != 0:
             phase_spectra = _wrap_phase(
@@ -1068,14 +1069,15 @@
 
 
 def _scale_spectrum(
     spectrum: np.ndarray,
     mode: str | None,
     time_length_samples: int,
     sampling_rate_hz: int,
+    window: np.ndarray | None = None,
 ) -> np.ndarray:
     """Scale the spectrum directly from the (unscaled) FFT. It is assumed that
     the time data was not windowed.
 
     Parameters
     ----------
     spectrum : `np.ndarray`
@@ -1091,14 +1093,21 @@
         Sampling rate.
 
     Returns
     -------
     `np.ndarray`
         Scaled spectrum
 
+    Notes
+    -----
+    - The amplitude spectrum shows the RMS value of each frequency in the
+      signal.
+    - Integrating the power spectral density over the frequency spectrum
+      delivers the total energy contained in the signal (parseval's theorem).
+
     """
     assert time_length_samples in (
         (spectrum.shape[0] - 1) * 2,
         spectrum.shape[0] * 2 - 1,
     ), "Time length does not match"
 
     if mode is None:
@@ -1109,24 +1118,31 @@
         "amplitude spectral density",
         "amplitude spectrum",
         "power spectral density",
         "power spectrum",
     ), f"{mode} is not a supported mode"
 
     if "spectral density" in mode:
-        factor = (1 / time_length_samples / sampling_rate_hz) ** 0.5
+        if window is None:
+            factor = (2 / time_length_samples / sampling_rate_hz) ** 0.5
+        else:
+            factor = (
+                2 / np.sum(window**2, axis=0, keepdims=True) / sampling_rate_hz
+            ) ** 0.5
     elif "spectrum" in mode:
-        factor = 1 / time_length_samples
+        if window is None:
+            factor = 2**0.5 / time_length_samples
+        else:
+            factor = 2**0.5 / np.sum(window, axis=0, keepdims=True)
 
     spectrum *= factor
 
+    spectrum[0] /= 2**0.5
     if time_length_samples % 2 == 0:
-        spectrum[1:-1] *= 2**0.5
-    else:
-        spectrum[1:] *= 2**0.5
+        spectrum[-1] /= 2**0.5
 
     if "power" in mode:
         spectrum = np.abs(spectrum) ** 2
 
     return spectrum
 
 
@@ -1150,32 +1166,32 @@
     latency_samples : `np.ndarray`
         Latency of impulses (in samples). It has shape (channels).
 
     """
     n_channels = time_data.shape[1]
     delay_samples = np.argmax(np.abs(time_data), axis=0).astype(int)
 
-    # Take only the part of the time vector with the impulses and some safety
-    # samples
+    # Take only the part of the time vector with the peaks and some safety
+    # samples (±200)
     time_data = time_data[: np.max(delay_samples) + 200, :]
+    start_offset = max(np.min(delay_samples) - 200, 0)
+    time_data = time_data[start_offset:, :]
+    delay_samples -= start_offset
 
-    h = hilbert(time_data, axis=0)
+    h = hilbert(time_data, axis=0).imag
     x = np.arange(-polynomial_points + 1, polynomial_points + 1)
 
     latency_samples = np.zeros(n_channels)
 
     for ch in range(n_channels):
         # ===== Ensure that delay_samples is before the peak in each channel
-        selection = h[delay_samples[ch] : delay_samples[ch] + 2, ch].imag
+        selection = h[delay_samples[ch] : delay_samples[ch] + 2, ch]
         move_back_one_sample = selection[0] * selection[1] > 0
         delay_samples[ch] -= int(move_back_one_sample)
-        if (
-            h[delay_samples[ch], ch].imag * h[delay_samples[ch] + 1, ch].imag
-            > 0
-        ):
+        if h[delay_samples[ch], ch] * h[delay_samples[ch] + 1, ch] > 0:
             latency_samples[ch] = delay_samples[ch] + int(move_back_one_sample)
             warn(
                 f"Fractional latency detection failed for channel {ch}. "
                 + "Integer latency is"
                 + " returned"
             )
             continue
@@ -1187,24 +1203,24 @@
             h[
                 delay_samples[ch]
                 - polynomial_points
                 + 1 : delay_samples[ch]
                 + polynomial_points
                 + 1,
                 ch,
-            ].imag,
+            ],
             deg=2 * polynomial_points - 1,
         )
 
-        # Find root and check it is less than one
-        roots = np.roots(pol).squeeze()
+        # Find roots
+        roots = np.roots(pol)
         # Get only root between 0 and 1
         roots = roots[
             (roots == roots.real)  # Real roots
-            & (roots <= 1 + 1e-10)  # Range
+            & (roots <= 1)  # Range
             & (roots >= 0)
         ].real
         try:
             fractional_delay_samples = roots[0]
         except IndexError as e:
             print(e)
             warn(
@@ -1212,15 +1228,15 @@
                 + "Integer latency is"
                 + " returned"
             )
             latency_samples[ch] = delay_samples[ch] + int(move_back_one_sample)
             continue
 
         latency_samples[ch] = delay_samples[ch] + fractional_delay_samples
-    return latency_samples
+    return latency_samples + start_offset
 
 
 def _remove_impulse_delay_from_phase(
     freqs: np.ndarray,
     phase: np.ndarray,
     time_data: np.ndarray,
     sampling_rate_hz: int,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dsptoolbox-0.3.4/dsptoolbox/_standard.py` & `dsptoolbox-0.3.5/dsptoolbox/_standard.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,37 +5,38 @@
 import numpy as np
 from scipy.signal import correlate, check_COLA, windows, hilbert, convolve
 from scipy.special import iv as bessel_first_mod
 from ._general_helpers import (
     _pad_trim,
     _compute_number_frames,
     _get_fractional_impulse_peak_index,
+    _wrap_phase,
 )
 from warnings import warn
 
 
 def _latency(
     in1: np.ndarray, in2: np.ndarray | None = None, polynomial_points: int = 0
 ):
     """Computes the latency between two functions using the correlation method.
     The variable polynomial_points is only a dummy to share the same function
     signature as the `_fractional_latency` function.
 
     """
     if in2 is None:
-        in2 = np.repeat(in1[:, 0][..., None], in1.shape[1] - 1, axis=1)
+        in2 = in1[:, 0][..., None]
         in1 = np.atleast_2d(in1[:, 1:])
-
-    latency_per_channel_samples = np.zeros(in1.shape[1], dtype=int)
-    for i in range(in1.shape[1]):
-        xcorr = correlate(in2[:, i].flatten(), in1[:, i].flatten())
-        latency_per_channel_samples[i] = int(
-            in1.shape[0] - np.argmax(np.abs(xcorr)) - 1
-        )
-    return latency_per_channel_samples
+        xcorr = correlate(in2, in1, mode="full")
+        peak_inds = np.argmax(np.abs(xcorr), axis=0)
+    else:
+        peak_inds = np.zeros(in1.shape[1], dtype=int)
+        for i in range(in1.shape[1]):
+            xcorr = correlate(in2[:, i].flatten(), in1[:, i].flatten())
+            peak_inds[i] = int(np.argmax(np.abs(xcorr)))
+    return in1.shape[0] - peak_inds - 1
 
 
 def _fractional_latency(
     td1: np.ndarray, td2: np.ndarray | None = None, polynomial_points: int = 1
 ):
     """This function computes the sub-sample latency between two signals using
     Zero-Crossing of the analytic (hilbert transformed) correlation function.
@@ -351,28 +352,28 @@
             )
 
     minimum_phase = -np.imag(
         hilbert(np.log(np.clip(magnitude, a_min=1e-40, a_max=None)), axis=0)
     )[:original_length]
 
     if not unwrapped:
-        minimum_phase = np.angle(np.exp(1j * minimum_phase))
+        minimum_phase = _wrap_phase(minimum_phase)
     return minimum_phase
 
 
 def _stft(
     x: np.ndarray,
     fs_hz: int,
     window_length_samples: int = 2048,
     window_type: str = "hann",
     overlap_percent=50,
     fft_length_samples: int | None = None,
     detrend: bool = True,
     padding: bool = False,
-    scaling: bool = False,
+    scaling: str | None = None,
 ):
     """Computes the STFT of a signal. Output matrix has (freqs_hz, seconds_s).
 
     Parameters
     ----------
     x : `np.ndarray`
         First signal
@@ -392,17 +393,18 @@
         `None` to use the window length. Default: `None`.
     detrend : bool, optional
         Detrending from each time segment (removing mean). Default: True.
     padding : bool, optional
         When `True`, the original signal is padded in the beginning and ending
         so that no energy is lost due to windowing when the COLA constraint is
         met. Default: `False`.
-    scaling : bool, optional
-        When `True`, the output is scaled as an amplitude spectrum, otherwise
-        no scaling is applied. See references for details. Default: `False`.
+    scaling : str, optional
+        Scale as `"amplitude spectrum"`, `"amplitude spectral density"`,
+        `"power spectrum"` or `"power spectral density"`. Pass `None`
+        to avoid any scaling. See references for details. Default: `None`.
 
     Returns
     -------
     time_s : `np.ndarray`
         Time vector in seconds for each frame.
     freqs_hz : `np.ndarray`
         Frequency vector.
@@ -420,20 +422,38 @@
     assert window_length_samples in valid_window_sizes, (
         "Window length should be a power of 2 between [16, 65536] or "
         + "[2**4, 2**16]"
     )
     assert overlap_percent >= 0 and overlap_percent < 100, (
         "overlap_percent" + " should be between 0 and 100"
     )
+    valid_scaling = [
+        "power spectrum",
+        "power spectral density",
+        "amplitude spectrum",
+        "amplitude spectral density",
+        None,
+    ]
+    assert scaling in valid_scaling, (
+        f"{scaling} is not valid. Use "
+        + "power spectrum, power spectral density, amplitude spectrum, "
+        + "amplitude spectral density or None"
+    )
+
+    if scaling is None:
+        scaling = ""
+
+    if fft_length_samples is None:
+        fft_length_samples = window_length_samples
 
     # Window and step
     window = windows.get_window(
         window_type, window_length_samples, fftbins=True
     )
-    overlap_samples = int(overlap_percent / 100 * window_length_samples)
+    overlap_samples = int(overlap_percent / 100 * window_length_samples + 0.5)
     step = window_length_samples - overlap_samples
 
     # Check COLA
     if not check_COLA(window, nperseg=len(window), noverlap=overlap_samples):
         warn(
             "Selected window type and overlap do not meet the constant "
             + "overlap and add constraint! Results might be distorted"
@@ -448,20 +468,32 @@
     time_x *= window[..., np.newaxis, np.newaxis]
     # Detrend
     if detrend:
         time_x -= np.mean(time_x, axis=0)
     # Spectra
     stft = np.fft.rfft(time_x, axis=0, n=fft_length_samples)
     # Scaling
-    if scaling:
-        factor = np.sqrt(2 / np.sum(window) ** 2)
+    if scaling in ("power spectrum", "amplitude spectrum"):
+        factor = 2**0.5 / np.sum(window)
+    elif scaling in ("power spectral density", "amplitude spectral density"):
+        factor = (2 / (window @ window) / fs_hz) ** 0.5
     else:
         factor = 1
+
     stft *= factor
 
+    if scaling:
+        stft[0, ...] /= 2**0.5
+
+    if scaling and fft_length_samples % 2 == 0:
+        stft[-1, ...] /= 2**0.5
+
+    if "power" in scaling:
+        stft = np.abs(stft) ** 2
+
     time_s = np.linspace(0, len(x) / fs_hz, stft.shape[1])
     freqs_hz = np.fft.rfftfreq(len(window), 1 / fs_hz)
     return time_s, freqs_hz, stft
 
 
 def _csm(
     time_data: np.ndarray,
```

### Comparing `dsptoolbox-0.3.4/dsptoolbox/standard_functions.py` & `dsptoolbox-0.3.5/dsptoolbox/standard_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1042,29 +1042,30 @@
     to calibrate other signals.
 
     """
 
     def __init__(
         self,
         calibration_data,
-        type_of_calibration: str = "94db",
+        calibration_spl_db: float = 94,
         high_snr: bool = True,
     ):
         """Load a calibration sound file. It is expected that it contains
-        a recorded harmonic tone of 1 kHz with either 94 dB or 114 dB SPL
-        according to [1]. This class can later be used to calibrate a signal.
+        a recorded harmonic tone of 1 kHz with the given dB(SPL) value, common
+        values are 94 dB or 114 dB SPL according to [1]. This class can later
+        be used to calibrate a signal.
 
         Parameters
         ----------
         calibration_data : str, tuple or `Signal`
             Calibration recording. It can be a path (str), a tuple with entries
             (time_data, sampling_rate) or a `Signal` object.
-        type_of_calibration : {'94db', '114db'} str, optional
-            Type of calibration data. It must be either `'94db'` or `'114db'`.
-            Default: `'94db'`.
+        calibration_spl_db : float, optional
+            dB(SPL) of calibration data. Typical values are 94 dB (1 Pa) or 114
+            dB (10 Pa). Default: 94.
         high_snr : bool, optional
             If the calibration is expected to have a high Signal-to-noise
             ratio, RMS value is computed directly through the time signal. This
             is done when set to `True`. If not, it might be more precise to
             take the spectrum of the signal and evaluate it at 1 kHz.
             This is recommended for systems where the SNR drops below 10 dB.
             Default: `True`.
@@ -1085,22 +1086,15 @@
             pass
         else:
             raise TypeError(
                 f"{type(calibration_data)} is not a valid type. Use "
                 "either str, tuple or Signal"
             )
         self.calibration_signal = calibration_data
-
-        type_of_calibration = type_of_calibration.lower()
-        assert type_of_calibration in (
-            "94db",
-            "114db",
-        ), f"{type_of_calibration} is not valid. Use 94db or 114db"
-        self.calibration_type = type_of_calibration
-
+        self.calibration_spl_db = calibration_spl_db
         self.high_snr = high_snr
         # State tracker
         self.__update = True
 
     def add_calibration_channel(self, new_channel):
         """Adds a new calibration channel to the calibration signal.
 
@@ -1135,17 +1129,16 @@
     def _compute_calibration_factors(self):
         """Computes the calibration factors for each channel."""
         if self.__update:
             if self.high_snr:
                 rms_channels = rms(self.calibration_signal, in_dbfs=False)
             else:
                 rms_channels = self._get_rms_from_spectrum()
-            factor = 94 if self.calibration_type == "94db" else 114
             p0 = 20e-6
-            p_analytical = 10 ** (factor / 20) * p0
+            p_analytical = 10 ** (self.calibration_spl_db / 20) * p0
             self.calibration_factors = p_analytical / rms_channels
             self.__update = False
 
     def _get_rms_from_spectrum(self):
         self.calibration_signal.set_spectrum_parameters(
             method="standard", scaling="amplitude spectrum"
         )
```

### Comparing `dsptoolbox-0.3.4/dsptoolbox/audio_io/__init__.py` & `dsptoolbox-0.3.5/dsptoolbox/audio_io/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/audio_io/_audio_io.py` & `dsptoolbox-0.3.5/dsptoolbox/audio_io/_audio_io.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/audio_io/audio_io.py` & `dsptoolbox-0.3.5/dsptoolbox/audio_io/audio_io.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/beamforming/__init__.py` & `dsptoolbox-0.3.5/dsptoolbox/beamforming/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/beamforming/_beamforming.py` & `dsptoolbox-0.3.5/dsptoolbox/beamforming/_beamforming.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/beamforming/beamforming.py` & `dsptoolbox-0.3.5/dsptoolbox/beamforming/beamforming.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/classes/__init__.py` & `dsptoolbox-0.3.5/dsptoolbox/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/classes/_filter.py` & `dsptoolbox-0.3.5/dsptoolbox/classes/_filter.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/classes/_lattice_ladder_filter.py` & `dsptoolbox-0.3.5/dsptoolbox/classes/_lattice_ladder_filter.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/classes/_phaseLinearizer.py` & `dsptoolbox-0.3.5/dsptoolbox/classes/_phaseLinearizer.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/classes/_plots.py` & `dsptoolbox-0.3.5/dsptoolbox/classes/_plots.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/classes/_svfilter.py` & `dsptoolbox-0.3.5/dsptoolbox/classes/_svfilter.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/classes/filter_class.py` & `dsptoolbox-0.3.5/dsptoolbox/classes/filter_class.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/classes/filterbank.py` & `dsptoolbox-0.3.5/dsptoolbox/classes/filterbank.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/classes/multibandsignal.py` & `dsptoolbox-0.3.5/dsptoolbox/classes/multibandsignal.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/classes/signal_class.py` & `dsptoolbox-0.3.5/dsptoolbox/classes/signal_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -508,15 +508,15 @@
         self,
         window_length_samples: int = 1024,
         window_type: str = "hann",
         overlap_percent=50,
         fft_length_samples: int | None = None,
         detrend: bool = False,
         padding: bool = True,
-        scaling: bool = False,
+        scaling: str | None = None,
     ):
         """Sets all necessary parameters for the computation of the
         spectrogram.
 
         Parameters
         ----------
         window_length_samples : int, optional
@@ -531,18 +531,18 @@
             `None` to use the window length. Default: `None`.
         detrend : bool, optional
             Detrending (subtracting mean) for each time frame.
             Default: `False`.
         padding : bool, optional
             Padding signal in the beginning and end to center it in order
             to avoid losing energy because of windowing. Default: `True`.
-        scaling : bool, optional
-            When `True`, the output is scaled as an amplitude spectrum,
-            otherwise no scaling is applied. See references for details.
-            Default: `False`.
+        scaling : str, optional
+            Scale as `"amplitude spectrum"`, `"amplitude spectral density"`,
+            `"power spectrum"` or `"power spectral density"`. Pass `None`
+            to avoid any scaling. See references for details. Default: `None`.
 
         References
         ----------
         - Heinzel, G., Rüdiger, A., & Schilling, R. (2002). Spectrum and
           spectral density estimation by the Discrete Fourier transform (DFT),
           including a comprehensive list of window functions and some new
           at-top windows.
@@ -640,14 +640,18 @@
                     f"{new_time_data.shape[0]} does not match "
                     + f"{self.time_data.shape[0]}. Activate padding_trimming "
                     + "for allowing this channel to be added"
                 )
         self.time_data = np.concatenate(
             [self.time_data, new_time_data], axis=1
         )
+        if hasattr(self, "window"):
+            self.window = np.concatenate(
+                [self.window, np.ones(new_time_data.shape)], axis=1
+            )
         self.__update_state()
 
     def remove_channel(self, channel_number: int = -1):
         """Removes a channel.
 
         Parameters
         ----------
@@ -796,14 +800,15 @@
                 # Length of signal for frequency vector and scaling
                 time_length = self.time_data.shape[0]
                 spectrum = _scale_spectrum(
                     spectrum,
                     self._spectrum_parameters["scaling"],
                     time_length,
                     self.sampling_rate_hz,
+                    None if not hasattr(self, "window") else self.window,
                 )
 
             self.spectrum = []
             self.spectrum.append(
                 np.fft.rfftfreq(time_length, 1 / self.sampling_rate_hz)
             )
             self.spectrum.append(spectrum)
@@ -966,27 +971,23 @@
         self._spectrum_parameters["smoothe"] = 0
 
         # Get spectrum
         f, sp = self.get_spectrum()
 
         self._spectrum_parameters["smoothe"] = prior_smoothing
 
-        if self._spectrum_parameters["scaling"] is not None:
-            mode = (
-                "welch"
-                if "power" in self._spectrum_parameters["scaling"]
-                else "standard"
-            )
-        else:
-            mode = self._spectrum_parameters["method"]
-
+        scaling = (
+            "amplitude"
+            if self._spectrum_parameters["scaling"] is None
+            else self._spectrum_parameters["scaling"]
+        )
         f, mag_db = _get_normalized_spectrum(
             f=f,
             spectra=sp,
-            mode=mode,
+            scaling=("amplitude" if "amplitude" in scaling else "power"),
             f_range_hz=range_hz,
             normalize=normalize,
             smoothe=smoothe,
             calibrated_data=self.calibrated_signal,
         )
         if show_info_box:
             txt = "Info"
@@ -1301,20 +1302,31 @@
         stft = stft[:, :, channel_number]
 
         ids = _find_nearest([20, 20000], f)
         if ids[0] == 0:
             ids[0] += 1
         f = f[ids[0] : ids[1]]
         stft = stft[ids[0] : ids[1], :]
-        stft_db = 20 * np.log10(np.clip(np.abs(stft), 1e-20, None))
-        stft_db = np.nan_to_num(stft_db, nan=np.min(stft_db))
+
         if self._spectrogram_parameters["scaling"]:
-            zlabel = "dB (Pa$^2$/Hz)"
+            if "power" in self._spectrogram_parameters["scaling"]:
+                factor = 10
+            else:
+                factor = 20
         else:
-            zlabel = "dB (No Scaling)"
+            factor = 20
+            zlabel = "dBFS"
+
+        stft_db = factor * np.log10(np.clip(np.abs(stft), 1e-30, None))
+
+        if self.calibrated_signal:
+            stft_db -= 20 * np.log10(2e-5)
+            zlabel = "dB"
+
+        stft_db = np.nan_to_num(stft_db, nan=np.min(stft_db))
         fig, ax = general_matrix_plot(
             matrix=stft_db,
             range_x=(t[0], t[-1]),
             range_y=(f[0], f[-1]),
             range_z=np.abs(dynamic_range_db),
             xlabel="Time / s",
             ylabel="Frequency / Hz",
```

### Comparing `dsptoolbox-0.3.4/dsptoolbox/distances/_distances.py` & `dsptoolbox-0.3.5/dsptoolbox/distances/_distances.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/distances/distances.py` & `dsptoolbox-0.3.5/dsptoolbox/distances/distances.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/effects/__init__.py` & `dsptoolbox-0.3.5/dsptoolbox/effects/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/effects/_effects.py` & `dsptoolbox-0.3.5/dsptoolbox/effects/_effects.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/effects/effects.py` & `dsptoolbox-0.3.5/dsptoolbox/effects/effects.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/filterbanks/__init__.py` & `dsptoolbox-0.3.5/dsptoolbox/filterbanks/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/filterbanks/_filterbank.py` & `dsptoolbox-0.3.5/dsptoolbox/filterbanks/_filterbank.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/filterbanks/filterbanks.py` & `dsptoolbox-0.3.5/dsptoolbox/filterbanks/filterbanks.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/generators/generators.py` & `dsptoolbox-0.3.5/dsptoolbox/generators/generators.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/plots/plots.py` & `dsptoolbox-0.3.5/dsptoolbox/plots/plots.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/room_acoustics/__init__.py` & `dsptoolbox-0.3.5/dsptoolbox/room_acoustics/__init__.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/room_acoustics/_room_acoustics.py` & `dsptoolbox-0.3.5/dsptoolbox/room_acoustics/_room_acoustics.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     ----------
     Regarding start of RIR: ISO 3382-1:2009-10, Acoustics - Measurement of
     the reverberation time of rooms with reference to other
     acoustical parameters. pp. 22.
 
     """
     if ir_start is None:
-        max_ind = _find_ir_start(h, threshold_dbfs=-20)
+        max_ind = np.argmax(np.abs(h))
     else:
         max_ind = ir_start
 
     edc = _compute_energy_decay_curve(h, max_ind, automatic_trimming, fs_hz)
     time_vector = np.linspace(0, len(edc) / fs_hz, len(edc))
 
     # Reverb
@@ -1206,14 +1206,21 @@
     the smooth (exponential) envelope of the energy time curve. First, a
     threshold is defined as the median of the trailing part of the RIR. Then
     non-overlapping windows are checked, so that the first window to grow its
     average energy after the impulse is taken as the end.
 
     This function returns the start and stop indices relative to the original
     time data, but the impulse index relative to the new vector.
+
+    Returns
+    -------
+    start : int
+    stop : int
+    impulse : int
+
     """
     # Envelope
     envelope = np.abs(hilbert(time_data, axis=0))
 
     # Start index
     impulse_index = int(np.argmax(envelope))
     offset_start_samples = int(offset_start_s * fs_hz + 0.5)
```

### Comparing `dsptoolbox-0.3.4/dsptoolbox/room_acoustics/room_acoustics.py` & `dsptoolbox-0.3.5/dsptoolbox/room_acoustics/room_acoustics.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,24 +39,20 @@
     mode : str, optional
         Reverberation time mode. Options are `'Topt'`, `'T20'`, `'T30'`,
         `'T60'` or `'EDT'`. Default: `'Topt'`.
     ir_start : int or array-like, optional
         If it is an integer, it is assumed as the start of the IR for all
         channels (and all bands). For more specific cases, pass a 1d-array
         containing the start indices for each channel or a 2d-array with
-        shape (band, channel) for a `MultiBandSignal`. When `None`, the starts
-        are automatically computed as the first point before the normalized IR
-        arrives at -20 dBFS. This is then done independently for each channel
-        and each band. Default: `None`.
+        shape (band, channel) for a `MultiBandSignal`. Default: `None`.
     automatic_trimming : bool, optional
-        When set to `True`, the IR is trimmed using `trim_rir` with offset 20
-        ms before the impulse, envelope smoothing of 10 ms and threshold
-        factor 0.66. This can influence significantly the energy decay curve
-        and, therefore, the reverberation time. See notes for details on the
-        algorithm. Default: `True`.
+        When set to `True`, the IR is trimmed using `trim_rir` independently
+        for each channel. This can influence significantly the energy decay
+        curve and, therefore, the reverberation time. See notes for details
+        on the algorithm. Default: `True`.
 
     Returns
     -------
     reverberation_times : `np.ndarray`
         Reverberation times for each channel. Shape is (band, channel)
         if `MultiBandSignal` object is passed.
     correlation_coefficient : `np.ndarray`
@@ -76,16 +72,16 @@
     - A correlation coefficient of -1 means there is a perfectly linear
       relation between time and energy decay, which is an optimal estimation.
       Coefficients larger than -0.9 might mean that the estimation is not
       valid.
     - In order to compare EDT to the other measures, it must be multiplied
       by 6.
     - For defining the ending of the IR automatically, `trim_rir(
-      offset_start_s = 0, threshold_factor = 0.66, window_time_s = 30e-3)` is
-      used.
+      offset_start_s = 20e-3, threshold_factor = 0.66,
+      window_time_s = 30e-3)` is used.
 
     """
     if type(signal) is Signal:
         ir_start = _check_ir_start_reverb(signal, ir_start)
         assert signal.signal_type in ("ir", "rir"), (
             f"{signal.signal_type} is not a valid signal type for "
             + "reverb_time. It should be ir or rir"
```

### Comparing `dsptoolbox-0.3.4/dsptoolbox/transfer_functions/__init__.py` & `dsptoolbox-0.3.5/dsptoolbox/transfer_functions/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,16 +30,18 @@
 - `minimum_group_delay()`
 - `excess_group_delay()`
 - `minimum_phase()`
 - `window_frequency_dependent()` (obtain a spectrum with a frequency-dependent
   window)
 - `find_ir_latency()`
 - `harmonics_from_chirp_ir()`
+- `harmonic_distortion_analysis()`
 
 """
+
 from .transfer_functions import (
     spectral_deconvolve,
     window_ir,
     window_frequency_dependent,
     window_centered_ir,
     compute_transfer_function,
     average_irs,
@@ -52,14 +54,15 @@
     minimum_phase,
     ir_to_filter,
     filter_to_ir,
     combine_ir_with_dirac,
     warp_ir,
     find_ir_latency,
     harmonics_from_chirp_ir,
+    harmonic_distortion_analysis,
 )
 
 __all__ = [
     "spectral_deconvolve",
     "window_ir",
     "compute_transfer_function",
     "average_irs",
@@ -74,8 +77,9 @@
     "ir_to_filter",
     "filter_to_ir",
     "combine_ir_with_dirac",
     "window_centered_ir",
     "warp_ir",
     "find_ir_latency",
     "harmonics_from_chirp_ir",
+    "harmonic_distortion_analysis",
 ]
```

### Comparing `dsptoolbox-0.3.4/dsptoolbox/transfer_functions/_transfer_functions.py` & `dsptoolbox-0.3.5/dsptoolbox/transfer_functions/_transfer_functions.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/transfer_functions/transfer_functions.py` & `dsptoolbox-0.3.5/dsptoolbox/transfer_functions/transfer_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Methods used for acquiring and windowing transfer functions
 """
 
 import numpy as np
 from scipy.signal import minimum_phase as min_phase_scipy
 from scipy.fft import rfft as rfft_scipy, next_fast_len as next_fast_length_fft
+from scipy.interpolate import interp1d
 
 from ._transfer_functions import (
     _spectral_deconvolve,
     _window_this_ir_tukey,
     _window_this_ir,
     _min_phase_ir_from_real_cepstrum,
     _get_minimum_phase_spectrum_from_real_cepstrum,
@@ -30,15 +31,15 @@
     _minimum_phase,
     _group_delay_direct,
     _pad_trim,
 )
 from ..standard_functions import fractional_delay, merge_signals, normalize
 from ..generators import dirac
 from ..filterbanks import linkwitz_riley_crossovers
-from ..room_acoustics._room_acoustics import _find_ir_start
+from ..room_acoustics._room_acoustics import _find_ir_start, _trim_rir
 
 
 def spectral_deconvolve(
     num: Signal,
     denum: Signal,
     mode: str = "regularized",
     start_stop_hz=None,
@@ -262,20 +263,16 @@
             constant_percentage,
             at_start,
             offset_samples,
             left_to_right_flank_length_ratio,
             adaptive,
         )
 
-    new_sig = Signal(
-        None,
-        new_time_data,
-        signal.sampling_rate_hz,
-        signal_type=signal.signal_type,
-    )
+    new_sig = signal.copy()
+    new_sig.time_data = new_time_data
     new_sig.set_window(window)
     return new_sig, start_positions_samples
 
 
 def window_centered_ir(
     signal: Signal,
     total_length_samples: int,
@@ -327,20 +324,16 @@
             new_time_data[:, n],
             window[:, n],
             start_positions_samples[n],
         ) = _window_this_ir(
             signal.time_data[:, n], total_length_samples, window_type
         )
 
-    new_sig = Signal(
-        None,
-        new_time_data,
-        signal.sampling_rate_hz,
-        signal_type=signal.signal_type,
-    )
+    new_sig = signal.copy()
+    new_sig.time_data = new_time_data
     new_sig.set_window(window)
     return new_sig, start_positions_samples
 
 
 def compute_transfer_function(
     output: Signal,
     input: Signal,
@@ -723,15 +716,15 @@
                     + f"than minimal group delay {gd_ms * 1000} ms for "
                     + f"channel {n}"
                 )
                 gd_ms = group_delay_ms
         else:
             gd_ms = group_delay_ms
 
-        phase = 2 * np.pi * f_vec * gd_ms
+        phase = -2 * np.pi * f_vec * gd_ms
         if spectrum_has_nyquist:
             phase = _correct_for_real_phase_spectrum(_wrap_phase(phase))
         lin_spectrum[:, n] = spectrum[:, n] * np.exp(1j * phase)
     time_data = np.fft.irfft(lin_spectrum, axis=0, n=original_length_time_data)
     sig_lin_phase = Signal(
         None,
         time_data=time_data,
@@ -763,15 +756,14 @@
 
     Returns
     -------
     min_phase_sig : `Signal`
         Minimum-phase IR as time signal.
 
     """
-    # Computation
     assert sig.signal_type in (
         "rir",
         "ir",
     ), "Signal type must be either rir or ir"
     method = method.lower()
     assert method in ("real cepstrum", "log hilbert", "equiripple"), (
         f"{method} is not valid. Use either real cepstrum, log hilbert or "
@@ -1344,20 +1336,24 @@
     for ch in range(td.shape[1]):
         n[:, ch] = np.arange(-ind_max[ch], td.shape[0] - ind_max[ch])
 
     # Scaling function
     if scaling == "amplitude spectrum":
 
         def scaling_func(window: np.ndarray):
-            return 2**0.5 / np.sum(window, axis=0)
+            return 2**0.5 / np.sum(window, axis=0, keepdims=True)
 
     elif scaling == "amplitude spectral density":
 
         def scaling_func(window: np.ndarray):
-            return (2 / np.sum(window**2, axis=0) / ir.sampling_rate_hz) ** 0.5
+            return (
+                2
+                / np.sum(window**2, axis=0, keepdims=True)
+                / ir.sampling_rate_hz
+            ) ** 0.5
 
     elif scaling == "fft":
         scaling_value = fast_length**-0.5
 
         def scaling_func(window: np.ndarray):
             return scaling_value
 
@@ -1513,14 +1509,17 @@
     assert ir.signal_type in (
         "ir",
         "rir",
     ), "Signal type has to be either ir or rir"
     assert (
         offset_percentage < 1 and offset_percentage >= 0
     ), "Offset must be smaller than one"
+    assert (
+        ir.number_of_channels == 1
+    ), "Only an IR with a single channel is supported"
 
     # Get offsets
     td = ir.time_data
     offsets = -np.argmax(td, axis=0) + 1
     td = np.roll(td, offsets, axis=0)
 
     # Get times of each harmonic
@@ -1529,30 +1528,228 @@
     )
     time_harmonics_samples = len(td) + (ts * ir.sampling_rate_hz + 0.5).astype(
         int
     )
 
     time_harmonics_samples = np.insert(time_harmonics_samples, 0, len(td))
 
+    # Dummy to obtain all metadata of the IR
+    ir_dummy = ir.copy()
+    ir_dummy.time_data = ir.time_data[:10]
+
     harmonics = []
     for nh in range(n_harmonics):
         max_ind = int(
             time_harmonics_samples[nh]
             - (time_harmonics_samples[nh] - time_harmonics_samples[nh + 1])
             * offset_percentage
         )
         min_ind = int(
             time_harmonics_samples[nh + 1]
             - (time_harmonics_samples[nh + 1] - time_harmonics_samples[nh + 2])
             * offset_percentage
         )
         snippet = td[min_ind:max_ind, 0]
-        harmonics.append(
-            Signal(
-                None,
-                snippet,
-                ir.sampling_rate_hz,
-                signal_type="ir",
-                constrain_amplitude=ir.constrain_amplitude,
-            )
-        )
+
+        new_harmonic = ir_dummy.copy()
+        new_harmonic.time_data = snippet
+        harmonics.append(new_harmonic)
     return harmonics
+
+
+def harmonic_distortion_analysis(
+    ir: Signal | list[Signal],
+    chirp_range_hz: list | None = None,
+    chirp_length_s: float | None = None,
+    n_harmonics: int | None = 8,
+    smoothing: int = 12,
+    generate_plot: bool = True,
+) -> dict:
+    """
+    Analyze non-linear distortion coming from an IR measured with an
+    exponential chirp. The range of the chirp and its length must be known.
+    The distortion spectra of each harmonic, as well as THD+N and THD, are
+    returned. Optionally, a plot can be generated.
+
+    Parameters
+    ----------
+    ir : `Signal` or list[`Signal`]
+        Impulse response. It should only have one channel. Alternatively,
+        a list containing the fundamental IR and all harmonics can be passed,
+        in which case `chirp_range_hz`, `chirp_length_s` and `n_harmonics`
+        will be ignored or inferred. In the second case, no windowing or
+        trimming will be applied to either the fundamental or the harmonics.
+    chirp_range_hz : list
+        List with length 2 containing the lowest and highest frequency of the
+        exponential chirp.
+    chirp_length_s : float
+        Length of the chirp (time from lowest to highest frequency) in seconds.
+    n_harmonics : int, optional
+        Number of harmonics to analyze. Default: 8.
+    smoothing : int, optional
+        Smoothing as fraction of an octave band to apply to all spectra.
+        Default: 12.
+    generate_plot : bool, optional
+        When `True`, a plot with all the distortion spectra is generated.
+        Default: `True`.
+
+    Returns
+    -------
+    dict
+        A dictionary containing each spectrum is returned. Each item is a list
+        with form [frequency vector, spectrum]. Its keys are:
+            - "1": spectrum of the fundamental.
+            - "2": spectrum of the second harmonic.
+            - "3": ...
+            - "thd": Total harmonic distortion.
+            - "thd_n": Total harmonic distortion + noise.
+            - "plot": a list with matplotlib's [figure, axes]. This is only
+              returned if the plot was generated.
+
+    Notes
+    -----
+    - The scaling of the spectrum is always done as set with
+      `set_spectrum_parameters()` of the original IR. THD and THD+N are always
+      returned with their quadratic (power) form. All spectra are in amplitude
+      or power values according to `scaling`, but not in dB.
+    - Distortion in percentage can be computed by dividing `thd` by the
+      spectrum of the fundamental. They have the same frequency resolution
+      but `thd` has a trimmed frequency vector.
+    - Passing `chirp_range_hz` with a list of IRs will still have an effect on
+      the upper limit frequency of each harmonic.
+
+    """
+    if type(ir) is list:
+        for each_ir in ir:
+            assert type(each_ir) is Signal, "Unsupported type"
+            assert (
+                each_ir.number_of_channels == 1
+            ), "Only single-channel IRs are supported"
+
+        ir2 = ir.pop(0)
+        ir2._spectrum_parameters["smoothe"] = smoothing
+
+        harm = ir
+        n_harmonics = len(harm)
+        if chirp_range_hz is None:
+            chirp_range_hz = [0, ir2.sampling_rate_hz // 2]
+
+        passed_harmonics = True
+
+    elif type(ir) is Signal:
+        # Get different harmonics
+        harm = harmonics_from_chirp_ir(
+            ir, chirp_range_hz, chirp_length_s, n_harmonics, 0.01
+        )
+
+        passed_harmonics = False
+
+        # Trim and window IR
+        ir2 = ir.copy()
+        start, stop, _ = _trim_rir(
+            ir2.time_data, ir.sampling_rate_hz, 10e-3, 0.75, 30e-3
+        )
+        ir2.time_data = ir2.time_data[start:stop]
+        ir2 = window_ir(ir2, len(ir2), constant_percentage=0.9)[0]
+        ir2._spectrum_parameters["smoothe"] = smoothing
+    else:
+        raise TypeError("Type for ir is not supported")
+
+    # At least 5 Hz frequency resolution for base spectrum
+    pad_length = max(ir2.sampling_rate_hz // 5, len(ir2)) - len(ir2)
+    ir2.time_data = np.pad(ir2.time_data, ((0, pad_length), (0, 0)))
+
+    # Accumulator for THD time samples and dictionary
+    thd = np.zeros(np.sum([len(h) for h in harm]))
+    pos_thd = len(thd)
+    d: dict = {}
+
+    # Spectrum of fundamental
+    freqs, base_spectrum = ir2.get_spectrum()
+    d["1"] = [freqs, base_spectrum.squeeze()]
+
+    # Accumulator for spectrum of harmonics
+    sp_thd = np.zeros(len(freqs))
+
+    scaling = ir2._spectrum_parameters["scaling"]
+    if scaling is None:
+        quadratic_spectrum = False
+    else:
+        quadratic_spectrum = "power" in scaling
+
+    if generate_plot:
+        fig, ax = ir2.plot_magnitude(smoothe=smoothing, normalize=None)
+
+    for i in range(len(harm)):
+        if not passed_harmonics:
+            harm[i] = window_ir(
+                harm[i], len(harm[i]), constant_percentage=0.9
+            )[0]
+        harm[i].set_spectrum_parameters(**ir2._spectrum_parameters)
+        f, sp = harm[i].get_spectrum()
+
+        # Select frequencies that really were excited by chirp and fftshift
+        # for true excitation frequency
+        inds = f < chirp_range_hz[-1]
+        f = f[inds]
+        sp = sp[inds]
+        f /= i + 2
+
+        # Get power
+        sp_power = (
+            sp.squeeze() if quadratic_spectrum else np.abs(sp.squeeze()) ** 2
+        )
+
+        # Save in dictionary
+        d[f"{i + 2}"] = [f, sp]
+
+        # Make plot
+        if generate_plot:
+            ax.plot(f, 10 * np.log10(sp_power))
+
+        # Accumulate time samples for THD+N
+        thd[pos_thd - len(harm[i]) : pos_thd] = harm[i].time_data.squeeze()
+        pos_thd -= len(harm[i])
+
+        # Sum power of each harmonic
+        sp_thd += interp1d(
+            f,
+            sp_power,
+            kind="linear",
+            bounds_error=False,
+            fill_value=0,
+            assume_sorted=True,
+        )(freqs)
+
+    # THD
+    ind_end = np.argmin(np.abs(freqs - chirp_range_hz[-1] / 2))
+    sp_thd = sp_thd[:ind_end]
+    freqs_thd = freqs[:ind_end]
+    if generate_plot:
+        sp_thd[sp_thd == 0] = np.nan
+        ax.plot(freqs_thd, 10 * np.log10(sp_thd), label="THD")
+        np.nan_to_num(sp_thd, False, 0)
+
+    # THD+N
+    thd_n = Signal(None, thd, ir2.sampling_rate_hz)
+    thd_n.set_spectrum_parameters(**ir2._spectrum_parameters)
+    f_thd_n, sp_thd_n = thd_n.get_spectrum()
+    if not quadratic_spectrum:
+        sp_thd_n = np.abs(sp_thd_n) ** 2
+
+    if generate_plot:
+        ax.plot(
+            f_thd_n,
+            10 * np.log10(sp_thd_n),
+            label="THD+N",
+        )
+        ax.legend(
+            ["Fundamental"]
+            + [f"{i + 2} Harmonic" for i in range(n_harmonics)]
+            + ["THD", "THD+N"]
+        )
+        d["plot"] = [fig, ax]
+
+    d["thd_n"] = [f_thd_n, sp_thd_n]
+    d["thd"] = [freqs_thd, sp_thd]
+
+    return d
```

### Comparing `dsptoolbox-0.3.4/dsptoolbox/transforms/__init__.py` & `dsptoolbox-0.3.5/dsptoolbox/transforms/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 - `mfcc()` (mel-frequency cepstral coefficients)
 - `istft()` (inverse STFT)
 - `MorletWavelet` (class for a complex morlet wavelet)
 - `cwt()` (continuous wavelet transform)
 - `chroma_stft()` (STFT adapted to the chroma scale)
 - `hilbert()` (Hilbert Transform)
 - `vqt()` (Variable-Q Transform)
+- `stereo_mid_side()` (Mid-Side representation of stereo signal)
 
 """
+
 from .transforms import (
     cepstrum,
     log_mel_spectrogram,
     mel_filterbank,
     plot_waterfall,
     mfcc,
     istft,
```

### Comparing `dsptoolbox-0.3.4/dsptoolbox/transforms/_transforms.py` & `dsptoolbox-0.3.5/dsptoolbox/transforms/_transforms.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/dsptoolbox/transforms/transforms.py` & `dsptoolbox-0.3.5/dsptoolbox/transforms/transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,17 @@
 def log_mel_spectrogram(
     s: Signal,
     channel: int = 0,
     range_hz=None,
     n_bands: int = 40,
     generate_plot: bool = True,
     stft_parameters: dict | None = None,
+) -> (
+    tuple[np.ndarray, np.ndarray, np.ndarray]
+    | tuple[np.ndarray, np.ndarray, np.ndarray, plt.Figure, plt.Axes]
 ):
     """Returns the log mel spectrogram of the specific signal and channel.
 
     Parameters
     ----------
     s : `Signal`
         Signal to generate the spectrogram.
@@ -275,24 +278,26 @@
     fig, ax = plt.subplots(figsize=(10, 8), subplot_kw=dict(projection="3d"))
     tt, ff = np.meshgrid(t, f)
     ax.plot_surface(tt, ff, 20 * np.log10(stft), cmap="magma")
     ax.set_xlabel("Time / s")
     ax.set_ylabel("Frequency / Hz")
     ax.set_zlabel("dB" + z_label_extra)
     fig.tight_layout()
-    # fig.colorbar(surface, ax=ax, shrink=0.4, aspect=10)
     return fig, ax
 
 
 def mfcc(
     signal: Signal,
     channel: int = 0,
     mel_filters: np.ndarray | None = None,
     generate_plot: bool = True,
     stft_parameters: dict | None = None,
+) -> (
+    tuple[np.ndarray, np.ndarray, np.ndarray]
+    | tuple[np.ndarray, np.ndarray, np.ndarray, plt.Figure, plt.Axes]
 ):
     """Mel-frequency cepstral coefficients for a windowed signal are computed
     and returned using the discrete cosine transform of type 2 (see
     `scipy.fft.dct` for more details).
 
     Parameters
     ----------
@@ -528,14 +533,17 @@
 
 
 def chroma_stft(
     signal: Signal,
     tuning_a_hz: float = 440,
     compression: float = 0.5,
     plot_channel: int = -1,
+) -> (
+    tuple[np.ndarray, np.ndarray, np.ndarray]
+    | tuple[np.ndarray, np.ndarray, np.ndarray, plt.Figure, plt.Axes]
 ):
     """This computes the Chroma Features and Pitch STFT. See [1] for details.
 
     Parameters
     ----------
     signal : `Signal`
         Signal for which to compute the chroma features. The saved parameters
@@ -733,15 +741,15 @@
     channel: np.ndarray | None = None,
     q: float = 1,
     gamma: float = 50,
     octaves: list = [1, 5],
     bins_per_octave: int = 24,
     a4_tuning: int = 440,
     window: str | tuple = "hann",
-):
+) -> tuple[np.ndarray, np.ndarray]:
     """Variable-Q Transform. This is a special case of the continuous wavelet
     transform with complex morlet wavelets for the time-frequency analysis.
     Constant-Q Transform can be obtained by setting `gamma = 0`.
 
     Parameters
     ----------
     signal : `Signal`
@@ -840,15 +848,15 @@
     cqt = np.flip(cqt, axis=0)
     f = a4_tuning * 2 ** (
         np.arange(octaves[0] - 4 - 9 / 12, octaves[1] - 4 + 2 / 12, 1 / 12)
     )
     return f, cqt
 
 
-def stereo_mid_side(signal: Signal, forward: bool):
+def stereo_mid_side(signal: Signal, forward: bool) -> Signal:
     """This function converts a left-right stereo signal to its mid-side
     representation or the other way around. It is only available for
     two-channels signals.
 
     Parameters
     ----------
     signal : `Signal`
```

### Comparing `dsptoolbox-0.3.4/examples/audio_io_module.ipynb` & `dsptoolbox-0.3.5/examples/audio_io_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/examples/beamforming_module.ipynb` & `dsptoolbox-0.3.5/examples/beamforming_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/examples/distances_module.ipynb` & `dsptoolbox-0.3.5/examples/distances_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/examples/filterbanks_module.ipynb` & `dsptoolbox-0.3.5/examples/filterbanks_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/examples/general.ipynb` & `dsptoolbox-0.3.5/examples/general.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/examples/generators_module.ipynb` & `dsptoolbox-0.3.5/examples/generators_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/examples/room_acoustics_module.ipynb` & `dsptoolbox-0.3.5/examples/room_acoustics_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/examples/standard_module.ipynb` & `dsptoolbox-0.3.5/examples/standard_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/examples/transfer_function_module.ipynb` & `dsptoolbox-0.3.5/examples/transfer_function_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/examples/transforms_module.ipynb` & `dsptoolbox-0.3.5/examples/transforms_module.ipynb`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/examples/data/array.xml` & `dsptoolbox-0.3.5/examples/data/array.xml`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/examples/data/chirp.wav` & `dsptoolbox-0.3.5/examples/data/chirp.wav`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/examples/data/chirp_mono.wav` & `dsptoolbox-0.3.5/examples/data/chirp_mono.wav`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/examples/data/chirp_stereo.wav` & `dsptoolbox-0.3.5/examples/data/chirp_stereo.wav`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/examples/data/fuer_elise.wav` & `dsptoolbox-0.3.5/examples/data/fuer_elise.wav`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/examples/data/rir.wav` & `dsptoolbox-0.3.5/examples/data/rir.wav`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/examples/data/speech.flac` & `dsptoolbox-0.3.5/examples/data/speech.flac`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/tests/test_beamforming.py` & `dsptoolbox-0.3.5/tests/test_beamforming.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/tests/test_classes.py` & `dsptoolbox-0.3.5/tests/test_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,25 +236,25 @@
         s.set_spectrogram_parameters(
             window_length_samples=1024,
             window_type="hann",
             overlap_percent=50,
             fft_length_samples=4096,
             detrend=False,
             padding=False,
-            scaling=False,
+            scaling="power spectrum",
         )
         t, f, stft = s.get_spectrogram()
         s.set_spectrogram_parameters(
             window_length_samples=1024,
             window_type="hann",
             overlap_percent=50,
             fft_length_samples=None,
             detrend=False,
             padding=False,
-            scaling=False,
+            scaling=None,
         )
         t, f, stft = s.get_spectrogram()
 
         # Validate result with librosa library if installed
         try:
             import librosa
```

### Comparing `dsptoolbox-0.3.4/tests/test_distances.py` & `dsptoolbox-0.3.5/tests/test_distances.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/tests/test_filterbanks.py` & `dsptoolbox-0.3.5/tests/test_filterbanks.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/tests/test_fx.py` & `dsptoolbox-0.3.5/tests/test_fx.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/tests/test_generators.py` & `dsptoolbox-0.3.5/tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/tests/test_room_acoustics.py` & `dsptoolbox-0.3.5/tests/test_room_acoustics.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/tests/test_standard.py` & `dsptoolbox-0.3.5/tests/test_standard.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,33 +16,33 @@
             (td.shape[0] + delay_samples, self.audio_multi.number_of_channels)
         )
         td_del[-td.shape[0] :] = td
 
         # Try latency
         s = dsp.Signal(None, td_del, self.fs)
         vector = dsp.latency(self.audio_multi, s)
-        assert np.all(np.abs(vector) == delay_samples)
+        assert np.all(vector == -delay_samples)
 
         # Try latency the other way around
         vector = dsp.latency(s, self.audio_multi)
-        assert np.all(np.abs(vector) == delay_samples)
+        assert np.all(vector == delay_samples)
 
         # Raise assertion when number of channels does not match
         with pytest.raises(AssertionError):
             vector = dsp.latency(s.get_channels(0), self.audio_multi)
 
         # Single channel
         td = s.time_data[:, :2]
         td[:, 1] = 0
         td[: len(self.audio_multi.time_data[:, 0]), 1] = (
             self.audio_multi.time_data[:, 0]
         )
         s = dsp.Signal(None, td, self.fs)
         value = dsp.latency(s)
-        assert np.all(np.abs(value) == delay_samples)
+        assert np.all(-value == delay_samples)
 
         # ===== Fractional delays
         delay = 0.003301
         noi = dsp.generators.noise(
             "white", length_seconds=1, sampling_rate_hz=10_000
         )
         noi_del = dsp.fractional_delay(noi, delay)
@@ -50,17 +50,19 @@
             np.abs(
                 dsp.latency(noi_del, noi, 2)[0] - delay * noi.sampling_rate_hz
             )
             < 0.9
         )
 
         noi = dsp.merge_signals(noi_del, noi)
-        latencies = dsp.latency(noi, polynomial_points=5)
+        latencies = dsp.latency(noi, polynomial_points=1)
         assert len(latencies) == noi.number_of_channels - 1
         assert np.abs(latencies[0] + delay * noi.sampling_rate_hz) < 0.5
+        latencies = dsp.latency(noi, polynomial_points=5)
+        assert np.abs(latencies[0] + delay * noi.sampling_rate_hz) < 0.5
 
     def test_pad_trim(self):
         # Check for signal: Trim at the end
         trim_length = 40_000
         td = self.audio_multi.time_data[:trim_length]
         s = dsp.Signal(None, td, self.fs)
         assert np.all(
```

### Comparing `dsptoolbox-0.3.4/tests/test_transfer_functions.py` & `dsptoolbox-0.3.5/tests/test_transfer_functions.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/tests/test_transforms.py` & `dsptoolbox-0.3.5/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/LICENSE` & `dsptoolbox-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/README.rst` & `dsptoolbox-0.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/pyproject.toml` & `dsptoolbox-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dsptoolbox-0.3.4/PKG-INFO` & `dsptoolbox-0.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: dsptoolbox
-Version: 0.3.4
+Version: 0.3.5
 Summary: Collection of dsp algorithms to be used for analysis of audio signals
 Project-URL: Homepage, https://github.com/nico-franco-gomez/dsptoolbox
 Project-URL: Bug Tracker, https://github.com/nico-franco-gomez/dsptoolbox/issues
 Project-URL: Documentation, https://dsptoolbox.readthedocs.io/en/latest/
 Author: Nicolas Franco-Gomez
 License-Expression: MIT
 License-File: LICENSE
```

