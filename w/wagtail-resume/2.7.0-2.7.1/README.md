# Comparing `tmp/wagtail_resume-2.7.0.tar.gz` & `tmp/wagtail_resume-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_resume-2.7.0.tar", max compression
+gzip compressed data, was "wagtail_resume-2.7.1.tar", max compression
```

## Comparing `wagtail_resume-2.7.0.tar` & `wagtail_resume-2.7.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1069 2024-04-17 20:43:02.110716 wagtail_resume-2.7.0/LICENSE
--rw-r--r--   0        0        0     3496 2024-04-17 20:43:02.110716 wagtail_resume-2.7.0/README.md
--rw-r--r--   0        0        0     3729 2024-04-17 20:43:02.110716 wagtail_resume-2.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/__init__.py
--rw-r--r--   0        0        0      138 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/apps.py
--rw-r--r--   0        0        0     7326 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/blocks.py
--rw-r--r--   0        0        0     1085 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/locale/sv/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3477 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0001_initial.py
--rw-r--r--   0        0        0     1955 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0002_auto_20191227_0916.py
--rw-r--r--   0        0        0     3655 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0003_auto_20200110_1525.py
--rw-r--r--   0        0        0      467 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0004_auto_20200110_1656.py
--rw-r--r--   0        0        0     3843 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0005_auto_20200227_1224.py
--rw-r--r--   0        0        0      694 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0006_alter_baseresumepage_social_links.py
--rw-r--r--   0        0        0      792 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0007_baseresumepage_pdf_generation_visibility.py
--rw-r--r--   0        0        0     4472 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0008_auto_20220211_1557.py
--rw-r--r--   0        0        0      953 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0009_alter_baseresumepage_pdf_generation_visibility.py
--rw-r--r--   0        0        0    18241 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0010_alter_baseresumepage_resume_and_more.py
--rw-r--r--   0        0        0    17599 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0011_baseresumepage_about_icon_and_more.py
--rw-r--r--   0        0        0    17734 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0012_alter_baseresumepage_resume.py
--rw-r--r--   0        0        0    18655 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0013_alter_baseresumepage_resume.py
--rw-r--r--   0        0        0      535 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/0014_baseresumepage_display_last_update.py
--rw-r--r--   0        0        0        0 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/migrations/__init__.py
--rw-r--r--   0        0        0     4037 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/models.py
--rw-r--r--   0        0        0        0 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/static/wagtail_resume/css/.gitkeep
--rw-r--r--   0        0        0     2024 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/static/wagtail_resume/css/resume_page.css
--rw-r--r--   0        0        0        0 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/static/wagtail_resume/images/.gitkeep
--rw-r--r--   0        0        0        0 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/static/wagtail_resume/js/.gitkeep
--rw-r--r--   0        0        0      406 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/blocks/contributions_block.html
--rw-r--r--   0        0        0     1516 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/blocks/education_block.html
--rw-r--r--   0        0        0      951 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/blocks/work_experience_block.html
--rw-r--r--   0        0        0      691 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/blocks/writings_block.html
--rw-r--r--   0        0        0      653 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/localization_dropdown.html
--rw-r--r--   0        0        0      107 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/resume_page.html
--rw-r--r--   0        0        0     2488 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/resume_page_body.html
--rw-r--r--   0        0        0      564 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/resume_page_head.html
--rw-r--r--   0        0        0        0 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/templatetags/__init__.py
--rw-r--r--   0        0        0      139 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/templatetags/wagtail_resume_extras.py
--rw-r--r--   0        0        0      142 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/urls.py
--rw-r--r--   0        0        0     2075 2024-04-17 20:43:02.114716 wagtail_resume-2.7.0/wagtail_resume/views.py
--rw-r--r--   0        0        0     4955 1970-01-01 00:00:00.000000 wagtail_resume-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-17 21:31:23.074343 wagtail_resume-2.7.1/LICENSE
+-rw-r--r--   0        0        0     3496 2024-04-17 21:31:23.078343 wagtail_resume-2.7.1/README.md
+-rw-r--r--   0        0        0     3729 2024-04-17 21:31:23.078343 wagtail_resume-2.7.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-17 21:31:23.078343 wagtail_resume-2.7.1/wagtail_resume/__init__.py
+-rw-r--r--   0        0        0      138 2024-04-17 21:31:23.078343 wagtail_resume-2.7.1/wagtail_resume/apps.py
+-rw-r--r--   0        0        0     7326 2024-04-17 21:31:23.078343 wagtail_resume-2.7.1/wagtail_resume/blocks.py
+-rw-r--r--   0        0        0     1085 2024-04-17 21:31:23.078343 wagtail_resume-2.7.1/wagtail_resume/locale/sv/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3477 2024-04-17 21:31:23.078343 wagtail_resume-2.7.1/wagtail_resume/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1955 2024-04-17 21:31:23.078343 wagtail_resume-2.7.1/wagtail_resume/migrations/0002_auto_20191227_0916.py
+-rw-r--r--   0        0        0     3655 2024-04-17 21:31:23.078343 wagtail_resume-2.7.1/wagtail_resume/migrations/0003_auto_20200110_1525.py
+-rw-r--r--   0        0        0      467 2024-04-17 21:31:23.078343 wagtail_resume-2.7.1/wagtail_resume/migrations/0004_auto_20200110_1656.py
+-rw-r--r--   0        0        0     3843 2024-04-17 21:31:23.078343 wagtail_resume-2.7.1/wagtail_resume/migrations/0005_auto_20200227_1224.py
+-rw-r--r--   0        0        0      694 2024-04-17 21:31:23.078343 wagtail_resume-2.7.1/wagtail_resume/migrations/0006_alter_baseresumepage_social_links.py
+-rw-r--r--   0        0        0      792 2024-04-17 21:31:23.078343 wagtail_resume-2.7.1/wagtail_resume/migrations/0007_baseresumepage_pdf_generation_visibility.py
+-rw-r--r--   0        0        0     4472 2024-04-17 21:31:23.078343 wagtail_resume-2.7.1/wagtail_resume/migrations/0008_auto_20220211_1557.py
+-rw-r--r--   0        0        0      953 2024-04-17 21:31:23.078343 wagtail_resume-2.7.1/wagtail_resume/migrations/0009_alter_baseresumepage_pdf_generation_visibility.py
+-rw-r--r--   0        0        0    18241 2024-04-17 21:31:23.078343 wagtail_resume-2.7.1/wagtail_resume/migrations/0010_alter_baseresumepage_resume_and_more.py
+-rw-r--r--   0        0        0    17599 2024-04-17 21:31:23.078343 wagtail_resume-2.7.1/wagtail_resume/migrations/0011_baseresumepage_about_icon_and_more.py
+-rw-r--r--   0        0        0    17734 2024-04-17 21:31:23.078343 wagtail_resume-2.7.1/wagtail_resume/migrations/0012_alter_baseresumepage_resume.py
+-rw-r--r--   0        0        0    18655 2024-04-17 21:31:23.078343 wagtail_resume-2.7.1/wagtail_resume/migrations/0013_alter_baseresumepage_resume.py
+-rw-r--r--   0        0        0      535 2024-04-17 21:31:23.078343 wagtail_resume-2.7.1/wagtail_resume/migrations/0014_baseresumepage_display_last_update.py
+-rw-r--r--   0        0        0        0 2024-04-17 21:31:23.078343 wagtail_resume-2.7.1/wagtail_resume/migrations/__init__.py
+-rw-r--r--   0        0        0     4037 2024-04-17 21:31:23.082343 wagtail_resume-2.7.1/wagtail_resume/models.py
+-rw-r--r--   0        0        0        0 2024-04-17 21:31:23.082343 wagtail_resume-2.7.1/wagtail_resume/static/wagtail_resume/css/.gitkeep
+-rw-r--r--   0        0        0     2024 2024-04-17 21:31:23.082343 wagtail_resume-2.7.1/wagtail_resume/static/wagtail_resume/css/resume_page.css
+-rw-r--r--   0        0        0        0 2024-04-17 21:31:23.082343 wagtail_resume-2.7.1/wagtail_resume/static/wagtail_resume/images/.gitkeep
+-rw-r--r--   0        0        0        0 2024-04-17 21:31:23.082343 wagtail_resume-2.7.1/wagtail_resume/static/wagtail_resume/js/.gitkeep
+-rw-r--r--   0        0        0      406 2024-04-17 21:31:23.082343 wagtail_resume-2.7.1/wagtail_resume/templates/wagtail_resume/blocks/contributions_block.html
+-rw-r--r--   0        0        0     1516 2024-04-17 21:31:23.082343 wagtail_resume-2.7.1/wagtail_resume/templates/wagtail_resume/blocks/education_block.html
+-rw-r--r--   0        0        0      951 2024-04-17 21:31:23.082343 wagtail_resume-2.7.1/wagtail_resume/templates/wagtail_resume/blocks/work_experience_block.html
+-rw-r--r--   0        0        0      691 2024-04-17 21:31:23.082343 wagtail_resume-2.7.1/wagtail_resume/templates/wagtail_resume/blocks/writings_block.html
+-rw-r--r--   0        0        0      653 2024-04-17 21:31:23.082343 wagtail_resume-2.7.1/wagtail_resume/templates/wagtail_resume/localization_dropdown.html
+-rw-r--r--   0        0        0      107 2024-04-17 21:31:23.082343 wagtail_resume-2.7.1/wagtail_resume/templates/wagtail_resume/resume_page.html
+-rw-r--r--   0        0        0     2563 2024-04-17 21:31:23.082343 wagtail_resume-2.7.1/wagtail_resume/templates/wagtail_resume/resume_page_body.html
+-rw-r--r--   0        0        0      564 2024-04-17 21:31:23.082343 wagtail_resume-2.7.1/wagtail_resume/templates/wagtail_resume/resume_page_head.html
+-rw-r--r--   0        0        0        0 2024-04-17 21:31:23.082343 wagtail_resume-2.7.1/wagtail_resume/templatetags/__init__.py
+-rw-r--r--   0        0        0      139 2024-04-17 21:31:23.082343 wagtail_resume-2.7.1/wagtail_resume/templatetags/wagtail_resume_extras.py
+-rw-r--r--   0        0        0      142 2024-04-17 21:31:23.082343 wagtail_resume-2.7.1/wagtail_resume/urls.py
+-rw-r--r--   0        0        0     2075 2024-04-17 21:31:23.082343 wagtail_resume-2.7.1/wagtail_resume/views.py
+-rw-r--r--   0        0        0     4955 1970-01-01 00:00:00.000000 wagtail_resume-2.7.1/PKG-INFO
```

### Comparing `wagtail_resume-2.7.0/LICENSE` & `wagtail_resume-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/README.md` & `wagtail_resume-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/pyproject.toml` & `wagtail_resume-2.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "wagtail-resume"
 authors = ["Adin Hodovic <hodovicadin@gmail.com>"]
 license = "MIT"
-version = "2.7.0"
+version = "2.7.1"
 readme = "README.md"
 homepage = "https://github.com/adinhodovic/wagtail-resume"
 repository = "https://github.com/adinhodovic/wagtail-resume"
 documentation = "https://github.com/adinhodovic/wagtail-resume"
 description = "A Wagtail project made to simplify creation of resumes for developers."
 keywords = ["Resume", "Django", "Wagtail", "CMS"]
 classifiers = [
```

### Comparing `wagtail_resume-2.7.0/wagtail_resume/blocks.py` & `wagtail_resume-2.7.1/wagtail_resume/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/wagtail_resume/locale/sv/LC_MESSAGES/django.po` & `wagtail_resume-2.7.1/wagtail_resume/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/wagtail_resume/migrations/0001_initial.py` & `wagtail_resume-2.7.1/wagtail_resume/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/wagtail_resume/migrations/0002_auto_20191227_0916.py` & `wagtail_resume-2.7.1/wagtail_resume/migrations/0002_auto_20191227_0916.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/wagtail_resume/migrations/0003_auto_20200110_1525.py` & `wagtail_resume-2.7.1/wagtail_resume/migrations/0003_auto_20200110_1525.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/wagtail_resume/migrations/0005_auto_20200227_1224.py` & `wagtail_resume-2.7.1/wagtail_resume/migrations/0005_auto_20200227_1224.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/wagtail_resume/migrations/0006_alter_baseresumepage_social_links.py` & `wagtail_resume-2.7.1/wagtail_resume/migrations/0006_alter_baseresumepage_social_links.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/wagtail_resume/migrations/0007_baseresumepage_pdf_generation_visibility.py` & `wagtail_resume-2.7.1/wagtail_resume/migrations/0007_baseresumepage_pdf_generation_visibility.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/wagtail_resume/migrations/0008_auto_20220211_1557.py` & `wagtail_resume-2.7.1/wagtail_resume/migrations/0008_auto_20220211_1557.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/wagtail_resume/migrations/0009_alter_baseresumepage_pdf_generation_visibility.py` & `wagtail_resume-2.7.1/wagtail_resume/migrations/0009_alter_baseresumepage_pdf_generation_visibility.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/wagtail_resume/migrations/0010_alter_baseresumepage_resume_and_more.py` & `wagtail_resume-2.7.1/wagtail_resume/migrations/0010_alter_baseresumepage_resume_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/wagtail_resume/migrations/0011_baseresumepage_about_icon_and_more.py` & `wagtail_resume-2.7.1/wagtail_resume/migrations/0011_baseresumepage_about_icon_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/wagtail_resume/migrations/0012_alter_baseresumepage_resume.py` & `wagtail_resume-2.7.1/wagtail_resume/migrations/0012_alter_baseresumepage_resume.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/wagtail_resume/migrations/0013_alter_baseresumepage_resume.py` & `wagtail_resume-2.7.1/wagtail_resume/migrations/0013_alter_baseresumepage_resume.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/wagtail_resume/migrations/0014_baseresumepage_display_last_update.py` & `wagtail_resume-2.7.1/wagtail_resume/migrations/0014_baseresumepage_display_last_update.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/wagtail_resume/models.py` & `wagtail_resume-2.7.1/wagtail_resume/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/wagtail_resume/static/wagtail_resume/css/resume_page.css` & `wagtail_resume-2.7.1/wagtail_resume/static/wagtail_resume/css/resume_page.css`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/blocks/education_block.html` & `wagtail_resume-2.7.1/wagtail_resume/templates/wagtail_resume/blocks/education_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/blocks/work_experience_block.html` & `wagtail_resume-2.7.1/wagtail_resume/templates/wagtail_resume/blocks/work_experience_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/blocks/writings_block.html` & `wagtail_resume-2.7.1/wagtail_resume/templates/wagtail_resume/blocks/writings_block.html`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/localization_dropdown.html` & `wagtail_resume-2.7.1/wagtail_resume/templates/wagtail_resume/localization_dropdown.html`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/resume_page_body.html` & `wagtail_resume-2.7.1/wagtail_resume/templates/wagtail_resume/resume_page_body.html`

 * *Files 20% similar despite different names*

```diff
@@ -37,15 +37,17 @@
                   {% else %}
                     <span class="ml-0">{{ social_link.value.text }}</span>
                   {% endif %}
                 </a>
               </div>
             {% endfor %}
           </div>
-          <p class="small italic mt-1">Last update: {{ page.latest_revision_created_at|date }}</p>
+          {% if page.latest_revision_created_at %}
+            <p class="small italic mt-1">Last update: {{ page.latest_revision_created_at|date }}</p>
+          {% endif %}
         </div>
         <div>{% image page.photo original class="photo" %}</div>
       </div>
       <div>
         <h2 class="mt-4 mb-0">
           {% if page.about_icon %}<i class="{{ page.about_icon }}"></i>{% endif %}
           <span>{% trans "About" %}</span>
```

#### html2text {}

```diff
@@ -8,15 +8,17 @@
 ********** {{{{ ppaaggee..rroollee }}}} **********
 {% endif %}
 {% for social_link in page.social_links %}
 _{_%_ _i_f_ _s_o_c_i_a_l___l_i_n_k_._v_a_l_u_e_._l_o_g_o_ _%_}_ _{_%_ _i_m_a_g_e_ _s_o_c_i_a_l___l_i_n_k_._v_a_l_u_e_._l_o_g_o_ _o_r_i_g_i_n_a_l
 _c_l_a_s_s_=_"_m_t_-_1_"_ _%_}_ _{_{_ _s_o_c_i_a_l___l_i_n_k_._v_a_l_u_e_._t_e_x_t_ _}_}_ _{_%_ _e_l_s_e_ _%_}_ _{
 _{_ _s_o_c_i_a_l___l_i_n_k_._v_a_l_u_e_._t_e_x_t_ _}_}_ _{_%_ _e_n_d_i_f_ _%_}
 {% endfor %}
+{% if page.latest_revision_created_at %}
 Last update: {{ page.latest_revision_created_at|date }}
+{% endif %}
 {% image page.photo original class="photo" %}
 {{%% iiff ppaaggee..aabboouutt__iiccoonn %%}}{{%% eennddiiff %%}} {{%% ttrraannss ""AAbboouutt"" %%}}
 ===============================================================================
 {{ page.about | markdown }}
 {% for block in page.resume %}{{ block }}{% endfor %} {% if
 page.pdf_generation_visibility == "always" or user.is_authenticated and
 page.pdf_generation_visibility == "authenticated" %} _{_%_ _t_r_a_n_s_ _"_G_e_t_ _P_D_F_"_ _%_} {%
```

### Comparing `wagtail_resume-2.7.0/wagtail_resume/templates/wagtail_resume/resume_page_head.html` & `wagtail_resume-2.7.1/wagtail_resume/templates/wagtail_resume/resume_page_head.html`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/wagtail_resume/views.py` & `wagtail_resume-2.7.1/wagtail_resume/views.py`

 * *Files identical despite different names*

### Comparing `wagtail_resume-2.7.0/PKG-INFO` & `wagtail_resume-2.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-resume
-Version: 2.7.0
+Version: 2.7.1
 Summary: A Wagtail project made to simplify creation of resumes for developers.
 Home-page: https://github.com/adinhodovic/wagtail-resume
 License: MIT
 Keywords: Resume,Django,Wagtail,CMS
 Author: Adin Hodovic
 Author-email: hodovicadin@gmail.com
 Requires-Python: >=3.10,<4.0
```

