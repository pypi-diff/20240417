# Comparing `tmp/wristwatch-1.1.0.tar.gz` & `tmp/wristwatch-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wristwatch-1.1.0.tar", last modified: Sun Apr 14 08:54:26 2024, max compression
+gzip compressed data, was "wristwatch-1.2.0.tar", last modified: Wed Apr 17 16:39:32 2024, max compression
```

## Comparing `wristwatch-1.1.0.tar` & `wristwatch-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-14 08:54:26.865802 wristwatch-1.1.0/
--rwxrwxrwx   0 zwolfrost  (1000) zwolfrost  (1000)     1086 2022-12-24 08:05:26.000000 wristwatch-1.1.0/LICENSE
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)     2867 2024-04-14 08:54:26.865802 wristwatch-1.1.0/PKG-INFO
--rwxrwxrwx   0 zwolfrost  (1000) zwolfrost  (1000)     2649 2024-04-14 08:53:35.000000 wristwatch-1.1.0/README.md
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       38 2024-04-14 08:54:26.865802 wristwatch-1.1.0/setup.cfg
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)      546 2024-04-14 08:24:21.000000 wristwatch-1.1.0/setup.py
-drwxrwxr-x   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-14 08:54:26.865802 wristwatch-1.1.0/wristwatch/
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-13 17:46:48.000000 wristwatch-1.1.0/wristwatch/__init__.py
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)     8283 2024-04-14 08:32:37.000000 wristwatch-1.1.0/wristwatch/wristwatch.py
-drwxrwxr-x   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-14 08:54:26.865802 wristwatch-1.1.0/wristwatch.egg-info/
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)     2867 2024-04-14 08:54:26.000000 wristwatch-1.1.0/wristwatch.egg-info/PKG-INFO
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)      280 2024-04-14 08:54:26.000000 wristwatch-1.1.0/wristwatch.egg-info/SOURCES.txt
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)        1 2024-04-14 08:54:26.000000 wristwatch-1.1.0/wristwatch.egg-info/dependency_links.txt
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       59 2024-04-14 08:54:26.000000 wristwatch-1.1.0/wristwatch.egg-info/entry_points.txt
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       69 2024-04-14 08:54:26.000000 wristwatch-1.1.0/wristwatch.egg-info/requires.txt
--rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       11 2024-04-14 08:54:26.000000 wristwatch-1.1.0/wristwatch.egg-info/top_level.txt
+drwxrwxr-x   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-17 16:39:32.340575 wristwatch-1.2.0/
+-rwxrwxrwx   0 zwolfrost  (1000) zwolfrost  (1000)     1086 2022-12-24 08:05:26.000000 wristwatch-1.2.0/LICENSE
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)     3294 2024-04-17 16:39:32.336575 wristwatch-1.2.0/PKG-INFO
+-rwxrwxrwx   0 zwolfrost  (1000) zwolfrost  (1000)     3081 2024-04-17 16:39:26.000000 wristwatch-1.2.0/README.md
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       38 2024-04-17 16:39:32.340575 wristwatch-1.2.0/setup.cfg
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)      554 2024-04-17 16:26:06.000000 wristwatch-1.2.0/setup.py
+drwxrwxr-x   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-17 16:39:32.336575 wristwatch-1.2.0/wristwatch/
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       36 2024-04-17 16:36:04.000000 wristwatch-1.2.0/wristwatch/__init__.py
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)     9213 2024-04-17 16:33:46.000000 wristwatch-1.2.0/wristwatch/wristwatch.py
+drwxrwxr-x   0 zwolfrost  (1000) zwolfrost  (1000)        0 2024-04-17 16:39:32.336575 wristwatch-1.2.0/wristwatch.egg-info/
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)     3294 2024-04-17 16:39:32.000000 wristwatch-1.2.0/wristwatch.egg-info/PKG-INFO
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)      280 2024-04-17 16:39:32.000000 wristwatch-1.2.0/wristwatch.egg-info/SOURCES.txt
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)        1 2024-04-17 16:39:32.000000 wristwatch-1.2.0/wristwatch.egg-info/dependency_links.txt
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       59 2024-04-17 16:39:32.000000 wristwatch-1.2.0/wristwatch.egg-info/entry_points.txt
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       77 2024-04-17 16:39:32.000000 wristwatch-1.2.0/wristwatch.egg-info/requires.txt
+-rw-rw-r--   0 zwolfrost  (1000) zwolfrost  (1000)       11 2024-04-17 16:39:32.000000 wristwatch-1.2.0/wristwatch.egg-info/top_level.txt
```

### Comparing `wristwatch-1.1.0/LICENSE` & `wristwatch-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wristwatch-1.1.0/PKG-INFO` & `wristwatch-1.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 Metadata-Version: 2.1
 Name: wristwatch
-Version: 1.1.0
+Version: 1.2.0
 Summary: Yet another Python watcher for website updates.
 Home-page: https://github.com/zWolfrost/wristwatch
 Author: zWolfrost
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wristwatch
-![PyPI version](https://img.shields.io/pypi/v/wristwatch)
-![PyPI downloads](https://img.shields.io/pypi/dm/wristwatch)
-![GitHub license](https://img.shields.io/github/license/zWolfrost/wristwatch)
+[![PyPI version](https://img.shields.io/pypi/v/wristwatch)](https://pypi.org/project/wristwatch/)
+[![PyPI downloads](https://img.shields.io/pypi/dm/wristwatch)](https://pypi.org/project/wristwatch/)
+[![GitHub license](https://img.shields.io/github/license/zWolfrost/wristwatch)](LICENSE)
 
 Yet another Python watcher for website updates.
 
 &nbsp;
 ## Features
 - Selecting elements to watch with CSS selectors.
-- Importing Cookies from any browser (to scrape webpages that require authentication).
+- Automatic importing of cookies from many browsers.
 - Emailing the changes to yourself.
-- Other minor features...
+- Other features...
 
 You can safely quit watching at any time by pressing `Ctrl+C`.
 
 &nbsp;
 ## Installation
 After having installed [Python 3](https://www.python.org/downloads/) with pip, you can install wristwatch using the following command:
 ```bash
 pip install wristwatch
 ```
 
 &nbsp;
 ## Arguments
-| Command     | Shorthand | Example                  | Description
-|:-:          |:-:        | :-:                      |:-
-|             |           | `https://example.com/`   | The URL of the webpage to scrape.
-| --browser   | -b        | `-b chrome`              | Name of the browser to get cookies from (default: any).
-| --frequency | -f        | `-f 60`                  | Frequency of fetches in seconds (default: 60).
-| --selector  | -s        | `-s #minutes -s #hours`  | CSS selector of element(s) to scrape. Can be used multiple times.
-| --email     | -e        | `-e example@gmail.com`   | Email address to self-send the changes to.
-| --password  | -p        | `-p aaaa bbbb cccc dddd` | Email "app" password. Here's a guide on how to generate one: https://support.google.com/accounts/answer/185833
-| --quiet     | -q        | `-q`                     | Decrease output verbosity.
-| --loop      | -l        | `-l`                     | Keep watching for changes even after the first one.
-| --output    | -o        | `-o output.txt`          | Save the last fetch to a file.
-| --input     | -i        | `-i input.txt`           | Load the first fetch from a file.
-| --alert     | -a        | `-a`                     | Play a sound when changes are detected.
-| --version   | -v        | `-v`                     | Show the program's version.
+| Command       | Shorthand | Example                  | Description
+|:-:            |:-:        | :-:                      |:-
+|               |           | `https://example.com/`   | The URL of the webpage to scrape.
+| `--browser`   | `-b`      | `-b chrome`              | Name of the browser to get cookies from (by default, any browser possible). See `--help` for supported browsers.
+| `--frequency` | `-f`      | `-f 60`                  | Frequency of fetches in seconds (default: 60).
+| `--selector`  | `-s`      | `-s #minutes -s #hours`  | CSS selector of element(s) to scrape. Can be used multiple times.
+| `--email`     | `-e`      | `-e example@gmail.com`   | Email address to self-send the changes to.
+| `--password`  | `-p`      | `-p aaaa bbbb cccc dddd` | Email "app" password. [Here's a guide on how to generate one](https://support.google.com/accounts/answer/185833#app-passwords).
+| `--quiet`     | `-q`      | `-q`                     | Decrease output verbosity.
+| `--loop`      | `-l`      | `-l`                     | Keep watching for changes even after the first one.
+| `--output`    | `-o`      | `-o output.txt`          | Save the last fetch to a file.
+| `--input`     | `-i`      | `-i input.txt`           | Load the first fetch from a file.
+| `--alert`     | `-a`      | `-a`                     | Play a sound when changes are detected.
+| `--version`   | `-v`      | `-v`                     | Show the program's version.
+| `--help`      | `-h`      | `-h`                     | Show the help message on how to use the program.
 
 &nbsp;
 ## Examples
 ```bash
 wristwatch "https://relaxingclock.com" -s "#minutes" -f 5 -a -l
 ```
 
@@ -68,8 +69,12 @@
 <br>- Initial release.
 	- 1.0.1
 	<br>-Specified dependencies version requirements
 	- 1.0.2
 	<br>-Fixed `--loop` argument not working
 - **1.1.0**:
 <br>- Added `--alert` argument to play a sound when changes are detected.
+- **1.2.0**:
+<br>- Added `--debug` argument to show debug info & error messages.
+<br>- Changed "rookiepy" dependency for "browser-cookie3"
+<br>- Better error handling.
```

### Comparing `wristwatch-1.1.0/README.md` & `wristwatch-1.2.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 # wristwatch
-![PyPI version](https://img.shields.io/pypi/v/wristwatch)
-![PyPI downloads](https://img.shields.io/pypi/dm/wristwatch)
-![GitHub license](https://img.shields.io/github/license/zWolfrost/wristwatch)
+[![PyPI version](https://img.shields.io/pypi/v/wristwatch)](https://pypi.org/project/wristwatch/)
+[![PyPI downloads](https://img.shields.io/pypi/dm/wristwatch)](https://pypi.org/project/wristwatch/)
+[![GitHub license](https://img.shields.io/github/license/zWolfrost/wristwatch)](LICENSE)
 
 Yet another Python watcher for website updates.
 
 &nbsp;
 ## Features
 - Selecting elements to watch with CSS selectors.
-- Importing Cookies from any browser (to scrape webpages that require authentication).
+- Automatic importing of cookies from many browsers.
 - Emailing the changes to yourself.
-- Other minor features...
+- Other features...
 
 You can safely quit watching at any time by pressing `Ctrl+C`.
 
 &nbsp;
 ## Installation
 After having installed [Python 3](https://www.python.org/downloads/) with pip, you can install wristwatch using the following command:
 ```bash
 pip install wristwatch
 ```
 
 &nbsp;
 ## Arguments
-| Command     | Shorthand | Example                  | Description
-|:-:          |:-:        | :-:                      |:-
-|             |           | `https://example.com/`   | The URL of the webpage to scrape.
-| --browser   | -b        | `-b chrome`              | Name of the browser to get cookies from (default: any).
-| --frequency | -f        | `-f 60`                  | Frequency of fetches in seconds (default: 60).
-| --selector  | -s        | `-s #minutes -s #hours`  | CSS selector of element(s) to scrape. Can be used multiple times.
-| --email     | -e        | `-e example@gmail.com`   | Email address to self-send the changes to.
-| --password  | -p        | `-p aaaa bbbb cccc dddd` | Email "app" password. Here's a guide on how to generate one: https://support.google.com/accounts/answer/185833
-| --quiet     | -q        | `-q`                     | Decrease output verbosity.
-| --loop      | -l        | `-l`                     | Keep watching for changes even after the first one.
-| --output    | -o        | `-o output.txt`          | Save the last fetch to a file.
-| --input     | -i        | `-i input.txt`           | Load the first fetch from a file.
-| --alert     | -a        | `-a`                     | Play a sound when changes are detected.
-| --version   | -v        | `-v`                     | Show the program's version.
+| Command       | Shorthand | Example                  | Description
+|:-:            |:-:        | :-:                      |:-
+|               |           | `https://example.com/`   | The URL of the webpage to scrape.
+| `--browser`   | `-b`      | `-b chrome`              | Name of the browser to get cookies from (by default, any browser possible). See `--help` for supported browsers.
+| `--frequency` | `-f`      | `-f 60`                  | Frequency of fetches in seconds (default: 60).
+| `--selector`  | `-s`      | `-s #minutes -s #hours`  | CSS selector of element(s) to scrape. Can be used multiple times.
+| `--email`     | `-e`      | `-e example@gmail.com`   | Email address to self-send the changes to.
+| `--password`  | `-p`      | `-p aaaa bbbb cccc dddd` | Email "app" password. [Here's a guide on how to generate one](https://support.google.com/accounts/answer/185833#app-passwords).
+| `--quiet`     | `-q`      | `-q`                     | Decrease output verbosity.
+| `--loop`      | `-l`      | `-l`                     | Keep watching for changes even after the first one.
+| `--output`    | `-o`      | `-o output.txt`          | Save the last fetch to a file.
+| `--input`     | `-i`      | `-i input.txt`           | Load the first fetch from a file.
+| `--alert`     | `-a`      | `-a`                     | Play a sound when changes are detected.
+| `--version`   | `-v`      | `-v`                     | Show the program's version.
+| `--help`      | `-h`      | `-h`                     | Show the help message on how to use the program.
 
 &nbsp;
 ## Examples
 ```bash
 wristwatch "https://relaxingclock.com" -s "#minutes" -f 5 -a -l
 ```
 
@@ -56,8 +57,12 @@
 - **1.0.0**:
 <br>- Initial release.
 	- 1.0.1
 	<br>-Specified dependencies version requirements
 	- 1.0.2
 	<br>-Fixed `--loop` argument not working
 - **1.1.0**:
-<br>- Added `--alert` argument to play a sound when changes are detected.
+<br>- Added `--alert` argument to play a sound when changes are detected.
+- **1.2.0**:
+<br>- Added `--debug` argument to show debug info & error messages.
+<br>- Changed "rookiepy" dependency for "browser-cookie3"
+<br>- Better error handling.
```

### Comparing `wristwatch-1.1.0/wristwatch/wristwatch.py` & `wristwatch-1.2.0/wristwatch/wristwatch.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,89 @@
 #! venv/bin/python 
 
-import time, os, sys, argparse, difflib, rookiepy, chime
+import time, os, sys, argparse, difflib
 from urllib.parse import urlparse
 
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver import Chrome
-from selenium.common.exceptions import InvalidArgumentException, WebDriverException
-
 from bs4 import BeautifulSoup
 from bs4.formatter import HTMLFormatter
+import browser_cookie3, chime
 
 import smtplib, ssl
 from email.message import EmailMessage
 
 
-def get_args():
-	parser = argparse.ArgumentParser(description="Yet another Python watcher for website updates.", prog="wristwatch")
+debug_mode = False
+
+
+
+def get_args() -> dict:
+	parser = argparse.ArgumentParser(prog="wristwatch", description="Yet another Python watcher for website updates.")
 
 	parser.add_argument("webpage", type=str, help="The URL of the webpage to scrape.", metavar="URL")
 
-	parser.add_argument("-b", "--browser", type=str, help="Name of the browser to get cookies from (default: any).", default="load", choices=["brave", "chrome", "chromium", "edge", "firefox", "internet_explorer", "librewolf", "octo_browser", "opera", "opera_gx", "safari", "vivaldi"])
+	parser.add_argument("-b", "--browser", type=str, help="Name of the browser to get cookies from (by default, any browser possible).", default="load", choices=["brave", "chrome", "chromium", "edge", "firefox", "librewolf", "opera", "opera_gx", "safari", "vivaldi"])
 	parser.add_argument("-f", "--frequency", type=int, help="Frequency of fetches in seconds (default: 60).", default=60, metavar="SECONDS")
 	parser.add_argument("-s", "--selector", type=str, help="CSS selector of element(s) to scrape. Can be used multiple times.", action="extend", nargs="+")
 
 	parser.add_argument("-e", "--email", type=str, help="Email address to self-send the changes to.", required=("-p" in sys.argv or "--password" in sys.argv))
 	parser.add_argument("-p", "--password", type=str, help="Email \"app\" password. Here's a guide on how to generate one: https://support.google.com/accounts/answer/185833", required=("-e" in sys.argv or "--email" in sys.argv))
 
 	parser.add_argument("-q", "--quiet", help="Decrease output verbosity.", action="store_true")
 	parser.add_argument("-l", "--loop", help="Keep watching for changes even after the first one.", action="store_true")
 
 	parser.add_argument("-o", "--output", type=str, help="Save the last fetch to a file.", metavar="FILE")
 	parser.add_argument("-i", "--input", type=str, help="Load the first fetch from a file.", metavar="FILE")
 
 	parser.add_argument("-a", "--alert", help="Play a sound when changes are detected.", action="store_true")
 
-	parser.add_argument("-v", "--version", action="version", version="%(prog)s 1.1.0")
+	parser.add_argument("-v", "--version", action="version", version="%(prog)s 1.2.0")
+	parser.add_argument("-d", "--debug", help="Enable debug mode.", action="store_true")
 
 	return vars(parser.parse_args())
 
 
-def init_driver():
-	options = Options()
-
-	options.add_argument("--headless=new")
-	options.add_argument("--no-sandbox")
-	options.add_argument("--disable-dev-shm-usage")
-	options.add_argument("--disable-gpu")
-	options.add_argument("--start-maximized")
-	options.add_argument("--ignore-certificate-errors")
-
-	# options.add_argument("--disable-infobars")
-	# options.add_argument("--disable-notifications")
-
-	# options.add_experimental_option("excludeSwitches", ["enable-logging"])
+def cookie_to_dict(cookie) -> dict:
+	cookie_dict = {
+		"name": getattr(cookie, "name", None),
+		"value": getattr(cookie, "value", None),
+		"path": getattr(cookie, "path", None),
+		"domain": getattr(cookie, "domain", None),
+
+		"secure": getattr(cookie, "secure", None) is True,
+		"httpOnly": "HTTPOnly" in getattr(cookie, "_rest", None),
+		"expiry": getattr(cookie, "expires", None),
+
+		# "sameSite" value not available in browser_cookie3
+	}
 
-	driver = Chrome(options=options)
+	if (debug_mode):
+		print(vars(cookie), "\n------------\n", cookie_dict, "\n")
 
-	return driver
+	return cookie_dict
 
-def add_cookies(driver: Chrome, cookies: list = None):
+def add_cookies(driver: Chrome, cookies: list = None) -> int:
 	if (cookies is None):
 		return None
 	else:
 		errorCookies = 0
 
-		for cookie in cookies:
+		for (i, cookie) in enumerate(cookies):
 			try:
 				driver.add_cookie(cookie)
-			except Exception:
+			except BaseException as e:
+				if (debug_mode):
+					print(f"COOKIE NO. {i + 1}")
+					print(e)
 				errorCookies += 1
 
 		return len(cookies) - errorCookies
 
-def fetch_driver(driver: Chrome, selectors: str = None):
+def fetch_driver(driver: Chrome, selectors: str = None) -> str:
 	formatter = HTMLFormatter(indent=3)
 	soup = BeautifulSoup(driver.page_source, "html.parser")
 
 	if (selectors is None):
 		return str(soup.prettify(formatter=formatter))
 	else:
 		fetch = ""
@@ -86,36 +93,19 @@
 				fetch += str(element.prettify(formatter=formatter))
 				if (i < len(soup.select(selector)) - 1):
 					fetch += "\n"
 
 		return fetch
 
 
-def send_email(from_email: str, to_email: str, password: str, subject="", body="", attachments=[]):
-	msg = EmailMessage()
-	msg["From"] = from_email
-	msg["To"] = to_email
-	msg["Subject"] = subject
-	msg.set_content(body)
-
-	for attachment in attachments:
-		with open(attachment, "rb") as f:
-			attachment_data = f.read()
-			attachment_name = os.path.basename(attachment)
-
-		msg.add_attachment(attachment_data, maintype="application", subtype="octet-stream", filename=attachment_name)
-
-	context = ssl.create_default_context()
-
-	with smtplib.SMTP_SSL("smtp.gmail.com", 465, context=context) as smtp:
-		smtp.login(from_email, password)
-		smtp.sendmail(from_email, to_email, msg.as_string())
-
-
 def print_text(text: str, line_numbers: bool = False, prefix: str = ""):
+	if (text == ""):
+		print("<empty>")
+		return
+
 	try:
 		max_length = os.get_terminal_size().columns
 	except:
 		max_length = None
 
 	break_line = "..."
 	padding = len(str(len(text.splitlines())))
@@ -133,50 +123,91 @@
 	padding = len(string.format(seconds))
 	for i in range(seconds, 0, -1):
 		print("\r" + (string.format(i)).ljust(padding), end="")
 		time.sleep(1)
 	print("\r" + " " * padding + "\r", end="")
 
 
+def send_email(from_email: str, to_email: str, password: str, subject="", body="", attachments=[]):
+	msg = EmailMessage()
+	msg["From"] = from_email
+	msg["To"] = to_email
+	msg["Subject"] = subject
+	msg.set_content(body)
+
+	for attachment in attachments:
+		with open(attachment, "rb") as f:
+			attachment_data = f.read()
+			attachment_name = os.path.basename(attachment)
+
+		msg.add_attachment(attachment_data, maintype="application", subtype="octet-stream", filename=attachment_name)
+
+	context = ssl.create_default_context()
+
+	with smtplib.SMTP_SSL("smtp.gmail.com", 465, context=context) as smtp:
+		smtp.login(from_email, password)
+		smtp.sendmail(from_email, to_email, msg.as_string())
+
+
 
 def main():
 	####
 	## Parse arguments and initialize driver
 	####
 
 	chime.theme("material")
 
 	ARGS = get_args()
 	DOMAIN = urlparse(ARGS["webpage"]).netloc
 
+	if (ARGS["debug"]):
+		global debug_mode
+		debug_mode = True
+		print("Debug mode enabled.")
+
+	if (debug_mode):
+		print(ARGS)
+
+	options = Options()
+	options.add_argument("--headless=new")
+	options.add_argument("--no-sandbox")
+	options.add_argument("--disable-dev-shm-usage")
+	options.add_argument("--disable-gpu")
+	options.add_argument("--ignore-certificate-errors")
+
+	driver = Chrome(options=options)
+
 	try:
-		driver = init_driver()
+		####
+		## Load the webpage
+		####
 
 		try:
 			driver.get(ARGS["webpage"])
-		except (InvalidArgumentException, WebDriverException):
-			print("Webpage URL is invalid. Please retry.")
+		except:
+			print("Failed to load the webpage. Please check the URL and ensure that your internet connection is working.")
 			sys.exit()
 
 
 
 		####
 		## Get cookies and apply them
 		####
 
 		try:
-			cookies = getattr(rookiepy, ARGS["browser"])([DOMAIN])
+			cookies = getattr(browser_cookie3, ARGS["browser"])(domain_name=DOMAIN)
+			cookies = [cookie_to_dict(cookie) for cookie in cookies]
 
 			if (cookies):
 				addedCookies = add_cookies(driver, cookies)
 				print(f"Successfully added {addedCookies} cookies of {len(cookies)} found for \"{DOMAIN}\"")
 			else:
 				print(f"No cookies found for \"{DOMAIN}\"")
-		except:
-			print(f"\"{ARGS['browser']}\" browser not found.")
+		except browser_cookie3.BrowserCookieError:
+			print(f"\"{ARGS['browser'].capitalize()}\" browser not found. No cookies were loaded.")
 
 
 
 		####
 		## Make first Fetch
 		####
 
@@ -214,15 +245,15 @@
 		if (not ARGS["quiet"]):
 			print("Starting to watch. You can safely quit at any time by pressing \"Ctrl+C\".\n")
 
 		fetches = 0
 
 		while True:
 			driver.refresh()
-			print_sleep(f"No changes detected ({fetches} fetches). Waiting {{}} seconds before the next one...", ARGS["frequency"])
+			print_sleep(f"No changes detected ({fetches} fetches). Waiting {{}} seconds before the next fetch...", ARGS["frequency"])
 			print("\rFetching...", end="")
 
 			current_fetch = fetch_driver(driver, ARGS["selector"])
 
 			fetches += 1
 
 			if (first_fetch != current_fetch):
@@ -247,20 +278,20 @@
 
 				if (ARGS["email"]):
 					print(f"Sending email to {ARGS['email']}...")
 					send_email(ARGS["email"], ARGS["email"], ARGS["password"], subject=f"Changes detected on {ARGS['webpage']}", body=diff)
 
 				if (ARGS["loop"]):
 					first_fetch = current_fetch
+					fetches = 0
 				else:
 					break
-	except (KeyboardInterrupt, SystemExit):
-		print(f"Stopped watching.")
-
 
+	except BaseException as e:
+		if (e.__class__ in (KeyboardInterrupt, SystemExit) and not debug_mode):
+			print(f"\nStopped watching.")
+		else:
+			print(f"\n\"{e.__class__.__name__}\" Exception")
 
-	####
-	## Close drivers
-	####
-
-	print(f"Closing drivers...")
-	driver.quit()
+	finally:
+		print(f"Closing drivers...")
+		driver.quit()
```

### Comparing `wristwatch-1.1.0/wristwatch.egg-info/PKG-INFO` & `wristwatch-1.2.0/wristwatch.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 Metadata-Version: 2.1
 Name: wristwatch
-Version: 1.1.0
+Version: 1.2.0
 Summary: Yet another Python watcher for website updates.
 Home-page: https://github.com/zWolfrost/wristwatch
 Author: zWolfrost
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wristwatch
-![PyPI version](https://img.shields.io/pypi/v/wristwatch)
-![PyPI downloads](https://img.shields.io/pypi/dm/wristwatch)
-![GitHub license](https://img.shields.io/github/license/zWolfrost/wristwatch)
+[![PyPI version](https://img.shields.io/pypi/v/wristwatch)](https://pypi.org/project/wristwatch/)
+[![PyPI downloads](https://img.shields.io/pypi/dm/wristwatch)](https://pypi.org/project/wristwatch/)
+[![GitHub license](https://img.shields.io/github/license/zWolfrost/wristwatch)](LICENSE)
 
 Yet another Python watcher for website updates.
 
 &nbsp;
 ## Features
 - Selecting elements to watch with CSS selectors.
-- Importing Cookies from any browser (to scrape webpages that require authentication).
+- Automatic importing of cookies from many browsers.
 - Emailing the changes to yourself.
-- Other minor features...
+- Other features...
 
 You can safely quit watching at any time by pressing `Ctrl+C`.
 
 &nbsp;
 ## Installation
 After having installed [Python 3](https://www.python.org/downloads/) with pip, you can install wristwatch using the following command:
 ```bash
 pip install wristwatch
 ```
 
 &nbsp;
 ## Arguments
-| Command     | Shorthand | Example                  | Description
-|:-:          |:-:        | :-:                      |:-
-|             |           | `https://example.com/`   | The URL of the webpage to scrape.
-| --browser   | -b        | `-b chrome`              | Name of the browser to get cookies from (default: any).
-| --frequency | -f        | `-f 60`                  | Frequency of fetches in seconds (default: 60).
-| --selector  | -s        | `-s #minutes -s #hours`  | CSS selector of element(s) to scrape. Can be used multiple times.
-| --email     | -e        | `-e example@gmail.com`   | Email address to self-send the changes to.
-| --password  | -p        | `-p aaaa bbbb cccc dddd` | Email "app" password. Here's a guide on how to generate one: https://support.google.com/accounts/answer/185833
-| --quiet     | -q        | `-q`                     | Decrease output verbosity.
-| --loop      | -l        | `-l`                     | Keep watching for changes even after the first one.
-| --output    | -o        | `-o output.txt`          | Save the last fetch to a file.
-| --input     | -i        | `-i input.txt`           | Load the first fetch from a file.
-| --alert     | -a        | `-a`                     | Play a sound when changes are detected.
-| --version   | -v        | `-v`                     | Show the program's version.
+| Command       | Shorthand | Example                  | Description
+|:-:            |:-:        | :-:                      |:-
+|               |           | `https://example.com/`   | The URL of the webpage to scrape.
+| `--browser`   | `-b`      | `-b chrome`              | Name of the browser to get cookies from (by default, any browser possible). See `--help` for supported browsers.
+| `--frequency` | `-f`      | `-f 60`                  | Frequency of fetches in seconds (default: 60).
+| `--selector`  | `-s`      | `-s #minutes -s #hours`  | CSS selector of element(s) to scrape. Can be used multiple times.
+| `--email`     | `-e`      | `-e example@gmail.com`   | Email address to self-send the changes to.
+| `--password`  | `-p`      | `-p aaaa bbbb cccc dddd` | Email "app" password. [Here's a guide on how to generate one](https://support.google.com/accounts/answer/185833#app-passwords).
+| `--quiet`     | `-q`      | `-q`                     | Decrease output verbosity.
+| `--loop`      | `-l`      | `-l`                     | Keep watching for changes even after the first one.
+| `--output`    | `-o`      | `-o output.txt`          | Save the last fetch to a file.
+| `--input`     | `-i`      | `-i input.txt`           | Load the first fetch from a file.
+| `--alert`     | `-a`      | `-a`                     | Play a sound when changes are detected.
+| `--version`   | `-v`      | `-v`                     | Show the program's version.
+| `--help`      | `-h`      | `-h`                     | Show the help message on how to use the program.
 
 &nbsp;
 ## Examples
 ```bash
 wristwatch "https://relaxingclock.com" -s "#minutes" -f 5 -a -l
 ```
 
@@ -68,8 +69,12 @@
 <br>- Initial release.
 	- 1.0.1
 	<br>-Specified dependencies version requirements
 	- 1.0.2
 	<br>-Fixed `--loop` argument not working
 - **1.1.0**:
 <br>- Added `--alert` argument to play a sound when changes are detected.
+- **1.2.0**:
+<br>- Added `--debug` argument to show debug info & error messages.
+<br>- Changed "rookiepy" dependency for "browser-cookie3"
+<br>- Better error handling.
```

