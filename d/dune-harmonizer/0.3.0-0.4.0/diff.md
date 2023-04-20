# Comparing `tmp/dune_harmonizer-0.3.0.tar.gz` & `tmp/dune_harmonizer-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_harmonizer-0.3.0.tar", max compression
+gzip compressed data, was "dune_harmonizer-0.4.0.tar", max compression
```

## Comparing `dune_harmonizer-0.3.0.tar` & `dune_harmonizer-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1061 2023-04-20 06:46:45.178685 dune_harmonizer-0.3.0/LICENSE
--rw-r--r--   0        0        0     2378 2023-04-20 06:46:45.178685 dune_harmonizer-0.3.0/README.md
--rw-r--r--   0        0        0      440 2023-04-20 06:46:45.178685 dune_harmonizer-0.3.0/dune/harmonizer/__init__.py
--rw-r--r--   0        0        0      849 2023-04-20 06:47:02.758997 dune_harmonizer-0.3.0/dune/harmonizer/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    19518 2023-04-20 06:47:02.934999 dune_harmonizer-0.3.0/dune/harmonizer/__pycache__/custom_transforms.cpython-311.pyc
--rw-r--r--   0        0        0      630 2023-04-20 06:47:02.934999 dune_harmonizer-0.3.0/dune/harmonizer/__pycache__/errors.cpython-311.pyc
--rw-r--r--   0        0        0     3103 2023-04-20 06:47:02.934999 dune_harmonizer-0.3.0/dune/harmonizer/__pycache__/table_replacements.cpython-311.pyc
--rw-r--r--   0        0        0     3305 2023-04-20 06:47:02.758997 dune_harmonizer-0.3.0/dune/harmonizer/__pycache__/translate.cpython-311.pyc
--rw-r--r--   0        0        0       54 2023-04-20 06:46:45.178685 dune_harmonizer-0.3.0/dune/harmonizer/constants.py
--rw-r--r--   0        0        0    17082 2023-04-20 06:46:45.178685 dune_harmonizer-0.3.0/dune/harmonizer/custom_transforms.py
--rw-r--r--   0        0        0      105 2023-04-20 06:46:45.178685 dune_harmonizer-0.3.0/dune/harmonizer/errors.py
--rw-r--r--   0        0        0     2018 2023-04-20 06:46:45.178685 dune_harmonizer-0.3.0/dune/harmonizer/table_replacements.py
--rw-r--r--   0        0        0     3050 2023-04-20 06:46:45.182685 dune_harmonizer-0.3.0/dune/harmonizer/translate.py
--rw-r--r--   0        0        0      570 2023-04-20 06:46:45.182685 dune_harmonizer-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2714 1970-01-01 00:00:00.000000 dune_harmonizer-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-20 10:36:09.577470 dune_harmonizer-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2378 2023-04-20 10:36:09.581471 dune_harmonizer-0.4.0/README.md
+-rw-r--r--   0        0        0      440 2023-04-20 10:36:09.581471 dune_harmonizer-0.4.0/dune/harmonizer/__init__.py
+-rw-r--r--   0        0        0      849 2023-04-20 10:36:30.181023 dune_harmonizer-0.4.0/dune/harmonizer/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    19835 2023-04-20 10:36:30.365021 dune_harmonizer-0.4.0/dune/harmonizer/__pycache__/custom_transforms.cpython-311.pyc
+-rw-r--r--   0        0        0      630 2023-04-20 10:36:30.365021 dune_harmonizer-0.4.0/dune/harmonizer/__pycache__/errors.cpython-311.pyc
+-rw-r--r--   0        0        0     3103 2023-04-20 10:36:30.365021 dune_harmonizer-0.4.0/dune/harmonizer/__pycache__/table_replacements.cpython-311.pyc
+-rw-r--r--   0        0        0     3528 2023-04-20 10:36:30.181023 dune_harmonizer-0.4.0/dune/harmonizer/__pycache__/translate.cpython-311.pyc
+-rw-r--r--   0        0        0       54 2023-04-20 10:36:09.581471 dune_harmonizer-0.4.0/dune/harmonizer/constants.py
+-rw-r--r--   0        0        0    17211 2023-04-20 10:36:09.581471 dune_harmonizer-0.4.0/dune/harmonizer/custom_transforms.py
+-rw-r--r--   0        0        0      105 2023-04-20 10:36:09.581471 dune_harmonizer-0.4.0/dune/harmonizer/errors.py
+-rw-r--r--   0        0        0     2018 2023-04-20 10:36:09.581471 dune_harmonizer-0.4.0/dune/harmonizer/table_replacements.py
+-rw-r--r--   0        0        0     2914 2023-04-20 10:36:09.581471 dune_harmonizer-0.4.0/dune/harmonizer/translate.py
+-rw-r--r--   0        0        0      570 2023-04-20 10:36:09.581471 dune_harmonizer-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2714 1970-01-01 00:00:00.000000 dune_harmonizer-0.4.0/PKG-INFO
```

### Comparing `dune_harmonizer-0.3.0/LICENSE` & `dune_harmonizer-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dune_harmonizer-0.3.0/README.md` & `dune_harmonizer-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dune_harmonizer-0.3.0/dune/harmonizer/__pycache__/__init__.cpython-311.pyc` & `dune_harmonizer-0.4.0/dune/harmonizer/__pycache__/__init__.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xd5df4064 (Thu Apr 20 06:46:45 2023 UTC)
+moddate:  0x99154164 (Thu Apr 20 10:36:09 2023 UTC)
 files sz: 440
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `dune_harmonizer-0.3.0/dune/harmonizer/__pycache__/custom_transforms.cpython-311.pyc` & `dune_harmonizer-0.4.0/dune/harmonizer/__pycache__/custom_transforms.cpython-311.pyc`

 * *Files 6% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xd5df4064 (Thu Apr 20 06:46:45 2023 UTC)
-files sz: 17082
+moddate:  0x99154164 (Thu Apr 20 10:36:09 2023 UTC)
+files sz: 17211
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064016c035a
@@ -14,15 +14,15 @@
       0aac08a6020000ab0200000000000000005a0b020065026508640bac08a6
       020000ab0200000000000000005a0c020065026508640cac08a6020000ab
       0200000000000000005a0d640d84005a0e640e5a0f640f5a106410650f9b
       009d025a1165109b0064109d025a126411650f9b009d025a1365109b0064
       119d025a14641284005a15641384005a16641484005a17641584005a1864
       1684005a19641784005a1a641884005a1b641984005a1c641a84005a1d64
       1b84005a1e641c84005a1f641d84005a20641e84005a21641f84005a2264
-      2084005a23642184005a24642284005a2564015300
+      2084005a23642184005a24642284005a25642384005a2664015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (re)
                  8 STORE_NAME               0 (re)
    
@@ -102,18 +102,18 @@
                178 CALL                     2
                188 STORE_NAME              13 (chain_where_polygon)
    
    142         190 LOAD_CONST              13 (<code object dex_trades_fixes, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 142>)
                192 MAKE_FUNCTION            0
                194 STORE_NAME              14 (dex_trades_fixes)
    
-   186         196 LOAD_CONST              14 ('parameter_placeholder_left_bracket')
+   186         196 LOAD_CONST              14 ('left_param_')
                198 STORE_NAME              15 (param_left_placeholder)
    
-   187         200 LOAD_CONST              15 ('parameter_placeholder_right_bracket')
+   187         200 LOAD_CONST              15 ('_right_param')
                202 STORE_NAME              16 (param_right_placeholder)
    
    188         204 LOAD_CONST              16 ('"')
                206 LOAD_NAME               15 (param_left_placeholder)
                208 FORMAT_VALUE             0
                210 BUILD_STRING             2
                212 STORE_NAME              17 (double_quoted_param_left_placeholder)
@@ -144,71 +144,75 @@
                252 MAKE_FUNCTION            0
                254 STORE_NAME              22 (cast_numeric)
    
    230         256 LOAD_CONST              20 (<code object cast_timestamp, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 230>)
                258 MAKE_FUNCTION            0
                260 STORE_NAME              23 (cast_timestamp)
    
-   248         262 LOAD_CONST              21 (<code object fix_boolean, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 248>)
+   245         262 LOAD_CONST              21 (<code object fix_boolean, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 245>)
                264 MAKE_FUNCTION            0
                266 STORE_NAME              24 (fix_boolean)
    
-   258         268 LOAD_CONST              22 (<code object warn_unnest, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 258>)
+   255         268 LOAD_CONST              22 (<code object warn_unnest, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 255>)
                270 MAKE_FUNCTION            0
                272 STORE_NAME              25 (warn_unnest)
    
-   272         274 LOAD_CONST              23 (<code object warn_sequence, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 272>)
+   269         274 LOAD_CONST              23 (<code object warn_sequence, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 269>)
                276 MAKE_FUNCTION            0
                278 STORE_NAME              26 (warn_sequence)
    
-   286         280 LOAD_CONST              24 (<code object prep_query, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 286>)
+   283         280 LOAD_CONST              24 (<code object prep_query, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 283>)
                282 MAKE_FUNCTION            0
                284 STORE_NAME              27 (prep_query)
    
-   298         286 LOAD_CONST              25 (<code object rename_amount_column, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 298>)
+   295         286 LOAD_CONST              25 (<code object rename_amount_column, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 295>)
                288 MAKE_FUNCTION            0
                290 STORE_NAME              28 (rename_amount_column)
    
-   303         292 LOAD_CONST              26 (<code object bytea2numeric, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 303>)
+   300         292 LOAD_CONST              26 (<code object bytea2numeric, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 300>)
                294 MAKE_FUNCTION            0
                296 STORE_NAME              29 (bytea2numeric)
    
-   317         298 LOAD_CONST              27 (<code object fix_bytearray_param, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 317>)
+   314         298 LOAD_CONST              27 (<code object fix_bytearray_param, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 314>)
                300 MAKE_FUNCTION            0
                302 STORE_NAME              30 (fix_bytearray_param)
    
-   323         304 LOAD_CONST              28 (<code object fix_bytearray_lower, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 323>)
+   320         304 LOAD_CONST              28 (<code object fix_bytearray_lower, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 320>)
                306 MAKE_FUNCTION            0
                308 STORE_NAME              31 (fix_bytearray_lower)
    
-   332         310 LOAD_CONST              29 (<code object chain_where, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 332>)
+   329         310 LOAD_CONST              29 (<code object chain_where, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 329>)
                312 MAKE_FUNCTION            0
                314 STORE_NAME              32 (chain_where)
    
-   342         316 LOAD_CONST              30 (<code object postgres_transforms, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 342>)
+   339         316 LOAD_CONST              30 (<code object postgres_transforms, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 339>)
                318 MAKE_FUNCTION            0
                320 STORE_NAME              33 (postgres_transforms)
    
-   365         322 LOAD_CONST              31 (<code object remove_quotes_around_0x_strings, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 365>)
+   362         322 LOAD_CONST              31 (<code object remove_quotes_around_0x_strings, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 362>)
                324 MAKE_FUNCTION            0
                326 STORE_NAME              34 (remove_quotes_around_0x_strings)
    
-   374         328 LOAD_CONST              32 (<code object spark_function_replacements, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 374>)
+   371         328 LOAD_CONST              32 (<code object spark_function_replacements, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 371>)
                330 MAKE_FUNCTION            0
                332 STORE_NAME              35 (spark_function_replacements)
    
-   382         334 LOAD_CONST              33 (<code object spark_transforms, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 382>)
+   379         334 LOAD_CONST              33 (<code object spark_transforms, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 379>)
                336 MAKE_FUNCTION            0
                338 STORE_NAME              36 (spark_transforms)
    
-   401         340 LOAD_CONST              34 (<code object add_warnings_and_banner, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 401>)
+   398         340 LOAD_CONST              34 (<code object add_warnings_and_banner, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 398>)
                342 MAKE_FUNCTION            0
                344 STORE_NAME              37 (add_warnings_and_banner)
-               346 LOAD_CONST               1 (None)
-               348 RETURN_VALUE
+   
+   430         346 LOAD_CONST              35 (<code object parameter_placeholder, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 430>)
+               348 MAKE_FUNCTION            0
+               350 STORE_NAME              38 (parameter_placeholder)
+               352 LOAD_CONST               1 (None)
+               354 RETURN_VALUE
    consts
       0
       None
       ('partial',)
       ('postgres_table_replacements',)
       code
          argcount  : 1
@@ -1018,16 +1022,16 @@
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'dex_trades_fixes'
          firstlineno 142
          lnotab
             0x0203160158025403080c08012a024603160102010201020116fc120616
             0102010201020116fc12072c01
-      'parameter_placeholder_left_bracket'
-      'parameter_placeholder_right_bracket'
+      'left_param_'
+      '_right_param'
       '"'
       "'"
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 7
          flags     : 3
@@ -1339,165 +1343,144 @@
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'cast_numeric'
          firstlineno 221
          lnotab 0x0403160136014201
       code
          argcount  : 1
          nlocals   : 3
-         stacksize : 6
+         stacksize : 7
          flags     : 3
          code
-            0x8700970089006a00000000000000000064016b02000000009001720174
-            03000000000000000000006a02000000000000000064028900a003000000
-            00000000000000000000000000000000006403ac04a6010000ab01000000
-            0000000000a6020000ab020000000000000000722d740900000000000000
-            0000006a05000000000000000064058900a0030000000000000000000000
-            0000000000000000006403ac04a6010000ab0100000000000000007a0000
-            006403ac06a6020000ab0200000000000000005300740300000000000000
-            0000006a060000000000000000740e00000000000000000000a6010000ab
-            01000000000000000064077a0000007403000000000000000000006a0600
-            00000000000000741000000000000000000000a6010000ab010000000000
-            0000007a0000007d017403000000000000000000006a0200000000000000
-            007c018900a00300000000000000000000000000000000000000006403ac
-            04a6010000ab010000000000000000a6020000ab0200000000000000007d
-            027c02724a741300000000000000000000880066016408840864094400a6
-            000000ab000000000000000000a6010000ab010000000000000000722f74
-            09000000000000000000006a050000000000000000640a7c02a00a000000
-            0000000000000000000000000000000000640ba6010000ab010000000000
-            0000007a000000640c7a0000006403ac06a6020000ab0200000000000000
-            00530089005300
+            0x8700970089006a00000000000000000064016b020000000072c9740300
+            0000000000000000006a02000000000000000064028900a0030000000000
+            0000000000000000000000000000006403ac04a6010000ab010000000000
+            000000a6020000ab020000000000000000722d7409000000000000000000
+            006a05000000000000000064058900a00300000000000000000000000000
+            000000000000006403ac04a6010000ab0100000000000000007a00000064
+            03ac06a6020000ab02000000000000000053006407740c00000000000000
+            0000007a00000064087a000000740e000000000000000000007a00000064
+            097a0000007d0174110000000000000000000088006601640a8408640b44
+            00a6000000ab000000000000000000a6010000ab01000000000000000072
+            407403000000000000000000006a0900000000000000007c01640c8900a0
+            0300000000000000000000000000000000000000006403ac04a6010000ab
+            010000000000000000a6030000ab0300000000000000007d027409000000
+            000000000000006a0500000000000000007c026403ac06a6020000ab0200
+            00000000000000530089005300
                        0 MAKE_CELL                0 (node)
          
          230           2 RESUME                   0
          
-         231           4 LOAD_DEREF               0 (node)
+         232           4 LOAD_DEREF               0 (node)
                        6 LOAD_ATTR                0 (key)
                       16 LOAD_CONST               1 ('literal')
                       18 COMPARE_OP               2 (==)
-                      24 EXTENDED_ARG             1
-                      26 POP_JUMP_FORWARD_IF_FALSE   257 (to 542)
+                      24 POP_JUMP_FORWARD_IF_FALSE   201 (to 428)
          
-         233          28 LOAD_GLOBAL              3 (NULL + re)
-                      40 LOAD_ATTR                2 (search)
-                      50 LOAD_CONST               2 ('\\d{4}-\\d{2}-\\d{2}')
-                      52 LOAD_DEREF               0 (node)
-                      54 LOAD_METHOD              3 (sql)
-                      76 LOAD_CONST               3 ('trino')
-                      78 KW_NAMES                 4
-                      80 PRECALL                  1
-                      84 CALL                     1
-                      94 PRECALL                  2
-                      98 CALL                     2
-                     108 POP_JUMP_FORWARD_IF_FALSE    45 (to 200)
+         234          26 LOAD_GLOBAL              3 (NULL + re)
+                      38 LOAD_ATTR                2 (search)
+                      48 LOAD_CONST               2 ('\\d{4}-\\d{2}-\\d{2}')
+                      50 LOAD_DEREF               0 (node)
+                      52 LOAD_METHOD              3 (sql)
+                      74 LOAD_CONST               3 ('trino')
+                      76 KW_NAMES                 4
+                      78 PRECALL                  1
+                      82 CALL                     1
+                      92 PRECALL                  2
+                      96 CALL                     2
+                     106 POP_JUMP_FORWARD_IF_FALSE    45 (to 198)
          
-         234         110 LOAD_GLOBAL              9 (NULL + sqlglot)
-                     122 LOAD_ATTR                5 (parse_one)
-                     132 LOAD_CONST               5 ('timestamp ')
-                     134 LOAD_DEREF               0 (node)
-                     136 LOAD_METHOD              3 (sql)
-                     158 LOAD_CONST               3 ('trino')
-                     160 KW_NAMES                 4
-                     162 PRECALL                  1
-                     166 CALL                     1
-                     176 BINARY_OP                0 (+)
-                     180 LOAD_CONST               3 ('trino')
-                     182 KW_NAMES                 6
-                     184 PRECALL                  2
-                     188 CALL                     2
-                     198 RETURN_VALUE
-         
-         238     >>  200 LOAD_GLOBAL              3 (NULL + re)
-                     212 LOAD_ATTR                6 (escape)
-                     222 LOAD_GLOBAL             14 (double_quoted_param_left_placeholder)
-                     234 PRECALL                  1
-                     238 CALL                     1
-         
-         239         248 LOAD_CONST               7 ('(.*?)')
-         
-         238         250 BINARY_OP                0 (+)
-         
-         240         254 LOAD_GLOBAL              3 (NULL + re)
-                     266 LOAD_ATTR                6 (escape)
-                     276 LOAD_GLOBAL             16 (double_quoted_param_right_placeholder)
-                     288 PRECALL                  1
-                     292 CALL                     1
-         
-         238         302 BINARY_OP                0 (+)
-         
-         237         306 STORE_FAST               1 (pattern)
-         
-         242         308 LOAD_GLOBAL              3 (NULL + re)
-                     320 LOAD_ATTR                2 (search)
-                     330 LOAD_FAST                1 (pattern)
-                     332 LOAD_DEREF               0 (node)
-                     334 LOAD_METHOD              3 (sql)
-                     356 LOAD_CONST               3 ('trino')
-                     358 KW_NAMES                 4
-                     360 PRECALL                  1
-                     364 CALL                     1
-                     374 PRECALL                  2
-                     378 CALL                     2
-                     388 STORE_FAST               2 (match)
-         
-         243         390 LOAD_FAST                2 (match)
-                     392 POP_JUMP_FORWARD_IF_FALSE    74 (to 542)
-                     394 LOAD_GLOBAL             19 (NULL + any)
-                     406 LOAD_CLOSURE             0 (node)
-                     408 BUILD_TUPLE              1
-                     410 LOAD_CONST               8 (<code object <genexpr>, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 243>)
-                     412 MAKE_FUNCTION            8 (closure)
-                     414 LOAD_CONST               9 (('date', 'time'))
-                     416 GET_ITER
-                     418 PRECALL                  0
-                     422 CALL                     0
-                     432 PRECALL                  1
-                     436 CALL                     1
-                     446 POP_JUMP_FORWARD_IF_FALSE    47 (to 542)
-         
-         244         448 LOAD_GLOBAL              9 (NULL + sqlglot)
-                     460 LOAD_ATTR                5 (parse_one)
-                     470 LOAD_CONST              10 ("timestamp '{{")
-                     472 LOAD_FAST                2 (match)
-                     474 LOAD_METHOD             10 (group)
-                     496 LOAD_CONST              11 (1)
-                     498 PRECALL                  1
-                     502 CALL                     1
-                     512 BINARY_OP                0 (+)
-                     516 LOAD_CONST              12 ("}}'")
-                     518 BINARY_OP                0 (+)
-                     522 LOAD_CONST               3 ('trino')
-                     524 KW_NAMES                 6
-                     526 PRECALL                  2
-                     530 CALL                     2
-                     540 RETURN_VALUE
+         235         108 LOAD_GLOBAL              9 (NULL + sqlglot)
+                     120 LOAD_ATTR                5 (parse_one)
+                     130 LOAD_CONST               5 ('timestamp ')
+                     132 LOAD_DEREF               0 (node)
+                     134 LOAD_METHOD              3 (sql)
+                     156 LOAD_CONST               3 ('trino')
+                     158 KW_NAMES                 4
+                     160 PRECALL                  1
+                     164 CALL                     1
+                     174 BINARY_OP                0 (+)
+                     178 LOAD_CONST               3 ('trino')
+                     180 KW_NAMES                 6
+                     182 PRECALL                  2
+                     186 CALL                     2
+                     196 RETURN_VALUE
+         
+         238     >>  198 LOAD_CONST               7 ("('")
+                     200 LOAD_GLOBAL             12 (param_left_placeholder)
+                     212 BINARY_OP                0 (+)
+                     216 LOAD_CONST               8 ('.*?')
+                     218 BINARY_OP                0 (+)
+                     222 LOAD_GLOBAL             14 (param_right_placeholder)
+                     234 BINARY_OP                0 (+)
+                     238 LOAD_CONST               9 ("')")
+                     240 BINARY_OP                0 (+)
+                     244 STORE_FAST               1 (pattern)
+         
+         239         246 LOAD_GLOBAL             17 (NULL + any)
+                     258 LOAD_CLOSURE             0 (node)
+                     260 BUILD_TUPLE              1
+                     262 LOAD_CONST              10 (<code object <genexpr>, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 239>)
+                     264 MAKE_FUNCTION            8 (closure)
+                     266 LOAD_CONST              11 (('date', 'time'))
+                     268 GET_ITER
+                     270 PRECALL                  0
+                     274 CALL                     0
+                     284 PRECALL                  1
+                     288 CALL                     1
+                     298 POP_JUMP_FORWARD_IF_FALSE    64 (to 428)
+         
+         240         300 LOAD_GLOBAL              3 (NULL + re)
+                     312 LOAD_ATTR                9 (sub)
+                     322 LOAD_FAST                1 (pattern)
+                     324 LOAD_CONST              12 ('timestamp \\1')
+                     326 LOAD_DEREF               0 (node)
+                     328 LOAD_METHOD              3 (sql)
+                     350 LOAD_CONST               3 ('trino')
+                     352 KW_NAMES                 4
+                     354 PRECALL                  1
+                     358 CALL                     1
+                     368 PRECALL                  3
+                     372 CALL                     3
+                     382 STORE_FAST               2 (q)
+         
+         241         384 LOAD_GLOBAL              9 (NULL + sqlglot)
+                     396 LOAD_ATTR                5 (parse_one)
+                     406 LOAD_FAST                2 (q)
+                     408 LOAD_CONST               3 ('trino')
+                     410 KW_NAMES                 6
+                     412 PRECALL                  2
+                     416 CALL                     2
+                     426 RETURN_VALUE
          
-         245     >>  542 LOAD_DEREF               0 (node)
-                     544 RETURN_VALUE
+         242     >>  428 LOAD_DEREF               0 (node)
+                     430 RETURN_VALUE
          consts
-            None
+            'Look for date-like literals and params and cast these as timestamps'
             'literal'
             '\\d{4}-\\d{2}-\\d{2}'
             'trino'
             ('dialect',)
             'timestamp '
             ('read',)
-            '(.*?)'
+            "('"
+            '.*?'
+            "')"
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 51
                code
                   0x95014b00010097007c005d2e7d017c018902a000000000000000000000
                   00000000000000000000006400ac01a6010000ab010000000000000000a0
                   010000000000000000000000000000000000000000a6000000ab00000000
                   000000000076005600970101008c2f64025300
                              0 COPY_FREE_VARS           1
                
-               243           2 RETURN_GENERATOR
+               239           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                              8 LOAD_FAST                0 (.0)
                        >>   10 FOR_ITER                46 (to 104)
                             12 STORE_FAST               1 (d)
                             14 LOAD_FAST                1 (d)
                             16 LOAD_DEREF               2 (node)
@@ -1522,28 +1505,26 @@
                   None
                names      ('sql', 'lower')
                varnames   ('.0', 'd')
                freevars   ('node',)
                cellvars   ()
                filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
                name       '<genexpr>'
-               firstlineno 243
+               firstlineno 239
                lnotab 0x
             ('date', 'time')
-            "timestamp '{{"
-            1
-            "}}'"
-         names      ('key', 're', 'search', 'sql', 'sqlglot', 'parse_one', 'escape', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'any', 'group')
-         varnames   ('node', 'pattern', 'match')
+            'timestamp \\1'
+         names      ('key', 're', 'search', 'sql', 'sqlglot', 'parse_one', 'param_left_placeholder', 'param_right_placeholder', 'any', 'sub')
+         varnames   ('node', 'pattern', 'q')
          freevars   ()
          cellvars   ('node',)
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'cast_timestamp'
          firstlineno 230
-         lnotab 0x0401180252015a04300102ff040230fe04ff020552013a015e01
+         lnotab 0x0402160252015a033001360154012c01
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
             0x8700970089006a00000000000000000064016b0200000000726f740300
@@ -1553,36 +1534,36 @@
             000000a003000000000000000000000000000000000000000064066407a6
             020000ab020000000000000000a003000000000000000000000000000000
             000000000064086407a6020000ab0200000000000000007d017409000000
             000000000000006a0500000000000000007c016404ac09a6020000ab0200
             00000000000000530089005300
                        0 MAKE_CELL                0 (node)
          
-         248           2 RESUME                   0
+         245           2 RESUME                   0
          
-         250           4 LOAD_DEREF               0 (node)
+         247           4 LOAD_DEREF               0 (node)
                        6 LOAD_ATTR                0 (key)
                       16 LOAD_CONST               1 ('literal')
                       18 COMPARE_OP               2 (==)
                       24 POP_JUMP_FORWARD_IF_FALSE   111 (to 248)
          
-         251          26 LOAD_GLOBAL              3 (NULL + any)
+         248          26 LOAD_GLOBAL              3 (NULL + any)
                       38 LOAD_CLOSURE             0 (node)
                       40 BUILD_TUPLE              1
-                      42 LOAD_CONST               2 (<code object <genexpr>, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 251>)
+                      42 LOAD_CONST               2 (<code object <genexpr>, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 248>)
                       44 MAKE_FUNCTION            8 (closure)
                       46 LOAD_CONST               3 (('true', 'false'))
                       48 GET_ITER
                       50 PRECALL                  0
                       54 CALL                     0
                       64 PRECALL                  1
                       68 CALL                     1
                       78 POP_JUMP_FORWARD_IF_FALSE    84 (to 248)
          
-         253          80 LOAD_DEREF               0 (node)
+         250          80 LOAD_DEREF               0 (node)
                       82 LOAD_METHOD              2 (sql)
                      104 LOAD_CONST               4 ('trino')
                      106 KW_NAMES                 5
                      108 PRECALL                  1
                      112 CALL                     1
                      122 LOAD_METHOD              3 (replace)
                      144 LOAD_CONST               6 ('"')
@@ -1592,24 +1573,24 @@
                      162 LOAD_METHOD              3 (replace)
                      184 LOAD_CONST               8 ("'")
                      186 LOAD_CONST               7 ('')
                      188 PRECALL                  2
                      192 CALL                     2
                      202 STORE_FAST               1 (bool_cleaned)
          
-         254         204 LOAD_GLOBAL              9 (NULL + sqlglot)
+         251         204 LOAD_GLOBAL              9 (NULL + sqlglot)
                      216 LOAD_ATTR                5 (parse_one)
                      226 LOAD_FAST                1 (bool_cleaned)
                      228 LOAD_CONST               4 ('trino')
                      230 KW_NAMES                 9
                      232 PRECALL                  2
                      236 CALL                     2
                      246 RETURN_VALUE
          
-         255     >>  248 LOAD_DEREF               0 (node)
+         252     >>  248 LOAD_DEREF               0 (node)
                      250 RETURN_VALUE
          consts
             "If node.key is 'literal' and contains 'true' or 'false' then cast to boolean"
             'literal'
             code
                argcount  : 1
                nlocals   : 2
@@ -1618,15 +1599,15 @@
                code
                   0x95014b00010097007c005d2e7d017c018902a000000000000000000000
                   00000000000000000000006400ac01a6010000ab010000000000000000a0
                   010000000000000000000000000000000000000000a6000000ab00000000
                   000000000076005600970101008c2f64025300
                              0 COPY_FREE_VARS           1
                
-               251           2 RETURN_GENERATOR
+               248           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                              8 LOAD_FAST                0 (.0)
                        >>   10 FOR_ITER                46 (to 104)
                             12 STORE_FAST               1 (boolean)
                             14 LOAD_FAST                1 (boolean)
                             16 LOAD_DEREF               2 (node)
@@ -1651,232 +1632,232 @@
                   None
                names      ('sql', 'lower')
                varnames   ('.0', 'boolean')
                freevars   ('node',)
                cellvars   ()
                filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
                name       '<genexpr>'
-               firstlineno 251
+               firstlineno 248
                lnotab 0x
             ('true', 'false')
             'trino'
             ('dialect',)
             '"'
             ''
             "'"
             ('read',)
          names      ('key', 'any', 'sql', 'replace', 'sqlglot', 'parse_one')
          varnames   ('node', 'bool_cleaned')
          freevars   ()
          cellvars   ('node',)
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'fix_boolean'
-         firstlineno 248
+         firstlineno 245
          lnotab 0x0402160136027c012c01
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 5
          flags     : 3
          code
             0x97007c006a000000000000000000a00100000000000000000000000000
             00000000000000a6000000ab00000000000000000064017600722d740500
             0000000000000000006a0300000000000000007c00a00400000000000000
             000000000000000000000000006402ac03a6010000ab0100000000000000
             0064047a0000006402ac05a6020000ab02000000000000000053007c0053
             00
-         258           0 RESUME                   0
+         255           0 RESUME                   0
          
-         260           2 LOAD_FAST                0 (node)
+         257           2 LOAD_FAST                0 (node)
                        4 LOAD_ATTR                0 (name)
                       14 LOAD_METHOD              1 (lower)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 LOAD_CONST               1 (('unnest', 'explode'))
                       52 CONTAINS_OP              0
                       54 POP_JUMP_FORWARD_IF_FALSE    45 (to 146)
          
-         261          56 LOAD_GLOBAL              5 (NULL + sqlglot)
+         258          56 LOAD_GLOBAL              5 (NULL + sqlglot)
                       68 LOAD_ATTR                3 (parse_one)
          
-         262          78 LOAD_FAST                0 (node)
+         259          78 LOAD_FAST                0 (node)
                       80 LOAD_METHOD              4 (sql)
                      102 LOAD_CONST               2 ('trino')
                      104 KW_NAMES                 3
                      106 PRECALL                  1
                      110 CALL                     1
          
-         264         120 LOAD_CONST               4 ("-- WARNING: You can't use explode/unnest inside SELECT anymore, it must be LATERAL or CROSS JOIN instead. Check out the docs here: https://dune.com/docs/query/syntax-differences/")
+         261         120 LOAD_CONST               4 ("-- WARNING: You can't use explode/unnest inside SELECT anymore, it must be LATERAL or CROSS JOIN instead. Check out the docs here: https://dune.com/docs/query/syntax-differences/")
          
-         262         122 BINARY_OP                0 (+)
+         259         122 BINARY_OP                0 (+)
          
-         267         126 LOAD_CONST               2 ('trino')
+         264         126 LOAD_CONST               2 ('trino')
          
-         261         128 KW_NAMES                 5
+         258         128 KW_NAMES                 5
                      130 PRECALL                  2
                      134 CALL                     2
                      144 RETURN_VALUE
          
-         269     >>  146 LOAD_FAST                0 (node)
+         266     >>  146 LOAD_FAST                0 (node)
                      148 RETURN_VALUE
          consts
             'Add a warning to the query if there is an unnest function call'
             ('unnest', 'explode')
             'trino'
             ('dialect',)
             "-- WARNING: You can't use explode/unnest inside SELECT anymore, it must be LATERAL or CROSS JOIN instead. Check out the docs here: https://dune.com/docs/query/syntax-differences/"
             ('read',)
          names      ('name', 'lower', 'sqlglot', 'parse_one', 'sql')
          varnames   ('node',)
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'warn_unnest'
-         firstlineno 258
+         firstlineno 255
          lnotab 0x0202360116012a0202fe040502fa1208
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 5
          flags     : 3
          code
             0x97007c006a000000000000000000a00100000000000000000000000000
             00000000000000a6000000ab00000000000000000064017600722d740500
             0000000000000000006a0300000000000000007c00a00400000000000000
             000000000000000000000000006402ac03a6010000ab0100000000000000
             0064047a0000006402ac05a6020000ab02000000000000000053007c0053
             00
-         272           0 RESUME                   0
+         269           0 RESUME                   0
          
-         274           2 LOAD_FAST                0 (node)
+         271           2 LOAD_FAST                0 (node)
                        4 LOAD_ATTR                0 (name)
                       14 LOAD_METHOD              1 (lower)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 LOAD_CONST               1 (('generate_series', 'sequence'))
                       52 CONTAINS_OP              0
                       54 POP_JUMP_FORWARD_IF_FALSE    45 (to 146)
          
-         275          56 LOAD_GLOBAL              5 (NULL + sqlglot)
+         272          56 LOAD_GLOBAL              5 (NULL + sqlglot)
                       68 LOAD_ATTR                3 (parse_one)
          
-         276          78 LOAD_FAST                0 (node)
+         273          78 LOAD_FAST                0 (node)
                       80 LOAD_METHOD              4 (sql)
                      102 LOAD_CONST               2 ('trino')
                      104 KW_NAMES                 3
                      106 PRECALL                  1
                      110 CALL                     1
          
-         278         120 LOAD_CONST               4 ('-- WARNING: Check out the docs for example of time series generation: https://dune.com/docs/query/syntax-differences/')
+         275         120 LOAD_CONST               4 ('-- WARNING: Check out the docs for example of time series generation: https://dune.com/docs/query/syntax-differences/')
          
-         276         122 BINARY_OP                0 (+)
+         273         122 BINARY_OP                0 (+)
          
-         281         126 LOAD_CONST               2 ('trino')
+         278         126 LOAD_CONST               2 ('trino')
          
-         275         128 KW_NAMES                 5
+         272         128 KW_NAMES                 5
                      130 PRECALL                  2
                      134 CALL                     2
                      144 RETURN_VALUE
          
-         283     >>  146 LOAD_FAST                0 (node)
+         280     >>  146 LOAD_FAST                0 (node)
                      148 RETURN_VALUE
          consts
             'Add a warning that links to docs if the query uses generate_series/sequence'
             ('generate_series', 'sequence')
             'trino'
             ('dialect',)
             '-- WARNING: Check out the docs for example of time series generation: https://dune.com/docs/query/syntax-differences/'
             ('read',)
          names      ('name', 'lower', 'sqlglot', 'parse_one', 'sql')
          varnames   ('node',)
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'warn_sequence'
-         firstlineno 272
+         firstlineno 269
          lnotab 0x0202360116012a0202fe040502fa1208
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 7
          flags     : 3
          code
             0x9700640144005d427d017401000000000000000000006a010000000000
             00000064027401000000000000000000006a0200000000000000007c01a6
             010000ab0100000000000000007a00000064037a00000064047c017a0000
             0064047a0000007c007400000000000000000000006a0300000000000000
             00ac05a6040000ab0400000000000000007d008c437c005300
-         286           0 RESUME                   0
+         283           0 RESUME                   0
          
-         287           2 LOAD_CONST               1 (('replace',))
+         284           2 LOAD_CONST               1 (('replace',))
                        4 GET_ITER
                  >>    6 FOR_ITER                66 (to 140)
                        8 STORE_FAST               1 (keyword)
          
-         289          10 LOAD_GLOBAL              1 (NULL + re)
+         286          10 LOAD_GLOBAL              1 (NULL + re)
                       22 LOAD_ATTR                1 (sub)
          
-         290          32 LOAD_CONST               2 ('\\b')
+         287          32 LOAD_CONST               2 ('\\b')
                       34 LOAD_GLOBAL              1 (NULL + re)
                       46 LOAD_ATTR                2 (escape)
                       56 LOAD_FAST                1 (keyword)
                       58 PRECALL                  1
                       62 CALL                     1
                       72 BINARY_OP                0 (+)
                       76 LOAD_CONST               3 ('(?!\\()')
                       78 BINARY_OP                0 (+)
          
-         291          82 LOAD_CONST               4 ('"')
+         288          82 LOAD_CONST               4 ('"')
                       84 LOAD_FAST                1 (keyword)
                       86 BINARY_OP                0 (+)
                       90 LOAD_CONST               4 ('"')
                       92 BINARY_OP                0 (+)
          
-         292          96 LOAD_FAST                0 (query)
+         289          96 LOAD_FAST                0 (query)
          
-         293          98 LOAD_GLOBAL              0 (re)
+         290          98 LOAD_GLOBAL              0 (re)
                      110 LOAD_ATTR                3 (IGNORECASE)
          
-         289         120 KW_NAMES                 5
+         286         120 KW_NAMES                 5
                      122 PRECALL                  4
                      126 CALL                     4
                      136 STORE_FAST               0 (query)
                      138 JUMP_BACKWARD           67 (to 6)
          
-         295     >>  140 LOAD_FAST                0 (query)
+         292     >>  140 LOAD_FAST                0 (query)
                      142 RETURN_VALUE
          consts
             None
             ('replace',)
             '\\b'
             '(?!\\()'
             '"'
             ('flags',)
          names      ('re', 'sub', 'escape', 'IGNORECASE')
          varnames   ('query', 'keyword')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'prep_query'
-         firstlineno 286
+         firstlineno 283
          lnotab 0x02010802160132010e01020116fc1406
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000007c00a00200
             000000000000000000000000000000000000006401ac02a6010000ab0100
             00000000000000a003000000000000000000000000000000000000000064
             036404a6020000ab0200000000000000006401ac05a6020000ab02000000
             00000000005300
-         298           0 RESUME                   0
+         295           0 RESUME                   0
          
-         300           2 LOAD_GLOBAL              1 (NULL + sqlglot)
+         297           2 LOAD_GLOBAL              1 (NULL + sqlglot)
                       14 LOAD_ATTR                1 (parse_one)
                       24 LOAD_FAST                0 (query)
                       26 LOAD_METHOD              2 (sql)
                       48 LOAD_CONST               1 ('trino')
                       50 KW_NAMES                 2
                       52 PRECALL                  1
                       56 CALL                     1
@@ -1899,15 +1880,15 @@
             ('read',)
          names      ('sqlglot', 'parse_one', 'sql', 'replace')
          varnames   ('query',)
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'rename_amount_column'
-         firstlineno 298
+         firstlineno 295
          lnotab 0x0202
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
@@ -1915,52 +1896,52 @@
             02a6010000ab0100000000000000007d0164037c01a00100000000000000
             00000000000000000000000000a6000000ab000000000000000000760072
             277405000000000000000000006a030000000000000000640364047c0174
             04000000000000000000006a040000000000000000ac05a6040000ab0400
             000000000000007d0164067c017a0000007d01740b000000000000000000
             006a0600000000000000007c016401ac07a6020000ab0200000000000000
             005300
-         303           0 RESUME                   0
+         300           0 RESUME                   0
          
-         305           2 LOAD_FAST                0 (node)
+         302           2 LOAD_FAST                0 (node)
                        4 LOAD_METHOD              0 (sql)
                       26 LOAD_CONST               1 ('trino')
                       28 KW_NAMES                 2
                       30 PRECALL                  1
                       34 CALL                     1
                       44 STORE_FAST               1 (query)
          
-         306          46 LOAD_CONST               3 ('bytea2numeric')
+         303          46 LOAD_CONST               3 ('bytea2numeric')
                       48 LOAD_FAST                1 (query)
                       50 LOAD_METHOD              1 (lower)
                       72 PRECALL                  0
                       76 CALL                     0
                       86 CONTAINS_OP              0
                       88 POP_JUMP_FORWARD_IF_FALSE    39 (to 168)
          
-         307          90 LOAD_GLOBAL              5 (NULL + re)
+         304          90 LOAD_GLOBAL              5 (NULL + re)
                      102 LOAD_ATTR                3 (sub)
                      112 LOAD_CONST               3 ('bytea2numeric')
                      114 LOAD_CONST               4 ('bytearray_to_bigint')
                      116 LOAD_FAST                1 (query)
                      118 LOAD_GLOBAL              4 (re)
                      130 LOAD_ATTR                4 (IGNORECASE)
                      140 KW_NAMES                 5
                      142 PRECALL                  4
                      146 CALL                     4
                      156 STORE_FAST               1 (query)
          
-         309         158 LOAD_CONST               6 ('/* !Bytea warning: We now have new bytearray functions to cover conversions and stuff like length, concat, substring, etc. Check out the docs here: https://dune.com/docs/reference/dune-v2/query-engine/#byte-array-to-numeric-functions */\n\n')
+         306         158 LOAD_CONST               6 ('/* !Bytea warning: We now have new bytearray functions to cover conversions and stuff like length, concat, substring, etc. Check out the docs here: https://dune.com/docs/reference/dune-v2/query-engine/#byte-array-to-numeric-functions */\n\n')
          
-         313         160 LOAD_FAST                1 (query)
+         310         160 LOAD_FAST                1 (query)
          
-         308         162 BINARY_OP                0 (+)
+         305         162 BINARY_OP                0 (+)
                      166 STORE_FAST               1 (query)
          
-         314     >>  168 LOAD_GLOBAL             11 (NULL + sqlglot)
+         311     >>  168 LOAD_GLOBAL             11 (NULL + sqlglot)
                      180 LOAD_ATTR                6 (parse_one)
                      190 LOAD_FAST                1 (query)
                      192 LOAD_CONST               1 ('trino')
                      194 KW_NAMES                 7
                      196 PRECALL                  2
                      200 CALL                     2
                      210 RETURN_VALUE
@@ -1975,31 +1956,31 @@
             ('read',)
          names      ('sql', 'lower', 're', 'sub', 'IGNORECASE', 'sqlglot', 'parse_one')
          varnames   ('node', 'query')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'bytea2numeric'
-         firstlineno 303
+         firstlineno 300
          lnotab 0x02022c012c014402020402fb0606
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
             0x970064017d017401000000000000000000006a0100000000000000007c
             0164027c007400000000000000000000006a020000000000000000ac03a6
             040000ab0400000000000000005300
-         317           0 RESUME                   0
+         314           0 RESUME                   0
          
-         319           2 LOAD_CONST               1 ('lower\\(\\s*[\'\\"]\\{\\{(.*?)\\}\\}[\'\\"]\\s*\\)')
+         316           2 LOAD_CONST               1 ('lower\\(\\s*[\'\\"]\\{\\{(.*?)\\}\\}[\'\\"]\\s*\\)')
                        4 STORE_FAST               1 (pattern)
          
-         320           6 LOAD_GLOBAL              1 (NULL + re)
+         317           6 LOAD_GLOBAL              1 (NULL + re)
                       18 LOAD_ATTR                1 (sub)
                       28 LOAD_FAST                1 (pattern)
                       30 LOAD_CONST               2 ('{{\\1}}')
                       32 LOAD_FAST                0 (query)
                       34 LOAD_GLOBAL              0 (re)
                       46 LOAD_ATTR                2 (IGNORECASE)
                       56 KW_NAMES                 3
@@ -2013,95 +1994,95 @@
             ('flags',)
          names      ('re', 'sub', 'IGNORECASE')
          varnames   ('query', 'pattern')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'fix_bytearray_param'
-         firstlineno 317
+         firstlineno 314
          lnotab 0x02020401
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
             0x970064017d017401000000000000000000006a0100000000000000007c
             0164027c007400000000000000000000006a020000000000000000ac03a6
             040000ab0400000000000000007d027c025300
-         323           0 RESUME                   0
+         320           0 RESUME                   0
          
-         327           2 LOAD_CONST               1 ('lower\\(\\s*[\'\\"]0x(.*?)[\'\\"]\\s*\\)')
+         324           2 LOAD_CONST               1 ('lower\\(\\s*[\'\\"]0x(.*?)[\'\\"]\\s*\\)')
                        4 STORE_FAST               1 (pattern)
          
-         328           6 LOAD_GLOBAL              1 (NULL + re)
+         325           6 LOAD_GLOBAL              1 (NULL + re)
                       18 LOAD_ATTR                1 (sub)
                       28 LOAD_FAST                1 (pattern)
                       30 LOAD_CONST               2 ('0x\\1')
                       32 LOAD_FAST                0 (query)
                       34 LOAD_GLOBAL              0 (re)
                       46 LOAD_ATTR                2 (IGNORECASE)
                       56 KW_NAMES                 3
                       58 PRECALL                  4
                       62 CALL                     4
                       72 STORE_FAST               2 (substituted)
          
-         329          74 LOAD_FAST                2 (substituted)
+         326          74 LOAD_FAST                2 (substituted)
                       76 RETURN_VALUE
          consts
             "Remove lower function call around '0x...' string literals, and remove the string since we have native hex types.\n\n    This has to happen after SQLGlot, since it will parse a bare 0x as a string literal"
             'lower\\(\\s*[\'\\"]0x(.*?)[\'\\"]\\s*\\)'
             '0x\\1'
             ('flags',)
          names      ('re', 'sub', 'IGNORECASE')
          varnames   ('query', 'pattern', 'substituted')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'fix_bytearray_lower'
-         firstlineno 323
+         firstlineno 320
          lnotab 0x020404014401
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 6
          flags     : 3
          code
             0x9700740000000000000000000000740200000000000000000000740400
             000000000000000000740600000000000000000000740800000000000000
             00000064019c057c00190000000000000000005300
-         332           0 RESUME                   0
+         329           0 RESUME                   0
          
-         334           2 LOAD_GLOBAL              0 (chain_where_gnosis)
+         331           2 LOAD_GLOBAL              0 (chain_where_gnosis)
          
-         335          14 LOAD_GLOBAL              2 (chain_where_optimism)
+         332          14 LOAD_GLOBAL              2 (chain_where_optimism)
          
-         336          26 LOAD_GLOBAL              4 (chain_where_bnb)
+         333          26 LOAD_GLOBAL              4 (chain_where_bnb)
          
-         337          38 LOAD_GLOBAL              6 (chain_where_polygon)
+         334          38 LOAD_GLOBAL              6 (chain_where_polygon)
          
-         338          50 LOAD_GLOBAL              8 (chain_where_ethereum)
+         335          50 LOAD_GLOBAL              8 (chain_where_ethereum)
          
-         333          62 LOAD_CONST               1 (('gnosis', 'optimism', 'bnb', 'polygon', 'ethereum'))
+         330          62 LOAD_CONST               1 (('gnosis', 'optimism', 'bnb', 'polygon', 'ethereum'))
                       64 BUILD_CONST_KEY_MAP      5
          
-         339          66 LOAD_FAST                0 (dataset)
+         336          66 LOAD_FAST                0 (dataset)
          
-         333          68 BINARY_SUBSCR
+         330          68 BINARY_SUBSCR
                       78 RETURN_VALUE
          consts
             None
             ('gnosis', 'optimism', 'bnb', 'polygon', 'ethereum')
          names      ('chain_where_gnosis', 'chain_where_optimism', 'chain_where_bnb', 'chain_where_polygon', 'chain_where_ethereum')
          varnames   ('dataset',)
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'chain_where'
-         firstlineno 332
+         firstlineno 329
          lnotab 0x02020c010c010c010c010cfb040602fa
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 11
          flags     : 3
          code
@@ -2111,170 +2092,170 @@
             000000000000000000740a00000000000000000000740c00000000000000
             000000740e00000000000000000000741000000000000000000000741300
             0000000000000000007c01a6010000ab0100000000000000007414000000
             000000000000007416000000000000000000007418000000000000000000
             00660b7d037c0344005d177d047c02a00d00000000000000000000000000
             000000000000007c04a6010000ab0100000000000000007d028c187c0253
             00
-         342           0 RESUME                   0
+         339           0 RESUME                   0
          
-         346           2 LOAD_GLOBAL              1 (NULL + sqlglot)
+         343           2 LOAD_GLOBAL              1 (NULL + sqlglot)
                       14 LOAD_ATTR                1 (parse_one)
                       24 LOAD_FAST                0 (query)
                       26 LOAD_CONST               1 ('trino')
                       28 KW_NAMES                 2
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (query_tree)
          
-         348          46 LOAD_GLOBAL              5 (NULL + postgres_table_replacements)
+         345          46 LOAD_GLOBAL              5 (NULL + postgres_table_replacements)
                       58 LOAD_FAST                1 (dataset)
                       60 PRECALL                  1
                       64 CALL                     1
          
-         349          74 LOAD_GLOBAL              6 (fix_boolean)
+         346          74 LOAD_GLOBAL              6 (fix_boolean)
          
-         350          86 LOAD_GLOBAL              8 (cast_numeric)
+         347          86 LOAD_GLOBAL              8 (cast_numeric)
          
-         351          98 LOAD_GLOBAL             10 (cast_timestamp)
+         348          98 LOAD_GLOBAL             10 (cast_timestamp)
          
-         352         110 LOAD_GLOBAL             12 (warn_unnest)
+         349         110 LOAD_GLOBAL             12 (warn_unnest)
          
-         353         122 LOAD_GLOBAL             14 (warn_sequence)
+         350         122 LOAD_GLOBAL             14 (warn_sequence)
          
-         354         134 LOAD_GLOBAL             16 (dex_trades_fixes)
+         351         134 LOAD_GLOBAL             16 (dex_trades_fixes)
          
-         355         146 LOAD_GLOBAL             19 (NULL + chain_where)
+         352         146 LOAD_GLOBAL             19 (NULL + chain_where)
                      158 LOAD_FAST                1 (dataset)
                      160 PRECALL                  1
                      164 CALL                     1
          
-         356         174 LOAD_GLOBAL             20 (bytearray_parameter_fix)
+         353         174 LOAD_GLOBAL             20 (bytearray_parameter_fix)
          
-         357         186 LOAD_GLOBAL             22 (rename_amount_column)
+         354         186 LOAD_GLOBAL             22 (rename_amount_column)
          
-         358         198 LOAD_GLOBAL             24 (bytea2numeric)
+         355         198 LOAD_GLOBAL             24 (bytea2numeric)
          
-         347         210 BUILD_TUPLE             11
+         344         210 BUILD_TUPLE             11
                      212 STORE_FAST               3 (transforms)
          
-         360         214 LOAD_FAST                3 (transforms)
+         357         214 LOAD_FAST                3 (transforms)
                      216 GET_ITER
                  >>  218 FOR_ITER                23 (to 266)
                      220 STORE_FAST               4 (f)
          
-         361         222 LOAD_FAST                2 (query_tree)
+         358         222 LOAD_FAST                2 (query_tree)
                      224 LOAD_METHOD             13 (transform)
                      246 LOAD_FAST                4 (f)
                      248 PRECALL                  1
                      252 CALL                     1
                      262 STORE_FAST               2 (query_tree)
                      264 JUMP_BACKWARD           24 (to 218)
          
-         362     >>  266 LOAD_FAST                2 (query_tree)
+         359     >>  266 LOAD_FAST                2 (query_tree)
                      268 RETURN_VALUE
          consts
             "Apply a series of transforms to the query tree, recursively using SQLGlot's recursive transform function.\n\n    Each transform takes and returns a sqlglot.Expression"
             'trino'
             ('read',)
          names      ('sqlglot', 'parse_one', 'postgres_table_replacements', 'fix_boolean', 'cast_numeric', 'cast_timestamp', 'warn_unnest', 'warn_sequence', 'dex_trades_fixes', 'chain_where', 'bytearray_parameter_fix', 'rename_amount_column', 'bytea2numeric', 'transform')
          varnames   ('query', 'dataset', 'query_tree', 'transforms', 'f')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'postgres_transforms'
-         firstlineno 342
+         firstlineno 339
          lnotab
             0x02042c021c010c010c010c010c010c010c011c010c010c010cf5040d08
             012c01
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
             0x970064017d017401000000000000000000006a0100000000000000007c
             0164027c007400000000000000000000006a020000000000000000ac03a6
             040000ab0400000000000000007d027c025300
-         365           0 RESUME                   0
+         362           0 RESUME                   0
          
-         369           2 LOAD_CONST               1 ("'0x(.*?)'")
+         366           2 LOAD_CONST               1 ("'0x(.*?)'")
                        4 STORE_FAST               1 (pattern)
          
-         370           6 LOAD_GLOBAL              1 (NULL + re)
+         367           6 LOAD_GLOBAL              1 (NULL + re)
                       18 LOAD_ATTR                1 (sub)
                       28 LOAD_FAST                1 (pattern)
                       30 LOAD_CONST               2 ('0x\\1')
                       32 LOAD_FAST                0 (query)
                       34 LOAD_GLOBAL              0 (re)
                       46 LOAD_ATTR                2 (IGNORECASE)
                       56 KW_NAMES                 3
                       58 PRECALL                  4
                       62 CALL                     4
                       72 STORE_FAST               2 (substituted)
          
-         371          74 LOAD_FAST                2 (substituted)
+         368          74 LOAD_FAST                2 (substituted)
                       76 RETURN_VALUE
          consts
             "Remove string quotes around '0x...' string literals\n\n    This has to happen after SQLGlot, since it will parse a bare 0x as a string literal"
             "'0x(.*?)'"
             '0x\\1'
             ('flags',)
          names      ('re', 'sub', 'IGNORECASE')
          varnames   ('query', 'pattern', 'substituted')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'remove_quotes_around_0x_strings'
-         firstlineno 365
+         firstlineno 362
          lnotab 0x020404014401
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
             0x97007c00a00000000000000000000000000000000000000000006401ac
             02a6010000ab0100000000000000007d0164037c01a00100000000000000
             00000000000000000000000000a6000000ab000000000000000000760072
             227405000000000000000000006a030000000000000000640464057c0174
             04000000000000000000006a040000000000000000ac06a6040000ab0400
             000000000000007d01740b000000000000000000006a0600000000000000
             007c016401ac07a6020000ab0200000000000000005300
-         374           0 RESUME                   0
+         371           0 RESUME                   0
          
-         376           2 LOAD_FAST                0 (node)
+         373           2 LOAD_FAST                0 (node)
                        4 LOAD_METHOD              0 (sql)
                       26 LOAD_CONST               1 ('trino')
                       28 KW_NAMES                 2
                       30 PRECALL                  1
                       34 CALL                     1
                       44 STORE_FAST               1 (query)
          
-         377          46 LOAD_CONST               3 ('timestamp(')
+         374          46 LOAD_CONST               3 ('timestamp(')
                       48 LOAD_FAST                1 (query)
                       50 LOAD_METHOD              1 (lower)
                       72 PRECALL                  0
                       76 CALL                     0
                       86 CONTAINS_OP              0
                       88 POP_JUMP_FORWARD_IF_FALSE    34 (to 158)
          
-         378          90 LOAD_GLOBAL              5 (NULL + re)
+         375          90 LOAD_GLOBAL              5 (NULL + re)
                      102 LOAD_ATTR                3 (sub)
                      112 LOAD_CONST               4 ('timestamp')
                      114 LOAD_CONST               5 ('from_unixtime')
                      116 LOAD_FAST                1 (query)
                      118 LOAD_GLOBAL              4 (re)
                      130 LOAD_ATTR                4 (IGNORECASE)
                      140 KW_NAMES                 6
                      142 PRECALL                  4
                      146 CALL                     4
                      156 STORE_FAST               1 (query)
          
-         379     >>  158 LOAD_GLOBAL             11 (NULL + sqlglot)
+         376     >>  158 LOAD_GLOBAL             11 (NULL + sqlglot)
                      170 LOAD_ATTR                6 (parse_one)
                      180 LOAD_FAST                1 (query)
                      182 LOAD_CONST               1 ('trino')
                      184 KW_NAMES                 7
                      186 PRECALL                  2
                      190 CALL                     2
                      200 RETURN_VALUE
@@ -2289,148 +2270,148 @@
             ('read',)
          names      ('sql', 'lower', 're', 'sub', 'IGNORECASE', 'sqlglot', 'parse_one')
          varnames   ('node', 'query')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'spark_function_replacements'
-         firstlineno 374
+         firstlineno 371
          lnotab 0x02022c012c014401
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 7
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000007c006401ac
             02a6020000ab0200000000000000007d0174040000000000000000000074
             0600000000000000000000740800000000000000000000740a0000000000
             0000000000740c00000000000000000000740e0000000000000000000074
             100000000000000000000066077d027c0244005d177d037c01a009000000
             00000000000000000000000000000000007c03a6010000ab010000000000
             0000007d018c187c015300
-         382           0 RESUME                   0
+         379           0 RESUME                   0
          
-         386           2 LOAD_GLOBAL              1 (NULL + sqlglot)
+         383           2 LOAD_GLOBAL              1 (NULL + sqlglot)
                       14 LOAD_ATTR                1 (parse_one)
                       24 LOAD_FAST                0 (query)
                       26 LOAD_CONST               1 ('trino')
                       28 KW_NAMES                 2
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               1 (query_tree)
          
-         388          46 LOAD_GLOBAL              4 (fix_boolean)
+         385          46 LOAD_GLOBAL              4 (fix_boolean)
          
-         389          58 LOAD_GLOBAL              6 (cast_numeric)
+         386          58 LOAD_GLOBAL              6 (cast_numeric)
          
-         390          70 LOAD_GLOBAL              8 (cast_timestamp)
+         387          70 LOAD_GLOBAL              8 (cast_timestamp)
          
-         391          82 LOAD_GLOBAL             10 (warn_unnest)
+         388          82 LOAD_GLOBAL             10 (warn_unnest)
          
-         392          94 LOAD_GLOBAL             12 (warn_sequence)
+         389          94 LOAD_GLOBAL             12 (warn_sequence)
          
-         393         106 LOAD_GLOBAL             14 (bytea2numeric)
+         390         106 LOAD_GLOBAL             14 (bytea2numeric)
          
-         394         118 LOAD_GLOBAL             16 (spark_function_replacements)
+         391         118 LOAD_GLOBAL             16 (spark_function_replacements)
          
-         387         130 BUILD_TUPLE              7
+         384         130 BUILD_TUPLE              7
                      132 STORE_FAST               2 (transforms)
          
-         396         134 LOAD_FAST                2 (transforms)
+         393         134 LOAD_FAST                2 (transforms)
                      136 GET_ITER
                  >>  138 FOR_ITER                23 (to 186)
                      140 STORE_FAST               3 (f)
          
-         397         142 LOAD_FAST                1 (query_tree)
+         394         142 LOAD_FAST                1 (query_tree)
                      144 LOAD_METHOD              9 (transform)
                      166 LOAD_FAST                3 (f)
                      168 PRECALL                  1
                      172 CALL                     1
                      182 STORE_FAST               1 (query_tree)
                      184 JUMP_BACKWARD           24 (to 138)
          
-         398     >>  186 LOAD_FAST                1 (query_tree)
+         395     >>  186 LOAD_FAST                1 (query_tree)
                      188 RETURN_VALUE
          consts
             "Apply a series of transforms to the query tree, recursively using SQLGlot's recursive transform function.\n\n    Each transform takes and returns a sqlglot.Expression"
             'trino'
             ('read',)
          names      ('sqlglot', 'parse_one', 'fix_boolean', 'cast_numeric', 'cast_timestamp', 'warn_unnest', 'warn_sequence', 'bytea2numeric', 'spark_function_replacements', 'transform')
          varnames   ('query', 'query_tree', 'transforms', 'f')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'spark_transforms'
-         firstlineno 382
+         firstlineno 379
          lnotab 0x02042c020c010c010c010c010c010c010cf9040908012c01
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
          flags     : 3
          code
             0x970064017c00a0000000000000000000000000000000000000000000a6
             000000ab0000000000000000007600720564027c007a0000007d00740300
             0000000000000000006a02000000000000000064037c00a6020000ab0200
             00000000000000720564047c007a0000007d0064057c00a0000000000000
             000000000000000000000000000000a6000000ab00000000000000000076
             00720564067c007a0000007d0064077c007a0000005300
-         401           0 RESUME                   0
+         398           0 RESUME                   0
          
-         403           2 LOAD_CONST               1 ("lower('{{")
+         400           2 LOAD_CONST               1 ("lower('{{")
                        4 LOAD_FAST                0 (query)
                        6 LOAD_METHOD              0 (lower)
                       28 PRECALL                  0
                       32 CALL                     0
                       42 CONTAINS_OP              0
                       44 POP_JUMP_FORWARD_IF_FALSE     5 (to 56)
          
-         405          46 LOAD_CONST               2 ("/* !Bytea parameter warning: Make sure to change \\x to 0x in the parameters, bytea types are native now (no need for quotes or lower or \\x)' */\n\n")
+         402          46 LOAD_CONST               2 ("/* !Bytea parameter warning: Make sure to change \\x to 0x in the parameters, bytea types are native now (no need for quotes or lower or \\x)' */\n\n")
          
-         408          48 LOAD_FAST                0 (query)
+         405          48 LOAD_FAST                0 (query)
          
-         404          50 BINARY_OP                0 (+)
+         401          50 BINARY_OP                0 (+)
                       54 STORE_FAST               0 (query)
          
-         411     >>   56 LOAD_GLOBAL              3 (NULL + re)
+         408     >>   56 LOAD_GLOBAL              3 (NULL + re)
                       68 LOAD_ATTR                2 (search)
                       78 LOAD_CONST               3 ('\\[.*\\]')
                       80 LOAD_FAST                0 (query)
                       82 PRECALL                  2
                       86 CALL                     2
                       96 POP_JUMP_FORWARD_IF_FALSE     5 (to 108)
          
-         413          98 LOAD_CONST               4 ('/* !Array warning: Arrays in dune SQL are indexed from 1, not 0. The migrator will not catch this if you indexed using variables */\n\n')
+         410          98 LOAD_CONST               4 ('/* !Array warning: Arrays in dune SQL are indexed from 1, not 0. The migrator will not catch this if you indexed using variables */\n\n')
          
-         416         100 LOAD_FAST                0 (query)
+         413         100 LOAD_FAST                0 (query)
          
-         412         102 BINARY_OP                0 (+)
+         409         102 BINARY_OP                0 (+)
                      106 STORE_FAST               0 (query)
          
-         418     >>  108 LOAD_CONST               5 ('dune_user_generated')
+         415     >>  108 LOAD_CONST               5 ('dune_user_generated')
                      110 LOAD_FAST                0 (query)
                      112 LOAD_METHOD              0 (lower)
                      134 PRECALL                  0
                      138 CALL                     0
                      148 CONTAINS_OP              0
                      150 POP_JUMP_FORWARD_IF_FALSE     5 (to 162)
          
-         420         152 LOAD_CONST               6 ("/* !Generated view warning: you can't query views in dune_user_generated anymore. All queries in DuneSQL are by default views though (try querying the table 'query_1747157') */\n\n")
+         417         152 LOAD_CONST               6 ("/* !Generated view warning: you can't query views in dune_user_generated anymore. All queries in DuneSQL are by default views though (try querying the table 'query_1747157') */\n\n")
          
-         423         154 LOAD_FAST                0 (query)
+         420         154 LOAD_FAST                0 (query)
          
-         419         156 BINARY_OP                0 (+)
+         416         156 BINARY_OP                0 (+)
                      160 STORE_FAST               0 (query)
          
-         427     >>  162 LOAD_CONST               7 ("/* Success! If you're still running into issues, check out https://dune.com/docs/query/syntax-differences/ or reach out in the #dune-sql Discord channel. */\n\n")
+         424     >>  162 LOAD_CONST               7 ("/* Success! If you're still running into issues, check out https://dune.com/docs/query/syntax-differences/ or reach out in the #dune-sql Discord channel. */\n\n")
          
-         430         164 LOAD_FAST                0 (query)
+         427         164 LOAD_FAST                0 (query)
          
-         426         166 BINARY_OP                0 (+)
+         423         166 BINARY_OP                0 (+)
                      170 RETURN_VALUE
          consts
             "Add a success banner at the top, and look for a few cases of things we don't fix and add a warning if present"
             "lower('{{"
             "/* !Bytea parameter warning: Make sure to change \\x to 0x in the parameters, bytea types are native now (no need for quotes or lower or \\x)' */\n\n"
             '\\[.*\\]'
             '/* !Array warning: Arrays in dune SQL are indexed from 1, not 0. The migrator will not catch this if you indexed using variables */\n\n'
@@ -2439,22 +2420,83 @@
             "/* Success! If you're still running into issues, check out https://dune.com/docs/query/syntax-differences/ or reach out in the #dune-sql Discord channel. */\n\n"
          names      ('lower', 're', 'search')
          varnames   ('query',)
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'add_warnings_and_banner'
-         firstlineno 401
+         firstlineno 398
          lnotab
             0x02022c02020302fc06072a02020302fc06062c02020302fc0608020302
             fc
-   names      ('re', 'functools', 'partial', 'sqlglot', 'dune.harmonizer.table_replacements', 'postgres_table_replacements', 'extract_nested_select', 'recurse_where', 'chain_where_blockchain', 'chain_where_ethereum', 'chain_where_gnosis', 'chain_where_optimism', 'chain_where_bnb', 'chain_where_polygon', 'dex_trades_fixes', 'param_left_placeholder', 'param_right_placeholder', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'single_quoted_param_left_placeholder', 'single_quoted_param_right_placeholder', 'bytearray_parameter_fix', 'cast_numeric', 'cast_timestamp', 'fix_boolean', 'warn_unnest', 'warn_sequence', 'prep_query', 'rename_amount_column', 'bytea2numeric', 'fix_bytearray_param', 'fix_bytearray_lower', 'chain_where', 'postgres_transforms', 'remove_quotes_around_0x_strings', 'spark_function_replacements', 'spark_transforms', 'add_warnings_and_banner')
+      code
+         argcount  : 1
+         nlocals   : 1
+         stacksize : 4
+         flags     : 3
+         code
+            0x97007c00a0000000000000000000000000000000000000000000640174
+            0200000000000000000000a6020000ab020000000000000000a000000000
+            000000000000000000000000000000000064027404000000000000000000
+            00a6020000ab020000000000000000a00000000000000000000000000000
+            0000000000000064036404a6020000ab020000000000000000a000000000
+            000000000000000000000000000000000064056404a6020000ab02000000
+            0000000000a0030000000000000000000000000000000000000000a60000
+            00ab0000000000000000005300
+         430           0 RESUME                   0
+         
+         432           2 LOAD_FAST                0 (p)
+                       4 LOAD_METHOD              0 (replace)
+                      26 LOAD_CONST               1 ('{{')
+                      28 LOAD_GLOBAL              2 (param_left_placeholder)
+                      40 PRECALL                  2
+                      44 CALL                     2
+         
+         433          54 LOAD_METHOD              0 (replace)
+                      76 LOAD_CONST               2 ('}}')
+                      78 LOAD_GLOBAL              4 (param_right_placeholder)
+                      90 PRECALL                  2
+                      94 CALL                     2
+         
+         434         104 LOAD_METHOD              0 (replace)
+                     126 LOAD_CONST               3 (' ')
+                     128 LOAD_CONST               4 ('_')
+                     130 PRECALL                  2
+                     134 CALL                     2
+         
+         435         144 LOAD_METHOD              0 (replace)
+                     166 LOAD_CONST               5 ('-')
+                     168 LOAD_CONST               4 ('_')
+                     170 PRECALL                  2
+                     174 CALL                     2
+         
+         436         184 LOAD_METHOD              3 (lower)
+                     206 PRECALL                  0
+                     210 CALL                     0
+         
+         431         220 RETURN_VALUE
+         consts
+            None
+            '{{'
+            '}}'
+            ' '
+            '_'
+            '-'
+         names      ('replace', 'param_left_placeholder', 'param_right_placeholder', 'lower')
+         varnames   ('p',)
+         freevars   ()
+         cellvars   ()
+         filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
+         name       'parameter_placeholder'
+         firstlineno 430
+         lnotab 0x0202340132012801280124fb
+   names      ('re', 'functools', 'partial', 'sqlglot', 'dune.harmonizer.table_replacements', 'postgres_table_replacements', 'extract_nested_select', 'recurse_where', 'chain_where_blockchain', 'chain_where_ethereum', 'chain_where_gnosis', 'chain_where_optimism', 'chain_where_bnb', 'chain_where_polygon', 'dex_trades_fixes', 'param_left_placeholder', 'param_right_placeholder', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'single_quoted_param_left_placeholder', 'single_quoted_param_right_placeholder', 'bytearray_parameter_fix', 'cast_numeric', 'cast_timestamp', 'fix_boolean', 'warn_unnest', 'warn_sequence', 'prep_query', 'rename_amount_column', 'bytea2numeric', 'fix_bytearray_param', 'fix_bytearray_lower', 'chain_where', 'postgres_transforms', 'remove_quotes_around_0x_strings', 'spark_function_replacements', 'spark_transforms', 'add_warnings_and_banner', 'parameter_placeholder')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020108010c0208020c030613065906121a011a011a011a011a0306
-      2c040104010a010a010a010a03061b06090612060a060e060e060c060506
-      0e06060609060a0617060906080613
+      2c040104010a010a010a010a03061b0609060f060a060e060e060c060506
+      0e06060609060a06170609060806130620
```

### Comparing `dune_harmonizer-0.3.0/dune/harmonizer/__pycache__/errors.cpython-311.pyc` & `dune_harmonizer-0.4.0/dune/harmonizer/__pycache__/errors.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xd5df4064 (Thu Apr 20 06:46:45 2023 UTC)
+moddate:  0x99154164 (Thu Apr 20 10:36:09 2023 UTC)
 files sz: 105
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `dune_harmonizer-0.3.0/dune/harmonizer/__pycache__/table_replacements.cpython-311.pyc` & `dune_harmonizer-0.4.0/dune/harmonizer/__pycache__/table_replacements.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xd5df4064 (Thu Apr 20 06:46:45 2023 UTC)
+moddate:  0x99154164 (Thu Apr 20 10:36:09 2023 UTC)
 files sz: 2018
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code 0x9700640064016c005a00640064016c015a01640284005a0264015300
```

### Comparing `dune_harmonizer-0.3.0/dune/harmonizer/custom_transforms.py` & `dune_harmonizer-0.4.0/dune/harmonizer/custom_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,16 +179,16 @@
                 flags=re.IGNORECASE,
             )
 
             return sqlglot.parse_one(final_where, read="trino")
     return node
 
 
-param_left_placeholder = "parameter_placeholder_left_bracket"
-param_right_placeholder = "parameter_placeholder_right_bracket"
+param_left_placeholder = "left_param_"
+param_right_placeholder = "_right_param"
 double_quoted_param_left_placeholder = f'"{param_left_placeholder}'
 double_quoted_param_right_placeholder = f'{param_right_placeholder}"'
 single_quoted_param_left_placeholder = f"'{param_left_placeholder}"
 single_quoted_param_right_placeholder = f"{param_right_placeholder}'"
 
 
 def bytearray_parameter_fix(node):
@@ -224,28 +224,25 @@
     if node.key == "column":
         if any(val in node.name.lower() for val in ("amount", "value")):
             return sqlglot.parse_one("cast(" + node.name + " as double)", read="trino")
     return node
 
 
 def cast_timestamp(node):
+    """Look for date-like literals and params and cast these as timestamps"""
     if node.key == "literal":
         # and contains 'yyyy-mm-dd' format then cast to timestamp
         if re.search(r"\d{4}-\d{2}-\d{2}", node.sql(dialect="trino")):
             return sqlglot.parse_one("timestamp " + node.sql(dialect="trino"), read="trino")
 
         # or if it is a param that contains date/time
-        pattern = (
-            re.escape(double_quoted_param_left_placeholder)
-            + r"(.*?)"
-            + re.escape(double_quoted_param_right_placeholder)
-        )
-        match = re.search(pattern, node.sql(dialect="trino"))
-        if match and any(d in node.sql(dialect="trino").lower() for d in ["date", "time"]):
-            return sqlglot.parse_one("timestamp '{{" + match.group(1) + "}}'", read="trino")
+        pattern = "('" + param_left_placeholder + r".*?" + param_right_placeholder + "')"
+        if any(d in node.sql(dialect="trino").lower() for d in ("date", "time")):
+            q = re.sub(pattern, r"timestamp \1", node.sql(dialect="trino"))
+            return sqlglot.parse_one(q, read="trino")
     return node
 
 
 def fix_boolean(node):
     """If node.key is 'literal' and contains 'true' or 'false' then cast to boolean"""
     if node.key == "literal":
         if any(boolean in node.sql(dialect="trino").lower() for boolean in ("true", "false")):
@@ -424,7 +421,17 @@
 
     # add note at top
     return (
         "/* Success! If you're still running into issues, check out https://dune.com/docs/query/syntax-differences/ "
         "or reach out in the #dune-sql Discord channel. */"
         "\n\n"
     ) + query
+
+
+def parameter_placeholder(p):
+    return (
+        p.replace("{{", param_left_placeholder)
+        .replace("}}", param_right_placeholder)
+        .replace(" ", "_")
+        .replace("-", "_")
+        .lower()
+    )
```

### Comparing `dune_harmonizer-0.3.0/dune/harmonizer/table_replacements.py` & `dune_harmonizer-0.4.0/dune/harmonizer/table_replacements.py`

 * *Files identical despite different names*

### Comparing `dune_harmonizer-0.3.0/dune/harmonizer/translate.py` & `dune_harmonizer-0.4.0/dune/harmonizer/translate.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 
 from dune.harmonizer.custom_transforms import (
     add_warnings_and_banner,
     double_quoted_param_left_placeholder,
     double_quoted_param_right_placeholder,
     fix_bytearray_lower,
     fix_bytearray_param,
+    parameter_placeholder,
     postgres_transforms,
     prep_query,
     remove_quotes_around_0x_strings,
-    single_quoted_param_left_placeholder,
-    single_quoted_param_right_placeholder,
     spark_transforms,
 )
 from dune.harmonizer.errors import DuneTranslationError
 
 
 def _clean_dataset(dataset):
     for d in ("gnosis", "optimism", "bnb", "polygon", "ethereum"):
@@ -26,17 +25,19 @@
     raise ValueError(f"Unknown dataset: {dataset}")
 
 
 def _translate_query(query, sqlglot_dialect, dataset=None):
     """Translate a query using SQLGLot plus custom rules"""
     try:
         # Insert placeholders for the parameters we use in Dune (`{{ param }}`), SQLGlot doesn't handle those
-        query = query.replace("{{", double_quoted_param_left_placeholder).replace(
-            "}}", double_quoted_param_right_placeholder
-        )
+        parameters = re.findall("({{.*?}})", query, flags=re.IGNORECASE)
+        parameter_map = {parameter_placeholder(p): p for p in parameters}
+        for replace, original in parameter_map.items():
+            query = query.replace(original, replace)
+
         query = prep_query(query)
 
         # Transpile to Trino
         query = sqlglot.transpile(query, read=sqlglot_dialect, write="trino", pretty=True)[0]
 
         # Perform custom transformations using SQLGlot's parsed representation
         if sqlglot_dialect == "spark":
@@ -46,20 +47,16 @@
             query = query.replace("\\x", "0x")
             query_tree = postgres_transforms(query, dataset)
 
         # Turn back to SQL
         query = query_tree.sql(dialect="trino", pretty=True)
 
         # Replace placeholders with Dune params again
-        query = (
-            query.replace(double_quoted_param_left_placeholder, "{{")
-            .replace(double_quoted_param_right_placeholder, "}}")
-            .replace(single_quoted_param_left_placeholder, "{{")
-            .replace(single_quoted_param_right_placeholder, "}}")
-        )
+        for replace, original in parameter_map.items():
+            query = query.replace(replace, original)
 
         # Non-SQLGlot transforms
         query = fix_bytearray_param(query)
         query = fix_bytearray_lower(query)
         query = remove_quotes_around_0x_strings(query)
 
         return add_warnings_and_banner(query)
```

### Comparing `dune_harmonizer-0.3.0/pyproject.toml` & `dune_harmonizer-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dune-harmonizer"
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 authors = ["Vegard Stikbakke <vegard@dune.com>"]
 readme = "README.md"
 packages = [{include = "dune"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `dune_harmonizer-0.3.0/PKG-INFO` & `dune_harmonizer-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-harmonizer
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Author: Vegard Stikbakke
 Author-email: vegard@dune.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: sqlglot (>=11.5.5,<12.0.0)
```

