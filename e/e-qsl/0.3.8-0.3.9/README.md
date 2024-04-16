# Comparing `tmp/e-qsl-0.3.8.tar.gz` & `tmp/e_qsl-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-qsl-0.3.8.tar", last modified: Sun Feb 25 17:35:52 2024, max compression
+gzip compressed data, was "e_qsl-0.3.9.tar", last modified: Tue Apr 16 22:44:51 2024, max compression
```

## Comparing `e-qsl-0.3.8.tar` & `e_qsl-0.3.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-02-25 17:35:52.288226 e-qsl-0.3.8/
--rw-r--r--   0 fred       (501) staff       (20)      112 2024-02-03 16:20:38.000000 e-qsl-0.3.8/.flake8
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-02-25 17:35:52.280108 e-qsl-0.3.8/.github/
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-02-25 17:35:52.282444 e-qsl-0.3.8/.github/workflows/
--rw-r--r--   0 fred       (501) staff       (20)      879 2024-02-16 15:53:11.000000 e-qsl-0.3.8/.github/workflows/main.yaml
--rw-r--r--   0 fred       (501) staff       (20)     1883 2024-02-15 19:07:07.000000 e-qsl-0.3.8/.gitignore
--rw-r--r--   0 fred       (501) staff       (20)      555 2024-02-23 00:56:04.000000 e-qsl-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0 fred       (501) staff       (20)     1498 2024-02-15 17:20:40.000000 e-qsl-0.3.8/LICENSE
--rw-r--r--   0 fred       (501) staff       (20)     3134 2024-02-25 17:35:52.288044 e-qsl-0.3.8/PKG-INFO
--rw-r--r--   0 fred       (501) staff       (20)      239 2023-03-29 15:20:51.000000 e-qsl-0.3.8/README.md
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-02-25 17:35:52.287579 e-qsl-0.3.8/e_qsl.egg-info/
--rw-r--r--   0 fred       (501) staff       (20)     3134 2024-02-25 17:35:52.000000 e-qsl-0.3.8/e_qsl.egg-info/PKG-INFO
--rw-r--r--   0 fred       (501) staff       (20)      543 2024-02-25 17:35:52.000000 e-qsl-0.3.8/e_qsl.egg-info/SOURCES.txt
--rw-r--r--   0 fred       (501) staff       (20)        1 2024-02-25 17:35:52.000000 e-qsl-0.3.8/e_qsl.egg-info/dependency_links.txt
--rw-r--r--   0 fred       (501) staff       (20)       65 2024-02-25 17:35:52.000000 e-qsl-0.3.8/e_qsl.egg-info/entry_points.txt
--rw-r--r--   0 fred       (501) staff       (20)       81 2024-02-25 17:35:52.000000 e-qsl-0.3.8/e_qsl.egg-info/requires.txt
--rw-r--r--   0 fred       (501) staff       (20)        5 2024-02-25 17:35:52.000000 e-qsl-0.3.8/e_qsl.egg-info/top_level.txt
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-02-25 17:35:52.283729 e-qsl-0.3.8/eqsl/
--rw-r--r--   0 fred       (501) staff       (20)      162 2024-02-15 17:20:40.000000 e-qsl-0.3.8/eqsl/__init__.py
--rwxr-xr-x   0 fred       (501) staff       (20)    13414 2024-02-25 17:31:52.000000 e-qsl-0.3.8/eqsl/_eqsl.py
--rw-r--r--   0 fred       (501) staff       (20)      411 2024-02-25 17:35:52.000000 e-qsl-0.3.8/eqsl/_version.py
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-02-25 17:35:52.283920 e-qsl-0.3.8/eqsl/card/
--rw-r--r--   0 fred       (501) staff       (20)   294889 2024-02-15 17:20:40.000000 e-qsl-0.3.8/eqsl/card/default.jpg
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-02-25 17:35:52.286391 e-qsl-0.3.8/eqsl/fonts/
--rw-r--r--   0 fred       (501) staff       (20)    78296 2024-02-15 17:20:40.000000 e-qsl-0.3.8/eqsl/fonts/DroidSansMono.ttf
--rw-r--r--   0 fred       (501) staff       (20)   183188 2024-02-15 17:20:40.000000 e-qsl-0.3.8/eqsl/fonts/Ubuntu Mono derivative Powerline Bold.ttf
--rwxr-xr-x   0 fred       (501) staff       (20)    54508 2024-02-15 17:20:40.000000 e-qsl-0.3.8/eqsl/fonts/VeraMono-Italic.ttf
--rwxr-xr-x   0 fred       (501) staff       (20)     3053 2024-02-24 15:43:02.000000 e-qsl-0.3.8/eqsl/sendcard.py
--rw-r--r--   0 fred       (501) staff       (20)     3196 2024-02-16 15:53:11.000000 e-qsl-0.3.8/eqsl.yaml.sample
-drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-02-25 17:35:52.286886 e-qsl-0.3.8/misc/
--rw-r--r--   0 fred       (501) staff       (20)   191436 2023-03-10 15:39:28.000000 e-qsl-0.3.8/misc/qsl-example.jpg
--rw-r--r--   0 fred       (501) staff       (20)    20281 2023-10-12 16:52:09.000000 e-qsl-0.3.8/pylintrc
--rw-r--r--   0 fred       (501) staff       (20)     1486 2024-02-16 15:53:11.000000 e-qsl-0.3.8/pyproject.toml
--rw-r--r--   0 fred       (501) staff       (20)       44 2024-02-16 01:28:44.000000 e-qsl-0.3.8/requirements.txt
--rw-r--r--   0 fred       (501) staff       (20)       38 2024-02-25 17:35:52.288264 e-qsl-0.3.8/setup.cfg
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-04-16 22:44:51.859217 e_qsl-0.3.9/
+-rw-r--r--   0 fred       (501) staff       (20)      112 2024-02-03 16:20:38.000000 e_qsl-0.3.9/.flake8
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-04-16 22:44:51.851354 e_qsl-0.3.9/.github/
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-04-16 22:44:51.853728 e_qsl-0.3.9/.github/workflows/
+-rw-r--r--   0 fred       (501) staff       (20)      879 2024-02-16 15:53:11.000000 e_qsl-0.3.9/.github/workflows/main.yaml
+-rw-r--r--   0 fred       (501) staff       (20)     1883 2024-02-15 19:07:07.000000 e_qsl-0.3.9/.gitignore
+-rw-r--r--   0 fred       (501) staff       (20)      555 2024-04-16 21:30:06.000000 e_qsl-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 fred       (501) staff       (20)     1498 2024-02-15 17:20:40.000000 e_qsl-0.3.9/LICENSE
+-rw-r--r--   0 fred       (501) staff       (20)     3134 2024-04-16 22:44:51.859022 e_qsl-0.3.9/PKG-INFO
+-rw-r--r--   0 fred       (501) staff       (20)      239 2023-03-29 15:20:51.000000 e_qsl-0.3.9/README.md
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-04-16 22:44:51.858512 e_qsl-0.3.9/e_qsl.egg-info/
+-rw-r--r--   0 fred       (501) staff       (20)     3134 2024-04-16 22:44:51.000000 e_qsl-0.3.9/e_qsl.egg-info/PKG-INFO
+-rw-r--r--   0 fred       (501) staff       (20)      543 2024-04-16 22:44:51.000000 e_qsl-0.3.9/e_qsl.egg-info/SOURCES.txt
+-rw-r--r--   0 fred       (501) staff       (20)        1 2024-04-16 22:44:51.000000 e_qsl-0.3.9/e_qsl.egg-info/dependency_links.txt
+-rw-r--r--   0 fred       (501) staff       (20)       65 2024-04-16 22:44:51.000000 e_qsl-0.3.9/e_qsl.egg-info/entry_points.txt
+-rw-r--r--   0 fred       (501) staff       (20)       81 2024-04-16 22:44:51.000000 e_qsl-0.3.9/e_qsl.egg-info/requires.txt
+-rw-r--r--   0 fred       (501) staff       (20)        5 2024-04-16 22:44:51.000000 e_qsl-0.3.9/e_qsl.egg-info/top_level.txt
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-04-16 22:44:51.855174 e_qsl-0.3.9/eqsl/
+-rw-r--r--   0 fred       (501) staff       (20)      162 2024-02-15 17:20:40.000000 e_qsl-0.3.9/eqsl/__init__.py
+-rwxr-xr-x   0 fred       (501) staff       (20)    13140 2024-04-16 21:28:24.000000 e_qsl-0.3.9/eqsl/_eqsl.py
+-rw-r--r--   0 fred       (501) staff       (20)      411 2024-04-16 22:44:51.000000 e_qsl-0.3.9/eqsl/_version.py
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-04-16 22:44:51.855389 e_qsl-0.3.9/eqsl/card/
+-rw-r--r--   0 fred       (501) staff       (20)   294889 2024-02-15 17:20:40.000000 e_qsl-0.3.9/eqsl/card/default.jpg
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-04-16 22:44:51.857447 e_qsl-0.3.9/eqsl/fonts/
+-rw-r--r--   0 fred       (501) staff       (20)    78296 2024-02-15 17:20:40.000000 e_qsl-0.3.9/eqsl/fonts/DroidSansMono.ttf
+-rw-r--r--   0 fred       (501) staff       (20)   183188 2024-02-15 17:20:40.000000 e_qsl-0.3.9/eqsl/fonts/Ubuntu Mono derivative Powerline Bold.ttf
+-rwxr-xr-x   0 fred       (501) staff       (20)    54508 2024-02-15 17:20:40.000000 e_qsl-0.3.9/eqsl/fonts/VeraMono-Italic.ttf
+-rwxr-xr-x   0 fred       (501) staff       (20)     2819 2024-04-16 22:33:16.000000 e_qsl-0.3.9/eqsl/sendcard.py
+-rw-r--r--   0 fred       (501) staff       (20)     3196 2024-02-16 15:53:11.000000 e_qsl-0.3.9/eqsl.yaml.sample
+drwxr-xr-x   0 fred       (501) staff       (20)        0 2024-04-16 22:44:51.857904 e_qsl-0.3.9/misc/
+-rw-r--r--   0 fred       (501) staff       (20)   191436 2023-03-10 15:39:28.000000 e_qsl-0.3.9/misc/qsl-example.jpg
+-rw-r--r--   0 fred       (501) staff       (20)    20281 2023-10-12 16:52:09.000000 e_qsl-0.3.9/pylintrc
+-rw-r--r--   0 fred       (501) staff       (20)     1486 2024-02-16 15:53:11.000000 e_qsl-0.3.9/pyproject.toml
+-rw-r--r--   0 fred       (501) staff       (20)       44 2024-02-16 01:28:44.000000 e_qsl-0.3.9/requirements.txt
+-rw-r--r--   0 fred       (501) staff       (20)       38 2024-04-16 22:44:51.859261 e_qsl-0.3.9/setup.cfg
```

### Comparing `e-qsl-0.3.8/.github/workflows/main.yaml` & `e_qsl-0.3.9/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `e-qsl-0.3.8/.gitignore` & `e_qsl-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `e-qsl-0.3.8/.pre-commit-config.yaml` & `e_qsl-0.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `e-qsl-0.3.8/LICENSE` & `e_qsl-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `e-qsl-0.3.8/PKG-INFO` & `e_qsl-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-qsl
-Version: 0.3.8
+Version: 0.3.9
 Summary: Send contacts confirmation cards (QSL Cards).
 Author: Fred C. (W6BSD)
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Fred Cirera
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `e-qsl-0.3.8/e_qsl.egg-info/PKG-INFO` & `e_qsl-0.3.9/e_qsl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-qsl
-Version: 0.3.8
+Version: 0.3.9
 Summary: Send contacts confirmation cards (QSL Cards).
 Author: Fred C. (W6BSD)
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Fred Cirera
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `e-qsl-0.3.8/e_qsl.egg-info/SOURCES.txt` & `e_qsl-0.3.9/e_qsl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `e-qsl-0.3.8/eqsl/_eqsl.py` & `e_qsl-0.3.9/eqsl/_eqsl.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     self.band = qso['BAND']
     self.mode = qso['MODE']
     self.rst_sent = qso.get('RST_SENT', '599')
     self.rst_rcvd = qso.get('RST_RCVD', '599')
     self.tx_pwr = int(qso.get('TX_PWR', 100))
     self.timestamp = qso_timestamp(date_on, time_on)
     self.name = qso.get('NAME', 'Dear OM')
-    self.email = qso.get('EMAIL')
+    self.email = os.getenv('DEBUG_EMAIL', qso.get('EMAIL'))
     if not self.email:
       self.email = self.email_lookup(self.call, cfg)
     self.pota_ref = qso.get('POTA_REF')
     self.sota_ref = qso.get('SOTA_REF')
     self.lang = qso.get('COUNTRY', 'default').lower()
 
   def email_lookup(self, call, cfg):
@@ -136,21 +136,20 @@
   lang = languages.get(qso.lang, 'default')
   if lang != 'default':
     logging.info('Using %s template for %s', lang, qso.lang)
   template = config.mail_templates.get(lang, "default")
   return string.Template(template + '\n' * 3).safe_substitute
 
 
-def send_mail(qso, image, debug_email=None):
+def send_mail(qso, image):
   template = get_template(qso)
-  to_addr = debug_email if debug_email else qso.email
 
   msg = MIMEMultipart()
   msg['From'] = config.smtp_from
-  msg['To'] = to_addr
+  msg['To'] = qso.email
   msg['Date'] = formatdate(localtime=True)
   msg['Subject'] = f"Digital QSL from {qso.my_call} to {qso.call}"
 
   data = asdict(qso)
   data['qso_date'] = datetime.fromtimestamp(qso.timestamp).strftime("%A %B %d, %Y at %X UTC")
 
   msg.attach(MIMEText(template(data)))
@@ -163,15 +162,15 @@
   context = ssl.create_default_context()
   try:
     with smtplib.SMTP(config.smtp_server, config.smtp_port) as server:
       server.ehlo()
       server.starttls(context=context)
       server.ehlo()
       server.login(config.smtp_login, config.smtp_password)
-      server.sendmail(config.smtp_from, to_addr, msg.as_string())
+      server.sendmail(config.smtp_from, qso.email, msg.as_string())
   except ConnectionRefusedError as err:
     logging.error('Connection "%s" error: %s', config.smtp_server, err)
     raise SystemExit("Exit send_mail error") from None
   except (smtplib.SMTPDataError, smtplib.SMTPAuthenticationError) as err:
     logging.error('SMTP "%s": %s', config.smtp_server, err.smtp_error.decode('utf-8'))
     raise SystemExit("Exit send_mail error") from None
 
@@ -227,15 +226,15 @@
 
   textbox.text((NEW_WIDTH-90, vsize-30), '@0x9900', font=font_foot, fill=(0x70, 0x70, 0xa0))
 
   img = Image.alpha_composite(img, overlay)
   img = img.convert("RGB")
 
   if not image_name:
-    image_name = NamedTemporaryFile(prefix='QSL-', suffix='.jpg', delete=False).name
+    image_name = NamedTemporaryFile(prefix=f'EQSL-{qso.call}-', suffix='.jpg', delete=False).name
   img.save(image_name, "JPEG", quality=80, optimize=True, progressive=True)
   if config.show_cards:
     img.show()
   return image_name
 
 
 def qso_timestamp(day, time='0000'):
@@ -296,15 +295,15 @@
 
 
 def move_adif(adif_file):
   src = adif_file.name
   dest, _ = os.path.splitext(src)
   dest = dest + '.old'
   if adif_file.name == dest:
-    logging.warning('The file "%s" cannot be moved', adif_file.name)
+    logging.debug('The file "%s" cannot be moved', adif_file.name)
   else:
     logging.info('Moving "%s" to "%s"', os.path.basename(adif_file.name), os.path.basename(dest))
     move(src, dest)
 
 
 def already_sent(qso):
   key = f'{qso.call}-{qso.band}-{qso.mode}'.upper()
@@ -337,15 +336,14 @@
                             '[Default: %(default)s]'))
   parser.add_argument("-n", "--no-email", action="store_true", default=False,
                       help='Do not send the mail, just generate the card only')
   parser.add_argument("-s", "--show", action="store_true", default=False,
                       help='Show the card')
   parser.add_argument("--resend", action="store_true", default=False,
                       help="Resend already sent QSL")
-  parser.add_argument("--debug-email", help="Email address for debuging")
   parser.add_argument("--version", action="version", version=f'%(prog)s {__version__}')
 
   return parser.parse_args()
 
 
 def main():
   global config  # pylint: disable=global-statement
@@ -355,43 +353,38 @@
   config.show_cards = bool(opts.show)
 
   try:
     qsos_raw, _ = adif_io.read_from_string(opts.adif_file.read())
   except IndexError:
     logging.error('Error reading the ADIF file "%s"', opts.adif_file.name)
     raise SystemExit("Exit with error") from None
+  finally:
+    opts.adif_file.close()
+  if not opts.keep:
+    move_adif(opts.adif_file)
 
-  for _qso in qsos_raw:
+  # Load all the QSOs information.
+  all_qso = []
+  for qso in qsos_raw:
     try:
-      qso = QSOData(_qso, config)
+      all_qso.append(QSOData(qso, config))
     except KeyError as err:
-      logging.error('The ADIF file is missing the key: %s', err)
-      raise SystemExit(f'ADIF missing key: {err}') from None
+      logging.error('Record ignored the ADIF file is missing the key: %s', err)
 
+  # Send cards
+  for qso in all_qso:
+    image_name = card(qso, config.signature)
     if not opts.resend and already_sent(qso):
-      logging.warning('QSL already sent to %s', qso.call)
+      logging.warning('QSL for %s already sent to %s', qso.call, qso.email)
       continue
-
     if not qso.email:
       logging.warning('No email found for %s', qso.call)
       continue
 
-    if not opts.no_email:
-      image_name = card(qso, config.signature)
-      try:
-        send_mail(qso, image_name, opts.debug_email)
-      except smtplib.SMTPRecipientsRefused:
-        logging.warning('Error Recipient "%s" malformed', qso.email)
-      else:
-        logging.info('Mail sent to %s at %s', qso.call,
-                     opts.debug_email if opts.debug_email else qso.email)
-
-    if not opts.keep:
-      os.unlink(image_name)
-
-  opts.adif_file.close()
-  if not opts.keep:
-    move_adif(opts.adif_file)
+    try:
+      send_mail(qso, image_name)
+    except smtplib.SMTPRecipientsRefused:
+      logging.warning('Error Recipient "%s" malformed', qso.email)
 
 
 if __name__ == "__main__":
   main()
```

### Comparing `e-qsl-0.3.8/eqsl/card/default.jpg` & `e_qsl-0.3.9/eqsl/card/default.jpg`

 * *Files identical despite different names*

### Comparing `e-qsl-0.3.8/eqsl/fonts/DroidSansMono.ttf` & `e_qsl-0.3.9/eqsl/fonts/DroidSansMono.ttf`

 * *Files identical despite different names*

### Comparing `e-qsl-0.3.8/eqsl/fonts/Ubuntu Mono derivative Powerline Bold.ttf` & `e_qsl-0.3.9/eqsl/fonts/Ubuntu Mono derivative Powerline Bold.ttf`

 * *Files identical despite different names*

### Comparing `e-qsl-0.3.8/eqsl/fonts/VeraMono-Italic.ttf` & `e_qsl-0.3.9/eqsl/fonts/VeraMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `e-qsl-0.3.8/eqsl.yaml.sample` & `e_qsl-0.3.9/eqsl.yaml.sample`

 * *Files identical despite different names*

### Comparing `e-qsl-0.3.8/misc/qsl-example.jpg` & `e_qsl-0.3.9/misc/qsl-example.jpg`

 * *Files identical despite different names*

### Comparing `e-qsl-0.3.8/pylintrc` & `e_qsl-0.3.9/pylintrc`

 * *Files identical despite different names*

### Comparing `e-qsl-0.3.8/pyproject.toml` & `e_qsl-0.3.9/pyproject.toml`

 * *Files identical despite different names*

