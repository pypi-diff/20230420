# Comparing `tmp/gate_drift-0.1.1.tar.gz` & `tmp/gate_drift-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gate_drift-0.1.1.tar", max compression
+gzip compressed data, was "gate_drift-0.1.2.tar", max compression
```

## Comparing `gate_drift-0.1.1.tar` & `gate_drift-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      626 2023-04-19 06:54:12.471200 gate_drift-0.1.1/README.md
--rw-r--r--   0        0        0      183 2023-04-19 23:37:10.238460 gate_drift-0.1.1/gate/__init__.py
--rw-r--r--   0        0        0    14397 2023-04-20 00:14:55.533086 gate_drift-0.1.1/gate/drift.py
--rw-r--r--   0        0        0      919 2023-04-19 23:38:50.065089 gate_drift-0.1.1/gate/statistics.py
--rw-r--r--   0        0        0     2379 2023-04-19 23:44:48.044269 gate_drift-0.1.1/gate/summarize.py
--rw-r--r--   0        0        0     7436 2023-04-20 00:07:33.640968 gate_drift-0.1.1/gate/summary.py
--rw-r--r--   0        0        0     1018 2023-04-20 00:19:55.673095 gate_drift-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1455 1970-01-01 00:00:00.000000 gate_drift-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1595 2023-04-20 00:23:42.803802 gate_drift-0.1.2/README.md
+-rw-r--r--   0        0        0      183 2023-04-19 23:37:10.238460 gate_drift-0.1.2/gate/__init__.py
+-rw-r--r--   0        0        0    14180 2023-04-20 00:24:26.316564 gate_drift-0.1.2/gate/drift.py
+-rw-r--r--   0        0        0      919 2023-04-19 23:38:50.065089 gate_drift-0.1.2/gate/statistics.py
+-rw-r--r--   0        0        0     2357 2023-04-20 00:24:26.178857 gate_drift-0.1.2/gate/summarize.py
+-rw-r--r--   0        0        0     7276 2023-04-20 00:24:26.267241 gate_drift-0.1.2/gate/summary.py
+-rw-r--r--   0        0        0     1018 2023-04-20 00:26:59.323979 gate_drift-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2424 1970-01-01 00:00:00.000000 gate_drift-0.1.2/PKG-INFO
```

### Comparing `gate_drift-0.1.1/gate/drift.py` & `gate_drift-0.1.2/gate/drift.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,17 +56,15 @@
         and meaning of column names (determined via embeddings). Returns
         a dictionary with cluster numbers as keys and lists of columns
         as values.
         """
         if self._clustered_features is None:
             raise ValueError("No clustering was performed.")
 
-        clustering_map = self._clustered_features.groupby("cluster")[
-            "column"
-        ].agg(set)
+        clustering_map = self._clustered_features.groupby("cluster")["column"].agg(set)
         clustering_map = clustering_map.apply(list)
 
         return clustering_map.to_dict()
 
     def drill_down(self) -> pd.DataFrame:
         """Compute the columns with highest magnitude anomaly scores.
         Anomaly scores are computed as the z-score of the column with
@@ -96,42 +94,34 @@
 
         # Return a dataframe with features with highest magnitude anomaly
         # scores
 
         last_day = self._nn_features.iloc[-1]
         sorted_cols = last_day.abs().sort_values(ascending=False).index
         sorted_df = last_day[sorted_cols].to_frame()
-        sorted_df.rename(
-            columns={sorted_df.columns[0]: "z-score"}, inplace=True
-        )
+        sorted_df.rename(columns={sorted_df.columns[0]: "z-score"}, inplace=True)
         sorted_df = sorted_df.rename_axis(["column", "statistic"])
 
         if self._clustered_features is not None:
             # Join the clustered features with the sorted_df
             # sorted_df.rename(index={"column": "cluster"}, inplace=True)
-            sorted_df = sorted_df.rename_axis(
-                ["cluster", "statistic"]
-            ).reset_index()
-            sorted_df.rename(
-                columns={"z-score": "z-score-cluster"}, inplace=True
-            )
+            sorted_df = sorted_df.rename_axis(["cluster", "statistic"]).reset_index()
+            sorted_df.rename(columns={"z-score": "z-score-cluster"}, inplace=True)
 
             sorted_df = sorted_df.merge(
                 self._clustered_features,
                 on=["cluster", "statistic"],
                 how="left",
             )
 
             # Sort again
             sorted_df = sorted_df.reindex(
                 sorted_df[["z-score-cluster", "z-score"]]
                 .abs()
-                .sort_values(
-                    by=["z-score-cluster", "z-score"], ascending=False
-                )
+                .sort_values(by=["z-score-cluster", "z-score"], ascending=False)
                 .index
             )
             sorted_df.set_index(["column", "statistic"], inplace=True)
 
         return sorted_df
 
     def __str__(self) -> str:
@@ -172,25 +162,21 @@
         dd_results = self.drill_down()
 
         if self._clustered_features is not None:
             # Sort by z-score first, then z-score-cluster
             dd_results = dd_results.reindex(
                 dd_results[["z-score-cluster", "z-score"]]
                 .abs()
-                .sort_values(
-                    by=["z-score", "z-score-cluster"], ascending=False
-                )
+                .sort_values(by=["z-score", "z-score-cluster"], ascending=False)
                 .index
             )
 
         dd_results.reset_index(inplace=True)
 
-        dd_results.drop_duplicates(
-            subset=["column"], keep="first", inplace=True
-        )
+        dd_results.drop_duplicates(subset=["column"], keep="first", inplace=True)
         dd_results.set_index("column", inplace=True)
 
         if self._clustered_features is not None:
             # Reorder columns
             dd_results = dd_results[
                 ["statistic", "z-score", "cluster", "z-score-cluster"]
             ]
@@ -226,16 +212,15 @@
             Number of nearest neighbor partitions to inspect.
             Defaults to 5.
 
     Returns (DriftResult): DriftResult object with score and score percentile.
     """
     if len(previous_summaries) == 0:
         raise ValueError(
-            "You must have at least 1 previous partition summary to detect"
-            " drift."
+            "You must have at least 1 previous partition summary to detect drift."
         )
 
     partition_key = current_summary.partition_key
     columns = current_summary.columns
     statistics = current_summary.statistics
 
     # Create validity vector
@@ -249,17 +234,17 @@
     validity.append(1)
 
     prev_summaries = [
         s.value for i, s in enumerate(previous_summaries) if validity[i] == 1
     ]
 
     # Normalize current and previous partition summaries
-    all_summaries = pd.concat(
-        prev_summaries + [current_summary.value]
-    ).reset_index(drop=True)
+    all_summaries = pd.concat(prev_summaries + [current_summary.value]).reset_index(
+        drop=True
+    )
 
     normalized = all_summaries.melt(
         id_vars=[partition_key, "column"],
         value_vars=statistics,
         var_name="statistic",
         value_name="value",
     ).dropna()
```

### Comparing `gate_drift-0.1.1/gate/statistics.py` & `gate_drift-0.1.2/gate/statistics.py`

 * *Files identical despite different names*

### Comparing `gate_drift-0.1.1/gate/summarize.py` & `gate_drift-0.1.2/gate/summarize.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,17 +42,15 @@
             If `partition_key `is empty and `previous_summaries` is empty.
         ValueError:
             If `partition_key` is not in `df.columns`.
         ValueError:
             If any column in `columns` is not in `df.columns`.
     """
     if partition_key == "group":
-        raise ValueError(
-            "Please rename the partition_key; it cannot be `group`."
-        )
+        raise ValueError("Please rename the partition_key; it cannot be `group`.")
 
     if len(previous_summaries) == 0:
         if len(columns) == 0:
             raise ValueError(
                 "You must pass in some columns if you do not have any previous"
                 " summaries."
             )
```

### Comparing `gate_drift-0.1.1/gate/summary.py` & `gate_drift-0.1.2/gate/summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,32 +79,28 @@
             int_columns = previous_summaries[0]._int_columns
         else:
             # Set up columns if it's the first partition
             assert len(columns) > 0
 
             if not set(columns).issubset(set(raw_data.columns)):
                 raise ValueError(
-                    "Columns to compute summaries on are not all in the"
-                    " dataframe."
+                    "Columns to compute summaries on are not all in the dataframe."
                 )
             types = raw_data.dtypes.to_dict()
             column_types = {c: types[c] for c in columns}
             string_columns = [c for c, t in column_types.items() if t == "O"]
-            float_columns = [
-                c for c, t in column_types.items() if t == "float"
-            ]
+            float_columns = [c for c, t in column_types.items() if t == "float"]
             int_columns = [c for c, t in column_types.items() if t == "int"]
-            assert len(string_columns) + len(float_columns) + len(
-                int_columns
-            ) == len(columns)
+            assert len(string_columns) + len(float_columns) + len(int_columns) == len(
+                columns
+            )
 
         if partition_key not in raw_data.columns:
             raise ValueError(
-                f"Partition column {partition_key} is not in dataframe"
-                " columns."
+                f"Partition column {partition_key} is not in dataframe columns."
             )
         if not set(columns).issubset(set(raw_data.columns)):
             raise ValueError(
                 "Columns to compute summaries on are not all in the dataframe."
             )
 
         # Compute the summary statistics
@@ -120,18 +116,15 @@
         # )
 
         statistics = {
             "coverage": polars_df.groupby(partition_key).agg(
                 [pl.col(c).is_not_null().mean().alias(c) for c in columns]
             ),
             "mean": polars_df.groupby(partition_key).agg(
-                [
-                    pl.col(c).mean().alias(c)
-                    for c in float_columns + int_columns
-                ]
+                [pl.col(c).mean().alias(c) for c in float_columns + int_columns]
             ),
             "stdev": polars_df.groupby(partition_key).agg(
                 [
                     pl.col(c).std().cast(pl.Float64).alias(c)
                     for c in float_columns + int_columns
                 ]
             ),
@@ -154,17 +147,15 @@
                     for c in float_columns + int_columns
                 ]
             ),
         }
 
         # Merge the statistics into a single dataframe
         for name, df in statistics.items():
-            statistics[name] = df.with_columns(
-                [pl.lit(name).alias("statistic")]
-            )
+            statistics[name] = df.with_columns([pl.lit(name).alias("statistic")])
 
         current_statistics = pl.concat(
             list(statistics.values()), how="diagonal"
         ).to_pandas()
 
         # Pivot such that columns are the statistics and rows are the row name,
         # and it's grouped by partition col
```

### Comparing `gate_drift-0.1.1/pyproject.toml` & `gate_drift-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gate-drift"
-version = "0.1.1"
+version = "0.1.2"
 description = "Data drift detection tool for machine learning pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "gate"}]
 
 [tool.poetry.dependencies]
```

