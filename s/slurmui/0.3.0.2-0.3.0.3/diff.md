# Comparing `tmp/slurmui-0.3.0.2-py3-none-any.whl.zip` & `tmp/slurmui-0.3.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6678 bytes, number of entries: 10
+Zip file size: 6685 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx       27 b- defN 23-Apr-20 15:06 slurmui/__init__.py
--rw-rw-r--  2.0 unx       23 b- defN 23-Apr-20 15:07 slurmui/_version.py
+-rw-rw-r--  2.0 unx       23 b- defN 23-Apr-20 15:19 slurmui/_version.py
 -rw-rw-r--  2.0 unx     9278 b- defN 23-Jan-13 19:20 slurmui/debug_strings.py
--rw-rw-r--  2.0 unx    11870 b- defN 23-Apr-20 15:06 slurmui/slurmui.py
+-rw-rw-r--  2.0 unx    11844 b- defN 23-Apr-20 15:18 slurmui/slurmui.py
 -rw-rw-r--  2.0 unx      269 b- defN 23-Jan-03 17:14 slurmui/slurmui_cli.py
--rw-rw-r--  2.0 unx      836 b- defN 23-Apr-20 15:07 slurmui-0.3.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-20 15:07 slurmui-0.3.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       60 b- defN 23-Apr-20 15:07 slurmui-0.3.0.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 23-Apr-20 15:07 slurmui-0.3.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      784 b- defN 23-Apr-20 15:07 slurmui-0.3.0.2.dist-info/RECORD
-10 files, 23247 bytes uncompressed, 5336 bytes compressed:  77.0%
+-rw-rw-r--  2.0 unx      836 b- defN 23-Apr-20 15:19 slurmui-0.3.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-20 15:19 slurmui-0.3.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       60 b- defN 23-Apr-20 15:19 slurmui-0.3.0.3.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 23-Apr-20 15:19 slurmui-0.3.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      784 b- defN 23-Apr-20 15:19 slurmui-0.3.0.3.dist-info/RECORD
+10 files, 23221 bytes uncompressed, 5343 bytes compressed:  77.0%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: slurmui/slurmui.py
 Comment: 
 
 Filename: slurmui/slurmui_cli.py
 Comment: 
 
-Filename: slurmui-0.3.0.2.dist-info/METADATA
+Filename: slurmui-0.3.0.3.dist-info/METADATA
 Comment: 
 
-Filename: slurmui-0.3.0.2.dist-info/WHEEL
+Filename: slurmui-0.3.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: slurmui-0.3.0.2.dist-info/entry_points.txt
+Filename: slurmui-0.3.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: slurmui-0.3.0.2.dist-info/top_level.txt
+Filename: slurmui-0.3.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: slurmui-0.3.0.2.dist-info/RECORD
+Filename: slurmui-0.3.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## slurmui/_version.py

```diff
@@ -1 +1 @@
-__version__ = "0.3.0.2"
+__version__ = "0.3.0.3"
```

## slurmui/slurmui.py

```diff
@@ -89,17 +89,18 @@
     # def action_modal(self):
     #     log_screen = LogScreen()
     #     #log_screen.load_log()
     #     self.push_screen(log_screen)
     #     log_screen.on_ready()
 
     def _get_selected_job(self):
-        selected_column = self.table.cursor_cell.row
-        job_id = self.table.data[selected_column][0]
-        job_name = self.table.data[selected_column][2]
+        row_idx = self.table.cursor_row
+        row = self.table.get_row_at(row_idx)
+        job_id = row[0]
+        job_name = row[2]
         return job_id, job_name
 
     def _minimize_text_log(self):
         self.table.styles.height="80%"
         self.txt_log.styles.max_height="10%"
         self.txt_log.can_focus = False
         self.txt_log.styles.border = ("heavy","grey")
```

## Comparing `slurmui-0.3.0.2.dist-info/METADATA` & `slurmui-0.3.0.3.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slurmui
-Version: 0.3.0.2
+Version: 0.3.0.3
 Summary: Terminal UI for Slurm
 Home-page: https://github.com/SirWyver/slurmui
 Author: Norman Müller
 Author-email: norman.mueller@tum.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `slurmui-0.3.0.2.dist-info/RECORD` & `slurmui-0.3.0.3.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 slurmui/__init__.py,sha256=BVNOMLHFAyGklO8r4IWoXKL-miYRwTy0R3yaPTqINVg,27
-slurmui/_version.py,sha256=NSOd25RVVJvwXfO5tNi7S2rrT_mYfzKniYFgJDcxi60,23
+slurmui/_version.py,sha256=qzaip15ihZ-sz-Z7wOU7tMHu_weizIUxrpoHOAFOyic,23
 slurmui/debug_strings.py,sha256=oMimK75barJFA0SHZC6rp1YN7IE1qOA80FRpthPm3Kc,9278
-slurmui/slurmui.py,sha256=ruyuMxkvHKTyBSO9XKJWcQP4y50PPcqSypeD5u7FcHw,11870
+slurmui/slurmui.py,sha256=QjLiNVBdShRFHbWfA1QRyuLlF6yMSSs_tsAU6UdwIHg,11844
 slurmui/slurmui_cli.py,sha256=sw6Rm-prSO6v3ErtWfwN7T7KVh0MNvbAV2WZG1pEQfo,269
-slurmui-0.3.0.2.dist-info/METADATA,sha256=92jYJrkTGpEeya4lqM41mA8D2pwyzMU6zpqzbOH-WC8,836
-slurmui-0.3.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-slurmui-0.3.0.2.dist-info/entry_points.txt,sha256=jSENaCY2DRNuV8d3E5YOf4cYXWLB_DsBx74-lfl2_ow,60
-slurmui-0.3.0.2.dist-info/top_level.txt,sha256=a9nYoG_4X7NSFipwEd72kKiZ2PuL-z3COkZfeqkgmu4,8
-slurmui-0.3.0.2.dist-info/RECORD,,
+slurmui-0.3.0.3.dist-info/METADATA,sha256=z3Ar8wOAeueIShzPeys3QOxPoB95MjTHpTXW5v0UXSg,836
+slurmui-0.3.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+slurmui-0.3.0.3.dist-info/entry_points.txt,sha256=jSENaCY2DRNuV8d3E5YOf4cYXWLB_DsBx74-lfl2_ow,60
+slurmui-0.3.0.3.dist-info/top_level.txt,sha256=a9nYoG_4X7NSFipwEd72kKiZ2PuL-z3COkZfeqkgmu4,8
+slurmui-0.3.0.3.dist-info/RECORD,,
```

