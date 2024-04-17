# Comparing `tmp/botocore-a-la-carte-emr-1.34.85.tar.gz` & `tmp/botocore-a-la-carte-emr-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-emr-1.34.85.tar", last modified: Wed Apr 17 01:00:58 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-emr-1.34.9.tar", last modified: Thu Dec 28 01:06:43 2023, max compression
```

## Comparing `botocore-a-la-carte-emr-1.34.85.tar` & `botocore-a-la-carte-emr-1.34.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:00:58.695626 botocore-a-la-carte-emr-1.34.85/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-17 01:00:58.000000 botocore-a-la-carte-emr-1.34.85/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-17 01:00:58.695626 botocore-a-la-carte-emr-1.34.85/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:00:58.691626 botocore-a-la-carte-emr-1.34.85/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:00:58.691626 botocore-a-la-carte-emr-1.34.85/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:00:58.691626 botocore-a-la-carte-emr-1.34.85/botocore/data/emr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:00:58.695626 botocore-a-la-carte-emr-1.34.85/botocore/data/emr/2009-03-31/
--rw-r--r--   0 runner    (1001) docker     (127)    15342 2024-04-17 01:00:41.000000 botocore-a-la-carte-emr-1.34.85/botocore/data/emr/2009-03-31/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 01:00:41.000000 botocore-a-la-carte-emr-1.34.85/botocore/data/emr/2009-03-31/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-17 01:00:41.000000 botocore-a-la-carte-emr-1.34.85/botocore/data/emr/2009-03-31/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   288523 2024-04-17 01:00:41.000000 botocore-a-la-carte-emr-1.34.85/botocore/data/emr/2009-03-31/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-17 01:00:41.000000 botocore-a-la-carte-emr-1.34.85/botocore/data/emr/2009-03-31/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 01:00:58.695626 botocore-a-la-carte-emr-1.34.85/botocore_a_la_carte_emr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-17 01:00:58.000000 botocore-a-la-carte-emr-1.34.85/botocore_a_la_carte_emr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-17 01:00:58.000000 botocore-a-la-carte-emr-1.34.85/botocore_a_la_carte_emr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 01:00:58.000000 botocore-a-la-carte-emr-1.34.85/botocore_a_la_carte_emr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 01:00:58.000000 botocore-a-la-carte-emr-1.34.85/botocore_a_la_carte_emr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 01:00:58.695626 botocore-a-la-carte-emr-1.34.85/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-17 01:00:58.000000 botocore-a-la-carte-emr-1.34.85/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:43.854295 botocore-a-la-carte-emr-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:43.000000 botocore-a-la-carte-emr-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2023-12-28 01:06:43.854295 botocore-a-la-carte-emr-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:43.850295 botocore-a-la-carte-emr-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:43.850295 botocore-a-la-carte-emr-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:43.850295 botocore-a-la-carte-emr-1.34.9/botocore/data/emr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:43.850295 botocore-a-la-carte-emr-1.34.9/botocore/data/emr/2009-03-31/
+-rw-r--r--   0 runner    (1001) docker     (127)    15342 2023-12-28 01:06:26.000000 botocore-a-la-carte-emr-1.34.9/botocore/data/emr/2009-03-31/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-28 01:06:26.000000 botocore-a-la-carte-emr-1.34.9/botocore/data/emr/2009-03-31/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2023-12-28 01:06:26.000000 botocore-a-la-carte-emr-1.34.9/botocore/data/emr/2009-03-31/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   285772 2023-12-28 01:06:26.000000 botocore-a-la-carte-emr-1.34.9/botocore/data/emr/2009-03-31/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2023-12-28 01:06:26.000000 botocore-a-la-carte-emr-1.34.9/botocore/data/emr/2009-03-31/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:43.854295 botocore-a-la-carte-emr-1.34.9/botocore_a_la_carte_emr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2023-12-28 01:06:43.000000 botocore-a-la-carte-emr-1.34.9/botocore_a_la_carte_emr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2023-12-28 01:06:43.000000 botocore-a-la-carte-emr-1.34.9/botocore_a_la_carte_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:43.000000 botocore-a-la-carte-emr-1.34.9/botocore_a_la_carte_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:43.000000 botocore-a-la-carte-emr-1.34.9/botocore_a_la_carte_emr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:43.854295 botocore-a-la-carte-emr-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2023-12-28 01:06:43.000000 botocore-a-la-carte-emr-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-emr-1.34.85/LICENSE.txt` & `botocore-a-la-carte-emr-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-emr-1.34.85/PKG-INFO` & `botocore-a-la-carte-emr-1.34.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-emr
-Version: 1.34.85
+Version: 1.34.9
 Summary: emr data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-emr-1.34.85/botocore/data/emr/2009-03-31/endpoint-rule-set-1.json` & `botocore-a-la-carte-emr-1.34.9/botocore/data/emr/2009-03-31/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-emr-1.34.85/botocore/data/emr/2009-03-31/paginators-1.json` & `botocore-a-la-carte-emr-1.34.9/botocore/data/emr/2009-03-31/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-emr-1.34.85/botocore/data/emr/2009-03-31/service-2.json` & `botocore-a-la-carte-emr-1.34.9/botocore/data/emr/2009-03-31/service-2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978191299178281%*

 * *Differences: {"'operations'": "{'SetTerminationProtection': {'documentation': '<p>SetTerminationProtection "*

 * *                 'locks a cluster (job flow) so the Amazon EC2 instances in the cluster cannot be '*

 * *                 'terminated by user intervention, an API call, or in the event of a job-flow '*

 * *                 'error. The cluster still terminates upon successful completion of the job flow. '*

 * *                 'Calling <code>SetTerminationProtection</code> on a cluster is similar to calling '*

 * *                 't […]*

```diff
@@ -967,45 +967,29 @@
             },
             "input": {
                 "shape": "SetKeepJobFlowAliveWhenNoStepsInput"
             },
             "name": "SetKeepJobFlowAliveWhenNoSteps"
         },
         "SetTerminationProtection": {
-            "documentation": "<p>SetTerminationProtection locks a cluster (job flow) so the Amazon EC2 instances in the cluster cannot be terminated by user intervention, an API call, or in the event of a job-flow error. The cluster still terminates upon successful completion of the job flow. Calling <code>SetTerminationProtection</code> on a cluster is similar to calling the Amazon EC2 <code>DisableAPITermination</code> API on all Amazon EC2 instances in a cluster.</p> <p> <code>SetTerminationProtection</code> is used to prevent accidental termination of a cluster and to ensure that in the event of an error, the instances persist so that you can recover any data stored in their ephemeral instance storage.</p> <p> To terminate a cluster that has been locked by setting <code>SetTerminationProtection</code> to <code>true</code>, you must first unlock the job flow by a subsequent call to <code>SetTerminationProtection</code> in which you set the value to <code>false</code>. </p> <p> For more information, see <a href=\"https://docs.aws.amazon.com/emr/latest/ManagementGuide/UsingEMR_TerminationProtection.html\">Managing Cluster Termination</a> in the <i>Amazon EMR Management Guide</i>. </p>",
+            "documentation": "<p>SetTerminationProtection locks a cluster (job flow) so the Amazon EC2 instances in the cluster cannot be terminated by user intervention, an API call, or in the event of a job-flow error. The cluster still terminates upon successful completion of the job flow. Calling <code>SetTerminationProtection</code> on a cluster is similar to calling the Amazon EC2 <code>DisableAPITermination</code> API on all Amazon EC2 instances in a cluster.</p> <p> <code>SetTerminationProtection</code> is used to prevent accidental termination of a cluster and to ensure that in the event of an error, the instances persist so that you can recover any data stored in their ephemeral instance storage.</p> <p> To terminate a cluster that has been locked by setting <code>SetTerminationProtection</code> to <code>true</code>, you must first unlock the job flow by a subsequent call to <code>SetTerminationProtection</code> in which you set the value to <code>false</code>. </p> <p> For more information, see<a href=\"https://docs.aws.amazon.com/emr/latest/ManagementGuide/UsingEMR_TerminationProtection.html\">Managing Cluster Termination</a> in the <i>Amazon EMR Management Guide</i>. </p>",
             "errors": [
                 {
                     "shape": "InternalServerError"
                 }
             ],
             "http": {
                 "method": "POST",
                 "requestUri": "/"
             },
             "input": {
                 "shape": "SetTerminationProtectionInput"
             },
             "name": "SetTerminationProtection"
         },
-        "SetUnhealthyNodeReplacement": {
-            "documentation": "<p>Specify whether to enable unhealthy node replacement, which lets Amazon EMR gracefully replace core nodes on a cluster if any nodes become unhealthy. For example, a node becomes unhealthy if disk usage is above 90%. If unhealthy node replacement is on and <code>TerminationProtected</code> are off, Amazon EMR immediately terminates the unhealthy core nodes. To use unhealthy node replacement and retain unhealthy core nodes, use to turn on termination protection. In such cases, Amazon EMR adds the unhealthy nodes to a denylist, reducing job interruptions and failures.</p> <p>If unhealthy node replacement is on, Amazon EMR notifies YARN and other applications on the cluster to stop scheduling tasks with these nodes, moves the data, and then terminates the nodes.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-plan-node-replacement.html\">graceful node replacement</a> in the <i>Amazon EMR Management Guide</i>.</p>",
-            "errors": [
-                {
-                    "shape": "InternalServerError"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "SetUnhealthyNodeReplacementInput"
-            },
-            "name": "SetUnhealthyNodeReplacement"
-        },
         "SetVisibleToAllUsers": {
             "documentation": "<important> <p>The SetVisibleToAllUsers parameter is no longer supported. Your cluster may be visible to all users in your account. To restrict cluster access using an IAM policy, see <a href=\"https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-plan-access-IAM.html\">Identity and Access Management for Amazon EMR</a>. </p> </important> <p>Sets the <a>Cluster$VisibleToAllUsers</a> value for an Amazon EMR cluster. When <code>true</code>, IAM principals in the Amazon Web Services account can perform Amazon EMR cluster actions that their IAM policies allow. When <code>false</code>, only the IAM principal that created the cluster and the Amazon Web Services account root user can perform Amazon EMR actions on the cluster, regardless of IAM permissions policies attached to other IAM principals.</p> <p>This action works on running clusters. When you create a cluster, use the <a>RunJobFlowInput$VisibleToAllUsers</a> parameter.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/emr/latest/ManagementGuide/security_IAM_emr-with-IAM.html#security_set_visible_to_all_users\">Understanding the Amazon EMR Cluster VisibleToAllUsers Setting</a> in the <i>Amazon EMR Management Guide</i>.</p>",
             "errors": [
                 {
                     "shape": "InternalServerError"
                 }
             ],
@@ -1646,15 +1630,15 @@
                     "shape": "String"
                 },
                 "MasterPublicDnsName": {
                     "documentation": "<p>The DNS name of the master node. If the cluster is on a private subnet, this is the private DNS name. On a public subnet, this is the public DNS name.</p>",
                     "shape": "String"
                 },
                 "Name": {
-                    "documentation": "<p>The name of the cluster. This parameter can't contain the characters &lt;, &gt;, $, |, or ` (backtick).</p>",
+                    "documentation": "<p>The name of the cluster.</p>",
                     "shape": "String"
                 },
                 "NormalizedInstanceHours": {
                     "documentation": "<p>An approximation of the cost of the cluster, represented in m1.small/hours. This value is incremented one time for every hour an m1.small instance runs. Larger instances are weighted more, so an Amazon EC2 instance that is roughly four times more expensive would result in the normalized instance hours being incremented by four. This result is only an approximation and does not reflect the actual billing rate.</p>",
                     "shape": "Integer"
                 },
                 "OSReleaseLabel": {
@@ -1709,18 +1693,14 @@
                     "documentation": "<p>A list of tags associated with a cluster.</p>",
                     "shape": "TagList"
                 },
                 "TerminationProtected": {
                     "documentation": "<p>Indicates whether Amazon EMR will lock the cluster to prevent the Amazon EC2 instances from being terminated by an API call or user intervention, or in the event of a cluster error.</p>",
                     "shape": "Boolean"
                 },
-                "UnhealthyNodeReplacement": {
-                    "documentation": "<p>Indicates whether Amazon EMR should gracefully replace Amazon EC2 core instances that have degraded within the cluster.</p>",
-                    "shape": "BooleanObject"
-                },
                 "VisibleToAllUsers": {
                     "documentation": "<p>Indicates whether the cluster is visible to IAM principals in the Amazon Web Services account associated with the cluster. When <code>true</code>, IAM principals in the Amazon Web Services account can perform Amazon EMR cluster actions on the cluster that their IAM policies allow. When <code>false</code>, only the IAM principal that created the cluster and the Amazon Web Services account root user can perform Amazon EMR actions, regardless of IAM permissions policies attached to other IAM principals.</p> <p>The default value is <code>true</code> if a value is not provided when creating a cluster using the Amazon EMR API <a>RunJobFlow</a> command, the CLI <a href=\"https://docs.aws.amazon.com/cli/latest/reference/emr/create-cluster.html\">create-cluster</a> command, or the Amazon Web Services Management Console.</p>",
                     "shape": "Boolean"
                 }
             },
             "type": "structure"
         },
@@ -3864,15 +3844,15 @@
                     "shape": "InstanceFleetConfigList"
                 },
                 "InstanceGroups": {
                     "documentation": "<p>Configuration for the instance groups in a cluster.</p>",
                     "shape": "InstanceGroupConfigList"
                 },
                 "KeepJobFlowAliveWhenNoSteps": {
-                    "documentation": "<p>Specifies whether the cluster should remain available after completing all steps. Defaults to <code>false</code>. For more information about configuring cluster termination, see <a href=\"https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-plan-termination.html\">Control Cluster Termination</a> in the <i>EMR Management Guide</i>.</p>",
+                    "documentation": "<p>Specifies whether the cluster should remain available after completing all steps. Defaults to <code>true</code>. For more information about configuring cluster termination, see <a href=\"https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-plan-termination.html\">Control Cluster Termination</a> in the <i>EMR Management Guide</i>.</p>",
                     "shape": "Boolean"
                 },
                 "MasterInstanceType": {
                     "documentation": "<p>The Amazon EC2 instance type of the master node.</p>",
                     "shape": "InstanceType"
                 },
                 "Placement": {
@@ -3886,18 +3866,14 @@
                 "SlaveInstanceType": {
                     "documentation": "<p>The Amazon EC2 instance type of the core and task nodes.</p>",
                     "shape": "InstanceType"
                 },
                 "TerminationProtected": {
                     "documentation": "<p>Specifies whether to lock the cluster to prevent the Amazon EC2 instances from being terminated by API call, user intervention, or in the event of a job-flow error.</p>",
                     "shape": "Boolean"
-                },
-                "UnhealthyNodeReplacement": {
-                    "documentation": "<p>Indicates whether Amazon EMR should gracefully replace core nodes that have degraded within the cluster.</p>",
-                    "shape": "BooleanObject"
                 }
             },
             "type": "structure"
         },
         "JobFlowInstancesDetail": {
             "documentation": "<p>Specify the type of Amazon EC2 instances that the cluster (job flow) runs on.</p>",
             "members": {
@@ -3948,18 +3924,14 @@
                 "SlaveInstanceType": {
                     "documentation": "<p>The Amazon EC2 core and task node instance type.</p>",
                     "shape": "InstanceType"
                 },
                 "TerminationProtected": {
                     "documentation": "<p>Specifies whether the Amazon EC2 instances in the cluster are protected from termination by API calls, user intervention, or in the event of a job-flow error.</p>",
                     "shape": "Boolean"
-                },
-                "UnhealthyNodeReplacement": {
-                    "documentation": "<p>Indicates whether Amazon EMR should gracefully replace core nodes that have degraded within the cluster.</p>",
-                    "shape": "BooleanObject"
                 }
             },
             "required": [
                 "MasterInstanceType",
                 "SlaveInstanceType",
                 "InstanceCount"
             ],
@@ -5464,31 +5436,14 @@
             },
             "required": [
                 "JobFlowIds",
                 "TerminationProtected"
             ],
             "type": "structure"
         },
-        "SetUnhealthyNodeReplacementInput": {
-            "members": {
-                "JobFlowIds": {
-                    "documentation": "<p>The list of strings that uniquely identify the clusters for which to turn on unhealthy node replacement. You can get these identifiers by running the <a>RunJobFlow</a> or the <a>DescribeJobFlows</a> operations.</p>",
-                    "shape": "XmlStringList"
-                },
-                "UnhealthyNodeReplacement": {
-                    "documentation": "<p>Indicates whether to turn on or turn off graceful unhealthy node replacement.</p>",
-                    "shape": "BooleanObject"
-                }
-            },
-            "required": [
-                "JobFlowIds",
-                "UnhealthyNodeReplacement"
-            ],
-            "type": "structure"
-        },
         "SetVisibleToAllUsersInput": {
             "documentation": "<p>The input to the SetVisibleToAllUsers action.</p>",
             "members": {
                 "JobFlowIds": {
                     "documentation": "<p>The unique identifier of the job flow (cluster).</p>",
                     "shape": "XmlStringList"
                 },
```

### Comparing `botocore-a-la-carte-emr-1.34.85/botocore/data/emr/2009-03-31/waiters-2.json` & `botocore-a-la-carte-emr-1.34.9/botocore/data/emr/2009-03-31/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-emr-1.34.85/botocore_a_la_carte_emr.egg-info/PKG-INFO` & `botocore-a-la-carte-emr-1.34.9/botocore_a_la_carte_emr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-emr
-Version: 1.34.85
+Version: 1.34.9
 Summary: emr data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-emr-1.34.85/setup.py` & `botocore-a-la-carte-emr-1.34.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-emr',
-    version="1.34.85",
+    version="1.34.9",
     description='emr data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/emr/*/*.json'],
```

