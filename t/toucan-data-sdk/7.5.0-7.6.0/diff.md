# Comparing `tmp/toucan_data_sdk-7.5.0.tar.gz` & `tmp/toucan_data_sdk-7.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toucan_data_sdk-7.5.0.tar", max compression
+gzip compressed data, was "toucan_data_sdk-7.6.0.tar", max compression
```

## Comparing `toucan_data_sdk-7.5.0.tar` & `toucan_data_sdk-7.6.0.tar`

### file list

```diff
@@ -1,49 +1,48 @@
--rw-r--r--   0        0        0     1510 2022-02-14 18:03:33.563123 toucan_data_sdk-7.5.0/LICENSE
--rw-r--r--   0        0        0     2093 2022-02-14 18:03:33.563123 toucan_data_sdk-7.5.0/README.md
--rw-r--r--   0        0        0     2093 2022-02-14 18:03:33.563123 toucan_data_sdk-7.5.0/pyproject.toml
--rw-r--r--   0        0        0       45 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/__init__.py
--rw-r--r--   0        0        0      145 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/fakir/__init__.py
--rw-r--r--   0        0        0     1407 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/fakir/fake_data_generator.py
--rw-r--r--   0        0        0      547 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/fakir/predict_number_of_row_from_conf.py
--rw-r--r--   0        0        0        0 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/py.typed
--rw-r--r--   0        0        0     7465 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/sdk.py
--rw-r--r--   0        0        0        0 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/__init__.py
--rw-r--r--   0        0        0    13576 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/decorators.py
--rw-r--r--   0        0        0      613 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/generic/__init__.py
--rw-r--r--   0        0        0     4065 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/generic/add_missing_row.py
--rw-r--r--   0        0        0     1337 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/generic/clean.py
--rw-r--r--   0        0        0     1494 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/generic/combine_columns_aggregation.py
--rw-r--r--   0        0        0     2203 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/generic/compute_cumsum.py
--rw-r--r--   0        0        0    10880 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/generic/compute_evolution.py
--rw-r--r--   0        0        0     1664 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/generic/compute_ffill_by_group.py
--rw-r--r--   0        0        0     4576 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/generic/date_requester.py
--rw-r--r--   0        0        0     3253 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/generic/roll_up.py
--rw-r--r--   0        0        0     2934 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/generic/two_values_melt.py
--rw-r--r--   0        0        0     6237 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/helpers.py
--rw-r--r--   0        0        0      981 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/__init__.py
--rw-r--r--   0        0        0     2729 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/add_aggregation_columns.py
--rw-r--r--   0        0        0     2598 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/argmax.py
--rw-r--r--   0        0        0     4303 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/categories_from_dates.py
--rw-r--r--   0        0        0     3958 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/converter.py
--rw-r--r--   0        0        0      809 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/cumsum.py
--rw-r--r--   0        0        0     1771 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/fillna.py
--rw-r--r--   0        0        0     1721 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/filter.py
--rw-r--r--   0        0        0     8652 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/filter_by_date.py
--rw-r--r--   0        0        0     2070 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/groupby.py
--rw-r--r--   0        0        0     5376 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/if_else.py
--rw-r--r--   0        0        0     2670 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/json_to_table.py
--rw-r--r--   0        0        0     3433 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/linear_regression.py
--rw-r--r--   0        0        0     9191 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/math.py
--rw-r--r--   0        0        0     1789 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/melt.py
--rw-r--r--   0        0        0     2019 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/percentage.py
--rw-r--r--   0        0        0     3943 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/pivot.py
--rw-r--r--   0        0        0     2820 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/rank.py
--rw-r--r--   0        0        0     2601 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/rename.py
--rw-r--r--   0        0        0     1583 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/replace.py
--rw-r--r--   0        0        0     1783 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/sort.py
--rw-r--r--   0        0        0    22481 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/text.py
--rw-r--r--   0        0        0     5202 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/top.py
--rw-r--r--   0        0        0    10074 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/waterfall.py
--rw-r--r--   0        0        0     2276 2022-02-14 18:03:33.567122 toucan_data_sdk-7.5.0/toucan_data_sdk/utils/traceback.py
--rw-r--r--   0        0        0     3074 2022-02-14 18:03:47.121108 toucan_data_sdk-7.5.0/setup.py
--rw-r--r--   0        0        0     3141 2022-02-14 18:03:47.121603 toucan_data_sdk-7.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1510 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/LICENSE
+-rw-r--r--   0        0        0     2093 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/README.md
+-rw-r--r--   0        0        0     2110 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/__init__.py
+-rw-r--r--   0        0        0      145 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/fakir/__init__.py
+-rw-r--r--   0        0        0     1407 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/fakir/fake_data_generator.py
+-rw-r--r--   0        0        0      547 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/fakir/predict_number_of_row_from_conf.py
+-rw-r--r--   0        0        0        0 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/py.typed
+-rw-r--r--   0        0        0     7465 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/sdk.py
+-rw-r--r--   0        0        0        0 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/__init__.py
+-rw-r--r--   0        0        0    13504 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/decorators.py
+-rw-r--r--   0        0        0      613 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/generic/__init__.py
+-rw-r--r--   0        0        0     4007 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/generic/add_missing_row.py
+-rw-r--r--   0        0        0     1337 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/generic/clean.py
+-rw-r--r--   0        0        0     1494 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/generic/combine_columns_aggregation.py
+-rw-r--r--   0        0        0     2203 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/generic/compute_cumsum.py
+-rw-r--r--   0        0        0    10880 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/generic/compute_evolution.py
+-rw-r--r--   0        0        0     1664 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/generic/compute_ffill_by_group.py
+-rw-r--r--   0        0        0     4576 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/generic/date_requester.py
+-rw-r--r--   0        0        0     3251 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/generic/roll_up.py
+-rw-r--r--   0        0        0     2934 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/generic/two_values_melt.py
+-rw-r--r--   0        0        0     6237 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/helpers.py
+-rw-r--r--   0        0        0      981 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/__init__.py
+-rw-r--r--   0        0        0     2729 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/add_aggregation_columns.py
+-rw-r--r--   0        0        0     2598 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/argmax.py
+-rw-r--r--   0        0        0     4303 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/categories_from_dates.py
+-rw-r--r--   0        0        0     3958 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/converter.py
+-rw-r--r--   0        0        0      809 2023-04-20 16:08:43.751954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/cumsum.py
+-rw-r--r--   0        0        0     1771 2023-04-20 16:08:43.755954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/fillna.py
+-rw-r--r--   0        0        0     1721 2023-04-20 16:08:43.755954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/filter.py
+-rw-r--r--   0        0        0     8652 2023-04-20 16:08:43.755954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/filter_by_date.py
+-rw-r--r--   0        0        0     2070 2023-04-20 16:08:43.755954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/groupby.py
+-rw-r--r--   0        0        0     4306 2023-04-20 16:08:43.755954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/if_else.py
+-rw-r--r--   0        0        0     2669 2023-04-20 16:08:43.755954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/json_to_table.py
+-rw-r--r--   0        0        0     3433 2023-04-20 16:08:43.755954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/linear_regression.py
+-rw-r--r--   0        0        0     9191 2023-04-20 16:08:43.755954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/math.py
+-rw-r--r--   0        0        0     1789 2023-04-20 16:08:43.755954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/melt.py
+-rw-r--r--   0        0        0     2019 2023-04-20 16:08:43.755954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/percentage.py
+-rw-r--r--   0        0        0     3943 2023-04-20 16:08:43.755954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/pivot.py
+-rw-r--r--   0        0        0     2820 2023-04-20 16:08:43.755954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/rank.py
+-rw-r--r--   0        0        0     2601 2023-04-20 16:08:43.755954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/rename.py
+-rw-r--r--   0        0        0     1583 2023-04-20 16:08:43.755954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/replace.py
+-rw-r--r--   0        0        0     1783 2023-04-20 16:08:43.755954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/sort.py
+-rw-r--r--   0        0        0    22481 2023-04-20 16:08:43.755954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/text.py
+-rw-r--r--   0        0        0     5202 2023-04-20 16:08:43.755954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/top.py
+-rw-r--r--   0        0        0    10074 2023-04-20 16:08:43.755954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/waterfall.py
+-rw-r--r--   0        0        0     2276 2023-04-20 16:08:43.755954 toucan_data_sdk-7.6.0/toucan_data_sdk/utils/traceback.py
+-rw-r--r--   0        0        0     3348 1970-01-01 00:00:00.000000 toucan_data_sdk-7.6.0/PKG-INFO
```

### Comparing `toucan_data_sdk-7.5.0/LICENSE` & `toucan_data_sdk-7.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/README.md` & `toucan_data_sdk-7.6.0/README.md`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/pyproject.toml` & `toucan_data_sdk-7.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "toucan_data_sdk"
-version = "7.5.0"
+version = "7.6.0"
 description = "Toucan data SDK"
 authors = ["Toucan Toco <dev@toucantoco.com>"]
 readme = "README.md"
 homepage = "https://github.com/ToucanToco/toucan-data-sdk"
 documentation = "https://toucantoco.github.io/toucan-data-sdk"
 repository = "https://github.com/ToucanToco/toucan-data-sdk"
 license = "BSD-3-Clause"
@@ -17,25 +17,25 @@
     "Programming Language :: Python :: 3.10",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 engarde = "^0.4.0"
-joblib = "<1"
+joblib = "^1"
 pandas = "^1.4.1"
-python-slugify = "^5.0.2"
-tabulate = "^0.8.9"
+python-slugify = ">=5.0.2,<7.0.0"
+tabulate = ">=0.8.9,<0.10.0"
 toucan-client = "^1.1.0"
 
 [tool.poetry.dev-dependencies]
-black = "^22.1.0"
+black = "^23.3.0"
 flake8 = "^4.0.1"
 isort = "^5.10.1"
-mypy = "^0.931"
+mypy = "^1.2.0"
 pre-commit = "^2.17.0"
 pytest = "^7.0.0"
 pytest-cov = "^3.0.0"
 pytest-mock = "^3.7.0"
 typing-extensions = "^4.1.1"
 # types
 types-python-slugify = "^5.0.3"
```

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/fakir/fake_data_generator.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/fakir/fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/fakir/predict_number_of_row_from_conf.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/fakir/predict_number_of_row_from_conf.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/sdk.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/decorators.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,15 +326,14 @@
 
             if check_param is True:
                 kwargs.update(tmp_extra_kwargs)
 
                 if applied_on_method:
                     self_arg, args = args[0], args[1:]
 
-                @wraps(func)
                 def f(*args, **kwargs):
                     # delete the extra parameters that the underlying function doesnt expect:
                     for k in tmp_extra_kwargs.keys():
                         del kwargs[k]
 
                     if applied_on_method:
                         args = (self_arg,) + args
@@ -345,25 +344,24 @@
             else:
                 if isinstance(check_param, str):
                     check_only_param_value = get_param_value_from_func_call(
                         param_name=check_param, func=func, call_args=args, call_kwargs=kwargs
                     )
                     tmp_extra_kwargs["__check_only__"] = check_only_param_value
 
-                @wraps(func)
-                def f(**tmp_extra_kwargs):
+                def f(*a, **k):
                     return func(*args, **kwargs)
 
                 f = current_memory.cache(f)
                 result = f(**tmp_extra_kwargs)  # type: ignore[no-untyped-call]
 
             if limit is not None:
                 clean_cachedir_old_entries(
                     f.store_backend,  # type: ignore[attr-defined]
-                    func.__name__,
+                    f.__name__,
                     limit,
                 )
 
             return result
 
         return wrapper
```

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/generic/__init__.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/generic/add_missing_row.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/generic/add_missing_row.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,16 +90,16 @@
         complex_index_values = df.groupby(cols_for_index).sum().index.values
     elif isinstance(complete_index, dict):
         if complete_index["type"] == "date":
             freq = complete_index["freq"]
             date_format = complete_index["format"]
             start = complete_index["start"]
             end = complete_index["end"]
-            if isinstance(freq, dict):  # type: ignore[unreachable]
-                freq = pd.DateOffset(**{k: int(v) for k, v in freq.items()})  # type: ignore[unreachable]
+            if isinstance(freq, dict):
+                freq = pd.DateOffset(**{k: int(v) for k, v in freq.items()})
             new_index = pd.date_range(start=start, end=end, freq=freq)
             complex_index_values = new_index.strftime(date_format).values
         else:
             raise ParamsValueError(f"Unknown complete index type: " f'{complete_index["type"]}')
     else:
         complex_index_values = list(complete_index)
```

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/generic/clean.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/generic/clean.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/generic/combine_columns_aggregation.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/generic/combine_columns_aggregation.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/generic/compute_cumsum.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/generic/compute_cumsum.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/generic/compute_evolution.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/generic/compute_evolution.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/generic/compute_ffill_by_group.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/generic/compute_ffill_by_group.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/generic/date_requester.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/generic/date_requester.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/generic/roll_up.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/generic/roll_up.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     groupby_cols_cpy = list(levels)
     levels_cpy = list(levels)
     levels_cpy.reverse()
 
     extra_groupby_cols = extra_groupby_cols or []
     drop_levels = drop_levels or []
     previous_level = None
-    for (idx, top_level) in enumerate(levels_cpy):
+    for idx, top_level in enumerate(levels_cpy):
         # Aggregation
         gb_df = getattr(
             df.groupby(groupby_cols_cpy + extra_groupby_cols)[groupby_vars], agg_func
         )().reset_index()
 
         # Melt-like columns
         gb_df[var_name] = top_level
```

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/generic/two_values_melt.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/generic/two_values_melt.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/helpers.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/__init__.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/add_aggregation_columns.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/add_aggregation_columns.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/argmax.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/argmax.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/categories_from_dates.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/categories_from_dates.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/converter.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/converter.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/cumsum.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/cumsum.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/fillna.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/fillna.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/filter.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/filter.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/filter_by_date.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/filter_by_date.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/groupby.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/groupby.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/if_else.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/if_else.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-import inspect
-from functools import wraps
 from typing import Any, Dict, List, Union
 
 import pandas as pd
+from typing_extensions import TypeAlias
 
 Condition = Dict[str, Any]
 
 
 def _apply_condition(
     df: pd.DataFrame,
     condition: Union[Condition, List[Condition], str, int, float, None],
@@ -41,57 +40,21 @@
     else:
         # Simple value: condition is a string or a number
         df[new_column] = condition
 
     return df
 
 
-def replace_by_reserved_keywords(f: Any) -> Any:
-    """
-    As `if`, `else` and `then` are reserved keywords, we have to
-    make the mapping to accepted keywords
-    """
-    reserved_keywords_mapping = {"if_": "if", "then_": "then", "else_": "else"}
-
-    @wraps(f)
-    def wrapper(*args, **kwargs):
-        # Update the params to be sent to `if_else` as `if_`, `else_`, `then_`
-        for accepted, reserved in reserved_keywords_mapping.items():
-            if reserved in kwargs:
-                kwargs[accepted] = kwargs.pop(reserved)
-        return f(*args, **kwargs)
-
-    # Update the signature of the wrapper to still have the right documentation
-    # and the excepted `if`, `else`, `then` params
-    sig_with_accepted_params = inspect.signature(f)
-    parameters_with_reserved_names = []
-
-    for param_name, param in sig_with_accepted_params.parameters.items():
-        if param_name in reserved_keywords_mapping:
-            parameters_with_reserved_names.append(
-                param.replace(name=reserved_keywords_mapping[param_name])
-            )
-        else:
-            parameters_with_reserved_names.append(param)
-
-    wrapper.__signature__ = sig_with_accepted_params.replace(  # type: ignore[attr-defined]
-        parameters=parameters_with_reserved_names
-    )
-
-    return wrapper
+_If: TypeAlias = str
+_Then: TypeAlias = Union[str, int, float, Condition, List[Condition]]
+_Else: TypeAlias = Union[None, str, int, float, Condition, List[Condition]]
 
 
-@replace_by_reserved_keywords
 def if_else(
-    df: pd.DataFrame,
-    *,
-    if_: str,
-    then_: Union[str, int, float, Condition, List[Condition]],
-    else_: Union[None, str, int, float, Condition, List[Condition]] = None,
-    new_column: str,
+    df: pd.DataFrame, *, new_column: str, **kwargs: Union[_If, _Then, _Else]
 ) -> pd.DataFrame:
     """
     The usual if...then...else... statement
 
     ---
 
     ### Parameters
@@ -142,14 +105,20 @@
     |  Hell    | HellCity |   -10 |      0     | -5.0 |
     """
     # If the index is not unique (e.g. if the dataframe is a concatenation
     # of multiple dataframes), recompute it
     if not df.index.is_unique:
         df.index = pd.RangeIndex(len(df.index))
 
+    if not (if_ := kwargs.get("if")):
+        raise ValueError("'if' parameter is mandatory")
+    if not (then_ := kwargs.get("then")):
+        raise ValueError("'then' parameter is mandatory")
+    else_ = kwargs.get("else")
+
     if_sub_df = df.query(if_)
     else_sub_df = df[~df.index.isin(if_sub_df.index)]
 
     if_sub_df = _apply_condition(if_sub_df, then_, new_column)
     else_sub_df = _apply_condition(else_sub_df, else_, new_column)
 
     new_df = pd.concat([if_sub_df, else_sub_df]).sort_index()
```

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/json_to_table.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/json_to_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
             "Data should have at least one column with simple data type (not list or dict)"
         )
 
     data = df.to_dict(orient="records")  # json_normalize takes python objects as input
     ret_data = df.copy()
 
     for col in columns:
-
         serie = df[col]
         first_valid_value = _first_valid_value(serie)
 
         if not isinstance(first_valid_value, (list, dict)):
             continue
 
         elif isinstance(first_valid_value, dict):  # creates new columns
```

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/linear_regression.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/linear_regression.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/math.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/math.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/melt.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/melt.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/percentage.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/percentage.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/pivot.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/pivot.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/rank.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/rank.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/rename.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/rename.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/replace.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/replace.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/sort.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/sort.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/text.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/text.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/top.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/top.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/postprocess/waterfall.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/postprocess/waterfall.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/toucan_data_sdk/utils/traceback.py` & `toucan_data_sdk-7.6.0/toucan_data_sdk/utils/traceback.py`

 * *Files identical despite different names*

### Comparing `toucan_data_sdk-7.5.0/PKG-INFO` & `toucan_data_sdk-7.6.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: toucan-data-sdk
-Version: 7.5.0
+Version: 7.6.0
 Summary: Toucan data SDK
 Home-page: https://github.com/ToucanToco/toucan-data-sdk
 License: BSD-3-Clause
 Author: Toucan Toco
 Author-email: dev@toucantoco.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
 Requires-Dist: engarde (>=0.4.0,<0.5.0)
-Requires-Dist: joblib (<1)
+Requires-Dist: joblib (>=1,<2)
 Requires-Dist: pandas (>=1.4.1,<2.0.0)
-Requires-Dist: python-slugify (>=5.0.2,<6.0.0)
-Requires-Dist: tabulate (>=0.8.9,<0.9.0)
+Requires-Dist: python-slugify (>=5.0.2,<7.0.0)
+Requires-Dist: tabulate (>=0.8.9,<0.10.0)
 Requires-Dist: toucan-client (>=1.1.0,<2.0.0)
 Project-URL: Documentation, https://toucantoco.github.io/toucan-data-sdk
 Project-URL: Repository, https://github.com/ToucanToco/toucan-data-sdk
 Description-Content-Type: text/markdown
 
 [![Pypi-v](https://img.shields.io/pypi/v/toucan-data-sdk.svg)](https://pypi.python.org/pypi/toucan-data-sdk)
 [![Pypi-pyversions](https://img.shields.io/pypi/pyversions/toucan-data-sdk.svg)](https://pypi.python.org/pypi/toucan-data-sdk)
```

