# Comparing `tmp/fortimanager_template_sync-0.0.1.tar.gz` & `tmp/fortimanager_template_sync-0.0.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fortimanager_template_sync-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fortimanager_template_sync-0.0.1.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fortimanager_template_sync-0.0.1.tar` & `fortimanager_template_sync-0.0.1.post1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0      729 2024-03-24 21:11:50.562818 fortimanager_template_sync-0.0.1/.github/workflows/deploy-docs.yml
--rw-r--r--   0        0        0      670 2024-03-24 21:11:50.562818 fortimanager_template_sync-0.0.1/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0      745 2024-03-24 21:11:50.562818 fortimanager_template_sync-0.0.1/.github/workflows/publish-test-pypi.yml
--rw-r--r--   0        0        0      128 2024-03-24 21:11:50.562818 fortimanager_template_sync-0.0.1/.gitignore
--rw-r--r--   0        0        0     1483 2024-03-24 21:11:50.562818 fortimanager_template_sync-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      402 2024-03-24 21:11:50.562818 fortimanager_template_sync-0.0.1/.relint.yml
--rw-r--r--   0        0        0     1069 2024-03-24 21:11:50.562818 fortimanager_template_sync-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1417 2024-03-24 21:11:50.562818 fortimanager_template_sync-0.0.1/README.md
--rw-r--r--   0        0        0      501 2024-03-24 21:11:50.562818 fortimanager_template_sync-0.0.1/docs/README.md
--rw-r--r--   0        0        0     1433 2024-03-24 21:11:50.562818 fortimanager_template_sync-0.0.1/docs/developer_guide/index.md
--rw-r--r--   0        0        0      250 2024-03-24 21:11:50.562818 fortimanager_template_sync-0.0.1/docs/extra.css
--rw-r--r--   0        0        0      903 2024-03-24 21:11:50.562818 fortimanager_template_sync-0.0.1/docs/gen_ref_pages.py
--rw-r--r--   0        0        0     3244 2024-03-24 21:11:50.562818 fortimanager_template_sync-0.0.1/docs/github_guide/github_actions.md
--rw-r--r--   0        0        0     4592 2024-03-24 21:11:50.562818 fortimanager_template_sync-0.0.1/docs/github_guide/github_repository.md
--rw-r--r--   0        0        0     6033 2024-03-24 21:11:50.566818 fortimanager_template_sync-0.0.1/docs/github_guide/github_workflow.md
--rw-r--r--   0        0        0      623 2024-03-24 21:11:50.566818 fortimanager_template_sync-0.0.1/docs/github_guide/index.md
--rw-r--r--   0        0        0    33852 2024-03-24 21:11:50.566818 fortimanager_template_sync-0.0.1/docs/img/create_branch.png
--rw-r--r--   0        0        0    18745 2024-03-24 21:11:50.566818 fortimanager_template_sync-0.0.1/docs/img/jinja_error.png
--rw-r--r--   0        0        0    56588 2024-03-24 21:11:50.566818 fortimanager_template_sync-0.0.1/docs/img/new_repo.png
--rw-r--r--   0        0        0    31684 2024-03-24 21:11:50.566818 fortimanager_template_sync-0.0.1/docs/img/open_pull_request.png
--rw-r--r--   0        0        0    59096 2024-03-24 21:11:50.566818 fortimanager_template_sync-0.0.1/docs/img/pr_details.png
--rw-r--r--   0        0        0    34031 2024-03-24 21:11:50.566818 fortimanager_template_sync-0.0.1/docs/img/pr_files_chg.png
--rw-r--r--   0        0        0    35369 2024-03-24 21:11:50.566818 fortimanager_template_sync-0.0.1/docs/img/pr_log.png
--rw-r--r--   0        0        0    15380 2024-03-24 21:11:50.566818 fortimanager_template_sync-0.0.1/docs/img/protect_branches1.png
--rw-r--r--   0        0        0    23952 2024-03-24 21:11:50.566818 fortimanager_template_sync-0.0.1/docs/img/protect_branches2.png
--rw-r--r--   0        0        0    22963 2024-03-24 21:11:50.566818 fortimanager_template_sync-0.0.1/docs/img/renaming_branch_1.png
--rw-r--r--   0        0        0    19412 2024-03-24 21:11:50.566818 fortimanager_template_sync-0.0.1/docs/img/renaming_branch_2.png
--rw-r--r--   0        0        0    24321 2024-03-24 21:11:50.566818 fortimanager_template_sync-0.0.1/docs/img/review.png
--rw-r--r--   0        0        0    82627 2024-03-24 21:11:50.566818 fortimanager_template_sync-0.0.1/docs/img/win_hyperv.png
--rw-r--r--   0        0        0      150 2024-03-24 21:11:50.566818 fortimanager_template_sync-0.0.1/docs/requirements.txt
--rw-r--r--   0        0        0     4101 2024-03-24 21:11:50.566818 fortimanager_template_sync-0.0.1/docs/user_guide/installation.md
--rw-r--r--   0        0        0     2859 2024-03-24 21:11:50.566818 fortimanager_template_sync-0.0.1/docs/user_guide/lab_setup.md
--rw-r--r--   0        0        0     9981 2024-03-24 21:11:50.566818 fortimanager_template_sync-0.0.1/docs/user_guide/quickstart.md
--rw-r--r--   0        0        0     4563 2024-03-24 21:11:50.566818 fortimanager_template_sync-0.0.1/docs/user_guide/repository.md
--rw-r--r--   0        0        0       56 2024-03-24 21:11:50.570818 fortimanager_template_sync-0.0.1/fortimanager_template_sync/__init__.py
--rw-r--r--   0        0        0     1928 2024-03-24 21:11:50.570818 fortimanager_template_sync-0.0.1/fortimanager_template_sync/__main__.py
--rw-r--r--   0        0        0     3944 2024-03-24 21:11:50.570818 fortimanager_template_sync-0.0.1/fortimanager_template_sync/common_task.py
--rw-r--r--   0        0        0     1808 2024-03-24 21:11:50.570818 fortimanager_template_sync-0.0.1/fortimanager_template_sync/config.py
--rw-r--r--   0        0        0     2932 2024-03-24 21:11:50.570818 fortimanager_template_sync-0.0.1/fortimanager_template_sync/deploy_run.py
--rw-r--r--   0        0        0     5907 2024-03-24 21:11:50.570818 fortimanager_template_sync-0.0.1/fortimanager_template_sync/deploy_task.py
--rw-r--r--   0        0        0      581 2024-03-24 21:11:50.570818 fortimanager_template_sync-0.0.1/fortimanager_template_sync/exceptions.py
--rw-r--r--   0        0        0      115 2024-03-24 21:11:50.570818 fortimanager_template_sync-0.0.1/fortimanager_template_sync/fmg_api/__init__.py
--rw-r--r--   0        0        0    14908 2024-03-24 21:11:50.570818 fortimanager_template_sync-0.0.1/fortimanager_template_sync/fmg_api/connection.py
--rw-r--r--   0        0        0     5622 2024-03-24 21:11:50.570818 fortimanager_template_sync-0.0.1/fortimanager_template_sync/fmg_api/data.py
--rw-r--r--   0        0        0     2534 2024-03-24 21:11:50.570818 fortimanager_template_sync-0.0.1/fortimanager_template_sync/misc.py
--rw-r--r--   0        0        0     2921 2024-03-24 21:11:50.570818 fortimanager_template_sync-0.0.1/fortimanager_template_sync/sync_run.py
--rw-r--r--   0        0        0    20774 2024-03-24 21:11:50.570818 fortimanager_template_sync-0.0.1/fortimanager_template_sync/sync_task.py
--rw-r--r--   0        0        0     2895 2024-03-24 21:11:50.570818 fortimanager_template_sync-0.0.1/mkdocs.yml
--rw-r--r--   0        0        0     3095 2024-03-24 21:11:50.570818 fortimanager_template_sync-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1701 2024-03-24 21:11:50.570818 fortimanager_template_sync-0.0.1/tasks.py
--rw-r--r--   0        0        0     1253 2024-03-24 21:11:50.570818 fortimanager_template_sync-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0     5477 2024-03-24 21:11:50.570818 fortimanager_template_sync-0.0.1/tests/test_fmg_api.py
--rw-r--r--   0        0        0      996 2024-03-24 21:11:50.570818 fortimanager_template_sync-0.0.1/tests/test_full_run.py
--rw-r--r--   0        0        0     4913 2024-03-24 21:11:50.570818 fortimanager_template_sync-0.0.1/tests/test_git.py
--rw-r--r--   0        0        0     4820 2024-03-24 21:11:50.570818 fortimanager_template_sync-0.0.1/tests/test_helpers.py
--rw-r--r--   0        0        0     3022 1970-01-01 00:00:00.000000 fortimanager_template_sync-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      729 2024-04-17 10:53:31.320528 fortimanager_template_sync-0.0.1.post1/.github/workflows/deploy-docs.yml
+-rw-r--r--   0        0        0      670 2024-04-17 10:53:31.320528 fortimanager_template_sync-0.0.1.post1/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0      745 2024-04-17 10:53:31.320528 fortimanager_template_sync-0.0.1.post1/.github/workflows/publish-test-pypi.yml
+-rw-r--r--   0        0        0      128 2024-04-17 10:53:31.320528 fortimanager_template_sync-0.0.1.post1/.gitignore
+-rw-r--r--   0        0        0     1483 2024-04-17 10:53:31.324528 fortimanager_template_sync-0.0.1.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      402 2024-04-17 10:53:31.324528 fortimanager_template_sync-0.0.1.post1/.relint.yml
+-rw-r--r--   0        0        0     1069 2024-04-17 10:53:31.324528 fortimanager_template_sync-0.0.1.post1/LICENSE.txt
+-rw-r--r--   0        0        0     1417 2024-04-17 10:53:31.324528 fortimanager_template_sync-0.0.1.post1/README.md
+-rw-r--r--   0        0        0      501 2024-04-17 10:53:31.324528 fortimanager_template_sync-0.0.1.post1/docs/README.md
+-rw-r--r--   0        0        0     1433 2024-04-17 10:53:31.324528 fortimanager_template_sync-0.0.1.post1/docs/developer_guide/index.md
+-rw-r--r--   0        0        0      250 2024-04-17 10:53:31.324528 fortimanager_template_sync-0.0.1.post1/docs/extra.css
+-rw-r--r--   0        0        0      903 2024-04-17 10:53:31.324528 fortimanager_template_sync-0.0.1.post1/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0     3244 2024-04-17 10:53:31.324528 fortimanager_template_sync-0.0.1.post1/docs/github_guide/github_actions.md
+-rw-r--r--   0        0        0     4592 2024-04-17 10:53:31.324528 fortimanager_template_sync-0.0.1.post1/docs/github_guide/github_repository.md
+-rw-r--r--   0        0        0     6033 2024-04-17 10:53:31.324528 fortimanager_template_sync-0.0.1.post1/docs/github_guide/github_workflow.md
+-rw-r--r--   0        0        0      623 2024-04-17 10:53:31.324528 fortimanager_template_sync-0.0.1.post1/docs/github_guide/index.md
+-rw-r--r--   0        0        0    33852 2024-04-17 10:53:31.324528 fortimanager_template_sync-0.0.1.post1/docs/img/create_branch.png
+-rw-r--r--   0        0        0    18745 2024-04-17 10:53:31.324528 fortimanager_template_sync-0.0.1.post1/docs/img/jinja_error.png
+-rw-r--r--   0        0        0    56588 2024-04-17 10:53:31.324528 fortimanager_template_sync-0.0.1.post1/docs/img/new_repo.png
+-rw-r--r--   0        0        0    31684 2024-04-17 10:53:31.324528 fortimanager_template_sync-0.0.1.post1/docs/img/open_pull_request.png
+-rw-r--r--   0        0        0    59096 2024-04-17 10:53:31.324528 fortimanager_template_sync-0.0.1.post1/docs/img/pr_details.png
+-rw-r--r--   0        0        0    34031 2024-04-17 10:53:31.324528 fortimanager_template_sync-0.0.1.post1/docs/img/pr_files_chg.png
+-rw-r--r--   0        0        0    35369 2024-04-17 10:53:31.324528 fortimanager_template_sync-0.0.1.post1/docs/img/pr_log.png
+-rw-r--r--   0        0        0    15380 2024-04-17 10:53:31.324528 fortimanager_template_sync-0.0.1.post1/docs/img/protect_branches1.png
+-rw-r--r--   0        0        0    23952 2024-04-17 10:53:31.324528 fortimanager_template_sync-0.0.1.post1/docs/img/protect_branches2.png
+-rw-r--r--   0        0        0    22963 2024-04-17 10:53:31.324528 fortimanager_template_sync-0.0.1.post1/docs/img/renaming_branch_1.png
+-rw-r--r--   0        0        0    19412 2024-04-17 10:53:31.324528 fortimanager_template_sync-0.0.1.post1/docs/img/renaming_branch_2.png
+-rw-r--r--   0        0        0    24321 2024-04-17 10:53:31.324528 fortimanager_template_sync-0.0.1.post1/docs/img/review.png
+-rw-r--r--   0        0        0    82627 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/docs/img/win_hyperv.png
+-rw-r--r--   0        0        0      150 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/docs/requirements.txt
+-rw-r--r--   0        0        0     4101 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/docs/user_guide/installation.md
+-rw-r--r--   0        0        0     2859 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/docs/user_guide/lab_setup.md
+-rw-r--r--   0        0        0     9981 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/docs/user_guide/quickstart.md
+-rw-r--r--   0        0        0     4563 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/docs/user_guide/repository.md
+-rw-r--r--   0        0        0       62 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/fortimanager_template_sync/__init__.py
+-rw-r--r--   0        0        0     1928 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/fortimanager_template_sync/__main__.py
+-rw-r--r--   0        0        0     3944 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/fortimanager_template_sync/common_task.py
+-rw-r--r--   0        0        0     1808 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/fortimanager_template_sync/config.py
+-rw-r--r--   0        0        0     2932 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/fortimanager_template_sync/deploy_run.py
+-rw-r--r--   0        0        0     5907 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/fortimanager_template_sync/deploy_task.py
+-rw-r--r--   0        0        0      581 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/fortimanager_template_sync/exceptions.py
+-rw-r--r--   0        0        0      115 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/fortimanager_template_sync/fmg_api/__init__.py
+-rw-r--r--   0        0        0    14908 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/fortimanager_template_sync/fmg_api/connection.py
+-rw-r--r--   0        0        0     5622 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/fortimanager_template_sync/fmg_api/data.py
+-rw-r--r--   0        0        0     2534 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/fortimanager_template_sync/misc.py
+-rw-r--r--   0        0        0     2921 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/fortimanager_template_sync/sync_run.py
+-rw-r--r--   0        0        0    20774 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/fortimanager_template_sync/sync_task.py
+-rw-r--r--   0        0        0     2905 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/mkdocs.yml
+-rw-r--r--   0        0        0     3116 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/pyproject.toml
+-rw-r--r--   0        0        0     1701 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/tasks.py
+-rw-r--r--   0        0        0     1253 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/tests/conftest.py
+-rw-r--r--   0        0        0     5477 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/tests/test_fmg_api.py
+-rw-r--r--   0        0        0      996 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/tests/test_full_run.py
+-rw-r--r--   0        0        0     4913 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/tests/test_git.py
+-rw-r--r--   0        0        0     4820 2024-04-17 10:53:31.328528 fortimanager_template_sync-0.0.1.post1/tests/test_helpers.py
+-rw-r--r--   0        0        0     3057 1970-01-01 00:00:00.000000 fortimanager_template_sync-0.0.1.post1/PKG-INFO
```

### Comparing `fortimanager_template_sync-0.0.1/.github/workflows/deploy-docs.yml` & `fortimanager_template_sync-0.0.1.post1/.github/workflows/deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/.github/workflows/publish-pypi.yml` & `fortimanager_template_sync-0.0.1.post1/.github/workflows/publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/.github/workflows/publish-test-pypi.yml` & `fortimanager_template_sync-0.0.1.post1/.github/workflows/publish-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/.pre-commit-config.yaml` & `fortimanager_template_sync-0.0.1.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/LICENSE.txt` & `fortimanager_template_sync-0.0.1.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/README.md` & `fortimanager_template_sync-0.0.1.post1/README.md`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/docs/developer_guide/index.md` & `fortimanager_template_sync-0.0.1.post1/docs/developer_guide/index.md`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/docs/gen_ref_pages.py` & `fortimanager_template_sync-0.0.1.post1/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/docs/github_guide/github_actions.md` & `fortimanager_template_sync-0.0.1.post1/docs/github_guide/github_actions.md`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/docs/github_guide/github_repository.md` & `fortimanager_template_sync-0.0.1.post1/docs/github_guide/github_repository.md`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/docs/github_guide/github_workflow.md` & `fortimanager_template_sync-0.0.1.post1/docs/github_guide/github_workflow.md`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/docs/github_guide/index.md` & `fortimanager_template_sync-0.0.1.post1/docs/github_guide/index.md`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/docs/img/create_branch.png` & `fortimanager_template_sync-0.0.1.post1/docs/img/create_branch.png`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/docs/img/jinja_error.png` & `fortimanager_template_sync-0.0.1.post1/docs/img/jinja_error.png`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/docs/img/new_repo.png` & `fortimanager_template_sync-0.0.1.post1/docs/img/new_repo.png`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/docs/img/open_pull_request.png` & `fortimanager_template_sync-0.0.1.post1/docs/img/open_pull_request.png`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/docs/img/pr_details.png` & `fortimanager_template_sync-0.0.1.post1/docs/img/pr_details.png`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/docs/img/pr_files_chg.png` & `fortimanager_template_sync-0.0.1.post1/docs/img/pr_files_chg.png`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/docs/img/pr_log.png` & `fortimanager_template_sync-0.0.1.post1/docs/img/pr_log.png`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/docs/img/protect_branches1.png` & `fortimanager_template_sync-0.0.1.post1/docs/img/protect_branches1.png`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/docs/img/protect_branches2.png` & `fortimanager_template_sync-0.0.1.post1/docs/img/protect_branches2.png`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/docs/img/renaming_branch_1.png` & `fortimanager_template_sync-0.0.1.post1/docs/img/renaming_branch_1.png`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/docs/img/renaming_branch_2.png` & `fortimanager_template_sync-0.0.1.post1/docs/img/renaming_branch_2.png`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/docs/img/review.png` & `fortimanager_template_sync-0.0.1.post1/docs/img/review.png`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/docs/img/win_hyperv.png` & `fortimanager_template_sync-0.0.1.post1/docs/img/win_hyperv.png`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/docs/user_guide/installation.md` & `fortimanager_template_sync-0.0.1.post1/docs/user_guide/installation.md`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/docs/user_guide/lab_setup.md` & `fortimanager_template_sync-0.0.1.post1/docs/user_guide/lab_setup.md`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/docs/user_guide/quickstart.md` & `fortimanager_template_sync-0.0.1.post1/docs/user_guide/quickstart.md`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/docs/user_guide/repository.md` & `fortimanager_template_sync-0.0.1.post1/docs/user_guide/repository.md`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/fortimanager_template_sync/__main__.py` & `fortimanager_template_sync-0.0.1.post1/fortimanager_template_sync/__main__.py`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/fortimanager_template_sync/common_task.py` & `fortimanager_template_sync-0.0.1.post1/fortimanager_template_sync/common_task.py`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/fortimanager_template_sync/config.py` & `fortimanager_template_sync-0.0.1.post1/fortimanager_template_sync/config.py`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/fortimanager_template_sync/deploy_run.py` & `fortimanager_template_sync-0.0.1.post1/fortimanager_template_sync/deploy_run.py`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/fortimanager_template_sync/deploy_task.py` & `fortimanager_template_sync-0.0.1.post1/fortimanager_template_sync/deploy_task.py`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/fortimanager_template_sync/exceptions.py` & `fortimanager_template_sync-0.0.1.post1/fortimanager_template_sync/exceptions.py`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/fortimanager_template_sync/fmg_api/connection.py` & `fortimanager_template_sync-0.0.1.post1/fortimanager_template_sync/fmg_api/connection.py`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/fortimanager_template_sync/fmg_api/data.py` & `fortimanager_template_sync-0.0.1.post1/fortimanager_template_sync/fmg_api/data.py`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/fortimanager_template_sync/misc.py` & `fortimanager_template_sync-0.0.1.post1/fortimanager_template_sync/misc.py`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/fortimanager_template_sync/sync_run.py` & `fortimanager_template_sync-0.0.1.post1/fortimanager_template_sync/sync_run.py`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/fortimanager_template_sync/sync_task.py` & `fortimanager_template_sync-0.0.1.post1/fortimanager_template_sync/sync_task.py`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/mkdocs.yml` & `fortimanager_template_sync-0.0.1.post1/mkdocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
 site_name: Fortimanager Template Sync
 site_description: Supporting of Fortinet CLI template development and deployment
 site_author: Viktor Kertesz
-site_url: https://fortimanager-template-sync.github.io/
+site_url: https://realvitya.github.io/fortimanager-template-sync/
 
 repo_name: realvitya/fortimanager-template-sync
 repo_url: https://github.com/realvitya/fortimanager-template-sync
 
 theme:
   name: material
   palette:
```

### Comparing `fortimanager_template_sync-0.0.1/pyproject.toml` & `fortimanager_template_sync-0.0.1.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     "pydantic>2,<3",
     "typer",
     "pydantic-settings",
     "more-itertools",
     "pyfortinet",
     "jinja2",
     "ruamel.yaml",
+    "python-dotenv",
 ]
 
 [project.optional-dependencies]
 dev = [
 #    "black",
     "pytest-cov",
     "pytest",
```

### Comparing `fortimanager_template_sync-0.0.1/tasks.py` & `fortimanager_template_sync-0.0.1.post1/tasks.py`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/tests/conftest.py` & `fortimanager_template_sync-0.0.1.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/tests/test_fmg_api.py` & `fortimanager_template_sync-0.0.1.post1/tests/test_fmg_api.py`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/tests/test_full_run.py` & `fortimanager_template_sync-0.0.1.post1/tests/test_full_run.py`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/tests/test_git.py` & `fortimanager_template_sync-0.0.1.post1/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/tests/test_helpers.py` & `fortimanager_template_sync-0.0.1.post1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `fortimanager_template_sync-0.0.1/PKG-INFO` & `fortimanager_template_sync-0.0.1.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortimanager_template_sync
-Version: 0.0.1
+Version: 0.0.1.post1
 Summary: FortiManager Template Sync
 Author-email: Viktor Kertesz <vkertesz2@gmail.com>
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
@@ -14,14 +14,15 @@
 Requires-Dist: pydantic>2,<3
 Requires-Dist: typer
 Requires-Dist: pydantic-settings
 Requires-Dist: more-itertools
 Requires-Dist: pyfortinet
 Requires-Dist: jinja2
 Requires-Dist: ruamel.yaml
+Requires-Dist: python-dotenv
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-dependency ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
 Requires-Dist: invoke ; extra == "dev"
 Requires-Dist: ruff ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
```

