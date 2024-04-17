# Comparing `tmp/iac_init-0.3.6.tar.gz` & `tmp/iac_init-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_init-0.3.6.tar", max compression
+gzip compressed data, was "iac_init-0.3.7.tar", max compression
```

## Comparing `iac_init-0.3.6.tar` & `iac_init-0.3.7.tar`

### file list

```diff
@@ -1,94 +1,94 @@
--rw-r--r--   0        0        0    16295 2024-04-17 05:10:41.110518 iac_init-0.3.6/LICENSE
--rw-r--r--   0        0        0        0 2024-04-17 05:10:41.110518 iac_init-0.3.6/README.md
--rw-r--r--   0        0        0      389 2024-04-17 05:10:41.110518 iac_init-0.3.6/iac_init/__init__.py
--rw-r--r--   0        0        0      162 2024-04-17 05:10:41.110518 iac_init-0.3.6/iac_init/__main__.py
--rw-r--r--   0        0        0     3993 2024-04-17 05:10:41.110518 iac_init-0.3.6/iac_init/cli/__pycache__/main.cpython-310.pyc
--rw-r--r--   0        0        0      265 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/cli/__pycache__/options.cpython-310.pyc
--rw-r--r--   0        0        0     5830 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/cli/main.py
--rw-r--r--   0        0        0      206 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/cli/options.py
--rw-r--r--   0        0        0     2064 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/conf/__init__.py
--rw-r--r--   0        0        0     2564 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/conf/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1656 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/conf/__pycache__/global_settings.cpython-310.pyc
--rw-r--r--   0        0        0     2054 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/conf/global_settings.py
--rw-r--r--   0        0        0      887 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/scripts/__pycache__/ansible_tool.cpython-310.pyc
--rw-r--r--   0        0        0     1981 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/scripts/__pycache__/apic_connecton_tool.cpython-310.pyc
--rw-r--r--   0        0        0     1337 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/scripts/__pycache__/create_threadingpool.cpython-310.pyc
--rw-r--r--   0        0        0     1185 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/scripts/__pycache__/log_tool.cpython-310.pyc
--rw-r--r--   0        0        0      551 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/scripts/__pycache__/ssh_tool.cpython-310.pyc
--rw-r--r--   0        0        0      403 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/scripts/__pycache__/telnet_tool.cpython-310.pyc
--rw-r--r--   0        0        0      747 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/scripts/ansible_tool.py
--rw-r--r--   0        0        0     2595 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/scripts/apic_connecton_tool.py
--rw-r--r--   0        0        0     6788 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/scripts/cimc_precheck_tool.py
--rw-r--r--   0        0        0      452 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/scripts/ssh_tool.py
--rw-r--r--   0        0        0      263 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/scripts/telnet_tool.py
--rw-r--r--   0        0        0      388 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/03-node_registration/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/06-fabric_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 05:10:41.114518 iac_init-0.3.6/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/07-access_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/09-smart_licensing/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/10-confg_aaa/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/11-config_monitor/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/templates/12-config_backup/inventory.yaml.j2
--rw-r--r--   0        0        0      370 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/utils/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0        0        0     3446 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/utils/__pycache__/functional.cpython-310.pyc
--rw-r--r--   0        0        0      101 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/utils/exceptions.py
--rw-r--r--   0        0        0     4910 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/utils/functional.py
--rw-r--r--   0        0        0    10407 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/validator.py
--rw-r--r--   0        0        0     4138 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/yaml_conf/__pycache__/yaml.cpython-310.pyc
--rw-r--r--   0        0        0     4043 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/yaml_conf/__pycache__/yaml_writer.cpython-310.pyc
--rw-r--r--   0        0        0     5093 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/yaml_conf/yaml.py
--rw-r--r--   0        0        0     5222 2024-04-17 05:10:41.118518 iac_init-0.3.6/iac_init/yaml_conf/yaml_writer.py
--rw-r--r--   0        0        0     1601 2024-04-17 05:10:41.122518 iac_init-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 iac_init-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-04-17 05:18:57.073058 iac_init-0.3.7/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-17 05:18:57.073058 iac_init-0.3.7/README.md
+-rw-r--r--   0        0        0      389 2024-04-17 05:18:57.073058 iac_init-0.3.7/iac_init/__init__.py
+-rw-r--r--   0        0        0      162 2024-04-17 05:18:57.073058 iac_init-0.3.7/iac_init/__main__.py
+-rw-r--r--   0        0        0     3993 2024-04-17 05:18:57.073058 iac_init-0.3.7/iac_init/cli/__pycache__/main.cpython-310.pyc
+-rw-r--r--   0        0        0      265 2024-04-17 05:18:57.073058 iac_init-0.3.7/iac_init/cli/__pycache__/options.cpython-310.pyc
+-rw-r--r--   0        0        0     5830 2024-04-17 05:18:57.073058 iac_init-0.3.7/iac_init/cli/main.py
+-rw-r--r--   0        0        0      206 2024-04-17 05:18:57.073058 iac_init-0.3.7/iac_init/cli/options.py
+-rw-r--r--   0        0        0     2064 2024-04-17 05:18:57.073058 iac_init-0.3.7/iac_init/conf/__init__.py
+-rw-r--r--   0        0        0     2564 2024-04-17 05:18:57.073058 iac_init-0.3.7/iac_init/conf/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1656 2024-04-17 05:18:57.073058 iac_init-0.3.7/iac_init/conf/__pycache__/global_settings.cpython-310.pyc
+-rw-r--r--   0        0        0     2057 2024-04-17 05:18:57.073058 iac_init-0.3.7/iac_init/conf/global_settings.py
+-rw-r--r--   0        0        0      887 2024-04-17 05:18:57.073058 iac_init-0.3.7/iac_init/scripts/__pycache__/ansible_tool.cpython-310.pyc
+-rw-r--r--   0        0        0     1981 2024-04-17 05:18:57.073058 iac_init-0.3.7/iac_init/scripts/__pycache__/apic_connecton_tool.cpython-310.pyc
+-rw-r--r--   0        0        0     1337 2024-04-17 05:18:57.073058 iac_init-0.3.7/iac_init/scripts/__pycache__/create_threadingpool.cpython-310.pyc
+-rw-r--r--   0        0        0     1185 2024-04-17 05:18:57.073058 iac_init-0.3.7/iac_init/scripts/__pycache__/log_tool.cpython-310.pyc
+-rw-r--r--   0        0        0      551 2024-04-17 05:18:57.073058 iac_init-0.3.7/iac_init/scripts/__pycache__/ssh_tool.cpython-310.pyc
+-rw-r--r--   0        0        0      403 2024-04-17 05:18:57.073058 iac_init-0.3.7/iac_init/scripts/__pycache__/telnet_tool.cpython-310.pyc
+-rw-r--r--   0        0        0      747 2024-04-17 05:18:57.073058 iac_init-0.3.7/iac_init/scripts/ansible_tool.py
+-rw-r--r--   0        0        0     2595 2024-04-17 05:18:57.073058 iac_init-0.3.7/iac_init/scripts/apic_connecton_tool.py
+-rw-r--r--   0        0        0     6788 2024-04-17 05:18:57.073058 iac_init-0.3.7/iac_init/scripts/cimc_precheck_tool.py
+-rw-r--r--   0        0        0      452 2024-04-17 05:18:57.073058 iac_init-0.3.7/iac_init/scripts/ssh_tool.py
+-rw-r--r--   0        0        0      263 2024-04-17 05:18:57.073058 iac_init-0.3.7/iac_init/scripts/telnet_tool.py
+-rw-r--r--   0        0        0      388 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/03-node_registration/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/06-fabric_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/07-access_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/09-smart_licensing/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 05:18:57.077057 iac_init-0.3.7/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 05:18:57.081057 iac_init-0.3.7/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 05:18:57.081057 iac_init-0.3.7/iac_init/templates/10-confg_aaa/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 05:18:57.081057 iac_init-0.3.7/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 05:18:57.081057 iac_init-0.3.7/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 05:18:57.081057 iac_init-0.3.7/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 05:18:57.081057 iac_init-0.3.7/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 05:18:57.081057 iac_init-0.3.7/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 05:18:57.081057 iac_init-0.3.7/iac_init/templates/11-config_monitor/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 05:18:57.081057 iac_init-0.3.7/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 05:18:57.081057 iac_init-0.3.7/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 05:18:57.081057 iac_init-0.3.7/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 05:18:57.081057 iac_init-0.3.7/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 05:18:57.081057 iac_init-0.3.7/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 05:18:57.081057 iac_init-0.3.7/iac_init/templates/12-config_backup/inventory.yaml.j2
+-rw-r--r--   0        0        0      370 2024-04-17 05:18:57.081057 iac_init-0.3.7/iac_init/utils/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0        0        0     3446 2024-04-17 05:18:57.081057 iac_init-0.3.7/iac_init/utils/__pycache__/functional.cpython-310.pyc
+-rw-r--r--   0        0        0      101 2024-04-17 05:18:57.081057 iac_init-0.3.7/iac_init/utils/exceptions.py
+-rw-r--r--   0        0        0     4910 2024-04-17 05:18:57.081057 iac_init-0.3.7/iac_init/utils/functional.py
+-rw-r--r--   0        0        0    10407 2024-04-17 05:18:57.081057 iac_init-0.3.7/iac_init/validator.py
+-rw-r--r--   0        0        0     4138 2024-04-17 05:18:57.081057 iac_init-0.3.7/iac_init/yaml_conf/__pycache__/yaml.cpython-310.pyc
+-rw-r--r--   0        0        0     4043 2024-04-17 05:18:57.081057 iac_init-0.3.7/iac_init/yaml_conf/__pycache__/yaml_writer.cpython-310.pyc
+-rw-r--r--   0        0        0     5093 2024-04-17 05:18:57.081057 iac_init-0.3.7/iac_init/yaml_conf/yaml.py
+-rw-r--r--   0        0        0     5222 2024-04-17 05:18:57.081057 iac_init-0.3.7/iac_init/yaml_conf/yaml_writer.py
+-rw-r--r--   0        0        0     1601 2024-04-17 05:18:57.081057 iac_init-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 iac_init-0.3.7/PKG-INFO
```

### Comparing `iac_init-0.3.6/LICENSE` & `iac_init-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.6/iac_init/cli/__pycache__/main.cpython-310.pyc` & `iac_init-0.3.7/iac_init/cli/__pycache__/main.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.6/iac_init/cli/main.py` & `iac_init-0.3.7/iac_init/cli/main.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.6/iac_init/conf/__init__.py` & `iac_init-0.3.7/iac_init/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.6/iac_init/conf/__pycache__/__init__.cpython-310.pyc` & `iac_init-0.3.7/iac_init/conf/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.6/iac_init/conf/__pycache__/global_settings.cpython-310.pyc` & `iac_init-0.3.7/iac_init/conf/__pycache__/global_settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.6/iac_init/conf/global_settings.py` & `iac_init-0.3.7/iac_init/conf/global_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright: (c) 2022, Wang Xiao <xiawang3@cisco.com>
 
 import os.path
 from pathlib import Path
 
 BASE_DIR = Path(__file__).resolve().parent.parent
 
-OUTPUT_BASE_DIR = os.path.join(BASE_DIR, "iac_init_output_working_dir")
+OUTPUT_BASE_DIR = os.path.join(os.getcwd(), "iac_init_output_working_dir")
 
 DEFAULT_USER_OPTIONS = [
     "Wipe an ACI fabric/PXE boot(APIC + Switch).",
     "Discovery an ACI fabric APIC(Single Pod, MultiPod, MultiSite, RemoteLeaf).",
     "ACI fabric Node Registration(NaC starts from here).",
     "Configure ACI OOB Mgmt address.",
     "Configure ACI system settings.",
```

### Comparing `iac_init-0.3.6/iac_init/scripts/__pycache__/ansible_tool.cpython-310.pyc` & `iac_init-0.3.7/iac_init/scripts/__pycache__/ansible_tool.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.6/iac_init/scripts/__pycache__/apic_connecton_tool.cpython-310.pyc` & `iac_init-0.3.7/iac_init/scripts/__pycache__/apic_connecton_tool.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.6/iac_init/scripts/__pycache__/create_threadingpool.cpython-310.pyc` & `iac_init-0.3.7/iac_init/scripts/__pycache__/create_threadingpool.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.6/iac_init/scripts/__pycache__/log_tool.cpython-310.pyc` & `iac_init-0.3.7/iac_init/scripts/__pycache__/log_tool.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.6/iac_init/scripts/__pycache__/ssh_tool.cpython-310.pyc` & `iac_init-0.3.7/iac_init/scripts/__pycache__/ssh_tool.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.6/iac_init/scripts/ansible_tool.py` & `iac_init-0.3.7/iac_init/scripts/ansible_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.6/iac_init/scripts/apic_connecton_tool.py` & `iac_init-0.3.7/iac_init/scripts/apic_connecton_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.6/iac_init/scripts/cimc_precheck_tool.py` & `iac_init-0.3.7/iac_init/scripts/cimc_precheck_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.6/iac_init/utils/__pycache__/functional.cpython-310.pyc` & `iac_init-0.3.7/iac_init/utils/__pycache__/functional.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.6/iac_init/utils/functional.py` & `iac_init-0.3.7/iac_init/utils/functional.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.6/iac_init/validator.py` & `iac_init-0.3.7/iac_init/validator.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.6/iac_init/yaml_conf/__pycache__/yaml.cpython-310.pyc` & `iac_init-0.3.7/iac_init/yaml_conf/__pycache__/yaml.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.6/iac_init/yaml_conf/__pycache__/yaml_writer.cpython-310.pyc` & `iac_init-0.3.7/iac_init/yaml_conf/__pycache__/yaml_writer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.6/iac_init/yaml_conf/yaml.py` & `iac_init-0.3.7/iac_init/yaml_conf/yaml.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.6/iac_init/yaml_conf/yaml_writer.py` & `iac_init-0.3.7/iac_init/yaml_conf/yaml_writer.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.6/pyproject.toml` & `iac_init-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iac-init"
-version = "0.3.6"
+version = "0.3.7"
 description = ""
 authors = ["Wang Xiao <xiawang3@cisco.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 iac-init = "iac_init.cli.main:main"
```

### Comparing `iac_init-0.3.6/PKG-INFO` & `iac_init-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-init
-Version: 0.3.6
+Version: 0.3.7
 Summary: 
 Author: Wang Xiao
 Author-email: xiawang3@cisco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

