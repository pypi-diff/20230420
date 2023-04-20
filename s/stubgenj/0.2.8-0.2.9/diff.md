# Comparing `tmp/stubgenj-0.2.8.tar.gz` & `tmp/stubgenj-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/scripting-tools/stubgenj/dist/.tmp-y9ls4hjl/stubgenj-0.2.8.tar", last modified: Tue Dec  6 10:52:39 2022, max compression
+gzip compressed data, was "/builds/scripting-tools/stubgenj/dist/.tmp-_4uozbeo/stubgenj-0.2.9.tar", last modified: Wed Dec 14 15:10:21 2022, max compression
```

## Comparing `stubgenj-0.2.8.tar` & `stubgenj-0.2.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 10:52:39.000000 stubgenj-0.2.8/
--rw-r--r--   0 root         (0) root         (0)       92 2022-12-06 10:52:12.000000 stubgenj-0.2.8/.gitignore
--rw-r--r--   0 root         (0) root         (0)      936 2022-12-06 10:52:12.000000 stubgenj-0.2.8/.gitlab-ci.yml
--rw-r--r--   0 root         (0) root         (0)     1152 2022-12-06 10:52:12.000000 stubgenj-0.2.8/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     3119 2022-12-06 10:52:39.000000 stubgenj-0.2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2571 2022-12-06 10:52:12.000000 stubgenj-0.2.8/README.md
--rw-r--r--   0 root         (0) root         (0)      407 2022-12-06 10:52:12.000000 stubgenj-0.2.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-06 10:52:39.000000 stubgenj-0.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1561 2022-12-06 10:52:12.000000 stubgenj-0.2.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 10:52:39.000000 stubgenj-0.2.8/stubgenj/
--rw-r--r--   0 root         (0) root         (0)       86 2022-12-06 10:52:12.000000 stubgenj-0.2.8/stubgenj/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2591 2022-12-06 10:52:12.000000 stubgenj-0.2.8/stubgenj/__main__.py
--rw-r--r--   0 root         (0) root         (0)    56680 2022-12-06 10:52:12.000000 stubgenj-0.2.8/stubgenj/_stubgenj.py
--rw-r--r--   0 root         (0) root         (0)      176 2022-12-06 10:52:39.000000 stubgenj-0.2.8/stubgenj/_version.py
--rw-r--r--   0 root         (0) root         (0)      520 2022-12-06 10:52:12.000000 stubgenj-0.2.8/stubgenj/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 10:52:39.000000 stubgenj-0.2.8/stubgenj/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-06 10:52:13.000000 stubgenj-0.2.8/stubgenj/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 10:52:39.000000 stubgenj-0.2.8/stubgenj/tests/stubtest/
--rw-r--r--   0 root         (0) root         (0)      246 2022-12-06 10:52:12.000000 stubgenj-0.2.8/stubgenj/tests/stubtest/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 10:52:39.000000 stubgenj-0.2.8/stubgenj/tests/stubtest/test-data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 10:52:39.000000 stubgenj-0.2.8/stubgenj/tests/stubtest/test-data/unit/
--rw-r--r--   0 root         (0) root         (0)      817 2022-12-06 10:52:12.000000 stubgenj-0.2.8/stubgenj/tests/stubtest/test-data/unit/arraylist.test
--rw-r--r--   0 root         (0) root         (0)     3135 2022-12-06 10:52:12.000000 stubgenj-0.2.8/stubgenj/tests/stubtest/test-data/unit/callbacks.test
--rw-r--r--   0 root         (0) root         (0)      753 2022-12-06 10:52:12.000000 stubgenj-0.2.8/stubgenj/tests/stubtest/test-data/unit/enummap.test
--rw-r--r--   0 root         (0) root         (0)      221 2022-12-06 10:52:12.000000 stubgenj-0.2.8/stubgenj/tests/stubtest/test-data/unit/forward_declaration.test
--rw-r--r--   0 root         (0) root         (0)      969 2022-12-06 10:52:12.000000 stubgenj-0.2.8/stubgenj/tests/stubtest/test-data/unit/hashmap.test
--rw-r--r--   0 root         (0) root         (0)      530 2022-12-06 10:52:12.000000 stubgenj-0.2.8/stubgenj/tests/stubtest/test-data/unit/jpype_jpackage.test
--rw-r--r--   0 root         (0) root         (0)      394 2022-12-06 10:52:12.000000 stubgenj-0.2.8/stubgenj/tests/stubtest/test-data/unit/mangled_python_keywords.test
--rw-r--r--   0 root         (0) root         (0)      638 2022-12-06 10:52:12.000000 stubgenj-0.2.8/stubgenj/tests/stubtest/test-data/unit/varargs.test
--rw-r--r--   0 root         (0) root         (0)     1629 2022-12-06 10:52:12.000000 stubgenj-0.2.8/stubgenj/tests/test_stubtest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-06 10:52:39.000000 stubgenj-0.2.8/stubgenj.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3119 2022-12-06 10:52:39.000000 stubgenj-0.2.8/stubgenj.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      884 2022-12-06 10:52:39.000000 stubgenj-0.2.8/stubgenj.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-06 10:52:39.000000 stubgenj-0.2.8/stubgenj.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      289 2022-12-06 10:52:39.000000 stubgenj-0.2.8/stubgenj.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-12-06 10:52:39.000000 stubgenj-0.2.8/stubgenj.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 15:10:21.000000 stubgenj-0.2.9/
+-rw-r--r--   0 root         (0) root         (0)       92 2022-12-14 15:10:00.000000 stubgenj-0.2.9/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      936 2022-12-14 15:10:00.000000 stubgenj-0.2.9/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)     1152 2022-12-14 15:10:00.000000 stubgenj-0.2.9/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     3119 2022-12-14 15:10:21.000000 stubgenj-0.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2571 2022-12-14 15:10:00.000000 stubgenj-0.2.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      407 2022-12-14 15:10:00.000000 stubgenj-0.2.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2022-12-14 15:10:21.000000 stubgenj-0.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1561 2022-12-14 15:10:00.000000 stubgenj-0.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 15:10:21.000000 stubgenj-0.2.9/stubgenj/
+-rw-r--r--   0 root         (0) root         (0)       86 2022-12-14 15:10:00.000000 stubgenj-0.2.9/stubgenj/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2591 2022-12-14 15:10:00.000000 stubgenj-0.2.9/stubgenj/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    56983 2022-12-14 15:10:00.000000 stubgenj-0.2.9/stubgenj/_stubgenj.py
+-rw-r--r--   0 root         (0) root         (0)      176 2022-12-14 15:10:21.000000 stubgenj-0.2.9/stubgenj/_version.py
+-rw-r--r--   0 root         (0) root         (0)      520 2022-12-14 15:10:00.000000 stubgenj-0.2.9/stubgenj/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 15:10:21.000000 stubgenj-0.2.9/stubgenj/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-14 15:10:00.000000 stubgenj-0.2.9/stubgenj/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 15:10:21.000000 stubgenj-0.2.9/stubgenj/tests/stubtest/
+-rw-r--r--   0 root         (0) root         (0)      246 2022-12-14 15:10:00.000000 stubgenj-0.2.9/stubgenj/tests/stubtest/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 15:10:21.000000 stubgenj-0.2.9/stubgenj/tests/stubtest/test-data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 15:10:21.000000 stubgenj-0.2.9/stubgenj/tests/stubtest/test-data/unit/
+-rw-r--r--   0 root         (0) root         (0)      817 2022-12-14 15:10:00.000000 stubgenj-0.2.9/stubgenj/tests/stubtest/test-data/unit/arraylist.test
+-rw-r--r--   0 root         (0) root         (0)     3135 2022-12-14 15:10:00.000000 stubgenj-0.2.9/stubgenj/tests/stubtest/test-data/unit/callbacks.test
+-rw-r--r--   0 root         (0) root         (0)      753 2022-12-14 15:10:00.000000 stubgenj-0.2.9/stubgenj/tests/stubtest/test-data/unit/enummap.test
+-rw-r--r--   0 root         (0) root         (0)      221 2022-12-14 15:10:00.000000 stubgenj-0.2.9/stubgenj/tests/stubtest/test-data/unit/forward_declaration.test
+-rw-r--r--   0 root         (0) root         (0)      969 2022-12-14 15:10:00.000000 stubgenj-0.2.9/stubgenj/tests/stubtest/test-data/unit/hashmap.test
+-rw-r--r--   0 root         (0) root         (0)      530 2022-12-14 15:10:00.000000 stubgenj-0.2.9/stubgenj/tests/stubtest/test-data/unit/jpype_jpackage.test
+-rw-r--r--   0 root         (0) root         (0)      394 2022-12-14 15:10:00.000000 stubgenj-0.2.9/stubgenj/tests/stubtest/test-data/unit/mangled_python_keywords.test
+-rw-r--r--   0 root         (0) root         (0)      638 2022-12-14 15:10:00.000000 stubgenj-0.2.9/stubgenj/tests/stubtest/test-data/unit/varargs.test
+-rw-r--r--   0 root         (0) root         (0)     1629 2022-12-14 15:10:00.000000 stubgenj-0.2.9/stubgenj/tests/test_stubtest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 15:10:21.000000 stubgenj-0.2.9/stubgenj.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3119 2022-12-14 15:10:21.000000 stubgenj-0.2.9/stubgenj.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      884 2022-12-14 15:10:21.000000 stubgenj-0.2.9/stubgenj.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-14 15:10:21.000000 stubgenj-0.2.9/stubgenj.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      289 2022-12-14 15:10:21.000000 stubgenj-0.2.9/stubgenj.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2022-12-14 15:10:21.000000 stubgenj-0.2.9/stubgenj.egg-info/top_level.txt
```

### Comparing `stubgenj-0.2.8/.gitlab-ci.yml` & `stubgenj-0.2.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `stubgenj-0.2.8/LICENSE.txt` & `stubgenj-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stubgenj-0.2.8/PKG-INFO` & `stubgenj-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stubgenj
-Version: 0.2.8
+Version: 0.2.9
 Summary: PEP-484 python stub generator for Java classes accessed through JPype
 Home-page: https://gitlab.cern.ch/scripting-tools/stubgenj
 Maintainer: CERN Accelerating Python
 Maintainer-email: acc-py-support@cern.ch
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `stubgenj-0.2.8/README.md` & `stubgenj-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `stubgenj-0.2.8/setup.py` & `stubgenj-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `stubgenj-0.2.8/stubgenj/__main__.py` & `stubgenj-0.2.9/stubgenj/__main__.py`

 * *Files identical despite different names*

### Comparing `stubgenj-0.2.8/stubgenj/_stubgenj.py` & `stubgenj-0.2.9/stubgenj/_stubgenj.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,32 +76,32 @@
 class Javadoc:
     description: str
     ctors: str = ''
     methods: Dict[str, str] = dataclasses.field(default_factory=dict)
     fields: Dict[str, str] = dataclasses.field(default_factory=dict)
 
 
-def isEmptyPseudoPackage(package: jpype.JPackage) -> bool:
+def isPseudoPackage(package: jpype.JPackage) -> bool:
     """
     Return True if the package is an (empty) "pseudo package" - a package that neither contains classes,
     nor sub-packages.
 
     Such packages are not importable in Java. Still, JPype can generate them e.g. for directories that are only present
     in Javadoc JARs but not in source JARs (e.g. "class-use" in Guava)
     """
-    return len(dir(package)) == 0
+    return len(dir(package)) == 0 or '$' in package.__name__
 
 
 def packageAndSubPackages(package: jpype.JPackage) -> Generator[jpype.JPackage, None, None]:
     """ Walk the java package tree and collect all packages in the JVM which are descendants of the given package. """
     yield package
     for name in dir(package):
         try:
             item = getattr(package, name)
-            if isinstance(item, jpype.JPackage) and not isEmptyPseudoPackage(item):
+            if isinstance(item, jpype.JPackage) and not isPseudoPackage(item):
                 yield from packageAndSubPackages(item)
         except Exception as e:
             log.warning(f'skipping {package.__name__}.{name}: {e}')
 
 
 def generateJavaStubs(parentPackages: List[jpype.JPackage],
                       useStubsSuffix: bool = True,
@@ -950,19 +950,21 @@
 
     for signature, overloadJavadoc in zip(signatures, overloadsJavadoc):
         if isOverloaded:
             output.append('@typing.overload')
         if signature.static:
             output.append('@staticmethod')
         sig = []
-        for arg in signature.args:
+        for i, arg in enumerate(signature.args):
             if arg.name == 'self':
                 argDef = arg.name
             else:
                 argDef = pysafe(arg.name)
+                if argDef is None:
+                    argDef = f'invalidArgName{i}'
                 if arg.varArgs:
                     argDef = '*' + argDef
 
                 if arg.argType:
                     argDef += ': ' + toAnnotatedType(arg.argType, parentName, classesDone, classesUsed, importsOutput)
 
             sig.append(argDef)
@@ -972,17 +974,20 @@
                 args=', '.join(sig),
                 ellipsis='' if overloadJavadoc else ' ...'
             ))
             if overloadJavadoc:
                 output.extend(toDocstringLines(overloadJavadoc))
                 output.append('    ...')
         else:
+            functionName = pysafe(signature.name)
+            if functionName is None:
+                continue
             # In the future, we should prevent keyword arguments from being used (PEP-570) but that requires 3.8+
             output.append('def {function}({args}) -> {ret}:{ellipsis}'.format(
-                function=pysafe(signature.name),
+                function=functionName,
                 args=', '.join(sig),
                 ret=toAnnotatedType(signature.retType, parentName, classesDone, classesUsed, importsOutput),
                 ellipsis='' if overloadJavadoc else ' ...'
             ))
             if overloadJavadoc:
                 output.extend(toDocstringLines(overloadJavadoc))
                 output.append('    ...')
@@ -1002,15 +1007,18 @@
     static = isStatic(jField)
     fieldName = str(jField.getName())
     fieldType = pythonType(jField.getType(), classTypeVars if not static else None)
     fieldTypeAnnotation = toAnnotatedType(fieldType, parentName, classesDone, classesUsed, importsOutput,
                                           canBeDeferred=True)
     if static:
         fieldTypeAnnotation = f'typing.ClassVar[{fieldTypeAnnotation}]'
-    output.append(f'{pysafe(fieldName)}: {fieldTypeAnnotation} = ...')
+    pySafeFieldName = pysafe(fieldName)
+    if pySafeFieldName is None:
+        return
+    output.append(f'{pySafeFieldName}: {fieldTypeAnnotation} = ...')
     if fieldName in javadoc:
         output.extend(toDocstringLines(javadoc[fieldName], indent=False))
 
 
 def pysafePackagePath(packagePath: str) -> str:
     """ Apply the JPype package name mangling. Segments which would clash with a python keyword are suffixed by '_'."""
     return '.'.join([pysafe(p) for p in packagePath.split('.')])
```

### Comparing `stubgenj-0.2.8/stubgenj/conftest.py` & `stubgenj-0.2.9/stubgenj/conftest.py`

 * *Files identical despite different names*

### Comparing `stubgenj-0.2.8/stubgenj/tests/stubtest/test-data/unit/arraylist.test` & `stubgenj-0.2.9/stubgenj/tests/stubtest/test-data/unit/arraylist.test`

 * *Files identical despite different names*

### Comparing `stubgenj-0.2.8/stubgenj/tests/stubtest/test-data/unit/callbacks.test` & `stubgenj-0.2.9/stubgenj/tests/stubtest/test-data/unit/callbacks.test`

 * *Files identical despite different names*

### Comparing `stubgenj-0.2.8/stubgenj/tests/stubtest/test-data/unit/enummap.test` & `stubgenj-0.2.9/stubgenj/tests/stubtest/test-data/unit/enummap.test`

 * *Files identical despite different names*

### Comparing `stubgenj-0.2.8/stubgenj/tests/stubtest/test-data/unit/hashmap.test` & `stubgenj-0.2.9/stubgenj/tests/stubtest/test-data/unit/hashmap.test`

 * *Files identical despite different names*

### Comparing `stubgenj-0.2.8/stubgenj/tests/stubtest/test-data/unit/jpype_jpackage.test` & `stubgenj-0.2.9/stubgenj/tests/stubtest/test-data/unit/jpype_jpackage.test`

 * *Files identical despite different names*

### Comparing `stubgenj-0.2.8/stubgenj/tests/stubtest/test-data/unit/varargs.test` & `stubgenj-0.2.9/stubgenj/tests/stubtest/test-data/unit/varargs.test`

 * *Files identical despite different names*

### Comparing `stubgenj-0.2.8/stubgenj/tests/test_stubtest.py` & `stubgenj-0.2.9/stubgenj/tests/test_stubtest.py`

 * *Files identical despite different names*

### Comparing `stubgenj-0.2.8/stubgenj.egg-info/PKG-INFO` & `stubgenj-0.2.9/stubgenj.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stubgenj
-Version: 0.2.8
+Version: 0.2.9
 Summary: PEP-484 python stub generator for Java classes accessed through JPype
 Home-page: https://gitlab.cern.ch/scripting-tools/stubgenj
 Maintainer: CERN Accelerating Python
 Maintainer-email: acc-py-support@cern.ch
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `stubgenj-0.2.8/stubgenj.egg-info/SOURCES.txt` & `stubgenj-0.2.9/stubgenj.egg-info/SOURCES.txt`

 * *Files identical despite different names*

