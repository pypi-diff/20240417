# Comparing `tmp/patchwork_cli-0.0.5.tar.gz` & `tmp/patchwork_cli-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patchwork_cli-0.0.5.tar", max compression
+gzip compressed data, was "patchwork_cli-0.0.6.tar", max compression
```

## Comparing `patchwork_cli-0.0.5.tar` & `patchwork_cli-0.0.6.tar`

### file list

```diff
@@ -1,92 +1,93 @@
--rw-r--r--   0        0        0    34523 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/LICENSE
--rw-r--r--   0        0        0     5534 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/README.md
--rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/__main__.py
--rw-r--r--   0        0        0     3036 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/app.py
--rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/common/client/__init__.py
--rw-r--r--   0        0        0    12704 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/common/client/scm.py
--rw-r--r--   0        0        0      816 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/common/utils.py
--rw-r--r--   0        0        0     1546 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/logger.py
--rw-r--r--   0        0        0      168 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/managed_files.py
--rw-r--r--   0        0        0     2775 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/AutoFix/AutoFix.py
--rw-r--r--   0        0        0     4783 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/AutoFix/README.md
--rw-r--r--   0        0        0     2182 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/AutoFix/default_prompt.json
--rw-r--r--   0        0        0      809 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/AutoFix/defaults.yml
--rw-r--r--   0        0        0     5434 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py
--rw-r--r--   0        0        0     5418 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/DependencyUpgrade/README.md
--rw-r--r--   0        0        0      704 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/DependencyUpgrade/defaults.yml
--rw-r--r--   0        0        0     2495 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json
--rw-r--r--   0        0        0     2210 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/GenerateREADME/GenerateREADME.py
--rw-r--r--   0        0        0     3832 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/GenerateREADME/README.md
--rw-r--r--   0        0        0      612 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/GenerateREADME/defaults.yml
--rw-r--r--   0        0        0      484 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/GenerateREADME/generate_readme_prompt.json
--rw-r--r--   0        0        0     3551 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/PRReview/PRReview.py
--rw-r--r--   0        0        0     3631 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/PRReview/README.md
--rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/PRReview/__init__.py
--rw-r--r--   0        0        0      608 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/PRReview/defaults.yml
--rw-r--r--   0        0        0      557 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/PRReview/pr_review_prompt.json
--rw-r--r--   0        0        0     2163 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/README.md
--rw-r--r--   0        0        0      276 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/patchflows/__init__.py
--rw-r--r--   0        0        0      499 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/step.py
--rw-r--r--   0        0        0     5970 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py
--rw-r--r--   0        0        0     1205 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/AnalyzeImpact/README.md
--rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/AnalyzeImpact/__init__.py
--rw-r--r--   0        0        0     2437 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py
--rw-r--r--   0        0        0      967 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CallCode2Prompt/README.md
--rw-r--r--   0        0        0      575 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py
--rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CallCode2Prompt/__init__.py
--rw-r--r--   0        0        0     3853 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CallOpenAI/CallOpenAI.py
--rw-r--r--   0        0        0      503 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CallOpenAI/README.md
--rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CallOpenAI/__init__.py
--rw-r--r--   0        0        0     5255 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CommitChanges/CommitChanges.py
--rw-r--r--   0        0        0     1106 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CommitChanges/README.md
--rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CommitChanges/__init__.py
--rw-r--r--   0        0        0     3907 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CreatePR/CreatePR.py
--rw-r--r--   0        0        0     1279 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CreatePR/README.md
--rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CreatePR/__init__.py
--rw-r--r--   0        0        0     1358 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CreatePRComment/CreatePRComment.py
--rw-r--r--   0        0        0      621 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CreatePRComment/README.md
--rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/CreatePRComment/__init__.py
--rw-r--r--   0        0        0     8519 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractCode/ExtractCode.py
--rw-r--r--   0        0        0      755 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractCode/README.md
--rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractCode/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractCode/context_strategy/__init__.py
--rw-r--r--   0        0        0     2585 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractCode/context_strategy/context_strategies.py
--rw-r--r--   0        0        0      593 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractCode/context_strategy/generic.py
--rw-r--r--   0        0        0     1491 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractCode/context_strategy/java.py
--rw-r--r--   0        0        0     2442 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractCode/context_strategy/javascript.py
--rw-r--r--   0        0        0      281 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractCode/context_strategy/protocol.py
--rw-r--r--   0        0        0     2885 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractCode/context_strategy/python.py
--rw-r--r--   0        0        0     8880 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractDiff/ExtractDiff.py
--rw-r--r--   0        0        0      833 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractDiff/README.md
--rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractDiff/__init__.py
--rw-r--r--   0        0        0     1648 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py
--rw-r--r--   0        0        0     1318 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractModelResponse/README.md
--rw-r--r--   0        0        0        0 2024-04-12 11:48:07.610295 patchwork_cli-0.0.5/patchwork/steps/ExtractModelResponse/__init__.py
--rw-r--r--   0        0        0    12392 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py
--rw-r--r--   0        0        0     1765 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ExtractPackageManagerFile/README.md
--rw-r--r--   0        0        0     6173 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py
--rw-r--r--   0        0        0        0 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ExtractPackageManagerFile/__init__.py
--rw-r--r--   0        0        0     3366 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ModifyCode/ModifyCode.py
--rw-r--r--   0        0        0     1045 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ModifyCode/README.md
--rw-r--r--   0        0        0        0 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ModifyCode/__init__.py
--rw-r--r--   0        0        0     3122 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/PreparePR/PreparePR.py
--rw-r--r--   0        0        0      743 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/PreparePR/README.md
--rw-r--r--   0        0        0        0 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/PreparePR/__init__.py
--rw-r--r--   0        0        0     3182 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/PreparePrompt/PreparePrompt.py
--rw-r--r--   0        0        0     1274 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/PreparePrompt/README.md
--rw-r--r--   0        0        0        0 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/PreparePrompt/__init__.py
--rw-r--r--   0        0        0     1652 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/README.md
--rw-r--r--   0        0        0      903 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ReadPRDiffs/README.md
--rw-r--r--   0        0        0     1764 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ReadPRDiffs/ReadPRDiffs.py
--rw-r--r--   0        0        0        0 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ReadPRDiffs/__init__.py
--rw-r--r--   0        0        0     1588 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ScanDepscan/README.md
--rw-r--r--   0        0        0     4744 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ScanDepscan/ScanDepscan.py
--rw-r--r--   0        0        0     2026 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ScanDepscan/TestScanDepscan.py
--rw-r--r--   0        0        0        0 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ScanDepscan/__init__.py
--rw-r--r--   0        0        0      677 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ScanSemgrep/README.md
--rw-r--r--   0        0        0     1055 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ScanSemgrep/ScanSemgrep.py
--rw-r--r--   0        0        0        0 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/ScanSemgrep/__init__.py
--rw-r--r--   0        0        0     1481 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/patchwork/steps/__init__.py
--rw-r--r--   0        0        0     2101 2024-04-12 11:48:07.614295 patchwork_cli-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     7213 1970-01-01 00:00:00.000000 patchwork_cli-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/LICENSE
+-rw-r--r--   0        0        0     5534 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/__main__.py
+-rw-r--r--   0        0        0     3953 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/app.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/common/client/__init__.py
+-rw-r--r--   0        0        0    12704 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/common/client/scm.py
+-rw-r--r--   0        0        0      816 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/common/utils.py
+-rw-r--r--   0        0        0     1548 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/interpreter.py
+-rw-r--r--   0        0        0     1546 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/logger.py
+-rw-r--r--   0        0        0      168 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/managed_files.py
+-rw-r--r--   0        0        0     3724 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/AutoFix/AutoFix.py
+-rw-r--r--   0        0        0     4783 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/AutoFix/README.md
+-rw-r--r--   0        0        0     2182 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/AutoFix/default_prompt.json
+-rw-r--r--   0        0        0      869 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/AutoFix/defaults.yml
+-rw-r--r--   0        0        0     5434 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py
+-rw-r--r--   0        0        0     5418 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/DependencyUpgrade/README.md
+-rw-r--r--   0        0        0      704 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/DependencyUpgrade/defaults.yml
+-rw-r--r--   0        0        0     2495 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json
+-rw-r--r--   0        0        0     2210 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/GenerateREADME/GenerateREADME.py
+-rw-r--r--   0        0        0     3834 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/GenerateREADME/README.md
+-rw-r--r--   0        0        0      612 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/GenerateREADME/defaults.yml
+-rw-r--r--   0        0        0      484 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/GenerateREADME/generate_readme_prompt.json
+-rw-r--r--   0        0        0     3551 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/PRReview/PRReview.py
+-rw-r--r--   0        0        0     3631 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/PRReview/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/PRReview/__init__.py
+-rw-r--r--   0        0        0      608 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/PRReview/defaults.yml
+-rw-r--r--   0        0        0      557 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/PRReview/pr_review_prompt.json
+-rw-r--r--   0        0        0     2163 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/README.md
+-rw-r--r--   0        0        0      276 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/patchflows/__init__.py
+-rw-r--r--   0        0        0      499 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/step.py
+-rw-r--r--   0        0        0     5970 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py
+-rw-r--r--   0        0        0     1205 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/AnalyzeImpact/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/AnalyzeImpact/__init__.py
+-rw-r--r--   0        0        0     2437 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py
+-rw-r--r--   0        0        0      967 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CallCode2Prompt/README.md
+-rw-r--r--   0        0        0      575 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CallCode2Prompt/__init__.py
+-rw-r--r--   0        0        0     4131 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CallOpenAI/CallOpenAI.py
+-rw-r--r--   0        0        0      503 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CallOpenAI/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CallOpenAI/__init__.py
+-rw-r--r--   0        0        0     5255 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CommitChanges/CommitChanges.py
+-rw-r--r--   0        0        0     1106 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CommitChanges/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CommitChanges/__init__.py
+-rw-r--r--   0        0        0     3907 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CreatePR/CreatePR.py
+-rw-r--r--   0        0        0     1279 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CreatePR/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CreatePR/__init__.py
+-rw-r--r--   0        0        0     1358 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CreatePRComment/CreatePRComment.py
+-rw-r--r--   0        0        0      621 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CreatePRComment/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/CreatePRComment/__init__.py
+-rw-r--r--   0        0        0    11565 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractCode/ExtractCode.py
+-rw-r--r--   0        0        0      755 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractCode/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractCode/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractCode/context_strategy/__init__.py
+-rw-r--r--   0        0        0     2585 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractCode/context_strategy/context_strategies.py
+-rw-r--r--   0        0        0      593 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractCode/context_strategy/generic.py
+-rw-r--r--   0        0        0     1491 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractCode/context_strategy/java.py
+-rw-r--r--   0        0        0     2442 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractCode/context_strategy/javascript.py
+-rw-r--r--   0        0        0      281 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractCode/context_strategy/protocol.py
+-rw-r--r--   0        0        0     2885 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractCode/context_strategy/python.py
+-rw-r--r--   0        0        0     8880 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractDiff/ExtractDiff.py
+-rw-r--r--   0        0        0      833 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractDiff/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractDiff/__init__.py
+-rw-r--r--   0        0        0     1648 2024-04-17 00:20:00.922293 patchwork_cli-0.0.6/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py
+-rw-r--r--   0        0        0     1318 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ExtractModelResponse/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ExtractModelResponse/__init__.py
+-rw-r--r--   0        0        0    12392 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py
+-rw-r--r--   0        0        0     1765 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ExtractPackageManagerFile/README.md
+-rw-r--r--   0        0        0     6173 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ExtractPackageManagerFile/__init__.py
+-rw-r--r--   0        0        0     3366 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ModifyCode/ModifyCode.py
+-rw-r--r--   0        0        0     1045 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ModifyCode/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ModifyCode/__init__.py
+-rw-r--r--   0        0        0     3122 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/PreparePR/PreparePR.py
+-rw-r--r--   0        0        0      743 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/PreparePR/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/PreparePR/__init__.py
+-rw-r--r--   0        0        0     3262 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/PreparePrompt/PreparePrompt.py
+-rw-r--r--   0        0        0     1274 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/PreparePrompt/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/PreparePrompt/__init__.py
+-rw-r--r--   0        0        0     1652 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/README.md
+-rw-r--r--   0        0        0      903 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ReadPRDiffs/README.md
+-rw-r--r--   0        0        0     1764 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ReadPRDiffs/ReadPRDiffs.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ReadPRDiffs/__init__.py
+-rw-r--r--   0        0        0     1588 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ScanDepscan/README.md
+-rw-r--r--   0        0        0     4744 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ScanDepscan/ScanDepscan.py
+-rw-r--r--   0        0        0     2026 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ScanDepscan/TestScanDepscan.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ScanDepscan/__init__.py
+-rw-r--r--   0        0        0      677 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ScanSemgrep/README.md
+-rw-r--r--   0        0        0     1055 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ScanSemgrep/ScanSemgrep.py
+-rw-r--r--   0        0        0        0 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/ScanSemgrep/__init__.py
+-rw-r--r--   0        0        0     1481 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/patchwork/steps/__init__.py
+-rw-r--r--   0        0        0     2243 2024-04-17 00:20:00.926293 patchwork_cli-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     7213 1970-01-01 00:00:00.000000 patchwork_cli-0.0.6/PKG-INFO
```

### Comparing `patchwork_cli-0.0.5/LICENSE` & `patchwork_cli-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/README.md` & `patchwork_cli-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/common/client/scm.py` & `patchwork_cli-0.0.6/patchwork/common/client/scm.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/common/utils.py` & `patchwork_cli-0.0.6/patchwork/common/utils.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/logger.py` & `patchwork_cli-0.0.6/patchwork/logger.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/patchflows/AutoFix/AutoFix.py` & `patchwork_cli-0.0.6/patchwork/patchflows/GenerateREADME/GenerateREADME.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,65 @@
-import json
 from pathlib import Path
 
 import yaml
 
 from patchwork.step import Step
 from patchwork.steps import (
+    CallCode2Prompt,
     CallOpenAI,
     CommitChanges,
     CreatePR,
-    ExtractCode,
     ExtractModelResponse,
     ModifyCode,
     PreparePR,
     PreparePrompt,
-    ScanSemgrep,
 )
 
-_DEFAULT_PROMPT_JSON = Path(__file__).parent / "default_prompt.json"
+_DEFAULT_PROMPT_JSON = Path(__file__).parent / "generate_readme_prompt.json"
 _DEFAULT_INPUT_FILE = Path(__file__).parent / "defaults.yml"
 
 
-class AutoFix(Step):
+class GenerateREADME(Step):
     def __init__(self, inputs: dict):
         final_inputs = yaml.safe_load(_DEFAULT_INPUT_FILE.read_text())
         final_inputs.update(inputs)
 
-        self.n = int(final_inputs.get("n", 1))
-        if "prompt_id" not in final_inputs.keys():
-            final_inputs["prompt_id"] = "fixprompt"
+        if "branch_prefix" not in final_inputs.keys():
+            final_inputs["branch_prefix"] = f"{self.__class__.__name__.lower()}-"
 
         if "prompt_template_file" not in final_inputs.keys():
             final_inputs["prompt_template_file"] = _DEFAULT_PROMPT_JSON
 
-        final_inputs["response_partitions"] = {
-            "commit_message": ["A. Commit message:", "B. Change summary:"],
-            "patch_message": ["B. Change summary:", "C. Compatibility Risk:"],
-            "patch": ["D. Fixed Code:", "```", "\n", "```"],
-        }
+        if "prompt_id" not in final_inputs.keys():
+            final_inputs["prompt_id"] = "generateREADME"
+
+        if "folder_path" not in final_inputs.keys():
+            final_inputs["folder_path"] = Path.cwd()
+        else:
+            final_inputs["folder_path"] = Path(final_inputs["folder_path"])
+
         final_inputs["pr_title"] = f"PatchWork {self.__class__.__name__}"
-        final_inputs["branch_prefix"] = f"{self.__class__.__name__.lower()}-"
 
         self.inputs = final_inputs
 
     def run(self) -> dict:
-        outputs = ScanSemgrep(self.inputs).run()
+        outputs = CallCode2Prompt(self.inputs).run()
         self.inputs.update(outputs)
-        outputs = ExtractCode(self.inputs).run()
+        self.inputs["response_partitions"] = {"patch": []}
+        outputs = PreparePrompt(self.inputs).run()
+        self.inputs.update(outputs)
+        outputs = CallOpenAI(self.inputs).run()
+        self.inputs.update(outputs)
+        outputs = ExtractModelResponse(self.inputs).run()
+        self.inputs.update(outputs)
+        outputs = ModifyCode(self.inputs).run()
         self.inputs.update(outputs)
 
-        for i in range(self.n):
-            outputs = PreparePrompt(self.inputs).run()
-            self.inputs.update(outputs)
-            outputs = CallOpenAI(self.inputs).run()
-            self.inputs.update(outputs)
-            outputs = ExtractModelResponse(self.inputs).run()
-            self.inputs.update(outputs)
-            outputs = ModifyCode(self.inputs).run()
-            self.inputs.update(outputs)
-
-            if i == self.n - 1:
-                break
-
-            # validation
-            self.inputs.pop("sarif_file_path", None)
-            outputs = ScanSemgrep(self.inputs).run()
-            self.inputs.update(outputs)
-            outputs = ExtractCode(self.inputs).run()
-            self.inputs.update(outputs)
-            if self.inputs.get("prompt_value_file") is not None:
-                with open(self.inputs["prompt_value_file"], "r") as fp:
-                    vulns = json.load(fp)
-                if len(vulns) < 1:
-                    break
-
+        number = len(self.inputs["modified_code_files"])
+        self.inputs["pr_header"] = f"This pull request from patchwork adds {number} READMEs."
         outputs = CommitChanges(self.inputs).run()
         self.inputs.update(outputs)
         outputs = PreparePR(self.inputs).run()
         self.inputs.update(outputs)
         outputs = CreatePR(self.inputs).run()
         self.inputs.update(outputs)
```

### Comparing `patchwork_cli-0.0.5/patchwork/patchflows/AutoFix/README.md` & `patchwork_cli-0.0.6/patchwork/patchflows/AutoFix/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/patchflows/AutoFix/default_prompt.json` & `patchwork_cli-0.0.6/patchwork/patchflows/AutoFix/default_prompt.json`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/patchflows/AutoFix/defaults.yml` & `patchwork_cli-0.0.6/patchwork/patchflows/DependencyUpgrade/defaults.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,24 @@
-# ExtractCode Inputs
-vulnerability_limit: 10
-context_size: 1000
-# sari_file_path should point to the generated SARIF file relative to the working directory
-# sarif_file_path: /mnt/data/sarif.json
-
 # PreparePrompt Inputs
 # prompt_template_file: your-prompt-template-here
 
 # CallOpenAI Inputs
 # openai_api_key: required
 model: gpt-3.5-turbo
 client_base_url: https://api.openai.com/v1
 # Example HF model
 # client_base_url: https://api-inference.huggingface.co/models/codellama/CodeLlama-70b-Instruct-hf/v1
 # model: codellama/CodeLlama-70b-Instruct-hf
 # model_temperature: 0.2
 # model_top_p: 0.95
 # model_max_tokens: 2000
 
+# Do impact analysis after dependency upgrades to modify source code
+analyze_impact: false
+
 # CommitChanges Inputs
 disable_branch: false
 
 # CreatePR Inputs
 disable_pr: false
 force_pr_creation: false
 # github_api_key: required-for-github-scm
```

### Comparing `patchwork_cli-0.0.5/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py` & `patchwork_cli-0.0.6/patchwork/patchflows/DependencyUpgrade/DependencyUpgrade.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/patchflows/DependencyUpgrade/README.md` & `patchwork_cli-0.0.6/patchwork/patchflows/DependencyUpgrade/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/patchflows/DependencyUpgrade/defaults.yml` & `patchwork_cli-0.0.6/patchwork/patchflows/GenerateREADME/defaults.yml`

 * *Files 27% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 # Example HF model
 # client_base_url: https://api-inference.huggingface.co/models/codellama/CodeLlama-70b-Instruct-hf/v1
 # model: codellama/CodeLlama-70b-Instruct-hf
 # model_temperature: 0.2
 # model_top_p: 0.95
 # model_max_tokens: 2000
 
-# Do impact analysis after dependency upgrades to modify source code
-analyze_impact: false
-
 # CommitChanges Inputs
 disable_branch: false
 
 # CreatePR Inputs
 disable_pr: false
 force_pr_creation: false
 # github_api_key: required-for-github-scm
```

### Comparing `patchwork_cli-0.0.5/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json` & `patchwork_cli-0.0.6/patchwork/patchflows/DependencyUpgrade/dependency_upgrade_prompt.json`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/patchflows/GenerateREADME/README.md` & `patchwork_cli-0.0.6/patchwork/patchflows/GenerateREADME/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 model_max_tokens: 1000
 ```
 and use the local model for inference.
 
 ### Filter
 You can restrict the kind of files to use for generating the documentation using the `filter` option.
 ```yaml
-filter: *.py
+filter: '*.py'
 ```
 
 ### Suppress comments
 If you do not want the comments in the file to be included set the `suppress_comments` option.
 ```yaml
 suppress_comments: false
 ```
```

### Comparing `patchwork_cli-0.0.5/patchwork/patchflows/GenerateREADME/defaults.yml` & `patchwork_cli-0.0.6/patchwork/patchflows/AutoFix/defaults.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+# AutoFix Inputs
+compatibility: unknown
+
+# ExtractCode Inputs
+vulnerability_limit: 10
+context_size: 1000
+severity: unknown
+# sarif_file_path should point to the generated SARIF file relative to the working directory
+# sarif_file_path: /mnt/data/sarif.json
+
 # PreparePrompt Inputs
 # prompt_template_file: your-prompt-template-here
 
 # CallOpenAI Inputs
 # openai_api_key: required
 model: gpt-3.5-turbo
 client_base_url: https://api.openai.com/v1
```

### Comparing `patchwork_cli-0.0.5/patchwork/patchflows/PRReview/PRReview.py` & `patchwork_cli-0.0.6/patchwork/patchflows/PRReview/PRReview.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/patchflows/PRReview/README.md` & `patchwork_cli-0.0.6/patchwork/patchflows/PRReview/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/patchflows/PRReview/defaults.yml` & `patchwork_cli-0.0.6/patchwork/patchflows/PRReview/defaults.yml`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/patchflows/PRReview/pr_review_prompt.json` & `patchwork_cli-0.0.6/patchwork/patchflows/PRReview/pr_review_prompt.json`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/patchflows/README.md` & `patchwork_cli-0.0.6/patchwork/patchflows/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py` & `patchwork_cli-0.0.6/patchwork/steps/AnalyzeImpact/AnalyzeImpact.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/AnalyzeImpact/README.md` & `patchwork_cli-0.0.6/patchwork/steps/AnalyzeImpact/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py` & `patchwork_cli-0.0.6/patchwork/steps/CallCode2Prompt/CallCode2Prompt.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/CallCode2Prompt/README.md` & `patchwork_cli-0.0.6/patchwork/steps/CallCode2Prompt/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py` & `patchwork_cli-0.0.6/patchwork/steps/CallCode2Prompt/TestCallCode2Prompt.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/CallOpenAI/CallOpenAI.py` & `patchwork_cli-0.0.6/patchwork/steps/CallOpenAI/CallOpenAI.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         # Set 'openai_key' from inputs or environment if not already set
         inputs.setdefault("openai_api_key", os.environ.get("OPENAI_API_KEY"))
 
         if not all(key in inputs.keys() for key in self.required_keys):
             raise ValueError(f'Missing required data: "{self.required_keys}"')
 
         self.model = inputs["model"]
+        self.allow_trunctated = inputs.get("allow_truncated", False)
         self.model_args = {key[len("model_") :]: value for key, value in inputs.items() if key.startswith("model_")}
         self.client_args = {key[len("client_") :]: value for key, value in inputs.items() if key.startswith("client_")}
 
         openai_key = inputs.get("openai_api_key") or os.environ.get("OPENAI_API_KEY")
         if openai_key is not None:
             self.openai_api_key = openai_key
 
@@ -77,16 +78,19 @@
             logger.debug(f"Message sent: \n{indent(pformat(prompt), '  ')}")
             completion = client.chat.completions.create(model=self.model, **kwargs)
 
             if len(completion.choices) < 1:
                 logger.error(f"No response choice given")
                 contents.append("")
             elif completion.choices[0].finish_reason == "length":
-                logger.error(f"Response truncated because of finish reason = length")
-                contents.append("")
+                if self.allow_trunctated:
+                    contents.append(completion.choices[0].message.content)
+                else:
+                    logger.error(f"Response truncated because of finish reason = length. Use --allow_truncated option to process truncated responses.")
+                    contents.append("")
             else:
                 logger.debug(f"Response received: \n{indent(completion.choices[0].message.content, '  ')}")
                 contents.append(completion.choices[0].message.content)
 
         response_file = Path(tempfile.mktemp(".json"))
         with open(response_file, "w") as outfile:
             json.dump(contents, outfile, indent=2)
```

### Comparing `patchwork_cli-0.0.5/patchwork/steps/CommitChanges/CommitChanges.py` & `patchwork_cli-0.0.6/patchwork/steps/CommitChanges/CommitChanges.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/CommitChanges/README.md` & `patchwork_cli-0.0.6/patchwork/steps/CommitChanges/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/CreatePR/CreatePR.py` & `patchwork_cli-0.0.6/patchwork/steps/CreatePR/CreatePR.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/CreatePR/README.md` & `patchwork_cli-0.0.6/patchwork/steps/CreatePR/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/CreatePRComment/CreatePRComment.py` & `patchwork_cli-0.0.6/patchwork/steps/CreatePRComment/CreatePRComment.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/CreatePRComment/README.md` & `patchwork_cli-0.0.6/patchwork/steps/CreatePRComment/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/ExtractCode/ExtractCode.py` & `patchwork_cli-0.0.6/patchwork/steps/ExtractCode/ExtractCode.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
 import os
 import sys
 import tempfile
 from collections import defaultdict
+from enum import IntEnum
 from pathlib import Path
+from typing import Any
 from urllib.parse import urlparse
 
 import tiktoken
 
 from patchwork.logger import logger
 from patchwork.step import Step
 
@@ -89,26 +91,118 @@
     uri = artifact_location.get("uri")
     if uri is not None:
         return parse_sarif_location(base_path, uri)
 
     return None
 
 
+class Severity(IntEnum):
+    CRITICAL = 5
+    HIGH = 4
+    ERROR = 4
+    MEDIUM = 3
+    LOW = 2
+    WARNING = 2
+    INFO = 1
+    NOTE = 1
+    UNKNOWN = 0
+
+    @staticmethod
+    def from_str(severity: str) -> "Severity":
+        try:
+            return Severity[severity.upper()]
+        except KeyError:
+            logger.error(f'Unknown severity: "{severity}"')
+            return Severity.UNKNOWN
+
+
+def get_rule_severity(rule: dict[str:Any]) -> Severity:
+    properties = rule.get("properties", {})
+
+    try:
+        security_severity = float(properties.get("security-severity"))
+    except (ValueError, TypeError):
+        security_severity = None
+
+    if security_severity is not None:
+        if security_severity >= 9.0:
+            return Severity.CRITICAL
+        elif security_severity >= 7.0:
+            return Severity.HIGH
+        elif security_severity >= 4.0:
+            return Severity.MEDIUM
+        else:
+            return Severity.LOW
+
+    properties_severity = properties.get("severity") or properties.get("Severity")
+    if properties_severity is not None:
+        return Severity.from_str(properties_severity)
+
+    return Severity.UNKNOWN
+
+
+def get_severity(result, reporting_descriptors):
+    properties = result.get("properties", {})
+    properties_severity = properties.get("severity") or properties.get("Severity")
+    if properties_severity is not None:
+        return Severity.from_str(properties_severity)
+
+    result_rule = result.get("rule", {})
+    result_rule_idx = result.get("ruleIndex") or result_rule.get("index")
+    result_rule_id = result.get("ruleId") or result_rule.get("id")
+    rule = None
+    if result_rule_idx is not None:
+        rule = reporting_descriptors[result_rule_idx]
+    elif result_rule_id is not None:
+        for reporting_descriptor in reporting_descriptors:
+            if reporting_descriptor.get("id") == result_rule_id:
+                rule = reporting_descriptor
+                break
+    elif len(result_rule) > 0:
+        rule = result_rule
+
+    rule_severity = Severity.UNKNOWN
+    if rule is not None:
+        rule_severity = get_rule_severity(rule)
+
+    if rule_severity != Severity.UNKNOWN:
+        return rule_severity
+
+    result_level = result.get("level")
+    if result_level is not None:
+        return Severity.from_str(result_level)
+
+    default_level = rule.get("defaultConfiguration", {}).get("level")
+    if default_level is not None:
+        return Severity.from_str(default_level)
+
+    return Severity.UNKNOWN
+
+
 def transform_sarif_results(
-    sarif_data: dict, base_path: Path, context_length: int, vulnerability_limit: int
+    sarif_data: dict, base_path: Path, context_length: int, vulnerability_limit: int, severity_threshold: Severity
 ) -> dict[tuple[str, int, int, int], list[str]]:
     # Process each result in SARIF data
     grouped_messages = defaultdict(list)
     vulnerability_count = 0
     for run_idx, run in enumerate(sarif_data.get("runs", [])):
         artifact_locations = [
             parse_sarif_location(base_path, artifact["location"]["uri"]) for artifact in run.get("artifacts", [])
         ]
 
+        tool = run.get("tool", {})
+        reporting_descriptors = tool.get("driver", {}).get("rules", [])
+        for tool_obj in tool.get("extensions", []):
+            reporting_descriptors.extend(tool_obj.get("rules", []))
+
         for result_idx, result in enumerate(run.get("results", [])):
+            severity = get_severity(result, reporting_descriptors)
+            if severity < severity_threshold:
+                continue
+
             for location_idx, location in enumerate(result.get("locations", [])):
                 physical_location = location.get("physicalLocation", {})
 
                 artifact_location = physical_location.get("artifactLocation", {})
                 uri = resolve_artifact_location(base_path, artifact_location, artifact_locations)
                 if uri is None:
                     logger.warn(
@@ -176,27 +270,29 @@
         self.sarif_file_path = Path(inputs["sarif_file_path"])
         if not self.sarif_file_path.exists() or not self.sarif_file_path.is_file():
             raise ValueError(f'SARIF file path does not exist or is not a file: "{self.sarif_file_path}"')
 
         # Check and set number of lines to extract
         self.context_length = inputs.get("context_size", 1000)
         self.vulnerability_limit = inputs.get("vulnerability_limit", 10)
+        self.severity_threshold = Severity.from_str(inputs.get("severity", "UNKNOWN"))
 
         # Prepare for data extraction
         self.extracted_code_contexts = []
 
     def run(self) -> dict:
         # Load SARIF data
         with open_with_chardet(self.sarif_file_path, "r") as file:
             sarif_data = json.load(file)
 
-        vulnerability_count = 0
         base_path = Path.cwd()
 
-        grouped_messages = transform_sarif_results(sarif_data, base_path, self.context_length, self.vulnerability_limit)
+        grouped_messages = transform_sarif_results(
+            sarif_data, base_path, self.context_length, self.vulnerability_limit, self.severity_threshold
+        )
 
         self.extracted_code_contexts = [
             {
                 "uri": str(file_path),
                 "startLine": start,
                 "endLine": end,
                 "affectedCode": context,
```

### Comparing `patchwork_cli-0.0.5/patchwork/steps/ExtractCode/README.md` & `patchwork_cli-0.0.6/patchwork/steps/ExtractCode/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/ExtractCode/context_strategy/context_strategies.py` & `patchwork_cli-0.0.6/patchwork/steps/ExtractCode/context_strategy/context_strategies.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/ExtractCode/context_strategy/generic.py` & `patchwork_cli-0.0.6/patchwork/steps/ExtractCode/context_strategy/generic.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/ExtractCode/context_strategy/java.py` & `patchwork_cli-0.0.6/patchwork/steps/ExtractCode/context_strategy/java.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/ExtractCode/context_strategy/javascript.py` & `patchwork_cli-0.0.6/patchwork/steps/ExtractCode/context_strategy/javascript.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/ExtractCode/context_strategy/python.py` & `patchwork_cli-0.0.6/patchwork/steps/ExtractCode/context_strategy/python.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/ExtractDiff/ExtractDiff.py` & `patchwork_cli-0.0.6/patchwork/steps/ExtractDiff/ExtractDiff.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/ExtractDiff/README.md` & `patchwork_cli-0.0.6/patchwork/steps/ExtractDiff/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py` & `patchwork_cli-0.0.6/patchwork/steps/ExtractModelResponse/ExtractModelResponse.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/ExtractModelResponse/README.md` & `patchwork_cli-0.0.6/patchwork/steps/ExtractModelResponse/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py` & `patchwork_cli-0.0.6/patchwork/steps/ExtractPackageManagerFile/ExtractPackageManagerFile.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/ExtractPackageManagerFile/README.md` & `patchwork_cli-0.0.6/patchwork/steps/ExtractPackageManagerFile/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py` & `patchwork_cli-0.0.6/patchwork/steps/ExtractPackageManagerFile/TestExtractPackageManagerFile.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/ModifyCode/ModifyCode.py` & `patchwork_cli-0.0.6/patchwork/steps/ModifyCode/ModifyCode.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/ModifyCode/README.md` & `patchwork_cli-0.0.6/patchwork/steps/ModifyCode/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/PreparePR/PreparePR.py` & `patchwork_cli-0.0.6/patchwork/steps/PreparePR/PreparePR.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/PreparePR/README.md` & `patchwork_cli-0.0.6/patchwork/steps/PreparePR/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/PreparePrompt/PreparePrompt.py` & `patchwork_cli-0.0.6/patchwork/steps/PreparePrompt/PreparePrompt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 import json
 import tempfile
 from pathlib import Path
 
 from patchwork.logger import logger
 from patchwork.step import Step
 
+PROMPT_TEMPLATE_FILE_KEY = "prompt_template_file"
+
 
 class PreparePrompt(Step):
-    required_keys = {"prompt_template_file", "prompt_id"}
+    required_keys = {("%s" % PROMPT_TEMPLATE_FILE_KEY), "prompt_id"}
 
     def __init__(self, inputs: dict):
         logger.info(f"Run started {self.__class__.__name__}")
 
         if not all(key in inputs.keys() for key in self.required_keys):
             raise ValueError(f'Missing required data: "{self.required_keys}"')
 
-        prompt_template_file = Path(inputs["prompt_template_file"])
+        prompt_template_file = Path(inputs[PROMPT_TEMPLATE_FILE_KEY])
         if not prompt_template_file.is_file():
-            raise ValueError(f"Prompt Template File {prompt_template_file} does not exist")
+            raise ValueError(f"Prompt Template File {PROMPT_TEMPLATE_FILE_KEY} does not exist")
         try:
             with open(prompt_template_file, "r") as fp:
                 prompt_templates = json.load(fp)
         except json.JSONDecodeError as e:
-            raise ValueError(f'Invalid Json Prompt Template file "{prompt_template_file}": {e}')
+            raise ValueError(f'Invalid Json Prompt Template file "{PROMPT_TEMPLATE_FILE_KEY}": {e}')
 
         prompt_template = next((prompt for prompt in prompt_templates if prompt["id"] == inputs["prompt_id"]), None)
         if prompt_template is None:
             raise ValueError(
-                f'Prompt ID "{inputs["prompt_id"]}" not found in Prompt Template file "{prompt_template_file}"'
+                f'Prompt ID "{inputs["prompt_id"]}" not found in Prompt Template file "{PROMPT_TEMPLATE_FILE_KEY}"'
             )
         self.prompt_template = prompt_template.get("prompts")
         if self.prompt_template is None:
             raise ValueError(
-                f'Prompt ID "{inputs["prompt_id"]}" does not have any prompts in Prompt Template file "{prompt_template_file}"'
+                f'Prompt ID "{inputs["prompt_id"]}" does not have any prompts in Prompt Template file "{PROMPT_TEMPLATE_FILE_KEY}"'
             )
 
         prompt_value_file = inputs.get("prompt_value_file")
         prompt_values = inputs.get("prompt_values")
         if prompt_value_file is None and prompt_values is None:
             raise ValueError('Missing required data: "prompt_value_file" or "prompt_values"')
         if prompt_values is None and not Path(prompt_value_file).is_file():
```

### Comparing `patchwork_cli-0.0.5/patchwork/steps/PreparePrompt/README.md` & `patchwork_cli-0.0.6/patchwork/steps/PreparePrompt/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/README.md` & `patchwork_cli-0.0.6/patchwork/steps/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/ReadPRDiffs/README.md` & `patchwork_cli-0.0.6/patchwork/steps/ReadPRDiffs/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/ReadPRDiffs/ReadPRDiffs.py` & `patchwork_cli-0.0.6/patchwork/steps/ReadPRDiffs/ReadPRDiffs.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/ScanDepscan/README.md` & `patchwork_cli-0.0.6/patchwork/steps/ScanDepscan/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/ScanDepscan/ScanDepscan.py` & `patchwork_cli-0.0.6/patchwork/steps/ScanDepscan/ScanDepscan.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/ScanDepscan/TestScanDepscan.py` & `patchwork_cli-0.0.6/patchwork/steps/ScanDepscan/TestScanDepscan.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/ScanSemgrep/README.md` & `patchwork_cli-0.0.6/patchwork/steps/ScanSemgrep/README.md`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/ScanSemgrep/ScanSemgrep.py` & `patchwork_cli-0.0.6/patchwork/steps/ScanSemgrep/ScanSemgrep.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/patchwork/steps/__init__.py` & `patchwork_cli-0.0.6/patchwork/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `patchwork_cli-0.0.5/pyproject.toml` & `patchwork_cli-0.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "patchwork-cli"
-version = "0.0.5"
+version = "0.0.6"
 description = ""
-authors = ["patched.code"]
+authors = ["patched.codes"]
 license = "AGPL"
 readme = "README.md"
 packages = [
     { include = "patchwork", from = "." }
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -19,32 +19,34 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Quality Assurance",
     "Topic :: Software Development :: Testing",
     "Topic :: Utilities"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.10, <3.12"
 click = "~8.1.0"
 pygithub = "~2.1.1"
 gitpython = "~3.1.40"
 semgrep = "^1.51.0"
 pydantic = "^2.6.4"
 openai = "^1.13.3"
 tree-sitter-languages = "^1.10.2"
-tiktoken = "^0.6.0"
+tiktoken = "~0.5.2"
 libcst = "~1.2.0"
 python-gitlab = "^4.4.0"
 owasp-depscan = "^5.2.12"
 patched-code2prompt = "0.2.0"
 pyyaml = "^6.0.1"
 packageurl-python = "~0.15.0"
 semver = "~3.0.2"
 requests = "~2.31.0"
 chardet = "^5.2.0"
+# TODO: bump this to at least 0.2.5 when it's released to fix python version dependency resolution issues
+open-interpreter = "~0.2.4"
 # pinning transitive dependencies
 orjson = "~3.9.15"
 
 [tool.poetry.group.dev.dependencies]
 setuptools = "*"
 poethepoet = { version = "^0.24.2", extras = ["poetry-plugin"] }
 mypy = "^1.7.1"
```

### Comparing `patchwork_cli-0.0.5/PKG-INFO` & `patchwork_cli-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 Metadata-Version: 2.1
 Name: patchwork-cli
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 License: AGPL
-Author: patched.code
-Requires-Python: >=3.10,<4.0
+Author: patched.codes
+Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Dist: chardet (>=5.2.0,<6.0.0)
 Requires-Dist: click (>=8.1.0,<8.2.0)
 Requires-Dist: gitpython (>=3.1.40,<3.2.0)
 Requires-Dist: libcst (>=1.2.0,<1.3.0)
+Requires-Dist: open-interpreter (>=0.2.4,<0.3.0)
 Requires-Dist: openai (>=1.13.3,<2.0.0)
 Requires-Dist: orjson (>=3.9.15,<3.10.0)
 Requires-Dist: owasp-depscan (>=5.2.12,<6.0.0)
 Requires-Dist: packageurl-python (>=0.15.0,<0.16.0)
 Requires-Dist: patched-code2prompt (==0.2.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: pygithub (>=2.1.1,<2.2.0)
 Requires-Dist: python-gitlab (>=4.4.0,<5.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<2.32.0)
 Requires-Dist: semgrep (>=1.51.0,<2.0.0)
 Requires-Dist: semver (>=3.0.2,<3.1.0)
-Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
+Requires-Dist: tiktoken (>=0.5.2,<0.6.0)
 Requires-Dist: tree-sitter-languages (>=1.10.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://github.com/patched-codes/patchwork/assets/126385808/a7adcf24-b615-43a0-a244-45789d184f0a" width="160" alt="PatchWork Logo">
 </p>
```

