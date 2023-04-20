# Comparing `tmp/crosstream-2.1.0.tar.gz` & `tmp/crosstream-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "E:\Users\bertw\Documents\Projects\crosstream\dist\.tmp-nl54sqyk\crosstream-2.1.0.tar", last modified: Mon Apr 17 21:09:25 2023, max compression
+gzip compressed data, was "C:\Users\bertw\Documents\GitHub\crosstream\dist\.tmp-77fu6v_m\crosstream-3.0.0.tar", last modified: Thu Apr 20 17:18:14 2023, max compression
```

## Comparing `crosstream-2.1.0.tar` & `crosstream-3.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 21:09:25.555880 crosstream-2.1.0/
--rw-rw-rw-   0        0        0     1089 2023-03-22 23:55:29.000000 crosstream-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     4129 2023-04-17 21:09:25.555880 crosstream-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3815 2023-04-17 20:56:58.000000 crosstream-2.1.0/README.md
--rw-rw-rw-   0        0        0       86 2023-03-22 23:55:29.000000 crosstream-2.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      530 2023-04-17 21:09:25.556853 crosstream-2.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 21:09:25.491130 crosstream-2.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 21:09:25.529851 crosstream-2.1.0/src/crosstream/
--rw-rw-rw-   0        0        0       89 2023-03-26 19:05:17.000000 crosstream-2.1.0/src/crosstream/__init__.py
--rw-rw-rw-   0        0        0     1415 2023-04-17 20:20:10.000000 crosstream-2.1.0/src/crosstream/api.py
--rw-rw-rw-   0        0        0     2498 2023-04-17 20:54:59.000000 crosstream-2.1.0/src/crosstream/hash_join.py
--rw-rw-rw-   0        0        0     3891 2023-03-26 19:05:17.000000 crosstream-2.1.0/src/crosstream/readers.py
-drwxrwxrwx   0        0        0        0 2023-04-17 21:09:25.552851 crosstream-2.1.0/src/crosstream.egg-info/
--rw-rw-rw-   0        0        0     4129 2023-04-17 21:09:25.000000 crosstream-2.1.0/src/crosstream.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-04-17 21:09:25.000000 crosstream-2.1.0/src/crosstream.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 21:09:25.000000 crosstream-2.1.0/src/crosstream.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-17 21:09:25.000000 crosstream-2.1.0/src/crosstream.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-17 21:09:25.000000 crosstream-2.1.0/src/crosstream.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 21:09:25.553853 crosstream-2.1.0/tests/
--rw-rw-rw-   0        0        0     5394 2023-04-17 20:53:09.000000 crosstream-2.1.0/tests/test_hash_join.py
+drwxrwxrwx   0        0        0        0 2023-04-20 17:18:14.067362 crosstream-3.0.0/
+-rw-rw-rw-   0        0        0     1089 2023-04-20 16:35:48.000000 crosstream-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0     3682 2023-04-20 17:18:14.068105 crosstream-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3368 2023-04-20 16:54:27.000000 crosstream-3.0.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-20 16:35:48.000000 crosstream-3.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      530 2023-04-20 17:18:14.083195 crosstream-3.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-20 17:18:13.976271 crosstream-3.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-20 17:18:14.018330 crosstream-3.0.0/src/crosstream/
+-rw-rw-rw-   0        0        0       89 2023-04-20 16:35:48.000000 crosstream-3.0.0/src/crosstream/__init__.py
+-rw-rw-rw-   0        0        0     1423 2023-04-20 17:15:23.000000 crosstream-3.0.0/src/crosstream/api.py
+-rw-rw-rw-   0        0        0     2679 2023-04-20 16:52:05.000000 crosstream-3.0.0/src/crosstream/hash_join.py
+-rw-rw-rw-   0        0        0     3891 2023-04-20 16:35:48.000000 crosstream-3.0.0/src/crosstream/readers.py
+drwxrwxrwx   0        0        0        0 2023-04-20 17:18:14.055319 crosstream-3.0.0/src/crosstream.egg-info/
+-rw-rw-rw-   0        0        0     3682 2023-04-20 17:18:13.000000 crosstream-3.0.0/src/crosstream.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-04-20 17:18:13.000000 crosstream-3.0.0/src/crosstream.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 17:18:13.000000 crosstream-3.0.0/src/crosstream.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-04-20 17:18:13.000000 crosstream-3.0.0/src/crosstream.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-20 17:18:13.000000 crosstream-3.0.0/src/crosstream.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 17:18:14.064869 crosstream-3.0.0/tests/
+-rw-rw-rw-   0        0        0     4998 2023-04-20 16:54:32.000000 crosstream-3.0.0/tests/test_hash_join.py
```

### Comparing `crosstream-2.1.0/LICENSE` & `crosstream-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crosstream-2.1.0/PKG-INFO` & `crosstream-3.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosstream
-Version: 2.1.0
+Version: 3.0.0
 Summary: A package for streaming cross-server dataset joins in memory
 Home-page: https://github.com/bertwagner/crosstream
 Author: Bert Wagner
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
@@ -68,35 +68,25 @@
 ### Custom method for determining equality
 
 By default, this package will join only if all values are equal.
 
 If you want to perform a transformation on your data before comparing for equality, or use more complicated join equality logic, you can pass in your own function into `override_build_join_key` to define how equality is determined:
 
 ```
-# define a function for joining on criteria that is modified before insert into hash table
-# row is the data, indices indicates which columns are to be part of the join key
-def custom_join_key(row,indices):
-    # calculate the hash of join values
-    join_values = []
-    join_key_values = []
-    for col_index in indices:
-        # here we transform our join key, removing any spaces from our values
-        col_value = str(row[col_index]).replace(' ','')
-        join_values.append(str(hash(col_value)))
-        join_key_values.append(col_value)
-    join_key = ''.join(join_values)
-
-    return join_key, join_key_values
+# define a function for transforming join key data before it's hashed
+def custom_join_key_transform(value):
+    transformed = value.replace(' ','')
+    return transformed
 ```
 
 And then pass that into the `inner_hash_join()` method:
 
 ```
 ...
-for row_left,row_right in cs.inner_hash_join(c1,c2,override_build_join_key=custom_join_key)
+for row_left,row_right in cs.inner_hash_join(c1,c2,override_join_key_transform=custom_join_key_transform)
 ...
 ```
 
 ### Custom method for processing matched hashes
 
 By default this package returns tuples of the joined rows. If you want to customize what the output of your matched data looks like (perform transformations after a match is found), you can pass a function to the `override_process_matched_hashes` argument:
```

### Comparing `crosstream-2.1.0/README.md` & `crosstream-3.0.0/src/crosstream.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: crosstream
+Version: 3.0.0
+Summary: A package for streaming cross-server dataset joins in memory
+Home-page: https://github.com/bertwagner/crosstream
+Author: Bert Wagner
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # crosstream 🐍🌊🤝
 
 This Python package helps join large datasets across servers efficiently. It accomplishes this by streaming the data, allowing it to:
  - read each dataset only once
  - not need to store the complete datasets in memory
 
 This is particularly helpful when your datasets are larger than the available memory on your machine or when you want to minimize network reads.
@@ -57,35 +68,25 @@
 ### Custom method for determining equality
 
 By default, this package will join only if all values are equal.
 
 If you want to perform a transformation on your data before comparing for equality, or use more complicated join equality logic, you can pass in your own function into `override_build_join_key` to define how equality is determined:
 
 ```
-# define a function for joining on criteria that is modified before insert into hash table
-# row is the data, indices indicates which columns are to be part of the join key
-def custom_join_key(row,indices):
-    # calculate the hash of join values
-    join_values = []
-    join_key_values = []
-    for col_index in indices:
-        # here we transform our join key, removing any spaces from our values
-        col_value = str(row[col_index]).replace(' ','')
-        join_values.append(str(hash(col_value)))
-        join_key_values.append(col_value)
-    join_key = ''.join(join_values)
-
-    return join_key, join_key_values
+# define a function for transforming join key data before it's hashed
+def custom_join_key_transform(value):
+    transformed = value.replace(' ','')
+    return transformed
 ```
 
 And then pass that into the `inner_hash_join()` method:
 
 ```
 ...
-for row_left,row_right in cs.inner_hash_join(c1,c2,override_build_join_key=custom_join_key)
+for row_left,row_right in cs.inner_hash_join(c1,c2,override_join_key_transform=custom_join_key_transform)
 ...
 ```
 
 ### Custom method for processing matched hashes
 
 By default this package returns tuples of the joined rows. If you want to customize what the output of your matched data looks like (perform transformations after a match is found), you can pass a function to the `override_process_matched_hashes` argument:
```

### Comparing `crosstream-2.1.0/setup.cfg` & `crosstream-3.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 726f 7373 7472 6561 6d0d 0a76   = crosstream..v
-00000020: 6572 7369 6f6e 203d 2032 2e31 2e30 0d0a  ersion = 2.1.0..
+00000020: 6572 7369 6f6e 203d 2033 2e30 2e30 0d0a  ersion = 3.0.0..
 00000030: 6175 7468 6f72 203d 2042 6572 7420 5761  author = Bert Wa
 00000040: 676e 6572 0d0a 6465 7363 7269 7074 696f  gner..descriptio
 00000050: 6e20 3d20 4120 7061 636b 6167 6520 666f  n = A package fo
 00000060: 7220 7374 7265 616d 696e 6720 6372 6f73  r streaming cros
 00000070: 732d 7365 7276 6572 2064 6174 6173 6574  s-server dataset
 00000080: 206a 6f69 6e73 2069 6e20 6d65 6d6f 7279   joins in memory
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
```

### Comparing `crosstream-2.1.0/src/crosstream/api.py` & `crosstream-3.0.0/src/crosstream/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,14 @@
     ...
 
 def read_odbc(connection_string, query, join_columns):
     """Lazily load the contents of an ODBC sql query one row at a time as needed."""
     return ODBCReader(connection_string, query, join_columns)
 
 reader = Union[CSVReader,ODBCReader]
-def inner_hash_join(input_1: reader, input_2: reader, override_build_join_key=None, override_process_matched_hashes=None):
+def inner_hash_join(input_1: reader, input_2: reader, override_join_key_transform=None, override_process_matched_hashes=None):
     """Join two datasets using a hash join.
 
         The smaller dataset should be passed into input_1.
         """
     h=HashJoin()
-    return h.inner_join(input_1,input_2,override_build_join_key,override_process_matched_hashes)
+    return h.inner_join(input_1,input_2,override_join_key_transform,override_process_matched_hashes)
```

### Comparing `crosstream-2.1.0/src/crosstream/hash_join.py` & `crosstream-3.0.0/src/crosstream/hash_join.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,35 +9,39 @@
         self.hash_buckets_key_values = defaultdict(list)
 
     def __build_hash_input(self, row, join_column_indexes):
         join_key, join_key_values = self.__build_join_key(row,join_column_indexes)
         self.hash_buckets[join_key].append(row)
         self.hash_buckets_key_values[join_key].append(join_key_values)
 
+    def __join_key_transform(self,value):
+        return value
+
     def __build_join_key(self,row,indices):
         # calculate the hash of join values
         join_values = []
         join_key_values = []
         for col_index in indices:
             # convert row[col_index] to string because CSVs can't don't define numeric datatypes - would have to interpret them.
             col_value = str(row[col_index])
-            join_values.append(str(hash(col_value)))
-            join_key_values.append(col_value)
+            transformed_col_value = self.__join_key_transform(col_value)
+            join_values.append(str(hash(transformed_col_value)))
+            join_key_values.append(transformed_col_value)
         join_key = ''.join(join_values)
 
         return join_key, join_key_values
 
     def __process_matched_hashes(self,bucket_row,probe_row, bucket_join_column_indexes, probe_join_column_indexes):
         return tuple(bucket_row),tuple(probe_row,)
 
     reader = Union[CSVReader,ODBCReader]
-    def inner_join(self, input_1: reader, input_2: reader, override_build_join_key=None, override_process_matched_hashes=None):
+    def inner_join(self, input_1: reader, input_2: reader, override_join_key_transform=None, override_process_matched_hashes=None):
 
-        if override_build_join_key != None:
-            self.__build_join_key = override_build_join_key
+        if override_join_key_transform != None:
+            self.__join_key_transform = override_join_key_transform
         if override_process_matched_hashes != None:
             self.__process_matched_hashes = override_process_matched_hashes
 
         self.hash_buckets = defaultdict(list)
 
         for row in input_1:
             self.__build_hash_input(row,input_1.join_column_indexes)
```

### Comparing `crosstream-2.1.0/src/crosstream/readers.py` & `crosstream-3.0.0/src/crosstream/readers.py`

 * *Files identical despite different names*

### Comparing `crosstream-2.1.0/src/crosstream.egg-info/PKG-INFO` & `crosstream-3.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: crosstream
-Version: 2.1.0
-Summary: A package for streaming cross-server dataset joins in memory
-Home-page: https://github.com/bertwagner/crosstream
-Author: Bert Wagner
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # crosstream 🐍🌊🤝
 
 This Python package helps join large datasets across servers efficiently. It accomplishes this by streaming the data, allowing it to:
  - read each dataset only once
  - not need to store the complete datasets in memory
 
 This is particularly helpful when your datasets are larger than the available memory on your machine or when you want to minimize network reads.
@@ -68,35 +57,25 @@
 ### Custom method for determining equality
 
 By default, this package will join only if all values are equal.
 
 If you want to perform a transformation on your data before comparing for equality, or use more complicated join equality logic, you can pass in your own function into `override_build_join_key` to define how equality is determined:
 
 ```
-# define a function for joining on criteria that is modified before insert into hash table
-# row is the data, indices indicates which columns are to be part of the join key
-def custom_join_key(row,indices):
-    # calculate the hash of join values
-    join_values = []
-    join_key_values = []
-    for col_index in indices:
-        # here we transform our join key, removing any spaces from our values
-        col_value = str(row[col_index]).replace(' ','')
-        join_values.append(str(hash(col_value)))
-        join_key_values.append(col_value)
-    join_key = ''.join(join_values)
-
-    return join_key, join_key_values
+# define a function for transforming join key data before it's hashed
+def custom_join_key_transform(value):
+    transformed = value.replace(' ','')
+    return transformed
 ```
 
 And then pass that into the `inner_hash_join()` method:
 
 ```
 ...
-for row_left,row_right in cs.inner_hash_join(c1,c2,override_build_join_key=custom_join_key)
+for row_left,row_right in cs.inner_hash_join(c1,c2,override_join_key_transform=custom_join_key_transform)
 ...
 ```
 
 ### Custom method for processing matched hashes
 
 By default this package returns tuples of the joined rows. If you want to customize what the output of your matched data looks like (perform transformations after a match is found), you can pass a function to the `override_process_matched_hashes` argument:
```

### Comparing `crosstream-2.1.0/tests/test_hash_join.py` & `crosstream-3.0.0/tests/test_hash_join.py`

 * *Files 6% similar despite different names*

```diff
@@ -114,27 +114,18 @@
 
 def test_custom_overrides(tmp_path_factory,csv_input_data,sqlite_input_data):
 
     # columns referred to by index and name
     c1=cs.read_csv(csv_input_data[0],True,[0,1])
     c2=cs.read_csv(csv_input_data[1], True, ['col1','col2'])
 
-    # define a function for joining on criteria that is modified before insert into hash table
-    def custom_join_key(row,indices):
-        # calculate the hash of join values
-        join_values = []
-        join_key_values = []
-        for col_index in indices:
-            # here we transform our join key, removing any spaces from our values
-            col_value = str(row[col_index]).replace(' ','')
-            join_values.append(str(hash(col_value)))
-            join_key_values.append(col_value)
-        join_key = ''.join(join_values)
-
-        return join_key, join_key_values
+    # define a function for transforming join key data before it's hashed
+    def custom_join_key_transform(value):
+        transformed = value.replace(' ','')
+        return transformed
 
     # define a function for performing additional transformations or adding additional outputs before the columns are returned
     def custom_process_matched_hashes(bucket_row,probe_row, bucket_join_column_indexes, probe_join_column_indexes):
         # adding a new column indicating the weights of these matches are equal to 1
         weight=1.0
         return tuple(bucket_row),tuple(probe_row),(weight,)
 
@@ -142,15 +133,15 @@
 
     with open(output_file, 'w', newline='') as f:
         w =csv.writer(f)
         
         # write header column names
         w.writerow(c1.column_names + c2.column_names + ['weight'])
 
-        for row_left,row_right,weight in cs.inner_hash_join(c1,c2,override_build_join_key=custom_join_key,override_process_matched_hashes=custom_process_matched_hashes):
+        for row_left,row_right,weight in cs.inner_hash_join(c1,c2,override_join_key_transform=custom_join_key_transform,override_process_matched_hashes=custom_process_matched_hashes):
             # write matched results
             w.writerow(row_left + row_right + weight)
 
     with open(output_file, 'r') as f:
         file_content = f.read()
 
         assert file_content == '''col1,col2,col1,col2,weight
```

