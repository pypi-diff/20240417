# Comparing `tmp/pyquiet-0.0.2.tar.gz` & `tmp/pyquiet-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquiet-0.0.2.tar", last modified: Tue Jan  2 00:56:30 2024, max compression
+gzip compressed data, was "pyquiet-0.0.3.tar", last modified: Wed Apr 17 07:43:08 2024, max compression
```

## Comparing `pyquiet-0.0.2.tar` & `pyquiet-0.0.3.tar`

### file list

```diff
@@ -1,54 +1,57 @@
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-01-02 00:56:30.976461 pyquiet-0.0.2/
--rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)     1435 2024-01-02 00:56:30.976461 pyquiet-0.0.2/PKG-INFO
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      811 2024-01-02 00:46:23.000000 pyquiet-0.0.2/README.md
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      103 2023-09-28 06:54:51.000000 pyquiet-0.0.2/pyproject.toml
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      803 2024-01-02 00:56:30.976461 pyquiet-0.0.2/setup.cfg
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       38 2023-09-28 06:54:51.000000 pyquiet-0.0.2/setup.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-01-02 00:56:30.968461 pyquiet-0.0.2/src/
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-01-02 00:56:30.972461 pyquiet-0.0.2/src/QiParser/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     2533 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/QiParser/QiParser.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/QiParser/__init__.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-01-02 00:56:30.972461 pyquiet-0.0.2/src/QiVisitor/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    38428 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/QiVisitor/QuietVisitor.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/QiVisitor/__init__.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-01-02 00:56:30.972461 pyquiet-0.0.2/src/antlr/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    19878 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/antlr/QuietLexer.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)   171109 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/antlr/QuietParser.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    19158 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/antlr/QuietParserListener.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    11534 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/antlr/QuietParserVisitor.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/antlr/__init__.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-01-02 00:56:30.976461 pyquiet-0.0.2/src/pyquiet.egg-info/
--rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)     1435 2024-01-02 00:56:30.000000 pyquiet-0.0.2/src/pyquiet.egg-info/PKG-INFO
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1116 2024-01-02 00:56:30.000000 pyquiet-0.0.2/src/pyquiet.egg-info/SOURCES.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        1 2024-01-02 00:56:30.000000 pyquiet-0.0.2/src/pyquiet.egg-info/dependency_links.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       37 2024-01-02 00:56:30.000000 pyquiet-0.0.2/src/pyquiet.egg-info/requires.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       29 2024-01-02 00:56:30.000000 pyquiet-0.0.2/src/pyquiet.egg-info/top_level.txt
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-01-02 00:56:30.972461 pyquiet-0.0.2/src/qir/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     2931 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/qir/QiProg.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1007 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/qir/Type.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1912 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/qir/Variable.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/qir/__init__.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-01-02 00:56:30.972461 pyquiet-0.0.2/src/qir/qModule/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1566 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/qir/qModule/ClassicalInsnBase.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      693 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/qir/qModule/ControlWords.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     3797 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/qir/qModule/FloatInstructions.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      243 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/qir/qModule/InstructionBase.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     9654 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/qir/qModule/IntInstruction.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1476 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/qir/qModule/QuietModules.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    13232 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/qir/qModule/StdInstructions.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/qir/qModule/__init__.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-01-02 00:56:30.972461 pyquiet-0.0.2/src/qir/qbody/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1134 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/qir/qbody/BodySection.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     4061 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/qir/qbody/Function.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1220 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/qir/qbody/FunctionCall.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      530 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/qir/qbody/VariableDecl.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/qir/qbody/__init__.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-01-02 00:56:30.976461 pyquiet-0.0.2/src/qir/qfile/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1116 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/qir/qfile/FileSection.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/qir/qfile/__init__.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      547 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/qir/qfile/file.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-01-02 00:56:30.976461 pyquiet-0.0.2/src/qir/qgate/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      960 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/qir/qgate/GateSection.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/qir/qgate/__init__.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     2065 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/qir/qgate/gate.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      328 2023-09-28 06:54:51.000000 pyquiet-0.0.2/src/qir/qutils.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 07:43:08.000620 pyquiet-0.0.3/
+-rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)     1435 2024-04-17 07:43:08.000620 pyquiet-0.0.3/PKG-INFO
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      811 2024-01-02 00:46:23.000000 pyquiet-0.0.3/README.md
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      103 2023-09-28 06:54:51.000000 pyquiet-0.0.3/pyproject.toml
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      803 2024-04-17 07:43:08.000620 pyquiet-0.0.3/setup.cfg
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       38 2023-09-28 06:54:51.000000 pyquiet-0.0.3/setup.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 07:43:07.988619 pyquiet-0.0.3/src/
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 07:43:07.992620 pyquiet-0.0.3/src/pyquiet/
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 07:43:07.992620 pyquiet-0.0.3/src/pyquiet/QiParser/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     2613 2024-04-03 08:04:48.000000 pyquiet-0.0.3/src/pyquiet/QiParser/QiParser.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 03:20:08.000000 pyquiet-0.0.3/src/pyquiet/QiParser/__init__.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    16715 2024-04-07 03:16:18.000000 pyquiet-0.0.3/src/pyquiet/QiSemanticChecker.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 07:43:07.992620 pyquiet-0.0.3/src/pyquiet/QiVisitor/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    41584 2024-04-07 01:21:44.000000 pyquiet-0.0.3/src/pyquiet/QiVisitor/QuietVisitor.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/QiVisitor/__init__.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/__init__.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 07:43:07.996620 pyquiet-0.0.3/src/pyquiet/antlr/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    19878 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/antlr/QuietLexer.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)   171109 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/antlr/QuietParser.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    19158 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/antlr/QuietParserListener.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    11534 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/antlr/QuietParserVisitor.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       98 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/antlr/__init__.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 07:43:07.996620 pyquiet-0.0.3/src/pyquiet/qir/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     3036 2024-04-03 07:01:28.000000 pyquiet-0.0.3/src/pyquiet/qir/QiProg.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1007 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/qir/Type.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1953 2024-04-03 02:45:10.000000 pyquiet-0.0.3/src/pyquiet/qir/Variable.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      308 2024-04-03 07:09:17.000000 pyquiet-0.0.3/src/pyquiet/qir/__init__.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 07:43:07.996620 pyquiet-0.0.3/src/pyquiet/qir/qModule/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1710 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/qir/qModule/ClassicalInsnBase.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      690 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/qir/qModule/ControlWords.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     4238 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/qir/qModule/FloatInstructions.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      243 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/qir/qModule/InstructionBase.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     9792 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/qir/qModule/IntInstruction.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     2070 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/qir/qModule/QuietModules.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    13280 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/qir/qModule/StdInstructions.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/qir/qModule/__init__.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 07:43:07.996620 pyquiet-0.0.3/src/pyquiet/qir/qbody/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1115 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/qir/qbody/BodySection.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     3977 2024-04-03 03:13:16.000000 pyquiet-0.0.3/src/pyquiet/qir/qbody/Function.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1236 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/qir/qbody/FunctionCall.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      597 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/qir/qbody/VariableDecl.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      218 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/qir/qbody/__init__.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 07:43:07.996620 pyquiet-0.0.3/src/pyquiet/qir/qfile/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1106 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/qir/qfile/FileSection.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       98 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/qir/qfile/__init__.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      547 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/qir/qfile/file.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 07:43:07.996620 pyquiet-0.0.3/src/pyquiet/qir/qgate/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      941 2024-04-03 08:07:37.000000 pyquiet-0.0.3/src/pyquiet/qir/qgate/GateSection.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      118 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/qir/qgate/__init__.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     2050 2024-04-03 08:07:23.000000 pyquiet-0.0.3/src/pyquiet/qir/qgate/gate.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      328 2024-04-03 01:43:37.000000 pyquiet-0.0.3/src/pyquiet/qir/qutils.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 07:43:07.992620 pyquiet-0.0.3/src/pyquiet.egg-info/
+-rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)     1435 2024-04-17 07:43:07.000000 pyquiet-0.0.3/src/pyquiet.egg-info/PKG-INFO
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1437 2024-04-17 07:43:07.000000 pyquiet-0.0.3/src/pyquiet.egg-info/SOURCES.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        1 2024-04-17 07:43:07.000000 pyquiet-0.0.3/src/pyquiet.egg-info/dependency_links.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       37 2024-04-17 07:43:07.000000 pyquiet-0.0.3/src/pyquiet.egg-info/requires.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        8 2024-04-17 07:43:07.000000 pyquiet-0.0.3/src/pyquiet.egg-info/top_level.txt
```

### Comparing `pyquiet-0.0.2/PKG-INFO` & `pyquiet-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquiet
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python Parser for the Quiet Quantum Instruction Set
 Home-page: https://gitee.com/hpcl_quanta/quiet-parser.git
 Author: Yuzhen Zheng, Zhengdong Tang, Xiang Fu
 Author-email: gtaifu@gmail.com
 Project-URL: Bug Tracker, https://gitee.com/hpcl_quanta/quiet-parser/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyquiet-0.0.2/README.md` & `pyquiet-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyquiet-0.0.2/setup.cfg` & `pyquiet-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyquiet
-version = 0.0.2
+version = 0.0.3
 py_modules = ['pyquiet']
 author = Yuzhen Zheng, Zhengdong Tang, Xiang Fu
 author_email = gtaifu@gmail.com
 use_2to3 = False
 description = A Python Parser for the Quiet Quantum Instruction Set
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `pyquiet-0.0.2/src/QiParser/QiParser.py` & `pyquiet-0.0.3/src/pyquiet/QiParser/QiParser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List
-from antlr4 import *
 from pathlib import Path
-from antlr.QuietLexer import QuietLexer
-from antlr.QuietParser import QuietParser
-from QiVisitor.QuietVisitor import QuietVisitor
-from qir.QiProg import *
+from antlr4 import InputStream, CommonTokenStream
+from pyquiet.antlr import QuietLexer, QuietParser
+from pyquiet.QiVisitor.QuietVisitor import QuietVisitor
+from pyquiet.qir import QiProgram, FunctionCall
+from pyquiet.qir.qfile import QiFile, QiFileSection
 
 
 def ensure_path(fn) -> Path:
     assert isinstance(fn, (str, Path))
     if isinstance(fn, str):
         fn = Path(fn).resolve()
     return fn
```

### Comparing `pyquiet-0.0.2/src/QiVisitor/QuietVisitor.py` & `pyquiet-0.0.3/src/pyquiet/QiVisitor/QuietVisitor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,76 @@
-from antlr4 import *
-from antlr.QuietLexer import QuietLexer
-from antlr.QuietParserVisitor import *
-from antlr.QuietParser import QuietParser
+import numpy
 from pathlib import Path
-from qir.QiProg import *
+
+from pyquiet.antlr.QuietParserVisitor import QuietParserVisitor
+from pyquiet.antlr.QuietParser import QuietParser
+from pyquiet.qir.Type import QubitType, IntType, DoubleType
+from pyquiet.qir.Variable import QiList, QiVariable
+from pyquiet.qir.qModule.ControlWords import ControlWords
+from pyquiet.qir.qModule.QuietModules import FloatModule, IntModule
+from pyquiet.qir.qModule.FloatInstructions import (
+    Adddi,
+    Divdi,
+    Ldd,
+    Movd,
+    Addd,
+    Muldi,
+    Subd,
+    Muld,
+    Divd,
+    Subdi,
+)
+from pyquiet.qir.qModule.IntInstruction import (
+    Mov,
+    Ld,
+    Lnot,
+    Land,
+    Lor,
+    Lxor,
+    Add,
+    Sub,
+    Mul,
+    Div,
+    Addi,
+    Subi,
+    Muli,
+    Divi,
+    Bne,
+    Beq,
+    Blt,
+    Ble,
+    Bgt,
+    Bge,
+    Jump,
+)
+from pyquiet.qir.qModule.StdInstructions import (
+    Sdag,
+    T,
+    Tdag,
+    S,
+    X,
+    Y,
+    Z,
+    H,
+    CNOT,
+    CZ,
+    SWAP,
+    U4,
+    Rx,
+    Ry,
+    Rz,
+    Rxy,
+    CP,
+    CRz,
+)
+from pyquiet.qir.qbody import QiFunction, VariableDecl, FunctionCall
+from pyquiet.qir.QiProg import QiProgram
+
+from pyquiet.qir.qfile.file import QiFile
+from pyquiet.qir.qgate.gate import QiDefineGate, QiDefineInfo
 
 
 class QuietVisitor(QuietParserVisitor):
     def __init__(self, file_name: str = "default", qi_path: Path = Path().cwd()):
         super().__init__()
         self.__prog = QiProgram(file_name)
         self.__qi_path = qi_path
@@ -199,15 +262,15 @@
         ins = self.visitInstruction(ctx.instruction())
         if isinstance(ins, list):
             # variable declaration
             # The label will point to the first instruction in the list.
             ins[0].label = label
             for insn in ins:
                 self.__current_function.push_instr(insn)
-        else:
+        elif ins is not None:
             ins.label = label
             self.__current_function.push_instr(ins)
 
     # Visit a parse tree produced by QuietParser#label.
     def visitLabel(self, ctx: QuietParser.LabelContext):
         if ctx is None:
             return None
@@ -225,14 +288,16 @@
             ins = self.visitFuncCall(ctx.funcCall())
         elif ctx.variableDecl() is not None:
             ins = self.visitVariableDecl(ctx.variableDecl())
         elif ctx.integerModuleInsn() is not None:
             ins = self.visitIntegerModuleInsn(ctx.integerModuleInsn())
         elif ctx.floatModuleInsn() is not None:
             ins = self.visitFloatModuleInsn(ctx.floatModuleInsn())
+        elif ctx.EOL() is not None:
+            return None
         else:
             raise ValueError("The instruction type is not supported yet.")
         return ins
 
     # Visit a parse tree produced by QuietParser#returnStmt.
     def visitReturnStmt(self, ctx: QuietParser.ReturnStmtContext):
         if ctx is None:
@@ -399,15 +464,18 @@
     # Visit a parse tree produced by QuietParser#number.
     def visitNumber(self, ctx: QuietParser.NumberContext):
         if ctx is None:
             raise ValueError("The number is None.")
         if ctx.IntLiteral() is not None:
             num = int(ctx.IntLiteral().getText())
         elif ctx.DoubleLiteral() is not None:
-            num = float(ctx.DoubleLiteral().getText())
+            if ctx.DoubleLiteral().getText() == "pi":
+                num = numpy.pi
+            else:
+                num = float(ctx.DoubleLiteral().getText())
         elif ctx.complexLiteral() is not None:
             num = self.visitComplexLiteral(ctx.complexLiteral())
         return num
 
     def visitComplexLiteral(self, ctx: QuietParser.ComplexLiteralContext):
         if ctx is None:
             raise ValueError("The complex literal is None.")
@@ -468,18 +536,24 @@
         num = 0
         return typeNoLen, num
 
     # Visit a parse tree produced by QuietParser#typeArrayWithLength.
     def visitTypeArrayWithLength(self, ctx: QuietParser.TypeArrayWithLengthContext):
         if ctx is None:
             raise ValueError("The type is None.")
-        if ctx.IntLiteral() is None:
-            num = str(ctx.Id().getText())
-        else:
+        if ctx.Id():
+            assert len(ctx.Id()) != 0
+            num = str(ctx.Id()[0].getText())
+        elif ctx.IntLiteral():
+            assert len(ctx.IntLiteral()) != 0
             num = int(ctx.IntLiteral()[0].getText())
+        else:
+            raise ValueError(
+                "The type with array length must have a number or variable."
+            )
         typeWithLen = self.visitTypeAtomic(ctx.typeAtomic())[0]
         return typeWithLen, num
 
     # Visit a parse tree produced by QuietParser#variableDecl.
     def visitVariableDecl(self, ctx: QuietParser.VariableDeclContext):
         if ctx is None:
             raise ValueError("The variable declaration is None.")
@@ -505,26 +579,62 @@
     # Visit a parse tree produced by QuietParser#variable.
     def visitVariable(self, ctx: QuietParser.VariableContext):
         if ctx is None:
             raise ValueError("The variable is None.")
         ids = ctx.Id()
         var_name = ids[0].getText()  # get the variable from the defined variables list.
         qi_var = self.__current_function.var_list().get_variable(str(var_name))
+
+        # we need a more detailed sematic check,
+        # the decalred variable and the used variable may be different.
         if isinstance(qi_var, QiList):
             if len(ids) == 2:
                 # it is a QiList Variable.
                 param = str(ids[1].getText())
-            else:
+            elif len(ids) == 1:
                 # If the IntLiteral is None, it indicates that the variable is a whole QiList.
+                # ? we should check the instr whether support vector operation or not.
                 param = None
-                if ctx.IntLiteral() is not None:
+                if ctx.IntLiteral():
                     param = int(ctx.IntLiteral().getText())
+            else:
+                # len(ids) == 0 case means it is not a variable. We don't need care about that.
+                raise ValueError(
+                    "We do not support the multi-index form of variable yet."
+                )
+
             # if the param is None, it indicates that the variable is a whole QiList.
             if param is not None:
                 qi_var = qi_var.var(param)
+        else:
+            if ctx.BracketLeft() and ctx.BracketRight():
+                qi_var = QiVariable(qi_var.type, qi_var.name)
+                if len(ids) == 2:
+                    # it is a QiList Variable.
+                    param = str(ids[1].getText())
+                elif len(ids) == 1:
+                    # If the IntLiteral is None, it indicates that the variable is a whole QiList.
+                    # ? we should check the instr whether support vector operation or not.
+                    param = None
+                    if ctx.IntLiteral():
+                        param = int(ctx.IntLiteral().getText())
+                else:
+                    # len(ids) == 0 case means it is not a variable. We don't need care about that.
+                    raise ValueError(
+                        "We do not support the multi-index form of variable yet."
+                    )
+
+                # if the param is None, it indicates that the variable is a whole QiList.
+                if param is not None:
+                    qi_var.set_index(param)
+                # raise SyntaxError(
+                #     "The variable {var} is not a QiList, but user add the idex.".format(
+                #         var=var_name
+                #     )
+                # )
         return qi_var
 
     # Visit a parse tree produced by QuietParser#funcCall.
     def visitFuncCall(self, ctx: QuietParser.FuncCallContext):
         if ctx is None:
             raise ValueError("The function call is described not correctly.")
         if ctx.controlModifier() is not None:
```

### Comparing `pyquiet-0.0.2/src/antlr/QuietLexer.py` & `pyquiet-0.0.3/src/pyquiet/antlr/QuietLexer.py`

 * *Files identical despite different names*

### Comparing `pyquiet-0.0.2/src/antlr/QuietParser.py` & `pyquiet-0.0.3/src/pyquiet/antlr/QuietParser.py`

 * *Files identical despite different names*

### Comparing `pyquiet-0.0.2/src/antlr/QuietParserListener.py` & `pyquiet-0.0.3/src/pyquiet/antlr/QuietParserListener.py`

 * *Files identical despite different names*

### Comparing `pyquiet-0.0.2/src/antlr/QuietParserVisitor.py` & `pyquiet-0.0.3/src/pyquiet/antlr/QuietParserVisitor.py`

 * *Files identical despite different names*

### Comparing `pyquiet-0.0.2/src/pyquiet.egg-info/PKG-INFO` & `pyquiet-0.0.3/src/pyquiet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquiet
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python Parser for the Quiet Quantum Instruction Set
 Home-page: https://gitee.com/hpcl_quanta/quiet-parser.git
 Author: Yuzhen Zheng, Zhengdong Tang, Xiang Fu
 Author-email: gtaifu@gmail.com
 Project-URL: Bug Tracker, https://gitee.com/hpcl_quanta/quiet-parser/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyquiet-0.0.2/src/pyquiet.egg-info/SOURCES.txt` & `pyquiet-0.0.3/src/pyquiet.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
-src/QiParser/QiParser.py
-src/QiParser/__init__.py
-src/QiVisitor/QuietVisitor.py
-src/QiVisitor/__init__.py
-src/antlr/QuietLexer.py
-src/antlr/QuietParser.py
-src/antlr/QuietParserListener.py
-src/antlr/QuietParserVisitor.py
-src/antlr/__init__.py
+src/pyquiet/QiSemanticChecker.py
+src/pyquiet/__init__.py
 src/pyquiet.egg-info/PKG-INFO
 src/pyquiet.egg-info/SOURCES.txt
 src/pyquiet.egg-info/dependency_links.txt
 src/pyquiet.egg-info/requires.txt
 src/pyquiet.egg-info/top_level.txt
-src/qir/QiProg.py
-src/qir/Type.py
-src/qir/Variable.py
-src/qir/__init__.py
-src/qir/qutils.py
-src/qir/qModule/ClassicalInsnBase.py
-src/qir/qModule/ControlWords.py
-src/qir/qModule/FloatInstructions.py
-src/qir/qModule/InstructionBase.py
-src/qir/qModule/IntInstruction.py
-src/qir/qModule/QuietModules.py
-src/qir/qModule/StdInstructions.py
-src/qir/qModule/__init__.py
-src/qir/qbody/BodySection.py
-src/qir/qbody/Function.py
-src/qir/qbody/FunctionCall.py
-src/qir/qbody/VariableDecl.py
-src/qir/qbody/__init__.py
-src/qir/qfile/FileSection.py
-src/qir/qfile/__init__.py
-src/qir/qfile/file.py
-src/qir/qgate/GateSection.py
-src/qir/qgate/__init__.py
-src/qir/qgate/gate.py
+src/pyquiet/QiParser/QiParser.py
+src/pyquiet/QiParser/__init__.py
+src/pyquiet/QiVisitor/QuietVisitor.py
+src/pyquiet/QiVisitor/__init__.py
+src/pyquiet/antlr/QuietLexer.py
+src/pyquiet/antlr/QuietParser.py
+src/pyquiet/antlr/QuietParserListener.py
+src/pyquiet/antlr/QuietParserVisitor.py
+src/pyquiet/antlr/__init__.py
+src/pyquiet/qir/QiProg.py
+src/pyquiet/qir/Type.py
+src/pyquiet/qir/Variable.py
+src/pyquiet/qir/__init__.py
+src/pyquiet/qir/qutils.py
+src/pyquiet/qir/qModule/ClassicalInsnBase.py
+src/pyquiet/qir/qModule/ControlWords.py
+src/pyquiet/qir/qModule/FloatInstructions.py
+src/pyquiet/qir/qModule/InstructionBase.py
+src/pyquiet/qir/qModule/IntInstruction.py
+src/pyquiet/qir/qModule/QuietModules.py
+src/pyquiet/qir/qModule/StdInstructions.py
+src/pyquiet/qir/qModule/__init__.py
+src/pyquiet/qir/qbody/BodySection.py
+src/pyquiet/qir/qbody/Function.py
+src/pyquiet/qir/qbody/FunctionCall.py
+src/pyquiet/qir/qbody/VariableDecl.py
+src/pyquiet/qir/qbody/__init__.py
+src/pyquiet/qir/qfile/FileSection.py
+src/pyquiet/qir/qfile/__init__.py
+src/pyquiet/qir/qfile/file.py
+src/pyquiet/qir/qgate/GateSection.py
+src/pyquiet/qir/qgate/__init__.py
+src/pyquiet/qir/qgate/gate.py
```

### Comparing `pyquiet-0.0.2/src/qir/QiProg.py` & `pyquiet-0.0.3/src/pyquiet/qir/QiProg.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from qir.qModule.QuietModules import *
-from qir.qfile.FileSection import *
-from qir.qgate.GateSection import *
-from qir.qbody.BodySection import *
+from typing import List
+from pyquiet.qir.qModule.QuietModules import QuietModule, std
+from pyquiet.qir.qbody import QiBodySection, QiFunction
+from pyquiet.qir.qfile import QiFileSection, QiFile
+from pyquiet.qir.qgate import QiGateSection, QiDefineInfo
 
 
 class QiProgram:
     """
        QiProgram is the intermediate representation of a `qi` file.
     It can be transformed from a quiet AST(CST), and extract the more essential information.
```

### Comparing `pyquiet-0.0.2/src/qir/Type.py` & `pyquiet-0.0.3/src/pyquiet/qir/Type.py`

 * *Files identical despite different names*

### Comparing `pyquiet-0.0.2/src/qir/Variable.py` & `pyquiet-0.0.3/src/pyquiet/qir/Variable.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from qir.Type import *
+from typing import Union
+from pyquiet.qir.Type import QuietType
 
 
 class QiVariable:
     def __init__(self, type: QuietType, var_name: str) -> None:
         self.__var_type = type
         self.__var_name = var_name
         # The variable in QiList is also a QiVariable, but it must be initialized with index.
```

### Comparing `pyquiet-0.0.2/src/qir/qModule/ClassicalInsnBase.py` & `pyquiet-0.0.3/src/pyquiet/qir/qModule/ClassicalInsnBase.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,64 @@
-from qir.qModule.InstructionBase import *
-from qir.Variable import *
-        
+from __future__ import annotations
+from pyquiet.qir.qModule.InstructionBase import InstructionBase
+from pyquiet.qir.Variable import QuietVariable
+
+
 class ArithmeticOpBase(InstructionBase):
-    def __init__(self, operation: str, dst_operand:QuietVariable, src_operand1: QuietVariable, src_operand2: QuietVariable or int or float, label: str = None) -> None:
+    def __init__(
+        self,
+        operation: str,
+        dst_operand: QuietVariable,
+        src_operand1: QuietVariable,
+        src_operand2: QuietVariable | int | float,
+        label: str = None,
+    ) -> None:
         super().__init__(operation, label)
         self.__d_operand = dst_operand
         self.__s_operand1 = src_operand1
         self.__s_operand2 = src_operand2
-    
+
     @property
     def src1(self) -> QuietVariable:
         return self.__s_operand1
-    
+
     @property
     def src2(self):
         return self.__s_operand2
-    
+
     @property
     def dst(self) -> QuietVariable:
         return self.__d_operand
-    
+
     def __str__(self) -> str:
         return f"{self.opname} {self.__d_operand}, {self.__s_operand1}, {self.__s_operand2}"
 
+
 class BranchOpBase(InstructionBase):
-    def __init__(self, operation: str, s_operand1:QuietVariable, s_operand2:QuietVariable, dst_label:str, label: str = None) -> None:
+    def __init__(
+        self,
+        operation: str,
+        s_operand1: QuietVariable,
+        s_operand2: QuietVariable,
+        dst_label: str,
+        label: str = None,
+    ) -> None:
         super().__init__(operation, label)
-        
+
         self.__src_operand1 = s_operand1
         self.__src_operand2 = s_operand2
         self.__dst_label = dst_label
-    
+
     @property
     def src1(self) -> QuietVariable:
         return self.__src_operand1
-    
+
     @property
     def src2(self) -> QuietVariable:
         return self.__src_operand2
-    
+
     @property
     def dst_label(self) -> str:
         return self.__dst_label
-    
+
     def __str__(self) -> str:
-        return f"{self.opname} {self.__src_operand1}, {self.__src_operand2}, {self.__dst_label}"
+        return f"{self.opname} {self.__src_operand1}, {self.__src_operand2}, {self.__dst_label}"
```

### Comparing `pyquiet-0.0.2/src/qir/qModule/ControlWords.py` & `pyquiet-0.0.3/src/pyquiet/qir/qModule/ControlWords.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-from qir.Variable import *
 from typing import List
+from pyquiet.qir.Variable import QiVariable
 
 ###########################################
 #        About Control Key Words.         #
 ###########################################
 
-class ControlWords():
+
+class ControlWords:
     def __init__(self) -> None:
         self.__ctrl = False
         # the control qubit is only one qubit.
-        self.__qubits: List[QiVariable] = None 
-    
+        self.__qubits: List[QiVariable] = None
+
     def set_ctrl(self) -> None:
         self.__ctrl = True
-    
+
     @property
     def ctrl(self) -> bool:
         return self.__ctrl
-    
+
     def set_qubits(self, qubits: List[QiVariable]) -> None:
         self.__qubits = qubits
-    
+
     @property
     def ctrl_qubits(self) -> List[QiVariable]:
-        return self.__qubits   
+        return self.__qubits
```

### Comparing `pyquiet-0.0.2/src/qir/qModule/IntInstruction.py` & `pyquiet-0.0.3/src/pyquiet/qir/qModule/IntInstruction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from qir.qModule.ClassicalInsnBase import *
+from typing import Union
+from pyquiet.qir.Variable import QiVariable, QuietVariable
+from pyquiet.qir.qModule.InstructionBase import InstructionBase
+from pyquiet.qir.qModule.ClassicalInsnBase import ArithmeticOpBase, BranchOpBase
 
 
 ###########################################
 #       Data Transfer Instructions        #
 ###########################################
 class Ld(InstructionBase):
     def __init__(
@@ -10,60 +13,62 @@
     ) -> None:
         super().__init__("ld", label)
         self.__d_operand = d_operand
         self.__s_operand = s_operand
 
     def __str__(self):
         return f"{super().__str__()} {self.__d_operand}, {self.__s_operand}"
-    
+
     @property
     def imm(self):
         return self.__s_operand
-    
+
     @property
     def dst(self) -> QuietVariable:
         return self.__d_operand
 
 
 class Mov(InstructionBase):
-    def __init__(self, d_operand: QuietVariable, s_operand: QuietVariable, label: str = None):
-        super().__init__("mov",  label)
+    def __init__(
+        self, d_operand: QuietVariable, s_operand: QuietVariable, label: str = None
+    ):
+        super().__init__("mov", label)
         self.__d_operand = d_operand
         self.__s_operand = s_operand
 
     def __str__(self):
         return f"{super().__str__()} {self.__d_operand}, {self.__s_operand}"
-    
+
     @property
     def src(self) -> QuietVariable:
         return self.__s_operand
-    
+
     @property
     def dst(self) -> QuietVariable:
         return self.__d_operand
 
 
 ###########################################
 #            Logic Instructions           #
 ###########################################
 class Lnot(InstructionBase):
     def __init__(
-        self, d_operand:QiVariable, s_operand:QiVariable, label: str = None
+        self, d_operand: QiVariable, s_operand: QiVariable, label: str = None
     ) -> None:
         super().__init__("lnot", label)
         self.__dst_operand = d_operand
         self.__src_operand = s_operand
 
     def __str__(self):
         return f"{self.opname} {self.__dst_operand}, {self.__dst_operand}"
-    
+
     @property
     def src(self) -> QuietVariable:
         return self.__src_operand
-    
+
     @property
     def dst(self) -> QuietVariable:
         return self.__dst_operand
 
 
 class Land(InstructionBase):
     def __init__(
@@ -76,23 +81,23 @@
         super().__init__("land", label)
         self.__dst_operand = d_operand
         self.__src_operand1 = s_operand1
         self.__src_operand2 = s_operand2
 
     def __str__(self):
         return f"{self.opname} {self.__dst_operand}, {self.__src_operand1}, {self.__src_operand2}"
-    
+
     @property
     def src1(self) -> QuietVariable:
         return self.__src_operand1
-    
+
     @property
     def src2(self) -> QuietVariable:
         return self.__src_operand2
-    
+
     @property
     def dst(self) -> QuietVariable:
         return self.__dst_operand
 
 
 class Lor(InstructionBase):
     def __init__(
@@ -105,23 +110,23 @@
         super().__init__("lor", label)
         self.__dst_operand = d_operand
         self.__src_operand1 = s_operand1
         self.__src_operand2 = s_operand2
 
     def __str__(self):
         return f"{self.opname} {self.__dst_operand}, {self.__src_operand1}, {self.__src_operand2}"
-    
+
     @property
     def src1(self) -> QuietVariable:
         return self.__src_operand1
-    
+
     @property
     def src2(self) -> QuietVariable:
         return self.__src_operand2
-    
+
     @property
     def dst(self) -> QuietVariable:
         return self.__dst_operand
 
 
 class Lxor(InstructionBase):
     def __init__(
@@ -134,31 +139,33 @@
         super().__init__("lxor", label)
         self.__dst_operand = d_operand
         self.__src_operand1 = s_operand1
         self.__src_operand2 = s_operand2
 
     def __str__(self):
         return f"{self.opname} {self.__dst_operand}, {self.__src_operand1}, {self.__src_operand2}"
-    
+
     @property
     def src1(self) -> QuietVariable:
         return self.__src_operand1
-    
+
     @property
     def src2(self) -> QuietVariable:
         return self.__src_operand2
-    
+
     @property
     def dst(self) -> QuietVariable:
         return self.__dst_operand
 
+
 ###########################################
 #         Arithmetic Instructions         #
 ###########################################
 
+
 class Add(ArithmeticOpBase):
     def __init__(
         self,
         d_operand: QuietVariable,
         s_operand1: QuietVariable,
         s_operand2: QuietVariable,
         label: str = None,
@@ -262,29 +269,31 @@
         label: str = None,
     ) -> None:
         super().__init__("divi", d_operand, s_operand1, s_operand2, label)
 
     def __str__(self):
         return super().__str__()
 
+
 ###########################################
 #       Branch and Jump Instruction       #
 ###########################################
 
+
 class Jump(InstructionBase):
     def __init__(self, dest_operand_label: str, insn_label: str = None) -> None:
         super().__init__("jump", insn_label)
         self.__label = dest_operand_label
 
     def __str__(self):
         return f"{super().__str__()} {self.__label}"
-    
+
     @property
     def destination_label(self) -> str:
-        return self.__label  
+        return self.__label
 
 
 class Bne(BranchOpBase):
     def __init__(
         self,
         s_operand1: QuietVariable,
         s_operand2: QuietVariable,
```

### Comparing `pyquiet-0.0.2/src/qir/qModule/QuietModules.py` & `pyquiet-0.0.3/src/pyquiet/qir/qModule/QuietModules.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,95 @@
 from typing import Union
-from qir.qModule.StdInstructions import *
-from qir.qModule.IntInstruction import *
-from qir.qModule.FloatInstructions import *
+from pyquiet.qir.qModule.StdInstructions import *
+from pyquiet.qir.qModule.IntInstruction import *
+from pyquiet.qir.qModule.FloatInstructions import *
+
 
 class Module:
     def __init__(self, name, instructions):
-        self.__module_name:str = name
-        self.__module_instructions:list = instructions
-    
+        self.__module_name: str = name
+        self.__module_instructions: list = instructions
+
     @property
     def module_name(self):
         return self.__module_name
-    
+
     @property
     def instructions_name(self):
         return [instr for instr in self.__module_instructions]
-    
+
 
 class StdModule(Module):
     def __init__(self):
         module_name = "std"
-        module_instructions = ["H", "X", "Y", "Z", "S", "T", "Sdag", "Tdag", "Rx", "Ry", "Rz", "Rxy", "CNOT", "CZ", "SWAP", "CP", "CRz", "U4",
+        module_instructions = [
+            "H",
+            "X",
+            "Y",
+            "Z",
+            "S",
+            "T",
+            "Sdag",
+            "Tdag",
+            "Rx",
+            "Ry",
+            "Rz",
+            "Rxy",
+            "CNOT",
+            "CZ",
+            "SWAP",
+            "CP",
+            "CRz",
+            "U4",
         ]
         super().__init__(module_name, module_instructions)
-            
-            
+
+
 class IntModule(Module):
     def __init__(self):
         module_name = "im"
-        module_instructions = ["jump", "ld", "mov", "lnot", "land", "lor", "lxor", "add", "sub", "mul", "div", "addi", "subi", "muli", "divi", "bne", "beq", "bgt", "bge", "blt", "ble",]
+        module_instructions = [
+            "jump",
+            "ld",
+            "mov",
+            "lnot",
+            "land",
+            "lor",
+            "lxor",
+            "add",
+            "sub",
+            "mul",
+            "div",
+            "addi",
+            "subi",
+            "muli",
+            "divi",
+            "bne",
+            "beq",
+            "bgt",
+            "bge",
+            "blt",
+            "ble",
+        ]
         super().__init__(module_name, module_instructions)
-        
+
 
 class FloatModule(Module):
     def __init__(self):
         module_name = "fm"
-        module_instructions = ["ldd", "movd", "addd", "subd", "muld", "divd", "adddi", "subdi", "muldi", "divdi",]
+        module_instructions = [
+            "ldd",
+            "movd",
+            "addd",
+            "subd",
+            "muld",
+            "divd",
+            "adddi",
+            "subdi",
+            "muldi",
+            "divdi",
+        ]
         super().__init__(module_name, module_instructions)
 
+
 QuietModule = Union[StdModule, IntModule, FloatModule]
-std = StdModule()
+std = StdModule()
```

### Comparing `pyquiet-0.0.2/src/qir/qModule/StdInstructions.py` & `pyquiet-0.0.3/src/pyquiet/qir/qModule/StdInstructions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from qir.qModule.InstructionBase import *
-from qir.Variable import *
 from typing import Union
 import numpy as np
-from qir.qModule.ControlWords import ControlWords
+from pyquiet.qir.Variable import QuietVariable
+from pyquiet.qir.qModule.InstructionBase import InstructionBase
+from pyquiet.qir.qModule.ControlWords import ControlWords
 
 
 ###########################################
 #         One Qubit Operations            #
 ###########################################
 class StdSingleQubitGate(InstructionBase):
     def __init__(
@@ -158,15 +158,15 @@
             )
         return self.__matrix
 
     @matrix.setter
     def matrix(self, matrix: np.ndarray):
         self.__matrix = matrix
 
-    def set_ctrl(self, c_word: ControlWords()) -> None:
+    def set_ctrl(self, c_word: ControlWords) -> None:
         self.__ctrl = c_word
 
     @property
     def ctrl_word(self) -> ControlWords:
         if self.__ctrl is None:
             raise ValueError("The instruction has not inited by control word yet.")
         return self.__ctrl
```

### Comparing `pyquiet-0.0.2/src/qir/qbody/BodySection.py` & `pyquiet-0.0.3/src/pyquiet/qir/qbody/BodySection.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict
-from qir.qbody.Function import *
-from qir.qbody.FunctionCall import *
+
+from pyquiet.qir.qbody.Function import QiFunction
 
 
 class QiBodySection:
     def __init__(self) -> None:
         self.__table: Dict[str, QiFunction] = {}
         # The measure operation is pre-defined in quiet-s.
         measure = QiFunction("measure")
```

### Comparing `pyquiet-0.0.2/src/qir/qbody/Function.py` & `pyquiet-0.0.3/src/pyquiet/qir/qbody/Function.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-from qir.qbody.VariableDecl import VariableDecl
-from qir.qgate.gate import *
 from typing import Dict, List
 
+from pyquiet.qir.qbody.VariableDecl import VariableDecl
+
 
 class QiLabelTable:
     def __init__(self) -> None:
-        self.__labels:Dict[str,int] = {}
-    
+        self.__labels: Dict[str, int] = {}
+
     def record(self, label: str, order: int):
         if label in self.__labels:
             raise ValueError(
                 "The label of instruction in a function body must be unique."
             )
         self.__labels[label] = order
 
     def index(self, label: str) -> int:
         if self.__labels[label] is None:
             raise ValueError("The label of instruction does not exist.")
         return self.__labels[label]
-    
-    def labels(self)->List[str]:
+
+    def labels(self) -> List[str]:
         return [label for label in self.__labels.keys()]
 
+
 class FunctionVariables:
     def __init__(self) -> None:
         self.__table: Dict[str, VariableDecl] = {}
 
     def try_emplace(self, decl: VariableDecl):
         var_name = decl.var.name
         if self.__table.get(var_name) != None:
             raise ValueError("The variable has been already declared.")
         self.__table[var_name] = decl
 
-    def get_variable(self, var_name:str):
+    def get_variable(self, var_name: str):
         if var_name not in self.__table:
             print("var name is:  ", var_name)
             print(self.__table)
             raise ValueError("The Variable has not been declared yet.")
         return self.__table[var_name].var
 
     @property
@@ -45,38 +46,37 @@
 
 
 class QiFunction:
     """
     The QiFunction is consist of function declaration and function body.
     The QiFunction can be identified by its function name.
         * func name: str
-    
+
     The function declaration is consist of input args and output args.
         * input args: []
         * output args: []
-    
+
     The function body is consist of a list of instructions.
         * function body: []
     """
-    
+
     def __init__(self, name: str = None) -> None:
         # The function name is public element.
-        self.func_name:str = name
-        
+        self.func_name: str = name
+
         # * 1. About Function Declaration
-        self.__input_args:List[VariableDecl] = []
-        self.__output_args:List[VariableDecl] = []
-        
+        self.__input_args: List[VariableDecl] = []
+        self.__output_args: List[VariableDecl] = []
+
         # The private elements.
         # * 2. About Function Body
         self.__func_body = []
         self.__label_table = QiLabelTable()
         self.__func_vars = FunctionVariables()
 
-    
     @property
     def declaration(self) -> str:
         inputs = ", ".join([str(arg) for arg in self.__input_args])
         o_args = ", ".join([str(arg) for arg in self.__output_args])
         outputs = f"-> {o_args}"
         if len(self.__output_args) == 0:
             outputs = ""
@@ -84,47 +84,46 @@
 
     @property
     def instrs(self) -> str:
         body = ""
         for instr in self.__func_body:
             body = f"{body}\n {instr}"
         return body
-    
+
     @property
     def body(self):
         return self.__func_body
-    
-    def init_input_args(self, args:List[VariableDecl] = None):
+
+    def init_input_args(self, args: List[VariableDecl] = None):
         if args is not None:
             for arg in args:
                 self.__func_vars.try_emplace(arg)
             self.__input_args = args
-    
+
     def init_output_args(self, args: List[VariableDecl] = None):
-        if args is not None:    
+        if args is not None:
             for arg in args:
                 self.__func_vars.try_emplace(arg)
             self.__output_args = args
-    
+
     def get_input_args(self) -> List[VariableDecl]:
         return self.__input_args
-    
+
     def get_output_args(self) -> List[VariableDecl]:
         return self.__output_args
-    
+
     def push_instr(self, instr):
         if instr.label is not None:
             index = len(self.__func_body)
             self.__label_table.record(instr.label, index)
         if isinstance(instr, VariableDecl):
             self.__func_vars.try_emplace(instr)
-        self.__func_body.append(instr)  
+        self.__func_body.append(instr)
 
     def var_list(self) -> FunctionVariables:
         return self.__func_vars
-    
+
     def label_table(self) -> QiLabelTable:
         return self.__label_table
 
-    def __str__(self)->str:
+    def __str__(self) -> str:
         return f"{self.declaration} \n {self.instrs}"
-
```

### Comparing `pyquiet-0.0.2/src/qir/qbody/FunctionCall.py` & `pyquiet-0.0.3/src/pyquiet/qir/qbody/FunctionCall.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from qir.qModule.InstructionBase import InstructionBase
-from qir.qbody.Function import QiFunction
+from pyquiet.qir.qModule.InstructionBase import InstructionBase
+from pyquiet.qir.qbody.Function import QiFunction
 
 
 class FunctionCall(InstructionBase):
     def __init__(
         self, func_name: str, inputs: list, outputs: list, label: str = None
     ) -> None:
         super().__init__(func_name, label)
```

### Comparing `pyquiet-0.0.2/src/qir/qfile/FileSection.py` & `pyquiet-0.0.3/src/pyquiet/qir/qfile/FileSection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from typing import Dict, List
-from qir.qfile.file import QiFile
+from pyquiet.qir.qfile.file import QiFile
+
 
 class QiFileSection:
     def __init__(self) -> None:
-        self.__table:Dict[str, QiFile] = {}
-    
-    def try_emplace(self, qi_include:QiFile):
+        self.__table: Dict[str, QiFile] = {}
+
+    def try_emplace(self, qi_include: QiFile):
         file_name = qi_include.file_name
         if self.__table.get(file_name) != None:
             raise ValueError("The QiFile has been already defined.")
         self.__table[file_name] = qi_include
-    
-    def get_file(self, file_name:str):
+
+    def get_file(self, file_name: str):
         file = self.__table.get(file_name)
         if file == None:
             raise ValueError("The file is not included yet.")
         return file
-    
-    def delete_file(self, file_name:str):
+
+    def delete_file(self, file_name: str):
         if self.__table.get(file_name) == None:
             raise ValueError("The file is not included yet.")
         del self.__table[file_name]
-    
+
     def included_files(self) -> List[QiFile]:
         files = [file for file in self.__table.values()]
         return files
-    
+
     def file_name_list(self) -> List[str]:
         files = [file for file in self.__table.keys()]
         return files
-    
+
     def __len__(self):
-        return len(self.__table)
+        return len(self.__table)
```

### Comparing `pyquiet-0.0.2/src/qir/qfile/file.py` & `pyquiet-0.0.3/src/pyquiet/qir/qfile/file.py`

 * *Files identical despite different names*

### Comparing `pyquiet-0.0.2/src/qir/qgate/GateSection.py` & `pyquiet-0.0.3/src/pyquiet/qir/qgate/GateSection.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from typing import Dict, List
-from types import new_class
-from qir.qgate.gate import QiDefineInfo
+from pyquiet.qir.qgate.gate import QiDefineInfo
 
 
 class QiGateSection:
     def __init__(self) -> None:
         self.__table: Dict[str, QiDefineInfo] = {}
 
     def try_emplace(self, qi_define: QiDefineInfo):
@@ -21,12 +20,12 @@
     @property
     def gate_names(self) -> List[str]:
         names = [name for name in self.__table.keys()]
         return names
 
     @property
     def infos(self) -> List[QiDefineInfo]:
-       infos = [gate for gate in self.__table.values()]
-       return infos 
+        infos = [gate for gate in self.__table.values()]
+        return infos
 
     def __len__(self):
         return len(self.__table)
```

### Comparing `pyquiet-0.0.2/src/qir/qgate/gate.py` & `pyquiet-0.0.3/src/pyquiet/qir/qgate/gate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,65 @@
 import math
-from qir.Variable import QuietVariable
-from qir.qModule.InstructionBase import InstructionBase
-from qir.qModule.ControlWords import ControlWords
 from typing import List
-from qir.qutils import gen_np_square_matrix
+from pyquiet.qir.Variable import QuietVariable
+from pyquiet.qir.qModule.InstructionBase import InstructionBase
+from pyquiet.qir.qModule.ControlWords import ControlWords
+from pyquiet.qir.qutils import gen_np_square_matrix
 
 
 class QiDefineInfo:
     def __init__(self, op_name: str, matrix: list) -> None:
         self.__name = op_name
         # form the matrix
         if int(math.log(len(matrix), 4)) % 1 != 0 & len(matrix) == 0:
             raise ValueError("Matrix size must be 4^n and not be equal to 0.")
         self.__matrix = gen_np_square_matrix(matrix)
-    
+
     @property
     def operation(self) -> str:
         return self.__name
 
     @property
     def matrix(self) -> list:
         return self.__matrix
-    
+
     def __str__(self) -> str:
         return f"{self.__name} {self.__matrix}"
 
+
 class QiDefineGate(InstructionBase):
-    def __init__(
-        self, qi_define: QiDefineInfo, label: str = None
-    ) -> None:
+    def __init__(self, qi_define: QiDefineInfo, label: str = None) -> None:
         super().__init__(qi_define.operation, label)
         self.__matrix = qi_define.matrix
         # check the operands and store them
         self.__qubits: List[QuietVariable] = None
         # control words.
-        self.__ctrl:ControlWords() = None 
+        self.__ctrl: ControlWords = None
 
     def operands(self, operands: List[QuietVariable]):
         qubits_num = math.log(len(self.__matrix), 2)
         if len(operands) != qubits_num:
             raise ValueError(
                 "The number of operands must be equal to log4 of matrix size."
             )
-        self.__qubits = operands  
-    
+        self.__qubits = operands
+
     @property
     def qubits(self):
         return self.__qubits
 
     @property
     def matrix(self):
         return self.__matrix
 
-    def set_ctrl(self, c_word: ControlWords()) -> None:
+    def set_ctrl(self, c_word: ControlWords) -> None:
         self.__ctrl = c_word
-    
+
     @property
     def ctrl_word(self) -> ControlWords:
         if self.__ctrl is None:
             raise ValueError("The instruction has not inited by control word yet.")
         return self.__ctrl
-    
+
     def __str__(self) -> str:
         qubits = ",".join(str(qubit) for qubit in self.__qubits)
         return f"{self.opname} {qubits}"
-    
-
-
-
```

