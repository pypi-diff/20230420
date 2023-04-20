# Comparing `tmp/nazo_rand-0.0.6.tar.gz` & `tmp/nazo_rand-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nazo_rand-0.0.6.tar", last modified: Sun Apr 16 12:37:35 2023, max compression
+gzip compressed data, was "nazo_rand-0.0.7.tar", last modified: Thu Apr 20 14:27:20 2023, max compression
```

## Comparing `nazo_rand-0.0.6.tar` & `nazo_rand-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:37:35.718857 nazo_rand-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-16 12:37:15.000000 nazo_rand-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-16 12:37:15.000000 nazo_rand-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-16 12:37:35.718857 nazo_rand-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-16 12:37:15.000000 nazo_rand-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:37:35.718857 nazo_rand-0.0.6/nazo_rand/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-16 12:37:15.000000 nazo_rand-0.0.6/nazo_rand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   235337 2023-04-16 12:37:25.000000 nazo_rand-0.0.6/nazo_rand/nazo_rand.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-16 12:37:15.000000 nazo_rand-0.0.6/nazo_rand/nazo_rand.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-16 12:37:15.000000 nazo_rand-0.0.6/nazo_rand/nazo_rand.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-16 12:37:15.000000 nazo_rand-0.0.6/nazo_rand/nazo_rand.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-16 12:37:15.000000 nazo_rand-0.0.6/nazo_rand/nazo_rand.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:37:35.718857 nazo_rand-0.0.6/nazo_rand.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-16 12:37:35.000000 nazo_rand-0.0.6/nazo_rand.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-16 12:37:35.000000 nazo_rand-0.0.6/nazo_rand.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 12:37:35.000000 nazo_rand-0.0.6/nazo_rand.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-16 12:37:35.000000 nazo_rand-0.0.6/nazo_rand.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-16 12:37:15.000000 nazo_rand-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 12:37:35.718857 nazo_rand-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-16 12:37:15.000000 nazo_rand-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:27:20.004364 nazo_rand-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-20 14:27:05.000000 nazo_rand-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-20 14:27:05.000000 nazo_rand-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-20 14:27:20.004364 nazo_rand-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-20 14:27:05.000000 nazo_rand-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:27:20.000364 nazo_rand-0.0.7/nazo_rand/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-20 14:27:05.000000 nazo_rand-0.0.7/nazo_rand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   249266 2023-04-20 14:27:09.000000 nazo_rand-0.0.7/nazo_rand/nazo_rand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-20 14:27:05.000000 nazo_rand-0.0.7/nazo_rand/nazo_rand.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-20 14:27:05.000000 nazo_rand-0.0.7/nazo_rand/nazo_rand.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-20 14:27:05.000000 nazo_rand-0.0.7/nazo_rand/nazo_rand.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-20 14:27:05.000000 nazo_rand-0.0.7/nazo_rand/nazo_rand.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 14:27:20.004364 nazo_rand-0.0.7/nazo_rand.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-20 14:27:19.000000 nazo_rand-0.0.7/nazo_rand.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-20 14:27:19.000000 nazo_rand-0.0.7/nazo_rand.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 14:27:19.000000 nazo_rand-0.0.7/nazo_rand.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 14:27:19.000000 nazo_rand-0.0.7/nazo_rand.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-20 14:27:05.000000 nazo_rand-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 14:27:20.004364 nazo_rand-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-20 14:27:05.000000 nazo_rand-0.0.7/setup.py
```

### Comparing `nazo_rand-0.0.6/LICENSE` & `nazo_rand-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nazo_rand-0.0.6/PKG-INFO` & `nazo_rand-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nazo_rand
-Version: 0.0.6
+Version: 0.0.7
 Summary: A fast random number generator for python
 Author: bymoye
 Author-email: s3moye@gmail.com
 License: Free for non-commercial use
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `nazo_rand-0.0.6/README.md` & `nazo_rand-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `nazo_rand-0.0.6/nazo_rand/nazo_rand.cpp` & `nazo_rand-0.0.7/nazo_rand/nazo_rand.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
             "nazo_rand/nazo_rand.hpp"
         ],
         "extra_compile_args": [
             "-std=c++17",
             "-O3"
         ],
         "extra_link_args": [
-            "-O3"
+            "-Wl,-O3"
         ],
         "include_dirs": [
             "nazo_rand"
         ],
         "language": "c++",
         "name": "nazo_rand.nazo_rand",
         "sources": [
@@ -994,17 +994,17 @@
 static const char *__pyx_f[] = {
   "nazo_rand/nazo_rand.pyx",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange;
 
-/* "nazo_rand/nazo_rand.pxd":12
- * cpdef int randbelow(int a)
- * cpdef int randint(int a,int b)
+/* "nazo_rand/nazo_rand.pxd":14
+ * cdef int64_t cy_random_below(int64_t number) nogil
+ * cdef int64_t cy_uniform_int_variate(int64_t a, int64_t b) nogil
  * cpdef int randrange(int start,int stop=?,int step=?)             # <<<<<<<<<<<<<<
  * cpdef double random_double(double a, double b)
  * cpdef double random_double_noargs()
  */
 struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange {
   int __pyx_n;
   int stop;
@@ -1325,14 +1325,20 @@
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
+/* CIntFromPy.proto */
+static CYTHON_INLINE int64_t __Pyx_PyInt_As_int64_t(PyObject *);
+
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int64_t(int64_t value);
+
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* FastTypeChecks.proto */
@@ -1354,48 +1360,50 @@
 /* FunctionExport.proto */
 static int __Pyx_ExportFunction(const char *name, void (*f)(void), const char *sig);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 
-/* Module declarations from 'cython' */
-
 /* Module declarations from 'libc.stdint' */
 
+/* Module declarations from 'cython' */
+
 /* Module declarations from 'nazo_rand.nazo_rand' */
 static void __pyx_f_9nazo_rand_9nazo_rand_shuffle(PyObject *, int __pyx_skip_dispatch); /*proto*/
 static int __pyx_f_9nazo_rand_9nazo_rand_random_integer_noargs(int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_9nazo_rand_9nazo_rand_random_choice(PyObject *, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_9nazo_rand_9nazo_rand_random_choices(PyObject *, Py_ssize_t, int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_9nazo_rand_9nazo_rand_random_sample(PyObject *, Py_ssize_t, int __pyx_skip_dispatch); /*proto*/
-static int __pyx_f_9nazo_rand_9nazo_rand_randbelow(int, int __pyx_skip_dispatch); /*proto*/
-static int __pyx_f_9nazo_rand_9nazo_rand_randint(int, int, int __pyx_skip_dispatch); /*proto*/
+static int64_t __pyx_f_9nazo_rand_9nazo_rand_cy_random_below(int64_t); /*proto*/
+static int64_t __pyx_f_9nazo_rand_9nazo_rand_cy_uniform_int_variate(int64_t, int64_t); /*proto*/
 static int __pyx_f_9nazo_rand_9nazo_rand_randrange(int, int __pyx_skip_dispatch, struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange *__pyx_optional_args); /*proto*/
 static double __pyx_f_9nazo_rand_9nazo_rand_random_double(double, double, int __pyx_skip_dispatch); /*proto*/
 static double __pyx_f_9nazo_rand_9nazo_rand_random_double_noargs(int __pyx_skip_dispatch); /*proto*/
 #define __Pyx_MODULE_NAME "nazo_rand.nazo_rand"
 extern int __pyx_module_is_main_nazo_rand__nazo_rand;
 int __pyx_module_is_main_nazo_rand__nazo_rand = 0;
 
 /* Implementation of 'nazo_rand.nazo_rand' */
 static PyObject *__pyx_builtin_reversed;
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_ValueError;
 static const char __pyx_k_a[] = "a";
 static const char __pyx_k_b[] = "b";
+static const char __pyx_k_int[] = "int";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_step[] = "step";
 static const char __pyx_k_stop[] = "stop";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_array[] = "array";
 static const char __pyx_k_count[] = "count";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_start[] = "start";
+static const char __pyx_k_return[] = "return";
 static const char __pyx_k_randint[] = "randint";
 static const char __pyx_k_shuffle[] = "shuffle";
 static const char __pyx_k_reversed[] = "reversed";
 static const char __pyx_k_container[] = "container";
 static const char __pyx_k_randbelow[] = "randbelow";
 static const char __pyx_k_randrange[] = "randrange";
 static const char __pyx_k_ValueError[] = "ValueError";
@@ -1413,38 +1421,40 @@
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_a;
 static PyObject *__pyx_n_s_array;
 static PyObject *__pyx_n_s_b;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_container;
 static PyObject *__pyx_n_s_count;
+static PyObject *__pyx_n_u_int;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_nazo_rand_nazo_rand;
 static PyObject *__pyx_kp_s_nazo_rand_nazo_rand_pyx;
 static PyObject *__pyx_n_s_randbelow;
 static PyObject *__pyx_n_s_randint;
 static PyObject *__pyx_n_s_random_choice;
 static PyObject *__pyx_n_s_random_choices;
 static PyObject *__pyx_n_s_random_double;
 static PyObject *__pyx_n_s_random_double_noargs;
 static PyObject *__pyx_n_s_random_integer_noargs;
 static PyObject *__pyx_n_s_random_sample;
 static PyObject *__pyx_n_s_randrange;
 static PyObject *__pyx_n_s_range;
+static PyObject *__pyx_n_s_return;
 static PyObject *__pyx_n_s_reversed;
 static PyObject *__pyx_n_s_shuffle;
 static PyObject *__pyx_n_s_start;
 static PyObject *__pyx_n_s_step;
 static PyObject *__pyx_n_s_stop;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_random_integer_noargs(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_2shuffle(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_array); /* proto */
-static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_4randbelow(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_a); /* proto */
-static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_6randint(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_a, int __pyx_v_b); /* proto */
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_4randbelow(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_a); /* proto */
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_6randint(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_a, PyObject *__pyx_v_b); /* proto */
 static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_8random_choice(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_container); /* proto */
 static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_10random_choices(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_container, Py_ssize_t __pyx_v_count); /* proto */
 static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_12random_sample(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_container, Py_ssize_t __pyx_v_count); /* proto */
 static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_14randrange(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_start, int __pyx_v_stop, int __pyx_v_step); /* proto */
 static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_16random_double(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_a, double __pyx_v_b); /* proto */
 static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_18random_double_noargs(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_tuple_;
@@ -1465,39 +1475,107 @@
 static PyObject *__pyx_codeobj__14;
 static PyObject *__pyx_codeobj__16;
 static PyObject *__pyx_codeobj__18;
 static PyObject *__pyx_codeobj__19;
 /* Late includes */
 
 /* "nazo_rand/nazo_rand.pyx":15
- *     double uniform_real_variate(double a, double b)
+ *     double uniform_real_variate(double a, double b) nogil
+ * 
+ * cdef int64_t cy_random_below(int64_t number) nogil:             # <<<<<<<<<<<<<<
+ *     return random_below(number)
+ * 
+ */
+
+static int64_t __pyx_f_9nazo_rand_9nazo_rand_cy_random_below(int64_t __pyx_v_number) {
+  int64_t __pyx_r;
+
+  /* "nazo_rand/nazo_rand.pyx":16
+ * 
+ * cdef int64_t cy_random_below(int64_t number) nogil:
+ *     return random_below(number)             # <<<<<<<<<<<<<<
+ * 
+ * cdef int64_t cy_uniform_int_variate(int64_t a, int64_t b) nogil:
+ */
+  __pyx_r = Storm::random_below(__pyx_v_number);
+  goto __pyx_L0;
+
+  /* "nazo_rand/nazo_rand.pyx":15
+ *     double uniform_real_variate(double a, double b) nogil
+ * 
+ * cdef int64_t cy_random_below(int64_t number) nogil:             # <<<<<<<<<<<<<<
+ *     return random_below(number)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "nazo_rand/nazo_rand.pyx":18
+ *     return random_below(number)
+ * 
+ * cdef int64_t cy_uniform_int_variate(int64_t a, int64_t b) nogil:             # <<<<<<<<<<<<<<
+ *     return uniform_int_variate(a, b)
+ * 
+ */
+
+static int64_t __pyx_f_9nazo_rand_9nazo_rand_cy_uniform_int_variate(int64_t __pyx_v_a, int64_t __pyx_v_b) {
+  int64_t __pyx_r;
+
+  /* "nazo_rand/nazo_rand.pyx":19
+ * 
+ * cdef int64_t cy_uniform_int_variate(int64_t a, int64_t b) nogil:
+ *     return uniform_int_variate(a, b)             # <<<<<<<<<<<<<<
+ * 
+ * cpdef int random_integer_noargs():
+ */
+  __pyx_r = Storm::uniform_int_variate(__pyx_v_a, __pyx_v_b);
+  goto __pyx_L0;
+
+  /* "nazo_rand/nazo_rand.pyx":18
+ *     return random_below(number)
+ * 
+ * cdef int64_t cy_uniform_int_variate(int64_t a, int64_t b) nogil:             # <<<<<<<<<<<<<<
+ *     return uniform_int_variate(a, b)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "nazo_rand/nazo_rand.pyx":21
+ *     return uniform_int_variate(a, b)
  * 
  * cpdef int random_integer_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_int_variate_noargs()
  * 
  */
 
 static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_1random_integer_noargs(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static int __pyx_f_9nazo_rand_9nazo_rand_random_integer_noargs(CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("random_integer_noargs", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":16
+  /* "nazo_rand/nazo_rand.pyx":22
  * 
  * cpdef int random_integer_noargs():
  *     return uniform_int_variate_noargs()             # <<<<<<<<<<<<<<
  * 
  * cpdef void shuffle(list array):
  */
   __pyx_r = Storm::uniform_int_variate_noargs();
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":15
- *     double uniform_real_variate(double a, double b)
+  /* "nazo_rand/nazo_rand.pyx":21
+ *     return uniform_int_variate(a, b)
  * 
  * cpdef int random_integer_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_int_variate_noargs()
  * 
  */
 
   /* function exit code */
@@ -1525,15 +1603,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_integer_noargs", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_9nazo_rand_9nazo_rand_random_integer_noargs(0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_9nazo_rand_9nazo_rand_random_integer_noargs(0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -1542,15 +1620,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":18
+/* "nazo_rand/nazo_rand.pyx":24
  *     return uniform_int_variate_noargs()
  * 
  * cpdef void shuffle(list array):             # <<<<<<<<<<<<<<
  *     for i in reversed(range(len(array) - 1)):
  *         j = randrange(i, len(array), 1)
  */
 
@@ -1567,81 +1645,81 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("shuffle", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":19
+  /* "nazo_rand/nazo_rand.pyx":25
  * 
  * cpdef void shuffle(list array):
  *     for i in reversed(range(len(array) - 1)):             # <<<<<<<<<<<<<<
  *         j = randrange(i, len(array), 1)
  *         array[i], array[j] = array[j], array[i]
  */
   if (unlikely(__pyx_v_array == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 19, __pyx_L1_error)
+    __PYX_ERR(0, 25, __pyx_L1_error)
   }
-  __pyx_t_1 = PyList_GET_SIZE(__pyx_v_array); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_t_1 = PyList_GET_SIZE(__pyx_v_array); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 25, __pyx_L1_error)
   for (__pyx_t_2 = (__pyx_t_1 - 1)-1; __pyx_t_2 >= 0; __pyx_t_2-=1) {
     __pyx_v_i = __pyx_t_2;
 
-    /* "nazo_rand/nazo_rand.pyx":20
+    /* "nazo_rand/nazo_rand.pyx":26
  * cpdef void shuffle(list array):
  *     for i in reversed(range(len(array) - 1)):
  *         j = randrange(i, len(array), 1)             # <<<<<<<<<<<<<<
  *         array[i], array[j] = array[j], array[i]
  * 
  */
     if (unlikely(__pyx_v_array == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      __PYX_ERR(0, 20, __pyx_L1_error)
+      __PYX_ERR(0, 26, __pyx_L1_error)
     }
-    __pyx_t_3 = PyList_GET_SIZE(__pyx_v_array); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 20, __pyx_L1_error)
+    __pyx_t_3 = PyList_GET_SIZE(__pyx_v_array); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 26, __pyx_L1_error)
     __pyx_t_5.__pyx_n = 2;
     __pyx_t_5.stop = __pyx_t_3;
     __pyx_t_5.step = 1;
     __pyx_t_4 = __pyx_f_9nazo_rand_9nazo_rand_randrange(__pyx_v_i, 0, &__pyx_t_5); 
     __pyx_v_j = __pyx_t_4;
 
-    /* "nazo_rand/nazo_rand.pyx":21
+    /* "nazo_rand/nazo_rand.pyx":27
  *     for i in reversed(range(len(array) - 1)):
  *         j = randrange(i, len(array), 1)
  *         array[i], array[j] = array[j], array[i]             # <<<<<<<<<<<<<<
  * 
  * 
  */
     if (unlikely(__pyx_v_array == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 21, __pyx_L1_error)
+      __PYX_ERR(0, 27, __pyx_L1_error)
     }
     __pyx_t_6 = PyList_GET_ITEM(__pyx_v_array, __pyx_v_j);
     __Pyx_INCREF(__pyx_t_6);
     if (unlikely(__pyx_v_array == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 21, __pyx_L1_error)
+      __PYX_ERR(0, 27, __pyx_L1_error)
     }
     __pyx_t_7 = PyList_GET_ITEM(__pyx_v_array, __pyx_v_i);
     __Pyx_INCREF(__pyx_t_7);
     if (unlikely(__pyx_v_array == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 21, __pyx_L1_error)
+      __PYX_ERR(0, 27, __pyx_L1_error)
     }
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_array, __pyx_v_i, __pyx_t_6, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 0, 0) < 0)) __PYX_ERR(0, 21, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_array, __pyx_v_i, __pyx_t_6, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 0, 0) < 0)) __PYX_ERR(0, 27, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (unlikely(__pyx_v_array == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 21, __pyx_L1_error)
+      __PYX_ERR(0, 27, __pyx_L1_error)
     }
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_array, __pyx_v_j, __pyx_t_7, int, 1, __Pyx_PyInt_From_int, 1, 0, 0) < 0)) __PYX_ERR(0, 21, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_array, __pyx_v_j, __pyx_t_7, int, 1, __Pyx_PyInt_From_int, 1, 0, 0) < 0)) __PYX_ERR(0, 27, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
 
-  /* "nazo_rand/nazo_rand.pyx":18
+  /* "nazo_rand/nazo_rand.pyx":24
  *     return uniform_int_variate_noargs()
  * 
  * cpdef void shuffle(list array):             # <<<<<<<<<<<<<<
  *     for i in reversed(range(len(array) - 1)):
  *         j = randrange(i, len(array), 1)
  */
 
@@ -1661,15 +1739,15 @@
 static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_3shuffle(PyObject *__pyx_self, PyObject *__pyx_v_array) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("shuffle (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_array), (&PyList_Type), 1, "array", 1))) __PYX_ERR(0, 18, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_array), (&PyList_Type), 1, "array", 1))) __PYX_ERR(0, 24, __pyx_L1_error)
   __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_2shuffle(__pyx_self, ((PyObject*)__pyx_v_array));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -1682,15 +1760,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("shuffle", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_void_to_None(__pyx_f_9nazo_rand_9nazo_rand_shuffle(__pyx_v_array, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_void_to_None(__pyx_f_9nazo_rand_9nazo_rand_shuffle(__pyx_v_array, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -1699,149 +1777,94 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":24
- * 
- * 
- * cpdef int randbelow(int a):             # <<<<<<<<<<<<<<
- *     return random_below(a)
- * 
- */
-
-static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_5randbelow(PyObject *__pyx_self, PyObject *__pyx_arg_a); /*proto*/
-static int __pyx_f_9nazo_rand_9nazo_rand_randbelow(int __pyx_v_a, CYTHON_UNUSED int __pyx_skip_dispatch) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("randbelow", 0);
-
-  /* "nazo_rand/nazo_rand.pyx":25
+/* "nazo_rand/nazo_rand.pyx":30
  * 
- * cpdef int randbelow(int a):
- *     return random_below(a)             # <<<<<<<<<<<<<<
  * 
- * cpdef int randint(int a, int b):
- */
-  __pyx_r = Storm::random_below(__pyx_v_a);
-  goto __pyx_L0;
-
-  /* "nazo_rand/nazo_rand.pyx":24
- * 
- * 
- * cpdef int randbelow(int a):             # <<<<<<<<<<<<<<
+ * def randbelow(a:int) -> int:             # <<<<<<<<<<<<<<
  *     return random_below(a)
  * 
  */
 
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
 /* Python wrapper */
-static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_5randbelow(PyObject *__pyx_self, PyObject *__pyx_arg_a); /*proto*/
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_5randbelow(PyObject *__pyx_self, PyObject *__pyx_v_a); /*proto*/
 static PyMethodDef __pyx_mdef_9nazo_rand_9nazo_rand_5randbelow = {"randbelow", (PyCFunction)__pyx_pw_9nazo_rand_9nazo_rand_5randbelow, METH_O, 0};
-static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_5randbelow(PyObject *__pyx_self, PyObject *__pyx_arg_a) {
-  int __pyx_v_a;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_5randbelow(PyObject *__pyx_self, PyObject *__pyx_v_a) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("randbelow (wrapper)", 0);
-  assert(__pyx_arg_a); {
-    __pyx_v_a = __Pyx_PyInt_As_int(__pyx_arg_a); if (unlikely((__pyx_v_a == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 24, __pyx_L3_error)
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("nazo_rand.nazo_rand.randbelow", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_4randbelow(__pyx_self, ((int)__pyx_v_a));
+  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_4randbelow(__pyx_self, ((PyObject *)__pyx_v_a));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_4randbelow(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_a) {
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_4randbelow(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_a) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
+  int64_t __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("randbelow", 0);
+
+  /* "nazo_rand/nazo_rand.pyx":31
+ * 
+ * def randbelow(a:int) -> int:
+ *     return random_below(a)             # <<<<<<<<<<<<<<
+ * 
+ * def randint(a:int, b:int) -> int:
+ */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_9nazo_rand_9nazo_rand_randbelow(__pyx_v_a, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyInt_As_int64_t(__pyx_v_a); if (unlikely((__pyx_t_1 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int64_t(Storm::random_below(__pyx_t_1)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
   goto __pyx_L0;
 
+  /* "nazo_rand/nazo_rand.pyx":30
+ * 
+ * 
+ * def randbelow(a:int) -> int:             # <<<<<<<<<<<<<<
+ *     return random_below(a)
+ * 
+ */
+
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_AddTraceback("nazo_rand.nazo_rand.randbelow", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":27
+/* "nazo_rand/nazo_rand.pyx":33
  *     return random_below(a)
  * 
- * cpdef int randint(int a, int b):             # <<<<<<<<<<<<<<
- *     return uniform_int_variate(a, b)
+ * def randint(a:int, b:int) -> int:             # <<<<<<<<<<<<<<
+ *     return cy_uniform_int_variate(a, b)
  * 
  */
 
-static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_7randint(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_f_9nazo_rand_9nazo_rand_randint(int __pyx_v_a, int __pyx_v_b, CYTHON_UNUSED int __pyx_skip_dispatch) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("randint", 0);
-
-  /* "nazo_rand/nazo_rand.pyx":28
- * 
- * cpdef int randint(int a, int b):
- *     return uniform_int_variate(a, b)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = Storm::uniform_int_variate(__pyx_v_a, __pyx_v_b);
-  goto __pyx_L0;
-
-  /* "nazo_rand/nazo_rand.pyx":27
- *     return random_below(a)
- * 
- * cpdef int randint(int a, int b):             # <<<<<<<<<<<<<<
- *     return uniform_int_variate(a, b)
- * 
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
 /* Python wrapper */
 static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_7randint(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_9nazo_rand_9nazo_rand_7randint = {"randint", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9nazo_rand_9nazo_rand_7randint, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_7randint(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  int __pyx_v_a;
-  int __pyx_v_b;
+  PyObject *__pyx_v_a = 0;
+  PyObject *__pyx_v_b = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("randint (wrapper)", 0);
   {
@@ -1863,75 +1886,95 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("randint", 1, 2, 2, 1); __PYX_ERR(0, 27, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("randint", 1, 2, 2, 1); __PYX_ERR(0, 33, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "randint") < 0)) __PYX_ERR(0, 27, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "randint") < 0)) __PYX_ERR(0, 33, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_a = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_a == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 27, __pyx_L3_error)
-    __pyx_v_b = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_b == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 27, __pyx_L3_error)
+    __pyx_v_a = values[0];
+    __pyx_v_b = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("randint", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 27, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("randint", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 33, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("nazo_rand.nazo_rand.randint", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_6randint(__pyx_self, __pyx_v_a, __pyx_v_b);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_6randint(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_a, int __pyx_v_b) {
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_6randint(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
+  int64_t __pyx_t_1;
+  int64_t __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("randint", 0);
+
+  /* "nazo_rand/nazo_rand.pyx":34
+ * 
+ * def randint(a:int, b:int) -> int:
+ *     return cy_uniform_int_variate(a, b)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_9nazo_rand_9nazo_rand_randint(__pyx_v_a, __pyx_v_b, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyInt_As_int64_t(__pyx_v_a); if (unlikely((__pyx_t_1 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_int64_t(__pyx_v_b); if (unlikely((__pyx_t_2 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int64_t(__pyx_f_9nazo_rand_9nazo_rand_cy_uniform_int_variate(__pyx_t_1, __pyx_t_2)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
   goto __pyx_L0;
 
+  /* "nazo_rand/nazo_rand.pyx":33
+ *     return random_below(a)
+ * 
+ * def randint(a:int, b:int) -> int:             # <<<<<<<<<<<<<<
+ *     return cy_uniform_int_variate(a, b)
+ * 
+ */
+
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("nazo_rand.nazo_rand.randint", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":34
+/* "nazo_rand/nazo_rand.pyx":40
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef object random_choice(object container):             # <<<<<<<<<<<<<<
- *     cdef Py_ssize_t index = randbelow(len(container))
+ *     cdef Py_ssize_t index = cy_random_below(len(container))
  *     return container[index]
  */
 
 static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_9random_choice(PyObject *__pyx_self, PyObject *__pyx_v_container); /*proto*/
 static PyObject *__pyx_f_9nazo_rand_9nazo_rand_random_choice(PyObject *__pyx_v_container, CYTHON_UNUSED int __pyx_skip_dispatch) {
   Py_ssize_t __pyx_v_index;
   PyObject *__pyx_r = NULL;
@@ -1939,43 +1982,43 @@
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_choice", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":35
+  /* "nazo_rand/nazo_rand.pyx":41
  * @cython.wraparound(False)
  * cpdef object random_choice(object container):
- *     cdef Py_ssize_t index = randbelow(len(container))             # <<<<<<<<<<<<<<
+ *     cdef Py_ssize_t index = cy_random_below(len(container))             # <<<<<<<<<<<<<<
  *     return container[index]
  * 
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_container); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 35, __pyx_L1_error)
-  __pyx_v_index = __pyx_f_9nazo_rand_9nazo_rand_randbelow(__pyx_t_1, 0);
+  __pyx_t_1 = PyObject_Length(__pyx_v_container); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_v_index = __pyx_f_9nazo_rand_9nazo_rand_cy_random_below(__pyx_t_1);
 
-  /* "nazo_rand/nazo_rand.pyx":36
+  /* "nazo_rand/nazo_rand.pyx":42
  * cpdef object random_choice(object container):
- *     cdef Py_ssize_t index = randbelow(len(container))
+ *     cdef Py_ssize_t index = cy_random_below(len(container))
  *     return container[index]             # <<<<<<<<<<<<<<
  * 
  * @cython.boundscheck(False)
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_container, __pyx_v_index, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_container, __pyx_v_index, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":34
+  /* "nazo_rand/nazo_rand.pyx":40
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef object random_choice(object container):             # <<<<<<<<<<<<<<
- *     cdef Py_ssize_t index = randbelow(len(container))
+ *     cdef Py_ssize_t index = cy_random_below(len(container))
  *     return container[index]
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_AddTraceback("nazo_rand.nazo_rand.random_choice", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -2005,15 +2048,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_choice", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_random_choice(__pyx_v_container, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_random_choice(__pyx_v_container, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2022,81 +2065,81 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":40
+/* "nazo_rand/nazo_rand.pyx":46
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef list[object] random_choices(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t container_length = len(container)
- *     return [container[randbelow(container_length)] for _ in range(count)]
+ *     return [container[cy_random_below(container_length)] for _ in range(count)]
  */
 
 static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_11random_choices(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_9nazo_rand_9nazo_rand_random_choices(PyObject *__pyx_v_container, Py_ssize_t __pyx_v_count, CYTHON_UNUSED int __pyx_skip_dispatch) {
   Py_ssize_t __pyx_v_container_length;
   CYTHON_UNUSED Py_ssize_t __pyx_7genexpr__pyx_v__;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
-  int __pyx_t_5;
+  int64_t __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_choices", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":41
+  /* "nazo_rand/nazo_rand.pyx":47
  * @cython.wraparound(False)
  * cpdef list[object] random_choices(object container, Py_ssize_t count):
  *     cdef Py_ssize_t container_length = len(container)             # <<<<<<<<<<<<<<
- *     return [container[randbelow(container_length)] for _ in range(count)]
+ *     return [container[cy_random_below(container_length)] for _ in range(count)]
  * 
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_container); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_container); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 47, __pyx_L1_error)
   __pyx_v_container_length = __pyx_t_1;
 
-  /* "nazo_rand/nazo_rand.pyx":42
+  /* "nazo_rand/nazo_rand.pyx":48
  * cpdef list[object] random_choices(object container, Py_ssize_t count):
  *     cdef Py_ssize_t container_length = len(container)
- *     return [container[randbelow(container_length)] for _ in range(count)]             # <<<<<<<<<<<<<<
+ *     return [container[cy_random_below(container_length)] for _ in range(count)]             # <<<<<<<<<<<<<<
  * 
  * @cython.boundscheck(False)
  */
   __Pyx_XDECREF(__pyx_r);
   { /* enter inner scope */
-    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
+    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = __pyx_v_count;
     __pyx_t_3 = __pyx_t_1;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_7genexpr__pyx_v__ = __pyx_t_4;
-      __pyx_t_5 = __pyx_f_9nazo_rand_9nazo_rand_randbelow(__pyx_v_container_length, 0);
-      __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_container, __pyx_t_5, int, 1, __Pyx_PyInt_From_int, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 42, __pyx_L1_error)
+      __pyx_t_5 = __pyx_f_9nazo_rand_9nazo_rand_cy_random_below(__pyx_v_container_length);
+      __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_container, __pyx_t_5, int64_t, 1, __Pyx_PyInt_From_int64_t, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 48, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 42, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 48, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
   } /* exit inner scope */
   __pyx_r = ((PyObject *)__pyx_t_2);
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":40
+  /* "nazo_rand/nazo_rand.pyx":46
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef list[object] random_choices(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t container_length = len(container)
- *     return [container[randbelow(container_length)] for _ in range(count)]
+ *     return [container[cy_random_below(container_length)] for _ in range(count)]
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("nazo_rand.nazo_rand.random_choices", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -2138,32 +2181,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_container)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_count)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("random_choices", 1, 2, 2, 1); __PYX_ERR(0, 40, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("random_choices", 1, 2, 2, 1); __PYX_ERR(0, 46, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_choices") < 0)) __PYX_ERR(0, 40, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_choices") < 0)) __PYX_ERR(0, 46, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_container = values[0];
-    __pyx_v_count = __Pyx_PyIndex_AsSsize_t(values[1]); if (unlikely((__pyx_v_count == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 40, __pyx_L3_error)
+    __pyx_v_count = __Pyx_PyIndex_AsSsize_t(values[1]); if (unlikely((__pyx_v_count == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 46, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("random_choices", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 40, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("random_choices", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 46, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("nazo_rand.nazo_rand.random_choices", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_10random_choices(__pyx_self, __pyx_v_container, __pyx_v_count);
 
@@ -2177,15 +2220,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_choices", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_random_choices(__pyx_v_container, __pyx_v_count, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_random_choices(__pyx_v_container, __pyx_v_count, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2194,15 +2237,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":46
+/* "nazo_rand/nazo_rand.pyx":52
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef list[object] random_sample(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t container_length = len(container)
  *     cdef Py_ssize_t i, j
  */
 
@@ -2221,146 +2264,146 @@
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_sample", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":47
+  /* "nazo_rand/nazo_rand.pyx":53
  * @cython.wraparound(False)
  * cpdef list[object] random_sample(object container, Py_ssize_t count):
  *     cdef Py_ssize_t container_length = len(container)             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t i, j
  *     cdef list result = [None] * count
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_container); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_container); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 53, __pyx_L1_error)
   __pyx_v_container_length = __pyx_t_1;
 
-  /* "nazo_rand/nazo_rand.pyx":49
+  /* "nazo_rand/nazo_rand.pyx":55
  *     cdef Py_ssize_t container_length = len(container)
  *     cdef Py_ssize_t i, j
  *     cdef list result = [None] * count             # <<<<<<<<<<<<<<
  *     cdef list temp = list(container)
  * 
  */
-  __pyx_t_2 = PyList_New(1 * ((__pyx_v_count<0) ? 0:__pyx_v_count)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(1 * ((__pyx_v_count<0) ? 0:__pyx_v_count)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 55, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   { Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < __pyx_v_count; __pyx_temp++) {
       __Pyx_INCREF(Py_None);
       __Pyx_GIVEREF(Py_None);
       PyList_SET_ITEM(__pyx_t_2, __pyx_temp, Py_None);
     }
   }
   __pyx_v_result = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":50
+  /* "nazo_rand/nazo_rand.pyx":56
  *     cdef Py_ssize_t i, j
  *     cdef list result = [None] * count
  *     cdef list temp = list(container)             # <<<<<<<<<<<<<<
  * 
  *     if count > container_length:
  */
-  __pyx_t_2 = PySequence_List(__pyx_v_container); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __pyx_t_2 = PySequence_List(__pyx_v_container); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 56, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_v_temp = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":52
+  /* "nazo_rand/nazo_rand.pyx":58
  *     cdef list temp = list(container)
  * 
  *     if count > container_length:             # <<<<<<<<<<<<<<
  *         raise ValueError("Sample larger than population")
  * 
  */
   __pyx_t_3 = ((__pyx_v_count > __pyx_v_container_length) != 0);
   if (unlikely(__pyx_t_3)) {
 
-    /* "nazo_rand/nazo_rand.pyx":53
+    /* "nazo_rand/nazo_rand.pyx":59
  * 
  *     if count > container_length:
  *         raise ValueError("Sample larger than population")             # <<<<<<<<<<<<<<
  * 
  *     for i in range(count):
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 59, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 53, __pyx_L1_error)
+    __PYX_ERR(0, 59, __pyx_L1_error)
 
-    /* "nazo_rand/nazo_rand.pyx":52
+    /* "nazo_rand/nazo_rand.pyx":58
  *     cdef list temp = list(container)
  * 
  *     if count > container_length:             # <<<<<<<<<<<<<<
  *         raise ValueError("Sample larger than population")
  * 
  */
   }
 
-  /* "nazo_rand/nazo_rand.pyx":55
+  /* "nazo_rand/nazo_rand.pyx":61
  *         raise ValueError("Sample larger than population")
  * 
  *     for i in range(count):             # <<<<<<<<<<<<<<
  *         j = uniform_int_variate(i, container_length - 1)
  *         result[i] = temp[j]
  */
   __pyx_t_1 = __pyx_v_count;
   __pyx_t_4 = __pyx_t_1;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
     __pyx_v_i = __pyx_t_5;
 
-    /* "nazo_rand/nazo_rand.pyx":56
+    /* "nazo_rand/nazo_rand.pyx":62
  * 
  *     for i in range(count):
  *         j = uniform_int_variate(i, container_length - 1)             # <<<<<<<<<<<<<<
  *         result[i] = temp[j]
  *         temp[j] = temp[i]
  */
     __pyx_v_j = Storm::uniform_int_variate(__pyx_v_i, (__pyx_v_container_length - 1));
 
-    /* "nazo_rand/nazo_rand.pyx":57
+    /* "nazo_rand/nazo_rand.pyx":63
  *     for i in range(count):
  *         j = uniform_int_variate(i, container_length - 1)
  *         result[i] = temp[j]             # <<<<<<<<<<<<<<
  *         temp[j] = temp[i]
  * 
  */
     __pyx_t_2 = PyList_GET_ITEM(__pyx_v_temp, __pyx_v_j);
     __Pyx_INCREF(__pyx_t_2);
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_result, __pyx_v_i, __pyx_t_2, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 0, 0) < 0)) __PYX_ERR(0, 57, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_result, __pyx_v_i, __pyx_t_2, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 0, 0) < 0)) __PYX_ERR(0, 63, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "nazo_rand/nazo_rand.pyx":58
+    /* "nazo_rand/nazo_rand.pyx":64
  *         j = uniform_int_variate(i, container_length - 1)
  *         result[i] = temp[j]
  *         temp[j] = temp[i]             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
     __pyx_t_2 = PyList_GET_ITEM(__pyx_v_temp, __pyx_v_i);
     __Pyx_INCREF(__pyx_t_2);
-    if (unlikely(__Pyx_SetItemInt(__pyx_v_temp, __pyx_v_j, __pyx_t_2, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 0, 0) < 0)) __PYX_ERR(0, 58, __pyx_L1_error)
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_temp, __pyx_v_j, __pyx_t_2, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 0, 0) < 0)) __PYX_ERR(0, 64, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
 
-  /* "nazo_rand/nazo_rand.pyx":60
+  /* "nazo_rand/nazo_rand.pyx":66
  *         temp[j] = temp[i]
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":46
+  /* "nazo_rand/nazo_rand.pyx":52
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef list[object] random_sample(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t container_length = len(container)
  *     cdef Py_ssize_t i, j
  */
 
@@ -2408,32 +2451,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_container)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_count)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("random_sample", 1, 2, 2, 1); __PYX_ERR(0, 46, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("random_sample", 1, 2, 2, 1); __PYX_ERR(0, 52, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_sample") < 0)) __PYX_ERR(0, 46, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_sample") < 0)) __PYX_ERR(0, 52, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_container = values[0];
-    __pyx_v_count = __Pyx_PyIndex_AsSsize_t(values[1]); if (unlikely((__pyx_v_count == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 46, __pyx_L3_error)
+    __pyx_v_count = __Pyx_PyIndex_AsSsize_t(values[1]); if (unlikely((__pyx_v_count == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 52, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("random_sample", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 46, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("random_sample", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 52, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("nazo_rand.nazo_rand.random_sample", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_12random_sample(__pyx_self, __pyx_v_container, __pyx_v_count);
 
@@ -2447,15 +2490,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_sample", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_random_sample(__pyx_v_container, __pyx_v_count, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_random_sample(__pyx_v_container, __pyx_v_count, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2464,15 +2507,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":62
+/* "nazo_rand/nazo_rand.pyx":68
  *     return result
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):             # <<<<<<<<<<<<<<
  *     if stop == 0:
  *         stop, start = start, 0
  */
 
@@ -2491,56 +2534,56 @@
       __pyx_v_stop = __pyx_optional_args->stop;
       if (__pyx_optional_args->__pyx_n > 1) {
         __pyx_v_step = __pyx_optional_args->step;
       }
     }
   }
 
-  /* "nazo_rand/nazo_rand.pyx":63
+  /* "nazo_rand/nazo_rand.pyx":69
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):
  *     if stop == 0:             # <<<<<<<<<<<<<<
  *         stop, start = start, 0
  *     return random_range(start, stop, step)
  */
   __pyx_t_1 = ((__pyx_v_stop == 0) != 0);
   if (__pyx_t_1) {
 
-    /* "nazo_rand/nazo_rand.pyx":64
+    /* "nazo_rand/nazo_rand.pyx":70
  * cpdef int randrange(int start, int stop=0, int step=1):
  *     if stop == 0:
  *         stop, start = start, 0             # <<<<<<<<<<<<<<
  *     return random_range(start, stop, step)
  * 
  */
     __pyx_t_2 = __pyx_v_start;
     __pyx_t_3 = 0;
     __pyx_v_stop = __pyx_t_2;
     __pyx_v_start = __pyx_t_3;
 
-    /* "nazo_rand/nazo_rand.pyx":63
+    /* "nazo_rand/nazo_rand.pyx":69
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):
  *     if stop == 0:             # <<<<<<<<<<<<<<
  *         stop, start = start, 0
  *     return random_range(start, stop, step)
  */
   }
 
-  /* "nazo_rand/nazo_rand.pyx":65
+  /* "nazo_rand/nazo_rand.pyx":71
  *     if stop == 0:
  *         stop, start = start, 0
  *     return random_range(start, stop, step)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = Storm::random_range(__pyx_v_start, __pyx_v_stop, __pyx_v_step);
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":62
+  /* "nazo_rand/nazo_rand.pyx":68
  *     return result
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):             # <<<<<<<<<<<<<<
  *     if stop == 0:
  *         stop, start = start, 0
  */
 
@@ -2594,42 +2637,42 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_step);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "randrange") < 0)) __PYX_ERR(0, 62, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "randrange") < 0)) __PYX_ERR(0, 68, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_start = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 62, __pyx_L3_error)
+    __pyx_v_start = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 68, __pyx_L3_error)
     if (values[1]) {
-      __pyx_v_stop = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_stop == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 62, __pyx_L3_error)
+      __pyx_v_stop = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_stop == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 68, __pyx_L3_error)
     } else {
       __pyx_v_stop = ((int)0);
     }
     if (values[2]) {
-      __pyx_v_step = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_step == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 62, __pyx_L3_error)
+      __pyx_v_step = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_step == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 68, __pyx_L3_error)
     } else {
       __pyx_v_step = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("randrange", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 62, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("randrange", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 68, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("nazo_rand.nazo_rand.randrange", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_14randrange(__pyx_self, __pyx_v_start, __pyx_v_stop, __pyx_v_step);
 
@@ -2649,15 +2692,15 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("randrange", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 2;
   __pyx_t_2.stop = __pyx_v_stop;
   __pyx_t_2.step = __pyx_v_step;
   __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_randrange(__pyx_v_start, 0, &__pyx_t_2); 
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2666,39 +2709,39 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":68
+/* "nazo_rand/nazo_rand.pyx":74
  * 
  * 
  * cpdef double random_double(double a, double b):             # <<<<<<<<<<<<<<
  *     return uniform_real_variate(a, b)
  * 
  */
 
 static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_17random_double(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static double __pyx_f_9nazo_rand_9nazo_rand_random_double(double __pyx_v_a, double __pyx_v_b, CYTHON_UNUSED int __pyx_skip_dispatch) {
   double __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("random_double", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":69
+  /* "nazo_rand/nazo_rand.pyx":75
  * 
  * cpdef double random_double(double a, double b):
  *     return uniform_real_variate(a, b)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = Storm::uniform_real_variate(__pyx_v_a, __pyx_v_b);
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":68
+  /* "nazo_rand/nazo_rand.pyx":74
  * 
  * 
  * cpdef double random_double(double a, double b):             # <<<<<<<<<<<<<<
  *     return uniform_real_variate(a, b)
  * 
  */
 
@@ -2739,32 +2782,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("random_double", 1, 2, 2, 1); __PYX_ERR(0, 68, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("random_double", 1, 2, 2, 1); __PYX_ERR(0, 74, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_double") < 0)) __PYX_ERR(0, 68, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_double") < 0)) __PYX_ERR(0, 74, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_a = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_a == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 68, __pyx_L3_error)
-    __pyx_v_b = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_b == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 68, __pyx_L3_error)
+    __pyx_v_a = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_a == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 74, __pyx_L3_error)
+    __pyx_v_b = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_b == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 74, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("random_double", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 68, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("random_double", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 74, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("nazo_rand.nazo_rand.random_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_16random_double(__pyx_self, __pyx_v_a, __pyx_v_b);
 
@@ -2778,15 +2821,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_double", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_9nazo_rand_9nazo_rand_random_double(__pyx_v_a, __pyx_v_b, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_9nazo_rand_9nazo_rand_random_double(__pyx_v_a, __pyx_v_b, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2795,36 +2838,36 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":72
+/* "nazo_rand/nazo_rand.pyx":78
  * 
  * 
  * cpdef double random_double_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_real_variate_noargs()
  */
 
 static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_19random_double_noargs(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static double __pyx_f_9nazo_rand_9nazo_rand_random_double_noargs(CYTHON_UNUSED int __pyx_skip_dispatch) {
   double __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("random_double_noargs", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":73
+  /* "nazo_rand/nazo_rand.pyx":79
  * 
  * cpdef double random_double_noargs():
  *     return uniform_real_variate_noargs()             # <<<<<<<<<<<<<<
  */
   __pyx_r = Storm::uniform_real_variate_noargs();
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":72
+  /* "nazo_rand/nazo_rand.pyx":78
  * 
  * 
  * cpdef double random_double_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_real_variate_noargs()
  */
 
   /* function exit code */
@@ -2852,15 +2895,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_double_noargs", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_9nazo_rand_9nazo_rand_random_double_noargs(0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_9nazo_rand_9nazo_rand_random_double_noargs(0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2923,172 +2966,174 @@
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_a, __pyx_k_a, sizeof(__pyx_k_a), 0, 0, 1, 1},
   {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
   {&__pyx_n_s_b, __pyx_k_b, sizeof(__pyx_k_b), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_container, __pyx_k_container, sizeof(__pyx_k_container), 0, 0, 1, 1},
   {&__pyx_n_s_count, __pyx_k_count, sizeof(__pyx_k_count), 0, 0, 1, 1},
+  {&__pyx_n_u_int, __pyx_k_int, sizeof(__pyx_k_int), 0, 1, 0, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_nazo_rand_nazo_rand, __pyx_k_nazo_rand_nazo_rand, sizeof(__pyx_k_nazo_rand_nazo_rand), 0, 0, 1, 1},
   {&__pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_k_nazo_rand_nazo_rand_pyx, sizeof(__pyx_k_nazo_rand_nazo_rand_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_randbelow, __pyx_k_randbelow, sizeof(__pyx_k_randbelow), 0, 0, 1, 1},
   {&__pyx_n_s_randint, __pyx_k_randint, sizeof(__pyx_k_randint), 0, 0, 1, 1},
   {&__pyx_n_s_random_choice, __pyx_k_random_choice, sizeof(__pyx_k_random_choice), 0, 0, 1, 1},
   {&__pyx_n_s_random_choices, __pyx_k_random_choices, sizeof(__pyx_k_random_choices), 0, 0, 1, 1},
   {&__pyx_n_s_random_double, __pyx_k_random_double, sizeof(__pyx_k_random_double), 0, 0, 1, 1},
   {&__pyx_n_s_random_double_noargs, __pyx_k_random_double_noargs, sizeof(__pyx_k_random_double_noargs), 0, 0, 1, 1},
   {&__pyx_n_s_random_integer_noargs, __pyx_k_random_integer_noargs, sizeof(__pyx_k_random_integer_noargs), 0, 0, 1, 1},
   {&__pyx_n_s_random_sample, __pyx_k_random_sample, sizeof(__pyx_k_random_sample), 0, 0, 1, 1},
   {&__pyx_n_s_randrange, __pyx_k_randrange, sizeof(__pyx_k_randrange), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
+  {&__pyx_n_s_return, __pyx_k_return, sizeof(__pyx_k_return), 0, 0, 1, 1},
   {&__pyx_n_s_reversed, __pyx_k_reversed, sizeof(__pyx_k_reversed), 0, 0, 1, 1},
   {&__pyx_n_s_shuffle, __pyx_k_shuffle, sizeof(__pyx_k_shuffle), 0, 0, 1, 1},
   {&__pyx_n_s_start, __pyx_k_start, sizeof(__pyx_k_start), 0, 0, 1, 1},
   {&__pyx_n_s_step, __pyx_k_step, sizeof(__pyx_k_step), 0, 0, 1, 1},
   {&__pyx_n_s_stop, __pyx_k_stop, sizeof(__pyx_k_stop), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_reversed = __Pyx_GetBuiltinName(__pyx_n_s_reversed); if (!__pyx_builtin_reversed) __PYX_ERR(0, 19, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 19, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_builtin_reversed = __Pyx_GetBuiltinName(__pyx_n_s_reversed); if (!__pyx_builtin_reversed) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 59, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":53
+  /* "nazo_rand/nazo_rand.pyx":59
  * 
  *     if count > container_length:
  *         raise ValueError("Sample larger than population")             # <<<<<<<<<<<<<<
  * 
  *     for i in range(count):
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_Sample_larger_than_population); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_Sample_larger_than_population); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "nazo_rand/nazo_rand.pyx":15
- *     double uniform_real_variate(double a, double b)
+  /* "nazo_rand/nazo_rand.pyx":21
+ *     return uniform_int_variate(a, b)
  * 
  * cpdef int random_integer_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_int_variate_noargs()
  * 
  */
-  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_integer_noargs, 15, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_integer_noargs, 21, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 21, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":18
+  /* "nazo_rand/nazo_rand.pyx":24
  *     return uniform_int_variate_noargs()
  * 
  * cpdef void shuffle(list array):             # <<<<<<<<<<<<<<
  *     for i in reversed(range(len(array) - 1)):
  *         j = randrange(i, len(array), 1)
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_n_s_array); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_n_s_array); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
-  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_shuffle, 18, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_shuffle, 24, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 24, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":24
+  /* "nazo_rand/nazo_rand.pyx":30
  * 
  * 
- * cpdef int randbelow(int a):             # <<<<<<<<<<<<<<
+ * def randbelow(a:int) -> int:             # <<<<<<<<<<<<<<
  *     return random_below(a)
  * 
  */
-  __pyx_tuple__5 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_a); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_n_s_a); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
-  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randbelow, 24, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randbelow, 30, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 30, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":27
+  /* "nazo_rand/nazo_rand.pyx":33
  *     return random_below(a)
  * 
- * cpdef int randint(int a, int b):             # <<<<<<<<<<<<<<
- *     return uniform_int_variate(a, b)
+ * def randint(a:int, b:int) -> int:             # <<<<<<<<<<<<<<
+ *     return cy_uniform_int_variate(a, b)
  * 
  */
-  __pyx_tuple__7 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randint, 27, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randint, 33, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 33, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":34
+  /* "nazo_rand/nazo_rand.pyx":40
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef object random_choice(object container):             # <<<<<<<<<<<<<<
- *     cdef Py_ssize_t index = randbelow(len(container))
+ *     cdef Py_ssize_t index = cy_random_below(len(container))
  *     return container[index]
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_n_s_container); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_n_s_container); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_choice, 34, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_choice, 40, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 40, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":40
+  /* "nazo_rand/nazo_rand.pyx":46
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef list[object] random_choices(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t container_length = len(container)
- *     return [container[randbelow(container_length)] for _ in range(count)]
+ *     return [container[cy_random_below(container_length)] for _ in range(count)]
  */
-  __pyx_tuple__11 = PyTuple_Pack(2, __pyx_n_s_container, __pyx_n_s_count); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(2, __pyx_n_s_container, __pyx_n_s_count); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_choices, 40, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_choices, 46, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 46, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":46
+  /* "nazo_rand/nazo_rand.pyx":52
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef list[object] random_sample(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t container_length = len(container)
  *     cdef Py_ssize_t i, j
  */
-  __pyx_tuple__13 = PyTuple_Pack(2, __pyx_n_s_container, __pyx_n_s_count); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(2, __pyx_n_s_container, __pyx_n_s_count); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
-  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_sample, 46, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_sample, 52, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 52, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":62
+  /* "nazo_rand/nazo_rand.pyx":68
  *     return result
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):             # <<<<<<<<<<<<<<
  *     if stop == 0:
  *         stop, start = start, 0
  */
-  __pyx_tuple__15 = PyTuple_Pack(3, __pyx_n_s_start, __pyx_n_s_stop, __pyx_n_s_step); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(3, __pyx_n_s_start, __pyx_n_s_stop, __pyx_n_s_step); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
-  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randrange, 62, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randrange, 68, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 68, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":68
+  /* "nazo_rand/nazo_rand.pyx":74
  * 
  * 
  * cpdef double random_double(double a, double b):             # <<<<<<<<<<<<<<
  *     return uniform_real_variate(a, b)
  * 
  */
-  __pyx_tuple__17 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
-  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_double, 68, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_double, 74, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 74, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":72
+  /* "nazo_rand/nazo_rand.pyx":78
  * 
  * 
  * cpdef double random_double_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_real_variate_noargs()
  */
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_double_noargs, 72, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_double_noargs, 78, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -3131,16 +3176,16 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_export_code", 0);
   /*--- Function export code ---*/
   if (__Pyx_ExportFunction("shuffle", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_shuffle, "void (PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("random_integer_noargs", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_random_integer_noargs, "int (int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("random_choice", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_random_choice, "PyObject *(PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("random_choices", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_random_choices, "PyObject *(PyObject *, Py_ssize_t, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("random_sample", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_random_sample, "PyObject *(PyObject *, Py_ssize_t, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ExportFunction("randbelow", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_randbelow, "int (int, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (__Pyx_ExportFunction("randint", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_randint, "int (int, int, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("cy_random_below", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_cy_random_below, "int64_t (int64_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("cy_uniform_int_variate", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_cy_uniform_int_variate, "int64_t (int64_t, int64_t)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("randrange", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_randrange, "int (int, int __pyx_skip_dispatch, struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange *__pyx_optional_args)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("random_double", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_random_double, "double (double, double, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("random_double_noargs", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_random_double_noargs, "double (int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
@@ -3270,14 +3315,15 @@
 
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec_nazo_rand(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
@@ -3375,131 +3421,144 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "nazo_rand/nazo_rand.pyx":15
- *     double uniform_real_variate(double a, double b)
+  /* "nazo_rand/nazo_rand.pyx":21
+ *     return uniform_int_variate(a, b)
  * 
  * cpdef int random_integer_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_int_variate_noargs()
  * 
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_1random_integer_noargs, 0, __pyx_n_s_random_integer_noargs, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_1random_integer_noargs, 0, __pyx_n_s_random_integer_noargs, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_integer_noargs, __pyx_t_1) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_integer_noargs, __pyx_t_1) < 0) __PYX_ERR(0, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":18
+  /* "nazo_rand/nazo_rand.pyx":24
  *     return uniform_int_variate_noargs()
  * 
  * cpdef void shuffle(list array):             # <<<<<<<<<<<<<<
  *     for i in reversed(range(len(array) - 1)):
  *         j = randrange(i, len(array), 1)
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_3shuffle, 0, __pyx_n_s_shuffle, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_3shuffle, 0, __pyx_n_s_shuffle, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_shuffle, __pyx_t_1) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_shuffle, __pyx_t_1) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":24
+  /* "nazo_rand/nazo_rand.pyx":30
  * 
  * 
- * cpdef int randbelow(int a):             # <<<<<<<<<<<<<<
+ * def randbelow(a:int) -> int:             # <<<<<<<<<<<<<<
  *     return random_below(a)
  * 
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_5randbelow, 0, __pyx_n_s_randbelow, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randbelow, __pyx_t_1) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_a, __pyx_n_u_int) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_return, __pyx_n_u_int) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_5randbelow, 0, __pyx_n_s_randbelow, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randbelow, __pyx_t_2) < 0) __PYX_ERR(0, 30, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":27
+  /* "nazo_rand/nazo_rand.pyx":33
  *     return random_below(a)
  * 
- * cpdef int randint(int a, int b):             # <<<<<<<<<<<<<<
- *     return uniform_int_variate(a, b)
+ * def randint(a:int, b:int) -> int:             # <<<<<<<<<<<<<<
+ *     return cy_uniform_int_variate(a, b)
  * 
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_7randint, 0, __pyx_n_s_randint, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_a, __pyx_n_u_int) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_b, __pyx_n_u_int) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_u_int) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_7randint, 0, __pyx_n_s_randint, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randint, __pyx_t_1) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
+  __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_1, __pyx_t_2);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randint, __pyx_t_1) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":34
+  /* "nazo_rand/nazo_rand.pyx":40
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef object random_choice(object container):             # <<<<<<<<<<<<<<
- *     cdef Py_ssize_t index = randbelow(len(container))
+ *     cdef Py_ssize_t index = cy_random_below(len(container))
  *     return container[index]
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_9random_choice, 0, __pyx_n_s_random_choice, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_9random_choice, 0, __pyx_n_s_random_choice, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_choice, __pyx_t_1) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_choice, __pyx_t_1) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":40
+  /* "nazo_rand/nazo_rand.pyx":46
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef list[object] random_choices(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t container_length = len(container)
- *     return [container[randbelow(container_length)] for _ in range(count)]
+ *     return [container[cy_random_below(container_length)] for _ in range(count)]
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_11random_choices, 0, __pyx_n_s_random_choices, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_11random_choices, 0, __pyx_n_s_random_choices, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_choices, __pyx_t_1) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_choices, __pyx_t_1) < 0) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":46
+  /* "nazo_rand/nazo_rand.pyx":52
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
  * cpdef list[object] random_sample(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t container_length = len(container)
  *     cdef Py_ssize_t i, j
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_13random_sample, 0, __pyx_n_s_random_sample, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_13random_sample, 0, __pyx_n_s_random_sample, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_sample, __pyx_t_1) < 0) __PYX_ERR(0, 46, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_sample, __pyx_t_1) < 0) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":62
+  /* "nazo_rand/nazo_rand.pyx":68
  *     return result
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):             # <<<<<<<<<<<<<<
  *     if stop == 0:
  *         stop, start = start, 0
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_15randrange, 0, __pyx_n_s_randrange, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_15randrange, 0, __pyx_n_s_randrange, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randrange, __pyx_t_1) < 0) __PYX_ERR(0, 62, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randrange, __pyx_t_1) < 0) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":68
+  /* "nazo_rand/nazo_rand.pyx":74
  * 
  * 
  * cpdef double random_double(double a, double b):             # <<<<<<<<<<<<<<
  *     return uniform_real_variate(a, b)
  * 
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_17random_double, 0, __pyx_n_s_random_double, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_17random_double, 0, __pyx_n_s_random_double, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_double, __pyx_t_1) < 0) __PYX_ERR(0, 68, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_double, __pyx_t_1) < 0) __PYX_ERR(0, 74, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":72
+  /* "nazo_rand/nazo_rand.pyx":78
  * 
  * 
  * cpdef double random_double_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_real_variate_noargs()
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_19random_double_noargs, 0, __pyx_n_s_random_double_noargs, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_19random_double_noargs, 0, __pyx_n_s_random_double_noargs, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_double_noargs, __pyx_t_1) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_double_noargs, __pyx_t_1) < 0) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "nazo_rand/nazo_rand.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
  * # distutils: language = c++
  * cimport cython
  */
@@ -3509,14 +3568,15 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
   if (__pyx_m) {
     if (__pyx_d) {
       __Pyx_AddTraceback("init nazo_rand.nazo_rand", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_ImportError, "init nazo_rand.nazo_rand");
@@ -5295,14 +5355,248 @@
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
     }
 }
 
+/* CIntFromPy */
+static CYTHON_INLINE int64_t __Pyx_PyInt_As_int64_t(PyObject *x) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int64_t neg_one = (int64_t) -1, const_zero = (int64_t) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+#if PY_MAJOR_VERSION < 3
+    if (likely(PyInt_Check(x))) {
+        if (sizeof(int64_t) < sizeof(long)) {
+            __PYX_VERIFY_RETURN_INT(int64_t, long, PyInt_AS_LONG(x))
+        } else {
+            long val = PyInt_AS_LONG(x);
+            if (is_unsigned && unlikely(val < 0)) {
+                goto raise_neg_overflow;
+            }
+            return (int64_t) val;
+        }
+    } else
+#endif
+    if (likely(PyLong_Check(x))) {
+        if (is_unsigned) {
+#if CYTHON_USE_PYLONG_INTERNALS
+            const digit* digits = ((PyLongObject*)x)->ob_digit;
+            switch (Py_SIZE(x)) {
+                case  0: return (int64_t) 0;
+                case  1: __PYX_VERIFY_RETURN_INT(int64_t, digit, digits[0])
+                case 2:
+                    if (8 * sizeof(int64_t) > 1 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int64_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int64_t) >= 2 * PyLong_SHIFT) {
+                            return (int64_t) (((((int64_t)digits[1]) << PyLong_SHIFT) | (int64_t)digits[0]));
+                        }
+                    }
+                    break;
+                case 3:
+                    if (8 * sizeof(int64_t) > 2 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int64_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int64_t) >= 3 * PyLong_SHIFT) {
+                            return (int64_t) (((((((int64_t)digits[2]) << PyLong_SHIFT) | (int64_t)digits[1]) << PyLong_SHIFT) | (int64_t)digits[0]));
+                        }
+                    }
+                    break;
+                case 4:
+                    if (8 * sizeof(int64_t) > 3 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int64_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int64_t) >= 4 * PyLong_SHIFT) {
+                            return (int64_t) (((((((((int64_t)digits[3]) << PyLong_SHIFT) | (int64_t)digits[2]) << PyLong_SHIFT) | (int64_t)digits[1]) << PyLong_SHIFT) | (int64_t)digits[0]));
+                        }
+                    }
+                    break;
+            }
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON
+            if (unlikely(Py_SIZE(x) < 0)) {
+                goto raise_neg_overflow;
+            }
+#else
+            {
+                int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                if (unlikely(result < 0))
+                    return (int64_t) -1;
+                if (unlikely(result == 1))
+                    goto raise_neg_overflow;
+            }
+#endif
+            if (sizeof(int64_t) <= sizeof(unsigned long)) {
+                __PYX_VERIFY_RETURN_INT_EXC(int64_t, unsigned long, PyLong_AsUnsignedLong(x))
+#ifdef HAVE_LONG_LONG
+            } else if (sizeof(int64_t) <= sizeof(unsigned PY_LONG_LONG)) {
+                __PYX_VERIFY_RETURN_INT_EXC(int64_t, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
+#endif
+            }
+        } else {
+#if CYTHON_USE_PYLONG_INTERNALS
+            const digit* digits = ((PyLongObject*)x)->ob_digit;
+            switch (Py_SIZE(x)) {
+                case  0: return (int64_t) 0;
+                case -1: __PYX_VERIFY_RETURN_INT(int64_t, sdigit, (sdigit) (-(sdigit)digits[0]))
+                case  1: __PYX_VERIFY_RETURN_INT(int64_t,  digit, +digits[0])
+                case -2:
+                    if (8 * sizeof(int64_t) - 1 > 1 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int64_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int64_t) - 1 > 2 * PyLong_SHIFT) {
+                            return (int64_t) (((int64_t)-1)*(((((int64_t)digits[1]) << PyLong_SHIFT) | (int64_t)digits[0])));
+                        }
+                    }
+                    break;
+                case 2:
+                    if (8 * sizeof(int64_t) > 1 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int64_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int64_t) - 1 > 2 * PyLong_SHIFT) {
+                            return (int64_t) ((((((int64_t)digits[1]) << PyLong_SHIFT) | (int64_t)digits[0])));
+                        }
+                    }
+                    break;
+                case -3:
+                    if (8 * sizeof(int64_t) - 1 > 2 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int64_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int64_t) - 1 > 3 * PyLong_SHIFT) {
+                            return (int64_t) (((int64_t)-1)*(((((((int64_t)digits[2]) << PyLong_SHIFT) | (int64_t)digits[1]) << PyLong_SHIFT) | (int64_t)digits[0])));
+                        }
+                    }
+                    break;
+                case 3:
+                    if (8 * sizeof(int64_t) > 2 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int64_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int64_t) - 1 > 3 * PyLong_SHIFT) {
+                            return (int64_t) ((((((((int64_t)digits[2]) << PyLong_SHIFT) | (int64_t)digits[1]) << PyLong_SHIFT) | (int64_t)digits[0])));
+                        }
+                    }
+                    break;
+                case -4:
+                    if (8 * sizeof(int64_t) - 1 > 3 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int64_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int64_t) - 1 > 4 * PyLong_SHIFT) {
+                            return (int64_t) (((int64_t)-1)*(((((((((int64_t)digits[3]) << PyLong_SHIFT) | (int64_t)digits[2]) << PyLong_SHIFT) | (int64_t)digits[1]) << PyLong_SHIFT) | (int64_t)digits[0])));
+                        }
+                    }
+                    break;
+                case 4:
+                    if (8 * sizeof(int64_t) > 3 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int64_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int64_t) - 1 > 4 * PyLong_SHIFT) {
+                            return (int64_t) ((((((((((int64_t)digits[3]) << PyLong_SHIFT) | (int64_t)digits[2]) << PyLong_SHIFT) | (int64_t)digits[1]) << PyLong_SHIFT) | (int64_t)digits[0])));
+                        }
+                    }
+                    break;
+            }
+#endif
+            if (sizeof(int64_t) <= sizeof(long)) {
+                __PYX_VERIFY_RETURN_INT_EXC(int64_t, long, PyLong_AsLong(x))
+#ifdef HAVE_LONG_LONG
+            } else if (sizeof(int64_t) <= sizeof(PY_LONG_LONG)) {
+                __PYX_VERIFY_RETURN_INT_EXC(int64_t, PY_LONG_LONG, PyLong_AsLongLong(x))
+#endif
+            }
+        }
+        {
+#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
+            PyErr_SetString(PyExc_RuntimeError,
+                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
+#else
+            int64_t val;
+            PyObject *v = __Pyx_PyNumber_IntOrLong(x);
+ #if PY_MAJOR_VERSION < 3
+            if (likely(v) && !PyLong_Check(v)) {
+                PyObject *tmp = v;
+                v = PyNumber_Long(tmp);
+                Py_DECREF(tmp);
+            }
+ #endif
+            if (likely(v)) {
+                int one = 1; int is_little = (int)*(unsigned char *)&one;
+                unsigned char *bytes = (unsigned char *)&val;
+                int ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                              bytes, sizeof(val),
+                                              is_little, !is_unsigned);
+                Py_DECREF(v);
+                if (likely(!ret))
+                    return val;
+            }
+#endif
+            return (int64_t) -1;
+        }
+    } else {
+        int64_t val;
+        PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
+        if (!tmp) return (int64_t) -1;
+        val = __Pyx_PyInt_As_int64_t(tmp);
+        Py_DECREF(tmp);
+        return val;
+    }
+raise_overflow:
+    PyErr_SetString(PyExc_OverflowError,
+        "value too large to convert to int64_t");
+    return (int64_t) -1;
+raise_neg_overflow:
+    PyErr_SetString(PyExc_OverflowError,
+        "can't convert negative value to int64_t");
+    return (int64_t) -1;
+}
+
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int64_t(int64_t value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int64_t neg_one = (int64_t) -1, const_zero = (int64_t) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(int64_t) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(int64_t) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int64_t) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(int64_t) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int64_t) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(int64_t),
+                                     little, !is_unsigned);
+    }
+}
+
 /* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
```

### Comparing `nazo_rand-0.0.6/nazo_rand/nazo_rand.hpp` & `nazo_rand-0.0.7/nazo_rand/nazo_rand.hpp`

 * *Files identical despite different names*

### Comparing `nazo_rand-0.0.6/nazo_rand/nazo_rand.pxd` & `nazo_rand-0.0.7/nazo_rand/nazo_rand.pxd`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # cython: language_level=3
 # distutils: language = c++
-
+from libc.stdint cimport int64_t
 #cpdef void seed(int rseed = ?)
 cpdef void shuffle(list array)
 cpdef int random_integer_noargs()
 cpdef object random_choice(object container)
 cpdef list[object] random_choices(object container, Py_ssize_t count)
 cpdef list[object] random_sample(object container, Py_ssize_t count)
-cpdef int randbelow(int a)
-cpdef int randint(int a,int b)
+# def int randbelow(int a)
+# def int randint(int a,int b)
+cdef int64_t cy_random_below(int64_t number) nogil
+cdef int64_t cy_uniform_int_variate(int64_t a, int64_t b) nogil
 cpdef int randrange(int start,int stop=?,int step=?)
 cpdef double random_double(double a, double b)
 cpdef double random_double_noargs()
```

### Comparing `nazo_rand-0.0.6/nazo_rand/nazo_rand.pyi` & `nazo_rand-0.0.7/nazo_rand/nazo_rand.pyi`

 * *Files identical despite different names*

### Comparing `nazo_rand-0.0.6/nazo_rand.egg-info/PKG-INFO` & `nazo_rand-0.0.7/nazo_rand.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nazo-rand
-Version: 0.0.6
+Version: 0.0.7
 Summary: A fast random number generator for python
 Author: bymoye
 Author-email: s3moye@gmail.com
 License: Free for non-commercial use
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `nazo_rand-0.0.6/setup.py` & `nazo_rand-0.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,50 @@
 from setuptools import setup, Extension
 from Cython.Build import cythonize
+from sys import platform
 
 
 def readme():
     with open("README.md") as f:
         return f.read()
 
 
+extra_compile_args = []
+extra_link_args = []
+
+if platform == "win32":
+    extra_compile_args = ["/std:c++17", "/O2"]
+elif platform == "linux":
+    extra_compile_args = ["-std=c++17", "-O3"]
+    extra_link_args = ["-Wl,-O3"]
+elif platform == "darwin":  # macOS
+    extra_compile_args = ["-std=c++17", "-O3"]
+    extra_link_args = ["-Wl,-dead_strip"]
+
 setup(
     name="nazo_rand",
     ext_modules=cythonize(
         Extension(
             name="",
             sources=["nazo_rand/nazo_rand.pyx"],
             language=["c++"],
-            extra_compile_args=["-std=c++17", "-O3"],
-            extra_link_args=["-O3"],
+            extra_compile_args=extra_compile_args,
+            extra_link_args=extra_link_args,
         ),
         compiler_directives={
             "language_level": 3,
             "boundscheck": False,
             "wraparound": False,
             "binding": True,
             "cdivision": True,
         },
     ),
     author="bymoye",
     author_email="s3moye@gmail.com",
-    version="0.0.6",
+    version="0.0.7",
     description="A fast random number generator for python",
     long_description=readme(),
     long_description_content_type="text/markdown",
     license="Free for non-commercial use",
     package_data={
         "": [
             "nazo_rand/nazo_rand.pyi",
```

