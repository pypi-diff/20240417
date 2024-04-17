# Comparing `tmp/pixi_kernel-0.2.1.tar.gz` & `tmp/pixi_kernel-0.3.0.tar.gz`

## Comparing `pixi_kernel-0.2.1.tar` & `pixi_kernel-0.3.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/codecov.yml
--rw-r--r--   0        0        0   494805 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/pixi.lock
--rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/pixi.toml
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/.github/workflows/release.yml
--rw-r--r--   0        0        0   169085 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/assets/launch-dark.png
--rw-r--r--   0        0        0   176986 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/assets/launch-light.png
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-bash/kernel.json
--rw-r--r--   0        0        0   801365 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-bash/logo-svg.svg
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-ir/kernel.js
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-ir/kernel.json
--rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-ir/logo-64x64.png
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-ir/logo-svg.svg
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-python3/kernel.json
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-python3/logo-32x32.png
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-python3/logo-64x64.png
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-python3/logo-svg.svg
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp11/kernel.json
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp11/logo-32x32.png
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp11/logo-64x64.png
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp11/logo-svg.svg
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp14/kernel.json
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp14/logo-32x32.png
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp14/logo-64x64.png
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp14/logo-svg.svg
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp17/kernel.json
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp17/logo-32x32.png
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp17/logo-64x64.png
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp17/logo-svg.svg
--rwxr-xr-x   0        0        0      466 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/scripts/update-lock.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/src/pixi_kernel/__init__.py
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/src/pixi_kernel/errors.py
--rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/src/pixi_kernel/pixi.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/src/pixi_kernel/provisioner.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/integration/bash_kernel/kernel.py
--rw-r--r--   0        0        0   123358 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/integration/bash_kernel/pixi.lock
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/integration/bash_kernel/pixi.toml
--rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/integration/ipykernel/kernel.py
--rw-r--r--   0        0        0   119641 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/integration/ipykernel/pixi.lock
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/integration/ipykernel/pixi.toml
--rw-r--r--   0        0        0    16817 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/integration/r-irkernel/kernel.py
--rw-r--r--   0        0        0   329298 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/integration/r-irkernel/pixi.lock
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/integration/r-irkernel/pixi.toml
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/integration/xeus-cling/kernel.py
--rw-r--r--   0        0        0    77254 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/integration/xeus-cling/pixi.lock
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/integration/xeus-cling/pixi.toml
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/unit/conftest.py
--rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/unit/test_pixi.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/unit/data/missing_ipykernel/pixi.toml
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/unit/data/pixi_project/pixi.toml
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/tests/unit/data/pyproject_project/pyproject.toml
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/LICENSE
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/README.md
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 pixi_kernel-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/codecov.yml
+-rw-r--r--   0        0        0   551274 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/pixi.lock
+-rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/pixi.toml
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0   169085 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/assets/launch-dark.png
+-rw-r--r--   0        0        0   176986 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/assets/launch-light.png
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/kernels/pixi-kernel-bash/kernel.json
+-rw-r--r--   0        0        0   801365 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/kernels/pixi-kernel-bash/logo-svg.svg
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/kernels/pixi-kernel-ir/kernel.js
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/kernels/pixi-kernel-ir/kernel.json
+-rw-r--r--   0        0        0     8492 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/kernels/pixi-kernel-ir/logo-64x64.png
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/kernels/pixi-kernel-ir/logo-svg.svg
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/kernels/pixi-kernel-python3/kernel.json
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/kernels/pixi-kernel-python3/logo-32x32.png
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/kernels/pixi-kernel-python3/logo-64x64.png
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/kernels/pixi-kernel-python3/logo-svg.svg
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/kernels/pixi-kernel-xcpp11/kernel.json
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/kernels/pixi-kernel-xcpp11/logo-32x32.png
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/kernels/pixi-kernel-xcpp11/logo-64x64.png
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/kernels/pixi-kernel-xcpp11/logo-svg.svg
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/kernels/pixi-kernel-xcpp14/kernel.json
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/kernels/pixi-kernel-xcpp14/logo-32x32.png
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/kernels/pixi-kernel-xcpp14/logo-64x64.png
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/kernels/pixi-kernel-xcpp14/logo-svg.svg
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/kernels/pixi-kernel-xcpp17/kernel.json
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/kernels/pixi-kernel-xcpp17/logo-32x32.png
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/kernels/pixi-kernel-xcpp17/logo-64x64.png
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/kernels/pixi-kernel-xcpp17/logo-svg.svg
+-rwxr-xr-x   0        0        0      466 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/scripts/update-lock.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/src/pixi_kernel/__init__.py
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/src/pixi_kernel/__main__.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/src/pixi_kernel/errors.py
+-rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/src/pixi_kernel/pixi.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/tests/integration/bash_kernel/kernel.py
+-rw-r--r--   0        0        0   123392 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/tests/integration/bash_kernel/pixi.lock
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/tests/integration/bash_kernel/pixi.toml
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/tests/integration/ipykernel/kernel.py
+-rw-r--r--   0        0        0   119675 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/tests/integration/ipykernel/pixi.lock
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/tests/integration/ipykernel/pixi.toml
+-rw-r--r--   0        0        0    16481 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/tests/integration/r-irkernel/kernel.py
+-rw-r--r--   0        0        0   365023 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/tests/integration/r-irkernel/pixi.lock
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/tests/integration/r-irkernel/pixi.toml
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/tests/integration/xeus-cling/kernel.py
+-rw-r--r--   0        0        0    96917 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/tests/integration/xeus-cling/pixi.lock
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/tests/integration/xeus-cling/pixi.toml
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/tests/unit/conftest.py
+-rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/tests/unit/test_pixi.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/tests/unit/data/missing_ipykernel/pixi.toml
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/tests/unit/data/pixi_project/pixi.toml
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/tests/unit/data/pyproject_project/pyproject.toml
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/README.md
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 pixi_kernel-0.3.0/PKG-INFO
```

### Comparing `pixi_kernel-0.2.1/CONTRIBUTING.md` & `pixi_kernel-0.3.0/CONTRIBUTING.md`

 * *Files 9% similar despite different names*

```diff
@@ -38,20 +38,21 @@
 
 ```
 pixi run -e py38 test-py38
 ```
 
 ## Code quality
 
-Pixi Kernel uses Ruff to ensure a minimum standard of code quality. The code quality commands are
-encapsulated with Pixi:
+Pixi Kernel uses Ruff and MyPy to ensure a minimum standard of code quality. The code quality
+commands are encapsulated with Pixi:
 
 ```
 pixi run format
 pixi run lint
+pixi run type-check
 ```
 
 ## Making a release
 
 1. Bump
    1. Increment version in `pyproject.toml` and in `pixi.toml`
    2. Update all Pixi lock files by running `pixi run update-lock`
@@ -72,15 +73,17 @@
 ## Adding support for new kernels
 
 Follow the steps below to add support for a new kernel:
 
 1. In a fresh Pixi environment install your kernel with `pixi install <kernel>`.
 2. Copy the new folders created at `.pixi/envs/default/share/jupyter/kernels/` to the `kernels`
    folder and commit the changes.
-3. Update the display name, metadata and command arguments in the kernel spec file `kernel.json`.
+3. Update the display name and command arguments in the kernel spec file `kernel.json`. The command
+   arguments should start with `["python", "-m", "pixi_kernel", <package_name>,
+<kernel_display_name>]` and all absolute paths should be removed.
 4. Update the Kernel Support table in the README.
 5. Add integration tests for the new kernel in the `tests/integration` folder and commit the
    changes.
 
 You can find below two examples of adding support for new kernels:
 
 Steps 1 and 2:
```

### Comparing `pixi_kernel-0.2.1/pixi.lock` & `pixi_kernel-0.3.0/pixi.lock`

 * *Files 1% similar despite different names*

```diff
@@ -25,28 +25,28 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyha804496_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.6.2-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-h807b86a_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h807b86a_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-hd590300_2.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.2-h2797004_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h7e041cc_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
@@ -61,31 +61,31 @@
       - conda: https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.43-hcad00b1_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.2-hab00c5b_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/secretstorage-3.3.3-py312h7900ff3_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/uv-0.1.31-h0e8d75e_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/uv-0.1.32-h0e8d75e_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zstandard-0.22.0-py312hd58854c_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.5-hfc55251_0.conda
       linux-aarch64:
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/_openmp_mutex-4.5-2_gnu.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
@@ -106,28 +106,28 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyha804496_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ld_impl_linux-aarch64-2.40-h2d8c526_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libexpat-2.6.2-h2f0025b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libffi-3.4.2-h3557bc0_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libgcc-ng-13.2.0-hf8544c7_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libglib-2.80.0-h9d8fbc1_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libglib-2.80.0-h9d8fbc1_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libgomp-13.2.0-hf8544c7_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libiconv-1.17-h31becfc_2.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libnsl-2.0.1-h31becfc_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libsqlite-3.45.2-h194ca79_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libstdcxx-ng-13.2.0-h9a76618_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libuuid-2.38.1-hb4cce97_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libxcrypt-4.4.36-h31becfc_1.conda
@@ -142,31 +142,31 @@
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/pcre2-10.43-hd0f9c67_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.2-h43d1f9e_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.3-h43d1f9e_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/readline-8.2-h8fc344f_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/secretstorage-3.3.3-py312h8025657_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/tk-8.6.13-h194ca79_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/uv-0.1.31-hb6a771c_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/uv-0.1.32-hb6a771c_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/xz-5.2.6-h9cdd2b7_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/zstandard-0.22.0-py312hb120188_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/zstd-1.5.5-h4c53e97_0.conda
       osx-64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
@@ -183,15 +183,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyh534df25_0.conda
@@ -209,30 +209,30 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.2-h9f0c242_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/uv-0.1.31-h2c5c2bd_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/uv-0.1.32-h2c5c2bd_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/zstandard-0.22.0-py312h7a629f7_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.5-h829000d_0.conda
       osx-arm64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
@@ -249,15 +249,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyh534df25_0.conda
@@ -275,30 +275,30 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.2-hdf0ec26_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.3-h4a7b5fc_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/uv-0.1.31-h2b8f702_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/uv-0.1.32-h2b8f702_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zstandard-0.22.0-py312h7975427_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zstd-1.5.5-h4f39d0f_0.conda
       win-64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda
@@ -316,15 +316,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyh7428d3b_0.conda
@@ -340,496 +340,890 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.2-h2628c8c_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.3-h2628c8c_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/pywin32-ctypes-0.2.2-py312h2e8e312_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/win-64/uv-0.1.31-h7ea99a0_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/uv-0.1.32-h7ea99a0_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hcf57466_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33130-h82b7239_18.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33130-hcb4865c_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/zstandard-0.22.0-py312h01d794b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.5-h12be248_0.conda
   default:
     channels:
     - url: https://conda.anaconda.org/conda-forge/
     packages:
       linux-64:
       - conda: https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2024.2.2-hbcca054_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/cffi-1.16.0-py312hf06ca03_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/coverage-7.4.4-py312h98912ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/cryptography-42.0.5-py312h241aef2_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/dbus-1.13.6-h5008d03_3.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.8.1-py312h30efb56_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.8-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/editables-0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/expat-2.6.2-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/filelock-3.13.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/h2-4.1.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyhd33586a_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.22.2-pyh707e725_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.7.2-py312h7900ff3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyha804496_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.6.2-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-h807b86a_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h807b86a_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-hd590300_2.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.2-h2797004_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h7e041cc_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/more-itertools-10.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/msgspec-0.18.6-py312h98912ed_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/mypy-1.9.0-py312h98912ed_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4.20240210-h59595ed_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.43-hcad00b1_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.8-py312h98912ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.2-hab00c5b_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.12-4_cp312.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.2-py312h886d080_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/pyzmq-26.0.0-py312h886d080_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ruff-0.3.7-py312h9118e91_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/secretstorage-3.3.3-py312h7900ff3_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tornado-6.4-py312h98912ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/uv-0.1.31-h0e8d75e_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/uv-0.1.32-h0e8d75e_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.5-h59595ed_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zstandard-0.22.0-py312hd58854c_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.5-hfc55251_0.conda
       - pypi: .
       linux-aarch64:
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/_openmp_mutex-4.5-2_gnu.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/bzip2-1.0.8-h31becfc_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ca-certificates-2024.2.2-hcefe29a_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/cffi-1.16.0-py312hf3c74c0_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/coverage-7.4.4-py312h9ef2f89_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/cryptography-42.0.5-py312h6f14deb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/dbus-1.13.6-h12b9eeb_3.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/debugpy-1.8.1-py312h2aa54b4_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.8-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/editables-0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/expat-2.6.2-h2f0025b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/filelock-3.13.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/h2-4.1.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyhd33586a_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.22.2-pyh707e725_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/jupyter_core-5.7.2-py312h996f985_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyha804496_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ld_impl_linux-aarch64-2.40-h2d8c526_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libexpat-2.6.2-h2f0025b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libffi-3.4.2-h3557bc0_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libgcc-ng-13.2.0-hf8544c7_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libglib-2.80.0-h9d8fbc1_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libglib-2.80.0-h9d8fbc1_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libgomp-13.2.0-hf8544c7_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libiconv-1.17-h31becfc_2.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libnsl-2.0.1-h31becfc_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libsodium-1.0.18-hb9de7d4_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libsqlite-3.45.2-h194ca79_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libstdcxx-ng-13.2.0-h9a76618_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libuuid-2.38.1-hb4cce97_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libxcrypt-4.4.36-h31becfc_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libzlib-1.2.13-h31becfc_5.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/more-itertools-10.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/msgspec-0.18.6-py312hdd3e373_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/mypy-1.9.0-py312hdd3e373_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ncurses-6.4.20240210-h0425590_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/openssl-3.2.1-h31becfc_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/pcre2-10.43-hd0f9c67_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/psutil-5.9.8-py312hdd3e373_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.2-h43d1f9e_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.3-h43d1f9e_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python_abi-3.12-4_cp312.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/pyzmq-25.1.2-py312h1c32067_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/pyzmq-26.0.0-py312h1c32067_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/readline-8.2-h8fc344f_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ruff-0.3.7-py312hb434743_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/secretstorage-3.3.3-py312h8025657_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/tk-8.6.13-h194ca79_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/tornado-6.4-py312h9ef2f89_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/uv-0.1.31-hb6a771c_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/uv-0.1.32-hb6a771c_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/xz-5.2.6-h9cdd2b7_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/zeromq-4.3.5-h2f0025b_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/zstandard-0.22.0-py312hb120188_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/zstd-1.5.5-h4c53e97_0.conda
       - pypi: .
       osx-64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/cffi-1.16.0-py312h38bf5a0_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/coverage-7.4.4-py312h41838bb_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.8.1-py312hede676d_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.8-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/editables-0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/filelock-3.13.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/h2-4.1.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyh3cd1d5f_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.22.2-pyh707e725_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.7.2-py312hb401068_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyh534df25_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libexpat-2.6.2-h73e2aa4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.2-h92b6c6a_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/more-itertools-10.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/msgspec-0.18.6-py312h41838bb_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/mypy-1.9.0-py312h41838bb_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4.20240210-h73e2aa4_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.2.1-hd75f5a5_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.8-py312h41838bb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.2-h9f0c242_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.12-4_cp312.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.2-py312hc789acb_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/pyzmq-26.0.0-py312hb81df1d_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ruff-0.3.7-py312h1bc86af_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tornado-6.4-py312h41838bb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/uv-0.1.31-h2c5c2bd_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/uv-0.1.32-h2c5c2bd_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.5-h93d8f39_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/zstandard-0.22.0-py312h7a629f7_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.5-h829000d_0.conda
       - pypi: .
       osx-arm64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ca-certificates-2024.2.2-hf0a4a13_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/cffi-1.16.0-py312h8e38eb3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/coverage-7.4.4-py312he37b823_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/debugpy-1.8.1-py312h20a0b95_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.8-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/editables-0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/filelock-3.13.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/h2-4.1.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyh3cd1d5f_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.22.2-pyh707e725_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/jupyter_core-5.7.2-py312h81bd7bf_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyh534df25_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libcxx-16.0.6-h4653b0c_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libexpat-2.6.2-hebf3989_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libffi-3.4.2-h3422bc3_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libsodium-1.0.18-h27ca646_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libsqlite-3.45.2-h091b4b1_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libzlib-1.2.13-h53f4e23_5.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/more-itertools-10.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/msgspec-0.18.6-py312he37b823_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/mypy-1.9.0-py312he37b823_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ncurses-6.4.20240210-h078ce10_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.2.1-h0d3ecfb_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/psutil-5.9.8-py312he37b823_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.2-hdf0ec26_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.3-h4a7b5fc_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.12-4_cp312.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pyzmq-25.1.2-py312h1edf716_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pyzmq-26.0.0-py312h2105c20_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ruff-0.3.7-py312h1ae9fbf_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tornado-6.4-py312he37b823_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/uv-0.1.31-h2b8f702_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/uv-0.1.32-h2b8f702_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zeromq-4.3.5-hebf3989_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zstandard-0.22.0-py312h7975427_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zstd-1.5.5-h4f39d0f_0.conda
       - pypi: .
       win-64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/cffi-1.16.0-py312he70551f_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-win_pyh7428d3b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/coverage-7.4.4-py312he70551f_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/debugpy-1.8.1-py312h53d5487_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.8-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/editables-0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/filelock-3.13.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/h11-0.14.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/h2-4.1.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyha63f2e9_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.22.2-pyh7428d3b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.7.2-py312h2e8e312_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyh7428d3b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libexpat-2.6.2-h63175ca_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.2-hcfcfb64_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/more-itertools-10.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/msgspec-0.18.6-py312he70551f_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/mypy-1.9.0-py312he70551f_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/openssl-3.2.1-hcfcfb64_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.8-py312he70551f_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.2-h2628c8c_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.3-h2628c8c_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/pywin32-306-py312h53d5487_2.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/pywin32-ctypes-0.2.2-py312h2e8e312_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/pyzmq-25.1.2-py312h1ac6f91_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/pyzmq-26.0.0-py312h1ac6f91_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ruff-0.3.7-py312h60fbdae_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/tornado-6.4-py312he70551f_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/win-64/uv-0.1.31-h7ea99a0_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/uv-0.1.32-h7ea99a0_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hcf57466_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33130-h82b7239_18.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33130-hcb4865c_18.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.5-h63175ca_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/zstandard-0.22.0-py312h01d794b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.5-h12be248_0.conda
       - pypi: .
+  mypy:
+    channels:
+    - url: https://conda.anaconda.org/conda-forge/
+    packages:
+      linux-64:
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2024.2.2-hbcca054_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.8.1-py312h30efb56_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyhd33586a_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.22.2-pyh707e725_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.7.2-py312h7900ff3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.6.2-h59595ed_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-h807b86a_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h807b86a_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.2-h2797004_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h7e041cc_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/msgspec-0.18.6-py312h98912ed_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/mypy-1.9.0-py312h98912ed_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4.20240210-h59595ed_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.8-py312h98912ed_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.12-4_cp312.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/pyzmq-26.0.0-py312h886d080_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/tornado-6.4-py312h98912ed_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.5-h59595ed_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
+      linux-aarch64:
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/_openmp_mutex-4.5-2_gnu.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/bzip2-1.0.8-h31becfc_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ca-certificates-2024.2.2-hcefe29a_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/debugpy-1.8.1-py312h2aa54b4_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyhd33586a_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.22.2-pyh707e725_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/jupyter_core-5.7.2-py312h996f985_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ld_impl_linux-aarch64-2.40-h2d8c526_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libexpat-2.6.2-h2f0025b_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libffi-3.4.2-h3557bc0_5.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libgcc-ng-13.2.0-hf8544c7_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libgomp-13.2.0-hf8544c7_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libnsl-2.0.1-h31becfc_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libsodium-1.0.18-hb9de7d4_1.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libsqlite-3.45.2-h194ca79_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libstdcxx-ng-13.2.0-h9a76618_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libuuid-2.38.1-hb4cce97_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libxcrypt-4.4.36-h31becfc_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libzlib-1.2.13-h31becfc_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/msgspec-0.18.6-py312hdd3e373_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/mypy-1.9.0-py312hdd3e373_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ncurses-6.4.20240210-h0425590_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/openssl-3.2.1-h31becfc_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/psutil-5.9.8-py312hdd3e373_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.3-h43d1f9e_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python_abi-3.12-4_cp312.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/pyzmq-26.0.0-py312h1c32067_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/readline-8.2-h8fc344f_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/tk-8.6.13-h194ca79_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/tornado-6.4-py312h9ef2f89_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/xz-5.2.6-h9cdd2b7_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/zeromq-4.3.5-h2f0025b_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
+      osx-64:
+      - conda: https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.8.1-py312hede676d_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyh3cd1d5f_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.22.2-pyh707e725_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.7.2-py312hb401068_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libexpat-2.6.2-h73e2aa4_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.2-h92b6c6a_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/msgspec-0.18.6-py312h41838bb_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/mypy-1.9.0-py312h41838bb_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4.20240210-h73e2aa4_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.2.1-hd75f5a5_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.8-py312h41838bb_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.12-4_cp312.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/pyzmq-26.0.0-py312hb81df1d_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/tornado-6.4-py312h41838bb_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.5-h93d8f39_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
+      osx-arm64:
+      - conda: https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ca-certificates-2024.2.2-hf0a4a13_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/debugpy-1.8.1-py312h20a0b95_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyh3cd1d5f_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.22.2-pyh707e725_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/jupyter_core-5.7.2-py312h81bd7bf_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libcxx-16.0.6-h4653b0c_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libexpat-2.6.2-hebf3989_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libffi-3.4.2-h3422bc3_5.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libsodium-1.0.18-h27ca646_1.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libsqlite-3.45.2-h091b4b1_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libzlib-1.2.13-h53f4e23_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/msgspec-0.18.6-py312he37b823_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/mypy-1.9.0-py312he37b823_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ncurses-6.4.20240210-h078ce10_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.2.1-h0d3ecfb_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/psutil-5.9.8-py312he37b823_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.3-h4a7b5fc_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.12-4_cp312.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pyzmq-26.0.0-py312h2105c20_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tornado-6.4-py312he37b823_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zeromq-4.3.5-hebf3989_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
+      win-64:
+      - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/debugpy-1.8.1-py312h53d5487_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyha63f2e9_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/ipython-8.22.2-pyh7428d3b_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.7.2-py312h2e8e312_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/libexpat-2.6.2-h63175ca_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.2-hcfcfb64_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/msgspec-0.18.6-py312he70551f_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/mypy-1.9.0-py312he70551f_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/openssl-3.2.1-hcfcfb64_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.8-py312he70551f_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.3-h2628c8c_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.12-4_cp312.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/pywin32-306-py312h53d5487_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/pyzmq-26.0.0-py312h1ac6f91_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/tornado-6.4-py312he70551f_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hcf57466_18.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33130-h82b7239_18.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33130-hcb4865c_18.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.5-h63175ca_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
   py310:
     channels:
     - url: https://conda.anaconda.org/conda-forge/
     packages:
       linux-64:
       - conda: https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2
@@ -853,29 +1247,29 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyha804496_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.6.2-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-h807b86a_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h807b86a_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-hd590300_2.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.2-h2797004_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h7e041cc_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
@@ -908,16 +1302,16 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/uv-0.1.31-h0e8d75e_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/uv-0.1.32-h0e8d75e_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zstandard-0.22.0-py310h1275a96_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.5-hfc55251_0.conda
       linux-aarch64:
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/_openmp_mutex-4.5-2_gnu.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
@@ -940,29 +1334,29 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyha804496_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ld_impl_linux-aarch64-2.40-h2d8c526_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libexpat-2.6.2-h2f0025b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libffi-3.4.2-h3557bc0_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libgcc-ng-13.2.0-hf8544c7_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libglib-2.80.0-h9d8fbc1_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libglib-2.80.0-h9d8fbc1_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libgomp-13.2.0-hf8544c7_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libiconv-1.17-h31becfc_2.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libnsl-2.0.1-h31becfc_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libsqlite-3.45.2-h194ca79_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libstdcxx-ng-13.2.0-h9a76618_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libuuid-2.38.1-hb4cce97_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libxcrypt-4.4.36-h31becfc_1.conda
@@ -995,16 +1389,16 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/uv-0.1.31-hb6a771c_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/uv-0.1.32-hb6a771c_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/xz-5.2.6-h9cdd2b7_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/zstandard-0.22.0-py310h468e293_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/zstd-1.5.5-h4c53e97_0.conda
       osx-64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
@@ -1023,15 +1417,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
@@ -1066,16 +1460,16 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/uv-0.1.31-h2c5c2bd_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/uv-0.1.32-h2c5c2bd_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/zstandard-0.22.0-py310hd88f66e_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.5-h829000d_0.conda
       osx-arm64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
@@ -1094,15 +1488,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
@@ -1137,16 +1531,16 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/uv-0.1.31-h2b8f702_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/uv-0.1.32-h2b8f702_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zstandard-0.22.0-py310h6289e41_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zstd-1.5.5-h4f39d0f_0.conda
       win-64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda
@@ -1165,15 +1559,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
@@ -1207,18 +1601,18 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/win-64/uv-0.1.31-h7ea99a0_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/uv-0.1.32-h7ea99a0_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hcf57466_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33130-h82b7239_18.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33130-hcb4865c_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/zstandard-0.22.0-py310h0009e47_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.5-h12be248_0.conda
   py311:
     channels:
@@ -1247,29 +1641,29 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyha804496_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.6.2-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-h807b86a_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h807b86a_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-hd590300_2.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.2-h2797004_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h7e041cc_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
@@ -1302,16 +1696,16 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/uv-0.1.31-h0e8d75e_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/uv-0.1.32-h0e8d75e_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zstandard-0.22.0-py311haa97af0_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.5-hfc55251_0.conda
       linux-aarch64:
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/_openmp_mutex-4.5-2_gnu.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
@@ -1334,29 +1728,29 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyha804496_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ld_impl_linux-aarch64-2.40-h2d8c526_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libexpat-2.6.2-h2f0025b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libffi-3.4.2-h3557bc0_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libgcc-ng-13.2.0-hf8544c7_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libglib-2.80.0-h9d8fbc1_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libglib-2.80.0-h9d8fbc1_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libgomp-13.2.0-hf8544c7_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libiconv-1.17-h31becfc_2.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libnsl-2.0.1-h31becfc_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libsqlite-3.45.2-h194ca79_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libstdcxx-ng-13.2.0-h9a76618_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libuuid-2.38.1-hb4cce97_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libxcrypt-4.4.36-h31becfc_1.conda
@@ -1389,16 +1783,16 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/uv-0.1.31-hb6a771c_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/uv-0.1.32-hb6a771c_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/xz-5.2.6-h9cdd2b7_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/zstandard-0.22.0-py311hb827a26_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/zstd-1.5.5-h4c53e97_0.conda
       osx-64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
@@ -1417,15 +1811,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
@@ -1461,16 +1855,16 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/uv-0.1.31-h2c5c2bd_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/uv-0.1.32-h2c5c2bd_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/zstandard-0.22.0-py311hed14148_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.5-h829000d_0.conda
       osx-arm64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
@@ -1489,15 +1883,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
@@ -1533,16 +1927,16 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/uv-0.1.31-h2b8f702_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/uv-0.1.32-h2b8f702_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zstandard-0.22.0-py311h67b91a1_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zstd-1.5.5-h4f39d0f_0.conda
       win-64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda
@@ -1561,15 +1955,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
@@ -1604,18 +1998,18 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/win-64/uv-0.1.31-h7ea99a0_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/uv-0.1.32-h7ea99a0_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hcf57466_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33130-h82b7239_18.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33130-hcb4865c_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/zstandard-0.22.0-py311he5d195f_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.5-h12be248_0.conda
   py312:
     channels:
@@ -1644,29 +2038,29 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyha804496_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.6.2-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-h807b86a_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h807b86a_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-hd590300_2.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.2-h2797004_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h7e041cc_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
@@ -1683,15 +2077,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.2-hab00c5b_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/secretstorage-3.3.3-py312h7900ff3_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
@@ -1699,16 +2093,16 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/uv-0.1.31-h0e8d75e_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/uv-0.1.32-h0e8d75e_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zstandard-0.22.0-py312hd58854c_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.5-hfc55251_0.conda
       linux-aarch64:
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/_openmp_mutex-4.5-2_gnu.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
@@ -1731,29 +2125,29 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyha804496_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ld_impl_linux-aarch64-2.40-h2d8c526_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libexpat-2.6.2-h2f0025b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libffi-3.4.2-h3557bc0_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libgcc-ng-13.2.0-hf8544c7_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libglib-2.80.0-h9d8fbc1_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libglib-2.80.0-h9d8fbc1_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libgomp-13.2.0-hf8544c7_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libiconv-1.17-h31becfc_2.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libnsl-2.0.1-h31becfc_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libsqlite-3.45.2-h194ca79_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libstdcxx-ng-13.2.0-h9a76618_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libuuid-2.38.1-hb4cce97_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libxcrypt-4.4.36-h31becfc_1.conda
@@ -1770,15 +2164,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.2-h43d1f9e_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.3-h43d1f9e_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/readline-8.2-h8fc344f_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/secretstorage-3.3.3-py312h8025657_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/tk-8.6.13-h194ca79_0.conda
@@ -1786,16 +2180,16 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/uv-0.1.31-hb6a771c_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/uv-0.1.32-hb6a771c_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/xz-5.2.6-h9cdd2b7_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/zstandard-0.22.0-py312hb120188_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/zstd-1.5.5-h4c53e97_0.conda
       osx-64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
@@ -1814,15 +2208,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
@@ -1843,31 +2237,31 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.2-h9f0c242_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/uv-0.1.31-h2c5c2bd_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/uv-0.1.32-h2c5c2bd_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/zstandard-0.22.0-py312h7a629f7_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.5-h829000d_0.conda
       osx-arm64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
@@ -1886,15 +2280,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
@@ -1915,31 +2309,31 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.2-hdf0ec26_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.3-h4a7b5fc_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/uv-0.1.31-h2b8f702_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/uv-0.1.32-h2b8f702_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zstandard-0.22.0-py312h7975427_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zstd-1.5.5-h4f39d0f_0.conda
       win-64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda
@@ -1958,15 +2352,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
@@ -1985,15 +2379,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.2-h2628c8c_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.3-h2628c8c_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/pywin32-ctypes-0.2.2-py312h2e8e312_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
@@ -2001,18 +2395,18 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/win-64/uv-0.1.31-h7ea99a0_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/uv-0.1.32-h7ea99a0_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hcf57466_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33130-h82b7239_18.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33130-hcb4865c_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/zstandard-0.22.0-py312h01d794b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.5-h12be248_0.conda
   py38:
     channels:
@@ -2041,29 +2435,29 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyha804496_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.6.2-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-h807b86a_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h807b86a_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-hd590300_2.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.2-h2797004_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h7e041cc_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
@@ -2095,16 +2489,16 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/uv-0.1.31-h0e8d75e_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/uv-0.1.32-h0e8d75e_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zstandard-0.22.0-py38ha98ab4e_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.5-hfc55251_0.conda
       linux-aarch64:
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/_openmp_mutex-4.5-2_gnu.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
@@ -2127,29 +2521,29 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyha804496_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ld_impl_linux-aarch64-2.40-h2d8c526_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libexpat-2.6.2-h2f0025b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libffi-3.4.2-h3557bc0_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libgcc-ng-13.2.0-hf8544c7_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libglib-2.80.0-h9d8fbc1_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libglib-2.80.0-h9d8fbc1_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libgomp-13.2.0-hf8544c7_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libiconv-1.17-h31becfc_2.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libnsl-2.0.1-h31becfc_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libsqlite-3.45.2-h194ca79_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libstdcxx-ng-13.2.0-h9a76618_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libuuid-2.38.1-hb4cce97_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libxcrypt-4.4.36-h31becfc_1.conda
@@ -2181,16 +2575,16 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/uv-0.1.31-hb6a771c_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/uv-0.1.32-hb6a771c_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/xz-5.2.6-h9cdd2b7_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/zstandard-0.22.0-py38hc2e9a1f_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/zstd-1.5.5-h4c53e97_0.conda
       osx-64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
@@ -2209,15 +2603,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
@@ -2251,16 +2645,16 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/uv-0.1.31-h2c5c2bd_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/uv-0.1.32-h2c5c2bd_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/zstandard-0.22.0-py38hca591b5_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.5-h829000d_0.conda
       osx-arm64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
@@ -2279,15 +2673,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
@@ -2321,16 +2715,16 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/uv-0.1.31-h2b8f702_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/uv-0.1.32-h2b8f702_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zstandard-0.22.0-py38h3d64ec1_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zstd-1.5.5-h4f39d0f_0.conda
       win-64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda
@@ -2349,15 +2743,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
@@ -2390,18 +2784,18 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/win-64/uv-0.1.31-h7ea99a0_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/uv-0.1.32-h7ea99a0_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hcf57466_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33130-h82b7239_18.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33130-hcb4865c_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/zstandard-0.22.0-py38hea8d35e_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.5-h12be248_0.conda
   py39:
     channels:
@@ -2430,29 +2824,29 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyha804496_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.6.2-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-h807b86a_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h807b86a_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libiconv-1.17-hd590300_2.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.2-h2797004_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h7e041cc_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
@@ -2485,16 +2879,16 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/uv-0.1.31-h0e8d75e_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/uv-0.1.32-h0e8d75e_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zstandard-0.22.0-py39h6e5214e_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.5-hfc55251_0.conda
       linux-aarch64:
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/_openmp_mutex-4.5-2_gnu.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
@@ -2517,29 +2911,29 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/keyring-25.1.0-pyha804496_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ld_impl_linux-aarch64-2.40-h2d8c526_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libexpat-2.6.2-h2f0025b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libffi-3.4.2-h3557bc0_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libgcc-ng-13.2.0-hf8544c7_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libglib-2.80.0-h9d8fbc1_4.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libglib-2.80.0-h9d8fbc1_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libgomp-13.2.0-hf8544c7_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libiconv-1.17-h31becfc_2.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libnsl-2.0.1-h31becfc_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libsqlite-3.45.2-h194ca79_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libstdcxx-ng-13.2.0-h9a76618_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libuuid-2.38.1-hb4cce97_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libxcrypt-4.4.36-h31becfc_1.conda
@@ -2572,16 +2966,16 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/uv-0.1.31-hb6a771c_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/uv-0.1.32-hb6a771c_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/xz-5.2.6-h9cdd2b7_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/zstandard-0.22.0-py39h1b5d086_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/zstd-1.5.5-h4c53e97_0.conda
       osx-64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
@@ -2600,15 +2994,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
@@ -2643,16 +3037,16 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/uv-0.1.31-h2c5c2bd_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/uv-0.1.32-h2c5c2bd_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/zstandard-0.22.0-py39h7211f3f_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.5-h829000d_0.conda
       osx-arm64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
@@ -2671,15 +3065,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
@@ -2714,16 +3108,16 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/uv-0.1.31-h2b8f702_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/uv-0.1.32-h2b8f702_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zstandard-0.22.0-py39h4818f0e_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zstd-1.5.5-h4f39d0f_0.conda
       win-64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda
@@ -2742,15 +3136,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatch-1.9.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hatchling-1.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hpack-4.0.0-pyh9f0ad1d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpcore-1.0.5-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/httpx-0.27.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperframe-6.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/hyperlink-21.0.0-pyhd3deb0d_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-7.1.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/importlib_resources-6.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.context-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/jaraco.functools-4.0.0-pyhd8ed1ab_0.conda
@@ -2784,18 +3178,18 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-w-1.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.4-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.4.10-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/win-64/uv-0.1.31-h7ea99a0_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/uv-0.1.32-h7ea99a0_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hcf57466_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33130-h82b7239_18.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33130-hcb4865c_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/zstandard-0.22.0-py39h95af829_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/zstd-1.5.5-h12be248_0.conda
   ruff:
     channels:
@@ -2815,15 +3209,15 @@
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.2-h2797004_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h7e041cc_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4.20240210-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.2-hab00c5b_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ruff-0.3.7-py312h9118e91_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
       linux-aarch64:
@@ -2839,15 +3233,15 @@
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libsqlite-3.45.2-h194ca79_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libstdcxx-ng-13.2.0-h9a76618_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libuuid-2.38.1-hb4cce97_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libxcrypt-4.4.36-h31becfc_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libzlib-1.2.13-h31becfc_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ncurses-6.4.20240210-h0425590_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/openssl-3.2.1-h31becfc_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.2-h43d1f9e_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.3-h43d1f9e_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/readline-8.2-h8fc344f_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ruff-0.3.7-py312hb434743_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/tk-8.6.13-h194ca79_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/xz-5.2.6-h9cdd2b7_0.tar.bz2
       osx-64:
@@ -2856,15 +3250,15 @@
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libexpat-2.6.2-h73e2aa4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.2-h92b6c6a_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4.20240210-h73e2aa4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.2.1-hd75f5a5_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.2-h9f0c242_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ruff-0.3.7-py312h1bc86af_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
       osx-arm64:
@@ -2873,30 +3267,30 @@
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libcxx-16.0.6-h4653b0c_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libexpat-2.6.2-hebf3989_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libffi-3.4.2-h3422bc3_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libsqlite-3.45.2-h091b4b1_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libzlib-1.2.13-h53f4e23_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ncurses-6.4.20240210-h078ce10_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.2.1-h0d3ecfb_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.2-hdf0ec26_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.3-h4a7b5fc_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ruff-0.3.7-py312h1ae9fbf_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
       win-64:
       - conda: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libexpat-2.6.2-h63175ca_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.2-hcfcfb64_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/openssl-3.2.1-hcfcfb64_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.2-h2628c8c_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.3-h2628c8c_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ruff-0.3.7-py312h60fbdae_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hcf57466_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33130-h82b7239_18.conda
@@ -2927,15 +3321,15 @@
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4.20240210-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.2-hab00c5b_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
@@ -2959,15 +3353,15 @@
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libzlib-1.2.13-h31becfc_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ncurses-6.4.20240210-h0425590_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/openssl-3.2.1-h31becfc_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.2-h43d1f9e_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.3-h43d1f9e_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/readline-8.2-h8fc344f_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/tk-8.6.13-h194ca79_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/xz-5.2.6-h9cdd2b7_0.tar.bz2
@@ -2984,15 +3378,15 @@
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4.20240210-h73e2aa4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.2.1-hd75f5a5_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.2-h9f0c242_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
@@ -3009,15 +3403,15 @@
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libzlib-1.2.13-h53f4e23_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ncurses-6.4.20240210-h078ce10_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.2.1-h0d3ecfb_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.2-hdf0ec26_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.3-h4a7b5fc_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
@@ -3033,15 +3427,15 @@
       - conda: https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.2-hcfcfb64_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/openssl-3.2.1-hcfcfb64_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.4.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.1.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.2-h2628c8c_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.3-h2628c8c_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hcf57466_18.conda
@@ -3138,14 +3532,49 @@
   - trio >=0.23
   - uvloop >=0.17
   license: MIT
   license_family: MIT
   size: 102331
   timestamp: 1708355504396
 - kind: conda
+  name: appnope
+  version: 0.1.4
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.4-pyhd8ed1ab_0.conda
+  sha256: 45ae2d41f4a4dcf8707633d3d7ae376fc62f0c09b1d063c3049c3f6f8c911670
+  md5: cc4834a9ee7cc49ce8d25177c47b10d8
+  depends:
+  - python >=3.7
+  license: BSD-2-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/appnope
+  size: 10241
+  timestamp: 1707233195627
+- kind: conda
+  name: asttokens
+  version: 2.4.1
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
+  sha256: 708168f026df19a0344983754d27d1f7b28bb21afc7b97a82f02c4798a3d2111
+  md5: 5f25798dcefd8252ce5f9dc494d5f571
+  depends:
+  - python >=3.5
+  - six >=1.12.0
+  license: Apache-2.0
+  license_family: Apache
+  purls:
+  - pkg:pypi/asttokens
+  size: 28922
+  timestamp: 1698341257884
+- kind: conda
   name: bzip2
   version: 1.0.8
   build: h10d778d_5
   build_number: 5
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
   sha256: 61fb2b488928a54d9472113e1280b468a309561caa54f33825a3593da390b242
@@ -3948,14 +4377,32 @@
   depends:
   - python >=3.7
   license: BSD-3-Clause
   license_family: BSD
   size: 25170
   timestamp: 1666700778190
 - kind: conda
+  name: comm
+  version: 0.2.2
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/comm-0.2.2-pyhd8ed1ab_0.conda
+  sha256: e923acf02708a8a0b591f3bce4bdc11c8e63b73198b99b35fe6cd96bfb6a0dbe
+  md5: 948d84721b578d426294e17a02e24cbb
+  depends:
+  - python >=3.6
+  - traitlets >=5.3
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/comm
+  size: 12134
+  timestamp: 1710320435158
+- kind: conda
   name: coverage
   version: 7.4.4
   build: py310h2372a71_0
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/coverage-7.4.4-py310h2372a71_0.conda
   sha256: e95f08ca0f555a5e16e7ef800317e04a237ef6622073d1c9dfb8792a06d28336
   md5: 2d948842110ae68e4f2e7738f92bf7e1
@@ -4734,14 +5181,132 @@
   - libgcc-ng >=9.4.0
   - libglib >=2.70.2,<3.0a0
   license: GPL-2.0-or-later
   license_family: GPL
   size: 618596
   timestamp: 1640112124844
 - kind: conda
+  name: debugpy
+  version: 1.8.1
+  build: py312h20a0b95_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/debugpy-1.8.1-py312h20a0b95_0.conda
+  sha256: d8ae528ddf391511387bb4c67d7dd4ad3cb808ee9b093429379803cf58a13807
+  md5: d850abbd9eeedbe2e734e397038f3f76
+  depends:
+  - libcxx >=16
+  - python >=3.12,<3.13.0a0
+  - python >=3.12,<3.13.0a0 *_cpython
+  - python_abi 3.12.* *_cp312
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/debugpy
+  - pkg:pypi/bytecode
+  size: 2077038
+  timestamp: 1707445014387
+- kind: conda
+  name: debugpy
+  version: 1.8.1
+  build: py312h2aa54b4_0
+  subdir: linux-aarch64
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/debugpy-1.8.1-py312h2aa54b4_0.conda
+  sha256: 42b00c41fec969ef118e46ff966c4a3f1d1cbedf88edfb55a3deaccd726333e1
+  md5: 2893bc781f67a580ad93f32f56c921e7
+  depends:
+  - libgcc-ng >=12
+  - libstdcxx-ng >=12
+  - python >=3.12,<3.13.0a0
+  - python >=3.12,<3.13.0a0 *_cpython
+  - python_abi 3.12.* *_cp312
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/debugpy
+  - pkg:pypi/bytecode
+  size: 2089528
+  timestamp: 1707444654939
+- kind: conda
+  name: debugpy
+  version: 1.8.1
+  build: py312h30efb56_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.8.1-py312h30efb56_0.conda
+  sha256: 8a8bd15c7a8435991649ab334816d4d64970c5b0d016f59806bc45f54f31a924
+  md5: bdd639417094ace2fb1ce10b20d68d5d
+  depends:
+  - libgcc-ng >=12
+  - libstdcxx-ng >=12
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/debugpy
+  - pkg:pypi/bytecode
+  size: 2079306
+  timestamp: 1707444570818
+- kind: conda
+  name: debugpy
+  version: 1.8.1
+  build: py312h53d5487_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/debugpy-1.8.1-py312h53d5487_0.conda
+  sha256: 5e8beecf42088481c88aa97118c52b2142f0e0d48ffed877e973c309c7fc83af
+  md5: 4094ccb019f079de8b0f61a5f366d294
+  depends:
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/bytecode
+  - pkg:pypi/debugpy
+  size: 3105043
+  timestamp: 1707445249662
+- kind: conda
+  name: debugpy
+  version: 1.8.1
+  build: py312hede676d_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/debugpy-1.8.1-py312hede676d_0.conda
+  sha256: f957393cb09e3df00176079253e0f845ab8c87dbca3c38e1a14df21ffe9d7083
+  md5: e0de4e018d6013b6c2e2ae42640fb65c
+  depends:
+  - libcxx >=16
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/debugpy
+  - pkg:pypi/bytecode
+  size: 2065572
+  timestamp: 1707444822563
+- kind: conda
+  name: decorator
+  version: 5.1.1
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2
+  sha256: 328a6a379f9bdfd0230e51de291ce858e6479411ea4b0545fb377c71662ef3e2
+  md5: 43afe5ab04e35e17ba28649471dd7364
+  depends:
+  - python >=3.5
+  license: BSD-2-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/decorator
+  size: 12072
+  timestamp: 1641555714315
+- kind: conda
   name: distlib
   version: 0.3.8
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/distlib-0.3.8-pyhd8ed1ab_0.conda
   sha256: 3ff11acdd5cc2f80227682966916e878e45ced94f59c402efb94911a5774e84e
@@ -4830,14 +5395,31 @@
   md5: 8d652ea2ee8eaee02ed8dc820bc794aa
   depends:
   - python >=3.7
   license: MIT and PSF-2.0
   size: 20551
   timestamp: 1704921321122
 - kind: conda
+  name: executing
+  version: 2.0.1
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/executing-2.0.1-pyhd8ed1ab_0.conda
+  sha256: c738804ab1e6376f8ea63372229a04c8d658dc90fd5a218c6273a2eaf02f4057
+  md5: e16be50e378d8a4533b989035b196ab8
+  depends:
+  - python >=2.7
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/executing
+  size: 27689
+  timestamp: 1698580072627
+- kind: conda
   name: expat
   version: 2.6.2
   build: h2f0025b_0
   subdir: linux-aarch64
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/expat-2.6.2-h2f0025b_0.conda
   sha256: a7a998faf6b9ed71d8c5c67f996e7faa52a7b9b02ed2d2f2ab6cfa1db8e5aca4
   md5: 6d31100ba1e12773b4f1ef0693fb0169
@@ -5249,44 +5831,44 @@
   - python
   license: MIT
   license_family: MIT
   size: 72732
   timestamp: 1610092261086
 - kind: conda
   name: idna
-  version: '3.6'
+  version: '3.7'
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
-  url: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
-  sha256: 6ee4c986d69ce61e60a20b2459b6f2027baeba153f0a64995fd3cb47c2cc7e07
-  md5: 1a76f09108576397c41c0b0c5bd84134
+  url: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
+  sha256: 9687ee909ed46169395d4f99a0ee94b80a52f87bed69cd454bb6d37ffeb0ec7b
+  md5: c0cc1420498b17414d8617d0b9f506ca
   depends:
   - python >=3.6
   license: BSD-3-Clause
   license_family: BSD
   purls:
   - pkg:pypi/idna
-  size: 50124
-  timestamp: 1701027126206
+  size: 52718
+  timestamp: 1713279497047
 - kind: conda
   name: idna
-  version: '3.6'
+  version: '3.7'
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
-  url: https://conda.anaconda.org/conda-forge/noarch/idna-3.6-pyhd8ed1ab_0.conda
-  sha256: 6ee4c986d69ce61e60a20b2459b6f2027baeba153f0a64995fd3cb47c2cc7e07
-  md5: 1a76f09108576397c41c0b0c5bd84134
+  url: https://conda.anaconda.org/conda-forge/noarch/idna-3.7-pyhd8ed1ab_0.conda
+  sha256: 9687ee909ed46169395d4f99a0ee94b80a52f87bed69cd454bb6d37ffeb0ec7b
+  md5: c0cc1420498b17414d8617d0b9f506ca
   depends:
   - python >=3.6
   license: BSD-3-Clause
   license_family: BSD
-  size: 50124
-  timestamp: 1701027126206
+  size: 52718
+  timestamp: 1713279497047
 - kind: conda
   name: importlib-metadata
   version: 7.1.0
   build: pyha770c72_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-7.1.0-pyha770c72_0.conda
@@ -5399,14 +5981,163 @@
   depends:
   - python >=3.7
   license: MIT
   license_family: MIT
   size: 11101
   timestamp: 1673103208955
 - kind: conda
+  name: ipykernel
+  version: 6.29.3
+  build: pyh3cd1d5f_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyh3cd1d5f_0.conda
+  sha256: ef2f9c1d83afd693db3793c368c5c6afcd37a416958ece490a2e1fbcd85012eb
+  md5: 28e74fca8d8abf09c1ed0d190a17e307
+  depends:
+  - __osx
+  - appnope
+  - comm >=0.1.1
+  - debugpy >=1.6.5
+  - ipython >=7.23.1
+  - jupyter_client >=6.1.12
+  - jupyter_core >=4.12,!=5.0.*
+  - matplotlib-inline >=0.1
+  - nest-asyncio
+  - packaging
+  - psutil
+  - python >=3.8
+  - pyzmq >=24
+  - tornado >=6.1
+  - traitlets >=5.4.0
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/ipykernel
+  size: 119602
+  timestamp: 1708996878886
+- kind: conda
+  name: ipykernel
+  version: 6.29.3
+  build: pyha63f2e9_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyha63f2e9_0.conda
+  sha256: 93ff46322a2512e9fb4ba456b1f0120d2f628a4b851f3102561a351e528d24d0
+  md5: d86f243bdd45a8019050e7326ed7bb2e
+  depends:
+  - __win
+  - comm >=0.1.1
+  - debugpy >=1.6.5
+  - ipython >=7.23.1
+  - jupyter_client >=6.1.12
+  - jupyter_core >=4.12,!=5.0.*
+  - matplotlib-inline >=0.1
+  - nest-asyncio
+  - packaging
+  - psutil
+  - python >=3.8
+  - pyzmq >=24
+  - tornado >=6.1
+  - traitlets >=5.4.0
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/ipykernel
+  size: 119670
+  timestamp: 1708996955969
+- kind: conda
+  name: ipykernel
+  version: 6.29.3
+  build: pyhd33586a_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.29.3-pyhd33586a_0.conda
+  sha256: 0314f15e666fd9a4fb653aae37d2cf4dc6bc3a18c0d9c2671a6a0783146adcfa
+  md5: e0deff12c601ce5cb7476f93718f3168
+  depends:
+  - __linux
+  - comm >=0.1.1
+  - debugpy >=1.6.5
+  - ipython >=7.23.1
+  - jupyter_client >=6.1.12
+  - jupyter_core >=4.12,!=5.0.*
+  - matplotlib-inline >=0.1
+  - nest-asyncio
+  - packaging
+  - psutil
+  - python >=3.8
+  - pyzmq >=24
+  - tornado >=6.1
+  - traitlets >=5.4.0
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/ipykernel
+  size: 119050
+  timestamp: 1708996727913
+- kind: conda
+  name: ipython
+  version: 8.22.2
+  build: pyh707e725_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/ipython-8.22.2-pyh707e725_0.conda
+  sha256: 7740505317669f094c881537a643ed26977e209510965164d84942799c997d42
+  md5: f0abe827c8a7c6d91bccdf90cb1fbee3
+  depends:
+  - __unix
+  - decorator
+  - exceptiongroup
+  - jedi >=0.16
+  - matplotlib-inline
+  - pexpect >4.3
+  - pickleshare
+  - prompt-toolkit >=3.0.41,<3.1.0
+  - pygments >=2.4.0
+  - python >=3.10
+  - stack_data
+  - traitlets >=5.13.0
+  - typing_extensions
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/ipython
+  size: 593746
+  timestamp: 1709559868257
+- kind: conda
+  name: ipython
+  version: 8.22.2
+  build: pyh7428d3b_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/ipython-8.22.2-pyh7428d3b_0.conda
+  sha256: f7196ab6d5251505fd5b9c6ff63694eff09be7959a0a3421b8c2336638de9aaf
+  md5: f803d121b60dff8f4d8f9264b7c6e8bf
+  depends:
+  - __win
+  - colorama
+  - decorator
+  - exceptiongroup
+  - jedi >=0.16
+  - matplotlib-inline
+  - pickleshare
+  - prompt-toolkit >=3.0.41,<3.1.0
+  - pygments >=2.4.0
+  - python >=3.10
+  - stack_data
+  - traitlets >=5.13.0
+  - typing_extensions
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/ipython
+  size: 593699
+  timestamp: 1709560407504
+- kind: conda
   name: jaraco.classes
   version: 3.4.0
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/jaraco.classes-3.4.0-pyhd8ed1ab_0.conda
   sha256: c44030b080f33299ec5eb5d47d1be30277cd55859701d67b1b6e4e38f4b5bf06
@@ -5499,14 +6230,32 @@
   - more-itertools
   - python >=3.8
   license: MIT
   license_family: MIT
   size: 15192
   timestamp: 1701695329516
 - kind: conda
+  name: jedi
+  version: 0.19.1
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/jedi-0.19.1-pyhd8ed1ab_0.conda
+  sha256: 362f0936ef37dfd1eaa860190e42a6ebf8faa094eaa3be6aa4d9ace95f40047a
+  md5: 81a3be0b2023e1ea8555781f0ad904a2
+  depends:
+  - parso >=0.8.3,<0.9.0
+  - python >=3.6
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/jedi
+  size: 841312
+  timestamp: 1696326218364
+- kind: conda
   name: jeepney
   version: 0.8.0
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/jeepney-0.8.0-pyhd8ed1ab_0.tar.bz2
   sha256: 16639759b811866d63315fe1391f6fb45f5478b823972f4d3d9f0392b7dd80b8
@@ -6025,51 +6774,51 @@
   license: GPL-3.0-only WITH GCC-exception-3.1
   license_family: GPL
   size: 456795
   timestamp: 1706820691781
 - kind: conda
   name: libglib
   version: 2.80.0
-  build: h9d8fbc1_4
-  build_number: 4
+  build: h9d8fbc1_5
+  build_number: 5
   subdir: linux-aarch64
-  url: https://conda.anaconda.org/conda-forge/linux-aarch64/libglib-2.80.0-h9d8fbc1_4.conda
-  sha256: 2d6e2315a592276b9ca03aa9a6dabd5348f627ab924b68eda06cf3d4acfbf82d
-  md5: b4772c0eb20b89e6866b46d9ffa66242
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/libglib-2.80.0-h9d8fbc1_5.conda
+  sha256: 9bb8ae5233e3100f4885d4032d696547709f16bbdf63a58ddf19ba430c360c24
+  md5: 9018b2472d16a309479f408ec9e15d21
   depends:
   - libffi >=3.4,<4.0a0
   - libgcc-ng >=12
   - libiconv >=1.17,<2.0a0
   - libzlib >=1.2.13,<1.3.0a0
   - pcre2 >=10.43,<10.44.0a0
   constrains:
-  - glib 2.80.0 *_4
+  - glib 2.80.0 *_5
   license: LGPL-2.1-or-later
-  size: 2990202
-  timestamp: 1712589847250
+  size: 2947036
+  timestamp: 1713203504849
 - kind: conda
   name: libglib
   version: 2.80.0
-  build: hf2295e7_4
-  build_number: 4
+  build: hf2295e7_5
+  build_number: 5
   subdir: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_4.conda
-  sha256: 99983c2514dd99da1bab50e9a25ed16cfc1d46aca0385c3be177c8e299731b51
-  md5: 0269d2b7fa89f4a37cdee5ad6161f6cc
+  url: https://conda.anaconda.org/conda-forge/linux-64/libglib-2.80.0-hf2295e7_5.conda
+  sha256: 18233d83e0385afc50148520e5b9c6ee65886c41ecdc69e335f60a279fb7a1f5
+  md5: 4423ae9726113b68e9527b27baae191f
   depends:
   - libffi >=3.4,<4.0a0
   - libgcc-ng >=12
   - libiconv >=1.17,<2.0a0
   - libzlib >=1.2.13,<1.3.0a0
   - pcre2 >=10.43,<10.44.0a0
   constrains:
-  - glib 2.80.0 *_4
+  - glib 2.80.0 *_5
   license: LGPL-2.1-or-later
-  size: 2900260
-  timestamp: 1712589943666
+  size: 3892640
+  timestamp: 1713203313894
 - kind: conda
   name: libgomp
   version: 13.2.0
   build: h807b86a_5
   build_number: 5
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h807b86a_5.conda
@@ -6482,14 +7231,32 @@
   - mdurl >=0.1,<1
   - python >=3.8
   license: MIT
   license_family: MIT
   size: 64356
   timestamp: 1686175179621
 - kind: conda
+  name: matplotlib-inline
+  version: 0.1.7
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
+  sha256: 7ea68676ea35fbb095420bbcc1c82c4767b8be7bb56abb6989b7f89d957a3bab
+  md5: 779345c95648be40d22aaa89de7d4254
+  depends:
+  - python >=3.6
+  - traitlets
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/matplotlib-inline
+  size: 14599
+  timestamp: 1713250613726
+- kind: conda
   name: mdurl
   version: 0.1.2
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda
   sha256: 64073dfb6bb429d52fff30891877b48c7ec0f89625b1bf844905b66a81cce6e1
@@ -6638,14 +7405,143 @@
   license: BSD-3-Clause
   license_family: BSD
   purls:
   - pkg:pypi/msgspec
   size: 195057
   timestamp: 1705902299019
 - kind: conda
+  name: mypy
+  version: 1.9.0
+  build: py312h41838bb_1
+  build_number: 1
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/mypy-1.9.0-py312h41838bb_1.conda
+  sha256: baac423f3b881efa351ccbcf40537fd6c3814f57fc77584cc0eca1bf08d21228
+  md5: be0026dcebe836ef612292be62dd600c
+  depends:
+  - mypy_extensions >=1.0.0
+  - psutil >=4.0
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  - typing_extensions >=4.1.0
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/mypy
+  size: 10225966
+  timestamp: 1713328828236
+- kind: conda
+  name: mypy
+  version: 1.9.0
+  build: py312h98912ed_1
+  build_number: 1
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/mypy-1.9.0-py312h98912ed_1.conda
+  sha256: a4bcb956e3c3faf401d1d7e3f578c96504c31a3ca0aa15623dccfeea3e25d271
+  md5: 26396161af12b4c016225bbab28c4579
+  depends:
+  - libgcc-ng >=12
+  - mypy_extensions >=1.0.0
+  - psutil >=4.0
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  - typing_extensions >=4.1.0
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/mypy
+  size: 16429118
+  timestamp: 1713328264160
+- kind: conda
+  name: mypy
+  version: 1.9.0
+  build: py312hdd3e373_1
+  build_number: 1
+  subdir: linux-aarch64
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/mypy-1.9.0-py312hdd3e373_1.conda
+  sha256: 2d959e391fab5a15ca4764cbf5737ba2c3549621c5b10ed7c1596b54ae629f17
+  md5: 036e12e05ab855daafa900b313d11246
+  depends:
+  - libgcc-ng >=12
+  - mypy_extensions >=1.0.0
+  - psutil >=4.0
+  - python >=3.12,<3.13.0a0
+  - python >=3.12,<3.13.0a0 *_cpython
+  - python_abi 3.12.* *_cp312
+  - typing_extensions >=4.1.0
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/mypy
+  size: 15319745
+  timestamp: 1713328656031
+- kind: conda
+  name: mypy
+  version: 1.9.0
+  build: py312he37b823_1
+  build_number: 1
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/mypy-1.9.0-py312he37b823_1.conda
+  sha256: 28b72d1c4df707c0e5400a652c592c292f4b3562ede6eeb1b6a2ce93ae06e144
+  md5: 43c2b6d571580d838a4cd24271681dde
+  depends:
+  - mypy_extensions >=1.0.0
+  - psutil >=4.0
+  - python >=3.12,<3.13.0a0
+  - python >=3.12,<3.13.0a0 *_cpython
+  - python_abi 3.12.* *_cp312
+  - typing_extensions >=4.1.0
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/mypy
+  size: 9537682
+  timestamp: 1713328977513
+- kind: conda
+  name: mypy
+  version: 1.9.0
+  build: py312he70551f_1
+  build_number: 1
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/mypy-1.9.0-py312he70551f_1.conda
+  sha256: 18808d80f4b978b56a9273bac64f9c18c1fb34058209419ab3d3b28b8ce06e05
+  md5: b1c28d607b091d640dc1f25ea533c343
+  depends:
+  - mypy_extensions >=1.0.0
+  - psutil >=4.0
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  - typing_extensions >=4.1.0
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/mypy
+  size: 8291302
+  timestamp: 1713328258213
+- kind: conda
+  name: mypy_extensions
+  version: 1.0.0
+  build: pyha770c72_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda
+  sha256: f240217476e148e825420c6bc3a0c0efb08c0718b7042fae960400c02af858a3
+  md5: 4eccaeba205f0aed9ac3a9ea58568ca3
+  depends:
+  - python >=3.5
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/mypy-extensions
+  size: 10492
+  timestamp: 1675543414256
+- kind: conda
   name: ncurses
   version: 6.4.20240210
   build: h0425590_0
   subdir: linux-aarch64
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/ncurses-6.4.20240210-h0425590_0.conda
   sha256: 4223dc34e2bddd37bf995158ae481e00be375b287d539bc7a0532634c0fc63b7
   md5: c1a1612ddaee95c83abfa0b2ec858626
@@ -6686,14 +7582,31 @@
   url: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4.20240210-h73e2aa4_0.conda
   sha256: 50b72acf08acbc4e5332807653e2ca6b26d4326e8af16fad1fd3f2ce9ea55503
   md5: 50f28c512e9ad78589e3eab34833f762
   license: X11 AND BSD-3-Clause
   size: 823010
   timestamp: 1710866856626
 - kind: conda
+  name: nest-asyncio
+  version: 1.6.0
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
+  sha256: 30db21d1f7e59b3408b831a7e0417b83b53ee6223afae56482c5f26da3ceb49a
+  md5: 6598c056f64dc8800d40add25e4e2c34
+  depends:
+  - python >=3.5
+  license: BSD-2-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/nest-asyncio
+  size: 11638
+  timestamp: 1705850780510
+- kind: conda
   name: openssl
   version: 3.2.1
   build: h0d3ecfb_1
   build_number: 1
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.2.1-h0d3ecfb_1.conda
   sha256: 519dc941d7ab0ebf31a2878d85c2f444450e7c5f6f41c4d07252c6bb3417b78b
@@ -6808,14 +7721,31 @@
   depends:
   - python >=3.8
   license: Apache-2.0
   license_family: APACHE
   size: 49832
   timestamp: 1710076089469
 - kind: conda
+  name: parso
+  version: 0.8.4
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
+  sha256: bfe404eebb930cc41782d34f8fc04c0388ea692eeebe2c5fc28df8ec8d4d61ae
+  md5: 81534b420deb77da8833f2289b8d47ac
+  depends:
+  - python >=3.6
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/parso
+  size: 75191
+  timestamp: 1712320447201
+- kind: conda
   name: pathspec
   version: 0.12.1
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
   sha256: 4e534e66bfe8b1e035d2169d0e5b185450546b17e36764272863e22e0370be4d
@@ -6903,20 +7833,39 @@
   md5: 629f3203c99b32e0988910c93e77f3b6
   depends:
   - ptyprocess >=0.5
   - python >=3.7
   license: ISC
   size: 53600
   timestamp: 1706113273252
+- kind: conda
+  name: pickleshare
+  version: 0.7.5
+  build: py_1003
+  build_number: 1003
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
+  sha256: a1ed1a094dd0d1b94a09ed85c283a0eb28943f2e6f22161fb45e128d35229738
+  md5: 415f0ebb6198cc2801c73438a9fb5761
+  depends:
+  - python >=3
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/pickleshare
+  size: 9332
+  timestamp: 1602536313357
 - kind: pypi
   name: pixi-kernel
-  version: 0.2.1
+  version: 0.3.0
   path: .
-  sha256: fc89be37749334e0eb20e8656e5ffcdace662e69fd273fa798213fdf1e64b7cb
+  sha256: 026726c0f08b63327906964394fdaf6d1b2324c25bf50c37e37b0300731fba40
   requires_dist:
+  - ipykernel >=6
   - jupyter-client >=7
   - msgspec >=0.18
   requires_python: <4.0,>=3.8
   editable: true
 - kind: conda
   name: platformdirs
   version: 4.2.0
@@ -6978,14 +7927,126 @@
   depends:
   - python >=3.8
   license: MIT
   license_family: MIT
   size: 23384
   timestamp: 1706116931972
 - kind: conda
+  name: prompt-toolkit
+  version: 3.0.42
+  build: pyha770c72_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
+  sha256: 58525b2a9305fb154b2b0d43a48b9a6495441b80e4fbea44f2a34a597d2cef16
+  md5: 0bf64bf10eee21f46ac83c161917fa86
+  depends:
+  - python >=3.7
+  - wcwidth
+  constrains:
+  - prompt_toolkit 3.0.42
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/prompt-toolkit
+  size: 270398
+  timestamp: 1702399557137
+- kind: conda
+  name: psutil
+  version: 5.9.8
+  build: py312h41838bb_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.8-py312h41838bb_0.conda
+  sha256: 12e5053d19bddaf7841e59cbe9ba98fa5d4d8502ceccddad80888515e1366107
+  md5: 03926e7089a5e61b77043b470ae7b553
+  depends:
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/psutil
+  size: 495162
+  timestamp: 1705722685887
+- kind: conda
+  name: psutil
+  version: 5.9.8
+  build: py312h98912ed_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.8-py312h98912ed_0.conda
+  sha256: 27e7f8f5d30c74439f39d61e21ac14c0cd03b5d55f7bf9f946fb619016f73c61
+  md5: 3facaca6cc0f7988df3250efccd32da3
+  depends:
+  - libgcc-ng >=12
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/psutil
+  size: 486243
+  timestamp: 1705722547420
+- kind: conda
+  name: psutil
+  version: 5.9.8
+  build: py312hdd3e373_0
+  subdir: linux-aarch64
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/psutil-5.9.8-py312hdd3e373_0.conda
+  sha256: 21466ab2102ee041dc11805e0d8e7354782beccf49df2bfa366758e3ceae6c70
+  md5: 1a87f588762a48fb42311b0c40fa1920
+  depends:
+  - libgcc-ng >=12
+  - python >=3.12,<3.13.0a0
+  - python >=3.12,<3.13.0a0 *_cpython
+  - python_abi 3.12.* *_cp312
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/psutil
+  size: 489623
+  timestamp: 1705722741120
+- kind: conda
+  name: psutil
+  version: 5.9.8
+  build: py312he37b823_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/psutil-5.9.8-py312he37b823_0.conda
+  sha256: a996bd5f878da264d1d3ba7fde717b0a2c158a86645efb1e899d087cca74832d
+  md5: cd6e99b9c5a623735161973b5f693a86
+  depends:
+  - python >=3.12,<3.13.0a0
+  - python >=3.12,<3.13.0a0 *_cpython
+  - python_abi 3.12.* *_cp312
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/psutil
+  size: 499490
+  timestamp: 1705722767772
+- kind: conda
+  name: psutil
+  version: 5.9.8
+  build: py312he70551f_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.8-py312he70551f_0.conda
+  sha256: 36f8addb327f80da4d6bd421170ff4cf8fb570d9ee8df39372427a4e33298dca
+  md5: 5f2998851564bea33a159bd00e6249e8
+  depends:
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  license: BSD-3-Clause
+  license_family: BSD
+  purls:
+  - pkg:pypi/psutil
+  size: 503677
+  timestamp: 1705722843679
+- kind: conda
   name: ptyprocess
   version: 0.7.0
   build: pyhd3deb0d_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
   sha256: fb31e006a25eb2e18f3440eb8d17be44c8ccfae559499199f73584566d0a444a
@@ -7008,14 +8069,31 @@
   md5: 359eeb6536da0e687af562ed265ec263
   depends:
   - python
   license: ISC
   size: 16546
   timestamp: 1609419417991
 - kind: conda
+  name: pure_eval
+  version: 0.2.2
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
+  sha256: 72792f9fc2b1820e37cc57f84a27bc819c71088c3002ca6db05a2e56404f9d44
+  md5: 6784285c7e55cb7212efabc79e4c2883
+  depends:
+  - python >=3.5
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/pure-eval
+  size: 14551
+  timestamp: 1642876055775
+- kind: conda
   name: pycparser
   version: '2.22'
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
   sha256: 406001ebf017688b1a1554b49127ca3a4ac4626ec0fd51dc75ffa4415b720b64
@@ -7680,148 +8758,150 @@
   constrains:
   - python_abi 3.11.* *_cp311
   license: Python-2.0
   size: 14623079
   timestamp: 1708116925163
 - kind: conda
   name: python
-  version: 3.12.2
+  version: 3.12.3
+  build: h1411813_0_cpython
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda
+  sha256: 3b327ffc152a245011011d1d730781577a8274fde1cf6243f073749ead8f1c2a
+  md5: df1448ec6cbf8eceb03d29003cf72ae6
+  depends:
+  - __osx >=10.9
+  - bzip2 >=1.0.8,<2.0a0
+  - libexpat >=2.6.2,<3.0a0
+  - libffi >=3.4,<4.0a0
+  - libsqlite >=3.45.2,<4.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - ncurses >=6.4.20240210,<7.0a0
+  - openssl >=3.2.1,<4.0a0
+  - readline >=8.2,<9.0a0
+  - tk >=8.6.13,<8.7.0a0
+  - tzdata
+  - xz >=5.2.6,<6.0a0
+  constrains:
+  - python_abi 3.12.* *_cp312
+  license: Python-2.0
+  size: 14557341
+  timestamp: 1713208068012
+- kind: conda
+  name: python
+  version: 3.12.3
   build: h2628c8c_0_cpython
   subdir: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/python-3.12.2-h2628c8c_0_cpython.conda
-  sha256: b8eda863b48ae4531635e23fd15e759d93212b6204c6847d591e25fa5fd67477
-  md5: be8803e9f75a477df61d4aabea3c1246
+  url: https://conda.anaconda.org/conda-forge/win-64/python-3.12.3-h2628c8c_0_cpython.conda
+  sha256: 1a95494abe572a8819c933f978df89f00bde72ea9432d46a70632599e8029ea4
+  md5: f07c8c5dd98767f9a652de5d039b284e
   depends:
   - bzip2 >=1.0.8,<2.0a0
-  - libexpat >=2.5.0,<3.0a0
+  - libexpat >=2.6.2,<3.0a0
   - libffi >=3.4,<4.0a0
-  - libsqlite >=3.45.1,<4.0a0
+  - libsqlite >=3.45.2,<4.0a0
   - libzlib >=1.2.13,<1.3.0a0
   - openssl >=3.2.1,<4.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.12.* *_cp312
   license: Python-2.0
-  size: 16083296
-  timestamp: 1708116662336
+  size: 16179248
+  timestamp: 1713205644673
 - kind: conda
   name: python
-  version: 3.12.2
+  version: 3.12.3
   build: h43d1f9e_0_cpython
   subdir: linux-aarch64
-  url: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.2-h43d1f9e_0_cpython.conda
-  sha256: 16c8e77c01b814d836af632ef77eac21b64b9e398a11e1403a3a1802bb5be366
-  md5: 3a41090f2ef0868f119825593948ed46
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.3-h43d1f9e_0_cpython.conda
+  sha256: e186f3ee570464241c844adff6a3ba8f395cef15c5d46c0a8f784cfd97b3bdca
+  md5: dc93ad1d2ba17ebc948bf5434ffa864b
   depends:
   - bzip2 >=1.0.8,<2.0a0
   - ld_impl_linux-aarch64 >=2.36.1
-  - libexpat >=2.5.0,<3.0a0
+  - libexpat >=2.6.2,<3.0a0
   - libffi >=3.4,<4.0a0
   - libgcc-ng >=12
   - libnsl >=2.0.1,<2.1.0a0
-  - libsqlite >=3.45.1,<4.0a0
+  - libsqlite >=3.45.2,<4.0a0
   - libuuid >=2.38.1,<3.0a0
   - libxcrypt >=4.4.36
   - libzlib >=1.2.13,<1.3.0a0
-  - ncurses >=6.4,<7.0a0
+  - ncurses >=6.4.20240210,<7.0a0
   - openssl >=3.2.1,<4.0a0
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.12.* *_cp312
   license: Python-2.0
-  size: 13823577
-  timestamp: 1708116074721
+  size: 14051797
+  timestamp: 1713205211165
 - kind: conda
   name: python
-  version: 3.12.2
-  build: h9f0c242_0_cpython
-  subdir: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.2-h9f0c242_0_cpython.conda
-  sha256: 7647ac06c3798a182a4bcb1ff58864f1ef81eb3acea6971295304c23e43252fb
-  md5: 0179b8007ba008cf5bec11f3b3853902
+  version: 3.12.3
+  build: h4a7b5fc_0_cpython
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.3-h4a7b5fc_0_cpython.conda
+  sha256: c761fb3713ea66bce3889b33b6f400afb2dd192d1fc2686446e9d8166cfcec6b
+  md5: 8643ab37bece6ae8f112464068d9df9c
   depends:
+  - __osx >=11.0
   - bzip2 >=1.0.8,<2.0a0
-  - libexpat >=2.5.0,<3.0a0
+  - libexpat >=2.6.2,<3.0a0
   - libffi >=3.4,<4.0a0
-  - libsqlite >=3.45.1,<4.0a0
+  - libsqlite >=3.45.2,<4.0a0
   - libzlib >=1.2.13,<1.3.0a0
-  - ncurses >=6.4,<7.0a0
+  - ncurses >=6.4.20240210,<7.0a0
   - openssl >=3.2.1,<4.0a0
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.12.* *_cp312
   license: Python-2.0
-  size: 14596811
-  timestamp: 1708118065292
+  size: 13207557
+  timestamp: 1713206576646
 - kind: conda
   name: python
-  version: 3.12.2
+  version: 3.12.3
   build: hab00c5b_0_cpython
   subdir: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.2-hab00c5b_0_cpython.conda
-  sha256: ddb7a2d8d78046bda5d7631e6814f9468d2eb054e10f86f4648c9d1fdaa30c0f
-  md5: ad7b68400f3a6ebe72b00be093c7f301
+  url: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda
+  sha256: f9865bcbff69f15fd89a33a2da12ad616e98d65ce7c83c644b92e66e5016b227
+  md5: 2540b74d304f71d3e89c81209db4db84
   depends:
   - bzip2 >=1.0.8,<2.0a0
   - ld_impl_linux-64 >=2.36.1
-  - libexpat >=2.5.0,<3.0a0
+  - libexpat >=2.6.2,<3.0a0
   - libffi >=3.4,<4.0a0
   - libgcc-ng >=12
   - libnsl >=2.0.1,<2.1.0a0
-  - libsqlite >=3.45.1,<4.0a0
+  - libsqlite >=3.45.2,<4.0a0
   - libuuid >=2.38.1,<3.0a0
   - libxcrypt >=4.4.36
   - libzlib >=1.2.13,<1.3.0a0
-  - ncurses >=6.4,<7.0a0
-  - openssl >=3.2.1,<4.0a0
-  - readline >=8.2,<9.0a0
-  - tk >=8.6.13,<8.7.0a0
-  - tzdata
-  - xz >=5.2.6,<6.0a0
-  constrains:
-  - python_abi 3.12.* *_cp312
-  license: Python-2.0
-  size: 32312631
-  timestamp: 1708118077305
-- kind: conda
-  name: python
-  version: 3.12.2
-  build: hdf0ec26_0_cpython
-  subdir: osx-arm64
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.2-hdf0ec26_0_cpython.conda
-  sha256: ccd6c55a286d51d907c878ed2bfa7d1becce0fee71374a9386c5eb90d803ac72
-  md5: 85e91138ae921a2771f57a50120272bd
-  depends:
-  - bzip2 >=1.0.8,<2.0a0
-  - libexpat >=2.5.0,<3.0a0
-  - libffi >=3.4,<4.0a0
-  - libsqlite >=3.45.1,<4.0a0
-  - libzlib >=1.2.13,<1.3.0a0
-  - ncurses >=6.4,<7.0a0
+  - ncurses >=6.4.20240210,<7.0a0
   - openssl >=3.2.1,<4.0a0
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.12.* *_cp312
   license: Python-2.0
-  size: 13085901
-  timestamp: 1708117361381
+  size: 31991381
+  timestamp: 1713208036041
 - kind: conda
   name: python-dateutil
   version: 2.9.0
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
@@ -8328,114 +9408,117 @@
   - python_abi 3.9.* *_cp39
   license: BSD-3-Clause
   license_family: BSD
   size: 45564
   timestamp: 1695395311565
 - kind: conda
   name: pyzmq
-  version: 25.1.2
+  version: 26.0.0
   build: py312h1ac6f91_0
   subdir: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/pyzmq-25.1.2-py312h1ac6f91_0.conda
-  sha256: 9371101999c75aa562c5aa4ae0dfefa140bee635a3f8e15768628689f70d7765
-  md5: 74194f888cc7b11d8c18edf416b61a1b
+  url: https://conda.anaconda.org/conda-forge/win-64/pyzmq-26.0.0-py312h1ac6f91_0.conda
+  sha256: 8d12105518f4ae9bbf48bbdbe031a0b3f2c0b1378350422172af2afc77014f54
+  md5: c69d5948bed236b2cfa323dd478d8de8
   depends:
   - libsodium >=1.0.18,<1.0.19.0a0
   - python >=3.12,<3.13.0a0
   - python_abi 3.12.* *_cp312
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   - zeromq >=4.3.5,<4.3.6.0a0
-  license: BSD-3-Clause AND LGPL-3.0-or-later
+  license: BSD-3-Clause
+  license_family: BSD
   purls:
   - pkg:pypi/pyzmq
-  size: 480772
-  timestamp: 1701783863250
+  size: 444664
+  timestamp: 1713208522670
 - kind: conda
   name: pyzmq
-  version: 25.1.2
+  version: 26.0.0
   build: py312h1c32067_0
   subdir: linux-aarch64
-  url: https://conda.anaconda.org/conda-forge/linux-aarch64/pyzmq-25.1.2-py312h1c32067_0.conda
-  sha256: 7394b1de60b33bbe7fc62d67a838671777cfe725074332d61861457efa0c1f62
-  md5: 7b450f76fbf279bd05304bc9fd879ff0
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/pyzmq-26.0.0-py312h1c32067_0.conda
+  sha256: 5c87c69960aba5292df0e8ece531b97f294336c15d022d2efafb171ab080983d
+  md5: 7f6de7d76e5253bdf14a9088fec24f04
   depends:
   - libgcc-ng >=12
   - libsodium >=1.0.18,<1.0.19.0a0
   - libstdcxx-ng >=12
   - python >=3.12,<3.13.0a0
   - python_abi 3.12.* *_cp312
   - zeromq >=4.3.5,<4.4.0a0
-  license: BSD-3-Clause AND LGPL-3.0-or-later
+  license: BSD-3-Clause
+  license_family: BSD
   purls:
   - pkg:pypi/pyzmq
-  size: 530614
-  timestamp: 1701785140508
+  size: 457757
+  timestamp: 1713209766265
 - kind: conda
   name: pyzmq
-  version: 25.1.2
-  build: py312h1edf716_0
+  version: 26.0.0
+  build: py312h2105c20_0
   subdir: osx-arm64
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/pyzmq-25.1.2-py312h1edf716_0.conda
-  sha256: a89712c6b0cab1e3385e44e0130a57b9d03df99b6f540486c0f00e2dae079e77
-  md5: 913db29987f836f5d80fa319e36b0a33
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/pyzmq-26.0.0-py312h2105c20_0.conda
+  sha256: b76223afe36332ac6472f8a2ff63de0ed018d24dcb414447eda05e8df58ca0e5
+  md5: a5e9d370c646a0d4cefedc5d6c5048b9
   depends:
-  - __osx >=10.9
-  - libcxx >=16.0.6
+  - libcxx >=16
   - libsodium >=1.0.18,<1.0.19.0a0
   - python >=3.12,<3.13.0a0
   - python >=3.12,<3.13.0a0 *_cpython
   - python_abi 3.12.* *_cp312
   - zeromq >=4.3.5,<4.4.0a0
-  license: BSD-3-Clause AND LGPL-3.0-or-later
+  license: BSD-3-Clause
+  license_family: BSD
   purls:
   - pkg:pypi/pyzmq
-  size: 495070
-  timestamp: 1701783687130
+  size: 446510
+  timestamp: 1713208013885
 - kind: conda
   name: pyzmq
-  version: 25.1.2
+  version: 26.0.0
   build: py312h886d080_0
   subdir: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.2-py312h886d080_0.conda
-  sha256: 5aa0ba1f67e2b25ede34a713df6655e519211a96ea109857768930d96bcd0ca0
-  md5: cc2cdf8f1792d29d21e17024745813d8
+  url: https://conda.anaconda.org/conda-forge/linux-64/pyzmq-26.0.0-py312h886d080_0.conda
+  sha256: c7fadc44057fe38d3b403ad435d8612172b981f02a30e399213f94760837d19f
+  md5: c06e639885a14ea35f77e9c0f3918808
   depends:
   - libgcc-ng >=12
   - libsodium >=1.0.18,<1.0.19.0a0
   - libstdcxx-ng >=12
   - python >=3.12,<3.13.0a0
   - python_abi 3.12.* *_cp312
   - zeromq >=4.3.5,<4.4.0a0
-  license: BSD-3-Clause AND LGPL-3.0-or-later
+  license: BSD-3-Clause
+  license_family: BSD
   purls:
   - pkg:pypi/pyzmq
-  size: 528745
-  timestamp: 1701783368181
+  size: 462029
+  timestamp: 1713207582684
 - kind: conda
   name: pyzmq
-  version: 25.1.2
-  build: py312hc789acb_0
+  version: 26.0.0
+  build: py312hb81df1d_0
   subdir: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.2-py312hc789acb_0.conda
-  sha256: 1e5fb7095be7edb90efd50cde7b417bf4f1f5ae216d0b597ada61ee201f56d29
-  md5: af49da330d412bc3203bc84f8153d685
+  url: https://conda.anaconda.org/conda-forge/osx-64/pyzmq-26.0.0-py312hb81df1d_0.conda
+  sha256: e9bc00caa0bfab25285161a400b2eca02994c6d4556abe185128ea7bbfb209b0
+  md5: 641c118ce3170463903086ffb677410e
   depends:
-  - __osx >=10.9
-  - libcxx >=16.0.6
+  - libcxx >=16
   - libsodium >=1.0.18,<1.0.19.0a0
   - python >=3.12,<3.13.0a0
   - python_abi 3.12.* *_cp312
   - zeromq >=4.3.5,<4.4.0a0
-  license: BSD-3-Clause AND LGPL-3.0-or-later
+  license: BSD-3-Clause
+  license_family: BSD
   purls:
   - pkg:pypi/pyzmq
-  size: 487865
-  timestamp: 1701783621950
+  size: 447416
+  timestamp: 1713207878913
 - kind: conda
   name: readline
   version: '8.2'
   build: h8228510_1
   build_number: 1
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
@@ -8942,14 +10025,34 @@
   depends:
   - python >=3.7
   license: Apache-2.0
   license_family: Apache
   size: 15064
   timestamp: 1708953086199
 - kind: conda
+  name: stack_data
+  version: 0.6.2
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
+  sha256: a58433e75229bec39f3be50c02efbe9b7083e53a1f31d8ee247564f370191eec
+  md5: e7df0fdd404616638df5ece6e69ba7af
+  depends:
+  - asttokens
+  - executing
+  - pure_eval
+  - python >=3.5
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/stack-data
+  size: 26205
+  timestamp: 1669632203115
+- kind: conda
   name: tk
   version: 8.6.13
   build: h194ca79_0
   subdir: linux-aarch64
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/tk-8.6.13-h194ca79_0.conda
   sha256: 7fa27cc512d3a783f38bd16bbbffc008807372499d5b65d089a8e43bde9db267
   md5: f75105e0585851f818e0009dd1dde4dc
@@ -9381,85 +10484,85 @@
   - python >=3.6
   license: MIT
   license_family: MIT
   size: 17423
   timestamp: 1632758637093
 - kind: conda
   name: uv
-  version: 0.1.31
+  version: 0.1.32
   build: h0e8d75e_0
   subdir: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/uv-0.1.31-h0e8d75e_0.conda
-  sha256: c98f386b8cf11e43c653cdccac46e4d9fc158bc0d0e8be199c84c9a62bead310
-  md5: f2de6f93655004cb162b730bbfcea0bc
+  url: https://conda.anaconda.org/conda-forge/linux-64/uv-0.1.32-h0e8d75e_0.conda
+  sha256: 436fd82877e86516b864fc4796f009408cc57b4983ccfc3781599194fd67d66d
+  md5: ed76c82c4f7d22aff51a8b76ec087d77
   depends:
   - libgcc-ng >=12
   - libstdcxx-ng >=12
   license: Apache-2.0 OR MIT
-  size: 11513645
-  timestamp: 1712704033294
+  size: 11498300
+  timestamp: 1713255137518
 - kind: conda
   name: uv
-  version: 0.1.31
+  version: 0.1.32
   build: h2b8f702_0
   subdir: osx-arm64
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/uv-0.1.31-h2b8f702_0.conda
-  sha256: 555b6b3e65302a959793abab82af955a50319bec15127a42cbeb38026ae90bee
-  md5: d22b758a5cc8c40e45761b8729136dd8
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/uv-0.1.32-h2b8f702_0.conda
+  sha256: 36bbef6c7e5c3717d2c348657f232f5f499815d0289fcf4ec4ca5f3d0fd7fcae
+  md5: 1c3e2d98608f1b8c22ba6df15ceb8b94
   depends:
   - libcxx >=16
   constrains:
   - __osx >=11.0
   license: Apache-2.0 OR MIT
-  size: 8471388
-  timestamp: 1712705177930
+  size: 8422096
+  timestamp: 1713256452817
 - kind: conda
   name: uv
-  version: 0.1.31
+  version: 0.1.32
   build: h2c5c2bd_0
   subdir: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/uv-0.1.31-h2c5c2bd_0.conda
-  sha256: 1964401a3acf6cc0b7cd360df726b3a80d12f48a03395a1fa6e2cb2c35248228
-  md5: fe8eca4e5e90c27abd3e18ff898575ff
+  url: https://conda.anaconda.org/conda-forge/osx-64/uv-0.1.32-h2c5c2bd_0.conda
+  sha256: 3d797ffb7569e559c0b4260168c494958b7dad61e6f87329cda3e5de02127546
+  md5: 8f8fc4fb1724d3b801e69e7b5c2292bb
   depends:
   - libcxx >=16
   constrains:
   - __osx >=10.12
   license: Apache-2.0 OR MIT
-  size: 8137767
-  timestamp: 1712705257304
+  size: 8108808
+  timestamp: 1713256190469
 - kind: conda
   name: uv
-  version: 0.1.31
+  version: 0.1.32
   build: h7ea99a0_0
   subdir: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/uv-0.1.31-h7ea99a0_0.conda
-  sha256: 9e92a0fe6263e4839f0a028ed338fbb2eae0a161860e93bc4657f0778c5126cc
-  md5: b2cee3ae47e61252e48f8f5c6cc1767c
+  url: https://conda.anaconda.org/conda-forge/win-64/uv-0.1.32-h7ea99a0_0.conda
+  sha256: 5af8d2a15846a22f169db95f68cd1be70de649462d9c2ea4244eb80dbe47fa20
+  md5: 08b5f9cf29c8f198c682d687eb7dadb1
   depends:
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   license: Apache-2.0 OR MIT
-  size: 6812801
-  timestamp: 1712705470751
+  size: 6774761
+  timestamp: 1713256030325
 - kind: conda
   name: uv
-  version: 0.1.31
+  version: 0.1.32
   build: hb6a771c_0
   subdir: linux-aarch64
-  url: https://conda.anaconda.org/conda-forge/linux-aarch64/uv-0.1.31-hb6a771c_0.conda
-  sha256: 425681825164753cbfb83899478bdc7d3cf66833ff6a44bd34a73820082b08f6
-  md5: e8ce890f80149db9b8c27197f2adb28b
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/uv-0.1.32-hb6a771c_0.conda
+  sha256: 1098a784249bee60ae054ce2f01edf64076460507f4e5beec650a7e6950b2d1e
+  md5: 8f799145aae09e78564321a2f92bd61b
   depends:
   - libgcc-ng >=12
   - libstdcxx-ng >=12
   license: Apache-2.0 OR MIT
-  size: 12433494
-  timestamp: 1712704300242
+  size: 12334091
+  timestamp: 1713255286627
 - kind: conda
   name: vc
   version: '14.3'
   build: hcf57466_18
   build_number: 18
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hcf57466_18.conda
@@ -9488,50 +10591,48 @@
   - vs2015_runtime 14.38.33130.* *_18
   license: LicenseRef-ProprietaryMicrosoft
   license_family: Proprietary
   size: 749868
   timestamp: 1702511239004
 - kind: conda
   name: virtualenv
-  version: 20.25.1
+  version: 20.25.2
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
-  url: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
-  sha256: 1ced4445cf72cd9dc344ad04bdaf703a08cc428c8c46e4bda928ad79786ee153
-  md5: 8797a4e26be36880a603aba29c785352
+  url: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
+  sha256: 78bd4b106c079ec082ffee50c48fcb317364ea0e1cc2ed069251c42f65ff9e93
+  md5: 550f27866347ba7986623d45f06f4e6c
   depends:
   - distlib <1,>=0.3.7
   - filelock <4,>=3.12.2
   - platformdirs <5,>=3.9.1
   - python >=3.8
   license: MIT
-  license_family: MIT
   purls:
   - pkg:pypi/virtualenv
-  size: 3148218
-  timestamp: 1708602229963
+  size: 3458265
+  timestamp: 1713348595021
 - kind: conda
   name: virtualenv
-  version: 20.25.1
+  version: 20.25.2
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
-  url: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.1-pyhd8ed1ab_0.conda
-  sha256: 1ced4445cf72cd9dc344ad04bdaf703a08cc428c8c46e4bda928ad79786ee153
-  md5: 8797a4e26be36880a603aba29c785352
+  url: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.25.2-pyhd8ed1ab_0.conda
+  sha256: 78bd4b106c079ec082ffee50c48fcb317364ea0e1cc2ed069251c42f65ff9e93
+  md5: 550f27866347ba7986623d45f06f4e6c
   depends:
   - distlib <1,>=0.3.7
   - filelock <4,>=3.12.2
   - platformdirs <5,>=3.9.1
   - python >=3.8
   license: MIT
-  license_family: MIT
-  size: 3148218
-  timestamp: 1708602229963
+  size: 3458265
+  timestamp: 1713348595021
 - kind: conda
   name: vs2015_runtime
   version: 14.38.33130
   build: hcb4865c_18
   build_number: 18
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33130-hcb4865c_18.conda
@@ -9540,14 +10641,31 @@
   depends:
   - vc14_runtime >=14.38.33130
   license: BSD-3-Clause
   license_family: BSD
   size: 16988
   timestamp: 1702511261442
 - kind: conda
+  name: wcwidth
+  version: 0.2.13
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
+  sha256: b6cd2fee7e728e620ec736d8dfee29c6c9e2adbd4e695a31f1d8f834a83e57e3
+  md5: 68f0738df502a14213624b288c60c9ad
+  depends:
+  - python >=3.8
+  license: MIT
+  license_family: MIT
+  purls:
+  - pkg:pypi/wcwidth
+  size: 32709
+  timestamp: 1704731373922
+- kind: conda
   name: xz
   version: 5.2.6
   build: h166bdaf_0
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
   sha256: 03a6d28ded42af8a347345f82f3eebdd6807a08526d47899a42d62d319609162
   md5: 2161070d867d1b1204ea749c8eec4ef0
```

### Comparing `pixi_kernel-0.2.1/pixi.toml` & `pixi_kernel-0.3.0/pixi.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [project]
 name = "pixi-kernel"
-version = "0.2.1"
-description = "Python Jupyter kernel using Pixi for reproducible notebooks"
+version = "0.3.0"
+description = "Jupyter kernels using Pixi for reproducible notebooks"
 authors = ["Renan Rodrigues dos Santos <renan.engmec@gmail.com>"]
 channels = ["conda-forge"]
 platforms = ["linux-64", "linux-aarch64", "osx-64", "osx-arm64", "win-64"]
 
 
 # Dependencies
 [feature.base.dependencies]
 python = ">=3.8,<4.0"
+ipykernel = ">=6"
 jupyter_client = ">=7"
 msgspec = ">=0.18"
 
 
 # Development
 [feature.dev.pypi-dependencies]
 pixi-kernel = { path = ".", editable = true }
@@ -60,14 +61,22 @@
 ruff = ">=0.3.5,<0.4"
 
 [feature.ruff.tasks]
 format = "ruff format . && ruff check . --select I --fix"
 lint = "ruff format --check . && ruff check ."
 
 
+# Type checking
+[feature.mypy.dependencies]
+mypy = ">=1.9"
+
+[feature.mypy.tasks]
+type-check = "mypy src"
+
+
 # Building
 [feature.build.dependencies]
 hatch = ">=1.9,<2"
 uv = "*"
 
 [feature.build.tasks]
 build = "hatch build"
@@ -103,16 +112,17 @@
 python = "3.12.*"
 
 [feature.py312.tasks]
 test-py312 = { depends_on = ["install", "test"] }
 
 
 [environments]
-default = { features = ["base", "build", "dev", "ruff", "test"], solve-group = "pixi-kernel" }
+default = { features = ["base", "build", "dev", "mypy", "ruff", "test"], solve-group = "pixi-kernel" }
 build = { features = ["build"], solve-group = "pixi-kernel" }
+mypy = { features = ["base", "mypy"], solve-group = "pixi-kernel" }
 ruff = { features = ["ruff"], solve-group = "pixi-kernel" }
 test = { features = ["test"], solve-group = "pixi-kernel" }
 
 # Python testing matrix
 py38 = ["py38", "build", "test"]
 py39 = ["py39", "build", "test"]
 py310 = ["py310", "build", "test"]
```

### Comparing `pixi_kernel-0.2.1/.github/workflows/ci.yml` & `pixi_kernel-0.3.0/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 env:
   pixi-version: "0.19.1"
 
 jobs:
   test:
     strategy:
       matrix:
-        os: [ubuntu-latest, macos-latest, windows-latest]
+        # Remove the noisy windows tests from matrix until figuring out the signals issue
+        # https://github.com/ipython/ipykernel/issues/713
+        # https://stackoverflow.com/questions/70841648/jupyter-reverts-signal-handler-to-default-when-running-next-cell
+        os: [ubuntu-latest, macos-latest]
         pixi-version: ["0.18.0", "0.19.1"]
         python-version: ["38", "39", "310", "311", "312"]
     runs-on: ${{ matrix.os }}
     steps:
       - name: Checkout repo
         uses: actions/checkout@v4
       - name: Install Pixi ${{ matrix.pixi-version }}
@@ -63,7 +66,19 @@
       - name: Install Pixi ${{ env.pixi-version }}
         uses: prefix-dev/setup-pixi@v0.5.1
         with:
           pixi-version: v${{ env.pixi-version }}
           run-install: false
       - name: Run code quality checks
         run: pixi run --locked --environment ruff lint
+  type-check:
+    runs-on: ubuntu-22.04
+    steps:
+      - name: Checkout repo
+        uses: actions/checkout@v4
+      - name: Install Pixi ${{ env.pixi-version }}
+        uses: prefix-dev/setup-pixi@v0.5.1
+        with:
+          pixi-version: v${{ env.pixi-version }}
+          run-install: false
+      - name: Run type checks
+        run: pixi run --locked --environment mypy type-check
```

### Comparing `pixi_kernel-0.2.1/.github/workflows/release.yml` & `pixi_kernel-0.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.1/assets/launch-dark.png` & `pixi_kernel-0.3.0/assets/launch-dark.png`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.1/assets/launch-light.png` & `pixi_kernel-0.3.0/assets/launch-light.png`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.1/kernels/pixi-kernel-bash/logo-svg.svg` & `pixi_kernel-0.3.0/kernels/pixi-kernel-bash/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.1/kernels/pixi-kernel-ir/kernel.js` & `pixi_kernel-0.3.0/kernels/pixi-kernel-ir/kernel.js`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.1/kernels/pixi-kernel-ir/logo-64x64.png` & `pixi_kernel-0.3.0/kernels/pixi-kernel-ir/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.1/kernels/pixi-kernel-ir/logo-svg.svg` & `pixi_kernel-0.3.0/kernels/pixi-kernel-ir/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.1/kernels/pixi-kernel-python3/logo-32x32.png` & `pixi_kernel-0.3.0/kernels/pixi-kernel-python3/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.1/kernels/pixi-kernel-python3/logo-64x64.png` & `pixi_kernel-0.3.0/kernels/pixi-kernel-python3/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.1/kernels/pixi-kernel-python3/logo-svg.svg` & `pixi_kernel-0.3.0/kernels/pixi-kernel-python3/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp11/logo-32x32.png` & `pixi_kernel-0.3.0/kernels/pixi-kernel-xcpp11/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp11/logo-64x64.png` & `pixi_kernel-0.3.0/kernels/pixi-kernel-xcpp11/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp11/logo-svg.svg` & `pixi_kernel-0.3.0/kernels/pixi-kernel-xcpp11/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp14/logo-32x32.png` & `pixi_kernel-0.3.0/kernels/pixi-kernel-xcpp14/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp14/logo-64x64.png` & `pixi_kernel-0.3.0/kernels/pixi-kernel-xcpp14/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp14/logo-svg.svg` & `pixi_kernel-0.3.0/kernels/pixi-kernel-xcpp14/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp17/logo-32x32.png` & `pixi_kernel-0.3.0/kernels/pixi-kernel-xcpp17/logo-32x32.png`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp17/logo-64x64.png` & `pixi_kernel-0.3.0/kernels/pixi-kernel-xcpp17/logo-64x64.png`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.1/kernels/pixi-kernel-xcpp17/logo-svg.svg` & `pixi_kernel-0.3.0/kernels/pixi-kernel-xcpp17/logo-svg.svg`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.1/src/pixi_kernel/errors.py` & `pixi_kernel-0.3.0/src/pixi_kernel/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,35 +5,34 @@
     1. Visit the Pixi installation guide at https://pixi.sh/latest/
     2. After installation, restart JupyterLab.
     3. Ensure that Pixi was added to your PATH by typing 'which pixi' in your terminal and checking if the Pixi directory is listed.
 
 If you continue to face issues, please report them at https://github.com/renan-r-santos/pixi-kernel/issues
 """
 
-PIXI_VERSION_ERROR = """Pixi was detected in your system but it appears to be corrupted. To run the {kernel_display_name} kernel, 
-please follow the steps below to reinstall Pixi:
+PIXI_VERSION_ERROR = """Pixi was detected in your system but it appears to be corrupted.
+To run the {kernel_display_name} kernel, please follow the steps below to reinstall Pixi:
     1. Visit the Pixi installation guide at https://pixi.sh/latest/
     2. After installation, restart JupyterLab.
     3. Ensure that Pixi is working by typing 'pixi --version' in your terminal and checking if the version string is listed.
 
 If you continue to face issues, please report them at https://github.com/renan-r-santos/pixi-kernel/issues
 """
 
 PIXI_VERSION_NOT_SUPPORTED = """Pixi was detected in your system but it appears to be outdated.
 You need at least Pixi {minimum_version} in order to run the {kernel_display_name} kernel.
-In your terminal, type 'pixi self-update' to update Pixi to the latest version.
+In your terminal, type 'pixi self-update' to update Pixi to the latest version and restart your kernel.
 
 If you continue to face issues, please report them at https://github.com/renan-r-santos/pixi-kernel/issues
 """
 
-PIXI_MANIFEST_NOT_FOUND = """Pixi Kernel could not find a project manifest file in
-the current working directory {cwd} nor in any of its parents.
-Make sure you initialize a Pixi project by running 'pixi init' in the project directory.
+PIXI_MANIFEST_NOT_FOUND = """Pixi Kernel could not find a project manifest file in the current working directory {cwd} nor in any of its parents.
+Make sure you initialize a Pixi project by running 'pixi init' in the project directory and restart your kernel.
 
 If you continue to face issues, please report them at https://github.com/renan-r-santos/pixi-kernel/issues
 """
 
 PIXI_KERNEL_NOT_FOUND = """To run the {kernel_display_name} kernel, you need to add the {package_name} package to your project dependencies.
-You can do this by running 'pixi add {package_name}' in your project directory and trying again.
+You can do this by running 'pixi add {package_name}' in your project directory and restarting your kernel.
 
 If you continue to face issues, please report them at https://github.com/renan-r-santos/pixi-kernel/issues
 """
```

### Comparing `pixi_kernel-0.2.1/src/pixi_kernel/pixi.py` & `pixi_kernel-0.3.0/src/pixi_kernel/pixi.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 from __future__ import annotations
 
+import logging
 import shutil
 import subprocess
-from logging import Logger
 from pathlib import Path
 from typing import List, Optional
 
 import msgspec
 
 from .errors import (
     PIXI_KERNEL_NOT_FOUND,
     PIXI_MANIFEST_NOT_FOUND,
     PIXI_NOT_FOUND,
     PIXI_VERSION_ERROR,
     PIXI_VERSION_NOT_SUPPORTED,
 )
 
+logger = logging.getLogger(__name__)
 MINIMUM_PIXI_VERSION = "0.18.0"
-required_major, required_minor, required_patch = map(int, MINIMUM_PIXI_VERSION.split("."))
+
+
+class PixiDiscoveryError(Exception):
+    def __init__(self, message: str):
+        self.message = message
 
 
 class PixiInfo(msgspec.Struct, frozen=True, kw_only=True):
     environments_info: List[EnvironmentInfo]
     project_info: Optional[ProjectInfo]
 
 
@@ -31,77 +36,70 @@
     pypi_dependencies: List[str]
 
 
 class ProjectInfo(msgspec.Struct, frozen=True, kw_only=True):
     manifest_path: str
 
 
-def find_project_manifest(
-    *,
-    cwd: Path,
-    package_name: str,
-    kernel_display_name: str,
-    logger: Logger,
-) -> Path:
+def find_project_manifest(*, cwd: Path, package_name: str, kernel_display_name: str) -> Path:
     # Ensure Pixi is in PATH
     if shutil.which("pixi") is None:
-        raise RuntimeError(PIXI_NOT_FOUND.format(kernel_display_name=kernel_display_name))
+        raise PixiDiscoveryError(PIXI_NOT_FOUND.format(kernel_display_name=kernel_display_name))
 
     # Ensure a supported Pixi version is installed
     result = subprocess.run(["pixi", "--version"], capture_output=True, text=True)
     if result.returncode != 0 or not result.stdout.startswith("pixi "):
-        raise RuntimeError(PIXI_VERSION_ERROR.format(kernel_display_name=kernel_display_name))
+        raise PixiDiscoveryError(
+            PIXI_VERSION_ERROR.format(kernel_display_name=kernel_display_name)
+        )
 
     pixi_version = result.stdout[len("pixi ") :].strip()
     major, minor, patch = map(int, pixi_version.split("."))
+    required_major, required_minor, required_patch = map(int, MINIMUM_PIXI_VERSION.split("."))
     if (major, minor, patch) < (required_major, required_minor, required_patch):
-        raise RuntimeError(
+        raise PixiDiscoveryError(
             PIXI_VERSION_NOT_SUPPORTED.format(
                 kernel_display_name=kernel_display_name,
                 minimum_version=MINIMUM_PIXI_VERSION,
             )
         )
-    logger.info(f"[pixi-kernel] found Pixi {pixi_version}")
+    logger.info(f"found Pixi {pixi_version}")
 
     # Find project's manifest file
     candidate_dirs = [cwd, *cwd.parents]
     for dir in candidate_dirs:
         for project_filename in ["pixi.toml", "pyproject.toml"]:
             result = subprocess.run(
                 ["pixi", "info", f"--manifest-path={project_filename}", "--json"],
                 cwd=dir,
                 capture_output=True,
+                text=True,
             )
             if result.returncode != 0:
-                logger.error(
-                    f"[pixi-kernel] failed to run 'pixi info' for directory {dir}: {result.stderr}"
-                )
+                logger.error(f"failed to run 'pixi info' for directory {dir}: {result.stderr}")
                 continue
 
             try:
                 pixi_info = msgspec.json.decode(result.stdout, type=PixiInfo)
             except msgspec.ValidationError as exception:
-                logger.error(
-                    f"[pixi-kernel] failed to parse pixi info {result.stdout}: {exception}"
-                )
+                logger.error(f"failed to parse pixi info {result.stdout}: {exception}")
                 continue
 
             if len(pixi_info.environments_info) == 0:
-                logger.warning(f"[pixi-kernel] found empty project at {dir}: {pixi_info}")
+                logger.warning(f"found empty project at {dir}: {pixi_info}")
                 continue
 
             for env in pixi_info.environments_info:
                 if env.name == "default" and pixi_info.project_info is not None:
                     if package_name not in env.dependencies + env.pypi_dependencies:
                         logger.error(
-                            f"[pixi-kernel] package {package_name} not found in project"
-                            f"dependencies {pixi_info}"
+                            f"package {package_name} not found in project dependencies {pixi_info}"
                         )
-                        raise RuntimeError(
+                        raise PixiDiscoveryError(
                             PIXI_KERNEL_NOT_FOUND.format(
                                 kernel_display_name=kernel_display_name,
                                 package_name=package_name,
                             )
                         )
                     return dir / project_filename
 
-    raise RuntimeError(PIXI_MANIFEST_NOT_FOUND.format(cwd=cwd))
+    raise PixiDiscoveryError(PIXI_MANIFEST_NOT_FOUND.format(cwd=cwd))
```

### Comparing `pixi_kernel-0.2.1/tests/integration/bash_kernel/pixi.lock` & `pixi_kernel-0.3.0/tests/integration/bash_kernel/pixi.lock`

 * *Files 1% similar despite different names*

```diff
@@ -32,32 +32,32 @@
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.2-h2797004_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h7e041cc_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4.20240210-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.8-py312h98912ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.2-hab00c5b_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.12-4_cp312.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.2-py312h886d080_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/pyzmq-26.0.0-py312h886d080_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tornado-6.4-py312h98912ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
@@ -101,32 +101,32 @@
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libnsl-2.0.1-h31becfc_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libsodium-1.0.18-hb9de7d4_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libsqlite-3.45.2-h194ca79_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libstdcxx-ng-13.2.0-h9a76618_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libuuid-2.38.1-hb4cce97_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libxcrypt-4.4.36-h31becfc_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libzlib-1.2.13-h31becfc_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ncurses-6.4.20240210-h0425590_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/openssl-3.2.1-h31becfc_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/psutil-5.9.8-py312hdd3e373_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.2-h43d1f9e_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.3-h43d1f9e_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python_abi-3.12-4_cp312.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/pyzmq-25.1.2-py312h1c32067_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/pyzmq-26.0.0-py312h1c32067_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/readline-8.2-h8fc344f_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/tk-8.6.13-h194ca79_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/tornado-6.4-py312h9ef2f89_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
@@ -164,32 +164,32 @@
       - conda: https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.7.2-py312hb401068_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libexpat-2.6.2-h73e2aa4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.2-h92b6c6a_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4.20240210-h73e2aa4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.2.1-hd75f5a5_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.8-py312h41838bb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.2-h9f0c242_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.12-4_cp312.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.2-py312hc789acb_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/pyzmq-26.0.0-py312hb81df1d_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tornado-6.4-py312h41838bb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
@@ -227,32 +227,32 @@
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/jupyter_core-5.7.2-py312h81bd7bf_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libcxx-16.0.6-h4653b0c_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libexpat-2.6.2-hebf3989_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libffi-3.4.2-h3422bc3_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libsodium-1.0.18-h27ca646_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libsqlite-3.45.2-h091b4b1_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libzlib-1.2.13-h53f4e23_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ncurses-6.4.20240210-h078ce10_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.2.1-h0d3ecfb_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/psutil-5.9.8-py312he37b823_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.2-hdf0ec26_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.3-h4a7b5fc_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.12-4_cp312.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pyzmq-25.1.2-py312h1edf716_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pyzmq-26.0.0-py312h2105c20_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tornado-6.4-py312he37b823_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
@@ -288,32 +288,32 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.7.2-py312h2e8e312_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libexpat-2.6.2-h63175ca_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.2-hcfcfb64_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/openssl-3.2.1-hcfcfb64_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.8-py312he70551f_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.2-h2628c8c_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.3-h2628c8c_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/pywin32-306-py312h53d5487_2.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/pyzmq-25.1.2-py312h1ac6f91_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/pyzmq-26.0.0-py312h1ac6f91_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/tornado-6.4-py312he70551f_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
@@ -779,16 +779,16 @@
   - python_abi 3.12.* *_cp312
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   license: MIT
   license_family: MIT
   purls:
-  - pkg:pypi/bytecode
   - pkg:pypi/debugpy
+  - pkg:pypi/bytecode
   size: 3105043
   timestamp: 1707445249662
 - kind: conda
   name: debugpy
   version: 1.8.1
   build: py312hede676d_0
   subdir: osx-64
@@ -798,16 +798,16 @@
   depends:
   - libcxx >=16
   - python >=3.12,<3.13.0a0
   - python_abi 3.12.* *_cp312
   license: MIT
   license_family: MIT
   purls:
-  - pkg:pypi/debugpy
   - pkg:pypi/bytecode
+  - pkg:pypi/debugpy
   size: 2065572
   timestamp: 1707444822563
 - kind: conda
   name: decorator
   version: 5.1.1
   build: pyhd8ed1ab_0
   subdir: noarch
@@ -1815,35 +1815,35 @@
   - zlib 1.2.13 *_5
   license: Zlib
   license_family: Other
   size: 61588
   timestamp: 1686575217516
 - kind: conda
   name: matplotlib-inline
-  version: 0.1.6
+  version: 0.1.7
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
-  url: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2
-  sha256: aa091b88aec55bfa2d9207028d8cdc689b9efb090ae27b99557e93c675be2f3c
-  md5: b21613793fcc81d944c76c9f2864a7de
+  url: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
+  sha256: 7ea68676ea35fbb095420bbcc1c82c4767b8be7bb56abb6989b7f89d957a3bab
+  md5: 779345c95648be40d22aaa89de7d4254
   depends:
   - python >=3.6
   - traitlets
   license: BSD-3-Clause
   license_family: BSD
   purls:
   - pkg:pypi/matplotlib-inline
-  size: 12273
-  timestamp: 1660814913405
+  size: 14599
+  timestamp: 1713250613726
 - kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/0e/f2/f864ed36a8a62c26b57c3e08d212bd8f3d12a3ca3ef64600be5452aa3c82/msgspec-0.18.6-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
-  sha256: e97dec6932ad5e3ee1e3c14718638ba333befc45e0661caa57033cd4cc489466
+  url: https://files.pythonhosted.org/packages/1d/b5/c8fbf1db814eb29eda402952374b594b2559419ba7ec6d0997a9e5687530/msgspec-0.18.6-cp312-cp312-macosx_10_9_x86_64.whl
+  sha256: d86f5071fe33e19500920333c11e2267a31942d18fed4d9de5bc2fbab267d28c
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -1873,16 +1873,16 @@
   - tomli-w ; extra == 'toml'
   - tomli ; python_version < '3.11' and extra == 'toml'
   - pyyaml ; extra == 'yaml'
   requires_python: '>=3.8'
 - kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/1d/b5/c8fbf1db814eb29eda402952374b594b2559419ba7ec6d0997a9e5687530/msgspec-0.18.6-cp312-cp312-macosx_10_9_x86_64.whl
-  sha256: d86f5071fe33e19500920333c11e2267a31942d18fed4d9de5bc2fbab267d28c
+  url: https://files.pythonhosted.org/packages/d7/9a/235d2dbab078a0b8e6f338205dc59be0b027ce000554ee6a9c41b19339e5/msgspec-0.18.6-cp312-cp312-macosx_11_0_arm64.whl
+  sha256: ce13981bfa06f5eb126a3a5a38b1976bddb49a36e4f46d8e6edecf33ccf11df1
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -1912,16 +1912,16 @@
   - tomli-w ; extra == 'toml'
   - tomli ; python_version < '3.11' and extra == 'toml'
   - pyyaml ; extra == 'yaml'
   requires_python: '>=3.8'
 - kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/3f/76/30d8f152299f65c85c46a2cbeaf95ad1d18516b5ce730acdaef696d4cfe6/msgspec-0.18.6-cp312-cp312-win_amd64.whl
-  sha256: 1003c20bfe9c6114cc16ea5db9c5466e49fae3d7f5e2e59cb70693190ad34da0
+  url: https://files.pythonhosted.org/packages/0e/f2/f864ed36a8a62c26b57c3e08d212bd8f3d12a3ca3ef64600be5452aa3c82/msgspec-0.18.6-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
+  sha256: e97dec6932ad5e3ee1e3c14718638ba333befc45e0661caa57033cd4cc489466
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -1951,16 +1951,16 @@
   - tomli-w ; extra == 'toml'
   - tomli ; python_version < '3.11' and extra == 'toml'
   - pyyaml ; extra == 'yaml'
   requires_python: '>=3.8'
 - kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/d7/9a/235d2dbab078a0b8e6f338205dc59be0b027ce000554ee6a9c41b19339e5/msgspec-0.18.6-cp312-cp312-macosx_11_0_arm64.whl
-  sha256: ce13981bfa06f5eb126a3a5a38b1976bddb49a36e4f46d8e6edecf33ccf11df1
+  url: https://files.pythonhosted.org/packages/73/16/dfef780ced7d690dd5497846ed242ef3e27e319d59d1ddaae816a4f2c15e/msgspec-0.18.6-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: ad237100393f637b297926cae1868b0d500f764ccd2f0623a380e2bcfb2809ca
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -1990,16 +1990,16 @@
   - tomli-w ; extra == 'toml'
   - tomli ; python_version < '3.11' and extra == 'toml'
   - pyyaml ; extra == 'yaml'
   requires_python: '>=3.8'
 - kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/73/16/dfef780ced7d690dd5497846ed242ef3e27e319d59d1ddaae816a4f2c15e/msgspec-0.18.6-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: ad237100393f637b297926cae1868b0d500f764ccd2f0623a380e2bcfb2809ca
+  url: https://files.pythonhosted.org/packages/3f/76/30d8f152299f65c85c46a2cbeaf95ad1d18516b5ce730acdaef696d4cfe6/msgspec-0.18.6-cp312-cp312-win_amd64.whl
+  sha256: 1003c20bfe9c6114cc16ea5db9c5466e49fae3d7f5e2e59cb70693190ad34da0
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -2252,18 +2252,19 @@
   license_family: MIT
   purls:
   - pkg:pypi/pickleshare
   size: 9332
   timestamp: 1602536313357
 - kind: pypi
   name: pixi-kernel
-  version: 0.2.1
+  version: 0.3.0
   path: ../../../../pixi-kernel
-  sha256: fc89be37749334e0eb20e8656e5ffcdace662e69fd273fa798213fdf1e64b7cb
+  sha256: 026726c0f08b63327906964394fdaf6d1b2324c25bf50c37e37b0300731fba40
   requires_dist:
+  - ipykernel >=6
   - jupyter-client >=7
   - msgspec >=0.18
   requires_python: <4.0,>=3.8
   editable: true
 - kind: conda
   name: platformdirs
   version: 4.2.0
@@ -2441,148 +2442,150 @@
   license_family: BSD
   purls:
   - pkg:pypi/pygments
   size: 860425
   timestamp: 1700608076927
 - kind: conda
   name: python
-  version: 3.12.2
+  version: 3.12.3
+  build: h1411813_0_cpython
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda
+  sha256: 3b327ffc152a245011011d1d730781577a8274fde1cf6243f073749ead8f1c2a
+  md5: df1448ec6cbf8eceb03d29003cf72ae6
+  depends:
+  - __osx >=10.9
+  - bzip2 >=1.0.8,<2.0a0
+  - libexpat >=2.6.2,<3.0a0
+  - libffi >=3.4,<4.0a0
+  - libsqlite >=3.45.2,<4.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - ncurses >=6.4.20240210,<7.0a0
+  - openssl >=3.2.1,<4.0a0
+  - readline >=8.2,<9.0a0
+  - tk >=8.6.13,<8.7.0a0
+  - tzdata
+  - xz >=5.2.6,<6.0a0
+  constrains:
+  - python_abi 3.12.* *_cp312
+  license: Python-2.0
+  size: 14557341
+  timestamp: 1713208068012
+- kind: conda
+  name: python
+  version: 3.12.3
   build: h2628c8c_0_cpython
   subdir: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/python-3.12.2-h2628c8c_0_cpython.conda
-  sha256: b8eda863b48ae4531635e23fd15e759d93212b6204c6847d591e25fa5fd67477
-  md5: be8803e9f75a477df61d4aabea3c1246
+  url: https://conda.anaconda.org/conda-forge/win-64/python-3.12.3-h2628c8c_0_cpython.conda
+  sha256: 1a95494abe572a8819c933f978df89f00bde72ea9432d46a70632599e8029ea4
+  md5: f07c8c5dd98767f9a652de5d039b284e
   depends:
   - bzip2 >=1.0.8,<2.0a0
-  - libexpat >=2.5.0,<3.0a0
+  - libexpat >=2.6.2,<3.0a0
   - libffi >=3.4,<4.0a0
-  - libsqlite >=3.45.1,<4.0a0
+  - libsqlite >=3.45.2,<4.0a0
   - libzlib >=1.2.13,<1.3.0a0
   - openssl >=3.2.1,<4.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.12.* *_cp312
   license: Python-2.0
-  size: 16083296
-  timestamp: 1708116662336
+  size: 16179248
+  timestamp: 1713205644673
 - kind: conda
   name: python
-  version: 3.12.2
+  version: 3.12.3
   build: h43d1f9e_0_cpython
   subdir: linux-aarch64
-  url: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.2-h43d1f9e_0_cpython.conda
-  sha256: 16c8e77c01b814d836af632ef77eac21b64b9e398a11e1403a3a1802bb5be366
-  md5: 3a41090f2ef0868f119825593948ed46
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.3-h43d1f9e_0_cpython.conda
+  sha256: e186f3ee570464241c844adff6a3ba8f395cef15c5d46c0a8f784cfd97b3bdca
+  md5: dc93ad1d2ba17ebc948bf5434ffa864b
   depends:
   - bzip2 >=1.0.8,<2.0a0
   - ld_impl_linux-aarch64 >=2.36.1
-  - libexpat >=2.5.0,<3.0a0
+  - libexpat >=2.6.2,<3.0a0
   - libffi >=3.4,<4.0a0
   - libgcc-ng >=12
   - libnsl >=2.0.1,<2.1.0a0
-  - libsqlite >=3.45.1,<4.0a0
+  - libsqlite >=3.45.2,<4.0a0
   - libuuid >=2.38.1,<3.0a0
   - libxcrypt >=4.4.36
   - libzlib >=1.2.13,<1.3.0a0
-  - ncurses >=6.4,<7.0a0
+  - ncurses >=6.4.20240210,<7.0a0
   - openssl >=3.2.1,<4.0a0
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.12.* *_cp312
   license: Python-2.0
-  size: 13823577
-  timestamp: 1708116074721
+  size: 14051797
+  timestamp: 1713205211165
 - kind: conda
   name: python
-  version: 3.12.2
-  build: h9f0c242_0_cpython
-  subdir: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.2-h9f0c242_0_cpython.conda
-  sha256: 7647ac06c3798a182a4bcb1ff58864f1ef81eb3acea6971295304c23e43252fb
-  md5: 0179b8007ba008cf5bec11f3b3853902
+  version: 3.12.3
+  build: h4a7b5fc_0_cpython
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.3-h4a7b5fc_0_cpython.conda
+  sha256: c761fb3713ea66bce3889b33b6f400afb2dd192d1fc2686446e9d8166cfcec6b
+  md5: 8643ab37bece6ae8f112464068d9df9c
   depends:
+  - __osx >=11.0
   - bzip2 >=1.0.8,<2.0a0
-  - libexpat >=2.5.0,<3.0a0
+  - libexpat >=2.6.2,<3.0a0
   - libffi >=3.4,<4.0a0
-  - libsqlite >=3.45.1,<4.0a0
+  - libsqlite >=3.45.2,<4.0a0
   - libzlib >=1.2.13,<1.3.0a0
-  - ncurses >=6.4,<7.0a0
+  - ncurses >=6.4.20240210,<7.0a0
   - openssl >=3.2.1,<4.0a0
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.12.* *_cp312
   license: Python-2.0
-  size: 14596811
-  timestamp: 1708118065292
+  size: 13207557
+  timestamp: 1713206576646
 - kind: conda
   name: python
-  version: 3.12.2
+  version: 3.12.3
   build: hab00c5b_0_cpython
   subdir: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.2-hab00c5b_0_cpython.conda
-  sha256: ddb7a2d8d78046bda5d7631e6814f9468d2eb054e10f86f4648c9d1fdaa30c0f
-  md5: ad7b68400f3a6ebe72b00be093c7f301
+  url: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda
+  sha256: f9865bcbff69f15fd89a33a2da12ad616e98d65ce7c83c644b92e66e5016b227
+  md5: 2540b74d304f71d3e89c81209db4db84
   depends:
   - bzip2 >=1.0.8,<2.0a0
   - ld_impl_linux-64 >=2.36.1
-  - libexpat >=2.5.0,<3.0a0
+  - libexpat >=2.6.2,<3.0a0
   - libffi >=3.4,<4.0a0
   - libgcc-ng >=12
   - libnsl >=2.0.1,<2.1.0a0
-  - libsqlite >=3.45.1,<4.0a0
+  - libsqlite >=3.45.2,<4.0a0
   - libuuid >=2.38.1,<3.0a0
   - libxcrypt >=4.4.36
   - libzlib >=1.2.13,<1.3.0a0
-  - ncurses >=6.4,<7.0a0
+  - ncurses >=6.4.20240210,<7.0a0
   - openssl >=3.2.1,<4.0a0
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.12.* *_cp312
   license: Python-2.0
-  size: 32312631
-  timestamp: 1708118077305
-- kind: conda
-  name: python
-  version: 3.12.2
-  build: hdf0ec26_0_cpython
-  subdir: osx-arm64
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.2-hdf0ec26_0_cpython.conda
-  sha256: ccd6c55a286d51d907c878ed2bfa7d1becce0fee71374a9386c5eb90d803ac72
-  md5: 85e91138ae921a2771f57a50120272bd
-  depends:
-  - bzip2 >=1.0.8,<2.0a0
-  - libexpat >=2.5.0,<3.0a0
-  - libffi >=3.4,<4.0a0
-  - libsqlite >=3.45.1,<4.0a0
-  - libzlib >=1.2.13,<1.3.0a0
-  - ncurses >=6.4,<7.0a0
-  - openssl >=3.2.1,<4.0a0
-  - readline >=8.2,<9.0a0
-  - tk >=8.6.13,<8.7.0a0
-  - tzdata
-  - xz >=5.2.6,<6.0a0
-  constrains:
-  - python_abi 3.12.* *_cp312
-  license: Python-2.0
-  size: 13085901
-  timestamp: 1708117361381
+  size: 31991381
+  timestamp: 1713208036041
 - kind: conda
   name: python-dateutil
   version: 2.9.0
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
@@ -2691,114 +2694,117 @@
   license_family: PSF
   purls:
   - pkg:pypi/pywin32
   size: 6127499
   timestamp: 1695974557413
 - kind: conda
   name: pyzmq
-  version: 25.1.2
+  version: 26.0.0
   build: py312h1ac6f91_0
   subdir: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/pyzmq-25.1.2-py312h1ac6f91_0.conda
-  sha256: 9371101999c75aa562c5aa4ae0dfefa140bee635a3f8e15768628689f70d7765
-  md5: 74194f888cc7b11d8c18edf416b61a1b
+  url: https://conda.anaconda.org/conda-forge/win-64/pyzmq-26.0.0-py312h1ac6f91_0.conda
+  sha256: 8d12105518f4ae9bbf48bbdbe031a0b3f2c0b1378350422172af2afc77014f54
+  md5: c69d5948bed236b2cfa323dd478d8de8
   depends:
   - libsodium >=1.0.18,<1.0.19.0a0
   - python >=3.12,<3.13.0a0
   - python_abi 3.12.* *_cp312
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   - zeromq >=4.3.5,<4.3.6.0a0
-  license: BSD-3-Clause AND LGPL-3.0-or-later
+  license: BSD-3-Clause
+  license_family: BSD
   purls:
   - pkg:pypi/pyzmq
-  size: 480772
-  timestamp: 1701783863250
+  size: 444664
+  timestamp: 1713208522670
 - kind: conda
   name: pyzmq
-  version: 25.1.2
+  version: 26.0.0
   build: py312h1c32067_0
   subdir: linux-aarch64
-  url: https://conda.anaconda.org/conda-forge/linux-aarch64/pyzmq-25.1.2-py312h1c32067_0.conda
-  sha256: 7394b1de60b33bbe7fc62d67a838671777cfe725074332d61861457efa0c1f62
-  md5: 7b450f76fbf279bd05304bc9fd879ff0
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/pyzmq-26.0.0-py312h1c32067_0.conda
+  sha256: 5c87c69960aba5292df0e8ece531b97f294336c15d022d2efafb171ab080983d
+  md5: 7f6de7d76e5253bdf14a9088fec24f04
   depends:
   - libgcc-ng >=12
   - libsodium >=1.0.18,<1.0.19.0a0
   - libstdcxx-ng >=12
   - python >=3.12,<3.13.0a0
   - python_abi 3.12.* *_cp312
   - zeromq >=4.3.5,<4.4.0a0
-  license: BSD-3-Clause AND LGPL-3.0-or-later
+  license: BSD-3-Clause
+  license_family: BSD
   purls:
   - pkg:pypi/pyzmq
-  size: 530614
-  timestamp: 1701785140508
+  size: 457757
+  timestamp: 1713209766265
 - kind: conda
   name: pyzmq
-  version: 25.1.2
-  build: py312h1edf716_0
+  version: 26.0.0
+  build: py312h2105c20_0
   subdir: osx-arm64
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/pyzmq-25.1.2-py312h1edf716_0.conda
-  sha256: a89712c6b0cab1e3385e44e0130a57b9d03df99b6f540486c0f00e2dae079e77
-  md5: 913db29987f836f5d80fa319e36b0a33
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/pyzmq-26.0.0-py312h2105c20_0.conda
+  sha256: b76223afe36332ac6472f8a2ff63de0ed018d24dcb414447eda05e8df58ca0e5
+  md5: a5e9d370c646a0d4cefedc5d6c5048b9
   depends:
-  - __osx >=10.9
-  - libcxx >=16.0.6
+  - libcxx >=16
   - libsodium >=1.0.18,<1.0.19.0a0
   - python >=3.12,<3.13.0a0
   - python >=3.12,<3.13.0a0 *_cpython
   - python_abi 3.12.* *_cp312
   - zeromq >=4.3.5,<4.4.0a0
-  license: BSD-3-Clause AND LGPL-3.0-or-later
+  license: BSD-3-Clause
+  license_family: BSD
   purls:
   - pkg:pypi/pyzmq
-  size: 495070
-  timestamp: 1701783687130
+  size: 446510
+  timestamp: 1713208013885
 - kind: conda
   name: pyzmq
-  version: 25.1.2
+  version: 26.0.0
   build: py312h886d080_0
   subdir: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.2-py312h886d080_0.conda
-  sha256: 5aa0ba1f67e2b25ede34a713df6655e519211a96ea109857768930d96bcd0ca0
-  md5: cc2cdf8f1792d29d21e17024745813d8
+  url: https://conda.anaconda.org/conda-forge/linux-64/pyzmq-26.0.0-py312h886d080_0.conda
+  sha256: c7fadc44057fe38d3b403ad435d8612172b981f02a30e399213f94760837d19f
+  md5: c06e639885a14ea35f77e9c0f3918808
   depends:
   - libgcc-ng >=12
   - libsodium >=1.0.18,<1.0.19.0a0
   - libstdcxx-ng >=12
   - python >=3.12,<3.13.0a0
   - python_abi 3.12.* *_cp312
   - zeromq >=4.3.5,<4.4.0a0
-  license: BSD-3-Clause AND LGPL-3.0-or-later
+  license: BSD-3-Clause
+  license_family: BSD
   purls:
   - pkg:pypi/pyzmq
-  size: 528745
-  timestamp: 1701783368181
+  size: 462029
+  timestamp: 1713207582684
 - kind: conda
   name: pyzmq
-  version: 25.1.2
-  build: py312hc789acb_0
+  version: 26.0.0
+  build: py312hb81df1d_0
   subdir: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.2-py312hc789acb_0.conda
-  sha256: 1e5fb7095be7edb90efd50cde7b417bf4f1f5ae216d0b597ada61ee201f56d29
-  md5: af49da330d412bc3203bc84f8153d685
+  url: https://conda.anaconda.org/conda-forge/osx-64/pyzmq-26.0.0-py312hb81df1d_0.conda
+  sha256: e9bc00caa0bfab25285161a400b2eca02994c6d4556abe185128ea7bbfb209b0
+  md5: 641c118ce3170463903086ffb677410e
   depends:
-  - __osx >=10.9
-  - libcxx >=16.0.6
+  - libcxx >=16
   - libsodium >=1.0.18,<1.0.19.0a0
   - python >=3.12,<3.13.0a0
   - python_abi 3.12.* *_cp312
   - zeromq >=4.3.5,<4.4.0a0
-  license: BSD-3-Clause AND LGPL-3.0-or-later
+  license: BSD-3-Clause
+  license_family: BSD
   purls:
   - pkg:pypi/pyzmq
-  size: 487865
-  timestamp: 1701783621950
+  size: 447416
+  timestamp: 1713207878913
 - kind: conda
   name: readline
   version: '8.2'
   build: h8228510_1
   build_number: 1
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
@@ -2865,41 +2871,41 @@
   requires_dist:
   - attrs >=22.2.0
   - rpds-py >=0.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
-  url: https://files.pythonhosted.org/packages/5a/57/2fcfd462cc53876ac4acef69dbf4fb941da971440049ca72051da54ea60d/rpds_py-0.18.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
-  sha256: cd5bf1af8efe569654bbef5a3e0a56eca45f87cfcffab31dd8dde70da5982475
-  requires_python: '>=3.8'
-- kind: pypi
-  name: rpds-py
-  version: 0.18.0
   url: https://files.pythonhosted.org/packages/09/b6/45690f5d3f8c551bb462e063a2f336d72c8884ed26aa19beb53a374d3854/rpds_py-0.18.0-cp312-cp312-macosx_10_12_x86_64.whl
   sha256: 7f2facbd386dd60cbbf1a794181e6aa0bd429bd78bfdf775436020172e2a23f0
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
-  url: https://files.pythonhosted.org/packages/14/8c/e69f5636f4ab6ee0855aef3b16e6c97f8b636e9e04fa5a4bcc75126acb13/rpds_py-0.18.0-cp312-none-win_amd64.whl
-  sha256: e003b002ec72c8d5a3e3da2989c7d6065b47d9eaa70cd8808b5384fbb970f4ec
+  url: https://files.pythonhosted.org/packages/7a/58/9bfc53b266df92f0515e72fd16e4890dc6b56fc3bfc216b3a2a729c866b5/rpds_py-0.18.0-cp312-cp312-macosx_11_0_arm64.whl
+  sha256: 1d9a5be316c15ffb2b3c405c4ff14448c36b4435be062a7f578ccd8b01f0c4d8
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
-  url: https://files.pythonhosted.org/packages/7a/58/9bfc53b266df92f0515e72fd16e4890dc6b56fc3bfc216b3a2a729c866b5/rpds_py-0.18.0-cp312-cp312-macosx_11_0_arm64.whl
-  sha256: 1d9a5be316c15ffb2b3c405c4ff14448c36b4435be062a7f578ccd8b01f0c4d8
+  url: https://files.pythonhosted.org/packages/5a/57/2fcfd462cc53876ac4acef69dbf4fb941da971440049ca72051da54ea60d/rpds_py-0.18.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
+  sha256: cd5bf1af8efe569654bbef5a3e0a56eca45f87cfcffab31dd8dde70da5982475
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
   url: https://files.pythonhosted.org/packages/c3/96/2211a1ca4b4e259e222169074ec0fa41f0ee18665dfc68988a139dc7e6e8/rpds_py-0.18.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
   sha256: 4457a94da0d5c53dc4b3e4de1158bdab077db23c53232f37a3cb7afdb053a4e3
   requires_python: '>=3.8'
+- kind: pypi
+  name: rpds-py
+  version: 0.18.0
+  url: https://files.pythonhosted.org/packages/14/8c/e69f5636f4ab6ee0855aef3b16e6c97f8b636e9e04fa5a4bcc75126acb13/rpds_py-0.18.0-cp312-none-win_amd64.whl
+  sha256: e003b002ec72c8d5a3e3da2989c7d6065b47d9eaa70cd8808b5384fbb970f4ec
+  requires_python: '>=3.8'
 - kind: conda
   name: six
   version: 1.16.0
   build: pyh6c4a22f_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
```

### Comparing `pixi_kernel-0.2.1/tests/integration/ipykernel/kernel.py` & `pixi_kernel-0.3.0/tests/integration/ipykernel/kernel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,15 @@
 """Reference: https://github.com/jupyter/jupyter_kernel_test/blob/5f2c65271b48dc95fc75a9585cb1d6db0bb55557/test_ipykernel.py"""
 # ruff: noqa: RUF012
 
-import os
 import unittest
-from contextlib import contextmanager
-from pathlib import Path
-from typing import Union
 
 import jupyter_kernel_test as jkt
 
 
-@contextmanager
-def cwd(new_dir: Union[str, Path]):
-    original_dir = Path.cwd().resolve()
-    try:
-        os.chdir(new_dir)
-        yield
-    finally:
-        os.chdir(original_dir)
-
-
 class IPyKernelTests(jkt.KernelTests):
     # the kernel to be tested
     # this is the normally the name of the directory containing the
     # kernel.json file - you should be able to do
     # `jupyter console --kernel KERNEL_NAME`
     kernel_name = "pixi-kernel-python3"
 
@@ -115,9 +101,8 @@
 
     # a code sample which should cause a `clear_output` message to be sent to
     # the client
     code_clear_output = "from IPython.display import clear_output; clear_output()"
 
 
 if __name__ == "__main__":
-    with cwd(Path(__file__).parent.resolve()):
-        unittest.main()
+    unittest.main()
```

### Comparing `pixi_kernel-0.2.1/tests/integration/ipykernel/pixi.lock` & `pixi_kernel-0.3.0/tests/integration/ipykernel/pixi.lock`

 * *Files 1% similar despite different names*

```diff
@@ -30,32 +30,32 @@
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.2-h2797004_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h7e041cc_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4.20240210-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.8-py312h98912ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.2-hab00c5b_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.12-4_cp312.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.2-py312h886d080_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/pyzmq-26.0.0-py312h886d080_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tornado-6.4-py312h98912ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
@@ -97,32 +97,32 @@
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libnsl-2.0.1-h31becfc_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libsodium-1.0.18-hb9de7d4_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libsqlite-3.45.2-h194ca79_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libstdcxx-ng-13.2.0-h9a76618_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libuuid-2.38.1-hb4cce97_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libxcrypt-4.4.36-h31becfc_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libzlib-1.2.13-h31becfc_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ncurses-6.4.20240210-h0425590_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/openssl-3.2.1-h31becfc_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/psutil-5.9.8-py312hdd3e373_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.2-h43d1f9e_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.3-h43d1f9e_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python_abi-3.12-4_cp312.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/pyzmq-25.1.2-py312h1c32067_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/pyzmq-26.0.0-py312h1c32067_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/readline-8.2-h8fc344f_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/tk-8.6.13-h194ca79_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/tornado-6.4-py312h9ef2f89_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
@@ -158,32 +158,32 @@
       - conda: https://conda.anaconda.org/conda-forge/osx-64/jupyter_core-5.7.2-py312hb401068_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libexpat-2.6.2-h73e2aa4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.2-h92b6c6a_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4.20240210-h73e2aa4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.2.1-hd75f5a5_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.8-py312h41838bb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.2-h9f0c242_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.12-4_cp312.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.2-py312hc789acb_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/pyzmq-26.0.0-py312hb81df1d_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tornado-6.4-py312h41838bb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
@@ -219,32 +219,32 @@
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/jupyter_core-5.7.2-py312h81bd7bf_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libcxx-16.0.6-h4653b0c_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libexpat-2.6.2-hebf3989_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libffi-3.4.2-h3422bc3_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libsodium-1.0.18-h27ca646_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libsqlite-3.45.2-h091b4b1_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libzlib-1.2.13-h53f4e23_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ncurses-6.4.20240210-h078ce10_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.2.1-h0d3ecfb_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/psutil-5.9.8-py312he37b823_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.2-hdf0ec26_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.3-h4a7b5fc_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.12-4_cp312.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pyzmq-25.1.2-py312h1edf716_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pyzmq-26.0.0-py312h2105c20_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tornado-6.4-py312he37b823_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
@@ -279,30 +279,30 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.6.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/jupyter_core-5.7.2-py312h2e8e312_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libexpat-2.6.2-h63175ca_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.2-hcfcfb64_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/openssl-3.2.1-hcfcfb64_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.8-py312he70551f_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.2-h2628c8c_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.3-h2628c8c_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/pywin32-306-py312h53d5487_2.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/pyzmq-25.1.2-py312h1ac6f91_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/pyzmq-26.0.0-py312h1ac6f91_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/tornado-6.4-py312he70551f_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
@@ -608,16 +608,16 @@
   - libcxx >=16
   - python >=3.12,<3.13.0a0
   - python >=3.12,<3.13.0a0 *_cpython
   - python_abi 3.12.* *_cp312
   license: MIT
   license_family: MIT
   purls:
-  - pkg:pypi/bytecode
   - pkg:pypi/debugpy
+  - pkg:pypi/bytecode
   size: 2077038
   timestamp: 1707445014387
 - kind: conda
   name: debugpy
   version: 1.8.1
   build: py312h2aa54b4_0
   subdir: linux-aarch64
@@ -670,16 +670,16 @@
   - python_abi 3.12.* *_cp312
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   license: MIT
   license_family: MIT
   purls:
-  - pkg:pypi/debugpy
   - pkg:pypi/bytecode
+  - pkg:pypi/debugpy
   size: 3105043
   timestamp: 1707445249662
 - kind: conda
   name: debugpy
   version: 1.8.1
   build: py312hede676d_0
   subdir: osx-64
@@ -1706,35 +1706,35 @@
   - zlib 1.2.13 *_5
   license: Zlib
   license_family: Other
   size: 61588
   timestamp: 1686575217516
 - kind: conda
   name: matplotlib-inline
-  version: 0.1.6
+  version: 0.1.7
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
-  url: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2
-  sha256: aa091b88aec55bfa2d9207028d8cdc689b9efb090ae27b99557e93c675be2f3c
-  md5: b21613793fcc81d944c76c9f2864a7de
+  url: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
+  sha256: 7ea68676ea35fbb095420bbcc1c82c4767b8be7bb56abb6989b7f89d957a3bab
+  md5: 779345c95648be40d22aaa89de7d4254
   depends:
   - python >=3.6
   - traitlets
   license: BSD-3-Clause
   license_family: BSD
   purls:
   - pkg:pypi/matplotlib-inline
-  size: 12273
-  timestamp: 1660814913405
+  size: 14599
+  timestamp: 1713250613726
 - kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/1d/b5/c8fbf1db814eb29eda402952374b594b2559419ba7ec6d0997a9e5687530/msgspec-0.18.6-cp312-cp312-macosx_10_9_x86_64.whl
-  sha256: d86f5071fe33e19500920333c11e2267a31942d18fed4d9de5bc2fbab267d28c
+  url: https://files.pythonhosted.org/packages/73/16/dfef780ced7d690dd5497846ed242ef3e27e319d59d1ddaae816a4f2c15e/msgspec-0.18.6-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: ad237100393f637b297926cae1868b0d500f764ccd2f0623a380e2bcfb2809ca
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -1764,16 +1764,16 @@
   - tomli-w ; extra == 'toml'
   - tomli ; python_version < '3.11' and extra == 'toml'
   - pyyaml ; extra == 'yaml'
   requires_python: '>=3.8'
 - kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/d7/9a/235d2dbab078a0b8e6f338205dc59be0b027ce000554ee6a9c41b19339e5/msgspec-0.18.6-cp312-cp312-macosx_11_0_arm64.whl
-  sha256: ce13981bfa06f5eb126a3a5a38b1976bddb49a36e4f46d8e6edecf33ccf11df1
+  url: https://files.pythonhosted.org/packages/0e/f2/f864ed36a8a62c26b57c3e08d212bd8f3d12a3ca3ef64600be5452aa3c82/msgspec-0.18.6-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
+  sha256: e97dec6932ad5e3ee1e3c14718638ba333befc45e0661caa57033cd4cc489466
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -1803,16 +1803,16 @@
   - tomli-w ; extra == 'toml'
   - tomli ; python_version < '3.11' and extra == 'toml'
   - pyyaml ; extra == 'yaml'
   requires_python: '>=3.8'
 - kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/73/16/dfef780ced7d690dd5497846ed242ef3e27e319d59d1ddaae816a4f2c15e/msgspec-0.18.6-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: ad237100393f637b297926cae1868b0d500f764ccd2f0623a380e2bcfb2809ca
+  url: https://files.pythonhosted.org/packages/1d/b5/c8fbf1db814eb29eda402952374b594b2559419ba7ec6d0997a9e5687530/msgspec-0.18.6-cp312-cp312-macosx_10_9_x86_64.whl
+  sha256: d86f5071fe33e19500920333c11e2267a31942d18fed4d9de5bc2fbab267d28c
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -1842,16 +1842,16 @@
   - tomli-w ; extra == 'toml'
   - tomli ; python_version < '3.11' and extra == 'toml'
   - pyyaml ; extra == 'yaml'
   requires_python: '>=3.8'
 - kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/0e/f2/f864ed36a8a62c26b57c3e08d212bd8f3d12a3ca3ef64600be5452aa3c82/msgspec-0.18.6-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
-  sha256: e97dec6932ad5e3ee1e3c14718638ba333befc45e0661caa57033cd4cc489466
+  url: https://files.pythonhosted.org/packages/d7/9a/235d2dbab078a0b8e6f338205dc59be0b027ce000554ee6a9c41b19339e5/msgspec-0.18.6-cp312-cp312-macosx_11_0_arm64.whl
+  sha256: ce13981bfa06f5eb126a3a5a38b1976bddb49a36e4f46d8e6edecf33ccf11df1
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -2143,18 +2143,19 @@
   license_family: MIT
   purls:
   - pkg:pypi/pickleshare
   size: 9332
   timestamp: 1602536313357
 - kind: pypi
   name: pixi-kernel
-  version: 0.2.1
+  version: 0.3.0
   path: ../../../../pixi-kernel
-  sha256: fc89be37749334e0eb20e8656e5ffcdace662e69fd273fa798213fdf1e64b7cb
+  sha256: 026726c0f08b63327906964394fdaf6d1b2324c25bf50c37e37b0300731fba40
   requires_dist:
+  - ipykernel >=6
   - jupyter-client >=7
   - msgspec >=0.18
   requires_python: <4.0,>=3.8
   editable: true
 - kind: conda
   name: platformdirs
   version: 4.2.0
@@ -2332,148 +2333,150 @@
   license_family: BSD
   purls:
   - pkg:pypi/pygments
   size: 860425
   timestamp: 1700608076927
 - kind: conda
   name: python
-  version: 3.12.2
+  version: 3.12.3
+  build: h1411813_0_cpython
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda
+  sha256: 3b327ffc152a245011011d1d730781577a8274fde1cf6243f073749ead8f1c2a
+  md5: df1448ec6cbf8eceb03d29003cf72ae6
+  depends:
+  - __osx >=10.9
+  - bzip2 >=1.0.8,<2.0a0
+  - libexpat >=2.6.2,<3.0a0
+  - libffi >=3.4,<4.0a0
+  - libsqlite >=3.45.2,<4.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - ncurses >=6.4.20240210,<7.0a0
+  - openssl >=3.2.1,<4.0a0
+  - readline >=8.2,<9.0a0
+  - tk >=8.6.13,<8.7.0a0
+  - tzdata
+  - xz >=5.2.6,<6.0a0
+  constrains:
+  - python_abi 3.12.* *_cp312
+  license: Python-2.0
+  size: 14557341
+  timestamp: 1713208068012
+- kind: conda
+  name: python
+  version: 3.12.3
   build: h2628c8c_0_cpython
   subdir: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/python-3.12.2-h2628c8c_0_cpython.conda
-  sha256: b8eda863b48ae4531635e23fd15e759d93212b6204c6847d591e25fa5fd67477
-  md5: be8803e9f75a477df61d4aabea3c1246
+  url: https://conda.anaconda.org/conda-forge/win-64/python-3.12.3-h2628c8c_0_cpython.conda
+  sha256: 1a95494abe572a8819c933f978df89f00bde72ea9432d46a70632599e8029ea4
+  md5: f07c8c5dd98767f9a652de5d039b284e
   depends:
   - bzip2 >=1.0.8,<2.0a0
-  - libexpat >=2.5.0,<3.0a0
+  - libexpat >=2.6.2,<3.0a0
   - libffi >=3.4,<4.0a0
-  - libsqlite >=3.45.1,<4.0a0
+  - libsqlite >=3.45.2,<4.0a0
   - libzlib >=1.2.13,<1.3.0a0
   - openssl >=3.2.1,<4.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.12.* *_cp312
   license: Python-2.0
-  size: 16083296
-  timestamp: 1708116662336
+  size: 16179248
+  timestamp: 1713205644673
 - kind: conda
   name: python
-  version: 3.12.2
+  version: 3.12.3
   build: h43d1f9e_0_cpython
   subdir: linux-aarch64
-  url: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.2-h43d1f9e_0_cpython.conda
-  sha256: 16c8e77c01b814d836af632ef77eac21b64b9e398a11e1403a3a1802bb5be366
-  md5: 3a41090f2ef0868f119825593948ed46
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.3-h43d1f9e_0_cpython.conda
+  sha256: e186f3ee570464241c844adff6a3ba8f395cef15c5d46c0a8f784cfd97b3bdca
+  md5: dc93ad1d2ba17ebc948bf5434ffa864b
   depends:
   - bzip2 >=1.0.8,<2.0a0
   - ld_impl_linux-aarch64 >=2.36.1
-  - libexpat >=2.5.0,<3.0a0
+  - libexpat >=2.6.2,<3.0a0
   - libffi >=3.4,<4.0a0
   - libgcc-ng >=12
   - libnsl >=2.0.1,<2.1.0a0
-  - libsqlite >=3.45.1,<4.0a0
+  - libsqlite >=3.45.2,<4.0a0
   - libuuid >=2.38.1,<3.0a0
   - libxcrypt >=4.4.36
   - libzlib >=1.2.13,<1.3.0a0
-  - ncurses >=6.4,<7.0a0
+  - ncurses >=6.4.20240210,<7.0a0
   - openssl >=3.2.1,<4.0a0
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.12.* *_cp312
   license: Python-2.0
-  size: 13823577
-  timestamp: 1708116074721
+  size: 14051797
+  timestamp: 1713205211165
 - kind: conda
   name: python
-  version: 3.12.2
-  build: h9f0c242_0_cpython
-  subdir: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.2-h9f0c242_0_cpython.conda
-  sha256: 7647ac06c3798a182a4bcb1ff58864f1ef81eb3acea6971295304c23e43252fb
-  md5: 0179b8007ba008cf5bec11f3b3853902
+  version: 3.12.3
+  build: h4a7b5fc_0_cpython
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.3-h4a7b5fc_0_cpython.conda
+  sha256: c761fb3713ea66bce3889b33b6f400afb2dd192d1fc2686446e9d8166cfcec6b
+  md5: 8643ab37bece6ae8f112464068d9df9c
   depends:
+  - __osx >=11.0
   - bzip2 >=1.0.8,<2.0a0
-  - libexpat >=2.5.0,<3.0a0
+  - libexpat >=2.6.2,<3.0a0
   - libffi >=3.4,<4.0a0
-  - libsqlite >=3.45.1,<4.0a0
+  - libsqlite >=3.45.2,<4.0a0
   - libzlib >=1.2.13,<1.3.0a0
-  - ncurses >=6.4,<7.0a0
+  - ncurses >=6.4.20240210,<7.0a0
   - openssl >=3.2.1,<4.0a0
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.12.* *_cp312
   license: Python-2.0
-  size: 14596811
-  timestamp: 1708118065292
+  size: 13207557
+  timestamp: 1713206576646
 - kind: conda
   name: python
-  version: 3.12.2
+  version: 3.12.3
   build: hab00c5b_0_cpython
   subdir: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.2-hab00c5b_0_cpython.conda
-  sha256: ddb7a2d8d78046bda5d7631e6814f9468d2eb054e10f86f4648c9d1fdaa30c0f
-  md5: ad7b68400f3a6ebe72b00be093c7f301
+  url: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda
+  sha256: f9865bcbff69f15fd89a33a2da12ad616e98d65ce7c83c644b92e66e5016b227
+  md5: 2540b74d304f71d3e89c81209db4db84
   depends:
   - bzip2 >=1.0.8,<2.0a0
   - ld_impl_linux-64 >=2.36.1
-  - libexpat >=2.5.0,<3.0a0
+  - libexpat >=2.6.2,<3.0a0
   - libffi >=3.4,<4.0a0
   - libgcc-ng >=12
   - libnsl >=2.0.1,<2.1.0a0
-  - libsqlite >=3.45.1,<4.0a0
+  - libsqlite >=3.45.2,<4.0a0
   - libuuid >=2.38.1,<3.0a0
   - libxcrypt >=4.4.36
   - libzlib >=1.2.13,<1.3.0a0
-  - ncurses >=6.4,<7.0a0
+  - ncurses >=6.4.20240210,<7.0a0
   - openssl >=3.2.1,<4.0a0
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.12.* *_cp312
   license: Python-2.0
-  size: 32312631
-  timestamp: 1708118077305
-- kind: conda
-  name: python
-  version: 3.12.2
-  build: hdf0ec26_0_cpython
-  subdir: osx-arm64
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.2-hdf0ec26_0_cpython.conda
-  sha256: ccd6c55a286d51d907c878ed2bfa7d1becce0fee71374a9386c5eb90d803ac72
-  md5: 85e91138ae921a2771f57a50120272bd
-  depends:
-  - bzip2 >=1.0.8,<2.0a0
-  - libexpat >=2.5.0,<3.0a0
-  - libffi >=3.4,<4.0a0
-  - libsqlite >=3.45.1,<4.0a0
-  - libzlib >=1.2.13,<1.3.0a0
-  - ncurses >=6.4,<7.0a0
-  - openssl >=3.2.1,<4.0a0
-  - readline >=8.2,<9.0a0
-  - tk >=8.6.13,<8.7.0a0
-  - tzdata
-  - xz >=5.2.6,<6.0a0
-  constrains:
-  - python_abi 3.12.* *_cp312
-  license: Python-2.0
-  size: 13085901
-  timestamp: 1708117361381
+  size: 31991381
+  timestamp: 1713208036041
 - kind: conda
   name: python-dateutil
   version: 2.9.0
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
@@ -2582,114 +2585,117 @@
   license_family: PSF
   purls:
   - pkg:pypi/pywin32
   size: 6127499
   timestamp: 1695974557413
 - kind: conda
   name: pyzmq
-  version: 25.1.2
+  version: 26.0.0
   build: py312h1ac6f91_0
   subdir: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/pyzmq-25.1.2-py312h1ac6f91_0.conda
-  sha256: 9371101999c75aa562c5aa4ae0dfefa140bee635a3f8e15768628689f70d7765
-  md5: 74194f888cc7b11d8c18edf416b61a1b
+  url: https://conda.anaconda.org/conda-forge/win-64/pyzmq-26.0.0-py312h1ac6f91_0.conda
+  sha256: 8d12105518f4ae9bbf48bbdbe031a0b3f2c0b1378350422172af2afc77014f54
+  md5: c69d5948bed236b2cfa323dd478d8de8
   depends:
   - libsodium >=1.0.18,<1.0.19.0a0
   - python >=3.12,<3.13.0a0
   - python_abi 3.12.* *_cp312
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   - zeromq >=4.3.5,<4.3.6.0a0
-  license: BSD-3-Clause AND LGPL-3.0-or-later
+  license: BSD-3-Clause
+  license_family: BSD
   purls:
   - pkg:pypi/pyzmq
-  size: 480772
-  timestamp: 1701783863250
+  size: 444664
+  timestamp: 1713208522670
 - kind: conda
   name: pyzmq
-  version: 25.1.2
+  version: 26.0.0
   build: py312h1c32067_0
   subdir: linux-aarch64
-  url: https://conda.anaconda.org/conda-forge/linux-aarch64/pyzmq-25.1.2-py312h1c32067_0.conda
-  sha256: 7394b1de60b33bbe7fc62d67a838671777cfe725074332d61861457efa0c1f62
-  md5: 7b450f76fbf279bd05304bc9fd879ff0
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/pyzmq-26.0.0-py312h1c32067_0.conda
+  sha256: 5c87c69960aba5292df0e8ece531b97f294336c15d022d2efafb171ab080983d
+  md5: 7f6de7d76e5253bdf14a9088fec24f04
   depends:
   - libgcc-ng >=12
   - libsodium >=1.0.18,<1.0.19.0a0
   - libstdcxx-ng >=12
   - python >=3.12,<3.13.0a0
   - python_abi 3.12.* *_cp312
   - zeromq >=4.3.5,<4.4.0a0
-  license: BSD-3-Clause AND LGPL-3.0-or-later
+  license: BSD-3-Clause
+  license_family: BSD
   purls:
   - pkg:pypi/pyzmq
-  size: 530614
-  timestamp: 1701785140508
+  size: 457757
+  timestamp: 1713209766265
 - kind: conda
   name: pyzmq
-  version: 25.1.2
-  build: py312h1edf716_0
+  version: 26.0.0
+  build: py312h2105c20_0
   subdir: osx-arm64
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/pyzmq-25.1.2-py312h1edf716_0.conda
-  sha256: a89712c6b0cab1e3385e44e0130a57b9d03df99b6f540486c0f00e2dae079e77
-  md5: 913db29987f836f5d80fa319e36b0a33
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/pyzmq-26.0.0-py312h2105c20_0.conda
+  sha256: b76223afe36332ac6472f8a2ff63de0ed018d24dcb414447eda05e8df58ca0e5
+  md5: a5e9d370c646a0d4cefedc5d6c5048b9
   depends:
-  - __osx >=10.9
-  - libcxx >=16.0.6
+  - libcxx >=16
   - libsodium >=1.0.18,<1.0.19.0a0
   - python >=3.12,<3.13.0a0
   - python >=3.12,<3.13.0a0 *_cpython
   - python_abi 3.12.* *_cp312
   - zeromq >=4.3.5,<4.4.0a0
-  license: BSD-3-Clause AND LGPL-3.0-or-later
+  license: BSD-3-Clause
+  license_family: BSD
   purls:
   - pkg:pypi/pyzmq
-  size: 495070
-  timestamp: 1701783687130
+  size: 446510
+  timestamp: 1713208013885
 - kind: conda
   name: pyzmq
-  version: 25.1.2
+  version: 26.0.0
   build: py312h886d080_0
   subdir: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.2-py312h886d080_0.conda
-  sha256: 5aa0ba1f67e2b25ede34a713df6655e519211a96ea109857768930d96bcd0ca0
-  md5: cc2cdf8f1792d29d21e17024745813d8
+  url: https://conda.anaconda.org/conda-forge/linux-64/pyzmq-26.0.0-py312h886d080_0.conda
+  sha256: c7fadc44057fe38d3b403ad435d8612172b981f02a30e399213f94760837d19f
+  md5: c06e639885a14ea35f77e9c0f3918808
   depends:
   - libgcc-ng >=12
   - libsodium >=1.0.18,<1.0.19.0a0
   - libstdcxx-ng >=12
   - python >=3.12,<3.13.0a0
   - python_abi 3.12.* *_cp312
   - zeromq >=4.3.5,<4.4.0a0
-  license: BSD-3-Clause AND LGPL-3.0-or-later
+  license: BSD-3-Clause
+  license_family: BSD
   purls:
   - pkg:pypi/pyzmq
-  size: 528745
-  timestamp: 1701783368181
+  size: 462029
+  timestamp: 1713207582684
 - kind: conda
   name: pyzmq
-  version: 25.1.2
-  build: py312hc789acb_0
+  version: 26.0.0
+  build: py312hb81df1d_0
   subdir: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/pyzmq-25.1.2-py312hc789acb_0.conda
-  sha256: 1e5fb7095be7edb90efd50cde7b417bf4f1f5ae216d0b597ada61ee201f56d29
-  md5: af49da330d412bc3203bc84f8153d685
+  url: https://conda.anaconda.org/conda-forge/osx-64/pyzmq-26.0.0-py312hb81df1d_0.conda
+  sha256: e9bc00caa0bfab25285161a400b2eca02994c6d4556abe185128ea7bbfb209b0
+  md5: 641c118ce3170463903086ffb677410e
   depends:
-  - __osx >=10.9
-  - libcxx >=16.0.6
+  - libcxx >=16
   - libsodium >=1.0.18,<1.0.19.0a0
   - python >=3.12,<3.13.0a0
   - python_abi 3.12.* *_cp312
   - zeromq >=4.3.5,<4.4.0a0
-  license: BSD-3-Clause AND LGPL-3.0-or-later
+  license: BSD-3-Clause
+  license_family: BSD
   purls:
   - pkg:pypi/pyzmq
-  size: 487865
-  timestamp: 1701783621950
+  size: 447416
+  timestamp: 1713207878913
 - kind: conda
   name: readline
   version: '8.2'
   build: h8228510_1
   build_number: 1
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
@@ -2756,34 +2762,34 @@
   requires_dist:
   - attrs >=22.2.0
   - rpds-py >=0.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
-  url: https://files.pythonhosted.org/packages/09/b6/45690f5d3f8c551bb462e063a2f336d72c8884ed26aa19beb53a374d3854/rpds_py-0.18.0-cp312-cp312-macosx_10_12_x86_64.whl
-  sha256: 7f2facbd386dd60cbbf1a794181e6aa0bd429bd78bfdf775436020172e2a23f0
+  url: https://files.pythonhosted.org/packages/c3/96/2211a1ca4b4e259e222169074ec0fa41f0ee18665dfc68988a139dc7e6e8/rpds_py-0.18.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: 4457a94da0d5c53dc4b3e4de1158bdab077db23c53232f37a3cb7afdb053a4e3
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
-  url: https://files.pythonhosted.org/packages/7a/58/9bfc53b266df92f0515e72fd16e4890dc6b56fc3bfc216b3a2a729c866b5/rpds_py-0.18.0-cp312-cp312-macosx_11_0_arm64.whl
-  sha256: 1d9a5be316c15ffb2b3c405c4ff14448c36b4435be062a7f578ccd8b01f0c4d8
+  url: https://files.pythonhosted.org/packages/5a/57/2fcfd462cc53876ac4acef69dbf4fb941da971440049ca72051da54ea60d/rpds_py-0.18.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
+  sha256: cd5bf1af8efe569654bbef5a3e0a56eca45f87cfcffab31dd8dde70da5982475
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
-  url: https://files.pythonhosted.org/packages/c3/96/2211a1ca4b4e259e222169074ec0fa41f0ee18665dfc68988a139dc7e6e8/rpds_py-0.18.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: 4457a94da0d5c53dc4b3e4de1158bdab077db23c53232f37a3cb7afdb053a4e3
+  url: https://files.pythonhosted.org/packages/09/b6/45690f5d3f8c551bb462e063a2f336d72c8884ed26aa19beb53a374d3854/rpds_py-0.18.0-cp312-cp312-macosx_10_12_x86_64.whl
+  sha256: 7f2facbd386dd60cbbf1a794181e6aa0bd429bd78bfdf775436020172e2a23f0
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
-  url: https://files.pythonhosted.org/packages/5a/57/2fcfd462cc53876ac4acef69dbf4fb941da971440049ca72051da54ea60d/rpds_py-0.18.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
-  sha256: cd5bf1af8efe569654bbef5a3e0a56eca45f87cfcffab31dd8dde70da5982475
+  url: https://files.pythonhosted.org/packages/7a/58/9bfc53b266df92f0515e72fd16e4890dc6b56fc3bfc216b3a2a729c866b5/rpds_py-0.18.0-cp312-cp312-macosx_11_0_arm64.whl
+  sha256: 1d9a5be316c15ffb2b3c405c4ff14448c36b4435be062a7f578ccd8b01f0c4d8
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
   url: https://files.pythonhosted.org/packages/14/8c/e69f5636f4ab6ee0855aef3b16e6c97f8b636e9e04fa5a4bcc75126acb13/rpds_py-0.18.0-cp312-none-win_amd64.whl
   sha256: e003b002ec72c8d5a3e3da2989c7d6065b47d9eaa70cd8808b5384fbb970f4ec
   requires_python: '>=3.8'
```

### Comparing `pixi_kernel-0.2.1/tests/integration/r-irkernel/kernel.py` & `pixi_kernel-0.3.0/tests/integration/r-irkernel/kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,25 @@
 """Reference: https://github.com/IRkernel/IRkernel/blob/1eddb304b246c14b62949abd946e8d4ca5080d25/tests/testthat/test_ir.py"""
 # ruff: noqa: RUF012
 
-import os
 import platform
 import unittest
-from contextlib import contextmanager
-from pathlib import Path
-from typing import Union
 
 import jupyter_kernel_test as jkt
 
 without_rich_display = """\
 options(jupyter.rich_display = FALSE)
 {}
 options(jupyter.rich_display = TRUE)
 """
 
 
 TIMEOUT = 15
 
 
-@contextmanager
-def cwd(new_dir: Union[str, Path]):
-    original_dir = Path.cwd().resolve()
-    try:
-        os.chdir(new_dir)
-        yield
-    finally:
-        os.chdir(original_dir)
-
-
 class IRKernelTests(jkt.KernelTests):
     # the kernel to be tested
     # this is the normally the name of the directory containing the
     # kernel.json file - you should be able to do
     # `jupyter console --kernel KERNEL_NAME`
     kernel_name = "pixi-kernel-ir"
 
@@ -409,9 +395,8 @@
                 assert set(reply["content"]["matches"]) == set(sample["matches"])
 
                 for var_name in sample["vars"]:
                     self._execute_code(f"rm({var_name})", tests=False)
 
 
 if __name__ == "__main__":
-    with cwd(Path(__file__).parent.resolve()):
-        unittest.main()
+    unittest.main()
```

### Comparing `pixi_kernel-0.2.1/tests/integration/r-irkernel/pixi.lock` & `pixi_kernel-0.3.0/tests/integration/r-irkernel/pixi.lock`

 * *Files 3% similar despite different names*

```diff
@@ -66,26 +66,26 @@
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.2-h2797004_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.11.0-h0841786_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/libstdcxx-devel_linux-64-13.2.0-ha9c7c90_105.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h7e041cc_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.6.0-h1dd3fc0_3.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.2-hd590300_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.4.0-hd590300_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.15-h0b41bf4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/make-4.3-hd18ef5c_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4.20240210-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/pango-1.52.1-ha41ecd1_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.42-hcad00b1_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/pixman-0.43.2-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/pthread-stubs-0.4-h36c2ea0_1001.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.2-hab00c5b_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/r-base-4.3.3-hb8ee39d_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/r-base64enc-0.1_3-r43h57805ef_1006.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/r-cli-3.6.2-r43ha503ecb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/r-crayon-1.5.2-r43hc72bb7e_2.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/r-digest-0.6.35-r43ha503ecb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/r-ellipsis-0.3.2-r43h57805ef_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/r-evaluate-0.23-r43hc72bb7e_0.conda
@@ -122,29 +122,49 @@
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xorg-renderproto-0.11.1-h7f98852_1002.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xorg-xextproto-7.3.0-h0b41bf4_1003.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xorg-xproto-7.0.31-h7f98852_1007.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.5-h59595ed_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.5-hfc55251_0.conda
+      - pypi: https://files.pythonhosted.org/packages/45/86/4736ac618d82a20d87d2f92ae19441ebc7ac9e7a581d7e58bbe79233b24a/asttokens-2.4.1-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/e0/44/827b2a91a5816512fcaf3cc4ebc465ccd5d598c45cefa6703fcf4a79018f/attrs-23.2.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/e6/75/49e5bfe642f71f272236b5b2d2691cf915a7283cc0ceda56357b61daa538/comm-0.2.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/3c/7a/e400d9f5ed6b4b5ec9f350b4d7974e986ca2d455221e567e648edfad898e/debugpy-1.8.1-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+      - pypi: https://files.pythonhosted.org/packages/d5/50/83c593b07763e1161326b3b8c6686f0f4b0f24d5526546bee538c89837d6/decorator-5.1.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/80/03/6ea8b1b2a5ab40a7a60dc464d3daa7aa546e0a74d74a9f8ff551ea7905db/executing-2.0.1-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/53/9d/40d5207db523363d9b5698f33778c18b0d591e3fdb6e0116b894b2a2491c/ipykernel-6.29.4-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/8a/15/ea245239487bbd8d7203fe010ea48c7539e42bf1fde0592313241a3fba3a/ipython-8.23.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/20/9f/bc63f0f0737ad7a60800bfd472a4836661adae21f9c2535f3957b1e54ceb/jedi-0.19.1-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/39/9d/b035d024c62c85f2e2d4806a59ca7b8520307f34e0932fbc8cc75fe7b2d9/jsonschema-4.21.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/ee/07/44bd408781594c4d0a027666ef27fab1e441b109dc3b76b4f836f8fd04fe/jsonschema_specifications-2023.12.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/75/6d/d7b55b9c1ac802ab066b3e5015e90faab1fffbbd67a2af498ffc6cc81c97/jupyter_client-8.6.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/c9/fb/108ecd1fe961941959ad0ee4e12ee7b8b1477247f30b1fdfd83ceaf017f0/jupyter_core-5.7.2-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/72/42/d57a938cad4e99bb799f35105561959b0a0550c65fbc1ed671196e27f909/jupyter_kernel_test-0.7.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/8f/8e/9ad090d3553c280a8060fbf6e24dc1c0c29704ee7d1c372f0c174aa59285/matplotlib_inline-0.1.7-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/73/16/dfef780ced7d690dd5497846ed242ef3e27e319d59d1ddaae816a4f2c15e/msgspec-0.18.6-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+      - pypi: https://files.pythonhosted.org/packages/a0/c4/c2971a3ba4c6103a3d10c4b0f24f461ddc027f0f09763220cf35ca1401b3/nest_asyncio-1.6.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/49/df/1fceb2f8900f8639e278b056416d49134fb8d84c5942ffaa01ad34782422/packaging-24.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/c6/ac/dac4a63f978e4dcb3c6d3a78c4d8e0192a113d288502a1216950c41b1027/parso-0.8.4-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/9e/c3/059298687310d527a58bb01f3b1965787ee3b40dce76752eda8b44e9a2c5/pexpect-4.9.0-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/55/72/4898c44ee9ea6f43396fbc23d9bfaf3d06e01b83698bdf2e4c919deceb7c/platformdirs-4.2.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/ee/fd/ca7bf3869e7caa7a037e23078539467b433a4e01eebd93f77180ab927766/prompt_toolkit-3.0.43-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/c5/4f/0e22aaa246f96d6ac87fe5ebb9c5a693fbe8877f537a1022527c47ca43c5/psutil-5.9.8-cp36-abi3-manylinux_2_12_x86_64.manylinux2010_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+      - pypi: https://files.pythonhosted.org/packages/22/a6/858897256d0deac81a172289110f31629fc4cee19b6f01283303e18c8db3/ptyprocess-0.7.0-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/2b/27/77f9d5684e6bce929f5cfe18d6cfbe5133013c06cb2fbf5933670e60761d/pure_eval-0.2.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/97/9c/372fef8377a6e340b1704768d20daaded98bf13282b5327beb2e2fe2c7ef/pygments-2.17.2-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/ec/57/56b9bcc3c9c6a792fcbaf139543cee77261f3651ca9da0c93f5c1221264b/python_dateutil-2.9.0.post0-py2.py3-none-any.whl
-      - pypi: https://files.pythonhosted.org/packages/93/b7/6e291eafbbbc66d0e87658dd21383ec2b4ab35edcfb283902c580a6db76f/pyzmq-25.1.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+      - pypi: https://files.pythonhosted.org/packages/61/01/eb6165d9160065845179f8f168ea70eaa24aa7e63f53b13966bbe368d6fa/pyzmq-26.0.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
       - pypi: https://files.pythonhosted.org/packages/42/8e/ae1de7b12223986e949bdb886c004de7c304b6fa94de5b87c926c1099656/referencing-0.34.0-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/c3/96/2211a1ca4b4e259e222169074ec0fa41f0ee18665dfc68988a139dc7e6e8/rpds_py-0.18.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
       - pypi: https://files.pythonhosted.org/packages/d9/5a/e7c31adbe875f2abbb91bd84cf2dc52d792b5a01506781dbcf25c91daf11/six-1.16.0-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/f1/7b/ce1eafaf1a76852e2ec9b22edecf1daa58175c090266e9f6c64afcd81d91/stack_data-0.6.3-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/9f/12/11d0a757bb67278d3380d41955ae98527d5ad18330b2edbdc8de222b569b/tornado-6.4-cp38-abi3-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl
       - pypi: https://files.pythonhosted.org/packages/7c/c4/366a09036c07f46eb8c9b2af39c97f502ef24f11f2a6e4d763655d9f2708/traitlets-5.14.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/fd/84/fd2ba7aafacbad3c4201d395674fc6348826569da3c0937e75505ead3528/wcwidth-0.2.13-py2.py3-none-any.whl
       - pypi: ../../../../pixi-kernel
       linux-aarch64:
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/_openmp_mutex-4.5-2_gnu.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/_r-mutex-1.0.1-anacondar_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/_sysroot_linux-aarch64_curr_repodata_hack-4-h57d6b7b_14.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/binutils_impl_linux-aarch64-2.40-h870a726_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/bwidget-1.9.14-h8af1aa0_1.tar.bz2
@@ -204,26 +224,26 @@
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libsodium-1.0.18-hb9de7d4_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libsqlite-3.45.2-h194ca79_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libssh2-1.11.0-h492db2e_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/libstdcxx-devel_linux-aarch64-13.2.0-h0a96a4f_105.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libstdcxx-ng-13.2.0-h9a76618_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libtiff-4.6.0-hf980d43_3.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libuuid-2.38.1-hb4cce97_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libwebp-base-1.3.2-h31becfc_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libwebp-base-1.4.0-h31becfc_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libxcb-1.15-h2a766a3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libxcrypt-4.4.36-h31becfc_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/libzlib-1.2.13-h31becfc_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/make-4.3-h309ac5b_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/ncurses-6.4.20240210-h0425590_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/openssl-3.2.1-h31becfc_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/pango-1.52.1-h11ef544_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/pcre2-10.42-hd0f9c67_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/pixman-0.43.4-h2f0025b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/pthread-stubs-0.4-hb9de7d4_1001.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.2-h43d1f9e_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.3-h43d1f9e_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/r-base-4.3.3-h7dc8e12_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/r-base64enc-0.1_3-r43h25e906a_1006.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/r-cli-3.6.2-r43h93f32a7_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/r-crayon-1.5.2-r43hc72bb7e_2.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/r-digest-0.6.35-r43h93f32a7_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/r-ellipsis-0.3.2-r43h25e906a_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/r-evaluate-0.23-r43hc72bb7e_0.conda
@@ -260,29 +280,49 @@
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/xorg-renderproto-0.11.1-h3557bc0_1002.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/xorg-xextproto-7.3.0-h2a766a3_1003.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/xorg-xproto-7.0.31-h3557bc0_1007.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/xz-5.2.6-h9cdd2b7_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/zeromq-4.3.5-h2f0025b_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/zlib-1.2.13-h31becfc_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/zstd-1.5.5-h4c53e97_0.conda
+      - pypi: https://files.pythonhosted.org/packages/45/86/4736ac618d82a20d87d2f92ae19441ebc7ac9e7a581d7e58bbe79233b24a/asttokens-2.4.1-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/e0/44/827b2a91a5816512fcaf3cc4ebc465ccd5d598c45cefa6703fcf4a79018f/attrs-23.2.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/e6/75/49e5bfe642f71f272236b5b2d2691cf915a7283cc0ceda56357b61daa538/comm-0.2.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/57/ab/6df7e24db51e1db642a5ea1759d44fb656251253995a27deb37af9b192ae/debugpy-1.8.1-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/d5/50/83c593b07763e1161326b3b8c6686f0f4b0f24d5526546bee538c89837d6/decorator-5.1.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/80/03/6ea8b1b2a5ab40a7a60dc464d3daa7aa546e0a74d74a9f8ff551ea7905db/executing-2.0.1-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/53/9d/40d5207db523363d9b5698f33778c18b0d591e3fdb6e0116b894b2a2491c/ipykernel-6.29.4-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/8a/15/ea245239487bbd8d7203fe010ea48c7539e42bf1fde0592313241a3fba3a/ipython-8.23.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/20/9f/bc63f0f0737ad7a60800bfd472a4836661adae21f9c2535f3957b1e54ceb/jedi-0.19.1-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/39/9d/b035d024c62c85f2e2d4806a59ca7b8520307f34e0932fbc8cc75fe7b2d9/jsonschema-4.21.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/ee/07/44bd408781594c4d0a027666ef27fab1e441b109dc3b76b4f836f8fd04fe/jsonschema_specifications-2023.12.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/75/6d/d7b55b9c1ac802ab066b3e5015e90faab1fffbbd67a2af498ffc6cc81c97/jupyter_client-8.6.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/c9/fb/108ecd1fe961941959ad0ee4e12ee7b8b1477247f30b1fdfd83ceaf017f0/jupyter_core-5.7.2-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/72/42/d57a938cad4e99bb799f35105561959b0a0550c65fbc1ed671196e27f909/jupyter_kernel_test-0.7.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/8f/8e/9ad090d3553c280a8060fbf6e24dc1c0c29704ee7d1c372f0c174aa59285/matplotlib_inline-0.1.7-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/0e/f2/f864ed36a8a62c26b57c3e08d212bd8f3d12a3ca3ef64600be5452aa3c82/msgspec-0.18.6-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
+      - pypi: https://files.pythonhosted.org/packages/a0/c4/c2971a3ba4c6103a3d10c4b0f24f461ddc027f0f09763220cf35ca1401b3/nest_asyncio-1.6.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/49/df/1fceb2f8900f8639e278b056416d49134fb8d84c5942ffaa01ad34782422/packaging-24.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/c6/ac/dac4a63f978e4dcb3c6d3a78c4d8e0192a113d288502a1216950c41b1027/parso-0.8.4-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/9e/c3/059298687310d527a58bb01f3b1965787ee3b40dce76752eda8b44e9a2c5/pexpect-4.9.0-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/55/72/4898c44ee9ea6f43396fbc23d9bfaf3d06e01b83698bdf2e4c919deceb7c/platformdirs-4.2.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/ee/fd/ca7bf3869e7caa7a037e23078539467b433a4e01eebd93f77180ab927766/prompt_toolkit-3.0.43-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/90/c7/6dc0a455d111f68ee43f27793971cf03fe29b6ef972042549db29eec39a2/psutil-5.9.8.tar.gz
+      - pypi: https://files.pythonhosted.org/packages/22/a6/858897256d0deac81a172289110f31629fc4cee19b6f01283303e18c8db3/ptyprocess-0.7.0-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/2b/27/77f9d5684e6bce929f5cfe18d6cfbe5133013c06cb2fbf5933670e60761d/pure_eval-0.2.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/97/9c/372fef8377a6e340b1704768d20daaded98bf13282b5327beb2e2fe2c7ef/pygments-2.17.2-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/ec/57/56b9bcc3c9c6a792fcbaf139543cee77261f3651ca9da0c93f5c1221264b/python_dateutil-2.9.0.post0-py2.py3-none-any.whl
-      - pypi: https://files.pythonhosted.org/packages/72/55/cc3163e20f40615a49245fa7041badec6103e8ee7e482dbb0feea00a7b84/pyzmq-25.1.2-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
+      - pypi: https://files.pythonhosted.org/packages/bf/4a/c6729cc692e2db85cc882bcf03a32536d9ff6a0e852f240156e71daade21/pyzmq-26.0.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
       - pypi: https://files.pythonhosted.org/packages/42/8e/ae1de7b12223986e949bdb886c004de7c304b6fa94de5b87c926c1099656/referencing-0.34.0-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/5a/57/2fcfd462cc53876ac4acef69dbf4fb941da971440049ca72051da54ea60d/rpds_py-0.18.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
       - pypi: https://files.pythonhosted.org/packages/d9/5a/e7c31adbe875f2abbb91bd84cf2dc52d792b5a01506781dbcf25c91daf11/six-1.16.0-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/f1/7b/ce1eafaf1a76852e2ec9b22edecf1daa58175c090266e9f6c64afcd81d91/stack_data-0.6.3-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/62/e5/3ee2ba523a13bae5c17d1658580d13597116c1639374ca5033d58fd04724/tornado-6.4-cp38-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
       - pypi: https://files.pythonhosted.org/packages/7c/c4/366a09036c07f46eb8c9b2af39c97f502ef24f11f2a6e4d763655d9f2708/traitlets-5.14.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/fd/84/fd2ba7aafacbad3c4201d395674fc6348826569da3c0937e75505ead3528/wcwidth-0.2.13-py2.py3-none-any.whl
       - pypi: ../../../../pixi-kernel
       osx-64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/_r-mutex-1.0.1-anacondar_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/bwidget-1.9.14-h694c41f_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/c-ares-1.28.1-h10d778d_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda
@@ -346,28 +386,28 @@
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libnghttp2-1.58.0-h64cf6d3_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libopenblas-0.3.27-openmp_hfef2a42_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libpng-1.6.43-h92b6c6a_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libsodium-1.0.18-hbcb3906_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.2-h92b6c6a_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libssh2-1.11.0-hd019ec5_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libtiff-4.6.0-h129831d_3.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.3.2-h10d778d_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.12.6-hc0ae0f7_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.4.0-h10d778d_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.12.6-hc0ae0f7_2.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/llvm-openmp-18.1.3-hb6ac08f_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/llvm-tools-18.1.3-hbcf5fad_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/make-4.3-h22f3db7_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/mpc-1.3.1-h81bd1dd_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/mpfr-4.2.1-h4f6b447_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4.20240210-h73e2aa4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.2.1-hd75f5a5_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/pango-1.52.1-h7f2093b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/pcre2-10.42-h0ad2156_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/pixman-0.43.4-h73e2aa4_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.2-h9f0c242_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/r-base-4.3.3-hbe75827_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/r-base64enc-0.1_3-r43h6dc245f_1006.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/r-cli-3.6.2-r43h64b2c41_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/r-crayon-1.5.2-r43hc72bb7e_2.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/r-digest-0.6.35-r43h29979af_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/r-ellipsis-0.3.2-r43h6dc245f_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/r-evaluate-0.23-r43hc72bb7e_0.conda
@@ -392,29 +432,50 @@
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tktable-2.10-ha166976_5.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.5-h93d8f39_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.13-h8a1eda9_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.5-h829000d_0.conda
+      - pypi: https://files.pythonhosted.org/packages/81/29/5ecc3a15d5a33e31b26c11426c45c501e439cb865d0bff96315d86443b78/appnope-0.1.4-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/45/86/4736ac618d82a20d87d2f92ae19441ebc7ac9e7a581d7e58bbe79233b24a/asttokens-2.4.1-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/e0/44/827b2a91a5816512fcaf3cc4ebc465ccd5d598c45cefa6703fcf4a79018f/attrs-23.2.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/e6/75/49e5bfe642f71f272236b5b2d2691cf915a7283cc0ceda56357b61daa538/comm-0.2.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/57/ab/6df7e24db51e1db642a5ea1759d44fb656251253995a27deb37af9b192ae/debugpy-1.8.1-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/d5/50/83c593b07763e1161326b3b8c6686f0f4b0f24d5526546bee538c89837d6/decorator-5.1.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/80/03/6ea8b1b2a5ab40a7a60dc464d3daa7aa546e0a74d74a9f8ff551ea7905db/executing-2.0.1-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/53/9d/40d5207db523363d9b5698f33778c18b0d591e3fdb6e0116b894b2a2491c/ipykernel-6.29.4-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/8a/15/ea245239487bbd8d7203fe010ea48c7539e42bf1fde0592313241a3fba3a/ipython-8.23.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/20/9f/bc63f0f0737ad7a60800bfd472a4836661adae21f9c2535f3957b1e54ceb/jedi-0.19.1-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/39/9d/b035d024c62c85f2e2d4806a59ca7b8520307f34e0932fbc8cc75fe7b2d9/jsonschema-4.21.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/ee/07/44bd408781594c4d0a027666ef27fab1e441b109dc3b76b4f836f8fd04fe/jsonschema_specifications-2023.12.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/75/6d/d7b55b9c1ac802ab066b3e5015e90faab1fffbbd67a2af498ffc6cc81c97/jupyter_client-8.6.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/c9/fb/108ecd1fe961941959ad0ee4e12ee7b8b1477247f30b1fdfd83ceaf017f0/jupyter_core-5.7.2-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/72/42/d57a938cad4e99bb799f35105561959b0a0550c65fbc1ed671196e27f909/jupyter_kernel_test-0.7.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/8f/8e/9ad090d3553c280a8060fbf6e24dc1c0c29704ee7d1c372f0c174aa59285/matplotlib_inline-0.1.7-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/1d/b5/c8fbf1db814eb29eda402952374b594b2559419ba7ec6d0997a9e5687530/msgspec-0.18.6-cp312-cp312-macosx_10_9_x86_64.whl
+      - pypi: https://files.pythonhosted.org/packages/a0/c4/c2971a3ba4c6103a3d10c4b0f24f461ddc027f0f09763220cf35ca1401b3/nest_asyncio-1.6.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/49/df/1fceb2f8900f8639e278b056416d49134fb8d84c5942ffaa01ad34782422/packaging-24.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/c6/ac/dac4a63f978e4dcb3c6d3a78c4d8e0192a113d288502a1216950c41b1027/parso-0.8.4-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/9e/c3/059298687310d527a58bb01f3b1965787ee3b40dce76752eda8b44e9a2c5/pexpect-4.9.0-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/55/72/4898c44ee9ea6f43396fbc23d9bfaf3d06e01b83698bdf2e4c919deceb7c/platformdirs-4.2.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/ee/fd/ca7bf3869e7caa7a037e23078539467b433a4e01eebd93f77180ab927766/prompt_toolkit-3.0.43-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/e7/e3/07ae864a636d70a8a6f58da27cb1179192f1140d5d1da10886ade9405797/psutil-5.9.8-cp36-abi3-macosx_10_9_x86_64.whl
+      - pypi: https://files.pythonhosted.org/packages/22/a6/858897256d0deac81a172289110f31629fc4cee19b6f01283303e18c8db3/ptyprocess-0.7.0-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/2b/27/77f9d5684e6bce929f5cfe18d6cfbe5133013c06cb2fbf5933670e60761d/pure_eval-0.2.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/97/9c/372fef8377a6e340b1704768d20daaded98bf13282b5327beb2e2fe2c7ef/pygments-2.17.2-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/ec/57/56b9bcc3c9c6a792fcbaf139543cee77261f3651ca9da0c93f5c1221264b/python_dateutil-2.9.0.post0-py2.py3-none-any.whl
-      - pypi: https://files.pythonhosted.org/packages/6e/f0/d71cf69dc039c9adc8b625efc3bad3684f3660a570e47f0f0c64df787b41/pyzmq-25.1.2-cp312-cp312-macosx_10_15_universal2.whl
+      - pypi: https://files.pythonhosted.org/packages/f6/2c/7074b0747be7a23c9d2b15d603fbc1a55aa305665a2c0798d27c3baafa9e/pyzmq-26.0.0-cp312-cp312-macosx_10_15_universal2.whl
       - pypi: https://files.pythonhosted.org/packages/42/8e/ae1de7b12223986e949bdb886c004de7c304b6fa94de5b87c926c1099656/referencing-0.34.0-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/09/b6/45690f5d3f8c551bb462e063a2f336d72c8884ed26aa19beb53a374d3854/rpds_py-0.18.0-cp312-cp312-macosx_10_12_x86_64.whl
       - pypi: https://files.pythonhosted.org/packages/d9/5a/e7c31adbe875f2abbb91bd84cf2dc52d792b5a01506781dbcf25c91daf11/six-1.16.0-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/f1/7b/ce1eafaf1a76852e2ec9b22edecf1daa58175c090266e9f6c64afcd81d91/stack_data-0.6.3-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/34/7a/e7ec972db24513ea69ac7132c1a5eef62309dc978566a4afffa314417a45/tornado-6.4-cp38-abi3-macosx_10_9_x86_64.whl
       - pypi: https://files.pythonhosted.org/packages/7c/c4/366a09036c07f46eb8c9b2af39c97f502ef24f11f2a6e4d763655d9f2708/traitlets-5.14.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/fd/84/fd2ba7aafacbad3c4201d395674fc6348826569da3c0937e75505ead3528/wcwidth-0.2.13-py2.py3-none-any.whl
       - pypi: ../../../../pixi-kernel
       osx-arm64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/_r-mutex-1.0.1-anacondar_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/bwidget-1.9.14-hce30654_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/c-ares-1.28.1-h93a5062_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ca-certificates-2024.2.2-hf0a4a13_0.conda
@@ -478,28 +539,28 @@
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libnghttp2-1.58.0-ha4dd798_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libopenblas-0.3.27-openmp_h6c19121_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libpng-1.6.43-h091b4b1_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libsodium-1.0.18-h27ca646_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libsqlite-3.45.2-h091b4b1_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libssh2-1.11.0-h7a5bd25_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libtiff-4.6.0-h07db509_3.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libwebp-base-1.3.2-h93a5062_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libxml2-2.12.6-h0d0cfa8_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libwebp-base-1.4.0-h93a5062_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libxml2-2.12.6-h0d0cfa8_2.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libzlib-1.2.13-h53f4e23_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/llvm-openmp-18.1.3-hcd81f8e_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/llvm-tools-18.1.3-h30cc82d_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/make-4.3-he57ea6c_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/mpc-1.3.1-h91ba8db_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/mpfr-4.2.1-h41d338b_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ncurses-6.4.20240210-h078ce10_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.2.1-h0d3ecfb_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pango-1.52.1-hb067d4f_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pcre2-10.42-h26f9a81_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pixman-0.43.4-hebf3989_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.2-hdf0ec26_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.3-h4a7b5fc_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/r-base-4.3.3-h53b85ff_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/r-base64enc-0.1_3-r43h21dc0da_1006.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/r-cli-3.6.2-r43he96f11e_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/r-crayon-1.5.2-r43hc72bb7e_2.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/r-digest-0.6.35-r43h65f505e_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/r-ellipsis-0.3.2-r43h21dc0da_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/r-evaluate-0.23-r43hc72bb7e_0.conda
@@ -524,41 +585,62 @@
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tktable-2.10-hd996620_5.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zeromq-4.3.5-hebf3989_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zlib-1.2.13-h53f4e23_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zstd-1.5.5-h4f39d0f_0.conda
+      - pypi: https://files.pythonhosted.org/packages/81/29/5ecc3a15d5a33e31b26c11426c45c501e439cb865d0bff96315d86443b78/appnope-0.1.4-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/45/86/4736ac618d82a20d87d2f92ae19441ebc7ac9e7a581d7e58bbe79233b24a/asttokens-2.4.1-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/e0/44/827b2a91a5816512fcaf3cc4ebc465ccd5d598c45cefa6703fcf4a79018f/attrs-23.2.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/e6/75/49e5bfe642f71f272236b5b2d2691cf915a7283cc0ceda56357b61daa538/comm-0.2.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/84/3e/5ab87207d811b1659763d8a1c762f7cae13b3f30674565fe8f3f47a41a6a/debugpy-1.8.1-cp312-cp312-macosx_11_0_universal2.whl
+      - pypi: https://files.pythonhosted.org/packages/d5/50/83c593b07763e1161326b3b8c6686f0f4b0f24d5526546bee538c89837d6/decorator-5.1.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/80/03/6ea8b1b2a5ab40a7a60dc464d3daa7aa546e0a74d74a9f8ff551ea7905db/executing-2.0.1-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/53/9d/40d5207db523363d9b5698f33778c18b0d591e3fdb6e0116b894b2a2491c/ipykernel-6.29.4-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/8a/15/ea245239487bbd8d7203fe010ea48c7539e42bf1fde0592313241a3fba3a/ipython-8.23.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/20/9f/bc63f0f0737ad7a60800bfd472a4836661adae21f9c2535f3957b1e54ceb/jedi-0.19.1-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/39/9d/b035d024c62c85f2e2d4806a59ca7b8520307f34e0932fbc8cc75fe7b2d9/jsonschema-4.21.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/ee/07/44bd408781594c4d0a027666ef27fab1e441b109dc3b76b4f836f8fd04fe/jsonschema_specifications-2023.12.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/75/6d/d7b55b9c1ac802ab066b3e5015e90faab1fffbbd67a2af498ffc6cc81c97/jupyter_client-8.6.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/c9/fb/108ecd1fe961941959ad0ee4e12ee7b8b1477247f30b1fdfd83ceaf017f0/jupyter_core-5.7.2-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/72/42/d57a938cad4e99bb799f35105561959b0a0550c65fbc1ed671196e27f909/jupyter_kernel_test-0.7.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/8f/8e/9ad090d3553c280a8060fbf6e24dc1c0c29704ee7d1c372f0c174aa59285/matplotlib_inline-0.1.7-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/d7/9a/235d2dbab078a0b8e6f338205dc59be0b027ce000554ee6a9c41b19339e5/msgspec-0.18.6-cp312-cp312-macosx_11_0_arm64.whl
+      - pypi: https://files.pythonhosted.org/packages/a0/c4/c2971a3ba4c6103a3d10c4b0f24f461ddc027f0f09763220cf35ca1401b3/nest_asyncio-1.6.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/49/df/1fceb2f8900f8639e278b056416d49134fb8d84c5942ffaa01ad34782422/packaging-24.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/c6/ac/dac4a63f978e4dcb3c6d3a78c4d8e0192a113d288502a1216950c41b1027/parso-0.8.4-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/9e/c3/059298687310d527a58bb01f3b1965787ee3b40dce76752eda8b44e9a2c5/pexpect-4.9.0-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/55/72/4898c44ee9ea6f43396fbc23d9bfaf3d06e01b83698bdf2e4c919deceb7c/platformdirs-4.2.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/ee/fd/ca7bf3869e7caa7a037e23078539467b433a4e01eebd93f77180ab927766/prompt_toolkit-3.0.43-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/05/33/2d74d588408caedd065c2497bdb5ef83ce6082db01289a1e1147f6639802/psutil-5.9.8-cp38-abi3-macosx_11_0_arm64.whl
+      - pypi: https://files.pythonhosted.org/packages/22/a6/858897256d0deac81a172289110f31629fc4cee19b6f01283303e18c8db3/ptyprocess-0.7.0-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/2b/27/77f9d5684e6bce929f5cfe18d6cfbe5133013c06cb2fbf5933670e60761d/pure_eval-0.2.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/97/9c/372fef8377a6e340b1704768d20daaded98bf13282b5327beb2e2fe2c7ef/pygments-2.17.2-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/ec/57/56b9bcc3c9c6a792fcbaf139543cee77261f3651ca9da0c93f5c1221264b/python_dateutil-2.9.0.post0-py2.py3-none-any.whl
-      - pypi: https://files.pythonhosted.org/packages/6e/f0/d71cf69dc039c9adc8b625efc3bad3684f3660a570e47f0f0c64df787b41/pyzmq-25.1.2-cp312-cp312-macosx_10_15_universal2.whl
+      - pypi: https://files.pythonhosted.org/packages/f6/2c/7074b0747be7a23c9d2b15d603fbc1a55aa305665a2c0798d27c3baafa9e/pyzmq-26.0.0-cp312-cp312-macosx_10_15_universal2.whl
       - pypi: https://files.pythonhosted.org/packages/42/8e/ae1de7b12223986e949bdb886c004de7c304b6fa94de5b87c926c1099656/referencing-0.34.0-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/7a/58/9bfc53b266df92f0515e72fd16e4890dc6b56fc3bfc216b3a2a729c866b5/rpds_py-0.18.0-cp312-cp312-macosx_11_0_arm64.whl
       - pypi: https://files.pythonhosted.org/packages/d9/5a/e7c31adbe875f2abbb91bd84cf2dc52d792b5a01506781dbcf25c91daf11/six-1.16.0-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/f1/7b/ce1eafaf1a76852e2ec9b22edecf1daa58175c090266e9f6c64afcd81d91/stack_data-0.6.3-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/4a/2e/3ba930e3af171847d610e07ae878e04fcb7e4d7822f1a2d29a27b128ea24/tornado-6.4-cp38-abi3-macosx_10_9_universal2.whl
       - pypi: https://files.pythonhosted.org/packages/7c/c4/366a09036c07f46eb8c9b2af39c97f502ef24f11f2a6e4d763655d9f2708/traitlets-5.14.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/fd/84/fd2ba7aafacbad3c4201d395674fc6348826569da3c0937e75505ead3528/wcwidth-0.2.13-py2.py3-none-any.whl
       - pypi: ../../../../pixi-kernel
       win-64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/_r-mutex-1.0.1-anacondar_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2024.1.0-h57928b3_965.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libblas-3.9.0-22_win64_mkl.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libhwloc-2.10.0-default_h2fffb23_1000.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libiconv-1.17-hcfcfb64_2.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/liblapack-3.9.0-22_win64_mkl.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libsodium-1.0.18-h8d14728_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.2-hcfcfb64_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/libxml2-2.12.6-h8a06e1b_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/libxml2-2.12.6-h8a06e1b_2.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libzlib-1.3.1-hcfcfb64_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/m2w64-bwidget-1.9.10-2.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/m2w64-bzip2-1.0.6-6.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/m2w64-expat-2.1.1-2.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/m2w64-fftw-3.3.4-6.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/m2w64-flac-1.3.1-3.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libgfortran-5.3.0-6.tar.bz2
@@ -617,31 +699,52 @@
       - conda: https://conda.anaconda.org/conda-forge/win-64/tbb-2021.12.0-h91493d7_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hcf57466_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33130-h82b7239_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33130-hcb4865c_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/zeromq-4.3.5-h63175ca_1.conda
+      - pypi: https://files.pythonhosted.org/packages/45/86/4736ac618d82a20d87d2f92ae19441ebc7ac9e7a581d7e58bbe79233b24a/asttokens-2.4.1-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/e0/44/827b2a91a5816512fcaf3cc4ebc465ccd5d598c45cefa6703fcf4a79018f/attrs-23.2.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/d1/d6/3965ed04c63042e047cb6a3e6ed1a63a35087b6a609aa3a15ed8ac56c221/colorama-0.4.6-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/e6/75/49e5bfe642f71f272236b5b2d2691cf915a7283cc0ceda56357b61daa538/comm-0.2.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/dc/33/22e2b1c4adab01e08381032fe2b3c7453f460bcf92882f31bddf7b908f1e/debugpy-1.8.1-cp39-cp39-win_amd64.whl
+      - pypi: https://files.pythonhosted.org/packages/d5/50/83c593b07763e1161326b3b8c6686f0f4b0f24d5526546bee538c89837d6/decorator-5.1.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/b8/9a/5028fd52db10e600f1c4674441b968cf2ea4959085bfb5b99fb1250e5f68/exceptiongroup-1.2.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/80/03/6ea8b1b2a5ab40a7a60dc464d3daa7aa546e0a74d74a9f8ff551ea7905db/executing-2.0.1-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/2d/0a/679461c511447ffaf176567d5c496d1de27cbe34a87df6677d7171b2fbd4/importlib_metadata-7.1.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/53/9d/40d5207db523363d9b5698f33778c18b0d591e3fdb6e0116b894b2a2491c/ipykernel-6.29.4-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/47/6b/d9fdcdef2eb6a23f391251fde8781c38d42acd82abe84d054cb74f7863b0/ipython-8.18.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/20/9f/bc63f0f0737ad7a60800bfd472a4836661adae21f9c2535f3957b1e54ceb/jedi-0.19.1-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/39/9d/b035d024c62c85f2e2d4806a59ca7b8520307f34e0932fbc8cc75fe7b2d9/jsonschema-4.21.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/ee/07/44bd408781594c4d0a027666ef27fab1e441b109dc3b76b4f836f8fd04fe/jsonschema_specifications-2023.12.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/75/6d/d7b55b9c1ac802ab066b3e5015e90faab1fffbbd67a2af498ffc6cc81c97/jupyter_client-8.6.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/c9/fb/108ecd1fe961941959ad0ee4e12ee7b8b1477247f30b1fdfd83ceaf017f0/jupyter_core-5.7.2-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/72/42/d57a938cad4e99bb799f35105561959b0a0550c65fbc1ed671196e27f909/jupyter_kernel_test-0.7.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/8f/8e/9ad090d3553c280a8060fbf6e24dc1c0c29704ee7d1c372f0c174aa59285/matplotlib_inline-0.1.7-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/cd/b2/283d010db6836db2fe059f7ee3c13823927229975ffbe1edcbeded85a556/msgspec-0.18.6-cp39-cp39-win_amd64.whl
+      - pypi: https://files.pythonhosted.org/packages/a0/c4/c2971a3ba4c6103a3d10c4b0f24f461ddc027f0f09763220cf35ca1401b3/nest_asyncio-1.6.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/49/df/1fceb2f8900f8639e278b056416d49134fb8d84c5942ffaa01ad34782422/packaging-24.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/c6/ac/dac4a63f978e4dcb3c6d3a78c4d8e0192a113d288502a1216950c41b1027/parso-0.8.4-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/55/72/4898c44ee9ea6f43396fbc23d9bfaf3d06e01b83698bdf2e4c919deceb7c/platformdirs-4.2.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/ee/fd/ca7bf3869e7caa7a037e23078539467b433a4e01eebd93f77180ab927766/prompt_toolkit-3.0.43-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/93/52/3e39d26feae7df0aa0fd510b14012c3678b36ed068f7d78b8d8784d61f0e/psutil-5.9.8-cp37-abi3-win_amd64.whl
+      - pypi: https://files.pythonhosted.org/packages/2b/27/77f9d5684e6bce929f5cfe18d6cfbe5133013c06cb2fbf5933670e60761d/pure_eval-0.2.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/97/9c/372fef8377a6e340b1704768d20daaded98bf13282b5327beb2e2fe2c7ef/pygments-2.17.2-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/ec/57/56b9bcc3c9c6a792fcbaf139543cee77261f3651ca9da0c93f5c1221264b/python_dateutil-2.9.0.post0-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/1c/f7/24d8ed4fd9c43b90354df7764f81f0dd5e623f9a50f1538f90fe085d6dff/pywin32-306-cp39-cp39-win_amd64.whl
-      - pypi: https://files.pythonhosted.org/packages/11/ae/d573f1c3854fff3714fe3cbf8ed3ce4200cc2aa81ab159dfe74b660d6523/pyzmq-25.1.2-cp39-cp39-win_amd64.whl
+      - pypi: https://files.pythonhosted.org/packages/41/fb/ddb8ed65b3be53eb2fdaacd57ef33d6019daf12a6155fa96181c1d264c13/pyzmq-26.0.0-cp39-cp39-win_amd64.whl
       - pypi: https://files.pythonhosted.org/packages/42/8e/ae1de7b12223986e949bdb886c004de7c304b6fa94de5b87c926c1099656/referencing-0.34.0-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/a0/62/c896cec9434e09fb933f3cadd5c699e9cea49ab8934d694b6634650748db/rpds_py-0.18.0-cp39-none-win_amd64.whl
       - pypi: https://files.pythonhosted.org/packages/d9/5a/e7c31adbe875f2abbb91bd84cf2dc52d792b5a01506781dbcf25c91daf11/six-1.16.0-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/f1/7b/ce1eafaf1a76852e2ec9b22edecf1daa58175c090266e9f6c64afcd81d91/stack_data-0.6.3-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/af/2b/4649926f17c1634d21c584cc855b5c5021f148b934919d26932a595bc034/tornado-6.4-cp38-abi3-win_amd64.whl
       - pypi: https://files.pythonhosted.org/packages/7c/c4/366a09036c07f46eb8c9b2af39c97f502ef24f11f2a6e4d763655d9f2708/traitlets-5.14.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/01/f3/936e209267d6ef7510322191003885de524fc48d1b43269810cd589ceaf5/typing_extensions-4.11.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/fd/84/fd2ba7aafacbad3c4201d395674fc6348826569da3c0937e75505ead3528/wcwidth-0.2.13-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/c2/0a/ba9d0ee9536d3ef73a3448e931776e658b36f128d344e175bc32b092a8bf/zipp-3.18.1-py3-none-any.whl
       - pypi: ../../../../pixi-kernel
 packages:
 - kind: conda
   name: _libgcc_mutex
   version: '0.1'
   build: conda_forge
@@ -711,14 +814,33 @@
   sha256: edac93a8e3beb9383abf508f66085505950bc89962116ef149558350a6213749
   md5: 18f0bdf689b6f345fecddbebaed945d6
   license: LGPL-2.0-or-later AND LGPL-2.0-or-later WITH exceptions AND GPL-2.0-or-later AND MPL-2.0
   license_family: GPL
   size: 21238
   timestamp: 1708000885951
 - kind: pypi
+  name: appnope
+  version: 0.1.4
+  url: https://files.pythonhosted.org/packages/81/29/5ecc3a15d5a33e31b26c11426c45c501e439cb865d0bff96315d86443b78/appnope-0.1.4-py2.py3-none-any.whl
+  sha256: 502575ee11cd7a28c0205f379b525beefebab9d161b7c964670864014ed7213c
+  requires_python: '>=3.6'
+- kind: pypi
+  name: asttokens
+  version: 2.4.1
+  url: https://files.pythonhosted.org/packages/45/86/4736ac618d82a20d87d2f92ae19441ebc7ac9e7a581d7e58bbe79233b24a/asttokens-2.4.1-py2.py3-none-any.whl
+  sha256: 051ed49c3dcae8913ea7cd08e46a606dba30b79993209636c4875bc1d637bc24
+  requires_dist:
+  - six >=1.12.0
+  - typing ; python_version < '3.5'
+  - astroid <2, >=1 ; python_version < '3' and extra == 'astroid'
+  - astroid <4, >=2 ; python_version >= '3' and extra == 'astroid'
+  - pytest ; extra == 'test'
+  - astroid <2, >=1 ; python_version < '3' and extra == 'test'
+  - astroid <4, >=2 ; python_version >= '3' and extra == 'test'
+- kind: pypi
   name: attrs
   version: 23.2.0
   url: https://files.pythonhosted.org/packages/e0/44/827b2a91a5816512fcaf3cc4ebc465ccd5d598c45cefa6703fcf4a79018f/attrs-23.2.0-py3-none-any.whl
   sha256: 99b87a485a5820b23b879f04c2305b44b951b502fd64be915879d77a7e8fc6f1
   requires_dist:
   - importlib-metadata ; python_version < '3.8'
   - attrs[tests] ; extra == 'cov'
@@ -1384,14 +1506,29 @@
   depends:
   - clang_osx-arm64 18.1.3 h54d7cd3_11
   - clangxx_impl_osx-arm64 18.1.3 h1ba0cb9_11
   license: BSD-3-Clause
   license_family: BSD
   size: 19244
   timestamp: 1712621431069
+- kind: pypi
+  name: colorama
+  version: 0.4.6
+  url: https://files.pythonhosted.org/packages/d1/d6/3965ed04c63042e047cb6a3e6ed1a63a35087b6a609aa3a15ed8ac56c221/colorama-0.4.6-py2.py3-none-any.whl
+  sha256: 4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
+  requires_python: '!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,!=3.6.*,>=2.7'
+- kind: pypi
+  name: comm
+  version: 0.2.2
+  url: https://files.pythonhosted.org/packages/e6/75/49e5bfe642f71f272236b5b2d2691cf915a7283cc0ceda56357b61daa538/comm-0.2.2-py3-none-any.whl
+  sha256: e6fb86cb70ff661ee8c9c14e7d36d6de3b4066f1441be4063df9c5009f0a64d3
+  requires_dist:
+  - traitlets >=4
+  - pytest ; extra == 'test'
+  requires_python: '>=3.8'
 - kind: conda
   name: compiler-rt
   version: 18.1.3
   build: h3808999_0
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/compiler-rt-18.1.3-h3808999_0.conda
   sha256: dfada604649fb2cfa6fb3dbd657fccf81cd01e00a7f6f29da24fc40e36cd51fa
@@ -1530,14 +1667,66 @@
   - libzlib >=1.2.13,<1.3.0a0
   - openssl >=3.2.1,<4.0a0
   - zstd >=1.5.5,<1.6.0a0
   license: curl
   license_family: MIT
   size: 164864
   timestamp: 1711548139831
+- kind: pypi
+  name: debugpy
+  version: 1.8.1
+  url: https://files.pythonhosted.org/packages/57/ab/6df7e24db51e1db642a5ea1759d44fb656251253995a27deb37af9b192ae/debugpy-1.8.1-py2.py3-none-any.whl
+  sha256: 28acbe2241222b87e255260c76741e1fbf04fdc3b6d094fcf57b6c6f75ce1242
+  requires_python: '>=3.8'
+- kind: pypi
+  name: debugpy
+  version: 1.8.1
+  url: https://files.pythonhosted.org/packages/dc/33/22e2b1c4adab01e08381032fe2b3c7453f460bcf92882f31bddf7b908f1e/debugpy-1.8.1-cp39-cp39-win_amd64.whl
+  sha256: 6df9aa9599eb05ca179fb0b810282255202a66835c6efb1d112d21ecb830ddd3
+  requires_python: '>=3.8'
+- kind: pypi
+  name: debugpy
+  version: 1.8.1
+  url: https://files.pythonhosted.org/packages/3c/7a/e400d9f5ed6b4b5ec9f350b4d7974e986ca2d455221e567e648edfad898e/debugpy-1.8.1-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: a2e658a9630f27534e63922ebf655a6ab60c370f4d2fc5c02a5b19baf4410ace
+  requires_python: '>=3.8'
+- kind: pypi
+  name: debugpy
+  version: 1.8.1
+  url: https://files.pythonhosted.org/packages/84/3e/5ab87207d811b1659763d8a1c762f7cae13b3f30674565fe8f3f47a41a6a/debugpy-1.8.1-cp312-cp312-macosx_11_0_universal2.whl
+  sha256: 3ebb70ba1a6524d19fa7bb122f44b74170c447d5746a503e36adc244a20ac539
+  requires_python: '>=3.8'
+- kind: pypi
+  name: decorator
+  version: 5.1.1
+  url: https://files.pythonhosted.org/packages/d5/50/83c593b07763e1161326b3b8c6686f0f4b0f24d5526546bee538c89837d6/decorator-5.1.1-py3-none-any.whl
+  sha256: b8c3f85900b9dc423225913c5aace94729fe1fa9763b38939a95226f02d37186
+  requires_python: '>=3.5'
+- kind: pypi
+  name: exceptiongroup
+  version: 1.2.0
+  url: https://files.pythonhosted.org/packages/b8/9a/5028fd52db10e600f1c4674441b968cf2ea4959085bfb5b99fb1250e5f68/exceptiongroup-1.2.0-py3-none-any.whl
+  sha256: 4bfd3996ac73b41e9b9628b04e079f193850720ea5945fc96a08633c66912f14
+  requires_dist:
+  - pytest >=6 ; extra == 'test'
+  requires_python: '>=3.7'
+- kind: pypi
+  name: executing
+  version: 2.0.1
+  url: https://files.pythonhosted.org/packages/80/03/6ea8b1b2a5ab40a7a60dc464d3daa7aa546e0a74d74a9f8ff551ea7905db/executing-2.0.1-py2.py3-none-any.whl
+  sha256: eac49ca94516ccc753f9fb5ce82603156e590b27525a8bc32cce8ae302eb61bc
+  requires_dist:
+  - asttokens >=2.1.0 ; extra == 'tests'
+  - ipython ; extra == 'tests'
+  - pytest ; extra == 'tests'
+  - coverage ; extra == 'tests'
+  - coverage-enable-subprocess ; extra == 'tests'
+  - littleutils ; extra == 'tests'
+  - rich ; python_version >= '3.11' and extra == 'tests'
+  requires_python: '>=3.5'
 - kind: conda
   name: expat
   version: 2.6.2
   build: h2f0025b_0
   subdir: linux-aarch64
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/expat-2.6.2-h2f0025b_0.conda
   sha256: a7a998faf6b9ed71d8c5c67f996e7faa52a7b9b02ed2d2f2ab6cfa1db8e5aca4
@@ -2471,14 +2660,186 @@
   url: https://conda.anaconda.org/conda-forge/win-64/intel-openmp-2024.1.0-h57928b3_965.conda
   sha256: 7b029e476ad6d401d645636ee3e4b40130bfcc9534f7415209dd5b666c6dd292
   md5: c66eb2fd33b999ccc258aef85689758e
   license: LicenseRef-ProprietaryIntel
   license_family: Proprietary
   size: 1617555
   timestamp: 1712943333029
+- kind: pypi
+  name: ipykernel
+  version: 6.29.4
+  url: https://files.pythonhosted.org/packages/53/9d/40d5207db523363d9b5698f33778c18b0d591e3fdb6e0116b894b2a2491c/ipykernel-6.29.4-py3-none-any.whl
+  sha256: 1181e653d95c6808039c509ef8e67c4126b3b3af7781496c7cbfb5ed938a27da
+  requires_dist:
+  - appnope ; platform_system == 'Darwin'
+  - comm >=0.1.1
+  - debugpy >=1.6.5
+  - ipython >=7.23.1
+  - jupyter-client >=6.1.12
+  - jupyter-core !=5.0.*, >=4.12
+  - matplotlib-inline >=0.1
+  - nest-asyncio
+  - packaging
+  - psutil
+  - pyzmq >=24
+  - tornado >=6.1
+  - traitlets >=5.4.0
+  - coverage[toml] ; extra == 'cov'
+  - curio ; extra == 'cov'
+  - matplotlib ; extra == 'cov'
+  - pytest-cov ; extra == 'cov'
+  - trio ; extra == 'cov'
+  - myst-parser ; extra == 'docs'
+  - pydata-sphinx-theme ; extra == 'docs'
+  - sphinx ; extra == 'docs'
+  - sphinx-autodoc-typehints ; extra == 'docs'
+  - sphinxcontrib-github-alt ; extra == 'docs'
+  - sphinxcontrib-spelling ; extra == 'docs'
+  - trio ; extra == 'docs'
+  - pyqt5 ; extra == 'pyqt5'
+  - pyside6 ; extra == 'pyside6'
+  - flaky ; extra == 'test'
+  - ipyparallel ; extra == 'test'
+  - pre-commit ; extra == 'test'
+  - pytest-asyncio >=0.23.5 ; extra == 'test'
+  - pytest-cov ; extra == 'test'
+  - pytest-timeout ; extra == 'test'
+  - pytest >=7.0 ; extra == 'test'
+  requires_python: '>=3.8'
+- kind: pypi
+  name: ipython
+  version: 8.18.1
+  url: https://files.pythonhosted.org/packages/47/6b/d9fdcdef2eb6a23f391251fde8781c38d42acd82abe84d054cb74f7863b0/ipython-8.18.1-py3-none-any.whl
+  sha256: e8267419d72d81955ec1177f8a29aaa90ac80ad647499201119e2f05e99aa397
+  requires_dist:
+  - decorator
+  - jedi >=0.16
+  - matplotlib-inline
+  - prompt-toolkit <3.1.0, >=3.0.41
+  - pygments >=2.4.0
+  - stack-data
+  - traitlets >=5
+  - typing-extensions ; python_version < '3.10'
+  - exceptiongroup ; python_version < '3.11'
+  - pexpect >4.3 ; sys_platform != 'win32'
+  - colorama ; sys_platform == 'win32'
+  - black ; extra == 'all'
+  - ipykernel ; extra == 'all'
+  - setuptools >=18.5 ; extra == 'all'
+  - sphinx >=1.3 ; extra == 'all'
+  - sphinx-rtd-theme ; extra == 'all'
+  - docrepr ; extra == 'all'
+  - matplotlib ; extra == 'all'
+  - stack-data ; extra == 'all'
+  - pytest <7 ; extra == 'all'
+  - typing-extensions ; extra == 'all'
+  - exceptiongroup ; extra == 'all'
+  - pytest <7.1 ; extra == 'all'
+  - pytest-asyncio <0.22 ; extra == 'all'
+  - testpath ; extra == 'all'
+  - pickleshare ; extra == 'all'
+  - nbconvert ; extra == 'all'
+  - nbformat ; extra == 'all'
+  - ipywidgets ; extra == 'all'
+  - notebook ; extra == 'all'
+  - ipyparallel ; extra == 'all'
+  - qtconsole ; extra == 'all'
+  - curio ; extra == 'all'
+  - matplotlib !=3.2.0 ; extra == 'all'
+  - numpy >=1.22 ; extra == 'all'
+  - pandas ; extra == 'all'
+  - trio ; extra == 'all'
+  - black ; extra == 'black'
+  - ipykernel ; extra == 'doc'
+  - setuptools >=18.5 ; extra == 'doc'
+  - sphinx >=1.3 ; extra == 'doc'
+  - sphinx-rtd-theme ; extra == 'doc'
+  - docrepr ; extra == 'doc'
+  - matplotlib ; extra == 'doc'
+  - stack-data ; extra == 'doc'
+  - pytest <7 ; extra == 'doc'
+  - typing-extensions ; extra == 'doc'
+  - exceptiongroup ; extra == 'doc'
+  - pytest <7.1 ; extra == 'doc'
+  - pytest-asyncio <0.22 ; extra == 'doc'
+  - testpath ; extra == 'doc'
+  - pickleshare ; extra == 'doc'
+  - ipykernel ; extra == 'kernel'
+  - nbconvert ; extra == 'nbconvert'
+  - nbformat ; extra == 'nbformat'
+  - ipywidgets ; extra == 'notebook'
+  - notebook ; extra == 'notebook'
+  - ipyparallel ; extra == 'parallel'
+  - qtconsole ; extra == 'qtconsole'
+  - pytest <7.1 ; extra == 'test'
+  - pytest-asyncio <0.22 ; extra == 'test'
+  - testpath ; extra == 'test'
+  - pickleshare ; extra == 'test'
+  - pytest <7.1 ; extra == 'test_extra'
+  - pytest-asyncio <0.22 ; extra == 'test_extra'
+  - testpath ; extra == 'test_extra'
+  - pickleshare ; extra == 'test_extra'
+  - curio ; extra == 'test_extra'
+  - matplotlib !=3.2.0 ; extra == 'test_extra'
+  - nbformat ; extra == 'test_extra'
+  - numpy >=1.22 ; extra == 'test_extra'
+  - pandas ; extra == 'test_extra'
+  - trio ; extra == 'test_extra'
+  requires_python: '>=3.9'
+- kind: pypi
+  name: ipython
+  version: 8.23.0
+  url: https://files.pythonhosted.org/packages/8a/15/ea245239487bbd8d7203fe010ea48c7539e42bf1fde0592313241a3fba3a/ipython-8.23.0-py3-none-any.whl
+  sha256: 07232af52a5ba146dc3372c7bf52a0f890a23edf38d77caef8d53f9cdc2584c1
+  requires_dist:
+  - decorator
+  - jedi >=0.16
+  - matplotlib-inline
+  - prompt-toolkit <3.1.0, >=3.0.41
+  - pygments >=2.4.0
+  - stack-data
+  - traitlets >=5.13.0
+  - exceptiongroup ; python_version < '3.11'
+  - typing-extensions ; python_version < '3.12'
+  - pexpect >4.3 ; sys_platform != 'win32' and sys_platform != 'emscripten'
+  - colorama ; sys_platform == 'win32'
+  - ipython[black,doc,kernel,matplotlib,nbconvert,nbformat,notebook,parallel,qtconsole] ; extra == 'all'
+  - ipython[test,test-extra] ; extra == 'all'
+  - black ; extra == 'black'
+  - ipykernel ; extra == 'doc'
+  - setuptools >=18.5 ; extra == 'doc'
+  - sphinx >=1.3 ; extra == 'doc'
+  - sphinx-rtd-theme ; extra == 'doc'
+  - sphinxcontrib-jquery ; extra == 'doc'
+  - docrepr ; extra == 'doc'
+  - matplotlib ; extra == 'doc'
+  - stack-data ; extra == 'doc'
+  - typing-extensions ; extra == 'doc'
+  - exceptiongroup ; extra == 'doc'
+  - ipython[test] ; extra == 'doc'
+  - ipykernel ; extra == 'kernel'
+  - matplotlib ; extra == 'matplotlib'
+  - nbconvert ; extra == 'nbconvert'
+  - nbformat ; extra == 'nbformat'
+  - ipywidgets ; extra == 'notebook'
+  - notebook ; extra == 'notebook'
+  - ipyparallel ; extra == 'parallel'
+  - qtconsole ; extra == 'qtconsole'
+  - pytest <8 ; extra == 'test'
+  - pytest-asyncio <0.22 ; extra == 'test'
+  - testpath ; extra == 'test'
+  - pickleshare ; extra == 'test'
+  - ipython[test] ; extra == 'test_extra'
+  - curio ; extra == 'test_extra'
+  - matplotlib !=3.2.0 ; extra == 'test_extra'
+  - nbformat ; extra == 'test_extra'
+  - numpy >=1.23 ; extra == 'test_extra'
+  - pandas ; extra == 'test_extra'
+  - trio ; extra == 'test_extra'
+  requires_python: '>=3.10'
 - kind: conda
   name: isl
   version: '0.26'
   build: imath32_h2e86a7b_101
   build_number: 101
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/isl-0.26-imath32_h2e86a7b_101.conda
@@ -2506,14 +2867,55 @@
   track_features:
   - isl_imath-32
   license: MIT
   license_family: MIT
   size: 819937
   timestamp: 1680649567633
 - kind: pypi
+  name: jedi
+  version: 0.19.1
+  url: https://files.pythonhosted.org/packages/20/9f/bc63f0f0737ad7a60800bfd472a4836661adae21f9c2535f3957b1e54ceb/jedi-0.19.1-py2.py3-none-any.whl
+  sha256: e983c654fe5c02867aef4cdfce5a2fbb4a50adc0af145f70504238f18ef5e7e0
+  requires_dist:
+  - parso <0.9.0, >=0.8.3
+  - jinja2 ==2.11.3 ; extra == 'docs'
+  - markupsafe ==1.1.1 ; extra == 'docs'
+  - pygments ==2.8.1 ; extra == 'docs'
+  - alabaster ==0.7.12 ; extra == 'docs'
+  - babel ==2.9.1 ; extra == 'docs'
+  - chardet ==4.0.0 ; extra == 'docs'
+  - commonmark ==0.8.1 ; extra == 'docs'
+  - docutils ==0.17.1 ; extra == 'docs'
+  - future ==0.18.2 ; extra == 'docs'
+  - idna ==2.10 ; extra == 'docs'
+  - imagesize ==1.2.0 ; extra == 'docs'
+  - mock ==1.0.1 ; extra == 'docs'
+  - packaging ==20.9 ; extra == 'docs'
+  - pyparsing ==2.4.7 ; extra == 'docs'
+  - pytz ==2021.1 ; extra == 'docs'
+  - readthedocs-sphinx-ext ==2.1.4 ; extra == 'docs'
+  - recommonmark ==0.5.0 ; extra == 'docs'
+  - requests ==2.25.1 ; extra == 'docs'
+  - six ==1.15.0 ; extra == 'docs'
+  - snowballstemmer ==2.1.0 ; extra == 'docs'
+  - sphinx-rtd-theme ==0.4.3 ; extra == 'docs'
+  - sphinx ==1.8.5 ; extra == 'docs'
+  - sphinxcontrib-serializinghtml ==1.1.4 ; extra == 'docs'
+  - sphinxcontrib-websupport ==1.2.4 ; extra == 'docs'
+  - urllib3 ==1.26.4 ; extra == 'docs'
+  - flake8 ==5.0.4 ; extra == 'qa'
+  - mypy ==0.971 ; extra == 'qa'
+  - types-setuptools ==67.2.0.1 ; extra == 'qa'
+  - django ; extra == 'testing'
+  - attrs ; extra == 'testing'
+  - colorama ; extra == 'testing'
+  - docopt ; extra == 'testing'
+  - pytest <7.0.0 ; extra == 'testing'
+  requires_python: '>=3.6'
+- kind: pypi
   name: jsonschema
   version: 4.21.1
   url: https://files.pythonhosted.org/packages/39/9d/b035d024c62c85f2e2d4806a59ca7b8520307f34e0932fbc8cc75fe7b2d9/jsonschema-4.21.1-py3-none-any.whl
   sha256: 7996507afae316306f9e2290407761157c6f78002dcf7419acb99822143d1c6f
   requires_dist:
   - attrs >=22.2.0
   - importlib-resources >=1.4.0 ; python_version < '3.9'
@@ -4927,76 +5329,72 @@
   - libgcc-ng >=12
   license: BSD-3-Clause
   license_family: BSD
   size: 35720
   timestamp: 1680113474501
 - kind: conda
   name: libwebp-base
-  version: 1.3.2
-  build: h10d778d_1
-  build_number: 1
+  version: 1.4.0
+  build: h10d778d_0
   subdir: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.3.2-h10d778d_1.conda
-  sha256: cd2d651e90b93b03e4e38617aa15ddf8e5537b2bd22dd2628784e4c80bc107eb
-  md5: 1ff09ca6e85ee516442a6a94cdfc7065
+  url: https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.4.0-h10d778d_0.conda
+  sha256: 7bafd8f4c637778cd0aa390bf3a894feef0e1fcf6ea6000c7ffc25c4c5a65538
+  md5: b2c0047ea73819d992484faacbbe1c24
   constrains:
-  - libwebp 1.3.2
+  - libwebp 1.4.0
   license: BSD-3-Clause
   license_family: BSD
-  size: 350825
-  timestamp: 1712602583307
+  size: 355099
+  timestamp: 1713200298965
 - kind: conda
   name: libwebp-base
-  version: 1.3.2
-  build: h31becfc_1
-  build_number: 1
+  version: 1.4.0
+  build: h31becfc_0
   subdir: linux-aarch64
-  url: https://conda.anaconda.org/conda-forge/linux-aarch64/libwebp-base-1.3.2-h31becfc_1.conda
-  sha256: 65f96a2671cacb81eadf26d65ba29038a1f12fe5ba4652b1789fac920f332099
-  md5: 675c1f4aa320704b899f4eb350a69418
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/libwebp-base-1.4.0-h31becfc_0.conda
+  sha256: 10dded60f274e29c573cfacf6e96f5d0fc374ee431250374a44cbd773916ab9d
+  md5: 5fd7ab3e5f382c70607fbac6335e6e19
   depends:
   - libgcc-ng >=12
   constrains:
-  - libwebp 1.3.2
+  - libwebp 1.4.0
   license: BSD-3-Clause
   license_family: BSD
-  size: 355942
-  timestamp: 1712603681172
+  size: 363577
+  timestamp: 1713201785160
 - kind: conda
   name: libwebp-base
-  version: 1.3.2
-  build: h93a5062_1
-  build_number: 1
+  version: 1.4.0
+  build: h93a5062_0
   subdir: osx-arm64
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/libwebp-base-1.3.2-h93a5062_1.conda
-  sha256: 4336a22660ba77e9d2f5940ba184a85bb1da1b2f5488ba11b486dceca0b39aa1
-  md5: ce4e2ea0aa859a8796b1437fe5cb07ed
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libwebp-base-1.4.0-h93a5062_0.conda
+  sha256: 0d4bad713a512d79bfeb4d61821f447afab8b0792aca823f505ce6b195e9fde5
+  md5: c0af0edfebe780b19940e94871f1a765
   constrains:
-  - libwebp 1.3.2
+  - libwebp 1.4.0
   license: BSD-3-Clause
   license_family: BSD
-  size: 283775
-  timestamp: 1712602560769
+  size: 287750
+  timestamp: 1713200194013
 - kind: conda
   name: libwebp-base
-  version: 1.3.2
-  build: hd590300_1
-  build_number: 1
+  version: 1.4.0
+  build: hd590300_0
   subdir: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.3.2-hd590300_1.conda
-  sha256: c230e238646d0481851a44086767581cf7e112f27e97bb1c0b89175a079d961d
-  md5: 049b7df8bae5e184d1de42cdf64855f8
+  url: https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.4.0-hd590300_0.conda
+  sha256: 49bc5f6b1e11cb2babf2a2a731d1a680a5e08a858280876a779dbda06c78c35f
+  md5: b26e8aa824079e1be0294e7152ca4559
   depends:
   - libgcc-ng >=12
   constrains:
-  - libwebp 1.3.2
+  - libwebp 1.4.0
   license: BSD-3-Clause
   license_family: BSD
-  size: 434659
-  timestamp: 1712602397804
+  size: 438953
+  timestamp: 1713199854503
 - kind: conda
   name: libxcb
   version: '1.15'
   build: h0b41bf4_0
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.15-h0b41bf4_0.conda
   sha256: a670902f0a3173a466c058d2ac22ca1dd0df0453d3a80e0212815c20a16b0485
@@ -5054,66 +5452,66 @@
   - libgcc-ng >=12
   license: LGPL-2.1-or-later
   size: 100393
   timestamp: 1702724383534
 - kind: conda
   name: libxml2
   version: 2.12.6
-  build: h0d0cfa8_1
-  build_number: 1
+  build: h0d0cfa8_2
+  build_number: 2
   subdir: osx-arm64
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/libxml2-2.12.6-h0d0cfa8_1.conda
-  sha256: f18775ca8494ead5451d4acfc53fa7ebf7a8b5ed04c43bcc50fab847c9780cb3
-  md5: c08526c957192192e1e7b4f622761144
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/libxml2-2.12.6-h0d0cfa8_2.conda
+  sha256: a5c10af641d6accf3effb3c3a3c594d931bb374f9e3e796719f3ecf769cfb0fc
+  md5: 27577d561de7659487b062c363d8a527
   depends:
   - icu >=73.2,<74.0a0
   - libiconv >=1.17,<2.0a0
   - libzlib >=1.2.13,<1.3.0a0
   - xz >=5.2.6,<6.0a0
   license: MIT
   license_family: MIT
-  size: 588539
-  timestamp: 1711318256840
+  size: 588638
+  timestamp: 1713314780561
 - kind: conda
   name: libxml2
   version: 2.12.6
-  build: h8a06e1b_1
-  build_number: 1
+  build: h8a06e1b_2
+  build_number: 2
   subdir: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/libxml2-2.12.6-h8a06e1b_1.conda
-  sha256: 8e89e2af8f2abd0238ab6e98fa1b73bc5826de80e92c434da0dc0521e7546bd3
-  md5: 44a0e1b0e8eb3859cbf6889bf99151af
+  url: https://conda.anaconda.org/conda-forge/win-64/libxml2-2.12.6-h8a06e1b_2.conda
+  sha256: 1814b8e30e951a861cf21c05dd9e1cf704e7fa0d04e110977bf5e50796281a18
+  md5: dac404ec2f483d6c6f1dc698561e6fe9
   depends:
   - libiconv >=1.17,<2.0a0
   - libzlib >=1.3.1,<1.4.0a0
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   license: MIT
   license_family: MIT
-  size: 1568448
-  timestamp: 1711318556517
+  size: 1590639
+  timestamp: 1713315124559
 - kind: conda
   name: libxml2
   version: 2.12.6
-  build: hc0ae0f7_1
-  build_number: 1
+  build: hc0ae0f7_2
+  build_number: 2
   subdir: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.12.6-hc0ae0f7_1.conda
-  sha256: 07a5dc7316d4c1ff3d924df6a76e6a13380d702fa5b3b1889e56d0672e5b8201
-  md5: bd85e0ca9e1ffaadc3b56079fd956035
+  url: https://conda.anaconda.org/conda-forge/osx-64/libxml2-2.12.6-hc0ae0f7_2.conda
+  sha256: 2598a525b1769338f96c3d4badad7d8b95c9ddcea86db3f9479a274803190e5c
+  md5: 50b997370584f2c83ca0c38e9028eab9
   depends:
   - icu >=73.2,<74.0a0
   - libiconv >=1.17,<2.0a0
   - libzlib >=1.2.13,<1.3.0a0
   - xz >=5.2.6,<6.0a0
   license: MIT
   license_family: MIT
-  size: 620164
-  timestamp: 1711318305209
+  size: 619622
+  timestamp: 1713314870641
 - kind: conda
   name: libzlib
   version: 1.2.13
   build: h31becfc_5
   build_number: 5
   subdir: linux-aarch64
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/libzlib-1.2.13-h31becfc_5.conda
@@ -5784,14 +6182,22 @@
   url: https://conda.anaconda.org/conda-forge/osx-arm64/make-4.3-he57ea6c_1.tar.bz2
   sha256: a011e3e1c4caec821eb4213d0a0154d39e5f81a44d2e8bafe6f84e7840c3909e
   md5: 1939d04ef89e38fde652ee8c669e092f
   license: GPL-3.0-or-later
   license_family: GPL
   size: 253227
   timestamp: 1602706492919
+- kind: pypi
+  name: matplotlib-inline
+  version: 0.1.7
+  url: https://files.pythonhosted.org/packages/8f/8e/9ad090d3553c280a8060fbf6e24dc1c0c29704ee7d1c372f0c174aa59285/matplotlib_inline-0.1.7-py3-none-any.whl
+  sha256: df192d39a4ff8f21b1895d72e6a13f5fcc5099f00fa84384e0ea28c2cc0653ca
+  requires_dist:
+  - traitlets
+  requires_python: '>=3.8'
 - kind: conda
   name: mkl
   version: 2024.1.0
   build: h66d3029_692
   build_number: 692
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/mkl-2024.1.0-h66d3029_692.conda
@@ -5863,16 +6269,16 @@
   license: LGPL-3.0-only
   license_family: LGPL
   size: 373442
   timestamp: 1712339833358
 - kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/73/16/dfef780ced7d690dd5497846ed242ef3e27e319d59d1ddaae816a4f2c15e/msgspec-0.18.6-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: ad237100393f637b297926cae1868b0d500f764ccd2f0623a380e2bcfb2809ca
+  url: https://files.pythonhosted.org/packages/1d/b5/c8fbf1db814eb29eda402952374b594b2559419ba7ec6d0997a9e5687530/msgspec-0.18.6-cp312-cp312-macosx_10_9_x86_64.whl
+  sha256: d86f5071fe33e19500920333c11e2267a31942d18fed4d9de5bc2fbab267d28c
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -5941,16 +6347,16 @@
   - tomli-w ; extra == 'toml'
   - tomli ; python_version < '3.11' and extra == 'toml'
   - pyyaml ; extra == 'yaml'
   requires_python: '>=3.8'
 - kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/1d/b5/c8fbf1db814eb29eda402952374b594b2559419ba7ec6d0997a9e5687530/msgspec-0.18.6-cp312-cp312-macosx_10_9_x86_64.whl
-  sha256: d86f5071fe33e19500920333c11e2267a31942d18fed4d9de5bc2fbab267d28c
+  url: https://files.pythonhosted.org/packages/73/16/dfef780ced7d690dd5497846ed242ef3e27e319d59d1ddaae816a4f2c15e/msgspec-0.18.6-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: ad237100393f637b297926cae1868b0d500f764ccd2f0623a380e2bcfb2809ca
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -6114,14 +6520,20 @@
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4.20240210-h73e2aa4_0.conda
   sha256: 50b72acf08acbc4e5332807653e2ca6b26d4326e8af16fad1fd3f2ce9ea55503
   md5: 50f28c512e9ad78589e3eab34833f762
   license: X11 AND BSD-3-Clause
   size: 823010
   timestamp: 1710866856626
+- kind: pypi
+  name: nest-asyncio
+  version: 1.6.0
+  url: https://files.pythonhosted.org/packages/a0/c4/c2971a3ba4c6103a3d10c4b0f24f461ddc027f0f09763220cf35ca1401b3/nest_asyncio-1.6.0-py3-none-any.whl
+  sha256: 87af6efd6b5e897c81050477ef65c62e2b2f35d51703cae01aff2905b1852e1c
+  requires_python: '>=3.5'
 - kind: conda
   name: openssl
   version: 3.2.1
   build: h0d3ecfb_1
   build_number: 1
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.2.1-h0d3ecfb_1.conda
@@ -6204,14 +6616,20 @@
   - ca-certificates
   constrains:
   - pyopenssl >=22.1
   license: Apache-2.0
   license_family: Apache
   size: 2506344
   timestamp: 1710793930515
+- kind: pypi
+  name: packaging
+  version: '24.0'
+  url: https://files.pythonhosted.org/packages/49/df/1fceb2f8900f8639e278b056416d49134fb8d84c5942ffaa01ad34782422/packaging-24.0-py3-none-any.whl
+  sha256: 2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5
+  requires_python: '>=3.7'
 - kind: conda
   name: pango
   version: 1.52.1
   build: h11ef544_0
   subdir: linux-aarch64
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/pango-1.52.1-h11ef544_0.conda
   sha256: b0e69b9743e20a8adeaaa82afb659bbce58588a609e1a2ba9efbe2be5d765ec9
@@ -6286,14 +6704,26 @@
   - fribidi >=1.0.10,<2.0a0
   - harfbuzz >=8.3.0,<9.0a0
   - libglib >=2.78.4,<3.0a0
   - libpng >=1.6.43,<1.7.0a0
   license: LGPL-2.1-or-later
   size: 413416
   timestamp: 1709762628624
+- kind: pypi
+  name: parso
+  version: 0.8.4
+  url: https://files.pythonhosted.org/packages/c6/ac/dac4a63f978e4dcb3c6d3a78c4d8e0192a113d288502a1216950c41b1027/parso-0.8.4-py2.py3-none-any.whl
+  sha256: a418670a20291dacd2dddc80c377c5c3791378ee1e8d12bffc35420643d43f18
+  requires_dist:
+  - flake8 ==5.0.4 ; extra == 'qa'
+  - mypy ==0.971 ; extra == 'qa'
+  - types-setuptools ==67.2.0.1 ; extra == 'qa'
+  - docopt ; extra == 'testing'
+  - pytest ; extra == 'testing'
+  requires_python: '>=3.6'
 - kind: conda
   name: pcre2
   version: '10.42'
   build: h0ad2156_0
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/pcre2-10.42-h0ad2156_0.conda
   sha256: 689559d94b64914e503d2ced53b78afc19562ed1ccfb284040797a6d41bb564c
@@ -6349,19 +6779,27 @@
   - libgcc-ng >=12
   - libzlib >=1.2.13,<1.3.0a0
   license: BSD-3-Clause
   license_family: BSD
   size: 944649
   timestamp: 1698610795381
 - kind: pypi
+  name: pexpect
+  version: 4.9.0
+  url: https://files.pythonhosted.org/packages/9e/c3/059298687310d527a58bb01f3b1965787ee3b40dce76752eda8b44e9a2c5/pexpect-4.9.0-py2.py3-none-any.whl
+  sha256: 7236d1e080e4936be2dc3e326cec0af72acf9212a7e1d060210e70a47e253523
+  requires_dist:
+  - ptyprocess >=0.5
+- kind: pypi
   name: pixi-kernel
-  version: 0.2.1
+  version: 0.3.0
   path: ../../../../pixi-kernel
-  sha256: fc89be37749334e0eb20e8656e5ffcdace662e69fd273fa798213fdf1e64b7cb
+  sha256: 026726c0f08b63327906964394fdaf6d1b2324c25bf50c37e37b0300731fba40
   requires_dist:
+  - ipykernel >=6
   - jupyter-client >=7
   - msgspec >=0.18
   requires_python: <4.0,>=3.8
   editable: true
 - kind: conda
   name: pixman
   version: 0.43.2
@@ -6432,14 +6870,82 @@
   - sphinx >=7.2.6 ; extra == 'docs'
   - appdirs ==1.4.4 ; extra == 'test'
   - covdefaults >=2.3 ; extra == 'test'
   - pytest-cov >=4.1 ; extra == 'test'
   - pytest-mock >=3.12 ; extra == 'test'
   - pytest >=7.4.3 ; extra == 'test'
   requires_python: '>=3.8'
+- kind: pypi
+  name: prompt-toolkit
+  version: 3.0.43
+  url: https://files.pythonhosted.org/packages/ee/fd/ca7bf3869e7caa7a037e23078539467b433a4e01eebd93f77180ab927766/prompt_toolkit-3.0.43-py3-none-any.whl
+  sha256: a11a29cb3bf0a28a387fe5122cdb649816a957cd9261dcedf8c9f1fef33eacf6
+  requires_dist:
+  - wcwidth
+  requires_python: '>=3.7.0'
+- kind: pypi
+  name: psutil
+  version: 5.9.8
+  url: https://files.pythonhosted.org/packages/e7/e3/07ae864a636d70a8a6f58da27cb1179192f1140d5d1da10886ade9405797/psutil-5.9.8-cp36-abi3-macosx_10_9_x86_64.whl
+  sha256: aee678c8720623dc456fa20659af736241f575d79429a0e5e9cf88ae0605cc81
+  requires_dist:
+  - ipaddress ; python_version < '3.0' and extra == 'test'
+  - mock ; python_version < '3.0' and extra == 'test'
+  - enum34 ; python_version <= '3.4' and extra == 'test'
+  - pywin32 ; sys_platform == 'win32' and extra == 'test'
+  - wmi ; sys_platform == 'win32' and extra == 'test'
+  requires_python: '>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*'
+- kind: pypi
+  name: psutil
+  version: 5.9.8
+  url: https://files.pythonhosted.org/packages/93/52/3e39d26feae7df0aa0fd510b14012c3678b36ed068f7d78b8d8784d61f0e/psutil-5.9.8-cp37-abi3-win_amd64.whl
+  sha256: 8db4c1b57507eef143a15a6884ca10f7c73876cdf5d51e713151c1236a0e68cf
+  requires_dist:
+  - ipaddress ; python_version < '3.0' and extra == 'test'
+  - mock ; python_version < '3.0' and extra == 'test'
+  - enum34 ; python_version <= '3.4' and extra == 'test'
+  - pywin32 ; sys_platform == 'win32' and extra == 'test'
+  - wmi ; sys_platform == 'win32' and extra == 'test'
+  requires_python: '>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*'
+- kind: pypi
+  name: psutil
+  version: 5.9.8
+  url: https://files.pythonhosted.org/packages/c5/4f/0e22aaa246f96d6ac87fe5ebb9c5a693fbe8877f537a1022527c47ca43c5/psutil-5.9.8-cp36-abi3-manylinux_2_12_x86_64.manylinux2010_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: d06016f7f8625a1825ba3732081d77c94589dca78b7a3fc072194851e88461a4
+  requires_dist:
+  - ipaddress ; python_version < '3.0' and extra == 'test'
+  - mock ; python_version < '3.0' and extra == 'test'
+  - enum34 ; python_version <= '3.4' and extra == 'test'
+  - pywin32 ; sys_platform == 'win32' and extra == 'test'
+  - wmi ; sys_platform == 'win32' and extra == 'test'
+  requires_python: '>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*'
+- kind: pypi
+  name: psutil
+  version: 5.9.8
+  url: https://files.pythonhosted.org/packages/05/33/2d74d588408caedd065c2497bdb5ef83ce6082db01289a1e1147f6639802/psutil-5.9.8-cp38-abi3-macosx_11_0_arm64.whl
+  sha256: d16bbddf0693323b8c6123dd804100241da461e41d6e332fb0ba6058f630f8c8
+  requires_dist:
+  - ipaddress ; python_version < '3.0' and extra == 'test'
+  - mock ; python_version < '3.0' and extra == 'test'
+  - enum34 ; python_version <= '3.4' and extra == 'test'
+  - pywin32 ; sys_platform == 'win32' and extra == 'test'
+  - wmi ; sys_platform == 'win32' and extra == 'test'
+  requires_python: '>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*'
+- kind: pypi
+  name: psutil
+  version: 5.9.8
+  url: https://files.pythonhosted.org/packages/90/c7/6dc0a455d111f68ee43f27793971cf03fe29b6ef972042549db29eec39a2/psutil-5.9.8.tar.gz
+  sha256: 6be126e3225486dff286a8fb9a06246a5253f4c7c53b475ea5f5ac934e64194c
+  requires_dist:
+  - ipaddress ; python_version < '3.0' and extra == 'test'
+  - mock ; python_version < '3.0' and extra == 'test'
+  - enum34 ; python_version <= '3.4' and extra == 'test'
+  - pywin32 ; sys_platform == 'win32' and extra == 'test'
+  - wmi ; sys_platform == 'win32' and extra == 'test'
+  requires_python: '>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*'
 - kind: conda
   name: pthread-stubs
   version: '0.4'
   build: h36c2ea0_1001
   build_number: 1001
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/pthread-stubs-0.4-h36c2ea0_1001.tar.bz2
@@ -6476,14 +6982,35 @@
   sha256: 576a228630a72f25d255a5e345e5f10878e153221a96560f2498040cd6f54005
   md5: e2da8758d7d51ff6aa78a14dfb9dbed4
   depends:
   - vc 14.*
   license: LGPL 2
   size: 144301
   timestamp: 1537755684331
+- kind: pypi
+  name: ptyprocess
+  version: 0.7.0
+  url: https://files.pythonhosted.org/packages/22/a6/858897256d0deac81a172289110f31629fc4cee19b6f01283303e18c8db3/ptyprocess-0.7.0-py2.py3-none-any.whl
+  sha256: 4b41f3967fce3af57cc7e94b888626c18bf37a083e3651ca8feeb66d492fef35
+- kind: pypi
+  name: pure-eval
+  version: 0.2.2
+  url: https://files.pythonhosted.org/packages/2b/27/77f9d5684e6bce929f5cfe18d6cfbe5133013c06cb2fbf5933670e60761d/pure_eval-0.2.2-py3-none-any.whl
+  sha256: 01eaab343580944bc56080ebe0a674b39ec44a945e6d09ba7db3cb8cec289350
+  requires_dist:
+  - pytest ; extra == 'tests'
+- kind: pypi
+  name: pygments
+  version: 2.17.2
+  url: https://files.pythonhosted.org/packages/97/9c/372fef8377a6e340b1704768d20daaded98bf13282b5327beb2e2fe2c7ef/pygments-2.17.2-py3-none-any.whl
+  sha256: b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c
+  requires_dist:
+  - importlib-metadata ; python_version < '3.8' and extra == 'plugins'
+  - colorama >=0.4.6 ; extra == 'windows-terminal'
+  requires_python: '>=3.7'
 - kind: conda
   name: python
   version: 3.9.7
   build: h900ac77_3_cpython
   build_number: 3
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/python-3.9.7-h900ac77_3_cpython.tar.bz2
@@ -6498,122 +7025,124 @@
   constrains:
   - python_abi 3.9.* *_cp39
   license: Python-2.0
   size: 21077172
   timestamp: 1632943539852
 - kind: conda
   name: python
-  version: 3.12.2
-  build: h43d1f9e_0_cpython
-  subdir: linux-aarch64
-  url: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.2-h43d1f9e_0_cpython.conda
-  sha256: 16c8e77c01b814d836af632ef77eac21b64b9e398a11e1403a3a1802bb5be366
-  md5: 3a41090f2ef0868f119825593948ed46
+  version: 3.12.3
+  build: h1411813_0_cpython
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda
+  sha256: 3b327ffc152a245011011d1d730781577a8274fde1cf6243f073749ead8f1c2a
+  md5: df1448ec6cbf8eceb03d29003cf72ae6
   depends:
+  - __osx >=10.9
   - bzip2 >=1.0.8,<2.0a0
-  - ld_impl_linux-aarch64 >=2.36.1
-  - libexpat >=2.5.0,<3.0a0
+  - libexpat >=2.6.2,<3.0a0
   - libffi >=3.4,<4.0a0
-  - libgcc-ng >=12
-  - libnsl >=2.0.1,<2.1.0a0
-  - libsqlite >=3.45.1,<4.0a0
-  - libuuid >=2.38.1,<3.0a0
-  - libxcrypt >=4.4.36
+  - libsqlite >=3.45.2,<4.0a0
   - libzlib >=1.2.13,<1.3.0a0
-  - ncurses >=6.4,<7.0a0
+  - ncurses >=6.4.20240210,<7.0a0
   - openssl >=3.2.1,<4.0a0
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.12.* *_cp312
   license: Python-2.0
-  size: 13823577
-  timestamp: 1708116074721
+  size: 14557341
+  timestamp: 1713208068012
 - kind: conda
   name: python
-  version: 3.12.2
-  build: h9f0c242_0_cpython
-  subdir: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.2-h9f0c242_0_cpython.conda
-  sha256: 7647ac06c3798a182a4bcb1ff58864f1ef81eb3acea6971295304c23e43252fb
-  md5: 0179b8007ba008cf5bec11f3b3853902
+  version: 3.12.3
+  build: h43d1f9e_0_cpython
+  subdir: linux-aarch64
+  url: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.12.3-h43d1f9e_0_cpython.conda
+  sha256: e186f3ee570464241c844adff6a3ba8f395cef15c5d46c0a8f784cfd97b3bdca
+  md5: dc93ad1d2ba17ebc948bf5434ffa864b
   depends:
   - bzip2 >=1.0.8,<2.0a0
-  - libexpat >=2.5.0,<3.0a0
+  - ld_impl_linux-aarch64 >=2.36.1
+  - libexpat >=2.6.2,<3.0a0
   - libffi >=3.4,<4.0a0
-  - libsqlite >=3.45.1,<4.0a0
+  - libgcc-ng >=12
+  - libnsl >=2.0.1,<2.1.0a0
+  - libsqlite >=3.45.2,<4.0a0
+  - libuuid >=2.38.1,<3.0a0
+  - libxcrypt >=4.4.36
   - libzlib >=1.2.13,<1.3.0a0
-  - ncurses >=6.4,<7.0a0
+  - ncurses >=6.4.20240210,<7.0a0
   - openssl >=3.2.1,<4.0a0
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.12.* *_cp312
   license: Python-2.0
-  size: 14596811
-  timestamp: 1708118065292
+  size: 14051797
+  timestamp: 1713205211165
 - kind: conda
   name: python
-  version: 3.12.2
-  build: hab00c5b_0_cpython
-  subdir: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.2-hab00c5b_0_cpython.conda
-  sha256: ddb7a2d8d78046bda5d7631e6814f9468d2eb054e10f86f4648c9d1fdaa30c0f
-  md5: ad7b68400f3a6ebe72b00be093c7f301
+  version: 3.12.3
+  build: h4a7b5fc_0_cpython
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.3-h4a7b5fc_0_cpython.conda
+  sha256: c761fb3713ea66bce3889b33b6f400afb2dd192d1fc2686446e9d8166cfcec6b
+  md5: 8643ab37bece6ae8f112464068d9df9c
   depends:
+  - __osx >=11.0
   - bzip2 >=1.0.8,<2.0a0
-  - ld_impl_linux-64 >=2.36.1
-  - libexpat >=2.5.0,<3.0a0
+  - libexpat >=2.6.2,<3.0a0
   - libffi >=3.4,<4.0a0
-  - libgcc-ng >=12
-  - libnsl >=2.0.1,<2.1.0a0
-  - libsqlite >=3.45.1,<4.0a0
-  - libuuid >=2.38.1,<3.0a0
-  - libxcrypt >=4.4.36
+  - libsqlite >=3.45.2,<4.0a0
   - libzlib >=1.2.13,<1.3.0a0
-  - ncurses >=6.4,<7.0a0
+  - ncurses >=6.4.20240210,<7.0a0
   - openssl >=3.2.1,<4.0a0
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.12.* *_cp312
   license: Python-2.0
-  size: 32312631
-  timestamp: 1708118077305
+  size: 13207557
+  timestamp: 1713206576646
 - kind: conda
   name: python
-  version: 3.12.2
-  build: hdf0ec26_0_cpython
-  subdir: osx-arm64
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.2-hdf0ec26_0_cpython.conda
-  sha256: ccd6c55a286d51d907c878ed2bfa7d1becce0fee71374a9386c5eb90d803ac72
-  md5: 85e91138ae921a2771f57a50120272bd
+  version: 3.12.3
+  build: hab00c5b_0_cpython
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda
+  sha256: f9865bcbff69f15fd89a33a2da12ad616e98d65ce7c83c644b92e66e5016b227
+  md5: 2540b74d304f71d3e89c81209db4db84
   depends:
   - bzip2 >=1.0.8,<2.0a0
-  - libexpat >=2.5.0,<3.0a0
+  - ld_impl_linux-64 >=2.36.1
+  - libexpat >=2.6.2,<3.0a0
   - libffi >=3.4,<4.0a0
-  - libsqlite >=3.45.1,<4.0a0
+  - libgcc-ng >=12
+  - libnsl >=2.0.1,<2.1.0a0
+  - libsqlite >=3.45.2,<4.0a0
+  - libuuid >=2.38.1,<3.0a0
+  - libxcrypt >=4.4.36
   - libzlib >=1.2.13,<1.3.0a0
-  - ncurses >=6.4,<7.0a0
+  - ncurses >=6.4.20240210,<7.0a0
   - openssl >=3.2.1,<4.0a0
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.12.* *_cp312
   license: Python-2.0
-  size: 13085901
-  timestamp: 1708117361381
+  size: 31991381
+  timestamp: 1713208036041
 - kind: pypi
   name: python-dateutil
   version: 2.9.0.post0
   url: https://files.pythonhosted.org/packages/ec/57/56b9bcc3c9c6a792fcbaf139543cee77261f3651ca9da0c93f5c1221264b/python_dateutil-2.9.0.post0-py2.py3-none-any.whl
   sha256: a8b2bc7bffae282281c8140a97d3aa9c14da0b136dfe83f850eea9a5f7470427
   requires_dist:
   - six >=1.5
@@ -6621,44 +7150,44 @@
 - kind: pypi
   name: pywin32
   version: '306'
   url: https://files.pythonhosted.org/packages/1c/f7/24d8ed4fd9c43b90354df7764f81f0dd5e623f9a50f1538f90fe085d6dff/pywin32-306-cp39-cp39-win_amd64.whl
   sha256: 39b61c15272833b5c329a2989999dcae836b1eed650252ab1b7bfbe1d59f30f4
 - kind: pypi
   name: pyzmq
-  version: 25.1.2
-  url: https://files.pythonhosted.org/packages/93/b7/6e291eafbbbc66d0e87658dd21383ec2b4ab35edcfb283902c580a6db76f/pyzmq-25.1.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: 02c9087b109070c5ab0b383079fa1b5f797f8d43e9a66c07a4b8b8bdecfd88ee
+  version: 26.0.0
+  url: https://files.pythonhosted.org/packages/f6/2c/7074b0747be7a23c9d2b15d603fbc1a55aa305665a2c0798d27c3baafa9e/pyzmq-26.0.0-cp312-cp312-macosx_10_15_universal2.whl
+  sha256: 469f4febd63c26b20132e54cc40048d5698123794b103758ccd21b8a45890dc3
   requires_dist:
   - cffi ; implementation_name == 'pypy'
-  requires_python: '>=3.6'
+  requires_python: '>=3.7'
 - kind: pypi
   name: pyzmq
-  version: 25.1.2
-  url: https://files.pythonhosted.org/packages/11/ae/d573f1c3854fff3714fe3cbf8ed3ce4200cc2aa81ab159dfe74b660d6523/pyzmq-25.1.2-cp39-cp39-win_amd64.whl
-  sha256: 8e9f3fabc445d0ce320ea2c59a75fe3ea591fdbdeebec5db6de530dd4b09412e
+  version: 26.0.0
+  url: https://files.pythonhosted.org/packages/41/fb/ddb8ed65b3be53eb2fdaacd57ef33d6019daf12a6155fa96181c1d264c13/pyzmq-26.0.0-cp39-cp39-win_amd64.whl
+  sha256: e0c08a6070358a2984900a4518e2dacbfaf24aac018ab086d7ac2f6069b13340
   requires_dist:
   - cffi ; implementation_name == 'pypy'
-  requires_python: '>=3.6'
+  requires_python: '>=3.7'
 - kind: pypi
   name: pyzmq
-  version: 25.1.2
-  url: https://files.pythonhosted.org/packages/6e/f0/d71cf69dc039c9adc8b625efc3bad3684f3660a570e47f0f0c64df787b41/pyzmq-25.1.2-cp312-cp312-macosx_10_15_universal2.whl
-  sha256: 11e70516688190e9c2db14fcf93c04192b02d457b582a1f6190b154691b4c93a
+  version: 26.0.0
+  url: https://files.pythonhosted.org/packages/61/01/eb6165d9160065845179f8f168ea70eaa24aa7e63f53b13966bbe368d6fa/pyzmq-26.0.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: af9f5b1b76753584c871c1c96db8a18650886b3adf9fc8c7d4019343eb329c28
   requires_dist:
   - cffi ; implementation_name == 'pypy'
-  requires_python: '>=3.6'
+  requires_python: '>=3.7'
 - kind: pypi
   name: pyzmq
-  version: 25.1.2
-  url: https://files.pythonhosted.org/packages/72/55/cc3163e20f40615a49245fa7041badec6103e8ee7e482dbb0feea00a7b84/pyzmq-25.1.2-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
-  sha256: 1b3cbba2f47062b85fe0ef9de5b987612140a9ba3a9c6d2543c6dec9f7c2ab27
+  version: 26.0.0
+  url: https://files.pythonhosted.org/packages/bf/4a/c6729cc692e2db85cc882bcf03a32536d9ff6a0e852f240156e71daade21/pyzmq-26.0.0-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
+  sha256: 6e0e94ca9a8f23000d54e11ecd727b69fb1994baf3b6b1eedb881cdd3196ecec
   requires_dist:
   - cffi ; implementation_name == 'pypy'
-  requires_python: '>=3.6'
+  requires_python: '>=3.7'
 - kind: conda
   name: r-base
   version: 4.1.3
   build: hdca333a_12
   build_number: 12
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/r-base-4.1.3-hdca333a_12.conda
@@ -8348,28 +8877,28 @@
   requires_dist:
   - attrs >=22.2.0
   - rpds-py >=0.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
-  url: https://files.pythonhosted.org/packages/c3/96/2211a1ca4b4e259e222169074ec0fa41f0ee18665dfc68988a139dc7e6e8/rpds_py-0.18.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: 4457a94da0d5c53dc4b3e4de1158bdab077db23c53232f37a3cb7afdb053a4e3
+  url: https://files.pythonhosted.org/packages/09/b6/45690f5d3f8c551bb462e063a2f336d72c8884ed26aa19beb53a374d3854/rpds_py-0.18.0-cp312-cp312-macosx_10_12_x86_64.whl
+  sha256: 7f2facbd386dd60cbbf1a794181e6aa0bd429bd78bfdf775436020172e2a23f0
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
   url: https://files.pythonhosted.org/packages/a0/62/c896cec9434e09fb933f3cadd5c699e9cea49ab8934d694b6634650748db/rpds_py-0.18.0-cp39-none-win_amd64.whl
   sha256: 6ef687afab047554a2d366e112dd187b62d261d49eb79b77e386f94644363294
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
-  url: https://files.pythonhosted.org/packages/09/b6/45690f5d3f8c551bb462e063a2f336d72c8884ed26aa19beb53a374d3854/rpds_py-0.18.0-cp312-cp312-macosx_10_12_x86_64.whl
-  sha256: 7f2facbd386dd60cbbf1a794181e6aa0bd429bd78bfdf775436020172e2a23f0
+  url: https://files.pythonhosted.org/packages/c3/96/2211a1ca4b4e259e222169074ec0fa41f0ee18665dfc68988a139dc7e6e8/rpds_py-0.18.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: 4457a94da0d5c53dc4b3e4de1158bdab077db23c53232f37a3cb7afdb053a4e3
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
   url: https://files.pythonhosted.org/packages/7a/58/9bfc53b266df92f0515e72fd16e4890dc6b56fc3bfc216b3a2a729c866b5/rpds_py-0.18.0-cp312-cp312-macosx_11_0_arm64.whl
   sha256: 1d9a5be316c15ffb2b3c405c4ff14448c36b4435be062a7f578ccd8b01f0c4d8
   requires_python: '>=3.8'
@@ -8451,14 +8980,28 @@
   - libsqlite 3.45.2 hcfcfb64_0
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   license: Unlicense
   size: 873024
   timestamp: 1710255122348
+- kind: pypi
+  name: stack-data
+  version: 0.6.3
+  url: https://files.pythonhosted.org/packages/f1/7b/ce1eafaf1a76852e2ec9b22edecf1daa58175c090266e9f6c64afcd81d91/stack_data-0.6.3-py3-none-any.whl
+  sha256: d5558e0c25a4cb0853cddad3d77da9891a08cb85dd9f9f91b9f8cd66e511e695
+  requires_dist:
+  - executing >=1.2.0
+  - asttokens >=2.1.0
+  - pure-eval
+  - pytest ; extra == 'tests'
+  - typeguard ; extra == 'tests'
+  - pygments ; extra == 'tests'
+  - littleutils ; extra == 'tests'
+  - cython ; extra == 'tests'
 - kind: conda
   name: sysroot_linux-64
   version: '2.12'
   build: he073ed8_17
   build_number: 17
   subdir: noarch
   noarch: generic
@@ -8526,14 +9069,15 @@
   md5: 21745fdd12f01b41178596143cbecffd
   depends:
   - libhwloc >=2.10.0,<2.10.1.0a0
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   license: Apache-2.0
+  license_family: APACHE
   size: 161618
   timestamp: 1712960215111
 - kind: conda
   name: tk
   version: 8.6.13
   build: h194ca79_0
   subdir: linux-aarch64
@@ -8650,28 +9194,28 @@
   - tk >=8.6.13,<8.7.0a0
   license: TCL
   size: 79797
   timestamp: 1695716570153
 - kind: pypi
   name: tornado
   version: '6.4'
-  url: https://files.pythonhosted.org/packages/9f/12/11d0a757bb67278d3380d41955ae98527d5ad18330b2edbdc8de222b569b/tornado-6.4-cp38-abi3-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: f0251554cdd50b4b44362f73ad5ba7126fc5b2c2895cc62b14a1c2d7ea32f212
+  url: https://files.pythonhosted.org/packages/34/7a/e7ec972db24513ea69ac7132c1a5eef62309dc978566a4afffa314417a45/tornado-6.4-cp38-abi3-macosx_10_9_x86_64.whl
+  sha256: 27787de946a9cffd63ce5814c33f734c627a87072ec7eed71f7fc4417bb16263
   requires_python: '>=3.8'
 - kind: pypi
   name: tornado
   version: '6.4'
   url: https://files.pythonhosted.org/packages/af/2b/4649926f17c1634d21c584cc855b5c5021f148b934919d26932a595bc034/tornado-6.4-cp38-abi3-win_amd64.whl
   sha256: 10aeaa8006333433da48dec9fe417877f8bcc21f48dda8d661ae79da357b2a63
   requires_python: '>=3.8'
 - kind: pypi
   name: tornado
   version: '6.4'
-  url: https://files.pythonhosted.org/packages/34/7a/e7ec972db24513ea69ac7132c1a5eef62309dc978566a4afffa314417a45/tornado-6.4-cp38-abi3-macosx_10_9_x86_64.whl
-  sha256: 27787de946a9cffd63ce5814c33f734c627a87072ec7eed71f7fc4417bb16263
+  url: https://files.pythonhosted.org/packages/9f/12/11d0a757bb67278d3380d41955ae98527d5ad18330b2edbdc8de222b569b/tornado-6.4-cp38-abi3-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: f0251554cdd50b4b44362f73ad5ba7126fc5b2c2895cc62b14a1c2d7ea32f212
   requires_python: '>=3.8'
 - kind: pypi
   name: tornado
   version: '6.4'
   url: https://files.pythonhosted.org/packages/4a/2e/3ba930e3af171847d610e07ae878e04fcb7e4d7822f1a2d29a27b128ea24/tornado-6.4-cp38-abi3-macosx_10_9_universal2.whl
   sha256: 02ccefc7d8211e5a7f9e8bc3f9e5b0ad6262ba2fbb683a6443ecc804e5224ce0
   requires_python: '>=3.8'
@@ -8693,14 +9237,20 @@
   - argcomplete >=3.0.3 ; extra == 'test'
   - mypy >=1.7.0 ; extra == 'test'
   - pre-commit ; extra == 'test'
   - pytest-mock ; extra == 'test'
   - pytest-mypy-testing ; extra == 'test'
   - pytest <8.1, >=7.0 ; extra == 'test'
   requires_python: '>=3.8'
+- kind: pypi
+  name: typing-extensions
+  version: 4.11.0
+  url: https://files.pythonhosted.org/packages/01/f3/936e209267d6ef7510322191003885de524fc48d1b43269810cd589ceaf5/typing_extensions-4.11.0-py3-none-any.whl
+  sha256: c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
+  requires_python: '>=3.8'
 - kind: conda
   name: tzdata
   version: 2024a
   build: h0c530f3_0
   subdir: noarch
   noarch: generic
   url: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
@@ -8768,14 +9318,21 @@
   md5: 10d42885e3ed84e575b454db30f1aa93
   depends:
   - vc14_runtime >=14.38.33130
   license: BSD-3-Clause
   license_family: BSD
   size: 16988
   timestamp: 1702511261442
+- kind: pypi
+  name: wcwidth
+  version: 0.2.13
+  url: https://files.pythonhosted.org/packages/fd/84/fd2ba7aafacbad3c4201d395674fc6348826569da3c0937e75505ead3528/wcwidth-0.2.13-py2.py3-none-any.whl
+  sha256: 3da69048e4540d84af32131829ff948f1e022c1c6bdb8d6102117aac784f6859
+  requires_dist:
+  - backports-functools-lru-cache >=1.2.1 ; python_version < '3.2'
 - kind: conda
   name: xorg-kbproto
   version: 1.0.7
   build: h3557bc0_1002
   build_number: 1002
   subdir: linux-aarch64
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/xorg-kbproto-1.0.7-h3557bc0_1002.tar.bz2
```

### Comparing `pixi_kernel-0.2.1/tests/integration/xeus-cling/kernel.py` & `pixi_kernel-0.3.0/tests/integration/xeus-cling/kernel.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,16 @@
 """Reference: https://github.com/jupyter/jupyter_kernel_test/blob/5f2c65271b48dc95fc75a9585cb1d6db0bb55557/test_xeus_cling.py"""
 # ruff: noqa: RUF012
 
-import os
 import unittest
-from contextlib import contextmanager
-from pathlib import Path
-from typing import Union
 
 import jupyter_kernel_test as jkt
 from jupyter_client.kernelspec import NoSuchKernel
 
 
-@contextmanager
-def cwd(new_dir: Union[str, Path]):
-    original_dir = Path.cwd().resolve()
-    try:
-        os.chdir(new_dir)
-        yield
-    finally:
-        os.chdir(original_dir)
-
-
 class XCpp17Tests(jkt.KernelTests):
     kernel_name = "pixi-kernel-xcpp17"
 
     @classmethod
     def setUpClass(cls):
         try:
             cls.km, cls.kc = jkt.start_new_kernel(kernel_name=cls.kernel_name)
@@ -54,9 +40,8 @@
 
 
 class XCpp11Tests(XCpp17Tests):
     kernel_name = "pixi-kernel-xcpp11"
 
 
 if __name__ == "__main__":
-    with cwd(Path(__file__).parent.resolve()):
-        unittest.main()
+    unittest.main()
```

### Comparing `pixi_kernel-0.2.1/tests/integration/xeus-cling/pixi.lock` & `pixi_kernel-0.3.0/tests/integration/xeus-cling/pixi.lock`

 * *Files 11% similar despite different names*

```diff
@@ -44,40 +44,60 @@
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/llvm-tools-9.0.1-cling_v0.9_h2b820e9_7.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/llvmdev-9.0.1-cling_v0.9_h2b820e9_7.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4.20240210-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/nlohmann_json-3.11.3-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/pugixml-1.14-h59595ed_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.2-hab00c5b_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/sysroot_linux-64-2.12-he073ed8_17.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xeus-3.1.5-h06414e2_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xeus-cling-0.15.3-he80cb83_2.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xeus-zmq-1.1.1-h6b5a882_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xtl-0.7.7-h00ab1b0_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.5-h59595ed_1.conda
+      - pypi: https://files.pythonhosted.org/packages/45/86/4736ac618d82a20d87d2f92ae19441ebc7ac9e7a581d7e58bbe79233b24a/asttokens-2.4.1-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/e0/44/827b2a91a5816512fcaf3cc4ebc465ccd5d598c45cefa6703fcf4a79018f/attrs-23.2.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/e6/75/49e5bfe642f71f272236b5b2d2691cf915a7283cc0ceda56357b61daa538/comm-0.2.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/3c/7a/e400d9f5ed6b4b5ec9f350b4d7974e986ca2d455221e567e648edfad898e/debugpy-1.8.1-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+      - pypi: https://files.pythonhosted.org/packages/d5/50/83c593b07763e1161326b3b8c6686f0f4b0f24d5526546bee538c89837d6/decorator-5.1.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/80/03/6ea8b1b2a5ab40a7a60dc464d3daa7aa546e0a74d74a9f8ff551ea7905db/executing-2.0.1-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/53/9d/40d5207db523363d9b5698f33778c18b0d591e3fdb6e0116b894b2a2491c/ipykernel-6.29.4-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/8a/15/ea245239487bbd8d7203fe010ea48c7539e42bf1fde0592313241a3fba3a/ipython-8.23.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/20/9f/bc63f0f0737ad7a60800bfd472a4836661adae21f9c2535f3957b1e54ceb/jedi-0.19.1-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/39/9d/b035d024c62c85f2e2d4806a59ca7b8520307f34e0932fbc8cc75fe7b2d9/jsonschema-4.21.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/ee/07/44bd408781594c4d0a027666ef27fab1e441b109dc3b76b4f836f8fd04fe/jsonschema_specifications-2023.12.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/75/6d/d7b55b9c1ac802ab066b3e5015e90faab1fffbbd67a2af498ffc6cc81c97/jupyter_client-8.6.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/c9/fb/108ecd1fe961941959ad0ee4e12ee7b8b1477247f30b1fdfd83ceaf017f0/jupyter_core-5.7.2-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/72/42/d57a938cad4e99bb799f35105561959b0a0550c65fbc1ed671196e27f909/jupyter_kernel_test-0.7.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/8f/8e/9ad090d3553c280a8060fbf6e24dc1c0c29704ee7d1c372f0c174aa59285/matplotlib_inline-0.1.7-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/73/16/dfef780ced7d690dd5497846ed242ef3e27e319d59d1ddaae816a4f2c15e/msgspec-0.18.6-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+      - pypi: https://files.pythonhosted.org/packages/a0/c4/c2971a3ba4c6103a3d10c4b0f24f461ddc027f0f09763220cf35ca1401b3/nest_asyncio-1.6.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/49/df/1fceb2f8900f8639e278b056416d49134fb8d84c5942ffaa01ad34782422/packaging-24.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/c6/ac/dac4a63f978e4dcb3c6d3a78c4d8e0192a113d288502a1216950c41b1027/parso-0.8.4-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/9e/c3/059298687310d527a58bb01f3b1965787ee3b40dce76752eda8b44e9a2c5/pexpect-4.9.0-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/55/72/4898c44ee9ea6f43396fbc23d9bfaf3d06e01b83698bdf2e4c919deceb7c/platformdirs-4.2.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/ee/fd/ca7bf3869e7caa7a037e23078539467b433a4e01eebd93f77180ab927766/prompt_toolkit-3.0.43-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/c5/4f/0e22aaa246f96d6ac87fe5ebb9c5a693fbe8877f537a1022527c47ca43c5/psutil-5.9.8-cp36-abi3-manylinux_2_12_x86_64.manylinux2010_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+      - pypi: https://files.pythonhosted.org/packages/22/a6/858897256d0deac81a172289110f31629fc4cee19b6f01283303e18c8db3/ptyprocess-0.7.0-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/2b/27/77f9d5684e6bce929f5cfe18d6cfbe5133013c06cb2fbf5933670e60761d/pure_eval-0.2.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/97/9c/372fef8377a6e340b1704768d20daaded98bf13282b5327beb2e2fe2c7ef/pygments-2.17.2-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/ec/57/56b9bcc3c9c6a792fcbaf139543cee77261f3651ca9da0c93f5c1221264b/python_dateutil-2.9.0.post0-py2.py3-none-any.whl
-      - pypi: https://files.pythonhosted.org/packages/93/b7/6e291eafbbbc66d0e87658dd21383ec2b4ab35edcfb283902c580a6db76f/pyzmq-25.1.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+      - pypi: https://files.pythonhosted.org/packages/61/01/eb6165d9160065845179f8f168ea70eaa24aa7e63f53b13966bbe368d6fa/pyzmq-26.0.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
       - pypi: https://files.pythonhosted.org/packages/42/8e/ae1de7b12223986e949bdb886c004de7c304b6fa94de5b87c926c1099656/referencing-0.34.0-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/c3/96/2211a1ca4b4e259e222169074ec0fa41f0ee18665dfc68988a139dc7e6e8/rpds_py-0.18.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
       - pypi: https://files.pythonhosted.org/packages/d9/5a/e7c31adbe875f2abbb91bd84cf2dc52d792b5a01506781dbcf25c91daf11/six-1.16.0-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/f1/7b/ce1eafaf1a76852e2ec9b22edecf1daa58175c090266e9f6c64afcd81d91/stack_data-0.6.3-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/9f/12/11d0a757bb67278d3380d41955ae98527d5ad18330b2edbdc8de222b569b/tornado-6.4-cp38-abi3-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl
       - pypi: https://files.pythonhosted.org/packages/7c/c4/366a09036c07f46eb8c9b2af39c97f502ef24f11f2a6e4d763655d9f2708/traitlets-5.14.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/fd/84/fd2ba7aafacbad3c4201d395674fc6348826569da3c0937e75505ead3528/wcwidth-0.2.13-py2.py3-none-any.whl
       - pypi: ../../../../pixi-kernel
       linux-aarch64:
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/_openmp_mutex-4.5-2_gnu.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/_sysroot_linux-aarch64_curr_repodata_hack-4-h57d6b7b_14.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/binutils_impl_linux-aarch64-2.39-h48546ad_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/binutils_linux-aarch64-2.39-h489c705_13.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/bzip2-1.0.8-h31becfc_5.conda
@@ -118,29 +138,50 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/xeus-2.4.1-h68f4542_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/xeus-cling-0.13.0-hf59949a_3.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/xtl-0.7.7-h2a328a1_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/xz-5.2.6-h9cdd2b7_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/zeromq-4.3.5-h2f0025b_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-aarch64/zlib-1.2.13-h31becfc_5.conda
+      - pypi: https://files.pythonhosted.org/packages/45/86/4736ac618d82a20d87d2f92ae19441ebc7ac9e7a581d7e58bbe79233b24a/asttokens-2.4.1-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/e0/44/827b2a91a5816512fcaf3cc4ebc465ccd5d598c45cefa6703fcf4a79018f/attrs-23.2.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/e6/75/49e5bfe642f71f272236b5b2d2691cf915a7283cc0ceda56357b61daa538/comm-0.2.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/57/ab/6df7e24db51e1db642a5ea1759d44fb656251253995a27deb37af9b192ae/debugpy-1.8.1-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/d5/50/83c593b07763e1161326b3b8c6686f0f4b0f24d5526546bee538c89837d6/decorator-5.1.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/80/03/6ea8b1b2a5ab40a7a60dc464d3daa7aa546e0a74d74a9f8ff551ea7905db/executing-2.0.1-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/53/9d/40d5207db523363d9b5698f33778c18b0d591e3fdb6e0116b894b2a2491c/ipykernel-6.29.4-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/8a/15/ea245239487bbd8d7203fe010ea48c7539e42bf1fde0592313241a3fba3a/ipython-8.23.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/20/9f/bc63f0f0737ad7a60800bfd472a4836661adae21f9c2535f3957b1e54ceb/jedi-0.19.1-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/39/9d/b035d024c62c85f2e2d4806a59ca7b8520307f34e0932fbc8cc75fe7b2d9/jsonschema-4.21.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/ee/07/44bd408781594c4d0a027666ef27fab1e441b109dc3b76b4f836f8fd04fe/jsonschema_specifications-2023.12.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/75/6d/d7b55b9c1ac802ab066b3e5015e90faab1fffbbd67a2af498ffc6cc81c97/jupyter_client-8.6.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/c9/fb/108ecd1fe961941959ad0ee4e12ee7b8b1477247f30b1fdfd83ceaf017f0/jupyter_core-5.7.2-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/72/42/d57a938cad4e99bb799f35105561959b0a0550c65fbc1ed671196e27f909/jupyter_kernel_test-0.7.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/8f/8e/9ad090d3553c280a8060fbf6e24dc1c0c29704ee7d1c372f0c174aa59285/matplotlib_inline-0.1.7-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/0d/e6/5dd960a7678cbaf90dc910611a0e700775ee341876f029c3c987122afe84/msgspec-0.18.6-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
+      - pypi: https://files.pythonhosted.org/packages/a0/c4/c2971a3ba4c6103a3d10c4b0f24f461ddc027f0f09763220cf35ca1401b3/nest_asyncio-1.6.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/49/df/1fceb2f8900f8639e278b056416d49134fb8d84c5942ffaa01ad34782422/packaging-24.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/c6/ac/dac4a63f978e4dcb3c6d3a78c4d8e0192a113d288502a1216950c41b1027/parso-0.8.4-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/9e/c3/059298687310d527a58bb01f3b1965787ee3b40dce76752eda8b44e9a2c5/pexpect-4.9.0-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/55/72/4898c44ee9ea6f43396fbc23d9bfaf3d06e01b83698bdf2e4c919deceb7c/platformdirs-4.2.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/ee/fd/ca7bf3869e7caa7a037e23078539467b433a4e01eebd93f77180ab927766/prompt_toolkit-3.0.43-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/90/c7/6dc0a455d111f68ee43f27793971cf03fe29b6ef972042549db29eec39a2/psutil-5.9.8.tar.gz
+      - pypi: https://files.pythonhosted.org/packages/22/a6/858897256d0deac81a172289110f31629fc4cee19b6f01283303e18c8db3/ptyprocess-0.7.0-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/2b/27/77f9d5684e6bce929f5cfe18d6cfbe5133013c06cb2fbf5933670e60761d/pure_eval-0.2.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/97/9c/372fef8377a6e340b1704768d20daaded98bf13282b5327beb2e2fe2c7ef/pygments-2.17.2-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/ec/57/56b9bcc3c9c6a792fcbaf139543cee77261f3651ca9da0c93f5c1221264b/python_dateutil-2.9.0.post0-py2.py3-none-any.whl
-      - pypi: https://files.pythonhosted.org/packages/bc/4a/ac6469c01813cb3652ab4e30ec4a37815cc9949afc18af33f64e2ec704aa/pyzmq-25.1.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
+      - pypi: https://files.pythonhosted.org/packages/ce/18/a80c6a9a958643a95d2f4d0076cd8351e3ab4dd45cde475a800a1873a230/pyzmq-26.0.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
       - pypi: https://files.pythonhosted.org/packages/42/8e/ae1de7b12223986e949bdb886c004de7c304b6fa94de5b87c926c1099656/referencing-0.34.0-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/2a/3e/d2ef968eed02cfd9494d5bac0906bce830c4eb2cd27658303d3884e82e27/rpds_py-0.18.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
       - pypi: https://files.pythonhosted.org/packages/d9/5a/e7c31adbe875f2abbb91bd84cf2dc52d792b5a01506781dbcf25c91daf11/six-1.16.0-py2.py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/f1/7b/ce1eafaf1a76852e2ec9b22edecf1daa58175c090266e9f6c64afcd81d91/stack_data-0.6.3-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/62/e5/3ee2ba523a13bae5c17d1658580d13597116c1639374ca5033d58fd04724/tornado-6.4-cp38-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
       - pypi: https://files.pythonhosted.org/packages/7c/c4/366a09036c07f46eb8c9b2af39c97f502ef24f11f2a6e4d763655d9f2708/traitlets-5.14.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/01/f3/936e209267d6ef7510322191003885de524fc48d1b43269810cd589ceaf5/typing_extensions-4.11.0-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/fd/84/fd2ba7aafacbad3c4201d395674fc6348826569da3c0937e75505ead3528/wcwidth-0.2.13-py2.py3-none-any.whl
       - pypi: ../../../../pixi-kernel
 packages:
 - kind: conda
   name: _libgcc_mutex
   version: '0.1'
   build: conda_forge
   subdir: linux-64
@@ -196,14 +237,27 @@
   sha256: edac93a8e3beb9383abf508f66085505950bc89962116ef149558350a6213749
   md5: 18f0bdf689b6f345fecddbebaed945d6
   license: LGPL-2.0-or-later AND LGPL-2.0-or-later WITH exceptions AND GPL-2.0-or-later AND MPL-2.0
   license_family: GPL
   size: 21238
   timestamp: 1708000885951
 - kind: pypi
+  name: asttokens
+  version: 2.4.1
+  url: https://files.pythonhosted.org/packages/45/86/4736ac618d82a20d87d2f92ae19441ebc7ac9e7a581d7e58bbe79233b24a/asttokens-2.4.1-py2.py3-none-any.whl
+  sha256: 051ed49c3dcae8913ea7cd08e46a606dba30b79993209636c4875bc1d637bc24
+  requires_dist:
+  - six >=1.12.0
+  - typing ; python_version < '3.5'
+  - astroid <2, >=1 ; python_version < '3' and extra == 'astroid'
+  - astroid <4, >=2 ; python_version >= '3' and extra == 'astroid'
+  - pytest ; extra == 'test'
+  - astroid <2, >=1 ; python_version < '3' and extra == 'test'
+  - astroid <4, >=2 ; python_version >= '3' and extra == 'test'
+- kind: pypi
   name: attrs
   version: 23.2.0
   url: https://files.pythonhosted.org/packages/e0/44/827b2a91a5816512fcaf3cc4ebc465ccd5d598c45cefa6703fcf4a79018f/attrs-23.2.0-py3-none-any.whl
   sha256: 99b87a485a5820b23b879f04c2305b44b951b502fd64be915879d77a7e8fc6f1
   requires_dist:
   - importlib-metadata ; python_version < '3.8'
   - attrs[tests] ; extra == 'cov'
@@ -527,14 +581,23 @@
   - libzlib >=1.2.13,<1.3.0a0
   constrains:
   - gxx_linux-64 !=9.5.0
   - gxx_linux-64 !=9.5.0
   license: NCSA OR LGPL-2.1-only
   size: 25644297
   timestamp: 1667126412402
+- kind: pypi
+  name: comm
+  version: 0.2.2
+  url: https://files.pythonhosted.org/packages/e6/75/49e5bfe642f71f272236b5b2d2691cf915a7283cc0ceda56357b61daa538/comm-0.2.2-py3-none-any.whl
+  sha256: e6fb86cb70ff661ee8c9c14e7d36d6de3b4066f1441be4063df9c5009f0a64d3
+  requires_dist:
+  - traitlets >=4
+  - pytest ; extra == 'test'
+  requires_python: '>=3.8'
 - kind: conda
   name: cppzmq
   version: 4.8.1
   build: hef188df_0
   subdir: linux-aarch64
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/cppzmq-4.8.1-hef188df_0.tar.bz2
   sha256: a696a6031c9554829020040598f0255f2411cc8f9601b62d08de2a315696e5ac
@@ -573,14 +636,46 @@
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/cxxopts-2.1.2-hd62202e_1001.tar.bz2
   sha256: f2d1893a5b179ce7780e51ae1266712c274a1e0451e8fd080b6110864b5fb2e2
   md5: 2d43020b4f0f64a2ab6ce91d72e734b6
   license: MIT
   license_family: MIT
   size: 15005
   timestamp: 1609925664762
+- kind: pypi
+  name: debugpy
+  version: 1.8.1
+  url: https://files.pythonhosted.org/packages/3c/7a/e400d9f5ed6b4b5ec9f350b4d7974e986ca2d455221e567e648edfad898e/debugpy-1.8.1-cp312-cp312-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: a2e658a9630f27534e63922ebf655a6ab60c370f4d2fc5c02a5b19baf4410ace
+  requires_python: '>=3.8'
+- kind: pypi
+  name: debugpy
+  version: 1.8.1
+  url: https://files.pythonhosted.org/packages/57/ab/6df7e24db51e1db642a5ea1759d44fb656251253995a27deb37af9b192ae/debugpy-1.8.1-py2.py3-none-any.whl
+  sha256: 28acbe2241222b87e255260c76741e1fbf04fdc3b6d094fcf57b6c6f75ce1242
+  requires_python: '>=3.8'
+- kind: pypi
+  name: decorator
+  version: 5.1.1
+  url: https://files.pythonhosted.org/packages/d5/50/83c593b07763e1161326b3b8c6686f0f4b0f24d5526546bee538c89837d6/decorator-5.1.1-py3-none-any.whl
+  sha256: b8c3f85900b9dc423225913c5aace94729fe1fa9763b38939a95226f02d37186
+  requires_python: '>=3.5'
+- kind: pypi
+  name: executing
+  version: 2.0.1
+  url: https://files.pythonhosted.org/packages/80/03/6ea8b1b2a5ab40a7a60dc464d3daa7aa546e0a74d74a9f8ff551ea7905db/executing-2.0.1-py2.py3-none-any.whl
+  sha256: eac49ca94516ccc753f9fb5ce82603156e590b27525a8bc32cce8ae302eb61bc
+  requires_dist:
+  - asttokens >=2.1.0 ; extra == 'tests'
+  - ipython ; extra == 'tests'
+  - pytest ; extra == 'tests'
+  - coverage ; extra == 'tests'
+  - coverage-enable-subprocess ; extra == 'tests'
+  - littleutils ; extra == 'tests'
+  - rich ; python_version >= '3.11' and extra == 'tests'
+  requires_python: '>=3.5'
 - kind: conda
   name: gcc_impl_linux-64
   version: 10.4.0
   build: h5231bdf_19
   build_number: 19
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/gcc_impl_linux-64-10.4.0-h5231bdf_19.tar.bz2
@@ -720,14 +815,147 @@
   - gxx_impl_linux-aarch64 9.5.0.*
   - sysroot_linux-aarch64
   license: BSD-3-Clause
   license_family: BSD
   size: 28394
   timestamp: 1682618033164
 - kind: pypi
+  name: ipykernel
+  version: 6.29.4
+  url: https://files.pythonhosted.org/packages/53/9d/40d5207db523363d9b5698f33778c18b0d591e3fdb6e0116b894b2a2491c/ipykernel-6.29.4-py3-none-any.whl
+  sha256: 1181e653d95c6808039c509ef8e67c4126b3b3af7781496c7cbfb5ed938a27da
+  requires_dist:
+  - appnope ; platform_system == 'Darwin'
+  - comm >=0.1.1
+  - debugpy >=1.6.5
+  - ipython >=7.23.1
+  - jupyter-client >=6.1.12
+  - jupyter-core !=5.0.*, >=4.12
+  - matplotlib-inline >=0.1
+  - nest-asyncio
+  - packaging
+  - psutil
+  - pyzmq >=24
+  - tornado >=6.1
+  - traitlets >=5.4.0
+  - coverage[toml] ; extra == 'cov'
+  - curio ; extra == 'cov'
+  - matplotlib ; extra == 'cov'
+  - pytest-cov ; extra == 'cov'
+  - trio ; extra == 'cov'
+  - myst-parser ; extra == 'docs'
+  - pydata-sphinx-theme ; extra == 'docs'
+  - sphinx ; extra == 'docs'
+  - sphinx-autodoc-typehints ; extra == 'docs'
+  - sphinxcontrib-github-alt ; extra == 'docs'
+  - sphinxcontrib-spelling ; extra == 'docs'
+  - trio ; extra == 'docs'
+  - pyqt5 ; extra == 'pyqt5'
+  - pyside6 ; extra == 'pyside6'
+  - flaky ; extra == 'test'
+  - ipyparallel ; extra == 'test'
+  - pre-commit ; extra == 'test'
+  - pytest-asyncio >=0.23.5 ; extra == 'test'
+  - pytest-cov ; extra == 'test'
+  - pytest-timeout ; extra == 'test'
+  - pytest >=7.0 ; extra == 'test'
+  requires_python: '>=3.8'
+- kind: pypi
+  name: ipython
+  version: 8.23.0
+  url: https://files.pythonhosted.org/packages/8a/15/ea245239487bbd8d7203fe010ea48c7539e42bf1fde0592313241a3fba3a/ipython-8.23.0-py3-none-any.whl
+  sha256: 07232af52a5ba146dc3372c7bf52a0f890a23edf38d77caef8d53f9cdc2584c1
+  requires_dist:
+  - decorator
+  - jedi >=0.16
+  - matplotlib-inline
+  - prompt-toolkit <3.1.0, >=3.0.41
+  - pygments >=2.4.0
+  - stack-data
+  - traitlets >=5.13.0
+  - exceptiongroup ; python_version < '3.11'
+  - typing-extensions ; python_version < '3.12'
+  - pexpect >4.3 ; sys_platform != 'win32' and sys_platform != 'emscripten'
+  - colorama ; sys_platform == 'win32'
+  - ipython[black,doc,kernel,matplotlib,nbconvert,nbformat,notebook,parallel,qtconsole] ; extra == 'all'
+  - ipython[test,test-extra] ; extra == 'all'
+  - black ; extra == 'black'
+  - ipykernel ; extra == 'doc'
+  - setuptools >=18.5 ; extra == 'doc'
+  - sphinx >=1.3 ; extra == 'doc'
+  - sphinx-rtd-theme ; extra == 'doc'
+  - sphinxcontrib-jquery ; extra == 'doc'
+  - docrepr ; extra == 'doc'
+  - matplotlib ; extra == 'doc'
+  - stack-data ; extra == 'doc'
+  - typing-extensions ; extra == 'doc'
+  - exceptiongroup ; extra == 'doc'
+  - ipython[test] ; extra == 'doc'
+  - ipykernel ; extra == 'kernel'
+  - matplotlib ; extra == 'matplotlib'
+  - nbconvert ; extra == 'nbconvert'
+  - nbformat ; extra == 'nbformat'
+  - ipywidgets ; extra == 'notebook'
+  - notebook ; extra == 'notebook'
+  - ipyparallel ; extra == 'parallel'
+  - qtconsole ; extra == 'qtconsole'
+  - pytest <8 ; extra == 'test'
+  - pytest-asyncio <0.22 ; extra == 'test'
+  - testpath ; extra == 'test'
+  - pickleshare ; extra == 'test'
+  - ipython[test] ; extra == 'test_extra'
+  - curio ; extra == 'test_extra'
+  - matplotlib !=3.2.0 ; extra == 'test_extra'
+  - nbformat ; extra == 'test_extra'
+  - numpy >=1.23 ; extra == 'test_extra'
+  - pandas ; extra == 'test_extra'
+  - trio ; extra == 'test_extra'
+  requires_python: '>=3.10'
+- kind: pypi
+  name: jedi
+  version: 0.19.1
+  url: https://files.pythonhosted.org/packages/20/9f/bc63f0f0737ad7a60800bfd472a4836661adae21f9c2535f3957b1e54ceb/jedi-0.19.1-py2.py3-none-any.whl
+  sha256: e983c654fe5c02867aef4cdfce5a2fbb4a50adc0af145f70504238f18ef5e7e0
+  requires_dist:
+  - parso <0.9.0, >=0.8.3
+  - jinja2 ==2.11.3 ; extra == 'docs'
+  - markupsafe ==1.1.1 ; extra == 'docs'
+  - pygments ==2.8.1 ; extra == 'docs'
+  - alabaster ==0.7.12 ; extra == 'docs'
+  - babel ==2.9.1 ; extra == 'docs'
+  - chardet ==4.0.0 ; extra == 'docs'
+  - commonmark ==0.8.1 ; extra == 'docs'
+  - docutils ==0.17.1 ; extra == 'docs'
+  - future ==0.18.2 ; extra == 'docs'
+  - idna ==2.10 ; extra == 'docs'
+  - imagesize ==1.2.0 ; extra == 'docs'
+  - mock ==1.0.1 ; extra == 'docs'
+  - packaging ==20.9 ; extra == 'docs'
+  - pyparsing ==2.4.7 ; extra == 'docs'
+  - pytz ==2021.1 ; extra == 'docs'
+  - readthedocs-sphinx-ext ==2.1.4 ; extra == 'docs'
+  - recommonmark ==0.5.0 ; extra == 'docs'
+  - requests ==2.25.1 ; extra == 'docs'
+  - six ==1.15.0 ; extra == 'docs'
+  - snowballstemmer ==2.1.0 ; extra == 'docs'
+  - sphinx-rtd-theme ==0.4.3 ; extra == 'docs'
+  - sphinx ==1.8.5 ; extra == 'docs'
+  - sphinxcontrib-serializinghtml ==1.1.4 ; extra == 'docs'
+  - sphinxcontrib-websupport ==1.2.4 ; extra == 'docs'
+  - urllib3 ==1.26.4 ; extra == 'docs'
+  - flake8 ==5.0.4 ; extra == 'qa'
+  - mypy ==0.971 ; extra == 'qa'
+  - types-setuptools ==67.2.0.1 ; extra == 'qa'
+  - django ; extra == 'testing'
+  - attrs ; extra == 'testing'
+  - colorama ; extra == 'testing'
+  - docopt ; extra == 'testing'
+  - pytest <7.0.0 ; extra == 'testing'
+  requires_python: '>=3.6'
+- kind: pypi
   name: jsonschema
   version: 4.21.1
   url: https://files.pythonhosted.org/packages/39/9d/b035d024c62c85f2e2d4806a59ca7b8520307f34e0932fbc8cc75fe7b2d9/jsonschema-4.21.1-py3-none-any.whl
   sha256: 7996507afae316306f9e2290407761157c6f78002dcf7419acb99822143d1c6f
   requires_dist:
   - attrs >=22.2.0
   - importlib-resources >=1.4.0 ; python_version < '3.9'
@@ -1385,18 +1613,26 @@
   track_features:
   - cling
   license: Apache-2.0 WITH LLVM-exception
   license_family: Apache
   size: 40492509
   timestamp: 1642246495072
 - kind: pypi
+  name: matplotlib-inline
+  version: 0.1.7
+  url: https://files.pythonhosted.org/packages/8f/8e/9ad090d3553c280a8060fbf6e24dc1c0c29704ee7d1c372f0c174aa59285/matplotlib_inline-0.1.7-py3-none-any.whl
+  sha256: df192d39a4ff8f21b1895d72e6a13f5fcc5099f00fa84384e0ea28c2cc0653ca
+  requires_dist:
+  - traitlets
+  requires_python: '>=3.8'
+- kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/0d/e6/5dd960a7678cbaf90dc910611a0e700775ee341876f029c3c987122afe84/msgspec-0.18.6-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
-  sha256: c3232fabacef86fe8323cecbe99abbc5c02f7698e3f5f2e248e3480b66a3596b
+  url: https://files.pythonhosted.org/packages/73/16/dfef780ced7d690dd5497846ed242ef3e27e319d59d1ddaae816a4f2c15e/msgspec-0.18.6-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: ad237100393f637b297926cae1868b0d500f764ccd2f0623a380e2bcfb2809ca
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -1426,16 +1662,16 @@
   - tomli-w ; extra == 'toml'
   - tomli ; python_version < '3.11' and extra == 'toml'
   - pyyaml ; extra == 'yaml'
   requires_python: '>=3.8'
 - kind: pypi
   name: msgspec
   version: 0.18.6
-  url: https://files.pythonhosted.org/packages/73/16/dfef780ced7d690dd5497846ed242ef3e27e319d59d1ddaae816a4f2c15e/msgspec-0.18.6-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: ad237100393f637b297926cae1868b0d500f764ccd2f0623a380e2bcfb2809ca
+  url: https://files.pythonhosted.org/packages/0d/e6/5dd960a7678cbaf90dc910611a0e700775ee341876f029c3c987122afe84/msgspec-0.18.6-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
+  sha256: c3232fabacef86fe8323cecbe99abbc5c02f7698e3f5f2e248e3480b66a3596b
   requires_dist:
   - pre-commit ; extra == 'dev'
   - coverage ; extra == 'dev'
   - gcovr ; extra == 'dev'
   - sphinx ; extra == 'dev'
   - furo ; extra == 'dev'
   - sphinx-copybutton ; extra == 'dev'
@@ -1488,14 +1724,20 @@
   sha256: aa0f005b6727aac6507317ed490f0904430584fa8ca722657e7f0fb94741de81
   md5: 97da8860a0da5413c7c98a3b3838a645
   depends:
   - libgcc-ng >=12
   license: X11 AND BSD-3-Clause
   size: 895669
   timestamp: 1710866638986
+- kind: pypi
+  name: nest-asyncio
+  version: 1.6.0
+  url: https://files.pythonhosted.org/packages/a0/c4/c2971a3ba4c6103a3d10c4b0f24f461ddc027f0f09763220cf35ca1401b3/nest_asyncio-1.6.0-py3-none-any.whl
+  sha256: 87af6efd6b5e897c81050477ef65c62e2b2f35d51703cae01aff2905b1852e1c
+  requires_python: '>=3.5'
 - kind: conda
   name: nlohmann_json
   version: 3.9.1
   build: h01db608_1
   build_number: 1
   subdir: linux-aarch64
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/nlohmann_json-3.9.1-h01db608_1.tar.bz2
@@ -1547,19 +1789,45 @@
   constrains:
   - pyopenssl >=22.1
   license: Apache-2.0
   license_family: Apache
   size: 2865379
   timestamp: 1710793235846
 - kind: pypi
+  name: packaging
+  version: '24.0'
+  url: https://files.pythonhosted.org/packages/49/df/1fceb2f8900f8639e278b056416d49134fb8d84c5942ffaa01ad34782422/packaging-24.0-py3-none-any.whl
+  sha256: 2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5
+  requires_python: '>=3.7'
+- kind: pypi
+  name: parso
+  version: 0.8.4
+  url: https://files.pythonhosted.org/packages/c6/ac/dac4a63f978e4dcb3c6d3a78c4d8e0192a113d288502a1216950c41b1027/parso-0.8.4-py2.py3-none-any.whl
+  sha256: a418670a20291dacd2dddc80c377c5c3791378ee1e8d12bffc35420643d43f18
+  requires_dist:
+  - flake8 ==5.0.4 ; extra == 'qa'
+  - mypy ==0.971 ; extra == 'qa'
+  - types-setuptools ==67.2.0.1 ; extra == 'qa'
+  - docopt ; extra == 'testing'
+  - pytest ; extra == 'testing'
+  requires_python: '>=3.6'
+- kind: pypi
+  name: pexpect
+  version: 4.9.0
+  url: https://files.pythonhosted.org/packages/9e/c3/059298687310d527a58bb01f3b1965787ee3b40dce76752eda8b44e9a2c5/pexpect-4.9.0-py2.py3-none-any.whl
+  sha256: 7236d1e080e4936be2dc3e326cec0af72acf9212a7e1d060210e70a47e253523
+  requires_dist:
+  - ptyprocess >=0.5
+- kind: pypi
   name: pixi-kernel
-  version: 0.2.1
+  version: 0.3.0
   path: ../../../../pixi-kernel
-  sha256: fc89be37749334e0eb20e8656e5ffcdace662e69fd273fa798213fdf1e64b7cb
+  sha256: 026726c0f08b63327906964394fdaf6d1b2324c25bf50c37e37b0300731fba40
   requires_dist:
+  - ipykernel >=6
   - jupyter-client >=7
   - msgspec >=0.18
   requires_python: <4.0,>=3.8
   editable: true
 - kind: pypi
   name: platformdirs
   version: 4.2.0
@@ -1572,14 +1840,51 @@
   - sphinx >=7.2.6 ; extra == 'docs'
   - appdirs ==1.4.4 ; extra == 'test'
   - covdefaults >=2.3 ; extra == 'test'
   - pytest-cov >=4.1 ; extra == 'test'
   - pytest-mock >=3.12 ; extra == 'test'
   - pytest >=7.4.3 ; extra == 'test'
   requires_python: '>=3.8'
+- kind: pypi
+  name: prompt-toolkit
+  version: 3.0.43
+  url: https://files.pythonhosted.org/packages/ee/fd/ca7bf3869e7caa7a037e23078539467b433a4e01eebd93f77180ab927766/prompt_toolkit-3.0.43-py3-none-any.whl
+  sha256: a11a29cb3bf0a28a387fe5122cdb649816a957cd9261dcedf8c9f1fef33eacf6
+  requires_dist:
+  - wcwidth
+  requires_python: '>=3.7.0'
+- kind: pypi
+  name: psutil
+  version: 5.9.8
+  url: https://files.pythonhosted.org/packages/c5/4f/0e22aaa246f96d6ac87fe5ebb9c5a693fbe8877f537a1022527c47ca43c5/psutil-5.9.8-cp36-abi3-manylinux_2_12_x86_64.manylinux2010_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: d06016f7f8625a1825ba3732081d77c94589dca78b7a3fc072194851e88461a4
+  requires_dist:
+  - ipaddress ; python_version < '3.0' and extra == 'test'
+  - mock ; python_version < '3.0' and extra == 'test'
+  - enum34 ; python_version <= '3.4' and extra == 'test'
+  - pywin32 ; sys_platform == 'win32' and extra == 'test'
+  - wmi ; sys_platform == 'win32' and extra == 'test'
+  requires_python: '>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*'
+- kind: pypi
+  name: psutil
+  version: 5.9.8
+  url: https://files.pythonhosted.org/packages/90/c7/6dc0a455d111f68ee43f27793971cf03fe29b6ef972042549db29eec39a2/psutil-5.9.8.tar.gz
+  sha256: 6be126e3225486dff286a8fb9a06246a5253f4c7c53b475ea5f5ac934e64194c
+  requires_dist:
+  - ipaddress ; python_version < '3.0' and extra == 'test'
+  - mock ; python_version < '3.0' and extra == 'test'
+  - enum34 ; python_version <= '3.4' and extra == 'test'
+  - pywin32 ; sys_platform == 'win32' and extra == 'test'
+  - wmi ; sys_platform == 'win32' and extra == 'test'
+  requires_python: '>=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*'
+- kind: pypi
+  name: ptyprocess
+  version: 0.7.0
+  url: https://files.pythonhosted.org/packages/22/a6/858897256d0deac81a172289110f31629fc4cee19b6f01283303e18c8db3/ptyprocess-0.7.0-py2.py3-none-any.whl
+  sha256: 4b41f3967fce3af57cc7e94b888626c18bf37a083e3651ca8feeb66d492fef35
 - kind: conda
   name: pugixml
   version: 1.11.4
   build: h2f0025b_1
   build_number: 1
   subdir: linux-aarch64
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/pugixml-1.11.4-h2f0025b_1.conda
@@ -1603,14 +1908,30 @@
   depends:
   - libgcc-ng >=12
   - libstdcxx-ng >=12
   license: MIT
   license_family: MIT
   size: 114871
   timestamp: 1696182708943
+- kind: pypi
+  name: pure-eval
+  version: 0.2.2
+  url: https://files.pythonhosted.org/packages/2b/27/77f9d5684e6bce929f5cfe18d6cfbe5133013c06cb2fbf5933670e60761d/pure_eval-0.2.2-py3-none-any.whl
+  sha256: 01eaab343580944bc56080ebe0a674b39ec44a945e6d09ba7db3cb8cec289350
+  requires_dist:
+  - pytest ; extra == 'tests'
+- kind: pypi
+  name: pygments
+  version: 2.17.2
+  url: https://files.pythonhosted.org/packages/97/9c/372fef8377a6e340b1704768d20daaded98bf13282b5327beb2e2fe2c7ef/pygments-2.17.2-py3-none-any.whl
+  sha256: b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c
+  requires_dist:
+  - importlib-metadata ; python_version < '3.8' and extra == 'plugins'
+  - colorama >=0.4.6 ; extra == 'windows-terminal'
+  requires_python: '>=3.7'
 - kind: conda
   name: python
   version: 3.11.0
   build: h38d2e7a_1_cpython
   build_number: 1
   subdir: linux-aarch64
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/python-3.11.0-h38d2e7a_1_cpython.conda
@@ -1634,66 +1955,66 @@
   constrains:
   - python_abi 3.11.* *_cp311
   license: Python-2.0
   size: 15269246
   timestamp: 1673672637174
 - kind: conda
   name: python
-  version: 3.12.2
+  version: 3.12.3
   build: hab00c5b_0_cpython
   subdir: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.2-hab00c5b_0_cpython.conda
-  sha256: ddb7a2d8d78046bda5d7631e6814f9468d2eb054e10f86f4648c9d1fdaa30c0f
-  md5: ad7b68400f3a6ebe72b00be093c7f301
+  url: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda
+  sha256: f9865bcbff69f15fd89a33a2da12ad616e98d65ce7c83c644b92e66e5016b227
+  md5: 2540b74d304f71d3e89c81209db4db84
   depends:
   - bzip2 >=1.0.8,<2.0a0
   - ld_impl_linux-64 >=2.36.1
-  - libexpat >=2.5.0,<3.0a0
+  - libexpat >=2.6.2,<3.0a0
   - libffi >=3.4,<4.0a0
   - libgcc-ng >=12
   - libnsl >=2.0.1,<2.1.0a0
-  - libsqlite >=3.45.1,<4.0a0
+  - libsqlite >=3.45.2,<4.0a0
   - libuuid >=2.38.1,<3.0a0
   - libxcrypt >=4.4.36
   - libzlib >=1.2.13,<1.3.0a0
-  - ncurses >=6.4,<7.0a0
+  - ncurses >=6.4.20240210,<7.0a0
   - openssl >=3.2.1,<4.0a0
   - readline >=8.2,<9.0a0
   - tk >=8.6.13,<8.7.0a0
   - tzdata
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.12.* *_cp312
   license: Python-2.0
-  size: 32312631
-  timestamp: 1708118077305
+  size: 31991381
+  timestamp: 1713208036041
 - kind: pypi
   name: python-dateutil
   version: 2.9.0.post0
   url: https://files.pythonhosted.org/packages/ec/57/56b9bcc3c9c6a792fcbaf139543cee77261f3651ca9da0c93f5c1221264b/python_dateutil-2.9.0.post0-py2.py3-none-any.whl
   sha256: a8b2bc7bffae282281c8140a97d3aa9c14da0b136dfe83f850eea9a5f7470427
   requires_dist:
   - six >=1.5
   requires_python: '!=3.0.*,!=3.1.*,!=3.2.*,>=2.7'
 - kind: pypi
   name: pyzmq
-  version: 25.1.2
-  url: https://files.pythonhosted.org/packages/bc/4a/ac6469c01813cb3652ab4e30ec4a37815cc9949afc18af33f64e2ec704aa/pyzmq-25.1.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
-  sha256: bc69c96735ab501419c432110016329bf0dea8898ce16fab97c6d9106dc0b348
+  version: 26.0.0
+  url: https://files.pythonhosted.org/packages/61/01/eb6165d9160065845179f8f168ea70eaa24aa7e63f53b13966bbe368d6fa/pyzmq-26.0.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: af9f5b1b76753584c871c1c96db8a18650886b3adf9fc8c7d4019343eb329c28
   requires_dist:
   - cffi ; implementation_name == 'pypy'
-  requires_python: '>=3.6'
+  requires_python: '>=3.7'
 - kind: pypi
   name: pyzmq
-  version: 25.1.2
-  url: https://files.pythonhosted.org/packages/93/b7/6e291eafbbbc66d0e87658dd21383ec2b4ab35edcfb283902c580a6db76f/pyzmq-25.1.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: 02c9087b109070c5ab0b383079fa1b5f797f8d43e9a66c07a4b8b8bdecfd88ee
+  version: 26.0.0
+  url: https://files.pythonhosted.org/packages/ce/18/a80c6a9a958643a95d2f4d0076cd8351e3ab4dd45cde475a800a1873a230/pyzmq-26.0.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
+  sha256: 8a5b4dc4d7a3f859026083906724ad1ae743261548b61d0d5abcf2d994122c2b
   requires_dist:
   - cffi ; implementation_name == 'pypy'
-  requires_python: '>=3.6'
+  requires_python: '>=3.7'
 - kind: conda
   name: readline
   version: '8.2'
   build: h8228510_1
   build_number: 1
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
@@ -1730,29 +2051,43 @@
   requires_dist:
   - attrs >=22.2.0
   - rpds-py >=0.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
-  url: https://files.pythonhosted.org/packages/2a/3e/d2ef968eed02cfd9494d5bac0906bce830c4eb2cd27658303d3884e82e27/rpds_py-0.18.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
-  sha256: fcb25daa9219b4cf3a0ab24b0eb9a5cc8949ed4dc72acb8fa16b7e1681aa3c58
+  url: https://files.pythonhosted.org/packages/c3/96/2211a1ca4b4e259e222169074ec0fa41f0ee18665dfc68988a139dc7e6e8/rpds_py-0.18.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: 4457a94da0d5c53dc4b3e4de1158bdab077db23c53232f37a3cb7afdb053a4e3
   requires_python: '>=3.8'
 - kind: pypi
   name: rpds-py
   version: 0.18.0
-  url: https://files.pythonhosted.org/packages/c3/96/2211a1ca4b4e259e222169074ec0fa41f0ee18665dfc68988a139dc7e6e8/rpds_py-0.18.0-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: 4457a94da0d5c53dc4b3e4de1158bdab077db23c53232f37a3cb7afdb053a4e3
+  url: https://files.pythonhosted.org/packages/2a/3e/d2ef968eed02cfd9494d5bac0906bce830c4eb2cd27658303d3884e82e27/rpds_py-0.18.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
+  sha256: fcb25daa9219b4cf3a0ab24b0eb9a5cc8949ed4dc72acb8fa16b7e1681aa3c58
   requires_python: '>=3.8'
 - kind: pypi
   name: six
   version: 1.16.0
   url: https://files.pythonhosted.org/packages/d9/5a/e7c31adbe875f2abbb91bd84cf2dc52d792b5a01506781dbcf25c91daf11/six-1.16.0-py2.py3-none-any.whl
   sha256: 8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
   requires_python: '>=2.7,!=3.0.*,!=3.1.*,!=3.2.*'
+- kind: pypi
+  name: stack-data
+  version: 0.6.3
+  url: https://files.pythonhosted.org/packages/f1/7b/ce1eafaf1a76852e2ec9b22edecf1daa58175c090266e9f6c64afcd81d91/stack_data-0.6.3-py3-none-any.whl
+  sha256: d5558e0c25a4cb0853cddad3d77da9891a08cb85dd9f9f91b9f8cd66e511e695
+  requires_dist:
+  - executing >=1.2.0
+  - asttokens >=2.1.0
+  - pure-eval
+  - pytest ; extra == 'tests'
+  - typeguard ; extra == 'tests'
+  - pygments ; extra == 'tests'
+  - littleutils ; extra == 'tests'
+  - cython ; extra == 'tests'
 - kind: conda
   name: sysroot_linux-64
   version: '2.12'
   build: he073ed8_17
   build_number: 17
   subdir: noarch
   noarch: generic
@@ -1812,22 +2147,22 @@
   license: TCL
   license_family: BSD
   size: 3318875
   timestamp: 1699202167581
 - kind: pypi
   name: tornado
   version: '6.4'
-  url: https://files.pythonhosted.org/packages/62/e5/3ee2ba523a13bae5c17d1658580d13597116c1639374ca5033d58fd04724/tornado-6.4-cp38-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
-  sha256: f7894c581ecdcf91666a0912f18ce5e757213999e183ebfc2c3fdbf4d5bd764e
+  url: https://files.pythonhosted.org/packages/9f/12/11d0a757bb67278d3380d41955ae98527d5ad18330b2edbdc8de222b569b/tornado-6.4-cp38-abi3-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: f0251554cdd50b4b44362f73ad5ba7126fc5b2c2895cc62b14a1c2d7ea32f212
   requires_python: '>=3.8'
 - kind: pypi
   name: tornado
   version: '6.4'
-  url: https://files.pythonhosted.org/packages/9f/12/11d0a757bb67278d3380d41955ae98527d5ad18330b2edbdc8de222b569b/tornado-6.4-cp38-abi3-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: f0251554cdd50b4b44362f73ad5ba7126fc5b2c2895cc62b14a1c2d7ea32f212
+  url: https://files.pythonhosted.org/packages/62/e5/3ee2ba523a13bae5c17d1658580d13597116c1639374ca5033d58fd04724/tornado-6.4-cp38-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl
+  sha256: f7894c581ecdcf91666a0912f18ce5e757213999e183ebfc2c3fdbf4d5bd764e
   requires_python: '>=3.8'
 - kind: pypi
   name: traitlets
   version: 5.14.2
   url: https://files.pythonhosted.org/packages/7c/c4/366a09036c07f46eb8c9b2af39c97f502ef24f11f2a6e4d763655d9f2708/traitlets-5.14.2-py3-none-any.whl
   sha256: fcdf85684a772ddeba87db2f398ce00b40ff550d1528c03c14dbf6a02003cd80
   requires_dist:
@@ -1837,26 +2172,39 @@
   - argcomplete >=3.0.3 ; extra == 'test'
   - mypy >=1.7.0 ; extra == 'test'
   - pre-commit ; extra == 'test'
   - pytest-mock ; extra == 'test'
   - pytest-mypy-testing ; extra == 'test'
   - pytest <8.1, >=7.0 ; extra == 'test'
   requires_python: '>=3.8'
+- kind: pypi
+  name: typing-extensions
+  version: 4.11.0
+  url: https://files.pythonhosted.org/packages/01/f3/936e209267d6ef7510322191003885de524fc48d1b43269810cd589ceaf5/typing_extensions-4.11.0-py3-none-any.whl
+  sha256: c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
+  requires_python: '>=3.8'
 - kind: conda
   name: tzdata
   version: 2024a
   build: h0c530f3_0
   subdir: noarch
   noarch: generic
   url: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
   sha256: 7b2b69c54ec62a243eb6fba2391b5e443421608c3ae5dbff938ad33ca8db5122
   md5: 161081fc7cec0bfda0d86d7cb595f8d8
   license: LicenseRef-Public-Domain
   size: 119815
   timestamp: 1706886945727
+- kind: pypi
+  name: wcwidth
+  version: 0.2.13
+  url: https://files.pythonhosted.org/packages/fd/84/fd2ba7aafacbad3c4201d395674fc6348826569da3c0937e75505ead3528/wcwidth-0.2.13-py2.py3-none-any.whl
+  sha256: 3da69048e4540d84af32131829ff948f1e022c1c6bdb8d6102117aac784f6859
+  requires_dist:
+  - backports-functools-lru-cache >=1.2.1 ; python_version < '3.2'
 - kind: conda
   name: xeus
   version: 2.4.1
   build: h68f4542_0
   subdir: linux-aarch64
   url: https://conda.anaconda.org/conda-forge/linux-aarch64/xeus-2.4.1-h68f4542_0.tar.bz2
   sha256: 1196721dfa80e18e1ad2690ad11ab95ee7f6c101abfc3d242312f86727326cf1
```

### Comparing `pixi_kernel-0.2.1/tests/unit/conftest.py` & `pixi_kernel-0.3.0/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.1/LICENSE` & `pixi_kernel-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.1/README.md` & `pixi_kernel-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pixi_kernel-0.2.1/pyproject.toml` & `pixi_kernel-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pixi-kernel"
-version = "0.2.1"
+version = "0.3.0"
 description = "Jupyter kernels using Pixi for reproducible notebooks"
 license = { text = "MIT" }
 authors = [
     { name = "Renan Rodrigues dos Santos", email = "renan.engmec@gmail.com" },
 ]
 
 readme = "README.md"
@@ -26,15 +26,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Typing :: Typed",
 ]
 
 requires-python = ">=3.8,<4.0"
-dependencies = ["jupyter-client>=7", "msgspec>=0.18"]
+dependencies = ["ipykernel>=6", "jupyter-client>=7", "msgspec>=0.18"]
 
 [project.urls]
 Documentation = "https://github.com/renan-r-santos/pixi-kernel"
 Homepage = "https://github.com/renan-r-santos/pixi-kernel"
 Repository = "https://github.com/renan-r-santos/pixi-kernel"
 
 [project.entry-points."jupyter_client.kernel_provisioners"]
@@ -54,14 +54,17 @@
     "C4", # flake8-comprehensions
     "PIE", # flake8-pie
     "PT", # flake8-pytest-style
     "PTH", # flake8-use-pathlib
     "ERA", # flake8-eradicate
 ]
 
+[tool.mypy]
+strict = true
+
 [tool.pytest.ini_options]
 addopts = ["--strict-config", "--strict-markers"]
 xfail_strict = true
 filterwarnings = [
     "error",
     "ignore:Jupyter is migrating its paths to use standard platformdirs",
 ]
```

### Comparing `pixi_kernel-0.2.1/PKG-INFO` & `pixi_kernel-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pixi-kernel
-Version: 0.2.1
+Version: 0.3.0
 Summary: Jupyter kernels using Pixi for reproducible notebooks
 Project-URL: Documentation, https://github.com/renan-r-santos/pixi-kernel
 Project-URL: Homepage, https://github.com/renan-r-santos/pixi-kernel
 Project-URL: Repository, https://github.com/renan-r-santos/pixi-kernel
 Author-email: Renan Rodrigues dos Santos <renan.engmec@gmail.com>
 License: MIT
 License-File: LICENSE
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: <4.0,>=3.8
+Requires-Dist: ipykernel>=6
 Requires-Dist: jupyter-client>=7
 Requires-Dist: msgspec>=0.18
 Description-Content-Type: text/markdown
 
 # Pixi Kernel
 
 [![Pixi Badge][pixi-badge]](https://pixi.sh)
```

