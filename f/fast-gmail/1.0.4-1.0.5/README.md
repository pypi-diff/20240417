# Comparing `tmp/fast_gmail-1.0.4.tar.gz` & `tmp/fast_gmail-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_gmail-1.0.4.tar", last modified: Mon Apr 15 09:01:50 2024, max compression
+gzip compressed data, was "fast_gmail-1.0.5.tar", last modified: Wed Apr 17 12:07:46 2024, max compression
```

## Comparing `fast_gmail-1.0.4.tar` & `fast_gmail-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-15 09:01:50.307557 fast_gmail-1.0.4/
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     1062 2024-04-08 06:15:40.000000 fast_gmail-1.0.4/LICENSE
--rw-r--r--   0 aleti     (1000) aleti     (1000)    14792 2024-04-15 09:01:50.307557 fast_gmail-1.0.4/PKG-INFO
--rw-rw-r--   0 aleti     (1000) aleti     (1000)    14032 2024-04-15 09:01:05.000000 fast_gmail-1.0.4/README.md
-drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-15 09:01:50.307557 fast_gmail-1.0.4/fast_gmail/
--rw-rw-r--   0 aleti     (1000) aleti     (1000)       30 2024-04-15 08:44:02.000000 fast_gmail-1.0.4/fast_gmail/__init__.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)      358 2024-04-15 06:27:06.000000 fast_gmail-1.0.4/fast_gmail/draft.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)    19262 2024-04-15 07:00:58.000000 fast_gmail-1.0.4/fast_gmail/gmail.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     7199 2024-04-15 06:26:53.000000 fast_gmail-1.0.4/fast_gmail/helpers.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)    25326 2024-04-15 06:27:25.000000 fast_gmail-1.0.4/fast_gmail/message.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     3601 2024-04-08 06:37:52.000000 fast_gmail-1.0.4/fast_gmail/search.py
-drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-15 09:01:50.307557 fast_gmail-1.0.4/fast_gmail.egg-info/
--rw-r--r--   0 aleti     (1000) aleti     (1000)    14792 2024-04-15 09:01:50.000000 fast_gmail-1.0.4/fast_gmail.egg-info/PKG-INFO
--rw-rw-r--   0 aleti     (1000) aleti     (1000)      323 2024-04-15 09:01:50.000000 fast_gmail-1.0.4/fast_gmail.egg-info/SOURCES.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)        1 2024-04-15 09:01:50.000000 fast_gmail-1.0.4/fast_gmail.egg-info/dependency_links.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)      116 2024-04-15 09:01:50.000000 fast_gmail-1.0.4/fast_gmail.egg-info/requires.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)       11 2024-04-15 09:01:50.000000 fast_gmail-1.0.4/fast_gmail.egg-info/top_level.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)       38 2024-04-15 09:01:50.307557 fast_gmail-1.0.4/setup.cfg
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     1056 2024-04-15 09:01:28.000000 fast_gmail-1.0.4/setup.py
+drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-17 12:07:46.498422 fast_gmail-1.0.5/
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     1062 2024-04-08 06:15:40.000000 fast_gmail-1.0.5/LICENSE
+-rw-r--r--   0 aleti     (1000) aleti     (1000)    14792 2024-04-17 12:07:46.498422 fast_gmail-1.0.5/PKG-INFO
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)    14032 2024-04-17 12:07:20.000000 fast_gmail-1.0.5/README.md
+drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-17 12:07:46.494423 fast_gmail-1.0.5/fast_gmail/
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)       30 2024-04-15 08:44:02.000000 fast_gmail-1.0.5/fast_gmail/__init__.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)      358 2024-04-15 06:27:06.000000 fast_gmail-1.0.5/fast_gmail/draft.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)    21074 2024-04-17 11:51:01.000000 fast_gmail-1.0.5/fast_gmail/gmail.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     7199 2024-04-15 06:26:53.000000 fast_gmail-1.0.5/fast_gmail/helpers.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)    25018 2024-04-17 11:49:05.000000 fast_gmail-1.0.5/fast_gmail/message.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     3601 2024-04-08 06:37:52.000000 fast_gmail-1.0.5/fast_gmail/search.py
+drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-17 12:07:46.498422 fast_gmail-1.0.5/fast_gmail.egg-info/
+-rw-r--r--   0 aleti     (1000) aleti     (1000)    14792 2024-04-17 12:07:46.000000 fast_gmail-1.0.5/fast_gmail.egg-info/PKG-INFO
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)      323 2024-04-17 12:07:46.000000 fast_gmail-1.0.5/fast_gmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)        1 2024-04-17 12:07:46.000000 fast_gmail-1.0.5/fast_gmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)      116 2024-04-17 12:07:46.000000 fast_gmail-1.0.5/fast_gmail.egg-info/requires.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)       11 2024-04-17 12:07:46.000000 fast_gmail-1.0.5/fast_gmail.egg-info/top_level.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)       38 2024-04-17 12:07:46.498422 fast_gmail-1.0.5/setup.cfg
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     1074 2024-04-17 12:07:33.000000 fast_gmail-1.0.5/setup.py
```

### Comparing `fast_gmail-1.0.4/LICENSE` & `fast_gmail-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.4/PKG-INFO` & `fast_gmail-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_gmail
-Version: 1.0.4
+Version: 1.0.5
 Summary: GmailApi wrapper
 Home-page: https://github.com/aleti1/fast_gmail
 Author: Aleti
 Author-email: aleti.open.source@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -18,16 +18,14 @@
 Requires-Dist: google-api-python-client==2.125.0
 Requires-Dist: google-auth-httplib2==0.2.0
 Requires-Dist: google-auth-oauthlib==1.2.0
 Requires-Dist: typing-extensions==4.11.0
 
 # Fast-gmail a simple python wrapper for gmailapi
 
-[![PyPI](https://img.shields.io/pypi/v/fast-gmail)](https://pypi.org/project/fast-gmail/)
-
 ---
 ## Functionalities:
 - Send text/html messages
 - Send messages with signature & attachments
 - Get messages with pagination
 - Filter messages
 - Get drafts
@@ -42,24 +40,23 @@
 
 ## Usage:
 
 ### Initialization
 - Go to https://console.developers.google.com/apis/credentials and login to correct account
 - Setup Oauth consent screen
 - Create new credentials with OAuth client ID for web or installed app
-- Set Authorized Javascript origins to http://localhost:3000/
-- Set Authorized redirect URIs to http://localhost:3000/
+- Set Authorized redirect URIs to http://localhost:3000/ (Notice the trailing slash)
 - Download the credentials.json file
 - Go to Enable APIs & services and enable GmailAPI
 
 With credentials.json file downloaded we can connect to Gmail
 ```
 gmail = GmailApi(
-    credentials_file_path = __path_to_credentials_json_file__,
-    port = 3000, # default is 3000 but you can use any other port IMPORTANT: if you change this default value don't forget to also changed on Authorized Javascript origins & Authorized redirect URIs
+    credentials_file_path = __path_to_credentials_json_file__,  # Defaults to ./credentials.json
+    port = 3000, # Defaults to 3000  !IMPORTANT: if you change this default value don't forget to also changed on Authorized redirect URIs
 )
 ```
 
 ### Send message
 ``` 
     from fast_gmail import GmailApi
 
@@ -68,26 +65,28 @@
         to: str,
         subject: str,
         html: Optional[str]=None,
         text: Optional[str]=None,
         cc: Optional[List[str] | str]=None,
         bcc: Optional[List[str] | str]=None,
         attachments: Optional[List[str] | str]=None,
+		in_reply_to: Optional[str] = None,
         signature: bool = True
     )
     """Sends an email message.
         Args:
             sender (str): Email address of the message sender.
             to (str): Email address of the recipient.
             subject (str): Subject line of the email.
             html (Optional[str], optional): HTML content of the email body. Defaults to None.
             text (Optional[str], optional): Plain text content of the email body. Defaults to None.
             cc (Optional[List[str] | str], optional): List of email addresses to carbon copy. Defaults to None.
             bcc (Optional[List[str] | str], optional): List of email addresses to blind carbon copy. Defaults to None.
             attachments (Optional[List[str] | str], optional): List of file paths to attach to the email. Defaults to None.
+            in_reply_to (Optional[str], optional): Message.message_id value that is replyed to. Defaults to None.
             signature (bool, optional): Whether to include a signature (if configured). Defaults to True.
         Returns:
             Optional[Message]: An object representing the sent message, or None on error.
     """
 ```
 
 ### Get messages
```

### Comparing `fast_gmail-1.0.4/README.md` & `fast_gmail-1.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # Fast-gmail a simple python wrapper for gmailapi
 
-[![PyPI](https://img.shields.io/pypi/v/fast-gmail)](https://pypi.org/project/fast-gmail/)
-
 ---
 ## Functionalities:
 - Send text/html messages
 - Send messages with signature & attachments
 - Get messages with pagination
 - Filter messages
 - Get drafts
@@ -20,24 +18,23 @@
 
 ## Usage:
 
 ### Initialization
 - Go to https://console.developers.google.com/apis/credentials and login to correct account
 - Setup Oauth consent screen
 - Create new credentials with OAuth client ID for web or installed app
-- Set Authorized Javascript origins to http://localhost:3000/
-- Set Authorized redirect URIs to http://localhost:3000/
+- Set Authorized redirect URIs to http://localhost:3000/ (Notice the trailing slash)
 - Download the credentials.json file
 - Go to Enable APIs & services and enable GmailAPI
 
 With credentials.json file downloaded we can connect to Gmail
 ```
 gmail = GmailApi(
-    credentials_file_path = __path_to_credentials_json_file__,
-    port = 3000, # default is 3000 but you can use any other port IMPORTANT: if you change this default value don't forget to also changed on Authorized Javascript origins & Authorized redirect URIs
+    credentials_file_path = __path_to_credentials_json_file__,  # Defaults to ./credentials.json
+    port = 3000, # Defaults to 3000  !IMPORTANT: if you change this default value don't forget to also changed on Authorized redirect URIs
 )
 ```
 
 ### Send message
 ``` 
     from fast_gmail import GmailApi
 
@@ -46,26 +43,28 @@
         to: str,
         subject: str,
         html: Optional[str]=None,
         text: Optional[str]=None,
         cc: Optional[List[str] | str]=None,
         bcc: Optional[List[str] | str]=None,
         attachments: Optional[List[str] | str]=None,
+		in_reply_to: Optional[str] = None,
         signature: bool = True
     )
     """Sends an email message.
         Args:
             sender (str): Email address of the message sender.
             to (str): Email address of the recipient.
             subject (str): Subject line of the email.
             html (Optional[str], optional): HTML content of the email body. Defaults to None.
             text (Optional[str], optional): Plain text content of the email body. Defaults to None.
             cc (Optional[List[str] | str], optional): List of email addresses to carbon copy. Defaults to None.
             bcc (Optional[List[str] | str], optional): List of email addresses to blind carbon copy. Defaults to None.
             attachments (Optional[List[str] | str], optional): List of file paths to attach to the email. Defaults to None.
+            in_reply_to (Optional[str], optional): Message.message_id value that is replyed to. Defaults to None.
             signature (bool, optional): Whether to include a signature (if configured). Defaults to True.
         Returns:
             Optional[Message]: An object representing the sent message, or None on error.
     """
 ```
 
 ### Get messages
```

### Comparing `fast_gmail-1.0.4/fast_gmail/gmail.py` & `fast_gmail-1.0.5/fast_gmail/gmail.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from typing import Optional
 from typing import Union
 from typing import List
 import mimetypes
 import base64
 import os
+import json
 
 from email.message import EmailMessage
 from email.header import Header
 from email import utils
 
 from googleapiclient.discovery import build
 from google.oauth2.credentials import Credentials
 from googleapiclient.errors import HttpError
-from google_auth_oauthlib.flow import InstalledAppFlow
+from google_auth_oauthlib.flow import InstalledAppFlow, Flow
 
 from fast_gmail.message import MessagePartBody
 from fast_gmail.message import Message
 from fast_gmail.search import SearchParams
 from fast_gmail.draft import Draft
 from fast_gmail.helpers import *
 
@@ -36,40 +37,77 @@
 	SEPARATOR_SYMBOL: str
 	profile_data: Optional[GmailProfile] = None
 
 	def __init__(
 		self,
 		token_file_path: str = "token.json",
 		credentials_file_path: str = "credentials.json",
-		port: int = 3000, # set the local server port for Authorized redirect URI 
+		port: int = 3000, # set the local server port for Authorized redirect URI
 		separator_symbol: Optional[str] = ", ",
-		user_id: Optional[str] = "me"
+		user_id: Optional[str] = "me",
+		application_type: ApplicationType = ApplicationType.WEB,
+		code: Optional[str] = None
 	)-> None:
 		"""https://github.com/googleapis/google-api-python-client/blob/main/docs/oauth-installed.md"""
+
 		# set separator for spliting/joining the array of existing previous_page_tokens for pagination
 		self.SEPARATOR_SYMBOL = separator_symbol
 		# The file token.json stores the user's access and refresh tokens, and is
 		# created automatically when the authorization flow completes for the first time.
 		if os.path.exists(token_file_path):
 			self.credentials = Credentials.from_authorized_user_file(token_file_path, SCOPES)
+		self.auth_url: str = ""
 		# If there are no (valid) credentials available, let the user log in.
 		if not self.credentials or not self.credentials.valid:
 			if self.credentials and self.credentials.expired and self.credentials.refresh_token:
+				# refresh access token
 				self.credentials = Credentials(
 					token=None,  # No initial token provided, refresh token will be used
 					refresh_token=self.credentials.refresh_token,
 					token_uri=self.credentials.token_uri,
 					client_id=self.credentials.client_id,
 					client_secret=self.credentials.client_secret
 				)
 			else:
-				flow = InstalledAppFlow.from_client_secrets_file(
-					credentials_file_path, SCOPES
-				)
-				self.credentials = flow.run_local_server(port=port)
+				if not os.path.exists(credentials_file_path):
+					raise FileNotFoundError(f"{credentials_file_path=} NOT FOUND!")
+				match application_type:
+					case ApplicationType.DESKTOP:
+						flow = InstalledAppFlow.from_client_secrets_file(
+							credentials_file_path, SCOPES
+						)
+						self.credentials = flow.run_local_server(port=port)
+					case ApplicationType.WEB:
+						cred_payload: Optional[dict] = None
+						with open(credentials_file_path, "r") as f:
+							cred_payload = json.loads(f.read())
+						if not cred_payload:
+							raise Exception(f"Could't read {credentials_file_path=}")
+						if not "web" in cred_payload:
+							raise Exception(f"{cred_payload=} content missing. \n\033[91mDid you create credentials for Web app?\033[0m")
+						if not "redirect_uris" in cred_payload["web"]:
+							raise Exception(f"Missing `redirect_uris` key from {cred_payload['web']}. \n\033[91mDid you define Authorized redirect URIs?\033[0m")
+						
+						redirect_uris = cred_payload["web"]["redirect_uris"]
+						for uri in redirect_uris:
+							if str(port) in uri:
+								self.redirect_uri = uri
+						if not self.redirect_uri:
+							self.redirect_uri = redirect_uris[0]
+						self.flow = Flow.from_client_secrets_file(
+							credentials_file_path,
+							SCOPES,
+							redirect_uri=self.redirect_uri
+						)
+						if code:
+							self.flow.fetch_token(code=code)
+							self.credentials: str = self.flow.credentials
+						else:
+							self.auth_url = f"{self.flow.authorization_url()[0]}&prompt=consent"
+							return
 			# Save the credentials for the next run
 			with open(token_file_path, "w") as token:
 				token.write(self.credentials.to_json())
 		try:
 			# Call the Gmail API and set the instance 
 			self.google_service = GoogleService(
 				service = build("gmail", "v1", credentials = self.credentials),
@@ -114,37 +152,42 @@
 		to: str,
 		subject: str,
 		html: Optional[str]=None,
 		text: Optional[str]=None,
 		cc: Optional[List[str] | str]=None,
 		bcc: Optional[List[str] | str]=None,
 		attachments: Optional[List[str] | str]=None,
+		in_reply_to: Optional[str] = None,
 		signature: bool = True
 	)-> Optional[Message]:
 		"""Sends an email message.
 			Args:
 				sender (str): Email address of the message sender.
 				to (str): Email address of the recipient.
 				subject (str): Subject line of the email.
 				html (Optional[str], optional): HTML content of the email body. Defaults to None.
 				text (Optional[str], optional): Plain text content of the email body. Defaults to None.
 				cc (Optional[List[str] | str], optional): List of email addresses to carbon copy. Defaults to None.
 				bcc (Optional[List[str] | str], optional): List of email addresses to blind carbon copy. Defaults to None.
 				attachments (Optional[List[str] | str], optional): List of file paths to attach to the email. Defaults to None.
+				in_reply_to (Optional[str], optional): Message.message_id value that is replyed to. Defaults to None.
 				signature (bool, optional): Whether to include a signature (if configured). Defaults to True.
 			Returns:
 				Optional[Message]: An object representing the sent message, or None on error.
 			"""
 		msg = EmailMessage()
 		msg["To"] = to
 		msg["From"] = str(Header(f"{sender} <{sender}>"))
-		msg["Subject"] = subject
+		msg["Subject"] = subject if not in_reply_to else f"Re: {subject}"
 		msg["Date"] = utils.formatdate(localtime=1)
 		msg["Cc"] = ", ".join(cc) if cc else ""
 		msg["Bcc"] = ", ".join(bcc) if bcc else ""
+		if in_reply_to:
+			msg["In-Reply-To"] = in_reply_to
+			msg["References"] = in_reply_to
 		if signature and html:
 			account_signature = self._alias_info(sender)
 			html = f"{html}<br/><br/>{account_signature['signature'] if 'signature' in account_signature else ''}"
 		if text:
 			msg.set_content(text.strip())
 		if html:
 			msg.add_alternative(html.strip(), subtype = "html")
```

### Comparing `fast_gmail-1.0.4/fast_gmail/helpers.py` & `fast_gmail-1.0.5/fast_gmail/helpers.py`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.4/fast_gmail/message.py` & `fast_gmail-1.0.5/fast_gmail/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -334,14 +334,29 @@
 	def message_headers(self)-> Optional[List[MessageHeader]]:
 		if not self.payload:
 			return None
 		if not self.payload.headers:
 			return None
 		return self.payload.headers
 
+	def _extract_content(self, part: MessagePart, result: dict)-> None:
+		# TODO: load cid: images into content
+		if part.mimeType not in ["text/plain", "text/html"]:
+			for sub_part in part.parts:
+				self._extract_content(sub_part, result)
+		if not part.mimeType in result:
+			result[part.mimeType] = []
+		if not part.body:
+			return
+		if not part.body.data:
+			return
+		result[part.mimeType].append(
+			base64.urlsafe_b64decode(part.body.data).decode("utf-8")
+		)
+
 	def _content(self)-> Optional[dict]:
 		if not self.payload:
 			return None
 		result = {}
 		if not self.payload.parts:
 			if self.payload.mimeType in ["text/plain", "text/html"] and self.payload.body:
 				if self.payload.body.data:
@@ -352,39 +367,15 @@
 					)
 					return result
 			return {
 				"multipart/alternative": base64.urlsafe_b64decode(
 					self.payload.body.data
 				).decode("utf-8")} if self.payload.body else None
 		for part in self.payload.parts:
-			if part.mimeType == "multipart/alternative":
-				for sub_part in part.parts:
-					if sub_part.mimeType not in ["text/plain", "text/html"]:
-						continue
-					if not sub_part.mimeType in result:
-						result[sub_part.mimeType] = []
-					if not sub_part.body:
-						continue
-					if not sub_part.body.data:
-						continue
-					result[sub_part.mimeType].append(
-						base64.urlsafe_b64decode(sub_part.body.data).decode("utf-8")
-					)
-			else:
-				if part.mimeType not in ["text/plain", "text/html"]:
-					continue
-				if not part.mimeType in result:
-					result[part.mimeType] = []
-				if not part.body:
-					continue
-				if not part.body.data:
-					continue
-				result[part.mimeType].append(
-					base64.urlsafe_b64decode(part.body.data).decode("utf-8")
-				)
+			self._extract_content(part, result)
 		return result
 	
 	@property
 	def body(self)-> str:
 		return self.html if self.html and len(self.html) > 0 else self.plain
 
 	@property
@@ -424,17 +415,15 @@
 		return None
 
 	@property
 	def message_id(self)-> Union[str, None]:
 		if not self.message_headers:
 			return None
 		for header in self.message_headers:
-			if header.name == "Message-ID":
-				return header.value
-			if header.name == "Message-Id":
+			if header.name.casefold() == "message-id":
 				return header.value
 		return None
 
 	@property
 	def subject(self)-> Union[str, None]:
 		if not self.message_headers:
 			return None
```

### Comparing `fast_gmail-1.0.4/fast_gmail/search.py` & `fast_gmail-1.0.5/fast_gmail/search.py`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.4/fast_gmail.egg-info/PKG-INFO` & `fast_gmail-1.0.5/fast_gmail.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_gmail
-Version: 1.0.4
+Version: 1.0.5
 Summary: GmailApi wrapper
 Home-page: https://github.com/aleti1/fast_gmail
 Author: Aleti
 Author-email: aleti.open.source@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -18,16 +18,14 @@
 Requires-Dist: google-api-python-client==2.125.0
 Requires-Dist: google-auth-httplib2==0.2.0
 Requires-Dist: google-auth-oauthlib==1.2.0
 Requires-Dist: typing-extensions==4.11.0
 
 # Fast-gmail a simple python wrapper for gmailapi
 
-[![PyPI](https://img.shields.io/pypi/v/fast-gmail)](https://pypi.org/project/fast-gmail/)
-
 ---
 ## Functionalities:
 - Send text/html messages
 - Send messages with signature & attachments
 - Get messages with pagination
 - Filter messages
 - Get drafts
@@ -42,24 +40,23 @@
 
 ## Usage:
 
 ### Initialization
 - Go to https://console.developers.google.com/apis/credentials and login to correct account
 - Setup Oauth consent screen
 - Create new credentials with OAuth client ID for web or installed app
-- Set Authorized Javascript origins to http://localhost:3000/
-- Set Authorized redirect URIs to http://localhost:3000/
+- Set Authorized redirect URIs to http://localhost:3000/ (Notice the trailing slash)
 - Download the credentials.json file
 - Go to Enable APIs & services and enable GmailAPI
 
 With credentials.json file downloaded we can connect to Gmail
 ```
 gmail = GmailApi(
-    credentials_file_path = __path_to_credentials_json_file__,
-    port = 3000, # default is 3000 but you can use any other port IMPORTANT: if you change this default value don't forget to also changed on Authorized Javascript origins & Authorized redirect URIs
+    credentials_file_path = __path_to_credentials_json_file__,  # Defaults to ./credentials.json
+    port = 3000, # Defaults to 3000  !IMPORTANT: if you change this default value don't forget to also changed on Authorized redirect URIs
 )
 ```
 
 ### Send message
 ``` 
     from fast_gmail import GmailApi
 
@@ -68,26 +65,28 @@
         to: str,
         subject: str,
         html: Optional[str]=None,
         text: Optional[str]=None,
         cc: Optional[List[str] | str]=None,
         bcc: Optional[List[str] | str]=None,
         attachments: Optional[List[str] | str]=None,
+		in_reply_to: Optional[str] = None,
         signature: bool = True
     )
     """Sends an email message.
         Args:
             sender (str): Email address of the message sender.
             to (str): Email address of the recipient.
             subject (str): Subject line of the email.
             html (Optional[str], optional): HTML content of the email body. Defaults to None.
             text (Optional[str], optional): Plain text content of the email body. Defaults to None.
             cc (Optional[List[str] | str], optional): List of email addresses to carbon copy. Defaults to None.
             bcc (Optional[List[str] | str], optional): List of email addresses to blind carbon copy. Defaults to None.
             attachments (Optional[List[str] | str], optional): List of file paths to attach to the email. Defaults to None.
+            in_reply_to (Optional[str], optional): Message.message_id value that is replyed to. Defaults to None.
             signature (bool, optional): Whether to include a signature (if configured). Defaults to True.
         Returns:
             Optional[Message]: An object representing the sent message, or None on error.
     """
 ```
 
 ### Get messages
```

### Comparing `fast_gmail-1.0.4/setup.py` & `fast_gmail-1.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from setuptools import find_packages
 
 with open("README.md", "r") as f:
     long_descrition=f.read()
 
 setup(
     name="fast_gmail",
-    version="1.0.4",
+    version="1.0.5",
     description="GmailApi wrapper",
-    long_description=long_descrition,  # Load description from README
+    long_description=long_descrition,
     long_description_content_type='text/markdown',
     author="Aleti",
     author_email="aleti.open.source@gmail.com",
     url="https://github.com/aleti1/fast_gmail",
     license="MIT",
     include_package_data=True,
     python_requires=">=3.10",
@@ -26,8 +26,9 @@
         'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
+    packages=find_packages(exclude=("examples",))
 )
```

