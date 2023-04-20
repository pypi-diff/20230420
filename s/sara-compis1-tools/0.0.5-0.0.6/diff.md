# Comparing `tmp/sara_compis1_tools-0.0.5.tar.gz` & `tmp/sara_compis1_tools-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sara_compis1_tools-0.0.5.tar", last modified: Wed Apr 19 20:42:32 2023, max compression
+gzip compressed data, was "sara_compis1_tools-0.0.6.tar", last modified: Thu Apr 20 00:11:06 2023, max compression
```

## Comparing `sara_compis1_tools-0.0.5.tar` & `sara_compis1_tools-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 20:42:32.712366 sara_compis1_tools-0.0.5/
--rw-rw-rw-   0        0        0      138 2023-04-19 20:39:04.000000 sara_compis1_tools-0.0.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1059 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0       26 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      748 2023-04-19 20:42:32.709318 sara_compis1_tools-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      101 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.5/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-19 20:42:32.682981 sara_compis1_tools-0.0.5/sara_compis1_tools/
--rw-rw-rw-   0        0        0     6072 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.5/sara_compis1_tools/Format.py
--rw-rw-rw-   0        0        0      216 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.5/sara_compis1_tools/StateAFD.py
--rw-rw-rw-   0        0        0     1502 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.5/sara_compis1_tools/Syntax.py
--rw-rw-rw-   0        0        0     1167 2023-04-19 20:23:20.000000 sara_compis1_tools-0.0.5/sara_compis1_tools/Visualizer.py
--rw-rw-rw-   0        0        0        0 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.5/sara_compis1_tools/__init__.py
--rw-rw-rw-   0        0        0    18584 2023-04-19 20:04:32.000000 sara_compis1_tools-0.0.5/sara_compis1_tools/directAFD.py
--rw-rw-rw-   0        0        0     1929 2023-04-19 20:29:35.000000 sara_compis1_tools-0.0.5/sara_compis1_tools/generated.py
--rw-rw-rw-   0        0        0    13324 2023-04-19 20:28:45.000000 sara_compis1_tools-0.0.5/sara_compis1_tools/lexGen.py
-drwxrwxrwx   0        0        0        0 2023-04-19 20:42:32.705015 sara_compis1_tools-0.0.5/sara_compis1_tools.egg-info/
--rw-rw-rw-   0        0        0      748 2023-04-19 20:42:32.000000 sara_compis1_tools-0.0.5/sara_compis1_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      532 2023-04-19 20:42:32.000000 sara_compis1_tools-0.0.5/sara_compis1_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 20:42:32.000000 sara_compis1_tools-0.0.5/sara_compis1_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-19 20:42:32.000000 sara_compis1_tools-0.0.5/sara_compis1_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-19 20:42:32.000000 sara_compis1_tools-0.0.5/sara_compis1_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 20:42:32.713594 sara_compis1_tools-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      766 2023-04-19 20:39:31.000000 sara_compis1_tools-0.0.5/setup.py
--rw-rw-rw-   0        0        0     1948 2023-04-19 18:13:23.000000 sara_compis1_tools-0.0.5/stateafd_objects.py
+drwxrwxrwx   0        0        0        0 2023-04-20 00:11:06.188101 sara_compis1_tools-0.0.6/
+-rw-rw-rw-   0        0        0      215 2023-04-20 00:02:21.000000 sara_compis1_tools-0.0.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1059 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      829 2023-04-20 00:11:06.186531 sara_compis1_tools-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      101 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.6/README.txt
+-rw-rw-rw-   0        0        0     1441 2023-04-19 23:26:29.000000 sara_compis1_tools-0.0.6/generated.py
+drwxrwxrwx   0        0        0        0 2023-04-20 00:11:06.161867 sara_compis1_tools-0.0.6/sara_compis1_tools/
+-rw-rw-rw-   0        0        0     6072 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.6/sara_compis1_tools/Format.py
+-rw-rw-rw-   0        0        0      255 2023-04-19 23:59:19.000000 sara_compis1_tools-0.0.6/sara_compis1_tools/StateAFD.py
+-rw-rw-rw-   0        0        0     1502 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.6/sara_compis1_tools/Syntax.py
+-rw-rw-rw-   0        0        0     1167 2023-04-19 20:23:20.000000 sara_compis1_tools-0.0.6/sara_compis1_tools/Visualizer.py
+-rw-rw-rw-   0        0        0        0 2023-04-09 06:54:43.000000 sara_compis1_tools-0.0.6/sara_compis1_tools/__init__.py
+-rw-rw-rw-   0        0        0    18584 2023-04-19 20:04:32.000000 sara_compis1_tools-0.0.6/sara_compis1_tools/directAFD.py
+-rw-rw-rw-   0        0        0     1618 2023-04-20 00:00:07.000000 sara_compis1_tools-0.0.6/sara_compis1_tools/generated.py
+-rw-rw-rw-   0        0        0    14271 2023-04-20 00:00:00.000000 sara_compis1_tools-0.0.6/sara_compis1_tools/lexGen.py
+-rw-rw-rw-   0        0        0     1937 2023-04-20 00:05:56.000000 sara_compis1_tools-0.0.6/sara_compis1_tools/stateafd_objects.py
+drwxrwxrwx   0        0        0        0 2023-04-20 00:11:06.181465 sara_compis1_tools-0.0.6/sara_compis1_tools.egg-info/
+-rw-rw-rw-   0        0        0      829 2023-04-20 00:11:05.000000 sara_compis1_tools-0.0.6/sara_compis1_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2023-04-20 00:11:06.000000 sara_compis1_tools-0.0.6/sara_compis1_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 00:11:05.000000 sara_compis1_tools-0.0.6/sara_compis1_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-20 00:11:05.000000 sara_compis1_tools-0.0.6/sara_compis1_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-20 00:11:05.000000 sara_compis1_tools-0.0.6/sara_compis1_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 00:11:06.188101 sara_compis1_tools-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      766 2023-04-20 00:02:31.000000 sara_compis1_tools-0.0.6/setup.py
+-rw-rw-rw-   0        0        0     1948 2023-04-19 18:13:23.000000 sara_compis1_tools-0.0.6/stateafd_objects.py
```

### Comparing `sara_compis1_tools-0.0.5/LICENSE.txt` & `sara_compis1_tools-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.5/PKG-INFO` & `sara_compis1_tools-0.0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sara_compis1_tools
-Version: 0.0.5
+Version: 0.0.6
 Summary: A collection of tools for the Language Design course
 Home-page: https://github.com/MGonza20/Compis_Lab4
 Author: Sara Paguaga
 Author-email: sara.paguaga@gmail.com
 License: MIT
 Keywords: Compiler
 Classifier: Development Status :: 3 - Alpha
@@ -21,7 +21,11 @@
 0.0.4 (08/04/2023)
 ------------------
 - More fixes.
 
 0.0.5 (19/04/2023)
 ------------------
 - Rearranging packages.
+
+0.0.6 (19/04/2023)
+------------------
+- More fields for the StateAFD class.
```

### Comparing `sara_compis1_tools-0.0.5/sara_compis1_tools/Format.py` & `sara_compis1_tools-0.0.6/sara_compis1_tools/Format.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.5/sara_compis1_tools/Syntax.py` & `sara_compis1_tools-0.0.6/sara_compis1_tools/Syntax.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.5/sara_compis1_tools/Visualizer.py` & `sara_compis1_tools-0.0.6/sara_compis1_tools/Visualizer.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.5/sara_compis1_tools/directAFD.py` & `sara_compis1_tools-0.0.6/sara_compis1_tools/directAFD.py`

 * *Files identical despite different names*

### Comparing `sara_compis1_tools-0.0.5/sara_compis1_tools/generated.py` & `sara_compis1_tools-0.0.6/sara_compis1_tools/stateafd_objects.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,5 @@
 from StateAFD import StateAFD
-from Visualizer import Visualizer
-
-mega = [StateAFD(name='init',transitions={'949': 'A'},accepting=False,start=True),StateAFD(name='A',transitions={'032': 'B', '009': 'B', '010': 'B'},accepting=False,start=False),StateAFD(name='B',transitions={},accepting=True,start=False),StateAFD(name='init',transitions={'949': 'C'},accepting=False,start=True),StateAFD(name='C',transitions={'032': 'D', '009': 'D', '010': 'D'},accepting=False,start=False),StateAFD(name='D',transitions={'032': 'D', '009': 'D', '010': 'D'},accepting=True,start=False),StateAFD(name='init',transitions={'949': 'E'},accepting=False,start=True),StateAFD(name='E',transitions={'048': 'F', '049': 'F', '050': 'F', '051': 'F'},accepting=False,start=False),StateAFD(name='F',transitions={},accepting=True,start=False),StateAFD(name='init',transitions={'949': 'G'},accepting=False,start=True),StateAFD(name='G',transitions={'045': 'H', '048': 'I', '049': 'I', '050': 'I', '051': 'I'},accepting=False,start=False),StateAFD(name='H',transitions={'048': 'I', '049': 'I', '050': 'I', '051': 'I'},accepting=False,start=False),StateAFD(name='I',transitions={'048': 'I', '049': 'I', '050': 'I', '051': 'I'},accepting=True,start=False),StateAFD(name='init',transitions={'949': 'J'},accepting=False,start=True),StateAFD(name='J',transitions={'097': 'K', '098': 'K', '099': 'K', '065': 'K', '066': 'K', '067': 'K'},accepting=False,start=False),StateAFD(name='K',transitions={},accepting=True,start=False),StateAFD(name='init',transitions={'949': 'L'},accepting=False,start=True),StateAFD(name='L',transitions={'097': 'M', '098': 'M', '099': 'M', '065': 'M', '066': 'M', '067': 'M'},accepting=False,start=False),StateAFD(name='M',transitions={'097': 'M', '098': 'M', '099': 'M', '065': 'M', '066': 'M', '067': 'M', '048': 'M', '049': 'M', '050': 'M', '051': 'M'},accepting=True,start=False)]
-
-visual = Visualizer()
-visual.draw_mega_afd(mega)
+from lexGen import Lexer
+stateafd_data = [StateAFD(name='init',transitions={'949': 'A'},accepting=False,start=True),StateAFD(name='A',transitions={'032': 'B', '009': 'B', '010': 'B'},accepting=False,start=False),StateAFD(name='B',transitions={},accepting=True,start=False),StateAFD(name='init',transitions={'949': 'C'},accepting=False,start=True),StateAFD(name='C',transitions={'032': 'D', '009': 'D', '010': 'D'},accepting=False,start=False),StateAFD(name='D',transitions={'032': 'D', '009': 'D', '010': 'D'},accepting=True,start=False),StateAFD(name='init',transitions={'949': 'E'},accepting=False,start=True),StateAFD(name='E',transitions={'048': 'F', '049': 'F', '050': 'F', '051': 'F'},accepting=False,start=False),StateAFD(name='F',transitions={},accepting=True,start=False),StateAFD(name='init',transitions={'949': 'G'},accepting=False,start=True),StateAFD(name='G',transitions={'045': 'H', '048': 'I', '049': 'I', '050': 'I', '051': 'I'},accepting=False,start=False),StateAFD(name='H',transitions={'048': 'I', '049': 'I', '050': 'I', '051': 'I'},accepting=False,start=False),StateAFD(name='I',transitions={'048': 'I', '049': 'I', '050': 'I', '051': 'I'},accepting=True,start=False),StateAFD(name='init',transitions={'949': 'J'},accepting=False,start=True),StateAFD(name='J',transitions={'097': 'K', '098': 'K', '099': 'K', '065': 'K', '066': 'K', '067': 'K'},accepting=False,start=False),StateAFD(name='K',transitions={},accepting=True,start=False),StateAFD(name='init',transitions={'949': 'L'},accepting=False,start=True),StateAFD(name='L',transitions={'097': 'M', '098': 'M', '099': 'M', '065': 'M', '066': 'M', '067': 'M'},accepting=False,start=False),StateAFD(name='M',transitions={'097': 'M', '098': 'M', '099': 'M', '065': 'M', '066': 'M', '067': 'M', '048': 'M', '049': 'M', '050': 'M', '051': 'M'},accepting=True,start=False)]
+lexerr = Lexer('p1.yal')
+lexerr.draw_mega_afd(stateafd_data)
```

### Comparing `sara_compis1_tools-0.0.5/sara_compis1_tools/lexGen.py` & `sara_compis1_tools-0.0.6/sara_compis1_tools/lexGen.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 
 class Token:
         def __init__(self, name):
             self.name = name
             self.regex = None
             self.line_no = None
+            self.value = None
     
         def __str__(self):
             return f"Token({self.name}, {self.regex})"
 
 
 class Lexer:
     def __init__(self, filename):
@@ -142,16 +143,16 @@
 
                     if not inside:
                         name += rule[i]
                     else:
                         value += rule[i]
 
                 if name:
-                    name = name[1:-1] if name[0] == "'" and name[-1] == "'" else name 
                     rules_dict[name] = value.strip()
+        return rules_dict
 
 
     def getTokens(self):
         lines = self.getLines()[0]
         for line_no, line in enumerate(lines, start=1):
             # generando tokens
             if line[:3] == 'let':
@@ -310,25 +311,45 @@
                 i += 1
         return output
 
     
     def generate_automatas(self):
         mega_content = []
         count = 0
+        return_values = self.assign_values()
+        done = []
         for token in self.tokens:
-            ff = Format(token.regex)
-            token.regex = ff.positiveId(token.regex + '#')
-            token.regex = ff.zeroOrOneId(token.regex)
-            token.regex = self.remove_double_parentheses(token.regex)
-            token.regex = ff.concat(token.regex)
-            
-            afdd = AFD(token)
-            new_afd = afdd.generateAFD(count)
-            mega_content.append(new_afd)
-            count += len(new_afd)
+            if token.name in return_values:
+                ff = Format(token.regex)
+                token.regex = ff.positiveId(token.regex + '#')
+                token.regex = ff.zeroOrOneId(token.regex)
+                token.regex = self.remove_double_parentheses(token.regex)
+                token.regex = ff.concat(token.regex)
+                token.value = return_values[token.name]
+                done.append(token.name)
+                
+                afdd = AFD(token)
+                new_afd = afdd.generateAFD(count)
+                mega_content.append(new_afd)
+                count += len(new_afd)
+
+        for value in return_values:
+            if len(value) == 3 and value[0] == "'" and value[2] == "'" and value not in done:
+                lenn = len(value)
+                token = Token(name=value[1:-1])
+                token.regex = value + '#'
+                token.value = return_values[value]
+                ff = Format(token.regex)
+                token.regex = ff.concat(token.regex)
+                done.append(token.name)
+                
+                afdd = AFD(token)
+                new_afd = afdd.generateAFD(count)
+                mega_content.append(new_afd)
+                count += len(new_afd)
         return mega_content
     
 
     def unify(self, mega_content):
         stack = []    
         for element in mega_content:
             for state in element:
@@ -349,31 +370,32 @@
         self.replace_tokens()
     
 
 
     
 if __name__ == '__main__':
 
-    if len(sys.argv) < 2:
-        print("Por favor ingrese el archivo .yal")
-        sys.exit(1)
+    # if len(sys.argv) < 2:
+    #     print("Por favor ingrese el archivo .yal")
+    #     sys.exit(1)
 
-    yal_file = sys.argv[1]
+    # yal_file = sys.argv[1]
+    yal_file = "p1.yal"
     lexer = Lexer(yal_file)
     
     lexer.read()
     mega_content = lexer.generate_automatas()
     mega_automata = lexer.unify(mega_content)
 
     with open('generated.py', 'w') as file:
-        file.write("from StateAFD import StateAFD\n")
-        file.write("from Visualizer import Visualizer\n\n")
+        file.write("from sara_compis1_tools.StateAFD import StateAFD\n")
+        file.write("from sara_compis1_tools.Visualizer import Visualizer\n\n")
         file.write("mega = [")
         for i, obj in enumerate(mega_automata):
-            file.write(f"StateAFD(name='{obj.name}',transitions={obj.transitions},accepting={obj.accepting},start={obj.start})")
+            file.write(f"StateAFD(name='{obj.name}',transitions={obj.transitions},accepting={obj.accepting},start={obj.start}, value={obj.value})")
             if i != len(mega_automata) - 1:
                 file.write(",") 
         file.write("]\n\n")
 
         file.write("visual = Visualizer()\n")
         file.write("visual.draw_mega_afd(mega)")
```

### Comparing `sara_compis1_tools-0.0.5/sara_compis1_tools.egg-info/PKG-INFO` & `sara_compis1_tools-0.0.6/sara_compis1_tools.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sara-compis1-tools
-Version: 0.0.5
+Version: 0.0.6
 Summary: A collection of tools for the Language Design course
 Home-page: https://github.com/MGonza20/Compis_Lab4
 Author: Sara Paguaga
 Author-email: sara.paguaga@gmail.com
 License: MIT
 Keywords: Compiler
 Classifier: Development Status :: 3 - Alpha
@@ -21,7 +21,11 @@
 0.0.4 (08/04/2023)
 ------------------
 - More fixes.
 
 0.0.5 (19/04/2023)
 ------------------
 - Rearranging packages.
+
+0.0.6 (19/04/2023)
+------------------
+- More fields for the StateAFD class.
```

### Comparing `sara_compis1_tools-0.0.5/sara_compis1_tools.egg-info/SOURCES.txt` & `sara_compis1_tools-0.0.6/sara_compis1_tools.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 CHANGELOG.txt
 LICENSE.txt
 MANIFEST.in
 README.txt
+generated.py
 setup.py
 stateafd_objects.py
 sara_compis1_tools/Format.py
 sara_compis1_tools/StateAFD.py
 sara_compis1_tools/Syntax.py
 sara_compis1_tools/Visualizer.py
 sara_compis1_tools/__init__.py
 sara_compis1_tools/directAFD.py
 sara_compis1_tools/generated.py
 sara_compis1_tools/lexGen.py
+sara_compis1_tools/stateafd_objects.py
 sara_compis1_tools.egg-info/PKG-INFO
 sara_compis1_tools.egg-info/SOURCES.txt
 sara_compis1_tools.egg-info/dependency_links.txt
 sara_compis1_tools.egg-info/requires.txt
 sara_compis1_tools.egg-info/top_level.txt
```

### Comparing `sara_compis1_tools-0.0.5/setup.py` & `sara_compis1_tools-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sara_compis1_tools',
-    version='0.0.5',
+    version='0.0.6',
     description='A collection of tools for the Language Design course',
     long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
     url='https://github.com/MGonza20/Compis_Lab4',
     author='Sara Paguaga',
     author_email='sara.paguaga@gmail.com',
     license='MIT',
     classifiers=[
```

### Comparing `sara_compis1_tools-0.0.5/stateafd_objects.py` & `sara_compis1_tools-0.0.6/stateafd_objects.py`

 * *Files identical despite different names*

