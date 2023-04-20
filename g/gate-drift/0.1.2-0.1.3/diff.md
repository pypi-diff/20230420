# Comparing `tmp/gate_drift-0.1.2.tar.gz` & `tmp/gate_drift-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gate_drift-0.1.2.tar", max compression
+gzip compressed data, was "gate_drift-0.1.3.tar", max compression
```

## Comparing `gate_drift-0.1.2.tar` & `gate_drift-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1595 2023-04-20 00:23:42.803802 gate_drift-0.1.2/README.md
--rw-r--r--   0        0        0      183 2023-04-19 23:37:10.238460 gate_drift-0.1.2/gate/__init__.py
--rw-r--r--   0        0        0    14180 2023-04-20 00:24:26.316564 gate_drift-0.1.2/gate/drift.py
--rw-r--r--   0        0        0      919 2023-04-19 23:38:50.065089 gate_drift-0.1.2/gate/statistics.py
--rw-r--r--   0        0        0     2357 2023-04-20 00:24:26.178857 gate_drift-0.1.2/gate/summarize.py
--rw-r--r--   0        0        0     7276 2023-04-20 00:24:26.267241 gate_drift-0.1.2/gate/summary.py
--rw-r--r--   0        0        0     1018 2023-04-20 00:26:59.323979 gate_drift-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2424 1970-01-01 00:00:00.000000 gate_drift-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-04-20 19:33:25.531694 gate_drift-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1595 2023-04-20 00:23:42.803802 gate_drift-0.1.3/README.md
+-rw-r--r--   0        0        0      183 2023-04-19 23:37:10.238460 gate_drift-0.1.3/gate/__init__.py
+-rw-r--r--   0        0        0    14182 2023-04-20 19:33:25.546152 gate_drift-0.1.3/gate/drift.py
+-rw-r--r--   0        0        0      961 2023-04-20 19:33:25.546362 gate_drift-0.1.3/gate/statistics.py
+-rw-r--r--   0        0        0     2357 2023-04-20 00:24:26.178857 gate_drift-0.1.3/gate/summarize.py
+-rw-r--r--   0        0        0     7581 2023-04-20 19:33:25.546579 gate_drift-0.1.3/gate/summary.py
+-rw-r--r--   0        0        0     1018 2023-04-20 19:34:04.471017 gate_drift-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2424 1970-01-01 00:00:00.000000 gate_drift-0.1.3/PKG-INFO
```

### Comparing `gate_drift-0.1.2/README.md` & `gate_drift-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gate_drift-0.1.2/gate/drift.py` & `gate_drift-0.1.3/gate/drift.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 
     @property
     def is_drifted(self) -> bool:
         """
         Indicates whether the partition is drifted or not, compared
         to previous partitions. This is determined by the percentile
         of the partition's score in the distribution of all scores.
-        The threshold is 90%.
+        The threshold is 95%.
         """
-        return self.score_percentile >= 0.85
+        return self.score_percentile >= 0.95
 
     @property
     def score_percentile(self) -> float:
         """Percentile of the partition's score in the distribution
         of all scores."""
         return percentileofscore(self.all_scores, self.score) * 1.0 / 100
 
@@ -217,15 +217,15 @@
     if len(previous_summaries) == 0:
         raise ValueError(
             "You must have at least 1 previous partition summary to detect drift."
         )
 
     partition_key = current_summary.partition_key
     columns = current_summary.columns
-    statistics = current_summary.statistics
+    statistics = current_summary.statistics()
 
     # Create validity vector
     if not validity:
         validity = [1] * len(previous_summaries)
     if len(validity) != len(previous_summaries):
         raise ValueError(
             f"Validity vector has length {len(validity)} but should have"
```

### Comparing `gate_drift-0.1.2/gate/statistics.py` & `gate_drift-0.1.3/gate/statistics.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,25 +16,27 @@
         ValueError: If the type is unknown.
     """
 
     if t == "int":
         return [
             "coverage",
             "mean",
-            "stdev",
+            "p50",
+            # "stdev",
             "num_unique_values",
             "occurrence_ratio",
             "p95",
         ]
 
     if t == "float":
         return [
             "coverage",
             "mean",
-            "stdev",
+            "p50",
+            # "stdev",
             "p95",
         ]
 
     if t == "string":
         return ["coverage", "num_unique_values", "occurrence_ratio"]
 
     raise ValueError(f"Unknown type {t}")
```

### Comparing `gate_drift-0.1.2/gate/summarize.py` & `gate_drift-0.1.3/gate/summarize.py`

 * *Files identical despite different names*

### Comparing `gate_drift-0.1.2/gate/summary.py` & `gate_drift-0.1.3/gate/summary.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,24 +43,25 @@
     @staticmethod
     def statistics() -> typing.List[str]:
         """
         Returns list of statistics computed for each column:
 
         * coverage: Fraction of rows that are not null.
         * mean: Mean of the column.
-        * stdev: Standard deviation of the column.
+        * p50: Median of the column.
         * num_unique_values: Number of unique values in the column.
         * occurrence_ratio: Ratio of the most common value to all other
         values.
         * num_frequent_values: Number of values that occur more than once.
         """
         return [
             "coverage",
             "mean",
-            "stdev",
+            # "stdev",
+            "p50",
             "num_unique_values",
             "occurrence_ratio",
             # "num_frequent_values",
             "p95",
         ]
 
     @classmethod
@@ -118,17 +119,23 @@
         statistics = {
             "coverage": polars_df.groupby(partition_key).agg(
                 [pl.col(c).is_not_null().mean().alias(c) for c in columns]
             ),
             "mean": polars_df.groupby(partition_key).agg(
                 [pl.col(c).mean().alias(c) for c in float_columns + int_columns]
             ),
-            "stdev": polars_df.groupby(partition_key).agg(
+            # "stdev": polars_df.groupby(partition_key).agg(
+            #     [
+            #         pl.col(c).std().cast(pl.Float64).alias(c)
+            #         for c in float_columns + int_columns
+            #     ]
+            # ),
+            "p50": polars_df.groupby(partition_key).agg(
                 [
-                    pl.col(c).std().cast(pl.Float64).alias(c)
+                    pl.col(c).quantile(0.5).cast(pl.Float64).alias(c)
                     for c in float_columns + int_columns
                 ]
             ),
             "num_unique_values": polars_df.groupby(partition_key).agg(
                 [
                     pl.col(c).approx_unique().cast(pl.Float64).alias(c)
                     for c in string_columns + int_columns
@@ -169,14 +176,15 @@
             .pivot(
                 index=[partition_key, "column"],
                 columns="statistic",
                 values="value",
             )
             .reset_index()
         )
+        pivoted.columns = pivoted.columns.tolist()
 
         groups = []
         for _, group in pivoted.groupby(partition_key):
             groups.append(
                 cls(
                     group.reset_index(drop=True),
                     string_columns,
```

### Comparing `gate_drift-0.1.2/pyproject.toml` & `gate_drift-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gate-drift"
-version = "0.1.2"
+version = "0.1.3"
 description = "Data drift detection tool for machine learning pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "gate"}]
 
 [tool.poetry.dependencies]
```

### Comparing `gate_drift-0.1.2/PKG-INFO` & `gate_drift-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gate-drift
-Version: 0.1.2
+Version: 0.1.3
 Summary: Data drift detection tool for machine learning pipelines.
 License: MIT
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

