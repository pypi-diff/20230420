# Comparing `tmp/slurmui-0.3.0.0-py3-none-any.whl.zip` & `tmp/slurmui-0.3.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6546 bytes, number of entries: 10
+Zip file size: 6578 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx       27 b- defN 23-Apr-20 12:40 slurmui/__init__.py
--rw-rw-r--  2.0 unx       23 b- defN 23-Apr-20 12:39 slurmui/_version.py
+-rw-rw-r--  2.0 unx       23 b- defN 23-Apr-20 13:16 slurmui/_version.py
 -rw-rw-r--  2.0 unx     9278 b- defN 23-Jan-13 19:20 slurmui/debug_strings.py
--rw-rw-r--  2.0 unx    11249 b- defN 23-Apr-20 12:47 slurmui/slurmui.py
+-rw-rw-r--  2.0 unx    11342 b- defN 23-Apr-20 13:16 slurmui/slurmui.py
 -rw-rw-r--  2.0 unx      269 b- defN 23-Jan-03 17:14 slurmui/slurmui_cli.py
--rw-rw-r--  2.0 unx      836 b- defN 23-Apr-20 12:47 slurmui-0.3.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-20 12:47 slurmui-0.3.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       60 b- defN 23-Apr-20 12:47 slurmui-0.3.0.0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 23-Apr-20 12:47 slurmui-0.3.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      784 b- defN 23-Apr-20 12:47 slurmui-0.3.0.0.dist-info/RECORD
-10 files, 22626 bytes uncompressed, 5204 bytes compressed:  77.0%
+-rw-rw-r--  2.0 unx      836 b- defN 23-Apr-20 13:17 slurmui-0.3.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-20 13:17 slurmui-0.3.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       60 b- defN 23-Apr-20 13:17 slurmui-0.3.0.1.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 23-Apr-20 13:17 slurmui-0.3.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      784 b- defN 23-Apr-20 13:17 slurmui-0.3.0.1.dist-info/RECORD
+10 files, 22719 bytes uncompressed, 5236 bytes compressed:  77.0%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: slurmui/slurmui.py
 Comment: 
 
 Filename: slurmui/slurmui_cli.py
 Comment: 
 
-Filename: slurmui-0.3.0.0.dist-info/METADATA
+Filename: slurmui-0.3.0.1.dist-info/METADATA
 Comment: 
 
-Filename: slurmui-0.3.0.0.dist-info/WHEEL
+Filename: slurmui-0.3.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: slurmui-0.3.0.0.dist-info/entry_points.txt
+Filename: slurmui-0.3.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: slurmui-0.3.0.0.dist-info/top_level.txt
+Filename: slurmui-0.3.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: slurmui-0.3.0.0.dist-info/RECORD
+Filename: slurmui-0.3.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## slurmui/_version.py

```diff
@@ -1 +1 @@
-__version__ = "0.3.0.0"
+__version__ = "0.3.0.1"
```

## slurmui/slurmui.py

```diff
@@ -33,36 +33,37 @@
     gpu_overview_df = None
     sqeue_df =None
 
     def compose(self) -> ComposeResult:
         self.header = Header()
         self.footer = Footer()
         self.table = DataTable( id="table")
+        self.table.zebra_stripes = True
         self.txt_log = TextLog(wrap=True, highlight=True, id="info")
         yield self.header
         yield Container(self.table, self.txt_log)
         yield self.footer
 
     
     def query_squeue(self, sort_column=None, sort_ascending=True):
         squeue_df = get_squeue() 
         if sort_column is not None:
             squeue_df = squeue_df.sort_values(squeue_df.columns[sort_column],ascending=sort_ascending)
         self.sqeue_df = squeue_df
         return squeue_df
 
     def update_squeue_table(self, sort_column=None, sort_ascending=True):
-        self.table.clear()
+        self.table.clear(columns=True)
         squeue_df = self.query_squeue(sort_column=sort_column, sort_ascending=sort_ascending)
         # add device information
         squeue_df["GPU_IDS"] = "N/A"
         real_session_mask = squeue_df["PA"]!="in"
         if real_session_mask.any():
             squeue_df["GPU_IDS"][real_session_mask] =squeue_df[real_session_mask]["JOBID"].apply(lambda x: get_job_gpu_ids(x))
-        self.table.columns = []
+        # self.table.columns = []
         self.table.add_columns(*squeue_df.columns)
         for row in squeue_df.iterrows():
             table_row = [str(x) for x in row[1].values]
             self.table.add_row(*table_row)
         self.table.focus()
 
     def action_refresh(self):
@@ -137,16 +138,15 @@
         total_num_gpus = overview_df["#Total"].sum()
         total_available = overview_df["#Avail"].sum()
         self.title = f"SlurmUI --- GPU STATS: {total_available}/{total_num_gpus} -- Version: {__version__}"
         return overview_df
 
 
     def update_gpu_table(self, sort_column=None, sort_ascending=True):
-        self.table.clear()
-        self.table.columns = []
+        self.table.clear(columns=True)
         overview_df = self.query_gpus(sort_column=sort_column, sort_ascending=sort_ascending)
         self.table.add_columns(*overview_df.columns)
         for row in overview_df.iterrows():
             table_row = [str(x) for x in row[1].values]
             self.table.add_row(*table_row)
         self.table.focus()
 
@@ -157,26 +157,27 @@
         try:
             self.update_gpu_table()
         except Exception as e:
             self.txt_log.clear()
             self.txt_log.write(str(e))
 
     def action_sort(self):
-        selected_column = self.table.cursor_cell
-        column_idx = selected_column.column
+        # selected_column = self.table.cursor_cell
+        column_idx = self.table.cursor_column
         if column_idx != self.STAGE.get("column_idx"):
             self.STAGE["sort_ascending"] = False
         else:
             self.STAGE["sort_ascending"] = not self.STAGE.get("sort_ascending",True)
         self.STAGE['column_idx'] = column_idx
         if self.STAGE["action"] == "monitor":
             self.update_squeue_table(sort_column=column_idx, sort_ascending=self.STAGE["sort_ascending"])
         elif self.STAGE["action"] == "gpu":
             self.update_gpu_table(sort_column=column_idx, sort_ascending=self.STAGE["sort_ascending"])
 
+        self.table.cursor_coordinate  = (0,column_idx)
 
 
     def update_log(self, job_id):
         if not DEBUG:
             log_fn = get_log_fn(job_id)
             txt_lines = read_log(log_fn)
         else:
```

