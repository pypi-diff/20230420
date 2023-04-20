# Comparing `tmp/ncbimetadata-0.0.7.tar.gz` & `tmp/ncbimetadata-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncbimetadata-0.0.7.tar", last modified: Thu Apr 20 09:29:35 2023, max compression
+gzip compressed data, was "ncbimetadata-0.0.8.tar", last modified: Thu Apr 20 10:14:53 2023, max compression
```

## Comparing `ncbimetadata-0.0.7.tar` & `ncbimetadata-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 09:29:35.191340 ncbimetadata-0.0.7/
--rw-r--r--   0 taiyuan    (501) staff       (20)     1073 2023-04-20 08:14:16.000000 ncbimetadata-0.0.7/LICENSE
--rw-r--r--   0 taiyuan    (501) staff       (20)     3041 2023-04-20 09:29:35.191226 ncbimetadata-0.0.7/PKG-INFO
--rw-r--r--   0 taiyuan    (501) staff       (20)     1428 2023-04-20 08:14:48.000000 ncbimetadata-0.0.7/README.md
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 09:29:35.189670 ncbimetadata-0.0.7/bin/
--rw-r--r--   0 taiyuan    (501) staff       (20)      152 2023-04-20 08:50:52.000000 ncbimetadata-0.0.7/bin/ncbimetadata
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 09:29:35.190011 ncbimetadata-0.0.7/ncbimetadata/
--rw-r--r--   0 taiyuan    (501) staff       (20)    11112 2023-04-20 08:02:11.000000 ncbimetadata-0.0.7/ncbimetadata/__init__.py
-drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 09:29:35.191064 ncbimetadata-0.0.7/ncbimetadata.egg-info/
--rw-r--r--   0 taiyuan    (501) staff       (20)     3041 2023-04-20 09:29:35.000000 ncbimetadata-0.0.7/ncbimetadata.egg-info/PKG-INFO
--rw-r--r--   0 taiyuan    (501) staff       (20)      282 2023-04-20 09:29:35.000000 ncbimetadata-0.0.7/ncbimetadata.egg-info/SOURCES.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 09:29:35.000000 ncbimetadata-0.0.7/ncbimetadata.egg-info/dependency_links.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 09:29:35.000000 ncbimetadata-0.0.7/ncbimetadata.egg-info/not-zip-safe
--rw-r--r--   0 taiyuan    (501) staff       (20)        9 2023-04-20 09:29:35.000000 ncbimetadata-0.0.7/ncbimetadata.egg-info/requires.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)       13 2023-04-20 09:29:35.000000 ncbimetadata-0.0.7/ncbimetadata.egg-info/top_level.txt
--rw-r--r--   0 taiyuan    (501) staff       (20)       38 2023-04-20 09:29:35.191383 ncbimetadata-0.0.7/setup.cfg
--rw-r--r--   0 taiyuan    (501) staff       (20)      742 2023-04-20 09:29:19.000000 ncbimetadata-0.0.7/setup.py
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 10:14:53.990058 ncbimetadata-0.0.8/
+-rw-r--r--   0 taiyuan    (501) staff       (20)     1073 2023-04-20 08:14:16.000000 ncbimetadata-0.0.8/LICENSE
+-rw-r--r--   0 taiyuan    (501) staff       (20)     3075 2023-04-20 10:14:53.989816 ncbimetadata-0.0.8/PKG-INFO
+-rw-r--r--   0 taiyuan    (501) staff       (20)     1428 2023-04-20 08:14:48.000000 ncbimetadata-0.0.8/README.md
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 10:14:53.987722 ncbimetadata-0.0.8/bin/
+-rw-r--r--   0 taiyuan    (501) staff       (20)      152 2023-04-20 08:50:52.000000 ncbimetadata-0.0.8/bin/ncbimetadata
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 10:14:53.988068 ncbimetadata-0.0.8/ncbimetadata/
+-rw-r--r--   0 taiyuan    (501) staff       (20)    11112 2023-04-20 08:02:11.000000 ncbimetadata-0.0.8/ncbimetadata/__init__.py
+drwxr-xr-x   0 taiyuan    (501) staff       (20)        0 2023-04-20 10:14:53.989544 ncbimetadata-0.0.8/ncbimetadata.egg-info/
+-rw-r--r--   0 taiyuan    (501) staff       (20)     3075 2023-04-20 10:14:53.000000 ncbimetadata-0.0.8/ncbimetadata.egg-info/PKG-INFO
+-rw-r--r--   0 taiyuan    (501) staff       (20)      282 2023-04-20 10:14:53.000000 ncbimetadata-0.0.8/ncbimetadata.egg-info/SOURCES.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 10:14:53.000000 ncbimetadata-0.0.8/ncbimetadata.egg-info/dependency_links.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)        1 2023-04-20 10:14:53.000000 ncbimetadata-0.0.8/ncbimetadata.egg-info/not-zip-safe
+-rw-r--r--   0 taiyuan    (501) staff       (20)        9 2023-04-20 10:14:53.000000 ncbimetadata-0.0.8/ncbimetadata.egg-info/requires.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)       13 2023-04-20 10:14:53.000000 ncbimetadata-0.0.8/ncbimetadata.egg-info/top_level.txt
+-rw-r--r--   0 taiyuan    (501) staff       (20)       38 2023-04-20 10:14:53.990155 ncbimetadata-0.0.8/setup.cfg
+-rw-r--r--   0 taiyuan    (501) staff       (20)      778 2023-04-20 10:14:46.000000 ncbimetadata-0.0.8/setup.py
```

### Comparing `ncbimetadata-0.0.7/LICENSE` & `ncbimetadata-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ncbimetadata-0.0.7/PKG-INFO` & `ncbimetadata-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncbimetadata
-Version: 0.0.7
+Version: 0.0.8
 Summary: ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and more functionalities are on the way!
 Home-page: https://github.com/RyanYuanSun/ncbimetadata
 Author: Ryan Alloriadonis
 Author-email: yuantai78@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Ryan Alloriadonis
@@ -22,14 +22,16 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+Platform: Linux
+Platform: MacOS X
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ncbimetadata
 ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and converting to csv format.
 <hr>
```

### Comparing `ncbimetadata-0.0.7/README.md` & `ncbimetadata-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ncbimetadata-0.0.7/ncbimetadata/__init__.py` & `ncbimetadata-0.0.8/ncbimetadata/__init__.py`

 * *Files identical despite different names*

### Comparing `ncbimetadata-0.0.7/ncbimetadata.egg-info/PKG-INFO` & `ncbimetadata-0.0.8/ncbimetadata.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncbimetadata
-Version: 0.0.7
+Version: 0.0.8
 Summary: ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and more functionalities are on the way!
 Home-page: https://github.com/RyanYuanSun/ncbimetadata
 Author: Ryan Alloriadonis
 Author-email: yuantai78@gmail.com
 License: MIT License
         
         Copyright (c) 2023 Ryan Alloriadonis
@@ -22,14 +22,16 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
+Platform: Linux
+Platform: MacOS X
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ncbimetadata
 ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and converting to csv format.
 <hr>
```

### Comparing `ncbimetadata-0.0.7/setup.py` & `ncbimetadata-0.0.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 def readfile(filename):
     with open(filename, 'r+') as f:
         return f.read()
 
 
 setup(
     name="ncbimetadata",
-    version="0.0.7",
+    version="0.0.8",
     description="ncbimetadata is a package for fast fetching and parsing metadata from ncbi database, and more functionalities are on the way!",
     long_description=readfile('README.md'),
     long_description_content_type='text/markdown',
     author="Ryan Alloriadonis",
     author_email="yuantai78@gmail.com",
     url="https://github.com/RyanYuanSun/ncbimetadata",
+    platforms=['Linux', 'MacOS X'],
     py_modules=['ncbimetadata'],
     packages=['ncbimetadata'],
     license=readfile('LICENSE'),
     scripts=['bin/ncbimetadata'],
     install_requires=[
           'requests',
       ],
```

