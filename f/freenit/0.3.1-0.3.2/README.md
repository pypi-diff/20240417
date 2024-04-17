# Comparing `tmp/freenit-0.3.1.tar.gz` & `tmp/freenit-0.3.2.tar.gz`

## Comparing `freenit-0.3.1.tar` & `freenit-0.3.2.tar`

### file list

```diff
@@ -1,103 +1,108 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 freenit-0.3.1/.pylintrc
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 freenit-0.3.1/MANIFEST.in
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 freenit-0.3.1/Makefile
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 freenit-0.3.1/alembic.ini
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 freenit-0.3.1/main.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 freenit-0.3.1/name.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 freenit-0.3.1/provisioners.mk
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 freenit-0.3.1/pytest.ini
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 freenit-0.3.1/requirements.yml
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 freenit-0.3.1/setup.cfg
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 freenit-0.3.1/setup.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 freenit-0.3.1/.github/workflows/pythonapp.yml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 freenit-0.3.1/alembic/README
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 freenit-0.3.1/alembic/env.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 freenit-0.3.1/alembic/script.py.mako
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 freenit-0.3.1/alembic/versions/06a043f2516a_initial.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 freenit-0.3.1/ansible/group_vars/.keep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.1/ansible/inventory/.keep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.1/ansible/roles/.keep
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 freenit-0.3.1/ansible/roles/devel/tasks/main.yml
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 freenit-0.3.1/ansible/roles/devel/vars/main.yml
--rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 freenit-0.3.1/bin/build.sh
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 freenit-0.3.1/bin/common.sh
--rwxr-xr-x   0        0        0      335 2020-02-02 00:00:00.000000 freenit-0.3.1/bin/devel.sh
--rwxr-xr-x   0        0        0    12122 2020-02-02 00:00:00.000000 freenit-0.3.1/bin/freenit.sh
--rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 freenit-0.3.1/bin/init.sh
--rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 freenit-0.3.1/bin/publish.sh
--rwxr-xr-x   0        0        0      163 2020-02-02 00:00:00.000000 freenit-0.3.1/bin/security.sh
--rwxr-xr-x   0        0        0      129 2020-02-02 00:00:00.000000 freenit-0.3.1/bin/test.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/__init__.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/app.py
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/auth.py
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/base_config.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/cli.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/config.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/decorators.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/mail.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/migration.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/permissions.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/api/__init__.py
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/api/auth.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/api/role.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/api/router.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/api/theme.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/api/user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/__init__.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/pagination.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/role.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/safe.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/theme.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/ldap/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/ldap/base.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/ldap/user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/ormar/__init__.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/ormar/base.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/ormar/role.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/ormar/theme.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/ormar/user.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/LICENSE
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/alembic.ini
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/main.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/provisioners.mk
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/pyproject.toml
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/requirements.yml
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/setup.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/alembic/script.py.mako
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/ansible/group_vars/.keep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/ansible/inventory/.keep
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/ansible/roles/devel/tasks/main.yml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/ansible/roles/devel/vars/main.yml
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/bin/common.sh
--rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/bin/devel.sh
--rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/bin/init.sh
--rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/bin/test.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/project/__init__.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/project/app.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/project/base_config.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/project/config.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/project/api/__init__.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/project/api/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/project/models/__init__.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/templates/site.yml.tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/tests/__init__.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/tests/client.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/tests/conftest.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/tests/factories.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/tests/test_user.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 freenit-0.3.1/templates/site.yml.tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 freenit-0.3.1/tests/client.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 freenit-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 freenit-0.3.1/tests/factories.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 freenit-0.3.1/tests/test_auth.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 freenit-0.3.1/tests/test_permission.py
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 freenit-0.3.1/tests/test_role.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 freenit-0.3.1/tests/test_user.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 freenit-0.3.1/.gitignore
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 freenit-0.3.1/LICENSE
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 freenit-0.3.1/README.md
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 freenit-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 freenit-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 freenit-0.3.2/.pylintrc
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 freenit-0.3.2/MANIFEST.in
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 freenit-0.3.2/Makefile
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 freenit-0.3.2/alembic.ini
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 freenit-0.3.2/main.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 freenit-0.3.2/name.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 freenit-0.3.2/provisioners.mk
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 freenit-0.3.2/pytest.ini
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 freenit-0.3.2/requirements.yml
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 freenit-0.3.2/setup.cfg
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 freenit-0.3.2/setup.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 freenit-0.3.2/.github/workflows/pythonapp.yml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 freenit-0.3.2/alembic/README
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 freenit-0.3.2/alembic/env.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 freenit-0.3.2/alembic/script.py.mako
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 freenit-0.3.2/alembic/versions/06a043f2516a_initial.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 freenit-0.3.2/ansible/group_vars/.keep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.2/ansible/inventory/.keep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.2/ansible/roles/.keep
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 freenit-0.3.2/ansible/roles/devel/tasks/main.yml
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 freenit-0.3.2/ansible/roles/devel/vars/main.yml
+-rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 freenit-0.3.2/bin/build.sh
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 freenit-0.3.2/bin/common.sh
+-rwxr-xr-x   0        0        0      335 2020-02-02 00:00:00.000000 freenit-0.3.2/bin/devel.sh
+-rwxr-xr-x   0        0        0    12122 2020-02-02 00:00:00.000000 freenit-0.3.2/bin/freenit.sh
+-rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 freenit-0.3.2/bin/init.sh
+-rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 freenit-0.3.2/bin/publish.sh
+-rwxr-xr-x   0        0        0      163 2020-02-02 00:00:00.000000 freenit-0.3.2/bin/security.sh
+-rwxr-xr-x   0        0        0      129 2020-02-02 00:00:00.000000 freenit-0.3.2/bin/test.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/__init__.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/app.py
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/auth.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/base_config.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/cli.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/config.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/decorators.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/mail.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/migration.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/permissions.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/api/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/api/router.py
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/api/theme.py
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/api/auth/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/api/role/__init__.py
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/api/role/ldap.py
+-rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/api/role/sql.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/api/user/__init__.py
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/api/user/ldap.py
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/api/user/sql.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/__init__.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/pagination.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/role.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/safe.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/theme.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/ldap/__init__.py
+-rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/ldap/base.py
+-rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/ldap/role.py
+-rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/ldap/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/sql/__init__.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/sql/base.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/sql/role.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/sql/theme.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/models/sql/user.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/LICENSE
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/alembic.ini
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/main.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/provisioners.mk
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/pyproject.toml
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/requirements.yml
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/setup.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/alembic/script.py.mako
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/ansible/group_vars/.keep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/ansible/inventory/.keep
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/ansible/roles/devel/tasks/main.yml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/ansible/roles/devel/vars/main.yml
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/bin/common.sh
+-rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/bin/devel.sh
+-rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/bin/init.sh
+-rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/bin/test.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/project/__init__.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/project/app.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/project/base_config.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/project/config.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/project/api/__init__.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/project/api/router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/project/models/__init__.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/templates/site.yml.tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/tests/__init__.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/tests/client.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/tests/conftest.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/tests/factories.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 freenit-0.3.2/freenit/project/tests/test_user.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 freenit-0.3.2/templates/site.yml.tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.2/tests/__init__.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 freenit-0.3.2/tests/client.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 freenit-0.3.2/tests/conftest.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 freenit-0.3.2/tests/factories.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 freenit-0.3.2/tests/test_auth.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 freenit-0.3.2/tests/test_permission.py
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 freenit-0.3.2/tests/test_role.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 freenit-0.3.2/tests/test_user.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 freenit-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 freenit-0.3.2/LICENSE
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 freenit-0.3.2/README.md
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 freenit-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 freenit-0.3.2/PKG-INFO
```

### Comparing `freenit-0.3.1/alembic.ini` & `freenit-0.3.2/alembic.ini`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/setup.py` & `freenit-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/alembic/versions/06a043f2516a_initial.py` & `freenit-0.3.2/alembic/versions/06a043f2516a_initial.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/bin/common.sh` & `freenit-0.3.2/bin/common.sh`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/bin/freenit.sh` & `freenit-0.3.2/bin/freenit.sh`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/freenit/auth.py` & `freenit-0.3.2/freenit/auth.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,61 +11,45 @@
     try:
         data = jwt.decode(token, config.secret, algorithms=["HS256"])
     except:
         raise HTTPException(status_code=403, detail="Unauthorized")
     pk = data.get("pk", None)
     if pk is None:
         raise HTTPException(status_code=403, detail="Unauthorized")
-    if User.dbtype() == "ormar":
+    if User.dbtype() == "sql":
         import ormar
         import ormar.exceptions
 
         try:
             user = await User.objects.get(pk=pk)
             return user
         except ormar.exceptions.NoMatch:
             raise HTTPException(status_code=403, detail="Unauthorized")
-    elif User.dbtype() == "bonsai":
-        import bonsai
-
-        client = bonsai.LDAPClient(f"ldap://{config.ldap.host}", config.ldap.tls)
-        async with client.connect(is_async=True) as conn:
-            res = await conn.search(
-                pk,
-                bonsai.LDAPSearchScope.BASE,
-                "objectClass=person",
-            )
-        data = res[0]
-        user = User(
-            email=data["mail"][0],
-            sn=data["sn"][0],
-            cn=data["cn"][0],
-            dn=str(data["dn"]),
-            uid=data["uid"][0],
-        )
+    elif User.dbtype() == "ldap":
+        user = await User.get(pk)
         return user
     raise HTTPException(status_code=409, detail="Unknown user type")
 
 
 def encode(user):
     config = getConfig()
     payload = {}
-    if user.dbtype() == "ormar":
+    if user.dbtype() == "sql":
         payload = {"pk": user.pk, "type": "ormar"}
-    elif user.dbtype() == "bonsai":
+    elif user.dbtype() == "ldap":
         payload = {"pk": user.dn, "type": "bonsai"}
     return jwt.encode(payload, config.secret, algorithm="HS256")
 
 
 async def authorize(request: Request, roles=[], allof=[], cookie="access"):
     token = request.cookies.get(cookie)
     if not token:
         raise HTTPException(status_code=403, detail="Unauthorized")
     user = await decode(token)
-    if user.dbtype() == "ormar":
+    if user.dbtype() == "sql":
         await user.load_all()
         if not user.active:
             raise HTTPException(status_code=403, detail="Permission denied")
         if user.admin:
             return user
         if len(user.roles) == 0:
             if len(roles) > 0 or len(allof) > 0:
@@ -80,15 +64,15 @@
                 if not found:
                     raise HTTPException(status_code=403, detail="Permission denied")
             if len(allof) > 0:
                 for role in user.roles:
                     if role.name not in allof:
                         raise HTTPException(status_code=403, detail="Permission denied")
         return user
-    elif user.dbtype() == "bonsai":
+    elif user.dbtype() == "ldap":
         pass
     return user
 
 
 def verify(password, encpassword):
     config = getConfig()
     return pbkdf2_sha256.verify(f"{config.secret}{password}", encpassword)
```

### Comparing `freenit-0.3.1/freenit/base_config.py` & `freenit-0.3.2/freenit/base_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 
 class Mail:
     def __init__(
         self,
         server="mail.example.com",
         user="user@example.com",
-        password="Secrit", #nosec
+        password="Sekrit",  # nosec
         port=587,
         tls=True,
         from_addr="no-reply@mail.com",
         register_subject="[Freenit] User Registration",
         register_message=register_message,
     ) -> None:
         self.server = server
@@ -47,36 +47,47 @@
         self.from_addr = from_addr
         self.register_subject = register_subject
         self.register_message = register_message
 
 
 class LDAP:
     def __init__(
-        self, host="ldap.example.com", tls=True, base="uid={},ou={},dc=account,dc=ldap"
+        self,
+        host="ldap.example.com",
+        tls=True,
+        base="uid={},ou={},dc=account,dc=ldap",
+        service_dn="cn=freenit,dc=service,dc=ldap",
+        service_pw="",
+        userClasses=["pilotPerson", "posixAccount"],
+        groupClasses=["groupOfUniqueNames"],
     ):
         self.host = host
         self.tls = tls
         self.base = base
+        self.service_dn = service_dn
+        self.service_pw = service_pw
+        self.userClasses = userClasses
+        self.groupClasses = groupClasses
 
 
 class BaseConfig:
     name = "Freenit"
     version = "0.0.1"
     api_root = "/api/v1"
     hostname = socket.gethostname()
     port = 5000
     debug = False
     metadata = sqlalchemy.MetaData()
     dburl = "sqlite:///db.sqlite"
     database = None
     engine = None
-    secret = "SECRET" #nosec
-    user = "freenit.models.ormar.user"
-    role = "freenit.models.ormar.role"
-    theme = "freenit.models.ormar.theme"
+    secret = "SECRET"  # nosec
+    user = "freenit.models.sql.user"
+    role = "freenit.models.sql.role"
+    theme = "freenit.models.sql.theme"
     theme_name = "Freenit"
     meta = None
     auth = Auth()
     mail = Mail()
     ldap = LDAP()
 
     def __init__(self):
@@ -111,8 +122,8 @@
     debug = True
     dburl = "sqlite:///test.sqlite"
     auth = Auth(secure=False)
     mail = None
 
 
 class ProdConfig(BaseConfig):
-    secret = "MORESECURESECRET" #nosec
+    secret = "MORESECURESECRET"  # nosec
```

### Comparing `freenit-0.3.1/freenit/config.py` & `freenit-0.3.2/freenit/config.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/freenit/decorators.py` & `freenit-0.3.2/freenit/decorators.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/freenit/migration.py` & `freenit-0.3.2/freenit/migration.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/freenit/api/auth.py` & `freenit-0.3.2/freenit/api/auth/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,29 +54,42 @@
         "expire": {
             "access": config.auth.expire,
             "refresh": config.auth.refresh_expire,
         },
     }
 
 
-@api.post("/auth/register", tags=["auth"])
-async def register(credentials: LoginInput, host=Header(default="")):
+async def register_sql(credentials: LoginInput) -> User:
     import ormar.exceptions
-
     try:
         user = await User.objects.get(email=credentials.email)
         raise HTTPException(status_code=409, detail="User already registered")
     except ormar.exceptions.NoMatch:
         pass
     user = User(
         email=credentials.email,
         password=encrypt(credentials.password),
         active=False,
     )
     await user.save()
+    return user
+
+
+async def register_ldap(credentials: LoginInput) -> User:
+    user = await User.register(credentials)
+    await user.save()
+    return user
+
+
+@api.post("/auth/register", tags=["auth"])
+async def register(credentials: LoginInput, host=Header(default="")):
+    if User.dbtype() == "sql":
+        user = await register_sql(credentials)
+    else:
+        user = await register_ldap(credentials)
     token = encode(user)
     print(token)
     mail = config.mail
     if mail is not None:
         message = mail.register_message.format(f"http://{host}/verify/{token}")
         msg = MIMEText(message, "plain", "utf-8")
         msg["From"] = mail.from_addr
```

### Comparing `freenit-0.3.1/freenit/api/role.py` & `freenit-0.3.2/freenit/api/role/sql.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from typing import List
-
 import ormar
 import ormar.exceptions
 from fastapi import Depends, Header, HTTPException
+
 from freenit.api.router import route
 from freenit.decorators import description
 from freenit.models.pagination import Page, paginate
 from freenit.models.role import Role, RoleOptional
 from freenit.models.safe import RoleSafe, UserSafe
 from freenit.models.user import User
 from freenit.permissions import role_perms
@@ -19,62 +18,64 @@
     @staticmethod
     @description("Get roles")
     async def get(
         page: int = Header(default=1),
         perpage: int = Header(default=10),
         _: User = Depends(role_perms),
     ) -> Page[RoleSafe]:
-        roles = Role.objects
-        return await paginate(roles, page, perpage)
+        return await paginate(Role.objects, page, perpage)
 
     @staticmethod
     async def post(role: Role, _: User = Depends(role_perms)) -> RoleSafe:
         await role.save()
         return role
 
 
 @route("/roles/{id}", tags=tags)
 class RoleDetailAPI:
     @staticmethod
-    async def get(id: int, _: User = Depends(role_perms)) -> RoleSafe:
+    async def get(id, _: User = Depends(role_perms)) -> RoleSafe:
         try:
             role = await Role.objects.get(pk=id)
         except ormar.exceptions.NoMatch:
             raise HTTPException(status_code=404, detail="No such role")
         await role.load_all(follow=True)
         return role
 
     @staticmethod
     async def patch(
-        id: int, role_data: RoleOptional, _: User = Depends(role_perms)
+        id, role_data: RoleOptional, _: User = Depends(role_perms)
     ) -> RoleSafe:
-        try:
-            role = await Role.objects.get(pk=id)
-        except ormar.exceptions.NoMatch:
-            raise HTTPException(status_code=404, detail="No such role")
-        await role.patch(role_data)
-        return role
+        if Role.dbtype() == "sql":
+            try:
+                role = await Role.objects.get(pk=id)
+            except ormar.exceptions.NoMatch:
+                raise HTTPException(status_code=404, detail="No such role")
+            await role.patch(role_data)
+            return role
+        raise HTTPException(
+            status_code=409,
+            detail=f"Role type {Role.dbtype()} doesn't support PATCH method",
+        )
 
     @staticmethod
-    async def delete(id: int, _: User = Depends(role_perms)) -> RoleSafe:
+    async def delete(id, _: User = Depends(role_perms)) -> RoleSafe:
         try:
             role = await Role.objects.get(pk=id)
         except ormar.exceptions.NoMatch:
             raise HTTPException(status_code=404, detail="No such role")
         await role.delete()
         return role
 
 
 @route("/roles/{role_id}/{user_id}", tags=tags)
 class RoleUserAPI:
     @staticmethod
     @description("Assign user to role")
-    async def post(
-        role_id: int, user_id: int, _: User = Depends(role_perms)
-    ) -> UserSafe:
+    async def post(role_id, user_id, _: User = Depends(role_perms)) -> UserSafe:
         try:
             user = await User.objects.get(pk=user_id)
         except ormar.exceptions.NoMatch:
             raise HTTPException(status_code=404, detail="No such user")
         await user.load_all()
         for role in user.roles:
             if role.id == role_id:
@@ -84,17 +85,15 @@
         except ormar.exceptions.NoMatch:
             raise HTTPException(status_code=404, detail="No such role")
         await user.roles.add(role)
         return user
 
     @staticmethod
     @description("Deassign user to role")
-    async def delete(
-        role_id: int, user_id: int, _: User = Depends(role_perms)
-    ) -> UserSafe:
+    async def delete(role_id, user_id, _: User = Depends(role_perms)) -> UserSafe:
         try:
             user = await User.objects.get(pk=user_id)
         except ormar.exceptions.NoMatch:
             raise HTTPException(status_code=404, detail="No such user")
         try:
             role = await Role.objects.get(pk=role_id)
         except ormar.exceptions.NoMatch:
```

### Comparing `freenit-0.3.1/freenit/api/theme.py` & `freenit-0.3.2/freenit/api/theme.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import List
-
 import ormar
 import ormar.exceptions
 from fastapi import Depends, Header, HTTPException
 
 from freenit.api.router import route
 from freenit.config import getConfig
 from freenit.decorators import description
```

### Comparing `freenit-0.3.1/freenit/models/pagination.py` & `freenit-0.3.2/freenit/models/pagination.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/freenit/models/ldap/user.py` & `freenit-0.3.2/freenit/models/ldap/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,88 @@
-from __future__ import annotations
+from typing import Generic, TypeVar
 
 from bonsai import LDAPClient, LDAPSearchScope, errors
+from bonsai.errors import AuthenticationError, InsufficientAccess, UnwillingToPerform
 from fastapi import HTTPException
-from pydantic import Field
+from pydantic import BaseModel, Field
 
 from freenit.config import getConfig
-from freenit.models.ldap.base import LDAPBaseModel, LDAPUserMixin
 
+T = TypeVar("T")
 config = getConfig()
 
 
-class UserSafe(LDAPBaseModel, LDAPUserMixin):
-    @classmethod
-    async def _login(cls, credentials) -> dict:
+def get_client(credentials=None):
+    client = LDAPClient(f"ldap://{config.ldap.host}", config.ldap.tls)
+    if credentials is not None:
         username, domain = credentials.email.split("@")
-        client = LDAPClient(f"ldap://{config.ldap.host}", config.ldap.tls)
         dn = config.ldap.base.format(username, domain)
         client.set_credentials("SIMPLE", user=dn, password=credentials.password)
+    else:
+        dn = config.ldap.service_dn
+        client.set_credentials("SIMPLE", user=dn, password=config.ldap.service_pw)
+    return client
+
+
+async def save_data(data):
+    client = get_client()
+    async with client.connect(is_async=True) as conn:
+        try:
+            await conn.add(data)
+        except InsufficientAccess:
+            raise HTTPException(
+                status_code=403, detail="No permission to create user"
+            )
+
+
+class LDAPBaseModel(BaseModel, Generic[T]):
+    @classmethod
+    def dbtype(cls):
+        return "ldap"
+
+    dn: str = Field("", description=("Distinguished name"))
+
+
+class LDAPUserMixin:
+    @classmethod
+    async def _login(cls, credentials) -> dict:
+        client = get_client(credentials)
         try:
             async with client.connect(is_async=True) as conn:
+                username, domain = credentials.email.split("@")
+                dn = config.ldap.base.format(username, domain)
                 res = await conn.search(dn, LDAPSearchScope.BASE, "objectClass=person")
         except errors.AuthenticationError:
             raise HTTPException(status_code=403, detail="Failed to login")
-
         data = res[0]
         return data
 
     @classmethod
-    async def login(cls, credentials) -> UserSafe:
+    async def login(cls, credentials):
         data = await cls._login(credentials)
         user = cls(
             dn=str(data["dn"]),
             email=credentials.email,
             sn=data["sn"][0],
             cn=data["cn"][0],
             uid=data["uid"][0],
         )
         return user
 
-
-class User(UserSafe):
-    password: str = Field("", description=("Password"))
-
-
-class UserOptional(User):
-    pass
-
-
-UserOptionalPydantic = UserOptional
+    @classmethod
+    async def register(cls, credentials):
+        client = get_client()
+        username, domain = credentials.email.split("@")
+        dn = config.ldap.base.format(username, domain)
+        try:
+            async with client.connect(is_async=True) as conn:
+                res = await conn.search(dn, LDAPSearchScope.BASE, "objectClass=person")
+                if len(res) > 0:
+                    raise HTTPException(status_code=409, detail="User already exists")
+        except UnwillingToPerform:
+            raise HTTPException(status_code=409, detail="Can not bind to LDAP")
+        except AuthenticationError:
+            raise HTTPException(status_code=409, detail="Can not bind to LDAP")
+        user = cls(
+            dn=dn, uid=username, email=credentials.email, password=credentials.password
+        )
+        return user
```

### Comparing `freenit-0.3.1/freenit/models/ormar/base.py` & `freenit-0.3.2/freenit/models/sql/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import ormar
 import pydantic
 
 from freenit.config import getConfig
 
-
 config = getConfig()
 
 
 class OrmarBaseModel(ormar.Model):
     @classmethod
     def dbtype(cls):
-        return 'ormar'
+        return "sql"
 
     async def patch(self, fields):
         result = {}
         data = fields.dict()
         for k in data:
             if data[k] is not None:
                 result[k] = data[k]
```

### Comparing `freenit-0.3.1/freenit/models/ormar/theme.py` & `freenit-0.3.2/freenit/models/sql/theme.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/freenit/models/ormar/user.py` & `freenit-0.3.2/freenit/models/sql/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import ormar
 import ormar.exceptions
 from fastapi import HTTPException
 
 from freenit.auth import verify
-from freenit.models.ormar.base import (
+from freenit.models.sql.base import (
     OrmarBaseModel,
     OrmarUserMixin,
     generate_optional,
     ormar_config,
 )
 from freenit.models.role import Role
```

### Comparing `freenit-0.3.1/freenit/project/alembic.ini` & `freenit-0.3.2/freenit/project/alembic.ini`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/freenit/project/pyproject.toml` & `freenit-0.3.2/freenit/project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/freenit/project/setup.py` & `freenit-0.3.2/freenit/project/setup.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/freenit/project/bin/common.sh` & `freenit-0.3.2/freenit/project/bin/common.sh`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/freenit/project/project/config.py` & `freenit-0.3.2/freenit/project/project/config.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/freenit/project/tests/client.py` & `freenit-0.3.2/freenit/project/tests/client.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/freenit/project/tests/conftest.py` & `freenit-0.3.2/freenit/project/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/freenit/project/tests/factories.py` & `freenit-0.3.2/freenit/project/tests/factories.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/tests/client.py` & `freenit-0.3.2/tests/client.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/tests/conftest.py` & `freenit-0.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/tests/factories.py` & `freenit-0.3.2/tests/factories.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/tests/test_auth.py` & `freenit-0.3.2/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/tests/test_permission.py` & `freenit-0.3.2/tests/test_permission.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/tests/test_role.py` & `freenit-0.3.2/tests/test_role.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/tests/test_user.py` & `freenit-0.3.2/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/LICENSE` & `freenit-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `freenit-0.3.1/pyproject.toml` & `freenit-0.3.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -45,14 +45,32 @@
     "black",
     "httpx",
     "isort",
     "pytest-asyncio",
     "pytest-factoryboy",
     "requests",
   ]
+  all = [
+    "beanie",
+    "aiosqlite",
+    "black",
+    "isort",
+    "uvicorn",
+    "bonsai",
+    "alembic",
+    "ormar",
+    "aiosqlite",
+    "bandit",
+    "black",
+    "httpx",
+    "isort",
+    "pytest-asyncio",
+    "pytest-factoryboy",
+    "requests",
+  ]
 
 [project.urls]
 Homepage = "https://freenit.org" 
 Repository = "https://github.com/freenit-framework/backend"
 
 [project.scripts]
 freenit = "freenit.cli:main"
```

