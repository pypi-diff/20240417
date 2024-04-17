# Comparing `tmp/wagtail_resume-2.6.0.tar.gz` & `tmp/wagtail_resume-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_resume-2.6.0.tar", max compression
+gzip compressed data, was "wagtail_resume-2.7.0.tar", max compression
```

## Comparing `wagtail_resume-2.6.0.tar` & `wagtail_resume-2.7.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     1069 2024-02-13 11:39:46.506235 wagtail_resume-2.6.0/LICENSE
--rw-r--r--   0        0        0     3496 2024-02-13 11:39:46.506235 wagtail_resume-2.6.0/README.md
--rw-r--r--   0        0        0     3560 2024-02-13 11:39:46.506235 wagtail_resume-2.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/__init__.py
--rw-r--r--   0        0        0      138 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/apps.py
--rw-r--r--   0        0        0     7326 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/blocks.py
--rw-r--r--   0        0        0     1085 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/locale/sv/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3477 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/migrations/0001_initial.py
--rw-r--r--   0        0        0     1955 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/migrations/0002_auto_20191227_0916.py
--rw-r--r--   0        0        0     3655 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/migrations/0003_auto_20200110_1525.py
--rw-r--r--   0        0        0      467 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/migrations/0004_auto_20200110_1656.py
--rw-r--r--   0        0        0     3843 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/migrations/0005_auto_20200227_1224.py
--rw-r--r--   0        0        0      694 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/migrations/0006_alter_baseresumepage_social_links.py
--rw-r--r--   0        0        0      792 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/migrations/0007_baseresumepage_pdf_generation_visibility.py
--rw-r--r--   0        0        0     4472 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/migrations/0008_auto_20220211_1557.py
--rw-r--r--   0        0        0      953 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/migrations/0009_alter_baseresumepage_pdf_generation_visibility.py
--rw-r--r--   0        0        0    18241 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/migrations/0010_alter_baseresumepage_resume_and_more.py
--rw-r--r--   0        0        0    17599 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/migrations/0011_baseresumepage_about_icon_and_more.py
--rw-r--r--   0        0        0    17734 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/migrations/0012_alter_baseresumepage_resume.py
--rw-r--r--   0        0        0    18655 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/migrations/0013_alter_baseresumepage_resume.py
--rw-r--r--   0        0        0        0 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/migrations/__init__.py
--rw-r--r--   0        0        0     3847 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/models.py
--rw-r--r--   0        0        0        0 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/static/wagtail_resume/css/.gitkeep
--rw-r--r--   0        0        0     2668 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/static/wagtail_resume/css/resume_page.css
--rw-r--r--   0        0        0        0 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/static/wagtail_resume/images/.gitkeep
--rw-r--r--   0        0        0        0 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/static/wagtail_resume/js/.gitkeep
--rw-r--r--   0        0        0      437 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/templates/wagtail_resume/blocks/contributions_block.html
--rw-r--r--   0        0        0     1406 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/templates/wagtail_resume/blocks/education_block.html
--rw-r--r--   0        0        0     1031 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/templates/wagtail_resume/blocks/work_experience_block.html
--rw-r--r--   0        0        0      685 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/templates/wagtail_resume/blocks/writings_block.html
--rw-r--r--   0        0        0      653 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/templates/wagtail_resume/localization_dropdown.html
--rw-r--r--   0        0        0      107 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/templates/wagtail_resume/resume_page.html
--rw-r--r--   0        0        0     2903 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/templates/wagtail_resume/resume_page_body.html
--rw-r--r--   0        0        0      564 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/templates/wagtail_resume/resume_page_head.html
--rw-r--r--   0        0        0        0 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/templatetags/__init__.py
--rw-r--r--   0        0        0      139 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/templatetags/wagtail_resume_extras.py
--rw-r--r--   0        0        0      142 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/urls.py
--rw-r--r--   0        0        0     2075 2024-02-13 11:39:46.510234 wagtail_resume-2.6.0/wagtail_resume/views.py
--rw-r--r--   0        0        0     4955 1970-01-01 00:00:00.000000 wagtail_resume-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-17 20:43:02.110716 wagtail_resume-2.7.0/LICENSE
+-rw-r--r--   0        0        0     3496 2024-04-17 20:43:02.110716 wagtail_resume-2.7.0/README.md
+-rw-r--r--   0        0        0     3729 2024-04-17 20:43:02.110716 wagtail_resume-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/__init__.py
+-rw-r--r--   0        0        0      138 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/apps.py
+-rw-r--r--   0        0        0     7326 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/blocks.py
+-rw-r--r--   0        0        0     1085 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/locale/sv/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3477 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1955 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0002_auto_20191227_0916.py
+-rw-r--r--   0        0        0     3655 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0003_auto_20200110_1525.py
+-rw-r--r--   0        0        0      467 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0004_auto_20200110_1656.py
+-rw-r--r--   0        0        0     3843 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0005_auto_20200227_1224.py
+-rw-r--r--   0        0        0      694 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0006_alter_baseresumepage_social_links.py
+-rw-r--r--   0        0        0      792 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0007_baseresumepage_pdf_generation_visibility.py
+-rw-r--r--   0        0        0     4472 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0008_auto_20220211_1557.py
+-rw-r--r--   0        0        0      953 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0009_alter_baseresumepage_pdf_generation_visibility.py
+-rw-r--r--   0        0        0    18241 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0010_alter_baseresumepage_resume_and_more.py
+-rw-r--r--   0        0        0    17599 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0011_baseresumepage_about_icon_and_more.py
+-rw-r--r--   0        0        0    17734 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0012_alter_baseresumepage_resume.py
+-rw-r--r--   0        0        0    18655 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0013_alter_baseresumepage_resume.py
+-rw-r--r--   0        0        0      535 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0014_baseresumepage_display_last_update.py
+-rw-r--r--   0        0        0        0 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/__init__.py
+-rw-r--r--   0        0        0     4037 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/models.py
+-rw-r--r--   0        0        0        0 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/static/wagtail_resume/css/.gitkeep
+-rw-r--r--   0        0        0     2024 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/static/wagtail_resume/css/resume_page.css
+-rw-r--r--   0        0        0        0 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/static/wagtail_resume/images/.gitkeep
+-rw-r--r--   0        0        0        0 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/static/wagtail_resume/js/.gitkeep
+-rw-r--r--   0        0        0      406 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/blocks/contributions_block.html
+-rw-r--r--   0        0        0     1516 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/blocks/education_block.html
+-rw-r--r--   0        0        0      951 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/blocks/work_experience_block.html
+-rw-r--r--   0        0        0      691 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/blocks/writings_block.html
+-rw-r--r--   0        0        0      653 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/localization_dropdown.html
+-rw-r--r--   0        0        0      107 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/resume_page.html
+-rw-r--r--   0        0        0     2488 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/resume_page_body.html
+-rw-r--r--   0        0        0      564 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/resume_page_head.html
+-rw-r--r--   0        0        0        0 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/templatetags/__init__.py
+-rw-r--r--   0        0        0      139 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/templatetags/wagtail_resume_extras.py
+-rw-r--r--   0        0        0      142 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/urls.py
+-rw-r--r--   0        0        0     2075 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/views.py
+-rw-r--r--   0        0        0     4955 1970-01-01 00:00:00.000000 wagtail_resume-2.7.0/PKG-INFO
```

### Comparing `wagtail_resume-2.6.0/LICENSE` & `wagtail_resume-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.6.0/README.md` & `wagtail_resume-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.6.0/pyproject.toml` & `wagtail_resume-2.7.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
+
 [tool.poetry]
 name = "wagtail-resume"
 authors = ["Adin Hodovic <hodovicadin@gmail.com>"]
 license = "MIT"
-version = "2.6.0"
+version = "2.7.0"
 readme = "README.md"
 homepage = "https://github.com/adinhodovic/wagtail-resume"
 repository = "https://github.com/adinhodovic/wagtail-resume"
 documentation = "https://github.com/adinhodovic/wagtail-resume"
 description = "A Wagtail project made to simplify creation of resumes for developers."
 keywords = ["Resume", "Django", "Wagtail", "CMS"]
 classifiers = [
@@ -54,17 +58,14 @@
 pytest-cov = "^2.8.1"
 pytest-django = "^4.5.2"
 pytest-clarity = "^1.0.1"
 pytest-mock = "^3.0.0"
 djlint = "^1.34.0"
 pudb = "^2022.1.3"
 
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = "--ds=tests.settings --reuse-db --pdbcls=pudb.debugger:Debugger"
 python_files = "tests.py test_*.py"
 norecursedirs = ".git */migrations/* */static/* venv .venv .poetry .virtualenv node_modules"
 
 [tool.black]
@@ -114,13 +115,17 @@
 ignore-comments = "yes"
 # Ignore docstrings when computing similarities.
 ignore-docstrings = "yes"
 # Ignore imports when computing similarities.
 ignore-imports = "yes"
 
 [tool.djlint]
-ignore = "H006,H030,H031"
-profile = "django"
-preserve_blank_lines = true
-use_gitignore = true
+blank_line_after_tag = "load,extends"
+close_void_tags = true
 format_css = true
 format_js = true
+# TODO: remove T002 when fixed https://github.com/Riverside-Healthcare/djLint/issues/687
+ignore = "H006,H030,H031,T002"
+include = "H017,H035"
+indent = 2
+max_line_length = 119
+profile = "django"
```

### Comparing `wagtail_resume-2.6.0/wagtail_resume/blocks.py` & `wagtail_resume-2.7.0/wagtail_resume/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.6.0/wagtail_resume/locale/sv/LC_MESSAGES/django.po` & `wagtail_resume-2.7.0/wagtail_resume/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.6.0/wagtail_resume/migrations/0001_initial.py` & `wagtail_resume-2.7.0/wagtail_resume/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.6.0/wagtail_resume/migrations/0002_auto_20191227_0916.py` & `wagtail_resume-2.7.0/wagtail_resume/migrations/0002_auto_20191227_0916.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.6.0/wagtail_resume/migrations/0003_auto_20200110_1525.py` & `wagtail_resume-2.7.0/wagtail_resume/migrations/0003_auto_20200110_1525.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.6.0/wagtail_resume/migrations/0005_auto_20200227_1224.py` & `wagtail_resume-2.7.0/wagtail_resume/migrations/0005_auto_20200227_1224.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.6.0/wagtail_resume/migrations/0006_alter_baseresumepage_social_links.py` & `wagtail_resume-2.7.0/wagtail_resume/migrations/0006_alter_baseresumepage_social_links.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.6.0/wagtail_resume/migrations/0007_baseresumepage_pdf_generation_visibility.py` & `wagtail_resume-2.7.0/wagtail_resume/migrations/0007_baseresumepage_pdf_generation_visibility.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.6.0/wagtail_resume/migrations/0008_auto_20220211_1557.py` & `wagtail_resume-2.7.0/wagtail_resume/migrations/0008_auto_20220211_1557.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.6.0/wagtail_resume/migrations/0009_alter_baseresumepage_pdf_generation_visibility.py` & `wagtail_resume-2.7.0/wagtail_resume/migrations/0009_alter_baseresumepage_pdf_generation_visibility.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.6.0/wagtail_resume/migrations/0010_alter_baseresumepage_resume_and_more.py` & `wagtail_resume-2.7.0/wagtail_resume/migrations/0010_alter_baseresumepage_resume_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.6.0/wagtail_resume/migrations/0011_baseresumepage_about_icon_and_more.py` & `wagtail_resume-2.7.0/wagtail_resume/migrations/0011_baseresumepage_about_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.6.0/wagtail_resume/migrations/0012_alter_baseresumepage_resume.py` & `wagtail_resume-2.7.0/wagtail_resume/migrations/0012_alter_baseresumepage_resume.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.6.0/wagtail_resume/migrations/0013_alter_baseresumepage_resume.py` & `wagtail_resume-2.7.0/wagtail_resume/migrations/0013_alter_baseresumepage_resume.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.6.0/wagtail_resume/models.py` & `wagtail_resume-2.7.0/wagtail_resume/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,17 @@
         help_text="""
             PDF generation is a heavy blocking operation,
             so it is recommended to only show it to logged in users.
             If available to everyone, ensure that you have multiple workers running.
         """,
         max_length=64,
     )
+    display_last_update = models.BooleanField(
+        default=True, help_text="If enabled, the last update date will be displayed."
+    )
 
     role = models.CharField(max_length=100, null=True, blank=True)
     about = MarkdownField(max_length=2500, null=True, blank=True)
     about_icon = models.CharField(
         max_length=50, default="fas fa-tools", null=True, blank=True
     )
     photo = models.ForeignKey(
@@ -83,14 +86,15 @@
 
     content_panels = Page.content_panels + [
         MultiFieldPanel(
             [
                 FieldPanel("font"),
                 FieldPanel("background_color"),
                 FieldPanel("pdf_generation_visibility"),
+                FieldPanel("display_last_update"),
             ],
             heading="Customization",
         ),
         MultiFieldPanel(
             [
                 FieldPanel("full_name"),
                 FieldPanel("role"),
```

### Comparing `wagtail_resume-2.6.0/wagtail_resume/static/wagtail_resume/css/resume_page.css` & `wagtail_resume-2.7.0/wagtail_resume/static/wagtail_resume/css/resume_page.css`

 * *Files 16% similar despite different names*

```diff
@@ -1,215 +1,179 @@
 body {
   margin: 0;
   color: #212121;
 }
 
 p {
   line-height: 1.5;
-  font-size: 1rem
+  font-size: 1rem;
 }
 
 h2 {
   font-weight: 600;
   font-size: 1.3rem;
 }
 
+h3 {
+  font-weight: 600;
+  font-size: 1rem;
+}
+
 hr {
   border-color: #fdfcfc;
   border-width: 0.1px;
   margin-top: 1rem;
   margin-bottom: 1rem;
 }
 
+.small {
+  font-size: 0.8rem;
+}
+
+.italic {
+  font-style: italic;
+}
+
 .mt-0 {
   margin-top: 0rem;
 }
 
 .mb-0 {
   margin-bottom: 0rem;
 }
 
+.ml-0 {
+  margin-left: 0 !important;
+}
+
 .mt-1 {
   margin-top: 0.25rem;
 }
 
 .mb-1 {
   margin-bottom: 0.25rem;
 }
 
-.name {
+.ml-1 {
+  margin-left: 0.25rem;
+}
+
+.mb-2 {
   margin-bottom: 0.5rem;
-  margin-top: 0;
+}
+
+.mt-2 {
+  margin-top: 0.5rem;
+}
+
+.ml-2 {
+  margin-left: 0.5rem;
+}
+
+.mr-2 {
+  margin-right: 0.5rem;
+}
+
+.mt-3 {
+  margin-top: 1rem;
+}
+
+.mt-4 {
+  margin-top: 2rem;
 }
 
 .container {
   width: 100% !important;
   max-width: 100%;
   margin: 0 auto;
   padding: 0;
   min-height: 100vh;
 }
 
-.work-experience-heading, .contribution-title {
-  font-size: 1.10rem;
-}
-
 .resume {
   box-shadow: 0px 5px 5px 0 rgb(159, 159, 159);
   margin: 0 auto;
   background: #fff;
   min-height: calc(100vh - 4rem);
 }
 
 img {
   max-width: 100%;
   height: auto;
 }
 
 a {
-  color: #4652F6;
+  color: #4652f6;
   text-decoration: none;
   background-color: transparent;
 }
 
-.personal-info {
-  margin-bottom: 0.1rem;
-  margin-top: 0.3rem;
-}
-
-.personal-info > div {
-  display: inline-block;
-}
-
-.personal-info > div:last-of-type {
-  float: right;
-}
-
 .photo {
-  margin-bottom: 3rem;
+  margin-bottom: 2.5rem;
   margin-top: 1rem;
   border-radius: 50%;
   width: 250px;
 }
 
 .social-links img {
-  margin-top: 0.4rem;
-  width: 30px;
+  width: 1.5rem;
 }
 
 .social-links span {
-  margin-left: 0.3rem;
   vertical-align: super;
 }
 
 .date {
   color: #5b5b55;
 }
 
-.text {
-  margin: 2rem 1rem;
-}
-
-.section-title {
-  margin-top: 2rem;
-  margin-bottom: 0rem;
-  align-items: center;
-}
-
-.section-title i {
-  margin-right: 0.6rem;
-}
-
-.post-date {
-  margin-top: 0.2rem;
-}
-
-.post-degree {
-  margin-top: 0.2rem;
-  margin-bottom: 0.2rem;
-}
-
-.contribution-title {
-  margin-bottom: 0.2rem;
-}
-
-.contribution-description {
-  margin: 0.8rem 0;
-}
-
-.section-title .fas, .section-title .fab {
-  font-size: 26px;
+.fas,
+.fab {
+  font-size: 1.5rem;
 }
 
 .pdf {
   display: None;
 }
 
 @media (min-width: 768px) {
-
   .personal-info {
     align-items: center;
     display: flex;
     justify-content: space-between;
   }
 
   .resume {
     padding: 4rem 3rem;
     width: 80%;
   }
 
   .pdf {
     color: white;
-    background: #2A3F76;
+    background: #2a3f76;
     border-radius: 8px;
     display: block;
     font-size: 16px;
     font-weight: 600;
-    padding: .6rem 1.2rem;
+    padding: 0.6rem 1.2rem;
     line-height: 25px;
     float: right;
   }
 }
 
 @media (min-width: 992px) {
-
   .resume {
     padding: 4rem 4rem;
     max-width: 950px;
     width: 60%;
   }
-
 }
 
-
 @media (max-width: 768px) {
-
-  .section-title .fas, .section-title .fab {
-    font-size: 20px;
-  }
-
-  .section-title i {
-    margin-right: 0.4rem;
-  }
-
-  h2 {
-    font-size: 1.6rem;
-  }
-
   .resume {
     padding: 1.5rem;
   }
 
-  .social-links img {
-    margin-top: 0.4rem;
-    width: 22px;
-  }
-
   .photo {
     width: 45%;
-    margin-bottom: 2rem;
   }
 }
-
-.margin-0 {
-  margin-left: 0 !important;
-}
```

### Comparing `wagtail_resume-2.6.0/wagtail_resume/templates/wagtail_resume/blocks/education_block.html` & `wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/blocks/education_block.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 {% load i18n %}
 {% load wagtailcore_tags %}
 
-<h2 class="section-title">
+<h2 class="mt-4 mb-0">
   {% if value.fa_icon %}<i class="{{ value.fa_icon }}"></i>{% endif %}
   <span>{{ value.heading }}</span>
 </h2>
-<hr>
+<hr />
 {% for education in value.educations %}
-{% if education.block_type == "degree" %}
-{% with education.value as degree %}
-<a href="{{ degree.university_url }}"><b>{{ degree.university_name }}</b></a>
-<p class="post-degree"><a href="{{ degree.degree_url }}">{{ degree.degree }}, {{ degree.field_of_study }}</a></p>
-<p class="date post-date">{{ degree.studies_starting_date|date:"Y" }} - {{ degree.studies_ending_date|date:"Y"}}</p>
-{% endwith %}
-{% elif education.block_type == "certificate" %}
-{% with education.value as certificate %}
-<a href="{{ certificate.institute_url }}"><b>{{ certificate.institute_name }}</b> - {% trans "Certificate" %}</a>
-<p class="post-degree"><a href="{{ certificate.certificate_url }}">{{ certificate.name }}</a></p>
-<p class="date post-date">{{ certificate.studies_starting_date|date:"m/Y" }} - {{ certificate.studies_ending_date|date:"m/Y"}}</p>
-{% endwith %}
-{% elif education.block_type == "course" %}
-{% with education.value as course %}
-<a href="{{ course.course_url }}"><b>{{ course.name }}</b> - {% trans "Course" %}</a>
-<p class="date post-date">{{ course.studies_starting_date|date:"m/Y" }} - {{ course.studies_ending_date|date:"m/Y"}}</p>
-{% endwith %}
-{% endif %}
+  {% if education.block_type == "degree" %}
+    {% with education.value as degree %}
+      <a href="{{ degree.university_url }}"><b>{{ degree.university_name }}</b></a>
+      <p class="mt-1 mb-0">
+        <a href="{{ degree.degree_url }}">{{ degree.degree }}, {{ degree.field_of_study }}</a>
+      </p>
+      <p class="date mt-1">{{ degree.studies_starting_date|date:"Y" }} - {{ degree.studies_ending_date|date:"Y" }}</p>
+    {% endwith %}
+  {% elif education.block_type == "certificate" %}
+    {% with education.value as certificate %}
+      <a href="{{ certificate.institute_url }}"><b>{{ certificate.institute_name }}</b> - {% trans "Certificate" %}</a>
+      <p class="mt-1 mb-0">
+        <a href="{{ certificate.certificate_url }}">{{ certificate.name }}</a>
+      </p>
+      <p class="date mt-1">
+        {{ certificate.studies_starting_date|date:"m/Y" }} - {{ certificate.studies_ending_date|date:"m/Y" }}
+      </p>
+    {% endwith %}
+  {% elif education.block_type == "course" %}
+    {% with education.value as course %}
+      <a href="{{ course.course_url }}"><b>{{ course.name }}</b> - {% trans "Course" %}</a>
+      <p class="date mt-1">{{ course.studies_starting_date|date:"m/Y" }} - {{ course.studies_ending_date|date:"m/Y" }}</p>
+    {% endwith %}
+  {% endif %}
 {% endfor %}
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
 {% load i18n %} {% load wagtailcore_tags %}
 {{%% iiff vvaalluuee..ffaa__iiccoonn %%}}{{%% eennddiiff %%}} {{{{ vvaalluuee..hheeaaddiinngg }}}}
 ===============================================================================
 {% for education in value.educations %} {% if education.block_type == "degree"
 %} {% with education.value as degree %} _{{_{{_ _dd_ee_gg_rr_ee_ee_.._uu_nn_ii_vv_ee_rr_ss_ii_tt_yy____nn_aa_mm_ee_ _}}_}}
 _{_{_ _d_e_g_r_e_e_._d_e_g_r_e_e_ _}_}_,_ _{_{_ _d_e_g_r_e_e_._f_i_e_l_d___o_f___s_t_u_d_y_ _}_}
 {{ degree.studies_starting_date|date:"Y" }} - {
-{ degree.studies_ending_date|date:"Y"}}
+{ degree.studies_ending_date|date:"Y" }}
 {% endwith %} {% elif education.block_type == "certificate" %} {% with
 education.value as certificate %} _{{_{{_ _cc_ee_rr_tt_ii_ff_ii_cc_aa_tt_ee_.._ii_nn_ss_tt_ii_tt_uu_tt_ee____nn_aa_mm_ee_ _}}_}}_ _-_ _{_%_ _t_r_a_n_s
 _"_C_e_r_t_i_f_i_c_a_t_e_"_ _%_}
 _{_{_ _c_e_r_t_i_f_i_c_a_t_e_._n_a_m_e_ _}_}
 {{ certificate.studies_starting_date|date:"m/Y" }} - {
-{ certificate.studies_ending_date|date:"m/Y"}}
+{ certificate.studies_ending_date|date:"m/Y" }}
 {% endwith %} {% elif education.block_type == "course" %} {% with
 education.value as course %} _{{_{{_ _cc_oo_uu_rr_ss_ee_.._nn_aa_mm_ee_ _}}_}}_ _-_ _{_%_ _t_r_a_n_s_ _"_C_o_u_r_s_e_"_ _%_}
 {{ course.studies_starting_date|date:"m/Y" }} - {
-{ course.studies_ending_date|date:"m/Y"}}
+{ course.studies_ending_date|date:"m/Y" }}
 {% endwith %} {% endif %} {% endfor %}
```

### Comparing `wagtail_resume-2.6.0/wagtail_resume/templates/wagtail_resume/blocks/work_experience_block.html` & `wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/blocks/work_experience_block.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 {% load i18n %}
 {% load wagtailmarkdown %}
-<h2 class="section-title">
-    {% if value.fa_icon %}<i class="{{ value.fa_icon }}"></i>{% endif %}
-    <span>{{ value.heading }}</span>
+
+<h2 class="mt-4 mb-0">
+  {% if value.fa_icon %}<i class="{{ value.fa_icon }}"></i>{% endif %}
+  <span>{{ value.heading }}</span>
 </h2>
-<hr>
+<hr />
 {% for experience in value.experiences %}
-    <p class="work-experience-heading mb-0">
-        <b>{{ experience.role }} · <a href="{{ experience.url }}">{{ experience.company }}</a></b>
-    </p>
-    {% if experience.location %}<p class="mt-0 mb-0">{{ experience.location }}</p>{% endif %}
-    <p class="date mt-0">
-        {{ experience.from_date }} -
-        {% if experience.currently_working_here %}
-            <b>{% trans "Present" %}</b>
-        {% else %}
-            {{ experience.to_date }}
-        {% endif %}
-    </p>
-    <div style="margin-top: 1.5rem;">{{ experience.text | markdown }}</div>
-    {% if not forloop.last %}<hr>{% endif %}
+  <h3 class="mb-1">
+    {{ experience.role }} · <a href="{{ experience.url }}">{{ experience.company }}</a>
+  </h3>
+  {% if experience.location %}<p class="mt-0 mb-0">{{ experience.location }}</p>{% endif %}
+  <p class="date mt-0">
+    {{ experience.from_date }} -
+    {% if experience.currently_working_here %}
+      <b>{% trans "Present" %}</b>
+    {% else %}
+      {{ experience.to_date }}
+    {% endif %}
+  </p>
+  <div style="margin-top: 1.5rem;">{{ experience.text | markdown }}</div>
+  {% if not forloop.last %}<hr />{% endif %}
 {% endfor %}
 {% if value.maximum_experiences_displayed > 0 %}
-    <p style="margin-top:2rem; font-weight:600; font-style: italic;">{{ value.maximum_experiences_user_text }}</p>
+  <p style="margin-top:2rem; font-weight:600; font-style: italic;">{{ value.maximum_experiences_user_text }}</p>
 {% endif %}
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% load i18n %} {% load wagtailmarkdown %}
 {{%% iiff vvaalluuee..ffaa__iiccoonn %%}}{{%% eennddiiff %%}} {{{{ vvaalluuee..hheeaaddiinngg }}}}
 ===============================================================================
 {% for experience in value.experiences %}
-{{{{ eexxppeerriieennccee..rroollee }}}} ?Â?· _{{_{{_ _ee_xx_pp_ee_rr_ii_ee_nn_cc_ee_.._cc_oo_mm_pp_aa_nn_yy_ _}}_}}
+******** {{{{ eexxppeerriieennccee..rroollee }}}} ?Â?· _{{_{{_ _ee_xx_pp_ee_rr_ii_ee_nn_cc_ee_.._cc_oo_mm_pp_aa_nn_yy_ _}}_}} ********
 {% if experience.location %}
 {{ experience.location }}
 {% endif %}
 {{ experience.from_date }} - {% if experience.currently_working_here %} {{%%
 ttrraannss ""PPrreesseenntt"" %%}} {% else %} {{ experience.to_date }} {% endif %}
 {{ experience.text | markdown }}
 {% if not forloop.last %}
```

### Comparing `wagtail_resume-2.6.0/wagtail_resume/templates/wagtail_resume/blocks/writings_block.html` & `wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/blocks/writings_block.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 {% load wagtailcore_tags %}
 
-<h2 class="section-title">
+<h2 class="mt-4 mb-0">
   {% if value.fa_icon %}<i class="{{ value.fa_icon }}"></i>{% endif %}
   <span>{{ value.heading }}</span>
 </h2>
-<hr>
+<hr />
 {% for post in value.posts %}
-<ul>
-  <li>
-    {% if post.block_type == "external_post" %}
-    <a href="{{ post.value.url }}">{{ post.value.title }}</a>
-    <p class="date post-date">
-      {{ post.value.date }}
-    </p>
-    {% else %}
-    {% with post.value.post as internal_post %}
-    <a href="{{ internal_post.url }}">{{ internal_post.title }}</a>
-    <p class="date post-date">
-      {{ internal_post.first_published_at|date:"M. d, Y" }}
-    </p>
-    {% endwith %}
-    {% endif %}
-  </li>
-</ul>
+  <ul>
+    <li>
+      {% if post.block_type == "external_post" %}
+        <a href="{{ post.value.url }}">{{ post.value.title }}</a>
+        <p class="date mt-1">{{ post.value.date }}</p>
+      {% else %}
+        {% with post.value.post as internal_post %}
+          <a href="{{ internal_post.url }}">{{ internal_post.title }}</a>
+          <p class="date mt-1">{{ internal_post.first_published_at|date:"M. d, Y" }}</p>
+        {% endwith %}
+      {% endif %}
+    </li>
+  </ul>
 {% endfor %}
```

### Comparing `wagtail_resume-2.6.0/wagtail_resume/templates/wagtail_resume/localization_dropdown.html` & `wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/localization_dropdown.html`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.6.0/wagtail_resume/templates/wagtail_resume/resume_page_body.html` & `wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/resume_page_body.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,63 @@
 {% load i18n %}
 {% load static %}
 {% load wagtailimages_tags %}
 {% load wagtailmarkdown %}
 {% load wagtail_resume_extras %}
 
 {% if debug_i18n %}
-{% include 'wagtail_resume/localization_dropdown.html' %}
+  {% include 'wagtail_resume/localization_dropdown.html' %}
 {% endif %}
-
-<!-- beautify ignore:start -->
+{# djlint:off #}
 <!-- We set bg_color within a style tag to only apply bg_color when having a min-width. Weasyprint does not support @media queries
      therefore setting a min-width to 1px ensures that the bg_color does not get applied when generating pdfs. -->
 {% with page.background_color|default_if_none:"#343A40" as bg_color %}
 <style>
-    @media (min-width: 1px) {
-        .container {
-            background-color: {{ bg_color }};
-        }
+  @media (min-width: 1px) {
+    .container {
+      background-color: {{ bg_color }};
     }
+  }
 </style>
 {% endwith %}
-<!-- beautify ignore:end -->
-
-<body style="font-family:{% if page.font %} '{{ page.font|title }}',{% endif %} 'Roboto Condensed', sans-serif;">
-    <div class="container">
-        <div class="resume">
-            <div class="personal-info">
-                <div>
-                    <h2 class="name">{{ page.full_name }}</h2>
-
-                    {% if page.role %}
-                    <h2 class="mt-0 role">{{ page.role }}</h2>
-                    {% endif %}
-
-                    <div class="social-links">
-                        {% for social_link in page.social_links %}
-                        <div class="social-links">
-                            <a class="social-link" href="{{ social_link.value.url }}">
-                                {% if social_link.value.logo %}
-                                {% image social_link.value.logo original %}
-                                <span>{{ social_link.value.text }}</span>
-                                {% else %}
-                                <span class="margin-0">{{ social_link.value.text }}</span>
-                                {% endif %}
-                            </a>
-                        </div>
-                        {% endfor %}
-                    </div>
-                </div>
-                <div>
-                    {% image page.photo original class="photo" %}
-                </div>
-            </div>
-
-            <div>
-              <h2 class="section-title">
-                {% if page.about_icon %}
-                  <i class="{{ page.about_icon }}"></i>
-                {% endif %}
-                <span>{% trans "About" %}</span>
-                </h2>
-                <hr>
-                <p class="about">
-                    {{ page.about | markdown }}
-                </p>
-            </div>
-
-            {% for block in page.resume %}
-            {{ block }}
+{# djlint:on #}
+<body style="font-family:{% if page.font %} '{{ page.font|title }}',{% endif %} 'Roboto Condensed', sans-serif">
+  <div class="container">
+    <div class="resume">
+      <div class="personal-info mt-2 mb-1">
+        <div>
+          <h2 class="mt-2 mb-0">{{ page.full_name }}</h2>
+          {% if page.role %}<h2 class="mt-2">{{ page.role }}</h2>{% endif %}
+          <div class="social-links">
+            {% for social_link in page.social_links %}
+              <div class="social-links">
+                <a class="social-link" href="{{ social_link.value.url }}">
+                  {% if social_link.value.logo %}
+                    {% image social_link.value.logo original class="mt-1" %}
+                    <span class="ml-1">{{ social_link.value.text }}</span>
+                  {% else %}
+                    <span class="ml-0">{{ social_link.value.text }}</span>
+                  {% endif %}
+                </a>
+              </div>
             {% endfor %}
-
-            {% if page.pdf_generation_visibility == "always" or user.is_authenticated and page.pdf_generation_visibility == "authenticated" %}
-            <a class="pdf" href="{% url 'generate_resume_pdf' %}?page_id={{ page.id }}">{% trans "Get PDF" %}</a>
-            {% endif %}
+          </div>
+          <p class="small italic mt-1">Last update: {{ page.latest_revision_created_at|date }}</p>
         </div>
+        <div>{% image page.photo original class="photo" %}</div>
+      </div>
+      <div>
+        <h2 class="mt-4 mb-0">
+          {% if page.about_icon %}<i class="{{ page.about_icon }}"></i>{% endif %}
+          <span>{% trans "About" %}</span>
+        </h2>
+        <hr />
+        <p>{{ page.about | markdown }}</p>
+      </div>
+      {% for block in page.resume %}{{ block }}{% endfor %}
+      {% if page.pdf_generation_visibility == "always" or user.is_authenticated and page.pdf_generation_visibility == "authenticated" %}
+        <a class="pdf"
+           href="{% url 'generate_resume_pdf' %}?page_id={{ page.id }}">{% trans "Get PDF" %}</a>
+      {% endif %}
     </div>
+  </div>
 </body>
```

#### html2text {}

```diff
@@ -1,21 +1,23 @@
 {% load i18n %} {% load static %} {% load wagtailimages_tags %} {% load
 wagtailmarkdown %} {% load wagtail_resume_extras %} {% if debug_i18n %} {%
-include 'wagtail_resume/localization_dropdown.html' %} {% endif %} {% with
-page.background_color|default_if_none:"#343A40" as bg_color %}
-{% endwith %}
+include 'wagtail_resume/localization_dropdown.html' %} {% endif %} {# djlint:
+off #} {% with page.background_color|default_if_none:"#343A40" as bg_color %}
+{% endwith %} {# djlint:on #}
 ********** {{{{ ppaaggee..ffuullll__nnaammee }}}} **********
 {% if page.role %}
 ********** {{{{ ppaaggee..rroollee }}}} **********
 {% endif %}
 {% for social_link in page.social_links %}
-_{_%_ _i_f_ _s_o_c_i_a_l___l_i_n_k_._v_a_l_u_e_._l_o_g_o_ _%_}_ _{_%_ _i_m_a_g_e_ _s_o_c_i_a_l___l_i_n_k_._v_a_l_u_e_._l_o_g_o_ _o_r_i_g_i_n_a_l_ _%_}_ _{
-_{_ _s_o_c_i_a_l___l_i_n_k_._v_a_l_u_e_._t_e_x_t_ _}_}_ _{_%_ _e_l_s_e_ _%_}_ _{_{_ _s_o_c_i_a_l___l_i_n_k_._v_a_l_u_e_._t_e_x_t_ _}_}_ _{_%_ _e_n_d_i_f_ _%_}
+_{_%_ _i_f_ _s_o_c_i_a_l___l_i_n_k_._v_a_l_u_e_._l_o_g_o_ _%_}_ _{_%_ _i_m_a_g_e_ _s_o_c_i_a_l___l_i_n_k_._v_a_l_u_e_._l_o_g_o_ _o_r_i_g_i_n_a_l
+_c_l_a_s_s_=_"_m_t_-_1_"_ _%_}_ _{_{_ _s_o_c_i_a_l___l_i_n_k_._v_a_l_u_e_._t_e_x_t_ _}_}_ _{_%_ _e_l_s_e_ _%_}_ _{
+_{_ _s_o_c_i_a_l___l_i_n_k_._v_a_l_u_e_._t_e_x_t_ _}_}_ _{_%_ _e_n_d_i_f_ _%_}
 {% endfor %}
+Last update: {{ page.latest_revision_created_at|date }}
 {% image page.photo original class="photo" %}
-{{%% iiff ppaaggee..aabboouutt__iiccoonn %%}} {{%% eennddiiff %%}} {{%% ttrraannss ""AAbboouutt"" %%}}
+{{%% iiff ppaaggee..aabboouutt__iiccoonn %%}}{{%% eennddiiff %%}} {{%% ttrraannss ""AAbboouutt"" %%}}
 ===============================================================================
 {{ page.about | markdown }}
-{% for block in page.resume %} {{ block }} {% endfor %} {% if
+{% for block in page.resume %}{{ block }}{% endfor %} {% if
 page.pdf_generation_visibility == "always" or user.is_authenticated and
 page.pdf_generation_visibility == "authenticated" %} _{_%_ _t_r_a_n_s_ _"_G_e_t_ _P_D_F_"_ _%_} {%
 endif %}
```

### Comparing `wagtail_resume-2.6.0/wagtail_resume/templates/wagtail_resume/resume_page_head.html` & `wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/resume_page_head.html`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.6.0/wagtail_resume/views.py` & `wagtail_resume-2.7.0/wagtail_resume/views.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.6.0/PKG-INFO` & `wagtail_resume-2.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-resume
-Version: 2.6.0
+Version: 2.7.0
 Summary: A Wagtail project made to simplify creation of resumes for developers.
 Home-page: https://github.com/adinhodovic/wagtail-resume
 License: MIT
 Keywords: Resume,Django,Wagtail,CMS
 Author: Adin Hodovic
 Author-email: hodovicadin@gmail.com
 Requires-Python: >=3.10,<4.0
```

