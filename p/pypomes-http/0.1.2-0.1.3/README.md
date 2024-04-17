# Comparing `tmp/pypomes_http-0.1.2.tar.gz` & `tmp/pypomes_http-0.1.3.tar.gz`

## Comparing `pypomes_http-0.1.2.tar` & `pypomes_http-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 pypomes_http-0.1.2/src/pypomes_http/__init__.py
--rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 pypomes_http-0.1.2/src/pypomes_http/http_async.py
--rw-r--r--   0        0        0    13799 2020-02-02 00:00:00.000000 pypomes_http-0.1.2/src/pypomes_http/http_pomes.py
--rw-r--r--   0        0        0    22949 2020-02-02 00:00:00.000000 pypomes_http-0.1.2/src/pypomes_http/http_statuses.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_http-0.1.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_http-0.1.2/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_http-0.1.2/README.md
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 pypomes_http-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pypomes_http-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pypomes_http-0.1.3/src/pypomes_http/__init__.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 pypomes_http-0.1.3/src/pypomes_http/http_async.py
+-rw-r--r--   0        0        0    15965 2020-02-02 00:00:00.000000 pypomes_http-0.1.3/src/pypomes_http/http_pomes.py
+-rw-r--r--   0        0        0    22977 2020-02-02 00:00:00.000000 pypomes_http-0.1.3/src/pypomes_http/http_statuses.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_http-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_http-0.1.3/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_http-0.1.3/README.md
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 pypomes_http-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pypomes_http-0.1.3/PKG-INFO
```

### Comparing `pypomes_http-0.1.2/src/pypomes_http/__init__.py` & `pypomes_http-0.1.3/src/pypomes_http/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from .http_async import (
     HttpAsync,
 )
 from .http_pomes import (
-    HTTP_DELETE_TIMEOUT, HTTP_GET_TIMEOUT, HTTP_POST_TIMEOUT, HTTP_PUT_TIMEOUT,
+    HTTP_DELETE_TIMEOUT, HTTP_GET_TIMEOUT, HTTP_PATCH_TIMEOUT, HTTP_POST_TIMEOUT, HTTP_PUT_TIMEOUT,
     MIMETYPE_BINARY, MIMETYPE_CSS, MIMETYPE_CSV, MIMETYPE_HTML, MIMETYPE_JAVASCRIPT,
     MIMETYPE_JSON, MIMETYPE_MULTIPART, MIMETYPE_PDF, MIMETYPE_PKCS7, MIMETYPE_SOAP,
     MIMETYPE_TEXT, MIMETYPE_URLENCODED, MIMETYPE_XML, MIMETYPE_ZIP,
     http_status_code, http_status_name, http_status_description,
-    http_delete, http_get, http_post, http_put,
     http_get_parameter, http_get_parameters,
+    http_delete, http_get, http_patch, http_post, http_put,
 )
 
 __all__ = [
     # http_async
     "HttpAsync",
     # http_pomes
-    "HTTP_DELETE_TIMEOUT", "HTTP_GET_TIMEOUT", "HTTP_POST_TIMEOUT", "HTTP_PUT_TIMEOUT",
+    "HTTP_DELETE_TIMEOUT", "HTTP_GET_TIMEOUT", "HTTP_PATCH_TIMEOUT", "HTTP_POST_TIMEOUT", "HTTP_PUT_TIMEOUT",
     "MIMETYPE_BINARY", "MIMETYPE_CSS", "MIMETYPE_CSV", "MIMETYPE_HTML", "MIMETYPE_JAVASCRIPT",
     "MIMETYPE_JSON", "MIMETYPE_MULTIPART", "MIMETYPE_PDF", "MIMETYPE_PKCS7", "MIMETYPE_SOAP",
     "MIMETYPE_TEXT", "MIMETYPE_URLENCODED", "MIMETYPE_XML", "MIMETYPE_ZIP",
     "http_status_code", "http_status_name", "http_status_description",
-    "http_delete", "http_get", "http_post", "http_put",
     "http_get_parameter", "http_get_parameters",
+    "http_delete", "http_get", "http_patch", "http_post", "http_put",
 ]
 
 from importlib.metadata import version
 __version__ = version("pypomes_http")
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
```

### Comparing `pypomes_http-0.1.2/src/pypomes_http/http_async.py` & `pypomes_http-0.1.3/src/pypomes_http/http_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,26 @@
 class HttpAsync(threading.Thread):
     """
     Asynchronous invocation of a *REST* service.
 
     This invocation is done with *request* and the method specified in *job_method*.
     """
 
-    def __init__(self, job_name: str, job_url: str,
-                 job_method: Literal["GET", "POST", "PUT"],
-                 callback: callable = None, report_content: bool = False,
-                 headers: dict = None, params: dict = None, data: dict = None, json: dict = None,
-                 auth: str = None, timeout: int = None, logger: Logger = None) -> None:
+    def __init__(self, job_name:
+                 str, job_url: str,
+                 job_method: Literal["DELETE", "GET", "PATCH", "POST", "PUT"],
+                 callback: callable = None,
+                 report_content: bool = False,
+                 headers: dict = None,
+                 params: dict = None,
+                 data: dict = None,
+                 json: dict = None,
+                 auth: str = None,
+                 timeout: int = None,
+                 logger: Logger = None) -> None:
         """
         Initiate the asychronous invocation of the *REST* service.
 
         if a *callback* is specified, it will be sent the results of the job invocaton, in *JSON* format.
         This is the structure of the results sent:
 
         {
@@ -106,15 +113,15 @@
 
         # has a callback been specified ?
         if self.callback:
             # yes, send it the results of the service invocation
             reply: dict = {
                 "job_name": self.job_name,
                 "start": self.start_timestamp,
-                "finish": self.finish_timestamp
+                "finish": self.finish_timestamp,
             }
 
             # any errors ?
             if len(errors) > 0:
                 # yes, report the errors messages
                 reply["errors"] = json.dumps(errors, ensure_ascii=False)
             elif self.report_content and \
```

### Comparing `pypomes_http-0.1.2/src/pypomes_http/http_pomes.py` & `pypomes_http-0.1.3/src/pypomes_http/http_pomes.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from requests import Response
 from typing import Any, Final
 
 from .http_statuses import _HTTP_STATUSES
 
 HTTP_DELETE_TIMEOUT: Final[int] = env_get_int(f"{APP_PREFIX}_HTTP_DELETE_TIMEOUT", 300)
 HTTP_GET_TIMEOUT: Final[int] = env_get_int(f"{APP_PREFIX}_HTTP_GET_TIMEOUT", 300)
+HTTP_PATCH_TIMEOUT: Final[int] = env_get_int(f"{APP_PREFIX}_HTTP_POST_TIMEOUT", 300)
 HTTP_POST_TIMEOUT: Final[int] = env_get_int(f"{APP_PREFIX}_HTTP_POST_TIMEOUT", 300)
 HTTP_PUT_TIMEOUT: Final[int] = env_get_int(f"{APP_PREFIX}_HTTP_PUT_TIMEOUT", 300)
 
 MIMETYPE_BINARY: Final[str] = "application/octet-stream"
 MIMETYPE_CSS: Final[str] = "text/css"
 MIMETYPE_CSV: Final[str] = "text/csv"
 MIMETYPE_HTML: Final[str] = "text/html"
@@ -31,15 +32,15 @@
 MIMETYPE_ZIP: Final[str] = "application/zip"
 
 
 def http_status_code(status_name: str) -> int:
     """
     Return the corresponding code of the HTTP status *status_name*.
 
-    :param status_name: the name of HTTP the status
+    :param status_name: the name of HTTP status
     :return: the corresponding HTTP status code
     """
     # initialize the return variable
     result: int | None = None
 
     for key, value in _HTTP_STATUSES:
         if status_name == value["name"]:
@@ -55,27 +56,29 @@
     :param status_code: the code of the HTTP status
     :return: the corresponding HTTP status name
     """
     item: dict = _HTTP_STATUSES.get(status_code)
     return (item or {"name": "Unknown status code"}).get("name")
 
 
-def http_status_description(status_code: int, lang: str = "en") -> str:
+def http_status_description(status_code: int,
+                            lang: str = "en") -> str:
     """
     Return the description of the HTTP status *status_code*.
 
     :param status_code: the code of the HTTP status
     :param lang: optional language ('en' or 'pt' - defaults to 'en')
     :return: the corresponding HTTP status description, in the given language
     """
     item: dict = _HTTP_STATUSES.get(status_code)
     return (item or {"en": "Unknown status code", "pt": "Status desconhecido"}).get(lang)
 
 
-def http_get_parameter(request: Request, param: str) -> Any:
+def http_get_parameter(request: Request,
+                       param: str) -> Any:
     """
     Obtain the *request*'s input parameter name *param_name*.
 
     Until *param* is found, the following are sequentially attempted:
         - elements in a HTML form
         - parameters in the URL's query part
         - key/value pairs in a *JSON* structure in the request's body
@@ -127,50 +130,60 @@
 
     # is JSON the content type of the request ?
     if request.mimetype == MIMETYPE_JSON:
         # yes, retrieve the JSON data
         result.update(request.get_json())
 
     # obtain parameters in URL query
-    result.update(request.values)  # noqa (bug: Ruff reports PD011)
+    result.update(request.values)
 
     # obtain parameters in form
     result.update(request.form)
 
     return result
 
 
-def http_delete(errors: list[str] | None, url: str, headers: dict = None,
-                params: dict = None, data: dict = None, json: dict = None, auth: str = None,
-                timeout: int | None = HTTP_DELETE_TIMEOUT, logger: logging.Logger = None) -> Response:
+def http_delete(errors: list[str] | None,
+                url: str,
+                headers: dict = None,
+                params: dict = None,
+                data: dict = None,
+                json: dict = None, auth: str = None,
+                timeout: int | None = HTTP_DELETE_TIMEOUT,
+                logger: logging.Logger = None) -> Response:
     """
-    Issue a *DELETE* request to the given *url*,and retrieve the returned response.
+    Issue a *DELETE* request to the given *url*, and return the retrieved response.
 
     The returned response might be *None*.
     The request might contain *headers* and *parameters*.
 
     :param errors: incidental error messages
     :param url: the destination URL
     :param headers: optional headers
     :param params: optional parameters
     :param data: optionaL data to send in the body of the request
     :param json: optional JSON to send in the body of the request
     :param auth: optional authentication scheme to use
-    :param timeout: timeout, in seconds (defaults to HTTP_POST_TIMEOUT - use None to omit)
+    :param timeout: timeout, in seconds (defaults to HTTP_DELETE_TIMEOUT - use None to omit)
     :param logger: optional logger to log the operation with
-    :return: the response to the PUT operation
+    :return: the response to the DELETE operation
     """
     return _http_rest(errors, "DELETE", url, headers, params, data, json, auth, timeout, logger)
 
 
-def http_get(errors: list[str] | None, url: str, headers: dict = None,
-             params: dict = None, data: dict = None, json: dict = None, auth: str = None,
-             timeout: int | None = HTTP_GET_TIMEOUT, logger: logging.Logger = None) -> Response:
+def http_get(errors: list[str] | None,
+             url: str,
+             headers: dict = None,
+             params: dict = None,
+             data: dict = None,
+             json: dict = None, auth: str = None,
+             timeout: int | None = HTTP_GET_TIMEOUT,
+             logger: logging.Logger = None) -> Response:
     """
-    Issue a *GET* request to the given *url*,and retrieve the returned response.
+    Issue a *GET* request to the given *url*, and return the retrieved response.
 
     The returned response might be *None*.
     The request might contain *headers* and *parameters*.
 
     :param errors: incidental error messages
     :param url: the destination URL
     :param headers: optional headers
@@ -178,22 +191,58 @@
     :param data: optionaL data to send in the body of the request
     :param json: optional JSON to send in the body of the request
     :param auth: optional authentication scheme to use
     :param timeout: timeout, in seconds (defaults to HTTP_GET_TIMEOUT - use None to omit)
     :param logger: optional logger
     :return: the response to the GET operation
     """
-    return _http_rest(errors, "GET", url, headers, params, data, json, auth, timeout, logger)
+    return _http_rest(errors, "GET", url, headers,
+                      params, data, json, auth, timeout, logger)
+
+
+def http_patch(errors: list[str] | None,
+               url: str,
+               headers: dict = None,
+               params: dict = None,
+               data: dict = None,
+               json: dict = None, auth: str = None,
+               timeout: int | None = HTTP_PATCH_TIMEOUT,
+               logger: logging.Logger = None) -> Response:
+    """
+    Issue a *PATCH* request to the given *url*, and return the retrieved response.
+
+    The returned response might be *None*.
+    The request might contain *headers* and *parameters*.
+
+    :param errors: incidental error messages
+    :param url: the destination URL
+    :param headers: optional headers
+    :param params: optional parameters
+    :param data: optionaL data to send in the body of the request
+    :param json: optional JSON to send in the body of the request
+    :param auth: optional authentication scheme to use
+    :param timeout: timeout, in seconds (defaults to HTTP_PATCH_TIMEOUT - use None to omit)
+    :param logger: optional logger to log the operation with
+    :return: the response to the PATCH operation
+    """
+    return _http_rest(errors, "POST", url, headers,
+                      params, data, json, auth, timeout, logger)
 
 
-def http_post(errors: list[str] | None, url: str, headers: dict = None,
-              params: dict = None, data: dict = None, json: dict = None, auth: str = None,
-              timeout: int | None = HTTP_POST_TIMEOUT, logger: logging.Logger = None) -> Response:
+def http_post(errors: list[str] | None,
+              url: str,
+              headers: dict = None,
+              params: dict = None,
+              data: dict = None,
+              json: dict = None,
+              auth: str = None,
+              timeout: int | None = HTTP_POST_TIMEOUT,
+              logger: logging.Logger = None) -> Response:
     """
-    Issue a *POST* request to the given *url*,and retrieve the returned response.
+    Issue a *POST* request to the given *url*, and return the retrieved response.
 
     The returned response might be *None*.
     The request might contain *headers* and *parameters*.
 
     :param errors: incidental error messages
     :param url: the destination URL
     :param headers: optional headers
@@ -201,22 +250,29 @@
     :param data: optionaL data to send in the body of the request
     :param json: optional JSON to send in the body of the request
     :param auth: optional authentication scheme to use
     :param timeout: timeout, in seconds (defaults to HTTP_POST_TIMEOUT - use None to omit)
     :param logger: optional logger to log the operation with
     :return: the response to the POST operation
     """
-    return _http_rest(errors, "POST", url, headers, params, data, json, auth, timeout, logger)
+    return _http_rest(errors, "POST", url, headers,
+                      params, data, json, auth, timeout, logger)
 
 
-def http_put(errors: list[str] | None, url: str, headers: dict = None,
-             params: dict = None, data: dict = None, json: dict = None, auth: str = None,
-             timeout: int | None = HTTP_POST_TIMEOUT, logger: logging.Logger = None) -> Response:
+def http_put(errors: list[str] | None,
+             url: str,
+             headers: dict = None,
+             params: dict = None,
+             data: dict = None,
+             json: dict = None,
+             auth: str = None,
+             timeout: int | None = HTTP_POST_TIMEOUT,
+             logger: logging.Logger = None) -> Response:
     """
-    Issue a *PUT* request to the given *url*,and retrieve the returned response.
+    Issue a *PUT* request to the given *url*, and return the retrieved response.
 
     The returned response might be *None*.
     The request might contain *headers* and *parameters*.
 
     :param errors: incidental error messages
     :param url: the destination URL
     :param headers: optional headers
@@ -224,22 +280,30 @@
     :param data: optionaL data to send in the body of the request
     :param json: optional JSON to send in the body of the request
     :param auth: optional authentication scheme to use
     :param timeout: timeout, in seconds (defaults to HTTP_POST_TIMEOUT - use None to omit)
     :param logger: optional logger to log the operation with
     :return: the response to the PUT operation
     """
-    return _http_rest(errors, "PUT", url, headers, params, data, json, auth, timeout, logger)
+    return _http_rest(errors, "PUT", url, headers,
+                      params, data, json, auth, timeout, logger)
 
 
-def _http_rest(errors: list[str], method: str, url: str, headers: dict,
-               params: dict, data: dict | None, json: dict | None,
-               auth: str | None, timeout: int, logger: logging.Logger) -> Response:
+def _http_rest(errors: list[str],
+               method: str,
+               url: str,
+               headers: dict,
+               params: dict,
+               data: dict | None,
+               json: dict | None,
+               auth: str | None,
+               timeout: int,
+               logger: logging.Logger) -> Response:
     """
-    Issue a *REST* request to the given *url*,and retrieve the returned response.
+    Issue a *REST* request to the given *url*, and return the retrieved response.
 
     The returned response might be *None*.
     The request might contain *headers* and *parameters*.
 
     :param errors: incidental error messages
     :param method: the REST method to use (GET, POST or PUT)
     :param url: the destination URL
@@ -299,14 +363,21 @@
                 case "GET":
                     result = requests.get(url=url,
                                           headers=op_headers,
                                           params=params,
                                           data=data,
                                           json=json,
                                           timeout=timeout)
+                case "PATCH":
+                    result = requests.patch(url=url,
+                                            headers=op_headers,
+                                            params=params,
+                                            data=data,
+                                            json=json,
+                                            timeout=timeout)
                 case "POST":
                     result = requests.post(url=url,
                                            headers=op_headers,
                                            params=params,
                                            data=data,
                                            json=json,
                                            timeout=timeout)
```

### Comparing `pypomes_http-0.1.2/src/pypomes_http/http_statuses.py` & `pypomes_http-0.1.3/src/pypomes_http/http_statuses.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,407 +1,406 @@
 from typing import Final
 
 # https://developer.mozilla.org/en-US/docs/Web/HTTP/Status
 # https://developer.mozilla.org/pt-BR/docs/Web/HTTP/Status
 
-# TODO: complete the descriptions
 _HTTP_STATUSES: Final[dict] = {
     # Informational responses
     100: {
         "name": "CONTINUE",
         "en": ("Interim response, indicating that the client should "
                "continue the request or ignore the response if the request is already finished."),
         "pt": ("Resposta provisória, indicando que o cliente deve continuar "
-               "a solicitação ou ignorar a resposta se a solicitação já estiver concluída.")
+               "a solicitação ou ignorar a resposta se a solicitação já estiver concluída."),
     },
     101: {
         "name": "SWITCHING PROTOCOLS",
         "en": ("Sent in response to an upgrade request header from the client, "
                "indicating the protocol the server is switching to."),
         "pt": ("Enviado em resposta a um cabeçalho de solicitação Upgrade do cliente, "
-               "indicando o protocolo para o qual o servidor está mudando.")
+               "indicando o protocolo para o qual o servidor está mudando."),
     },
     102: {
         "name": "PROCESSING",
         "en": ("Indicates that the server has received and is processing the request, "
                "but no response is available yet."),
         "pt": ("Indica que o servidor recebeu e está processando a requisição, "
-               "mas nenhuma resposta está disponível ainda.")
+               "mas nenhuma resposta está disponível ainda."),
     },
     103: {
         "name": "EARLY HINTS",
         "en": ("Used with the 'Link' header, letting the user agent start "
                "preloading resources while the server prepares a response."),
         "pt": ("Usado com o cabeçalho 'Link', permitindo que o agente do usuário "
-               "inicie o pré-carregamento de recursos enquanto o servidor prepara uma resposta.")
+               "inicie o pré-carregamento de recursos enquanto o servidor prepara uma resposta."),
     },
     # Successful responses
     200: {
         "name": "OK",
         "en": "The request succeeded.",
-        "pt": "A solicitação foi bem-sucedida."
+        "pt": "A solicitação foi bem-sucedida.",
     },
     201: {
         "name": "CREATED",
         "en": "The request succeeded, and a new resource was created as a result.",
-        "pt": "A requisição foi bem sucedida e um novo recurso foi criado como resultado."
+        "pt": "A requisição foi bem sucedida e um novo recurso foi criado como resultado.",
     },
     202: {
         "name": "ACCEPTED",
         "en": "The request has been received but not yet acted upon.",
-        "pt": "A solicitação foi recebida, mas ainda não foi atendida."
+        "pt": "A solicitação foi recebida, mas ainda não foi atendida.",
     },
     203: {
         "name": "NON AUTHORITATIVE INFORMATION",
         "en": ("The returned metadata is not exactly the same as is available from the origin server, "
                "but is collected from a local or a third-party copy."),
         "pt": ("Os metadados retornados não são exatamente os mesmos que estão disponíveis "
-               "no servidor de origem, mas são coletados de uma cópia local ou de terceiros.")
+               "no servidor de origem, mas são coletados de uma cópia local ou de terceiros."),
     },
     204: {
         "name": "NO CONTENT",
         "en": "There is no content to send for this request, but the headers may be useful.",
-        "pt": "Não há conteúdo para enviar para esta solicitação, mas os cabeçalhos podem ser úteis."
+        "pt": "Não há conteúdo para enviar para esta solicitação, mas os cabeçalhos podem ser úteis.",
     },
     205: {
         "name": "RESET CONTENT",
         "en": "Tells the user agent to reset the document which sent this request.",
-        "pt": "Diz ao agente do usuário para redefinir o documento que enviou esta solicitação."
+        "pt": "Diz ao agente do usuário para redefinir o documento que enviou esta solicitação.",
     },
     206: {
         "name": "PARTIAL CONTENT",
         "en": "used when the 'Range' header is sent from the client to request only part of a resource.",
-        "pt": "Usado quando o cabeçalho 'Range' é enviado do cliente para solicitar apenas parte de um recurso."
+        "pt": "Usado quando o cabeçalho 'Range' é enviado do cliente para solicitar apenas parte de um recurso.",
     },
     207: {
         "name": "MULTI-STATUS",
         "en": ("Conveys information about multiple resources, "
                "for situations where multiple status codes might be appropriate."),
         "pt": ("Transmite informações sobre vários recursos, "
-               "para situações em que vários códigos de status podem ser apropriados.")
+               "para situações em que vários códigos de status podem ser apropriados."),
     },
     208: {
         "name": "ALREADY REPORTED",
         "en": "Used inside a '<dav:propstat>' response element to avoid "
               "repeatedly enumerating the internal members of multiple bindings to the same collection.",
         "pt": ("Usado dentro de um elemento de resposta '<dav:propstat>' para evitar "
-               "enumerar repetidamente os membros internos de várias ligações para a mesma coleção.")
+               "enumerar repetidamente os membros internos de várias ligações para a mesma coleção."),
     },
     226: {
         "name": "IM USED",
         "en": ("The server has fulfilled a 'GET' request for the resource, and the response is a "
                "representation of the result of one or more instance-manipulations applied to the current instance."),
         "pt": ("O servidor atendeu a uma solicitação 'GET' para o recurso e a resposta é uma representação "
-               "do resultado de uma ou mais manipulações de instância aplicadas à instância atual.")
+               "do resultado de uma ou mais manipulações de instância aplicadas à instância atual."),
     },
     # Redirection messages
     300: {
         "name": "MULTIPLE CHOICES",
         "en": ("The request has more than one possible response. "
                "The user agent or user should choose one of them."),
         "pt": ("A solicitação tem mais de uma resposta possível. "
-               "O agente do usuário ou usuário deve escolher uma delas.")
+               "O agente do usuário ou usuário deve escolher uma delas."),
     },
     301: {
         "name": "MOVED PERMANENTLY",
         "en": "The URL of the requested resource has been changed permanently. The new URL is given in the response.",
-        "pt": "A URL do recurso solicitado foi permanentemente alterada. A nova URL é fornecida na resposta."
+        "pt": "A URL do recurso solicitado foi permanentemente alterada. A nova URL é fornecida na resposta.",
     },
     302: {
         "name": "FOUND",
         "en": ("The URI of requested resource has been changed temporarily. "
                "Further changes in the URI might be made in the future. "),
         "pt": ("A URI do recurso solicitado foi alterado temporariamente. "
-               "Outras alterações na URI podem ser feitas no futuro.")
+               "Outras alterações na URI podem ser feitas no futuro."),
     },
     303: {
         "name": "SEE OTHER",
         "en": ("The server sent this response to direct the client to get "
                 "the requested resource at another URI with a 'GET' request."),
         "pt": ("O servidor enviou esta resposta para direcionar o cliente "
-               "a obter o recurso solicitado em outro URI com uma solicitação 'GET'.")
+               "a obter o recurso solicitado em outro URI com uma solicitação 'GET'."),
     },
     304: {
         "name": "NOT MODIFIED",
         "en": ("Tells the client that the response has not been modified, "
                "so the client can continue to use the same cached version of the response."),
         "pt": ("Informa ao cliente que a resposta não foi modificada; "
-               "portanto, o cliente pode continuar a usar a mesma versão em cache da resposta.")
+               "portanto, o cliente pode continuar a usar a mesma versão em cache da resposta."),
     },
     305: {
         "name": "USE PROXY",
         "en": ("Indicates that a requested response must be accessed by a proxy. "
                "It has been deprecated due to security concerns regarding in-band configuration of a proxy."),
         "pt": ("Indica que uma resposta solicitada deve ser acessada por um proxy. "
-               "Foi descontinuado devido a questões de segurança em relação à configuração em banda de um proxy.")
+               "Foi descontinuado devido a questões de segurança em relação à configuração em banda de um proxy."),
     },
     307: {
         "name": "TEMPORARY REDIRECT",
         "en": ("The server sends this response to direct the client to get the "
                "requested resource at another URI, with the same method that was used in the prior request."),
         "pt": ("O servidor envia esta resposta para direcionar o cliente a obter "
-               "o recurso solicitado em outra URI, com o mesmo método usado na solicitação anterior.")
+               "o recurso solicitado em outra URI, com o mesmo método usado na solicitação anterior."),
     },
     308: {
         "name": "PERMANENT REDIRECT",
         "en": ("Indicates that the resource is now permanently located at another URI, "
                "specified by the 'Location:' HTTP Response header."),
         "pt": ("Indica que o recurso agora está permanentemente localizado em outra URI, "
-               "especificada pelo cabeçalho de resposta HTTP 'Location:'.")
+               "especificada pelo cabeçalho de resposta HTTP 'Location:'."),
     },
     # Client error responses
     400: {
         "name": "BAD REQUEST",
         "en": ("The server cannot process the request due to something that is perceived to be a client error "
                "(e.g., malformed request syntax, invalid request message framing, or deceptive request routing)."),
         "pt": ("O servidor não pode processar a solicitação devido a algo que é percebido como um erro do cliente "
-               "(e.g., solicitação malformada, roteamento ou enquadramento de mensagem de solicitação inválida).")
+               "(e.g., solicitação malformada, roteamento ou enquadramento de mensagem de solicitação inválida)."),
     },
     401: {
         "name": "UNAUTHORIZED",
         "en": ("Semantically, this response means 'unauthenticated'. "
                "The client must authenticate itself to get the requested response."),
         "pt": ("Semanticamente, essa resposta significa 'unauthenticated'. "
-               "O cliente deve se autenticar para obter a resposta solicitada.")
+               "O cliente deve se autenticar para obter a resposta solicitada."),
     },
     402: {
         "name": "PAYMENT REQUIRED",
         "en": "This response code is reserved for future use; no standard exists.",
-        "pt": "Este código de resposta está reservado para uso futuro; não existe convenção padrão."
+        "pt": "Este código de resposta está reservado para uso futuro; não existe convenção padrão.",
     },
     403: {
         "name": "FORBIDDEN",
         "en": ("The client does not have access rights to the content. "
                "Unlike '401 Unauthorized', the client's identity is known to the server."),
         "pt": ("O cliente não tem direitos de acesso ao conteúdo. "
-               "Ao contrário do '401 Unauthorized', a identidade do cliente é conhecida pelo servidor.")
+               "Ao contrário do '401 Unauthorized', a identidade do cliente é conhecida pelo servidor."),
     },
     404: {
         "name": "NOT FOUND",
         "en": ("The server cannot find the requested resource. Either the URL is not recognized, the resource "
                "does not exist, or the server is hiding the existence of a resource from an unauthorized client."),
         "pt": ("O servidor não pode encontrar o recurso solicitado. A URL não é reconhecida, o recurso não existe, "
-               "ou o servidor está ocultando a existência de um recurso de um cliente não autorizado.")
+               "ou o servidor está ocultando a existência de um recurso de um cliente não autorizado."),
     },
     405: {
         "name": "METHOD NOT ALLOWED",
         "en": "The request method is known by the server but is not supported by the target resource. "
               "For example, an API may not allow calling 'DELETE' to remove a resource.",
         "pt": "O método de solicitação é conhecido pelo servidor, mas não é suportado pelo recurso de destino. "
-              "Por exemplo, uma API pode não permitir chamar 'DELETE' para remover um recurso."
+              "Por exemplo, uma API pode não permitir chamar 'DELETE' para remover um recurso.",
     },
     406: {
         "name": "NOT ACCEPTABLE",
         "en": ("After performing server-driven content negotiation, the server "
                "does not find any content that conforms to the criteria given by the user agent."),
         "pt": ("Após realizar negociação de conteúdo, o servidor não encontra conteúdo "
-               "que esteja em conformidade com os critérios fornecidos pelo o agente do usuário.")
+               "que esteja em conformidade com os critérios fornecidos pelo o agente do usuário."),
     },
     407: {
         "name": "PROXY AUTHENTICATION REQUIRED",
         "en": "Semelhante a '401 Unauthorized', mas a autenticação precisa ser feita por um proxy.",
-        "pt": "This is similar to '401 Unauthorized' but the authentication needs to be done by a proxy."
+        "pt": "This is similar to '401 Unauthorized' but the authentication needs to be done by a proxy.",
     },
     408: {
         "name": "REQUEST TIMEOUT",
         "en": ("This response is sent on an idle or unused connection "
                "by the server, whenever it feels the need to shut it down."),
         "pt": ("Esta resposta é enviada pelo servidor em uma conexão ociosa ou "
-               "não utilizada, sempre que seu desligamento se fizer necessário.")
+               "não utilizada, sempre que seu desligamento se fizer necessário."),
     },
     409: {
         "name": "CONFLICT",
         "en": "This response is sent when a request conflicts with the current state of the server.",
-        "pt": "Esta resposta é enviada quando uma requisição conflitar com o estado atual do servidor."
+        "pt": "Esta resposta é enviada quando uma requisição conflitar com o estado atual do servidor.",
     },
     410: {
         "name": "GONE",
         "en": ("This response is sent when the requested content "
                "has been permanently deleted from server, with no forwarding address."),
         "pt": ("Esta resposta é enviada quando o conteúdo solicitado "
-               "foi excluído permanentemente do servidor, sem endereço de encaminhamento.")
+               "foi excluído permanentemente do servidor, sem endereço de encaminhamento."),
     },
     411: {
         "name": "LENGTH REQUIRED",
         "en": ("The server rejected the request because the 'Content-Length' "
                "header field is not defined, and the server requires it."),
         "pt": ("O servidor rejeitou a solicitação porque o campo de cabeçalho "
-               "'Content-Length' não está definido, e o servidor o exige.")
+               "'Content-Length' não está definido, e o servidor o exige."),
     },
     412: {
         "name": "PRECONDITION FAILED",
         "en": "The client has indicated preconditions in its headers which the server does not meet.",
-        "pt": "O cliente indicou nos seus cabeçalhos pré-condições que o servidor não atende."
+        "pt": "O cliente indicou nos seus cabeçalhos pré-condições que o servidor não atende.",
     },
     413: {
         "name": "PAYLOAD TOO LARGE",
         "en": ("The request entity is larger than limits defined by server. "
                "The server might close the connection or return a 'Retry-After' header field."),
         "pt": ("A entidade requisição é maior do que os limites definidos pelo servidor. "
-               "O servidor pode fechar a conexão ou retornar um campo de cabeçalho 'Retry-After'.")
+               "O servidor pode fechar a conexão ou retornar um campo de cabeçalho 'Retry-After'."),
     },
     414: {
         "name": "URI TOO LONG",
         "en": "The URI requested by the client is longer than the server is willing to interpret.",
-        "pt": "A URI solicitada pelo cliente é mais longa do que o servidor está disposto a interpretar."
+        "pt": "A URI solicitada pelo cliente é mais longa do que o servidor está disposto a interpretar.",
     },
     415: {
         "name": "UNSUPPORTED MEDIA TYPE",
         "en": ("The media format of the requested data is not supported by the server, "
                "so the server is rejecting the request."),
         "pt": ("O formato de mídia dos dados requisitados não é suportado pelo servidor, "
-               "que portanto está rejeitando a requisição.")
+               "que portanto está rejeitando a requisição."),
     },
     416: {
         "name": "RANGE NOT SATISFIABLE",
         "en": ("The range specified by the 'Range' header field in the request cannot be fulfilled. "
                "It's possible that the range is outside the size of the target URI's data."),
         "pt": ("O intervalo especificado pelo campo de cabeçalho 'Range' na solicitação não pode ser atendido. "
-               "É possível que o intervalo esteja fora do tamanho dos dados da URI de destino.")
+               "É possível que o intervalo esteja fora do tamanho dos dados da URI de destino."),
     },
     417: {
         "name": "EXPECTATION FAILED",
         "en": "The expectation indicated by the 'Expect' request header field cannot be met by the server.",
-        "pt": "A expectativa indicada pelo campo de cabeçalho 'Expect' não pode ser atendida pelo servidor."
+        "pt": "A expectativa indicada pelo campo de cabeçalho 'Expect' não pode ser atendida pelo servidor.",
     },
     418: {
         "name": "I'M A TEAPOT",
         "en": ("The server refuses the attempt to brew coffee with a teapot. "
                "This was an April Fools joke from 1998, kept in the official standard by popular demand."),
         "pt": ("O servidor recusa a tentativa de coar café num bule de chá. "
-               "Essa foi uma brincadeira de 1o. de Abril em 1998, mantida no padrão oficial por clamor popular.")
+               "Essa foi uma brincadeira de 1o. de Abril em 1998, mantida no padrão oficial por clamor popular."),
     },
     421: {
         "name": "MISDIRECTED REQUEST",
         "en": ("The request was directed at a server that is not able to produce a response. "
                "The server is not configured to produce responses for the combination "
                "of scheme and authority that are included in the request URI."),
         "pt": ("A requisição foi direcionada a um servidor inapto a produzir a resposta. "
                "O servidor não está configurado para produzir respostas para a combinação "
-               "de esquema e autoridade inclusas na URI da requisição.")
+               "de esquema e autoridade inclusas na URI da requisição."),
     },
     422: {
         "name": "UNPROCESSABLE CONTENT",
         "en": "The request was well-formed but was unable to be followed, due to semantic errors.",
-        "pt": "A solicitação foi bem formada, mas não pôde ser atendida devido a erros semânticos."
+        "pt": "A solicitação foi bem formada, mas não pôde ser atendida devido a erros semânticos.",
     },
     423: {
         "name": "LOCKED",
         "en": "The resource that is being accessed is locked.",
-        "pt": "O recurso que está sendo acessado está bloqueado."
+        "pt": "O recurso que está sendo acessado está bloqueado.",
     },
     424: {
         "name": "FAILED DEPENDENCY",
         "en": "The request failed due to failure of a previous request.",
-        "pt": "A solicitação falhou devido à falha de uma solicitação anterior."
+        "pt": "A solicitação falhou devido à falha de uma solicitação anterior.",
     },
     425: {
         "name": "TOO EARLY",
         "en": "The server is unwilling to risk processing a request that might be replayed.",
-        "pt": "O servidor não está disposto a correr o risco de processar uma solicitação que pode ser repetida."
+        "pt": "O servidor não está disposto a correr o risco de processar uma solicitação que pode ser repetida.",
     },
     426: {
         "name": "UPGRADE REQUIRED",
         "en": ("The server refuses to perform the request using the current protocol, "
                "but might be willing to do so after the client upgrades to a different protocol. "
                "The server sends an 'Upgrade' header in this response to indicate the required protocol(s)."),
         "pt": "O servidor se recusa a executar a solicitação usando o protocolo atual, "
               "mas pode estar disposto a fazê-lo depois que o cliente atualizar para um protocolo diferente. "
-              "O servidor envia um cabeçalho 'Upgrade' nessa resposta, para indicar os protocolos necessários."
+              "O servidor envia um cabeçalho 'Upgrade' nessa resposta, para indicar os protocolos necessários.",
     },
     428: {
         "name": "PRECONDITION REQUIRED",
         "en": ("The origin server requires the request to be conditional. "
                "Intended to prevent the 'lost update' problem, where a client 'GET's a resource's state, "
                "modifies it, and 'PUT's it back to the server, when meanwhile a third party has modified "
                "the state on the server, leading to a conflict."),
         "pt": ("O servidor de origem exige que a solicitação seja condicional. "
                "Previne o problema da 'atualização perdida', onde um cliente obtem ('GET') "
                "o estado de um recurso, o modifica e o coloca ('PUT') de volta no servidor, "
-               "quando entretanto um terceiro modificou o estado no servidor, levando a um conflito.")
+               "quando entretanto um terceiro modificou o estado no servidor, levando a um conflito."),
     },
     429: {
         "name": "TOO MANY REQUESTS",
         "en": "The user has sent too many requests in a given amount of time ('rate limiting').",
-        "pt": "O usuário enviou muitas requisições num dado tempo ('limitação de taxa')."
+        "pt": "O usuário enviou muitas requisições num dado tempo ('limitação de taxa').",
     },
     431: {
         "name": "REQUEST HEADER FIELDS TOO LARGE",
         "en": ("The server is unwilling to process the request because its header fields are too large. "
                "The request may be resubmitted after the reduction of the size of the request header fields."),
         "pt": ("O servidor recusa-se a processar a solicitação porque seus campos de cabeçalho são muito grandes. "
-               "A solicitação pode ser reenviada após a redução o tamanho dos campos do cabeçalho da solicitação.")
+               "A solicitação pode ser reenviada após a redução o tamanho dos campos do cabeçalho da solicitação."),
     },
     451: {
         "name": "UNAVAILABLE FOR LEGAL REASONS",
         "en": ("The user agent requested a resource that cannot legally be provided, "
                "such as a web page censored by a government."),
         "pt": ("O agente do usuário solicitou um recurso que não pode ser fornecido legalmente, "
-               "tal como uma página da Web censurada por um governo.")
+               "tal como uma página da Web censurada por um governo."),
     },
     # Server error responses
     500: {
         "name": "INTERNAL SERVER ERROR",
         "en": "The server has encountered a situation it does not know how to handle.",
-        "pt": "O servidor encontrou uma situação com a qual não sabe lidar."
+        "pt": "O servidor encontrou uma situação com a qual não sabe lidar.",
     },
     501: {
         "name": "NOT IMPLEMENTED",
         "en": "The request method is not supported by the server and cannot be handled. "
               "The only methods that servers are required to support are 'GET' and 'HEAD'.",
         "pt": "O método da requisição não é suportado pelo servidor e não pode ser manipulado. "
-              "Os únicos métodos que servidores são obrigados a suportar são 'GET' e 'HEAD'."
+              "Os únicos métodos que servidores são obrigados a suportar são 'GET' e 'HEAD'.",
     },
     502: {
         "name": "BAD GATEWAY",
         "en": ("The server, while working as a gateway to get a response "
                "needed to handle the request, got an invalid response."),
         "pt": ("O servidor, enquanto trabalhava como um gateway para obter uma resposta "
-               "necessária para lidar com a solicitação, obteve uma resposta inválida.")
+               "necessária para lidar com a solicitação, obteve uma resposta inválida."),
     },
     503: {
         "name": "SERVICE UNAVAILABLE",
         "en": ("The server is not ready to handle the request. "
                "Common causes are a server that is down for maintenance or is overloaded."),
         "pt": ("O servidor não está pronto para manipular a requisição. "
-               "Causas comuns são um servidor em manutenção ou sobrecarregado.")
+               "Causas comuns são um servidor em manutenção ou sobrecarregado."),
     },
     504: {
         "name": "GATEWAY TIMEOUT",
         "en": "The server is acting as a gateway and cannot get a response in time.",
-        "pt": "O servidor está atuando como um gateway e não consegue obter uma resposta a tempo."
+        "pt": "O servidor está atuando como um gateway e não consegue obter uma resposta a tempo.",
     },
     505: {
         "name": "HTTP VERSION NOT SUPPORTED",
         "en": "The HTTP version used in the request is not supported by the server.",
-        "pt": "A versão HTTP usada na requisição não é suportada pelo servidor."
+        "pt": "A versão HTTP usada na requisição não é suportada pelo servidor.",
     },
     506: {
         "name": "VARIANT ALSO NEGOTIATES",
         "en": ("The chosen variant resource is configured to engage in transparent content negotiation itself, "
                "and is therefore not a proper end point in the negotiation process."),
         "pt": ("O recurso variante escolhido está configurado para se envolver em negociação "
-               "de conteúdo transparente, e portanto, não é um 'endpoint' adequado no processo de negociação.")
+               "de conteúdo transparente, e portanto, não é um 'endpoint' adequado no processo de negociação."),
     },
     507: {
         "name": "INSUFFICIENT STORAGE",
         "en": ("The method could not be performed on the resource, because the server "
                "is unable to store the representation needed to successfully complete the request."),
         "pt": ("O método não pôde ser executado no recurso porque o servidor "
-               "não pode armazenar a representação necessária para concluir a solicitação com êxito.")
+               "não pode armazenar a representação necessária para concluir a solicitação com êxito."),
     },
     508: {
         "name": "LOOP DETECTED",
         "en": "The server detected an infinite loop while processing the request.",
-        "pt": "O servidor detectou um loop infinito ao processar a solicitação."
+        "pt": "O servidor detectou um loop infinito ao processar a solicitação.",
     },
     510: {
         "name": "NOT EXTENDED",
         "en": "Further extensions to the request are required for the server to fulfill it.",
-        "pt": "Extensões adicionais à solicitação são necessárias para que o servidor a atenda."
+        "pt": "Extensões adicionais à solicitação são necessárias para que o servidor a atenda.",
     },
     511: {
         "name": "NETWORK AUTHENTICATION REQUIRED",
         "en": "Indicates that the client needs to authenticate to gain network access.",
-        "pt": "Indica que o cliente precisa se autenticar para obter acesso à rede."
-    }
+        "pt": "Indica que o cliente precisa se autenticar para obter acesso à rede.",
+    },
 }
```

### Comparing `pypomes_http-0.1.2/LICENSE` & `pypomes_http-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.1.2/pyproject.toml` & `pypomes_http-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_http"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (HTTP modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_http-0.1.2/PKG-INFO` & `pypomes_http-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_http
-Version: 0.1.2
+Version: 0.1.3
 Summary: A collection of Python pomes, pennyeach (HTTP modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-HTTP
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-HTTP/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

