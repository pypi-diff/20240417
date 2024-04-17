# Comparing `tmp/awsibox-0.8.9.tar.gz` & `tmp/awsibox-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsibox-0.8.9.tar", last modified: Fri Jul 14 09:59:16 2023, max compression
+gzip compressed data, was "awsibox-0.9.1.tar", last modified: Wed Apr 17 10:19:19 2024, max compression
```

## Comparing `awsibox-0.8.9.tar` & `awsibox-0.9.1.tar`

### file list

```diff
@@ -1,290 +1,290 @@
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.235693 awsibox-0.8.9/
--rw-r--r--   0 mello     (1000) mello     (1000)      771 2020-01-23 17:57:57.000000 awsibox-0.8.9/.gitignore
--rw-r--r--   0 mello     (1000) mello     (1000)    10297 2022-03-14 08:29:15.000000 awsibox-0.8.9/LICENSE
--rw-r--r--   0 mello     (1000) mello     (1000)      257 2023-06-16 08:09:06.000000 awsibox-0.8.9/MANIFEST.in
--rw-r--r--   0 mello     (1000) mello     (1000)      877 2023-07-14 09:59:16.235693 awsibox-0.8.9/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)      373 2022-03-14 08:29:15.000000 awsibox-0.8.9/README.md
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.051690 awsibox-0.8.9/awsibox/
--rw-r--r--   0 mello     (1000) mello     (1000)    19454 2023-07-08 15:37:21.000000 awsibox-0.8.9/awsibox/RP.py
--rw-r--r--   0 mello     (1000) mello     (1000)       39 2023-07-14 09:58:45.000000 awsibox-0.8.9/awsibox/__init__.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2251 2022-07-01 08:39:37.000000 awsibox-0.8.9/awsibox/args.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.051690 awsibox-0.8.9/awsibox/aws/
--rw-r--r--   0 mello     (1000) mello     (1000)  7094944 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/aws/CloudFormationResourceSpecification.json
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.015689 awsibox-0.8.9/awsibox/cfg/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.031690 awsibox-0.8.9/awsibox/cfg/ibox/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.099691 awsibox-0.8.9/awsibox/cfg/ibox/com/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.107691 awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/
--rw-r--r--   0 mello     (1000) mello     (1000)     5580 2023-07-13 13:05:17.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/autoscalinggroup-elasticloadbalancing.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      534 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/capacity.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      459 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/cloudwatch-agent.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1252 2023-06-16 09:13:11.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1357 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1303 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2303 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2934 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2206 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.107691 awsibox-0.8.9/awsibox/cfg/ibox/com/certificatemanager/
--rw-r--r--   0 mello     (1000) mello     (1000)     1222 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.111691 awsibox-0.8.9/awsibox/cfg/ibox/com/cloudfront/
--rw-r--r--   0 mello     (1000) mello     (1000)     1481 2023-07-06 14:25:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1656 2023-07-03 12:08:45.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/cloudfront/for-services.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      197 2023-07-06 10:29:30.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/cloudfront/i_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      495 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/cloudfront/origin-adhoc.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.111691 awsibox-0.8.9/awsibox/cfg/ibox/com/codedeploy/
--rw-r--r--   0 mello     (1000) mello     (1000)      190 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/codedeploy/deployment-group.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2002 2023-07-13 20:06:15.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/common.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.111691 awsibox-0.8.9/awsibox/cfg/ibox/com/dynamodb/
--rw-r--r--   0 mello     (1000) mello     (1000)      579 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.115691 awsibox-0.8.9/awsibox/cfg/ibox/com/ec2/
--rw-r--r--   0 mello     (1000) mello     (1000)     1975 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/ec2/bottlerocket.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      265 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/ec2/securitygroup.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      672 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.119691 awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/
--rw-r--r--   0 mello     (1000) mello     (1000)     2452 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/capacityprovider.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1435 2023-07-11 11:57:43.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1369 2023-07-13 09:22:24.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/fargate-spot.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3201 2023-07-13 12:23:53.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      905 2023-07-13 13:05:23.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     5739 2023-07-03 14:54:45.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      734 2023-07-13 13:05:29.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/task.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      399 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/taskdefinition-volume.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.119691 awsibox-0.8.9/awsibox/cfg/ibox/com/efs/
--rw-r--r--   0 mello     (1000) mello     (1000)      378 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/efs/accesspoint-app.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.123691 awsibox-0.8.9/awsibox/cfg/ibox/com/elasticloadbalancing/
--rw-r--r--   0 mello     (1000) mello     (1000)     1287 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2246 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1945 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      242 2023-06-14 15:18:04.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/elasticloadbalancing/i_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      201 2023-06-14 16:13:04.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/elasticloadbalancing/loadbalancer.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      194 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/elasticloadbalancing/v2-listener.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.131691 awsibox-0.8.9/awsibox/cfg/ibox/com/events/
--rw-r--r--   0 mello     (1000) mello     (1000)     2890 2023-07-13 13:04:45.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1340 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/events/cluster-autoscale.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     6911 2023-07-13 13:05:02.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/events/ec2.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1581 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2584 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/events/ecs-spot.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1568 2023-07-13 13:04:53.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/events/ecs.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1201 2023-07-13 13:05:09.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/events/spot_advisor.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.131691 awsibox-0.8.9/awsibox/cfg/ibox/com/iam/
--rw-r--r--   0 mello     (1000) mello     (1000)     5020 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/iam/managed-policies.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      435 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/iam/policy-ecs-exec.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      938 2023-07-13 13:05:44.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2115 2023-05-18 13:24:47.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/iam/policy-update_stack.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1591 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1939 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/iam/roles.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.135691 awsibox-0.8.9/awsibox/cfg/ibox/com/kms/
--rw-r--r--   0 mello     (1000) mello     (1000)      684 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.139691 awsibox-0.8.9/awsibox/cfg/ibox/com/lambda/
--rw-r--r--   0 mello     (1000) mello     (1000)      607 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3732 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1393 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml
--rw-r--r--   0 mello     (1000) mello     (1000)       46 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/lambda/layers.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      935 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/lambda/py-packager.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1204 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/lambda/service-unavailable.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.139691 awsibox-0.8.9/awsibox/cfg/ibox/com/route53/
--rw-r--r--   0 mello     (1000) mello     (1000)      428 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/route53/resolverendpoint-outbound.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.139691 awsibox-0.8.9/awsibox/cfg/ibox/com/s3/
--rw-r--r--   0 mello     (1000) mello     (1000)      566 2023-07-07 19:35:03.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/s3/bucket-log.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.139691 awsibox-0.8.9/awsibox/cfg/ibox/com/servicediscovery/
--rw-r--r--   0 mello     (1000) mello     (1000)      374 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/servicediscovery/publicdnsnamespace-find.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.143691 awsibox-0.8.9/awsibox/cfg/ibox/com/sns/
--rw-r--r--   0 mello     (1000) mello     (1000)      950 2023-07-13 13:05:35.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      225 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/sns/cloudwatch-alarm.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.143691 awsibox-0.8.9/awsibox/cfg/ibox/com/ssm/
--rw-r--r--   0 mello     (1000) mello     (1000)      312 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/com/ssm/parameter-user-password.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.031690 awsibox-0.8.9/awsibox/cfg/ibox/res/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.147691 awsibox-0.8.9/awsibox/cfg/ibox/res/apigateway/
--rw-r--r--   0 mello     (1000) mello     (1000)      146 2023-07-13 13:10:32.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/apigateway/accounts.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      250 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/apigateway/deployments.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      491 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/apigateway/domain-names.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1821 2023-06-14 15:29:04.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/apigateway/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.147691 awsibox-0.8.9/awsibox/cfg/ibox/res/application-autoscaling/
--rw-r--r--   0 mello     (1000) mello     (1000)      832 2023-06-14 15:40:34.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2925 2023-07-13 13:15:35.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2143 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.151691 awsibox-0.8.9/awsibox/cfg/ibox/res/autoscaling/
--rw-r--r--   0 mello     (1000) mello     (1000)     2401 2023-07-13 13:08:29.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3163 2023-06-14 15:45:28.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     5129 2023-07-13 12:23:49.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1889 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.151691 awsibox-0.8.9/awsibox/cfg/ibox/res/certificatemanager/
--rw-r--r--   0 mello     (1000) mello     (1000)      222 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/certificatemanager/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.151691 awsibox-0.8.9/awsibox/cfg/ibox/res/cloudformation/
--rw-r--r--   0 mello     (1000) mello     (1000)      706 2023-07-13 13:10:28.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/cloudformation/custom-resources.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      528 2023-07-13 21:39:37.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/cloudformation/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.155691 awsibox-0.8.9/awsibox/cfg/ibox/res/cloudfront/
--rw-r--r--   0 mello     (1000) mello     (1000)     5910 2023-07-07 08:35:38.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      504 2023-07-06 09:46:36.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/cloudfront/origin-access-controls.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     5958 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/cloudfront/policies.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.155691 awsibox-0.8.9/awsibox/cfg/ibox/res/cloudwatch/
--rw-r--r--   0 mello     (1000) mello     (1000)     7798 2023-07-13 13:11:33.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/cloudwatch/alarms.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1041 2023-06-14 15:57:15.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/cloudwatch/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      966 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.159691 awsibox-0.8.9/awsibox/cfg/ibox/res/codedeploy/
--rw-r--r--   0 mello     (1000) mello     (1000)      364 2023-06-14 16:02:37.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/codedeploy/deployment-groups.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1076 2023-07-13 13:15:55.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.163691 awsibox-0.8.9/awsibox/cfg/ibox/res/ec2/
--rw-r--r--   0 mello     (1000) mello     (1000)      602 2023-07-13 13:07:25.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/ec2/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1794 2023-07-04 07:39:01.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/ec2/securitygroupingresses.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      346 2023-06-29 13:36:52.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/ec2/securitygroups.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      438 2023-07-10 13:10:42.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/ec2/subnet-routetable-associations.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1245 2023-07-10 13:15:14.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/ec2/subnets.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      118 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/ec2/vpc-endpoints.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.163691 awsibox-0.8.9/awsibox/cfg/ibox/res/ecr/
--rw-r--r--   0 mello     (1000) mello     (1000)     1405 2023-06-29 14:55:24.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/ecr/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.163691 awsibox-0.8.9/awsibox/cfg/ibox/res/ecs/
--rw-r--r--   0 mello     (1000) mello     (1000)    10167 2023-07-13 15:52:54.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/ecs/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1964 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/ecs/services.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1020 2023-07-13 13:08:36.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/ecs/taskdefinitions.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.167692 awsibox-0.8.9/awsibox/cfg/ibox/res/efs/
--rw-r--r--   0 mello     (1000) mello     (1000)       68 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/efs/filesystems.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1961 2023-07-03 12:08:45.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/efs/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.167692 awsibox-0.8.9/awsibox/cfg/ibox/res/elasticache/
--rw-r--r--   0 mello     (1000) mello     (1000)     5325 2023-07-13 13:07:56.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/elasticache/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)       69 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/elasticache/subnet-groups.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.171692 awsibox-0.8.9/awsibox/cfg/ibox/res/elasticloadbalancing/
--rw-r--r--   0 mello     (1000) mello     (1000)     3978 2023-07-03 13:48:39.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1002 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     5049 2023-07-04 07:33:41.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listeners.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2828 2023-07-13 13:10:06.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3613 2023-07-13 13:10:19.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.171692 awsibox-0.8.9/awsibox/cfg/ibox/res/events/
--rw-r--r--   0 mello     (1000) mello     (1000)     1860 2023-07-13 13:07:34.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/events/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.175692 awsibox-0.8.9/awsibox/cfg/ibox/res/iam/
--rw-r--r--   0 mello     (1000) mello     (1000)     3064 2023-07-04 13:41:29.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/iam/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      143 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/iam/instance-profiles.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3686 2023-07-13 13:10:37.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/iam/managed-policies.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1716 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/iam/policies.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      918 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/iam/roles.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.175692 awsibox-0.8.9/awsibox/cfg/ibox/res/lambda/
--rw-r--r--   0 mello     (1000) mello     (1000)     1286 2023-07-03 12:08:45.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/lambda/functions.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2591 2023-06-14 16:23:01.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/lambda/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      213 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/lambda/layer_permissions.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      938 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/lambda/permissions.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      586 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/lambda/versions.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.175692 awsibox-0.8.9/awsibox/cfg/ibox/res/rds/
--rw-r--r--   0 mello     (1000) mello     (1000)      576 2023-07-04 15:47:10.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/rds/db-parameter_groups.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      393 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/rds/db-subnet-groups.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     9059 2023-07-13 13:09:53.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/rds/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.179692 awsibox-0.8.9/awsibox/cfg/ibox/res/route53/
--rw-r--r--   0 mello     (1000) mello     (1000)     1426 2023-07-13 13:07:50.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/route53/hostedzones.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      410 2023-06-14 15:15:46.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/route53/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     7294 2023-07-13 13:07:43.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/route53/recordsets.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.179692 awsibox-0.8.9/awsibox/cfg/ibox/res/s3/
--rw-r--r--   0 mello     (1000) mello     (1000)       41 2023-07-05 12:35:38.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/s3/bucket-policies.yml
--rw-r--r--   0 mello     (1000) mello     (1000)    12432 2023-07-11 12:34:02.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/s3/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.179692 awsibox-0.8.9/awsibox/cfg/ibox/res/scheduler/
--rw-r--r--   0 mello     (1000) mello     (1000)     1574 2023-07-13 13:08:03.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/scheduler/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.183692 awsibox-0.8.9/awsibox/cfg/ibox/res/sns/
--rw-r--r--   0 mello     (1000) mello     (1000)      449 2023-06-14 16:29:21.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/sns/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      719 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/sns/subscriptions.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.183692 awsibox-0.8.9/awsibox/cfg/ibox/res/sqs/
--rw-r--r--   0 mello     (1000) mello     (1000)      467 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/sqs/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      978 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/sqs/queue-policies.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.183692 awsibox-0.8.9/awsibox/cfg/ibox/res/ssm/
--rw-r--r--   0 mello     (1000) mello     (1000)       57 2023-07-13 15:07:21.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/ssm/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      227 2023-07-13 15:48:42.000000 awsibox-0.8.9/awsibox/cfg/ibox/res/ssm/parameters.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.035689 awsibox-0.8.9/awsibox/cfg/ibox/stacks/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.183692 awsibox-0.8.9/awsibox/cfg/ibox/stacks/agw/
--rw-r--r--   0 mello     (1000) mello     (1000)     1690 2023-06-14 15:29:08.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/agw/i_type.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2612 2023-04-27 10:02:55.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/agw/infra-info.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.187692 awsibox-0.8.9/awsibox/cfg/ibox/stacks/cch/
--rw-r--r--   0 mello     (1000) mello     (1000)      280 2023-06-14 15:24:02.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/cch/i_type.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.187692 awsibox-0.8.9/awsibox/cfg/ibox/stacks/clf/
--rw-r--r--   0 mello     (1000) mello     (1000)       89 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/clf/i_type.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.187692 awsibox-0.8.9/awsibox/cfg/ibox/stacks/ec2/
--rw-r--r--   0 mello     (1000) mello     (1000)     4605 2023-07-13 13:06:47.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3590 2023-07-13 13:06:56.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/ec2/i_type.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.187692 awsibox-0.8.9/awsibox/cfg/ibox/stacks/ecs/
--rw-r--r--   0 mello     (1000) mello     (1000)      839 2023-06-15 07:56:29.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/ecs/buildkite.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2399 2023-07-11 12:06:08.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/ecs/i_type.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      690 2023-06-15 07:55:51.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.191692 awsibox-0.8.9/awsibox/cfg/ibox/stacks/lbd/
--rw-r--r--   0 mello     (1000) mello     (1000)     1289 2023-07-13 13:07:11.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.191692 awsibox-0.8.9/awsibox/cfg/ibox/stacks/rds/
--rw-r--r--   0 mello     (1000) mello     (1000)      241 2023-07-04 15:47:16.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/rds/i_type.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.199692 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/
--rw-r--r--   0 mello     (1000) mello     (1000)      633 2023-06-15 07:57:04.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1542 2023-07-13 13:07:03.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      794 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3497 2023-06-14 15:55:04.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      139 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-event-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      559 2023-06-16 09:17:19.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-extra-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      749 2023-07-04 10:04:47.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     4645 2023-06-14 16:16:30.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      108 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-iam-user-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      655 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)       29 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-s3-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     4070 2023-07-10 13:18:33.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/vpc.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.199692 awsibox-0.8.9/awsibox/cfg/ibox/stacks/tsk/
--rw-r--r--   0 mello     (1000) mello     (1000)     2890 2023-07-13 13:06:26.000000 awsibox-0.8.9/awsibox/cfg/ibox/stacks/tsk/i_type.yml
--rw-r--r--   0 mello     (1000) mello     (1000)    17392 2023-07-13 20:36:17.000000 awsibox-0.8.9/awsibox/cfg.py
--rw-r--r--   0 mello     (1000) mello     (1000)     6633 2023-07-13 20:39:31.000000 awsibox-0.8.9/awsibox/common.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1867 2023-04-27 09:19:18.000000 awsibox-0.8.9/awsibox/discover.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2315 2023-07-05 16:08:18.000000 awsibox-0.8.9/awsibox/generate.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.219692 awsibox-0.8.9/awsibox/lambdas/
--rw-r--r--   0 mello     (1000) mello     (1000)     1687 2022-03-14 08:29:15.000000 awsibox-0.8.9/awsibox/lambdas/ASGSpot.code
--rw-r--r--   0 mello     (1000) mello     (1000)      812 2022-03-14 08:29:15.000000 awsibox-0.8.9/awsibox/lambdas/AtEdgeAddHeaders.code
--rw-r--r--   0 mello     (1000) mello     (1000)     4305 2023-07-11 08:26:15.000000 awsibox-0.8.9/awsibox/lambdas/CCRFargateSpot.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2759 2022-11-22 10:02:17.000000 awsibox-0.8.9/awsibox/lambdas/CCRLightHouse.code
--rw-r--r--   0 mello     (1000) mello     (1000)     3916 2023-04-11 07:35:07.000000 awsibox-0.8.9/awsibox/lambdas/CCRStackReplicator.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2115 2022-11-22 13:27:14.000000 awsibox-0.8.9/awsibox/lambdas/CloudWatchAlarmStateChange.code
--rw-r--r--   0 mello     (1000) mello     (1000)     1675 2022-11-22 13:26:46.000000 awsibox-0.8.9/awsibox/lambdas/CloudWatchRepeatedNotify.code
--rw-r--r--   0 mello     (1000) mello     (1000)      739 2022-03-14 08:29:15.000000 awsibox-0.8.9/awsibox/lambdas/EC2StartStopTagged.code
--rwxr-xr-x   0 mello     (1000) mello     (1000)     6507 2022-11-30 10:37:32.000000 awsibox-0.8.9/awsibox/lambdas/ECSClusterAutoscale.code
--rw-r--r--   0 mello     (1000) mello     (1000)     6697 2022-11-29 16:18:45.000000 awsibox-0.8.9/awsibox/lambdas/ECSDrainInstance.code
--rw-r--r--   0 mello     (1000) mello     (1000)     7111 2023-04-17 15:59:09.000000 awsibox-0.8.9/awsibox/lambdas/ECSDrainTasks.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2899 2022-11-22 15:41:37.000000 awsibox-0.8.9/awsibox/lambdas/ECSEventTaskStateChange.code
--rw-r--r--   0 mello     (1000) mello     (1000)     4193 2023-04-12 09:41:12.000000 awsibox-0.8.9/awsibox/lambdas/ECSEventsSpot.code
--rw-r--r--   0 mello     (1000) mello     (1000)     6177 2023-04-12 10:46:40.000000 awsibox-0.8.9/awsibox/lambdas/ECSRaiseASGAlarm.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2792 2022-11-30 13:18:45.000000 awsibox-0.8.9/awsibox/lambdas/ECSRunTask.code
--rw-r--r--   0 mello     (1000) mello     (1000)      987 2022-03-14 08:29:15.000000 awsibox-0.8.9/awsibox/lambdas/ECSUpdateDesiredCount.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2167 2022-03-14 08:29:15.000000 awsibox-0.8.9/awsibox/lambdas/ElasticSearchSnapShot.code
--rwxr-xr-x   0 mello     (1000) mello     (1000)     5370 2023-06-07 12:49:30.000000 awsibox-0.8.9/awsibox/lambdas/InfraInfo.code
--rw-r--r--   0 mello     (1000) mello     (1000)     1267 2022-04-23 16:11:28.000000 awsibox-0.8.9/awsibox/lambdas/ManageService.code
--rw-r--r--   0 mello     (1000) mello     (1000)      547 2022-03-14 08:29:15.000000 awsibox-0.8.9/awsibox/lambdas/PaidApi.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2724 2023-04-07 09:45:45.000000 awsibox-0.8.9/awsibox/lambdas/PyPackager.code
--rw-r--r--   0 mello     (1000) mello     (1000)      844 2022-03-14 08:29:15.000000 awsibox-0.8.9/awsibox/lambdas/Python37SSM.layer
--rw-r--r--   0 mello     (1000) mello     (1000)     3826 2022-11-30 13:32:53.000000 awsibox-0.8.9/awsibox/lambdas/R53RecordInstanceId.code
--rw-r--r--   0 mello     (1000) mello     (1000)     4360 2022-11-30 14:07:17.000000 awsibox-0.8.9/awsibox/lambdas/ServiceDiscovery.code
--rw-r--r--   0 mello     (1000) mello     (1000)      890 2022-11-30 13:39:06.000000 awsibox-0.8.9/awsibox/lambdas/ServiceUnavailable.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2589 2023-05-18 20:19:14.000000 awsibox-0.8.9/awsibox/lambdas/StacksOps.code
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.223692 awsibox-0.8.9/awsibox/mod/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.227692 awsibox-0.8.9/awsibox/mod/__pycache__/
--rw-r--r--   0 mello     (1000) mello     (1000)     5503 2023-07-10 12:23:40.000000 awsibox-0.8.9/awsibox/mod/__pycache__/autoscaling.cpython-311.pyc
--rw-r--r--   0 mello     (1000) mello     (1000)     6051 2023-07-03 12:05:44.000000 awsibox-0.8.9/awsibox/mod/__pycache__/cloudformation.cpython-311.pyc
--rw-r--r--   0 mello     (1000) mello     (1000)     3330 2023-07-10 12:23:40.000000 awsibox-0.8.9/awsibox/mod/__pycache__/cloudfront.cpython-311.pyc
--rw-r--r--   0 mello     (1000) mello     (1000)    17996 2023-07-10 12:23:40.000000 awsibox-0.8.9/awsibox/mod/__pycache__/ec2.cpython-311.pyc
--rw-r--r--   0 mello     (1000) mello     (1000)     6211 2023-07-03 12:05:44.000000 awsibox-0.8.9/awsibox/mod/__pycache__/elasticloadbalancing.cpython-311.pyc
--rw-r--r--   0 mello     (1000) mello     (1000)     4581 2023-07-03 12:05:44.000000 awsibox-0.8.9/awsibox/mod/__pycache__/iam.cpython-311.pyc
--rw-r--r--   0 mello     (1000) mello     (1000)     3491 2023-07-10 12:23:40.000000 awsibox-0.8.9/awsibox/mod/__pycache__/joker.cpython-311.pyc
--rw-r--r--   0 mello     (1000) mello     (1000)     6017 2023-07-03 12:05:44.000000 awsibox-0.8.9/awsibox/mod/__pycache__/rds.cpython-311.pyc
--rw-r--r--   0 mello     (1000) mello     (1000)     3068 2023-07-03 12:05:44.000000 awsibox-0.8.9/awsibox/mod/__pycache__/s3.cpython-311.pyc
--rw-r--r--   0 mello     (1000) mello     (1000)    14961 2023-07-03 12:05:44.000000 awsibox-0.8.9/awsibox/mod/__pycache__/waf.cpython-311.pyc
--rw-r--r--   0 mello     (1000) mello     (1000)     3685 2023-07-13 20:39:15.000000 awsibox-0.8.9/awsibox/mod/autoscaling.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3557 2023-07-13 20:39:15.000000 awsibox-0.8.9/awsibox/mod/cloudformation.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1941 2023-07-08 12:36:18.000000 awsibox-0.8.9/awsibox/mod/cloudfront.py
--rw-r--r--   0 mello     (1000) mello     (1000)     9160 2023-07-13 19:22:10.000000 awsibox-0.8.9/awsibox/mod/ec2.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3076 2023-07-13 19:22:00.000000 awsibox-0.8.9/awsibox/mod/joker.py
--rw-r--r--   0 mello     (1000) mello     (1000)    45364 2023-07-14 09:57:33.000000 awsibox-0.8.9/awsibox/shared.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.231692 awsibox-0.8.9/awsibox/user-data/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.235693 awsibox-0.8.9/awsibox/user-data/SCRIPTS/
--rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-02 14:06:20.000000 awsibox-0.8.9/awsibox/user-data/SCRIPTS/ELBCHECK.sh
--rw-r--r--   0 mello     (1000) mello     (1000)      685 2023-02-28 14:52:11.000000 awsibox-0.8.9/awsibox/user-data/SCRIPTS/END.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     1467 2023-01-03 11:25:14.000000 awsibox-0.8.9/awsibox/user-data/SCRIPTS/INIT.sh
--rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-05 16:57:15.000000 awsibox-0.8.9/awsibox/user-data/SCRIPTS/PACKAGE.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     1184 2023-01-02 14:06:20.000000 awsibox-0.8.9/awsibox/user-data/SCRIPTS/SERVICE.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     1771 2023-01-03 16:26:40.000000 awsibox-0.8.9/awsibox/user-data/SCRIPTS/SETUP.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     2521 2023-01-03 11:24:26.000000 awsibox-0.8.9/awsibox/user-data/ecs-cluster.sh
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.015689 awsibox-0.8.9/build/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.015689 awsibox-0.8.9/build/lib/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.043690 awsibox-0.8.9/build/lib/awsibox.egg-info/
--rw-r--r--   0 mello     (1000) mello     (1000)      877 2023-07-14 09:59:15.000000 awsibox-0.8.9/build/lib/awsibox.egg-info/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)     9546 2023-07-14 09:59:15.000000 awsibox-0.8.9/build/lib/awsibox.egg-info/SOURCES.txt
--rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-07-14 09:59:15.000000 awsibox-0.8.9/build/lib/awsibox.egg-info/dependency_links.txt
--rw-r--r--   0 mello     (1000) mello     (1000)       44 2023-07-14 09:59:15.000000 awsibox-0.8.9/build/lib/awsibox.egg-info/requires.txt
--rw-r--r--   0 mello     (1000) mello     (1000)        8 2023-07-14 09:59:15.000000 awsibox-0.8.9/build/lib/awsibox.egg-info/top_level.txt
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-14 09:59:16.235693 awsibox-0.8.9/scripts/
--rwxr-xr-x   0 mello     (1000) mello     (1000)     3350 2023-06-15 12:57:11.000000 awsibox-0.8.9/scripts/ibox_generate_templates.py
--rw-r--r--   0 mello     (1000) mello     (1000)      556 2023-07-14 09:59:16.239693 awsibox-0.8.9/setup.cfg
--rw-r--r--   0 mello     (1000) mello     (1000)      536 2023-06-16 08:09:19.000000 awsibox-0.8.9/setup.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.405598 awsibox-0.9.1/
+-rw-r--r--   0 mello     (1000) mello     (1000)      771 2020-01-23 17:57:57.000000 awsibox-0.9.1/.gitignore
+-rw-r--r--   0 mello     (1000) mello     (1000)    10297 2022-03-14 08:29:15.000000 awsibox-0.9.1/LICENSE
+-rw-r--r--   0 mello     (1000) mello     (1000)      257 2023-06-16 08:09:06.000000 awsibox-0.9.1/MANIFEST.in
+-rw-r--r--   0 mello     (1000) mello     (1000)      877 2024-04-17 10:19:19.405598 awsibox-0.9.1/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)      373 2022-03-14 08:29:15.000000 awsibox-0.9.1/README.md
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.229596 awsibox-0.9.1/awsibox/
+-rw-r--r--   0 mello     (1000) mello     (1000)    19454 2023-07-08 15:37:21.000000 awsibox-0.9.1/awsibox/RP.py
+-rw-r--r--   0 mello     (1000) mello     (1000)       39 2024-04-17 10:17:31.000000 awsibox-0.9.1/awsibox/__init__.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2251 2022-07-01 08:39:37.000000 awsibox-0.9.1/awsibox/args.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.233596 awsibox-0.9.1/awsibox/aws/
+-rw-r--r--   0 mello     (1000) mello     (1000)  7094944 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/aws/CloudFormationResourceSpecification.json
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.193596 awsibox-0.9.1/awsibox/cfg/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.213596 awsibox-0.9.1/awsibox/cfg/ibox/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.265597 awsibox-0.9.1/awsibox/cfg/ibox/com/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.273597 awsibox-0.9.1/awsibox/cfg/ibox/com/autoscaling/
+-rw-r--r--   0 mello     (1000) mello     (1000)     5580 2023-07-13 13:05:17.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/autoscaling/autoscalinggroup-elasticloadbalancing.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      534 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/autoscaling/capacity.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      459 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/autoscaling/cloudwatch-agent.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1252 2023-06-16 09:13:11.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1357 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1303 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2303 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2934 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2206 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.273597 awsibox-0.9.1/awsibox/cfg/ibox/com/certificatemanager/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1222 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.277597 awsibox-0.9.1/awsibox/cfg/ibox/com/cloudfront/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1481 2023-07-06 14:25:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1656 2024-01-22 10:45:00.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/cloudfront/for-services.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      197 2023-07-06 10:29:30.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/cloudfront/i_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      495 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/cloudfront/origin-adhoc.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.281597 awsibox-0.9.1/awsibox/cfg/ibox/com/codedeploy/
+-rw-r--r--   0 mello     (1000) mello     (1000)      190 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/codedeploy/deployment-group.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2002 2023-07-13 20:06:15.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/common.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.281597 awsibox-0.9.1/awsibox/cfg/ibox/com/dynamodb/
+-rw-r--r--   0 mello     (1000) mello     (1000)      579 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.285597 awsibox-0.9.1/awsibox/cfg/ibox/com/ec2/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1975 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/ec2/bottlerocket.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      265 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/ec2/securitygroup.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      672 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.289597 awsibox-0.9.1/awsibox/cfg/ibox/com/ecs/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2452 2024-03-05 10:53:53.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/ecs/capacityprovider.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1435 2023-07-11 11:57:43.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1369 2023-07-13 09:22:24.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/ecs/fargate-spot.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3201 2023-07-13 12:23:53.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1332 2023-12-13 09:07:40.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     5739 2023-07-03 14:54:45.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      734 2023-07-13 13:05:29.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/ecs/task.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      399 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/ecs/taskdefinition-volume.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.293597 awsibox-0.9.1/awsibox/cfg/ibox/com/efs/
+-rw-r--r--   0 mello     (1000) mello     (1000)      378 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/efs/accesspoint-app.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.297597 awsibox-0.9.1/awsibox/cfg/ibox/com/elasticloadbalancing/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1287 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2246 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1945 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      242 2023-06-14 15:18:04.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/elasticloadbalancing/i_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      201 2023-06-14 16:13:04.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/elasticloadbalancing/loadbalancer.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      194 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/elasticloadbalancing/v2-listener.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.301597 awsibox-0.9.1/awsibox/cfg/ibox/com/events/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2890 2023-07-13 13:04:45.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1340 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/events/cluster-autoscale.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     6911 2023-07-13 13:05:02.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/events/ec2.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1581 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2584 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/events/ecs-spot.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1568 2024-01-12 11:29:27.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/events/ecs.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1201 2023-07-13 13:05:09.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/events/spot_advisor.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.305597 awsibox-0.9.1/awsibox/cfg/ibox/com/iam/
+-rw-r--r--   0 mello     (1000) mello     (1000)     5020 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/iam/managed-policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      435 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/iam/policy-ecs-exec.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      938 2023-07-13 13:05:44.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2115 2023-05-18 13:24:47.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/iam/policy-update_stack.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1591 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2026 2023-11-08 23:03:24.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/iam/roles.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.305597 awsibox-0.9.1/awsibox/cfg/ibox/com/kms/
+-rw-r--r--   0 mello     (1000) mello     (1000)      684 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.309597 awsibox-0.9.1/awsibox/cfg/ibox/com/lambda/
+-rw-r--r--   0 mello     (1000) mello     (1000)      607 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3732 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1393 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)       46 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/lambda/layers.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      935 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/lambda/py-packager.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1204 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/lambda/service-unavailable.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.309597 awsibox-0.9.1/awsibox/cfg/ibox/com/route53/
+-rw-r--r--   0 mello     (1000) mello     (1000)      428 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/route53/resolverendpoint-outbound.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.309597 awsibox-0.9.1/awsibox/cfg/ibox/com/s3/
+-rw-r--r--   0 mello     (1000) mello     (1000)      566 2023-07-07 19:35:03.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/s3/bucket-log.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.313597 awsibox-0.9.1/awsibox/cfg/ibox/com/servicediscovery/
+-rw-r--r--   0 mello     (1000) mello     (1000)      374 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/servicediscovery/publicdnsnamespace-find.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.313597 awsibox-0.9.1/awsibox/cfg/ibox/com/sns/
+-rw-r--r--   0 mello     (1000) mello     (1000)      950 2023-07-13 13:05:35.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1269 2024-01-12 13:29:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/sns/cloudwatch-alarm.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.313597 awsibox-0.9.1/awsibox/cfg/ibox/com/ssm/
+-rw-r--r--   0 mello     (1000) mello     (1000)      312 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/com/ssm/parameter-user-password.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.213596 awsibox-0.9.1/awsibox/cfg/ibox/res/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.317597 awsibox-0.9.1/awsibox/cfg/ibox/res/apigateway/
+-rw-r--r--   0 mello     (1000) mello     (1000)      146 2023-07-13 13:10:32.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/apigateway/accounts.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      250 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/apigateway/deployments.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      491 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/apigateway/domain-names.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1821 2023-06-14 15:29:04.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/apigateway/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.317597 awsibox-0.9.1/awsibox/cfg/ibox/res/application-autoscaling/
+-rw-r--r--   0 mello     (1000) mello     (1000)      832 2023-06-14 15:40:34.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2925 2023-07-13 13:15:35.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2143 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.321597 awsibox-0.9.1/awsibox/cfg/ibox/res/autoscaling/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2401 2023-07-13 13:08:29.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3163 2023-06-14 15:45:28.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     5129 2023-07-13 12:23:49.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1889 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.321597 awsibox-0.9.1/awsibox/cfg/ibox/res/certificatemanager/
+-rw-r--r--   0 mello     (1000) mello     (1000)      222 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/certificatemanager/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.321597 awsibox-0.9.1/awsibox/cfg/ibox/res/cloudformation/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1312 2023-07-14 13:31:19.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/cloudformation/custom-resources.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      528 2023-07-13 21:39:37.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/cloudformation/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.325597 awsibox-0.9.1/awsibox/cfg/ibox/res/cloudfront/
+-rw-r--r--   0 mello     (1000) mello     (1000)     5910 2024-01-30 13:59:58.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      504 2023-07-06 09:46:36.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/cloudfront/origin-access-controls.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     5958 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/cloudfront/policies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.325597 awsibox-0.9.1/awsibox/cfg/ibox/res/cloudwatch/
+-rw-r--r--   0 mello     (1000) mello     (1000)     7713 2023-08-02 08:10:05.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/cloudwatch/alarms.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      778 2023-08-02 08:33:22.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/cloudwatch/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      966 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.325597 awsibox-0.9.1/awsibox/cfg/ibox/res/codedeploy/
+-rw-r--r--   0 mello     (1000) mello     (1000)      364 2023-06-14 16:02:37.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/codedeploy/deployment-groups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1076 2023-07-13 13:15:55.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.329597 awsibox-0.9.1/awsibox/cfg/ibox/res/ec2/
+-rw-r--r--   0 mello     (1000) mello     (1000)      602 2023-07-13 13:07:25.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/ec2/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1794 2023-07-04 07:39:01.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/ec2/securitygroupingresses.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      346 2023-06-29 13:36:52.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/ec2/securitygroups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      438 2023-07-10 13:10:42.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/ec2/subnet-routetable-associations.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1245 2023-07-10 13:15:14.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/ec2/subnets.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      118 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/ec2/vpc-endpoints.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.329597 awsibox-0.9.1/awsibox/cfg/ibox/res/ecr/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1545 2024-02-22 09:58:13.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/ecr/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.333598 awsibox-0.9.1/awsibox/cfg/ibox/res/ecs/
+-rw-r--r--   0 mello     (1000) mello     (1000)    10167 2023-07-13 15:52:54.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/ecs/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2547 2023-11-23 14:32:10.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/ecs/services.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1020 2023-07-13 13:08:36.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/ecs/taskdefinitions.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.333598 awsibox-0.9.1/awsibox/cfg/ibox/res/efs/
+-rw-r--r--   0 mello     (1000) mello     (1000)       68 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/efs/filesystems.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1961 2023-07-03 12:08:45.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/efs/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.333598 awsibox-0.9.1/awsibox/cfg/ibox/res/elasticache/
+-rw-r--r--   0 mello     (1000) mello     (1000)     5325 2023-07-13 13:07:56.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/elasticache/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)       69 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/elasticache/subnet-groups.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.337597 awsibox-0.9.1/awsibox/cfg/ibox/res/elasticloadbalancing/
+-rw-r--r--   0 mello     (1000) mello     (1000)     3978 2023-07-03 13:48:39.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1002 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     5049 2023-11-06 13:49:58.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listeners.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2828 2023-07-13 13:10:06.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3613 2023-07-13 13:10:19.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.341598 awsibox-0.9.1/awsibox/cfg/ibox/res/events/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1860 2023-07-13 13:07:34.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/events/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.341598 awsibox-0.9.1/awsibox/cfg/ibox/res/iam/
+-rw-r--r--   0 mello     (1000) mello     (1000)     3064 2023-07-04 13:41:29.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/iam/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      143 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/iam/instance-profiles.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3686 2023-07-13 13:10:37.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/iam/managed-policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1716 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/iam/policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      918 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/iam/roles.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.345598 awsibox-0.9.1/awsibox/cfg/ibox/res/lambda/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1286 2023-07-03 12:08:45.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/lambda/functions.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2687 2024-02-26 13:27:57.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/lambda/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      213 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/lambda/layer_permissions.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      938 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/lambda/permissions.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      586 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/lambda/versions.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.349598 awsibox-0.9.1/awsibox/cfg/ibox/res/rds/
+-rw-r--r--   0 mello     (1000) mello     (1000)      576 2023-07-04 15:47:10.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/rds/db-parameter_groups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      393 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/rds/db-subnet-groups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     8446 2024-03-25 10:05:13.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/rds/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.349598 awsibox-0.9.1/awsibox/cfg/ibox/res/route53/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1426 2023-07-13 13:07:50.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/route53/hostedzones.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      410 2023-06-14 15:15:46.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/route53/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     7294 2023-07-13 13:07:43.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/route53/recordsets.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.349598 awsibox-0.9.1/awsibox/cfg/ibox/res/s3/
+-rw-r--r--   0 mello     (1000) mello     (1000)       41 2023-07-05 12:35:38.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/s3/bucket-policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)    12432 2023-07-11 12:34:02.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/s3/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.349598 awsibox-0.9.1/awsibox/cfg/ibox/res/scheduler/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1574 2023-11-08 11:37:57.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/scheduler/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.353598 awsibox-0.9.1/awsibox/cfg/ibox/res/sns/
+-rw-r--r--   0 mello     (1000) mello     (1000)      557 2024-01-12 13:23:24.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/sns/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      719 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/sns/subscriptions.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.353598 awsibox-0.9.1/awsibox/cfg/ibox/res/sqs/
+-rw-r--r--   0 mello     (1000) mello     (1000)      467 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/sqs/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      978 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/sqs/queue-policies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.353598 awsibox-0.9.1/awsibox/cfg/ibox/res/ssm/
+-rw-r--r--   0 mello     (1000) mello     (1000)       57 2023-07-13 15:07:21.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/ssm/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      227 2023-07-13 15:48:42.000000 awsibox-0.9.1/awsibox/cfg/ibox/res/ssm/parameters.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.213596 awsibox-0.9.1/awsibox/cfg/ibox/stacks/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.357598 awsibox-0.9.1/awsibox/cfg/ibox/stacks/agw/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1690 2023-06-14 15:29:08.000000 awsibox-0.9.1/awsibox/cfg/ibox/stacks/agw/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2651 2023-10-16 13:27:19.000000 awsibox-0.9.1/awsibox/cfg/ibox/stacks/agw/infra-info.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.357598 awsibox-0.9.1/awsibox/cfg/ibox/stacks/cch/
+-rw-r--r--   0 mello     (1000) mello     (1000)      280 2023-06-14 15:24:02.000000 awsibox-0.9.1/awsibox/cfg/ibox/stacks/cch/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.357598 awsibox-0.9.1/awsibox/cfg/ibox/stacks/clf/
+-rw-r--r--   0 mello     (1000) mello     (1000)       89 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/stacks/clf/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.357598 awsibox-0.9.1/awsibox/cfg/ibox/stacks/ec2/
+-rw-r--r--   0 mello     (1000) mello     (1000)     4876 2024-03-22 08:55:44.000000 awsibox-0.9.1/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3590 2023-07-13 13:06:56.000000 awsibox-0.9.1/awsibox/cfg/ibox/stacks/ec2/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.361598 awsibox-0.9.1/awsibox/cfg/ibox/stacks/ecs/
+-rw-r--r--   0 mello     (1000) mello     (1000)      865 2024-01-05 09:10:25.000000 awsibox-0.9.1/awsibox/cfg/ibox/stacks/ecs/buildkite.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2399 2023-07-11 12:06:08.000000 awsibox-0.9.1/awsibox/cfg/ibox/stacks/ecs/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      690 2023-06-15 07:55:51.000000 awsibox-0.9.1/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.361598 awsibox-0.9.1/awsibox/cfg/ibox/stacks/lbd/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1289 2023-07-13 13:07:11.000000 awsibox-0.9.1/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.361598 awsibox-0.9.1/awsibox/cfg/ibox/stacks/rds/
+-rw-r--r--   0 mello     (1000) mello     (1000)      241 2023-07-04 15:47:16.000000 awsibox-0.9.1/awsibox/cfg/ibox/stacks/rds/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.369598 awsibox-0.9.1/awsibox/cfg/ibox/stacks/res/
+-rw-r--r--   0 mello     (1000) mello     (1000)      633 2023-06-15 07:57:04.000000 awsibox-0.9.1/awsibox/cfg/ibox/stacks/res/res-base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1542 2023-07-13 13:07:03.000000 awsibox-0.9.1/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      794 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3497 2023-06-14 15:55:04.000000 awsibox-0.9.1/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      139 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/stacks/res/res-event-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      559 2023-06-16 09:17:19.000000 awsibox-0.9.1/awsibox/cfg/ibox/stacks/res/res-extra-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      749 2023-07-04 10:04:47.000000 awsibox-0.9.1/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     4645 2023-06-14 16:16:30.000000 awsibox-0.9.1/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      108 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/stacks/res/res-iam-user-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      655 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)       29 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/cfg/ibox/stacks/res/res-s3-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     4070 2023-07-10 13:18:33.000000 awsibox-0.9.1/awsibox/cfg/ibox/stacks/res/vpc.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.373598 awsibox-0.9.1/awsibox/cfg/ibox/stacks/tsk/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2890 2023-07-13 13:06:26.000000 awsibox-0.9.1/awsibox/cfg/ibox/stacks/tsk/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)    18297 2024-03-25 10:14:01.000000 awsibox-0.9.1/awsibox/cfg.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     6633 2023-07-13 20:39:31.000000 awsibox-0.9.1/awsibox/common.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1867 2023-04-27 09:19:18.000000 awsibox-0.9.1/awsibox/discover.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2315 2023-07-05 16:08:18.000000 awsibox-0.9.1/awsibox/generate.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.389598 awsibox-0.9.1/awsibox/lambdas/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1687 2022-03-14 08:29:15.000000 awsibox-0.9.1/awsibox/lambdas/ASGSpot.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      812 2022-03-14 08:29:15.000000 awsibox-0.9.1/awsibox/lambdas/AtEdgeAddHeaders.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     4305 2023-07-11 08:26:15.000000 awsibox-0.9.1/awsibox/lambdas/CCRFargateSpot.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2759 2022-11-22 10:02:17.000000 awsibox-0.9.1/awsibox/lambdas/CCRLightHouse.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     3940 2023-07-14 13:39:39.000000 awsibox-0.9.1/awsibox/lambdas/CCRStackReplicator.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2115 2022-11-22 13:27:14.000000 awsibox-0.9.1/awsibox/lambdas/CloudWatchAlarmStateChange.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     1675 2022-11-22 13:26:46.000000 awsibox-0.9.1/awsibox/lambdas/CloudWatchRepeatedNotify.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      739 2022-03-14 08:29:15.000000 awsibox-0.9.1/awsibox/lambdas/EC2StartStopTagged.code
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     6507 2022-11-30 10:37:32.000000 awsibox-0.9.1/awsibox/lambdas/ECSClusterAutoscale.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     6844 2023-10-30 12:49:45.000000 awsibox-0.9.1/awsibox/lambdas/ECSDrainInstance.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     7111 2023-04-17 15:59:09.000000 awsibox-0.9.1/awsibox/lambdas/ECSDrainTasks.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2899 2022-11-22 15:41:37.000000 awsibox-0.9.1/awsibox/lambdas/ECSEventTaskStateChange.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     4193 2023-04-12 09:41:12.000000 awsibox-0.9.1/awsibox/lambdas/ECSEventsSpot.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     6177 2023-04-12 10:46:40.000000 awsibox-0.9.1/awsibox/lambdas/ECSRaiseASGAlarm.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2792 2023-11-08 21:46:32.000000 awsibox-0.9.1/awsibox/lambdas/ECSRunTask.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      987 2022-03-14 08:29:15.000000 awsibox-0.9.1/awsibox/lambdas/ECSUpdateDesiredCount.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2167 2022-03-14 08:29:15.000000 awsibox-0.9.1/awsibox/lambdas/ElasticSearchSnapShot.code
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     8028 2023-10-17 07:47:06.000000 awsibox-0.9.1/awsibox/lambdas/InfraInfo.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     1267 2022-04-23 16:11:28.000000 awsibox-0.9.1/awsibox/lambdas/ManageService.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      547 2022-03-14 08:29:15.000000 awsibox-0.9.1/awsibox/lambdas/PaidApi.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2724 2023-04-07 09:45:45.000000 awsibox-0.9.1/awsibox/lambdas/PyPackager.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     1322 2023-09-19 09:26:06.000000 awsibox-0.9.1/awsibox/lambdas/Python37SSM.layer
+-rw-r--r--   0 mello     (1000) mello     (1000)     3826 2022-11-30 13:32:53.000000 awsibox-0.9.1/awsibox/lambdas/R53RecordInstanceId.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     4360 2022-11-30 14:07:17.000000 awsibox-0.9.1/awsibox/lambdas/ServiceDiscovery.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      890 2022-11-30 13:39:06.000000 awsibox-0.9.1/awsibox/lambdas/ServiceUnavailable.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2589 2023-05-18 20:19:14.000000 awsibox-0.9.1/awsibox/lambdas/StacksOps.code
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.393598 awsibox-0.9.1/awsibox/mod/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.401598 awsibox-0.9.1/awsibox/mod/__pycache__/
+-rw-r--r--   0 mello     (1000) mello     (1000)     5174 2023-11-21 14:12:23.000000 awsibox-0.9.1/awsibox/mod/__pycache__/autoscaling.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)     4318 2023-11-21 14:12:23.000000 awsibox-0.9.1/awsibox/mod/__pycache__/cloudformation.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)     3330 2023-07-10 12:23:40.000000 awsibox-0.9.1/awsibox/mod/__pycache__/cloudfront.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)    10536 2023-11-21 14:12:23.000000 awsibox-0.9.1/awsibox/mod/__pycache__/ec2.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)     6211 2023-07-03 12:05:44.000000 awsibox-0.9.1/awsibox/mod/__pycache__/elasticloadbalancing.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)     4581 2023-07-03 12:05:44.000000 awsibox-0.9.1/awsibox/mod/__pycache__/iam.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)     3844 2023-11-21 14:12:23.000000 awsibox-0.9.1/awsibox/mod/__pycache__/joker.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)     6017 2023-07-03 12:05:44.000000 awsibox-0.9.1/awsibox/mod/__pycache__/rds.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)     3068 2023-07-03 12:05:44.000000 awsibox-0.9.1/awsibox/mod/__pycache__/s3.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)    14961 2023-07-03 12:05:44.000000 awsibox-0.9.1/awsibox/mod/__pycache__/waf.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)     3685 2023-07-13 20:39:15.000000 awsibox-0.9.1/awsibox/mod/autoscaling.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2707 2023-07-14 13:32:19.000000 awsibox-0.9.1/awsibox/mod/cloudformation.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1941 2023-07-08 12:36:18.000000 awsibox-0.9.1/awsibox/mod/cloudfront.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     9160 2023-07-13 19:22:10.000000 awsibox-0.9.1/awsibox/mod/ec2.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3346 2024-01-12 13:25:50.000000 awsibox-0.9.1/awsibox/mod/joker.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    46089 2024-02-22 16:56:38.000000 awsibox-0.9.1/awsibox/shared.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.401598 awsibox-0.9.1/awsibox/user-data/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.405598 awsibox-0.9.1/awsibox/user-data/SCRIPTS/
+-rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-02 14:06:20.000000 awsibox-0.9.1/awsibox/user-data/SCRIPTS/ELBCHECK.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)      685 2023-02-28 14:52:11.000000 awsibox-0.9.1/awsibox/user-data/SCRIPTS/END.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     1467 2023-01-03 11:25:14.000000 awsibox-0.9.1/awsibox/user-data/SCRIPTS/INIT.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-05 16:57:15.000000 awsibox-0.9.1/awsibox/user-data/SCRIPTS/PACKAGE.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     1184 2023-01-02 14:06:20.000000 awsibox-0.9.1/awsibox/user-data/SCRIPTS/SERVICE.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     1771 2023-01-03 16:26:40.000000 awsibox-0.9.1/awsibox/user-data/SCRIPTS/SETUP.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     2521 2023-01-03 11:24:26.000000 awsibox-0.9.1/awsibox/user-data/ecs-cluster.sh
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.193596 awsibox-0.9.1/build/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.193596 awsibox-0.9.1/build/lib/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.225596 awsibox-0.9.1/build/lib/awsibox.egg-info/
+-rw-r--r--   0 mello     (1000) mello     (1000)      877 2024-04-17 10:19:18.000000 awsibox-0.9.1/build/lib/awsibox.egg-info/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)     9546 2024-04-17 10:19:18.000000 awsibox-0.9.1/build/lib/awsibox.egg-info/SOURCES.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)        1 2024-04-17 10:19:18.000000 awsibox-0.9.1/build/lib/awsibox.egg-info/dependency_links.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)       44 2024-04-17 10:19:18.000000 awsibox-0.9.1/build/lib/awsibox.egg-info/requires.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)        8 2024-04-17 10:19:18.000000 awsibox-0.9.1/build/lib/awsibox.egg-info/top_level.txt
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2024-04-17 10:19:19.405598 awsibox-0.9.1/scripts/
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     3350 2023-06-15 12:57:11.000000 awsibox-0.9.1/scripts/ibox_generate_templates.py
+-rw-r--r--   0 mello     (1000) mello     (1000)      556 2024-04-17 10:19:19.405598 awsibox-0.9.1/setup.cfg
+-rw-r--r--   0 mello     (1000) mello     (1000)      536 2023-06-16 08:09:19.000000 awsibox-0.9.1/setup.py
```

### Comparing `awsibox-0.8.9/.gitignore` & `awsibox-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/LICENSE` & `awsibox-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/PKG-INFO` & `awsibox-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsibox
-Version: 0.8.9
+Version: 0.9.1
 Summary: AWS Infrastructure in a Box
 Home-page: https://github.com/mello7tre/AwsIBox
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Open Software License 3.0 (OSL-3.0)
```

### Comparing `awsibox-0.8.9/awsibox/RP.py` & `awsibox-0.9.1/awsibox/RP.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/args.py` & `awsibox-0.9.1/awsibox/args.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/aws/CloudFormationResourceSpecification.json` & `awsibox-0.9.1/awsibox/aws/CloudFormationResourceSpecification.json`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/autoscalinggroup-elasticloadbalancing.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/autoscaling/autoscalinggroup-elasticloadbalancing.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/capacity.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/autoscaling/capacity.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/cloudfront/for-services.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/cloudfront/for-services.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/common.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/common.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/ec2/bottlerocket.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/ec2/bottlerocket.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/capacityprovider.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/ecs/capacityprovider.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/fargate-spot.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/ecs/fargate-spot.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml`

 * *Files 13% similar despite different names*

```diff
@@ -20,12 +20,19 @@
   ECSService:
     - Base:
         IBOX_OUTPUT:
           - ECSRunTaskClusterName:
               Value: ${Cluster}
           - ECSRunTaskSubnetsPrivate:
               Value: ImportValue("SubnetsPrivate")
+          - ECSRunTaskSecurityGroups:
+              Condition: ECSTaskDefinitionBaseNetworkModeStandard
+              # ugly trick to remove SecurityGroupEcsService from SecurityGroups
+              Value: >-
+                Sub(
+                  ",".join(cfg.Outputs['SecurityGroups'].Value.data["Fn::Sub"][0].split(",")[1:]),
+                  dict(list(cfg.Outputs['SecurityGroups'].Value.data["Fn::Sub"][1].items())[1:]))
   ECSTaskDefinition:
     - Fargate:
         IBOX_ENABLED: True
         Cpu: '1024'
         Memory: '2048'
```

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/ecs/task.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/ecs/task.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/events/cluster-autoscale.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/events/cluster-autoscale.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/events/ec2.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/events/ec2.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/events/ecs-spot.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/events/ecs-spot.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/events/ecs.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/events/ecs.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/events/spot_advisor.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/events/spot_advisor.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/iam/managed-policies.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/iam/managed-policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/iam/policy-update_stack.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/iam/policy-update_stack.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/iam/roles.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/iam/roles.yml`

 * *Files 5% similar despite different names*

```diff
@@ -44,8 +44,9 @@
         Export: True
         AssumeRolePolicyDocument:
           Statement:
             - 1:
                 Condition: {"StringEquals": {"aws:SourceAccount": Ref("AWS::AccountId")}}
         ManagedPolicyArns:
           - 'arn:aws:iam::aws:policy/service-role/AWSLambdaRole'
+          - 'arn:aws:iam::aws:policy/service-role/AmazonEC2ContainerServiceEventsRole'
         Principal: scheduler.amazonaws.com
```

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/lambda/py-packager.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/lambda/py-packager.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/lambda/service-unavailable.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/lambda/service-unavailable.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/s3/bucket-log.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/s3/bucket-log.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/apigateway/ibox_base.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/apigateway/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/cloudformation/ibox_base.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/cloudformation/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
           ViewerCertificate:
             AcmCertificateArn: If(f'{IBOX_RESNAME}AcmCertificate', get_endvalue('GlobalCertificateArn'), Ref('AWS::NoValue'))
             CloudFrontDefaultCertificate: If(f'{IBOX_RESNAME}AcmCertificate', Ref('AWS::NoValue'), True)
             SslSupportMethod: If(f'{IBOX_RESNAME}AcmCertificate', 'sni-only', Ref('AWS::NoValue'))
             MinimumProtocolVersion.IBOX_CODE: If(f'{IBOX_RESNAME}AcmCertificate', get_endvalue(IBOX_CURNAME), Ref('AWS::NoValue'))
             MinimumProtocolVersion.IBOX_AUTO_PO:
               Description: 'The minimum SSL/TLS protocol and ciphers that CloudFront can use to communicate with viewers'
-            MinimumProtocolVersion: TLSv1.2_2018
+            MinimumProtocolVersion: TLSv1.2_2019
           WebACLId.IBOX_CODE: get_endvalue(IBOX_CURNAME, condition=True)
           WebACLId.IBOX_AUTO_PO:
             Description: 'CloudFront WebACLId - empty for default based on env/role'
             CONDITION: get_condition('', 'not_equals', 'none', IBOX_CURNAME)
             Value: ${WebACLId}
           WebACLId: none
         LogEnabled.IBOX_AUTO_PO:
```

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/cloudfront/policies.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/cloudfront/policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/cloudwatch/alarms.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/cloudwatch/alarms.yml`

 * *Files 2% similar despite different names*

```diff
@@ -229,15 +229,14 @@
         Namespace: 'CWAgent'
         Statistic: 'Maximum'
         Threshold: '80'
         Unit: Percent
     - SQSQueueDeadLetter:
         IBOX_PARAMETER:
           - _Threshold:
-              AllowedValues: ['', '1', '2', '3', '4', '5', '6', '7', '8', '9', '10']
               AlarmActions: [ImportValue('SNSTopicCloudWatchAlarm')]
         AlarmActions: [ImportValue('SNSTopicCloudWatchAlarm')]
         EvaluationPeriods: 1
         ComparisonOperator: GreaterThanThreshold
         Dimensions:
           - SQSQueue:
               Name: QueueName
```

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/ec2/ibox_base.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/ec2/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/ec2/securitygroupingresses.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/ec2/securitygroupingresses.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/ec2/subnets.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/ec2/subnets.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/ecr/ibox_base.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/ecr/ibox_base.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,15 @@
 global:
+  ECRRegistryPolicy:
+    - IBOX_BASE:
+        PolicyText:
+          Statement:
+            - IBOX_LIST: {}
+          Version: "2012-10-17"
+
   ECRRepository:
     - IBOX_BASE:
         IBOX_TITLE: Repository.IBOX_INDEXNAME
         LifecyclePolicy:
           LifecyclePolicyText:
             rules:
               - IBOX_LIST:
```

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/ecs/ibox_base.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/ecs/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/ecs/taskdefinitions.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/ecs/taskdefinitions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/efs/ibox_base.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/efs/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/elasticache/ibox_base.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/elasticache/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listeners.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listeners.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/events/ibox_base.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/events/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/iam/ibox_base.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/iam/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/iam/managed-policies.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/iam/managed-policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/iam/policies.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/iam/policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/iam/roles.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/iam/roles.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/lambda/functions.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/lambda/functions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/lambda/ibox_base.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/lambda/ibox_base.yml`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         Layers.IBOX_CUSTOM_OBJ:
           IBOX_PARAMETER:
             - _:
                 Description: str(IBOX_RESNAME)
           IBOX_OUTPUT:
             - _:
                 Value: get_endvalue(IBOX_RESNAME)
-          Value: get_endvalue(IBOX_RESNAME)
+          Value: Join(":",["arn:aws:lambda", Ref("AWS::Region"), Ref("AWS::AccountId"), "layer", IBOX_RESNAME, get_endvalue(IBOX_RESNAME)])
         LogGroupCreate: "yes"
         Handler: "index.lambda_handler"
         MemorySize.IBOX_AUTO_PO: {}
         MemorySize: 128
         Role: GetAtt(f"RoleLambda{IBOX_INDEXNAME}", "Arn")
         FunctionName: Sub("${AWS::StackName}-${EnvRole}-%s" % IBOX_INDEXNAME)
         Environment:
```

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/lambda/permissions.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/lambda/permissions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/lambda/versions.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/lambda/versions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/rds/db-parameter_groups.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/rds/db-parameter_groups.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/rds/ibox_base.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/rds/ibox_base.yml`

 * *Files 12% similar despite different names*

```diff
@@ -37,22 +37,15 @@
         IBOX_PARAMETER:
           - IBOX_MAPNAME.AllocatedStorage:
               Description: 'Storage Size in GB - empty for mapped value'
           - IBOX_MAPNAME.MaxAllocatedStorage:
               Description: 'Max Storage Size in GB (Enable Storage Autoscaling)- empty for mapped value - 0 to disable'
           - IBOX_MAPNAME.DBInstanceClass:
               Description: 'Instance Type - empty for mapped value'
-              AllowedValues: [
-                '', 'db.m3.medium', 'db.m3.large', 'db.m3.xlarge', 'db.m3.2xlarge',
-                'db.m4.large', 'db.m4.xlarge', 'db.m4.2xlarge', 'db.m4.4xlarge', 'db.m4.10xlarge',
-                'db.m5.large', 'db.m5.xlarge', 'db.m5.2xlarge', 'db.m5.4xlarge', 'db.m5.12xlarge',
-                'db.r3.large', 'db.r3.xlarge', 'db.r3.2xlarge', 'db.r3.4xlarge', 'db.r3.8xlarge',
-                'db.r5.large', 'db.r5.xlarge', 'db.r5.2xlarge', 'db.r5.4xlarge', 'db.r5.12xlarge',
-                'db.t2.micro', 'db.t2.small', 'db.t2.medium', 'db.t2.large',
-                'db.t3.micro', 'db.t3.small', 'db.t3.medium', 'db.t3.large']
+              AllowedValues: cfg.INSTANCE_LIST_RDS
           - IBOX_MAPNAME.DBName:
               Description: 'Empty for mapped value'
           - IBOX_MAPNAME.DBSnapshotIdentifier:
               Description: 'DB snapshot used to restore the DB instance - "none" for not using one - empty for mapped value'
           - IBOX_MAPNAME.DeletionProtection:
               Description: 'empty for mapped value'
               AllowedValues: ['', 'true', 'false']
```

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/route53/hostedzones.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/route53/hostedzones.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/route53/recordsets.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/route53/recordsets.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/s3/ibox_base.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/s3/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/scheduler/ibox_base.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/scheduler/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/sns/subscriptions.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/sns/subscriptions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/res/sqs/queue-policies.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/res/sqs/queue-policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/stacks/agw/i_type.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/stacks/agw/i_type.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/stacks/agw/infra-info.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/stacks/agw/infra-info.yml`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,15 @@
             - 1:
                 Action:
                   - 'cloudformation:DescribeStack*'
                   - 'cloudformation:ListStacks'
                   - 'ecs:ListClusters'
                   - 'ecs:ListServices'
                   - 'ecs:DescribeServices'
+                  - 'events:ListRules'
                   - 'application-autoscaling:DescribeScalableTargets'
                 Effect: Allow
                 Resource: '*'
   Lambda:
     - InfraInfov1:
         Architectures:
           - arm64
```

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml`

 * *Files 4% similar despite different names*

```diff
@@ -22,22 +22,26 @@
     - Cluster:
         Value: Ref('Cluster')
         Export: Export(Sub('Cluster-${AWS::StackName}'))
   AutoScalingLifecycleHook:
     - ECSDrainInstance:
         IBOX_TITLE: ASGLifecycleHookECSDrainInstance
         AutoScalingGroupName: Ref('AutoScalingGroup')
-        DefaultResult: 'ABANDON'
+        DefaultResult: CONTINUE
         HeartbeatTimeout.IBOX_AUTO_PO: {}
         HeartbeatTimeout: 3600
         LifecycleTransition: 'autoscaling:EC2_INSTANCE_TERMINATING'
         NotificationTargetARN: ImportValue('SNSTopicECSDrainInstance')
         RoleARN: ImportValue('RoleASGLifecycleHookECSDrainInstance')
   AutoScalingGroup:
     - Base:
+        IBOX_CONDITION:
+          _NewInstancesProtectedFromScaleIn:
+            get_condition('', 'equals', 'ENABLED', f'ECSCapacityProviderBaseAutoScalingGroupProviderManagedTerminationProtection')
+        NewInstancesProtectedFromScaleIn: If(IBOX_CURNAME, True, False)
         Tags:
           - ECSCluster:
               Key: ECSCluster
               Value: Ref('Cluster')
               PropagateAtLaunch: true
   AutoScalingScalingPolicy:
     - Custom:
```

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/stacks/ec2/i_type.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/stacks/ec2/i_type.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/stacks/ecs/buildkite.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/stacks/ecs/buildkite.yml`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,15 @@
       ContainerDefinitions:
       - 1:
           Cpu: 128
           Environment:
           - AWSDEFAULTREGION:
               Name: AWS_DEFAULT_REGION
               Value: Ref('AWS::Region')
+          ImageSuffix: ""
           Memory: 128
           MountPoints:
           - DockerSock:
               ReadOnly: false
               SourceVolume: DockerSock
               ContainerPath: /var/run/docker.sock
```

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/stacks/ecs/i_type.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/stacks/ecs/i_type.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-base.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/stacks/res/res-base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-extra-01.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/stacks/res/res-extra-01.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/stacks/res/vpc.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/stacks/res/vpc.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg/ibox/stacks/tsk/i_type.yml` & `awsibox-0.9.1/awsibox/cfg/ibox/stacks/tsk/i_type.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/cfg.py` & `awsibox-0.9.1/awsibox/cfg.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,15 +79,18 @@
 VPC_DEFAULT_SUBNETS_CIDR_BLOCK_PUBLIC = [
     f"{VPC_DEFAULT_CIDR_BLOCK_PREFIX}.{i + 200}.0/24" for i in range(AZones["MAX"])
 ]
 
 TROPO_CLASS_TO_CFM = {
     "AWS::WAFv2::WebACL": {
         "WebACLRule": "Rule",
-    }
+    },
+    "AWS::ECR::ReplicationConfiguration": {
+        "ReplicationConfigurationProperty": "ReplicationConfiguration"
+    },
 }
 
 EVAL_TROPO_FUNCTIONS_IN_CFG = (
     "Sub(",
     "Ref(",
     "GetAtt(",
     "Split(",
@@ -151,59 +154,66 @@
 ]
 
 INSTANCE_FAMILY = [
     {
         "Name": "t2",
         "Min": "nano",
         "Max": "2xlarge",
+        "RDS": True,
     },
     {
         "Name": "m4",
         "Min": "large",
         "Max": "4xlarge",
+        "RDS": True,
     },
     {
         "Name": "c4",
         "Min": "large",
         "Max": "4xlarge",
     },
     {
         "Name": "r4",
         "Min": "large",
         "Max": "4xlarge",
+        "RDS": True,
     },
     {
         "Name": "t3",
         "Min": "nano",
         "Max": "2xlarge",
+        "RDS": True,
     },
     {
         "Name": "m5",
         "Min": "large",
         "Max": "4xlarge",
+        "RDS": True,
     },
     {
         "Name": "c5",
         "Min": "large",
         "Max": "4xlarge",
     },
     {
         "Name": "r5",
         "Min": "large",
         "Max": "4xlarge",
+        "RDS": True,
     },
     {
         "Name": "t3a",
         "Min": "nano",
         "Max": "2xlarge",
     },
     {
         "Name": "t4g",
         "Min": "nano",
         "Max": "2xlarge",
+        "RDS": True,
     },
     {
         "Name": "m5a",
         "Min": "large",
         "Max": "4xlarge",
     },
     {
@@ -216,24 +226,26 @@
         "Min": "large",
         "Max": "4xlarge",
     },
     {
         "Name": "m6i",
         "Min": "large",
         "Max": "4xlarge",
+        "RDS": True,
     },
     {
         "Name": "c6i",
         "Min": "large",
         "Max": "4xlarge",
     },
     {
         "Name": "r6i",
         "Min": "large",
         "Max": "4xlarge",
+        "RDS": True,
     },
     {
         "Name": "m6a",
         "Min": "large",
         "Max": "4xlarge",
     },
     {
@@ -242,14 +254,20 @@
         "Max": "4xlarge",
     },
     {
         "Name": "c7g",
         "Min": "large",
         "Max": "4xlarge",
     },
+    {
+        "Name": "m7g",
+        "Min": "large",
+        "Max": "4xlarge",
+        "RDS": True,
+    },
 ]
 
 # currently nearly empty as no more used with newer generations instances
 EPHEMERAL_MAP: {
     "InstaceEphemeral0": ["m3.medium", "m3.xlarge"],
     "InstaceEphemeral1": ["m3.xlarge"],
     "InstaceEphemeral2": [""],
@@ -261,31 +279,34 @@
         exec(f.read())
 except FileNotFoundError:
     pass
 
 # build instances list
 def build_instance_list():
     family_instances_list = []
+    family_instances_list_rds = []
     for family in INSTANCE_FAMILY:
         name = family["Name"]
         min_size = INSTANCE_SIZES.index(family["Min"])
         max_size = INSTANCE_SIZES.index(family["Max"])
 
         for s in INSTANCE_SIZES[min_size : max_size + 1]:
             family_instances_list.append(f"{name}.{s}")
+            if family.get("RDS"):
+                family_instances_list_rds.append(f"db.{name}.{s}")
 
-    return family_instances_list
+    return ["default"] + family_instances_list, [""] + family_instances_list_rds
 
 
-INSTANCE_LIST = ["default"] + build_instance_list()
+INSTANCE_LIST, INSTANCE_LIST_RDS = build_instance_list()
 
 # Order is VERY important do not CHANGE it!
 CFG_TO_FUNC = {
     "Parameter": {"module": "joker", "func": (None, "Parameter")},
-    "Condition": {"module": "cloudformation", "func": "CFM_Conditions"},
+    "Condition": {"module": "joker", "func": (None, "Condition")},
     "Mapping": {"module": "cloudformation", "func": "CFM_Mappings"},
     "ApiGatewayAccount": {"module": "joker", "func": ("apigateway", "Account")},
     "ApiGatewayApiKey": {"module": "joker", "func": ("apigateway", "ApiKey")},
     "ApiGatewayBasePathMapping": {
         "module": "joker",
         "func": ("apigateway", "BasePathMapping"),
     },
@@ -315,15 +336,15 @@
     "AutoScalingLifecycleHook": {
         "module": "joker",
         "func": ("autoscaling", "LifecycleHook"),
     },
     "AutoScalingGroup": {
         "module": "autoscaling",
         "func": "AS_Autoscaling",
-        "dep": ["SecurityGroups"],
+        "dep": ["SecurityGroups", "ECSCapacityProvider"],
     },
     "AutoScalingScalingPolicy": {
         "module": "joker",
         "func": ("autoscaling", "ScalingPolicy"),
     },
     "AutoScalingScheduledAction": {
         "module": "joker",
@@ -415,14 +436,19 @@
         "module": "joker",
         "func": ("ec2", "VPCGatewayAttachment"),
     },
     "EC2VPCPeeringConnection": {
         "module": "joker",
         "func": ("ec2", "VPCPeeringConnection"),
     },
+    "ECRRegistryPolicy": {"module": "joker", "func": ("ecr", "RegistryPolicy")},
+    "ECRReplicationConfiguration": {
+        "module": "joker",
+        "func": ("ecr", "ReplicationConfiguration"),
+    },
     "ECRRepository": {"module": "joker", "func": ("ecr", "Repository")},
     "ECSCapacityProvider": {"module": "joker", "func": ("ecs", "CapacityProvider")},
     "ECSCluster": {"module": "joker", "func": ("ecs", "Cluster")},
     "ECSClusterCapacityProviderAssociations": {
         "module": "joker",
         "func": ("ecs", "ClusterCapacityProviderAssociations"),
     },
@@ -590,14 +616,15 @@
     "SQSQueuePolicy": {
         "module": "joker",
         "func": ("sqs", "QueuePolicy"),
         "dep": ["SNSSubscription"],
     },
     "SNSSubscription": {"module": "joker", "func": ("sns", "SubscriptionResource")},
     "SNSTopic": {"module": "joker", "func": ("sns", "Topic")},
+    "SNSTopicPolicy": {"module": "joker", "func": ("sns", "TopicPolicy")},
     "SSMParameter": {"module": "joker", "func": ("ssm", "Parameter")},
     "WAFv2IPSet": {
         "module": "joker",
         "func": ("wafv2", "IPSet"),
     },
     "WAFv2WebACL": {
         "module": "joker",
```

### Comparing `awsibox-0.8.9/awsibox/common.py` & `awsibox-0.9.1/awsibox/common.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/discover.py` & `awsibox-0.9.1/awsibox/discover.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/generate.py` & `awsibox-0.9.1/awsibox/generate.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/lambdas/ASGSpot.code` & `awsibox-0.9.1/awsibox/lambdas/ASGSpot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/lambdas/AtEdgeAddHeaders.code` & `awsibox-0.9.1/awsibox/lambdas/AtEdgeAddHeaders.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/lambdas/CCRFargateSpot.code` & `awsibox-0.9.1/awsibox/lambdas/CCRFargateSpot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/lambdas/CCRLightHouse.code` & `awsibox-0.9.1/awsibox/lambdas/CCRLightHouse.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/lambdas/CCRStackReplicator.code` & `awsibox-0.9.1/awsibox/lambdas/CCRStackReplicator.code`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 
 def set_cfg_stackparams(resource_properties):
     exclude_list = [
         "ServiceToken",
         "EnvStackVersion",
         "CCRReplicateRegions",
+        "IBOX_ENABLED",
     ]
     for p, v in resource_properties.items():
         if p not in exclude_list:
             setattr(i_cfg, p, v)
 
 
 def run_stackops(regions, mode):
```

### Comparing `awsibox-0.8.9/awsibox/lambdas/CloudWatchAlarmStateChange.code` & `awsibox-0.9.1/awsibox/lambdas/CloudWatchAlarmStateChange.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/lambdas/CloudWatchRepeatedNotify.code` & `awsibox-0.9.1/awsibox/lambdas/CloudWatchRepeatedNotify.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/lambdas/EC2StartStopTagged.code` & `awsibox-0.9.1/awsibox/lambdas/EC2StartStopTagged.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/lambdas/ECSClusterAutoscale.code` & `awsibox-0.9.1/awsibox/lambdas/ECSClusterAutoscale.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/lambdas/ECSDrainInstance.code` & `awsibox-0.9.1/awsibox/lambdas/ECSDrainInstance.code`

 * *Files 1% similar despite different names*

```diff
@@ -162,21 +162,25 @@
             msg["Cluster"] = cluster
             msg["Tasks"] = task_to_msg
         else:
             end_lf = True
 
     # lifecycle
     if end_lf:
-        CLIENT_AUTOSCALING.complete_lifecycle_action(
-            LifecycleHookName=lifecyclehook_name,
-            AutoScalingGroupName=asg_name,
-            LifecycleActionResult="CONTINUE",
-            InstanceId=instance_id,
-        )
-        logger.info("Completed lifecycle")
+        try:
+            CLIENT_AUTOSCALING.complete_lifecycle_action(
+                LifecycleHookName=lifecyclehook_name,
+                AutoScalingGroupName=asg_name,
+                LifecycleActionResult="CONTINUE",
+                InstanceId=instance_id,
+            )
+        except Exception as e:
+            logger.error(f"Error completing lifecycle: {e}")
+        else:
+            logger.info("Completed lifecycle")
     elif datetime.now(timezone.utc) < msg_time + timedelta(
         seconds=get_heartbeat_timeout(asg_name, lifecyclehook_name)
     ):
         # send a message with only the task not stopped to re-trigger lambda until 0 task running or LifeCycle timeout
         logger.info("Sending message with tasks running.")
         CLIENT_SQS.send_message(
             QueueUrl=SQS_QUEUE, MessageBody=json.dumps(msg), DelaySeconds=20
```

### Comparing `awsibox-0.8.9/awsibox/lambdas/ECSDrainTasks.code` & `awsibox-0.9.1/awsibox/lambdas/ECSDrainTasks.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/lambdas/ECSEventTaskStateChange.code` & `awsibox-0.9.1/awsibox/lambdas/ECSEventTaskStateChange.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/lambdas/ECSEventsSpot.code` & `awsibox-0.9.1/awsibox/lambdas/ECSEventsSpot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/lambdas/ECSRaiseASGAlarm.code` & `awsibox-0.9.1/awsibox/lambdas/ECSRaiseASGAlarm.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/lambdas/ECSRunTask.code` & `awsibox-0.9.1/awsibox/lambdas/ECSRunTask.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/lambdas/ECSUpdateDesiredCount.code` & `awsibox-0.9.1/awsibox/lambdas/ECSUpdateDesiredCount.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/lambdas/ElasticSearchSnapShot.code` & `awsibox-0.9.1/awsibox/lambdas/ElasticSearchSnapShot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/lambdas/ManageService.code` & `awsibox-0.9.1/awsibox/lambdas/ManageService.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/lambdas/PaidApi.code` & `awsibox-0.9.1/awsibox/lambdas/PaidApi.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/lambdas/PyPackager.code` & `awsibox-0.9.1/awsibox/lambdas/PyPackager.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/lambdas/R53RecordInstanceId.code` & `awsibox-0.9.1/awsibox/lambdas/R53RecordInstanceId.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/lambdas/ServiceDiscovery.code` & `awsibox-0.9.1/awsibox/lambdas/ServiceDiscovery.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/lambdas/ServiceUnavailable.code` & `awsibox-0.9.1/awsibox/lambdas/ServiceUnavailable.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/lambdas/StacksOps.code` & `awsibox-0.9.1/awsibox/lambdas/StacksOps.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/mod/__pycache__/autoscaling.cpython-311.pyc` & `awsibox-0.9.1/awsibox/mod/__pycache__/autoscaling.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x89d6a264 (Mon Jul  3 14:09:13 2023 UTC)
-files sz: 3950
+moddate:  0xf360b064 (Thu Jul 13 20:39:15 2023 UTC)
+files sz: 3685
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c006d015a020100640064016c036d045a040100640264
@@ -46,67 +46,62 @@
                 58 STORE_NAME              11 (get_dictvalue)
                 60 POP_TOP
    
     14          62 LOAD_CONST               5 (<code object AS_LaunchTemplate, file "/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/autoscaling.py", line 14>)
                 64 MAKE_FUNCTION            0
                 66 STORE_NAME              12 (AS_LaunchTemplate)
    
-    89          68 LOAD_CONST               6 (<code object AS_Autoscaling, file "/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/autoscaling.py", line 89>)
+    83          68 LOAD_CONST               6 (<code object AS_Autoscaling, file "/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/autoscaling.py", line 83>)
                 70 MAKE_FUNCTION            0
                 72 STORE_NAME              13 (AS_Autoscaling)
                 74 LOAD_CONST               1 (None)
                 76 RETURN_VALUE
    consts
       0
       None
       2
       ('*',)
       ('get_endvalue', 'auto_get_props', 'add_obj', 'import_user_data', 'get_dictvalue')
       code
          argcount  : 0
-         nlocals   : 7
+         nlocals   : 6
          stacksize : 10
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000006401740500
             0000000000000000006402a6010000ab010000000000000000ac03a60200
             00ab0200000000000000007d007401000000000000000000006a03000000
             00000000006404a6010000ab0100000000000000007d0174090000000000
-            00000000007c0164046405ac06a6030000ab030000000000000000010074
-            0b00000000000000000000740c0000000000000000000064076408a60300
-            00ab030000000000000000720367007d026e0c740c000000000000000000
-            006a0700000000000000007d027c016a0800000000000000006409190000
-            000000000000006a090000000000000000a00a0000000000000000000000
-            0000000000000000007c02a6010000ab01000000000000000001007c017c
-            005f030000000000000000740b00000000000000000000740c0000000000
-            0000000000640a740b00000000000000000000740c000000000000000000
-            00640ba6020000ab020000000000000000a6030000ab0300000000000000
-            007d037417000000000000000000007c03a6010000ab0100000000000000
-            007d047c047332640c640d640e640f641064117c036412660844005d277d
-            057c04a00a00000000000000000000000000000000000000007417000000
-            0000000000000064137c059b009d02a6010000ab010000000000000000a6
-            010000ab01000000000000000001008c2874190000000000000000000064
-            147c04a6020000ab0200000000000000007d04741b000000000000000000
-            007c04a6010000ab0100000000000000007c015f0e000000000000000074
-            0b00000000000000000000740c0000000000000000000064156408a60300
-            00ab0300000000000000007245741b00000000000000000000741f000000
-            000000000000006415741900000000000000000000641664178400740c00
-            0000000000000000006a1000000000000000004400a6000000ab00000000
-            0000000000a6020000ab0200000000000000007c04a6030000ab03000000
-            0000000000a6010000ab0100000000000000007c015f0e00000000000000
-            007423000000000000000000007c00a6010000ab01000000000000000001
-            00742500000000000000000000740c000000000000000000006418a60200
-            00ab020000000000000000726c7c006a0300000000000000006a13000000
-            000000000044005d617d067c066a1400000000000000006419760072547c
-            066a1500000000000000006a160000000000000000a00a00000000000000
-            00000000000000000000000000641a8400742f0000000000000000000074
-            0c000000000000000000006a1800000000000000006418ac1ba6020000ab
-            020000000000000000a01900000000000000000000000000000000000000
-            00a6000000ab0000000000000000004400a6000000ab0000000000000000
-            00a6010000ab01000000000000000001008c606400530064005300
+            00000000007c0164046405ac06a6030000ab03000000000000000001007c
+            017c005f030000000000000000740b00000000000000000000740c000000
+            000000000000006407740b00000000000000000000740c00000000000000
+            0000006408a6020000ab020000000000000000a6030000ab030000000000
+            0000007d02740f000000000000000000007c02a6010000ab010000000000
+            0000007d037c0373326409640a640b640c640d640e7c02640f660844005d
+            277d047c03a0080000000000000000000000000000000000000000740f00
+            00000000000000000064107c049b009d02a6010000ab0100000000000000
+            00a6010000ab01000000000000000001008c287413000000000000000000
+            0064117c03a6020000ab0200000000000000007d03741500000000000000
+            0000007c03a6010000ab0100000000000000007c015f0b00000000000000
+            00740b00000000000000000000740c0000000000000000000064126413a6
+            030000ab0300000000000000007245741500000000000000000000741900
+            000000000000000000641274130000000000000000000064146415840074
+            0c000000000000000000006a0d00000000000000004400a6000000ab0000
+            00000000000000a6020000ab0200000000000000007c03a6030000ab0300
+            00000000000000a6010000ab0100000000000000007c015f0b0000000000
+            000000741d000000000000000000007c00a6010000ab0100000000000000
+            000100741f00000000000000000000740c000000000000000000006416a6
+            020000ab020000000000000000726c7c006a0300000000000000006a1000
+            0000000000000044005d617d057c056a1100000000000000006417760072
+            547c056a1200000000000000006a130000000000000000a0080000000000
+            000000000000000000000000000000641884007429000000000000000000
+            00740c000000000000000000006a1500000000000000006416ac19a60200
+            00ab020000000000000000a0160000000000000000000000000000000000
+            000000a6000000ab0000000000000000004400a6000000ab000000000000
+            000000a6010000ab01000000000000000001008c606400530064005300
           14           0 RESUME                   0
          
           16           2 LOAD_GLOBAL              1 (NULL + ec2)
                       14 LOAD_ATTR                1 (LaunchTemplate)
          
           17          24 LOAD_CONST               1 ('LaunchTemplate')
          
@@ -136,330 +131,301 @@
           25         128 LOAD_CONST               5 ('AWS::EC2::LaunchTemplate')
          
           22         130 KW_NAMES                 6
                      132 PRECALL                  3
                      136 CALL                     3
                      146 POP_TOP
          
-          28         148 LOAD_GLOBAL             11 (NULL + getattr)
-                     160 LOAD_GLOBAL             12 (cfg)
-                     172 LOAD_CONST               7 ('IBOX_LAUNCH_TEMPLATE_NO_SG_EXTRA')
-                     174 LOAD_CONST               8 (False)
-                     176 PRECALL                  3
-                     180 CALL                     3
-                     190 POP_JUMP_FORWARD_IF_FALSE     3 (to 198)
-         
-          29         192 BUILD_LIST               0
-                     194 STORE_FAST               2 (SecurityGroups)
-                     196 JUMP_FORWARD            12 (to 222)
-         
-          31     >>  198 LOAD_GLOBAL             12 (cfg)
-                     210 LOAD_ATTR                7 (SecurityGroupsImport)
-                     220 STORE_FAST               2 (SecurityGroups)
-         
-          32     >>  222 LOAD_FAST                1 (LaunchTemplateData)
-                     224 LOAD_ATTR                8 (NetworkInterfaces)
-                     234 LOAD_CONST               9 (0)
-                     236 BINARY_SUBSCR
-                     246 LOAD_ATTR                9 (Groups)
-                     256 LOAD_METHOD             10 (extend)
-                     278 LOAD_FAST                2 (SecurityGroups)
-                     280 PRECALL                  1
-                     284 CALL                     1
-                     294 POP_TOP
+          28         148 LOAD_FAST                1 (LaunchTemplateData)
+                     150 LOAD_FAST                0 (R_LaunchTemplate)
+                     152 STORE_ATTR               3 (LaunchTemplateData)
+         
+          30         162 LOAD_GLOBAL             11 (NULL + getattr)
+                     174 LOAD_GLOBAL             12 (cfg)
+                     186 LOAD_CONST               7 ('IBOX_ROLE_EX')
+                     188 LOAD_GLOBAL             11 (NULL + getattr)
+                     200 LOAD_GLOBAL             12 (cfg)
+                     212 LOAD_CONST               8 ('envrole')
+                     214 PRECALL                  2
+                     218 CALL                     2
+                     228 PRECALL                  3
+                     232 CALL                     3
+                     242 STORE_FAST               2 (ud_envrole)
+         
+          32         244 LOAD_GLOBAL             15 (NULL + import_user_data)
+                     256 LOAD_FAST                2 (ud_envrole)
+                     258 PRECALL                  1
+                     262 CALL                     1
+                     272 STORE_FAST               3 (user_data)
+         
+          34         274 LOAD_FAST                3 (user_data)
+                     276 POP_JUMP_FORWARD_IF_TRUE    50 (to 378)
+         
+          37         278 LOAD_CONST               9 ('INIT')
+         
+          38         280 LOAD_CONST              10 ('PACKAGE')
+         
+          39         282 LOAD_CONST              11 ('SETUP')
+         
+          40         284 LOAD_CONST              12 ('APPS')
+         
+          41         286 LOAD_CONST              13 ('SERVICE')
+         
+          42         288 LOAD_CONST              14 ('ELBCHECK')
+         
+          43         290 LOAD_FAST                2 (ud_envrole)
+         
+          44         292 LOAD_CONST              15 ('END')
+         
+          36         294 BUILD_TUPLE              8
+                     296 GET_ITER
+                 >>  298 FOR_ITER                39 (to 378)
+                     300 STORE_FAST               4 (user_data_section)
+         
+          46         302 LOAD_FAST                3 (user_data)
+                     304 LOAD_METHOD              8 (extend)
+                     326 LOAD_GLOBAL             15 (NULL + import_user_data)
+                     338 LOAD_CONST              16 ('SCRIPTS/')
+                     340 LOAD_FAST                4 (user_data_section)
+                     342 FORMAT_VALUE             0
+                     344 BUILD_STRING             2
+                     346 PRECALL                  1
+                     350 CALL                     1
+                     360 PRECALL                  1
+                     364 CALL                     1
+                     374 POP_TOP
+                     376 JUMP_BACKWARD           40 (to 298)
+         
+          48     >>  378 LOAD_GLOBAL             19 (NULL + Join)
+                     390 LOAD_CONST              17 ('')
+                     392 LOAD_FAST                3 (user_data)
+                     394 PRECALL                  2
+                     398 CALL                     2
+                     408 STORE_FAST               3 (user_data)
+         
+          49         410 LOAD_GLOBAL             21 (NULL + Base64)
+                     422 LOAD_FAST                3 (user_data)
+                     424 PRECALL                  1
+                     428 CALL                     1
+                     438 LOAD_FAST                1 (LaunchTemplateData)
+                     440 STORE_ATTR              11 (UserData)
+         
+          51         450 LOAD_GLOBAL             11 (NULL + getattr)
+                     462 LOAD_GLOBAL             12 (cfg)
+                     474 LOAD_CONST              18 ('BottleRocket')
+                     476 LOAD_CONST              19 (False)
+                     478 PRECALL                  3
+                     482 CALL                     3
+                     492 POP_JUMP_FORWARD_IF_FALSE    69 (to 632)
+         
+          53         494 LOAD_GLOBAL             21 (NULL + Base64)
+         
+          54         506 LOAD_GLOBAL             25 (NULL + If)
+         
+          55         518 LOAD_CONST              18 ('BottleRocket')
+         
+          56         520 LOAD_GLOBAL             19 (NULL + Join)
+         
+          57         532 LOAD_CONST              20 ('\n')
+         
+          58         534 LOAD_CONST              21 (<code object <listcomp>, file "/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/autoscaling.py", line 58>)
+                     536 MAKE_FUNCTION            0
+         
+          60         538 LOAD_GLOBAL             12 (cfg)
+                     550 LOAD_ATTR               13 (BottleRocketUserData)
+         
+          58         560 GET_ITER
+                     562 PRECALL                  0
+                     566 CALL                     0
+         
+          56         576 PRECALL                  2
+                     580 CALL                     2
+         
+          63         590 LOAD_FAST                3 (user_data)
+         
+          54         592 PRECALL                  3
+                     596 CALL                     3
+         
+          53         606 PRECALL                  1
+                     610 CALL                     1
+                     620 LOAD_FAST                1 (LaunchTemplateData)
+                     622 STORE_ATTR              11 (UserData)
+         
+          67     >>  632 LOAD_GLOBAL             29 (NULL + add_obj)
+                     644 LOAD_FAST                0 (R_LaunchTemplate)
+                     646 PRECALL                  1
+                     650 CALL                     1
+                     660 POP_TOP
+         
+          70         662 LOAD_GLOBAL             31 (NULL + hasattr)
+                     674 LOAD_GLOBAL             12 (cfg)
+                     686 LOAD_CONST              22 ('MetadataTags')
+                     688 PRECALL                  2
+                     692 CALL                     2
+                     702 POP_JUMP_FORWARD_IF_FALSE   108 (to 920)
+         
+          71         704 LOAD_FAST                0 (R_LaunchTemplate)
+                     706 LOAD_ATTR                3 (LaunchTemplateData)
+                     716 LOAD_ATTR               16 (TagSpecifications)
+                     726 GET_ITER
+                 >>  728 FOR_ITER                97 (to 924)
+                     730 STORE_FAST               5 (n)
+         
+          72         732 LOAD_FAST                5 (n)
+                     734 LOAD_ATTR               17 (ResourceType)
+                     744 LOAD_CONST              23 (('instance', 'volume'))
+                     746 CONTAINS_OP              0
+                     748 POP_JUMP_FORWARD_IF_FALSE    84 (to 918)
+         
+          73         750 LOAD_FAST                5 (n)
+                     752 LOAD_ATTR               18 (Tags)
+                     762 LOAD_ATTR               19 (tags)
+                     772 LOAD_METHOD              8 (extend)
+         
+          74         794 LOAD_CONST              24 (<code object <listcomp>, file "/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/autoscaling.py", line 74>)
+                     796 MAKE_FUNCTION            0
+         
+          76         798 LOAD_GLOBAL             41 (NULL + get_dictvalue)
+         
+          77         810 LOAD_GLOBAL             12 (cfg)
+                     822 LOAD_ATTR               21 (MetadataTags)
+                     832 LOAD_CONST              22 ('MetadataTags')
          
-          34         296 LOAD_FAST                1 (LaunchTemplateData)
-                     298 LOAD_FAST                0 (R_LaunchTemplate)
-                     300 STORE_ATTR               3 (LaunchTemplateData)
-         
-          36         310 LOAD_GLOBAL             11 (NULL + getattr)
-                     322 LOAD_GLOBAL             12 (cfg)
-                     334 LOAD_CONST              10 ('IBOX_ROLE_EX')
-                     336 LOAD_GLOBAL             11 (NULL + getattr)
-                     348 LOAD_GLOBAL             12 (cfg)
-                     360 LOAD_CONST              11 ('envrole')
-                     362 PRECALL                  2
-                     366 CALL                     2
-                     376 PRECALL                  3
-                     380 CALL                     3
-                     390 STORE_FAST               3 (ud_envrole)
-         
-          38         392 LOAD_GLOBAL             23 (NULL + import_user_data)
-                     404 LOAD_FAST                3 (ud_envrole)
-                     406 PRECALL                  1
-                     410 CALL                     1
-                     420 STORE_FAST               4 (user_data)
-         
-          40         422 LOAD_FAST                4 (user_data)
-                     424 POP_JUMP_FORWARD_IF_TRUE    50 (to 526)
-         
-          43         426 LOAD_CONST              12 ('INIT')
-         
-          44         428 LOAD_CONST              13 ('PACKAGE')
-         
-          45         430 LOAD_CONST              14 ('SETUP')
-         
-          46         432 LOAD_CONST              15 ('APPS')
-         
-          47         434 LOAD_CONST              16 ('SERVICE')
-         
-          48         436 LOAD_CONST              17 ('ELBCHECK')
-         
-          49         438 LOAD_FAST                3 (ud_envrole)
-         
-          50         440 LOAD_CONST              18 ('END')
-         
-          42         442 BUILD_TUPLE              8
-                     444 GET_ITER
-                 >>  446 FOR_ITER                39 (to 526)
-                     448 STORE_FAST               5 (user_data_section)
-         
-          52         450 LOAD_FAST                4 (user_data)
-                     452 LOAD_METHOD             10 (extend)
-                     474 LOAD_GLOBAL             23 (NULL + import_user_data)
-                     486 LOAD_CONST              19 ('SCRIPTS/')
-                     488 LOAD_FAST                5 (user_data_section)
-                     490 FORMAT_VALUE             0
-                     492 BUILD_STRING             2
-                     494 PRECALL                  1
-                     498 CALL                     1
-                     508 PRECALL                  1
-                     512 CALL                     1
-                     522 POP_TOP
-                     524 JUMP_BACKWARD           40 (to 446)
-         
-          54     >>  526 LOAD_GLOBAL             25 (NULL + Join)
-                     538 LOAD_CONST              20 ('')
-                     540 LOAD_FAST                4 (user_data)
-                     542 PRECALL                  2
-                     546 CALL                     2
-                     556 STORE_FAST               4 (user_data)
-         
-          55         558 LOAD_GLOBAL             27 (NULL + Base64)
-                     570 LOAD_FAST                4 (user_data)
-                     572 PRECALL                  1
-                     576 CALL                     1
-                     586 LOAD_FAST                1 (LaunchTemplateData)
-                     588 STORE_ATTR              14 (UserData)
-         
-          57         598 LOAD_GLOBAL             11 (NULL + getattr)
-                     610 LOAD_GLOBAL             12 (cfg)
-                     622 LOAD_CONST              21 ('BottleRocket')
-                     624 LOAD_CONST               8 (False)
-                     626 PRECALL                  3
-                     630 CALL                     3
-                     640 POP_JUMP_FORWARD_IF_FALSE    69 (to 780)
-         
-          59         642 LOAD_GLOBAL             27 (NULL + Base64)
-         
-          60         654 LOAD_GLOBAL             31 (NULL + If)
-         
-          61         666 LOAD_CONST              21 ('BottleRocket')
-         
-          62         668 LOAD_GLOBAL             25 (NULL + Join)
-         
-          63         680 LOAD_CONST              22 ('\n')
-         
-          64         682 LOAD_CONST              23 (<code object <listcomp>, file "/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/autoscaling.py", line 64>)
-                     684 MAKE_FUNCTION            0
-         
-          66         686 LOAD_GLOBAL             12 (cfg)
-                     698 LOAD_ATTR               16 (BottleRocketUserData)
-         
-          64         708 GET_ITER
-                     710 PRECALL                  0
-                     714 CALL                     0
-         
-          62         724 PRECALL                  2
-                     728 CALL                     2
-         
-          69         738 LOAD_FAST                4 (user_data)
-         
-          60         740 PRECALL                  3
-                     744 CALL                     3
-         
-          59         754 PRECALL                  1
-                     758 CALL                     1
-                     768 LOAD_FAST                1 (LaunchTemplateData)
-                     770 STORE_ATTR              14 (UserData)
-         
-          73     >>  780 LOAD_GLOBAL             35 (NULL + add_obj)
-                     792 LOAD_FAST                0 (R_LaunchTemplate)
-                     794 PRECALL                  1
-                     798 CALL                     1
-                     808 POP_TOP
-         
-          76         810 LOAD_GLOBAL             37 (NULL + hasattr)
-                     822 LOAD_GLOBAL             12 (cfg)
-                     834 LOAD_CONST              24 ('MetadataTags')
+          76         834 KW_NAMES                25
                      836 PRECALL                  2
                      840 CALL                     2
-                     850 POP_JUMP_FORWARD_IF_FALSE   108 (to 1068)
          
-          77         852 LOAD_FAST                0 (R_LaunchTemplate)
-                     854 LOAD_ATTR                3 (LaunchTemplateData)
-                     864 LOAD_ATTR               19 (TagSpecifications)
-                     874 GET_ITER
-                 >>  876 FOR_ITER                97 (to 1072)
-                     878 STORE_FAST               6 (n)
-         
-          78         880 LOAD_FAST                6 (n)
-                     882 LOAD_ATTR               20 (ResourceType)
-                     892 LOAD_CONST              25 (('instance', 'volume'))
-                     894 CONTAINS_OP              0
-                     896 POP_JUMP_FORWARD_IF_FALSE    84 (to 1066)
-         
-          79         898 LOAD_FAST                6 (n)
-                     900 LOAD_ATTR               21 (Tags)
-                     910 LOAD_ATTR               22 (tags)
-                     920 LOAD_METHOD             10 (extend)
-         
-          80         942 LOAD_CONST              26 (<code object <listcomp>, file "/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/autoscaling.py", line 80>)
-                     944 MAKE_FUNCTION            0
-         
-          82         946 LOAD_GLOBAL             47 (NULL + get_dictvalue)
-         
-          83         958 LOAD_GLOBAL             12 (cfg)
-                     970 LOAD_ATTR               24 (MetadataTags)
-                     980 LOAD_CONST              24 ('MetadataTags')
-         
-          82         982 KW_NAMES                27
-                     984 PRECALL                  2
-                     988 CALL                     2
-         
-          84         998 LOAD_METHOD             25 (items)
-                    1020 PRECALL                  0
-                    1024 CALL                     0
-         
-          80        1034 GET_ITER
-                    1036 PRECALL                  0
-                    1040 CALL                     0
-         
-          79        1050 PRECALL                  1
-                    1054 CALL                     1
-                    1064 POP_TOP
-                 >> 1066 JUMP_BACKWARD           96 (to 876)
+          78         850 LOAD_METHOD             22 (items)
+                     872 PRECALL                  0
+                     876 CALL                     0
+         
+          74         886 GET_ITER
+                     888 PRECALL                  0
+                     892 CALL                     0
+         
+          73         902 PRECALL                  1
+                     906 CALL                     1
+                     916 POP_TOP
+                 >>  918 JUMP_BACKWARD           96 (to 728)
          
-          76     >> 1068 LOAD_CONST               0 (None)
-                    1070 RETURN_VALUE
+          70     >>  920 LOAD_CONST               0 (None)
+                     922 RETURN_VALUE
          
-          77     >> 1072 LOAD_CONST               0 (None)
-                    1074 RETURN_VALUE
+          71     >>  924 LOAD_CONST               0 (None)
+                     926 RETURN_VALUE
          consts
             None
             'LaunchTemplate'
             '${AWS::StackName}-${EnvRole}'
             ('LaunchTemplateName',)
             'LaunchTemplateData'
             'AWS::EC2::LaunchTemplate'
             ('res_obj_type',)
-            'IBOX_LAUNCH_TEMPLATE_NO_SG_EXTRA'
-            False
-            0
             'IBOX_ROLE_EX'
             'envrole'
             'INIT'
             'PACKAGE'
             'SETUP'
             'APPS'
             'SERVICE'
             'ELBCHECK'
             'END'
             'SCRIPTS/'
             ''
             'BottleRocket'
+            False
             '\n'
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 7
                flags     : 19
                code
                   0x970067007c005d157d0174010000000000000000000064007c019b0064
                   019d03a6010000ab01000000000000000091028c165300
-                64           0 RESUME                   0
+                58           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                21 (to 50)
                
-                66           8 STORE_FAST               1 (n)
+                60           8 STORE_FAST               1 (n)
                
-                65          10 LOAD_GLOBAL              1 (NULL + get_endvalue)
+                59          10 LOAD_GLOBAL              1 (NULL + get_endvalue)
                             22 LOAD_CONST               0 ('BottleRocketUserData')
                             24 LOAD_FAST                1 (n)
                             26 FORMAT_VALUE             0
                             28 LOAD_CONST               1 ('Line')
                             30 BUILD_STRING             3
                             32 PRECALL                  1
                             36 CALL                     1
                
-                64          46 LIST_APPEND              2
+                58          46 LIST_APPEND              2
                             48 JUMP_BACKWARD           22 (to 6)
                        >>   50 RETURN_VALUE
                consts
                   'BottleRocketUserData'
                   'Line'
                names      ('get_endvalue',)
                varnames   ('.0', 'n')
                freevars   ()
                cellvars   ()
                filename   '/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/autoscaling.py'
                name       '<listcomp>'
-               firstlineno 64
+               firstlineno 58
                lnotab 0x080202ff24ff
             'MetadataTags'
             ('instance', 'volume')
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 19
                code
                   0x970067007c005d0a5c0200007d017d027c017c0264009c0291028c0b53
                   00
-                80           0 RESUME                   0
+                74           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                10 (to 28)
                
-                82           8 UNPACK_SEQUENCE          2
+                76           8 UNPACK_SEQUENCE          2
                             12 STORE_FAST               1 (n)
                             14 STORE_FAST               2 (v)
                
-                81          16 LOAD_FAST                1 (n)
+                75          16 LOAD_FAST                1 (n)
                             18 LOAD_FAST                2 (v)
                             20 LOAD_CONST               0 (('Key', 'Value'))
                             22 BUILD_CONST_KEY_MAP      2
                
-                80          24 LIST_APPEND              2
+                74          24 LIST_APPEND              2
                             26 JUMP_BACKWARD           11 (to 6)
                        >>   28 RETURN_VALUE
                consts
                   ('Key', 'Value')
                names      ()
                varnames   ('.0', 'n', 'v')
                freevars   ()
                cellvars   ()
                filename   '/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/autoscaling.py'
                name       '<listcomp>'
-               firstlineno 80
+               firstlineno 74
                lnotab 0x080208ff08ff
             ('mapname',)
-         names      ('ec2', 'LaunchTemplate', 'Sub', 'LaunchTemplateData', 'auto_get_props', 'getattr', 'cfg', 'SecurityGroupsImport', 'NetworkInterfaces', 'Groups', 'extend', 'import_user_data', 'Join', 'Base64', 'UserData', 'If', 'BottleRocketUserData', 'add_obj', 'hasattr', 'TagSpecifications', 'ResourceType', 'Tags', 'tags', 'get_dictvalue', 'MetadataTags', 'items')
-         varnames   ('R_LaunchTemplate', 'LaunchTemplateData', 'SecurityGroups', 'ud_envrole', 'user_data', 'user_data_section', 'n')
+         names      ('ec2', 'LaunchTemplate', 'Sub', 'LaunchTemplateData', 'auto_get_props', 'getattr', 'cfg', 'import_user_data', 'extend', 'Join', 'Base64', 'UserData', 'If', 'BottleRocketUserData', 'add_obj', 'hasattr', 'TagSpecifications', 'ResourceType', 'Tags', 'tags', 'get_dictvalue', 'MetadataTags', 'items')
+         varnames   ('R_LaunchTemplate', 'LaunchTemplateData', 'ud_envrole', 'user_data', 'user_data_section', 'n')
          freevars   ()
          cellvars   ()
          filename   '/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/autoscaling.py'
          name       'AS_LaunchTemplate'
          firstlineno 14
          lnotab
-            0x0202160102011cfe120528010c010201020102fd12062c01060218014a
-            020e0252021e020403020102010201020102010201020102f8080a4c0220
-            0128022c020c010c0102010c010201040216fe10fe0e0702f70eff1a0e1e
-            032a011c0112012c0104020c0118ff100224fc10ff12fd0401
+            0x0202160102011cfe120528010c010201020102fd12060e0252021e0204
+            03020102010201020102010201020102f8080a4c02200128022c020c010c
+            0102010c010201040216fe10fe0e0702f70eff1a0e1e032a011c0112012c
+            0104020c0118ff100224fc10ff12fd0401
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 9
          flags     : 3
          code
             0x970067007d0167007d027400000000000000000000006a010000000000
@@ -489,199 +455,197 @@
             00000000007d05741f000000000000000000007c05a6010000ab01000000
             0000000000010009007c056a10000000000000000001007c056a10000000
             0000000000a01100000000000000000000000000000000000000007c02a6
             010000ab01000000000000000001006e1723007424000000000000000000
             002400720a01007c027c055f10000000000000000059006e047700780359
             0077017427000000000000000000007c056701a6010000ab010000000000
             000000010064005300
-          89           0 RESUME                   0
+          83           0 RESUME                   0
          
-          90           2 BUILD_LIST               0
+          84           2 BUILD_LIST               0
                        4 STORE_FAST               1 (LoadBalancers)
          
-          91           6 BUILD_LIST               0
+          85           6 BUILD_LIST               0
                        8 STORE_FAST               2 (TargetGroups)
          
-          92          10 LOAD_GLOBAL              0 (cfg)
+          86          10 LOAD_GLOBAL              0 (cfg)
                       22 LOAD_ATTR                1 (LoadBalancerType)
                       32 LOAD_CONST               1 ('Classic')
                       34 COMPARE_OP               2 (==)
                       40 POP_JUMP_FORWARD_IF_FALSE   128 (to 298)
          
-          93          42 LOAD_GLOBAL              0 (cfg)
+          87          42 LOAD_GLOBAL              0 (cfg)
                       54 LOAD_ATTR                2 (LoadBalancer)
                       64 LOAD_METHOD              3 (replace)
                       86 LOAD_CONST               2 (',')
                       88 LOAD_CONST               3 (' ')
                       90 PRECALL                  2
                       94 CALL                     2
                      104 LOAD_METHOD              4 (split)
                      126 PRECALL                  0
                      130 CALL                     0
                      140 GET_ITER
                  >>  142 FOR_ITER                77 (to 298)
                      144 STORE_FAST               3 (n)
          
-          94         146 LOAD_FAST                1 (LoadBalancers)
+          88         146 LOAD_FAST                1 (LoadBalancers)
                      148 LOAD_METHOD              5 (append)
                      170 LOAD_GLOBAL             13 (NULL + Ref)
                      182 LOAD_CONST               4 ('LoadBalancerClassic')
                      184 LOAD_FAST                3 (n)
                      186 FORMAT_VALUE             0
                      188 BUILD_STRING             2
                      190 PRECALL                  1
                      194 CALL                     1
                      204 PRECALL                  1
                      208 CALL                     1
                      218 POP_TOP
          
-          95         220 LOAD_GLOBAL             15 (NULL + setattr)
+          89         220 LOAD_GLOBAL             15 (NULL + setattr)
          
-          96         232 LOAD_GLOBAL              0 (cfg)
+          90         232 LOAD_GLOBAL              0 (cfg)
          
-          97         244 LOAD_CONST               5 ('EC2InstanceUserDataELBClassicCheckLoadBalancerName')
+          91         244 LOAD_CONST               5 ('EC2InstanceUserDataELBClassicCheckLoadBalancerName')
          
-          98         246 LOAD_GLOBAL             13 (NULL + Ref)
+          92         246 LOAD_GLOBAL             13 (NULL + Ref)
                      258 LOAD_CONST               4 ('LoadBalancerClassic')
                      260 LOAD_FAST                3 (n)
                      262 FORMAT_VALUE             0
                      264 BUILD_STRING             2
                      266 PRECALL                  1
                      270 CALL                     1
          
-          95         280 PRECALL                  3
+          89         280 PRECALL                  3
                      284 CALL                     3
                      294 POP_TOP
                      296 JUMP_BACKWARD           78 (to 142)
          
-         100     >>  298 LOAD_GLOBAL              0 (cfg)
+          94     >>  298 LOAD_GLOBAL              0 (cfg)
                      310 LOAD_ATTR                1 (LoadBalancerType)
                      320 LOAD_CONST               6 (('Application', 'Network'))
                      322 CONTAINS_OP              0
                      324 POP_JUMP_FORWARD_IF_FALSE   164 (to 654)
          
-         101         326 LOAD_GLOBAL             17 (NULL + getattr)
+          95         326 LOAD_GLOBAL             17 (NULL + getattr)
                      338 LOAD_GLOBAL              0 (cfg)
                      350 LOAD_CONST               7 ('ElasticLoadBalancingV2TargetGroup')
                      352 BUILD_MAP                0
                      354 PRECALL                  3
                      358 CALL                     3
                      368 LOAD_METHOD              9 (items)
                      390 PRECALL                  0
                      394 CALL                     0
                      404 GET_ITER
                  >>  406 FOR_ITER               123 (to 654)
                      408 UNPACK_SEQUENCE          2
                      412 STORE_FAST               3 (n)
                      414 STORE_FAST               4 (v)
          
-         103         416 LOAD_FAST                3 (n)
+          97         416 LOAD_FAST                3 (n)
                      418 LOAD_METHOD             10 (startswith)
                      440 LOAD_CONST               8 ('EC2')
                      442 PRECALL                  1
                      446 CALL                     1
                      456 POP_JUMP_FORWARD_IF_FALSE    97 (to 652)
                      458 LOAD_FAST                4 (v)
                      460 LOAD_METHOD             11 (get)
                      482 LOAD_CONST               9 ('IBOX_ENABLED')
                      484 LOAD_CONST              10 (True)
                      486 PRECALL                  2
                      490 CALL                     2
                      500 POP_JUMP_FORWARD_IF_FALSE    75 (to 652)
          
-         104         502 LOAD_FAST                2 (TargetGroups)
+          98         502 LOAD_FAST                2 (TargetGroups)
                      504 LOAD_METHOD              5 (append)
-         
-         105         526 LOAD_GLOBAL             13 (NULL + Ref)
+                     526 LOAD_GLOBAL             13 (NULL + Ref)
                      538 LOAD_CONST               7 ('ElasticLoadBalancingV2TargetGroup')
                      540 LOAD_FAST                3 (n)
                      542 FORMAT_VALUE             0
                      544 BUILD_STRING             2
                      546 PRECALL                  1
                      550 CALL                     1
-         
-         104         560 PRECALL                  1
+                     560 PRECALL                  1
                      564 CALL                     1
                      574 POP_TOP
          
-         107         576 LOAD_GLOBAL             15 (NULL + setattr)
+          99         576 LOAD_GLOBAL             15 (NULL + setattr)
          
-         108         588 LOAD_GLOBAL              0 (cfg)
+         100         588 LOAD_GLOBAL              0 (cfg)
          
-         109         600 LOAD_CONST              11 ('EC2InstanceUserDataELBV2CheckTargetGroupArn')
+         101         600 LOAD_CONST              11 ('EC2InstanceUserDataELBV2CheckTargetGroupArn')
          
-         110         602 LOAD_GLOBAL             13 (NULL + Ref)
+         102         602 LOAD_GLOBAL             13 (NULL + Ref)
                      614 LOAD_CONST               7 ('ElasticLoadBalancingV2TargetGroup')
                      616 LOAD_FAST                3 (n)
                      618 FORMAT_VALUE             0
                      620 BUILD_STRING             2
                      622 PRECALL                  1
                      626 CALL                     1
          
-         107         636 PRECALL                  3
+          99         636 PRECALL                  3
                      640 CALL                     3
                      650 POP_TOP
                  >>  652 JUMP_BACKWARD          124 (to 406)
          
-         114     >>  654 LOAD_GLOBAL             25 (NULL + AS_LaunchTemplate)
+         106     >>  654 LOAD_GLOBAL             25 (NULL + AS_LaunchTemplate)
                      666 PRECALL                  0
                      670 CALL                     0
                      680 POP_TOP
          
-         116         682 LOAD_GLOBAL             27 (NULL + asg)
+         108         682 LOAD_GLOBAL             27 (NULL + asg)
                      694 LOAD_ATTR               14 (AutoScalingGroup)
          
-         117         704 LOAD_CONST              12 ('AutoScalingGroupBase')
+         109         704 LOAD_CONST              12 ('AutoScalingGroupBase')
          
-         118         706 LOAD_FAST                1 (LoadBalancers)
+         110         706 LOAD_FAST                1 (LoadBalancers)
          
-         116         708 KW_NAMES                13
+         108         708 KW_NAMES                13
                      710 PRECALL                  2
                      714 CALL                     2
                      724 STORE_FAST               5 (R_ASG)
          
-         121         726 LOAD_GLOBAL             31 (NULL + auto_get_props)
+         113         726 LOAD_GLOBAL             31 (NULL + auto_get_props)
                      738 LOAD_FAST                5 (R_ASG)
                      740 PRECALL                  1
                      744 CALL                     1
                      754 POP_TOP
          
-         123         756 NOP
+         115         756 NOP
          
-         124         758 LOAD_FAST                5 (R_ASG)
+         116         758 LOAD_FAST                5 (R_ASG)
                      760 LOAD_ATTR               16 (TargetGroupARNs)
                      770 POP_TOP
          
-         128         772 LOAD_FAST                5 (R_ASG)
+         120         772 LOAD_FAST                5 (R_ASG)
                      774 LOAD_ATTR               16 (TargetGroupARNs)
                      784 LOAD_METHOD             17 (extend)
                      806 LOAD_FAST                2 (TargetGroups)
                      808 PRECALL                  1
                      812 CALL                     1
                      822 POP_TOP
                      824 JUMP_FORWARD            23 (to 872)
                  >>  826 PUSH_EXC_INFO
          
-         125         828 LOAD_GLOBAL             36 (Exception)
+         117         828 LOAD_GLOBAL             36 (Exception)
                      840 CHECK_EXC_MATCH
                      842 POP_JUMP_FORWARD_IF_FALSE    10 (to 864)
                      844 POP_TOP
          
-         126         846 LOAD_FAST                2 (TargetGroups)
+         118         846 LOAD_FAST                2 (TargetGroups)
                      848 LOAD_FAST                5 (R_ASG)
                      850 STORE_ATTR              16 (TargetGroupARNs)
                      860 POP_EXCEPT
                      862 JUMP_FORWARD             4 (to 872)
          
-         125     >>  864 RERAISE                  0
+         117     >>  864 RERAISE                  0
                  >>  866 COPY                     3
                      868 POP_EXCEPT
                      870 RERAISE                  1
          
-         130     >>  872 LOAD_GLOBAL             39 (NULL + add_obj)
+         122     >>  872 LOAD_GLOBAL             39 (NULL + add_obj)
                      884 LOAD_FAST                5 (R_ASG)
                      886 BUILD_LIST               1
                      888 PRECALL                  1
                      892 CALL                     1
                      902 POP_TOP
                      904 LOAD_CONST               0 (None)
                      906 RETURN_VALUE
@@ -706,20 +670,20 @@
             ('LoadBalancerNames',)
          names      ('cfg', 'LoadBalancerType', 'LoadBalancer', 'replace', 'split', 'append', 'Ref', 'setattr', 'getattr', 'items', 'startswith', 'get', 'AS_LaunchTemplate', 'asg', 'AutoScalingGroup', 'auto_get_props', 'TargetGroupARNs', 'extend', 'Exception', 'add_obj')
          varnames   ('key', 'LoadBalancers', 'TargetGroups', 'n', 'v', 'R_ASG')
          freevars   ()
          cellvars   ()
          filename   '/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/autoscaling.py'
          name       'AS_Autoscaling'
-         firstlineno 89
+         firstlineno 83
          lnotab
-            0x020104010401200168014a010c010c01020122fd12051c015a02560118
-            0122ff10030c010c01020122fd12071c021601020102fe12051e0202010e
-            0438fd120112ff0805
+            0x020104010401200168014a010c010c01020122fd12051c015a0256014a
+            010c010c01020122fd12071c021601020102fe12051e0202010e0438fd12
+            0112ff0805
    names      ('troposphere.autoscaling', 'autoscaling', 'asg', 'troposphere.ec2', 'ec2', 'common', 'shared', 'get_endvalue', 'auto_get_props', 'add_obj', 'import_user_data', 'get_dictvalue', 'AS_LaunchTemplate', 'AS_Autoscaling')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/autoscaling.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c010c0208011c09064b
+   lnotab 0x00ff02010c010c0208011c090645
```

### Comparing `awsibox-0.8.9/awsibox/mod/__pycache__/cloudformation.cpython-311.pyc` & `awsibox-0.9.1/awsibox/mod/__pycache__/cloudformation.cpython-311.pyc`

 * *Files 23% similar despite different names*

#### Python bytecode

```diff
@@ -1,20 +1,19 @@
 magic:    0xa70d0d0a
-moddate:  0x7a2a8c64 (Fri Jun 16 09:25:14 2023 UTC)
-files sz: 3746
+moddate:  0x634eb164 (Fri Jul 14 13:32:19 2023 UTC)
+files sz: 2707
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c006d015a020100640264036c035400640264046c046d
-      055a056d065a066d075a076d085a086d095a096d0a5a0a6d0b5a0b010064
-      0584005a0c640684005a0d640784005a0e640884005a0f640984005a1064
-      0a84005a11640b84005a12640c84005a1364015300
+      055a056d065a066d075a070100640584005a08640684005a09640784005a
+      0a640884005a0b640984005a0c64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (troposphere.cloudformation)
                  8 IMPORT_FROM              1 (cloudformation)
                 10 STORE_NAME               2 (cfm)
@@ -22,71 +21,51 @@
    
      3          14 LOAD_CONST               2 (2)
                 16 LOAD_CONST               3 (('*',))
                 18 IMPORT_NAME              3 (common)
                 20 IMPORT_STAR
    
      4          22 LOAD_CONST               2 (2)
-                24 LOAD_CONST               4 (('Parameter', 'do_no_override', 'get_endvalue', 'get_expvalue', 'get_condition', 'add_obj', 'auto_build_obj'))
+                24 LOAD_CONST               4 (('get_endvalue', 'add_obj', 'auto_get_props'))
                 26 IMPORT_NAME              4 (shared)
-                28 IMPORT_FROM              5 (Parameter)
-                30 STORE_NAME               5 (Parameter)
-                32 IMPORT_FROM              6 (do_no_override)
-                34 STORE_NAME               6 (do_no_override)
-                36 IMPORT_FROM              7 (get_endvalue)
-                38 STORE_NAME               7 (get_endvalue)
-                40 IMPORT_FROM              8 (get_expvalue)
-                42 STORE_NAME               8 (get_expvalue)
-                44 IMPORT_FROM              9 (get_condition)
-                46 STORE_NAME               9 (get_condition)
-                48 IMPORT_FROM             10 (add_obj)
-                50 STORE_NAME              10 (add_obj)
-                52 IMPORT_FROM             11 (auto_build_obj)
-                54 STORE_NAME              11 (auto_build_obj)
-                56 POP_TOP
-   
-    16          58 LOAD_CONST               5 (<code object mapping_EnvRegion, file "/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/cloudformation.py", line 16>)
-                60 MAKE_FUNCTION            0
-                62 STORE_NAME              12 (mapping_EnvRegion)
-   
-    38          64 LOAD_CONST               6 (<code object mapping_EC2, file "/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/cloudformation.py", line 38>)
-                66 MAKE_FUNCTION            0
-                68 STORE_NAME              13 (mapping_EC2)
-   
-    62          70 LOAD_CONST               7 (<code object mapping_AZ, file "/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/cloudformation.py", line 62>)
-                72 MAKE_FUNCTION            0
-                74 STORE_NAME              14 (mapping_AZ)
-   
-    87          76 LOAD_CONST               8 (<code object CFM_Parameters, file "/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/cloudformation.py", line 87>)
-                78 MAKE_FUNCTION            0
-                80 STORE_NAME              15 (CFM_Parameters)
-   
-    91          82 LOAD_CONST               9 (<code object CFM_Conditions, file "/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/cloudformation.py", line 91>)
-                84 MAKE_FUNCTION            0
-                86 STORE_NAME              16 (CFM_Conditions)
-   
-   100          88 LOAD_CONST              10 (<code object CFM_Mappings, file "/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/cloudformation.py", line 100>)
-                90 MAKE_FUNCTION            0
-                92 STORE_NAME              17 (CFM_Mappings)
-   
-   114          94 LOAD_CONST              11 (<code object CFM_Outputs, file "/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/cloudformation.py", line 114>)
-                96 MAKE_FUNCTION            0
-                98 STORE_NAME              18 (CFM_Outputs)
-   
-   118         100 LOAD_CONST              12 (<code object CFM_CustomResourceReplicator, file "/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/cloudformation.py", line 118>)
-               102 MAKE_FUNCTION            0
-               104 STORE_NAME              19 (CFM_CustomResourceReplicator)
-               106 LOAD_CONST               1 (None)
-               108 RETURN_VALUE
+                28 IMPORT_FROM              5 (get_endvalue)
+                30 STORE_NAME               5 (get_endvalue)
+                32 IMPORT_FROM              6 (add_obj)
+                34 STORE_NAME               6 (add_obj)
+                36 IMPORT_FROM              7 (auto_get_props)
+                38 STORE_NAME               7 (auto_get_props)
+                40 POP_TOP
+   
+    11          42 LOAD_CONST               5 (<code object mapping_EnvRegion, file "/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/cloudformation.py", line 11>)
+                44 MAKE_FUNCTION            0
+                46 STORE_NAME               8 (mapping_EnvRegion)
+   
+    33          48 LOAD_CONST               6 (<code object mapping_EC2, file "/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/cloudformation.py", line 33>)
+                50 MAKE_FUNCTION            0
+                52 STORE_NAME               9 (mapping_EC2)
+   
+    57          54 LOAD_CONST               7 (<code object mapping_AZ, file "/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/cloudformation.py", line 57>)
+                56 MAKE_FUNCTION            0
+                58 STORE_NAME              10 (mapping_AZ)
+   
+    82          60 LOAD_CONST               8 (<code object CFM_Mappings, file "/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/cloudformation.py", line 82>)
+                62 MAKE_FUNCTION            0
+                64 STORE_NAME              11 (CFM_Mappings)
+   
+    96          66 LOAD_CONST               9 (<code object CFM_CustomResourceReplicator, file "/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/cloudformation.py", line 96>)
+                68 MAKE_FUNCTION            0
+                70 STORE_NAME              12 (CFM_CustomResourceReplicator)
+                72 LOAD_CONST               1 (None)
+                74 RETURN_VALUE
    consts
       0
       None
       2
       ('*',)
-      ('Parameter', 'do_no_override', 'get_endvalue', 'get_expvalue', 'get_condition', 'add_obj', 'auto_build_obj')
+      ('get_endvalue', 'add_obj', 'auto_get_props')
       code
          argcount  : 0
          nlocals   : 5
          stacksize : 7
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
@@ -100,134 +79,134 @@
             0319000000000000000000760172360900740f0000000000000000000074
             04000000000000000000007c04a6020000ab0200000000000000007c007c
             01190000000000000000007c03190000000000000000007c043c0000008c
             38230074100000000000000000000024007203010059008c447700780359
             0077018c497c007c01190000000000000000007c03190000000000000000
             0073097c007c01190000000000000000007c033d008c6f7c007c01190000
             0000000000000073037c007c013d008ca67c005300
-          16           0 RESUME                   0
+          11           0 RESUME                   0
          
-          17           2 LOAD_GLOBAL              0 (copy)
+          12           2 LOAD_GLOBAL              0 (copy)
                       14 LOAD_METHOD              1 (deepcopy)
                       36 LOAD_GLOBAL              4 (cfg)
                       48 LOAD_ATTR                3 (RP_map)
                       58 PRECALL                  1
                       62 CALL                     1
                       72 STORE_FAST               0 (RP)
          
-          19          74 LOAD_GLOBAL              9 (NULL + list)
+          14          74 LOAD_GLOBAL              9 (NULL + list)
                       86 LOAD_FAST                0 (RP)
                       88 PRECALL                  1
                       92 CALL                     1
                      102 GET_ITER
                  >>  104 FOR_ITER               165 (to 436)
                      106 STORE_FAST               1 (env)
          
-          20         108 LOAD_FAST                0 (RP)
+          15         108 LOAD_FAST                0 (RP)
                      110 LOAD_FAST                1 (env)
                      112 BINARY_SUBSCR
                      122 STORE_FAST               2 (rvalue)
          
-          21         124 LOAD_GLOBAL              9 (NULL + list)
+          16         124 LOAD_GLOBAL              9 (NULL + list)
                      136 LOAD_FAST                2 (rvalue)
                      138 LOAD_METHOD              5 (keys)
                      160 PRECALL                  0
                      164 CALL                     0
                      174 PRECALL                  1
                      178 CALL                     1
                      188 GET_ITER
                  >>  190 FOR_ITER               110 (to 412)
                      192 STORE_FAST               3 (region)
          
-          22         194 LOAD_GLOBAL              4 (cfg)
+          17         194 LOAD_GLOBAL              4 (cfg)
                      206 LOAD_ATTR                6 (mappedvalues)
                      216 GET_ITER
                  >>  218 FOR_ITER                72 (to 364)
                      220 STORE_FAST               4 (key)
          
-          23         222 LOAD_FAST                4 (key)
+          18         222 LOAD_FAST                4 (key)
                      224 LOAD_FAST                0 (RP)
                      226 LOAD_FAST                1 (env)
                      228 BINARY_SUBSCR
                      238 LOAD_FAST                3 (region)
                      240 BINARY_SUBSCR
                      250 CONTAINS_OP              1
                      252 POP_JUMP_FORWARD_IF_FALSE    54 (to 362)
          
-          25         254 NOP
+          20         254 NOP
          
-          26         256 LOAD_GLOBAL             15 (NULL + getattr)
+          21         256 LOAD_GLOBAL             15 (NULL + getattr)
                      268 LOAD_GLOBAL              4 (cfg)
                      280 LOAD_FAST                4 (key)
                      282 PRECALL                  2
                      286 CALL                     2
                      296 LOAD_FAST                0 (RP)
                      298 LOAD_FAST                1 (env)
                      300 BINARY_SUBSCR
                      310 LOAD_FAST                3 (region)
                      312 BINARY_SUBSCR
                      322 LOAD_FAST                4 (key)
                      324 STORE_SUBSCR
                      328 JUMP_BACKWARD           56 (to 218)
                  >>  330 PUSH_EXC_INFO
          
-          27         332 LOAD_GLOBAL             16 (Exception)
+          22         332 LOAD_GLOBAL             16 (Exception)
                      344 CHECK_EXC_MATCH
                      346 POP_JUMP_FORWARD_IF_FALSE     3 (to 354)
                      348 POP_TOP
          
-          28         350 POP_EXCEPT
+          23         350 POP_EXCEPT
                      352 JUMP_BACKWARD           68 (to 218)
          
-          27     >>  354 RERAISE                  0
+          22     >>  354 RERAISE                  0
                  >>  356 COPY                     3
                      358 POP_EXCEPT
                      360 RERAISE                  1
          
-          23     >>  362 JUMP_BACKWARD           73 (to 218)
+          18     >>  362 JUMP_BACKWARD           73 (to 218)
          
-          30     >>  364 LOAD_FAST                0 (RP)
+          25     >>  364 LOAD_FAST                0 (RP)
                      366 LOAD_FAST                1 (env)
                      368 BINARY_SUBSCR
                      378 LOAD_FAST                3 (region)
                      380 BINARY_SUBSCR
                      390 POP_JUMP_FORWARD_IF_TRUE     9 (to 410)
          
-          31         392 LOAD_FAST                0 (RP)
+          26         392 LOAD_FAST                0 (RP)
                      394 LOAD_FAST                1 (env)
                      396 BINARY_SUBSCR
                      406 LOAD_FAST                3 (region)
                      408 DELETE_SUBSCR
                  >>  410 JUMP_BACKWARD          111 (to 190)
          
-          32     >>  412 LOAD_FAST                0 (RP)
+          27     >>  412 LOAD_FAST                0 (RP)
                      414 LOAD_FAST                1 (env)
                      416 BINARY_SUBSCR
                      426 POP_JUMP_FORWARD_IF_TRUE     3 (to 434)
          
-          33         428 LOAD_FAST                0 (RP)
+          28         428 LOAD_FAST                0 (RP)
                      430 LOAD_FAST                1 (env)
                      432 DELETE_SUBSCR
                  >>  434 JUMP_BACKWARD          166 (to 104)
          
-          35     >>  436 LOAD_FAST                0 (RP)
+          30     >>  436 LOAD_FAST                0 (RP)
                      438 RETURN_VALUE
          ExceptionTable:
            256 to 326 -> 330 [3]
            330 to 348 -> 356 [4] lasti
            354 to 354 -> 356 [4] lasti
          consts
             None
          names      ('copy', 'deepcopy', 'cfg', 'RP_map', 'list', 'keys', 'mappedvalues', 'getattr', 'Exception')
          varnames   ('RP', 'env', 'rvalue', 'region', 'key')
          freevars   ()
          cellvars   ()
          filename   '/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/cloudformation.py'
          name       'mapping_EnvRegion'
-         firstlineno 16
+         firstlineno 11
          lnotab
             0x020148022201100146011c01200202014c01120104ff08fc02071c0114
             0110010802
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 9
@@ -238,87 +217,87 @@
             0200000000000000000000000000000000000000007c017c017400000000
             000000000000006a03000000000000000064021900000000000000000076
             00720264036e0164047c017400000000000000000000006a030000000000
             0000006405190000000000000000007600720264036e0164047c01740000
             0000000000000000006a0300000000000000006406190000000000000000
             007600720264036e01640464079c036901a6010000ab0100000000000000
             0001008c667c005300
-          38           0 RESUME                   0
+          33           0 RESUME                   0
          
-          39           2 BUILD_MAP                0
+          34           2 BUILD_MAP                0
                        4 STORE_FAST               0 (mappings)
          
-          40           6 BUILD_MAP                0
+          35           6 BUILD_MAP                0
                        8 LOAD_FAST                0 (mappings)
                       10 LOAD_CONST               1 ('InstanceTypes')
                       12 STORE_SUBSCR
          
-          42          16 LOAD_GLOBAL              0 (cfg)
+          37          16 LOAD_GLOBAL              0 (cfg)
                       28 LOAD_ATTR                1 (INSTANCE_LIST)
                       38 GET_ITER
                  >>   40 FOR_ITER               101 (to 244)
                       42 STORE_FAST               1 (i)
          
-          43          44 LOAD_FAST                0 (mappings)
+          38          44 LOAD_FAST                0 (mappings)
                       46 LOAD_CONST               1 ('InstanceTypes')
                       48 BINARY_SUBSCR
                       58 LOAD_METHOD              2 (update)
          
-          45          80 LOAD_FAST                1 (i)
+          40          80 LOAD_FAST                1 (i)
          
-          47          82 LOAD_FAST                1 (i)
+          42          82 LOAD_FAST                1 (i)
                       84 LOAD_GLOBAL              0 (cfg)
                       96 LOAD_ATTR                3 (EPHEMERAL_MAP)
                      106 LOAD_CONST               2 ('InstaceEphemeral0')
                      108 BINARY_SUBSCR
                      118 CONTAINS_OP              0
                      120 POP_JUMP_FORWARD_IF_FALSE     2 (to 126)
          
-          46         122 LOAD_CONST               3 ('1')
+          41         122 LOAD_CONST               3 ('1')
                      124 JUMP_FORWARD             1 (to 128)
          
-          48     >>  126 LOAD_CONST               4 ('0')
+          43     >>  126 LOAD_CONST               4 ('0')
          
-          50     >>  128 LOAD_FAST                1 (i)
+          45     >>  128 LOAD_FAST                1 (i)
                      130 LOAD_GLOBAL              0 (cfg)
                      142 LOAD_ATTR                3 (EPHEMERAL_MAP)
                      152 LOAD_CONST               5 ('InstaceEphemeral1')
                      154 BINARY_SUBSCR
                      164 CONTAINS_OP              0
                      166 POP_JUMP_FORWARD_IF_FALSE     2 (to 172)
          
-          49         168 LOAD_CONST               3 ('1')
+          44         168 LOAD_CONST               3 ('1')
                      170 JUMP_FORWARD             1 (to 174)
          
-          51     >>  172 LOAD_CONST               4 ('0')
+          46     >>  172 LOAD_CONST               4 ('0')
          
-          53     >>  174 LOAD_FAST                1 (i)
+          48     >>  174 LOAD_FAST                1 (i)
                      176 LOAD_GLOBAL              0 (cfg)
                      188 LOAD_ATTR                3 (EPHEMERAL_MAP)
                      198 LOAD_CONST               6 ('InstaceEphemeral2')
                      200 BINARY_SUBSCR
                      210 CONTAINS_OP              0
                      212 POP_JUMP_FORWARD_IF_FALSE     2 (to 218)
          
-          52         214 LOAD_CONST               3 ('1')
+          47         214 LOAD_CONST               3 ('1')
                      216 JUMP_FORWARD             1 (to 220)
          
-          54     >>  218 LOAD_CONST               4 ('0')
+          49     >>  218 LOAD_CONST               4 ('0')
          
-          45     >>  220 LOAD_CONST               7 (('InstaceEphemeral0', 'InstaceEphemeral1', 'InstaceEphemeral2'))
+          40     >>  220 LOAD_CONST               7 (('InstaceEphemeral0', 'InstaceEphemeral1', 'InstaceEphemeral2'))
                      222 BUILD_CONST_KEY_MAP      3
          
-          44         224 BUILD_MAP                1
+          39         224 BUILD_MAP                1
          
-          43         226 PRECALL                  1
+          38         226 PRECALL                  1
                      230 CALL                     1
                      240 POP_TOP
                      242 JUMP_BACKWARD          102 (to 40)
          
-          59     >>  244 LOAD_FAST                0 (mappings)
+          54     >>  244 LOAD_FAST                0 (mappings)
                      246 RETURN_VALUE
          consts
             None
             'InstanceTypes'
             'InstaceEphemeral0'
             '1'
             '0'
@@ -327,15 +306,15 @@
             ('InstaceEphemeral0', 'InstaceEphemeral1', 'InstaceEphemeral2')
          names      ('cfg', 'INSTANCE_LIST', 'update', 'EPHEMERAL_MAP')
          varnames   ('mappings', 'i')
          freevars   ()
          cellvars   ()
          filename   '/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/cloudformation.py'
          name       'mapping_EC2'
-         firstlineno 38
+         firstlineno 33
          lnotab
             0x020104010a021c012402020228ff0402020228ff0402020228ff040202
             f704ff02ff1210
       code
          argcount  : 0
          nlocals   : 6
          stacksize : 6
@@ -349,124 +328,124 @@
             00000000006a0400000000000000006403190000000000000000007c0219
             0000000000000000006404190000000000000000007d046e102300740600
             00000000000000000024007203010059006e047700780359007701740b00
             0000000000000000007c01640519000000000000000000a6010000ab0100
             0000000000000044005d127d057c047c056b0400000000720264066e0164
             077c0364087c059b009d023c0000008c137c037c00640119000000000000
             0000007c023c0000008c8a7c005300
-          62           0 RESUME                   0
+          57           0 RESUME                   0
          
-          63           2 BUILD_MAP                0
+          58           2 BUILD_MAP                0
                        4 STORE_FAST               0 (mappings)
          
-          64           6 BUILD_MAP                0
+          59           6 BUILD_MAP                0
                        8 LOAD_FAST                0 (mappings)
                       10 LOAD_CONST               1 ('AvabilityZones')
                       12 STORE_SUBSCR
          
-          65          16 LOAD_GLOBAL              0 (cfg)
+          60          16 LOAD_GLOBAL              0 (cfg)
                       28 LOAD_ATTR                1 (AZones)
                       38 STORE_FAST               1 (AZ)
          
-          67          40 LOAD_GLOBAL              0 (cfg)
+          62          40 LOAD_GLOBAL              0 (cfg)
                       52 LOAD_ATTR                2 (regions)
                       62 GET_ITER
                  >>   64 FOR_ITER               137 (to 340)
                       66 STORE_FAST               2 (r)
          
-          68          68 BUILD_MAP                0
+          63          68 BUILD_MAP                0
                       70 STORE_FAST               3 (zones)
          
-          69          72 NOP
+          64          72 NOP
          
-          70          74 LOAD_FAST                1 (AZ)
+          65          74 LOAD_FAST                1 (AZ)
                       76 LOAD_FAST                2 (r)
                       78 BINARY_SUBSCR
                       88 STORE_FAST               4 (nzones)
                       90 JUMP_FORWARD            24 (to 140)
                  >>   92 PUSH_EXC_INFO
          
-          71          94 LOAD_GLOBAL              6 (Exception)
+          66          94 LOAD_GLOBAL              6 (Exception)
                      106 CHECK_EXC_MATCH
                      108 POP_JUMP_FORWARD_IF_FALSE    11 (to 132)
                      110 POP_TOP
          
-          72         112 LOAD_FAST                1 (AZ)
+          67         112 LOAD_FAST                1 (AZ)
                      114 LOAD_CONST               2 ('default')
                      116 BINARY_SUBSCR
                      126 STORE_FAST               4 (nzones)
                      128 POP_EXCEPT
                      130 JUMP_FORWARD             4 (to 140)
          
-          71     >>  132 RERAISE                  0
+          66     >>  132 RERAISE                  0
                  >>  134 COPY                     3
                      136 POP_EXCEPT
                      138 RERAISE                  1
          
-          74     >>  140 NOP
+          69     >>  140 NOP
          
-          75         142 LOAD_GLOBAL              0 (cfg)
+          70         142 LOAD_GLOBAL              0 (cfg)
                      154 LOAD_ATTR                4 (RP)
                      164 LOAD_CONST               3 ('dev')
                      166 BINARY_SUBSCR
                      176 LOAD_FAST                2 (r)
                      178 BINARY_SUBSCR
                      188 LOAD_CONST               4 ('AZones')
                      190 BINARY_SUBSCR
                      200 STORE_FAST               4 (nzones)
                      202 JUMP_FORWARD            16 (to 236)
                  >>  204 PUSH_EXC_INFO
          
-          76         206 LOAD_GLOBAL              6 (Exception)
+          71         206 LOAD_GLOBAL              6 (Exception)
                      218 CHECK_EXC_MATCH
                      220 POP_JUMP_FORWARD_IF_FALSE     3 (to 228)
                      222 POP_TOP
          
-          77         224 POP_EXCEPT
+          72         224 POP_EXCEPT
                      226 JUMP_FORWARD             4 (to 236)
          
-          76     >>  228 RERAISE                  0
+          71     >>  228 RERAISE                  0
                  >>  230 COPY                     3
                      232 POP_EXCEPT
                      234 RERAISE                  1
          
-          79     >>  236 LOAD_GLOBAL             11 (NULL + range)
+          74     >>  236 LOAD_GLOBAL             11 (NULL + range)
                      248 LOAD_FAST                1 (AZ)
                      250 LOAD_CONST               5 ('MAX')
                      252 BINARY_SUBSCR
                      262 PRECALL                  1
                      266 CALL                     1
                      276 GET_ITER
                  >>  278 FOR_ITER                18 (to 316)
                      280 STORE_FAST               5 (n)
          
-          80         282 LOAD_FAST                4 (nzones)
+          75         282 LOAD_FAST                4 (nzones)
                      284 LOAD_FAST                5 (n)
                      286 COMPARE_OP               4 (>)
                      292 POP_JUMP_FORWARD_IF_FALSE     2 (to 298)
                      294 LOAD_CONST               6 ('True')
                      296 JUMP_FORWARD             1 (to 300)
                  >>  298 LOAD_CONST               7 ('False')
                  >>  300 LOAD_FAST                3 (zones)
                      302 LOAD_CONST               8 ('Zone')
                      304 LOAD_FAST                5 (n)
                      306 FORMAT_VALUE             0
                      308 BUILD_STRING             2
                      310 STORE_SUBSCR
                      314 JUMP_BACKWARD           19 (to 278)
          
-          82     >>  316 LOAD_FAST                3 (zones)
+          77     >>  316 LOAD_FAST                3 (zones)
                      318 LOAD_FAST                0 (mappings)
                      320 LOAD_CONST               1 ('AvabilityZones')
                      322 BINARY_SUBSCR
                      332 LOAD_FAST                2 (r)
                      334 STORE_SUBSCR
                      338 JUMP_BACKWARD          138 (to 64)
          
-          84     >>  340 LOAD_FAST                0 (mappings)
+          79     >>  340 LOAD_FAST                0 (mappings)
                      342 RETURN_VALUE
          ExceptionTable:
            74 to 88 -> 92 [1]
            92 to 126 -> 134 [2] lasti
            132 to 132 -> 134 [2] lasti
            142 to 200 -> 204 [1]
            204 to 222 -> 230 [2] lasti
@@ -483,407 +462,204 @@
             'Zone'
          names      ('cfg', 'AZones', 'regions', 'Exception', 'RP', 'range')
          varnames   ('mappings', 'AZ', 'r', 'zones', 'nzones', 'n')
          freevars   ()
          cellvars   ()
          filename   '/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/cloudformation.py'
          name       'mapping_AZ'
-         firstlineno 62
+         firstlineno 57
          lnotab
             0x020104010a0118021c01040102011401120114ff080302014001120104
             ff08032e0122021802
       code
          argcount  : 1
-         nlocals   : 1
-         stacksize : 7
-         flags     : 3
-         code
-            0x97007401000000000000000000007403000000000000000000006401a6
-            010000ab0100000000000000007405000000000000000000007406000000
-            000000000000007c00a6020000ab020000000000000000a6020000ab0200
-            00000000000000010064005300
-          87           0 RESUME                   0
-         
-          88           2 LOAD_GLOBAL              1 (NULL + auto_build_obj)
-                      14 LOAD_GLOBAL              3 (NULL + Parameter)
-                      26 LOAD_CONST               1 ('')
-                      28 PRECALL                  1
-                      32 CALL                     1
-                      42 LOAD_GLOBAL              5 (NULL + getattr)
-                      54 LOAD_GLOBAL              6 (cfg)
-                      66 LOAD_FAST                0 (key)
-                      68 PRECALL                  2
-                      72 CALL                     2
-                      82 PRECALL                  2
-                      86 CALL                     2
-                      96 POP_TOP
-                      98 LOAD_CONST               0 (None)
-                     100 RETURN_VALUE
-         consts
-            None
-            ''
-         names      ('auto_build_obj', 'Parameter', 'getattr', 'cfg')
-         varnames   ('key',)
-         freevars   ()
-         cellvars   ()
-         filename   '/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/cloudformation.py'
-         name       'CFM_Parameters'
-         firstlineno 87
-         lnotab 0x0201
-      code
-         argcount  : 1
-         nlocals   : 4
-         stacksize : 5
-         flags     : 3
-         code
-            0x97007401000000000000000000006401a6010000ab0100000000000000
-            0001007403000000000000000000007404000000000000000000007c00a6
-            020000ab020000000000000000a003000000000000000000000000000000
-            0000000000a6000000ab00000000000000000044005d255c0200007d017d
-            027c017409000000000000000000007c02a6010000ab0100000000000000
-            0069017d03740b000000000000000000007c03a6010000ab010000000000
-            00000001008c267401000000000000000000006402a6010000ab01000000
-            0000000000010064005300
-          91           0 RESUME                   0
-         
-          92           2 LOAD_GLOBAL              1 (NULL + do_no_override)
-                      14 LOAD_CONST               1 (True)
-                      16 PRECALL                  1
-                      20 CALL                     1
-                      30 POP_TOP
-         
-          93          32 LOAD_GLOBAL              3 (NULL + getattr)
-                      44 LOAD_GLOBAL              4 (cfg)
-                      56 LOAD_FAST                0 (key)
-                      58 PRECALL                  2
-                      62 CALL                     2
-                      72 LOAD_METHOD              3 (items)
-                      94 PRECALL                  0
-                      98 CALL                     0
-                     108 GET_ITER
-                 >>  110 FOR_ITER                37 (to 186)
-                     112 UNPACK_SEQUENCE          2
-                     116 STORE_FAST               1 (n)
-                     118 STORE_FAST               2 (v)
-         
-          94         120 LOAD_FAST                1 (n)
-                     122 LOAD_GLOBAL              9 (NULL + eval)
-                     134 LOAD_FAST                2 (v)
-                     136 PRECALL                  1
-                     140 CALL                     1
-                     150 BUILD_MAP                1
-                     152 STORE_FAST               3 (c_Condition)
-         
-          96         154 LOAD_GLOBAL             11 (NULL + add_obj)
-                     166 LOAD_FAST                3 (c_Condition)
-                     168 PRECALL                  1
-                     172 CALL                     1
-                     182 POP_TOP
-                     184 JUMP_BACKWARD           38 (to 110)
-         
-          97     >>  186 LOAD_GLOBAL              1 (NULL + do_no_override)
-                     198 LOAD_CONST               2 (False)
-                     200 PRECALL                  1
-                     204 CALL                     1
-                     214 POP_TOP
-                     216 LOAD_CONST               0 (None)
-                     218 RETURN_VALUE
-         consts
-            None
-            True
-            False
-         names      ('do_no_override', 'getattr', 'cfg', 'items', 'eval', 'add_obj')
-         varnames   ('key', 'n', 'v', 'c_Condition')
-         freevars   ()
-         cellvars   ()
-         filename   '/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/cloudformation.py'
-         name       'CFM_Conditions'
-         firstlineno 91
-         lnotab 0x02011e01580122022001
-      code
-         argcount  : 1
          nlocals   : 4
          stacksize : 4
          flags     : 3
          code
             0x97007401000000000000000000007402000000000000000000007c00a6
             020000ab020000000000000000a002000000000000000000000000000000
             0000000000a6000000ab00000000000000000044005d675c0200007d017d
             027c0164016b0200000000720f740700000000000000000000a6000000ab
             0000000000000000007d036e2e7c0164026b0200000000720f7409000000
             00000000000000a6000000ab0000000000000000007d036e197c0164036b
             0200000000720f740b00000000000000000000a6000000ab000000000000
             0000007d036e047c017c0269017d037402000000000000000000006a0600
             00000000000000a00700000000000000000000000000000000000000007c
             03a6010000ab01000000000000000001008c6864005300
-         100           0 RESUME                   0
+          82           0 RESUME                   0
          
-         101           2 LOAD_GLOBAL              1 (NULL + getattr)
+          83           2 LOAD_GLOBAL              1 (NULL + getattr)
                       14 LOAD_GLOBAL              2 (cfg)
                       26 LOAD_FAST                0 (key)
                       28 PRECALL                  2
                       32 CALL                     2
                       42 LOAD_METHOD              2 (items)
                       64 PRECALL                  0
                       68 CALL                     0
                       78 GET_ITER
                  >>   80 FOR_ITER               103 (to 288)
                       82 UNPACK_SEQUENCE          2
                       86 STORE_FAST               1 (n)
                       88 STORE_FAST               2 (v)
          
-         102          90 LOAD_FAST                1 (n)
+          84          90 LOAD_FAST                1 (n)
                       92 LOAD_CONST               1 ('IBoxEnvRegion')
                       94 COMPARE_OP               2 (==)
                      100 POP_JUMP_FORWARD_IF_FALSE    15 (to 132)
          
-         103         102 LOAD_GLOBAL              7 (NULL + mapping_EnvRegion)
+          85         102 LOAD_GLOBAL              7 (NULL + mapping_EnvRegion)
                      114 PRECALL                  0
                      118 CALL                     0
                      128 STORE_FAST               3 (c_Mapping)
                      130 JUMP_FORWARD            46 (to 224)
          
-         104     >>  132 LOAD_FAST                1 (n)
+          86     >>  132 LOAD_FAST                1 (n)
                      134 LOAD_CONST               2 ('IBoxEC2')
                      136 COMPARE_OP               2 (==)
                      142 POP_JUMP_FORWARD_IF_FALSE    15 (to 174)
          
-         105         144 LOAD_GLOBAL              9 (NULL + mapping_EC2)
+          87         144 LOAD_GLOBAL              9 (NULL + mapping_EC2)
                      156 PRECALL                  0
                      160 CALL                     0
                      170 STORE_FAST               3 (c_Mapping)
                      172 JUMP_FORWARD            25 (to 224)
          
-         106     >>  174 LOAD_FAST                1 (n)
+          88     >>  174 LOAD_FAST                1 (n)
                      176 LOAD_CONST               3 ('IBoxAZ')
                      178 COMPARE_OP               2 (==)
                      184 POP_JUMP_FORWARD_IF_FALSE    15 (to 216)
          
-         107         186 LOAD_GLOBAL             11 (NULL + mapping_AZ)
+          89         186 LOAD_GLOBAL             11 (NULL + mapping_AZ)
                      198 PRECALL                  0
                      202 CALL                     0
                      212 STORE_FAST               3 (c_Mapping)
                      214 JUMP_FORWARD             4 (to 224)
          
-         109     >>  216 LOAD_FAST                1 (n)
+          91     >>  216 LOAD_FAST                1 (n)
                      218 LOAD_FAST                2 (v)
                      220 BUILD_MAP                1
                      222 STORE_FAST               3 (c_Mapping)
          
-         111     >>  224 LOAD_GLOBAL              2 (cfg)
+          93     >>  224 LOAD_GLOBAL              2 (cfg)
                      236 LOAD_ATTR                6 (Mappings)
                      246 LOAD_METHOD              7 (update)
                      268 LOAD_FAST                3 (c_Mapping)
                      270 PRECALL                  1
                      274 CALL                     1
                      284 POP_TOP
                      286 JUMP_BACKWARD          104 (to 80)
          
-         101     >>  288 LOAD_CONST               0 (None)
+          83     >>  288 LOAD_CONST               0 (None)
                      290 RETURN_VALUE
          consts
             None
             'IBoxEnvRegion'
             'IBoxEC2'
             'IBoxAZ'
          names      ('getattr', 'cfg', 'items', 'mapping_EnvRegion', 'mapping_EC2', 'mapping_AZ', 'Mappings', 'update')
          varnames   ('key', 'n', 'v', 'c_Mapping')
          freevars   ()
          cellvars   ()
          filename   '/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/cloudformation.py'
          name       'CFM_Mappings'
-         firstlineno 100
+         firstlineno 82
          lnotab 0x020158010c011e010c011e010c011e02080240f6
       code
          argcount  : 1
-         nlocals   : 1
-         stacksize : 7
-         flags     : 3
-         code
-            0x97007401000000000000000000007403000000000000000000006401a6
-            010000ab0100000000000000007405000000000000000000007406000000
-            000000000000007c00a6020000ab020000000000000000a6020000ab0200
-            00000000000000010064005300
-         114           0 RESUME                   0
-         
-         115           2 LOAD_GLOBAL              1 (NULL + auto_build_obj)
-                      14 LOAD_GLOBAL              3 (NULL + Output)
-                      26 LOAD_CONST               1 ('')
-                      28 PRECALL                  1
-                      32 CALL                     1
-                      42 LOAD_GLOBAL              5 (NULL + getattr)
-                      54 LOAD_GLOBAL              6 (cfg)
-                      66 LOAD_FAST                0 (key)
-                      68 PRECALL                  2
-                      72 CALL                     2
-                      82 PRECALL                  2
-                      86 CALL                     2
-                      96 POP_TOP
-                      98 LOAD_CONST               0 (None)
-                     100 RETURN_VALUE
-         consts
-            None
-            ''
-         names      ('auto_build_obj', 'Output', 'getattr', 'cfg')
-         varnames   ('key',)
-         freevars   ()
-         cellvars   ()
-         filename   '/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/cloudformation.py'
-         name       'CFM_Outputs'
-         firstlineno 114
-         lnotab 0x0201
-      code
-         argcount  : 1
-         nlocals   : 7
+         nlocals   : 5
          stacksize : 6
          flags     : 3
          code
-            0x970064017d01740100000000000000000000640264036404ac05a60300
-            00ab0300000000000000007d027403000000000000000000007c02a60100
-            00ab01000000000000000001007405000000000000000000006a03000000
-            00000000007c01a6010000ab0100000000000000007d0364067408000000
-            000000000000006a0500000000000000007600721d64077c035f06000000
-            0000000000740f0000000000000000000064066408a6020000ab02000000
-            00000000007c035f0800000000000000006e147413000000000000000000
-            006406a6010000ab0100000000000000007c035f08000000000000000074
-            08000000000000000000006a0a0000000000000000a00b00000000000000
-            00000000000000000000000000a6000000ab00000000000000000044005d
-            4a5c0200007d047d057c04a00c0000000000000000000000000000000000
-            0000006409a6010000ab0100000000000000007310741b00000000000000
-            0000007c04a6010000ab0100000000000000007d066e0f741d0000000000
-            00000000007c04a6010000ab0100000000000000007d06741f0000000000
-            00000000007c037c047c06a6030000ab03000000000000000001008c4b74
-            03000000000000000000007c03a6010000ab010000000000000000010064
-            005300
-         118           0 RESUME                   0
-         
-         119           2 LOAD_CONST               1 ('CloudFormationCustomResourceStackReplicator')
-                       4 STORE_FAST               1 (resname)
-         
-         121           6 LOAD_GLOBAL              1 (NULL + Parameter)
-         
-         122          18 LOAD_CONST               2 ('CCRReplicateRegions')
-         
-         123          20 LOAD_CONST               3 ('Regions where to replicate - none to disable - empty for default based on env/role')
-         
-         124          22 LOAD_CONST               4 ('CommaDelimitedList')
-         
-         121          24 KW_NAMES                 5
-                      26 PRECALL                  3
-                      30 CALL                     3
-                      40 STORE_FAST               2 (P_ReplicateRegions)
+            0x97007401000000000000000000006a0100000000000000006401a60100
+            00ab0100000000000000007d017405000000000000000000007c01a60100
+            00ab01000000000000000001007406000000000000000000006a04000000
+            0000000000a0050000000000000000000000000000000000000000a60000
+            00ab00000000000000000044005d4a5c0200007d027d037c02a006000000
+            00000000000000000000000000000000006402a6010000ab010000000000
+            0000007310740f000000000000000000007c02a6010000ab010000000000
+            0000007d046e0f7411000000000000000000007c02a6010000ab01000000
+            00000000007d047413000000000000000000007c017c027c04a6030000ab
+            03000000000000000001008c4b7415000000000000000000007c01a60100
+            00ab010000000000000000010064005300
+          96           0 RESUME                   0
+         
+          97           2 LOAD_GLOBAL              1 (NULL + cfm)
+                      14 LOAD_ATTR                1 (CustomResource)
+                      24 LOAD_CONST               1 ('CloudFormationCustomResourceStackReplicator')
+                      26 PRECALL                  1
+                      30 CALL                     1
+                      40 STORE_FAST               1 (R_Replicator)
          
-         127          42 LOAD_GLOBAL              3 (NULL + add_obj)
-                      54 LOAD_FAST                2 (P_ReplicateRegions)
+          98          42 LOAD_GLOBAL              5 (NULL + auto_get_props)
+                      54 LOAD_FAST                1 (R_Replicator)
                       56 PRECALL                  1
                       60 CALL                     1
                       70 POP_TOP
          
-         130          72 LOAD_GLOBAL              5 (NULL + cfm)
-                      84 LOAD_ATTR                3 (CustomResource)
-                      94 LOAD_FAST                1 (resname)
-                      96 PRECALL                  1
-                     100 CALL                     1
-                     110 STORE_FAST               3 (R_Replicator)
-         
-         132         112 LOAD_CONST               6 ('LambdaCCRStackReplicator')
-                     114 LOAD_GLOBAL              8 (cfg)
-                     126 LOAD_ATTR                5 (Resources)
-                     136 CONTAINS_OP              0
-                     138 POP_JUMP_FORWARD_IF_FALSE    29 (to 198)
-         
-         133         140 LOAD_CONST               7 ('IAMPolicyLambdaCCRStackReplicator')
-                     142 LOAD_FAST                3 (R_Replicator)
-                     144 STORE_ATTR               6 (DependsOn)
-         
-         134         154 LOAD_GLOBAL             15 (NULL + GetAtt)
-                     166 LOAD_CONST               6 ('LambdaCCRStackReplicator')
-                     168 LOAD_CONST               8 ('Arn')
-                     170 PRECALL                  2
-                     174 CALL                     2
-                     184 LOAD_FAST                3 (R_Replicator)
-                     186 STORE_ATTR               8 (ServiceToken)
-                     196 JUMP_FORWARD            20 (to 238)
-         
-         136     >>  198 LOAD_GLOBAL             19 (NULL + get_expvalue)
-                     210 LOAD_CONST               6 ('LambdaCCRStackReplicator')
-                     212 PRECALL                  1
-                     216 CALL                     1
-                     226 LOAD_FAST                3 (R_Replicator)
-                     228 STORE_ATTR               8 (ServiceToken)
-         
-         138     >>  238 LOAD_GLOBAL              8 (cfg)
-                     250 LOAD_ATTR               10 (Parameters)
-                     260 LOAD_METHOD             11 (items)
-                     282 PRECALL                  0
-                     286 CALL                     0
-                     296 GET_ITER
-                 >>  298 FOR_ITER                74 (to 448)
-                     300 UNPACK_SEQUENCE          2
-                     304 STORE_FAST               4 (p)
-                     306 STORE_FAST               5 (v)
-         
-         139         308 LOAD_FAST                4 (p)
-                     310 LOAD_METHOD             12 (startswith)
-                     332 LOAD_CONST               9 ('Env')
-                     334 PRECALL                  1
-                     338 CALL                     1
-                     348 POP_JUMP_FORWARD_IF_TRUE    16 (to 382)
-         
-         140         350 LOAD_GLOBAL             27 (NULL + get_endvalue)
-                     362 LOAD_FAST                4 (p)
-                     364 PRECALL                  1
-                     368 CALL                     1
-                     378 STORE_FAST               6 (value)
-                     380 JUMP_FORWARD            15 (to 412)
-         
-         142     >>  382 LOAD_GLOBAL             29 (NULL + Ref)
-                     394 LOAD_FAST                4 (p)
-                     396 PRECALL                  1
-                     400 CALL                     1
-                     410 STORE_FAST               6 (value)
-         
-         143     >>  412 LOAD_GLOBAL             31 (NULL + setattr)
-                     424 LOAD_FAST                3 (R_Replicator)
-                     426 LOAD_FAST                4 (p)
-                     428 LOAD_FAST                6 (value)
-                     430 PRECALL                  3
-                     434 CALL                     3
-                     444 POP_TOP
-                     446 JUMP_BACKWARD           75 (to 298)
-         
-         145     >>  448 LOAD_GLOBAL              3 (NULL + add_obj)
-                     460 LOAD_FAST                3 (R_Replicator)
-                     462 PRECALL                  1
-                     466 CALL                     1
-                     476 POP_TOP
-                     478 LOAD_CONST               0 (None)
-                     480 RETURN_VALUE
+         100          72 LOAD_GLOBAL              6 (cfg)
+                      84 LOAD_ATTR                4 (Parameters)
+                      94 LOAD_METHOD              5 (items)
+                     116 PRECALL                  0
+                     120 CALL                     0
+                     130 GET_ITER
+                 >>  132 FOR_ITER                74 (to 282)
+                     134 UNPACK_SEQUENCE          2
+                     138 STORE_FAST               2 (p)
+                     140 STORE_FAST               3 (v)
+         
+         101         142 LOAD_FAST                2 (p)
+                     144 LOAD_METHOD              6 (startswith)
+                     166 LOAD_CONST               2 ('Env')
+                     168 PRECALL                  1
+                     172 CALL                     1
+                     182 POP_JUMP_FORWARD_IF_TRUE    16 (to 216)
+         
+         102         184 LOAD_GLOBAL             15 (NULL + get_endvalue)
+                     196 LOAD_FAST                2 (p)
+                     198 PRECALL                  1
+                     202 CALL                     1
+                     212 STORE_FAST               4 (value)
+                     214 JUMP_FORWARD            15 (to 246)
+         
+         104     >>  216 LOAD_GLOBAL             17 (NULL + Ref)
+                     228 LOAD_FAST                2 (p)
+                     230 PRECALL                  1
+                     234 CALL                     1
+                     244 STORE_FAST               4 (value)
+         
+         105     >>  246 LOAD_GLOBAL             19 (NULL + setattr)
+                     258 LOAD_FAST                1 (R_Replicator)
+                     260 LOAD_FAST                2 (p)
+                     262 LOAD_FAST                4 (value)
+                     264 PRECALL                  3
+                     268 CALL                     3
+                     278 POP_TOP
+                     280 JUMP_BACKWARD           75 (to 132)
+         
+         107     >>  282 LOAD_GLOBAL             21 (NULL + add_obj)
+                     294 LOAD_FAST                1 (R_Replicator)
+                     296 PRECALL                  1
+                     300 CALL                     1
+                     310 POP_TOP
+                     312 LOAD_CONST               0 (None)
+                     314 RETURN_VALUE
          consts
             None
             'CloudFormationCustomResourceStackReplicator'
-            'CCRReplicateRegions'
-            'Regions where to replicate - none to disable - empty for default based on env/role'
-            'CommaDelimitedList'
-            ('Description', 'Type')
-            'LambdaCCRStackReplicator'
-            'IAMPolicyLambdaCCRStackReplicator'
-            'Arn'
             'Env'
-         names      ('Parameter', 'add_obj', 'cfm', 'CustomResource', 'cfg', 'Resources', 'DependsOn', 'GetAtt', 'ServiceToken', 'get_expvalue', 'Parameters', 'items', 'startswith', 'get_endvalue', 'Ref', 'setattr')
-         varnames   ('key', 'resname', 'P_ReplicateRegions', 'R_Replicator', 'p', 'v', 'value')
+         names      ('cfm', 'CustomResource', 'auto_get_props', 'cfg', 'Parameters', 'items', 'startswith', 'get_endvalue', 'Ref', 'setattr', 'add_obj')
+         varnames   ('key', 'R_Replicator', 'p', 'v', 'value')
          freevars   ()
          cellvars   ()
          filename   '/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/cloudformation.py'
          name       'CFM_CustomResourceReplicator'
-         firstlineno 118
-         lnotab
-            0x020104020c010201020102fd12061e0328021c010e012c02280246012a
-            0120021e012402
-   names      ('troposphere.cloudformation', 'cloudformation', 'cfm', 'common', 'shared', 'Parameter', 'do_no_override', 'get_endvalue', 'get_expvalue', 'get_condition', 'add_obj', 'auto_build_obj', 'mapping_EnvRegion', 'mapping_EC2', 'mapping_AZ', 'CFM_Parameters', 'CFM_Conditions', 'CFM_Mappings', 'CFM_Outputs', 'CFM_CustomResourceReplicator')
+         firstlineno 96
+         lnotab 0x020128011e0246012a0120021e012402
+   names      ('troposphere.cloudformation', 'cloudformation', 'cfm', 'common', 'shared', 'get_endvalue', 'add_obj', 'auto_get_props', 'mapping_EnvRegion', 'mapping_EC2', 'mapping_AZ', 'CFM_Mappings', 'CFM_CustomResourceReplicator')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/mello/Private/Documenti/work/repos/AwsIBox/awsibox/mod/cloudformation.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c020801240c06160618061906040609060e0604
+   lnotab 0x00ff02010c0208011407061606180619060e
```

### Comparing `awsibox-0.8.9/awsibox/mod/__pycache__/cloudfront.cpython-311.pyc` & `awsibox-0.9.1/awsibox/mod/__pycache__/cloudfront.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/mod/__pycache__/elasticloadbalancing.cpython-311.pyc` & `awsibox-0.9.1/awsibox/mod/__pycache__/elasticloadbalancing.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/mod/__pycache__/iam.cpython-311.pyc` & `awsibox-0.9.1/awsibox/mod/__pycache__/iam.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/mod/__pycache__/rds.cpython-311.pyc` & `awsibox-0.9.1/awsibox/mod/__pycache__/rds.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/mod/__pycache__/s3.cpython-311.pyc` & `awsibox-0.9.1/awsibox/mod/__pycache__/s3.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/mod/__pycache__/waf.cpython-311.pyc` & `awsibox-0.9.1/awsibox/mod/__pycache__/waf.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/mod/autoscaling.py` & `awsibox-0.9.1/awsibox/mod/autoscaling.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/mod/cloudformation.py` & `awsibox-0.9.1/awsibox/mod/cloudformation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import troposphere.cloudformation as cfm
 
 from ..common import *
 from ..shared import (
-    do_no_override,
     get_endvalue,
-    get_expvalue,
-    # need it even if not directly used cause eval in CFM_Conditions
-    get_condition,
     add_obj,
+    auto_get_props
 )
 
 
 def mapping_EnvRegion():
     RP = copy.deepcopy(cfg.RP_map)
 
     for env in list(RP):
@@ -78,23 +75,14 @@
             zones[f"Zone{n}"] = "True" if nzones > n else "False"
 
         mappings["AvabilityZones"][r] = zones
 
     return mappings
 
 
-def CFM_Conditions(key):
-    do_no_override(True)
-    for n, v in getattr(cfg, key).items():
-        c_Condition = {n: eval(v)}
-
-        add_obj(c_Condition)
-    do_no_override(False)
-
-
 def CFM_Mappings(key):
     for n, v in getattr(cfg, key).items():
         if n == "IBoxEnvRegion":
             c_Mapping = mapping_EnvRegion()
         elif n == "IBoxEC2":
             c_Mapping = mapping_EC2()
         elif n == "IBoxAZ":
@@ -102,32 +90,16 @@
         else:
             c_Mapping = {n: v}
 
         cfg.Mappings.update(c_Mapping)
 
 
 def CFM_CustomResourceReplicator(key):
-    resname = "CloudFormationCustomResourceStackReplicator"
-    # Parameters
-    P_ReplicateRegions = Parameter(
-        "CCRReplicateRegions",
-        Description="Regions where to replicate - none to disable - empty for default based on env/role",
-        Type="CommaDelimitedList",
-    )
-
-    add_obj(P_ReplicateRegions)
-
-    # Resources
-    R_Replicator = cfm.CustomResource(resname)
-
-    if "LambdaCCRStackReplicator" in cfg.Resources:
-        R_Replicator.DependsOn = "IAMPolicyLambdaCCRStackReplicator"
-        R_Replicator.ServiceToken = GetAtt("LambdaCCRStackReplicator", "Arn")
-    else:
-        R_Replicator.ServiceToken = get_expvalue("LambdaCCRStackReplicator")
+    R_Replicator = cfm.CustomResource("CloudFormationCustomResourceStackReplicator")
+    auto_get_props(R_Replicator)
 
     for p, v in cfg.Parameters.items():
         if not p.startswith("Env"):
             value = get_endvalue(p)
         else:
             value = Ref(p)
         setattr(R_Replicator, p, value)
```

### Comparing `awsibox-0.8.9/awsibox/mod/cloudfront.py` & `awsibox-0.9.1/awsibox/mod/cloudfront.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/mod/ec2.py` & `awsibox-0.9.1/awsibox/mod/ec2.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/mod/joker.py` & `awsibox-0.9.1/awsibox/mod/joker.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 from ..common import *
-from ..shared import auto_get_props, add_obj, get_condition, parse_ibox_key
+from ..shared import (
+    auto_get_props,
+    add_obj,
+    do_no_override,
+    get_condition,
+    get_endvalue,
+    parse_ibox_key,
+)
 from ..RP import RP_to_cfg, merge_dict
 
 
 def Joker(key, module, cls):
     for n, v in getattr(cfg, key).items():
+        if key == "Condition":
+            # Condition are just dict, directly add them
+            do_no_override(True)
+            add_obj({n: eval(v)})
+            do_no_override(False)
+            continue
+
         if not v.get("IBOX_ENABLED", True):
             continue
         if not eval(v.get("IBOX_ENABLED_IF", "True")):
             continue
 
         parse_ibox_key_conf = {"IBOX_INDEXNAME": n}
         resname = f"{key}{n}"
```

### Comparing `awsibox-0.8.9/awsibox/shared.py` & `awsibox-0.9.1/awsibox/shared.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 IBOX_SPECIAL_KEYS = (
     "IBOX_RESNAME",
     "IBOX_MAPNAME",
     "IBOX_REMAPNAME",
     "IBOX_INDEXNAME",
     "IBOX_PROPNAME",
     "IBOX_CURNAME",
+    "IBOX_CURMAP",
     "IBOX_REFNAME",
     "IBOX_TITLE",
     "IBOX_LINKED_OBJ_NAME",
     "IBOX_LINKED_OBJ_INDEX",
     "IBOX_LINKED_OBJ_FOR",
 )
 
@@ -616,26 +617,32 @@
             return obj_tags
 
         obj_class = obj.__class__.__name__
         obj_mod_name = obj.__module__
         prop_class = props.get(obj_propname, [None])[0]
         # print(f"TYPE: {res_obj_type}, CLASS: {obj_class}, PROP: {obj_propname}")
 
-        # detect attributes as CreationPolicy not included in obj properties
         if obj_propname in ["CreationPolicy", "UpdatePolicy"]:
+            # detect attributes as CreationPolicy not included in obj properties
             prop_class = getattr(policies, obj_propname)
         elif callable(prop_class) and prop_class.__name__ not in [
             "validate_variables_name",
             "policytypes",
         ]:
-            # prop_class is a method fallback and try to use CloudFormationResourceSpecification
-            if res_obj_type in cfg.TROPO_CLASS_TO_CFM:
-                obj_class = cfg.TROPO_CLASS_TO_CFM[res_obj_type].get(
-                    obj_class, obj_class
-                )
+            # find out if troposphere class names differ from cloudformation ones
+            tropo_class_map = cfg.TROPO_CLASS_TO_CFM.get(res_obj_type, {})
+
+            if obj_class in tropo_class_map:
+                # obj_class is tropo class and i need to found out cfm class
+                obj_class = tropo_class_map[obj_class]
+                tropo_to_cfm = True
+            else:
+                tropo_to_cfm = False
+
+            # use CloudFormationResourceSpecification to find out class names
             try:
                 res_obj_propname = cfg.cfm_res_spec["PropertyTypes"][
                     f"{res_obj_type}.{obj_class}"
                 ]["Properties"][obj_propname]
             except Exception:
                 try:
                     res_obj_propname = cfg.cfm_res_spec["ResourceTypes"][res_obj_type][
@@ -649,14 +656,21 @@
                 prop_class_type = res_obj_propname.get("ItemType")
                 if not prop_class_type:
                     prop_class_type = obj_prop_type
                 if not prop_class_type:
                     prop_class_type = res_obj_propname.get("PrimitiveType")
 
                 # print(f"PROP_CLASS_TYPE: {prop_class_type}")
+
+                if not tropo_to_cfm and obj_class in tropo_class_map.values():
+                    # obj_class is cfm class and i need to directly get tropo class
+                    prop_class_type = next(
+                        (k for k, v in tropo_class_map.items() if v == obj_class), None
+                    )
+
                 try:
                     prop_class = getattr(sys.modules[obj_mod_name], prop_class_type)
                 except Exception:
                     pass
                 else:
                     if obj_prop_type == "List":
                         prop_class = [prop_class]
@@ -759,15 +773,15 @@
         ) or (
             callable(prop_class)
             and prop_class.__name__ in ["policytypes", "validate_variables_name"]
         ):
             return get_dictvalue(key[obj_propname])
 
     def _populate(obj, key=None, mapname=None, rootdict=None):
-        global IBOX_RESNAME, IBOX_CURNAME, IBOX_REFNAME, IBOX_TITLE
+        global IBOX_RESNAME, IBOX_CURNAME, IBOX_CURMAP, IBOX_REFNAME, IBOX_TITLE
 
         if not mapname:
             mapname = obj.title
         if rootdict:
             key = rootdict
             mapname = ""
         if not key:
@@ -917,16 +931,16 @@
                 else:
                     values.append(value)
             return values
 
         def _linked_obj(linked_obj_data):
             # need to parse them here to have the right values
             lo_name = parse_ibox_key(linked_obj_data.get("Name", IBOX_RESNAME))
-            lo_key = parse_ibox_key(linked_obj_data.get("Key", ""))
-            lo_type = parse_ibox_key(linked_obj_data.get("Type", ""))
+            lo_key = parse_ibox_key(linked_obj_data["Key"])
+            lo_type = parse_ibox_key(linked_obj_data["Type"])
             if not lo_type:
                 return
             # this way even if without key "For", for cycle will run at least one time
             lo_for_cycle = parse_ibox_key(linked_obj_data.get("For", [""]))
 
             louc_cfg = {}
             for lo_for_index in lo_for_cycle:
@@ -988,15 +1002,19 @@
         props = list(vars(obj)["propnames"])
         props.extend(vars(obj)["attributes"])
 
         # needed by IBOX_BASE used on Resource Properties
         if key.get("IBOX_BASE_REF"):
             IBOX_REFNAME = mapname
 
-        # Parameters, Conditions, Outpus in yaml cfg
+        # set mapname before processing Parameters, Conditions, Outputs
+        if mapname:
+            IBOX_CURMAP = mapname
+
+        # Parameters, Conditions, Outputs in yaml cfg
         _try_PCO_in_obj(key)
 
         # For linked resources as r53recordset, update their keys conf.
         # This way they can be enabled or their name can be changed, or so on...
         ibox_linked_obj = key.get("IBOX_LINKED_OBJ")
         if ibox_linked_obj:
             # bad hack to use a dict for ibox_linked_obj, so that i can modify it if needed using the index name
@@ -1148,14 +1166,15 @@
                 if ibox_auto_po in key:
                     ibox_auto_po_value = key[ibox_auto_po]
                     _auto_PO(propname, ibox_auto_po_value, "o", value)
 
         # need to redefine it here because it's has been changed by nested supprop
         if not isinstance(obj, (Output, Parameter, Condition)):
             IBOX_CURNAME = mapname
+            IBOX_CURMAP = mapname
 
         # title override
         try:
             obj.title = parse_ibox_key(key["IBOX_TITLE"])
         except Exception:
             pass
```

### Comparing `awsibox-0.8.9/awsibox/user-data/SCRIPTS/ELBCHECK.sh` & `awsibox-0.9.1/awsibox/user-data/SCRIPTS/ELBCHECK.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/user-data/SCRIPTS/END.sh` & `awsibox-0.9.1/awsibox/user-data/SCRIPTS/END.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/user-data/SCRIPTS/INIT.sh` & `awsibox-0.9.1/awsibox/user-data/SCRIPTS/INIT.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/user-data/SCRIPTS/PACKAGE.sh` & `awsibox-0.9.1/awsibox/user-data/SCRIPTS/PACKAGE.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/user-data/SCRIPTS/SERVICE.sh` & `awsibox-0.9.1/awsibox/user-data/SCRIPTS/SERVICE.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/user-data/SCRIPTS/SETUP.sh` & `awsibox-0.9.1/awsibox/user-data/SCRIPTS/SETUP.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/awsibox/user-data/ecs-cluster.sh` & `awsibox-0.9.1/awsibox/user-data/ecs-cluster.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/build/lib/awsibox.egg-info/PKG-INFO` & `awsibox-0.9.1/build/lib/awsibox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsibox
-Version: 0.8.9
+Version: 0.9.1
 Summary: AWS Infrastructure in a Box
 Home-page: https://github.com/mello7tre/AwsIBox
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Open Software License 3.0 (OSL-3.0)
```

### Comparing `awsibox-0.8.9/build/lib/awsibox.egg-info/SOURCES.txt` & `awsibox-0.9.1/build/lib/awsibox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/scripts/ibox_generate_templates.py` & `awsibox-0.9.1/scripts/ibox_generate_templates.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/setup.cfg` & `awsibox-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.9/setup.py` & `awsibox-0.9.1/setup.py`

 * *Files identical despite different names*

