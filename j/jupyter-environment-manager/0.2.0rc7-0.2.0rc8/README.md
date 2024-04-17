# Comparing `tmp/jupyter_environment_manager-0.2.0rc7.tar.gz` & `tmp/jupyter_environment_manager-0.2.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter_environment_manager-0.2.0rc7.tar", last modified: Wed Mar 27 21:58:10 2024, max compression
+gzip compressed data, was "jupyter_environment_manager-0.2.0rc8.tar", last modified: Wed Apr 17 16:41:04 2024, max compression
```

## Comparing `jupyter_environment_manager-0.2.0rc7.tar` & `jupyter_environment_manager-0.2.0rc8.tar`

### file list

```diff
@@ -1,128 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:58:10.850049 jupyter_environment_manager-0.2.0rc7/
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-03-27 21:58:10.850049 jupyter_environment_manager-0.2.0rc7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/install.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:58:10.802049 jupyter_environment_manager-0.2.0rc7/jupyter-config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:58:10.810049 jupyter_environment_manager-0.2.0rc7/jupyter-config/nb-config/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/jupyter-config/nb-config/jupyter_environment_manager.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:58:10.810049 jupyter_environment_manager-0.2.0rc7/jupyter-config/server-config/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/jupyter-config/server-config/jupyter_environment_manager.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:58:10.818049 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/envs_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    11501 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/envs_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/envs_pkgs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/envs_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/envs_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/kernels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:58:10.818049 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:58:10.830049 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (127)    94749 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/0.99dd872e735721a05b18.js
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/0.99dd872e735721a05b18.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17291 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/113.063bb6057d77be1f85f3.js
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/113.063bb6057d77be1f85f3.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/151.18af1747c52fa1890fce.js
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/174.7b162c87cb727f7c2712.js
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/174.7b162c87cb727f7c2712.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   195750 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/185.4cb0a9019311d36636ce.js
--rw-r--r--   0 runner    (1001) docker     (127)  3944216 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/24.a6fec73552ceb9bdb6aa.js
--rw-r--r--   0 runner    (1001) docker     (127)   300035 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11262 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/378.8fdd4b1246fb17037bb3.js
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/478.b1efc8dc1ed4a16150ef.js
--rw-r--r--   0 runner    (1001) docker     (127)    22112 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/554.3ee5e631ee6f4d8c24e2.js
--rw-r--r--   0 runner    (1001) docker     (127)    22640 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/569.110780388cdcc5605903.js
--rw-r--r--   0 runner    (1001) docker     (127)    37522 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/588.634556691591dc1dac9b.js
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/588.634556691591dc1dac9b.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    37522 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/66.715eff54360a4988967a.js
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/66.715eff54360a4988967a.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/697.61315fde7050f7a02689.js
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/747.6d49dfe38d298a9d88e1.js
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/813.4baf0234297462c92d8b.js
--rw-r--r--   0 runner    (1001) docker     (127)   454999 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/909.c50074d4e4be5aa7c06a.js
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/909.c50074d4e4be5aa7c06a.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   446062 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/991.b0c652da28634799e4d5.js
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/remoteEntry.efb45905ee8f674ba5f4.js
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-27 21:57:17.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (127)   509524 2024-03-27 21:58:04.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/qbraid_core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:58:10.850049 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-03-27 21:58:10.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-03-27 21:58:10.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 21:58:10.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 21:56:57.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-27 21:58:10.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-27 21:58:10.000000 jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-03-27 21:56:40.000000 jupyter_environment_manager-0.2.0rc7/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 21:58:10.850049 jupyter_environment_manager-0.2.0rc7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:58:10.834049 jupyter_environment_manager-0.2.0rc7/src/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/EnvironmentsSidebarWidget.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/Flux.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:58:10.838049 jupyter_environment_manager-0.2.0rc7/src/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/actions/ApiActions.js
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/actions/AuthActions.js
--rw-r--r--   0 runner    (1001) docker     (127)    28134 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/actions/EnvironmentActions.js
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/actions/JupyterApiActions.js
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/actions/UserActions.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:58:10.802049 jupyter_environment_manager-0.2.0rc7/src/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:58:10.842049 jupyter_environment_manager-0.2.0rc7/src/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/assets/icons/BackIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/assets/icons/CloseIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/assets/icons/ConfirmIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/assets/icons/DescriptionIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/assets/icons/EnvIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/assets/icons/IconString.js
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/assets/icons/LinkIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/assets/icons/Loading.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/assets/icons/RefreshIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/assets/icons/SearchIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/assets/icons/UserIcon.tsx
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/assets/icons/WhiteCube.tsx
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/assets.d.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:58:10.846049 jupyter_environment_manager-0.2.0rc7/src/components/
--rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/components/EndUserAgreement.js
--rw-r--r--   0 runner    (1001) docker     (127)    96989 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/components/EnvironmentEditor.js
--rw-r--r--   0 runner    (1001) docker     (127)    13092 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/components/EnvironmentTile.js
--rw-r--r--   0 runner    (1001) docker     (127)    96111 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/components/EnvironmentsSidebar.js
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/components/Loading.js
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/components/LogoLoader.js
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/components/MuiStyledComponents.js
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/components/UserNotFound.js
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/contextTypes.js
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/global.d.ts
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:58:10.846049 jupyter_environment_manager-0.2.0rc7/src/stores/
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/stores/AuthStore.js
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/stores/EnvironmentStore.js
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/stores/UserStore.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:58:10.846049 jupyter_environment_manager-0.2.0rc7/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/utils/googleAnalytics.js
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/src/utils/theme.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:58:10.850049 jupyter_environment_manager-0.2.0rc7/style/
--rw-r--r--   0 runner    (1001) docker     (127)    19395 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/style/EnvironmentEditor.css
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/style/EnvironmentTile.css
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/style/EnvironmentsSidebar.css
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/style/Loading.css
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/style/LogoLoader.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/style/base.css
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/style/index.css
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/style/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:58:10.850049 jupyter_environment_manager-0.2.0rc7/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/tools/create_dev_build.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     3841 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/tools/stamp_pre_release.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)   607255 2024-03-27 21:55:53.000000 jupyter_environment_manager-0.2.0rc7/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:04.020308 jupyter_environment_manager-0.2.0rc8/
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-17 16:41:04.020308 jupyter_environment_manager-0.2.0rc8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/install.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:03.968308 jupyter_environment_manager-0.2.0rc8/jupyter-config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:03.976308 jupyter_environment_manager-0.2.0rc8/jupyter-config/nb-config/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter-config/nb-config/jupyter_environment_manager.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:03.976308 jupyter_environment_manager-0.2.0rc8/jupyter-config/server-config/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter-config/server-config/jupyter_environment_manager.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:03.980308 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/envs_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/envs_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/envs_pkgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/envs_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/envs_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/kernels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:03.980308 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:03.996308 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    94749 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/0.99dd872e735721a05b18.js
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/0.99dd872e735721a05b18.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17291 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/113.063bb6057d77be1f85f3.js
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/113.063bb6057d77be1f85f3.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/151.18af1747c52fa1890fce.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/174.7b162c87cb727f7c2712.js
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/174.7b162c87cb727f7c2712.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   195536 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/185.5d7f6d37c97924a89805.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3944216 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/24.a6fec73552ceb9bdb6aa.js
+-rw-r--r--   0 runner    (1001) docker     (127)   300035 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11262 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/378.8fdd4b1246fb17037bb3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/478.b1efc8dc1ed4a16150ef.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22112 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/554.3ee5e631ee6f4d8c24e2.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22640 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/569.110780388cdcc5605903.js
+-rw-r--r--   0 runner    (1001) docker     (127)    37522 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/588.634556691591dc1dac9b.js
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/588.634556691591dc1dac9b.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    37522 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/66.715eff54360a4988967a.js
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/66.715eff54360a4988967a.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/697.61315fde7050f7a02689.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/747.6d49dfe38d298a9d88e1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/813.4baf0234297462c92d8b.js
+-rw-r--r--   0 runner    (1001) docker     (127)   454999 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/909.c50074d4e4be5aa7c06a.js
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/909.c50074d4e4be5aa7c06a.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   446062 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/991.b0c652da28634799e4d5.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/remoteEntry.64b15d2280d9c5210de7.js
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-17 16:40:13.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (127)   509524 2024-04-17 16:40:59.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:04.020308 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-17 16:41:03.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-17 16:41:03.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:41:03.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 16:38:28.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-17 16:41:03.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-17 16:41:03.000000 jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-17 16:38:16.000000 jupyter_environment_manager-0.2.0rc8/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 16:41:04.020308 jupyter_environment_manager-0.2.0rc8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:04.000308 jupyter_environment_manager-0.2.0rc8/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/EnvironmentsSidebarWidget.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/Flux.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:04.000308 jupyter_environment_manager-0.2.0rc8/src/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/actions/ApiActions.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/actions/AuthActions.js
+-rw-r--r--   0 runner    (1001) docker     (127)    28082 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/actions/EnvironmentActions.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/actions/JupyterApiActions.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/actions/UserActions.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:03.968308 jupyter_environment_manager-0.2.0rc8/src/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:04.004308 jupyter_environment_manager-0.2.0rc8/src/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets/icons/BackIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets/icons/CloseIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets/icons/ConfirmIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets/icons/DescriptionIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets/icons/EnvIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets/icons/IconString.js
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets/icons/LinkIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets/icons/Loading.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets/icons/RefreshIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets/icons/SearchIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets/icons/UserIcon.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets/icons/WhiteCube.tsx
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/assets.d.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:04.008308 jupyter_environment_manager-0.2.0rc8/src/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/components/EndUserAgreement.js
+-rw-r--r--   0 runner    (1001) docker     (127)    97122 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/components/EnvironmentEditor.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13092 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/components/EnvironmentTile.js
+-rw-r--r--   0 runner    (1001) docker     (127)    96041 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/components/EnvironmentsSidebar.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/components/Loading.js
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/components/LogoLoader.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/components/MuiStyledComponents.js
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/components/UserNotFound.js
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/contextTypes.js
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/global.d.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:04.012308 jupyter_environment_manager-0.2.0rc8/src/stores/
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/stores/AuthStore.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/stores/EnvironmentStore.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/stores/UserStore.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:04.012308 jupyter_environment_manager-0.2.0rc8/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/utils/googleAnalytics.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/src/utils/theme.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:04.016308 jupyter_environment_manager-0.2.0rc8/style/
+-rw-r--r--   0 runner    (1001) docker     (127)    19395 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/style/EnvironmentEditor.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/style/EnvironmentTile.css
+-rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/style/EnvironmentsSidebar.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/style/Loading.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/style/LogoLoader.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/style/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 16:41:04.020308 jupyter_environment_manager-0.2.0rc8/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/tools/create_dev_build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3841 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/tools/stamp_pre_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)   607255 2024-04-17 16:37:50.000000 jupyter_environment_manager-0.2.0rc8/yarn.lock
```

### Comparing `jupyter_environment_manager-0.2.0rc7/CONTRIBUTING.md` & `jupyter_environment_manager-0.2.0rc8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/LICENSE` & `jupyter_environment_manager-0.2.0rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/MANIFEST.in` & `jupyter_environment_manager-0.2.0rc8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/PKG-INFO` & `jupyter_environment_manager-0.2.0rc8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_environment_manager
-Version: 0.2.0rc7
+Version: 0.2.0rc8
 Summary: JupyterLab extension for managing execution environments, packages, and kernels.
 Home-page: https://github.com/qBraid/qBraid-Lab
 Author: qBraid Development Team
 Author-email: contact@qbraid.com
 License: Proprietary
 Project-URL: Documentation, https://docs.qbraid.com/projects/lab/en/latest/lab/environments.html
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
@@ -29,15 +29,15 @@
 Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jupyter_server<2,>=1.6
 Requires-Dist: jupyter_client~=7.1.0
 Requires-Dist: tornado>=6.1.0
 Requires-Dist: notebook<7
-Requires-Dist: qbraid-cli
+Requires-Dist: qbraid-core<0.2,>=0.1.3
 
 # jupyter-environment-manager
 
 [![Documentation](https://img.shields.io/badge/Documentation-DF0982)](https://docs.qbraid.com/projects/lab/en/latest/lab/environments.html)
 [![PyPI version](https://img.shields.io/pypi/v/jupyter-environment-manager.svg?color=blue)](https://pypi.org/project/jupyter-environment-manager/)
 [![GitHub](https://img.shields.io/badge/issue_tracking-github-blue?logo=github)](https://github.com/qBraid/qBraid-Lab/issues)
 [![Discord](https://img.shields.io/discord/771898982564626445.svg?color=pink)](https://discord.gg/TPBU2sa8Et)
```

### Comparing `jupyter_environment_manager-0.2.0rc7/README.md` & `jupyter_environment_manager-0.2.0rc8/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/__init__.py` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/_version.py` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/_version.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/configure.py` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 import time
 from datetime import datetime
 from pathlib import Path
 from typing import Optional
 
 import tornado
 from notebook.base.handlers import APIHandler
-
-from .qbraid_core import is_valid_python
+from qbraid_core.system.executables import is_valid_python
 
 logging.basicConfig(
     level=logging.ERROR,
     format="%(asctime)s - %(levelname)s - %(message)s",
 )
```

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/devices.py` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/devices.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/envs_create.py` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/envs_create.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 import sys
 import threading
 from pathlib import Path
 
 import tornado
 from jupyter_client.kernelspec import KernelSpecManager
 from notebook.base.handlers import APIHandler
-
-from .envs_state import update_install_status
-from .qbraid_core import local_qbraid_envs_path, replace_str
+from qbraid_core.services.environments.paths import DEFAULT_LOCAL_ENVS_PATH
+from qbraid_core.services.environments.state import update_install_status
+from qbraid_core.system.generic import replace_str
 
 logging.basicConfig(
     level=logging.ERROR,
     format="%(asctime)s - %(levelname)s - %(message)s",
 )
 
 
@@ -37,15 +37,15 @@
     def post(self):
         """Create a new qBraid environment."""
         input_data = self.get_json_body()
         slug = input_data.get("slug")
         prompt = input_data.get("prompt")
         display_name = input_data.get("kernelName")
         image_data_url = input_data.get("image")
-        slug_path = os.path.join(local_qbraid_envs_path, slug)
+        slug_path = os.path.join(str(DEFAULT_LOCAL_ENVS_PATH), slug)
         local_resource_dir = os.path.join(slug_path, "kernels", f"python3_{slug}")
         os.makedirs(local_resource_dir, exist_ok=True)
 
         try:
             # create state.json
             update_install_status(slug_path, 0, 0)
```

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/envs_list.py` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/envs_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,42 +14,67 @@
 import shutil
 import subprocess
 import sys
 from typing import List, Optional, Set
 
 import tornado
 from notebook.base.handlers import APIHandler
-
-from .envs_state import install_status_codes
-from .jobs import quantum_jobs_enabled, quantum_jobs_supported
-from .kernels import get_kernels
-from .qbraid_core import (
-    env_path,
+from qbraid_core.services.environments.paths import (
+    DEFAULT_LOCAL_ENVS_PATH,
+    get_default_envs_paths,
+    get_env_path,
     get_next_tmpn,
     get_tmp_dir_names,
-    is_valid_python,
-    local_qbraid_envs_path,
-    replace_str,
-    sys_qbraid_envs_path,
     which_python,
 )
+from qbraid_core.services.environments.state import install_status_codes
+from qbraid_core.system.executables import is_valid_python
+from qbraid_core.system.generic import replace_str
+
+from .jobs import quantum_jobs_supported_enabled
+from .kernels import get_kernels
 
 logging.basicConfig(
     level=logging.ERROR,
     format="%(asctime)s - %(levelname)s - %(message)s",
 )
 
 
 def _uri_to_filepath(uri: str) -> str:
     """Convert a file URI to a local file path."""
     if uri.startswith("file://"):
         return uri[len("file://") :]
     raise ValueError(f"Invalid URI: {uri}")
 
 
+def extract_short_hash(pip_freeze_line: str) -> str:
+    """
+    Extracts the 7-character shortened hash from a pip freeze output line that includes a Git path.
+
+    Args:
+        pip_freeze_line (str): A line from pip freeze output containing a Git path.
+
+    Returns:
+        str: The 7-character shortened Git hash.
+
+    Raises:
+        ValueError: If no valid Git hash is found in the input.
+    """
+    # Regular expression to find the git hash in the provided string
+    match = re.search(r"@ git\+https://.*@([a-fA-F0-9]{40})", pip_freeze_line)
+
+    if match:
+        # Extract the full 40-character hash and return the first 7 characters
+        full_hash = match.group(1)
+        return full_hash[:7]
+
+    # If no hash is found, raise an error
+    raise ValueError("No valid Git hash found in the input.")
+
+
 def _extract_package_version(pip_freeze_string: str) -> Optional[str]:
     """Extract the version of a package from a pip freeze string.
     Return None if the version cannot be extracted."""
 
     # semantic versioning pattern
     semver_pattern = r"(\d+\.\d+\.\d+)"
     match = re.search(semver_pattern, pip_freeze_string)
@@ -65,14 +90,19 @@
         r"egg=[a-zA-Z0-9._-]+$"
     )
     if re.match(git_editable_pattern, pip_freeze_string):
         parts = pip_freeze_string.split("#egg=")
         return parts[0].split(" ", 1)[-1]
 
     try:
+        return extract_short_hash(pip_freeze_string)
+    except ValueError:
+        pass
+
+    try:
         # extract version from locally installed package setup file path
         maybe_uri = pip_freeze_string.split(" @ ")[1]
         filepath = _uri_to_filepath(maybe_uri).strip("\n")
         setup_cfg_path = os.path.join(filepath, "setup.cfg")
         config = configparser.ConfigParser()
         config.read(setup_cfg_path)
         return config.get("metadata", "version")
@@ -121,15 +151,15 @@
     with open(file_path, "w", encoding="utf-8") as file:
         file.writelines(updated_requirements)
 
 
 def get_pip_list(slug: str) -> List[str]:
     """Return packages in requirements.txt in list form.
     If file not found, return empty list."""
-    slug_path = env_path(slug)
+    slug_path = str(get_env_path(slug))
     reqs_txt = os.path.join(slug_path, "requirements.txt")
 
     pip_list = []
 
     if os.path.isfile(reqs_txt):
         with open(f"{reqs_txt}", "r", encoding="utf-8") as f:
             pip_lines = f.readlines()
@@ -140,15 +170,15 @@
     return pip_list
 
 
 def put_pip_list(slug: str, system_site_packages: Optional[bool] = True) -> List[str]:
     """Update/insert requirements.txt and return pip list."""
     python = which_python(slug)
     if is_valid_python(python) and python != sys.executable:
-        slug_path = env_path(slug)
+        slug_path = str(get_env_path(slug))
         cfg = os.path.join(slug_path, "pyenv", "pyvenv.cfg")
         reqs_txt = os.path.join(slug_path, "requirements.txt")
         replace_str("true", "false", cfg)
         with open(reqs_txt, "w", encoding="utf-8") as file:
             subprocess.run(
                 [python, "-m", "pip", "freeze"],
                 stdout=file,
@@ -189,15 +219,16 @@
     def get(self):
         """Gets data surrounding installed environments including any installing
         environment, installed environments, active environments, and pip lists
         of all installed environments."""
         _, kernels_list = get_kernels()  # list of names of installed kernels
 
         # list of directories where environments can be installed
-        env_dir_lst = [sys_qbraid_envs_path, local_qbraid_envs_path]
+        envs_paths = get_default_envs_paths()
+        env_dir_lst = [str(env_path) for env_path in envs_paths]
         uninstalling = self.uninstalling_envs()  # set of slugs currently being uninstalled
 
         installing = None  # name of currently installing, if any
         installed = []  # list of installed environments
         active = []  # list of active environments
         qjobs_supported = []  # list of environments with quantum jobs functionality
         qjobs_enabled = []  # list of environments with quantum jobs enabled
@@ -226,17 +257,18 @@
 
                 # Initialize 'installing' status if it's None
                 if installing is None:
                     installing = self.check_install_status(slug)
 
                 # Check if quantum jobs are supported and/or enabled
                 try:
-                    if quantum_jobs_supported(slug_path):
+                    supported, enabled = quantum_jobs_supported_enabled(slug)
+                    if supported:
                         qjobs_supported.append(slug)
-                        if quantum_jobs_enabled(slug_path):
+                        if enabled:
                             qjobs_enabled.append(slug)
                 except Exception as err:  # pylint: disable=broad-exception-caught
                     logging.error("Error determining quantum jobs state: %s", err)
 
         installing = "" if installing is None else installing
 
         data = {
@@ -250,19 +282,19 @@
 
         self.finish(json.dumps(data))
 
     @staticmethod
     def uninstalling_envs() -> Set[str]:
         """Return set of environment slugs currently being uninstalled."""
         # Assuming local_qbraid_envs_path and get_tmp_dir_names are defined elsewhere.
-        tmpd_names = get_tmp_dir_names(local_qbraid_envs_path)
+        tmpd_names = get_tmp_dir_names(DEFAULT_LOCAL_ENVS_PATH)
         uninstalling = set()
 
         for tmpd_name in tmpd_names:
-            tmpdir = os.path.join(local_qbraid_envs_path, tmpd_name)
+            tmpdir = os.path.join(str(DEFAULT_LOCAL_ENVS_PATH), tmpd_name)
             if os.path.isdir(tmpdir):
                 uninstalling.update(os.listdir(tmpdir))
 
         return uninstalling
 
     @staticmethod
     def validate_slug_env(slug_path: str) -> bool:
@@ -280,18 +312,18 @@
         if len(slug) <= 7 or len(slug) > 20 or slug[-7] != "_":
             return False
 
         persistent_files = ["state.json", "install_status.txt"]
         if any(os.path.isfile(os.path.join(slug_path, file)) for file in persistent_files):
             return True
 
-        if os.path.dirname(slug_path) == local_qbraid_envs_path:
-            tmpd_names = get_tmp_dir_names(local_qbraid_envs_path)
+        if os.path.dirname(slug_path) == str(DEFAULT_LOCAL_ENVS_PATH):
+            tmpd_names = get_tmp_dir_names(DEFAULT_LOCAL_ENVS_PATH)
             tmpn = get_next_tmpn(tmpd_names)
-            rm_dir = os.path.join(local_qbraid_envs_path, tmpn)
+            rm_dir = os.path.join(str(DEFAULT_LOCAL_ENVS_PATH), tmpn)
             os.makedirs(rm_dir, exist_ok=True)
             shutil.move(slug_path, rm_dir)
 
         return False
 
     @staticmethod
     def check_install_status(slug: str) -> Optional[str]:
```

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/envs_pkgs.py` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/envs_pkgs.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,21 @@
 import subprocess
 import sys
 import threading
 from typing import List, Optional
 
 import tornado
 from notebook.base.handlers import APIHandler
-
-from .envs_state import update_install_status
-from .qbraid_core import env_path, local_qbraid_envs_path, replace_str, which_python
+from qbraid_core.services.environments.paths import (
+    DEFAULT_LOCAL_ENVS_PATH,
+    get_env_path,
+    which_python,
+)
+from qbraid_core.services.environments.state import update_install_status
+from qbraid_core.system.generic import replace_str
 
 logging.basicConfig(
     level=logging.ERROR,
     format="%(asctime)s - %(levelname)s - %(message)s",
 )
 
 
@@ -41,15 +45,15 @@
         res_data = {}
         if len(package_lst) == 0 and upgrade_pip is False:
             res_data["status"] = 200
             res_data["message"] += "No package(s) provided."
         else:
             res_data["status"] = 202
             res_data["message"] = "Started pip installs"
-            slug_path = os.path.join(local_qbraid_envs_path, slug)
+            slug_path = os.path.join(str(DEFAULT_LOCAL_ENVS_PATH), slug)
             update_install_status(slug_path, 0, 0)
             thread = threading.Thread(
                 target=self.install_packages,
                 args=(
                     slug,
                     slug_path,
                     package_lst,
@@ -120,15 +124,15 @@
         res_data = {}
         if package is None or len(package) == 0:
             res_data["status"] = 400
             res_data["message"] += "No package provided."
         else:
             res_data["status"] = 202
             res_data["message"] = "Started pip uninstall"
-            slug_path = os.path.join(local_qbraid_envs_path, slug)
+            slug_path = os.path.join(str(DEFAULT_LOCAL_ENVS_PATH), slug)
             update_install_status(slug_path, 0, 0)
             thread = threading.Thread(
                 target=self.uninstall_package,
                 args=(
                     slug,
                     package,
                 ),
@@ -136,15 +140,15 @@
             thread.start()
         self.finish(json.dumps(res_data))
 
     @staticmethod
     def uninstall_package(slug: str, package: str) -> None:
         """Uninstall package from virtual environment."""
         python = which_python(slug)
-        slug_path = env_path(slug)
+        slug_path = get_env_path(slug)
         result = subprocess.run(
             [python, "-m", "pip", "uninstall", package, "-y"], capture_output=True, check=False
         )
         stderr_msg = result.stderr.decode("utf-8")
         stdout_msg = result.stdout.decode("utf-8")
         uninstall_msg = stderr_msg + stdout_msg.strip("\n").split("\n")[-1]
         update_install_status(slug_path, 1, 1, message=uninstall_msg)
```

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/envs_remove.py` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/envs_remove.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,21 @@
 import os
 import shutil
 import threading
 import time
 
 import tornado
 from notebook.base.handlers import APIHandler
+from qbraid_core.services.environments.paths import (
+    DEFAULT_LOCAL_ENVS_PATH,
+    get_next_tmpn,
+    get_tmp_dir_names,
+)
 
 from .kernels import get_kernels
-from .qbraid_core import get_next_tmpn, get_tmp_dir_names, local_qbraid_envs_path
 
 logging.basicConfig(level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s")
 
 
 class UninstallThreader:
     """Class for performing recursive removal of files and directories using multi-threading."""
 
@@ -136,54 +140,54 @@
 
         data = {"status": status, "message": message}
         self.finish(json.dumps(data))
 
     @staticmethod
     def uninstall_env_kernels(slug: str) -> None:
         """Remove environment's kernels from JupyterKernelSpecManager, if they exist."""
-        kernelspec_path = os.path.join(local_qbraid_envs_path, slug, "kernels")
+        kernelspec_path = os.path.join(str(DEFAULT_LOCAL_ENVS_PATH), slug, "kernels")
 
         if os.path.isdir(kernelspec_path):
             kernel_spec_manager, kernels_list = get_kernels()
             for f in os.listdir(kernelspec_path):
                 if f in kernels_list:
                     kernel_spec_manager.remove_kernel_spec(f)
 
     @staticmethod
     def remove_env_cycle(slug: str) -> None:
         """Remove tmp directories in the background."""
         start = time.time()
         threader = UninstallThreader()
-        slug_path = os.path.join(local_qbraid_envs_path, slug)
-        tmpd_names = get_tmp_dir_names(local_qbraid_envs_path)
+        slug_path = os.path.join(str(DEFAULT_LOCAL_ENVS_PATH), slug)
+        tmpd_names = get_tmp_dir_names(DEFAULT_LOCAL_ENVS_PATH)
         init_tmp_dirs = len(tmpd_names)
         num_cylces = 0
         sec_elapsed = 0
 
         while len(tmpd_names) > 0 or os.path.isdir(slug_path) and sec_elapsed < 60:
             if os.path.isdir(slug_path):
                 tmpn = get_next_tmpn(tmpd_names)
-                rm_dir = os.path.join(local_qbraid_envs_path, tmpn)
+                rm_dir = os.path.join(str(DEFAULT_LOCAL_ENVS_PATH), tmpn)
                 os.makedirs(rm_dir, exist_ok=True)
                 shutil.move(slug_path, rm_dir)
                 tmpd_names.append(tmpn)
                 if num_cylces == 0:
                     init_tmp_dirs += 1
 
             for tmpd_name in tmpd_names:
-                tmpdir = os.path.join(local_qbraid_envs_path, tmpd_name)
+                tmpdir = os.path.join(str(DEFAULT_LOCAL_ENVS_PATH), tmpd_name)
                 try:
                     threader.threaded_remove(tmpdir)
                 except Exception as err:  # pylint: disable=broad-exception-caught
                     logging.error("Error removing directory %s: %s", tmpdir, err)
 
             # wait 5 seconds for each tmp rm to finish
             time.sleep(5)
 
-            tmpd_names = get_tmp_dir_names(local_qbraid_envs_path)
+            tmpd_names = get_tmp_dir_names(DEFAULT_LOCAL_ENVS_PATH)
             sec_elapsed = int(time.time() - start)
             num_cylces += 1
 
         num_threads = threader.counter()
         threader.join_threads()
         threader.reset_counter()
```

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/handlers.py` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/handlers.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/kernels.py` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/kernels.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 import os
 import sys
 from typing import List, Tuple
 
 import tornado
 from jupyter_client.kernelspec import KernelSpecManager
 from notebook.base.handlers import APIHandler
-
-from .qbraid_core import env_path, is_exe, sys_qbraid_envs_path
+from qbraid_core.services.environments.paths import DEFAULT_LOCAL_ENVS_PATH, get_env_path
+from qbraid_core.system.executables import is_exe
 
 
 def get_kernels() -> Tuple[KernelSpecManager, List[str]]:
     """Get list of all installed kernels with valid executables."""
     kernel_spec_manager = KernelSpecManager()
     kernelspec_dict = kernel_spec_manager.get_all_specs()
 
@@ -45,26 +45,26 @@
 
     @tornado.web.authenticated
     def post(self):
         """Activate/deactivate environment by adding/removing kernel"""
         input_data = self.get_json_body()
         slug = input_data.get("slug")
 
-        slug_path = env_path(slug)
+        slug_path = str(get_env_path(slug))
         kernels_path = os.path.join(slug_path, "kernels")
         kernel_spec_manager, kernels_list = get_kernels()
         for f in os.listdir(kernels_path):
             if f in kernels_list:
                 # If kernel exists, remove it
                 kernel_spec_manager.remove_kernel_spec(f)
             else:
                 # If kernel doesn't exist, add it
                 resource_path = (
                     sys.prefix
-                    if os.path.exists(os.path.join(sys_qbraid_envs_path, slug))
+                    if not os.path.exists(os.path.join(str(DEFAULT_LOCAL_ENVS_PATH), slug))
                     else os.path.join(os.path.expanduser("~"), ".local")
                 )
                 join_path_kernels = os.path.join(kernels_path, f)
                 kernel_spec_manager.install_kernel_spec(join_path_kernels, prefix=resource_path)
 
         data = {}
         self.finish(json.dumps(data))
```

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/package.json` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9778079710144927%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.64b15d2280d9c5210de7.js'}}",*

 * * "'version'": "'0.2.0-rc.8'"}*

```diff
@@ -51,15 +51,15 @@
                 "jlpm"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.efb45905ee8f674ba5f4.js",
+            "load": "static/remoteEntry.64b15d2280d9c5210de7.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_environment_manager"
                 },
@@ -112,9 +112,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.0-rc.7"
+    "version": "0.2.0-rc.8"
 }
```

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/0.99dd872e735721a05b18.js` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/0.99dd872e735721a05b18.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/113.063bb6057d77be1f85f3.js` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/113.063bb6057d77be1f85f3.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/174.7b162c87cb727f7c2712.js` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/174.7b162c87cb727f7c2712.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/185.4cb0a9019311d36636ce.js` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/185.5d7f6d37c97924a89805.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1031,17 +1031,15 @@
                                 t.success && (this.setState({
                                     quantumJobsEnabled: !e,
                                     qjobsStatus: {
                                         open: !0,
                                         error: !1,
                                         message: e ? "Disabled" : "Enabled"
                                     }
-                                }), this.resetQjobsStatus()), this.context.getActions("EnvironmentActions").registerInstalled().catch((e => {
-                                    throw new Error(e)
-                                }))
+                                }), this.resetQjobsStatus())
                             })).catch((e => {
                                 console.log("Quantum Jobs Toggle Error: ", e), this.setState({
                                     qjobsStatus: {
                                         open: !0,
                                         error: !0,
                                         message: "Error: failed to enable Quantum Jobs"
                                     }
@@ -1208,23 +1206,23 @@
                             disabled: this.props.installing || this.props.env.isPreInstalled || this.state.lockedEnv,
                             onClick: !this.props.env.isPreInstalled && (async () => {
                                 try {
                                     (await this.context.getActions("EnvironmentActions").addQuantumJobs(this.props.env.slug)).success && (this.setState({
                                         quantumJobsAdditionSuccess: !0
                                     }), setTimeout((() => {
                                         this.context.getActions("EnvironmentActions").updateAll().then((() => {
-                                            this.context.getActions("EnvironmentActions").registerInstalled(), this.setState({
+                                            this.setState({
                                                 quantumJobsAdditionSuccess: !1,
                                                 quantumJobs: !0,
                                                 quantumJobsEnabled: !0
                                             })
                                         }))
                                     }), 1750))
                                 } catch (e) {
-                                    console.log("Error adding quantum jobs. ", e), alert("Unable to add quantum jobs at this time. Please try again later, and verify that the qbraid-cli is installed and configured correctly.")
+                                    console.log("Error adding quantum jobs. ", e), alert("Unable to add quantum jobs at this time. Please try again later, and verify that qbraid-core is installed and configured correctly.")
                                 }
                             })
                         }, s().createElement(_.AddCircleOutlineOutlined, {
                             fontSize: "inherit"
                         }))), this.state.quantumJobsAdditionSuccess && s().createElement(v.Box, {
                             display: "flex",
                             alignItems: "center",
@@ -2086,15 +2084,15 @@
                         }
                     }, e)), this.renderInstallInfoPane = () => s().createElement(v.Grid, {
                         item: !0,
                         xs: 12
                     }, s().createElement("div", {
                         className: "env-editor-pane-new",
                         style: {
-                            minHeight: 50
+                            minHeight: 150
                         }
                     }, s().createElement("div", {
                         className: "env-pane-content"
                     }, this.props.packageInstallingEnv === this.props.env._id ? s().createElement(v.Stack, {
                         sx: {
                             width: "100%",
                             color: "grey.500"
@@ -2115,15 +2113,15 @@
                         sx: {
                             width: "100%",
                             color: "grey.500"
                         },
                         spacing: 1
                     }, s().createElement(v.Typography, {
                         className: "env-pane-prompt"
-                    }, this.state.cancelling ? "Cancelling installation" : "Environment is being installed"), s().createElement(v.LinearProgress, {
+                    }, this.state.cancelling ? "Cancelling installation" : "Environment is being installed/updated"), s().createElement(v.LinearProgress, {
                         sx: {
                             backgroundColor: this.state.cancelling ? "red" : "#9909e091",
                             "& .MuiLinearProgress-bar": {
                                 backgroundColor: this.state.cancelling ? "darkred" : "#673ab7"
                             }
                         }
                     }))))), this.renderUpdatePane = () => {
@@ -2288,15 +2286,15 @@
                         disableFocusRipple: !0
                     }, "Delete"))), this.renderCancelInstallPane = () => this.props.env && this.props.env.isPreInstalled ? null : s().createElement(v.Grid, {
                         item: !0,
                         xs: 12
                     }, s().createElement("div", {
                         className: "env-editor-pane-new",
                         style: {
-                            minHeight: 50
+                            minHeight: 150
                         }
                     }, s().createElement("div", {
                         className: "env-pane-content"
                     }, s().createElement(v.Button, {
                         fullWidth: !0,
                         variant: "contained",
                         size: "medium",
@@ -3394,17 +3392,17 @@
                             let n = t;
                             return t._id === e && (n.pinned ? this.handleRemovePinned(e) : this.handleAddPinned(e), n.pinned = !n.pinned), n
                         }));
                         this.setState({
                             environments: t
                         })
                     }, this.handleOpenEnvEditorInstalled = (e, t) => {
-                        this.openEnvironmentEditor(e), this.setState({
+                        this.openEnvironmentEditor(e), "qsharp_b54crn" === e.slug || t || (this.setState({
                             packageLoading: !0
-                        }), "qsharp_b54crn" === e.slug || t || (this.props.flux.getActions("EnvironmentActions").updateQuantumJobStatus(e.slug).catch((e => {
+                        }), this.props.flux.getActions("EnvironmentActions").updateQuantumJobStatus(e.slug).catch((e => {
                             console.log("Error updating quantum job status:", e)
                         })), this.props.flux.getActions("EnvironmentActions").updatePackagesList(e._id).then((() => {
                             this.setState({
                                 packageLoading: !1
                             })
                         })).catch((e => {
                             console.log("Error updating package list:", e), this.setState({
@@ -3908,15 +3906,15 @@
                         containerWidth: null === (t = null === (e = this.aceContainerRef) || void 0 === e ? void 0 : e.current) || void 0 === t ? void 0 : t.offsetWidth
                     })
                 }
                 componentDidUpdate(e, t) {
                     var n, i, a, s, r;
                     (null === (i = null === (n = this.aceContainerRef) || void 0 === n ? void 0 : n.current) || void 0 === i ? void 0 : i.offsetWidth) !== (null === (a = null == this ? void 0 : this.state) || void 0 === a ? void 0 : a.containerWidth) && (this.resizeEditor(), this.setState({
                         containerWidth: null === (r = null === (s = this.aceContainerRef) || void 0 === s ? void 0 : s.current) || void 0 === r ? void 0 : r.offsetWidth
-                    })), console.log("selectedEnvironment", this.state.selectedEnvironment)
+                    }))
                 }
                 componentWillUnmount() {
                     this.props.flux.getStore("EnvironmentStore").unlisten(this.handleUpdateEnvironments)
                 }
                 render() {
                     return s().createElement(v.ThemeProvider, {
                         theme: this.state.currentTheme
@@ -4820,15 +4818,15 @@
                             this.alt.getActions("JupyterApiActions").query("quantum-jobs", {
                                 body: JSON.stringify(a),
                                 method: "PUT"
                             }).then((e => {
                                 e.success ? n({
                                     success: e.success,
                                     stdout: e.stdout
-                                }) : (console.log(`ERROR: ${e.stderr}`), i(new Error(`Action failed with error: ${e.stderr}`)))
+                                }) : i(new Error(`Action failed with error: ${e.stderr}`))
                             })).catch((e => {
                                 const t = `Error in toggleQuantumJobs: ${e.message}`;
                                 return i(t)
                             }))
                         } catch (e) {
                             return i("Quantum jobs is disabled.")
                         }
@@ -5260,15 +5258,15 @@
             n.d(t, {
                 Z: () => s
             });
             var i = n(3645),
                 a = n.n(i)()((function(e) {
                     return e[1]
                 }));
-            a.push([e.id, "#environments-sidebar {\n  min-width: 300px !important;\n  background-color: red !important;\n}\n/* side bar formating start */\n\n/* these classes are over riden in ui tweeks,\nif ui tweeks is not available, while working with this extension,\n uncomment bellow code to format right side bar */\n\n/* .jp-SideBar.lm-TabBar.jp-mod-right {\n  width: 60px !important;\n  max-width: 60px !important;\n  min-width: 60px !important;\n  left: unset !important;\n  right: 0 !important;\n}\n.jp-mod-right > ul > li {\n  display: flex !important;\n  flex-direction: column !important;\n  justify-content: center !important;\n  align-items: center !important;\n  width: 60px !important;\n  max-width: 60px !important;\n  min-width: 60px !important;\n  height: 60px !important;\n  max-height: 60px !important;\n  min-height: 60px !important;\n  align-items: center !important;\n  margin: 0 !important;\n  padding: 0 !important;\n  text-align: center;\n  color: var(--jp-ui-font-color1) !important;\n  transform: rotate(-90deg) translateX(28px) !important;\n  border-right: var(--jp-border-width) solid var(--jp-border-color1) !important;\n  border-left: unset !important;\n} */\n\n.env_icon_parent {\n  transition: none !important;\n  transform: rotate(0deg) !important;\n}\nbody[data-jp-theme-light='true'] .env_icon {\n  filter: invert(0.6);\n}\n.env_icon {\n  width: 30px;\n  height: 30px;\n  min-width: 30px;\n  min-height: 30px;\n  margin-top: 5px !important;\n}\n/* this class is for the right side bar list item for environment manger extesion\n.environment_sidebar_li {\n } */\n\n.environment_sidebar_li div:nth-child(2) {\n  text-align: center !important;\n  min-width: fit-content !important;\n  font-size: 10px !important;\n  text-transform: uppercase !important;\n  flex: 0 1 auto !important;\n  margin-top: -5px !important;\n}\n\n/* side bar formating end  */\n\n.environments-sidebar {\n  /* position: relative; */\n  position: absolute;\n  height: 100%;\n  width: 100%;\n  /* width: 420px; */\n  background-color: var(--jp-layout-color1) !important;\n  /* overflow-x: visible; */\n}\n\n.environments-sidebar-header {\n  padding: 15px 10px;\n  color: #d30982;\n  font-weight: 600;\n  text-transform: uppercase;\n  letter-spacing: 1px;\n}\n\n.environments-sidebar-spacer {\n  width: 100%;\n  height: var(--jp-border-width);\n  background-color: var(--jp-border-color2);\n}\n\n.environments-sidebar-list-pane,\n.environments-sidebar-search-pane {\n  position: absolute;\n  right: 0%;\n  height: calc(100% - 50px);\n  overflow-x: hidden;\n  overflow-y: auto;\n  /* height: 100%; */\n}\n\n.environments-sidebar-list-pane {\n  width: 100%;\n  transition: 300ms right ease;\n}\n\n.environments-sidebar-search-pane {\n  width: 0%;\n  transition: width 300ms ease;\n}\n\n.environments-sidebar-environment-list {\n  padding-bottom: 200px;\n}\n\n.envoronments-sidebar-search-wrapper {\n  position: relative;\n}\n\n.environments-sidebar-search-icon {\n  position: absolute;\n  width: 16px;\n  top: 0px;\n  left: 1rem;\n  color: var(--jp-ui-font-color2);\n}\n\n.environments-sidebar-search-bar {\n  width: calc(100% - 62px);\n  /* 62px accounts for horizontal margin and padding */\n  margin: 10px;\n  font-size: 14px;\n  border: 1px solid var(--jp-border-color2);\n  border-radius: 2px;\n  color: var(--jp-ui-font-color2);\n  /* background: url(https://qbraid-static.s3.amazonaws.com/search.svg) no-repeat */\n  /* scroll 8px 10px; */\n  background-color: var(--jp-input-background);\n  padding: 10px 10px 10px 32px;\n  /* background-size: 16px; */\n  box-sizing: content-box !important;\n  transition: all 0.2s linear;\n}\n\n.environments-sidebar-search-bar:hover {\n  border-color: var(--jp-border-color1);\n}\n\n.environments-sidebar-search-bar:focus {\n  outline: none;\n  border-color: var(--jp-border-color1);\n  background-color: var(--jp-input-active-background);\n}\n\n.refresh-btn {\n  fill: #d30982;\n  border-radius: 50%;\n  height: 20px;\n  width: 20px;\n}\n\n.refresh-btn:hover {\n  cursor: pointer;\n  fill: #ff24a7;\n  /* border-radius: 50%;\n  box-shadow: 0px 1px 3px 2px rgb(0 0 0 / 40%); */\n}\n\n.div-refresh-btn {\n  height: 20px;\n  margin-left: 5px;\n}\n\n.environments-sidebar-refresh-btn {\n  cursor: pointer;\n  height: 20px;\n  margin-left: 4px;\n  transition: 300ms opacity ease;\n}\n\n.environments-sidebar-add-btn {\n  float: right;\n  color: #d30982;\n  /* color: #ff24a7; */\n  /* color: #aaa; */\n  cursor: pointer;\n  opacity: 1;\n  transition: 300ms opacity ease;\n}\n\n.environments-sidebar-left-arrow {\n  font-size: 20px;\n  margin-top: -2px;\n}\n\n.environments-sidebar-add-btn:hover {\n  color: #ff24a7;\n}\n\n.environments-sidebar-back-btn {\n  vertical-align: baseline;\n  display: inline-block;\n  margin-right: 5px;\n  height: 0;\n  transition: 300ms opacity ease;\n  margin-top: -22px;\n  cursor: pointer;\n}\n\n.environments-sidebar-back-btn:hover {\n  color: #ff24a7;\n}\n\n.environments-sidebar-tab-empty {\n  color: var(--jp-ui-font-color3);\n  margin-top: 20px;\n  text-align: center;\n  font-style: italic;\n}\n\n.environments-sidebar-create-env {\n  position: relative;\n  display: flex;\n  flex-direction: row;\n  justify-content: center;\n  align-items: center;\n  margin: 10px;\n  padding: 4px 10px;\n  border: 2px solid transparent;\n  border-radius: 10px;\n  box-sizing: content-box !important;\n  /* overrides jupyterhub, which sets box-sizing: border-box */\n  background-color: #845bc3;\n  background-color: #673ab7;\n  color: white;\n  box-shadow: 0px 1px 4px -2px #555;\n  cursor: pointer;\n}\n\n.environment-tile {\n  margin: 10px;\n  padding: 10px;\n  background-color: var(--jp-layout-color2);\n  border-radius: 4px;\n  border-bottom: 1px solid var(--jp-layout-color3);\n  cursor: pointer;\n}\n\n.environment-tile-name {\n  color: var(--jp-ui-font-color2);\n}\n\n.environment-tile-active-flag {\n  float: right;\n  /* color: #d20882; */\n  color: #742857;\n}\n\n.qbraid-splash-background {\n  position: fixed;\n  top: 0px;\n  bottom: 0px;\n  left: 0px;\n  right: 0px;\n  z-index: 999999;\n  background-color: #212121;\n  opacity: 1;\n  transition: 500ms opacity linear;\n}\n\n.qbraid-splash-foreground {\n  position: fixed;\n  top: calc(50vh - 200px);\n  width: 100vw;\n  text-align: center;\n  user-select: none;\n}\n\n.qbraid-splash-logo {\n  position: relative;\n  width: 200px;\n}\n\n.qbraid-splash-text {\n  position: relative;\n  margin-top: 20px;\n  font-size: 24px;\n  font-family: Helvetica;\n  color: #8c357d;\n}\n\n.overlay-background {\n  position: fixed;\n  display: flex;\n  flex-direction: column;\n  justify-content: center;\n  align-items: center;\n  height: 100vh;\n  width: 100vw;\n  top: 0;\n  left: 0;\n  background-color: rgba(0, 0, 0, 0.5);\n  z-index: 999998;\n}\n\n.overlay-dialog {\n  position: relative;\n  width: 50%;\n  margin-top: -40px;\n  border-radius: 25px;\n  background-color: #f5f5f5;\n  box-shadow: 0 5px 5px -3px rgba(0, 0, 0, 0.2),\n    0 8px 10px 1px rgba(0, 0, 0, 0.14), 0 3px 14px 2px rgba(0, 0, 0, 0.12);\n  z-index: 999999;\n}\n\n.overlay-title {\n  background: linear-gradient(90deg, #7643be 5.23%, #b469e0 84.11%);\n  border-radius: 25px 25px 0px 0px;\n}\n\n.overlay-backicon-wrapper {\n  padding: 5px;\n}\n\n.overlay-backicon {\n  cursor: pointer;\n}\n\n.overlay-content {\n  padding: 10px 20px 20px 20px;\n}\n\n.overlay-closeicon-wrapper {\n  position: absolute;\n  right: -24px;\n  top: -24px;\n}\n\n.overlay-closeicon {\n  cursor: pointer;\n}\n\n.overlay-icon-wrapper {\n  display: flex;\n  justify-content: center;\n  align-items: center;\n  width: 32px;\n  height: 32px;\n  background: #fb9b2a;\n  border-radius: 16px;\n  margin-right: 15px;\n}\n\n.overlay-icon-vector {\n  width: 16px;\n  height: 16px;\n}\n\n.overlay-input-wrapper {\n  display: flex;\n  margin-top: 5px;\n  background: #ffffff;\n  border-radius: 8px;\n  padding: 9px 20px;\n  align-items: center;\n}\n\n.overlay-inputgroup {\n  margin-top: 10px;\n}\n\n.overlay-input {\n  border: none;\n  flex-grow: 1;\n  padding-left: 9px;\n  border-left: 1px solid #d1d1d1;\n}\n\n.overlay-textfield {\n  border: none;\n  flex-grow: 1;\n}\n\n.overlay-button {\n  padding: 12px 20px;\n  border: none;\n  border-radius: 8px;\n  cursor: pointer;\n}\n\n.overlay-buttongroup {\n  display: flex;\n  margin-top: 20px;\n  background: #f5f5f5;\n  border: 1px solid #7f49c3;\n  border-radius: 8px;\n  box-sizing: border-box;\n}\n\n.overlay-toggle-button {\n  flex-grow: 1;\n  color: #7f49c3;\n}\n\n.overlay-toggle-active-button {\n  background: #7f49c3;\n  color: white;\n}\n\n.overlay-close-button {\n  background: #515254;\n  color: white;\n}\n\n.overlay-confirm-button {\n  background: #515254;\n  color: white;\n}\n\n.overlay-confirm-button-wrapper {\n  display: flex;\n  justify-content: end;\n  margin-top: 20px;\n}\n\n.editor-ace-wrapper {\n  flex: 1;\n  overflow: auto;\n  margin-top: 5px;\n}\n\n.env-dialog-img-title {\n  display: flex;\n  flex-direction: column;\n  justify-content: center;\n  align-items: center;\n}\n\n.env-dialog-img-content {\n  display: flex;\n  flex-direction: column;\n  justify-content: center;\n  align-items: center;\n  gap: 8px;\n}\n\n.env-dialog-img {\n  position: relative;\n  margin-inline: auto;\n  width: 250px;\n  height: 250px;\n  object-fit: scale-down;\n  border: 2px dashed #555;\n}\n\n.uploadImg-dialog-description {\n  font-size: 0.8rem !important;\n}\n\n.uploadImg-error-text {\n  flex: 1;\n  text-align: left;\n  color: indianred;\n  padding-left: 1em;\n  font-size: 0.8rem !important;\n}\n\n.env-sidebar-msg-popup {\n  position: absolute;\n  width: calc(100% - 4em);\n  margin: 0px 1em;\n  height: 3rem;\n  display: flex;\n  align-items: center;\n  justify-content: center;\n  border-radius: 10px;\n  bottom: 10px;\n  padding: 0.25em 1em;\n}\n.success {\n  background-color: green;\n  color: white;\n}\n.error {\n  background-color: indianred;\n  color: white;\n}\n.stay-longer {\n  animation-duration: 4s !important;\n}\n\n.highlight-kernel {\n  border: 1px solid #883ae8;\n  border-radius: 4px;\n  animation: blip-notify 3s alternate both;\n  animation-timing-function: cubic-bezier(0.47, 0, 0.75, 0.72);\n  --_text-clr: var(--jp-ui-font-color0);\n}\n\n.highlight-kernel .jp-ToolbarButtonComponent-label {\n  color: var(--_text-clr) !important;\n}\n\n.pos-fixed-kernel_message {\n  position: fixed;\n  top: 6rem;\n  right: 20rem;\n  background-color: var(--jp-layout-color1);\n  border: 1px solid var(--jp-border-color1);\n  border-radius: 4px;\n  padding: 8px;\n  color: var(--jp-ui-font-color0);\n  font-size: 14px;\n  box-shadow: var(--jp-elevation-z6);\n  opacity: 0;\n  transition: right 150ms ease, opacity 250ms ease;\n}\n\n.pos-fixed-kernel_message::after {\n  content: '';\n  position: absolute;\n  width: 15px;\n  height: 15px;\n  background-color: var(--jp-layout-color1);\n  top: -14px;\n  right: 15px;\n  clip-path: polygon(50% 0%, 0% 100%, 100% 100%);\n  box-shadow: var(--jp-elevation-z6);\n}\n\n.env_dialog-btn_cancel {\n  background-color: transparent !important;\n  border: 1px solid #6640b3 !important;\n  border-radius: 6px;\n  color: #6640b3 !important;\n}\n\n.env_dialog-btn_confirm {\n  background-color: #6640b3 !important;\n  border-radius: 6px;\n  color: white !important;\n}\n\n.gpu_warn_dialog-checkbox {\n  width: 100%;\n  padding-bottom: 8px;\n}\n\n.jp-Dialog-footer {\n  flex-wrap: wrap;\n}\n\n/* animation css */\n.slide-in-bottom {\n  -webkit-animation: slide-in-bottom 2.5s cubic-bezier(0.645, 0.045, 0.355, 1)\n    both;\n  animation: slide-in-bottom 2.5s cubic-bezier(0.645, 0.045, 0.355, 1) both;\n  /* animation-iteration-count: infinite; */\n}\n\n/**\n * ----------------------------------------\n * animation slide-in-bottom\n * ----------------------------------------\n */\n\n@keyframes slide-in-bottom {\n  0% {\n    -webkit-transform: translateY(40px);\n    transform: translateY(40px);\n    opacity: 0;\n  }\n  30% {\n    -webkit-transform: translateY(0);\n    transform: translateY(0);\n    opacity: 1;\n  }\n  80% {\n    -webkit-transform: translateY(0);\n    transform: translateY(0);\n    opacity: 1;\n  }\n  100% {\n    -webkit-transform: translateY(40px);\n    transform: translateY(40px);\n    opacity: 0;\n  }\n}\n\n/**\n * ----------------------------------------\n * animation pulsing-notification\n * ----------------------------------------\n */\n\n@keyframes blip-notify {\n  from {\n    background: #673ab7;\n    --_text-clr: white;\n  }\n  to {\n    background: #aa89e438;\n    --_text-clr: var(--jp-ui-font-color0);\n  }\n}\n", ""]);
+            a.push([e.id, "#environments-sidebar {\n  min-width: 300px !important;\n  background-color: red !important;\n}\n/* side bar formating start */\n\n/* these classes are over riden in ui tweeks,\nif ui tweeks is not available, while working with this extension,\n uncomment bellow code to format right side bar */\n\n/* .jp-SideBar.lm-TabBar.jp-mod-right {\n  width: 60px !important;\n  max-width: 60px !important;\n  min-width: 60px !important;\n  left: unset !important;\n  right: 0 !important;\n}\n.jp-mod-right > ul > li {\n  display: flex !important;\n  flex-direction: column !important;\n  justify-content: center !important;\n  align-items: center !important;\n  width: 60px !important;\n  max-width: 60px !important;\n  min-width: 60px !important;\n  height: 60px !important;\n  max-height: 60px !important;\n  min-height: 60px !important;\n  align-items: center !important;\n  margin: 0 !important;\n  padding: 0 !important;\n  text-align: center;\n  color: var(--jp-ui-font-color1) !important;\n  transform: rotate(-90deg) translateX(28px) !important;\n  border-right: var(--jp-border-width) solid var(--jp-border-color1) !important;\n  border-left: unset !important;\n} */\n\n.env_icon_parent {\n  transition: none !important;\n  transform: rotate(0deg) !important;\n}\nbody[data-jp-theme-light='true'] .env_icon {\n  filter: invert(0.6);\n}\n.env_icon {\n  width: 30px;\n  height: 30px;\n  min-width: 30px;\n  min-height: 30px;\n  margin-top: 5px !important;\n}\n/* this class is for the right side bar list item for environment manger extesion\n.environment_sidebar_li {\n } */\n\n.environment_sidebar_li div:nth-child(2) {\n  text-align: center !important;\n  min-width: fit-content !important;\n  font-size: 10px !important;\n  text-transform: uppercase !important;\n  flex: 0 1 auto !important;\n  margin-top: -5px !important;\n}\n\n/* side bar formating end  */\n\n.environments-sidebar {\n  /* position: relative; */\n  position: absolute;\n  height: 100%;\n  width: 100%;\n  /* width: 420px; */\n  background-color: var(--jp-layout-color1) !important;\n  /* overflow-x: visible; */\n}\n\n.environments-sidebar-header {\n  padding: 15px 10px;\n  color: #d30982;\n  font-weight: 600;\n  text-transform: uppercase;\n  letter-spacing: 1px;\n}\n\n.environments-sidebar-spacer {\n  width: 100%;\n  height: var(--jp-border-width);\n  background-color: var(--jp-border-color2);\n}\n\n.environments-sidebar-list-pane,\n.environments-sidebar-search-pane {\n  position: absolute;\n  right: 0%;\n  height: calc(100% - 50px);\n  overflow-x: hidden;\n  overflow-y: auto;\n  /* height: 100%; */\n}\n\n.environments-sidebar-list-pane {\n  width: 100%;\n  transition: 300ms right ease;\n}\n\n.environments-sidebar-search-pane {\n  width: 0%;\n  transition: width 300ms ease;\n}\n\n.environments-sidebar-environment-list {\n  padding-bottom: 200px;\n  background-color: var(--jp-layout-color1);\n}\n\n.envoronments-sidebar-search-wrapper {\n  position: relative;\n}\n\n.environments-sidebar-search-icon {\n  position: absolute;\n  width: 16px;\n  top: 0px;\n  left: 1rem;\n  color: var(--jp-ui-font-color2);\n}\n\n.environments-sidebar-search-bar {\n  width: calc(100% - 62px);\n  /* 62px accounts for horizontal margin and padding */\n  margin: 10px;\n  font-size: 14px;\n  border: 1px solid var(--jp-border-color2);\n  border-radius: 2px;\n  color: var(--jp-ui-font-color2);\n  /* background: url(https://qbraid-static.s3.amazonaws.com/search.svg) no-repeat */\n  /* scroll 8px 10px; */\n  background-color: var(--jp-input-background);\n  padding: 10px 10px 10px 32px;\n  /* background-size: 16px; */\n  box-sizing: content-box !important;\n  transition: all 0.2s linear;\n}\n\n.environments-sidebar-search-bar:hover {\n  border-color: var(--jp-border-color1);\n}\n\n.environments-sidebar-search-bar:focus {\n  outline: none;\n  border-color: var(--jp-border-color1);\n  background-color: var(--jp-input-active-background);\n}\n\n.refresh-btn {\n  fill: #d30982;\n  border-radius: 50%;\n  height: 20px;\n  width: 20px;\n}\n\n.refresh-btn:hover {\n  cursor: pointer;\n  fill: #ff24a7;\n  /* border-radius: 50%;\n  box-shadow: 0px 1px 3px 2px rgb(0 0 0 / 40%); */\n}\n\n.div-refresh-btn {\n  height: 20px;\n  margin-left: 5px;\n}\n\n.environments-sidebar-refresh-btn {\n  cursor: pointer;\n  height: 20px;\n  margin-left: 4px;\n  transition: 300ms opacity ease;\n}\n\n.environments-sidebar-add-btn {\n  float: right;\n  color: #d30982;\n  /* color: #ff24a7; */\n  /* color: #aaa; */\n  cursor: pointer;\n  opacity: 1;\n  transition: 300ms opacity ease;\n}\n\n.environments-sidebar-left-arrow {\n  font-size: 20px;\n  margin-top: -2px;\n}\n\n.environments-sidebar-add-btn:hover {\n  color: #ff24a7;\n}\n\n.environments-sidebar-back-btn {\n  vertical-align: baseline;\n  display: inline-block;\n  margin-right: 5px;\n  height: 0;\n  transition: 300ms opacity ease;\n  margin-top: -22px;\n  cursor: pointer;\n}\n\n.environments-sidebar-back-btn:hover {\n  color: #ff24a7;\n}\n\n.environments-sidebar-tab-empty {\n  color: var(--jp-ui-font-color3);\n  margin-top: 20px;\n  text-align: center;\n  font-style: italic;\n}\n\n.environments-sidebar-create-env {\n  position: relative;\n  display: flex;\n  flex-direction: row;\n  justify-content: center;\n  align-items: center;\n  margin: 10px;\n  padding: 4px 10px;\n  border: 2px solid transparent;\n  border-radius: 10px;\n  box-sizing: content-box !important;\n  /* overrides jupyterhub, which sets box-sizing: border-box */\n  background-color: #845bc3;\n  background-color: #673ab7;\n  color: white;\n  box-shadow: 0px 1px 4px -2px #555;\n  cursor: pointer;\n}\n\n.environment-tile {\n  margin: 10px;\n  padding: 10px;\n  background-color: var(--jp-layout-color2);\n  border-radius: 4px;\n  border-bottom: 1px solid var(--jp-layout-color3);\n  cursor: pointer;\n}\n\n.environment-tile-name {\n  color: var(--jp-ui-font-color2);\n}\n\n.environment-tile-active-flag {\n  float: right;\n  /* color: #d20882; */\n  color: #742857;\n}\n\n.qbraid-splash-background {\n  position: fixed;\n  top: 0px;\n  bottom: 0px;\n  left: 0px;\n  right: 0px;\n  z-index: 999999;\n  background-color: #212121;\n  opacity: 1;\n  transition: 500ms opacity linear;\n}\n\n.qbraid-splash-foreground {\n  position: fixed;\n  top: calc(50vh - 200px);\n  width: 100vw;\n  text-align: center;\n  user-select: none;\n}\n\n.qbraid-splash-logo {\n  position: relative;\n  width: 200px;\n}\n\n.qbraid-splash-text {\n  position: relative;\n  margin-top: 20px;\n  font-size: 24px;\n  font-family: Helvetica;\n  color: #8c357d;\n}\n\n.overlay-background {\n  position: fixed;\n  display: flex;\n  flex-direction: column;\n  justify-content: center;\n  align-items: center;\n  height: 100vh;\n  width: 100vw;\n  top: 0;\n  left: 0;\n  background-color: rgba(0, 0, 0, 0.5);\n  z-index: 999998;\n}\n\n.overlay-dialog {\n  position: relative;\n  width: 50%;\n  margin-top: -40px;\n  border-radius: 25px;\n  background-color: #f5f5f5;\n  box-shadow: 0 5px 5px -3px rgba(0, 0, 0, 0.2),\n    0 8px 10px 1px rgba(0, 0, 0, 0.14), 0 3px 14px 2px rgba(0, 0, 0, 0.12);\n  z-index: 999999;\n}\n\n.overlay-title {\n  background: linear-gradient(90deg, #7643be 5.23%, #b469e0 84.11%);\n  border-radius: 25px 25px 0px 0px;\n}\n\n.overlay-backicon-wrapper {\n  padding: 5px;\n}\n\n.overlay-backicon {\n  cursor: pointer;\n}\n\n.overlay-content {\n  padding: 10px 20px 20px 20px;\n}\n\n.overlay-closeicon-wrapper {\n  position: absolute;\n  right: -24px;\n  top: -24px;\n}\n\n.overlay-closeicon {\n  cursor: pointer;\n}\n\n.overlay-icon-wrapper {\n  display: flex;\n  justify-content: center;\n  align-items: center;\n  width: 32px;\n  height: 32px;\n  background: #fb9b2a;\n  border-radius: 16px;\n  margin-right: 15px;\n}\n\n.overlay-icon-vector {\n  width: 16px;\n  height: 16px;\n}\n\n.overlay-input-wrapper {\n  display: flex;\n  margin-top: 5px;\n  background: #ffffff;\n  border-radius: 8px;\n  padding: 9px 20px;\n  align-items: center;\n}\n\n.overlay-inputgroup {\n  margin-top: 10px;\n}\n\n.overlay-input {\n  border: none;\n  flex-grow: 1;\n  padding-left: 9px;\n  border-left: 1px solid #d1d1d1;\n}\n\n.overlay-textfield {\n  border: none;\n  flex-grow: 1;\n}\n\n.overlay-button {\n  padding: 12px 20px;\n  border: none;\n  border-radius: 8px;\n  cursor: pointer;\n}\n\n.overlay-buttongroup {\n  display: flex;\n  margin-top: 20px;\n  background: #f5f5f5;\n  border: 1px solid #7f49c3;\n  border-radius: 8px;\n  box-sizing: border-box;\n}\n\n.overlay-toggle-button {\n  flex-grow: 1;\n  color: #7f49c3;\n}\n\n.overlay-toggle-active-button {\n  background: #7f49c3;\n  color: white;\n}\n\n.overlay-close-button {\n  background: #515254;\n  color: white;\n}\n\n.overlay-confirm-button {\n  background: #515254;\n  color: white;\n}\n\n.overlay-confirm-button-wrapper {\n  display: flex;\n  justify-content: end;\n  margin-top: 20px;\n}\n\n.editor-ace-wrapper {\n  flex: 1;\n  overflow: auto;\n  margin-top: 5px;\n}\n\n.env-dialog-img-title {\n  display: flex;\n  flex-direction: column;\n  justify-content: center;\n  align-items: center;\n}\n\n.env-dialog-img-content {\n  display: flex;\n  flex-direction: column;\n  justify-content: center;\n  align-items: center;\n  gap: 8px;\n}\n\n.env-dialog-img {\n  position: relative;\n  margin-inline: auto;\n  width: 250px;\n  height: 250px;\n  object-fit: scale-down;\n  border: 2px dashed #555;\n}\n\n.uploadImg-dialog-description {\n  font-size: 0.8rem !important;\n}\n\n.uploadImg-error-text {\n  flex: 1;\n  text-align: left;\n  color: indianred;\n  padding-left: 1em;\n  font-size: 0.8rem !important;\n}\n\n.env-sidebar-msg-popup {\n  position: absolute;\n  width: calc(100% - 4em);\n  margin: 0px 1em;\n  height: 3rem;\n  display: flex;\n  align-items: center;\n  justify-content: center;\n  border-radius: 10px;\n  bottom: 10px;\n  padding: 0.25em 1em;\n}\n.success {\n  background-color: green;\n  color: white;\n}\n.error {\n  background-color: indianred;\n  color: white;\n}\n.stay-longer {\n  animation-duration: 4s !important;\n}\n\n.highlight-kernel {\n  border: 1px solid #883ae8;\n  border-radius: 4px;\n  animation: blip-notify 3s alternate both;\n  animation-timing-function: cubic-bezier(0.47, 0, 0.75, 0.72);\n  --_text-clr: var(--jp-ui-font-color0);\n}\n\n.highlight-kernel .jp-ToolbarButtonComponent-label {\n  color: var(--_text-clr) !important;\n}\n\n.pos-fixed-kernel_message {\n  position: fixed;\n  top: 6rem;\n  right: 20rem;\n  background-color: var(--jp-layout-color1);\n  border: 1px solid var(--jp-border-color1);\n  border-radius: 4px;\n  padding: 8px;\n  color: var(--jp-ui-font-color0);\n  font-size: 14px;\n  box-shadow: var(--jp-elevation-z6);\n  opacity: 0;\n  transition: right 150ms ease, opacity 250ms ease;\n}\n\n.pos-fixed-kernel_message::after {\n  content: '';\n  position: absolute;\n  width: 15px;\n  height: 15px;\n  background-color: var(--jp-layout-color1);\n  top: -14px;\n  right: 15px;\n  clip-path: polygon(50% 0%, 0% 100%, 100% 100%);\n  box-shadow: var(--jp-elevation-z6);\n}\n\n.env_dialog-btn_cancel {\n  background-color: transparent !important;\n  border: 1px solid #6640b3 !important;\n  border-radius: 6px;\n  color: #6640b3 !important;\n}\n\n.env_dialog-btn_confirm {\n  background-color: #6640b3 !important;\n  border-radius: 6px;\n  color: white !important;\n}\n\n.gpu_warn_dialog-checkbox {\n  width: 100%;\n  padding-bottom: 8px;\n}\n\n.jp-Dialog-footer {\n  flex-wrap: wrap;\n}\n\n/* animation css */\n.slide-in-bottom {\n  -webkit-animation: slide-in-bottom 2.5s cubic-bezier(0.645, 0.045, 0.355, 1)\n    both;\n  animation: slide-in-bottom 2.5s cubic-bezier(0.645, 0.045, 0.355, 1) both;\n  /* animation-iteration-count: infinite; */\n}\n\n/**\n * ----------------------------------------\n * animation slide-in-bottom\n * ----------------------------------------\n */\n\n@keyframes slide-in-bottom {\n  0% {\n    -webkit-transform: translateY(40px);\n    transform: translateY(40px);\n    opacity: 0;\n  }\n  30% {\n    -webkit-transform: translateY(0);\n    transform: translateY(0);\n    opacity: 1;\n  }\n  80% {\n    -webkit-transform: translateY(0);\n    transform: translateY(0);\n    opacity: 1;\n  }\n  100% {\n    -webkit-transform: translateY(40px);\n    transform: translateY(40px);\n    opacity: 0;\n  }\n}\n\n/**\n * ----------------------------------------\n * animation pulsing-notification\n * ----------------------------------------\n */\n\n@keyframes blip-notify {\n  from {\n    background: #673ab7;\n    --_text-clr: white;\n  }\n  to {\n    background: #aa89e438;\n    --_text-clr: var(--jp-ui-font-color0);\n  }\n}\n", ""]);
             const s = a
         },
         6513: (e, t, n) => {
             n.d(t, {
                 Z: () => s
             });
             var i = n(3645),
```

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/24.a6fec73552ceb9bdb6aa.js` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/24.a6fec73552ceb9bdb6aa.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js.LICENSE.txt` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/378.8fdd4b1246fb17037bb3.js` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/378.8fdd4b1246fb17037bb3.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/478.b1efc8dc1ed4a16150ef.js` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/478.b1efc8dc1ed4a16150ef.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/554.3ee5e631ee6f4d8c24e2.js` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/554.3ee5e631ee6f4d8c24e2.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/569.110780388cdcc5605903.js` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/569.110780388cdcc5605903.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/588.634556691591dc1dac9b.js` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/588.634556691591dc1dac9b.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/66.715eff54360a4988967a.js` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/66.715eff54360a4988967a.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/697.61315fde7050f7a02689.js` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/697.61315fde7050f7a02689.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/747.6d49dfe38d298a9d88e1.js` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/747.6d49dfe38d298a9d88e1.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/813.4baf0234297462c92d8b.js` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/813.4baf0234297462c92d8b.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/909.c50074d4e4be5aa7c06a.js` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/909.c50074d4e4be5aa7c06a.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js.LICENSE.txt` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/991.b0c652da28634799e4d5.js` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/991.b0c652da28634799e4d5.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/remoteEntry.efb45905ee8f674ba5f4.js` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/remoteEntry.64b15d2280d9c5210de7.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, i, d, f, l, c, u, s, b, p, h, m, v, g, y, w = {
+    var e, r, t, a, n, o, i, d, c, f, l, u, s, b, p, h, m, v, g, y, w = {
             7413: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(66), t.e(588), t.e(0), t.e(271), t.e(222), t.e(456), t.e(185)]).then((() => () => t(4185))),
                         "./extension": () => Promise.all([t.e(66), t.e(588), t.e(0), t.e(271), t.e(222), t.e(456), t.e(185)]).then((() => () => t(4185))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
@@ -52,15 +52,15 @@
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         0: "99dd872e735721a05b18",
         24: "a6fec73552ceb9bdb6aa",
         66: "715eff54360a4988967a",
         113: "063bb6057d77be1f85f3",
         151: "18af1747c52fa1890fce",
         174: "7b162c87cb727f7c2712",
-        185: "4cb0a9019311d36636ce",
+        185: "5d7f6d37c97924a89805",
         211: "600bba662ff9e624e2f6",
         222: "6dffdbe65a2e7cc44707",
         271: "36aa2c7fc0a5419d0981",
         313: "f6abbabc37aacd77b555",
         378: "8fdd4b1246fb17037bb3",
         456: "31436070dfbf8e0b6319",
         478: "b1efc8dc1ed4a16150ef",
@@ -77,15 +77,15 @@
     } [e] + ".js?v=" + {
         0: "99dd872e735721a05b18",
         24: "a6fec73552ceb9bdb6aa",
         66: "715eff54360a4988967a",
         113: "063bb6057d77be1f85f3",
         151: "18af1747c52fa1890fce",
         174: "7b162c87cb727f7c2712",
-        185: "4cb0a9019311d36636ce",
+        185: "5d7f6d37c97924a89805",
         211: "600bba662ff9e624e2f6",
         222: "6dffdbe65a2e7cc44707",
         271: "36aa2c7fc0a5419d0981",
         313: "f6abbabc37aacd77b555",
         378: "8fdd4b1246fb17037bb3",
         456: "31436070dfbf8e0b6319",
         478: "b1efc8dc1ed4a16150ef",
@@ -107,18 +107,18 @@
             if ("object" == typeof window) return window
         }
     }(), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@qbraid/jupyter-environment-manager:", j.l = (t, a, n, o) => {
         if (e[t]) e[t].push(a);
         else {
             var i, d;
             if (void 0 !== n)
-                for (var f = document.getElementsByTagName("script"), l = 0; l < f.length; l++) {
-                    var c = f[l];
-                    if (c.getAttribute("src") == t || c.getAttribute("data-webpack") == r + n) {
-                        i = c;
+                for (var c = document.getElementsByTagName("script"), f = 0; f < c.length; f++) {
+                    var l = c[f];
+                    if (l.getAttribute("src") == t || l.getAttribute("data-webpack") == r + n) {
+                        i = l;
                         break
                     }
                 }
             i || (d = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, j.nc && i.setAttribute("nonce", j.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [a];
             var u = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(s);
                     var n = e[t];
@@ -153,16 +153,16 @@
                             d = n[r];
                         (!d || !d.loaded && (!a != !d.eager ? a : i > d.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
-                    f = [];
-                return "default" === t && (d("@aws-amplify/auth", "4.6.0", (() => Promise.all([j.e(313), j.e(151)]).then((() => () => j(8313))))), d("@emotion/react", "11.10.0", (() => Promise.all([j.e(113), j.e(271), j.e(991)]).then((() => () => j(3113))))), d("@emotion/styled", "11.10.0", (() => Promise.all([j.e(378), j.e(271), j.e(211), j.e(799)]).then((() => () => j(4378))))), d("@mui/icons-material", "5.8.4", (() => Promise.all([j.e(66), j.e(24), j.e(271), j.e(222)]).then((() => () => j(4024))))), d("@mui/material", "5.15.10", (() => Promise.all([j.e(66), j.e(909), j.e(588), j.e(271), j.e(211), j.e(222), j.e(456)]).then((() => () => j(1909))))), d("@qbraid/jupyter-environment-manager", "0.2.0-rc.7", (() => Promise.all([j.e(66), j.e(588), j.e(0), j.e(271), j.e(222), j.e(456), j.e(185)]).then((() => () => j(4185))))), d("alt", "0.17.9", (() => j.e(554).then((() => () => j(4554))))), d("react-ace", "9.5.0", (() => Promise.all([j.e(981), j.e(271), j.e(697)]).then((() => () => j(4981))))), d("superagent-use", "0.1.0", (() => j.e(174).then((() => () => j(3738))))), d("superagent", "5.3.1", (() => j.e(569).then((() => () => j(569)))))), e[t] = f.length ? Promise.all(f).then((() => e[t] = 1)) : 1
+                    c = [];
+                return "default" === t && (d("@aws-amplify/auth", "4.6.0", (() => Promise.all([j.e(313), j.e(151)]).then((() => () => j(8313))))), d("@emotion/react", "11.10.0", (() => Promise.all([j.e(113), j.e(271), j.e(991)]).then((() => () => j(3113))))), d("@emotion/styled", "11.10.0", (() => Promise.all([j.e(378), j.e(271), j.e(211), j.e(799)]).then((() => () => j(4378))))), d("@mui/icons-material", "5.8.4", (() => Promise.all([j.e(66), j.e(24), j.e(271), j.e(222)]).then((() => () => j(4024))))), d("@mui/material", "5.15.10", (() => Promise.all([j.e(66), j.e(909), j.e(588), j.e(271), j.e(211), j.e(222), j.e(456)]).then((() => () => j(1909))))), d("@qbraid/jupyter-environment-manager", "0.2.0-rc.8", (() => Promise.all([j.e(66), j.e(588), j.e(0), j.e(271), j.e(222), j.e(456), j.e(185)]).then((() => () => j(4185))))), d("alt", "0.17.9", (() => j.e(554).then((() => () => j(4554))))), d("react-ace", "9.5.0", (() => Promise.all([j.e(981), j.e(271), j.e(697)]).then((() => () => j(4981))))), d("superagent-use", "0.1.0", (() => j.e(174).then((() => () => j(3738))))), d("superagent", "5.3.1", (() => j.e(569).then((() => () => j(569)))))), e[t] = c.length ? Promise.all(c).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -197,47 +197,47 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var a = 1, o = 1; o < e.length; o++) a--, t += "u" == (typeof(d = e[o]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, d);
             return t
         }
         var i = [];
         for (o = 1; o < e.length; o++) {
             var d = e[o];
-            i.push(0 === d ? "not(" + f() + ")" : 1 === d ? "(" + f() + " || " + f() + ")" : 2 === d ? i.pop() + " " + i.pop() : n(d))
+            i.push(0 === d ? "not(" + c() + ")" : 1 === d ? "(" + c() + " || " + c() + ")" : 2 === d ? i.pop() + " " + i.pop() : n(d))
         }
-        return f();
+        return c();
 
-        function f() {
+        function c() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 n = a < 0;
             n && (a = -a - 1);
-            for (var i = 0, d = 1, f = !0;; d++, i++) {
-                var l, c, u = d < e.length ? (typeof e[d])[0] : "";
-                if (i >= r.length || "o" == (c = (typeof(l = r[i]))[0])) return !f || ("u" == u ? d > a && !n : "" == u != n);
-                if ("u" == c) {
-                    if (!f || "u" != u) return !1
-                } else if (f)
-                    if (u == c)
+            for (var i = 0, d = 1, c = !0;; d++, i++) {
+                var f, l, u = d < e.length ? (typeof e[d])[0] : "";
+                if (i >= r.length || "o" == (l = (typeof(f = r[i]))[0])) return !c || ("u" == u ? d > a && !n : "" == u != n);
+                if ("u" == l) {
+                    if (!c || "u" != u) return !1
+                } else if (c)
+                    if (u == l)
                         if (d <= a) {
-                            if (l != e[d]) return !1
+                            if (f != e[d]) return !1
                         } else {
-                            if (n ? l > e[d] : l < e[d]) return !1;
-                            l != e[d] && (f = !1)
+                            if (n ? f > e[d] : f < e[d]) return !1;
+                            f != e[d] && (c = !1)
                         }
                 else if ("s" != u && "n" != u) {
                     if (n || d <= a) return !1;
-                    f = !1, d--
+                    c = !1, d--
                 } else {
-                    if (d <= a || c < u != n) return !1;
-                    f = !1
-                } else "s" != u && "n" != u && (f = !1, d--)
+                    if (d <= a || l < u != n) return !1;
+                    c = !1
+                } else "s" != u && "n" != u && (c = !1, d--)
             }
         }
         var s = [],
             b = s.pop.bind(s);
         for (i = 1; i < e.length; i++) {
             var p = e[i];
             s.push(1 == p ? b() | b() : 2 == p ? b() & b() : p ? o(p, r) : !b())
@@ -246,27 +246,27 @@
     }, i = (e, r) => {
         var t = j.S[e];
         if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, d = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || a(e, r) ? r : e), 0)) && t[r]
-    }, f = (e, r) => {
+    }, c = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
-    }, l = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", c = (e, r, t, a) => {
-        var n = f(e, t);
-        return o(a, n) || "undefined" != typeof console && console.warn && console.warn(l(e, t, n, a)), s(e[t][n])
+    }, f = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", l = (e, r, t, a) => {
+        var n = c(e, t);
+        return o(a, n) || "undefined" != typeof console && console.warn && console.warn(f(e, t, n, a)), s(e[t][n])
     }, u = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
     }, s = e => (e.loaded = 1, e.get()), p = (b = e => function(r, t, a, n) {
         var o = j.I(r);
         return o && o.then ? o.then(e.bind(e, r, j.S[r], t, a, n)) : e(r, j.S[r], t, a, n)
-    })(((e, r, t, a) => r && j.o(r, t) ? s(d(r, t)) : a())), h = b(((e, r, t, a) => (i(e, t), c(r, 0, t, a)))), m = b(((e, r, t, a, n) => {
+    })(((e, r, t, a) => r && j.o(r, t) ? s(d(r, t)) : a())), h = b(((e, r, t, a) => (i(e, t), l(r, 0, t, a)))), m = b(((e, r, t, a, n) => {
         var o = r && j.o(r, t) && u(r, t, a);
         return o ? s(o) : n()
     })), v = {}, g = {
         6271: () => h("default", "react", [1, 17, 0, 1]),
         2148: () => m("default", "@emotion/react", [1, 11, 4, 1], (() => Promise.all([j.e(113), j.e(813)]).then((() => () => j(3113))))),
         8800: () => m("default", "@emotion/styled", [1, 11, 3, 0], (() => Promise.all([j.e(378), j.e(211), j.e(799)]).then((() => () => j(4378))))),
         4456: () => h("default", "react-dom", [1, 17, 0, 1]),
@@ -331,20 +331,20 @@
                         i.message = "Loading chunk " + r + " failed.\n(" + n + ": " + o + ")", i.name = "ChunkLoadError", i.type = n, i.request = o, a[1](i)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
                 var a, n, [o, i, d] = t,
-                    f = 0;
+                    c = 0;
                 if (o.some((r => 0 !== e[r]))) {
                     for (a in i) j.o(i, a) && (j.m[a] = i[a]);
                     d && d(j)
                 }
-                for (r && r(t); f < o.length; f++) n = o[f], j.o(e, n) && e[n] && e[n][0](), e[n] = 0
+                for (r && r(t); c < o.length; c++) n = o[c], j.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_qbraid_jupyter_environment_manager = self.webpackChunk_qbraid_jupyter_environment_manager || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), j.nc = void 0;
     var S = j(7413);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@qbraid/jupyter-environment-manager"] = S
 })();
```

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager/labextension/static/third-party-licenses.json` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager.egg-info/PKG-INFO` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_environment_manager
-Version: 0.2.0rc7
+Version: 0.2.0rc8
 Summary: JupyterLab extension for managing execution environments, packages, and kernels.
 Home-page: https://github.com/qBraid/qBraid-Lab
 Author: qBraid Development Team
 Author-email: contact@qbraid.com
 License: Proprietary
 Project-URL: Documentation, https://docs.qbraid.com/projects/lab/en/latest/lab/environments.html
 Project-URL: Bug Tracker, https://github.com/qBraid/qBraid-Lab/issues
@@ -29,15 +29,15 @@
 Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jupyter_server<2,>=1.6
 Requires-Dist: jupyter_client~=7.1.0
 Requires-Dist: tornado>=6.1.0
 Requires-Dist: notebook<7
-Requires-Dist: qbraid-cli
+Requires-Dist: qbraid-core<0.2,>=0.1.3
 
 # jupyter-environment-manager
 
 [![Documentation](https://img.shields.io/badge/Documentation-DF0982)](https://docs.qbraid.com/projects/lab/en/latest/lab/environments.html)
 [![PyPI version](https://img.shields.io/pypi/v/jupyter-environment-manager.svg?color=blue)](https://pypi.org/project/jupyter-environment-manager/)
 [![GitHub](https://img.shields.io/badge/issue_tracking-github-blue?logo=github)](https://github.com/qBraid/qBraid-Lab/issues)
 [![Discord](https://img.shields.io/discord/771898982564626445.svg?color=pink)](https://discord.gg/TPBU2sa8Et)
```

### Comparing `jupyter_environment_manager-0.2.0rc7/jupyter_environment_manager.egg-info/SOURCES.txt` & `jupyter_environment_manager-0.2.0rc8/jupyter_environment_manager.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -19,30 +19,29 @@
 jupyter_environment_manager/envs_list.py
 jupyter_environment_manager/envs_pkgs.py
 jupyter_environment_manager/envs_remove.py
 jupyter_environment_manager/envs_state.py
 jupyter_environment_manager/handlers.py
 jupyter_environment_manager/jobs.py
 jupyter_environment_manager/kernels.py
-jupyter_environment_manager/qbraid_core.py
 jupyter_environment_manager.egg-info/PKG-INFO
 jupyter_environment_manager.egg-info/SOURCES.txt
 jupyter_environment_manager.egg-info/dependency_links.txt
 jupyter_environment_manager.egg-info/not-zip-safe
 jupyter_environment_manager.egg-info/requires.txt
 jupyter_environment_manager.egg-info/top_level.txt
 jupyter_environment_manager/labextension/package.json
 jupyter_environment_manager/labextension/static/0.99dd872e735721a05b18.js
 jupyter_environment_manager/labextension/static/0.99dd872e735721a05b18.js.LICENSE.txt
 jupyter_environment_manager/labextension/static/113.063bb6057d77be1f85f3.js
 jupyter_environment_manager/labextension/static/113.063bb6057d77be1f85f3.js.LICENSE.txt
 jupyter_environment_manager/labextension/static/151.18af1747c52fa1890fce.js
 jupyter_environment_manager/labextension/static/174.7b162c87cb727f7c2712.js
 jupyter_environment_manager/labextension/static/174.7b162c87cb727f7c2712.js.LICENSE.txt
-jupyter_environment_manager/labextension/static/185.4cb0a9019311d36636ce.js
+jupyter_environment_manager/labextension/static/185.5d7f6d37c97924a89805.js
 jupyter_environment_manager/labextension/static/24.a6fec73552ceb9bdb6aa.js
 jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js
 jupyter_environment_manager/labextension/static/313.f6abbabc37aacd77b555.js.LICENSE.txt
 jupyter_environment_manager/labextension/static/378.8fdd4b1246fb17037bb3.js
 jupyter_environment_manager/labextension/static/478.b1efc8dc1ed4a16150ef.js
 jupyter_environment_manager/labextension/static/554.3ee5e631ee6f4d8c24e2.js
 jupyter_environment_manager/labextension/static/569.110780388cdcc5605903.js
@@ -54,15 +53,15 @@
 jupyter_environment_manager/labextension/static/747.6d49dfe38d298a9d88e1.js
 jupyter_environment_manager/labextension/static/813.4baf0234297462c92d8b.js
 jupyter_environment_manager/labextension/static/909.c50074d4e4be5aa7c06a.js
 jupyter_environment_manager/labextension/static/909.c50074d4e4be5aa7c06a.js.LICENSE.txt
 jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js
 jupyter_environment_manager/labextension/static/981.f54a04f7142174f18f0d.js.LICENSE.txt
 jupyter_environment_manager/labextension/static/991.b0c652da28634799e4d5.js
-jupyter_environment_manager/labextension/static/remoteEntry.efb45905ee8f674ba5f4.js
+jupyter_environment_manager/labextension/static/remoteEntry.64b15d2280d9c5210de7.js
 jupyter_environment_manager/labextension/static/style.js
 jupyter_environment_manager/labextension/static/third-party-licenses.json
 src/EnvironmentsSidebarWidget.tsx
 src/Flux.js
 src/assets.d.ts
 src/contextTypes.js
 src/global.d.ts
```

### Comparing `jupyter_environment_manager-0.2.0rc7/package.json` & `jupyter_environment_manager-0.2.0rc8/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9782608695652174%*

 * *Differences: {"'version'": "'0.2.0-rc.8'"}*

```diff
@@ -107,9 +107,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.0-rc.7"
+    "version": "0.2.0-rc.8"
 }
```

### Comparing `jupyter_environment_manager-0.2.0rc7/pyproject.toml` & `jupyter_environment_manager-0.2.0rc8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/setup.py` & `jupyter_environment_manager-0.2.0rc8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=[
         "jupyter_server>=1.6,<2",
         "jupyter_client~=7.1.0",
         "tornado>=6.1.0",
         "notebook<7",
-        "qbraid-cli",
+        "qbraid-core>=0.1.3,<0.2",
     ],
     zip_safe=False,
     include_package_data=True,
     python_requires=">= 3.9",
     platforms="Linux, Mac OS X, Windows",
     keywords=["IPython", "Jupyter", "JupyterLab"],
     classifiers=[
```

### Comparing `jupyter_environment_manager-0.2.0rc7/src/EnvironmentsSidebarWidget.tsx` & `jupyter_environment_manager-0.2.0rc8/src/EnvironmentsSidebarWidget.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/Flux.js` & `jupyter_environment_manager-0.2.0rc8/src/Flux.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/actions/ApiActions.js` & `jupyter_environment_manager-0.2.0rc8/src/actions/ApiActions.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/actions/AuthActions.js` & `jupyter_environment_manager-0.2.0rc8/src/actions/AuthActions.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/actions/EnvironmentActions.js` & `jupyter_environment_manager-0.2.0rc8/src/actions/EnvironmentActions.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -589,15 +589,14 @@
                     .then(data => {
                         if (data.success) {
                             resolve({
                                 success: data.success,
                                 stdout: data.stdout
                             });
                         } else {
-                            console.log(`ERROR: ${data.stderr}`);
                             reject(new Error(`Action failed with error: ${data.stderr}`));
                         }
                     })
                     .catch(err => {
                         const errorMsg = `Error in toggleQuantumJobs: ${err.message}`;
                         return reject(errorMsg);
                     });
```

### Comparing `jupyter_environment_manager-0.2.0rc7/src/actions/JupyterApiActions.js` & `jupyter_environment_manager-0.2.0rc8/src/actions/JupyterApiActions.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/actions/UserActions.js` & `jupyter_environment_manager-0.2.0rc8/src/actions/UserActions.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/assets/icons/BackIcon.tsx` & `jupyter_environment_manager-0.2.0rc8/src/assets/icons/BackIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/assets/icons/CloseIcon.tsx` & `jupyter_environment_manager-0.2.0rc8/src/assets/icons/CloseIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/assets/icons/ConfirmIcon.tsx` & `jupyter_environment_manager-0.2.0rc8/src/assets/icons/ConfirmIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/assets/icons/DescriptionIcon.tsx` & `jupyter_environment_manager-0.2.0rc8/src/assets/icons/DescriptionIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/assets/icons/EnvIcon.tsx` & `jupyter_environment_manager-0.2.0rc8/src/assets/icons/EnvIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/assets/icons/IconString.js` & `jupyter_environment_manager-0.2.0rc8/src/assets/icons/IconString.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/assets/icons/LinkIcon.tsx` & `jupyter_environment_manager-0.2.0rc8/src/assets/icons/LinkIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/assets/icons/Loading.tsx` & `jupyter_environment_manager-0.2.0rc8/src/assets/icons/Loading.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/assets/icons/RefreshIcon.tsx` & `jupyter_environment_manager-0.2.0rc8/src/assets/icons/RefreshIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/assets/icons/SearchIcon.tsx` & `jupyter_environment_manager-0.2.0rc8/src/assets/icons/SearchIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/assets/icons/UserIcon.tsx` & `jupyter_environment_manager-0.2.0rc8/src/assets/icons/UserIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/assets/icons/WhiteCube.tsx` & `jupyter_environment_manager-0.2.0rc8/src/assets/icons/WhiteCube.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/components/EndUserAgreement.js` & `jupyter_environment_manager-0.2.0rc8/src/components/EndUserAgreement.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/components/EnvironmentEditor.js` & `jupyter_environment_manager-0.2.0rc8/src/components/EnvironmentEditor.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -674,15 +674,15 @@
                     const filterPackLength = this.state.packagesInImage.filter(
                         pkg =>
                         pkg
                         .split('=')[0]
                         .toLowerCase()
                         .trim()
                         .indexOf(this.state.packageFilter.replaceAll('-', '')) !== -1
-                    ).length;
+                    ).length; // gets the number of PACKAGES FOUND from the existing list of packages in the current environment
 
                     if (filterPackLength === 0 && !this.props.env.isPreInstalled) {
                         // package not found in env package list
                         this.setState({
                             addPackageDialogOpen: true,
                             packageListLoading: true,
                             searchInput: this.state.packageFilter
@@ -1164,20 +1164,20 @@
                                 open: true,
                                 error: false,
                                 message: `${initialJobsState ? 'Disabled' : 'Enabled'}`
                             }
                         });
                         this.resetQjobsStatus();
                     }
-                    this.context
-                        .getActions('EnvironmentActions')
-                        .registerInstalled()
-                        .catch(err => {
-                            throw new Error(err);
-                        });
+                    // this.context
+                    //   .getActions('EnvironmentActions')
+                    //   .registerInstalled()
+                    //   .catch(err => {
+                    //     throw new Error(err);
+                    //   });
                 })
                 .catch(err => {
                     console.log('Quantum Jobs Toggle Error: ', err);
                     this.setState({
                         qjobsStatus: {
                             open: true,
                             error: true,
@@ -1342,31 +1342,31 @@
                         quantumJobsAdditionSuccess: true
                     });
                     setTimeout(() => {
                         this.context
                             .getActions('EnvironmentActions')
                             .updateAll()
                             .then(() => {
-                                this.context
-                                    .getActions('EnvironmentActions')
-                                    .registerInstalled();
+                                // this.context
+                                //   .getActions('EnvironmentActions')
+                                //   .registerInstalled();
 
                                 this.setState({
                                     quantumJobsAdditionSuccess: false,
                                     quantumJobs: true,
                                     quantumJobsEnabled: true
                                 });
                             });
                     }, 1750);
                 }
             } catch (err) {
                 console.log('Error adding quantum jobs. ', err);
                 alert(
                     'Unable to add quantum jobs at this time. ' +
-                    'Please try again later, and verify that the qbraid-cli ' +
+                    'Please try again later, and verify that qbraid-core ' +
                     'is installed and configured correctly.'
                 );
             }
         };
 
         return ( <
             Stack flexDirection = "row"
@@ -3235,15 +3235,15 @@
                 Grid item xs = {
                     12
                 } >
                 <
                 div className = "env-editor-pane-new"
                 style = {
                     {
-                        minHeight: 50
+                        minHeight: 150
                     }
                 } >
                 <
                 div className = "env-pane-content" > {
                     this.props.packageInstallingEnv === this.props.env._id ? ( <
                         Stack sx = {
                             {
@@ -3283,15 +3283,15 @@
                         spacing = {
                             1
                         } >
                         <
                         Typography className = "env-pane-prompt" > {
                             this.state.cancelling ?
                             'Cancelling installation' :
-                                'Environment is being installed'
+                                'Environment is being installed/updated'
                         } <
                         /Typography> <
                         LinearProgress sx = {
                             {
                                 backgroundColor: this.state.cancelling ?
                                     'red' :
                                     '#9909e091',
@@ -3660,15 +3660,15 @@
                 Grid item xs = {
                     12
                 } >
                 <
                 div className = "env-editor-pane-new"
                 style = {
                     {
-                        minHeight: 50
+                        minHeight: 150
                     }
                 } >
                 <
                 div className = "env-pane-content" >
                 <
                 Button fullWidth variant = "contained"
                 size = "medium"
```

### Comparing `jupyter_environment_manager-0.2.0rc7/src/components/EnvironmentTile.js` & `jupyter_environment_manager-0.2.0rc8/src/components/EnvironmentTile.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/components/EnvironmentsSidebar.js` & `jupyter_environment_manager-0.2.0rc8/src/components/EnvironmentsSidebar.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -296,15 +296,14 @@
             this.aceContainerRef?.current?.offsetWidth !== this?.state?.containerWidth
         ) {
             this.resizeEditor();
             this.setState({
                 containerWidth: this.aceContainerRef?.current?.offsetWidth
             });
         }
-        console.log('selectedEnvironment', this.state.selectedEnvironment);
     }
 
     componentWillUnmount() {
         this.props.flux
             .getStore('EnvironmentStore')
             .unlisten(this.handleUpdateEnvironments);
     }
@@ -1323,19 +1322,19 @@
         this.setState({
             environments: newEnvironment
         });
     };
 
     handleOpenEnvEditorInstalled = (env, installing) => {
         this.openEnvironmentEditor(env);
-        this.setState({
-            packageLoading: true
-        });
         // Don't update package list for envs that use base conda python
         if (env.slug !== 'qsharp_b54crn' && !installing) {
+            this.setState({
+                packageLoading: true
+            });
             this.props.flux
                 .getActions('EnvironmentActions')
                 .updateQuantumJobStatus(env.slug)
                 .catch(err => {
                     console.log('Error updating quantum job status:', err);
                 });
             this.props.flux
```

### Comparing `jupyter_environment_manager-0.2.0rc7/src/components/Loading.js` & `jupyter_environment_manager-0.2.0rc8/src/components/Loading.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/components/LogoLoader.js` & `jupyter_environment_manager-0.2.0rc8/src/components/LogoLoader.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/components/MuiStyledComponents.js` & `jupyter_environment_manager-0.2.0rc8/src/components/MuiStyledComponents.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/components/UserNotFound.js` & `jupyter_environment_manager-0.2.0rc8/src/components/UserNotFound.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/index.ts` & `jupyter_environment_manager-0.2.0rc8/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/stores/AuthStore.js` & `jupyter_environment_manager-0.2.0rc8/src/stores/AuthStore.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/stores/EnvironmentStore.js` & `jupyter_environment_manager-0.2.0rc8/src/stores/EnvironmentStore.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/stores/UserStore.js` & `jupyter_environment_manager-0.2.0rc8/src/stores/UserStore.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/utils/googleAnalytics.js` & `jupyter_environment_manager-0.2.0rc8/src/utils/googleAnalytics.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/src/utils/theme.js` & `jupyter_environment_manager-0.2.0rc8/src/utils/theme.js`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/style/EnvironmentEditor.css` & `jupyter_environment_manager-0.2.0rc8/style/EnvironmentEditor.css`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/style/EnvironmentTile.css` & `jupyter_environment_manager-0.2.0rc8/style/EnvironmentTile.css`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/style/EnvironmentsSidebar.css` & `jupyter_environment_manager-0.2.0rc8/style/EnvironmentsSidebar.css`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 .environments-sidebar-search-pane {
   width: 0%;
   transition: width 300ms ease;
 }
 
 .environments-sidebar-environment-list {
   padding-bottom: 200px;
+  background-color: var(--jp-layout-color1);
 }
 
 .envoronments-sidebar-search-wrapper {
   position: relative;
 }
 
 .environments-sidebar-search-icon {
```

### Comparing `jupyter_environment_manager-0.2.0rc7/style/Loading.css` & `jupyter_environment_manager-0.2.0rc8/style/Loading.css`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/style/LogoLoader.css` & `jupyter_environment_manager-0.2.0rc8/style/LogoLoader.css`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/tools/create_dev_build.sh` & `jupyter_environment_manager-0.2.0rc8/tools/create_dev_build.sh`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/tools/stamp_pre_release.py` & `jupyter_environment_manager-0.2.0rc8/tools/stamp_pre_release.py`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/tsconfig.json` & `jupyter_environment_manager-0.2.0rc8/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_environment_manager-0.2.0rc7/yarn.lock` & `jupyter_environment_manager-0.2.0rc8/yarn.lock`

 * *Files identical despite different names*

