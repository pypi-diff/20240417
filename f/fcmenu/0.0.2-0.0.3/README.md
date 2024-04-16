# Comparing `tmp/fcmenu-0.0.2.tar.gz` & `tmp/fcmenu-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcmenu-0.0.2.tar", last modified: Fri Apr 12 01:10:27 2024, max compression
+gzip compressed data, was "fcmenu-0.0.3.tar", last modified: Tue Apr 16 22:44:32 2024, max compression
```

## Comparing `fcmenu-0.0.2.tar` & `fcmenu-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 01:10:27.067755 fcmenu-0.0.2/
--rw-rw-rw-   0        0        0      357 2024-04-12 01:10:27.066754 fcmenu-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       36 2024-04-11 03:27:48.000000 fcmenu-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 01:10:27.050754 fcmenu-0.0.2/fcmenu/
--rw-rw-rw-   0        0        0    48620 2024-04-12 01:06:44.000000 fcmenu-0.0.2/fcmenu/Chrome_Session.py
--rw-rw-rw-   0        0        0       57 2024-04-11 02:42:44.000000 fcmenu-0.0.2/fcmenu/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 01:10:27.065754 fcmenu-0.0.2/fcmenu.egg-info/
--rw-rw-rw-   0        0        0      357 2024-04-12 01:10:26.000000 fcmenu-0.0.2/fcmenu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2024-04-12 01:10:26.000000 fcmenu-0.0.2/fcmenu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 01:10:26.000000 fcmenu-0.0.2/fcmenu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-12 01:10:26.000000 fcmenu-0.0.2/fcmenu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-12 01:10:26.000000 fcmenu-0.0.2/fcmenu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 01:10:27.067755 fcmenu-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      734 2024-04-12 01:10:04.000000 fcmenu-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 22:44:32.249784 fcmenu-0.0.3/
+-rw-rw-rw-   0        0        0      357 2024-04-16 22:44:32.248787 fcmenu-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       36 2024-04-11 03:27:48.000000 fcmenu-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 22:44:32.234786 fcmenu-0.0.3/fcmenu/
+-rw-rw-rw-   0        0        0    42377 2024-04-16 22:41:18.000000 fcmenu-0.0.3/fcmenu/Chrome_Session.py
+-rw-rw-rw-   0        0        0       57 2024-04-11 02:42:44.000000 fcmenu-0.0.3/fcmenu/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 22:44:32.247784 fcmenu-0.0.3/fcmenu.egg-info/
+-rw-rw-rw-   0        0        0      357 2024-04-16 22:44:32.000000 fcmenu-0.0.3/fcmenu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2024-04-16 22:44:32.000000 fcmenu-0.0.3/fcmenu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 22:44:32.000000 fcmenu-0.0.3/fcmenu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-16 22:44:32.000000 fcmenu-0.0.3/fcmenu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-16 22:44:32.000000 fcmenu-0.0.3/fcmenu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 22:44:32.250285 fcmenu-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      734 2024-04-16 22:43:52.000000 fcmenu-0.0.3/setup.py
```

### Comparing `fcmenu-0.0.2/fcmenu/Chrome_Session.py` & `fcmenu-0.0.3/fcmenu/Chrome_Session.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,186 +7,48 @@
     import csv
     import io
     from PIL import Image
     import time
     import glob
     import time
     import pandas as pd
-    from datetime import datetime
     from datetime import datetime, timedelta
-    from selenium.common.exceptions import WebDriverException, TimeoutException, NoSuchElementException, StaleElementReferenceException,  ElementClickInterceptedException, UnexpectedAlertPresentException, NoAlertPresentException, NoSuchWindowException
+    from selenium.common.exceptions import WebDriverException, TimeoutException, NoSuchElementException, StaleElementReferenceException,  ElementClickInterceptedException, UnexpectedAlertPresentException, NoAlertPresentException, NoSuchWindowException, ElementNotInteractableException
     from selenium.webdriver.support.ui import WebDriverWait
     from selenium.webdriver.support import expected_conditions as EC
     from selenium.webdriver.chrome.options import Options as ChromeOptions
     from selenium.webdriver.common.action_chains import ActionChains
     from selenium.webdriver.common.keys import Keys
     from selenium.webdriver.common.by import By
     from selenium.webdriver import Chrome
+    from selenium.webdriver.remote.webelement import WebElement
+    from util.utilities import locator, header, constants
+    
 except ImportError as e:
     missing_module = str(e).split("'")[1]
     print(f"Module '{missing_module}' is not installed. Installing...")
     subprocess.check_call([sys.executable, '-m', 'pip', 'install', missing_module])
     print(f"Module '{missing_module}' has been installed. Please restart the script.")
     sys.exit(1)
 logging.basicConfig(level=logging.ERROR)
 
-LOGIN_URL = "https://fcmenu-iad-regionalized.corp.amazon.com/login"
-CHROME_PATH = r"C:\Users\nuneadon\AppData\Local\Google\Chrome\Application\chrome.exe"
-ARGUMENTS = ['--log-level=3','--force-device-scale-factor=0.7','--disable-blink-features=AutomationControlled','--disable-notifications','--disable-infobars','--disable-extensions','--disable-dev-shm-usage','--disable-gpu','--disable-browser-side-navigation','--disable-features=VizDisplayCompositor','--no-sandbox','--disable-logging']
-
-class locator:
-    body = '/html/body'
-    nav = '/html/body/nav'
-    class xpath:
-        class sideline_app:
-            input = '/html/body/div[1]/div/div/div[2]/div/div[1]/div/div[2]/div/div/div/div/div/div/div[2]/div/div[1]/div/div/div[1]/input'
-            change_container = '/html/body/div[1]/div/div/div[2]/div/div[2]/div/div[1]/div/div/div/div/div[3]/button/div/span'
-            confirmation_yes = '/html/body/div[4]/div/div/div/div[3]/div/div[4]/button/div/span'
-            source_container = '/html/body/div[1]/div/div/div[2]/div/div[2]/div/div[1]/div/div/div/div/div[2]/span'
-            confirmed = '/html/body/div[1]/div/div/div[2]/div/div[1]/div/div[2]/div/div[1]/div/div/div/div/div[2]/div/div/span'
-            confirmation_div_overlay = '/html/body/div[4]/div/div/div'
-            main_panel = '/html/body/div[1]/div/div/div[2]/div/div[1]'
-        class counts:
-            time_span = '/html/body/div[2]/nav/div[2]/ul[2]/li[3]/a'
-            iframe = '/html/body/div/iframe'
-            absolute = '/html/body/div[2]/config/div/div[1]/kbn-timepicker/div/div/div[1]/div/div[1]/ul/li[3]/a'
-            time_from = '/html/body/div[2]/config/div/div[1]/kbn-timepicker/div/div/div[1]/div/div[2]/div/div/form/div[1]/div[1]/input'
-            time_to = '/html/body/div[2]/config/div/div[1]/kbn-timepicker/div/div/div[1]/div/div[2]/div/div/form/div[2]/div[1]/input'
-            go = '/html/body/div[2]/config/div/div[1]/kbn-timepicker/div/div/div[1]/div/div[2]/div/div/form/div[3]/div/button'
-            okay = '/html/body/div[4]/div/div/div[2]/button[2]'
-
-        class delete:
-            H1_header = '/html/body/div[1]/div[4]/div/div[2]/div[1]/div/div/h1'
-            restart = '/html/body/div[1]/div[2]/div/div[2]/ul/li[2]/span/span/a'
-            btn_restart = '/html/body/div[4]/div/div/div/div[1]/div[1]/span[2]/div/div/div/div[1]/h1'
-
-            class scan:
-                input = '/html/body/div[1]/div[4]/div/div[2]/div[1]/span/form/div/input'
-                enter = '/html/body/div[1]/div[4]/div/div[2]/div[1]/span/form/span/span/input'
-            class select:
-                enter = '/html/body/div[1]/div[4]/div/div[2]/div[1]/span/form/span[1]/span/input'
-                container_empty = '/html/body/div[1]/div[4]/div/div[2]/div[1]/span/form/div[2]/div/div'
-            class reason:
-                reason_statement  = '/html/body/div[1]/div[4]/div/div[1]/div/dl[3]/dd'
-                sweeping_out = '/html/body/div[1]/div[4]/div/div[2]/div[1]/span/form/div[1]/fieldset/div[1]/div/div/label/span'
-                enter = '/html/body/div[1]/div[4]/div/div[2]/div[1]/span/form/span[1]/span/input'
-            class confirm:
-                enter = '/html/body/div[1]/div[4]/div/div[2]/div[1]/form/span[1]/span/span/input'
-
-        class fcmenu:
-            input_badge = '//*[@id="badgeBarcodeId"]'
-            inbound = '/html/body/div[3]/div/div[2]/ul[1]/li[1]/a'
-            outbound = '/html/body/div[3]/div/div[2]/ul[1]/li[2]/a'
-            picking = '/html/body/div[3]/div/div[2]/ul[1]/li[1]/a'
-            move_container_145 = '/html/body/div[3]/div/div[2]/ul[2]/li[3]/a'
-            individually_workflow = '/html/body/div/div/div/ul/li[2]'
-            problem_solve = '/html/body/div[3]/div/div[2]/ul[2]/li[5]/a'
-            sideline_app = '/html/body/div[3]/div/div[2]/ul[1]/li[1]/a'
-
-            class move_container:
-                input = '/html/body/div/div[7]/div/input'
-                error_msg = '/html/body/div/div[4]/div[2]/div[1]'
-            class peculiar_inventory:
-                table_body = '/html/body/div[1]/div[3]/div/div[1]/div/div[1]/table/tbody'
-
-            class fcresearch:
-                asin = '/html/body/div[2]/div/div[1]/div/div[6]/div/div[2]/div/div/div[1]/div[2]/table/tbody/tr/td[2]/a'
-
-            class pick:
-                no_batch = '/html/body/div[1]/div[5]/ul/li[2]/a'
-                input = '/html/body/div[1]/div[5]/form/input[6]'
-                commit = '/html/body/div[1]/div[5]/form/input[7]'
-                class vehicle:
-                    input = '/html/body/div[1]/div[5]/form/input[6]'
-                    title = '/html/body/div[1]/div[5]/p[1]/b'
-                
-                class cage:
-                    title = '/html/body/div[1]/div[5]/div[1]'
-                
-                class scan_bin:
-                    case = '/html/body/div[1]/div[5]/div[3]/div[1]/span[2]'
-                    input = '/html/body/div[1]/div[5]/form[1]/input[9]'
-                    commit = '/html/body/div[1]/div[5]/form[1]/input[10]'
-                    P1 = '/html/body/div[1]/div[5]/div[1]/div[2]/div/span[1]'
-                    P2 = '/html/body/div[1]/div[5]/div[1]/div[2]/div/span[2]'
-                    P3 = '/html/body/div[1]/div[5]/div[1]/div[2]/div/span[3]'
-                
-                class scan_case:
-                    input = '/html/body/div[1]/div[5]/form/input[10]'
-                    commit = '/html/body/div[1]/div[5]/form/input[11]'
-
-                    
-
-        class picking_console:
-            error_msg = '/html/body/div/div/div/awsui-app-layout/div/main/div/div[1]/div/span/awsui-flashbar/div/awsui-flash/div/div[2]/div/div/span/span/span'
-            table = '/html/body/div/div/div/awsui-app-layout/div/main/div/div[2]/div[2]/span/div/div[3]/div/div/awsui-table/div/div[3]'
-
-        class fc_andons:
-            error_msg = '/html/body/div/div/div/awsui-app-layout/div/main/div/div[2]/div/span/div/awsui-flash/div/div[2]/div/div'
-
-    class class_name:
-        class delete:
-            enter = 'a-button-input'
-
-        class counts:
-            spinner = 'spinner.large'
-
-        class sideline_app:
-            step = 'text text--bold'
-            trans_out = 'text text--size-xl text--variant-white'
-
-        class pick:
-            bin = 'greyed-text'
-
-    class ID:
-        
-        class pick:
-            spinner = 'spinner'
-
-
-class header:  
-    SCAN = 'Scan container'
-    SELECT = 'Select item to delete'
-    REASON = ['Select reason to delete','Select deletion reason']
-    CONFIRM = 'Confirm the deletion'
+LOGIN_URL = constants.LOGIN_URL
+CHROME_PATH = constants.CHROME_PATH
+ARGUMENTS = constants.ARGUMENTS
 
 class chromeSession():
     def __init__(self, site: str, badge: int):
         """Sideline Shorting, DeleteItems App, PickUI and other ICQA related data scrapping. Use close() method to end chrome process"""
         self.step = int
         self.driver = None
         self.badge = str(badge)
         self.site = str(site).upper()
         self.file_prefixes = ["Pick All types", "Bin Item Defects All types"]
         self.start()
 
-    def delete_cookie_by_name(self, cookie_name) -> None:
-        """Deletes a cookie by name in the Chrome settings."""
-        # Open Chrome settings
-        self.driver.get("chrome://settings/content/all")
-
-        # Wait for the cookies to load
-        WebDriverWait(self.driver, 10).until(EC.presence_of_element_located(('xpath', "/html/body/settings-ui//div[2]/settings-main//settings-basic-page//div[1]/settings-section[5]/settings-privacy-page//settings-animated-pages/settings-subpage/all-sites//div[6]/iron-list/site-entry[1]//div/div/div[2]/cr-icon-button")))
-
-        # Find all cookies
-        cookies = self.driver.find_element('xpath', "/html/body/settings-ui//div[2]/settings-main//settings-basic-page//div[1]/settings-section[5]/settings-privacy-page//settings-animated-pages/settings-subpage/all-sites//div[6]/iron-list/site-entry[1]//div/div/div[2]/cr-icon-button")
-
-        # Iterate over cookies to find the one with the specified name
-        for cookie in cookies:
-            # Check if the cookie name matches
-            if cookie.find_element(By.CSS_SELECTOR, ".settings-cookie-name").text == cookie_name:
-                # Click on the corresponding trash button
-                trash_button = cookie.find_element(By.CSS_SELECTOR, ".settings-cookie-remove")
-                trash_button.click()
-
-                # Find and click the "Delete site data and permissions" link
-                delete_link = self.driver.find_element(By.XPATH, '//button[@title="Delete site data and permissions for a2z.com"]')
-                delete_link.click()
-                break
-
     def install_module(self, module_name: str) -> None:
         try:
             importlib.import_module(module_name)
         except ModuleNotFoundError:
             logging.info(f"{module_name} not found. Installing it now...")
             try:
                 subprocess.run([sys.executable, '-m', 'pip',
@@ -628,21 +490,25 @@
 
                 elif current_state == header.CONFIRM:
                     confirm_deletion()
                     print(f"{container} DELETED\n{'-' * 47}")
                     current_state = 'end'
 
 
-    def sideline_delete(self, container):
+    def sideline_delete(self, container: str, shorted_container_to_dz: str):
         """
         Short containers via SidelineApp
         """
         STEP = str
         url_sideline = 'https://aft-poirot-website-iad.iad.proxy.amazon.com/'
-        self.navigate(url_sideline) if self.driver.current_url != url_sideline else None
+        try:
+            self.navigate(url_sideline) if self.driver.current_url != url_sideline else None
+        except NoSuchWindowException:
+            print(f"Verify Chrome Window is displayed on-screen, it seems it is not\n\nError:\n{e}")
+            sys.exit(0)
         if self.driver.current_url != url_sideline:
             WebDriverWait(self.driver, 10).until(EC.visibility_of_element_located((By.XPATH, locator.xpath.fcmenu.problem_solve))).click()
             WebDriverWait(self.driver, 10).until(EC.visibility_of_element_located((By.XPATH, locator.xpath.fcmenu.sideline_app))).click()
 
         def get_step():
             text =  WebDriverWait(self.driver, 5).until(EC.presence_of_element_located((By.XPATH, locator.xpath.sideline_app.source_container))).text
             if text == "":
@@ -701,56 +567,58 @@
                     change_container()
                     time.sleep(.2)
                     self.step = 3
                     if self.step == 3:
                         overlay = WebDriverWait(self.driver, 5).until(EC.presence_of_element_located((By.XPATH, locator.xpath.sideline_app.confirmation_div_overlay)))
                         if overlay:
                             STEP = confirm()
+                            # self.move_container(200, container, shorted_container_to_dz)
                         else: self.step = 2
                     else: self.step = 2
             except TimeoutException:
                 start_over()
                 self.step = 0
 
-    def pickUI(self, vehicle: str, cage: str) -> str:
+    def pickUI(self, vehicle: str, cage: str, dirtyVehicle_dz_location: str, deleted_container_to_dz: str) -> str:
         """
         Simulate picker's picking actions followed by deleting the container and moving container to TRASH
         
         Ensure DeleteItemsApp is set to container mode. Preferably, set picking eligibilities to csX and not including paX containers
         """
-        vehicle_dropoff = 'veCG00245'
+        vehicle_dropoff = str(dirtyVehicle_dz_location)
         if self.driver.current_url == f'http://pickui-{self.site.lower()}.aka.amazon.com/pick/pick' or self.driver.current_url != f'http://pickui-{self.site.lower()}.aka.amazon.com/pick/scan_bin':
             if self.driver.current_url != f'https://fcmenu-iad-regionalized.corp.amazon.com/{self.site}':
-                self.FCMenu_login()
+                self.FCMenu_login(self.badge)
             try:
                 outbound = WebDriverWait(self.driver, 10).until(EC.visibility_of_element_located((By.XPATH, locator.xpath.fcmenu.outbound)))
                 if outbound.is_displayed():
                     outbound.click()
                     WebDriverWait(self.driver, 10).until(EC.visibility_of_element_located((By.XPATH, locator.xpath.fcmenu.picking))).click()
                 else:
                     raise NoSuchWindowException
             except NoSuchWindowException as e:
                 print(f"Verify Chrome Window is displayed on-screen, it seems it is not\n\nError:\n{e}")
+                sys.exit(0)
         
         def scan(input, container):
             self.driver.execute_script("arguments[0].setAttribute('value', arguments[1])", input, container)
 
         def select_no_batch():
             time.sleep(1)
-            no_batch = WebDriverWait(self.driver, 10).until(EC.presence_of_element_located((By.XPATH, locator.xpath.fcmenu.pick.no_batch)))
+            no_batch = WebDriverWait(self.driver, 10).until(EC.presence_of_element_located((By.XPATH, locator.xpath.fcmenu.pickUI.no_batch)))
             no_batch.click()
 
         def scan_vehicle(ve):
             time.sleep(1.5)
             # wait for "Scan Your Vehicle"
-            WebDriverWait(self.driver, 30).until(EC.text_to_be_present_in_element((By.XPATH, locator.xpath.fcmenu.pick.vehicle.title),'Scan Your Vehicle'))
-            input = WebDriverWait(self.driver, 10).until(EC.presence_of_element_located((By.XPATH, locator.xpath.fcmenu.pick.input)))
+            WebDriverWait(self.driver, 30).until(EC.text_to_be_present_in_element((By.XPATH, locator.xpath.fcmenu.pickUI.vehicle.title),'Scan Your Vehicle'))
+            input = WebDriverWait(self.driver, 10).until(EC.presence_of_element_located((By.XPATH, locator.xpath.fcmenu.pickUI.input)))
             scan(input, ve)
             # commit input
-            WebDriverWait(self.driver, 10).until(EC.presence_of_element_located((By.XPATH, locator.xpath.fcmenu.pick.commit))).submit()
+            WebDriverWait(self.driver, 10).until(EC.presence_of_element_located((By.XPATH, locator.xpath.fcmenu.pickUI.commit))).submit()
 
         def check_vehicle() -> str:
             try:
                 error_div = WebDriverWait(self.driver, .8).until(EC.presence_of_element_located((By.ID, "error")))
                 if 'dirty' in error_div.text:
                     return 'dirty'
                 elif error_div.text == 'No more work: Unable to get job for picker':
@@ -759,26 +627,26 @@
                     return 'clean'
             except TimeoutException:
                 return 'clean'
 
         def scan_cage(paX):
             time.sleep(1)
             # wait for "Scan New Cage"
-            WebDriverWait(self.driver, 10).until(EC.text_to_be_present_in_element((By.XPATH, locator.xpath.fcmenu.pick.cage.title),'Scan New Cage'))
-            input = WebDriverWait(self.driver, 10).until(EC.presence_of_element_located((By.XPATH, locator.xpath.fcmenu.pick.input)))
+            WebDriverWait(self.driver, 10).until(EC.text_to_be_present_in_element((By.XPATH, locator.xpath.fcmenu.pickUI.cage.title),'Scan New Cage'))
+            input = WebDriverWait(self.driver, 10).until(EC.presence_of_element_located((By.XPATH, locator.xpath.fcmenu.pickUI.input)))
             scan(input, paX)
             # commit input
-            WebDriverWait(self.driver, 10).until(EC.presence_of_element_located((By.XPATH, locator.xpath.fcmenu.pick.commit))).submit()
+            WebDriverWait(self.driver, 10).until(EC.presence_of_element_located((By.XPATH, locator.xpath.fcmenu.pickUI.commit))).submit()
 
         def new_tab():
             self.driver.execute_script("window.open('about:blank', '_blank');")
             time.sleep(.5)
             self.driver.switch_to.window(self.driver.window_handles[-1])
 
-        def close_tab(tab: int):
+        def close_tab():
             switch_to_tab
             self.driver.close()
         
         def switch_to_tab(tab: int):
             self.driver.switch_to.window(self.driver.window_handles[tab])
         
         def skip_skip():
@@ -789,31 +657,31 @@
             time.sleep(1)
             body.send_keys('s')
             time.sleep(1)
             body.send_keys(Keys.ENTER)
 
 
         def check_if_pallet():
-            P2 = self.driver.find_element(By.XPATH, locator.xpath.fcmenu.pick.scan_bin.P2).text
+            P2 = self.driver.find_element(By.XPATH, locator.xpath.fcmenu.pickUI.scan_bin.P2).text
             time.sleep(1)
             while 'P' in P2:
                 try:
                     spinner = WebDriverWait(self.driver, 1).until(EC.presence_of_element_located((By.ID, locator.ID.pick.spinner)))
                 except TimeoutException:
                     spinner = 'invis'
-                if spinner:
+                if spinner == WebElement:
                     invis_spinner = WebDriverWait(self.driver, 30).until(EC.invisibility_of_element_located((By.ID, locator.ID.pick.spinner)))
                     invis_spinner = 'invis'
                 else:
                     spinner = 'invis'
                 if invis_spinner == 'invis':
                     if 'P' in P2:
                         skip_skip()
                     try:
-                        P2 = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.XPATH, locator.xpath.fcmenu.pick.scan_bin.P2))).text
+                        P2 = WebDriverWait(self.driver, 30).until(EC.presence_of_element_located((By.XPATH, locator.xpath.fcmenu.pickUI.scan_bin.P2))).text
                     except TimeoutException:
                         P2 = WebDriverWait(self.driver, 30).until(EC.presence_of_all_elements_located((By.CLASS_NAME, locator.class_name.pick.bin)))
                         P2 = P2[1].text
 
 
         status = bool | str
         select_no_batch()
@@ -843,40 +711,46 @@
             scan_cage(cage)
             check_if_pallet()
             case = ''
             while True:
                 if 'csX' in case:
                     break
                 try:
-                    case = WebDriverWait(self.driver, 5).until(EC.presence_of_element_located((By.XPATH, locator.xpath.fcmenu.pick.scan_bin.case))).text
+                    case = WebDriverWait(self.driver, 5).until(EC.presence_of_element_located((By.XPATH, locator.xpath.fcmenu.pickUI.scan_bin.case))).text
                     break
                 except TimeoutException:
                     skip_skip()
-                    case = WebDriverWait(self.driver, 5).until(EC.presence_of_element_located((By.XPATH, locator.xpath.fcmenu.pick.scan_bin.case))).text
+                    case = WebDriverWait(self.driver, 5).until(EC.presence_of_element_located((By.XPATH, locator.xpath.fcmenu.pickUI.scan_bin.case))).text
 
             switch_to_tab(1)
             self.deleteItem(case)
             switch_to_tab(2)
-            self.move_container(200, case, 'TRASH')
+            self.move_container(200, case, str(deleted_container_to_dz))
             switch_to_tab(0)
-            P1 = self.driver.find_element(By.XPATH, locator.xpath.fcmenu.pick.scan_bin.P1).text
-            P2 = self.driver.find_element(By.XPATH, locator.xpath.fcmenu.pick.scan_bin.P2).text
-            P3 = self.driver.find_element(By.XPATH, locator.xpath.fcmenu.pick.scan_bin.P3).text
+            P1 = self.driver.find_element(By.XPATH, locator.xpath.fcmenu.pickUI.scan_bin.P1).text
+            P2 = self.driver.find_element(By.XPATH, locator.xpath.fcmenu.pickUI.scan_bin.P2).text
+            P3 = self.driver.find_element(By.XPATH, locator.xpath.fcmenu.pickUI.scan_bin.P3).text
             
             bin = P1 + '-' + P2 + P3
 
-            scan(self.driver.find_element(By.XPATH, locator.xpath.fcmenu.pick.scan_bin.input), bin)
-            self.driver.find_element(By.XPATH, locator.xpath.fcmenu.pick.scan_bin.commit).submit()
+            scan(self.driver.find_element(By.XPATH, locator.xpath.fcmenu.pickUI.scan_bin.input), bin)
+            self.driver.find_element(By.XPATH, locator.xpath.fcmenu.pickUI.scan_bin.commit).submit()
             
-            scan(self.driver.find_element(By.XPATH, locator.xpath.fcmenu.pick.scan_case.input), case)
-            self.driver.find_element(By.XPATH, locator.xpath.fcmenu.pick.scan_case.commit).submit()
+            scan(self.driver.find_element(By.XPATH, locator.xpath.fcmenu.pickUI.scan_case.input), case)
+            self.driver.find_element(By.XPATH, locator.xpath.fcmenu.pickUI.scan_case.commit).submit()
             return case
             # print(f'{datetime.now()} // {case} // Deleted')
             
-
+    def PAWS_tradional_picking(self):
+        site = 'https://taskui-gateway-iad.corp.amazon.com/?listingID=97fc5f2d-c627-46cb-afa0-7026e28e34fe&hideTasks=1&messaging=1&fans=1&interrupts=true&training=true&logoutWorkflowEnabled=1&skipTaskCenter=1#initialized'
+        self.navigate(site)
+        body = WebDriverWait(self.driver, 10).until(EC.presence_of_element_located((By.XPATH, locator.body)))
+        WebDriverWait(self.driver, 10).until(EC.presence_of_element_located((By.XPATH, locator.xpath.fcmenu.PAWS_Traditional_Picking.no_batch))).click()
+        body.send_keys('veCG00201')
+        body.send_keys('veCG00201')
         
 
     def move_container(self, workflow: int, container: str, destination: str) -> None:
         """Moves container with Move Container App"""
         move_fails = ['Move was unsuccessful']
         move_URL = f'https://aft-moveapp-iad-iad.iad.proxy.amazon.com/move-container?jobId={workflow}'
         self.navigate(move_URL)
@@ -902,36 +776,50 @@
                         body = self.driver.find_element(By.XPATH, locator.body)
                     except UnexpectedAlertPresentException:
                         try:
                             alert = self.driver.switch_to.alert
                             alert.accept()
                         except NoAlertPresentException:
                             pass
-            self.driver.find_element(By.XPATH, locator.body).send_keys('t')
-            input = self.driver.find_element(By.XPATH, locator.xpath.fcmenu.move_container.input)
-            input.clear()
-            input.click()
-            input.send_keys(container_)
-            input.send_keys(Keys.ENTER)
+            try:
+                body.send_keys('t')
+            except UnboundLocalError:
+                body = self.driver.find_element(By.XPATH, locator.body)
+                body.send_keys('t')
+            try:
+                input = WebDriverWait(self.driver, 5).until(EC.presence_of_element_located((By.XPATH, locator.xpath.fcmenu.move_container.input)))
+                input.clear()
+            except ElementNotInteractableException:
+                body.send_keys('t')
+                input = self.driver.find_element(By.XPATH, locator.xpath.fcmenu.move_container.input)
+
+            if input.is_displayed():
+                input.click()
+                input.send_keys(container_)
+                input.send_keys(Keys.ENTER)
 
         if ready_to_move:
             if workflow == 200:
                 self.navigate(move_URL)
                 enter_container(container)
                 time.sleep(.5)
                 enter_container(destination)
                 time.sleep(.2)
                 msg = self.driver.find_element(By.XPATH, locator.xpath.fcmenu.move_container.error_msg).text
                 print(f'MOVE STATUS: {container} > "{msg}"')
                 if msg in move_fails or msg == '':
                     input = self.driver.find_element(By.XPATH, locator.xpath.fcmenu.move_container.input)
                     for i in range(2):
                         time.sleep(1.2)
-                        input.send_keys(Keys.ENTER)
-                    print(f'{container} TRASHED\n')
+                        try:
+                            input.send_keys(Keys.ENTER)
+                        except ElementNotInteractableException:
+                            self.driver.find_element(By.XPATH, locator.body).send_keys('t')
+                            input.send_keys('t')
+                    print(f'{container} moved\n')
                     time.sleep(.5)
             elif workflow == 300:
                 enter_container(container)
                 for i in range(2):
                     time.sleep(.5)
                     enter_container(destination)
                 time.sleep(1.5)
```

### Comparing `fcmenu-0.0.2/setup.py` & `fcmenu-0.0.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_desc = fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'ICQA / FCMenu automation functions'
 
 # Setting up
 setup(
     name="fcmenu",
     version=VERSION,
     author="Adonis N",
```

