# Comparing `tmp/bkpaas-auth-2.0.8.tar.gz` & `tmp/bkpaas-auth-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bkpaas-auth-2.0.8.tar", max compression
+gzip compressed data, was "bkpaas-auth-2.1.0.tar", max compression
```

## Comparing `bkpaas-auth-2.0.8.tar` & `bkpaas-auth-2.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     5197 2023-12-26 07:36:42.513179 bkpaas-auth-2.0.8/README.md
--rw-r--r--   0        0        0     1012 2023-12-26 07:36:42.513790 bkpaas-auth-2.0.8/bkpaas_auth/__init__.py
--rw-r--r--   0        0        0      191 2023-12-26 07:36:42.514023 bkpaas-auth-2.0.8/bkpaas_auth/apps.py
--rw-r--r--   0        0        0     8077 2023-12-26 07:36:42.514379 bkpaas-auth-2.0.8/bkpaas_auth/backends.py
--rw-r--r--   0        0        0     2526 2023-12-26 07:36:42.514613 bkpaas-auth-2.0.8/bkpaas_auth/conf.py
--rw-r--r--   0        0        0        0 2023-12-26 07:36:42.514868 bkpaas-auth-2.0.8/bkpaas_auth/core/__init__.py
--rw-r--r--   0        0        0      346 2023-12-26 07:36:42.515091 bkpaas-auth-2.0.8/bkpaas_auth/core/constants.py
--rw-r--r--   0        0        0     2302 2023-12-26 07:36:42.515413 bkpaas-auth-2.0.8/bkpaas_auth/core/encoder.py
--rw-r--r--   0        0        0      437 2023-12-26 07:36:42.515629 bkpaas-auth-2.0.8/bkpaas_auth/core/exceptions.py
--rw-r--r--   0        0        0     2641 2023-12-26 07:36:42.515858 bkpaas-auth-2.0.8/bkpaas_auth/core/http.py
--rw-r--r--   0        0        0     1173 2023-12-26 07:36:42.516059 bkpaas-auth-2.0.8/bkpaas_auth/core/plugins.py
--rw-r--r--   0        0        0     3313 2023-12-26 07:36:42.516495 bkpaas-auth-2.0.8/bkpaas_auth/core/services.py
--rw-r--r--   0        0        0     4475 2023-12-26 07:36:42.516736 bkpaas-auth-2.0.8/bkpaas_auth/core/token.py
--rw-r--r--   0        0        0     2493 2023-12-26 07:36:42.516996 bkpaas-auth-2.0.8/bkpaas_auth/core/user_info.py
--rw-r--r--   0        0        0      641 2023-12-26 07:36:42.517181 bkpaas-auth-2.0.8/bkpaas_auth/core/utils.py
--rw-r--r--   0        0        0     4041 2023-12-26 07:36:42.517368 bkpaas-auth-2.0.8/bkpaas_auth/middlewares.py
--rw-r--r--   0        0        0     3368 2023-12-26 07:36:42.517554 bkpaas-auth-2.0.8/bkpaas_auth/models.py
--rw-r--r--   0        0        0     1264 2023-12-26 07:36:42.517736 bkpaas-auth-2.0.8/bkpaas_auth/monkey.py
--rw-r--r--   0        0        0     1332 2023-12-26 07:36:42.517916 bkpaas-auth-2.0.8/bkpaas_auth/utils.py
--rw-r--r--   0        0        0     1512 2023-12-26 07:36:42.520773 bkpaas-auth-2.0.8/pyproject.toml
--rw-r--r--   0        0        0     6058 2023-12-26 07:37:25.651177 bkpaas-auth-2.0.8/setup.py
--rw-r--r--   0        0        0     5915 2023-12-26 07:37:25.651794 bkpaas-auth-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     5197 2023-12-28 08:29:17.369660 bkpaas-auth-2.1.0/README.md
+-rw-r--r--   0        0        0     1012 2024-04-17 06:21:20.363837 bkpaas-auth-2.1.0/bkpaas_auth/__init__.py
+-rw-r--r--   0        0        0      191 2023-12-28 08:29:17.370945 bkpaas-auth-2.1.0/bkpaas_auth/apps.py
+-rw-r--r--   0        0        0     9361 2024-04-17 06:16:16.638706 bkpaas-auth-2.1.0/bkpaas_auth/backends.py
+-rw-r--r--   0        0        0     2526 2023-12-28 08:29:17.373075 bkpaas-auth-2.1.0/bkpaas_auth/conf.py
+-rw-r--r--   0        0        0        0 2023-12-28 08:29:17.373436 bkpaas-auth-2.1.0/bkpaas_auth/core/__init__.py
+-rw-r--r--   0        0        0      346 2023-12-28 08:29:17.374050 bkpaas-auth-2.1.0/bkpaas_auth/core/constants.py
+-rw-r--r--   0        0        0     2302 2023-12-28 08:29:17.374585 bkpaas-auth-2.1.0/bkpaas_auth/core/encoder.py
+-rw-r--r--   0        0        0      437 2023-12-28 08:29:17.375110 bkpaas-auth-2.1.0/bkpaas_auth/core/exceptions.py
+-rw-r--r--   0        0        0     2641 2024-04-17 06:15:56.166105 bkpaas-auth-2.1.0/bkpaas_auth/core/http.py
+-rw-r--r--   0        0        0     1173 2023-12-28 08:29:17.377097 bkpaas-auth-2.1.0/bkpaas_auth/core/plugins.py
+-rw-r--r--   0        0        0     3313 2024-04-17 06:15:56.166512 bkpaas-auth-2.1.0/bkpaas_auth/core/services.py
+-rw-r--r--   0        0        0     4475 2024-04-17 06:15:56.167838 bkpaas-auth-2.1.0/bkpaas_auth/core/token.py
+-rw-r--r--   0        0        0     2493 2023-12-28 08:29:17.378419 bkpaas-auth-2.1.0/bkpaas_auth/core/user_info.py
+-rw-r--r--   0        0        0      641 2023-12-28 08:29:17.378850 bkpaas-auth-2.1.0/bkpaas_auth/core/utils.py
+-rw-r--r--   0        0        0     4041 2023-12-28 08:29:17.379247 bkpaas-auth-2.1.0/bkpaas_auth/middlewares.py
+-rw-r--r--   0        0        0     3368 2023-12-28 08:29:17.379609 bkpaas-auth-2.1.0/bkpaas_auth/models.py
+-rw-r--r--   0        0        0     1264 2024-04-17 06:15:56.168234 bkpaas-auth-2.1.0/bkpaas_auth/monkey.py
+-rw-r--r--   0        0        0     1332 2024-04-17 06:15:56.168461 bkpaas-auth-2.1.0/bkpaas_auth/utils.py
+-rw-r--r--   0        0        0     1512 2024-04-17 06:16:16.639147 bkpaas-auth-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6058 2024-04-17 06:22:19.275051 bkpaas-auth-2.1.0/setup.py
+-rw-r--r--   0        0        0     5864 2024-04-17 06:22:19.275586 bkpaas-auth-2.1.0/PKG-INFO
```

### Comparing `bkpaas-auth-2.0.8/README.md` & `bkpaas-auth-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.8/bkpaas_auth/__init__.py` & `bkpaas-auth-2.1.0/bkpaas_auth/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "2.0.6"
+__version__ = "2.1.0"
 
 
 def get_user_by_user_id(user_id: str, username_only: bool = True):
     """Get a user object from given user_id"""
     from bkpaas_auth.core.constants import ProviderType
     from bkpaas_auth.core.encoder import user_id_encoder
     from bkpaas_auth.core.services import get_bk_user_info, get_rtx_user_info
```

### Comparing `bkpaas-auth-2.0.8/bkpaas_auth/backends.py` & `bkpaas-auth-2.1.0/bkpaas_auth/backends.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # -*- coding: utf-8 -*-
+import inspect
 import logging
 import pickle
 from typing import Dict, Optional, Union
 
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import AnonymousUser
@@ -35,68 +36,69 @@
     found in the middleware module of this package.
     """
 
     request: HttpRequest
 
     def __init__(self):
         self.backend_type = bkauth_settings.BACKEND_TYPE
-        if self.backend_type == 'bk_ticket':
+        if self.backend_type == "bk_ticket":
             self.plugin = BkTicketPlugin()
             self.request_backend = RequestBackend()
-        elif self.backend_type == 'bk_token':
+        elif self.backend_type == "bk_token":
             self.plugin = BkTokenPlugin()
             self.request_backend = TokenRequestBackend()
         else:
             raise ImproperlyConfigured("BKAUTH_BACKEND_TYPE not set")
 
     def authenticate(self, request: HttpRequest, auth_credentials: Dict) -> Optional[Union[User, AnonymousUser]]:
         try:
             username = self.request_backend.request_username(**auth_credentials)
             login_token = generate_random_token()
             token = LoginToken(
                 login_token=login_token,
                 expires_in=bkauth_settings.LOGIN_TOKEN_EXPIRE_IN,
             )
             token.user_info = UserInfo(username=username)
-            logger.debug('New login token exchanged by credentials')
+            logger.debug("New login token exchanged by credentials")
         except InvalidTokenCredentialsError:
-            logger.warning('authenticate error, invalid credentials given')
+            logger.warning("authenticate error, invalid credentials given")
             return None
         except ServiceError:
-            logger.warning('authenticate error, Error requesting third-party API service')
+            logger.warning("authenticate error, Error requesting third-party API service")
             return None
 
         return self.get_user_by_token(token)
 
     def get_user(self, user_id):
         """Get user from current session"""
-        if not hasattr(self, 'request'):
-            return
+        if not hasattr(self, "request"):
+            return None
 
         # Try to get login_token from session
         token = self.get_token_from_session(self.request)
         if token:
             # Q: 为什么不调用 get_user_by_token?
             # A: 由于 get_user_by_token 需要访问远程服务, 但事实上在 authenticate 时, 用户信息已经被缓存到 token 对象中.
             #    为了减少网络开销, 所以直接调用 create_user_from_token.
             return create_user_from_token(token)
+        return None
 
     def get_credentials(self, *args, **kwargs):
         return self.plugin.get_credentials(*args, **kwargs)
 
     def get_token_from_session(self, request: HttpRequest) -> Optional[LoginToken]:
         """Try getting token object from session"""
         if "user_token" not in request.session:
             return None
 
         try:
-            user_token_pickled = force_bytes(request.session['user_token'], 'latin1')
+            user_token_pickled = force_bytes(request.session["user_token"], "latin1")
             user_token: LoginToken = pickle.loads(user_token_pickled)
-        except Exception as error:
-            logger.exception("pickle loads user_token failed, %s", error)
+        except Exception:
+            logger.exception("pickle loads user_token failed")
             return None
 
         # token 已经过期则不返回，否则会出现 403
         if self.plugin.validate_login_token(user_token):
             return user_token
         return None
 
@@ -138,15 +140,15 @@
         user = super().get_user(user_id)
         if user:
             user = self.connect_to_django_user(user)
         return user
 
     def connect_to_django_user(self, user: User):
         """Connect bkpaas_auth.User to the UserModel in the database."""
-        UserModel = get_user_model()
+        UserModel = get_user_model()  # noqa: N806
         if self.create_unknown_user:
             db_user, created = UserModel._default_manager.get_or_create(**{UserModel.USERNAME_FIELD: user.username})
             if created:
                 logger.info("User named %s is created!", user.username)
                 db_user = self.configure_user(db_user=db_user, bk_user=user)
         else:
             try:
@@ -162,47 +164,74 @@
             db_user.token = user.token
         return db_user
 
     def configure_user(self, db_user, bk_user: User):
         """
         Configure a user after creation and return the updated user.
         """
-        default_admin_superusers = getattr(settings, 'DEFAULT_ADMIN_SUPERUSERS', [])
+        default_admin_superusers = getattr(settings, "DEFAULT_ADMIN_SUPERUSERS", [])
         if db_user.username in default_admin_superusers:
             db_user.is_active = True
             db_user.is_staff = True
             db_user.is_superuser = True
 
         db_user.email = bk_user.email or ""
         db_user.save(update_fields=["is_active", "is_staff", "is_superuser", "email"])
         return db_user
 
 
 class APIGatewayAuthBackend:
     """This backend is to be used in conjunction with the ``ApiGatewayJWTUserMiddleware``
     found in the middleware module of ``apigw_manager`` package.
+
     """
 
-    def authenticate(self, request, api_name, bk_username, verified, **credential):
+    def authenticate_with_signature_v3(self, request, gateway_name, bk_username, verified, **credentials):
+        """authenticate function with signature required by ApiGatewayJWTUserMiddleware in apigw_manager == '^3.0.0'"""
+        if not verified:
+            return self.make_anonymous_user(bk_username)
+
+        return User(
+            token=LoginToken("any_token", expires_in=86400),
+            provider_type=self.get_provider_type(),
+            username=bk_username,
+        )
+
+    def authenticate_with_signature_v1(self, request, api_name, bk_username, verified, **credentials):
+        """authenticate function with signature required by ApiGatewayJWTUserMiddleware in apigw_manager == '^1.0.0'"""
         if not verified:
             return self.make_anonymous_user(bk_username)
 
         return User(
-            token=LoginToken('any_token', expires_in=86400),
+            token=LoginToken("any_token", expires_in=86400),
             provider_type=self.get_provider_type(),
             username=bk_username,
         )
 
+    try:
+        from apigw_manager.apigw.authentication import ApiGatewayJWTUserMiddleware
+
+        get_user_parameters = sorted(inspect.signature(ApiGatewayJWTUserMiddleware.get_user).parameters.keys())
+        v3_parameters = sorted(inspect.signature(authenticate_with_signature_v3).parameters.keys())
+        if get_user_parameters == v3_parameters:
+            authenticate = authenticate_with_signature_v3
+        else:
+            authenticate = authenticate_with_signature_v1
+        del get_user_parameters
+        del v3_parameters
+    except ImportError:
+        authenticate = authenticate_with_signature_v1
+
     def get_user(self, user_id):
         raise NotImplementedError(
             "ApiGatewayJWTUserMiddleware should be overwrite request.user, "
             "so that APIGatewayAuthBackend.get_user will never be called."
         )
 
     def get_provider_type(self):
-        name = getattr(settings, 'BKAUTH_DEFAULT_PROVIDER_TYPE', "RTX")
+        name = getattr(settings, "BKAUTH_DEFAULT_PROVIDER_TYPE", "RTX")
         return getattr(ProviderType, name)
 
     def make_anonymous_user(self, bk_username=None):
         user = AnonymousUser()
         user.username = bk_username
         return user
```

### Comparing `bkpaas-auth-2.0.8/bkpaas_auth/conf.py` & `bkpaas-auth-2.1.0/bkpaas_auth/conf.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.8/bkpaas_auth/core/encoder.py` & `bkpaas-auth-2.1.0/bkpaas_auth/core/encoder.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.8/bkpaas_auth/core/http.py` & `bkpaas-auth-2.1.0/bkpaas_auth/core/http.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.8/bkpaas_auth/core/plugins.py` & `bkpaas-auth-2.1.0/bkpaas_auth/core/plugins.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.8/bkpaas_auth/core/services.py` & `bkpaas-auth-2.1.0/bkpaas_auth/core/services.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.8/bkpaas_auth/core/token.py` & `bkpaas-auth-2.1.0/bkpaas_auth/core/token.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.8/bkpaas_auth/core/user_info.py` & `bkpaas-auth-2.1.0/bkpaas_auth/core/user_info.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.8/bkpaas_auth/core/utils.py` & `bkpaas-auth-2.1.0/bkpaas_auth/core/utils.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.8/bkpaas_auth/middlewares.py` & `bkpaas-auth-2.1.0/bkpaas_auth/middlewares.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.8/bkpaas_auth/models.py` & `bkpaas-auth-2.1.0/bkpaas_auth/models.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.8/bkpaas_auth/monkey.py` & `bkpaas-auth-2.1.0/bkpaas_auth/monkey.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.8/bkpaas_auth/utils.py` & `bkpaas-auth-2.1.0/bkpaas_auth/utils.py`

 * *Files identical despite different names*

### Comparing `bkpaas-auth-2.0.8/pyproject.toml` & `bkpaas-auth-2.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bkpaas-auth"
-version = "2.0.8"
+version = "2.1.0"
 description = "User authentication django app for blueking internal projects"
 readme = "README.md"
 authors = ["blueking <blueking@tencent.com>"]
 license = "MIT"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `bkpaas-auth-2.0.8/setup.py` & `bkpaas-auth-2.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['cryptography', 'django>=1.11,<4.0', 'requests', 'six']
 
 setup_kwargs = {
     'name': 'bkpaas-auth',
-    'version': '2.0.8',
+    'version': '2.1.0',
     'description': 'User authentication django app for blueking internal projects',
     'long_description': '# bkpaas-auth\n\n蓝鲸 PaaS 平台内部服务使用的用户鉴权模块。\n\n## 版本历史\n\n详见 `CHANGES.md`。\n\n## 开发指南\n\n### 发布包\n\n- 在 `bkpaas_auth/__init__.py`  文件中更新 `__version__`\n- 在 `setup.py` 文件中更新 `version`\n- 在 `pyproject.toml` 中更新 `version`\n- 在 `CHANGES.md` 中添加对应的版本日志\n- 执行 `poetry build` 命令在 dist 目录下生成当前版本的包。然后执行 `twine upload dist/* --repository-url {pypi_address} --username {your_name} --password {your_token}` 将其上传到 pypi 服务器上。\n\n### 关于 setup.py\n\n虽然在 [PEP 517](https://python-poetry.org/docs/pyproject/#poetry-and-pep-517) 规范里，Python 包不再需要 `setup.py` 文件。但真正少了 `setup.py` 文件后，会发现有些功能就没法正常使用，比如 pip 的可编辑安装模式、tox 等（[相关文档](https://github.com/python-poetry/poetry/issues/761)）。所以我们仍然需要它。\n\n为了避免维护重复的 `pyproject.toml` 和 `setup.py` 文件，我们使用了 [dephell](https://github.com/dephell/dephell) 工具来自动生成 `setup.py` 文件。\n\n- 安装 dephell\n- 在根目录执行 `dephell deps convert --from pyproject.toml --to setup.py`\n\n## 使用指南\n1. 更新 settings：\n```python\nINSTALLED_APPS = [\n    ...\n    \'bkpaas_auth\',\n    ...\n]\n\nMIDDLEWARE = [\n    ...\n    \'bkpaas_auth.middlewares.CookieLoginMiddleware\',\n    ...\n]\n\nAUTHENTICATION_BACKENDS = [\n    # [推荐] 使用内置的虚拟用户类型，不依赖于数据库表.\n    \'bkpaas_auth.backends.UniversalAuthBackend\',\n    # 如果项目需要保留使用数据库表的方式来设计用户模型, 则需要使用 DjangoAuthUserCompatibleBackend\n    # \'bkpaas_auth.backends.DjangoAuthUserCompatibleBackend\',\n]\n\n# 使用 bkpaas_auth 内置的基于内存的用户模型\n# 如果项目需要保留使用数据库表的方式来设计用户模型, 可阅读 「关于AUTH_USER_MODEL」的部分说明\nAUTH_USER_MODEL = \'bkpaas_auth.User\'\n\n# 用户登录态认证类型\nBKAUTH_BACKEND_TYPE = "bk_token" # 可选值：bk_token/bk_ticket\n# 验证用户登录态的 API，如 蓝鲸统一登录校验登录态的 API\nBKAUTH_USER_COOKIE_VERIFY_URL = "http://bk-login-web/api/v3/is_login/"\n\n# [可选]`BKAUTH_DEFAULT_PROVIDER_TYPE` 的值用于 JWT 校验时获取默认的用户认证类型。\nBKAUTH_DEFAULT_PROVIDER_TYPE = \'RTX\'  # 可选值：RTX/UIN/BK，详见 ProviderType\n```\n\n2. 在 app config 中进行 patch：\n\n配置登录模块的 apps.py\n\n```python\nfrom bkpaas_auth.backends import DjangoAuthUserCompatibleBackend\nfrom bkpaas_auth.models import User\nfrom django.apps import AppConfig\n\n\nclass MyAppConfig(AppConfig):\n    name = \'my_app\'\n\n    def ready(self):\n        from bkpaas_auth.monkey import patch_middleware_get_user\n\n        patch_middleware_get_user()\n```\n\n更新 `__init__.py`，配置 default_app_config\n```\ndefault_app_config = \'xxx.apps.MyAppConfig\'\n```\n\n3. 配置日志（可选）\n在 django settings 的 LOGGING 中，为 sdk 配置 logger，如\n\n```python\nLOGGING = {\n    "handlers": {\n        "root": {\n            ...\n        },\n    },\n    "loggers": {\n        "bkpaas_auth": {\n            "handlers": ["root"],\n            "level": "WARNING",\n            "propagate": True,\n        },\n    },\n}\n```\n\n### 关于 AUTH_USER_MODEL\n\nbkpaas-auth 内置的基于内存的不依赖于数据库表的用户模型, 如果需要复用原有的用户模型, 则需要使用 `DjangoAuthUserCompatibleBackend` 作为用户校验后端.\n\n在默认情况下, `DjangoAuthUserCompatibleBackend` 会从 bkpaas-auth 获取到当前登录的用户信息, 并会根据用户信息尝试创建一个基于数据库的用户模型.\n如果你有以下诉求, 则应当继承 `DjangoAuthUserCompatibleBackend`, 自行实现具体的业务逻辑:\n\n1. 不希望自动创建基于数据库的用户模型:\n```python\n\n\nclass YourDjangoAuthUserCompatibleBackend(DjangoAuthUserCompatibleBackend):\n    create_unknown_user = False\n```\n\n2. 用户模型有与 django `auth.User` 不兼容的字段或其他需要初始化的字段:\n```python\n\nclass YourDjangoAuthUserCompatibleBackend(DjangoAuthUserCompatibleBackend):\n    def configure_user(self, db_user, bk_user: User):\n        """\n        Configure a user after creation and return the updated user.\n        """\n        ...\n        return db_user\n```\n\n#### 和 [apigw-manager](../apigw-manager) 集成\n该 SDK 可以和 apigw-manager 集成，完成网关 JWT 的校验，在 settings 中配置：\n```python\nINSTALLED_APPS += ["apigw_manager.apigw"]\nAUTHENTICATION_BACKENDS += ["bkpaas_auth.backends.APIGatewayAuthBackend"]\nMIDDLEWARE += [\n    "apigw_manager.apigw.authentication.ApiGatewayJWTGenericMiddleware",  # JWT 认证\n    "apigw_manager.apigw.authentication.ApiGatewayJWTAppMiddleware",  # JWT 透传的应用信息\n    "apigw_manager.apigw.authentication.ApiGatewayJWTUserMiddleware",  # JWT 透传的用户信息\n]\n```\n\n设置之后，通过 JWT 透传的用户态会验证后，会写入到 `request.user` 中。注意，配置了不认证用户的网关资源透传的请求，会生成一个有对应用户名的匿名用户对象（`is_authenticated` 为 `False`）。\n',
     'author': 'blueking',
     'author_email': 'blueking@tencent.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `bkpaas-auth-2.0.8/PKG-INFO` & `bkpaas-auth-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: bkpaas-auth
-Version: 2.0.8
+Version: 2.1.0
 Summary: User authentication django app for blueking internal projects
 License: MIT
 Author: blueking
 Author-email: blueking@tencent.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: cryptography
 Requires-Dist: django (>=1.11,<4.0)
 Requires-Dist: requests
```

