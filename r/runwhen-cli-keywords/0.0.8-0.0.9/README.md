# Comparing `tmp/runwhen-cli-keywords-0.0.8.tar.gz` & `tmp/runwhen-cli-keywords-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runwhen-cli-keywords-0.0.8.tar", last modified: Sun Nov 19 04:39:49 2023, max compression
+gzip compressed data, was "runwhen-cli-keywords-0.0.9.tar", last modified: Tue Nov 21 15:34:11 2023, max compression
```

## Comparing `runwhen-cli-keywords-0.0.8.tar` & `runwhen-cli-keywords-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 04:39:49.244361 runwhen-cli-keywords-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11339 2023-11-19 04:39:46.000000 runwhen-cli-keywords-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-19 04:39:46.000000 runwhen-cli-keywords-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    24266 2023-11-19 04:39:49.244361 runwhen-cli-keywords-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23745 2023-11-19 04:39:46.000000 runwhen-cli-keywords-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 04:39:49.240361 runwhen-cli-keywords-0.0.8/RW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 04:39:49.240361 runwhen-cli-keywords-0.0.8/RW/CLI/
--rw-r--r--   0 runner    (1001) docker     (127)    12753 2023-11-19 04:39:46.000000 runwhen-cli-keywords-0.0.8/RW/CLI/CLI.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-11-19 04:39:46.000000 runwhen-cli-keywords-0.0.8/RW/CLI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2023-11-19 04:39:46.000000 runwhen-cli-keywords-0.0.8/RW/CLI/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18845 2023-11-19 04:39:46.000000 runwhen-cli-keywords-0.0.8/RW/CLI/json_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2023-11-19 04:39:46.000000 runwhen-cli-keywords-0.0.8/RW/CLI/local_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    18730 2023-11-19 04:39:46.000000 runwhen-cli-keywords-0.0.8/RW/CLI/stdout_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 04:39:49.240361 runwhen-cli-keywords-0.0.8/RW/K8sApplications/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-19 04:39:46.000000 runwhen-cli-keywords-0.0.8/RW/K8sApplications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6209 2023-11-19 04:39:46.000000 runwhen-cli-keywords-0.0.8/RW/K8sApplications/k8s_applications.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-19 04:39:46.000000 runwhen-cli-keywords-0.0.8/RW/K8sApplications/migrations_inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5025 2023-11-19 04:39:46.000000 runwhen-cli-keywords-0.0.8/RW/K8sApplications/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15312 2023-11-19 04:39:46.000000 runwhen-cli-keywords-0.0.8/RW/K8sApplications/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 04:39:49.240361 runwhen-cli-keywords-0.0.8/RW/NextSteps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 04:39:49.240361 runwhen-cli-keywords-0.0.8/RW/NextSteps/Kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2023-11-19 04:39:46.000000 runwhen-cli-keywords-0.0.8/RW/NextSteps/Kubernetes/mapping.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5079 2023-11-19 04:39:46.000000 runwhen-cli-keywords-0.0.8/RW/NextSteps/Suggest.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-19 04:39:46.000000 runwhen-cli-keywords-0.0.8/RW/NextSteps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2023-11-19 04:39:46.000000 runwhen-cli-keywords-0.0.8/RW/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-19 04:39:49.240361 runwhen-cli-keywords-0.0.8/runwhen_cli_keywords.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24266 2023-11-19 04:39:49.000000 runwhen-cli-keywords-0.0.8/runwhen_cli_keywords.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      667 2023-11-19 04:39:49.000000 runwhen-cli-keywords-0.0.8/runwhen_cli_keywords.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-19 04:39:49.000000 runwhen-cli-keywords-0.0.8/runwhen_cli_keywords.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-11-19 04:39:49.000000 runwhen-cli-keywords-0.0.8/runwhen_cli_keywords.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2023-11-19 04:39:49.000000 runwhen-cli-keywords-0.0.8/runwhen_cli_keywords.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-11-19 04:39:49.244361 runwhen-cli-keywords-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      810 2023-11-19 04:39:46.000000 runwhen-cli-keywords-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:34:11.172309 runwhen-cli-keywords-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11339 2023-11-21 15:34:08.000000 runwhen-cli-keywords-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-21 15:34:08.000000 runwhen-cli-keywords-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    25558 2023-11-21 15:34:11.176309 runwhen-cli-keywords-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25037 2023-11-21 15:34:08.000000 runwhen-cli-keywords-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:34:11.172309 runwhen-cli-keywords-0.0.9/RW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:34:11.172309 runwhen-cli-keywords-0.0.9/RW/CLI/
+-rw-r--r--   0 runner    (1001) docker     (127)    13531 2023-11-21 15:34:08.000000 runwhen-cli-keywords-0.0.9/RW/CLI/CLI.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2023-11-21 15:34:08.000000 runwhen-cli-keywords-0.0.9/RW/CLI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2023-11-21 15:34:08.000000 runwhen-cli-keywords-0.0.9/RW/CLI/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18845 2023-11-21 15:34:08.000000 runwhen-cli-keywords-0.0.9/RW/CLI/json_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2023-11-21 15:34:08.000000 runwhen-cli-keywords-0.0.9/RW/CLI/local_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18730 2023-11-21 15:34:08.000000 runwhen-cli-keywords-0.0.9/RW/CLI/stdout_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:34:11.172309 runwhen-cli-keywords-0.0.9/RW/K8sApplications/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-21 15:34:08.000000 runwhen-cli-keywords-0.0.9/RW/K8sApplications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2023-11-21 15:34:08.000000 runwhen-cli-keywords-0.0.9/RW/K8sApplications/k8s_applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-21 15:34:08.000000 runwhen-cli-keywords-0.0.9/RW/K8sApplications/migrations_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5025 2023-11-21 15:34:08.000000 runwhen-cli-keywords-0.0.9/RW/K8sApplications/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15312 2023-11-21 15:34:08.000000 runwhen-cli-keywords-0.0.9/RW/K8sApplications/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:34:11.172309 runwhen-cli-keywords-0.0.9/RW/NextSteps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:34:11.172309 runwhen-cli-keywords-0.0.9/RW/NextSteps/Kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2023-11-21 15:34:08.000000 runwhen-cli-keywords-0.0.9/RW/NextSteps/Kubernetes/mapping.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5079 2023-11-21 15:34:08.000000 runwhen-cli-keywords-0.0.9/RW/NextSteps/Suggest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-21 15:34:08.000000 runwhen-cli-keywords-0.0.9/RW/NextSteps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2023-11-21 15:34:08.000000 runwhen-cli-keywords-0.0.9/RW/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 15:34:11.172309 runwhen-cli-keywords-0.0.9/runwhen_cli_keywords.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25558 2023-11-21 15:34:11.000000 runwhen-cli-keywords-0.0.9/runwhen_cli_keywords.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2023-11-21 15:34:11.000000 runwhen-cli-keywords-0.0.9/runwhen_cli_keywords.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 15:34:11.000000 runwhen-cli-keywords-0.0.9/runwhen_cli_keywords.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2023-11-21 15:34:11.000000 runwhen-cli-keywords-0.0.9/runwhen_cli_keywords.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2023-11-21 15:34:11.000000 runwhen-cli-keywords-0.0.9/runwhen_cli_keywords.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-11-21 15:34:11.176309 runwhen-cli-keywords-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2023-11-21 15:34:08.000000 runwhen-cli-keywords-0.0.9/setup.py
```

### Comparing `runwhen-cli-keywords-0.0.8/LICENSE` & `runwhen-cli-keywords-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `runwhen-cli-keywords-0.0.8/PKG-INFO` & `runwhen-cli-keywords-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: runwhen-cli-keywords
-Version: 0.0.8
+Version: 0.0.9
 Summary: A set of RunWhen published CLI keywords and python libraries for interacting with APIs using CLIs
 Home-page: https://github.com/runwhen-contrib/rw-cli-codecollection
 Author: Kyle Forster
 Author-email: kyle.forster@runwhen.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Troubleshooting Tasks in Codecollection: **123**
-Codebundles in Codecollection: **44**
+Troubleshooting Tasks in Codecollection: **128**
+Codebundles in Codecollection: **45**
 
 ![](docs/GitHub_Banner.jpg)
 
 <p align="center">
   <a href="https://discord.gg/Ut7Ws4rm8Q">
     <img src="https://img.shields.io/discord/1131539039665791077?label=Join%20Discord&logo=discord&logoColor=white&style=for-the-badge" alt="Join Discord">
   </a>
@@ -64,45 +64,46 @@
 |---|---|---|---|
 | [AWS CloudWatch Overutlized EC2 Inspection](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/aws-cloudwatch-overused-ec2/runbook.robot) | `AWS`, `CloudWatch` | `Check For Overutilized Ec2 Instances` | Queries AWS CloudWatch for a list of EC2 instances with a high amount of resource utilization, raising issues when overutilized instances are found. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/aws-cloudwatch-overused-ec2) |
 | [AWS EKS Nodegroup Status Check](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/aws-eks-node-reboot/runbook.robot) | `AWS`, `EKS` | `Check EKS Nodegroup Status` | Queries a node group within a EKS cluster to check if the nodegroup has degraded service, indicating ongoing reboots or other issues. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/aws-eks-node-reboot) |
 | [Azure Internal LoadBalancer Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/azure-loadbalancer-triage/runbook.robot) | `Kubernetes`, `AKS`, `Azure` | `Health Check Internal Azure Load Balancer` | Triages issues related to a Azure Loadbalancers and its activity logs. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/azure-loadbalancer-triage) |
 | [Azure Monitor Activity Log SLI](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/azure-monitor-event-triage/sli.robot) | `Kubernetes`, `AKS`, `Azure` | `Run Azure Monitor Activity Log Triage` | Measures the count of error activity log entries as a SLI metric for the Azure tenancy. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/azure-monitor-event-triage) |
 | [Azure Monitor Event Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/azure-monitor-event-triage/runbook.robot) | `Kubernetes`, `AKS`, `Azure` | `Run Azure Monitor Activity Log Triage` | Triages issues related to a Azure Loadbalancers, Kubernetes ingress objects and services. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/azure-monitor-event-triage) |
 | [GCP Gcloud Log Inspection](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/gcloud-log-inspection/runbook.robot) | `GCP`, `Gcloud`, `Google Monitoring` | `Inspect GCP Logs For Common Errors` | Fetches logs from a GCP using a configurable query and raises an issue with details on the most common issues. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/gcloud-log-inspection) |
-| [GCP Node Prempt List](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/gcloud-node-preempt/runbook.robot) | `GCP`, `GKE` | `List all nodes in an active prempt operation` | List all GCP nodes that have an active preempt operation. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/gcloud-node-preempt) |
+| [GCP Node Prempt List](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/gcloud-node-preempt/sli.robot) | `GCP`, `GKE` | `Count the number of nodes in active prempt operation` | Check if any GCP nodes have an active preempt operation. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/gcloud-node-preempt) |
 | [GKE Kong Ingress Host Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/curl-gmp-kong-ingress-inspection/runbook.robot) | `GCP`, `GMP`, `Ingress`, `Kong`, `Metrics` | `Check If Kong Ingress HTTP Error Rate Violates HTTP Error Threshold`, `Check If Kong Ingress HTTP Request Latency Violates Threshold`, `Check If Kong Ingress Controller Reports Upstream Errors` | Collects Kong ingress host metrics from GMP on GCP and inspects the results for ingress with a HTTP error code rate greater than zero over a configurable duration and raises issues based on the number of ingress with error codes. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/curl-gmp-kong-ingress-inspection) |
-| [GKE Nginx Ingress Host Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/curl-gmp-nginx-ingress-inspection/runbook.robot) | `GCP`, `GMP`, `Ingress`, `Nginx`, `Metrics` | `Fetch Nginx Ingress HTTP Errors From GMP And Perform Inspection On Results`, `Find Ingress Owner and Service Health` | Collects Nginx ingress host controller metrics from GMP on GCP and inspects the results for ingress with a HTTP error code rate greater than zero over a configurable duration and raises issues based on the number of ingress with error codes. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/curl-gmp-nginx-ingress-inspection) |
+| [GKE Nginx Ingress Host Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/curl-gmp-nginx-ingress-inspection/runbook.robot) | `GCP`, `GMP`, `Ingress`, `Nginx`, `Metrics` | `Fetch Nginx HTTP Errors From GMP for Ingress `${INGRESS_OBJECT_NAME}``, `Find Owner and Service Health for Ingress `${INGRESS_OBJECT_NAME}`` | Collects Nginx ingress host controller metrics from GMP on GCP and inspects the results for ingress with a HTTP error code rate greater than zero over a configurable duration and raises issues based on the number of ingress with error codes. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/curl-gmp-nginx-ingress-inspection) |
 | [Kubeprometheus Operator Troubleshoot](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-prometheus-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Prometheus` | `Check Prometheus Service Monitors`, `Check For Successful Rule Setup`, `Verify Prometheus RBAC Can Access ServiceMonitors`, `Identify Endpoint Scraping Errors`, `Check Prometheus API Healthy` | This taskset investigates the logs, state and health of Kubernetes Prometheus operator. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-prometheus-healthcheck) |
-| [Kubernetes Application Troubleshoot](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-app-troubleshoot/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Resource Logs`, `Scan For Misconfigured Environment` | Triages issues related to a deployment and its replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-app-troubleshoot) |
+| [Kubernetes Application Monitor](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-app-troubleshoot/sli.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Measure Application Exceptions` | Measures the number of exception stacktraces present in an application's logs over a time period. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-app-troubleshoot) |
+| [Kubernetes Application Troubleshoot](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-app-troubleshoot/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Workload Logs`, `Scan For Misconfigured Environment`, `Troubleshoot Application Logs` | Triages issues related to a deployment and its replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-app-troubleshoot) |
 | [Kubernetes ArgoCD Application Health & Troubleshoot](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-argocd-application-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `ArgoCD` | `Fetch ArgoCD Application Sync Status & Health`, `Fetch ArgoCD Application Last Sync Operation Details`, `Fetch Unhealthy ArgoCD Application Resources`, `Scan For Errors in Pod Logs Related to ArgoCD Application Deployments`, `Fully Describe ArgoCD Application` | This taskset collects information and runs general troubleshooting checks against argocd application objects within a namespace. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-argocd-application-health) |
 | [Kubernetes ArgoCD HelmRelease TaskSet](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-argocd-helm-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `ArgoCD` | `Fetch all available ArgoCD Helm releases`, `Fetch Installed ArgoCD Helm release versions` | This codebundle runs a series of tasks to identify potential helm release issues related to ArgoCD managed Helm objects. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-argocd-helm-health) |
 | [Kubernetes Artifactory Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-artifactory-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Artifactory` | `Check Artifactory Liveness and Readiness Endpoints` | Performs a triage on the Open Source version of Artifactory in a Kubernetes cluster. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-artifactory-health) |
-| [Kubernetes CertManager Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-certmanager-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `CertManager` | `Get Namespace Certificate Summary`, `Find Failed Certificate Requests and Identify Issues` | This taskset checks that your cert manager certificates are renewing as expected, raising issues when they are past due in the configured namespace [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-certmanager-healthcheck) |
+| [Kubernetes CertManager Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-certmanager-healthcheck/sli.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Health Score of CertManager Workloads` | Check the health of pods deployed by cert-manager. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-certmanager-healthcheck) |
 | [Kubernetes Daemonset Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-daemonset-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get DaemonSet Log Details For Report`, `Get Related Daemonset Events`, `Check Daemonset Replicas` | Triages issues related to a Daemonset and its available replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-daemonset-healthcheck) |
-| [Kubernetes Deployment Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-deployment-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Check Deployment Log For Issues`, `Troubleshoot Deployment Warning Events`, `Get Deployment Workload Details For Report`, `Troubleshoot Deployment Replicas`, `Check For Deployment Event Anomalies` | Triages issues related to a deployment and its replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-deployment-healthcheck) |
+| [Kubernetes Deployment Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-deployment-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Check Deployment Log For Issues with `${DEPLOYMENT_NAME}``, `Check Liveness Probe Configuration for Deployment `${DEPLOYMENT_NAME}``, `Check Readiness Probe Configuration for Deployment `${DEPLOYMENT_NAME}``, `Troubleshoot Deployment Warning Events for `${DEPLOYMENT_NAME}``, `Get Deployment Workload Details For `${DEPLOYMENT_NAME}` and Add to Report`, `Troubleshoot Deployment Replicas for `${DEPLOYMENT_NAME}``, `Check Deployment Event Anomalies for `${DEPLOYMENT_NAME}`` | Triages issues related to a deployment and its replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-deployment-healthcheck) |
 | [Kubernetes Flux Choas Testing](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-chaos-flux/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Suspend the Flux Resource Reconciliation`, `Find Random FluxCD Workload as Chaos Target`, `Execute Chaos Command`, `Execute Additional Chaos Command`, `Resume Flux Resource Reconciliation` | This taskset is used to suspend a flux resource for the purposes of executing chaos tasks. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-chaos-flux) |
 | [Kubernetes FluxCD HelmRelease TaskSet](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-fluxcd-helm-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `FluxCD` | `List all available FluxCD Helmreleases`, `Fetch Installed FluxCD Helmrelease Versions`, `Fetch Mismatched FluxCD HelmRelease Version`, `Fetch FluxCD HelmRelease Error Messages`, `Check for Available Helm Chart Updates` | This codebundle runs a series of tasks to identify potential helm release issues related to Flux managed Helm objects. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-fluxcd-helm-health) |
 | [Kubernetes FluxCD Kustomization TaskSet](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-fluxcd-kustomization-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `FluxCD` | `List all available Kustomization objects`, `Get details for unready Kustomizations` | This codebundle runs a series of tasks to identify potential Kustomization issues related to Flux managed Kustomization objects. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-fluxcd-kustomization-health) |
 | [Kubernetes Grafana Loki Health Check](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-loki-healthcheck/runbook.robot) | `k8s` | `Check Loki Ring API`, `Check Loki API Ready` | This taskset checks the health of Grafana Loki and its hash ring. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-loki-healthcheck) |
-| [Kubernetes Image Check](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-image-check/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Check Image Rollover Times In Namespace`, `List Images and Tags for Every Container in Running Pods`, `List Images and Tags for Every Container in Failed Pods`, `List ImagePullBackOff Events and Test Path and Tags` | This taskset provides detailed information about the images used in a Kubernetes namespace. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-image-check) |
+| [Kubernetes Image Check](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-image-check/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Check Image Rollover Times for Namespace `${NAMESPACE}``, `List Images and Tags for Every Container in Running Pods for Namespace `${NAMESPACE}``, `List Images and Tags for Every Container in Failed Pods for Namespace `${NAMESPACE}``, `List ImagePullBackOff Events and Test Path and Tags for Namespace `${NAMESPACE}`` | This taskset provides detailed information about the images used in a Kubernetes namespace. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-image-check) |
 | [Kubernetes Ingress GCE & GCP HTTP Load Balancer Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-ingress-gce-healthcheck/runbook.robot) | `Kubernetes`, `GKE`, `GCE`, `GCP` | `Search For GCE Ingress Warnings in GKE`, `Identify Unhealthy GCE HTTP Ingress Backends`, `Validate GCP HTTP Load Balancer Configurations`, `Fetch Network Error Logs from GCP Operations Manager for Ingress Backends`, `Review GCP Operations Logging Dashboard` | Troubleshoot GCE Ingress Resources related to GCP HTTP Load Balancer in GKE [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-ingress-gce-healthcheck) |
-| [Kubernetes Ingress Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-ingress-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Fetch Ingress Object Health in Namespace` | Triages issues related to a ingress objects and services. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-ingress-healthcheck) |
+| [Kubernetes Ingress Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-ingress-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Fetch Ingress Object Health in Namespace `${NAMESPACE}``, `Check for Ingress and Service Conflicts in Namespace `${NAMESPACE}`` | Triages issues related to a ingress objects and services. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-ingress-healthcheck) |
 | [Kubernetes Jenkins Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-jenkins-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Jenkins` | `Query The Jenkins Kubernetes Workload HTTP Endpoint`, `Query For Stuck Jenkins Jobs` | This taskset collects information about perstistent volumes and persistent volume claims to validate health or help troubleshoot potential issues. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-jenkins-healthcheck) |
 | [Kubernetes Labeled Pod Count](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-labeledpods-healthcheck/sli.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Measure Number of Running Pods with Label` | This codebundle fetches the number of running pods with the set of provided labels, letting you measure the number of running pods. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-labeledpods-healthcheck) |
 | [Kubernetes Namespace Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-namespace-healthcheck/sli.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Event Count and Score`, `Get Container Restarts and Score`, `Get NotReady Pods`, `Generate Namspace Score` | This SLI uses kubectl to score namespace health. Produces a value between 0 (completely failing thet test) and 1 (fully passing the test). Looks for container restarts, events, and pods not ready. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-namespace-healthcheck) |
-| [Kubernetes Namespace Troubleshoot](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-namespace-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Trace And Troubleshoot Namespace Warning Events And Errors`, `Troubleshoot Container Restarts In Namespace`, `Troubleshoot Pending Pods In Namespace`, `Troubleshoot Failed Pods In Namespace`, `Troubleshoot Workload Status Conditions In Namespace`, `Get Listing Of Resources In Namespace`, `Check For Namespace Event Anomalies`, `Troubleshoot Namespace Services And Application Workloads`, `Check Missing or Risky PodDisruptionBudget Policies` | This taskset runs general troubleshooting checks against all applicable objects in a namespace, checks error events, and searches pod logs for error entries. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-namespace-healthcheck) |
-| [Kubernetes Persistent Volume Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-pvc-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Fetch Events for Unhealthy Kubernetes PersistentVolumeClaims`, `List PersistentVolumeClaims in Terminating State`, `List PersistentVolumes in Terminating State`, `List Pods with Attached Volumes and Related PersistentVolume Details`, `Fetch the Storage Utilization for PVC Mounts`, `Check for RWO Persistent Volume Node Attachment Issues` | This taskset collects information about storage such as PersistentVolumes and PersistentVolumeClaims to validate health or help troubleshoot potential storage issues. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-pvc-healthcheck) |
-| [Kubernetes Pod Resources Scan](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-podresources-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Scan Labeled Pods and Show All Containers Without Resource Limit or Resource Requests Set`, `Get Labeled Container Top Info` | Inspects the resources provisioned for a given set of pods, selected by their labels and raises issues if no resources were specified. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-podresources-health) |
+| [Kubernetes Namespace Troubleshoot](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-namespace-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Troubleshoot Warning Events in Namespace `${NAMESPACE}``, `Troubleshoot Container Restarts In Namespace `${NAMESPACE}``, `Troubleshoot Pending Pods In Namespace `${NAMESPACE}``, `Troubleshoot Failed Pods In Namespace `${NAMESPACE}``, `Troubleshoot Workload Status Conditions In Namespace `${NAMESPACE}``, `Get Listing Of Resources In Namespace `${NAMESPACE}``, `Check Event Anomalies in Namespace `${NAMESPACE}``, `Troubleshoot Services And Application Workloads in Namespace `${NAMESPACE}``, `Check Missing or Risky PodDisruptionBudget Policies in Namepace `${NAMESPACE}`` | This taskset runs general troubleshooting checks against all applicable objects in a namespace. Looks for warning events, odd or frequent normal events, restarting containers and failed or pending pods. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-namespace-healthcheck) |
+| [Kubernetes Persistent Volume Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-pvc-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Fetch Events for Unhealthy Kubernetes PersistentVolumeClaims in Namespace `${NAMESPACE}``, `List PersistentVolumeClaims in Terminating State in Namespace `${NAMESPACE}``, `List PersistentVolumes in Terminating State in Namespace `${NAMESPACE}``, `List Pods with Attached Volumes and Related PersistentVolume Details in Namespace `${NAMESPACE}``, `Fetch the Storage Utilization for PVC Mounts in Namespace `${NAMESPACE}``, `Check for RWO Persistent Volume Node Attachment Issues in Namespace `${NAMESPACE}`` | This taskset collects information about storage such as PersistentVolumes and PersistentVolumeClaims to validate health or help troubleshoot potential storage issues. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-pvc-healthcheck) |
+| [Kubernetes Pod Resources Scan](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-podresources-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Show Pods Without Resource Limit or Resource Requests Set in Namespace `${NAMESPACE}``, `Get Pod Resource Utilization with Top in Namespace `${NAMESPACE}`` | Inspects the resources provisioned for a given set of pods, selected by their labels and raises issues if no resources were specified. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-podresources-health) |
 | [Kubernetes Postgres Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-postgres-triage/runbook.robot) | `AKS`, `EKS`, `GKE`, `Kubernetes`, `Patroni`, `Postgres` | `Get Standard Postgres Resource Information`, `Describe Postgres Custom Resources`, `Get Postgres Pod Logs & Events`, `Get Postgres Pod Resource Utilization`, `Get Running Postgres Configuration`, `Get Patroni Output`, `Run DB Queries` | Runs multiple Kubernetes and psql commands to report on the health of a postgres cluster. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-postgres-triage) |
-| [Kubernetes Redis Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-redis-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Redis` | `Ping Redis Workload`, `Verify Redis Read Write Operation` | This taskset collects information on your redis workload in your Kubernetes cluster and raises issues if any health checks fail. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-redis-healthcheck) |
+| [Kubernetes Redis Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-redis-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Redis` | `Ping `${DEPLOYMENT_NAME}` Redis Workload`, `Verify `${DEPLOYMENT_NAME}` Redis Read Write Operation` | This taskset collects information on your redis workload in your Kubernetes cluster and raises issues if any health checks fail. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-redis-healthcheck) |
 | [Kubernetes Restart resource](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-restart-resource/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Current Resource State`, `Get Resource Logs`, `Restart Resource` | This taskset restarts a resource with a given set of labels, typically used with other tasksets. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-restart-resource) |
 | [Kubernetes Service Account Check](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-serviceaccount-check/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Redis` | `Test Service Account Access to Kubernetes API Server` | This taskset provides tasks to troubleshoot service accounts in a Kubernetes namespace. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-serviceaccount-check) |
-| [Kubernetes StatefulSet Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-statefulset-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Fetch StatefulSet Logs`, `Get Related StatefulSet Events`, `Fetch StatefulSet Manifest Details`, `List StatefulSets with Unhealthy Replica Counts` | Triages issues related to a StatefulSet and its replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-statefulset-healthcheck) |
+| [Kubernetes StatefulSet Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-statefulset-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Fetch StatefulSet `${STATEFULSET_NAME}` Logs`, `Get Related StatefulSet `${STATEFULSET_NAME}` Events`, `Fetch StatefulSet `${STATEFULSET_NAME}` Manifest Details`, `List StatefulSets with Unhealthy Replica Counts In Namespace `${NAMESPACE}`` | Triages issues related to a StatefulSet and its replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-statefulset-healthcheck) |
 | [Kubernetes Vault Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-vault-healthcheck/runbook.robot) | `AKS`, `EKS`, `GKE`, `Kubernetes`, `Vault` | `Fetch Vault CSI Driver Logs`, `Get Vault CSI Driver Warning Events`, `Check Vault CSI Driver Replicas`, `Fetch Vault Logs`, `Get Related Vault Events`, `Fetch Vault StatefulSet Manifest Details`, `Fetch Vault DaemonSet Manifest Details`, `Verify Vault Availability`, `Check Vault StatefulSet Replicas` | A suite of tasks that can be used to triage potential issues in your vault namespace. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-vault-healthcheck) |
 | [Terraform Cloud Workspace Lock Check](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/terraform-cloud-workspace-lock-check/runbook.robot) | `Terraform Cloud` | `Checking whether the Terraform Cloud Workspace is in a locked state` | Check whether the Terraform Cloud Workspace is in a locked state. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/terraform-cloud-workspace-lock-check) |
 | [Test Issues](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/test-issue/runbook.robot) | `Test` | `Raise Full Issue` | A codebundle for testing the issues feature. Purely for testing flow. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/test-issue) |
-| [cURL HTTP OK](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/curl-http-ok/runbook.robot) | `Linux macOS Windows HTTP` | `Checking HTTP URL Is Available And Timely` | This taskset uses curl to validate the response code of the endpoint and provides the total time of the request. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/curl-http-ok) |
+| [cURL HTTP OK](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/curl-http-ok/sli.robot) | `Linux macOS Windows HTTP` | `Checking HTTP URL Is Available And Timely` | This taskset uses curl to validate the response code of the endpoint. Returns ascore of 1 if healthy, an 0 if unhealthy. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/curl-http-ok) |
 | [cli-test-taskset](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/cli-test/runbook.robot) | `cli` | `Run CLI and Parse Output For Issues`, `Exec Test`, `Local Process Test` | This taskset smoketests the CLI codebundle setup and run process [Docs](https://docs.runwhen.com/public/v/cli-codecollection/cli-test) |
 | [cmd-test-taskset](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/cmd-test/runbook.robot) | `cmd` | `Run CLI Command`, `Run Bash File`, `Log Suggestion` | This taskset smoketests the CLI codebundle setup and run process by running a bare command [Docs](https://docs.runwhen.com/public/v/cli-codecollection/cmd-test) |
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: runwhen-cli-keywords Version: 0.0.8 Summary: A set
+Metadata-Version: 2.1 Name: runwhen-cli-keywords Version: 0.0.9 Summary: A set
 of RunWhen published CLI keywords and python libraries for interacting with
 APIs using CLIs Home-page: https://github.com/runwhen-contrib/rw-cli-
 codecollection Author: Kyle Forster Author-email: kyle.forster@runwhen.com
 License: Apache License 2.0 Platform: UNKNOWN Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown License-File: LICENSE Troubleshooting
-Tasks in Codecollection: **123** Codebundles in Codecollection: **44** ![]
+Tasks in Codecollection: **128** Codebundles in Codecollection: **45** ![]
 (docs/GitHub_Banner.jpg)
                                 _[_J_o_i_n_ _D_i_s_c_o_r_d_]
                                  _[_J_o_i_n_ _S_l_a_c_k_]
 _[_O_p_e_n_ _i_n_ _G_i_t_H_u_b_ _C_o_d_e_s_p_a_c_e_s_]# RunWhen Public Codecollection This repository is a
 codecollection that is to be used within the RunWhen platform. It contains
 codebundles that can be used in SLIs, and TaskSets. Please see the **
 [contributing](CONTRIBUTING.md)** and **[code of conduct](CODE_OF_CONDUCT.md)**
@@ -63,91 +63,99 @@
 public/v/cli-codecollection/azure-monitor-event-triage) | | [GCP Gcloud Log
 Inspection](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
 codebundles/gcloud-log-inspection/runbook.robot) | `GCP`, `Gcloud`, `Google
 Monitoring` | `Inspect GCP Logs For Common Errors` | Fetches logs from a GCP
 using a configurable query and raises an issue with details on the most common
 issues. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/gcloud-log-
 inspection) | | [GCP Node Prempt List](https://github.com/runwhen-contrib/rw-
-cli-codecollection/blob/main/codebundles/gcloud-node-preempt/runbook.robot) |
-`GCP`, `GKE` | `List all nodes in an active prempt operation` | List all GCP
-nodes that have an active preempt operation. [Docs](https://docs.runwhen.com/
-public/v/cli-codecollection/gcloud-node-preempt) | | [GKE Kong Ingress Host
-Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
-codebundles/curl-gmp-kong-ingress-inspection/runbook.robot) | `GCP`, `GMP`,
-`Ingress`, `Kong`, `Metrics` | `Check If Kong Ingress HTTP Error Rate Violates
-HTTP Error Threshold`, `Check If Kong Ingress HTTP Request Latency Violates
-Threshold`, `Check If Kong Ingress Controller Reports Upstream Errors` |
-Collects Kong ingress host metrics from GMP on GCP and inspects the results for
-ingress with a HTTP error code rate greater than zero over a configurable
+cli-codecollection/blob/main/codebundles/gcloud-node-preempt/sli.robot) |
+`GCP`, `GKE` | `Count the number of nodes in active prempt operation` | Check
+if any GCP nodes have an active preempt operation. [Docs](https://
+docs.runwhen.com/public/v/cli-codecollection/gcloud-node-preempt) | | [GKE Kong
+Ingress Host Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/
+blob/main/codebundles/curl-gmp-kong-ingress-inspection/runbook.robot) | `GCP`,
+`GMP`, `Ingress`, `Kong`, `Metrics` | `Check If Kong Ingress HTTP Error Rate
+Violates HTTP Error Threshold`, `Check If Kong Ingress HTTP Request Latency
+Violates Threshold`, `Check If Kong Ingress Controller Reports Upstream Errors`
+| Collects Kong ingress host metrics from GMP on GCP and inspects the results
+for ingress with a HTTP error code rate greater than zero over a configurable
 duration and raises issues based on the number of ingress with error codes.
 [Docs](https://docs.runwhen.com/public/v/cli-codecollection/curl-gmp-kong-
 ingress-inspection) | | [GKE Nginx Ingress Host Triage](https://github.com/
 runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/curl-gmp-nginx-
 ingress-inspection/runbook.robot) | `GCP`, `GMP`, `Ingress`, `Nginx`, `Metrics`
-| `Fetch Nginx Ingress HTTP Errors From GMP And Perform Inspection On Results`,
-`Find Ingress Owner and Service Health` | Collects Nginx ingress host
-controller metrics from GMP on GCP and inspects the results for ingress with a
-HTTP error code rate greater than zero over a configurable duration and raises
-issues based on the number of ingress with error codes. [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/curl-gmp-nginx-ingress-inspection)
-| | [Kubeprometheus Operator Troubleshoot](https://github.com/runwhen-contrib/
-rw-cli-codecollection/blob/main/codebundles/k8s-prometheus-healthcheck/
-runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Prometheus` |
-`Check Prometheus Service Monitors`, `Check For Successful Rule Setup`, `Verify
-Prometheus RBAC Can Access ServiceMonitors`, `Identify Endpoint Scraping
-Errors`, `Check Prometheus API Healthy` | This taskset investigates the logs,
-state and health of Kubernetes Prometheus operator. [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/k8s-prometheus-healthcheck) | |
+| `Fetch Nginx HTTP Errors From GMP for Ingress `${INGRESS_OBJECT_NAME}``,
+`Find Owner and Service Health for Ingress `${INGRESS_OBJECT_NAME}`` | Collects
+Nginx ingress host controller metrics from GMP on GCP and inspects the results
+for ingress with a HTTP error code rate greater than zero over a configurable
+duration and raises issues based on the number of ingress with error codes.
+[Docs](https://docs.runwhen.com/public/v/cli-codecollection/curl-gmp-nginx-
+ingress-inspection) | | [Kubeprometheus Operator Troubleshoot](https://
+github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-
+prometheus-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`,
+`OpenShift`, `Prometheus` | `Check Prometheus Service Monitors`, `Check For
+Successful Rule Setup`, `Verify Prometheus RBAC Can Access ServiceMonitors`,
+`Identify Endpoint Scraping Errors`, `Check Prometheus API Healthy` | This
+taskset investigates the logs, state and health of Kubernetes Prometheus
+operator. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-
+prometheus-healthcheck) | | [Kubernetes Application Monitor](https://
+github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-app-
+troubleshoot/sli.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` |
+`Measure Application Exceptions` | Measures the number of exception stacktraces
+present in an application's logs over a time period. [Docs](https://
+docs.runwhen.com/public/v/cli-codecollection/k8s-app-troubleshoot) | |
 [Kubernetes Application Troubleshoot](https://github.com/runwhen-contrib/rw-
 cli-codecollection/blob/main/codebundles/k8s-app-troubleshoot/runbook.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Resource Logs`, `Scan For
-Misconfigured Environment` | Triages issues related to a deployment and its
-replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-app-
-troubleshoot) | | [Kubernetes ArgoCD Application Health & Troubleshoot](https:/
-/github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-
-argocd-application-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`,
-`OpenShift`, `ArgoCD` | `Fetch ArgoCD Application Sync Status & Health`, `Fetch
-ArgoCD Application Last Sync Operation Details`, `Fetch Unhealthy ArgoCD
-Application Resources`, `Scan For Errors in Pod Logs Related to ArgoCD
-Application Deployments`, `Fully Describe ArgoCD Application` | This taskset
-collects information and runs general troubleshooting checks against argocd
-application objects within a namespace. [Docs](https://docs.runwhen.com/public/
-v/cli-codecollection/k8s-argocd-application-health) | | [Kubernetes ArgoCD
-HelmRelease TaskSet](https://github.com/runwhen-contrib/rw-cli-codecollection/
-blob/main/codebundles/k8s-argocd-helm-health/runbook.robot) | `Kubernetes`,
-`AKS`, `EKS`, `GKE`, `OpenShift`, `ArgoCD` | `Fetch all available ArgoCD Helm
-releases`, `Fetch Installed ArgoCD Helm release versions` | This codebundle
-runs a series of tasks to identify potential helm release issues related to
-ArgoCD managed Helm objects. [Docs](https://docs.runwhen.com/public/v/cli-
-codecollection/k8s-argocd-helm-health) | | [Kubernetes Artifactory Triage]
-(https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
-codebundles/k8s-artifactory-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`,
-`GKE`, `OpenShift`, `Artifactory` | `Check Artifactory Liveness and Readiness
-Endpoints` | Performs a triage on the Open Source version of Artifactory in a
-Kubernetes cluster. [Docs](https://docs.runwhen.com/public/v/cli-
-codecollection/k8s-artifactory-health) | | [Kubernetes CertManager Healthcheck]
-(https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
-codebundles/k8s-certmanager-healthcheck/runbook.robot) | `Kubernetes`, `AKS`,
-`EKS`, `GKE`, `OpenShift`, `CertManager` | `Get Namespace Certificate Summary`,
-`Find Failed Certificate Requests and Identify Issues` | This taskset checks
-that your cert manager certificates are renewing as expected, raising issues
-when they are past due in the configured namespace [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/k8s-certmanager-healthcheck) | |
-[Kubernetes Daemonset Triage](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/k8s-daemonset-healthcheck/runbook.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get DaemonSet Log Details For
-Report`, `Get Related Daemonset Events`, `Check Daemonset Replicas` | Triages
-issues related to a Daemonset and its available replicas. [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/k8s-daemonset-healthcheck) | |
-[Kubernetes Deployment Triage](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/k8s-deployment-healthcheck/runbook.robot)
-| `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Check Deployment Log For
-Issues`, `Troubleshoot Deployment Warning Events`, `Get Deployment Workload
-Details For Report`, `Troubleshoot Deployment Replicas`, `Check For Deployment
-Event Anomalies` | Triages issues related to a deployment and its replicas.
+`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Workload Logs`, `Scan For
+Misconfigured Environment`, `Troubleshoot Application Logs` | Triages issues
+related to a deployment and its replicas. [Docs](https://docs.runwhen.com/
+public/v/cli-codecollection/k8s-app-troubleshoot) | | [Kubernetes ArgoCD
+Application Health & Troubleshoot](https://github.com/runwhen-contrib/rw-cli-
+codecollection/blob/main/codebundles/k8s-argocd-application-health/
+runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `ArgoCD` |
+`Fetch ArgoCD Application Sync Status & Health`, `Fetch ArgoCD Application Last
+Sync Operation Details`, `Fetch Unhealthy ArgoCD Application Resources`, `Scan
+For Errors in Pod Logs Related to ArgoCD Application Deployments`, `Fully
+Describe ArgoCD Application` | This taskset collects information and runs
+general troubleshooting checks against argocd application objects within a
+namespace. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-
+argocd-application-health) | | [Kubernetes ArgoCD HelmRelease TaskSet](https://
+github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-
+argocd-helm-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`,
+`OpenShift`, `ArgoCD` | `Fetch all available ArgoCD Helm releases`, `Fetch
+Installed ArgoCD Helm release versions` | This codebundle runs a series of
+tasks to identify potential helm release issues related to ArgoCD managed Helm
+objects. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-
+argocd-helm-health) | | [Kubernetes Artifactory Triage](https://github.com/
+runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-artifactory-
+health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`,
+`Artifactory` | `Check Artifactory Liveness and Readiness Endpoints` | Performs
+a triage on the Open Source version of Artifactory in a Kubernetes cluster.
+[Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-artifactory-
+health) | | [Kubernetes CertManager Healthcheck](https://github.com/runwhen-
+contrib/rw-cli-codecollection/blob/main/codebundles/k8s-certmanager-
+healthcheck/sli.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get
+Health Score of CertManager Workloads` | Check the health of pods deployed by
+cert-manager. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-
+certmanager-healthcheck) | | [Kubernetes Daemonset Triage](https://github.com/
+runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-daemonset-
+healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` |
+`Get DaemonSet Log Details For Report`, `Get Related Daemonset Events`, `Check
+Daemonset Replicas` | Triages issues related to a Daemonset and its available
+replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-
+daemonset-healthcheck) | | [Kubernetes Deployment Triage](https://github.com/
+runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-deployment-
+healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` |
+`Check Deployment Log For Issues with `${DEPLOYMENT_NAME}``, `Check Liveness
+Probe Configuration for Deployment `${DEPLOYMENT_NAME}``, `Check Readiness
+Probe Configuration for Deployment `${DEPLOYMENT_NAME}``, `Troubleshoot
+Deployment Warning Events for `${DEPLOYMENT_NAME}``, `Get Deployment Workload
+Details For `${DEPLOYMENT_NAME}` and Add to Report`, `Troubleshoot Deployment
+Replicas for `${DEPLOYMENT_NAME}``, `Check Deployment Event Anomalies for `$
+{DEPLOYMENT_NAME}`` | Triages issues related to a deployment and its replicas.
 [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-deployment-
 healthcheck) | | [Kubernetes Flux Choas Testing](https://github.com/runwhen-
 contrib/rw-cli-codecollection/blob/main/codebundles/k8s-chaos-flux/
 runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Suspend the
 Flux Resource Reconciliation`, `Find Random FluxCD Workload as Chaos Target`,
 `Execute Chaos Command`, `Execute Additional Chaos Command`, `Resume Flux
 Resource Reconciliation` | This taskset is used to suspend a flux resource for
@@ -171,116 +179,126 @@
 health) | | [Kubernetes Grafana Loki Health Check](https://github.com/runwhen-
 contrib/rw-cli-codecollection/blob/main/codebundles/k8s-loki-healthcheck/
 runbook.robot) | `k8s` | `Check Loki Ring API`, `Check Loki API Ready` | This
 taskset checks the health of Grafana Loki and its hash ring. [Docs](https://
 docs.runwhen.com/public/v/cli-codecollection/k8s-loki-healthcheck) | |
 [Kubernetes Image Check](https://github.com/runwhen-contrib/rw-cli-
 codecollection/blob/main/codebundles/k8s-image-check/runbook.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Check Image Rollover Times In
-Namespace`, `List Images and Tags for Every Container in Running Pods`, `List
-Images and Tags for Every Container in Failed Pods`, `List ImagePullBackOff
-Events and Test Path and Tags` | This taskset provides detailed information
-about the images used in a Kubernetes namespace. [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/k8s-image-check) | | [Kubernetes
-Ingress GCE & GCP HTTP Load Balancer Healthcheck](https://github.com/runwhen-
-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-ingress-gce-
-healthcheck/runbook.robot) | `Kubernetes`, `GKE`, `GCE`, `GCP` | `Search For
-GCE Ingress Warnings in GKE`, `Identify Unhealthy GCE HTTP Ingress Backends`,
-`Validate GCP HTTP Load Balancer Configurations`, `Fetch Network Error Logs
-from GCP Operations Manager for Ingress Backends`, `Review GCP Operations
-Logging Dashboard` | Troubleshoot GCE Ingress Resources related to GCP HTTP
-Load Balancer in GKE [Docs](https://docs.runwhen.com/public/v/cli-
+`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Check Image Rollover Times
+for Namespace `${NAMESPACE}``, `List Images and Tags for Every Container in
+Running Pods for Namespace `${NAMESPACE}``, `List Images and Tags for Every
+Container in Failed Pods for Namespace `${NAMESPACE}``, `List ImagePullBackOff
+Events and Test Path and Tags for Namespace `${NAMESPACE}`` | This taskset
+provides detailed information about the images used in a Kubernetes namespace.
+[Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-image-check) |
+| [Kubernetes Ingress GCE & GCP HTTP Load Balancer Healthcheck](https://
+github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-
+ingress-gce-healthcheck/runbook.robot) | `Kubernetes`, `GKE`, `GCE`, `GCP` |
+`Search For GCE Ingress Warnings in GKE`, `Identify Unhealthy GCE HTTP Ingress
+Backends`, `Validate GCP HTTP Load Balancer Configurations`, `Fetch Network
+Error Logs from GCP Operations Manager for Ingress Backends`, `Review GCP
+Operations Logging Dashboard` | Troubleshoot GCE Ingress Resources related to
+GCP HTTP Load Balancer in GKE [Docs](https://docs.runwhen.com/public/v/cli-
 codecollection/k8s-ingress-gce-healthcheck) | | [Kubernetes Ingress
 Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/
 main/codebundles/k8s-ingress-healthcheck/runbook.robot) | `Kubernetes`, `AKS`,
-`EKS`, `GKE`, `OpenShift` | `Fetch Ingress Object Health in Namespace` |
-Triages issues related to a ingress objects and services. [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/k8s-ingress-healthcheck) | |
-[Kubernetes Jenkins Healthcheck](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/k8s-jenkins-healthcheck/runbook.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Jenkins` | `Query The Jenkins
-Kubernetes Workload HTTP Endpoint`, `Query For Stuck Jenkins Jobs` | This
-taskset collects information about perstistent volumes and persistent volume
-claims to validate health or help troubleshoot potential issues. [Docs](https:/
-/docs.runwhen.com/public/v/cli-codecollection/k8s-jenkins-healthcheck) | |
-[Kubernetes Labeled Pod Count](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/k8s-labeledpods-healthcheck/sli.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Measure Number of Running
-Pods with Label` | This codebundle fetches the number of running pods with the
-set of provided labels, letting you measure the number of running pods. [Docs]
-(https://docs.runwhen.com/public/v/cli-codecollection/k8s-labeledpods-
-healthcheck) | | [Kubernetes Namespace Healthcheck](https://github.com/runwhen-
-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-namespace-healthcheck/
-sli.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Event Count
-and Score`, `Get Container Restarts and Score`, `Get NotReady Pods`, `Generate
-Namspace Score` | This SLI uses kubectl to score namespace health. Produces a
-value between 0 (completely failing thet test) and 1 (fully passing the test).
-Looks for container restarts, events, and pods not ready. [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/k8s-namespace-healthcheck) | |
-[Kubernetes Namespace Troubleshoot](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/k8s-namespace-healthcheck/runbook.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Trace And Troubleshoot
-Namespace Warning Events And Errors`, `Troubleshoot Container Restarts In
-Namespace`, `Troubleshoot Pending Pods In Namespace`, `Troubleshoot Failed Pods
-In Namespace`, `Troubleshoot Workload Status Conditions In Namespace`, `Get
-Listing Of Resources In Namespace`, `Check For Namespace Event Anomalies`,
-`Troubleshoot Namespace Services And Application Workloads`, `Check Missing or
-Risky PodDisruptionBudget Policies` | This taskset runs general troubleshooting
-checks against all applicable objects in a namespace, checks error events, and
-searches pod logs for error entries. [Docs](https://docs.runwhen.com/public/v/
-cli-codecollection/k8s-namespace-healthcheck) | | [Kubernetes Persistent Volume
+`EKS`, `GKE`, `OpenShift` | `Fetch Ingress Object Health in Namespace `$
+{NAMESPACE}``, `Check for Ingress and Service Conflicts in Namespace `$
+{NAMESPACE}`` | Triages issues related to a ingress objects and services.
+[Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-ingress-
+healthcheck) | | [Kubernetes Jenkins Healthcheck](https://github.com/runwhen-
+contrib/rw-cli-codecollection/blob/main/codebundles/k8s-jenkins-healthcheck/
+runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Jenkins` |
+`Query The Jenkins Kubernetes Workload HTTP Endpoint`, `Query For Stuck Jenkins
+Jobs` | This taskset collects information about perstistent volumes and
+persistent volume claims to validate health or help troubleshoot potential
+issues. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-
+jenkins-healthcheck) | | [Kubernetes Labeled Pod Count](https://github.com/
+runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-labeledpods-
+healthcheck/sli.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` |
+`Measure Number of Running Pods with Label` | This codebundle fetches the
+number of running pods with the set of provided labels, letting you measure the
+number of running pods. [Docs](https://docs.runwhen.com/public/v/cli-
+codecollection/k8s-labeledpods-healthcheck) | | [Kubernetes Namespace
 Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/
-main/codebundles/k8s-pvc-healthcheck/runbook.robot) | `Kubernetes`, `AKS`,
-`EKS`, `GKE`, `OpenShift` | `Fetch Events for Unhealthy Kubernetes
-PersistentVolumeClaims`, `List PersistentVolumeClaims in Terminating State`,
-`List PersistentVolumes in Terminating State`, `List Pods with Attached Volumes
-and Related PersistentVolume Details`, `Fetch the Storage Utilization for PVC
-Mounts`, `Check for RWO Persistent Volume Node Attachment Issues` | This
-taskset collects information about storage such as PersistentVolumes and
-PersistentVolumeClaims to validate health or help troubleshoot potential
-storage issues. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/
-k8s-pvc-healthcheck) | | [Kubernetes Pod Resources Scan](https://github.com/
-runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-podresources-
-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Scan
-Labeled Pods and Show All Containers Without Resource Limit or Resource
-Requests Set`, `Get Labeled Container Top Info` | Inspects the resources
-provisioned for a given set of pods, selected by their labels and raises issues
-if no resources were specified. [Docs](https://docs.runwhen.com/public/v/cli-
-codecollection/k8s-podresources-health) | | [Kubernetes Postgres Triage](https:
-//github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-
-postgres-triage/runbook.robot) | `AKS`, `EKS`, `GKE`, `Kubernetes`, `Patroni`,
+main/codebundles/k8s-namespace-healthcheck/sli.robot) | `Kubernetes`, `AKS`,
+`EKS`, `GKE`, `OpenShift` | `Get Event Count and Score`, `Get Container
+Restarts and Score`, `Get NotReady Pods`, `Generate Namspace Score` | This SLI
+uses kubectl to score namespace health. Produces a value between 0 (completely
+failing thet test) and 1 (fully passing the test). Looks for container
+restarts, events, and pods not ready. [Docs](https://docs.runwhen.com/public/v/
+cli-codecollection/k8s-namespace-healthcheck) | | [Kubernetes Namespace
+Troubleshoot](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/
+main/codebundles/k8s-namespace-healthcheck/runbook.robot) | `Kubernetes`,
+`AKS`, `EKS`, `GKE`, `OpenShift` | `Troubleshoot Warning Events in Namespace `$
+{NAMESPACE}``, `Troubleshoot Container Restarts In Namespace `${NAMESPACE}``,
+`Troubleshoot Pending Pods In Namespace `${NAMESPACE}``, `Troubleshoot Failed
+Pods In Namespace `${NAMESPACE}``, `Troubleshoot Workload Status Conditions In
+Namespace `${NAMESPACE}``, `Get Listing Of Resources In Namespace `$
+{NAMESPACE}``, `Check Event Anomalies in Namespace `${NAMESPACE}``,
+`Troubleshoot Services And Application Workloads in Namespace `${NAMESPACE}``,
+`Check Missing or Risky PodDisruptionBudget Policies in Namepace `$
+{NAMESPACE}`` | This taskset runs general troubleshooting checks against all
+applicable objects in a namespace. Looks for warning events, odd or frequent
+normal events, restarting containers and failed or pending pods. [Docs](https:/
+/docs.runwhen.com/public/v/cli-codecollection/k8s-namespace-healthcheck) | |
+[Kubernetes Persistent Volume Healthcheck](https://github.com/runwhen-contrib/
+rw-cli-codecollection/blob/main/codebundles/k8s-pvc-healthcheck/runbook.robot)
+| `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Fetch Events for Unhealthy
+Kubernetes PersistentVolumeClaims in Namespace `${NAMESPACE}``, `List
+PersistentVolumeClaims in Terminating State in Namespace `${NAMESPACE}``, `List
+PersistentVolumes in Terminating State in Namespace `${NAMESPACE}``, `List Pods
+with Attached Volumes and Related PersistentVolume Details in Namespace `$
+{NAMESPACE}``, `Fetch the Storage Utilization for PVC Mounts in Namespace `$
+{NAMESPACE}``, `Check for RWO Persistent Volume Node Attachment Issues in
+Namespace `${NAMESPACE}`` | This taskset collects information about storage
+such as PersistentVolumes and PersistentVolumeClaims to validate health or help
+troubleshoot potential storage issues. [Docs](https://docs.runwhen.com/public/
+v/cli-codecollection/k8s-pvc-healthcheck) | | [Kubernetes Pod Resources Scan]
+(https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
+codebundles/k8s-podresources-health/runbook.robot) | `Kubernetes`, `AKS`,
+`EKS`, `GKE`, `OpenShift` | `Show Pods Without Resource Limit or Resource
+Requests Set in Namespace `${NAMESPACE}``, `Get Pod Resource Utilization with
+Top in Namespace `${NAMESPACE}`` | Inspects the resources provisioned for a
+given set of pods, selected by their labels and raises issues if no resources
+were specified. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/
+k8s-podresources-health) | | [Kubernetes Postgres Triage](https://github.com/
+runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-postgres-
+triage/runbook.robot) | `AKS`, `EKS`, `GKE`, `Kubernetes`, `Patroni`,
 `Postgres` | `Get Standard Postgres Resource Information`, `Describe Postgres
 Custom Resources`, `Get Postgres Pod Logs & Events`, `Get Postgres Pod Resource
 Utilization`, `Get Running Postgres Configuration`, `Get Patroni Output`, `Run
 DB Queries` | Runs multiple Kubernetes and psql commands to report on the
 health of a postgres cluster. [Docs](https://docs.runwhen.com/public/v/cli-
 codecollection/k8s-postgres-triage) | | [Kubernetes Redis Healthcheck](https://
 github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-
 redis-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`,
-`OpenShift`, `Redis` | `Ping Redis Workload`, `Verify Redis Read Write
-Operation` | This taskset collects information on your redis workload in your
-Kubernetes cluster and raises issues if any health checks fail. [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/k8s-redis-healthcheck) | |
-[Kubernetes Restart resource](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/k8s-restart-resource/runbook.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Current Resource State`,
-`Get Resource Logs`, `Restart Resource` | This taskset restarts a resource with
-a given set of labels, typically used with other tasksets. [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/k8s-restart-resource) | |
-[Kubernetes Service Account Check](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/k8s-serviceaccount-check/runbook.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Redis` | `Test Service Account
-Access to Kubernetes API Server` | This taskset provides tasks to troubleshoot
-service accounts in a Kubernetes namespace. [Docs](https://docs.runwhen.com/
-public/v/cli-codecollection/k8s-serviceaccount-check) | | [Kubernetes
-StatefulSet Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/
-blob/main/codebundles/k8s-statefulset-healthcheck/runbook.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Fetch StatefulSet Logs`, `Get
-Related StatefulSet Events`, `Fetch StatefulSet Manifest Details`, `List
-StatefulSets with Unhealthy Replica Counts` | Triages issues related to a
+`OpenShift`, `Redis` | `Ping `${DEPLOYMENT_NAME}` Redis Workload`, `Verify `$
+{DEPLOYMENT_NAME}` Redis Read Write Operation` | This taskset collects
+information on your redis workload in your Kubernetes cluster and raises issues
+if any health checks fail. [Docs](https://docs.runwhen.com/public/v/cli-
+codecollection/k8s-redis-healthcheck) | | [Kubernetes Restart resource](https:/
+/github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-
+restart-resource/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`,
+`OpenShift` | `Get Current Resource State`, `Get Resource Logs`, `Restart
+Resource` | This taskset restarts a resource with a given set of labels,
+typically used with other tasksets. [Docs](https://docs.runwhen.com/public/v/
+cli-codecollection/k8s-restart-resource) | | [Kubernetes Service Account Check]
+(https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
+codebundles/k8s-serviceaccount-check/runbook.robot) | `Kubernetes`, `AKS`,
+`EKS`, `GKE`, `OpenShift`, `Redis` | `Test Service Account Access to Kubernetes
+API Server` | This taskset provides tasks to troubleshoot service accounts in a
+Kubernetes namespace. [Docs](https://docs.runwhen.com/public/v/cli-
+codecollection/k8s-serviceaccount-check) | | [Kubernetes StatefulSet Triage]
+(https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
+codebundles/k8s-statefulset-healthcheck/runbook.robot) | `Kubernetes`, `AKS`,
+`EKS`, `GKE`, `OpenShift` | `Fetch StatefulSet `${STATEFULSET_NAME}` Logs`,
+`Get Related StatefulSet `${STATEFULSET_NAME}` Events`, `Fetch StatefulSet `$
+{STATEFULSET_NAME}` Manifest Details`, `List StatefulSets with Unhealthy
+Replica Counts In Namespace `${NAMESPACE}`` | Triages issues related to a
 StatefulSet and its replicas. [Docs](https://docs.runwhen.com/public/v/cli-
 codecollection/k8s-statefulset-healthcheck) | | [Kubernetes Vault Triage]
 (https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
 codebundles/k8s-vault-healthcheck/runbook.robot) | `AKS`, `EKS`, `GKE`,
 `Kubernetes`, `Vault` | `Fetch Vault CSI Driver Logs`, `Get Vault CSI Driver
 Warning Events`, `Check Vault CSI Driver Replicas`, `Fetch Vault Logs`, `Get
 Related Vault Events`, `Fetch Vault StatefulSet Manifest Details`, `Fetch Vault
@@ -294,21 +312,21 @@
 | Check whether the Terraform Cloud Workspace is in a locked state. [Docs]
 (https://docs.runwhen.com/public/v/cli-codecollection/terraform-cloud-
 workspace-lock-check) | | [Test Issues](https://github.com/runwhen-contrib/rw-
 cli-codecollection/blob/main/codebundles/test-issue/runbook.robot) | `Test` |
 `Raise Full Issue` | A codebundle for testing the issues feature. Purely for
 testing flow. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/test-
 issue) | | [cURL HTTP OK](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/curl-http-ok/runbook.robot) | `Linux macOS
+codecollection/blob/main/codebundles/curl-http-ok/sli.robot) | `Linux macOS
 Windows HTTP` | `Checking HTTP URL Is Available And Timely` | This taskset uses
-curl to validate the response code of the endpoint and provides the total time
-of the request. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/
-curl-http-ok) | | [cli-test-taskset](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/cli-test/runbook.robot) | `cli` | `Run CLI
-and Parse Output For Issues`, `Exec Test`, `Local Process Test` | This taskset
-smoketests the CLI codebundle setup and run process [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/cli-test) | | [cmd-test-taskset]
-(https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
+curl to validate the response code of the endpoint. Returns ascore of 1 if
+healthy, an 0 if unhealthy. [Docs](https://docs.runwhen.com/public/v/cli-
+codecollection/curl-http-ok) | | [cli-test-taskset](https://github.com/runwhen-
+contrib/rw-cli-codecollection/blob/main/codebundles/cli-test/runbook.robot) |
+`cli` | `Run CLI and Parse Output For Issues`, `Exec Test`, `Local Process
+Test` | This taskset smoketests the CLI codebundle setup and run process [Docs]
+(https://docs.runwhen.com/public/v/cli-codecollection/cli-test) | | [cmd-test-
+taskset](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
 codebundles/cmd-test/runbook.robot) | `cmd` | `Run CLI Command`, `Run Bash
 File`, `Log Suggestion` | This taskset smoketests the CLI codebundle setup and
 run process by running a bare command [Docs](https://docs.runwhen.com/public/v/
 cli-codecollection/cmd-test) |
```

### Comparing `runwhen-cli-keywords-0.0.8/README.md` & `runwhen-cli-keywords-0.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Troubleshooting Tasks in Codecollection: **123**
-Codebundles in Codecollection: **44**
+Troubleshooting Tasks in Codecollection: **128**
+Codebundles in Codecollection: **45**
 
 ![](docs/GitHub_Banner.jpg)
 
 <p align="center">
   <a href="https://discord.gg/Ut7Ws4rm8Q">
     <img src="https://img.shields.io/discord/1131539039665791077?label=Join%20Discord&logo=discord&logoColor=white&style=for-the-badge" alt="Join Discord">
   </a>
@@ -50,43 +50,44 @@
 |---|---|---|---|
 | [AWS CloudWatch Overutlized EC2 Inspection](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/aws-cloudwatch-overused-ec2/runbook.robot) | `AWS`, `CloudWatch` | `Check For Overutilized Ec2 Instances` | Queries AWS CloudWatch for a list of EC2 instances with a high amount of resource utilization, raising issues when overutilized instances are found. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/aws-cloudwatch-overused-ec2) |
 | [AWS EKS Nodegroup Status Check](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/aws-eks-node-reboot/runbook.robot) | `AWS`, `EKS` | `Check EKS Nodegroup Status` | Queries a node group within a EKS cluster to check if the nodegroup has degraded service, indicating ongoing reboots or other issues. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/aws-eks-node-reboot) |
 | [Azure Internal LoadBalancer Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/azure-loadbalancer-triage/runbook.robot) | `Kubernetes`, `AKS`, `Azure` | `Health Check Internal Azure Load Balancer` | Triages issues related to a Azure Loadbalancers and its activity logs. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/azure-loadbalancer-triage) |
 | [Azure Monitor Activity Log SLI](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/azure-monitor-event-triage/sli.robot) | `Kubernetes`, `AKS`, `Azure` | `Run Azure Monitor Activity Log Triage` | Measures the count of error activity log entries as a SLI metric for the Azure tenancy. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/azure-monitor-event-triage) |
 | [Azure Monitor Event Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/azure-monitor-event-triage/runbook.robot) | `Kubernetes`, `AKS`, `Azure` | `Run Azure Monitor Activity Log Triage` | Triages issues related to a Azure Loadbalancers, Kubernetes ingress objects and services. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/azure-monitor-event-triage) |
 | [GCP Gcloud Log Inspection](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/gcloud-log-inspection/runbook.robot) | `GCP`, `Gcloud`, `Google Monitoring` | `Inspect GCP Logs For Common Errors` | Fetches logs from a GCP using a configurable query and raises an issue with details on the most common issues. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/gcloud-log-inspection) |
-| [GCP Node Prempt List](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/gcloud-node-preempt/runbook.robot) | `GCP`, `GKE` | `List all nodes in an active prempt operation` | List all GCP nodes that have an active preempt operation. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/gcloud-node-preempt) |
+| [GCP Node Prempt List](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/gcloud-node-preempt/sli.robot) | `GCP`, `GKE` | `Count the number of nodes in active prempt operation` | Check if any GCP nodes have an active preempt operation. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/gcloud-node-preempt) |
 | [GKE Kong Ingress Host Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/curl-gmp-kong-ingress-inspection/runbook.robot) | `GCP`, `GMP`, `Ingress`, `Kong`, `Metrics` | `Check If Kong Ingress HTTP Error Rate Violates HTTP Error Threshold`, `Check If Kong Ingress HTTP Request Latency Violates Threshold`, `Check If Kong Ingress Controller Reports Upstream Errors` | Collects Kong ingress host metrics from GMP on GCP and inspects the results for ingress with a HTTP error code rate greater than zero over a configurable duration and raises issues based on the number of ingress with error codes. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/curl-gmp-kong-ingress-inspection) |
-| [GKE Nginx Ingress Host Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/curl-gmp-nginx-ingress-inspection/runbook.robot) | `GCP`, `GMP`, `Ingress`, `Nginx`, `Metrics` | `Fetch Nginx Ingress HTTP Errors From GMP And Perform Inspection On Results`, `Find Ingress Owner and Service Health` | Collects Nginx ingress host controller metrics from GMP on GCP and inspects the results for ingress with a HTTP error code rate greater than zero over a configurable duration and raises issues based on the number of ingress with error codes. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/curl-gmp-nginx-ingress-inspection) |
+| [GKE Nginx Ingress Host Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/curl-gmp-nginx-ingress-inspection/runbook.robot) | `GCP`, `GMP`, `Ingress`, `Nginx`, `Metrics` | `Fetch Nginx HTTP Errors From GMP for Ingress `${INGRESS_OBJECT_NAME}``, `Find Owner and Service Health for Ingress `${INGRESS_OBJECT_NAME}`` | Collects Nginx ingress host controller metrics from GMP on GCP and inspects the results for ingress with a HTTP error code rate greater than zero over a configurable duration and raises issues based on the number of ingress with error codes. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/curl-gmp-nginx-ingress-inspection) |
 | [Kubeprometheus Operator Troubleshoot](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-prometheus-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Prometheus` | `Check Prometheus Service Monitors`, `Check For Successful Rule Setup`, `Verify Prometheus RBAC Can Access ServiceMonitors`, `Identify Endpoint Scraping Errors`, `Check Prometheus API Healthy` | This taskset investigates the logs, state and health of Kubernetes Prometheus operator. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-prometheus-healthcheck) |
-| [Kubernetes Application Troubleshoot](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-app-troubleshoot/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Resource Logs`, `Scan For Misconfigured Environment` | Triages issues related to a deployment and its replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-app-troubleshoot) |
+| [Kubernetes Application Monitor](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-app-troubleshoot/sli.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Measure Application Exceptions` | Measures the number of exception stacktraces present in an application's logs over a time period. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-app-troubleshoot) |
+| [Kubernetes Application Troubleshoot](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-app-troubleshoot/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Workload Logs`, `Scan For Misconfigured Environment`, `Troubleshoot Application Logs` | Triages issues related to a deployment and its replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-app-troubleshoot) |
 | [Kubernetes ArgoCD Application Health & Troubleshoot](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-argocd-application-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `ArgoCD` | `Fetch ArgoCD Application Sync Status & Health`, `Fetch ArgoCD Application Last Sync Operation Details`, `Fetch Unhealthy ArgoCD Application Resources`, `Scan For Errors in Pod Logs Related to ArgoCD Application Deployments`, `Fully Describe ArgoCD Application` | This taskset collects information and runs general troubleshooting checks against argocd application objects within a namespace. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-argocd-application-health) |
 | [Kubernetes ArgoCD HelmRelease TaskSet](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-argocd-helm-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `ArgoCD` | `Fetch all available ArgoCD Helm releases`, `Fetch Installed ArgoCD Helm release versions` | This codebundle runs a series of tasks to identify potential helm release issues related to ArgoCD managed Helm objects. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-argocd-helm-health) |
 | [Kubernetes Artifactory Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-artifactory-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Artifactory` | `Check Artifactory Liveness and Readiness Endpoints` | Performs a triage on the Open Source version of Artifactory in a Kubernetes cluster. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-artifactory-health) |
-| [Kubernetes CertManager Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-certmanager-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `CertManager` | `Get Namespace Certificate Summary`, `Find Failed Certificate Requests and Identify Issues` | This taskset checks that your cert manager certificates are renewing as expected, raising issues when they are past due in the configured namespace [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-certmanager-healthcheck) |
+| [Kubernetes CertManager Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-certmanager-healthcheck/sli.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Health Score of CertManager Workloads` | Check the health of pods deployed by cert-manager. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-certmanager-healthcheck) |
 | [Kubernetes Daemonset Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-daemonset-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get DaemonSet Log Details For Report`, `Get Related Daemonset Events`, `Check Daemonset Replicas` | Triages issues related to a Daemonset and its available replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-daemonset-healthcheck) |
-| [Kubernetes Deployment Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-deployment-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Check Deployment Log For Issues`, `Troubleshoot Deployment Warning Events`, `Get Deployment Workload Details For Report`, `Troubleshoot Deployment Replicas`, `Check For Deployment Event Anomalies` | Triages issues related to a deployment and its replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-deployment-healthcheck) |
+| [Kubernetes Deployment Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-deployment-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Check Deployment Log For Issues with `${DEPLOYMENT_NAME}``, `Check Liveness Probe Configuration for Deployment `${DEPLOYMENT_NAME}``, `Check Readiness Probe Configuration for Deployment `${DEPLOYMENT_NAME}``, `Troubleshoot Deployment Warning Events for `${DEPLOYMENT_NAME}``, `Get Deployment Workload Details For `${DEPLOYMENT_NAME}` and Add to Report`, `Troubleshoot Deployment Replicas for `${DEPLOYMENT_NAME}``, `Check Deployment Event Anomalies for `${DEPLOYMENT_NAME}`` | Triages issues related to a deployment and its replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-deployment-healthcheck) |
 | [Kubernetes Flux Choas Testing](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-chaos-flux/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Suspend the Flux Resource Reconciliation`, `Find Random FluxCD Workload as Chaos Target`, `Execute Chaos Command`, `Execute Additional Chaos Command`, `Resume Flux Resource Reconciliation` | This taskset is used to suspend a flux resource for the purposes of executing chaos tasks. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-chaos-flux) |
 | [Kubernetes FluxCD HelmRelease TaskSet](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-fluxcd-helm-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `FluxCD` | `List all available FluxCD Helmreleases`, `Fetch Installed FluxCD Helmrelease Versions`, `Fetch Mismatched FluxCD HelmRelease Version`, `Fetch FluxCD HelmRelease Error Messages`, `Check for Available Helm Chart Updates` | This codebundle runs a series of tasks to identify potential helm release issues related to Flux managed Helm objects. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-fluxcd-helm-health) |
 | [Kubernetes FluxCD Kustomization TaskSet](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-fluxcd-kustomization-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `FluxCD` | `List all available Kustomization objects`, `Get details for unready Kustomizations` | This codebundle runs a series of tasks to identify potential Kustomization issues related to Flux managed Kustomization objects. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-fluxcd-kustomization-health) |
 | [Kubernetes Grafana Loki Health Check](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-loki-healthcheck/runbook.robot) | `k8s` | `Check Loki Ring API`, `Check Loki API Ready` | This taskset checks the health of Grafana Loki and its hash ring. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-loki-healthcheck) |
-| [Kubernetes Image Check](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-image-check/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Check Image Rollover Times In Namespace`, `List Images and Tags for Every Container in Running Pods`, `List Images and Tags for Every Container in Failed Pods`, `List ImagePullBackOff Events and Test Path and Tags` | This taskset provides detailed information about the images used in a Kubernetes namespace. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-image-check) |
+| [Kubernetes Image Check](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-image-check/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Check Image Rollover Times for Namespace `${NAMESPACE}``, `List Images and Tags for Every Container in Running Pods for Namespace `${NAMESPACE}``, `List Images and Tags for Every Container in Failed Pods for Namespace `${NAMESPACE}``, `List ImagePullBackOff Events and Test Path and Tags for Namespace `${NAMESPACE}`` | This taskset provides detailed information about the images used in a Kubernetes namespace. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-image-check) |
 | [Kubernetes Ingress GCE & GCP HTTP Load Balancer Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-ingress-gce-healthcheck/runbook.robot) | `Kubernetes`, `GKE`, `GCE`, `GCP` | `Search For GCE Ingress Warnings in GKE`, `Identify Unhealthy GCE HTTP Ingress Backends`, `Validate GCP HTTP Load Balancer Configurations`, `Fetch Network Error Logs from GCP Operations Manager for Ingress Backends`, `Review GCP Operations Logging Dashboard` | Troubleshoot GCE Ingress Resources related to GCP HTTP Load Balancer in GKE [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-ingress-gce-healthcheck) |
-| [Kubernetes Ingress Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-ingress-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Fetch Ingress Object Health in Namespace` | Triages issues related to a ingress objects and services. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-ingress-healthcheck) |
+| [Kubernetes Ingress Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-ingress-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Fetch Ingress Object Health in Namespace `${NAMESPACE}``, `Check for Ingress and Service Conflicts in Namespace `${NAMESPACE}`` | Triages issues related to a ingress objects and services. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-ingress-healthcheck) |
 | [Kubernetes Jenkins Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-jenkins-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Jenkins` | `Query The Jenkins Kubernetes Workload HTTP Endpoint`, `Query For Stuck Jenkins Jobs` | This taskset collects information about perstistent volumes and persistent volume claims to validate health or help troubleshoot potential issues. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-jenkins-healthcheck) |
 | [Kubernetes Labeled Pod Count](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-labeledpods-healthcheck/sli.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Measure Number of Running Pods with Label` | This codebundle fetches the number of running pods with the set of provided labels, letting you measure the number of running pods. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-labeledpods-healthcheck) |
 | [Kubernetes Namespace Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-namespace-healthcheck/sli.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Event Count and Score`, `Get Container Restarts and Score`, `Get NotReady Pods`, `Generate Namspace Score` | This SLI uses kubectl to score namespace health. Produces a value between 0 (completely failing thet test) and 1 (fully passing the test). Looks for container restarts, events, and pods not ready. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-namespace-healthcheck) |
-| [Kubernetes Namespace Troubleshoot](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-namespace-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Trace And Troubleshoot Namespace Warning Events And Errors`, `Troubleshoot Container Restarts In Namespace`, `Troubleshoot Pending Pods In Namespace`, `Troubleshoot Failed Pods In Namespace`, `Troubleshoot Workload Status Conditions In Namespace`, `Get Listing Of Resources In Namespace`, `Check For Namespace Event Anomalies`, `Troubleshoot Namespace Services And Application Workloads`, `Check Missing or Risky PodDisruptionBudget Policies` | This taskset runs general troubleshooting checks against all applicable objects in a namespace, checks error events, and searches pod logs for error entries. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-namespace-healthcheck) |
-| [Kubernetes Persistent Volume Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-pvc-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Fetch Events for Unhealthy Kubernetes PersistentVolumeClaims`, `List PersistentVolumeClaims in Terminating State`, `List PersistentVolumes in Terminating State`, `List Pods with Attached Volumes and Related PersistentVolume Details`, `Fetch the Storage Utilization for PVC Mounts`, `Check for RWO Persistent Volume Node Attachment Issues` | This taskset collects information about storage such as PersistentVolumes and PersistentVolumeClaims to validate health or help troubleshoot potential storage issues. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-pvc-healthcheck) |
-| [Kubernetes Pod Resources Scan](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-podresources-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Scan Labeled Pods and Show All Containers Without Resource Limit or Resource Requests Set`, `Get Labeled Container Top Info` | Inspects the resources provisioned for a given set of pods, selected by their labels and raises issues if no resources were specified. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-podresources-health) |
+| [Kubernetes Namespace Troubleshoot](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-namespace-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Troubleshoot Warning Events in Namespace `${NAMESPACE}``, `Troubleshoot Container Restarts In Namespace `${NAMESPACE}``, `Troubleshoot Pending Pods In Namespace `${NAMESPACE}``, `Troubleshoot Failed Pods In Namespace `${NAMESPACE}``, `Troubleshoot Workload Status Conditions In Namespace `${NAMESPACE}``, `Get Listing Of Resources In Namespace `${NAMESPACE}``, `Check Event Anomalies in Namespace `${NAMESPACE}``, `Troubleshoot Services And Application Workloads in Namespace `${NAMESPACE}``, `Check Missing or Risky PodDisruptionBudget Policies in Namepace `${NAMESPACE}`` | This taskset runs general troubleshooting checks against all applicable objects in a namespace. Looks for warning events, odd or frequent normal events, restarting containers and failed or pending pods. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-namespace-healthcheck) |
+| [Kubernetes Persistent Volume Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-pvc-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Fetch Events for Unhealthy Kubernetes PersistentVolumeClaims in Namespace `${NAMESPACE}``, `List PersistentVolumeClaims in Terminating State in Namespace `${NAMESPACE}``, `List PersistentVolumes in Terminating State in Namespace `${NAMESPACE}``, `List Pods with Attached Volumes and Related PersistentVolume Details in Namespace `${NAMESPACE}``, `Fetch the Storage Utilization for PVC Mounts in Namespace `${NAMESPACE}``, `Check for RWO Persistent Volume Node Attachment Issues in Namespace `${NAMESPACE}`` | This taskset collects information about storage such as PersistentVolumes and PersistentVolumeClaims to validate health or help troubleshoot potential storage issues. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-pvc-healthcheck) |
+| [Kubernetes Pod Resources Scan](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-podresources-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Show Pods Without Resource Limit or Resource Requests Set in Namespace `${NAMESPACE}``, `Get Pod Resource Utilization with Top in Namespace `${NAMESPACE}`` | Inspects the resources provisioned for a given set of pods, selected by their labels and raises issues if no resources were specified. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-podresources-health) |
 | [Kubernetes Postgres Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-postgres-triage/runbook.robot) | `AKS`, `EKS`, `GKE`, `Kubernetes`, `Patroni`, `Postgres` | `Get Standard Postgres Resource Information`, `Describe Postgres Custom Resources`, `Get Postgres Pod Logs & Events`, `Get Postgres Pod Resource Utilization`, `Get Running Postgres Configuration`, `Get Patroni Output`, `Run DB Queries` | Runs multiple Kubernetes and psql commands to report on the health of a postgres cluster. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-postgres-triage) |
-| [Kubernetes Redis Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-redis-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Redis` | `Ping Redis Workload`, `Verify Redis Read Write Operation` | This taskset collects information on your redis workload in your Kubernetes cluster and raises issues if any health checks fail. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-redis-healthcheck) |
+| [Kubernetes Redis Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-redis-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Redis` | `Ping `${DEPLOYMENT_NAME}` Redis Workload`, `Verify `${DEPLOYMENT_NAME}` Redis Read Write Operation` | This taskset collects information on your redis workload in your Kubernetes cluster and raises issues if any health checks fail. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-redis-healthcheck) |
 | [Kubernetes Restart resource](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-restart-resource/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Current Resource State`, `Get Resource Logs`, `Restart Resource` | This taskset restarts a resource with a given set of labels, typically used with other tasksets. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-restart-resource) |
 | [Kubernetes Service Account Check](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-serviceaccount-check/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Redis` | `Test Service Account Access to Kubernetes API Server` | This taskset provides tasks to troubleshoot service accounts in a Kubernetes namespace. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-serviceaccount-check) |
-| [Kubernetes StatefulSet Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-statefulset-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Fetch StatefulSet Logs`, `Get Related StatefulSet Events`, `Fetch StatefulSet Manifest Details`, `List StatefulSets with Unhealthy Replica Counts` | Triages issues related to a StatefulSet and its replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-statefulset-healthcheck) |
+| [Kubernetes StatefulSet Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-statefulset-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Fetch StatefulSet `${STATEFULSET_NAME}` Logs`, `Get Related StatefulSet `${STATEFULSET_NAME}` Events`, `Fetch StatefulSet `${STATEFULSET_NAME}` Manifest Details`, `List StatefulSets with Unhealthy Replica Counts In Namespace `${NAMESPACE}`` | Triages issues related to a StatefulSet and its replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-statefulset-healthcheck) |
 | [Kubernetes Vault Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-vault-healthcheck/runbook.robot) | `AKS`, `EKS`, `GKE`, `Kubernetes`, `Vault` | `Fetch Vault CSI Driver Logs`, `Get Vault CSI Driver Warning Events`, `Check Vault CSI Driver Replicas`, `Fetch Vault Logs`, `Get Related Vault Events`, `Fetch Vault StatefulSet Manifest Details`, `Fetch Vault DaemonSet Manifest Details`, `Verify Vault Availability`, `Check Vault StatefulSet Replicas` | A suite of tasks that can be used to triage potential issues in your vault namespace. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-vault-healthcheck) |
 | [Terraform Cloud Workspace Lock Check](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/terraform-cloud-workspace-lock-check/runbook.robot) | `Terraform Cloud` | `Checking whether the Terraform Cloud Workspace is in a locked state` | Check whether the Terraform Cloud Workspace is in a locked state. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/terraform-cloud-workspace-lock-check) |
 | [Test Issues](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/test-issue/runbook.robot) | `Test` | `Raise Full Issue` | A codebundle for testing the issues feature. Purely for testing flow. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/test-issue) |
-| [cURL HTTP OK](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/curl-http-ok/runbook.robot) | `Linux macOS Windows HTTP` | `Checking HTTP URL Is Available And Timely` | This taskset uses curl to validate the response code of the endpoint and provides the total time of the request. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/curl-http-ok) |
+| [cURL HTTP OK](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/curl-http-ok/sli.robot) | `Linux macOS Windows HTTP` | `Checking HTTP URL Is Available And Timely` | This taskset uses curl to validate the response code of the endpoint. Returns ascore of 1 if healthy, an 0 if unhealthy. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/curl-http-ok) |
 | [cli-test-taskset](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/cli-test/runbook.robot) | `cli` | `Run CLI and Parse Output For Issues`, `Exec Test`, `Local Process Test` | This taskset smoketests the CLI codebundle setup and run process [Docs](https://docs.runwhen.com/public/v/cli-codecollection/cli-test) |
 | [cmd-test-taskset](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/cmd-test/runbook.robot) | `cmd` | `Run CLI Command`, `Run Bash File`, `Log Suggestion` | This taskset smoketests the CLI codebundle setup and run process by running a bare command [Docs](https://docs.runwhen.com/public/v/cli-codecollection/cmd-test) |
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Troubleshooting Tasks in Codecollection: **123** Codebundles in Codecollection:
-**44** ![](docs/GitHub_Banner.jpg)
+Troubleshooting Tasks in Codecollection: **128** Codebundles in Codecollection:
+**45** ![](docs/GitHub_Banner.jpg)
                                 _[_J_o_i_n_ _D_i_s_c_o_r_d_]
                                  _[_J_o_i_n_ _S_l_a_c_k_]
 _[_O_p_e_n_ _i_n_ _G_i_t_H_u_b_ _C_o_d_e_s_p_a_c_e_s_]# RunWhen Public Codecollection This repository is a
 codecollection that is to be used within the RunWhen platform. It contains
 codebundles that can be used in SLIs, and TaskSets. Please see the **
 [contributing](CONTRIBUTING.md)** and **[code of conduct](CODE_OF_CONDUCT.md)**
 for details on adding your contributions to this project. Documentation for
@@ -56,91 +56,99 @@
 public/v/cli-codecollection/azure-monitor-event-triage) | | [GCP Gcloud Log
 Inspection](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
 codebundles/gcloud-log-inspection/runbook.robot) | `GCP`, `Gcloud`, `Google
 Monitoring` | `Inspect GCP Logs For Common Errors` | Fetches logs from a GCP
 using a configurable query and raises an issue with details on the most common
 issues. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/gcloud-log-
 inspection) | | [GCP Node Prempt List](https://github.com/runwhen-contrib/rw-
-cli-codecollection/blob/main/codebundles/gcloud-node-preempt/runbook.robot) |
-`GCP`, `GKE` | `List all nodes in an active prempt operation` | List all GCP
-nodes that have an active preempt operation. [Docs](https://docs.runwhen.com/
-public/v/cli-codecollection/gcloud-node-preempt) | | [GKE Kong Ingress Host
-Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
-codebundles/curl-gmp-kong-ingress-inspection/runbook.robot) | `GCP`, `GMP`,
-`Ingress`, `Kong`, `Metrics` | `Check If Kong Ingress HTTP Error Rate Violates
-HTTP Error Threshold`, `Check If Kong Ingress HTTP Request Latency Violates
-Threshold`, `Check If Kong Ingress Controller Reports Upstream Errors` |
-Collects Kong ingress host metrics from GMP on GCP and inspects the results for
-ingress with a HTTP error code rate greater than zero over a configurable
+cli-codecollection/blob/main/codebundles/gcloud-node-preempt/sli.robot) |
+`GCP`, `GKE` | `Count the number of nodes in active prempt operation` | Check
+if any GCP nodes have an active preempt operation. [Docs](https://
+docs.runwhen.com/public/v/cli-codecollection/gcloud-node-preempt) | | [GKE Kong
+Ingress Host Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/
+blob/main/codebundles/curl-gmp-kong-ingress-inspection/runbook.robot) | `GCP`,
+`GMP`, `Ingress`, `Kong`, `Metrics` | `Check If Kong Ingress HTTP Error Rate
+Violates HTTP Error Threshold`, `Check If Kong Ingress HTTP Request Latency
+Violates Threshold`, `Check If Kong Ingress Controller Reports Upstream Errors`
+| Collects Kong ingress host metrics from GMP on GCP and inspects the results
+for ingress with a HTTP error code rate greater than zero over a configurable
 duration and raises issues based on the number of ingress with error codes.
 [Docs](https://docs.runwhen.com/public/v/cli-codecollection/curl-gmp-kong-
 ingress-inspection) | | [GKE Nginx Ingress Host Triage](https://github.com/
 runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/curl-gmp-nginx-
 ingress-inspection/runbook.robot) | `GCP`, `GMP`, `Ingress`, `Nginx`, `Metrics`
-| `Fetch Nginx Ingress HTTP Errors From GMP And Perform Inspection On Results`,
-`Find Ingress Owner and Service Health` | Collects Nginx ingress host
-controller metrics from GMP on GCP and inspects the results for ingress with a
-HTTP error code rate greater than zero over a configurable duration and raises
-issues based on the number of ingress with error codes. [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/curl-gmp-nginx-ingress-inspection)
-| | [Kubeprometheus Operator Troubleshoot](https://github.com/runwhen-contrib/
-rw-cli-codecollection/blob/main/codebundles/k8s-prometheus-healthcheck/
-runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Prometheus` |
-`Check Prometheus Service Monitors`, `Check For Successful Rule Setup`, `Verify
-Prometheus RBAC Can Access ServiceMonitors`, `Identify Endpoint Scraping
-Errors`, `Check Prometheus API Healthy` | This taskset investigates the logs,
-state and health of Kubernetes Prometheus operator. [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/k8s-prometheus-healthcheck) | |
+| `Fetch Nginx HTTP Errors From GMP for Ingress `${INGRESS_OBJECT_NAME}``,
+`Find Owner and Service Health for Ingress `${INGRESS_OBJECT_NAME}`` | Collects
+Nginx ingress host controller metrics from GMP on GCP and inspects the results
+for ingress with a HTTP error code rate greater than zero over a configurable
+duration and raises issues based on the number of ingress with error codes.
+[Docs](https://docs.runwhen.com/public/v/cli-codecollection/curl-gmp-nginx-
+ingress-inspection) | | [Kubeprometheus Operator Troubleshoot](https://
+github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-
+prometheus-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`,
+`OpenShift`, `Prometheus` | `Check Prometheus Service Monitors`, `Check For
+Successful Rule Setup`, `Verify Prometheus RBAC Can Access ServiceMonitors`,
+`Identify Endpoint Scraping Errors`, `Check Prometheus API Healthy` | This
+taskset investigates the logs, state and health of Kubernetes Prometheus
+operator. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-
+prometheus-healthcheck) | | [Kubernetes Application Monitor](https://
+github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-app-
+troubleshoot/sli.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` |
+`Measure Application Exceptions` | Measures the number of exception stacktraces
+present in an application's logs over a time period. [Docs](https://
+docs.runwhen.com/public/v/cli-codecollection/k8s-app-troubleshoot) | |
 [Kubernetes Application Troubleshoot](https://github.com/runwhen-contrib/rw-
 cli-codecollection/blob/main/codebundles/k8s-app-troubleshoot/runbook.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Resource Logs`, `Scan For
-Misconfigured Environment` | Triages issues related to a deployment and its
-replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-app-
-troubleshoot) | | [Kubernetes ArgoCD Application Health & Troubleshoot](https:/
-/github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-
-argocd-application-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`,
-`OpenShift`, `ArgoCD` | `Fetch ArgoCD Application Sync Status & Health`, `Fetch
-ArgoCD Application Last Sync Operation Details`, `Fetch Unhealthy ArgoCD
-Application Resources`, `Scan For Errors in Pod Logs Related to ArgoCD
-Application Deployments`, `Fully Describe ArgoCD Application` | This taskset
-collects information and runs general troubleshooting checks against argocd
-application objects within a namespace. [Docs](https://docs.runwhen.com/public/
-v/cli-codecollection/k8s-argocd-application-health) | | [Kubernetes ArgoCD
-HelmRelease TaskSet](https://github.com/runwhen-contrib/rw-cli-codecollection/
-blob/main/codebundles/k8s-argocd-helm-health/runbook.robot) | `Kubernetes`,
-`AKS`, `EKS`, `GKE`, `OpenShift`, `ArgoCD` | `Fetch all available ArgoCD Helm
-releases`, `Fetch Installed ArgoCD Helm release versions` | This codebundle
-runs a series of tasks to identify potential helm release issues related to
-ArgoCD managed Helm objects. [Docs](https://docs.runwhen.com/public/v/cli-
-codecollection/k8s-argocd-helm-health) | | [Kubernetes Artifactory Triage]
-(https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
-codebundles/k8s-artifactory-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`,
-`GKE`, `OpenShift`, `Artifactory` | `Check Artifactory Liveness and Readiness
-Endpoints` | Performs a triage on the Open Source version of Artifactory in a
-Kubernetes cluster. [Docs](https://docs.runwhen.com/public/v/cli-
-codecollection/k8s-artifactory-health) | | [Kubernetes CertManager Healthcheck]
-(https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
-codebundles/k8s-certmanager-healthcheck/runbook.robot) | `Kubernetes`, `AKS`,
-`EKS`, `GKE`, `OpenShift`, `CertManager` | `Get Namespace Certificate Summary`,
-`Find Failed Certificate Requests and Identify Issues` | This taskset checks
-that your cert manager certificates are renewing as expected, raising issues
-when they are past due in the configured namespace [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/k8s-certmanager-healthcheck) | |
-[Kubernetes Daemonset Triage](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/k8s-daemonset-healthcheck/runbook.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get DaemonSet Log Details For
-Report`, `Get Related Daemonset Events`, `Check Daemonset Replicas` | Triages
-issues related to a Daemonset and its available replicas. [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/k8s-daemonset-healthcheck) | |
-[Kubernetes Deployment Triage](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/k8s-deployment-healthcheck/runbook.robot)
-| `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Check Deployment Log For
-Issues`, `Troubleshoot Deployment Warning Events`, `Get Deployment Workload
-Details For Report`, `Troubleshoot Deployment Replicas`, `Check For Deployment
-Event Anomalies` | Triages issues related to a deployment and its replicas.
+`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Workload Logs`, `Scan For
+Misconfigured Environment`, `Troubleshoot Application Logs` | Triages issues
+related to a deployment and its replicas. [Docs](https://docs.runwhen.com/
+public/v/cli-codecollection/k8s-app-troubleshoot) | | [Kubernetes ArgoCD
+Application Health & Troubleshoot](https://github.com/runwhen-contrib/rw-cli-
+codecollection/blob/main/codebundles/k8s-argocd-application-health/
+runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `ArgoCD` |
+`Fetch ArgoCD Application Sync Status & Health`, `Fetch ArgoCD Application Last
+Sync Operation Details`, `Fetch Unhealthy ArgoCD Application Resources`, `Scan
+For Errors in Pod Logs Related to ArgoCD Application Deployments`, `Fully
+Describe ArgoCD Application` | This taskset collects information and runs
+general troubleshooting checks against argocd application objects within a
+namespace. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-
+argocd-application-health) | | [Kubernetes ArgoCD HelmRelease TaskSet](https://
+github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-
+argocd-helm-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`,
+`OpenShift`, `ArgoCD` | `Fetch all available ArgoCD Helm releases`, `Fetch
+Installed ArgoCD Helm release versions` | This codebundle runs a series of
+tasks to identify potential helm release issues related to ArgoCD managed Helm
+objects. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-
+argocd-helm-health) | | [Kubernetes Artifactory Triage](https://github.com/
+runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-artifactory-
+health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`,
+`Artifactory` | `Check Artifactory Liveness and Readiness Endpoints` | Performs
+a triage on the Open Source version of Artifactory in a Kubernetes cluster.
+[Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-artifactory-
+health) | | [Kubernetes CertManager Healthcheck](https://github.com/runwhen-
+contrib/rw-cli-codecollection/blob/main/codebundles/k8s-certmanager-
+healthcheck/sli.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get
+Health Score of CertManager Workloads` | Check the health of pods deployed by
+cert-manager. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-
+certmanager-healthcheck) | | [Kubernetes Daemonset Triage](https://github.com/
+runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-daemonset-
+healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` |
+`Get DaemonSet Log Details For Report`, `Get Related Daemonset Events`, `Check
+Daemonset Replicas` | Triages issues related to a Daemonset and its available
+replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-
+daemonset-healthcheck) | | [Kubernetes Deployment Triage](https://github.com/
+runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-deployment-
+healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` |
+`Check Deployment Log For Issues with `${DEPLOYMENT_NAME}``, `Check Liveness
+Probe Configuration for Deployment `${DEPLOYMENT_NAME}``, `Check Readiness
+Probe Configuration for Deployment `${DEPLOYMENT_NAME}``, `Troubleshoot
+Deployment Warning Events for `${DEPLOYMENT_NAME}``, `Get Deployment Workload
+Details For `${DEPLOYMENT_NAME}` and Add to Report`, `Troubleshoot Deployment
+Replicas for `${DEPLOYMENT_NAME}``, `Check Deployment Event Anomalies for `$
+{DEPLOYMENT_NAME}`` | Triages issues related to a deployment and its replicas.
 [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-deployment-
 healthcheck) | | [Kubernetes Flux Choas Testing](https://github.com/runwhen-
 contrib/rw-cli-codecollection/blob/main/codebundles/k8s-chaos-flux/
 runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Suspend the
 Flux Resource Reconciliation`, `Find Random FluxCD Workload as Chaos Target`,
 `Execute Chaos Command`, `Execute Additional Chaos Command`, `Resume Flux
 Resource Reconciliation` | This taskset is used to suspend a flux resource for
@@ -164,116 +172,126 @@
 health) | | [Kubernetes Grafana Loki Health Check](https://github.com/runwhen-
 contrib/rw-cli-codecollection/blob/main/codebundles/k8s-loki-healthcheck/
 runbook.robot) | `k8s` | `Check Loki Ring API`, `Check Loki API Ready` | This
 taskset checks the health of Grafana Loki and its hash ring. [Docs](https://
 docs.runwhen.com/public/v/cli-codecollection/k8s-loki-healthcheck) | |
 [Kubernetes Image Check](https://github.com/runwhen-contrib/rw-cli-
 codecollection/blob/main/codebundles/k8s-image-check/runbook.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Check Image Rollover Times In
-Namespace`, `List Images and Tags for Every Container in Running Pods`, `List
-Images and Tags for Every Container in Failed Pods`, `List ImagePullBackOff
-Events and Test Path and Tags` | This taskset provides detailed information
-about the images used in a Kubernetes namespace. [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/k8s-image-check) | | [Kubernetes
-Ingress GCE & GCP HTTP Load Balancer Healthcheck](https://github.com/runwhen-
-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-ingress-gce-
-healthcheck/runbook.robot) | `Kubernetes`, `GKE`, `GCE`, `GCP` | `Search For
-GCE Ingress Warnings in GKE`, `Identify Unhealthy GCE HTTP Ingress Backends`,
-`Validate GCP HTTP Load Balancer Configurations`, `Fetch Network Error Logs
-from GCP Operations Manager for Ingress Backends`, `Review GCP Operations
-Logging Dashboard` | Troubleshoot GCE Ingress Resources related to GCP HTTP
-Load Balancer in GKE [Docs](https://docs.runwhen.com/public/v/cli-
+`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Check Image Rollover Times
+for Namespace `${NAMESPACE}``, `List Images and Tags for Every Container in
+Running Pods for Namespace `${NAMESPACE}``, `List Images and Tags for Every
+Container in Failed Pods for Namespace `${NAMESPACE}``, `List ImagePullBackOff
+Events and Test Path and Tags for Namespace `${NAMESPACE}`` | This taskset
+provides detailed information about the images used in a Kubernetes namespace.
+[Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-image-check) |
+| [Kubernetes Ingress GCE & GCP HTTP Load Balancer Healthcheck](https://
+github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-
+ingress-gce-healthcheck/runbook.robot) | `Kubernetes`, `GKE`, `GCE`, `GCP` |
+`Search For GCE Ingress Warnings in GKE`, `Identify Unhealthy GCE HTTP Ingress
+Backends`, `Validate GCP HTTP Load Balancer Configurations`, `Fetch Network
+Error Logs from GCP Operations Manager for Ingress Backends`, `Review GCP
+Operations Logging Dashboard` | Troubleshoot GCE Ingress Resources related to
+GCP HTTP Load Balancer in GKE [Docs](https://docs.runwhen.com/public/v/cli-
 codecollection/k8s-ingress-gce-healthcheck) | | [Kubernetes Ingress
 Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/
 main/codebundles/k8s-ingress-healthcheck/runbook.robot) | `Kubernetes`, `AKS`,
-`EKS`, `GKE`, `OpenShift` | `Fetch Ingress Object Health in Namespace` |
-Triages issues related to a ingress objects and services. [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/k8s-ingress-healthcheck) | |
-[Kubernetes Jenkins Healthcheck](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/k8s-jenkins-healthcheck/runbook.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Jenkins` | `Query The Jenkins
-Kubernetes Workload HTTP Endpoint`, `Query For Stuck Jenkins Jobs` | This
-taskset collects information about perstistent volumes and persistent volume
-claims to validate health or help troubleshoot potential issues. [Docs](https:/
-/docs.runwhen.com/public/v/cli-codecollection/k8s-jenkins-healthcheck) | |
-[Kubernetes Labeled Pod Count](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/k8s-labeledpods-healthcheck/sli.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Measure Number of Running
-Pods with Label` | This codebundle fetches the number of running pods with the
-set of provided labels, letting you measure the number of running pods. [Docs]
-(https://docs.runwhen.com/public/v/cli-codecollection/k8s-labeledpods-
-healthcheck) | | [Kubernetes Namespace Healthcheck](https://github.com/runwhen-
-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-namespace-healthcheck/
-sli.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Event Count
-and Score`, `Get Container Restarts and Score`, `Get NotReady Pods`, `Generate
-Namspace Score` | This SLI uses kubectl to score namespace health. Produces a
-value between 0 (completely failing thet test) and 1 (fully passing the test).
-Looks for container restarts, events, and pods not ready. [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/k8s-namespace-healthcheck) | |
-[Kubernetes Namespace Troubleshoot](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/k8s-namespace-healthcheck/runbook.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Trace And Troubleshoot
-Namespace Warning Events And Errors`, `Troubleshoot Container Restarts In
-Namespace`, `Troubleshoot Pending Pods In Namespace`, `Troubleshoot Failed Pods
-In Namespace`, `Troubleshoot Workload Status Conditions In Namespace`, `Get
-Listing Of Resources In Namespace`, `Check For Namespace Event Anomalies`,
-`Troubleshoot Namespace Services And Application Workloads`, `Check Missing or
-Risky PodDisruptionBudget Policies` | This taskset runs general troubleshooting
-checks against all applicable objects in a namespace, checks error events, and
-searches pod logs for error entries. [Docs](https://docs.runwhen.com/public/v/
-cli-codecollection/k8s-namespace-healthcheck) | | [Kubernetes Persistent Volume
+`EKS`, `GKE`, `OpenShift` | `Fetch Ingress Object Health in Namespace `$
+{NAMESPACE}``, `Check for Ingress and Service Conflicts in Namespace `$
+{NAMESPACE}`` | Triages issues related to a ingress objects and services.
+[Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-ingress-
+healthcheck) | | [Kubernetes Jenkins Healthcheck](https://github.com/runwhen-
+contrib/rw-cli-codecollection/blob/main/codebundles/k8s-jenkins-healthcheck/
+runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Jenkins` |
+`Query The Jenkins Kubernetes Workload HTTP Endpoint`, `Query For Stuck Jenkins
+Jobs` | This taskset collects information about perstistent volumes and
+persistent volume claims to validate health or help troubleshoot potential
+issues. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-
+jenkins-healthcheck) | | [Kubernetes Labeled Pod Count](https://github.com/
+runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-labeledpods-
+healthcheck/sli.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` |
+`Measure Number of Running Pods with Label` | This codebundle fetches the
+number of running pods with the set of provided labels, letting you measure the
+number of running pods. [Docs](https://docs.runwhen.com/public/v/cli-
+codecollection/k8s-labeledpods-healthcheck) | | [Kubernetes Namespace
 Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/
-main/codebundles/k8s-pvc-healthcheck/runbook.robot) | `Kubernetes`, `AKS`,
-`EKS`, `GKE`, `OpenShift` | `Fetch Events for Unhealthy Kubernetes
-PersistentVolumeClaims`, `List PersistentVolumeClaims in Terminating State`,
-`List PersistentVolumes in Terminating State`, `List Pods with Attached Volumes
-and Related PersistentVolume Details`, `Fetch the Storage Utilization for PVC
-Mounts`, `Check for RWO Persistent Volume Node Attachment Issues` | This
-taskset collects information about storage such as PersistentVolumes and
-PersistentVolumeClaims to validate health or help troubleshoot potential
-storage issues. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/
-k8s-pvc-healthcheck) | | [Kubernetes Pod Resources Scan](https://github.com/
-runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-podresources-
-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Scan
-Labeled Pods and Show All Containers Without Resource Limit or Resource
-Requests Set`, `Get Labeled Container Top Info` | Inspects the resources
-provisioned for a given set of pods, selected by their labels and raises issues
-if no resources were specified. [Docs](https://docs.runwhen.com/public/v/cli-
-codecollection/k8s-podresources-health) | | [Kubernetes Postgres Triage](https:
-//github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-
-postgres-triage/runbook.robot) | `AKS`, `EKS`, `GKE`, `Kubernetes`, `Patroni`,
+main/codebundles/k8s-namespace-healthcheck/sli.robot) | `Kubernetes`, `AKS`,
+`EKS`, `GKE`, `OpenShift` | `Get Event Count and Score`, `Get Container
+Restarts and Score`, `Get NotReady Pods`, `Generate Namspace Score` | This SLI
+uses kubectl to score namespace health. Produces a value between 0 (completely
+failing thet test) and 1 (fully passing the test). Looks for container
+restarts, events, and pods not ready. [Docs](https://docs.runwhen.com/public/v/
+cli-codecollection/k8s-namespace-healthcheck) | | [Kubernetes Namespace
+Troubleshoot](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/
+main/codebundles/k8s-namespace-healthcheck/runbook.robot) | `Kubernetes`,
+`AKS`, `EKS`, `GKE`, `OpenShift` | `Troubleshoot Warning Events in Namespace `$
+{NAMESPACE}``, `Troubleshoot Container Restarts In Namespace `${NAMESPACE}``,
+`Troubleshoot Pending Pods In Namespace `${NAMESPACE}``, `Troubleshoot Failed
+Pods In Namespace `${NAMESPACE}``, `Troubleshoot Workload Status Conditions In
+Namespace `${NAMESPACE}``, `Get Listing Of Resources In Namespace `$
+{NAMESPACE}``, `Check Event Anomalies in Namespace `${NAMESPACE}``,
+`Troubleshoot Services And Application Workloads in Namespace `${NAMESPACE}``,
+`Check Missing or Risky PodDisruptionBudget Policies in Namepace `$
+{NAMESPACE}`` | This taskset runs general troubleshooting checks against all
+applicable objects in a namespace. Looks for warning events, odd or frequent
+normal events, restarting containers and failed or pending pods. [Docs](https:/
+/docs.runwhen.com/public/v/cli-codecollection/k8s-namespace-healthcheck) | |
+[Kubernetes Persistent Volume Healthcheck](https://github.com/runwhen-contrib/
+rw-cli-codecollection/blob/main/codebundles/k8s-pvc-healthcheck/runbook.robot)
+| `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Fetch Events for Unhealthy
+Kubernetes PersistentVolumeClaims in Namespace `${NAMESPACE}``, `List
+PersistentVolumeClaims in Terminating State in Namespace `${NAMESPACE}``, `List
+PersistentVolumes in Terminating State in Namespace `${NAMESPACE}``, `List Pods
+with Attached Volumes and Related PersistentVolume Details in Namespace `$
+{NAMESPACE}``, `Fetch the Storage Utilization for PVC Mounts in Namespace `$
+{NAMESPACE}``, `Check for RWO Persistent Volume Node Attachment Issues in
+Namespace `${NAMESPACE}`` | This taskset collects information about storage
+such as PersistentVolumes and PersistentVolumeClaims to validate health or help
+troubleshoot potential storage issues. [Docs](https://docs.runwhen.com/public/
+v/cli-codecollection/k8s-pvc-healthcheck) | | [Kubernetes Pod Resources Scan]
+(https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
+codebundles/k8s-podresources-health/runbook.robot) | `Kubernetes`, `AKS`,
+`EKS`, `GKE`, `OpenShift` | `Show Pods Without Resource Limit or Resource
+Requests Set in Namespace `${NAMESPACE}``, `Get Pod Resource Utilization with
+Top in Namespace `${NAMESPACE}`` | Inspects the resources provisioned for a
+given set of pods, selected by their labels and raises issues if no resources
+were specified. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/
+k8s-podresources-health) | | [Kubernetes Postgres Triage](https://github.com/
+runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-postgres-
+triage/runbook.robot) | `AKS`, `EKS`, `GKE`, `Kubernetes`, `Patroni`,
 `Postgres` | `Get Standard Postgres Resource Information`, `Describe Postgres
 Custom Resources`, `Get Postgres Pod Logs & Events`, `Get Postgres Pod Resource
 Utilization`, `Get Running Postgres Configuration`, `Get Patroni Output`, `Run
 DB Queries` | Runs multiple Kubernetes and psql commands to report on the
 health of a postgres cluster. [Docs](https://docs.runwhen.com/public/v/cli-
 codecollection/k8s-postgres-triage) | | [Kubernetes Redis Healthcheck](https://
 github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-
 redis-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`,
-`OpenShift`, `Redis` | `Ping Redis Workload`, `Verify Redis Read Write
-Operation` | This taskset collects information on your redis workload in your
-Kubernetes cluster and raises issues if any health checks fail. [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/k8s-redis-healthcheck) | |
-[Kubernetes Restart resource](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/k8s-restart-resource/runbook.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Current Resource State`,
-`Get Resource Logs`, `Restart Resource` | This taskset restarts a resource with
-a given set of labels, typically used with other tasksets. [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/k8s-restart-resource) | |
-[Kubernetes Service Account Check](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/k8s-serviceaccount-check/runbook.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Redis` | `Test Service Account
-Access to Kubernetes API Server` | This taskset provides tasks to troubleshoot
-service accounts in a Kubernetes namespace. [Docs](https://docs.runwhen.com/
-public/v/cli-codecollection/k8s-serviceaccount-check) | | [Kubernetes
-StatefulSet Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/
-blob/main/codebundles/k8s-statefulset-healthcheck/runbook.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Fetch StatefulSet Logs`, `Get
-Related StatefulSet Events`, `Fetch StatefulSet Manifest Details`, `List
-StatefulSets with Unhealthy Replica Counts` | Triages issues related to a
+`OpenShift`, `Redis` | `Ping `${DEPLOYMENT_NAME}` Redis Workload`, `Verify `$
+{DEPLOYMENT_NAME}` Redis Read Write Operation` | This taskset collects
+information on your redis workload in your Kubernetes cluster and raises issues
+if any health checks fail. [Docs](https://docs.runwhen.com/public/v/cli-
+codecollection/k8s-redis-healthcheck) | | [Kubernetes Restart resource](https:/
+/github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-
+restart-resource/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`,
+`OpenShift` | `Get Current Resource State`, `Get Resource Logs`, `Restart
+Resource` | This taskset restarts a resource with a given set of labels,
+typically used with other tasksets. [Docs](https://docs.runwhen.com/public/v/
+cli-codecollection/k8s-restart-resource) | | [Kubernetes Service Account Check]
+(https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
+codebundles/k8s-serviceaccount-check/runbook.robot) | `Kubernetes`, `AKS`,
+`EKS`, `GKE`, `OpenShift`, `Redis` | `Test Service Account Access to Kubernetes
+API Server` | This taskset provides tasks to troubleshoot service accounts in a
+Kubernetes namespace. [Docs](https://docs.runwhen.com/public/v/cli-
+codecollection/k8s-serviceaccount-check) | | [Kubernetes StatefulSet Triage]
+(https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
+codebundles/k8s-statefulset-healthcheck/runbook.robot) | `Kubernetes`, `AKS`,
+`EKS`, `GKE`, `OpenShift` | `Fetch StatefulSet `${STATEFULSET_NAME}` Logs`,
+`Get Related StatefulSet `${STATEFULSET_NAME}` Events`, `Fetch StatefulSet `$
+{STATEFULSET_NAME}` Manifest Details`, `List StatefulSets with Unhealthy
+Replica Counts In Namespace `${NAMESPACE}`` | Triages issues related to a
 StatefulSet and its replicas. [Docs](https://docs.runwhen.com/public/v/cli-
 codecollection/k8s-statefulset-healthcheck) | | [Kubernetes Vault Triage]
 (https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
 codebundles/k8s-vault-healthcheck/runbook.robot) | `AKS`, `EKS`, `GKE`,
 `Kubernetes`, `Vault` | `Fetch Vault CSI Driver Logs`, `Get Vault CSI Driver
 Warning Events`, `Check Vault CSI Driver Replicas`, `Fetch Vault Logs`, `Get
 Related Vault Events`, `Fetch Vault StatefulSet Manifest Details`, `Fetch Vault
@@ -287,21 +305,21 @@
 | Check whether the Terraform Cloud Workspace is in a locked state. [Docs]
 (https://docs.runwhen.com/public/v/cli-codecollection/terraform-cloud-
 workspace-lock-check) | | [Test Issues](https://github.com/runwhen-contrib/rw-
 cli-codecollection/blob/main/codebundles/test-issue/runbook.robot) | `Test` |
 `Raise Full Issue` | A codebundle for testing the issues feature. Purely for
 testing flow. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/test-
 issue) | | [cURL HTTP OK](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/curl-http-ok/runbook.robot) | `Linux macOS
+codecollection/blob/main/codebundles/curl-http-ok/sli.robot) | `Linux macOS
 Windows HTTP` | `Checking HTTP URL Is Available And Timely` | This taskset uses
-curl to validate the response code of the endpoint and provides the total time
-of the request. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/
-curl-http-ok) | | [cli-test-taskset](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/cli-test/runbook.robot) | `cli` | `Run CLI
-and Parse Output For Issues`, `Exec Test`, `Local Process Test` | This taskset
-smoketests the CLI codebundle setup and run process [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/cli-test) | | [cmd-test-taskset]
-(https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
+curl to validate the response code of the endpoint. Returns ascore of 1 if
+healthy, an 0 if unhealthy. [Docs](https://docs.runwhen.com/public/v/cli-
+codecollection/curl-http-ok) | | [cli-test-taskset](https://github.com/runwhen-
+contrib/rw-cli-codecollection/blob/main/codebundles/cli-test/runbook.robot) |
+`cli` | `Run CLI and Parse Output For Issues`, `Exec Test`, `Local Process
+Test` | This taskset smoketests the CLI codebundle setup and run process [Docs]
+(https://docs.runwhen.com/public/v/cli-codecollection/cli-test) | | [cmd-test-
+taskset](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
 codebundles/cmd-test/runbook.robot) | `cmd` | `Run CLI Command`, `Run Bash
 File`, `Log Suggestion` | This taskset smoketests the CLI codebundle setup and
 run process by running a bare command [Docs](https://docs.runwhen.com/public/v/
 cli-codecollection/cmd-test) |
```

### Comparing `runwhen-cli-keywords-0.0.8/RW/CLI/CLI.py` & `runwhen-cli-keywords-0.0.9/RW/CLI/CLI.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,19 @@
         files (dict, optional): a list of files to include in the environment during the command. Defaults to None.
 
     Returns:
         ShellServiceResponse: _description_
     """
     if not service:
         return execute_local_command(
-            cmd=cmd, request_secrets=request_secrets, env=env, files=files, timeout_seconds=timeout_seconds
+            cmd=cmd,
+            request_secrets=request_secrets,
+            env=env,
+            files=files,
+            timeout_seconds=timeout_seconds,
         )
     else:
         return platform.execute_shell_command(
             cmd=cmd,
             service=service,
             request_secrets=request_secrets,
             env=env,
@@ -83,53 +87,64 @@
     namespace: str = "",
     context: str = "",
     **kwargs,
 ) -> str:
     """**DEPRECATED**"""
     # if no specific workload name but labels provided, fetch the first running pod with labels
     if not workload_name and labels:
-        request_secrets: [platform.ShellServiceRequestSecret] = [] if len(kwargs.keys()) > 0 else None
+        request_secrets: [platform.ShellServiceRequestSecret] = (
+            [] if len(kwargs.keys()) > 0 else None
+        )
         request_secrets = _create_secrets_from_kwargs(**kwargs)
         pod_name_cmd = (
             f"kubectl get pods --field-selector=status.phase==Running -l {labels}"
             + " -o jsonpath='{.items[0].metadata.name}'"
             + f" -n {namespace} --context={context}"
         )
-        rsp = execute_command(cmd=pod_name_cmd, service=target_service, request_secrets=request_secrets, env=env)
+        rsp = execute_command(
+            cmd=pod_name_cmd,
+            service=target_service,
+            request_secrets=request_secrets,
+            env=env,
+        )
         SHELL_HISTORY.append(pod_name_cmd)
         cli_utils.verify_rsp(rsp)
         workload_name = rsp.stdout
     # use eval so that env variables are evaluated in the subprocess
-    cmd_template: str = (
-        f"eval $(echo \"kubectl exec -n {namespace} --context={context} {workload_name} -- /bin/bash -c '{cmd}'\")"
-    )
+    cmd_template: str = f"eval $(echo \"kubectl exec -n {namespace} --context={context} {workload_name} -- /bin/bash -c '{cmd}'\")"
     cmd = cmd_template
     logger.info(f"Templated remote exec: {cmd}")
     return cmd
 
 
 def _create_secrets_from_kwargs(**kwargs) -> list[platform.ShellServiceRequestSecret]:
     """Helper to organize dynamically set secrets in a kwargs list
 
     Returns:
         list[platform.ShellServiceRequestSecret]: secrets objects in list form.
     """
     global SECRET_PREFIX
     global SECRET_FILE_PREFIX
-    request_secrets: list[platform.ShellServiceRequestSecret] = [] if len(kwargs.keys()) > 0 else None
+    request_secrets: list[platform.ShellServiceRequestSecret] = (
+        [] if len(kwargs.keys()) > 0 else None
+    )
     for key, value in kwargs.items():
         if not key.startswith(SECRET_PREFIX) and not key.startswith(SECRET_FILE_PREFIX):
             continue
         if not isinstance(value, platform.Secret):
-            logger.warning(f"kwarg secret {value} in key {key} is the wrong type, should be platform.Secret")
+            logger.warning(
+                f"kwarg secret {value} in key {key} is the wrong type, should be platform.Secret"
+            )
             continue
         if key.startswith(SECRET_PREFIX):
             request_secrets.append(platform.ShellServiceRequestSecret(value))
         elif key.startswith(SECRET_FILE_PREFIX):
-            request_secrets.append(platform.ShellServiceRequestSecret(value, as_file=True))
+            request_secrets.append(
+                platform.ShellServiceRequestSecret(value, as_file=True)
+            )
     return request_secrets
 
 
 def run_bash_file(
     bash_file: str,
     target_service: platform.Service = None,
     env: dict = None,
@@ -163,25 +178,39 @@
             if rw_path_to_robot:
                 # Split the path at the patterns you provided and join with the new prefix
                 for pattern in ["sli.robot", "runbook.robot"]:
                     if pattern in rw_path_to_robot:
                         path, _ = rw_path_to_robot.split(pattern)
                         new_path = os.path.join("/collection", path)
                         # Modify the bash_file to point to the new directory
+                        local_bash_file = f"./{bash_file}"
                         bash_file = os.path.join(new_path, bash_file)
                         if os.path.exists(bash_file):
-                            logger.info(f"File '{bash_file}' found at derived path: {new_path}.")
-                            cmd_overide = f"{bash_file}"
+                            logger.info(
+                                f"File '{bash_file}' found at derived path: {new_path}."
+                            )
+                            if cmd_overide:
+                                cmd_overide = cmd_overide.replace(
+                                    f"{local_bash_file}", f"{bash_file}"
+                                )
+                            else:
+                                cmd_overide = f"{bash_file}"
                             break
                         else:
-                            logger.warning(f"File '{bash_file}' not found at derived path: {new_path}.")
+                            logger.warning(
+                                f"File '{bash_file}' not found at derived path: {new_path}."
+                            )
             else:
-                logger.warning("Current directory is root, but 'RW_PATH_TO_ROBOT' is not set.")
+                logger.warning(
+                    "Current directory is root, but 'RW_PATH_TO_ROBOT' is not set."
+                )
         else:
-            logger.warning(f"File '{bash_file}' not found in the current directory and current directory is not root.")
+            logger.warning(
+                f"File '{bash_file}' not found in the current directory and current directory is not root."
+            )
 
     if not cmd_overide:
         cmd_overide = f"./{bash_file}"
     logger.info(f"Received kwargs: {kwargs}")
     request_secrets = _create_secrets_from_kwargs(**kwargs)
     file_contents: str = ""
     with open(f"{bash_file}", "r") as fh:
@@ -240,27 +269,31 @@
 
     Returns:
         platform.ShellServiceResponse: the structured response from running the shell commands.
     """
     global SHELL_HISTORY
     looped_results = []
     rsp = None
-    logger.info(f"Requesting command: {cmd} with service: {target_service} - None indicates run local")
+    logger.info(
+        f"Requesting command: {cmd} with service: {target_service} - None indicates run local"
+    )
     if run_in_workload_with_labels or run_in_workload_with_name:
         cmd = _create_kubernetes_remote_exec(
             cmd=cmd,
             target_service=target_service,
             env=env,
             labels=run_in_workload_with_labels,
             workload_name=run_in_workload_with_name,
             namespace=optional_namespace,
             context=optional_context,
             **kwargs,
         )
-    request_secrets: [platform.ShellServiceRequestSecret] = [] if len(kwargs.keys()) > 0 else None
+    request_secrets: [platform.ShellServiceRequestSecret] = (
+        [] if len(kwargs.keys()) > 0 else None
+    )
     logger.info(f"Received kwargs: {kwargs}")
     request_secrets = _create_secrets_from_kwargs(**kwargs)
     if loop_with_items and len(loop_with_items) > 0:
         for item in loop_with_items:
             cmd = cmd.format(item=item)
             iter_rsp = execute_command(
                 cmd=cmd,
@@ -284,15 +317,19 @@
             returncode=rsp.returncode,
             status=rsp.status,
             body=rsp.body,
             errors=rsp.errors,
         )
     else:
         rsp = execute_command(
-            cmd=cmd, service=target_service, request_secrets=request_secrets, env=env, timeout_seconds=timeout_seconds
+            cmd=cmd,
+            service=target_service,
+            request_secrets=request_secrets,
+            env=env,
+            timeout_seconds=timeout_seconds,
         )
         if include_in_history:
             SHELL_HISTORY.append(cmd)
     logger.info(f"shell stdout: {rsp.stdout}")
     logger.info(f"shell stderr: {rsp.stderr}")
     logger.info(f"shell status: {rsp.status}")
     logger.info(f"shell returncode: {rsp.returncode}")
```

### Comparing `runwhen-cli-keywords-0.0.8/RW/CLI/cli_utils.py` & `runwhen-cli-keywords-0.0.9/RW/CLI/cli_utils.py`

 * *Files identical despite different names*

### Comparing `runwhen-cli-keywords-0.0.8/RW/CLI/json_parser.py` & `runwhen-cli-keywords-0.0.9/RW/CLI/json_parser.py`

 * *Files identical despite different names*

### Comparing `runwhen-cli-keywords-0.0.8/RW/CLI/local_process.py` & `runwhen-cli-keywords-0.0.9/RW/CLI/local_process.py`

 * *Files identical despite different names*

### Comparing `runwhen-cli-keywords-0.0.8/RW/CLI/stdout_parser.py` & `runwhen-cli-keywords-0.0.9/RW/CLI/stdout_parser.py`

 * *Files identical despite different names*

### Comparing `runwhen-cli-keywords-0.0.8/RW/K8sApplications/k8s_applications.py` & `runwhen-cli-keywords-0.0.9/RW/K8sApplications/k8s_applications.py`

 * *Files identical despite different names*

### Comparing `runwhen-cli-keywords-0.0.8/RW/K8sApplications/parsers.py` & `runwhen-cli-keywords-0.0.9/RW/K8sApplications/parsers.py`

 * *Files identical despite different names*

### Comparing `runwhen-cli-keywords-0.0.8/RW/K8sApplications/repository.py` & `runwhen-cli-keywords-0.0.9/RW/K8sApplications/repository.py`

 * *Files identical despite different names*

### Comparing `runwhen-cli-keywords-0.0.8/RW/NextSteps/Kubernetes/mapping.yaml` & `runwhen-cli-keywords-0.0.9/RW/NextSteps/Kubernetes/mapping.yaml`

 * *Files identical despite different names*

### Comparing `runwhen-cli-keywords-0.0.8/RW/NextSteps/Suggest.py` & `runwhen-cli-keywords-0.0.9/RW/NextSteps/Suggest.py`

 * *Files identical despite different names*

### Comparing `runwhen-cli-keywords-0.0.8/runwhen_cli_keywords.egg-info/PKG-INFO` & `runwhen-cli-keywords-0.0.9/runwhen_cli_keywords.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: runwhen-cli-keywords
-Version: 0.0.8
+Version: 0.0.9
 Summary: A set of RunWhen published CLI keywords and python libraries for interacting with APIs using CLIs
 Home-page: https://github.com/runwhen-contrib/rw-cli-codecollection
 Author: Kyle Forster
 Author-email: kyle.forster@runwhen.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Troubleshooting Tasks in Codecollection: **123**
-Codebundles in Codecollection: **44**
+Troubleshooting Tasks in Codecollection: **128**
+Codebundles in Codecollection: **45**
 
 ![](docs/GitHub_Banner.jpg)
 
 <p align="center">
   <a href="https://discord.gg/Ut7Ws4rm8Q">
     <img src="https://img.shields.io/discord/1131539039665791077?label=Join%20Discord&logo=discord&logoColor=white&style=for-the-badge" alt="Join Discord">
   </a>
@@ -64,45 +64,46 @@
 |---|---|---|---|
 | [AWS CloudWatch Overutlized EC2 Inspection](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/aws-cloudwatch-overused-ec2/runbook.robot) | `AWS`, `CloudWatch` | `Check For Overutilized Ec2 Instances` | Queries AWS CloudWatch for a list of EC2 instances with a high amount of resource utilization, raising issues when overutilized instances are found. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/aws-cloudwatch-overused-ec2) |
 | [AWS EKS Nodegroup Status Check](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/aws-eks-node-reboot/runbook.robot) | `AWS`, `EKS` | `Check EKS Nodegroup Status` | Queries a node group within a EKS cluster to check if the nodegroup has degraded service, indicating ongoing reboots or other issues. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/aws-eks-node-reboot) |
 | [Azure Internal LoadBalancer Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/azure-loadbalancer-triage/runbook.robot) | `Kubernetes`, `AKS`, `Azure` | `Health Check Internal Azure Load Balancer` | Triages issues related to a Azure Loadbalancers and its activity logs. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/azure-loadbalancer-triage) |
 | [Azure Monitor Activity Log SLI](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/azure-monitor-event-triage/sli.robot) | `Kubernetes`, `AKS`, `Azure` | `Run Azure Monitor Activity Log Triage` | Measures the count of error activity log entries as a SLI metric for the Azure tenancy. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/azure-monitor-event-triage) |
 | [Azure Monitor Event Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/azure-monitor-event-triage/runbook.robot) | `Kubernetes`, `AKS`, `Azure` | `Run Azure Monitor Activity Log Triage` | Triages issues related to a Azure Loadbalancers, Kubernetes ingress objects and services. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/azure-monitor-event-triage) |
 | [GCP Gcloud Log Inspection](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/gcloud-log-inspection/runbook.robot) | `GCP`, `Gcloud`, `Google Monitoring` | `Inspect GCP Logs For Common Errors` | Fetches logs from a GCP using a configurable query and raises an issue with details on the most common issues. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/gcloud-log-inspection) |
-| [GCP Node Prempt List](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/gcloud-node-preempt/runbook.robot) | `GCP`, `GKE` | `List all nodes in an active prempt operation` | List all GCP nodes that have an active preempt operation. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/gcloud-node-preempt) |
+| [GCP Node Prempt List](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/gcloud-node-preempt/sli.robot) | `GCP`, `GKE` | `Count the number of nodes in active prempt operation` | Check if any GCP nodes have an active preempt operation. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/gcloud-node-preempt) |
 | [GKE Kong Ingress Host Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/curl-gmp-kong-ingress-inspection/runbook.robot) | `GCP`, `GMP`, `Ingress`, `Kong`, `Metrics` | `Check If Kong Ingress HTTP Error Rate Violates HTTP Error Threshold`, `Check If Kong Ingress HTTP Request Latency Violates Threshold`, `Check If Kong Ingress Controller Reports Upstream Errors` | Collects Kong ingress host metrics from GMP on GCP and inspects the results for ingress with a HTTP error code rate greater than zero over a configurable duration and raises issues based on the number of ingress with error codes. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/curl-gmp-kong-ingress-inspection) |
-| [GKE Nginx Ingress Host Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/curl-gmp-nginx-ingress-inspection/runbook.robot) | `GCP`, `GMP`, `Ingress`, `Nginx`, `Metrics` | `Fetch Nginx Ingress HTTP Errors From GMP And Perform Inspection On Results`, `Find Ingress Owner and Service Health` | Collects Nginx ingress host controller metrics from GMP on GCP and inspects the results for ingress with a HTTP error code rate greater than zero over a configurable duration and raises issues based on the number of ingress with error codes. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/curl-gmp-nginx-ingress-inspection) |
+| [GKE Nginx Ingress Host Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/curl-gmp-nginx-ingress-inspection/runbook.robot) | `GCP`, `GMP`, `Ingress`, `Nginx`, `Metrics` | `Fetch Nginx HTTP Errors From GMP for Ingress `${INGRESS_OBJECT_NAME}``, `Find Owner and Service Health for Ingress `${INGRESS_OBJECT_NAME}`` | Collects Nginx ingress host controller metrics from GMP on GCP and inspects the results for ingress with a HTTP error code rate greater than zero over a configurable duration and raises issues based on the number of ingress with error codes. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/curl-gmp-nginx-ingress-inspection) |
 | [Kubeprometheus Operator Troubleshoot](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-prometheus-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Prometheus` | `Check Prometheus Service Monitors`, `Check For Successful Rule Setup`, `Verify Prometheus RBAC Can Access ServiceMonitors`, `Identify Endpoint Scraping Errors`, `Check Prometheus API Healthy` | This taskset investigates the logs, state and health of Kubernetes Prometheus operator. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-prometheus-healthcheck) |
-| [Kubernetes Application Troubleshoot](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-app-troubleshoot/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Resource Logs`, `Scan For Misconfigured Environment` | Triages issues related to a deployment and its replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-app-troubleshoot) |
+| [Kubernetes Application Monitor](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-app-troubleshoot/sli.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Measure Application Exceptions` | Measures the number of exception stacktraces present in an application's logs over a time period. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-app-troubleshoot) |
+| [Kubernetes Application Troubleshoot](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-app-troubleshoot/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Workload Logs`, `Scan For Misconfigured Environment`, `Troubleshoot Application Logs` | Triages issues related to a deployment and its replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-app-troubleshoot) |
 | [Kubernetes ArgoCD Application Health & Troubleshoot](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-argocd-application-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `ArgoCD` | `Fetch ArgoCD Application Sync Status & Health`, `Fetch ArgoCD Application Last Sync Operation Details`, `Fetch Unhealthy ArgoCD Application Resources`, `Scan For Errors in Pod Logs Related to ArgoCD Application Deployments`, `Fully Describe ArgoCD Application` | This taskset collects information and runs general troubleshooting checks against argocd application objects within a namespace. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-argocd-application-health) |
 | [Kubernetes ArgoCD HelmRelease TaskSet](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-argocd-helm-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `ArgoCD` | `Fetch all available ArgoCD Helm releases`, `Fetch Installed ArgoCD Helm release versions` | This codebundle runs a series of tasks to identify potential helm release issues related to ArgoCD managed Helm objects. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-argocd-helm-health) |
 | [Kubernetes Artifactory Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-artifactory-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Artifactory` | `Check Artifactory Liveness and Readiness Endpoints` | Performs a triage on the Open Source version of Artifactory in a Kubernetes cluster. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-artifactory-health) |
-| [Kubernetes CertManager Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-certmanager-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `CertManager` | `Get Namespace Certificate Summary`, `Find Failed Certificate Requests and Identify Issues` | This taskset checks that your cert manager certificates are renewing as expected, raising issues when they are past due in the configured namespace [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-certmanager-healthcheck) |
+| [Kubernetes CertManager Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-certmanager-healthcheck/sli.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Health Score of CertManager Workloads` | Check the health of pods deployed by cert-manager. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-certmanager-healthcheck) |
 | [Kubernetes Daemonset Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-daemonset-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get DaemonSet Log Details For Report`, `Get Related Daemonset Events`, `Check Daemonset Replicas` | Triages issues related to a Daemonset and its available replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-daemonset-healthcheck) |
-| [Kubernetes Deployment Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-deployment-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Check Deployment Log For Issues`, `Troubleshoot Deployment Warning Events`, `Get Deployment Workload Details For Report`, `Troubleshoot Deployment Replicas`, `Check For Deployment Event Anomalies` | Triages issues related to a deployment and its replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-deployment-healthcheck) |
+| [Kubernetes Deployment Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-deployment-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Check Deployment Log For Issues with `${DEPLOYMENT_NAME}``, `Check Liveness Probe Configuration for Deployment `${DEPLOYMENT_NAME}``, `Check Readiness Probe Configuration for Deployment `${DEPLOYMENT_NAME}``, `Troubleshoot Deployment Warning Events for `${DEPLOYMENT_NAME}``, `Get Deployment Workload Details For `${DEPLOYMENT_NAME}` and Add to Report`, `Troubleshoot Deployment Replicas for `${DEPLOYMENT_NAME}``, `Check Deployment Event Anomalies for `${DEPLOYMENT_NAME}`` | Triages issues related to a deployment and its replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-deployment-healthcheck) |
 | [Kubernetes Flux Choas Testing](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-chaos-flux/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Suspend the Flux Resource Reconciliation`, `Find Random FluxCD Workload as Chaos Target`, `Execute Chaos Command`, `Execute Additional Chaos Command`, `Resume Flux Resource Reconciliation` | This taskset is used to suspend a flux resource for the purposes of executing chaos tasks. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-chaos-flux) |
 | [Kubernetes FluxCD HelmRelease TaskSet](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-fluxcd-helm-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `FluxCD` | `List all available FluxCD Helmreleases`, `Fetch Installed FluxCD Helmrelease Versions`, `Fetch Mismatched FluxCD HelmRelease Version`, `Fetch FluxCD HelmRelease Error Messages`, `Check for Available Helm Chart Updates` | This codebundle runs a series of tasks to identify potential helm release issues related to Flux managed Helm objects. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-fluxcd-helm-health) |
 | [Kubernetes FluxCD Kustomization TaskSet](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-fluxcd-kustomization-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `FluxCD` | `List all available Kustomization objects`, `Get details for unready Kustomizations` | This codebundle runs a series of tasks to identify potential Kustomization issues related to Flux managed Kustomization objects. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-fluxcd-kustomization-health) |
 | [Kubernetes Grafana Loki Health Check](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-loki-healthcheck/runbook.robot) | `k8s` | `Check Loki Ring API`, `Check Loki API Ready` | This taskset checks the health of Grafana Loki and its hash ring. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-loki-healthcheck) |
-| [Kubernetes Image Check](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-image-check/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Check Image Rollover Times In Namespace`, `List Images and Tags for Every Container in Running Pods`, `List Images and Tags for Every Container in Failed Pods`, `List ImagePullBackOff Events and Test Path and Tags` | This taskset provides detailed information about the images used in a Kubernetes namespace. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-image-check) |
+| [Kubernetes Image Check](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-image-check/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Check Image Rollover Times for Namespace `${NAMESPACE}``, `List Images and Tags for Every Container in Running Pods for Namespace `${NAMESPACE}``, `List Images and Tags for Every Container in Failed Pods for Namespace `${NAMESPACE}``, `List ImagePullBackOff Events and Test Path and Tags for Namespace `${NAMESPACE}`` | This taskset provides detailed information about the images used in a Kubernetes namespace. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-image-check) |
 | [Kubernetes Ingress GCE & GCP HTTP Load Balancer Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-ingress-gce-healthcheck/runbook.robot) | `Kubernetes`, `GKE`, `GCE`, `GCP` | `Search For GCE Ingress Warnings in GKE`, `Identify Unhealthy GCE HTTP Ingress Backends`, `Validate GCP HTTP Load Balancer Configurations`, `Fetch Network Error Logs from GCP Operations Manager for Ingress Backends`, `Review GCP Operations Logging Dashboard` | Troubleshoot GCE Ingress Resources related to GCP HTTP Load Balancer in GKE [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-ingress-gce-healthcheck) |
-| [Kubernetes Ingress Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-ingress-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Fetch Ingress Object Health in Namespace` | Triages issues related to a ingress objects and services. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-ingress-healthcheck) |
+| [Kubernetes Ingress Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-ingress-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Fetch Ingress Object Health in Namespace `${NAMESPACE}``, `Check for Ingress and Service Conflicts in Namespace `${NAMESPACE}`` | Triages issues related to a ingress objects and services. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-ingress-healthcheck) |
 | [Kubernetes Jenkins Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-jenkins-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Jenkins` | `Query The Jenkins Kubernetes Workload HTTP Endpoint`, `Query For Stuck Jenkins Jobs` | This taskset collects information about perstistent volumes and persistent volume claims to validate health or help troubleshoot potential issues. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-jenkins-healthcheck) |
 | [Kubernetes Labeled Pod Count](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-labeledpods-healthcheck/sli.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Measure Number of Running Pods with Label` | This codebundle fetches the number of running pods with the set of provided labels, letting you measure the number of running pods. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-labeledpods-healthcheck) |
 | [Kubernetes Namespace Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-namespace-healthcheck/sli.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Event Count and Score`, `Get Container Restarts and Score`, `Get NotReady Pods`, `Generate Namspace Score` | This SLI uses kubectl to score namespace health. Produces a value between 0 (completely failing thet test) and 1 (fully passing the test). Looks for container restarts, events, and pods not ready. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-namespace-healthcheck) |
-| [Kubernetes Namespace Troubleshoot](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-namespace-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Trace And Troubleshoot Namespace Warning Events And Errors`, `Troubleshoot Container Restarts In Namespace`, `Troubleshoot Pending Pods In Namespace`, `Troubleshoot Failed Pods In Namespace`, `Troubleshoot Workload Status Conditions In Namespace`, `Get Listing Of Resources In Namespace`, `Check For Namespace Event Anomalies`, `Troubleshoot Namespace Services And Application Workloads`, `Check Missing or Risky PodDisruptionBudget Policies` | This taskset runs general troubleshooting checks against all applicable objects in a namespace, checks error events, and searches pod logs for error entries. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-namespace-healthcheck) |
-| [Kubernetes Persistent Volume Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-pvc-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Fetch Events for Unhealthy Kubernetes PersistentVolumeClaims`, `List PersistentVolumeClaims in Terminating State`, `List PersistentVolumes in Terminating State`, `List Pods with Attached Volumes and Related PersistentVolume Details`, `Fetch the Storage Utilization for PVC Mounts`, `Check for RWO Persistent Volume Node Attachment Issues` | This taskset collects information about storage such as PersistentVolumes and PersistentVolumeClaims to validate health or help troubleshoot potential storage issues. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-pvc-healthcheck) |
-| [Kubernetes Pod Resources Scan](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-podresources-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Scan Labeled Pods and Show All Containers Without Resource Limit or Resource Requests Set`, `Get Labeled Container Top Info` | Inspects the resources provisioned for a given set of pods, selected by their labels and raises issues if no resources were specified. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-podresources-health) |
+| [Kubernetes Namespace Troubleshoot](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-namespace-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Troubleshoot Warning Events in Namespace `${NAMESPACE}``, `Troubleshoot Container Restarts In Namespace `${NAMESPACE}``, `Troubleshoot Pending Pods In Namespace `${NAMESPACE}``, `Troubleshoot Failed Pods In Namespace `${NAMESPACE}``, `Troubleshoot Workload Status Conditions In Namespace `${NAMESPACE}``, `Get Listing Of Resources In Namespace `${NAMESPACE}``, `Check Event Anomalies in Namespace `${NAMESPACE}``, `Troubleshoot Services And Application Workloads in Namespace `${NAMESPACE}``, `Check Missing or Risky PodDisruptionBudget Policies in Namepace `${NAMESPACE}`` | This taskset runs general troubleshooting checks against all applicable objects in a namespace. Looks for warning events, odd or frequent normal events, restarting containers and failed or pending pods. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-namespace-healthcheck) |
+| [Kubernetes Persistent Volume Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-pvc-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Fetch Events for Unhealthy Kubernetes PersistentVolumeClaims in Namespace `${NAMESPACE}``, `List PersistentVolumeClaims in Terminating State in Namespace `${NAMESPACE}``, `List PersistentVolumes in Terminating State in Namespace `${NAMESPACE}``, `List Pods with Attached Volumes and Related PersistentVolume Details in Namespace `${NAMESPACE}``, `Fetch the Storage Utilization for PVC Mounts in Namespace `${NAMESPACE}``, `Check for RWO Persistent Volume Node Attachment Issues in Namespace `${NAMESPACE}`` | This taskset collects information about storage such as PersistentVolumes and PersistentVolumeClaims to validate health or help troubleshoot potential storage issues. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-pvc-healthcheck) |
+| [Kubernetes Pod Resources Scan](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-podresources-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Show Pods Without Resource Limit or Resource Requests Set in Namespace `${NAMESPACE}``, `Get Pod Resource Utilization with Top in Namespace `${NAMESPACE}`` | Inspects the resources provisioned for a given set of pods, selected by their labels and raises issues if no resources were specified. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-podresources-health) |
 | [Kubernetes Postgres Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-postgres-triage/runbook.robot) | `AKS`, `EKS`, `GKE`, `Kubernetes`, `Patroni`, `Postgres` | `Get Standard Postgres Resource Information`, `Describe Postgres Custom Resources`, `Get Postgres Pod Logs & Events`, `Get Postgres Pod Resource Utilization`, `Get Running Postgres Configuration`, `Get Patroni Output`, `Run DB Queries` | Runs multiple Kubernetes and psql commands to report on the health of a postgres cluster. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-postgres-triage) |
-| [Kubernetes Redis Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-redis-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Redis` | `Ping Redis Workload`, `Verify Redis Read Write Operation` | This taskset collects information on your redis workload in your Kubernetes cluster and raises issues if any health checks fail. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-redis-healthcheck) |
+| [Kubernetes Redis Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-redis-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Redis` | `Ping `${DEPLOYMENT_NAME}` Redis Workload`, `Verify `${DEPLOYMENT_NAME}` Redis Read Write Operation` | This taskset collects information on your redis workload in your Kubernetes cluster and raises issues if any health checks fail. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-redis-healthcheck) |
 | [Kubernetes Restart resource](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-restart-resource/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Current Resource State`, `Get Resource Logs`, `Restart Resource` | This taskset restarts a resource with a given set of labels, typically used with other tasksets. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-restart-resource) |
 | [Kubernetes Service Account Check](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-serviceaccount-check/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Redis` | `Test Service Account Access to Kubernetes API Server` | This taskset provides tasks to troubleshoot service accounts in a Kubernetes namespace. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-serviceaccount-check) |
-| [Kubernetes StatefulSet Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-statefulset-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Fetch StatefulSet Logs`, `Get Related StatefulSet Events`, `Fetch StatefulSet Manifest Details`, `List StatefulSets with Unhealthy Replica Counts` | Triages issues related to a StatefulSet and its replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-statefulset-healthcheck) |
+| [Kubernetes StatefulSet Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-statefulset-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Fetch StatefulSet `${STATEFULSET_NAME}` Logs`, `Get Related StatefulSet `${STATEFULSET_NAME}` Events`, `Fetch StatefulSet `${STATEFULSET_NAME}` Manifest Details`, `List StatefulSets with Unhealthy Replica Counts In Namespace `${NAMESPACE}`` | Triages issues related to a StatefulSet and its replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-statefulset-healthcheck) |
 | [Kubernetes Vault Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-vault-healthcheck/runbook.robot) | `AKS`, `EKS`, `GKE`, `Kubernetes`, `Vault` | `Fetch Vault CSI Driver Logs`, `Get Vault CSI Driver Warning Events`, `Check Vault CSI Driver Replicas`, `Fetch Vault Logs`, `Get Related Vault Events`, `Fetch Vault StatefulSet Manifest Details`, `Fetch Vault DaemonSet Manifest Details`, `Verify Vault Availability`, `Check Vault StatefulSet Replicas` | A suite of tasks that can be used to triage potential issues in your vault namespace. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-vault-healthcheck) |
 | [Terraform Cloud Workspace Lock Check](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/terraform-cloud-workspace-lock-check/runbook.robot) | `Terraform Cloud` | `Checking whether the Terraform Cloud Workspace is in a locked state` | Check whether the Terraform Cloud Workspace is in a locked state. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/terraform-cloud-workspace-lock-check) |
 | [Test Issues](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/test-issue/runbook.robot) | `Test` | `Raise Full Issue` | A codebundle for testing the issues feature. Purely for testing flow. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/test-issue) |
-| [cURL HTTP OK](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/curl-http-ok/runbook.robot) | `Linux macOS Windows HTTP` | `Checking HTTP URL Is Available And Timely` | This taskset uses curl to validate the response code of the endpoint and provides the total time of the request. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/curl-http-ok) |
+| [cURL HTTP OK](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/curl-http-ok/sli.robot) | `Linux macOS Windows HTTP` | `Checking HTTP URL Is Available And Timely` | This taskset uses curl to validate the response code of the endpoint. Returns ascore of 1 if healthy, an 0 if unhealthy. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/curl-http-ok) |
 | [cli-test-taskset](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/cli-test/runbook.robot) | `cli` | `Run CLI and Parse Output For Issues`, `Exec Test`, `Local Process Test` | This taskset smoketests the CLI codebundle setup and run process [Docs](https://docs.runwhen.com/public/v/cli-codecollection/cli-test) |
 | [cmd-test-taskset](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/cmd-test/runbook.robot) | `cmd` | `Run CLI Command`, `Run Bash File`, `Log Suggestion` | This taskset smoketests the CLI codebundle setup and run process by running a bare command [Docs](https://docs.runwhen.com/public/v/cli-codecollection/cmd-test) |
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: runwhen-cli-keywords Version: 0.0.8 Summary: A set
+Metadata-Version: 2.1 Name: runwhen-cli-keywords Version: 0.0.9 Summary: A set
 of RunWhen published CLI keywords and python libraries for interacting with
 APIs using CLIs Home-page: https://github.com/runwhen-contrib/rw-cli-
 codecollection Author: Kyle Forster Author-email: kyle.forster@runwhen.com
 License: Apache License 2.0 Platform: UNKNOWN Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown License-File: LICENSE Troubleshooting
-Tasks in Codecollection: **123** Codebundles in Codecollection: **44** ![]
+Tasks in Codecollection: **128** Codebundles in Codecollection: **45** ![]
 (docs/GitHub_Banner.jpg)
                                 _[_J_o_i_n_ _D_i_s_c_o_r_d_]
                                  _[_J_o_i_n_ _S_l_a_c_k_]
 _[_O_p_e_n_ _i_n_ _G_i_t_H_u_b_ _C_o_d_e_s_p_a_c_e_s_]# RunWhen Public Codecollection This repository is a
 codecollection that is to be used within the RunWhen platform. It contains
 codebundles that can be used in SLIs, and TaskSets. Please see the **
 [contributing](CONTRIBUTING.md)** and **[code of conduct](CODE_OF_CONDUCT.md)**
@@ -63,91 +63,99 @@
 public/v/cli-codecollection/azure-monitor-event-triage) | | [GCP Gcloud Log
 Inspection](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
 codebundles/gcloud-log-inspection/runbook.robot) | `GCP`, `Gcloud`, `Google
 Monitoring` | `Inspect GCP Logs For Common Errors` | Fetches logs from a GCP
 using a configurable query and raises an issue with details on the most common
 issues. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/gcloud-log-
 inspection) | | [GCP Node Prempt List](https://github.com/runwhen-contrib/rw-
-cli-codecollection/blob/main/codebundles/gcloud-node-preempt/runbook.robot) |
-`GCP`, `GKE` | `List all nodes in an active prempt operation` | List all GCP
-nodes that have an active preempt operation. [Docs](https://docs.runwhen.com/
-public/v/cli-codecollection/gcloud-node-preempt) | | [GKE Kong Ingress Host
-Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
-codebundles/curl-gmp-kong-ingress-inspection/runbook.robot) | `GCP`, `GMP`,
-`Ingress`, `Kong`, `Metrics` | `Check If Kong Ingress HTTP Error Rate Violates
-HTTP Error Threshold`, `Check If Kong Ingress HTTP Request Latency Violates
-Threshold`, `Check If Kong Ingress Controller Reports Upstream Errors` |
-Collects Kong ingress host metrics from GMP on GCP and inspects the results for
-ingress with a HTTP error code rate greater than zero over a configurable
+cli-codecollection/blob/main/codebundles/gcloud-node-preempt/sli.robot) |
+`GCP`, `GKE` | `Count the number of nodes in active prempt operation` | Check
+if any GCP nodes have an active preempt operation. [Docs](https://
+docs.runwhen.com/public/v/cli-codecollection/gcloud-node-preempt) | | [GKE Kong
+Ingress Host Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/
+blob/main/codebundles/curl-gmp-kong-ingress-inspection/runbook.robot) | `GCP`,
+`GMP`, `Ingress`, `Kong`, `Metrics` | `Check If Kong Ingress HTTP Error Rate
+Violates HTTP Error Threshold`, `Check If Kong Ingress HTTP Request Latency
+Violates Threshold`, `Check If Kong Ingress Controller Reports Upstream Errors`
+| Collects Kong ingress host metrics from GMP on GCP and inspects the results
+for ingress with a HTTP error code rate greater than zero over a configurable
 duration and raises issues based on the number of ingress with error codes.
 [Docs](https://docs.runwhen.com/public/v/cli-codecollection/curl-gmp-kong-
 ingress-inspection) | | [GKE Nginx Ingress Host Triage](https://github.com/
 runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/curl-gmp-nginx-
 ingress-inspection/runbook.robot) | `GCP`, `GMP`, `Ingress`, `Nginx`, `Metrics`
-| `Fetch Nginx Ingress HTTP Errors From GMP And Perform Inspection On Results`,
-`Find Ingress Owner and Service Health` | Collects Nginx ingress host
-controller metrics from GMP on GCP and inspects the results for ingress with a
-HTTP error code rate greater than zero over a configurable duration and raises
-issues based on the number of ingress with error codes. [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/curl-gmp-nginx-ingress-inspection)
-| | [Kubeprometheus Operator Troubleshoot](https://github.com/runwhen-contrib/
-rw-cli-codecollection/blob/main/codebundles/k8s-prometheus-healthcheck/
-runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Prometheus` |
-`Check Prometheus Service Monitors`, `Check For Successful Rule Setup`, `Verify
-Prometheus RBAC Can Access ServiceMonitors`, `Identify Endpoint Scraping
-Errors`, `Check Prometheus API Healthy` | This taskset investigates the logs,
-state and health of Kubernetes Prometheus operator. [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/k8s-prometheus-healthcheck) | |
+| `Fetch Nginx HTTP Errors From GMP for Ingress `${INGRESS_OBJECT_NAME}``,
+`Find Owner and Service Health for Ingress `${INGRESS_OBJECT_NAME}`` | Collects
+Nginx ingress host controller metrics from GMP on GCP and inspects the results
+for ingress with a HTTP error code rate greater than zero over a configurable
+duration and raises issues based on the number of ingress with error codes.
+[Docs](https://docs.runwhen.com/public/v/cli-codecollection/curl-gmp-nginx-
+ingress-inspection) | | [Kubeprometheus Operator Troubleshoot](https://
+github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-
+prometheus-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`,
+`OpenShift`, `Prometheus` | `Check Prometheus Service Monitors`, `Check For
+Successful Rule Setup`, `Verify Prometheus RBAC Can Access ServiceMonitors`,
+`Identify Endpoint Scraping Errors`, `Check Prometheus API Healthy` | This
+taskset investigates the logs, state and health of Kubernetes Prometheus
+operator. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-
+prometheus-healthcheck) | | [Kubernetes Application Monitor](https://
+github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-app-
+troubleshoot/sli.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` |
+`Measure Application Exceptions` | Measures the number of exception stacktraces
+present in an application's logs over a time period. [Docs](https://
+docs.runwhen.com/public/v/cli-codecollection/k8s-app-troubleshoot) | |
 [Kubernetes Application Troubleshoot](https://github.com/runwhen-contrib/rw-
 cli-codecollection/blob/main/codebundles/k8s-app-troubleshoot/runbook.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Resource Logs`, `Scan For
-Misconfigured Environment` | Triages issues related to a deployment and its
-replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-app-
-troubleshoot) | | [Kubernetes ArgoCD Application Health & Troubleshoot](https:/
-/github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-
-argocd-application-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`,
-`OpenShift`, `ArgoCD` | `Fetch ArgoCD Application Sync Status & Health`, `Fetch
-ArgoCD Application Last Sync Operation Details`, `Fetch Unhealthy ArgoCD
-Application Resources`, `Scan For Errors in Pod Logs Related to ArgoCD
-Application Deployments`, `Fully Describe ArgoCD Application` | This taskset
-collects information and runs general troubleshooting checks against argocd
-application objects within a namespace. [Docs](https://docs.runwhen.com/public/
-v/cli-codecollection/k8s-argocd-application-health) | | [Kubernetes ArgoCD
-HelmRelease TaskSet](https://github.com/runwhen-contrib/rw-cli-codecollection/
-blob/main/codebundles/k8s-argocd-helm-health/runbook.robot) | `Kubernetes`,
-`AKS`, `EKS`, `GKE`, `OpenShift`, `ArgoCD` | `Fetch all available ArgoCD Helm
-releases`, `Fetch Installed ArgoCD Helm release versions` | This codebundle
-runs a series of tasks to identify potential helm release issues related to
-ArgoCD managed Helm objects. [Docs](https://docs.runwhen.com/public/v/cli-
-codecollection/k8s-argocd-helm-health) | | [Kubernetes Artifactory Triage]
-(https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
-codebundles/k8s-artifactory-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`,
-`GKE`, `OpenShift`, `Artifactory` | `Check Artifactory Liveness and Readiness
-Endpoints` | Performs a triage on the Open Source version of Artifactory in a
-Kubernetes cluster. [Docs](https://docs.runwhen.com/public/v/cli-
-codecollection/k8s-artifactory-health) | | [Kubernetes CertManager Healthcheck]
-(https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
-codebundles/k8s-certmanager-healthcheck/runbook.robot) | `Kubernetes`, `AKS`,
-`EKS`, `GKE`, `OpenShift`, `CertManager` | `Get Namespace Certificate Summary`,
-`Find Failed Certificate Requests and Identify Issues` | This taskset checks
-that your cert manager certificates are renewing as expected, raising issues
-when they are past due in the configured namespace [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/k8s-certmanager-healthcheck) | |
-[Kubernetes Daemonset Triage](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/k8s-daemonset-healthcheck/runbook.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get DaemonSet Log Details For
-Report`, `Get Related Daemonset Events`, `Check Daemonset Replicas` | Triages
-issues related to a Daemonset and its available replicas. [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/k8s-daemonset-healthcheck) | |
-[Kubernetes Deployment Triage](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/k8s-deployment-healthcheck/runbook.robot)
-| `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Check Deployment Log For
-Issues`, `Troubleshoot Deployment Warning Events`, `Get Deployment Workload
-Details For Report`, `Troubleshoot Deployment Replicas`, `Check For Deployment
-Event Anomalies` | Triages issues related to a deployment and its replicas.
+`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Workload Logs`, `Scan For
+Misconfigured Environment`, `Troubleshoot Application Logs` | Triages issues
+related to a deployment and its replicas. [Docs](https://docs.runwhen.com/
+public/v/cli-codecollection/k8s-app-troubleshoot) | | [Kubernetes ArgoCD
+Application Health & Troubleshoot](https://github.com/runwhen-contrib/rw-cli-
+codecollection/blob/main/codebundles/k8s-argocd-application-health/
+runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `ArgoCD` |
+`Fetch ArgoCD Application Sync Status & Health`, `Fetch ArgoCD Application Last
+Sync Operation Details`, `Fetch Unhealthy ArgoCD Application Resources`, `Scan
+For Errors in Pod Logs Related to ArgoCD Application Deployments`, `Fully
+Describe ArgoCD Application` | This taskset collects information and runs
+general troubleshooting checks against argocd application objects within a
+namespace. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-
+argocd-application-health) | | [Kubernetes ArgoCD HelmRelease TaskSet](https://
+github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-
+argocd-helm-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`,
+`OpenShift`, `ArgoCD` | `Fetch all available ArgoCD Helm releases`, `Fetch
+Installed ArgoCD Helm release versions` | This codebundle runs a series of
+tasks to identify potential helm release issues related to ArgoCD managed Helm
+objects. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-
+argocd-helm-health) | | [Kubernetes Artifactory Triage](https://github.com/
+runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-artifactory-
+health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`,
+`Artifactory` | `Check Artifactory Liveness and Readiness Endpoints` | Performs
+a triage on the Open Source version of Artifactory in a Kubernetes cluster.
+[Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-artifactory-
+health) | | [Kubernetes CertManager Healthcheck](https://github.com/runwhen-
+contrib/rw-cli-codecollection/blob/main/codebundles/k8s-certmanager-
+healthcheck/sli.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get
+Health Score of CertManager Workloads` | Check the health of pods deployed by
+cert-manager. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-
+certmanager-healthcheck) | | [Kubernetes Daemonset Triage](https://github.com/
+runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-daemonset-
+healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` |
+`Get DaemonSet Log Details For Report`, `Get Related Daemonset Events`, `Check
+Daemonset Replicas` | Triages issues related to a Daemonset and its available
+replicas. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-
+daemonset-healthcheck) | | [Kubernetes Deployment Triage](https://github.com/
+runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-deployment-
+healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` |
+`Check Deployment Log For Issues with `${DEPLOYMENT_NAME}``, `Check Liveness
+Probe Configuration for Deployment `${DEPLOYMENT_NAME}``, `Check Readiness
+Probe Configuration for Deployment `${DEPLOYMENT_NAME}``, `Troubleshoot
+Deployment Warning Events for `${DEPLOYMENT_NAME}``, `Get Deployment Workload
+Details For `${DEPLOYMENT_NAME}` and Add to Report`, `Troubleshoot Deployment
+Replicas for `${DEPLOYMENT_NAME}``, `Check Deployment Event Anomalies for `$
+{DEPLOYMENT_NAME}`` | Triages issues related to a deployment and its replicas.
 [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-deployment-
 healthcheck) | | [Kubernetes Flux Choas Testing](https://github.com/runwhen-
 contrib/rw-cli-codecollection/blob/main/codebundles/k8s-chaos-flux/
 runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Suspend the
 Flux Resource Reconciliation`, `Find Random FluxCD Workload as Chaos Target`,
 `Execute Chaos Command`, `Execute Additional Chaos Command`, `Resume Flux
 Resource Reconciliation` | This taskset is used to suspend a flux resource for
@@ -171,116 +179,126 @@
 health) | | [Kubernetes Grafana Loki Health Check](https://github.com/runwhen-
 contrib/rw-cli-codecollection/blob/main/codebundles/k8s-loki-healthcheck/
 runbook.robot) | `k8s` | `Check Loki Ring API`, `Check Loki API Ready` | This
 taskset checks the health of Grafana Loki and its hash ring. [Docs](https://
 docs.runwhen.com/public/v/cli-codecollection/k8s-loki-healthcheck) | |
 [Kubernetes Image Check](https://github.com/runwhen-contrib/rw-cli-
 codecollection/blob/main/codebundles/k8s-image-check/runbook.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Check Image Rollover Times In
-Namespace`, `List Images and Tags for Every Container in Running Pods`, `List
-Images and Tags for Every Container in Failed Pods`, `List ImagePullBackOff
-Events and Test Path and Tags` | This taskset provides detailed information
-about the images used in a Kubernetes namespace. [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/k8s-image-check) | | [Kubernetes
-Ingress GCE & GCP HTTP Load Balancer Healthcheck](https://github.com/runwhen-
-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-ingress-gce-
-healthcheck/runbook.robot) | `Kubernetes`, `GKE`, `GCE`, `GCP` | `Search For
-GCE Ingress Warnings in GKE`, `Identify Unhealthy GCE HTTP Ingress Backends`,
-`Validate GCP HTTP Load Balancer Configurations`, `Fetch Network Error Logs
-from GCP Operations Manager for Ingress Backends`, `Review GCP Operations
-Logging Dashboard` | Troubleshoot GCE Ingress Resources related to GCP HTTP
-Load Balancer in GKE [Docs](https://docs.runwhen.com/public/v/cli-
+`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Check Image Rollover Times
+for Namespace `${NAMESPACE}``, `List Images and Tags for Every Container in
+Running Pods for Namespace `${NAMESPACE}``, `List Images and Tags for Every
+Container in Failed Pods for Namespace `${NAMESPACE}``, `List ImagePullBackOff
+Events and Test Path and Tags for Namespace `${NAMESPACE}`` | This taskset
+provides detailed information about the images used in a Kubernetes namespace.
+[Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-image-check) |
+| [Kubernetes Ingress GCE & GCP HTTP Load Balancer Healthcheck](https://
+github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-
+ingress-gce-healthcheck/runbook.robot) | `Kubernetes`, `GKE`, `GCE`, `GCP` |
+`Search For GCE Ingress Warnings in GKE`, `Identify Unhealthy GCE HTTP Ingress
+Backends`, `Validate GCP HTTP Load Balancer Configurations`, `Fetch Network
+Error Logs from GCP Operations Manager for Ingress Backends`, `Review GCP
+Operations Logging Dashboard` | Troubleshoot GCE Ingress Resources related to
+GCP HTTP Load Balancer in GKE [Docs](https://docs.runwhen.com/public/v/cli-
 codecollection/k8s-ingress-gce-healthcheck) | | [Kubernetes Ingress
 Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/
 main/codebundles/k8s-ingress-healthcheck/runbook.robot) | `Kubernetes`, `AKS`,
-`EKS`, `GKE`, `OpenShift` | `Fetch Ingress Object Health in Namespace` |
-Triages issues related to a ingress objects and services. [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/k8s-ingress-healthcheck) | |
-[Kubernetes Jenkins Healthcheck](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/k8s-jenkins-healthcheck/runbook.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Jenkins` | `Query The Jenkins
-Kubernetes Workload HTTP Endpoint`, `Query For Stuck Jenkins Jobs` | This
-taskset collects information about perstistent volumes and persistent volume
-claims to validate health or help troubleshoot potential issues. [Docs](https:/
-/docs.runwhen.com/public/v/cli-codecollection/k8s-jenkins-healthcheck) | |
-[Kubernetes Labeled Pod Count](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/k8s-labeledpods-healthcheck/sli.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Measure Number of Running
-Pods with Label` | This codebundle fetches the number of running pods with the
-set of provided labels, letting you measure the number of running pods. [Docs]
-(https://docs.runwhen.com/public/v/cli-codecollection/k8s-labeledpods-
-healthcheck) | | [Kubernetes Namespace Healthcheck](https://github.com/runwhen-
-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-namespace-healthcheck/
-sli.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Event Count
-and Score`, `Get Container Restarts and Score`, `Get NotReady Pods`, `Generate
-Namspace Score` | This SLI uses kubectl to score namespace health. Produces a
-value between 0 (completely failing thet test) and 1 (fully passing the test).
-Looks for container restarts, events, and pods not ready. [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/k8s-namespace-healthcheck) | |
-[Kubernetes Namespace Troubleshoot](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/k8s-namespace-healthcheck/runbook.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Trace And Troubleshoot
-Namespace Warning Events And Errors`, `Troubleshoot Container Restarts In
-Namespace`, `Troubleshoot Pending Pods In Namespace`, `Troubleshoot Failed Pods
-In Namespace`, `Troubleshoot Workload Status Conditions In Namespace`, `Get
-Listing Of Resources In Namespace`, `Check For Namespace Event Anomalies`,
-`Troubleshoot Namespace Services And Application Workloads`, `Check Missing or
-Risky PodDisruptionBudget Policies` | This taskset runs general troubleshooting
-checks against all applicable objects in a namespace, checks error events, and
-searches pod logs for error entries. [Docs](https://docs.runwhen.com/public/v/
-cli-codecollection/k8s-namespace-healthcheck) | | [Kubernetes Persistent Volume
+`EKS`, `GKE`, `OpenShift` | `Fetch Ingress Object Health in Namespace `$
+{NAMESPACE}``, `Check for Ingress and Service Conflicts in Namespace `$
+{NAMESPACE}`` | Triages issues related to a ingress objects and services.
+[Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-ingress-
+healthcheck) | | [Kubernetes Jenkins Healthcheck](https://github.com/runwhen-
+contrib/rw-cli-codecollection/blob/main/codebundles/k8s-jenkins-healthcheck/
+runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Jenkins` |
+`Query The Jenkins Kubernetes Workload HTTP Endpoint`, `Query For Stuck Jenkins
+Jobs` | This taskset collects information about perstistent volumes and
+persistent volume claims to validate health or help troubleshoot potential
+issues. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/k8s-
+jenkins-healthcheck) | | [Kubernetes Labeled Pod Count](https://github.com/
+runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-labeledpods-
+healthcheck/sli.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` |
+`Measure Number of Running Pods with Label` | This codebundle fetches the
+number of running pods with the set of provided labels, letting you measure the
+number of running pods. [Docs](https://docs.runwhen.com/public/v/cli-
+codecollection/k8s-labeledpods-healthcheck) | | [Kubernetes Namespace
 Healthcheck](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/
-main/codebundles/k8s-pvc-healthcheck/runbook.robot) | `Kubernetes`, `AKS`,
-`EKS`, `GKE`, `OpenShift` | `Fetch Events for Unhealthy Kubernetes
-PersistentVolumeClaims`, `List PersistentVolumeClaims in Terminating State`,
-`List PersistentVolumes in Terminating State`, `List Pods with Attached Volumes
-and Related PersistentVolume Details`, `Fetch the Storage Utilization for PVC
-Mounts`, `Check for RWO Persistent Volume Node Attachment Issues` | This
-taskset collects information about storage such as PersistentVolumes and
-PersistentVolumeClaims to validate health or help troubleshoot potential
-storage issues. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/
-k8s-pvc-healthcheck) | | [Kubernetes Pod Resources Scan](https://github.com/
-runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-podresources-
-health/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Scan
-Labeled Pods and Show All Containers Without Resource Limit or Resource
-Requests Set`, `Get Labeled Container Top Info` | Inspects the resources
-provisioned for a given set of pods, selected by their labels and raises issues
-if no resources were specified. [Docs](https://docs.runwhen.com/public/v/cli-
-codecollection/k8s-podresources-health) | | [Kubernetes Postgres Triage](https:
-//github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-
-postgres-triage/runbook.robot) | `AKS`, `EKS`, `GKE`, `Kubernetes`, `Patroni`,
+main/codebundles/k8s-namespace-healthcheck/sli.robot) | `Kubernetes`, `AKS`,
+`EKS`, `GKE`, `OpenShift` | `Get Event Count and Score`, `Get Container
+Restarts and Score`, `Get NotReady Pods`, `Generate Namspace Score` | This SLI
+uses kubectl to score namespace health. Produces a value between 0 (completely
+failing thet test) and 1 (fully passing the test). Looks for container
+restarts, events, and pods not ready. [Docs](https://docs.runwhen.com/public/v/
+cli-codecollection/k8s-namespace-healthcheck) | | [Kubernetes Namespace
+Troubleshoot](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/
+main/codebundles/k8s-namespace-healthcheck/runbook.robot) | `Kubernetes`,
+`AKS`, `EKS`, `GKE`, `OpenShift` | `Troubleshoot Warning Events in Namespace `$
+{NAMESPACE}``, `Troubleshoot Container Restarts In Namespace `${NAMESPACE}``,
+`Troubleshoot Pending Pods In Namespace `${NAMESPACE}``, `Troubleshoot Failed
+Pods In Namespace `${NAMESPACE}``, `Troubleshoot Workload Status Conditions In
+Namespace `${NAMESPACE}``, `Get Listing Of Resources In Namespace `$
+{NAMESPACE}``, `Check Event Anomalies in Namespace `${NAMESPACE}``,
+`Troubleshoot Services And Application Workloads in Namespace `${NAMESPACE}``,
+`Check Missing or Risky PodDisruptionBudget Policies in Namepace `$
+{NAMESPACE}`` | This taskset runs general troubleshooting checks against all
+applicable objects in a namespace. Looks for warning events, odd or frequent
+normal events, restarting containers and failed or pending pods. [Docs](https:/
+/docs.runwhen.com/public/v/cli-codecollection/k8s-namespace-healthcheck) | |
+[Kubernetes Persistent Volume Healthcheck](https://github.com/runwhen-contrib/
+rw-cli-codecollection/blob/main/codebundles/k8s-pvc-healthcheck/runbook.robot)
+| `Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Fetch Events for Unhealthy
+Kubernetes PersistentVolumeClaims in Namespace `${NAMESPACE}``, `List
+PersistentVolumeClaims in Terminating State in Namespace `${NAMESPACE}``, `List
+PersistentVolumes in Terminating State in Namespace `${NAMESPACE}``, `List Pods
+with Attached Volumes and Related PersistentVolume Details in Namespace `$
+{NAMESPACE}``, `Fetch the Storage Utilization for PVC Mounts in Namespace `$
+{NAMESPACE}``, `Check for RWO Persistent Volume Node Attachment Issues in
+Namespace `${NAMESPACE}`` | This taskset collects information about storage
+such as PersistentVolumes and PersistentVolumeClaims to validate health or help
+troubleshoot potential storage issues. [Docs](https://docs.runwhen.com/public/
+v/cli-codecollection/k8s-pvc-healthcheck) | | [Kubernetes Pod Resources Scan]
+(https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
+codebundles/k8s-podresources-health/runbook.robot) | `Kubernetes`, `AKS`,
+`EKS`, `GKE`, `OpenShift` | `Show Pods Without Resource Limit or Resource
+Requests Set in Namespace `${NAMESPACE}``, `Get Pod Resource Utilization with
+Top in Namespace `${NAMESPACE}`` | Inspects the resources provisioned for a
+given set of pods, selected by their labels and raises issues if no resources
+were specified. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/
+k8s-podresources-health) | | [Kubernetes Postgres Triage](https://github.com/
+runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-postgres-
+triage/runbook.robot) | `AKS`, `EKS`, `GKE`, `Kubernetes`, `Patroni`,
 `Postgres` | `Get Standard Postgres Resource Information`, `Describe Postgres
 Custom Resources`, `Get Postgres Pod Logs & Events`, `Get Postgres Pod Resource
 Utilization`, `Get Running Postgres Configuration`, `Get Patroni Output`, `Run
 DB Queries` | Runs multiple Kubernetes and psql commands to report on the
 health of a postgres cluster. [Docs](https://docs.runwhen.com/public/v/cli-
 codecollection/k8s-postgres-triage) | | [Kubernetes Redis Healthcheck](https://
 github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-
 redis-healthcheck/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`,
-`OpenShift`, `Redis` | `Ping Redis Workload`, `Verify Redis Read Write
-Operation` | This taskset collects information on your redis workload in your
-Kubernetes cluster and raises issues if any health checks fail. [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/k8s-redis-healthcheck) | |
-[Kubernetes Restart resource](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/k8s-restart-resource/runbook.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Get Current Resource State`,
-`Get Resource Logs`, `Restart Resource` | This taskset restarts a resource with
-a given set of labels, typically used with other tasksets. [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/k8s-restart-resource) | |
-[Kubernetes Service Account Check](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/k8s-serviceaccount-check/runbook.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift`, `Redis` | `Test Service Account
-Access to Kubernetes API Server` | This taskset provides tasks to troubleshoot
-service accounts in a Kubernetes namespace. [Docs](https://docs.runwhen.com/
-public/v/cli-codecollection/k8s-serviceaccount-check) | | [Kubernetes
-StatefulSet Triage](https://github.com/runwhen-contrib/rw-cli-codecollection/
-blob/main/codebundles/k8s-statefulset-healthcheck/runbook.robot) |
-`Kubernetes`, `AKS`, `EKS`, `GKE`, `OpenShift` | `Fetch StatefulSet Logs`, `Get
-Related StatefulSet Events`, `Fetch StatefulSet Manifest Details`, `List
-StatefulSets with Unhealthy Replica Counts` | Triages issues related to a
+`OpenShift`, `Redis` | `Ping `${DEPLOYMENT_NAME}` Redis Workload`, `Verify `$
+{DEPLOYMENT_NAME}` Redis Read Write Operation` | This taskset collects
+information on your redis workload in your Kubernetes cluster and raises issues
+if any health checks fail. [Docs](https://docs.runwhen.com/public/v/cli-
+codecollection/k8s-redis-healthcheck) | | [Kubernetes Restart resource](https:/
+/github.com/runwhen-contrib/rw-cli-codecollection/blob/main/codebundles/k8s-
+restart-resource/runbook.robot) | `Kubernetes`, `AKS`, `EKS`, `GKE`,
+`OpenShift` | `Get Current Resource State`, `Get Resource Logs`, `Restart
+Resource` | This taskset restarts a resource with a given set of labels,
+typically used with other tasksets. [Docs](https://docs.runwhen.com/public/v/
+cli-codecollection/k8s-restart-resource) | | [Kubernetes Service Account Check]
+(https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
+codebundles/k8s-serviceaccount-check/runbook.robot) | `Kubernetes`, `AKS`,
+`EKS`, `GKE`, `OpenShift`, `Redis` | `Test Service Account Access to Kubernetes
+API Server` | This taskset provides tasks to troubleshoot service accounts in a
+Kubernetes namespace. [Docs](https://docs.runwhen.com/public/v/cli-
+codecollection/k8s-serviceaccount-check) | | [Kubernetes StatefulSet Triage]
+(https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
+codebundles/k8s-statefulset-healthcheck/runbook.robot) | `Kubernetes`, `AKS`,
+`EKS`, `GKE`, `OpenShift` | `Fetch StatefulSet `${STATEFULSET_NAME}` Logs`,
+`Get Related StatefulSet `${STATEFULSET_NAME}` Events`, `Fetch StatefulSet `$
+{STATEFULSET_NAME}` Manifest Details`, `List StatefulSets with Unhealthy
+Replica Counts In Namespace `${NAMESPACE}`` | Triages issues related to a
 StatefulSet and its replicas. [Docs](https://docs.runwhen.com/public/v/cli-
 codecollection/k8s-statefulset-healthcheck) | | [Kubernetes Vault Triage]
 (https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
 codebundles/k8s-vault-healthcheck/runbook.robot) | `AKS`, `EKS`, `GKE`,
 `Kubernetes`, `Vault` | `Fetch Vault CSI Driver Logs`, `Get Vault CSI Driver
 Warning Events`, `Check Vault CSI Driver Replicas`, `Fetch Vault Logs`, `Get
 Related Vault Events`, `Fetch Vault StatefulSet Manifest Details`, `Fetch Vault
@@ -294,21 +312,21 @@
 | Check whether the Terraform Cloud Workspace is in a locked state. [Docs]
 (https://docs.runwhen.com/public/v/cli-codecollection/terraform-cloud-
 workspace-lock-check) | | [Test Issues](https://github.com/runwhen-contrib/rw-
 cli-codecollection/blob/main/codebundles/test-issue/runbook.robot) | `Test` |
 `Raise Full Issue` | A codebundle for testing the issues feature. Purely for
 testing flow. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/test-
 issue) | | [cURL HTTP OK](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/curl-http-ok/runbook.robot) | `Linux macOS
+codecollection/blob/main/codebundles/curl-http-ok/sli.robot) | `Linux macOS
 Windows HTTP` | `Checking HTTP URL Is Available And Timely` | This taskset uses
-curl to validate the response code of the endpoint and provides the total time
-of the request. [Docs](https://docs.runwhen.com/public/v/cli-codecollection/
-curl-http-ok) | | [cli-test-taskset](https://github.com/runwhen-contrib/rw-cli-
-codecollection/blob/main/codebundles/cli-test/runbook.robot) | `cli` | `Run CLI
-and Parse Output For Issues`, `Exec Test`, `Local Process Test` | This taskset
-smoketests the CLI codebundle setup and run process [Docs](https://
-docs.runwhen.com/public/v/cli-codecollection/cli-test) | | [cmd-test-taskset]
-(https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
+curl to validate the response code of the endpoint. Returns ascore of 1 if
+healthy, an 0 if unhealthy. [Docs](https://docs.runwhen.com/public/v/cli-
+codecollection/curl-http-ok) | | [cli-test-taskset](https://github.com/runwhen-
+contrib/rw-cli-codecollection/blob/main/codebundles/cli-test/runbook.robot) |
+`cli` | `Run CLI and Parse Output For Issues`, `Exec Test`, `Local Process
+Test` | This taskset smoketests the CLI codebundle setup and run process [Docs]
+(https://docs.runwhen.com/public/v/cli-codecollection/cli-test) | | [cmd-test-
+taskset](https://github.com/runwhen-contrib/rw-cli-codecollection/blob/main/
 codebundles/cmd-test/runbook.robot) | `cmd` | `Run CLI Command`, `Run Bash
 File`, `Log Suggestion` | This taskset smoketests the CLI codebundle setup and
 run process by running a bare command [Docs](https://docs.runwhen.com/public/v/
 cli-codecollection/cmd-test) |
```

### Comparing `runwhen-cli-keywords-0.0.8/runwhen_cli_keywords.egg-info/SOURCES.txt` & `runwhen-cli-keywords-0.0.9/runwhen_cli_keywords.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `runwhen-cli-keywords-0.0.8/setup.py` & `runwhen-cli-keywords-0.0.9/setup.py`

 * *Files identical despite different names*

