# Comparing `tmp/fancy_dataclass-0.3.0.tar.gz` & `tmp/fancy_dataclass-0.3.1.tar.gz`

## Comparing `fancy_dataclass-0.3.0.tar` & `fancy_dataclass-0.3.1.tar`

### file list

```diff
@@ -1,363 +1,361 @@
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.readthedocs.yaml
--rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/TODO.md
--rw-r--r--   0        0        0     8949 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/fancy_dataclass.json
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/loc-summary.txt
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/mkdocs.yml
--rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/ruff.toml
--rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/summarize.sh
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/website_config.toml
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.github/workflows/workflow.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/.lock
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/CACHEDIR.TAG
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/pyvenv.cfg
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/bin/activate
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/bin/activate.bat
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/bin/activate.csh
--rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/bin/activate.fish
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/bin/activate.nu
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/bin/activate.ps1
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/bin/activate_this.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/bin/deactivate.bat
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/bin/pydoc.bat
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/bin/python -> /Users/jerm/.pyenv/versions/3.11.0/bin/python3.11
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/bin/python3.11 -> python
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/_virtualenv.pth
--rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/_virtualenv.py
--rw-r--r--   0        0        0   117599 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/typing_extensions.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/INSTALLER
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/LICENSE
--rw-r--r--   0        0        0     9602 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/METADATA
--rw-r--r--   0        0        0    24616 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/REQUESTED
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/WHEEL
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/top_level.txt
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/__init__.py
--rw-r--r--   0        0        0    13134 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/cli.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/config.py
--rw-r--r--   0        0        0    16663 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/dict.py
--rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/json.py
--rw-r--r--   0        0        0    11440 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/mixin.py
--rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/sql.py
--rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/subprocess.py
--rw-r--r--   0        0        0    15970 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/utils.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/METADATA
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/WHEEL
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/direct_url.json
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/licenses/LICENSE.txt
--rw-r--r--   0        0        0    13033 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/events.py
--rw-r--r--   0        0        0    23976 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/exc.py
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/inspection.py
--rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/log.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/py.typed
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/schema.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/types.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/__init__.py
--rw-r--r--   0        0        0     5288 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/aioodbc.py
--rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/asyncio.py
--rw-r--r--   0        0        0     8501 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/pyodbc.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/__init__.py
--rwxr-xr-x   0        0        0   273374 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/collections.cpython-311-darwin.so
--rw-r--r--   0        0        0    12571 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/collections.pyx
--rwxr-xr-x   0        0        0   125312 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/immutabledict.cpython-311-darwin.so
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/immutabledict.pxd
--rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/immutabledict.pyx
--rwxr-xr-x   0        0        0   104925 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/processors.cpython-311-darwin.so
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/processors.pyx
--rwxr-xr-x   0        0        0   107806 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/resultproxy.cpython-311-darwin.so
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/resultproxy.pyx
--rwxr-xr-x   0        0        0   125335 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/util.cpython-311-darwin.so
--rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/util.pyx
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/__init__.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/_typing.py
--rw-r--r--   0        0        0     8239 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/type_migration_guidelines.txt
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/__init__.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/aioodbc.py
--rw-r--r--   0        0        0   132301 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/base.py
--rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/information_schema.py
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/json.py
--rw-r--r--   0        0        0     5362 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/provision.py
--rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/pymssql.py
--rw-r--r--   0        0        0    27056 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/pyodbc.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/__init__.py
--rw-r--r--   0        0        0     9964 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/aiomysql.py
--rw-r--r--   0        0        0    10033 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/asyncmy.py
--rw-r--r--   0        0        0   120850 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/base.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/cymysql.py
--rw-r--r--   0        0        0     7645 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/dml.py
--rw-r--r--   0        0        0     8448 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/enumerated.py
--rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/expression.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/json.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mariadb.py
--rw-r--r--   0        0        0     8568 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mariadbconnector.py
--rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mysqlconnector.py
--rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mysqldb.py
--rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/provision.py
--rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/pymysql.py
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/pyodbc.py
--rw-r--r--   0        0        0    22822 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/reflection.py
--rw-r--r--   0        0        0     9258 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/reserved_words.py
--rw-r--r--   0        0        0    24343 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/types.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/__init__.py
--rw-r--r--   0        0        0   118246 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/base.py
--rw-r--r--   0        0        0    55566 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/cx_oracle.py
--rw-r--r--   0        0        0    19519 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/dictionary.py
--rw-r--r--   0        0        0     9487 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/oracledb.py
--rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/provision.py
--rw-r--r--   0        0        0     8231 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/types.py
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/__init__.py
--rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/_psycopg_common.py
--rw-r--r--   0        0        0    13734 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/array.py
--rw-r--r--   0        0        0    40240 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/asyncpg.py
--rw-r--r--   0        0        0   178989 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/base.py
--rw-r--r--   0        0        0    11212 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/dml.py
--rw-r--r--   0        0        0    16262 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/ext.py
--rw-r--r--   0        0        0    11541 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/hstore.py
--rw-r--r--   0        0        0    11217 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/json.py
--rw-r--r--   0        0        0    17594 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/named_types.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/operators.py
--rw-r--r--   0        0        0    18640 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/pg8000.py
--rw-r--r--   0        0        0     9254 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/pg_catalog.py
--rw-r--r--   0        0        0     5762 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/provision.py
--rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg.py
--rw-r--r--   0        0        0    31607 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg2.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg2cffi.py
--rw-r--r--   0        0        0    32949 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/ranges.py
--rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/types.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/__init__.py
--rw-r--r--   0        0        0    12305 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/aiosqlite.py
--rw-r--r--   0        0        0    96794 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/base.py
--rw-r--r--   0        0        0     8443 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/dml.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/json.py
--rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/provision.py
--rw-r--r--   0        0        0     5356 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/pysqlcipher.py
--rw-r--r--   0        0        0    28045 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/pysqlite.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/__init__.py
--rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_processors.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_row.py
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_util.py
--rw-r--r--   0        0        0   123050 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/base.py
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/characteristics.py
--rw-r--r--   0        0        0    33206 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/create.py
--rw-r--r--   0        0        0    76314 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/cursor.py
--rw-r--r--   0        0        0    83993 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/default.py
--rw-r--r--   0        0        0    37381 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/events.py
--rw-r--r--   0        0        0   112832 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/interfaces.py
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/mock.py
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/processors.py
--rw-r--r--   0        0        0    75127 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/reflection.py
--rw-r--r--   0        0        0    77603 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/result.py
--rw-r--r--   0        0        0    12032 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/row.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/strategies.py
--rw-r--r--   0        0        0    30784 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/url.py
--rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/util.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/__init__.py
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/api.py
--rw-r--r--   0        0        0    20751 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/attr.py
--rw-r--r--   0        0        0    14954 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/base.py
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/legacy.py
--rw-r--r--   0        0        0    10835 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/registry.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/__init__.py
--rw-r--r--   0        0        0    65771 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/associationproxy.py
--rw-r--r--   0        0        0    61576 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/automap.py
--rw-r--r--   0        0        0    17807 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/baked.py
--rw-r--r--   0        0        0    20391 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/compiler.py
--rw-r--r--   0        0        0    16750 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/horizontal_shard.py
--rw-r--r--   0        0        0    52432 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/hybrid.py
--rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/indexable.py
--rw-r--r--   0        0        0    15707 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/instrumentation.py
--rw-r--r--   0        0        0    37355 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mutable.py
--rw-r--r--   0        0        0    14384 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/orderinglist.py
--rw-r--r--   0        0        0     6178 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/serializer.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/__init__.py
--rw-r--r--   0        0        0     8905 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/base.py
--rw-r--r--   0        0        0    48190 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/engine.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/exc.py
--rw-r--r--   0        0        0    30409 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/result.py
--rw-r--r--   0        0        0    52597 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/scoping.py
--rw-r--r--   0        0        0    63092 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/session.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/declarative/__init__.py
--rw-r--r--   0        0        0    19547 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/declarative/extensions.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/__init__.py
--rw-r--r--   0        0        0    10550 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/apply.py
--rw-r--r--   0        0        0    17384 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/decl_class.py
--rw-r--r--   0        0        0    19369 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/infer.py
--rw-r--r--   0        0        0    10479 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/names.py
--rw-r--r--   0        0        0     9750 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/plugin.py
--rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/util.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/future/__init__.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/future/engine.py
--rw-r--r--   0        0        0     8463 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/__init__.py
--rw-r--r--   0        0        0    99461 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/_orm_constructors.py
--rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/_typing.py
--rw-r--r--   0        0        0    92535 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/attributes.py
--rw-r--r--   0        0        0    27466 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/base.py
--rw-r--r--   0        0        0    70022 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/bulk_persistence.py
--rw-r--r--   0        0        0    17958 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/clsregistry.py
--rw-r--r--   0        0        0    52179 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/collections.py
--rw-r--r--   0        0        0   112001 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/context.py
--rw-r--r--   0        0        0    63674 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/decl_api.py
--rw-r--r--   0        0        0    81601 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/decl_base.py
--rw-r--r--   0        0        0    47631 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/dependency.py
--rw-r--r--   0        0        0    37180 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/descriptor_props.py
--rw-r--r--   0        0        0     9786 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/dynamic.py
--rw-r--r--   0        0        0    11925 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/evaluator.py
--rw-r--r--   0        0        0   127703 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/events.py
--rw-r--r--   0        0        0     7413 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/exc.py
--rw-r--r--   0        0        0     9249 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/identity.py
--rw-r--r--   0        0        0    24321 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/instrumentation.py
--rw-r--r--   0        0        0    48502 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/interfaces.py
--rw-r--r--   0        0        0    57537 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/loading.py
--rw-r--r--   0        0        0    19690 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/mapped_collection.py
--rw-r--r--   0        0        0   171059 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/mapper.py
--rw-r--r--   0        0        0    25850 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/path_registry.py
--rw-r--r--   0        0        0    61701 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/persistence.py
--rw-r--r--   0        0        0    29294 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/properties.py
--rw-r--r--   0        0        0   117596 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/query.py
--rw-r--r--   0        0        0   128644 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/relationships.py
--rw-r--r--   0        0        0    78677 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/scoping.py
--rw-r--r--   0        0        0   193181 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/session.py
--rw-r--r--   0        0        0    37520 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/state.py
--rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/state_changes.py
--rw-r--r--   0        0        0   114206 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/strategies.py
--rw-r--r--   0        0        0    84563 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/strategy_options.py
--rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/sync.py
--rw-r--r--   0        0        0    27033 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/unitofwork.py
--rw-r--r--   0        0        0    80660 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/util.py
--rw-r--r--   0        0        0    22305 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/writeonly.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/pool/__init__.py
--rw-r--r--   0        0        0    52236 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/pool/base.py
--rw-r--r--   0        0        0    13147 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/pool/events.py
--rw-r--r--   0        0        0    18944 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/pool/impl.py
--rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/__init__.py
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_dml_constructors.py
--rw-r--r--   0        0        0    62587 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_elements_constructors.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_orm_types.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_py_util.py
--rw-r--r--   0        0        0    18780 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_selectable_constructors.py
--rw-r--r--   0        0        0    12713 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_typing.py
--rw-r--r--   0        0        0    18245 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/annotation.py
--rw-r--r--   0        0        0    73797 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/base.py
--rw-r--r--   0        0        0    33668 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/cache_key.py
--rw-r--r--   0        0        0    40493 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/coercions.py
--rw-r--r--   0        0        0   274503 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/compiler.py
--rw-r--r--   0        0        0    56521 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/crud.py
--rw-r--r--   0        0        0    45602 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/ddl.py
--rw-r--r--   0        0        0    16707 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/default_comparator.py
--rw-r--r--   0        0        0    65614 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/dml.py
--rw-r--r--   0        0        0   173693 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/elements.py
--rw-r--r--   0        0        0    18290 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/events.py
--rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/expression.py
--rw-r--r--   0        0        0    63689 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/functions.py
--rw-r--r--   0        0        0    49292 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/lambdas.py
--rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/naming.py
--rw-r--r--   0        0        0    75935 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/operators.py
--rw-r--r--   0        0        0     7662 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/roles.py
--rw-r--r--   0        0        0   228317 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/schema.py
--rw-r--r--   0        0        0   232848 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/selectable.py
--rw-r--r--   0        0        0   126076 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/sqltypes.py
--rw-r--r--   0        0        0    33589 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/traversals.py
--rw-r--r--   0        0        0    83208 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/type_api.py
--rw-r--r--   0        0        0    48077 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/util.py
--rw-r--r--   0        0        0    36317 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/visitors.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/__init__.py
--rw-r--r--   0        0        0    31439 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/assertions.py
--rw-r--r--   0        0        0    16817 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/assertsql.py
--rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/asyncio.py
--rw-r--r--   0        0        0    12090 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/config.py
--rw-r--r--   0        0        0    13481 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/engines.py
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/entities.py
--rw-r--r--   0        0        0    12460 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/exclusions.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/pickleable.py
--rw-r--r--   0        0        0    10148 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/profiling.py
--rw-r--r--   0        0        0    14619 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/provision.py
--rw-r--r--   0        0        0    51817 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/requirements.py
--rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/schema.py
--rw-r--r--   0        0        0    14080 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/util.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/warnings.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/__init__.py
--rw-r--r--   0        0        0    12256 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/base.py
--rw-r--r--   0        0        0    11973 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/mypy.py
--rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/orm.py
--rw-r--r--   0        0        0    15774 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/sql.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/__init__.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/bootstrap.py
--rw-r--r--   0        0        0    21578 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/plugin_base.py
--rw-r--r--   0        0        0    27656 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/pytestplugin.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/__init__.py
--rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_cte.py
--rw-r--r--   0        0        0    12031 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_ddl.py
--rw-r--r--   0        0        0     5337 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_deprecations.py
--rw-r--r--   0        0        0    22923 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_dialect.py
--rw-r--r--   0        0        0    18824 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_insert.py
--rw-r--r--   0        0        0   106466 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_reflection.py
--rw-r--r--   0        0        0    15937 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_results.py
--rw-r--r--   0        0        0     7900 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_rowcount.py
--rw-r--r--   0        0        0    58574 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_select.py
--rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_sequence.py
--rw-r--r--   0        0        0    65677 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_types.py
--rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_unicode_ddl.py
--rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_update_delete.py
--rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/__init__.py
--rw-r--r--   0        0        0    20063 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/_collections.py
--rw-r--r--   0        0        0     9191 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/_concurrency_py3k.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/_has_cy.py
--rw-r--r--   0        0        0    16714 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/_py_collections.py
--rw-r--r--   0        0        0     8714 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/compat.py
--rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/concurrency.py
--rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/deprecations.py
--rw-r--r--   0        0        0    64957 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/langhelpers.py
--rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/preloaded.py
--rw-r--r--   0        0        0    10185 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/queue.py
--rw-r--r--   0        0        0     6135 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/tool_support.py
--rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/topological.py
--rw-r--r--   0        0        0    16641 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/typing.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/INSTALLER
--rw-r--r--   0        0        0    13936 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/LICENSE
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/METADATA
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/WHEEL
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/docs/LICENSE.txt
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/docs/cli.md
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/docs/config.md
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/docs/gen_ref_pages.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/docs/json.md
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/docs/sql.md
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/docs/subprocess.md
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/docs/toml.md
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/docs/stylesheets/extra.css
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/fancy_dataclass/__init__.py
--rw-r--r--   0        0        0    14512 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/fancy_dataclass/cli.py
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/fancy_dataclass/config.py
--rw-r--r--   0        0        0    16986 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/fancy_dataclass/dict.py
--rw-r--r--   0        0        0     6562 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/fancy_dataclass/json.py
--rw-r--r--   0        0        0    11440 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/fancy_dataclass/mixin.py
--rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/fancy_dataclass/serialize.py
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/fancy_dataclass/sql.py
--rw-r--r--   0        0        0     8070 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/fancy_dataclass/subprocess.py
--rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/fancy_dataclass/toml.py
--rw-r--r--   0        0        0    20195 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/fancy_dataclass/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0    12195 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/tests/test_cli.py
--rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/tests/test_config.py
--rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/tests/test_dict.py
--rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/tests/test_inheritance.py
--rw-r--r--   0        0        0    10619 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/tests/test_mixin.py
--rw-r--r--   0        0        0    24866 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/tests/test_serializable.py
--rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/tests/test_sql.py
--rw-r--r--   0        0        0     7083 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/tests/test_subprocess.py
--rw-r--r--   0        0        0    11567 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/tests/test_utils.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/workflows/mypy.yml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/workflows/ruff.yml
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/.gitignore
--rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/docs/README.md
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.readthedocs.yaml
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/TODO.md
+-rw-r--r--   0        0        0     8949 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/fancy_dataclass.json
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/mkdocs.yml
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/ruff.toml
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/website_config.toml
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.github/workflows/workflow.yml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/.lock
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/CACHEDIR.TAG
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/pyvenv.cfg
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/bin/activate
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/bin/activate.bat
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/bin/activate.csh
+-rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/bin/activate.fish
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/bin/activate.nu
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/bin/activate.ps1
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/bin/activate_this.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/bin/deactivate.bat
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/bin/pydoc.bat
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/bin/python -> /Users/jerm/.pyenv/versions/3.11.0/bin/python3.11
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/bin/python3.11 -> python
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/_virtualenv.pth
+-rw-r--r--   0        0        0     4375 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/_virtualenv.py
+-rw-r--r--   0        0        0   117599 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/typing_extensions.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/LICENSE
+-rw-r--r--   0        0        0     9602 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/METADATA
+-rw-r--r--   0        0        0    24616 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/REQUESTED
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/WHEEL
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/top_level.txt
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass/__init__.py
+-rw-r--r--   0        0        0    13134 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass/cli.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass/config.py
+-rw-r--r--   0        0        0    16663 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass/dict.py
+-rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass/json.py
+-rw-r--r--   0        0        0    11440 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass/mixin.py
+-rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass/sql.py
+-rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass/subprocess.py
+-rw-r--r--   0        0        0    15970 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass/utils.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/direct_url.json
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/licenses/LICENSE.txt
+-rw-r--r--   0        0        0    13033 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/events.py
+-rw-r--r--   0        0        0    23976 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/exc.py
+-rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/inspection.py
+-rw-r--r--   0        0        0     8607 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/log.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/py.typed
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/schema.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/types.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/__init__.py
+-rw-r--r--   0        0        0     5288 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/aioodbc.py
+-rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/asyncio.py
+-rw-r--r--   0        0        0     8501 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/pyodbc.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/__init__.py
+-rwxr-xr-x   0        0        0   273374 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/collections.cpython-311-darwin.so
+-rw-r--r--   0        0        0    12571 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/collections.pyx
+-rwxr-xr-x   0        0        0   125312 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/immutabledict.cpython-311-darwin.so
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/immutabledict.pxd
+-rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/immutabledict.pyx
+-rwxr-xr-x   0        0        0   104925 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/processors.cpython-311-darwin.so
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/processors.pyx
+-rwxr-xr-x   0        0        0   107806 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/resultproxy.cpython-311-darwin.so
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/resultproxy.pyx
+-rwxr-xr-x   0        0        0   125335 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/util.cpython-311-darwin.so
+-rw-r--r--   0        0        0     2530 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/util.pyx
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/__init__.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/_typing.py
+-rw-r--r--   0        0        0     8239 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/type_migration_guidelines.txt
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/__init__.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/aioodbc.py
+-rw-r--r--   0        0        0   132301 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/base.py
+-rw-r--r--   0        0        0     8084 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/information_schema.py
+-rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/json.py
+-rw-r--r--   0        0        0     5362 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/provision.py
+-rw-r--r--   0        0        0     4038 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/pymssql.py
+-rw-r--r--   0        0        0    27056 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/pyodbc.py
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/__init__.py
+-rw-r--r--   0        0        0     9964 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/aiomysql.py
+-rw-r--r--   0        0        0    10033 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/asyncmy.py
+-rw-r--r--   0        0        0   120850 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/base.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/cymysql.py
+-rw-r--r--   0        0        0     7645 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/dml.py
+-rw-r--r--   0        0        0     8448 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/enumerated.py
+-rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/expression.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/json.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mariadb.py
+-rw-r--r--   0        0        0     8568 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mariadbconnector.py
+-rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mysqlconnector.py
+-rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mysqldb.py
+-rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/provision.py
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/pymysql.py
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/pyodbc.py
+-rw-r--r--   0        0        0    22822 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/reflection.py
+-rw-r--r--   0        0        0     9258 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/reserved_words.py
+-rw-r--r--   0        0        0    24343 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/types.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/__init__.py
+-rw-r--r--   0        0        0   118246 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/base.py
+-rw-r--r--   0        0        0    55566 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/cx_oracle.py
+-rw-r--r--   0        0        0    19519 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/dictionary.py
+-rw-r--r--   0        0        0     9487 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/oracledb.py
+-rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/provision.py
+-rw-r--r--   0        0        0     8231 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/types.py
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/__init__.py
+-rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/_psycopg_common.py
+-rw-r--r--   0        0        0    13734 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/array.py
+-rw-r--r--   0        0        0    40240 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/asyncpg.py
+-rw-r--r--   0        0        0   178989 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/base.py
+-rw-r--r--   0        0        0    11212 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/dml.py
+-rw-r--r--   0        0        0    16262 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/ext.py
+-rw-r--r--   0        0        0    11541 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/hstore.py
+-rw-r--r--   0        0        0    11217 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/json.py
+-rw-r--r--   0        0        0    17594 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/named_types.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/operators.py
+-rw-r--r--   0        0        0    18640 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/pg8000.py
+-rw-r--r--   0        0        0     9254 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/pg_catalog.py
+-rw-r--r--   0        0        0     5762 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/provision.py
+-rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg.py
+-rw-r--r--   0        0        0    31607 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg2.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg2cffi.py
+-rw-r--r--   0        0        0    32949 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/ranges.py
+-rw-r--r--   0        0        0     7300 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/types.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/__init__.py
+-rw-r--r--   0        0        0    12305 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/aiosqlite.py
+-rw-r--r--   0        0        0    96794 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/base.py
+-rw-r--r--   0        0        0     8443 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/dml.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/json.py
+-rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/provision.py
+-rw-r--r--   0        0        0     5356 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/pysqlcipher.py
+-rw-r--r--   0        0        0    28045 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/pysqlite.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/__init__.py
+-rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_processors.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_row.py
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_util.py
+-rw-r--r--   0        0        0   123050 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/base.py
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/characteristics.py
+-rw-r--r--   0        0        0    33206 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/create.py
+-rw-r--r--   0        0        0    76314 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/cursor.py
+-rw-r--r--   0        0        0    83993 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/default.py
+-rw-r--r--   0        0        0    37381 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/events.py
+-rw-r--r--   0        0        0   112832 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/interfaces.py
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/mock.py
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/processors.py
+-rw-r--r--   0        0        0    75127 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/reflection.py
+-rw-r--r--   0        0        0    77603 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/result.py
+-rw-r--r--   0        0        0    12032 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/row.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/strategies.py
+-rw-r--r--   0        0        0    30784 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/url.py
+-rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/util.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/event/__init__.py
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/event/api.py
+-rw-r--r--   0        0        0    20751 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/event/attr.py
+-rw-r--r--   0        0        0    14954 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/event/base.py
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/event/legacy.py
+-rw-r--r--   0        0        0    10835 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/event/registry.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/__init__.py
+-rw-r--r--   0        0        0    65771 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/associationproxy.py
+-rw-r--r--   0        0        0    61576 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/automap.py
+-rw-r--r--   0        0        0    17807 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/baked.py
+-rw-r--r--   0        0        0    20391 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/compiler.py
+-rw-r--r--   0        0        0    16750 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/horizontal_shard.py
+-rw-r--r--   0        0        0    52432 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/hybrid.py
+-rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/indexable.py
+-rw-r--r--   0        0        0    15707 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/instrumentation.py
+-rw-r--r--   0        0        0    37355 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mutable.py
+-rw-r--r--   0        0        0    14384 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/orderinglist.py
+-rw-r--r--   0        0        0     6178 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/serializer.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/__init__.py
+-rw-r--r--   0        0        0     8905 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/base.py
+-rw-r--r--   0        0        0    48190 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/engine.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/exc.py
+-rw-r--r--   0        0        0    30409 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/result.py
+-rw-r--r--   0        0        0    52597 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/scoping.py
+-rw-r--r--   0        0        0    63092 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/session.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/declarative/__init__.py
+-rw-r--r--   0        0        0    19547 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/declarative/extensions.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/__init__.py
+-rw-r--r--   0        0        0    10550 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/apply.py
+-rw-r--r--   0        0        0    17384 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/decl_class.py
+-rw-r--r--   0        0        0    19369 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/infer.py
+-rw-r--r--   0        0        0    10479 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/names.py
+-rw-r--r--   0        0        0     9750 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/plugin.py
+-rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/util.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/future/__init__.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/future/engine.py
+-rw-r--r--   0        0        0     8463 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/__init__.py
+-rw-r--r--   0        0        0    99461 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/_orm_constructors.py
+-rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/_typing.py
+-rw-r--r--   0        0        0    92535 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/attributes.py
+-rw-r--r--   0        0        0    27466 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/base.py
+-rw-r--r--   0        0        0    70022 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/bulk_persistence.py
+-rw-r--r--   0        0        0    17958 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/clsregistry.py
+-rw-r--r--   0        0        0    52179 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/collections.py
+-rw-r--r--   0        0        0   112001 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/context.py
+-rw-r--r--   0        0        0    63674 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/decl_api.py
+-rw-r--r--   0        0        0    81601 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/decl_base.py
+-rw-r--r--   0        0        0    47631 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/dependency.py
+-rw-r--r--   0        0        0    37180 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/descriptor_props.py
+-rw-r--r--   0        0        0     9786 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/dynamic.py
+-rw-r--r--   0        0        0    11925 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/evaluator.py
+-rw-r--r--   0        0        0   127703 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/events.py
+-rw-r--r--   0        0        0     7413 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/exc.py
+-rw-r--r--   0        0        0     9249 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/identity.py
+-rw-r--r--   0        0        0    24321 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/instrumentation.py
+-rw-r--r--   0        0        0    48502 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/interfaces.py
+-rw-r--r--   0        0        0    57537 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/loading.py
+-rw-r--r--   0        0        0    19690 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/mapped_collection.py
+-rw-r--r--   0        0        0   171059 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/mapper.py
+-rw-r--r--   0        0        0    25850 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/path_registry.py
+-rw-r--r--   0        0        0    61701 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/persistence.py
+-rw-r--r--   0        0        0    29294 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/properties.py
+-rw-r--r--   0        0        0   117596 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/query.py
+-rw-r--r--   0        0        0   128644 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/relationships.py
+-rw-r--r--   0        0        0    78677 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/scoping.py
+-rw-r--r--   0        0        0   193181 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/session.py
+-rw-r--r--   0        0        0    37520 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/state.py
+-rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/state_changes.py
+-rw-r--r--   0        0        0   114206 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/strategies.py
+-rw-r--r--   0        0        0    84563 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/strategy_options.py
+-rw-r--r--   0        0        0     5779 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/sync.py
+-rw-r--r--   0        0        0    27033 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/unitofwork.py
+-rw-r--r--   0        0        0    80660 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/util.py
+-rw-r--r--   0        0        0    22305 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/writeonly.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/pool/__init__.py
+-rw-r--r--   0        0        0    52236 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/pool/base.py
+-rw-r--r--   0        0        0    13147 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/pool/events.py
+-rw-r--r--   0        0        0    18944 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/pool/impl.py
+-rw-r--r--   0        0        0     5820 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/__init__.py
+-rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_dml_constructors.py
+-rw-r--r--   0        0        0    62587 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_elements_constructors.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_orm_types.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_py_util.py
+-rw-r--r--   0        0        0    18780 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_selectable_constructors.py
+-rw-r--r--   0        0        0    12713 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_typing.py
+-rw-r--r--   0        0        0    18245 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/annotation.py
+-rw-r--r--   0        0        0    73797 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/base.py
+-rw-r--r--   0        0        0    33668 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/cache_key.py
+-rw-r--r--   0        0        0    40493 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/coercions.py
+-rw-r--r--   0        0        0   274503 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/compiler.py
+-rw-r--r--   0        0        0    56521 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/crud.py
+-rw-r--r--   0        0        0    45602 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/ddl.py
+-rw-r--r--   0        0        0    16707 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/default_comparator.py
+-rw-r--r--   0        0        0    65614 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/dml.py
+-rw-r--r--   0        0        0   173693 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/elements.py
+-rw-r--r--   0        0        0    18290 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/events.py
+-rw-r--r--   0        0        0     7586 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/expression.py
+-rw-r--r--   0        0        0    63689 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/functions.py
+-rw-r--r--   0        0        0    49292 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/lambdas.py
+-rw-r--r--   0        0        0     6858 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/naming.py
+-rw-r--r--   0        0        0    75935 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/operators.py
+-rw-r--r--   0        0        0     7662 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/roles.py
+-rw-r--r--   0        0        0   228317 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/schema.py
+-rw-r--r--   0        0        0   232848 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/selectable.py
+-rw-r--r--   0        0        0   126076 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/sqltypes.py
+-rw-r--r--   0        0        0    33589 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/traversals.py
+-rw-r--r--   0        0        0    83208 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/type_api.py
+-rw-r--r--   0        0        0    48077 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/util.py
+-rw-r--r--   0        0        0    36317 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/visitors.py
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/__init__.py
+-rw-r--r--   0        0        0    31439 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/assertions.py
+-rw-r--r--   0        0        0    16817 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/assertsql.py
+-rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/asyncio.py
+-rw-r--r--   0        0        0    12090 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/config.py
+-rw-r--r--   0        0        0    13481 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/engines.py
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/entities.py
+-rw-r--r--   0        0        0    12460 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/exclusions.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/pickleable.py
+-rw-r--r--   0        0        0    10148 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/profiling.py
+-rw-r--r--   0        0        0    14619 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/provision.py
+-rw-r--r--   0        0        0    51817 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/requirements.py
+-rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/schema.py
+-rw-r--r--   0        0        0    14080 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/util.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/warnings.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/__init__.py
+-rw-r--r--   0        0        0    12256 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/base.py
+-rw-r--r--   0        0        0    11973 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/mypy.py
+-rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/orm.py
+-rw-r--r--   0        0        0    15774 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/sql.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/__init__.py
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/bootstrap.py
+-rw-r--r--   0        0        0    21578 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/plugin_base.py
+-rw-r--r--   0        0        0    27656 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/pytestplugin.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/__init__.py
+-rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_cte.py
+-rw-r--r--   0        0        0    12031 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_ddl.py
+-rw-r--r--   0        0        0     5337 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_deprecations.py
+-rw-r--r--   0        0        0    22923 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_dialect.py
+-rw-r--r--   0        0        0    18824 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_insert.py
+-rw-r--r--   0        0        0   106466 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_reflection.py
+-rw-r--r--   0        0        0    15937 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_results.py
+-rw-r--r--   0        0        0     7900 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_rowcount.py
+-rw-r--r--   0        0        0    58574 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_select.py
+-rw-r--r--   0        0        0     9923 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_sequence.py
+-rw-r--r--   0        0        0    65677 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_types.py
+-rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_unicode_ddl.py
+-rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_update_delete.py
+-rw-r--r--   0        0        0     8277 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/__init__.py
+-rw-r--r--   0        0        0    20063 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/_collections.py
+-rw-r--r--   0        0        0     9191 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/_concurrency_py3k.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/_has_cy.py
+-rw-r--r--   0        0        0    16714 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/_py_collections.py
+-rw-r--r--   0        0        0     8714 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/compat.py
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/concurrency.py
+-rw-r--r--   0        0        0    11971 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/deprecations.py
+-rw-r--r--   0        0        0    64957 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/langhelpers.py
+-rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/preloaded.py
+-rw-r--r--   0        0        0    10185 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/queue.py
+-rw-r--r--   0        0        0     6135 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/tool_support.py
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/topological.py
+-rw-r--r--   0        0        0    16641 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/typing.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0    13936 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/METADATA
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/WHEEL
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/docs/LICENSE.txt
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/docs/cli.md
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/docs/config.md
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/docs/json.md
+-rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/docs/sql.md
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/docs/subprocess.md
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/docs/toml.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/fancy_dataclass/__init__.py
+-rw-r--r--   0        0        0    14512 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/fancy_dataclass/cli.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/fancy_dataclass/config.py
+-rw-r--r--   0        0        0    16778 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/fancy_dataclass/dict.py
+-rw-r--r--   0        0        0     6562 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/fancy_dataclass/json.py
+-rw-r--r--   0        0        0    11440 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/fancy_dataclass/mixin.py
+-rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/fancy_dataclass/serialize.py
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/fancy_dataclass/sql.py
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/fancy_dataclass/subprocess.py
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/fancy_dataclass/toml.py
+-rw-r--r--   0        0        0    20328 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/fancy_dataclass/utils.py
+-rwxr-xr-x   0        0        0     2467 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/scripts/check_version.py
+-rwxr-xr-x   0        0        0      134 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/scripts/summarize.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0    12195 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/tests/test_cli.py
+-rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/tests/test_config.py
+-rw-r--r--   0        0        0     5577 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/tests/test_dict.py
+-rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/tests/test_inheritance.py
+-rw-r--r--   0        0        0    10619 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/tests/test_mixin.py
+-rw-r--r--   0        0        0    24866 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/tests/test_serializable.py
+-rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/tests/test_sql.py
+-rw-r--r--   0        0        0     7135 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/tests/test_subprocess.py
+-rw-r--r--   0        0        0    11986 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/tests/test_utils.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/.gitignore
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/docs/README.md
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 fancy_dataclass-0.3.1/PKG-INFO
```

### Comparing `fancy_dataclass-0.3.0/.pre-commit-config.yaml` & `fancy_dataclass-0.3.1/.pre-commit-config.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
-default_install_hook_types: [commit-msg, pre-commit]
+default_install_hook_types: [commit-msg, pre-commit, pre-push]
 default_stages: [commit]
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.5.0
   hooks:
     - id: check-added-large-files
       args: ['--maxkb=5000']
@@ -17,21 +17,27 @@
   hooks:
     - id: ruff
 - repo: https://github.com/netromdk/vermin
   rev: v1.6.0
   hooks:
     - id: vermin-all
       # specify your target version here, OR in a Vermin config file as usual:
-      args: ['-t=3.8-', '--no-tips', '--violations', '--exclude', 'enum.StrEnum', '.']
+      args: ['-t=3.8-', '--no-tips', '--violations', '--exclude', 'enum.StrEnum', '--exclude', 'types.UnionType', '.']
 - repo: https://github.com/commitizen-tools/commitizen
   rev: v3.20.0
   hooks:
     - id: commitizen
       stages: [commit-msg]
 - repo: local
   hooks:
     - id: summarize
       name: summarize
-      entry: summarize.sh
+      entry: scripts/summarize.sh
       language: script
       pass_filenames: false
       verbose: true
+    - id: check-version
+      stages: [commit, push]
+      name: check-version
+      entry: scripts/check_version.py
+      language: python
+      verbose: true
```

### Comparing `fancy_dataclass-0.3.0/TODO.md` & `fancy_dataclass-0.3.1/TODO.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # TODO
 
-## v0.3.0
+## v0.4.0
 
-- Github Actions for automated testing
-  - Coverage badge
-  - Auto-publish when new tag is pushed (see: https://pypi.org/manage/project/fancy-dataclass/settings/publishing/)
-- Release
-  - CHANGELOG update
-  - Tag v0.3.0
-  - Check PyPI page links to Read the Docs
+- `DictConfig` subclass of `Config` (unstructured configs loaded from JSON/TOML)
+- `FileSerializable`
+  - Add `save` and `load` convenience methods?
 
-## v0.3.1
+## v0.4.1
 
-- `DictConfig` subclass of `Config` (unstructured configs loaded from JSON/TOML)
+- `mkdocs` output in `package_data`?
+  - `_docs` subdirectory?
+  - Pre-commit hook to run `mkdocs build`
+    - Takse only a second, but could use file hashes to prevent redundant build
+  - Need some hook (post-tag?) to require the docs be up-to-date
 - documentation
   - Dataclass mixins/settings
     - For now, `dataclass` decorator is required
     - Note purpose of `flattened=True` (good for tabular data like CSV/SQL)
     - Advanced: how to handle name collisions in settings for multiple inheritance (e.g. `ArgparseDataclass`/`SubprocessDataclass`)
   - JSON
   - TOML
@@ -27,46 +27,49 @@
   - Subprocess
   - Config
   - Defining new mixins (what dunders need to be set)
     - Top-level settings, field-level settings, collisions
 
 ## Future
 
-- `FileSerializable`
-  - Add `save` and `load` convenience methods?
+- `TabularDataclass`? CSV/TSV/parquet/feather
+  - Simplest if single class can save/load all these file types
+  - Convert to/from `pandas` `Series` and `DataFrame`?
+    - If so, make `pandas` an optional dependency
+    - Easy to implement conversion via `dict`, if we subclass `DictDataclass`
 - `TOMLDataclass`
   - Require subclass to set `qualified_type=True`, like `JSONDataclass`?
   - Preserve document structure via `tomlkit`
     - NOTE: the parsed values themselves have a `_trivia` attribute storing various formatting info
     - Use field metadata (`help`?) as comment prior to the field
   - For `None`, serialize as commented field?
-- `TabularDataclass`? CSV/TSV/parquet/feather
-  - Make `SQLDataclass` inherit from it
-  - Convert to/from `pandas` `Series` and `DataFrame`?
-- Support subparsers in `ArgparseDataclass`
+- `ArgparseDataclass`
+  - Support subparsers
+  - Test subparsers, groups, mutually exclusive groups
 - Field metadata
   - Be strict about unknown field metadata keys? (Maybe issue warning?)
     - Might be annoying if people want to store extra metadata.
   - PEP 712 (`converter` argument for dataclass fields)
   - Allow `Annotated` as an alternative to `field.metadata`
     - Esp. with `Doc`: this could auto-populate JSON schema, argparse description
+- Tiered configs?
 - Improve `mkdocs` documentation
   - Auto-generate per-field descriptions via PEP 727?
   - Auto-generate dataclass field docs?
 - Automatic JSON schema generation (see `pydantic`)
   - Borrow/use: https://github.com/Peter554/dc_schema/tree/master?tab=MIT-1-ov-file#readme
     - Attribution?
 - Versioning (`version` ClassVar, with suppress=False)
   - `@version` decorator (with required integer argument)
     - Allows you to define multiple classes with the same name; stores distinct `version` `ClassVar` attributes and registers them with the same name
     - `from_dict` looks up the version number in the registry; if only newer exists:
       - If `strict=True`, raises an error; otherwise, attempts to coerce and issues a warning
     - Error if duplicate versions are set
   - Migration
-- `CallableDataclass`
+- `CallableDataclass` / `FuncDataclass`
   - ABC providing `__call__` method on variadic positional args
   - `callable_dataclass` decorator wrapping a function into a `CallableDataclass` subclass where `kwargs` are parameters
     - To make class name explicit, would probably need to call it directly, e.g. `MyType = callable_dataclass(my_func)`
 - Validation
   - More robust type validation when `validate=True` in `DictDataclass`
   - `ValidatedDataclass` to validate at construction time?
 - More test coverage
```

### Comparing `fancy_dataclass-0.3.0/fancy_dataclass.json` & `fancy_dataclass-0.3.1/fancy_dataclass.json`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/mkdocs.yml` & `fancy_dataclass-0.3.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/ruff.toml` & `fancy_dataclass-0.3.1/ruff.toml`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,16 @@
     "UP035"  # import replacements (collections.abc)
 ]
 # ignore = ["B019", "E203", "E251", "E301", "E302", "E305", "E306", "E501", "E722", "E731", "E741", "W292", "W391"]
 
 # paths to exclude
 lint.exclude = [
     ".venv",
-    "tmp*"
+    "tmp*",
+    "scripts/*",
 ]
 
 # ignore unused imports in __init__.py files
 lint.ignore-init-module-imports = true
 
 line-length = 10000
```

### Comparing `fancy_dataclass-0.3.0/.github/workflows/workflow.yml` & `fancy_dataclass-0.3.1/.github/workflows/workflow.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 name: fancy-dataclass
 
-on: [push, pull_request]
+on:
+  push:
+    branches:
+      - '*'  # matches every branch that doesn't contain a '/'
+      - '!coverage-badge'
+  pull_request:
 
 jobs:
   build:
     name: "Code checks"
     runs-on: ubuntu-latest
-    # strategy:
-    #   matrix:
-    #     python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
           python-version: |
             3.8
             3.9
             3.10
-            3.11
             3.12
+            3.11
       - name: Set up pip cache
         if: runner.os == 'Linux'
         uses: actions/cache@v4
         with:
           path: ~/.cache/pip
           key: ${{ runner.os }}-pip-${{ hashFiles('pyproject.toml') }}
           restore-keys: ${{ runner.os }}-pip-
       - name: Install hatch
         run: pip install hatch
       - name: Configure hatch
         run: hatch config set dirs.env.virtual .venv
       - name: Cache hatch virtualenv
-        uses: actions/cache@v2
+        uses: actions/cache@v4
         id: cache-venv
         with:
           path: ./.venv/
           # cache key depends on pyproject.toml
           key: ${{ runner.os }}-venv-${{ hashFiles('pyproject.toml') }}
           restore-keys: |
             ${{ runner.os }}-venv-
@@ -53,13 +55,29 @@
       - name: Lint (ruff)
         run: hatch run lint:run-ruff
       - name: Python compatibility (vermin)
         run: hatch run lint:run-vermin
       - name: Type-check (mypy)
         run: hatch run lint:run-mypy
       - name: Test (pytest)
-        run: hatch run test:test --verbosity=0
+        run: |
+          hatch run test:test --verbosity=0
+          hatch run test.py3.11:cov-report
+      - name: Coverage Badge
+        run: |
+          hatch run badge:badges
+          git checkout -B coverage-badge
+          git config --local user.email "github-actions[bot]@users.noreply.github.com"
+          git config --local user.name "github-actions[bot]"
+          git add coverage-badge.svg
+          git commit -m "ci: update coverage badge"
+      - name: Push changes
+        uses: ad-m/github-push-action@master
+        with:
+          github_token: ${{ secrets.github_token }}
+          branch: coverage-badge
+          force: true
       # - name: Build dist
       #   run: hatch build
       # - name: Publish on PyPI
       #   if: github.ref == 'refs/heads/main'
       #   run: hatch publish
```

### Comparing `fancy_dataclass-0.3.0/.venv/bin/activate` & `fancy_dataclass-0.3.1/.venv/bin/activate`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/bin/activate.bat` & `fancy_dataclass-0.3.1/.venv/bin/activate.bat`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/bin/activate.csh` & `fancy_dataclass-0.3.1/.venv/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/bin/activate.fish` & `fancy_dataclass-0.3.1/.venv/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/bin/activate.nu` & `fancy_dataclass-0.3.1/.venv/bin/activate.nu`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/bin/activate.ps1` & `fancy_dataclass-0.3.1/.venv/bin/activate.ps1`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/bin/activate_this.py` & `fancy_dataclass-0.3.1/.venv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/bin/deactivate.bat` & `fancy_dataclass-0.3.1/.venv/bin/deactivate.bat`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/bin/pydoc.bat` & `fancy_dataclass-0.3.1/.venv/bin/pydoc.bat`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/_virtualenv.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/_virtualenv.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/typing_extensions.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/LICENSE` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/METADATA` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/RECORD` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/SQLAlchemy-2.0.29.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/cli.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass/cli.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/config.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass/config.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/dict.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass/dict.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/json.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass/json.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/mixin.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass/mixin.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/sql.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass/sql.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/subprocess.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass/subprocess.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass/utils.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass/utils.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/METADATA` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/RECORD` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/licenses/LICENSE.txt` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/fancy_dataclass-0.2.0.dist-info/licenses/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/__init__.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/events.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/events.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/exc.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/exc.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/inspection.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/inspection.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/log.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/log.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/schema.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/schema.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/types.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/aioodbc.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/aioodbc.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/asyncio.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/asyncio.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/pyodbc.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/connectors/pyodbc.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/collections.cpython-311-darwin.so` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/collections.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/collections.pyx` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/collections.pyx`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/immutabledict.cpython-311-darwin.so` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/immutabledict.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/immutabledict.pyx` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/immutabledict.pyx`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/processors.cpython-311-darwin.so` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/processors.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/processors.pyx` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/processors.pyx`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/resultproxy.cpython-311-darwin.so` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/resultproxy.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/resultproxy.pyx` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/resultproxy.pyx`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/util.cpython-311-darwin.so` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/util.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/util.pyx` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/cyextension/util.pyx`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/__init__.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/_typing.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/_typing.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/type_migration_guidelines.txt` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/type_migration_guidelines.txt`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/__init__.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/aioodbc.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/aioodbc.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/base.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/information_schema.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/information_schema.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/json.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/json.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/provision.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/provision.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/pymssql.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/pymssql.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/pyodbc.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mssql/pyodbc.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/__init__.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/aiomysql.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/aiomysql.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/asyncmy.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/asyncmy.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/base.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/cymysql.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/cymysql.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/dml.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/dml.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/enumerated.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/enumerated.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/expression.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/expression.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/json.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/json.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mariadb.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mariadb.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mariadbconnector.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mariadbconnector.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mysqlconnector.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mysqlconnector.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mysqldb.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/mysqldb.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/provision.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/provision.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/pymysql.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/pymysql.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/pyodbc.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/pyodbc.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/reflection.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/reflection.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/reserved_words.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/reserved_words.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/types.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/mysql/types.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/__init__.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/base.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/cx_oracle.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/cx_oracle.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/dictionary.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/dictionary.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/oracledb.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/oracledb.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/provision.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/provision.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/types.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/oracle/types.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/__init__.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/_psycopg_common.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/_psycopg_common.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/array.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/array.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/asyncpg.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/asyncpg.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/base.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/dml.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/dml.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/ext.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/ext.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/hstore.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/hstore.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/json.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/json.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/named_types.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/named_types.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/operators.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/operators.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/pg8000.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/pg8000.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/pg_catalog.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/pg_catalog.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/provision.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/provision.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg2.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg2.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg2cffi.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/psycopg2cffi.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/ranges.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/ranges.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/types.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/postgresql/types.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/__init__.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/aiosqlite.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/aiosqlite.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/base.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/dml.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/dml.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/json.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/json.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/provision.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/provision.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/pysqlcipher.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/pysqlcipher.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/pysqlite.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/dialects/sqlite/pysqlite.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/__init__.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_processors.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_processors.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_row.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_row.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_util.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/_py_util.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/base.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/characteristics.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/characteristics.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/create.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/create.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/cursor.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/cursor.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/default.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/default.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/events.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/events.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/interfaces.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/interfaces.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/mock.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/mock.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/processors.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/processors.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/reflection.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/reflection.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/result.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/result.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/row.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/row.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/url.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/url.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/engine/util.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/engine/util.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/__init__.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/event/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/api.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/event/api.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/attr.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/event/attr.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/base.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/event/base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/legacy.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/event/legacy.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/event/registry.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/event/registry.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/associationproxy.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/associationproxy.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/automap.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/automap.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/baked.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/baked.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/compiler.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/compiler.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/horizontal_shard.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/horizontal_shard.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/hybrid.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/hybrid.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/indexable.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/indexable.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/instrumentation.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/instrumentation.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mutable.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mutable.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/orderinglist.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/orderinglist.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/serializer.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/serializer.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/__init__.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/base.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/engine.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/engine.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/exc.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/exc.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/result.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/result.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/scoping.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/scoping.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/session.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/asyncio/session.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/declarative/__init__.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/declarative/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/declarative/extensions.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/declarative/extensions.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/apply.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/apply.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/decl_class.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/decl_class.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/infer.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/infer.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/names.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/names.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/plugin.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/plugin.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/util.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/ext/mypy/util.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/future/__init__.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/future/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/__init__.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/_orm_constructors.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/_orm_constructors.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/_typing.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/_typing.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/attributes.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/attributes.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/base.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/bulk_persistence.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/bulk_persistence.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/clsregistry.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/clsregistry.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/collections.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/collections.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/context.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/context.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/decl_api.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/decl_api.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/decl_base.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/decl_base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/dependency.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/dependency.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/descriptor_props.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/descriptor_props.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/dynamic.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/dynamic.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/evaluator.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/evaluator.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/events.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/events.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/exc.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/exc.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/identity.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/identity.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/instrumentation.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/instrumentation.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/interfaces.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/interfaces.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/loading.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/loading.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/mapped_collection.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/mapped_collection.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/mapper.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/mapper.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/path_registry.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/path_registry.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/persistence.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/persistence.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/properties.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/properties.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/query.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/query.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/relationships.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/relationships.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/scoping.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/scoping.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/session.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/session.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/state.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/state.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/state_changes.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/state_changes.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/strategies.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/strategies.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/strategy_options.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/strategy_options.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/sync.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/sync.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/unitofwork.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/unitofwork.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/util.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/util.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/orm/writeonly.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/orm/writeonly.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/pool/__init__.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/pool/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/pool/base.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/pool/base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/pool/events.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/pool/events.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/pool/impl.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/pool/impl.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/__init__.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_dml_constructors.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_dml_constructors.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_elements_constructors.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_elements_constructors.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_orm_types.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_orm_types.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_py_util.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_py_util.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_selectable_constructors.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_selectable_constructors.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_typing.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/_typing.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/annotation.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/annotation.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/base.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/cache_key.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/cache_key.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/coercions.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/coercions.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/compiler.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/compiler.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/crud.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/crud.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/ddl.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/ddl.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/default_comparator.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/default_comparator.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/dml.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/dml.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/elements.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/elements.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/events.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/events.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/expression.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/expression.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/functions.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/functions.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/lambdas.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/lambdas.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/naming.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/naming.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/operators.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/operators.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/roles.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/roles.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/schema.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/schema.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/selectable.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/selectable.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/sqltypes.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/sqltypes.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/traversals.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/traversals.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/type_api.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/type_api.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/util.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/util.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/sql/visitors.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/sql/visitors.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/__init__.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/assertions.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/assertsql.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/assertsql.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/asyncio.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/asyncio.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/config.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/config.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/engines.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/engines.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/entities.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/entities.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/exclusions.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/exclusions.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/pickleable.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/pickleable.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/profiling.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/profiling.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/provision.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/provision.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/requirements.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/requirements.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/schema.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/schema.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/util.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/util.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/warnings.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/warnings.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/__init__.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/base.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/mypy.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/mypy.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/orm.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/orm.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/sql.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/fixtures/sql.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/bootstrap.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/bootstrap.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/plugin_base.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/plugin_base.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/pytestplugin.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/plugin/pytestplugin.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/__init__.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_cte.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_cte.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_ddl.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_ddl.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_deprecations.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_deprecations.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_dialect.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_dialect.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_insert.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_insert.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_reflection.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_reflection.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_results.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_results.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_rowcount.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_rowcount.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_select.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_select.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_sequence.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_sequence.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_types.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_types.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_unicode_ddl.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_unicode_ddl.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_update_delete.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/testing/suite/test_update_delete.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/__init__.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/__init__.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/_collections.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/_collections.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/_concurrency_py3k.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/_concurrency_py3k.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/_has_cy.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/_has_cy.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/_py_collections.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/_py_collections.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/compat.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/compat.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/concurrency.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/concurrency.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/deprecations.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/deprecations.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/langhelpers.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/langhelpers.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/preloaded.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/preloaded.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/queue.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/queue.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/tool_support.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/tool_support.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/topological.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/topological.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/sqlalchemy/util/typing.py` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/sqlalchemy/util/typing.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/LICENSE` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/METADATA` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/RECORD` & `fancy_dataclass-0.3.1/.venv/lib/python3.11/site-packages/typing_extensions-4.10.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/docs/CHANGELOG.md` & `fancy_dataclass-0.3.1/docs/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -12,19 +12,48 @@
     - Removed
     - Fixed
     - Security
 -->
 
 ## [Unreleased]
 
+## [0.3.1]
+
+2024-04-16
+
+### Added
+
+- Documentation: Badges in README (workflow passing, coverage, docs, etc.)
+- CI:
+    - More GH Actions code checks
+    - Testing Python versions 3.8-3.12 via `hatch` matrix
+
+### Changed
+
+- Top-level `*`-imports mostly limited to mixin classes via `__all__`
+- Renamed `Config.configure` context manager to `as_config`
+- Renamed `SubprocessDataclass.args` method to `get_args`
+
+### Fixed
+
+- Support for Python 3.8, 3.9 (which lack some newer type annotation features)
+
+## [0.3.0]
+
+2024-04-14
+
 ### Added
 
 - `TOMLDataclass` for saving/loading TOML via [`tomlkit`](https://tomlkit.readthedocs.io/en/latest/)
     - Support for loading TOML configurations in `ConfigDataclass`
 - `FileSerializable` and `DictFileSerializableDataclass` mixins to factor out shared functionality between JSON/TOML serialization
+- Documentation
+    - Usage examples for `TOMLDataclass` and `ConfigDataclass`
+    - Hosting on Read the Docs [here](https://fancy-dataclass.readthedocs.io/en/latest/)
+- CI: Github Actions to automate building/linting/testing
 
 ## [0.2.0]
 
 2024-04-13
 
 ### Added
 
@@ -60,15 +89,17 @@
     - `ArgparseDataclass`: command-line argument parsing
     - `CLIDataclass`: command-line argument parsing and `main` function
     - `DictDataclass`: conversion to/from Python dict
     - `JSONDataclass`: conversion to/from JSON
     - `SQLDataclass`: SQL persistence via `sqlalchemy`
     - `SubprocessDataclass`: call out to another program via `subprocess`
 
-[unreleased]: https://github.com/jeremander/fancy-dataclass/compare/v0.2.0...HEAD
+[unreleased]: https://github.com/jeremander/fancy-dataclass/compare/v0.3.1...HEAD
+[0.3.1]: https://github.com/jeremander/fancy-dataclass/releases/tag/v0.3.1
+[0.3.0]: https://github.com/jeremander/fancy-dataclass/releases/tag/v0.3.0
 [0.2.0]: https://github.com/jeremander/fancy-dataclass/releases/tag/v0.2.0
 [0.1.0]: https://github.com/jeremander/fancy-dataclass/releases/tag/v0.1.0
 
 <br>
 
 <!-- hide version subsections in nav sidebar -->
```

#### html2text {}

```diff
@@ -1,29 +1,41 @@
 # Changelog All notable changes to this project will be documented in this
 file. The format is based on [Keep a Changelog](https://keepachangelog.com/en/
 1.1.0/), and this project attempts to adhere to [Semantic Versioning](https://
-semver.org/spec/v2.0.0.html). ## [Unreleased] ### Added - `TOMLDataclass` for
-saving/loading TOML via [`tomlkit`](https://tomlkit.readthedocs.io/en/latest/
-) - Support for loading TOML configurations in `ConfigDataclass` -
-`FileSerializable` and `DictFileSerializableDataclass` mixins to factor out
-shared functionality between JSON/TOML serialization ## [0.2.0] 2024-04-13 ###
-Added - `ConfigDataclass` mixin for global configurations - Customization of
-`DataclassMixin`: - `DataclassMixinSettings` for mixin class configuration -
-`FieldSettings` for field-specific settings - `__post_dataclass_wrap__` hook to
-customize behavior after `dataclass` decorator is applied (e.g. validating
-fields at definition time) - Documentation - [Reference pages](README.md) via
-[`mkdocs-material`](https://squidfunk.github.io/mkdocs-material) and
-[`mkdocstrings`](https://mkdocstrings.github.io) - Basic usage examples for
-main mixin classes - [CHANGELOG](#changelog) - Linting via [`ruff`](https://
-docs.astral.sh/ruff/) - Unit tests - Over 90% code coverage, via [`pytest-cov`]
-(https://pytest-cov.readthedocs.io/en/latest/readme.html) ### Changed - Build
-via [`hatch`](https://github.com/pypa/hatch) - Better flattened/nested
-dataclass conversions ### Fixed - More robust type handling ## [0.1.0] 2022-06-
-06 ### Added - `DataclassMixin` class providing extra dataclass features -
+semver.org/spec/v2.0.0.html). ## [Unreleased] ## [0.3.1] 2024-04-16 ### Added -
+Documentation: Badges in README (workflow passing, coverage, docs, etc.) - CI:
+- More GH Actions code checks - Testing Python versions 3.8-3.12 via `hatch`
+matrix ### Changed - Top-level `*`-imports mostly limited to mixin classes via
+`__all__` - Renamed `Config.configure` context manager to `as_config` - Renamed
+`SubprocessDataclass.args` method to `get_args` ### Fixed - Support for Python
+3.8, 3.9 (which lack some newer type annotation features) ## [0.3.0] 2024-04-14
+### Added - `TOMLDataclass` for saving/loading TOML via [`tomlkit`](https://
+tomlkit.readthedocs.io/en/latest/) - Support for loading TOML configurations in
+`ConfigDataclass` - `FileSerializable` and `DictFileSerializableDataclass`
+mixins to factor out shared functionality between JSON/TOML serialization -
+Documentation - Usage examples for `TOMLDataclass` and `ConfigDataclass` -
+Hosting on Read the Docs [here](https://fancy-dataclass.readthedocs.io/en/
+latest/) - CI: Github Actions to automate building/linting/testing ## [0.2.0]
+2024-04-13 ### Added - `ConfigDataclass` mixin for global configurations -
+Customization of `DataclassMixin`: - `DataclassMixinSettings` for mixin class
+configuration - `FieldSettings` for field-specific settings -
+`__post_dataclass_wrap__` hook to customize behavior after `dataclass`
+decorator is applied (e.g. validating fields at definition time) -
+Documentation - [Reference pages](README.md) via [`mkdocs-material`](https://
+squidfunk.github.io/mkdocs-material) and [`mkdocstrings`](https://
+mkdocstrings.github.io) - Basic usage examples for main mixin classes -
+[CHANGELOG](#changelog) - Linting via [`ruff`](https://docs.astral.sh/ruff/) -
+Unit tests - Over 90% code coverage, via [`pytest-cov`](https://pytest-
+cov.readthedocs.io/en/latest/readme.html) ### Changed - Build via [`hatch`]
+(https://github.com/pypa/hatch) - Better flattened/nested dataclass conversions
+### Fixed - More robust type handling ## [0.1.0] 2022-06-06 ### Added -
+`DataclassMixin` class providing extra dataclass features -
 `ArgparseDataclass`: command-line argument parsing - `CLIDataclass`: command-
 line argument parsing and `main` function - `DictDataclass`: conversion to/from
 Python dict - `JSONDataclass`: conversion to/from JSON - `SQLDataclass`: SQL
 persistence via `sqlalchemy` - `SubprocessDataclass`: call out to another
 program via `subprocess` [unreleased]: https://github.com/jeremander/fancy-
-dataclass/compare/v0.2.0...HEAD [0.2.0]: https://github.com/jeremander/fancy-
+dataclass/compare/v0.3.1...HEAD [0.3.1]: https://github.com/jeremander/fancy-
+dataclass/releases/tag/v0.3.1 [0.3.0]: https://github.com/jeremander/fancy-
+dataclass/releases/tag/v0.3.0 [0.2.0]: https://github.com/jeremander/fancy-
 dataclass/releases/tag/v0.2.0 [0.1.0]: https://github.com/jeremander/fancy-
 dataclass/releases/tag/v0.1.0
```

### Comparing `fancy_dataclass-0.3.0/docs/LICENSE.txt` & `fancy_dataclass-0.3.1/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/docs/cli.md` & `fancy_dataclass-0.3.1/docs/cli.md`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,18 @@
 3
 ```
 
 ## Details
 
 🚧 **Under construction** 🚧
 
+<!--
+- Can modify parser manually, or customize handling a specific arg
+-->
+
 <style>
 .md-sidebar--secondary {
     display: none !important;
 }
 
 .md-main__inner .md-content {
     max-width: 45rem;
```

### Comparing `fancy_dataclass-0.3.0/docs/config.md` & `fancy_dataclass-0.3.1/docs/config.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 @dataclass
 class WebsiteConfig(ConfigDataclass):
     site: SiteInfo
     server: ServerConfig
     database: DatabaseConfig
 ```
 
-Now suppose you have a configuration file we want to load from, `website_config.toml`, whose schema matches the `WebsiteConfig` class:
+Now suppose you have a configuration file you want to load from, `website_config.toml`, whose schema matches the `WebsiteConfig` class:
 
 ```toml
 # Website Configuration
 
 [site]
 title = "My Awesome Website"
 author = "Webby McWebface"
@@ -83,34 +83,38 @@
     global_cfg = WebsiteConfig.get_config()
     print(global_cfg.database.username)
 ```
 
 ```python
 >>> print_current_username()
 admin
-# updates only the local copy
+
+# update only the local copy
 >>> cfg.database.username = 'test'
 >>> print_current_username()
 admin
-# updates the global config
+
+# update the global config
 >>> cfg.update_config()
 >>> print_current_username()
 test
 ```
 
 Sometimes it is useful to modify the configs temporarily:
 
 ```python
 >>> print_current_username()
 test
 >>> cfg.database.username = 'temporary'
+
 # temporarily update global config with the local version
->>> with cfg.configure():
+>>> with cfg.as_config():
         print_current_username()
 temporary
+
 # global config reverts back to its value before 'configure' was called
 >>> print_current_username()
 test
 ```
 
 ## Details
```

### Comparing `fancy_dataclass-0.3.0/docs/gen_ref_pages.py` & `fancy_dataclass-0.3.1/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/docs/json.md` & `fancy_dataclass-0.3.1/docs/json.md`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/docs/sql.md` & `fancy_dataclass-0.3.1/docs/sql.md`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/docs/subprocess.md` & `fancy_dataclass-0.3.1/docs/subprocess.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,16 @@
 
 Instantiate `ListDir`, inspect its arguments, and call `ls` in a subprocess.
 
 ```python
 >>> listdir = ListDir(long=True, dir_name='test_dir')
 >>> listdir.get_executable()
 'ls'
->>> listdir.args()
-['-l', 'test_dir']
+>>> listdir.get_args()
+['ls', '-l', 'test_dir']
 >>> listdir.run_subprocess()
 total 0
 -rw-r--r--  1 root  root  0 Apr  5 23:33 test.txt
 ```
 
 ## Details
```

### Comparing `fancy_dataclass-0.3.0/docs/toml.md` & `fancy_dataclass-0.3.1/docs/toml.md`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/docs/stylesheets/extra.css` & `fancy_dataclass-0.3.1/docs/stylesheets/extra.css`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 .md-nav__title {
   /* color: #303030;
   font-size: 12pt;
   font-style: italic; */
   visibility: hidden;
 }
 
+.md-nav__source {
+  background-color: var(--md-primary-fg-color);
+}
+
 .md-search__input {
   background-color: #707070;
   border-radius: 3px;
 }
 
 .md-nav__link--active {
   font-weight: bold;
```

### Comparing `fancy_dataclass-0.3.0/fancy_dataclass/cli.py` & `fancy_dataclass-0.3.1/fancy_dataclass/cli.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/fancy_dataclass/config.py` & `fancy_dataclass-0.3.1/fancy_dataclass/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         cls._set_config(None)
 
     def update_config(self) -> None:
         """Updates the global configuration, setting it equal to this object."""
         type(self)._set_config(self)
 
     @contextmanager
-    def configure(self) -> Iterator[None]:
+    def as_config(self) -> Iterator[None]:
         """Context manager which temporarily updates the global configuration with this object."""
         try:
             orig_config = type(self).get_config()
             self.update_config()
             yield
         finally:
             type(self)._set_config(orig_config)
```

### Comparing `fancy_dataclass-0.3.0/fancy_dataclass/dict.py` & `fancy_dataclass-0.3.1/fancy_dataclass/dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from dataclasses import Field, dataclass
 from functools import partial
 from typing import TYPE_CHECKING, Any, ClassVar, Dict, Iterable, Literal, Optional, Type, TypeVar, Union, _TypedDictMeta, get_args, get_origin  # type: ignore[attr-defined]
 
 from typing_extensions import Self, _AnnotatedAlias
 
 from fancy_dataclass.mixin import DataclassMixin, DataclassMixinSettings, FieldSettings
-from fancy_dataclass.utils import TypeConversionError, _flatten_dataclass, check_dataclass, fully_qualified_class_name, issubclass_safe, obj_class_name, safe_dict_insert, type_is_optional
+from fancy_dataclass.utils import TypeConversionError, _flatten_dataclass, check_dataclass, fully_qualified_class_name, issubclass_safe, obj_class_name, safe_dict_insert
 
 
 if TYPE_CHECKING:
     from _typeshed import DataclassInstance
 
 T = TypeVar('T', bound=DataclassMixin)
 D = TypeVar('D', bound='DataclassInstance')
@@ -246,18 +246,14 @@
             elif origin_type == tuple:
                 subtypes = args
                 if subtypes[-1] == Ellipsis:  # treat it like a list
                     subtype = subtypes[0]
                     return tuple(convert_val(subtype, elt) for elt in val)
                 return tuple(convert_val(subtype, elt) for (subtype, elt) in zip(args, val))
             elif origin_type == Union:
-                if type_is_optional(tp):
-                    assert len(args) == 2
-                    assert args[1] is type(None)
-                    args = args[::-1]  # check None first
                 for subtype in args:
                     try:
                         # NB: will resolve to the first valid type in the Union
                         return convert_val(subtype, val)
                     except Exception:
                         continue
             elif origin_type == Literal:
```

### Comparing `fancy_dataclass-0.3.0/fancy_dataclass/json.py` & `fancy_dataclass-0.3.1/fancy_dataclass/json.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/fancy_dataclass/mixin.py` & `fancy_dataclass-0.3.1/fancy_dataclass/mixin.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/fancy_dataclass/serialize.py` & `fancy_dataclass-0.3.1/fancy_dataclass/serialize.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/fancy_dataclass/sql.py` & `fancy_dataclass-0.3.1/fancy_dataclass/sql.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/fancy_dataclass/subprocess.py` & `fancy_dataclass-0.3.1/fancy_dataclass/subprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         if get_origin(fld.type) is ClassVar:
             # ignore fields associated with the class, rather than the instance
             return []
         val = getattr(self, name, None)
         if val is None:  # optional value is None
             return []
         if isinstance(val, SubprocessDataclass):  # get args via nested SubprocessDataclass
-            return val.args(suppress_defaults=suppress_defaults)
+            return val.get_args(suppress_defaults=suppress_defaults)
         if suppress_defaults:  # if value matches the default, suppress the argument
             default = None
             has_default = True
             if fld.default == MISSING:
                 if fld.default_factory == MISSING:
                     has_default = False
                 else:
@@ -136,15 +136,15 @@
         if self.__settings__.exec:
             return _check_type(self.__settings__.exec)
         for fld in get_dataclass_fields(self, include_classvars=True):
             if fld.metadata.get('exec', False):
                 return _check_type(getattr(self, fld.name, None))
         return None
 
-    def args(self, suppress_defaults: bool = False) -> List[str]:
+    def get_args(self, suppress_defaults: bool = False) -> List[str]:
         """Converts dataclass fields to a list of command-line arguments for a subprocess call.
 
         This includes the executable name itself as the first argument.
 
         Args:
             suppress_defaults: If `True`, suppresses arguments that are equal to the default values
 
@@ -165,8 +165,8 @@
             kwargs: Keyword arguments passed to `subprocess.run`
 
         Returns:
             `CompletedProcess` object produced by `subprocess.run`
 
         Raises:
             ValueError: If no executable was found from the `get_executable` method"""
-        return subprocess.run(self.args(), **kwargs)
+        return subprocess.run(self.get_args(), **kwargs)
```

### Comparing `fancy_dataclass-0.3.0/fancy_dataclass/toml.py` & `fancy_dataclass-0.3.1/fancy_dataclass/toml.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/fancy_dataclass/utils.py` & `fancy_dataclass-0.3.1/fancy_dataclass/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from copy import copy
 import dataclasses
 from dataclasses import Field, dataclass, is_dataclass, make_dataclass
 from functools import lru_cache
 import importlib
 from pathlib import Path
 import re
+import types
 from typing import TYPE_CHECKING, Any, BinaryIO, Callable, Dict, ForwardRef, Generic, Iterable, Iterator, List, Optional, Sequence, Set, TextIO, Tuple, Type, TypeVar, Union, get_args, get_origin, get_type_hints
 
 from typing_extensions import TypeGuard
 
 
 if TYPE_CHECKING:
     from _typeshed import DataclassInstance
@@ -51,15 +52,18 @@
     Args:
         tp: Type to check
 
     Returns:
         True if the type is Optional"""
     origin_type = get_origin(tp)
     args = get_args(tp)
-    return (origin_type == Union) and (len(args) == 2) and (type(None) in args)
+    union_types: List[Any] = [Union]
+    if hasattr(types, 'UnionType'):  # Python >= 3.10
+        union_types.append(types.UnionType)
+    return (origin_type in union_types) and (type(None) in args)
 
 def safe_dict_insert(d: Dict[Any, Any], key: str, val: Any) -> None:
     """Inserts a (key, value) pair into a dict, if the key is not already present.
 
     Args:
         d: Dict to modify
         key: Key to insert
```

### Comparing `fancy_dataclass-0.3.0/tests/test_cli.py` & `fancy_dataclass-0.3.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/tests/test_config.py` & `fancy_dataclass-0.3.1/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,24 +27,24 @@
     assert MyConfig.get_config() == cfg
     assert MyConfig.get_config() is not cfg
     cfg2 = MyConfig()
     assert MyConfig.get_config() == cfg2
     assert MyConfig.get_config() is not cfg2
     cfg2.y = 'b'
     assert cfg2 != cfg
-    with cfg2.configure():
+    with cfg2.as_config():
         assert MyConfig.get_config() == cfg2
         assert MyConfig.get_config() is not cfg2
         # updating instance field affects the global config
         cfg2.y = 'c'
         assert MyConfig.get_config().y == 'c'
     assert MyConfig.get_config() == cfg
     MyConfig.clear_config()
     assert MyConfig.get_config() is None
-    with cfg2.configure():
+    with cfg2.as_config():
         assert MyConfig.get_config() == cfg2
         assert MyConfig.get_config() is not cfg2
     assert MyConfig.get_config() is None
     @dataclass
     class OuterConfig(ConfigDataclass):
         inner: MyConfig
         z: float = 3.14
@@ -84,15 +84,15 @@
     inner.x = 3
     assert Outer.get_config().inner.x == 3
     inner_copy = deepcopy(inner)
     inner_copy.x = 4
     assert Outer.get_config().inner.x == 3
     cfg.inner = inner_copy
     assert Outer.get_config().inner.x == 4
-    with Outer(Inner(x=5)).configure():
+    with Outer(Inner(x=5)).as_config():
         assert Outer.get_config().inner.x == 5
     assert Outer.get_config().inner.x == 4
     toml_str = 'y = "a"\n[inner]\nx = 1\n'
     cfg_path = tmpdir / 'test.toml'
     Path(cfg_path).write_text(toml_str)
     Outer.load_config(cfg_path)
     assert Outer.get_config() == Outer(Inner())
```

### Comparing `fancy_dataclass-0.3.0/tests/test_dict.py` & `fancy_dataclass-0.3.1/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/tests/test_inheritance.py` & `fancy_dataclass-0.3.1/tests/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/tests/test_mixin.py` & `fancy_dataclass-0.3.1/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/tests/test_serializable.py` & `fancy_dataclass-0.3.1/tests/test_serializable.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/tests/test_sql.py` & `fancy_dataclass-0.3.1/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `fancy_dataclass-0.3.0/tests/test_subprocess.py` & `fancy_dataclass-0.3.1/tests/test_subprocess.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     DC2FieldSettings = merge_dataclasses(DC1.__field_settings_type__, SubprocessDataclassFieldSettings, allow_duplicates=True)
     @dataclass
     class DC2(DictDataclass, DC1, SubprocessDataclass):
         __field_settings_type__ = DC2FieldSettings
         prog: str = field(default = 'prog', metadata = {'exec': True})
     prog = str(tmpdir / 'prog.py')
     dc2 = DC2(required_string='positional_arg', input_file='my_input', output_file='my_output', choice='a', optional='default', flag=True, extra_items=[], x=7, y=3.14, pair=(0,0), ignored_value='ignored', prog = prog)
-    assert dc2.args() == [prog, 'positional_arg', '-i', 'my_input', '-o', 'my_output', '--choice', 'a', '--optional', 'default', '--flag', '-x', '7', '-y', '3.14', '--pair', '0', '0']
-    assert dc2.args(suppress_defaults=True) == [prog, 'positional_arg', '-i', 'my_input', '-o', 'my_output', '--flag']
+    assert dc2.get_args() == [prog, 'positional_arg', '-i', 'my_input', '-o', 'my_output', '--choice', 'a', '--optional', 'default', '--flag', '-x', '7', '-y', '3.14', '--pair', '0', '0']
+    assert dc2.get_args(suppress_defaults=True) == [prog, 'positional_arg', '-i', 'my_input', '-o', 'my_output', '--flag']
     # create a script to run the CLIDataclass
     dc1 = coerce_to_dataclass(DC1, dc2)
     cwd = str(Path(__file__).parent)
     with open(prog, 'w') as f:
         print(f"""#!/usr/bin/env python3
 import sys
 sys.path.insert(0, {cwd!r})
@@ -53,15 +53,15 @@
     """Tests retrieval of the executable name."""
     # executable in field
     @dataclass
     class DC3(SubprocessDataclass):
         prog: str = field(metadata={'exec': True})
     obj = DC3('myprog')
     assert obj.get_executable() == 'myprog'
-    assert obj.args() == ['myprog']
+    assert obj.get_args() == ['myprog']
     # non-string executable
     obj = DC3(1)
     with pytest.raises(ValueError, match=re.escape('executable is 1 (must be a string)')):
         _ = obj.get_executable()
     # executable in ClassVar field
     @dataclass
     class DC4(SubprocessDataclass):
@@ -79,15 +79,15 @@
     # no executable
     @dataclass
     class DC6(SubprocessDataclass):
         ...
     obj = DC6()
     assert obj.get_executable() is None
     with pytest.raises(ValueError, match='no executable identified for use with DC6 instance'):
-        _ = obj.args()
+        _ = obj.get_args()
     # multiple exec fields
     with pytest.raises(TypeError, match=re.escape("cannot have more than one field with 'exec' flag set to True (already set executable to prog1)")):
         @dataclass
         class DC7(SubprocessDataclass):
             prog1: ClassVar[str] = field(metadata={'exec': True})
             prog2: str = field(metadata={'exec': True})
     # exec in both class settings and field
@@ -99,15 +99,15 @@
     @dataclass
     class DC9(SubprocessDataclass):
         x: int
         yy: float
         prog: str = field(metadata={'exec': True})
     obj = DC9(3, 4.7, 'myprog')
     assert obj.get_executable() == 'myprog'
-    assert obj.args() == ['myprog', '-x', '3', '--yy', '4.7']
+    assert obj.get_args() == ['myprog', '-x', '3', '--yy', '4.7']
 
 def test_field_args():
     """Tests behavior of the 'args' metadata in a field."""
     @dataclass
     class DC10(SubprocessDataclass, exec='prog'):
         # if a non-empty list, use the first entry as the argument name (only if it starts with a dash)
         a: int = field(metadata={'args': ['-a']})
@@ -117,44 +117,44 @@
         d: int
         ee: int
         f: int = field(metadata={'args': None})
         # if an empty list, exclude this field from the arguments
         g: int = field(metadata={'args': []})
         # string is the same as singleton list
         h: int = field(metadata={'args': '--hh'})
-    assert DC10(1, 2, 3, 4, 5, 6, 7, 8).args() == ['prog', '-a', '1', '-b', '2', '--c', '3', '-d', '4', '--ee', '5', '-f', '6', '--hh', '8']
+    assert DC10(1, 2, 3, 4, 5, 6, 7, 8).get_args() == ['prog', '-a', '1', '-b', '2', '--c', '3', '-d', '4', '--ee', '5', '-f', '6', '--hh', '8']
     # args not starting with dash
     @dataclass
     class DC11(SubprocessDataclass, exec='prog'):
         a: int = field(metadata={'args': ['a']})
-    assert DC11(1).args() == ['prog', '1']
+    assert DC11(1).get_args() == ['prog', '1']
     @dataclass
     class DC12(SubprocessDataclass, exec='prog'):
         a: int = field(metadata={'args': ['a']})
         b: int = field(metadata={'args': ''})
         c: int = field(metadata={'args': ['c', '-c']})
-    assert DC12(1, 2, 3).args() == ['prog', '1', '2', '3']
+    assert DC12(1, 2, 3).get_args() == ['prog', '1', '2', '3']
     @dataclass
     class DC13(SubprocessDataclass, exec='prog'):
         a: int = field(metadata={'args': ['a']})
         b: int
-    assert DC13(1, 2).args() == ['prog', '1', '-b', '2']
+    assert DC13(1, 2).get_args() == ['prog', '1', '-b', '2']
     @dataclass
     class DC14(SubprocessDataclass, exec='prog'):
         a: int
         b: int = field(metadata={'args': ['b']})
-    assert DC14(1, 2).args() == ['prog', '-a', '1', '2']
+    assert DC14(1, 2).get_args() == ['prog', '-a', '1', '2']
 
 def test_flag():
     """Tests a boolean field being treated as an on/off flag."""
     @dataclass
     class DC15(SubprocessDataclass, exec='prog'):
         flag: bool
-    assert DC15(False).args() == ['prog']
-    assert DC15(True).args() == ['prog', '--flag']
+    assert DC15(False).get_args() == ['prog']
+    assert DC15(True).get_args() == ['prog', '--flag']
 
 def test_underscore_conversion():
     """Tests that underscores are converted to dashes for automatic argument naming."""
     @dataclass
     class DC16(SubprocessDataclass, exec='prog'):
         my_arg: int
-    assert DC16(1).args() == ['prog', '--my-arg', '1']
+    assert DC16(1).get_args() == ['prog', '--my-arg', '1']
```

### Comparing `fancy_dataclass-0.3.0/tests/test_utils.py` & `fancy_dataclass-0.3.1/tests/test_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 from dataclasses import dataclass, is_dataclass
+import sys
 from typing import Any, ClassVar, Dict, List, Optional, Sequence, Union
 
 import pytest
 from pytest import param
 
 from fancy_dataclass.utils import _flatten_dataclass, _is_instance, get_dataclass_fields, merge_dataclasses, traverse_dataclass, type_is_optional
 
 
 @pytest.mark.parametrize(['tp', 'is_optional'], [
     (int, False),
+    (type(None), False),
     (Optional[int], True),
     (Optional[Optional[int]], True),
-    (Union[int, Optional[float]], False),
-    (Union[Optional[float], int], False),
+    (Union[int, Optional[float]], True),
+    (Union[Optional[float], int], True),
     (Optional[type(None)], False),  # Optional[NoneType] -> NoneType
     (List[Optional[int]], False),
 ])
 def test_type_is_optional(tp, is_optional):
     assert type_is_optional(tp) == is_optional
 
+@pytest.mark.skipif(sys.version_info[:2] < (3, 10), reason='Py3.10 union type')
+def test_type_is_optional_py39():
+    assert type_is_optional(int | None)
+    assert type_is_optional(None | int)
+    assert type_is_optional(None | int | str)
+    assert type_is_optional(int | str | None)
+    assert type_is_optional(Optional[int | str])
+    assert type_is_optional(Optional[int] | str)
+
 @pytest.mark.parametrize(['obj', 'tp', 'output'], [
     (1, int, True),
     ('a', int, False),
     (None, int, False),
     (None, type(None), True),
     (1, type(None), False),
     (1, Any, True),
```

### Comparing `fancy_dataclass-0.3.0/pyproject.toml` & `fancy_dataclass-0.3.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fancy-dataclass"
 dynamic = ["version"]
-description = "Spiff up your dataclasses with additional features."
+description = "Spiff up your dataclasses with extra features."
 readme = "docs/README.md"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = ["dataclass", "cli", "config", "orm", "serialize", "json", "toml"]
 authors = [
   { name = "Jeremy Silver", email = "jeremys@nessiness.com" }
 ]
@@ -23,14 +23,15 @@
 ]
 
 [project.urls]
 # Documentation = "https://github.com/jeremander/fancy-dataclass#readme"
 Documentation = "https://fancy-dataclass.readthedocs.io"
 Issues = "https://github.com/jeremander/fancy-dataclass/issues"
 Source = "https://github.com/jeremander/fancy-dataclass"
+Changelog = "https://fancy-dataclass.readthedocs.io/en/stable/CHANGELOG"
 
 [tool.hatch.build.targets.sdist]
 exclude = ["TODO.txt"]
 
 [tool.hatch.version]
 path = "fancy_dataclass/__init__.py"
 
@@ -58,35 +59,45 @@
   "radon",
   "ruff>=0.3",
   "vermin",
 ]
 
 [tool.hatch.envs.lint.scripts]
 run-ruff = "ruff check"
-run-vermin = "vermin {args:-t=3.8- --eval-annotations --no-tips --violations --exclude 'tests.test_serializable.StrEnum' fancy_dataclass}"
+run-vermin = "vermin {args:-t=3.8- --eval-annotations --no-tips --violations --exclude enum.StrEnum --exclude types.UnionType .}"
 run-mypy = "mypy --install-types --non-interactive {args:fancy_dataclass tests}"
-run-loc-summary = "./summarize.sh"
+run-loc-summary = "./scripts/summarize.sh"
 all = ["run-ruff", "run-vermin", "run-mypy", "run-loc-summary"]
 
 [tool.hatch.envs.test]
 dependencies = [
     "numpy",
     "pytest",
     "pytest-cov",
 ]
 
 [tool.hatch.envs.test.scripts]
 test = "pytest {args:tests}"
 test-debug = "pytest --pdb {args:tests}"
-cov-report = ["- coverage combine", "coverage report"]
-cov = ["test-cov", "cov-report"]
+cov-report = ["- coverage combine", "coverage report", "coverage html"]
+cov = ["test", "cov-report"]
 
 [[tool.hatch.envs.test.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
+[tool.hatch.envs.badge]
+dependencies = [
+  "coverage",
+  "genbadge[tests,coverage]"
+]
+
+[tool.hatch.envs.badge.scripts]
+badge-cov = ["coverage xml", "genbadge coverage -i coverage.xml"]
+badges = ["badge-cov"]
+
 [tool.hatch.publish.index]
 disable = true
 
 [tool.coverage.run]
 source_pkgs = ["fancy_dataclass", "tests"]
 branch = true
 parallel = true
@@ -101,15 +112,15 @@
   "if TYPE_CHECKING:",
 ]
 
 [tool.commitizen]
 tag_format = "v$major.$minor.$patch"
 
 [tool.mypy]
-exclude = ["docs/", "site/", "tmp.*"]
+exclude = ["docs/", "scripts/", "site/", "tmp.*"]
 warn_unused_configs = true
 strict = true
 
 [[tool.mypy.overrides]]
 module = "tests.*"
 strict = false
 disable_error_code = ["arg-type", "attr-defined", "call-arg", "comparison-overlap", "no-redef", "no-untyped-call", "no-untyped-def", "type-arg"]
```

### Comparing `fancy_dataclass-0.3.0/docs/README.md` & `fancy_dataclass-0.3.1/docs/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,26 @@
+[![PyPI - Version](https://img.shields.io/pypi/v/fancy-dataclass)](https://pypi.org/project/fancy-dataclass/)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/jeremander/fancy-dataclass/workflow.yml)
+![Coverage Status](https://github.com/jeremander/fancy-dataclass/raw/coverage-badge/coverage-badge.svg)
+[![Read the Docs](https://img.shields.io/readthedocs/fancy-dataclass)](https://fancy-dataclass.readthedocs.io)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/jeremander/fancy-dataclass/raw/readme-badges/docs/LICENSE.txt)
+
 # Basics
 
 🤵🏻‍♂️ ***Fancy Dataclass***: A library to spiff up your dataclasses with extra features.
 
 ## Introduction
 
 Python 3.7 introduced the `dataclasses` module which lets you write "statically typed" classes using the type hinting mechanism.
 
 By inspecting dataclasses' type annotations, it is possible to endow them with special powers that help cut down on boilerplate code in a wide variety of domains, such as:
 
 - *JSON/TOML conversion*: convert dataclasses to JSON/TOML files and vice versa
 - *Configuration management*: store global configurations and use them anywhere in your program
-- *SQL persistence*: define a SQL table, and save/load objects from a database
+- *SQL persistence*: define SQL tables, and save/load objects from a database
 - *CLI parsing*: parse command-line arguments and store their values in a dataclass, then use them to execute your main program logic
 - *Subprocess calls*: generate command-line arguments to be passed to another program
 
 `fancy_dataclass` borrows ideas from other excellent libraries such as [`marshmallow`](https://marshmallow.readthedocs.io/en/stable/), [`pydantic`](https://docs.pydantic.dev/latest), and [`argparse_dataclass`](https://github.com/mivade/argparse_dataclass), but it aims to be as lightweight as possible in terms of its dependencies and learning curve.
 
 ## How to install
 
@@ -70,14 +76,14 @@
 }
 ```
 
 ## Documentation
 
 Read the official documentation [here](https://fancy-dataclass.readthedocs.io).
 
-The documentation is made with [Material for MkDocs](https://squidfunk.github.io/mkdocs-material) and is hosted by [Read the Docs](https://readthedocs.org).
+The documentation is made with [Material for MkDocs](https://squidfunk.github.io/mkdocs-material) and is hosted by [Read the Docs](https://readthedocs.com).
 
 View the Changelog [here](CHANGELOG.md).
 
 ## License
 
 This library is distributed under the terms of the [MIT](LICENSE.txt) license.
```

### Comparing `fancy_dataclass-0.3.0/PKG-INFO` & `fancy_dataclass-0.3.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 Metadata-Version: 2.3
 Name: fancy-dataclass
-Version: 0.3.0
-Summary: Spiff up your dataclasses with additional features.
+Version: 0.3.1
+Summary: Spiff up your dataclasses with extra features.
 Project-URL: Documentation, https://fancy-dataclass.readthedocs.io
 Project-URL: Issues, https://github.com/jeremander/fancy-dataclass/issues
 Project-URL: Source, https://github.com/jeremander/fancy-dataclass
+Project-URL: Changelog, https://fancy-dataclass.readthedocs.io/en/stable/CHANGELOG
 Author-email: Jeremy Silver <jeremys@nessiness.com>
 License-Expression: MIT
 Keywords: cli,config,dataclass,json,orm,serialize,toml
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Requires-Dist: sqlalchemy>=2.0
 Requires-Dist: tomlkit>=0.11
 Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
+[![PyPI - Version](https://img.shields.io/pypi/v/fancy-dataclass)](https://pypi.org/project/fancy-dataclass/)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/jeremander/fancy-dataclass/workflow.yml)
+![Coverage Status](https://github.com/jeremander/fancy-dataclass/raw/coverage-badge/coverage-badge.svg)
+[![Read the Docs](https://img.shields.io/readthedocs/fancy-dataclass)](https://fancy-dataclass.readthedocs.io)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/jeremander/fancy-dataclass/raw/readme-badges/docs/LICENSE.txt)
+
 # Basics
 
 🤵🏻‍♂️ ***Fancy Dataclass***: A library to spiff up your dataclasses with extra features.
 
 ## Introduction
 
 Python 3.7 introduced the `dataclasses` module which lets you write "statically typed" classes using the type hinting mechanism.
 
 By inspecting dataclasses' type annotations, it is possible to endow them with special powers that help cut down on boilerplate code in a wide variety of domains, such as:
 
 - *JSON/TOML conversion*: convert dataclasses to JSON/TOML files and vice versa
 - *Configuration management*: store global configurations and use them anywhere in your program
-- *SQL persistence*: define a SQL table, and save/load objects from a database
+- *SQL persistence*: define SQL tables, and save/load objects from a database
 - *CLI parsing*: parse command-line arguments and store their values in a dataclass, then use them to execute your main program logic
 - *Subprocess calls*: generate command-line arguments to be passed to another program
 
 `fancy_dataclass` borrows ideas from other excellent libraries such as [`marshmallow`](https://marshmallow.readthedocs.io/en/stable/), [`pydantic`](https://docs.pydantic.dev/latest), and [`argparse_dataclass`](https://github.com/mivade/argparse_dataclass), but it aims to be as lightweight as possible in terms of its dependencies and learning curve.
 
 ## How to install
 
@@ -87,14 +94,14 @@
 }
 ```
 
 ## Documentation
 
 Read the official documentation [here](https://fancy-dataclass.readthedocs.io).
 
-The documentation is made with [Material for MkDocs](https://squidfunk.github.io/mkdocs-material) and is hosted by [Read the Docs](https://readthedocs.org).
+The documentation is made with [Material for MkDocs](https://squidfunk.github.io/mkdocs-material) and is hosted by [Read the Docs](https://readthedocs.com).
 
 View the Changelog [here](CHANGELOG.md).
 
 ## License
 
 This library is distributed under the terms of the [MIT](LICENSE.txt) license.
```

