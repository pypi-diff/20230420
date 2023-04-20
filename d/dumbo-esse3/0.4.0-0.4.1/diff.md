# Comparing `tmp/dumbo_esse3-0.4.0.tar.gz` & `tmp/dumbo_esse3-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dumbo_esse3-0.4.0.tar", max compression
+gzip compressed data, was "dumbo_esse3-0.4.1.tar", max compression
```

## Comparing `dumbo_esse3-0.4.0.tar` & `dumbo_esse3-0.4.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2022-09-11 08:55:51.265066 dumbo_esse3-0.4.0/LICENSE
--rw-r--r--   0        0        0        0 2022-09-11 07:49:43.077054 dumbo_esse3-0.4.0/dumbo_esse3/__init__.py
--rw-r--r--   0        0        0      101 2023-01-18 08:46:22.755370 dumbo_esse3-0.4.0/dumbo_esse3/__main__.py
--rwxr-xr-x   0        0        0    22679 2023-02-03 22:51:06.785031 dumbo_esse3-0.4.0/dumbo_esse3/cli.py
--rw-r--r--   0        0        0    22816 2023-02-04 00:40:23.866498 dumbo_esse3-0.4.0/dumbo_esse3/esse3_wrapper.py
--rw-r--r--   0        0        0    10306 2023-02-03 22:04:42.668983 dumbo_esse3-0.4.0/dumbo_esse3/primitives.py
--rw-r--r--   0        0        0      515 2023-02-04 00:42:42.230532 dumbo_esse3-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 dumbo_esse3-0.4.0/setup.py
--rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 dumbo_esse3-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-09-11 08:55:51.265066 dumbo_esse3-0.4.1/LICENSE
+-rw-r--r--   0        0        0        0 2022-09-11 07:49:43.077054 dumbo_esse3-0.4.1/dumbo_esse3/__init__.py
+-rw-r--r--   0        0        0      101 2023-01-18 08:46:22.755370 dumbo_esse3-0.4.1/dumbo_esse3/__main__.py
+-rwxr-xr-x   0        0        0    22679 2023-02-03 22:51:06.785031 dumbo_esse3-0.4.1/dumbo_esse3/cli.py
+-rw-r--r--   0        0        0    23044 2023-04-20 16:08:42.523435 dumbo_esse3-0.4.1/dumbo_esse3/esse3_wrapper.py
+-rw-r--r--   0        0        0    10306 2023-02-03 22:04:42.668983 dumbo_esse3-0.4.1/dumbo_esse3/primitives.py
+-rw-r--r--   0        0        0      515 2023-04-20 16:12:06.099681 dumbo_esse3-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      740 1970-01-01 00:00:00.000000 dumbo_esse3-0.4.1/setup.py
+-rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 dumbo_esse3-0.4.1/PKG-INFO
```

### Comparing `dumbo_esse3-0.4.0/LICENSE` & `dumbo_esse3-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dumbo_esse3-0.4.0/dumbo_esse3/cli.py` & `dumbo_esse3-0.4.1/dumbo_esse3/cli.py`

 * *Files identical despite different names*

### Comparing `dumbo_esse3-0.4.0/dumbo_esse3/esse3_wrapper.py` & `dumbo_esse3-0.4.1/dumbo_esse3/esse3_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,16 +322,14 @@
         validate("at least one student", student_graduation_list, min_len=1, help_msg="No student was provided")
         self.driver.get(URLs["graduation_day_list"])
         self.driver.find_element(
             By.XPATH,
             f"//table[@id = 'seduteAperte']/tbody/tr/td[text() = '{graduation_day}']/../td/a"
         ).send_keys(Keys.RETURN)
 
-        # PAGINATION MUST BE HANDLED AS FOR COMMITTEE EVALUATIONS
-
         html_document = html.fromstring(self.driver.page_source)
         rows = html_document.xpath('//table[@id="elencoLaureandi"]/tbody/tr')
         student_to_url = {
             Student.of(
                 student_id=row.xpath("td[2]")[0].text,
                 student_name=row.xpath("td[1]")[0].text,
             ): ESSE3_SERVER + '/' + row.xpath("td/a/@href")[0]
@@ -368,25 +366,26 @@
             thesis_score = graduation.final_score.value - starting_score
             validate("thesis_score", thesis_score, min_value=1, max_value=15, help_msg="Wrong thesis score")
 
             self.__replace_content(
                 self.driver.find_element(By.ID, 'grad-dettLau-annotazioni'),
                 graduation.notes.value
             )
+            self.driver.execute_script("arguments[0].setAttribute('onchange', () => {})", self.driver.find_element(By.ID, 'grad-dettLau-puntiTesi'))
             self.__replace_content(
                 self.driver.find_element(By.ID, 'grad-dettLau-puntiTesi'),
                 str(thesis_score)
             )
             self.__replace_content(
                 self.driver.find_element(By.ID, 'grad-dettLau-dataCt'),
                 graduation_date
             )
-            if graduation.laude:
+            if graduation.laude != self.driver.find_element(By.ID, 'grad-dettLau-lode1').is_selected():
                 self.driver.find_element(By.ID, 'grad-dettLau-lode1').send_keys(Keys.SPACE)
-            if graduation.special_mention:
+            if graduation.special_mention != self.driver.find_element(By.ID, 'grad-dettLau-menzione1').is_selected():
                 self.driver.find_element(By.ID, 'grad-dettLau-menzione1').send_keys(Keys.SPACE)
 
             if committee:
                 checkboxes = self.driver.find_elements(
                     By.XPATH,
                     '//table[starts-with(@id, "gradDettLauCommissione")]//input[@type = "checkbox"]'
                 )
```

### Comparing `dumbo_esse3-0.4.0/dumbo_esse3/primitives.py` & `dumbo_esse3-0.4.1/dumbo_esse3/primitives.py`

 * *Files identical despite different names*

### Comparing `dumbo_esse3-0.4.0/pyproject.toml` & `dumbo_esse3-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dumbo-esse3"
-version = "0.4.0"
+version = "0.4.1"
 description = "Esse3 command line utility, to save my future time!"
 authors = ["Mario Alviano <mario.alviano@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 dateutils = "^0.6.12"
 dumbo-utils = "^0.1.4"
```

### Comparing `dumbo_esse3-0.4.0/setup.py` & `dumbo_esse3-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['dateutils>=0.6.12,<0.7.0',
  'dumbo-utils>=0.1.4,<0.2.0',
  'lxml>=4.9.2,<5.0.0',
  'selenium>=4.4.3,<5.0.0']
 
 setup_kwargs = {
     'name': 'dumbo-esse3',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': 'Esse3 command line utility, to save my future time!',
     'long_description': 'None',
     'author': 'Mario Alviano',
     'author_email': 'mario.alviano@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dumbo_esse3-0.4.0/PKG-INFO` & `dumbo_esse3-0.4.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dumbo-esse3
-Version: 0.4.0
+Version: 0.4.1
 Summary: Esse3 command line utility, to save my future time!
 Author: Mario Alviano
 Author-email: mario.alviano@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

