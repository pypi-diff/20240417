# Comparing `tmp/iac_init-0.3.9.tar.gz` & `tmp/iac_init-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_init-0.3.9.tar", max compression
+gzip compressed data, was "iac_init-0.4.0.tar", max compression
```

## Comparing `iac_init-0.3.9.tar` & `iac_init-0.4.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
--rw-r--r--   0        0        0    16295 2024-04-17 08:04:48.224080 iac_init-0.3.9/LICENSE
--rw-r--r--   0        0        0        0 2024-04-17 08:04:48.224080 iac_init-0.3.9/README.md
--rw-r--r--   0        0        0      389 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/__init__.py
--rw-r--r--   0        0        0      162 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/__main__.py
--rw-r--r--   0        0        0     3993 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/cli/__pycache__/main.cpython-310.pyc
--rw-r--r--   0        0        0      265 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/cli/__pycache__/options.cpython-310.pyc
--rw-r--r--   0        0        0     5833 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/cli/main.py
--rw-r--r--   0        0        0      206 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/cli/options.py
--rw-r--r--   0        0        0     2064 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/conf/__init__.py
--rw-r--r--   0        0        0     2564 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/conf/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1656 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/conf/__pycache__/global_settings.cpython-310.pyc
--rw-r--r--   0        0        0     2057 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/conf/global_settings.py
--rw-r--r--   0        0        0      887 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/scripts/__pycache__/ansible_tool.cpython-310.pyc
--rw-r--r--   0        0        0     1981 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/scripts/__pycache__/apic_connecton_tool.cpython-310.pyc
--rw-r--r--   0        0        0     1337 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/scripts/__pycache__/create_threadingpool.cpython-310.pyc
--rw-r--r--   0        0        0     1185 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/scripts/__pycache__/log_tool.cpython-310.pyc
--rw-r--r--   0        0        0      551 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/scripts/__pycache__/ssh_tool.cpython-310.pyc
--rw-r--r--   0        0        0      403 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/scripts/__pycache__/telnet_tool.cpython-310.pyc
--rw-r--r--   0        0        0      747 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/scripts/ansible_tool.py
--rw-r--r--   0        0        0     2595 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/scripts/apic_connecton_tool.py
--rw-r--r--   0        0        0     6788 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/scripts/cimc_precheck_tool.py
--rw-r--r--   0        0        0      452 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/scripts/ssh_tool.py
--rw-r--r--   0        0        0      263 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/scripts/telnet_tool.py
--rw-r--r--   0        0        0      388 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/templates/03-node_registration/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 08:04:48.224080 iac_init-0.3.9/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/06-fabric_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/07-access_policy/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/09-smart_licensing/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/10-confg_aaa/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/11-config_monitor/inventory.yaml.j2
--rw-r--r--   0        0        0      388 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/templates/12-config_backup/inventory.yaml.j2
--rw-r--r--   0        0        0      370 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/utils/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0        0        0     3446 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/utils/__pycache__/functional.cpython-310.pyc
--rw-r--r--   0        0        0      101 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/utils/exceptions.py
--rw-r--r--   0        0        0     4910 2024-04-17 08:04:48.228080 iac_init-0.3.9/iac_init/utils/functional.py
--rw-r--r--   0        0        0    10421 2024-04-17 08:04:48.232080 iac_init-0.3.9/iac_init/validator.py
--rw-r--r--   0        0        0     4138 2024-04-17 08:04:48.232080 iac_init-0.3.9/iac_init/yaml_conf/__pycache__/yaml.cpython-310.pyc
--rw-r--r--   0        0        0     4043 2024-04-17 08:04:48.232080 iac_init-0.3.9/iac_init/yaml_conf/__pycache__/yaml_writer.cpython-310.pyc
--rw-r--r--   0        0        0     5093 2024-04-17 08:04:48.232080 iac_init-0.3.9/iac_init/yaml_conf/yaml.py
--rw-r--r--   0        0        0     5222 2024-04-17 08:04:48.232080 iac_init-0.3.9/iac_init/yaml_conf/yaml_writer.py
--rw-r--r--   0        0        0     1601 2024-04-17 08:04:48.232080 iac_init-0.3.9/pyproject.toml
--rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 iac_init-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-04-17 08:52:09.822073 iac_init-0.4.0/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-17 08:52:09.822073 iac_init-0.4.0/README.md
+-rw-r--r--   0        0        0      389 2024-04-17 08:52:09.822073 iac_init-0.4.0/iac_init/__init__.py
+-rw-r--r--   0        0        0      162 2024-04-17 08:52:09.822073 iac_init-0.4.0/iac_init/__main__.py
+-rw-r--r--   0        0        0     3993 2024-04-17 08:52:09.822073 iac_init-0.4.0/iac_init/cli/__pycache__/main.cpython-310.pyc
+-rw-r--r--   0        0        0      265 2024-04-17 08:52:09.822073 iac_init-0.4.0/iac_init/cli/__pycache__/options.cpython-310.pyc
+-rw-r--r--   0        0        0     5880 2024-04-17 08:52:09.822073 iac_init-0.4.0/iac_init/cli/main.py
+-rw-r--r--   0        0        0      206 2024-04-17 08:52:09.822073 iac_init-0.4.0/iac_init/cli/options.py
+-rw-r--r--   0        0        0     2064 2024-04-17 08:52:09.822073 iac_init-0.4.0/iac_init/conf/__init__.py
+-rw-r--r--   0        0        0     2564 2024-04-17 08:52:09.822073 iac_init-0.4.0/iac_init/conf/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1656 2024-04-17 08:52:09.822073 iac_init-0.4.0/iac_init/conf/__pycache__/global_settings.cpython-310.pyc
+-rw-r--r--   0        0        0     2057 2024-04-17 08:52:09.822073 iac_init-0.4.0/iac_init/conf/global_settings.py
+-rw-r--r--   0        0        0      887 2024-04-17 08:52:09.822073 iac_init-0.4.0/iac_init/scripts/__pycache__/ansible_tool.cpython-310.pyc
+-rw-r--r--   0        0        0     1981 2024-04-17 08:52:09.822073 iac_init-0.4.0/iac_init/scripts/__pycache__/apic_connecton_tool.cpython-310.pyc
+-rw-r--r--   0        0        0     1337 2024-04-17 08:52:09.822073 iac_init-0.4.0/iac_init/scripts/__pycache__/create_threadingpool.cpython-310.pyc
+-rw-r--r--   0        0        0     1185 2024-04-17 08:52:09.822073 iac_init-0.4.0/iac_init/scripts/__pycache__/log_tool.cpython-310.pyc
+-rw-r--r--   0        0        0      551 2024-04-17 08:52:09.822073 iac_init-0.4.0/iac_init/scripts/__pycache__/ssh_tool.cpython-310.pyc
+-rw-r--r--   0        0        0      403 2024-04-17 08:52:09.822073 iac_init-0.4.0/iac_init/scripts/__pycache__/telnet_tool.cpython-310.pyc
+-rw-r--r--   0        0        0      747 2024-04-17 08:52:09.822073 iac_init-0.4.0/iac_init/scripts/ansible_tool.py
+-rw-r--r--   0        0        0     2595 2024-04-17 08:52:09.822073 iac_init-0.4.0/iac_init/scripts/apic_connecton_tool.py
+-rw-r--r--   0        0        0     6788 2024-04-17 08:52:09.822073 iac_init-0.4.0/iac_init/scripts/cimc_precheck_tool.py
+-rw-r--r--   0        0        0      452 2024-04-17 08:52:09.822073 iac_init-0.4.0/iac_init/scripts/ssh_tool.py
+-rw-r--r--   0        0        0      263 2024-04-17 08:52:09.822073 iac_init-0.4.0/iac_init/scripts/telnet_tool.py
+-rw-r--r--   0        0        0      388 2024-04-17 08:52:09.822073 iac_init-0.4.0/iac_init/templates/03-node_registration/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/03-node_registration/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/03-node_registration/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/03-node_registration/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/03-node_registration/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/03-node_registration/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/04-oob_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/04-oob_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/04-oob_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/04-oob_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/04-oob_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/04-oob_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/05-aci_system_settings/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/05-aci_system_settings/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/05-aci_system_settings/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/05-aci_system_settings/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/05-aci_system_settings/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/05-aci_system_settings/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/06-fabric_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/06-fabric_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/06-fabric_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/06-fabric_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/06-fabric_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/06-fabric_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/07-access_policy/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/07-access_policy/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/07-access_policy/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/07-access_policy/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/07-access_policy/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/07-access_policy/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/08-inb_mgmt/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/08-inb_mgmt/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/08-inb_mgmt/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/08-inb_mgmt/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/08-inb_mgmt/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/08-inb_mgmt/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/09-smart_licensing/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/09-smart_licensing/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/09-smart_licensing/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/09-smart_licensing/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/09-smart_licensing/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/09-smart_licensing/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/10-confg_aaa/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/10-confg_aaa/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/10-confg_aaa/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/10-confg_aaa/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 08:52:09.826073 iac_init-0.4.0/iac_init/templates/10-confg_aaa/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 08:52:09.830073 iac_init-0.4.0/iac_init/templates/10-confg_aaa/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 08:52:09.830073 iac_init-0.4.0/iac_init/templates/11-config_monitor/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 08:52:09.830073 iac_init-0.4.0/iac_init/templates/11-config_monitor/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 08:52:09.830073 iac_init-0.4.0/iac_init/templates/11-config_monitor/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 08:52:09.830073 iac_init-0.4.0/iac_init/templates/11-config_monitor/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 08:52:09.830073 iac_init-0.4.0/iac_init/templates/11-config_monitor/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 08:52:09.830073 iac_init-0.4.0/iac_init/templates/11-config_monitor/inventory.yaml.j2
+-rw-r--r--   0        0        0      388 2024-04-17 08:52:09.830073 iac_init-0.4.0/iac_init/templates/12-config_backup/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-04-17 08:52:09.830073 iac_init-0.4.0/iac_init/templates/12-config_backup/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-04-17 08:52:09.830073 iac_init-0.4.0/iac_init/templates/12-config_backup/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-04-17 08:52:09.830073 iac_init-0.4.0/iac_init/templates/12-config_backup/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-04-17 08:52:09.830073 iac_init-0.4.0/iac_init/templates/12-config_backup/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-04-17 08:52:09.830073 iac_init-0.4.0/iac_init/templates/12-config_backup/inventory.yaml.j2
+-rw-r--r--   0        0        0      370 2024-04-17 08:52:09.830073 iac_init-0.4.0/iac_init/utils/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0        0        0     3446 2024-04-17 08:52:09.830073 iac_init-0.4.0/iac_init/utils/__pycache__/functional.cpython-310.pyc
+-rw-r--r--   0        0        0      101 2024-04-17 08:52:09.830073 iac_init-0.4.0/iac_init/utils/exceptions.py
+-rw-r--r--   0        0        0     4910 2024-04-17 08:52:09.830073 iac_init-0.4.0/iac_init/utils/functional.py
+-rw-r--r--   0        0        0    10263 2024-04-17 08:52:09.830073 iac_init-0.4.0/iac_init/validator.py
+-rw-r--r--   0        0        0     4138 2024-04-17 08:52:09.830073 iac_init-0.4.0/iac_init/yaml_conf/__pycache__/yaml.cpython-310.pyc
+-rw-r--r--   0        0        0     4043 2024-04-17 08:52:09.830073 iac_init-0.4.0/iac_init/yaml_conf/__pycache__/yaml_writer.cpython-310.pyc
+-rw-r--r--   0        0        0     5093 2024-04-17 08:52:09.830073 iac_init-0.4.0/iac_init/yaml_conf/yaml.py
+-rw-r--r--   0        0        0     5222 2024-04-17 08:52:09.830073 iac_init-0.4.0/iac_init/yaml_conf/yaml_writer.py
+-rw-r--r--   0        0        0     1601 2024-04-17 08:52:09.830073 iac_init-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      806 1970-01-01 00:00:00.000000 iac_init-0.4.0/PKG-INFO
```

### Comparing `iac_init-0.3.9/LICENSE` & `iac_init-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.9/iac_init/cli/__pycache__/main.cpython-310.pyc` & `iac_init-0.4.0/iac_init/cli/__pycache__/main.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.9/iac_init/cli/main.py` & `iac_init-0.4.0/iac_init/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,27 +14,29 @@
 from loguru import logger
 from iac_init.conf import settings
 from iac_init.yaml_conf import yaml_writer
 from iac_init.scripts.ansible_tool import run_ansible_playbook
 
 error_handler = errorhandler.ErrorHandler()
 
-logger.add(sink=os.path.join(settings.OUTPUT_BASE_DIR, 'iac_init_log', 'iac-init-main.log'),
-           , format='{time:YYYY-MM-DD HH:mm:ss} | {level} | {message}', encoding='utf-8')
-logger.add(logging.StreamHandler(), format="")
-
 @click.command(context_settings=dict(help_option_names=["-h", "--help"]))
 @click.version_option(iac_init.__version__)
 @options.yaml_dir_path
 def main(
         data: str
 ) -> None:
     """A CLI tool to perform APIC initialize."""
     output = settings.OUTPUT_BASE_DIR
 
+    if os.path.exists(output) and os.path.isdir(output):
+        shutil.rmtree(output)
+
+    logger.add(sink=os.path.join(settings.OUTPUT_BASE_DIR, 'iac_init_log', 'iac-init-main.log'),
+               format='{time:YYYY-MM-DD HH:mm:ss} | {level} | {message}', encoding='utf-8')
+
     validator = iac_init.validator.Validator(data, output)
 
     # Type single number or multiple number (1,2...)
     option_prompt = "Select single or multiple options to init APIC:\n{}\nExample: (1,2,..)".format(
         "\n".join([f"[{i + 1}]  {option}" for i, option in enumerate(settings.DEFAULT_USER_OPTIONS)]))
     option_choice = click.prompt(
         click.style(option_prompt, fg='green'),
```

### Comparing `iac_init-0.3.9/iac_init/conf/__init__.py` & `iac_init-0.4.0/iac_init/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.9/iac_init/conf/__pycache__/__init__.cpython-310.pyc` & `iac_init-0.4.0/iac_init/conf/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.9/iac_init/conf/__pycache__/global_settings.cpython-310.pyc` & `iac_init-0.4.0/iac_init/conf/__pycache__/global_settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.9/iac_init/conf/global_settings.py` & `iac_init-0.4.0/iac_init/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.9/iac_init/scripts/__pycache__/ansible_tool.cpython-310.pyc` & `iac_init-0.4.0/iac_init/scripts/__pycache__/ansible_tool.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.9/iac_init/scripts/__pycache__/apic_connecton_tool.cpython-310.pyc` & `iac_init-0.4.0/iac_init/scripts/__pycache__/apic_connecton_tool.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.9/iac_init/scripts/__pycache__/create_threadingpool.cpython-310.pyc` & `iac_init-0.4.0/iac_init/scripts/__pycache__/create_threadingpool.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.9/iac_init/scripts/__pycache__/log_tool.cpython-310.pyc` & `iac_init-0.4.0/iac_init/scripts/__pycache__/log_tool.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.9/iac_init/scripts/__pycache__/ssh_tool.cpython-310.pyc` & `iac_init-0.4.0/iac_init/scripts/__pycache__/ssh_tool.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.9/iac_init/scripts/ansible_tool.py` & `iac_init-0.4.0/iac_init/scripts/ansible_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.9/iac_init/scripts/apic_connecton_tool.py` & `iac_init-0.4.0/iac_init/scripts/apic_connecton_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.9/iac_init/scripts/cimc_precheck_tool.py` & `iac_init-0.4.0/iac_init/scripts/cimc_precheck_tool.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.9/iac_init/utils/__pycache__/functional.cpython-310.pyc` & `iac_init-0.4.0/iac_init/utils/__pycache__/functional.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.9/iac_init/utils/functional.py` & `iac_init-0.4.0/iac_init/utils/functional.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.9/iac_init/validator.py` & `iac_init-0.4.0/iac_init/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from iac_init.yaml_conf.yaml import load_yaml_files
 from iac_init.scripts.ssh_tool import check_ssh_connection
 from iac_init.scripts.apic_connecton_tool import apic_login
 from iac_init.scripts.cimc_precheck_tool import cimc_precheck
 from iac_init.scripts.telnet_tool import check_tennet_connection
 
 logger.add(sink=os.path.join(settings.OUTPUT_BASE_DIR, 'iac_init_log', 'iac-init-main.log'), format='{time:YYYY-MM-DD HH:mm:ss} | {level} | {message}', encoding='utf-8')
-logger.add(logging.StreamHandler(), format='')
 
 class Validator:
     def __init__(self, data_path: str, output: str):
         self.data: Optional[Dict[str, Any]] = None
         self.data_path = data_path
         self.output = output
         self.global_policy = None
@@ -42,17 +41,14 @@
                 return True
         else:
             msg = "Yaml Directory not exist.: {}".format(self.data_path)
             logger.error(msg)
             self.errors.append(msg)
             return True
 
-        if os.path.exists(self.output) and os.path.isdir(self.output):
-            shutil.rmtree(self.output)
-
         logger.info("Loaded Yaml directory: {}".format(self.data_path))
 
         return self._validate_yaml()
 
     def _validate_syntax_file(self, file_path: str):
         """Run syntactic validation for a single file"""
         filename = os.path.basename(file_path)
```

### Comparing `iac_init-0.3.9/iac_init/yaml_conf/__pycache__/yaml.cpython-310.pyc` & `iac_init-0.4.0/iac_init/yaml_conf/__pycache__/yaml.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.9/iac_init/yaml_conf/__pycache__/yaml_writer.cpython-310.pyc` & `iac_init-0.4.0/iac_init/yaml_conf/__pycache__/yaml_writer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.9/iac_init/yaml_conf/yaml.py` & `iac_init-0.4.0/iac_init/yaml_conf/yaml.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.9/iac_init/yaml_conf/yaml_writer.py` & `iac_init-0.4.0/iac_init/yaml_conf/yaml_writer.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.3.9/pyproject.toml` & `iac_init-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iac-init"
-version = "0.3.9"
+version = "0.4.0"
 description = ""
 authors = ["Wang Xiao <xiawang3@cisco.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 iac-init = "iac_init.cli.main:main"
```

### Comparing `iac_init-0.3.9/PKG-INFO` & `iac_init-0.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-init
-Version: 0.3.9
+Version: 0.4.0
 Summary: 
 Author: Wang Xiao
 Author-email: xiawang3@cisco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

