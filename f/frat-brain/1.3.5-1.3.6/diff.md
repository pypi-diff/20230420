# Comparing `tmp/frat_brain-1.3.5.tar.gz` & `tmp/frat_brain-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frat_brain-1.3.5.tar", max compression
+gzip compressed data, was "frat_brain-1.3.6.tar", max compression
```

## Comparing `frat_brain-1.3.5.tar` & `frat_brain-1.3.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    11357 2023-02-27 16:39:34.675704 frat_brain-1.3.5/LICENSE
--rw-r--r--   0        0        0     3458 2023-03-16 16:32:12.397831 frat_brain-1.3.5/README.md
--rw-r--r--   0        0        0    53751 2023-03-31 16:34:44.888814 frat_brain-1.3.5/fRAT/__main__.py
--rw-r--r--   0        0        0       22 2023-04-03 15:48:56.862090 frat_brain-1.3.5/fRAT/_version.py
--rw-r--r--   0        0        0       62 2023-01-10 15:17:29.388582 frat_brain-1.3.5/fRAT/configuration_profiles/latest_settings.toml
--rw-r--r--   0        0        0     4160 2023-03-30 13:46:51.050383 frat_brain-1.3.5/fRAT/configuration_profiles/maps/default_config.toml
--rw-r--r--   0        0        0     4291 2023-03-30 13:46:51.091125 frat_brain-1.3.5/fRAT/configuration_profiles/maps/statmap_config.toml
--rw-r--r--   0        0        0     4160 2023-03-30 13:46:51.060703 frat_brain-1.3.5/fRAT/configuration_profiles/maps/test_config.toml
--rw-r--r--   0        0        0    17981 2023-03-30 13:46:50.969594 frat_brain-1.3.5/fRAT/configuration_profiles/roi_analysis/default_config.toml
--rw-r--r--   0        0        0    17786 2023-03-30 14:29:23.024195 frat_brain-1.3.5/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml
--rw-r--r--   0        0        0    17395 2023-03-30 13:46:51.070056 frat_brain-1.3.5/fRAT/configuration_profiles/roi_analysis/test_config.toml
--rw-r--r--   0        0        0     7414 2021-01-13 12:54:50.481721 frat_brain-1.3.5/fRAT/images/fRAT.gif
--rw-r--r--   0        0        0    10608 2023-03-16 15:13:18.683527 frat_brain-1.3.5/fRAT/nogui.py
--rw-r--r--   0        0        0      172 2023-02-15 18:49:01.736319 frat_brain-1.3.5/fRAT/utils/__init__.py
--rw-r--r--   0        0        0      358 2023-03-06 14:01:57.326471 frat_brain-1.3.5/fRAT/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    46762 2023-03-30 13:46:51.911473 frat_brain-1.3.5/fRAT/utils/__pycache__/analysis.cpython-310.pyc
--rw-r--r--   0        0        0     6517 2023-03-06 14:02:43.973079 frat_brain-1.3.5/fRAT/utils/__pycache__/dash_report.cpython-310.pyc
--rw-r--r--   0        0        0     2487 2023-03-06 14:02:43.887374 frat_brain-1.3.5/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc
--rw-r--r--   0        0        0    17440 2023-03-31 16:31:35.239156 frat_brain-1.3.5/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc
--rw-r--r--   0        0        0    22222 2023-03-30 13:38:00.532124 frat_brain-1.3.5/fRAT/utils/__pycache__/figures.cpython-310.pyc
--rw-r--r--   0        0        0     6376 2023-03-06 14:02:43.623174 frat_brain-1.3.5/fRAT/utils/__pycache__/html_report.cpython-310.pyc
--rw-r--r--   0        0        0     2833 2023-03-06 14:02:48.146041 frat_brain-1.3.5/fRAT/utils/__pycache__/printResults.cpython-310.pyc
--rw-r--r--   0        0        0    30421 2023-03-30 13:25:04.257333 frat_brain-1.3.5/fRAT/utils/__pycache__/statistics.cpython-310.pyc
--rw-r--r--   0        0        0    11331 2023-03-14 17:05:50.271422 frat_brain-1.3.5/fRAT/utils/__pycache__/statmap.cpython-310.pyc
--rw-r--r--   0        0        0     5375 2023-03-06 14:02:43.929731 frat_brain-1.3.5/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc
--rw-r--r--   0        0        0    14966 2023-03-31 15:25:12.995866 frat_brain-1.3.5/fRAT/utils/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0    78887 2023-03-30 13:40:55.436286 frat_brain-1.3.5/fRAT/utils/analysis.py
--rw-r--r--   0        0        0   201570 2023-01-05 15:18:43.590726 frat_brain-1.3.5/fRAT/utils/bootstrap.css
--rw-r--r--   0        0        0     8001 2023-02-15 18:37:18.803196 frat_brain-1.3.5/fRAT/utils/dash_report.py
--rw-r--r--   0        0        0     2587 2023-02-14 13:47:31.387338 frat_brain-1.3.5/fRAT/utils/directory_comparison.py
--rw-r--r--   0        0        0    34582 2023-04-03 14:11:00.889152 frat_brain-1.3.5/fRAT/utils/fRAT_config_setup.py
--rw-r--r--   0        0        0    36602 2023-03-30 13:31:17.393317 frat_brain-1.3.5/fRAT/utils/figures.py
--rw-r--r--   0        0        0     6636 2023-01-20 14:35:18.848122 frat_brain-1.3.5/fRAT/utils/html_report.py
--rw-r--r--   0        0        0     3151 2023-02-15 19:00:37.924453 frat_brain-1.3.5/fRAT/utils/printResults.py
--rw-r--r--   0        0        0       97 2023-01-05 15:18:43.590957 frat_brain-1.3.5/fRAT/utils/script.js
--rw-r--r--   0        0        0    50167 2023-03-30 13:20:28.588609 frat_brain-1.3.5/fRAT/utils/statistics.py
--rw-r--r--   0        0        0    16388 2023-03-14 17:05:44.468988 frat_brain-1.3.5/fRAT/utils/statmap.py
--rw-r--r--   0        0        0     8967 2023-01-31 14:53:42.200233 frat_brain-1.3.5/fRAT/utils/statmap_config_setup.py
--rw-r--r--   0        0        0    18878 2023-03-30 14:24:26.183184 frat_brain-1.3.5/fRAT/utils/utils.py
--rw-r--r--   0        0        0     2390 2023-04-03 15:48:45.725455 frat_brain-1.3.5/pyproject.toml
--rw-r--r--   0        0        0     6398 1970-01-01 00:00:00.000000 frat_brain-1.3.5/setup.py
--rw-r--r--   0        0        0     7198 1970-01-01 00:00:00.000000 frat_brain-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-27 16:39:34.675704 frat_brain-1.3.6/LICENSE
+-rw-r--r--   0        0        0     3046 2023-04-05 12:46:27.664420 frat_brain-1.3.6/README.md
+-rw-r--r--   0        0        0    54049 2023-04-05 12:18:29.787029 frat_brain-1.3.6/fRAT/__main__.py
+-rw-r--r--   0        0        0       22 2023-04-03 15:48:56.862090 frat_brain-1.3.6/fRAT/_version.py
+-rw-r--r--   0        0        0       62 2023-01-10 15:17:29.388582 frat_brain-1.3.6/fRAT/configuration_profiles/latest_settings.toml
+-rw-r--r--   0        0        0     4160 2023-03-30 13:46:51.050383 frat_brain-1.3.6/fRAT/configuration_profiles/maps/default_config.toml
+-rw-r--r--   0        0        0     4291 2023-03-30 13:46:51.091125 frat_brain-1.3.6/fRAT/configuration_profiles/maps/statmap_config.toml
+-rw-r--r--   0        0        0     4160 2023-03-30 13:46:51.060703 frat_brain-1.3.6/fRAT/configuration_profiles/maps/test_config.toml
+-rw-r--r--   0        0        0    17981 2023-03-30 13:46:50.969594 frat_brain-1.3.6/fRAT/configuration_profiles/roi_analysis/default_config.toml
+-rw-r--r--   0        0        0    17981 2023-04-20 15:58:41.535925 frat_brain-1.3.6/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml
+-rw-r--r--   0        0        0    17395 2023-03-30 13:46:51.070056 frat_brain-1.3.6/fRAT/configuration_profiles/roi_analysis/test_config.toml
+-rw-r--r--   0        0        0     7414 2021-01-13 12:54:50.481721 frat_brain-1.3.6/fRAT/images/fRAT.gif
+-rw-r--r--   0        0        0    10608 2023-03-16 15:13:18.683527 frat_brain-1.3.6/fRAT/nogui.py
+-rw-r--r--   0        0        0      172 2023-02-15 18:49:01.736319 frat_brain-1.3.6/fRAT/utils/__init__.py
+-rw-r--r--   0        0        0      358 2023-03-06 14:01:57.326471 frat_brain-1.3.6/fRAT/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    46762 2023-03-30 13:46:51.911473 frat_brain-1.3.6/fRAT/utils/__pycache__/analysis.cpython-310.pyc
+-rw-r--r--   0        0        0     6517 2023-03-06 14:02:43.973079 frat_brain-1.3.6/fRAT/utils/__pycache__/dash_report.cpython-310.pyc
+-rw-r--r--   0        0        0     2487 2023-03-06 14:02:43.887374 frat_brain-1.3.6/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc
+-rw-r--r--   0        0        0    17636 2023-04-05 12:13:52.837379 frat_brain-1.3.6/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc
+-rw-r--r--   0        0        0    22256 2023-04-20 15:50:49.215386 frat_brain-1.3.6/fRAT/utils/__pycache__/figures.cpython-310.pyc
+-rw-r--r--   0        0        0     6376 2023-03-06 14:02:43.623174 frat_brain-1.3.6/fRAT/utils/__pycache__/html_report.cpython-310.pyc
+-rw-r--r--   0        0        0     2833 2023-03-06 14:02:48.146041 frat_brain-1.3.6/fRAT/utils/__pycache__/printResults.cpython-310.pyc
+-rw-r--r--   0        0        0    30421 2023-03-30 13:25:04.257333 frat_brain-1.3.6/fRAT/utils/__pycache__/statistics.cpython-310.pyc
+-rw-r--r--   0        0        0    11331 2023-03-14 17:05:50.271422 frat_brain-1.3.6/fRAT/utils/__pycache__/statmap.cpython-310.pyc
+-rw-r--r--   0        0        0     5375 2023-03-06 14:02:43.929731 frat_brain-1.3.6/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc
+-rw-r--r--   0        0        0    14975 2023-04-20 11:52:26.913182 frat_brain-1.3.6/fRAT/utils/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0    78887 2023-03-30 13:40:55.436286 frat_brain-1.3.6/fRAT/utils/analysis.py
+-rw-r--r--   0        0        0   201570 2023-01-05 15:18:43.590726 frat_brain-1.3.6/fRAT/utils/bootstrap.css
+-rw-r--r--   0        0        0     8001 2023-02-15 18:37:18.803196 frat_brain-1.3.6/fRAT/utils/dash_report.py
+-rw-r--r--   0        0        0     2587 2023-02-14 13:47:31.387338 frat_brain-1.3.6/fRAT/utils/directory_comparison.py
+-rw-r--r--   0        0        0    34582 2023-04-03 14:11:00.889152 frat_brain-1.3.6/fRAT/utils/fRAT_config_setup.py
+-rw-r--r--   0        0        0    36613 2023-04-20 15:50:28.699673 frat_brain-1.3.6/fRAT/utils/figures.py
+-rw-r--r--   0        0        0     6636 2023-01-20 14:35:18.848122 frat_brain-1.3.6/fRAT/utils/html_report.py
+-rw-r--r--   0        0        0     3151 2023-02-15 19:00:37.924453 frat_brain-1.3.6/fRAT/utils/printResults.py
+-rw-r--r--   0        0        0       97 2023-01-05 15:18:43.590957 frat_brain-1.3.6/fRAT/utils/script.js
+-rw-r--r--   0        0        0    50167 2023-03-30 13:20:28.588609 frat_brain-1.3.6/fRAT/utils/statistics.py
+-rw-r--r--   0        0        0    16388 2023-03-14 17:05:44.468988 frat_brain-1.3.6/fRAT/utils/statmap.py
+-rw-r--r--   0        0        0     8967 2023-01-31 14:53:42.200233 frat_brain-1.3.6/fRAT/utils/statmap_config_setup.py
+-rw-r--r--   0        0        0    18883 2023-04-20 10:26:54.263057 frat_brain-1.3.6/fRAT/utils/utils.py
+-rw-r--r--   0        0        0     2390 2023-04-20 16:00:24.878174 frat_brain-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0     5978 1970-01-01 00:00:00.000000 frat_brain-1.3.6/setup.py
+-rw-r--r--   0        0        0     6786 1970-01-01 00:00:00.000000 frat_brain-1.3.6/PKG-INFO
```

### Comparing `frat_brain-1.3.5/LICENSE` & `frat_brain-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/README.md` & `frat_brain-1.3.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -19,37 +19,28 @@
 
 [Installation instructions](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/installation.html)
 
 [ROI analysis tutorial](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/tutorials/Basic-ROI-analysis.html)
 
 ## Reporting bugs
 
-To report a bug, please go to [fRAT's Issues](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/issues/new).
+To report a bug or suggest a new feature, please go to [fRAT's Issues](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/issues/new/choose).
 
 For other questions, issues or discussion please go to [fRAT's Discussions](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/discussions).
 
-## Contributing with development
+## Contributing to the project
 
-The [Fork & Pull Request Workflow](https://docs.github.com/en/get-started/quickstart/contributing-to-projects) is used for contributing. Below is a summary of the necessary steps for this workflow:
-
-1. Fork this repository.
-2. Clone the repository at your machine.
-3. Add your changes in a branch named after the feature (`lower-case-with-hyphens`).
-4. Make a pull request to `fRAT`, targeting the `master` branch.
-
-## Images
-<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/GUI.png?raw=true" title="Example of the fRAT GUI" width=700>
-
-<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/ROI_example.png?raw=true" 
-  title="A region of interest map created using fRAT, showing the mean temporal Signal-to-Noise for each region. Data is displayed in MNI152 standard space and combines data from multiple subjects." 
-width=700>
-
-<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/HTML_report.png?raw=true" title="Example of a HTML report output by fRAT" width=600>
+If you'd like to contribute to the project please read our [contributing guidelines](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/CONTRIBUTING.md). Please also read through our [code of conduct](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/CODE_OF_CONDUCT.md).
 
 ## Versioning
 We use [Semantic versioning](http://semver.org/) for versioning. For the versions available, see the
 [tag list](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/tags) for this project.
 
 ## Licensing
 This project uses the Apache 2.0 license. For the text version of the license see
 [here](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/LICENSE). 
 Prior to version 1.0.0, this project used an MIT license.
+
+## Images
+<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/GUI.png?raw=true" title="Example of the fRAT GUI" width=700>
+
+<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/HTML_report.png?raw=true" title="Example of a HTML report output by fRAT" width=600>
```

### Comparing `frat_brain-1.3.5/fRAT/__main__.py` & `frat_brain-1.3.6/fRAT/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,16 +105,21 @@
     def setup_fonts(self):
         self.default_font = font.Font(font='TkDefaultFont')
         self.important_font = font.Font(font='TkDefaultFont')
         self.heading_font = font.Font(font='TkDefaultFont')
         self.subheading_font = font.Font(font='TkDefaultFont')
 
         self.important_font.configure(weight='bold')
-        self.heading_font.configure(weight='bold', size=20)
-        self.subheading_font.configure(weight='bold', size=18)
+
+        if platform.system() == 'Darwin':
+            self.heading_font.configure(weight='bold', size=20)
+            self.subheading_font.configure(weight='bold', size=18)
+        else:
+            self.heading_font.configure(weight='bold', size=15)
+            self.subheading_font.configure(weight='bold', size=12)
 
     def change_page_specific_settings(self, window):
         statistics_width = "530"
         home_width = "512"
         parsing_width = "450"
 
         if self.page == 'Home':
@@ -716,15 +721,19 @@
         self.widget = widget
         self.widget_type = widget.winfo_class()
         self.tooltip_window = None
         self.id = None
         self.x = self.y = 0
 
         self.font = font.Font(font='TkTooltipFont')
-        self.font.configure(size=12)
+
+        if platform.system() == 'Darwin':
+            self.font.configure(size=12)
+        else:
+            self.font.configure(size=10)
 
     def showtip(self, text):
         "Display text in tooltip window"
         self.text = text
 
         if self.tooltip_window or not self.text:
             return
```

### Comparing `frat_brain-1.3.5/fRAT/configuration_profiles/maps/default_config.toml` & `frat_brain-1.3.6/fRAT/configuration_profiles/maps/default_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/configuration_profiles/maps/statmap_config.toml` & `frat_brain-1.3.6/fRAT/configuration_profiles/maps/statmap_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/configuration_profiles/maps/test_config.toml` & `frat_brain-1.3.6/fRAT/configuration_profiles/maps/test_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/configuration_profiles/roi_analysis/default_config.toml` & `frat_brain-1.3.6/fRAT/configuration_profiles/roi_analysis/default_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml` & `frat_brain-1.3.6/fRAT/configuration_profiles/roi_analysis/fRAT_config.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # General
-run_analysis = true                                                               # true or false. Can skip this step if json files have already been created.
+run_analysis = false                                                              # true or false. Can skip this step if json files have already been created.
 run_statistics = false                                                            # true or false.
-run_plotting = false                                                              # true or false.
+run_plotting = true                                                               # true or false.
 verbose = true                                                                    # true or false.
 verbose_cmd_line_args = false                                                     # true or false.
-multicore_processing = false                                                      # true or false. Use multicore processing during analysis? Multicore processing currently works within participants not between them. Recommended: true
+multicore_processing = true                                                       # true or false. Use multicore processing during analysis? Multicore processing currently works within participants not between them. Recommended: true
 max_core_usage = 'max'                                                            # 'max' to select number of cores available on the system, alternatively an int to manually select number of cores to use. Recommended: 'max' Options: ['max', 6, 5, 4, 3, 2, 1].
 brain_file_loc = ''                                                               # Either the absolute location of brain files or blank, if blank then a browser window will allow you to search for the files at runtime. If passing in this information as a command line flag, this will be ignored.
 report_output_folder = ''                                                         # Either the absolute location of json files or blank, if blank then a browser window will allow you to search for the files at runtime. If passing in this information as a command line flag, this will be ignored.
 averaging_type = 'Participant averaged'                                           # Participant averaged or Session averaged. This setting is used to determine which statistics to use for plotting, and when accessing results (for example through the interactive report).  Note: Histograms will always use the raw results. The linear mixed model from the statistics will always use session averaged data Options: ['Session averaged', 'Participant averaged'].
 parameter_file = 'paramValues.csv'                                                # Recommended: paramValues.csv Name of the file to parse for critical params. Option added to allow quick swapping between different parameter files.
 file_cleanup = 'move'                                                             # Move or delete intermediate files. Options: ['move', 'delete'].
 
 ## Installation testing
 delete_test_folder = 'Never'                                                      # Option to choose whether the folder generated while running tests is deleted upon completion. This only applies when running the full comparison. Options: ['Always', 'If completed without error', 'Never'].
 verbose_errors = true                                                             # true or false. Print all missing files and differences found during testing to the terminal.
 
 # Analysis
 atlas_number = 'HarvardOxford-cort'                                               #  Options: ['Cerebellum-MNIflirt', 'Cerebellum-MNIfnirt', 'HarvardOxford-cort', 'HarvardOxford-sub', 'JHU-ICBM-labels', 'JHU-ICBM-tracts', 'juelich', 'MNI', 'SMATT-labels', 'STN', 'striatum-structural', 'Talairach-labels', 'Thalamus'].
 input_folder_name = 'func_cleaned'                                                # Folder found in each subjects directory containing the files to be analysed. func_cleaned is the default option as this folder will automatically be created when making statmaps. If the "Noise volume included in time series" option was set to true, or motion outlier removal was used when creating the statmaps, this folder will contain cleaned versions of the original func files. However if these options were not used when creating the statmaps, the folder will still be present, however the files will be identical to those in the "func" folder.
-output_folder = 'DEFAULT'                                                         # Directory to save output. If set to DEFAULT, output directory will be set to the cortical atlas used appended with "_ROI_report".  Example: HarvardOxford-Cortical_ROI_report/
+output_folder = 'TEST'                                                            # Directory to save output. If set to DEFAULT, output directory will be set to the cortical atlas used appended with "_ROI_report".  Example: HarvardOxford-Cortical_ROI_report/
 dof = 12                                                                          # Degrees of freedom for FLIRT (only used for the fMRI to anatomical alignment when using Correlation Ratio cost function). Recommended: 12
 anat_align_cost_function = 'BBR'                                                  # BBR or Correlation Ratio. Recommended: BBR. Using BBR (Boundary-Based Registration) requires an FSL FAST segmentation (this will be automatically created if necessary if the Run FSL FAST option is set to "Run if files not found") and a wholehead non-brain extracted anatomical placed in the anat folder. Options: ['BBR', 'Correlation Ratio'].
 grey_matter_segment = true                                                        # true or false. Recommended: true if using a cortical atlas. Note: FSL FAST segmentation files should be placed in the sub-{id}/fslfast/ directory. Only the FSL FAST file appended with pve_1 needs to be in this directory, however if all files output by FAST are placed in this directory, then fRAT will find the necessary file.
-run_fsl_fast = 'Run if files not found'                                           # Recommended: "Run if files not found".  These files will only be searched for (and thus created) if "Use FSL FAST segmentation" is set to true. Options: ['Run if files not found', 'Never run'].
+run_fsl_fast = 'Run if files not found'                                           # Recommended: "Run if files not found". These files will only be searched for (and thus created) if "Use FSL FAST segmentation" is set to true. Options: ['Run if files not found', 'Never run'].
 fslfast_min_prob = 0.1                                                            # Recommended: 0.1
 stat_map_folder = ''                                                              # Folder name which contains the statistical map files. Example: temporalSNR_report
 stat_map_suffix = '_tStd.nii.gz'                                                  # File name suffix of the statistical map files. Include the file extension. Example: _tSNR.img
 conf_level_number = '95%, 1.96'                                                   # Set the confidence level for confidence interval calculations. Numbers represent the confidence level and the corresponding critical z value. Recommended: 95%, 1.96. Options: ['80%, 1.28', '85%, 1.44', '90%, 1.64', '95%, 1.96', '98%, 2.33', '99%, 2.58'].
 binary_params = ['']                                                              # Add parameters here which will either be on or off.
 
 ## Outlier detection
@@ -58,65 +58,65 @@
 main_and_interaction_effects = true                                               # true or false. Note: This option is independent from the other effect calculations.
 interaction_effects = false                                                       # true or false. Note: This option is independent from the other effect calculations.
 
 ## R2 vs voxel count LMM
 max_below_thresh = 0                                                              # Recommended value 0.  For a given ROI, this value sets the maximum percent of sessions that can be excluded (due to having insufficient voxel count) before the ROI is not included in r2 vs voxel count statistics. With the default value of 100(%) an ROI will not be included in this calculation if any sessions have been excluded.
 
 # Parsing
-parameter_dict1 = ['Multiband', 'SENSE']                                          # Comma-separated list of independent variables.  As these critical parameters will also be used when labelling the rows and columns of both the violin plots and histograms, they should be written as you want them to appear in these figures. Note: Leave blank if you do not want to compare between different conditions, for example, if you wish to see the overall tSNR for each region across the entire dataset.
+parameter_dict1 = ['Multiband', 'SENSE']                                          # Comma-separated list of independent variables. The critical parameter settings are used to supply the names and file name abbreviations of the independent variables, therefore `fRAT` supports the use of any parameters (and any number of them). As these critical parameters will also be used when labelling the rows and columns of both the violin plots and histograms, they should be written as you want them to appear in these figures. Note: Leave blank if you do not want to compare between different conditions, for example, if you wish to see the overall tSNR for each region across the entire dataset.
 parameter_dict2 = ['mb', 's']                                                     # Comma-separated list of terms to parse the file name for. Each entry corresponds to a critical parameter above.  Optional if using table parameter verification, however if the file name contains this information it can use this information to auto-detect the critical parameters used for each fMRI volume. Note: This field can be blank.
 make_folder_structure = false                                                     # true or false. Make folder structure when creating paramValues.csv
 parsing_folder = 'func'                                                           # Folder to find files to add to paramValues.csv. If using "Make folder structure" option, this will be the directory the files in the participant folder will be moved to.
 
 # Plotting
 
 ## General plot settings
 plot_dpi = 600                                                                    # Recommended value 600
 plot_font_size = 40                                                               # Recommended value 30
 plot_scale = 10                                                                   # Recommended value 10
-make_violin_plot = true                                                           # true or false.
+make_violin_plot = false                                                          # true or false.
 make_brain_table = true                                                           # true or false.
-make_one_region_fig = true                                                        # true or false.
-make_histogram = true                                                             # true or false.
+make_one_region_fig = false                                                       # true or false.
+make_histogram = false                                                            # true or false.
 colorblind_friendly_plot_colours = ['#ffeda0', '#feb24c', '#fc4e2a', '#bd0026']   # Hex values of colourblind friendly colour scale.
 regional_fig_rois = ['all']                                                       # Provide a comma-separated list of regions to plot e.g. '3, 5', the string 'all' for all rois or the string 'Runtime' to provide regions at runtime.
 
 ## Brain table
 brain_tight_layout = false                                                        # true or false. Use a tight layout when laying out the figure. Recommended: false
 brain_fig_value_min = 0                                                           # Provides the minimum value of the colourbar when creating mean and median images. For example, set minimum to 50 to make areas with values below 50 appear black. Recommended value: 0
 brain_fig_value_max = 'None'                                                      # Provides the maximum value of the colourbar when creating mean and median images. For example, set maximum to 50 to make areas with values above 50 appear as the brighest colour on the colourbar. Recommended value: None. Note: will default to 100 for scaled maps.
 brain_x_coord = -1                                                                # Voxel location to slice the images at in the x axis. Recommended settings for both variables: 91 or 58
 brain_z_coord = 19                                                                # Voxel location to slice the images at in the z axis. Recommended settings for both variables: 91 or 58
-brain_table_col_labels = ''                                                       # Label for columns.
-brain_table_row_labels = ''                                                       # Label for rows.
-brain_table_cols = ''                                                             # 
-brain_table_rows = ''                                                             # 
+brain_table_col_labels = 'Multiband'                                              # Label for columns.
+brain_table_row_labels = 'SENSE'                                                  # Label for rows.
+brain_table_cols = 'Multiband'                                                    # 
+brain_table_rows = 'SENSE'                                                        # 
 
 ## Violin plot
 table_x_label = 'tSNR mean'                                                       # 
 table_y_label = 'ROI'                                                             # 
 violin_show_data = true                                                           # true or false.
 violin_jitter = true                                                              # true or false.
 violin_colour = '#fc4e2a'                                                         # Hex value of colour blind friendly colour. Value taken from colorblind friendly plot colours.
 boxplot_colour = '#feb24c'                                                        # Hex value of colour blind friendly colour. Value taken from colorblind friendly plot colours.
-table_cols = ''                                                                   # 
-table_rows = ''                                                                   # 
+table_cols = 'Multiband'                                                          # 
+table_rows = 'SENSE'                                                              # 
 
 ## Regional bar chart
 single_roi_fig_label_x = 'Multiband factor'                                       # 
 single_roi_fig_label_y = 'temporal Signal to Noise Ratio'                         # 
 single_roi_fig_label_fill = 'SENSE factor'                                        # 
-single_roi_fig_x_axis = ''                                                        # 
-single_roi_fig_colour = ''                                                        # 
+single_roi_fig_x_axis = 'Multiband'                                               # 
+single_roi_fig_colour = 'SENSE'                                                   # 
 
 ## Regional histogram
 histogram_binwidth = 2                                                            # 
 histogram_fig_label_x = 'temporal Signal to Noise Ratio'                          # 
 histogram_fig_label_y = 'Frequency'                                               # 
 histogram_stat_line_size = 1.5                                                    # 
 histogram_show_mean = true                                                        # true or false.
 histogram_show_median = true                                                      # true or false.
 histogram_show_legend = true                                                      # true or false.
-histogram_fig_x_facet = ''                                                        # 
-histogram_fig_y_facet = ''                                                        # 
+histogram_fig_x_facet = 'Multiband'                                               # 
+histogram_fig_y_facet = 'SENSE'                                                   # 
 histogram_fig_colour = '#fc4e2a'                                                  # Hex value of colour blind friendly colour. Value taken from colorblind friendly plot colours.
```

### Comparing `frat_brain-1.3.5/fRAT/configuration_profiles/roi_analysis/test_config.toml` & `frat_brain-1.3.6/fRAT/configuration_profiles/roi_analysis/test_config.toml`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/images/fRAT.gif` & `frat_brain-1.3.6/fRAT/images/fRAT.gif`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/nogui.py` & `frat_brain-1.3.6/fRAT/nogui.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/utils/__pycache__/analysis.cpython-310.pyc` & `frat_brain-1.3.6/fRAT/utils/__pycache__/analysis.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/utils/__pycache__/dash_report.cpython-310.pyc` & `frat_brain-1.3.6/fRAT/utils/__pycache__/dash_report.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc` & `frat_brain-1.3.6/fRAT/utils/__pycache__/directory_comparison.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc` & `frat_brain-1.3.6/fRAT/utils/__pycache__/fRAT_config_setup.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Mar 31 16:31:33 2023 UTC, .py size: 34259 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 e50a 2764 d385 0000  o.........'d....
+00000000: 6f0d 0d0a 0000 0000 74de 2a64 1687 0000  o.......t.*d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0014 0000 0040 0000 0073 8e07 0000 6400  .....@...s....d.
 00000030: 5a00 6700 6401 a201 5a01 0900 6900 6402  Z.g.d...Z...i.d.
 00000040: 6403 6404 6405 6406 6407 6408 9c05 9301  d.d.d.d.d.d.....
 00000050: 6409 6403 6404 6405 640a 640b 6408 9c05  d.d.d.d.d.d.d...
 00000060: 9301 640c 6403 6404 6405 640a 640d 6408  ..d.d.d.d.d.d.d.
 00000070: 9c05 9301 640e 6403 6404 640a 640f 6410  ....d.d.d.d.d.d.
@@ -763,328 +763,341 @@
 00002fa0: 6169 6e5f 616e 645f 696e 7465 7261 6374  ain_and_interact
 00002fb0: 696f 6e5f 6566 6665 6374 735a 1369 6e74  ion_effectsZ.int
 00002fc0: 6572 6163 7469 6f6e 5f65 6666 6563 7473  eraction_effects
 00002fd0: 7a15 5232 2076 7320 766f 7865 6c20 636f  z.R2 vs voxel co
 00002fe0: 756e 7420 4c4d 4d5a 106d 6178 5f62 656c  unt LMMZ.max_bel
 00002ff0: 6f77 5f74 6872 6573 687a 094d 422c 2053  ow_threshz.MB, S
 00003000: 454e 5345 7a13 4372 6974 6963 616c 2070  ENSEz.Critical p
-00003010: 6172 616d 6574 6572 7361 9901 0000 436f  arametersa....Co
+00003010: 6172 616d 6574 6572 7361 5d02 0000 436f  arametersa]...Co
 00003020: 6d6d 612d 7365 7061 7261 7465 6420 6c69  mma-separated li
 00003030: 7374 206f 6620 696e 6465 7065 6e64 656e  st of independen
-00003040: 7420 7661 7269 6162 6c65 732e 200a 4173  t variables. .As
-00003050: 2074 6865 7365 2063 7269 7469 6361 6c20   these critical 
-00003060: 7061 7261 6d65 7465 7273 2077 696c 6c20  parameters will 
-00003070: 616c 736f 2062 6520 7573 6564 2077 6865  also be used whe
-00003080: 6e20 6c61 6265 6c6c 696e 6720 7468 6520  n labelling the 
-00003090: 726f 7773 2061 6e64 2063 6f6c 756d 6e73  rows and columns
-000030a0: 206f 6620 626f 7468 2074 6865 2076 696f   of both the vio
-000030b0: 6c69 6e20 706c 6f74 7320 616e 6420 6869  lin plots and hi
-000030c0: 7374 6f67 7261 6d73 2c20 7468 6579 2073  stograms, they s
-000030d0: 686f 756c 6420 6265 2077 7269 7474 656e  hould be written
-000030e0: 2061 7320 796f 7520 7761 6e74 2074 6865   as you want the
-000030f0: 6d20 746f 2061 7070 6561 7220 696e 2074  m to appear in t
-00003100: 6865 7365 2066 6967 7572 6573 2e0a 4e6f  hese figures..No
-00003110: 7465 3a20 4c65 6176 6520 626c 616e 6b20  te: Leave blank 
-00003120: 6966 2079 6f75 2064 6f20 6e6f 7420 7761  if you do not wa
-00003130: 6e74 2074 6f20 636f 6d70 6172 6520 6265  nt to compare be
-00003140: 7477 6565 6e20 6469 6666 6572 656e 7420  tween different 
-00003150: 636f 6e64 6974 696f 6e73 2c20 666f 7220  conditions, for 
-00003160: 6578 616d 706c 652c 2069 6620 796f 7520  example, if you 
-00003170: 7769 7368 2074 6f20 7365 6520 7468 6520  wish to see the 
-00003180: 6f76 6572 616c 6c20 7453 4e52 2066 6f72  overall tSNR for
-00003190: 2065 6163 6820 7265 6769 6f6e 2061 6372   each region acr
-000031a0: 6f73 7320 7468 6520 656e 7469 7265 2064  oss the entire d
-000031b0: 6174 6173 6574 2e29 0672 0b00 0000 720d  ataset.).r....r.
-000031c0: 0000 0072 0c00 0000 7221 0000 0072 0f00  ...r....r!...r..
-000031d0: 0000 720e 0000 007a 056d 622c 2073 7a1f  ..r....z.mb, sz.
-000031e0: 4372 6974 6963 616c 2070 6172 616d 6574  Critical paramet
-000031f0: 6572 2061 6262 7265 7669 6174 696f 6e61  er abbreviationa
-00003200: 5001 0000 436f 6d6d 612d 7365 7061 7261  P...Comma-separa
-00003210: 7465 6420 6c69 7374 206f 6620 7465 726d  ted list of term
-00003220: 7320 746f 2070 6172 7365 2074 6865 2066  s to parse the f
-00003230: 696c 6520 6e61 6d65 2066 6f72 2e20 4561  ile name for. Ea
-00003240: 6368 2065 6e74 7279 2063 6f72 7265 7370  ch entry corresp
-00003250: 6f6e 6473 2074 6f20 6120 6372 6974 6963  onds to a critic
-00003260: 616c 2070 6172 616d 6574 6572 2061 626f  al parameter abo
-00003270: 7665 2e20 0a4f 7074 696f 6e61 6c20 6966  ve. .Optional if
-00003280: 2075 7369 6e67 2074 6162 6c65 2070 6172   using table par
-00003290: 616d 6574 6572 2076 6572 6966 6963 6174  ameter verificat
-000032a0: 696f 6e2c 2068 6f77 6576 6572 2069 6620  ion, however if 
-000032b0: 7468 6520 6669 6c65 206e 616d 6520 636f  the file name co
-000032c0: 6e74 6169 6e73 2074 6869 7320 696e 666f  ntains this info
-000032d0: 726d 6174 696f 6e20 6974 2063 616e 2075  rmation it can u
-000032e0: 7365 2074 6869 7320 696e 666f 726d 6174  se this informat
-000032f0: 696f 6e20 746f 2061 7574 6f2d 6465 7465  ion to auto-dete
-00003300: 6374 2074 6865 2063 7269 7469 6361 6c20  ct the critical 
-00003310: 7061 7261 6d65 7465 7273 2075 7365 6420  parameters used 
-00003320: 666f 7220 6561 6368 2066 4d52 4920 766f  for each fMRI vo
-00003330: 6c75 6d65 2e0a 4e6f 7465 3a20 5468 6973  lume..Note: This
-00003340: 2066 6965 6c64 2063 616e 2062 6520 626c   field can be bl
-00003350: 616e 6b2e 7a42 7472 7565 206f 7220 6661  ank.zBtrue or fa
-00003360: 6c73 652e 204d 616b 6520 666f 6c64 6572  lse. Make folder
-00003370: 2073 7472 7563 7475 7265 2077 6865 6e20   structure when 
-00003380: 6372 6561 7469 6e67 2070 6172 616d 5661  creating paramVa
-00003390: 6c75 6573 2e63 7376 da04 6675 6e63 7aa9  lues.csv..funcz.
-000033a0: 466f 6c64 6572 2074 6f20 6669 6e64 2066  Folder to find f
-000033b0: 696c 6573 2074 6f20 6164 6420 746f 2070  iles to add to p
-000033c0: 6172 616d 5661 6c75 6573 2e63 7376 2e20  aramValues.csv. 
-000033d0: 4966 2075 7369 6e67 2022 4d61 6b65 2066  If using "Make f
-000033e0: 6f6c 6465 7220 7374 7275 6374 7572 6522  older structure"
-000033f0: 206f 7074 696f 6e2c 2074 6869 7320 7769   option, this wi
-00003400: 6c6c 2062 6520 7468 6520 6469 7265 6374  ll be the direct
-00003410: 6f72 7920 7468 6520 6669 6c65 7320 696e  ory the files in
-00003420: 2074 6865 2070 6172 7469 6369 7061 6e74   the participant
-00003430: 2066 6f6c 6465 7220 7769 6c6c 2062 6520   folder will be 
-00003440: 6d6f 7665 6420 746f 2e29 04da 0f70 6172  moved to.)...par
-00003450: 616d 6574 6572 5f64 6963 7431 da0f 7061  ameter_dict1..pa
-00003460: 7261 6d65 7465 725f 6469 6374 32da 156d  rameter_dict2..m
-00003470: 616b 655f 666f 6c64 6572 5f73 7472 7563  ake_folder_struc
-00003480: 7475 7265 da0e 7061 7273 696e 675f 666f  ture..parsing_fo
-00003490: 6c64 6572 7a15 4765 6e65 7261 6c20 706c  lderz.General pl
-000034a0: 6f74 2073 6574 7469 6e67 735a 0870 6c6f  ot settingsZ.plo
-000034b0: 745f 6470 6969 5802 0000 7a0a 4669 6775  t_dpiiX...z.Figu
-000034c0: 7265 2044 5049 7a15 5265 636f 6d6d 656e  re DPIz.Recommen
-000034d0: 6465 6420 7661 6c75 6520 3630 305a 0e70  ded value 600Z.p
-000034e0: 6c6f 745f 666f 6e74 5f73 697a 65e9 2800  lot_font_size.(.
-000034f0: 0000 7a10 4669 6775 7265 2066 6f6e 7420  ..z.Figure font 
-00003500: 7369 7a65 7a14 5265 636f 6d6d 656e 6465  sizez.Recommende
-00003510: 6420 7661 6c75 6520 3330 5a0a 706c 6f74  d value 30Z.plot
-00003520: 5f73 6361 6c65 e90a 0000 007a 0c46 6967  _scale.....z.Fig
-00003530: 7572 6520 7363 616c 657a 1452 6563 6f6d  ure scalez.Recom
-00003540: 6d65 6e64 6564 2076 616c 7565 2031 305a  mended value 10Z
-00003550: 106d 616b 655f 7669 6f6c 696e 5f70 6c6f  .make_violin_plo
-00003560: 747a 114d 616b 6520 7669 6f6c 696e 2070  tz.Make violin p
-00003570: 6c6f 7473 5a10 6d61 6b65 5f62 7261 696e  lotsZ.make_brain
-00003580: 5f74 6162 6c65 7a19 4d61 6b65 2062 7261  _tablez.Make bra
-00003590: 696e 2076 6973 7561 6c69 7361 7469 6f6e  in visualisation
-000035a0: 735a 136d 616b 655f 6f6e 655f 7265 6769  sZ.make_one_regi
-000035b0: 6f6e 5f66 6967 7a17 4d61 6b65 2072 6567  on_figz.Make reg
-000035c0: 696f 6e61 6c20 6261 7263 6861 7274 735a  ional barchartsZ
-000035d0: 0e6d 616b 655f 6869 7374 6f67 7261 6d7a  .make_histogramz
-000035e0: 184d 616b 6520 7265 6769 6f6e 616c 2068  .Make regional h
-000035f0: 6973 746f 6772 616d 735a 2063 6f6c 6f72  istogramsZ color
-00003600: 626c 696e 645f 6672 6965 6e64 6c79 5f70  blind_friendly_p
-00003610: 6c6f 745f 636f 6c6f 7572 737a 2223 6666  lot_coloursz"#ff
-00003620: 6564 6130 2c20 2366 6562 3234 632c 2023  eda0, #feb24c, #
-00003630: 6663 3465 3261 2c20 2362 6430 3032 367a  fc4e2a, #bd0026z
-00003640: 3048 6578 2076 616c 7565 7320 6f66 2063  0Hex values of c
-00003650: 6f6c 6f75 7262 6c69 6e64 2066 7269 656e  olourblind frien
-00003660: 646c 7920 636f 6c6f 7572 2073 6361 6c65  dly colour scale
-00003670: 2e5a 1172 6567 696f 6e61 6c5f 6669 675f  .Z.regional_fig_
-00003680: 726f 6973 7a0c 524f 4973 2074 6f20 706c  roisz.ROIs to pl
-00003690: 6f74 7a93 5072 6f76 6964 6520 6120 636f  otz.Provide a co
-000036a0: 6d6d 612d 7365 7061 7261 7465 6420 6c69  mma-separated li
-000036b0: 7374 206f 6620 7265 6769 6f6e 7320 746f  st of regions to
-000036c0: 2070 6c6f 7420 652e 672e 2027 332c 2035   plot e.g. '3, 5
-000036d0: 272c 2074 6865 2073 7472 696e 6720 2761  ', the string 'a
-000036e0: 6c6c 2720 666f 7220 616c 6c20 726f 6973  ll' for all rois
-000036f0: 206f 7220 7468 6520 7374 7269 6e67 2027   or the string '
-00003700: 5275 6e74 696d 6527 2074 6f20 7072 6f76  Runtime' to prov
-00003710: 6964 6520 7265 6769 6f6e 7320 6174 2072  ide regions at r
-00003720: 756e 7469 6d65 2e7a 0b42 7261 696e 2074  untime.z.Brain t
-00003730: 6162 6c65 5a12 6272 6169 6e5f 7469 6768  ableZ.brain_tigh
-00003740: 745f 6c61 796f 7574 7a50 7472 7565 206f  t_layoutzPtrue o
-00003750: 7220 6661 6c73 652e 2055 7365 2061 2074  r false. Use a t
-00003760: 6967 6874 206c 6179 6f75 7420 7768 656e  ight layout when
-00003770: 206c 6179 696e 6720 6f75 7420 7468 6520   laying out the 
-00003780: 6669 6775 7265 2e20 5265 636f 6d6d 656e  figure. Recommen
-00003790: 6465 643a 2066 616c 7365 5a13 6272 6169  ded: falseZ.brai
-000037a0: 6e5f 6669 675f 7661 6c75 655f 6d69 6e7a  n_fig_value_minz
-000037b0: 1d4d 696e 696d 756d 206d 6564 6961 6e20  .Minimum median 
-000037c0: 616e 6420 6d65 616e 2076 616c 7565 7ab6  and mean valuez.
-000037d0: 5072 6f76 6964 6573 2074 6865 206d 696e  Provides the min
-000037e0: 696d 756d 2076 616c 7565 206f 6620 7468  imum value of th
-000037f0: 6520 636f 6c6f 7572 6261 7220 7768 656e  e colourbar when
-00003800: 2063 7265 6174 696e 6720 6d65 616e 2061   creating mean a
-00003810: 6e64 206d 6564 6961 6e20 696d 6167 6573  nd median images
-00003820: 2e20 466f 7220 6578 616d 706c 652c 2073  . For example, s
-00003830: 6574 206d 696e 696d 756d 2074 6f20 3530  et minimum to 50
-00003840: 2074 6f20 6d61 6b65 2061 7265 6173 2077   to make areas w
-00003850: 6974 6820 7661 6c75 6573 2062 656c 6f77  ith values below
-00003860: 2035 3020 6170 7065 6172 2062 6c61 636b   50 appear black
-00003870: 2e0a 5265 636f 6d6d 656e 6465 6420 7661  ..Recommended va
-00003880: 6c75 653a 2030 5a13 6272 6169 6e5f 6669  lue: 0Z.brain_fi
-00003890: 675f 7661 6c75 655f 6d61 784e 7a1d 4d61  g_value_maxNz.Ma
-000038a0: 7869 6d75 6d20 6d65 6469 616e 2061 6e64  ximum median and
-000038b0: 206d 6561 6e20 7661 6c75 6561 0701 0000   mean valuea....
-000038c0: 5072 6f76 6964 6573 2074 6865 206d 6178  Provides the max
-000038d0: 696d 756d 2076 616c 7565 206f 6620 7468  imum value of th
-000038e0: 6520 636f 6c6f 7572 6261 7220 7768 656e  e colourbar when
-000038f0: 2063 7265 6174 696e 6720 6d65 616e 2061   creating mean a
-00003900: 6e64 206d 6564 6961 6e20 696d 6167 6573  nd median images
-00003910: 2e20 466f 7220 6578 616d 706c 652c 2073  . For example, s
-00003920: 6574 206d 6178 696d 756d 2074 6f20 3530  et maximum to 50
-00003930: 2074 6f20 6d61 6b65 2061 7265 6173 2077   to make areas w
-00003940: 6974 6820 7661 6c75 6573 2061 626f 7665  ith values above
-00003950: 2035 3020 6170 7065 6172 2061 7320 7468   50 appear as th
-00003960: 6520 6272 6967 6865 7374 2063 6f6c 6f75  e brighest colou
-00003970: 7220 6f6e 2074 6865 2063 6f6c 6f75 7262  r on the colourb
-00003980: 6172 2e0a 5265 636f 6d6d 656e 6465 6420  ar..Recommended 
-00003990: 7661 6c75 653a 204e 6f6e 652e 204e 6f74  value: None. Not
-000039a0: 653a 2077 696c 6c20 6465 6661 756c 7420  e: will default 
-000039b0: 746f 2031 3030 2066 6f72 2073 6361 6c65  to 100 for scale
-000039c0: 6420 6d61 7073 2e5a 0d62 7261 696e 5f78  d maps.Z.brain_x
-000039d0: 5f63 6f6f 7264 e9ff ffff ff7a 6656 6f78  _coord.....zfVox
-000039e0: 656c 206c 6f63 6174 696f 6e20 746f 2073  el location to s
-000039f0: 6c69 6365 2074 6865 2069 6d61 6765 7320  lice the images 
-00003a00: 6174 2069 6e20 7468 6520 7820 6178 6973  at in the x axis
-00003a10: 2e20 5265 636f 6d6d 656e 6465 6420 7365  . Recommended se
-00003a20: 7474 696e 6773 2066 6f72 2062 6f74 6820  ttings for both 
-00003a30: 7661 7269 6162 6c65 733a 2039 3120 6f72  variables: 91 or
-00003a40: 2035 385a 0d62 7261 696e 5f7a 5f63 6f6f   58Z.brain_z_coo
-00003a50: 7264 e913 0000 007a 6656 6f78 656c 206c  rd.....zfVoxel l
-00003a60: 6f63 6174 696f 6e20 746f 2073 6c69 6365  ocation to slice
-00003a70: 2074 6865 2069 6d61 6765 7320 6174 2069   the images at i
-00003a80: 6e20 7468 6520 7a20 6178 6973 2e20 5265  n the z axis. Re
-00003a90: 636f 6d6d 656e 6465 6420 7365 7474 696e  commended settin
-00003aa0: 6773 2066 6f72 2062 6f74 6820 7661 7269  gs for both vari
-00003ab0: 6162 6c65 733a 2039 3120 6f72 2035 38da  ables: 91 or 58.
-00003ac0: 1662 7261 696e 5f74 6162 6c65 5f63 6f6c  .brain_table_col
-00003ad0: 5f6c 6162 656c 737a 1743 4841 4e47 4520  _labelsz.CHANGE 
-00003ae0: 544f 2044 4553 4952 4544 204c 4142 454c  TO DESIRED LABEL
-00003af0: 7a0d 436f 6c75 6d6e 206c 6162 656c 737a  z.Column labelsz
-00003b00: 124c 6162 656c 2066 6f72 2063 6f6c 756d  .Label for colum
-00003b10: 6e73 2e29 0672 0b00 0000 720c 0000 0072  ns.).r....r....r
-00003b20: 2100 0000 720f 0000 0072 6200 0000 720e  !...r....rb...r.
-00003b30: 0000 00da 1662 7261 696e 5f74 6162 6c65  .....brain_table
-00003b40: 5f72 6f77 5f6c 6162 656c 737a 0a52 6f77  _row_labelsz.Row
-00003b50: 206c 6162 656c 737a 0f4c 6162 656c 2066   labelsz.Label f
-00003b60: 6f72 2072 6f77 732e da10 6272 6169 6e5f  or rows...brain_
-00003b70: 7461 626c 655f 636f 6c73 2907 720b 0000  table_cols).r...
-00003b80: 0072 0c00 0000 7220 0000 0072 5200 0000  .r....r ...rR...
-00003b90: 7221 0000 0072 6200 0000 720e 0000 00da  r!...rb...r.....
-00003ba0: 1062 7261 696e 5f74 6162 6c65 5f72 6f77  .brain_table_row
-00003bb0: 737a 0b56 696f 6c69 6e20 706c 6f74 5a0d  sz.Violin plotZ.
-00003bc0: 7461 626c 655f 785f 6c61 6265 6c7a 0974  table_x_labelz.t
-00003bd0: 534e 5220 6d65 616e 5a0d 7461 626c 655f  SNR meanZ.table_
-00003be0: 795f 6c61 6265 6c5a 0352 4f49 5a10 7669  y_labelZ.ROIZ.vi
-00003bf0: 6f6c 696e 5f73 686f 775f 6461 7461 7a10  olin_show_dataz.
-00003c00: 5368 6f77 2064 6174 6120 706f 696e 7473  Show data points
-00003c10: 5a0d 7669 6f6c 696e 5f6a 6974 7465 727a  Z.violin_jitterz
-00003c20: 124a 6974 7465 7220 6461 7461 2070 6f69  .Jitter data poi
-00003c30: 6e74 735a 0d76 696f 6c69 6e5f 636f 6c6f  ntsZ.violin_colo
-00003c40: 7572 7a07 2366 6334 6532 617a 2c50 6c6f  urz.#fc4e2az,Plo
-00003c50: 7474 696e 675b 2263 6f6c 6f72 626c 696e  tting["colorblin
-00003c60: 645f 6672 6965 6e64 6c79 5f70 6c6f 745f  d_friendly_plot_
-00003c70: 636f 6c6f 7572 7322 5d7a 5d48 6578 2076  colours"]z]Hex v
-00003c80: 616c 7565 206f 6620 636f 6c6f 7572 2062  alue of colour b
-00003c90: 6c69 6e64 2066 7269 656e 646c 7920 636f  lind friendly co
-00003ca0: 6c6f 7572 2e20 5661 6c75 6520 7461 6b65  lour. Value take
-00003cb0: 6e20 6672 6f6d 2063 6f6c 6f72 626c 696e  n from colorblin
-00003cc0: 6420 6672 6965 6e64 6c79 2070 6c6f 7420  d friendly plot 
-00003cd0: 636f 6c6f 7572 732e 5a0e 626f 7870 6c6f  colours.Z.boxplo
-00003ce0: 745f 636f 6c6f 7572 7a07 2366 6562 3234  t_colourz.#feb24
-00003cf0: 63da 0a74 6162 6c65 5f63 6f6c 73da 0a74  c..table_cols..t
-00003d00: 6162 6c65 5f72 6f77 737a 1252 6567 696f  able_rowsz.Regio
-00003d10: 6e61 6c20 6261 7220 6368 6172 745a 1673  nal bar chartZ.s
-00003d20: 696e 676c 655f 726f 695f 6669 675f 6c61  ingle_roi_fig_la
-00003d30: 6265 6c5f 787a 104d 756c 7469 6261 6e64  bel_xz.Multiband
-00003d40: 2066 6163 746f 725a 1673 696e 676c 655f   factorZ.single_
-00003d50: 726f 695f 6669 675f 6c61 6265 6c5f 797a  roi_fig_label_yz
-00003d60: 1e74 656d 706f 7261 6c20 5369 676e 616c  .temporal Signal
-00003d70: 2074 6f20 4e6f 6973 6520 5261 7469 6f5a   to Noise RatioZ
-00003d80: 1973 696e 676c 655f 726f 695f 6669 675f  .single_roi_fig_
-00003d90: 6c61 6265 6c5f 6669 6c6c 7a0c 5345 4e53  label_fillz.SENS
-00003da0: 4520 6661 6374 6f72 da15 7369 6e67 6c65  E factor..single
-00003db0: 5f72 6f69 5f66 6967 5f78 5f61 7869 7372  _roi_fig_x_axisr
-00003dc0: 1d00 0000 7a09 4269 6e20 7769 6474 687a  ....z.Bin widthz
-00003dd0: 0c78 2d61 7869 7320 6c61 6265 6cda 0946  .x-axis label..F
-00003de0: 7265 7175 656e 6379 7a0c 792d 6178 6973  requencyz.y-axis
-00003df0: 206c 6162 656c 6700 0000 0000 00f8 3f7a   labelg.......?z
-00003e00: 1353 7461 7469 7374 6963 206c 696e 6520  .Statistic line 
-00003e10: 7369 7a65 7a09 5368 6f77 206d 6561 6e7a  sizez.Show meanz
-00003e20: 0b53 686f 7720 6d65 6469 616e 7a0b 5368  .Show medianz.Sh
-00003e30: 6f77 206c 6567 656e 647a 0c78 2d61 7869  ow legendz.x-axi
-00003e40: 7320 6661 6365 7429 0872 0b00 0000 720c  s facet).r....r.
-00003e50: 0000 0072 0f00 0000 7220 0000 0072 5200  ...r....r ...rR.
-00003e60: 0000 7221 0000 0072 6200 0000 720e 0000  ..r!...rb...r...
-00003e70: 007a 0c79 2d61 7869 7320 6661 6365 747a  .z.y-axis facetz
-00003e80: 0a42 696e 2063 6f6c 6f75 7229 0772 0b00  .Bin colour).r..
-00003e90: 0000 720c 0000 0072 0f00 0000 7220 0000  ..r....r....r ..
-00003ea0: 0072 5200 0000 7221 0000 0072 0e00 0000  .rR...r!...r....
-00003eb0: 290c da15 7369 6e67 6c65 5f72 6f69 5f66  )...single_roi_f
-00003ec0: 6967 5f63 6f6c 6f75 727a 1252 6567 696f  ig_colourz.Regio
-00003ed0: 6e61 6c20 6869 7374 6f67 7261 6d5a 1268  nal histogramZ.h
-00003ee0: 6973 746f 6772 616d 5f62 696e 7769 6474  istogram_binwidt
-00003ef0: 685a 1568 6973 746f 6772 616d 5f66 6967  hZ.histogram_fig
-00003f00: 5f6c 6162 656c 5f78 5a15 6869 7374 6f67  _label_xZ.histog
-00003f10: 7261 6d5f 6669 675f 6c61 6265 6c5f 795a  ram_fig_label_yZ
-00003f20: 1868 6973 746f 6772 616d 5f73 7461 745f  .histogram_stat_
-00003f30: 6c69 6e65 5f73 697a 655a 1368 6973 746f  line_sizeZ.histo
-00003f40: 6772 616d 5f73 686f 775f 6d65 616e 5a15  gram_show_meanZ.
-00003f50: 6869 7374 6f67 7261 6d5f 7368 6f77 5f6d  histogram_show_m
-00003f60: 6564 6961 6e5a 1568 6973 746f 6772 616d  edianZ.histogram
-00003f70: 5f73 686f 775f 6c65 6765 6e64 da15 6869  _show_legend..hi
-00003f80: 7374 6f67 7261 6d5f 6669 675f 785f 6661  stogram_fig_x_fa
-00003f90: 6365 74da 1568 6973 746f 6772 616d 5f66  cet..histogram_f
-00003fa0: 6967 5f79 5f66 6163 6574 5a14 6869 7374  ig_y_facetZ.hist
-00003fb0: 6f67 7261 6d5f 6669 675f 636f 6c6f 7572  ogram_fig_colour
-00003fc0: 2907 da07 5f5f 646f 635f 5fda 0570 6167  )...__doc__..pag
-00003fd0: 6573 7202 0000 0072 0300 0000 7204 0000  esr....r....r...
-00003fe0: 0072 0500 0000 7206 0000 00a9 0072 7900  .r....r......ry.
-00003ff0: 0000 7279 0000 00fa 5c2f 5573 6572 732f  ..ry....\/Users/
-00004000: 6c70 7865 6831 302f 446f 6375 6d65 6e74  lpxeh10/Document
-00004010: 732f 5265 706f 7369 746f 7269 6573 2f66  s/Repositories/f
-00004020: 4d52 495f 524f 495f 616e 616c 7973 6973  MRI_ROI_analysis
-00004030: 5f74 6f6f 6c2f 6652 4154 2f75 7469 6c73  _tool/fRAT/utils
-00004040: 2f66 5241 545f 636f 6e66 6967 5f73 6574  /fRAT_config_set
-00004050: 7570 2e70 79da 083c 6d6f 6475 6c65 3e01  up.py..<module>.
-00004060: 0000 0073 b803 0000 0400 0801 0202 0201  ...s............
-00004070: 0601 0201 0201 0201 04fd 02ff 0606 0201  ................
-00004080: 0401 04fe 02fa 060a 0201 0401 04fe 02f6  ................
-00004090: 060e 0401 04ff 02f2 0611 0401 04ff 02ef  ................
-000040a0: 0614 0201 04ff 02ec 0c17 0201 0201 04fe  ................
-000040b0: 02e9 081b 0201 0201 04fe 02e5 081f 0201  ................
-000040c0: 0201 04fe 02e1 0423 0201 0601 0201 0201  .......#........
-000040d0: 04fc 02dd 082d 0201 04ff 02d3 0e32 0401  .....-.......2..
-000040e0: 04ff 02ce 0835 02cb 0a37 0201 04ff 02c9  .....5...7......
-000040f0: 043a 0201 0601 0201 0201 04fc 02c6 0641  .:.............A
-00004100: 0201 04ff 04bf 0246 0201 0a01 0601 020f  .......F........
-00004110: 04f0 02ff 0813 0201 04ff 02ed 0a1d 0201  ................
-00004120: 04ff 02e3 0822 0201 04ff 02de 0426 0201  .....".......&..
-00004130: 0201 0601 0201 0201 04fb 02da 0432 0401  .............2..
-00004140: 0201 04fe 02ce 043a 0601 0201 0201 0202  .......:........
-00004150: 0201 04fa 02c6 0c42 0401 04ff 02be 0845  .......B.......E
-00004160: 0201 0201 0201 04fd 02bb 084b 0201 0201  ...........K....
-00004170: 0201 04fd 02b5 0654 0601 0401 0201 04fd  .......T........
-00004180: 02ac 0a5b 0401 0401 04fe 02a5 085f 02a1  ...[........._..
-00004190: 0661 0201 04ff 029f 0668 0201 0201 04fe  .a.......h......
-000041a0: 0298 0c6d 0201 0201 04fe 0293 0672 0601  ...m.........r..
-000041b0: 0401 0201 04fd 048e 027a 0201 0801 0201  .........z......
-000041c0: 0201 04fe 02ff 0407 0201 0201 04fe 02f9  ................
-000041d0: 040f 0201 0201 0201 04fd 02f1 0614 0201  ................
-000041e0: 0201 04fe 02ec 0419 0201 0201 04fe 02e7  ................
-000041f0: 0624 0201 04ff 02dc 0629 0201 04ff 02d7  .$.......)......
-00004200: 082e 0201 0201 04fe 02d2 0633 0201 0201  ...........3....
-00004210: 0201 0201 0201 04fb 02cd 063d 0201 0201  ...........=....
-00004220: 0203 04fb 02c3 0844 02bc 0646 0201 0201  .......D...F....
-00004230: 04fe 02ba 064a 0201 0a01 0601 0201 04fc  .....J..........
-00004240: 02b6 085a 02a6 065c 0201 0201 04fe 02a4  ...Z...\........
-00004250: 0a60 0201 0201 0201 04fd 02a0 0465 0201  .`...........e..
-00004260: 0201 0201 04fd 029b 026b 0201 0201 0201  .........k......
-00004270: 04fd 0206 0201 0201 0201 04fd 0606 0602  ................
-00004280: 0201 04ff 0887 007f 0203 0202 0201 0601  ................
-00004290: 0201 04fd 020b 0201 0401 0201 0201 04fc  ................
-000042a0: 040b 0201 04ff 0603 0201 04ff 06e6 0220  ............... 
-000042b0: 0201 0801 02ff 0803 0201 04ff 02fd 0806  ................
-000042c0: 0201 04ff 02fa 0809 0201 04ff 02f7 080c  ................
-000042d0: 0201 04ff 02f4 080f 0201 04ff 02f1 0812  ................
-000042e0: 0201 04ff 02ee 0815 0201 04ff 02eb 0618  ................
-000042f0: 0201 0201 04fe 02e8 0a1c 0201 04ff 02e4  ................
-00004300: 0820 02e0 0622 0201 04ff 02de 0825 0201  . ...".......%..
-00004310: 04ff 02db 082b 0201 04ff 02d5 0631 0201  .....+.......1..
-00004320: 04ff 02cf 0a35 0401 04ff 02cb 0c39 0401  .....5.......9..
-00004330: 0601 06fe 04c7 0c3d 0401 0601 06fe 02c3  .......=........
-00004340: 0a41 0401 0401 06fe 02bf 0a45 0401 0401  .A.........E....
-00004350: 06fe 02bb 0a49 02b7 0c4b 0201 04ff 02b5  .....I...K......
-00004360: 0c4e 0201 04ff 02b2 0c51 0201 04ff 02af  .N.......Q......
-00004370: 0c54 0201 04ff 02ac 0a57 0401 0401 0401  .T.......W......
-00004380: 04fd 02a9 0a5c 0401 0401 0401 04fd 02a4  .....\..........
-00004390: 0a61 0601 0201 06fe 029f 0a65 0601 0201  .a.........e....
-000043a0: 06fe 029b 0a69 0297 0c6b 0201 04ff 0295  .....i...k......
-000043b0: 0c6e 0201 04ff 0292 0c71 0201 04ff 028f  .n.......q......
-000043c0: 0a74 0601 0201 06fe 048c 0678 0601 0201  .t.........x....
-000043d0: 06fe 0604 1002 0602 0601 0201 04fe 0604  ................
-000043e0: 0601 0201 04fe 0a04 0201 04ff 0803 0201  ................
-000043f0: 04ff 0803 0201 04ff 0803 0201 04ff 0803  ................
-00004400: 0201 0601 0201 06fd 0805 0201 0401 0401  ................
-00004410: 06fd 0a05 0401 0401 0401 06fd 0081 0ee1  ................
+00003040: 7420 7661 7269 6162 6c65 732e 0a54 6865  t variables..The
+00003050: 2063 7269 7469 6361 6c20 7061 7261 6d65   critical parame
+00003060: 7465 7220 7365 7474 696e 6773 2061 7265  ter settings are
+00003070: 2075 7365 6420 746f 2073 7570 706c 7920   used to supply 
+00003080: 7468 6520 6e61 6d65 7320 616e 6420 6669  the names and fi
+00003090: 6c65 206e 616d 6520 6162 6272 6576 6961  le name abbrevia
+000030a0: 7469 6f6e 7320 6f66 2074 6865 2069 6e64  tions of the ind
+000030b0: 6570 656e 6465 6e74 2076 6172 6961 626c  ependent variabl
+000030c0: 6573 2c20 7468 6572 6566 6f72 6520 6066  es, therefore `f
+000030d0: 5241 5460 2073 7570 706f 7274 7320 7468  RAT` supports th
+000030e0: 6520 7573 6520 6f66 2061 6e79 2070 6172  e use of any par
+000030f0: 616d 6574 6572 7320 2861 6e64 2061 6e79  ameters (and any
+00003100: 206e 756d 6265 7220 6f66 2074 6865 6d29   number of them)
+00003110: 2e0a 4173 2074 6865 7365 2063 7269 7469  ..As these criti
+00003120: 6361 6c20 7061 7261 6d65 7465 7273 2077  cal parameters w
+00003130: 696c 6c20 616c 736f 2062 6520 7573 6564  ill also be used
+00003140: 2077 6865 6e20 6c61 6265 6c6c 696e 6720   when labelling 
+00003150: 7468 6520 726f 7773 2061 6e64 2063 6f6c  the rows and col
+00003160: 756d 6e73 206f 6620 626f 7468 2074 6865  umns of both the
+00003170: 2076 696f 6c69 6e20 706c 6f74 7320 616e   violin plots an
+00003180: 6420 6869 7374 6f67 7261 6d73 2c20 7468  d histograms, th
+00003190: 6579 2073 686f 756c 6420 6265 2077 7269  ey should be wri
+000031a0: 7474 656e 2061 7320 796f 7520 7761 6e74  tten as you want
+000031b0: 2074 6865 6d20 746f 2061 7070 6561 7220   them to appear 
+000031c0: 696e 2074 6865 7365 2066 6967 7572 6573  in these figures
+000031d0: 2e0a 4e6f 7465 3a20 4c65 6176 6520 626c  ..Note: Leave bl
+000031e0: 616e 6b20 6966 2079 6f75 2064 6f20 6e6f  ank if you do no
+000031f0: 7420 7761 6e74 2074 6f20 636f 6d70 6172  t want to compar
+00003200: 6520 6265 7477 6565 6e20 6469 6666 6572  e between differ
+00003210: 656e 7420 636f 6e64 6974 696f 6e73 2c20  ent conditions, 
+00003220: 666f 7220 6578 616d 706c 652c 2069 6620  for example, if 
+00003230: 796f 7520 7769 7368 2074 6f20 7365 6520  you wish to see 
+00003240: 7468 6520 6f76 6572 616c 6c20 7453 4e52  the overall tSNR
+00003250: 2066 6f72 2065 6163 6820 7265 6769 6f6e   for each region
+00003260: 2061 6372 6f73 7320 7468 6520 656e 7469   across the enti
+00003270: 7265 2064 6174 6173 6574 2e29 0672 0b00  re dataset.).r..
+00003280: 0000 720d 0000 0072 0c00 0000 7221 0000  ..r....r....r!..
+00003290: 0072 0f00 0000 720e 0000 007a 056d 622c  .r....r....z.mb,
+000032a0: 2073 7a1f 4372 6974 6963 616c 2070 6172   sz.Critical par
+000032b0: 616d 6574 6572 2061 6262 7265 7669 6174  ameter abbreviat
+000032c0: 696f 6e61 5001 0000 436f 6d6d 612d 7365  ionaP...Comma-se
+000032d0: 7061 7261 7465 6420 6c69 7374 206f 6620  parated list of 
+000032e0: 7465 726d 7320 746f 2070 6172 7365 2074  terms to parse t
+000032f0: 6865 2066 696c 6520 6e61 6d65 2066 6f72  he file name for
+00003300: 2e20 4561 6368 2065 6e74 7279 2063 6f72  . Each entry cor
+00003310: 7265 7370 6f6e 6473 2074 6f20 6120 6372  responds to a cr
+00003320: 6974 6963 616c 2070 6172 616d 6574 6572  itical parameter
+00003330: 2061 626f 7665 2e20 0a4f 7074 696f 6e61   above. .Optiona
+00003340: 6c20 6966 2075 7369 6e67 2074 6162 6c65  l if using table
+00003350: 2070 6172 616d 6574 6572 2076 6572 6966   parameter verif
+00003360: 6963 6174 696f 6e2c 2068 6f77 6576 6572  ication, however
+00003370: 2069 6620 7468 6520 6669 6c65 206e 616d   if the file nam
+00003380: 6520 636f 6e74 6169 6e73 2074 6869 7320  e contains this 
+00003390: 696e 666f 726d 6174 696f 6e20 6974 2063  information it c
+000033a0: 616e 2075 7365 2074 6869 7320 696e 666f  an use this info
+000033b0: 726d 6174 696f 6e20 746f 2061 7574 6f2d  rmation to auto-
+000033c0: 6465 7465 6374 2074 6865 2063 7269 7469  detect the criti
+000033d0: 6361 6c20 7061 7261 6d65 7465 7273 2075  cal parameters u
+000033e0: 7365 6420 666f 7220 6561 6368 2066 4d52  sed for each fMR
+000033f0: 4920 766f 6c75 6d65 2e0a 4e6f 7465 3a20  I volume..Note: 
+00003400: 5468 6973 2066 6965 6c64 2063 616e 2062  This field can b
+00003410: 6520 626c 616e 6b2e 7a42 7472 7565 206f  e blank.zBtrue o
+00003420: 7220 6661 6c73 652e 204d 616b 6520 666f  r false. Make fo
+00003430: 6c64 6572 2073 7472 7563 7475 7265 2077  lder structure w
+00003440: 6865 6e20 6372 6561 7469 6e67 2070 6172  hen creating par
+00003450: 616d 5661 6c75 6573 2e63 7376 da04 6675  amValues.csv..fu
+00003460: 6e63 7aa9 466f 6c64 6572 2074 6f20 6669  ncz.Folder to fi
+00003470: 6e64 2066 696c 6573 2074 6f20 6164 6420  nd files to add 
+00003480: 746f 2070 6172 616d 5661 6c75 6573 2e63  to paramValues.c
+00003490: 7376 2e20 4966 2075 7369 6e67 2022 4d61  sv. If using "Ma
+000034a0: 6b65 2066 6f6c 6465 7220 7374 7275 6374  ke folder struct
+000034b0: 7572 6522 206f 7074 696f 6e2c 2074 6869  ure" option, thi
+000034c0: 7320 7769 6c6c 2062 6520 7468 6520 6469  s will be the di
+000034d0: 7265 6374 6f72 7920 7468 6520 6669 6c65  rectory the file
+000034e0: 7320 696e 2074 6865 2070 6172 7469 6369  s in the partici
+000034f0: 7061 6e74 2066 6f6c 6465 7220 7769 6c6c  pant folder will
+00003500: 2062 6520 6d6f 7665 6420 746f 2e29 04da   be moved to.)..
+00003510: 0f70 6172 616d 6574 6572 5f64 6963 7431  .parameter_dict1
+00003520: da0f 7061 7261 6d65 7465 725f 6469 6374  ..parameter_dict
+00003530: 32da 156d 616b 655f 666f 6c64 6572 5f73  2..make_folder_s
+00003540: 7472 7563 7475 7265 da0e 7061 7273 696e  tructure..parsin
+00003550: 675f 666f 6c64 6572 7a15 4765 6e65 7261  g_folderz.Genera
+00003560: 6c20 706c 6f74 2073 6574 7469 6e67 735a  l plot settingsZ
+00003570: 0870 6c6f 745f 6470 6969 5802 0000 7a0a  .plot_dpiiX...z.
+00003580: 4669 6775 7265 2044 5049 7a15 5265 636f  Figure DPIz.Reco
+00003590: 6d6d 656e 6465 6420 7661 6c75 6520 3630  mmended value 60
+000035a0: 305a 0e70 6c6f 745f 666f 6e74 5f73 697a  0Z.plot_font_siz
+000035b0: 65e9 2800 0000 7a10 4669 6775 7265 2066  e.(...z.Figure f
+000035c0: 6f6e 7420 7369 7a65 7a14 5265 636f 6d6d  ont sizez.Recomm
+000035d0: 656e 6465 6420 7661 6c75 6520 3330 5a0a  ended value 30Z.
+000035e0: 706c 6f74 5f73 6361 6c65 e90a 0000 007a  plot_scale.....z
+000035f0: 0c46 6967 7572 6520 7363 616c 657a 1452  .Figure scalez.R
+00003600: 6563 6f6d 6d65 6e64 6564 2076 616c 7565  ecommended value
+00003610: 2031 305a 106d 616b 655f 7669 6f6c 696e   10Z.make_violin
+00003620: 5f70 6c6f 747a 114d 616b 6520 7669 6f6c  _plotz.Make viol
+00003630: 696e 2070 6c6f 7473 5a10 6d61 6b65 5f62  in plotsZ.make_b
+00003640: 7261 696e 5f74 6162 6c65 7a19 4d61 6b65  rain_tablez.Make
+00003650: 2062 7261 696e 2076 6973 7561 6c69 7361   brain visualisa
+00003660: 7469 6f6e 735a 136d 616b 655f 6f6e 655f  tionsZ.make_one_
+00003670: 7265 6769 6f6e 5f66 6967 7a17 4d61 6b65  region_figz.Make
+00003680: 2072 6567 696f 6e61 6c20 6261 7263 6861   regional barcha
+00003690: 7274 735a 0e6d 616b 655f 6869 7374 6f67  rtsZ.make_histog
+000036a0: 7261 6d7a 184d 616b 6520 7265 6769 6f6e  ramz.Make region
+000036b0: 616c 2068 6973 746f 6772 616d 735a 2063  al histogramsZ c
+000036c0: 6f6c 6f72 626c 696e 645f 6672 6965 6e64  olorblind_friend
+000036d0: 6c79 5f70 6c6f 745f 636f 6c6f 7572 737a  ly_plot_coloursz
+000036e0: 2223 6666 6564 6130 2c20 2366 6562 3234  "#ffeda0, #feb24
+000036f0: 632c 2023 6663 3465 3261 2c20 2362 6430  c, #fc4e2a, #bd0
+00003700: 3032 367a 3048 6578 2076 616c 7565 7320  026z0Hex values 
+00003710: 6f66 2063 6f6c 6f75 7262 6c69 6e64 2066  of colourblind f
+00003720: 7269 656e 646c 7920 636f 6c6f 7572 2073  riendly colour s
+00003730: 6361 6c65 2e5a 1172 6567 696f 6e61 6c5f  cale.Z.regional_
+00003740: 6669 675f 726f 6973 7a0c 524f 4973 2074  fig_roisz.ROIs t
+00003750: 6f20 706c 6f74 7a93 5072 6f76 6964 6520  o plotz.Provide 
+00003760: 6120 636f 6d6d 612d 7365 7061 7261 7465  a comma-separate
+00003770: 6420 6c69 7374 206f 6620 7265 6769 6f6e  d list of region
+00003780: 7320 746f 2070 6c6f 7420 652e 672e 2027  s to plot e.g. '
+00003790: 332c 2035 272c 2074 6865 2073 7472 696e  3, 5', the strin
+000037a0: 6720 2761 6c6c 2720 666f 7220 616c 6c20  g 'all' for all 
+000037b0: 726f 6973 206f 7220 7468 6520 7374 7269  rois or the stri
+000037c0: 6e67 2027 5275 6e74 696d 6527 2074 6f20  ng 'Runtime' to 
+000037d0: 7072 6f76 6964 6520 7265 6769 6f6e 7320  provide regions 
+000037e0: 6174 2072 756e 7469 6d65 2e7a 0b42 7261  at runtime.z.Bra
+000037f0: 696e 2074 6162 6c65 5a12 6272 6169 6e5f  in tableZ.brain_
+00003800: 7469 6768 745f 6c61 796f 7574 7a50 7472  tight_layoutzPtr
+00003810: 7565 206f 7220 6661 6c73 652e 2055 7365  ue or false. Use
+00003820: 2061 2074 6967 6874 206c 6179 6f75 7420   a tight layout 
+00003830: 7768 656e 206c 6179 696e 6720 6f75 7420  when laying out 
+00003840: 7468 6520 6669 6775 7265 2e20 5265 636f  the figure. Reco
+00003850: 6d6d 656e 6465 643a 2066 616c 7365 5a13  mmended: falseZ.
+00003860: 6272 6169 6e5f 6669 675f 7661 6c75 655f  brain_fig_value_
+00003870: 6d69 6e7a 1d4d 696e 696d 756d 206d 6564  minz.Minimum med
+00003880: 6961 6e20 616e 6420 6d65 616e 2076 616c  ian and mean val
+00003890: 7565 7ab6 5072 6f76 6964 6573 2074 6865  uez.Provides the
+000038a0: 206d 696e 696d 756d 2076 616c 7565 206f   minimum value o
+000038b0: 6620 7468 6520 636f 6c6f 7572 6261 7220  f the colourbar 
+000038c0: 7768 656e 2063 7265 6174 696e 6720 6d65  when creating me
+000038d0: 616e 2061 6e64 206d 6564 6961 6e20 696d  an and median im
+000038e0: 6167 6573 2e20 466f 7220 6578 616d 706c  ages. For exampl
+000038f0: 652c 2073 6574 206d 696e 696d 756d 2074  e, set minimum t
+00003900: 6f20 3530 2074 6f20 6d61 6b65 2061 7265  o 50 to make are
+00003910: 6173 2077 6974 6820 7661 6c75 6573 2062  as with values b
+00003920: 656c 6f77 2035 3020 6170 7065 6172 2062  elow 50 appear b
+00003930: 6c61 636b 2e0a 5265 636f 6d6d 656e 6465  lack..Recommende
+00003940: 6420 7661 6c75 653a 2030 5a13 6272 6169  d value: 0Z.brai
+00003950: 6e5f 6669 675f 7661 6c75 655f 6d61 784e  n_fig_value_maxN
+00003960: 7a1d 4d61 7869 6d75 6d20 6d65 6469 616e  z.Maximum median
+00003970: 2061 6e64 206d 6561 6e20 7661 6c75 6561   and mean valuea
+00003980: 0701 0000 5072 6f76 6964 6573 2074 6865  ....Provides the
+00003990: 206d 6178 696d 756d 2076 616c 7565 206f   maximum value o
+000039a0: 6620 7468 6520 636f 6c6f 7572 6261 7220  f the colourbar 
+000039b0: 7768 656e 2063 7265 6174 696e 6720 6d65  when creating me
+000039c0: 616e 2061 6e64 206d 6564 6961 6e20 696d  an and median im
+000039d0: 6167 6573 2e20 466f 7220 6578 616d 706c  ages. For exampl
+000039e0: 652c 2073 6574 206d 6178 696d 756d 2074  e, set maximum t
+000039f0: 6f20 3530 2074 6f20 6d61 6b65 2061 7265  o 50 to make are
+00003a00: 6173 2077 6974 6820 7661 6c75 6573 2061  as with values a
+00003a10: 626f 7665 2035 3020 6170 7065 6172 2061  bove 50 appear a
+00003a20: 7320 7468 6520 6272 6967 6865 7374 2063  s the brighest c
+00003a30: 6f6c 6f75 7220 6f6e 2074 6865 2063 6f6c  olour on the col
+00003a40: 6f75 7262 6172 2e0a 5265 636f 6d6d 656e  ourbar..Recommen
+00003a50: 6465 6420 7661 6c75 653a 204e 6f6e 652e  ded value: None.
+00003a60: 204e 6f74 653a 2077 696c 6c20 6465 6661   Note: will defa
+00003a70: 756c 7420 746f 2031 3030 2066 6f72 2073  ult to 100 for s
+00003a80: 6361 6c65 6420 6d61 7073 2e5a 0d62 7261  caled maps.Z.bra
+00003a90: 696e 5f78 5f63 6f6f 7264 e9ff ffff ff7a  in_x_coord.....z
+00003aa0: 6656 6f78 656c 206c 6f63 6174 696f 6e20  fVoxel location 
+00003ab0: 746f 2073 6c69 6365 2074 6865 2069 6d61  to slice the ima
+00003ac0: 6765 7320 6174 2069 6e20 7468 6520 7820  ges at in the x 
+00003ad0: 6178 6973 2e20 5265 636f 6d6d 656e 6465  axis. Recommende
+00003ae0: 6420 7365 7474 696e 6773 2066 6f72 2062  d settings for b
+00003af0: 6f74 6820 7661 7269 6162 6c65 733a 2039  oth variables: 9
+00003b00: 3120 6f72 2035 385a 0d62 7261 696e 5f7a  1 or 58Z.brain_z
+00003b10: 5f63 6f6f 7264 e913 0000 007a 6656 6f78  _coord.....zfVox
+00003b20: 656c 206c 6f63 6174 696f 6e20 746f 2073  el location to s
+00003b30: 6c69 6365 2074 6865 2069 6d61 6765 7320  lice the images 
+00003b40: 6174 2069 6e20 7468 6520 7a20 6178 6973  at in the z axis
+00003b50: 2e20 5265 636f 6d6d 656e 6465 6420 7365  . Recommended se
+00003b60: 7474 696e 6773 2066 6f72 2062 6f74 6820  ttings for both 
+00003b70: 7661 7269 6162 6c65 733a 2039 3120 6f72  variables: 91 or
+00003b80: 2035 38da 1662 7261 696e 5f74 6162 6c65   58..brain_table
+00003b90: 5f63 6f6c 5f6c 6162 656c 737a 1743 4841  _col_labelsz.CHA
+00003ba0: 4e47 4520 544f 2044 4553 4952 4544 204c  NGE TO DESIRED L
+00003bb0: 4142 454c 7a0d 436f 6c75 6d6e 206c 6162  ABELz.Column lab
+00003bc0: 656c 737a 124c 6162 656c 2066 6f72 2063  elsz.Label for c
+00003bd0: 6f6c 756d 6e73 2e29 0672 0b00 0000 720c  olumns.).r....r.
+00003be0: 0000 0072 2100 0000 720f 0000 0072 6200  ...r!...r....rb.
+00003bf0: 0000 720e 0000 00da 1662 7261 696e 5f74  ..r......brain_t
+00003c00: 6162 6c65 5f72 6f77 5f6c 6162 656c 737a  able_row_labelsz
+00003c10: 0a52 6f77 206c 6162 656c 737a 0f4c 6162  .Row labelsz.Lab
+00003c20: 656c 2066 6f72 2072 6f77 732e da10 6272  el for rows...br
+00003c30: 6169 6e5f 7461 626c 655f 636f 6c73 2907  ain_table_cols).
+00003c40: 720b 0000 0072 0c00 0000 7220 0000 0072  r....r....r ...r
+00003c50: 5200 0000 7221 0000 0072 6200 0000 720e  R...r!...rb...r.
+00003c60: 0000 00da 1062 7261 696e 5f74 6162 6c65  .....brain_table
+00003c70: 5f72 6f77 737a 0b56 696f 6c69 6e20 706c  _rowsz.Violin pl
+00003c80: 6f74 5a0d 7461 626c 655f 785f 6c61 6265  otZ.table_x_labe
+00003c90: 6c7a 0974 534e 5220 6d65 616e 5a0d 7461  lz.tSNR meanZ.ta
+00003ca0: 626c 655f 795f 6c61 6265 6c5a 0352 4f49  ble_y_labelZ.ROI
+00003cb0: 5a10 7669 6f6c 696e 5f73 686f 775f 6461  Z.violin_show_da
+00003cc0: 7461 7a10 5368 6f77 2064 6174 6120 706f  taz.Show data po
+00003cd0: 696e 7473 5a0d 7669 6f6c 696e 5f6a 6974  intsZ.violin_jit
+00003ce0: 7465 727a 124a 6974 7465 7220 6461 7461  terz.Jitter data
+00003cf0: 2070 6f69 6e74 735a 0d76 696f 6c69 6e5f   pointsZ.violin_
+00003d00: 636f 6c6f 7572 7a07 2366 6334 6532 617a  colourz.#fc4e2az
+00003d10: 2c50 6c6f 7474 696e 675b 2263 6f6c 6f72  ,Plotting["color
+00003d20: 626c 696e 645f 6672 6965 6e64 6c79 5f70  blind_friendly_p
+00003d30: 6c6f 745f 636f 6c6f 7572 7322 5d7a 5d48  lot_colours"]z]H
+00003d40: 6578 2076 616c 7565 206f 6620 636f 6c6f  ex value of colo
+00003d50: 7572 2062 6c69 6e64 2066 7269 656e 646c  ur blind friendl
+00003d60: 7920 636f 6c6f 7572 2e20 5661 6c75 6520  y colour. Value 
+00003d70: 7461 6b65 6e20 6672 6f6d 2063 6f6c 6f72  taken from color
+00003d80: 626c 696e 6420 6672 6965 6e64 6c79 2070  blind friendly p
+00003d90: 6c6f 7420 636f 6c6f 7572 732e 5a0e 626f  lot colours.Z.bo
+00003da0: 7870 6c6f 745f 636f 6c6f 7572 7a07 2366  xplot_colourz.#f
+00003db0: 6562 3234 63da 0a74 6162 6c65 5f63 6f6c  eb24c..table_col
+00003dc0: 73da 0a74 6162 6c65 5f72 6f77 737a 1252  s..table_rowsz.R
+00003dd0: 6567 696f 6e61 6c20 6261 7220 6368 6172  egional bar char
+00003de0: 745a 1673 696e 676c 655f 726f 695f 6669  tZ.single_roi_fi
+00003df0: 675f 6c61 6265 6c5f 787a 104d 756c 7469  g_label_xz.Multi
+00003e00: 6261 6e64 2066 6163 746f 725a 1673 696e  band factorZ.sin
+00003e10: 676c 655f 726f 695f 6669 675f 6c61 6265  gle_roi_fig_labe
+00003e20: 6c5f 797a 1e74 656d 706f 7261 6c20 5369  l_yz.temporal Si
+00003e30: 676e 616c 2074 6f20 4e6f 6973 6520 5261  gnal to Noise Ra
+00003e40: 7469 6f5a 1973 696e 676c 655f 726f 695f  tioZ.single_roi_
+00003e50: 6669 675f 6c61 6265 6c5f 6669 6c6c 7a0c  fig_label_fillz.
+00003e60: 5345 4e53 4520 6661 6374 6f72 da15 7369  SENSE factor..si
+00003e70: 6e67 6c65 5f72 6f69 5f66 6967 5f78 5f61  ngle_roi_fig_x_a
+00003e80: 7869 7372 1d00 0000 7a09 4269 6e20 7769  xisr....z.Bin wi
+00003e90: 6474 687a 0c78 2d61 7869 7320 6c61 6265  dthz.x-axis labe
+00003ea0: 6cda 0946 7265 7175 656e 6379 7a0c 792d  l..Frequencyz.y-
+00003eb0: 6178 6973 206c 6162 656c 6700 0000 0000  axis labelg.....
+00003ec0: 00f8 3f7a 1353 7461 7469 7374 6963 206c  ..?z.Statistic l
+00003ed0: 696e 6520 7369 7a65 7a09 5368 6f77 206d  ine sizez.Show m
+00003ee0: 6561 6e7a 0b53 686f 7720 6d65 6469 616e  eanz.Show median
+00003ef0: 7a0b 5368 6f77 206c 6567 656e 647a 0c78  z.Show legendz.x
+00003f00: 2d61 7869 7320 6661 6365 7429 0872 0b00  -axis facet).r..
+00003f10: 0000 720c 0000 0072 0f00 0000 7220 0000  ..r....r....r ..
+00003f20: 0072 5200 0000 7221 0000 0072 6200 0000  .rR...r!...rb...
+00003f30: 720e 0000 007a 0c79 2d61 7869 7320 6661  r....z.y-axis fa
+00003f40: 6365 747a 0a42 696e 2063 6f6c 6f75 7229  cetz.Bin colour)
+00003f50: 0772 0b00 0000 720c 0000 0072 0f00 0000  .r....r....r....
+00003f60: 7220 0000 0072 5200 0000 7221 0000 0072  r ...rR...r!...r
+00003f70: 0e00 0000 290c da15 7369 6e67 6c65 5f72  ....)...single_r
+00003f80: 6f69 5f66 6967 5f63 6f6c 6f75 727a 1252  oi_fig_colourz.R
+00003f90: 6567 696f 6e61 6c20 6869 7374 6f67 7261  egional histogra
+00003fa0: 6d5a 1268 6973 746f 6772 616d 5f62 696e  mZ.histogram_bin
+00003fb0: 7769 6474 685a 1568 6973 746f 6772 616d  widthZ.histogram
+00003fc0: 5f66 6967 5f6c 6162 656c 5f78 5a15 6869  _fig_label_xZ.hi
+00003fd0: 7374 6f67 7261 6d5f 6669 675f 6c61 6265  stogram_fig_labe
+00003fe0: 6c5f 795a 1868 6973 746f 6772 616d 5f73  l_yZ.histogram_s
+00003ff0: 7461 745f 6c69 6e65 5f73 697a 655a 1368  tat_line_sizeZ.h
+00004000: 6973 746f 6772 616d 5f73 686f 775f 6d65  istogram_show_me
+00004010: 616e 5a15 6869 7374 6f67 7261 6d5f 7368  anZ.histogram_sh
+00004020: 6f77 5f6d 6564 6961 6e5a 1568 6973 746f  ow_medianZ.histo
+00004030: 6772 616d 5f73 686f 775f 6c65 6765 6e64  gram_show_legend
+00004040: da15 6869 7374 6f67 7261 6d5f 6669 675f  ..histogram_fig_
+00004050: 785f 6661 6365 74da 1568 6973 746f 6772  x_facet..histogr
+00004060: 616d 5f66 6967 5f79 5f66 6163 6574 5a14  am_fig_y_facetZ.
+00004070: 6869 7374 6f67 7261 6d5f 6669 675f 636f  histogram_fig_co
+00004080: 6c6f 7572 2907 da07 5f5f 646f 635f 5fda  lour)...__doc__.
+00004090: 0570 6167 6573 7202 0000 0072 0300 0000  .pagesr....r....
+000040a0: 7204 0000 0072 0500 0000 7206 0000 00a9  r....r....r.....
+000040b0: 0072 7900 0000 7279 0000 00fa 5c2f 5573  .ry...ry....\/Us
+000040c0: 6572 732f 6c70 7865 6831 302f 446f 6375  ers/lpxeh10/Docu
+000040d0: 6d65 6e74 732f 5265 706f 7369 746f 7269  ments/Repositori
+000040e0: 6573 2f66 4d52 495f 524f 495f 616e 616c  es/fMRI_ROI_anal
+000040f0: 7973 6973 5f74 6f6f 6c2f 6652 4154 2f75  ysis_tool/fRAT/u
+00004100: 7469 6c73 2f66 5241 545f 636f 6e66 6967  tils/fRAT_config
+00004110: 5f73 6574 7570 2e70 79da 083c 6d6f 6475  _setup.py..<modu
+00004120: 6c65 3e01 0000 0073 b803 0000 0400 0801  le>....s........
+00004130: 0202 0201 0601 0201 0201 0201 04fd 02ff  ................
+00004140: 0606 0201 0401 04fe 02fa 060a 0201 0401  ................
+00004150: 04fe 02f6 060e 0401 04ff 02f2 0611 0401  ................
+00004160: 04ff 02ef 0614 0201 04ff 02ec 0c17 0201  ................
+00004170: 0201 04fe 02e9 081b 0201 0201 04fe 02e5  ................
+00004180: 081f 0201 0201 04fe 02e1 0423 0201 0601  ...........#....
+00004190: 0201 0201 04fc 02dd 082d 0201 04ff 02d3  .........-......
+000041a0: 0e32 0401 04ff 02ce 0835 02cb 0a37 0201  .2.......5...7..
+000041b0: 04ff 02c9 043a 0201 0601 0201 0201 04fc  .....:..........
+000041c0: 02c6 0641 0201 04ff 04bf 0246 0201 0a01  ...A.......F....
+000041d0: 0601 020f 04f0 02ff 0813 0201 04ff 02ed  ................
+000041e0: 0a1d 0201 04ff 02e3 0822 0201 04ff 02de  ........."......
+000041f0: 0426 0201 0201 0601 0201 0201 04fb 02da  .&..............
+00004200: 0432 0401 0201 04fe 02ce 043a 0601 0201  .2.........:....
+00004210: 0201 0202 0201 04fa 02c6 0c42 0401 04ff  ...........B....
+00004220: 02be 0845 0201 0201 0201 04fd 02bb 084b  ...E...........K
+00004230: 0201 0201 0201 04fd 02b5 0654 0601 0401  ...........T....
+00004240: 0201 04fd 02ac 0a5b 0401 0401 04fe 02a5  .......[........
+00004250: 085f 02a1 0661 0201 04ff 029f 0668 0201  ._...a.......h..
+00004260: 0201 04fe 0298 0c6d 0201 0201 04fe 0293  .......m........
+00004270: 0672 0601 0401 0201 04fd 048e 027a 0201  .r...........z..
+00004280: 0801 0201 0201 04fe 02ff 0407 0201 0201  ................
+00004290: 04fe 02f9 040f 0201 0201 0201 04fd 02f1  ................
+000042a0: 0614 0201 0201 04fe 02ec 0419 0201 0201  ................
+000042b0: 04fe 02e7 0624 0201 04ff 02dc 0629 0201  .....$.......)..
+000042c0: 04ff 02d7 082e 0201 0201 04fe 02d2 0633  ...............3
+000042d0: 0201 0201 0201 0201 0201 04fb 02cd 063d  ...............=
+000042e0: 0201 0201 0203 04fb 02c3 0844 02bc 0646  ...........D...F
+000042f0: 0201 0201 04fe 02ba 064a 0201 0a01 0601  .........J......
+00004300: 0201 04fc 02b6 085a 02a6 065c 0201 0201  .......Z...\....
+00004310: 04fe 02a4 0a60 0201 0201 0201 04fd 02a0  .....`..........
+00004320: 0465 0201 0201 0201 04fd 029b 026b 0201  .e...........k..
+00004330: 0201 0201 04fd 0206 0201 0201 0201 04fd  ................
+00004340: 0606 0602 0201 04ff 0887 007f 0203 0202  ................
+00004350: 0201 0601 0201 04fd 020e 0201 0401 0201  ................
+00004360: 0201 04fc 040b 0201 04ff 0603 0201 04ff  ................
+00004370: 06e3 0223 0201 0801 02ff 0803 0201 04ff  ...#............
+00004380: 02fd 0806 0201 04ff 02fa 0809 0201 04ff  ................
+00004390: 02f7 080c 0201 04ff 02f4 080f 0201 04ff  ................
+000043a0: 02f1 0812 0201 04ff 02ee 0815 0201 04ff  ................
+000043b0: 02eb 0618 0201 0201 04fe 02e8 0a1c 0201  ................
+000043c0: 04ff 02e4 0820 02e0 0622 0201 04ff 02de  ..... ..."......
+000043d0: 0825 0201 04ff 02db 082b 0201 04ff 02d5  .%.......+......
+000043e0: 0631 0201 04ff 02cf 0a35 0401 04ff 02cb  .1.......5......
+000043f0: 0c39 0401 0601 06fe 04c7 0c3d 0401 0601  .9.........=....
+00004400: 06fe 02c3 0a41 0401 0401 06fe 02bf 0a45  .....A.........E
+00004410: 0401 0401 06fe 02bb 0a49 02b7 0c4b 0201  .........I...K..
+00004420: 04ff 02b5 0c4e 0201 04ff 02b2 0c51 0201  .....N.......Q..
+00004430: 04ff 02af 0c54 0201 04ff 02ac 0a57 0401  .....T.......W..
+00004440: 0401 0401 04fd 02a9 0a5c 0401 0401 0401  .........\......
+00004450: 04fd 02a4 0a61 0601 0201 06fe 029f 0a65  .....a.........e
+00004460: 0601 0201 06fe 029b 0a69 0297 0c6b 0201  .........i...k..
+00004470: 04ff 0295 0c6e 0201 04ff 0292 0c71 0201  .....n.......q..
+00004480: 04ff 028f 0a74 0601 0201 06fe 048c 0678  .....t.........x
+00004490: 0601 0201 06fe 0604 1002 0602 0601 0201  ................
+000044a0: 04fe 0604 0601 0201 04fe 0a04 0201 04ff  ................
+000044b0: 0803 0201 04ff 0803 0201 04ff 0803 0201  ................
+000044c0: 04ff 0803 0201 0601 0201 06fd 0805 0201  ................
+000044d0: 0401 0401 06fd 0a05 0401 0401 0401 06fd  ................
+000044e0: 0081 0ee1                                ....
```

### Comparing `frat_brain-1.3.5/fRAT/utils/__pycache__/figures.cpython-310.pyc` & `frat_brain-1.3.6/fRAT/utils/__pycache__/figures.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Mar 30 13:31:17 2023 UTC, .py size: 36602 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 258f 2564 fa8e 0000  o.......%.%d....
+00000000: 6f0d 0d0a 0000 0000 445f 4164 058f 0000  o.......D_Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 0601 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6402 6c05 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6403 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6401 6c08 6d09 5a0a 0100 6400 6401 6c0b  d.l.m.Z...d.d.l.
@@ -462,928 +462,930 @@
 00001cd0: 734a 0000 0010 030a 0108 0104 010a fe0a  sJ..............
 00001ce0: 0516 010a 0108 020a 010e 010a 020e 0128  ...............(
 00001cf0: 020e 011e 0102 ff06 0206 fe28 040e 011e  ...........(....
 00001d00: 0102 ff06 0206 fe02 8012 0408 0208 011a  ................
 00001d10: 0202 0106 ff1a 0202 0106 ff08 0204 027a  ...............z
 00001d20: 1442 7261 696e 4772 6964 2e6d 616b 655f  .BrainGrid.make_
 00001d30: 7461 626c 6563 0a00 0000 0000 0000 0000  tablec..........
-00001d40: 0000 1200 0000 0b00 0000 4300 0000 7306  ..........C...s.
+00001d40: 0000 1200 0000 0b00 0000 4300 0000 7326  ..........C...s&
 00001d50: 0100 007c 019b 0064 017c 029b 0064 029d  ...|...d.|...d..
 00001d60: 047d 0a7c 07a0 007c 0aa1 0101 0064 037c  .}.|...|.....d.|
 00001d70: 099b 0064 047c 019b 007c 039b 009d 057d  ...d.|...|.....}
 00001d80: 0b7c 0364 017c 089b 0064 059d 036b 0272  .|.d.|...d...k.r
 00001d90: 3e7c 02a0 0164 06a1 0164 076b 0272 3e74  >|...d...d.k.r>t
 00001da0: 02a0 037c 0ba1 017d 0c7c 0ca0 04a1 007d  ...|...}.|.....}
 00001db0: 0c74 05a0 067c 0ca1 017d 047c 05a0 0074  .t...|...}.|...t
 00001dc0: 05a0 067c 0ca1 017c 0166 02a1 0101 0074  ...|...|.f.....t
 00001dd0: 02a0 037c 0ba1 017d 0d74 02a0 0774 05a0  ...|...}.t...t..
 00001de0: 087c 0da0 04a1 00a1 017c 0d6a 097c 0d6a  .|.......|.j.|.j
 00001df0: 0aa1 037d 0d74 0b6a 0c7c 0d64 0864 0864  ...}.t.j.|.d.d.d
 00001e00: 0964 0a7c 067c 047c 006a 0d6a 0e7c 006a  .d.|.|.|.j.j.|.j
 00001e10: 0d6a 0f66 0264 0b64 0c8d 097d 0e7c 0e6a  .j.f.d.d...}.|.j
 00001e20: 107c 0a7c 006a 0d6a 1164 0d8d 0201 007c  .|.|.j.j.d.....|
-00001e30: 0ea0 12a1 0001 0074 13a0 147c 0aa1 017d  .......t...|...}
-00001e40: 0f7c 0f6a 155c 027d 107d 117c 0a7c 077c  .|.j.\.}.}.|.|.|
-00001e50: 107c 1166 0266 0353 0029 0e4e 720e 0000  .|.f.f.S.).Nr...
-00001e60: 0072 4700 0000 728c 0000 0072 4600 0000  .rG...r....rF...
-00001e70: 728e 0000 0072 a300 0000 72a4 0000 0046  r....r....r....F
-00001e80: 54da 0278 7ada 0769 6e66 6572 6e6f 2908  T..xz..inferno).
-00001e90: 5a0a 6472 6177 5f63 726f 7373 5a08 616e  Z.draw_crossZ.an
-00001ea0: 6e6f 7461 7465 da08 636f 6c6f 7262 6172  notate..colorbar
-00001eb0: 5a0c 6469 7370 6c61 795f 6d6f 6465 72b8  Z.display_moder.
-00001ec0: 0000 0072 b600 0000 5a0a 6375 745f 636f  ...r....Z.cut_co
-00001ed0: 6f72 6473 da04 636d 6170 2901 72c0 0000  ords..cmap).r...
-00001ee0: 0029 16da 0661 7070 656e 64da 0466 696e  .)...append..fin
-00001ef0: 64da 036e 6962 7270 0000 00da 0967 6574  d..nibrp.....get
-00001f00: 5f66 6461 7461 da02 6e70 da06 6e61 6e6d  _fdata..np..nanm
-00001f10: 6178 da0b 4e69 6674 6931 496d 6167 65da  ax..Nifti1Image.
-00001f20: 0a6e 616e 5f74 6f5f 6e75 6dda 0661 6666  .nan_to_num..aff
-00001f30: 696e 65da 0668 6561 6465 7272 0500 0000  ine..headerr....
-00001f40: 5a09 706c 6f74 5f61 6e61 7472 1300 0000  Z.plot_anatr....
-00001f50: da0d 6272 6169 6e5f 785f 636f 6f72 64da  ..brain_x_coord.
-00001f60: 0d62 7261 696e 5f7a 5f63 6f6f 7264 72d1  .brain_z_coordr.
-00001f70: 0000 0072 d200 0000 722d 0000 0072 0700  ...r....r-...r..
-00001f80: 0000 726d 0000 00da 0473 697a 6529 1272  ..rm.....size).r
-00001f90: 2f00 0000 726f 0000 0072 b000 0000 7295  /...ro...r....r.
-00001fa0: 0000 0072 b600 0000 72b7 0000 0072 b800  ...r....r....r..
-00001fb0: 0000 7296 0000 0072 9400 0000 7293 0000  ..r....r....r...
-00001fc0: 005a 0870 6e67 5f70 6174 685a 0a6e 6966  .Z.png_pathZ.nif
-00001fd0: 7469 5f70 6174 68da 0562 7261 696e 7297  ti_path..brainr.
-00001fe0: 0000 00da 0470 6c6f 74da 0269 6d72 4b00  .....plot..imrK.
-00001ff0: 0000 724a 0000 0072 3500 0000 7235 0000  ..rJ...r5...r5..
-00002000: 0072 3600 0000 72c2 0000 0035 0100 0073  .r6...r....5...s
-00002010: 2a00 0000 1004 0a01 1402 1e02 0a02 0801  *...............
-00002020: 0a02 1404 0a03 1c01 0602 0801 0401 0e01  ................
-00002030: 0201 06fc 1205 0801 0a02 0a01 0e02 7a19  ..............z.
-00002040: 4272 6169 6e47 7269 642e 7361 7665 5f62  BrainGrid.save_b
-00002050: 7261 696e 5f69 6d67 7363 0200 0000 0000  rain_imgsc......
-00002060: 0000 0000 0000 1100 0000 0800 0000 4300  ..............C.
-00002070: 0000 73be 0100 0067 007d 0267 007d 037c  ..s....g.}.g.}.|
-00002080: 006a 006a 0144 005d 187d 0474 0274 037c  .j.j.D.].}.t.t.|
-00002090: 017c 0419 00a0 04a1 0083 0183 017d 0564  .|...........}.d
-000020a0: 0164 0284 007c 0544 0083 017d 057c 02a0  .d...|.D...}.|..
-000020b0: 057c 05a1 0101 0071 087c 027d 0674 037c  .|.....q.|.}.t.|
-000020c0: 006a 006a 01a0 06a1 0083 017d 077c 006a  .j.j.......}.|.j
-000020d0: 006a 0764 0367 0167 0064 049c 037c 006a  .j.d.g.g.d...|.j
-000020e0: 006a 0864 0367 0167 0064 049c 0364 059c  .j.d.g.g.d...d..
-000020f0: 027d 087c 0844 005d 1a7d 097c 087c 0919  .}.|.D.].}.|.|..
-00002100: 0064 0619 0064 076b 0272 4b71 407c 067c  .d...d.k.rKq@|.|
-00002110: 07a0 097c 087c 0919 0064 0619 00a1 0119  ...|.|...d......
-00002120: 007c 087c 0919 0064 083c 0071 4074 0a7c  .|.|...d.<.q@t.|
-00002130: 0864 0919 0064 0819 0083 017d 0a74 0a7c  .d...d.....}.t.|
-00002140: 0864 0a19 0064 0819 0083 017d 0b74 0b7c  .d...d.....}.t.|
-00002150: 0164 0b19 00a0 04a1 0083 0144 005d 655c  .d.........D.]e\
-00002160: 027d 0c7d 0d67 007d 0e7c 017c 0164 0b19  .}.}.g.}.|.|.d..
-00002170: 007c 0d6b 0219 006a 0c64 0319 007d 0f7c  .|.k...j.d...}.|
-00002180: 0844 005d 407d 097c 087c 0919 0064 0819  .D.]@}.|.|...d..
-00002190: 0064 0367 016b 0372 b874 0d7c 0f7c 087c  .d.g.k.r.t.|.|.|
-000021a0: 0919 0064 0619 0019 0083 017d 107c 087c  ...d.......}.|.|
-000021b0: 0919 0064 0c19 00a0 057c 087c 0919 0064  ...d.....|.|...d
-000021c0: 0819 00a0 097c 10a1 01a1 0101 007c 0ea0  .....|.......|..
-000021d0: 057c 087c 0919 0064 0819 00a0 097c 10a1  .|.|...d.....|..
-000021e0: 01a1 0101 0071 867c 087c 0919 0064 0c19  .....q.|.|...d..
-000021f0: 00a0 0564 03a1 0101 007c 0ea0 0564 03a1  ...d.....|...d..
-00002200: 0101 0071 867c 03a0 0574 0ea0 0f7c 0e64  ...q.|...t...|.d
-00002210: 0d19 007c 0e64 0319 0066 027c 0b7c 0a66  ...|.d...f.|.|.f
-00002220: 02a1 02a1 0101 0071 737c 087c 037c 0b7c  .......qs|.|.|.|
-00002230: 0a66 0453 0029 0e4e 6301 0000 0000 0000  .f.S.).Nc.......
-00002240: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
-00002250: 0073 1400 0000 6700 7c00 5d06 7d01 7400  .s....g.|.].}.t.
-00002260: 7c01 8301 9102 7102 5300 7235 0000 0029  |.....q.S.r5...)
-00002270: 0172 7500 0000 2902 7299 0000 00da 0570  .ru...).r......p
-00002280: 6172 616d 7235 0000 0072 3500 0000 7236  aramr5...r5...r6
-00002290: 0000 0072 9c00 0000 6101 0000 f302 0000  ...r....a.......
-000022a0: 0014 007a 2942 7261 696e 4772 6964 2e74  ...z)BrainGrid.t
-000022b0: 6162 6c65 5f73 6574 7570 2e3c 6c6f 6361  able_setup.<loca
-000022c0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7201  ls>.<listcomp>r.
-000022d0: 0000 0029 0372 ea00 0000 72bc 0000 0072  ...).r....r....r
-000022e0: ba00 0000 2902 72bb 0000 0072 b900 0000  ....).r....r....
-000022f0: 72ea 0000 0072 4400 0000 72bc 0000 0072  r....rD...r....r
-00002300: bb00 0000 72b9 0000 0072 5800 0000 72ba  ....r....rX...r.
-00002310: 0000 0072 0800 0000 2910 7213 0000 00da  ...r....).r.....
-00002320: 0e70 6172 616d 6574 6572 5f64 6963 7472  .parameter_dictr
-00002330: ad00 0000 7268 0000 0072 a600 0000 72da  ....rh...r....r.
-00002340: 0000 00da 046b 6579 73da 1062 7261 696e  .....keys..brain
-00002350: 5f74 6162 6c65 5f63 6f6c 73da 1062 7261  _table_cols..bra
-00002360: 696e 5f74 6162 6c65 5f72 6f77 73da 0569  in_table_rows..i
-00002370: 6e64 6578 72c9 0000 0072 c100 0000 7277  ndexr....r....rw
-00002380: 0000 0072 7500 0000 72de 0000 00da 1172  ...ru...r......r
-00002390: 6176 656c 5f6d 756c 7469 5f69 6e64 6578  avel_multi_index
-000023a0: 2911 722f 0000 0072 af00 0000 5a0d 756e  ).r/...r....Z.un
-000023b0: 6971 7565 5f70 6172 616d 7372 b300 0000  ique_paramsr....
-000023c0: da03 6b65 79da 0670 6172 616d 735a 0b70  ..key..paramsZ.p
-000023d0: 6c6f 745f 7661 6c75 6573 5a0b 6178 6973  lot_valuesZ.axis
-000023e0: 5f74 6974 6c65 7372 b200 0000 7240 0000  _titlesr....r@..
-000023f0: 0072 b500 0000 72b4 0000 0072 d300 0000  .r....r....r....
-00002400: da09 6669 6c65 5f6e 616d 655a 1074 656d  ..file_nameZ.tem
-00002410: 705f 6f72 6465 725f 7374 6f72 655a 0d66  p_order_storeZ.f
-00002420: 696c 655f 6e61 6d65 5f72 6f77 5a0a 6669  ile_name_rowZ.fi
-00002430: 6c65 5f70 6172 616d 7235 0000 0072 3500  le_paramr5...r5.
-00002440: 0000 7236 0000 0072 a700 0000 5a01 0000  ..r6...r....Z...
-00002450: 7342 0000 0004 0204 010c 0214 010e 010c  sB..............
-00002460: 0104 0210 0110 0210 0106 ff08 0310 0102  ................
-00002470: 0102 0210 010e ff10 0310 0118 0204 0116  ................
-00002480: 0108 0212 0114 0220 021a 0112 020c 0116  ....... ........
-00002490: 0206 0108 ff0c 037a 1542 7261 696e 4772  .......z.BrainGr
-000024a0: 6964 2e74 6162 6c65 5f73 6574 7570 6306  id.table_setupc.
-000024b0: 0000 0000 0000 0000 0000 000b 0000 0007  ................
-000024c0: 0000 0043 0000 0073 4801 0000 7400 a001  ...C...sH...t...
-000024d0: 6401 7c05 6402 1900 7c05 6403 1900 6602  d.|.d...|.d...f.
-000024e0: 6404 a103 7d06 7402 7c01 6405 1900 6406  d...}.t.|.d...d.
-000024f0: 1900 8301 4400 5d4c 5c02 7d07 7d08 7403  ....D.]L\.}.}.t.
-00002500: a004 6402 7c07 6602 7c04 7c03 6602 a102  ..d.|.f.|.|.f...
-00002510: 7d09 7c09 7c02 7601 7261 7405 a006 7c04  }.|.|.v.rat...|.
-00002520: 7c03 7c09 6403 1700 a103 0100 7405 a007  |.|.d.......t...
-00002530: 7c06 a101 0100 7c00 a008 a100 0100 7405  |.....|.......t.
-00002540: 6a09 7c00 6a0a 6a0b 6407 1700 7c08 1700  j.|.j.j.d...|...
-00002550: 7c00 6a0a 6a0c 6408 8d02 0100 7c09 6402  |.j.j.d.....|.d.
-00002560: 6b02 7261 7405 6a0d 7c00 6a0a 6a0e 6407  k.rat.j.|.j.j.d.
-00002570: 1700 7c01 6409 1900 6406 1900 6402 1900  ..|.d...d...d...
-00002580: 1700 7c00 6a0a 6a0c 6408 8d02 0100 7115  ..|.j.j.d.....q.
-00002590: 7402 7c01 6409 1900 6406 1900 8301 4400  t.|.d...d.....D.
-000025a0: 5d37 5c02 7d07 7d0a 7403 a004 7c07 6402  ]7\.}.}.t...|.d.
-000025b0: 6602 7c04 7c03 6602 a102 7d09 7c09 7c02  f.|.|.f...}.|.|.
-000025c0: 7601 72a1 7c09 6402 6b03 72a1 7405 a006  v.r.|.d.k.r.t...
-000025d0: 7c04 7c03 7c09 6403 1700 a103 0100 7405  |.|.|.d.......t.
-000025e0: a007 7c06 a101 0100 7c00 a008 a100 0100  ..|.....|.......
-000025f0: 7405 6a0d 7c00 6a0a 6a0e 6407 1700 7c0a  t.j.|.j.j.d...|.
-00002600: 1700 7c00 6a0a 6a0c 6408 8d02 0100 716a  ..|.j.j.d.....qj
-00002610: 6400 5300 290a 4eda 0352 4742 7201 0000  d.S.).N..RGBr...
-00002620: 0072 0800 0000 2903 e9ff 0000 0072 f600  .r....)......r..
-00002630: 0000 72f6 0000 0072 bb00 0000 72bc 0000  ..r....r....r...
-00002640: 0072 0d00 0000 72bd 0000 0072 b900 0000  .r....r....r....
-00002650: 290f 7207 0000 0072 5500 0000 72c1 0000  ).r....rU...r...
-00002660: 0072 de00 0000 72f1 0000 0072 a800 0000  .r....r....r....
-00002670: 72c5 0000 0072 c600 0000 da13 6d61 6b65  r....r......make
-00002680: 5f63 656c 6c5f 696e 7669 7369 626c 6572  _cell_invisibler
-00002690: 4f00 0000 7213 0000 0072 ca00 0000 72cb  O...r....r....r.
-000026a0: 0000 0072 cc00 0000 72cd 0000 0029 0b72  ...r....r....).r
-000026b0: 2f00 0000 72b2 0000 0072 b300 0000 72b5  /...r....r....r.
-000026c0: 0000 0072 b400 0000 72d4 0000 0072 9700  ...r....r....r..
-000026d0: 0000 da07 636f 756e 7465 725a 0778 5f74  ....counterZ.x_t
-000026e0: 6974 6c65 5a0b 6869 6464 656e 5f63 656c  itleZ.hidden_cel
-000026f0: 6c5a 0779 5f74 6974 6c65 7235 0000 0072  lZ.y_titler5...r
-00002700: 3500 0000 7236 0000 0072 ce00 0000 8801  5...r6...r......
-00002710: 0000 732c 0000 001a 0318 0214 0108 0212  ..s,............
-00002720: 010a 0108 011e 0208 021e 0106 0106 ff02  ................
-00002730: 8018 0314 0110 0212 010a 0108 011e 0202  ................
-00002740: 8004 f87a 1f42 7261 696e 4772 6964 2e6c  ...z.BrainGrid.l
-00002750: 6162 656c 5f62 6c61 6e6b 5f63 656c 6c5f  abel_blank_cell_
-00002760: 6178 6573 6300 0000 0000 0000 0000 0000  axesc...........
-00002770: 0001 0000 0003 0000 0043 0000 0073 6c00  .........C...sl.
-00002780: 0000 7400 a001 a100 7d00 7c00 6a02 a003  ..t.....}.|.j...
-00002790: a100 a004 6700 a101 0100 7c00 6a02 a005  ....g.....|.j...
-000027a0: a100 a004 6700 a101 0100 7c00 6a06 6401  ....g.....|.j.d.
-000027b0: 1900 a007 6402 a101 0100 7c00 6a06 6403  ....d.....|.j.d.
-000027c0: 1900 a007 6402 a101 0100 7c00 6a06 6404  ....d.....|.j.d.
-000027d0: 1900 a007 6402 a101 0100 7c00 6a06 6405  ....d.....|.j.d.
-000027e0: 1900 a007 6402 a101 0100 6400 5300 2906  ....d.....d.S.).
-000027f0: 4eda 046c 6566 7446 da05 7269 6768 74da  N..leftF..right.
-00002800: 0662 6f74 746f 6dda 0374 6f70 2908 72a8  .bottom..top).r.
-00002810: 0000 0072 c700 0000 723b 0000 00da 0967  ...r....r;.....g
-00002820: 6574 5f78 6178 6973 5a09 7365 745f 7469  et_xaxisZ.set_ti
-00002830: 636b 73da 0967 6574 5f79 6178 6973 5a06  cks..get_yaxisZ.
-00002840: 7370 696e 6573 da0b 7365 745f 7669 7369  spines..set_visi
-00002850: 626c 6529 01da 0566 7261 6d65 7235 0000  ble)...framer5..
-00002860: 0072 3500 0000 7236 0000 0072 f700 0000  .r5...r6...r....
-00002870: a501 0000 730e 0000 0008 0210 0110 0110  ....s...........
-00002880: 0110 0110 0114 017a 1d42 7261 696e 4772  .......z.BrainGr
-00002890: 6964 2e6d 616b 655f 6365 6c6c 5f69 6e76  id.make_cell_inv
-000028a0: 6973 6962 6c65 4e29 0c72 8700 0000 7288  isibleN).r....r.
-000028b0: 0000 0072 8900 0000 728a 0000 0072 2600  ...r....r....r&.
-000028c0: 0000 722b 0000 0072 ac00 0000 72c2 0000  ..r+...r....r...
-000028d0: 0072 a700 0000 72ce 0000 0072 8b00 0000  .r....r....r....
-000028e0: 72f7 0000 0072 3500 0000 7235 0000 0072  r....r5...r5...r
-000028f0: 3500 0000 7236 0000 0072 2500 0000 a700  5...r6...r%.....
-00002900: 0000 731e 0000 0008 0002 010a 0102 220a  ..s...........".
-00002910: 0102 3e0a 0102 2a0a 0102 240a 0102 2d0a  ..>...*...$...-.
-00002920: 0102 1c0e 0172 2500 0000 6300 0000 0000  .....r%...c.....
-00002930: 0000 0000 0000 0000 0000 0003 0000 0040  ...............@
-00002940: 0000 0073 1800 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
-00002950: 6503 6401 6402 8400 8301 5a04 6403 5300  e.d.d.....Z.d.S.
-00002960: 2904 7229 0000 0063 0200 0000 0000 0000  ).r)...c........
-00002970: 0000 0000 0700 0000 0800 0000 4300 0000  ............C...
-00002980: 7364 0200 0074 00a0 017c 01a1 017d 027c  sd...t...|...}.|
-00002990: 027c 0264 0119 0064 026b 037c 0264 0119  .|.d...d.k.|.d..
-000029a0: 0064 036b 0340 0019 007d 027c 027c 0264  .d.k.@...}.|.|.d
-000029b0: 0419 0064 056b 0419 007d 027c 006a 026a  ...d.k...}.|.j.j
-000029c0: 0364 066b 0273 387c 006a 026a 0464 066b  .d.k.s8|.j.j.d.k
-000029d0: 0273 387c 02a0 057c 006a 026a 037c 006a  .s8|...|.j.j.|.j
-000029e0: 026a 0467 02a1 01a0 0664 0764 0884 00a1  .j.g.....d.d....
-000029f0: 017d 026e 257c 006a 026a 0364 066b 0273  .}.n%|.j.j.d.k.s
-00002a00: 4b7c 02a0 057c 006a 026a 03a1 01a0 0664  K|...|.j.j.....d
-00002a10: 0964 0884 00a1 017d 026e 127c 006a 026a  .d.....}.n.|.j.j
-00002a20: 0464 066b 0273 5d7c 02a0 057c 006a 026a  .d.k.s]|...|.j.j
-00002a30: 04a1 01a0 0664 0a64 0884 00a1 017d 027c  .....d.d.....}.|
-00002a40: 026a 0764 0b64 0c8d 017d 0264 0d7c 0264  .j.d.d...}.d.|.d
-00002a50: 0e3c 0064 0f7d 0374 086a 0974 086a 0a64  .<.d.}.t.j.t.j.d
-00002a60: 0e64 1064 118d 0264 128d 017d 0474 086a  .d.d...d...}.t.j
-00002a70: 0974 086a 0a64 0e64 1364 118d 0264 128d  .t.j.d.d.d...d..
-00002a80: 017d 0574 08a0 0b7c 02a1 0174 086a 0964  .}.t...|...t.j.d
-00002a90: 0e64 0464 148d 0217 0074 086a 0c7c 0564  .d.d.....t.j.|.d
-00002aa0: 0b64 157c 006a 026a 0d64 1664 178d 0517  .d.|.j.j.d.d....
-00002ab0: 0074 086a 0e64 0f64 057c 006a 026a 0f64  .t.j.d.d.|.j.j.d
-00002ac0: 1664 188d 0417 0074 08a0 1064 1964 1aa1  .d.....t...d.d..
-00002ad0: 0217 0074 08a0 1164 0564 00a1 0217 0074  ...t...d.d.....t
-00002ae0: 08a0 127c 006a 026a 13a1 0117 0074 08a0  ...|.j.j.....t..
-00002af0: 1464 06a1 0117 0074 086a 157c 006a 026a  .d.....t.j.|.j.j
-00002b00: 049b 0064 1b7c 006a 026a 039b 009d 0364  ...d.|.j.j.....d
-00002b10: 0b64 1c64 1d8d 0317 0074 08a0 16a1 0017  .d.d.....t......
-00002b20: 0074 086a 1774 086a 186a 1964 0d64 1e8d  .t.j.t.j.j.d.d..
-00002b30: 0174 086a 186a 1964 0564 1e8d 0174 086a  .t.j.j.d.d...t.j
-00002b40: 1a64 1f64 0f64 208d 0274 08a0 1ba1 007c  .d.d.d ..t.....|
-00002b50: 006a 026a 1c64 218d 0517 007d 067c 006a  .j.j.d!....}.|.j
-00002b60: 026a 1d90 0172 057c 006a 026a 1e72 ff7c  .j...r.|.j.j.r.|
-00002b70: 0674 086a 1f64 2264 0564 238d 0237 007d  .t.j.d"d.d#..7.}
-00002b80: 066e 067c 0674 08a0 20a1 0037 007d 067c  .n.|.t.. ..7.}.|
-00002b90: 066a 2164 247c 006a 026a 227c 006a 026a  .j!d$|.j.j"|.j.j
-00002ba0: 2264 2514 0064 2664 2664 278d 0501 007c  "d%..d&d&d'....|
-00002bb0: 066a 2164 287c 006a 026a 227c 006a 026a  .j!d(|.j.j"|.j.j
-00002bc0: 2264 2514 0064 2664 2664 278d 0501 007c  "d%..d&d&d'....|
-00002bd0: 006a 026a 2390 0172 3074 2464 2983 0101  .j.j#..r0t$d)...
-00002be0: 0064 0053 0064 0053 0029 2a4e 72f0 0000  .d.S.d.S.)*Nr...
-00002bf0: 00da 074f 7665 7261 6c6c fa06 4e6f 2052  ...Overall..No R
-00002c00: 4f49 725b 0000 0072 0100 0000 7244 0000  OIr[...r....rD..
-00002c10: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-00002c20: 0000 0300 0000 5300 0000 f30c 0000 007c  ......S........|
-00002c30: 00a0 0064 0167 01a1 0153 00a9 024e 725b  ...d.g...S...Nr[
-00002c40: 0000 00a9 01da 0b73 6f72 745f 7661 6c75  .......sort_valu
-00002c50: 6573 a901 da01 7872 3500 0000 7235 0000  es....xr5...r5..
-00002c60: 0072 3600 0000 da08 3c6c 616d 6264 613e  .r6.....<lambda>
-00002c70: ba01 0000 f302 0000 000c 007a 2156 696f  ...........z!Vio
-00002c80: 6c69 6e50 6c6f 742e 6d61 6b65 2e3c 6c6f  linPlot.make.<lo
-00002c90: 6361 6c73 3e2e 3c6c 616d 6264 613e 6301  cals>.<lambda>c.
-00002ca0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00002cb0: 0000 0053 0000 0072 0301 0000 7204 0100  ...S...r....r...
-00002cc0: 0072 0501 0000 7207 0100 0072 3500 0000  .r....r....r5...
-00002cd0: 7235 0000 0072 3600 0000 7209 0100 00bd  r5...r6...r.....
-00002ce0: 0100 0072 0a01 0000 6301 0000 0000 0000  ...r....c.......
-00002cf0: 0000 0000 0001 0000 0003 0000 0053 0000  .............S..
-00002d00: 0072 0301 0000 7204 0100 0072 0501 0000  .r....r....r....
-00002d10: 7207 0100 0072 3500 0000 7235 0000 0072  r....r5...r5...r
-00002d20: 3600 0000 7209 0100 00c0 0100 0072 0a01  6...r........r..
-00002d30: 0000 54a9 01da 0464 726f 7072 0800 0000  ..T....dropr....
-00002d40: da08 636f 6e73 7461 6e74 72a0 0000 007a  ..constantr....z
-00002d50: 0778 2b73 6869 6674 2901 5a0b 6166 7465  .x+shift).Z.afte
-00002d60: 725f 7363 616c 6572 0701 0000 7a07 782d  r_scaler....z.x-
-00002d70: 7368 6966 74a9 0272 0801 0000 da01 7972  shift..r......yr
-00002d80: f900 0000 6733 3333 3333 33e3 3f29 04da  ....g333333.?)..
-00002d90: 056e 615f 726d da05 7374 796c 65da 0466  .na_rm..style..f
-00002da0: 696c 6c72 e600 0000 2904 724b 0000 005a  illr....).rK...Z
-00002db0: 0d6f 7574 6c69 6572 5f61 6c70 6861 7212  .outlier_alphar.
-00002dc0: 0100 0072 e600 0000 679a 9999 9999 99d9  ...r....g.......
-00002dd0: 3f67 6666 6666 6666 f63f da01 7eda 0a6c  ?gffffff.?..~..l
-00002de0: 6162 656c 5f62 6f74 68a9 0272 0c01 0000  abel_both..r....
-00002df0: 5a08 6c61 6265 6c6c 6572 a901 da05 616c  Z.labeller....al
-00002e00: 7068 61da 0467 7261 79a9 0272 1201 0000  pha..gray..r....
-00002e10: 7217 0100 0029 05da 1270 616e 656c 5f67  r....)...panel_g
-00002e20: 7269 645f 6d61 6a6f 725f 79da 1270 616e  rid_major_y..pan
-00002e30: 656c 5f67 7269 645f 6d61 6a6f 725f 78da  el_grid_major_x.
-00002e40: 1070 616e 656c 5f62 6163 6b67 726f 756e  .panel_backgroun
-00002e50: 64da 0b61 7869 735f 7465 7874 5f78 72c0  d..axis_text_xr.
-00002e60: 0000 0067 7b14 ae47 e17a a43f 2902 724b  ...g{..G.z.?).rK
-00002e70: 0000 0072 4a00 0000 7a23 4669 6775 7265  ...rJ...z#Figure
-00002e80: 732f 5669 6f6c 696e 5f70 6c6f 7473 2f76  s/Violin_plots/v
-00002e90: 696f 6c69 6e70 6c6f 742e 706e 6772 4800  iolinplot.pngrH.
-00002ea0: 0000 4672 4900 0000 7a23 4669 6775 7265  ..FrI...z#Figure
-00002eb0: 732f 5669 6f6c 696e 5f70 6c6f 7473 2f76  s/Violin_plots/v
-00002ec0: 696f 6c69 6e70 6c6f 742e 7376 677a 1253  iolinplot.svgz.S
-00002ed0: 6176 6564 2076 696f 6c69 6e20 706c 6f74  aved violin plot
-00002ee0: 2129 25da 0463 6f70 79da 0864 6565 7063  !)%..copy..deepc
-00002ef0: 6f70 7972 1300 0000 da0a 7461 626c 655f  opyr......table_
-00002f00: 636f 6c73 da0a 7461 626c 655f 726f 7773  cols..table_rows
-00002f10: da07 6772 6f75 7062 79da 0561 7070 6c79  ..groupby..apply
-00002f20: da0b 7265 7365 745f 696e 6465 78da 0470  ..reset_index..p
-00002f30: 6c74 6eda 0361 6573 da05 7374 6167 65da  ltn..aes..stage.
-00002f40: 0667 6770 6c6f 745a 0b67 656f 6d5f 7669  .ggplotZ.geom_vi
-00002f50: 6f6c 696e da0d 7669 6f6c 696e 5f63 6f6c  olin..violin_col
-00002f60: 6f75 725a 0c67 656f 6d5f 626f 7870 6c6f  ourZ.geom_boxplo
-00002f70: 74da 0e62 6f78 706c 6f74 5f63 6f6c 6f75  t..boxplot_colou
-00002f80: 72da 0478 6c69 6dda 0479 6c69 6d5a 0479  r..xlim..ylimZ.y
-00002f90: 6c61 62da 0d74 6162 6c65 5f78 5f6c 6162  lab..table_x_lab
-00002fa0: 656c 5a04 786c 6162 da0a 6661 6365 745f  elZ.xlab..facet_
-00002fb0: 6772 6964 da09 7468 656d 655f 3533 38da  grid..theme_538.
-00002fc0: 0574 6865 6d65 da06 7468 656d 6573 da0c  .theme..themes..
-00002fd0: 656c 656d 656e 745f 6c69 6e65 da0c 656c  element_line..el
-00002fe0: 656d 656e 745f 7265 6374 5a0d 656c 656d  ement_rectZ.elem
-00002ff0: 656e 745f 626c 616e 6b72 d200 0000 da10  ent_blankr......
-00003000: 7669 6f6c 696e 5f73 686f 775f 6461 7461  violin_show_data
-00003010: da0d 7669 6f6c 696e 5f6a 6974 7465 725a  ..violin_jitterZ
-00003020: 0b67 656f 6d5f 6a69 7474 6572 da0a 6765  .geom_jitter..ge
-00003030: 6f6d 5f70 6f69 6e74 7250 0000 0072 5100  om_pointrP...rQ.
-00003040: 0000 721e 0000 0072 1f00 0000 2907 722f  ..r....r....).r/
-00003050: 0000 005a 076f 7269 675f 6466 72af 0000  ...Z.orig_dfr...
-00003060: 00da 0573 6869 6674 da0b 7269 6768 745f  ...shift..right_
-00003070: 7368 6966 74da 0a6c 6566 745f 7368 6966  shift..left_shif
-00003080: 7472 3f00 0000 7235 0000 0072 3500 0000  tr?...r5...r5...
-00003090: 7236 0000 0072 2600 0000 b101 0000 7372  r6...r&.......sr
-000030a0: 0000 000a 021c 0210 0118 0222 020c 021a  ..........."....
-000030b0: 010c 0218 010c 0208 0204 0316 0216 0108  ................
-000030c0: 020c 0102 ff16 0202 fe14 0302 fd0a 0402  ................
-000030d0: fc0a 0502 fb0c 0602 fa08 0702 f91a 0802  ................
-000030e0: 0104 ff02 f806 0a02 f610 0b0c 010c 0106  ................
-000030f0: 0106 0104 fc04 f50a 1108 0114 010c 020c  ................
-00003100: 020a 0104 0106 fe0c 040a 0104 0106 fe0a  ................
-00003110: 040c 0104 ff7a 0f56 696f 6c69 6e50 6c6f  .....z.ViolinPlo
-00003120: 742e 6d61 6b65 4e29 0572 8700 0000 7288  t.makeN).r....r.
-00003130: 0000 0072 8900 0000 728a 0000 0072 2600  ...r....r....r&.
-00003140: 0000 7235 0000 0072 3500 0000 7235 0000  ..r5...r5...r5..
-00003150: 0072 3600 0000 7229 0000 00b0 0100 0073  .r6...r).......s
-00003160: 0600 0000 0800 0201 0e01 7229 0000 0063  ..........r)...c
-00003170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003180: 0300 0000 4000 0000 7324 0000 0065 005a  ....@...s$...e.Z
-00003190: 0164 005a 0265 0364 0164 0284 0083 015a  .d.Z.e.d.d.....Z
-000031a0: 0465 0564 0364 0484 0083 015a 0664 0553  .e.d.d.....Z.d.S
-000031b0: 0029 0672 2a00 0000 6303 0000 0000 0000  .).r*...c.......
-000031c0: 0000 0000 0007 0000 000a 0000 0043 0000  .............C..
-000031d0: 0073 5001 0000 7c00 6a00 6a01 6401 6b02  .sP...|.j.j.d.k.
-000031e0: 720a 7402 6402 8301 8201 7403 a004 6403  r.t.d.....t...d.
-000031f0: a101 0100 7405 7c01 6404 1900 a006 a100  ....t.|.d.......
-00003200: 8301 7d03 7403 6a07 7c03 6405 7c00 6a00  ..}.t.j.|.d.|.j.
-00003210: 6a08 6406 8d03 7d04 7a04 7c04 0100 5700  j.d...}.z.|...W.
-00003220: 6e15 0400 7409 793a 0100 0100 0100 7c00  n...t.y:......|.
-00003230: 6a00 6a0a 7237 740b 6407 8301 0100 5900  j.j.r7t.d.....Y.
-00003240: 6400 5300 5900 6400 5300 7700 7c00 6a00  d.S.Y.d.S.w.|.j.
-00003250: 6a0a 7243 740b 6408 8301 0100 6409 7d05  j.rCt.d.....d.}.
-00003260: 0900 740c 740d a00e 7c00 6a0f a101 7c04  ..t.t...|.j...|.
-00003270: 740d a00e 7c01 a101 740d a00e 7c05 a101  t...|...t...|...
-00003280: 740d a00e 7c00 6a10 a101 740d a00e 7c00  t...|.j...t...|.
-00003290: 6a11 a101 740d a00e 7c00 6a00 a101 8307  j...t...|.j.....
-000032a0: 7d06 7c02 7270 7c02 a012 7403 6a13 7c06  }.|.rp|...t.j.|.
-000032b0: a102 7d05 6e09 7405 740d a012 7403 6a13  ..}.n.t.t...t.j.
-000032c0: 7c06 a102 8301 7d05 7414 7c05 8301 72a5  |.....}.t.|...r.
-000032d0: 7c05 6a15 640b 640c 8400 640d 8d01 0100  |.j.d.d...d.....
-000032e0: 7c00 6a00 6a0a 729e 740b 640e 7416 7c05  |.j.j.r.t.d.t.|.
-000032f0: 640f 1900 6410 1900 8301 9b00 6411 7c05  d...d.......d.|.
-00003300: 640f 1900 6412 1900 9b00 6413 9d05 8301  d...d.....d.....
-00003310: 0100 7c05 640f 1900 6410 1900 7d05 6e02  ..|.d...d...}.n.
-00003320: 6400 5300 7146 2914 4e72 4400 0000 7a45  d.S.qF).NrD...zE
-00003330: 5061 7261 6d65 7465 7220 746f 2070 6c6f  Parameter to plo
-00003340: 7420 616c 6f6e 6720 7468 6520 782d 6178  t along the x-ax
-00003350: 6573 206f 6620 7468 6520 6261 7263 6861  es of the barcha
-00003360: 7274 7320 6861 7320 6e6f 7420 6265 656e  rts has not been
-00003370: 2073 6574 2e7a 1146 6967 7572 6573 2f42   set.z.Figures/B
-00003380: 6172 6368 6172 7473 72f0 0000 007a 144f  archartsr....z.O
-00003390: 6e65 2072 6567 696f 6e20 6261 7220 6368  ne region bar ch
-000033a0: 6172 74a9 02da 0966 756e 635f 6e61 6d65  art....func_name
-000033b0: da11 636f 6e66 6967 5f72 6567 696f 6e5f  ..config_region_
-000033c0: 7661 727a 1b53 6b69 7070 696e 6720 6261  varz.Skipping ba
-000033d0: 7263 6861 7274 2063 7265 6174 696f 6e2e  rchart creation.
-000033e0: 7a1a 0a2d 2d2d 2042 6172 6368 6172 7420  z..--- Barchart 
-000033f0: 6372 6561 7469 6f6e 202d 2d2d 7201 0000  creation ---r...
-00003400: 0054 6301 0000 0000 0000 0000 0000 0001  .Tc.............
-00003410: 0000 0002 0000 0053 0000 00f3 0800 0000  .......S........
-00003420: 7c00 6401 1900 5300 a902 4e72 0800 0000  |.d...S...Nr....
-00003430: 7235 0000 0072 0701 0000 7235 0000 0072  r5...r....r5...r
-00003440: 3500 0000 7236 0000 0072 0901 0000 1002  5...r6...r......
-00003450: 0000 f302 0000 0008 007a 2042 6172 6368  .........z Barch
-00003460: 6172 742e 7365 7475 702e 3c6c 6f63 616c  art.setup.<local
-00003470: 733e 2e3c 6c61 6d62 6461 3ea9 0172 f200  s>.<lambda>..r..
-00003480: 0000 7a14 4d61 7869 6d75 6d20 7920 6c69  ..z.Maximum y li
-00003490: 6d69 7420 6f66 3a20 72a4 0000 0072 0800  mit of: r....r..
-000034a0: 0000 fa10 2073 6565 6e20 7769 7468 2052  .... seen with R
-000034b0: 4f49 3a20 725f 0000 007a 262e 2043 7265  OI: r_...z&. Cre
-000034c0: 6174 696e 6720 6669 6775 7265 7320 7769  ating figures wi
-000034d0: 7468 2074 6869 7320 7920 6c69 6d69 742e  th this y limit.
-000034e0: 0a29 1772 1300 0000 da15 7369 6e67 6c65  .).r......single
-000034f0: 5f72 6f69 5f66 6967 5f78 5f61 7869 73da  _roi_fig_x_axis.
-00003500: 0945 7863 6570 7469 6f6e 7209 0000 0072  .Exceptionr....r
-00003510: 2800 0000 7268 0000 0072 a600 0000 da10  (...rh...r......
-00003520: 6669 6e64 5f63 686f 7365 6e5f 726f 6973  find_chosen_rois
-00003530: da11 7265 6769 6f6e 616c 5f66 6967 5f72  ..regional_fig_r
-00003540: 6f69 73da 094e 616d 6545 7272 6f72 721e  ois..NameErrorr.
-00003550: 0000 0072 1f00 0000 da03 7a69 70da 0969  ...r......zip..i
-00003560: 7465 7274 6f6f 6c73 da06 7265 7065 6174  tertools..repeat
-00003570: 7226 0000 0072 5600 0000 7243 0000 00da  r&...rV...rC....
-00003580: 0773 7461 726d 6170 da14 636c 6173 735f  .starmap..class_
-00003590: 6d65 7468 6f64 5f68 616e 646c 6572 da03  method_handler..
-000035a0: 616e 79da 0473 6f72 7472 ae00 0000 2907  any..sortr....).
-000035b0: 722f 0000 0072 af00 0000 7234 0000 00da  r/...r....r4....
-000035c0: 096c 6973 745f 726f 6973 da0b 6368 6f73  .list_rois..chos
-000035d0: 656e 5f72 6f69 7372 2c01 0000 da08 6974  en_roisr,.....it
-000035e0: 6572 6162 6c65 7235 0000 0072 3500 0000  erabler5...r5...
-000035f0: 7236 0000 0072 2b00 0000 f001 0000 7340  r6...r+.......s@
-00003600: 0000 000c 0208 010a 0210 0208 0106 0106  ................
-00003610: ff02 0208 010c 0108 010e 0106 ff02 ff08  ................
-00003620: 0408 0104 0202 0116 0112 0114 0104 fe04  ................
-00003630: 0410 0112 0308 0210 0108 022a 010e 0304  ...........*....
-00003640: 0202 ec7a 0e42 6172 6368 6172 742e 7365  ...z.Barchart.se
-00003650: 7475 7063 0600 0000 0000 0000 0000 0000  tupc............
-00003660: 0b00 0000 0f00 0000 4300 0000 736c 0200  ........C...sl..
-00003670: 007c 016a 007c 0164 0119 007c 006b 0219  .|.j.|.d...|.k..
-00003680: 007d 067c 06a0 017c 056a 0267 01a1 017d  .}.|...|.j.g...}
-00003690: 067c 066a 0364 0264 038d 017d 0674 046a  .|.j.d.d...}.t.j
-000036a0: 057c 067c 056a 0219 007c 067c 056a 0219  .|.|.j...|.|.j..
-000036b0: 00a0 06a1 0064 048d 027c 067c 056a 023c  .....d...|.|.j.<
-000036c0: 0064 0564 0684 007c 066a 0744 0083 017c  .d.d...|.j.D...|
-000036d0: 065f 077c 056a 02a0 0864 0764 08a1 027c  ._.|.j...d.d...|
-000036e0: 055f 027c 056a 09a0 0864 0764 08a1 027c  ._.|.j...d.d...|
-000036f0: 055f 0974 0aa0 0b7c 06a1 0174 0aa0 0ca1  ._.t...|...t....
-00003700: 0017 0074 0a6a 0d74 0a6a 0e64 0964 0a64  ...t.j.t.j.d.d.d
-00003710: 0b8d 0264 0a64 0264 0c8d 0317 0074 0a6a  ...d.d.d.....t.j
-00003720: 0f64 0d74 0a6a 0e64 0964 0a64 0b8d 0264  .d.t.j.d.d.d...d
-00003730: 0e8d 0217 0074 0a6a 1067 0064 0f8d 0117  .....t.j.g.d....
-00003740: 0074 0a6a 1174 0a6a 1264 1064 118d 0174  .t.j.t.j.d.d...t
-00003750: 0a6a 1364 1264 1364 148d 0274 0a6a 1464  .j.d.d.d...t.j.d
-00003760: 1564 1664 1764 188d 0374 0a6a 1464 1564  .d.d.d...t.j.d.d
-00003770: 1664 1764 188d 0374 0a6a 1464 1764 1664  .d.d...t.j.d.d.d
-00003780: 198d 0274 0a6a 1464 1764 1564 1664 1a64  ...t.j.d.d.d.d.d
-00003790: 1769 0164 1b8d 0474 0a6a 1464 1764 1664  .i.d...t.j.d.d.d
-000037a0: 1c64 1d69 0164 1e8d 0364 1f64 2064 2164  .d.i.d...d.d d!d
-000037b0: 2269 0164 237c 056a 1564 248d 0c17 0074  "i.d#|.j.d$....t
-000037c0: 0a6a 1674 0a6a 1764 257c 056a 0264 268d  .j.t.j.d%|.j.d&.
-000037d0: 0264 1664 1764 2764 288d 0417 0074 0a6a  .d.d.d'd(....t.j
-000037e0: 187c 056a 1964 298d 0117 007d 0764 2a64  .|.j.d)....}.d*d
-000037f0: 0684 007c 06a0 1aa1 0044 0083 0164 1019  ...|.....D...d..
-00003800: 007d 087c 056a 0964 2b6b 0273 e77c 0774  .}.|.j.d+k.s.|.t
-00003810: 0a6a 177c 056a 0264 2c64 2d7c 089b 009d  .j.|.j.d,d-|....
-00003820: 0264 2e7c 089b 009d 0264 2f7c 056a 099b  .d.|.....d/|.j..
-00003830: 0064 309d 0364 318d 0537 007d 076e 127c  .d0..d1..7.}.n.|
-00003840: 0774 0a6a 177c 056a 0264 2c64 2d7c 089b  .t.j.|.j.d,d-|..
-00003850: 009d 0264 2e7c 089b 009d 0264 328d 0437  ...d.|.....d2..7
-00003860: 007d 077c 0774 0a6a 1b7c 056a 1c7c 056a  .}.|.t.j.|.j.|.j
-00003870: 1d7c 056a 1e64 338d 0337 007d 077c 0290  .|.j.d3..7.}.|..
-00003880: 0172 157c 0774 0aa0 1f64 007c 02a1 0237  .r.|.t...d.|...7
-00003890: 007d 077c 0064 3437 007d 0064 107d 097c  .}.|.d47.}.d.}.|
-000038a0: 0264 106b 0290 0172 257c 047c 007c 0764  .d.k...r%|.|.|.d
-000038b0: 3583 037d 0964 367d 0a6e 077c 0264 106b  5..}.d6}.n.|.d.k
-000038c0: 0390 0172 2c64 377d 0a7c 037c 077c 007c  ...r,d7}.|.|.|.|
-000038d0: 0a64 387c 0583 0501 007c 0953 0029 394e  .d8|.....|.S.)9N
-000038e0: 72f0 0000 0054 720b 0100 0029 01da 0a63  r....Tr....)...c
-000038f0: 6174 6567 6f72 6965 7363 0100 0000 0000  ategoriesc......
-00003900: 0000 0000 0000 0200 0000 0600 0000 5300  ..............S.
-00003910: 0000 7318 0000 0067 007c 005d 087d 017c  ..s....g.|.].}.|
-00003920: 01a0 0064 0064 01a1 0291 0271 0253 0029  ...d.d.....q.S.)
-00003930: 0272 0d00 0000 720e 0000 0029 0172 1c00  .r....r....).r..
-00003940: 0000 2902 7299 0000 00da 0163 7235 0000  ..).r......cr5..
-00003950: 0072 3500 0000 7236 0000 0072 9c00 0000  .r5...r6...r....
-00003960: 2402 0000 f302 0000 0018 007a 2142 6172  $..........z!Bar
-00003970: 6368 6172 742e 6d61 6b65 2e3c 6c6f 6361  chart.make.<loca
-00003980: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 720d  ls>.<listcomp>r.
-00003990: 0000 0072 0e00 0000 da06 7369 6e67 6c65  ...r......single
-000039a0: e79a 9999 9999 99e9 3f29 02da 0870 7265  ........?)...pre
-000039b0: 7365 7276 6572 4b00 0000 2903 da08 706f  serverK...)...po
-000039c0: 7369 7469 6f6e 724b 0000 0072 1001 0000  sitionrK...r....
-000039d0: 7208 0000 0029 0272 e600 0000 7257 0100  r....).r....rW..
-000039e0: 0029 01da 066c 6162 656c 7372 0100 0000  .)...labelsr....
-000039f0: 7216 0100 00da 0577 6869 7465 679a 9999  r......whiteg...
-00003a00: 9999 99c9 3f72 1901 0000 da04 626f 6c64  ....?r......bold
-00003a10: da05 626c 6163 6be9 1400 0000 a903 da06  ..black.........
-00003a20: 7765 6967 6874 da05 636f 6c6f 7272 e600  weight..colorr..
-00003a30: 0000 a902 72e6 0000 0072 5f01 0000 da01  ....r....r_.....
-00003a40: 6229 0472 e600 0000 725e 0100 0072 5f01  b).r....r^...r_.
-00003a50: 0000 da06 6d61 7267 696e da01 6ce9 0500  ....margin..l...
-00003a60: 0000 2903 72e6 0000 0072 5f01 0000 7262  ..).r....r_...rb
-00003a70: 0100 00e9 0a00 0000 e91e 0000 0072 fa00  .............r..
-00003a80: 0000 6733 3333 3333 33eb 3f29 0267 cdcc  ..g333333.?).g..
-00003a90: cccc cccc ec3f 7255 0100 0029 0c72 1b01  .....?rU...).r..
-00003aa0: 0000 721c 0100 00da 0c61 7869 735f 7469  ..r......axis_ti
-00003ab0: 746c 655f 78da 0c61 7869 735f 7469 746c  tle_x..axis_titl
-00003ac0: 655f 79da 0b61 7869 735f 7465 7874 5f79  e_y..axis_text_y
-00003ad0: 5a0c 6c65 6765 6e64 5f74 6974 6c65 5a0b  Z.legend_titleZ.
-00003ae0: 6c65 6765 6e64 5f74 6578 745a 146c 6567  legend_textZ.leg
-00003af0: 656e 645f 656e 7472 795f 7370 6163 696e  end_entry_spacin
-00003b00: 675a 0f6c 6567 656e 645f 6b65 795f 7369  gZ.legend_key_si
-00003b10: 7a65 da0f 7375 6270 6c6f 7473 5f61 646a  ze..subplots_adj
-00003b20: 7573 74da 0f6c 6567 656e 645f 706f 7369  ust..legend_posi
-00003b30: 7469 6f6e 72c0 0000 0067 6666 6666 6666  tionr....gffffff
-00003b40: e6bf 2902 720f 0100 00da 056c 6162 656c  ..).r......label
-00003b50: 72fc 0000 0029 0372 5f01 0000 72e6 0000  r....).r_...r...
-00003b60: 00da 0276 61a9 0172 bc00 0000 6301 0000  ...va..r....c...
-00003b70: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00003b80: 0053 0000 0073 1800 0000 6700 7c00 5d08  .S...s....g.|.].
-00003b90: 7d01 6400 7c01 7600 7202 7c01 9102 7102  }.d.|.v.r.|...q.
-00003ba0: 5300 2901 5a08 436f 6e66 5f49 6e74 7235  S.).Z.Conf_Intr5
-00003bb0: 0000 0029 0272 9900 0000 7208 0100 0072  ...).r....r....r
-00003bc0: 3500 0000 7235 0000 0072 3600 0000 729c  5...r5...r6...r.
-00003bd0: 0000 0040 0200 0072 5301 0000 7244 0000  ...@...rS...rD..
-00003be0: 0072 5b00 0000 7a05 4d65 616e 2d7a 054d  .r[...z.Mean-z.M
-00003bf0: 6561 6e2b 7a07 6661 6374 6f72 28fa 0129  ean+z.factor(..)
-00003c00: 2905 7208 0100 0072 0f01 0000 da04 796d  ).r....r......ym
-00003c10: 696e da04 796d 6178 7212 0100 0029 0472  in..ymaxr....).r
-00003c20: 0801 0000 720f 0100 0072 7001 0000 7271  ....r....rp...rq
-00003c30: 0100 0029 0372 0801 0000 720f 0100 0072  ...).r....r....r
-00003c40: 1201 0000 5a0a 5f73 616d 655f 796c 696d  ....Z._same_ylim
-00003c50: 7239 0000 005a 0f44 6966 6665 7265 6e74  r9...Z.Different
-00003c60: 5f79 6178 6973 5a0a 5361 6d65 5f79 6178  _yaxisZ.Same_yax
-00003c70: 6973 5a08 6261 7263 6861 7274 2920 7271  isZ.barchart) rq
-00003c80: 0000 0072 0601 0000 7242 0100 0072 2401  ...r....rB...r$.
-00003c90: 0000 7266 0000 00da 0b43 6174 6567 6f72  ..rf.....Categor
-00003ca0: 6963 616c 72a6 0000 0072 7600 0000 721c  icalr....rv...r.
-00003cb0: 0000 00da 1573 696e 676c 655f 726f 695f  .....single_roi_
-00003cc0: 6669 675f 636f 6c6f 7572 7225 0100 0072  fig_colourr%...r
-00003cd0: 2801 0000 722f 0100 005a 0867 656f 6d5f  (...r/...Z.geom_
-00003ce0: 636f 6c5a 0e70 6f73 6974 696f 6e5f 646f  colZ.position_do
-00003cf0: 6467 655a 0d67 656f 6d5f 6572 726f 7262  dgeZ.geom_errorb
-00003d00: 6172 5a10 7363 616c 655f 785f 6469 7363  arZ.scale_x_disc
-00003d10: 7265 7465 7230 0100 0072 3201 0000 7233  reter0...r2...r3
-00003d20: 0100 00da 0c65 6c65 6d65 6e74 5f74 6578  .....element_tex
-00003d30: 7472 d200 0000 5a09 6765 6f6d 5f74 6578  tr....Z.geom_tex
-00003d40: 7472 2601 0000 5a11 7363 616c 655f 6669  tr&...Z.scale_fi
-00003d50: 6c6c 5f6d 616e 7561 6cda 2063 6f6c 6f72  ll_manual. color
-00003d60: 626c 696e 645f 6672 6965 6e64 6c79 5f70  blind_friendly_p
-00003d70: 6c6f 745f 636f 6c6f 7572 7372 ed00 0000  lot_coloursr....
-00003d80: da04 6c61 6273 da16 7369 6e67 6c65 5f72  ..labs..single_r
-00003d90: 6f69 5f66 6967 5f6c 6162 656c 5f78 da16  oi_fig_label_x..
-00003da0: 7369 6e67 6c65 5f72 6f69 5f66 6967 5f6c  single_roi_fig_l
-00003db0: 6162 656c 5f79 da19 7369 6e67 6c65 5f72  abel_y..single_r
-00003dc0: 6f69 5f66 6967 5f6c 6162 656c 5f66 696c  oi_fig_label_fil
-00003dd0: 6c72 2c01 0000 290b 723e 0000 0072 af00  lr,...).r>...r..
-00003de0: 0000 5a06 796c 696d 6974 da0d 7361 7665  ..Z.ylimit..save
-00003df0: 5f66 756e 6374 696f 6e5a 1266 696e 645f  _functionZ.find_
-00003e00: 796c 696d 5f66 756e 6374 696f 6e72 1300  ylim_functionr..
-00003e10: 0000 da0a 6375 7272 656e 745f 6466 723f  ....current_dfr?
-00003e20: 0000 005a 0f63 6f6e 665f 696e 745f 7374  ...Z.conf_int_st
-00003e30: 7269 6e67 5a0d 7265 7475 726e 6564 5f79  ringZ.returned_y
-00003e40: 6c69 6d72 5200 0000 7235 0000 0072 3500  limrR...r5...r5.
-00003e50: 0000 7236 0000 0072 2600 0000 1a02 0000  ..r6...r&.......
-00003e60: 7382 0000 0012 020e 020c 010c 0102 0104  s...............
-00003e70: 0102 ff04 010c fe12 0410 0110 0108 0306  ................
-00003e80: 0102 ff18 0202 fe16 0302 fd0a 0402 fc0e  ................
-00003e90: 050c 010e 010e 010c 0114 0112 0102 0102  ................
-00003ea0: 0106 0102 0104 0104 f502 fb12 1206 0104  ................
-00003eb0: ff02 ee0c 1402 ec02 ff16 180a 020c 0110  ................
-00003ec0: 010c 010a fe0c 0410 0108 ff0e 0304 0108  ................
-00003ed0: ff06 0310 0208 0104 020a 010c 0106 010a  ................
-00003ee0: 0104 0110 0204 027a 0d42 6172 6368 6172  .......z.Barchar
-00003ef0: 742e 6d61 6b65 4e29 0772 8700 0000 7288  t.makeN).r....r.
-00003f00: 0000 0072 8900 0000 728a 0000 0072 2b00  ...r....r....r+.
-00003f10: 0000 728b 0000 0072 2600 0000 7235 0000  ..r....r&...r5..
-00003f20: 0072 3500 0000 7235 0000 0072 3600 0000  .r5...r5...r6...
-00003f30: 722a 0000 00ef 0100 0073 0a00 0000 0800  r*.......s......
-00003f40: 0201 0a01 0229 0e01 722a 0000 0063 0000  .....)..r*...c..
-00003f50: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-00003f60: 0000 4000 0000 7330 0000 0065 005a 0164  ..@...s0...e.Z.d
-00003f70: 005a 0265 0364 0164 0284 0083 015a 0465  .Z.e.d.d.....Z.e
-00003f80: 0364 0364 0484 0083 015a 0565 0664 0564  .d.d.....Z.e.d.d
-00003f90: 0684 0083 015a 0764 0753 0029 0872 2c00  .....Z.d.S.).r,.
-00003fa0: 0000 6303 0000 0000 0000 0000 0000 000b  ..c.............
-00003fb0: 0000 000a 0000 0043 0000 0073 a401 0000  .......C...s....
-00003fc0: 7400 a001 6401 a101 0100 7402 7c01 6402  t...d.....t.|.d.
-00003fd0: 1900 a003 a100 8301 7d03 7400 6a04 7c03  ........}.t.j.|.
-00003fe0: 6403 7c00 6a05 6a06 6404 8d03 7d04 7a04  d.|.j.j.d...}.z.
-00003ff0: 7c04 0100 5700 6e15 0400 7407 7930 0100  |...W.n...t.y0..
-00004000: 0100 0100 7c00 6a05 6a08 722d 7409 6405  ....|.j.j.r-t.d.
-00004010: 8301 0100 5900 6400 5300 5900 6400 5300  ....Y.d.S.Y.d.S.
-00004020: 7700 7c00 6a05 6a08 7239 7409 6406 8301  w.|.j.j.r9t.d...
-00004030: 0100 6407 6408 8400 7400 a00a 6409 640a  ..d.d...t...d.d.
-00004040: a102 4400 8301 7d05 7c00 6a0b 7c00 6a05  ..D...}.|.j.|.j.
-00004050: 7c05 7c01 640b 640c 8d04 7d06 6700 7d07  |.|.d.d...}.g.}.
-00004060: 7c04 4400 5d0c 7d08 7c07 a00c 7c00 a00d  |.D.].}.|...|...
-00004070: 7c08 7c06 7c01 a103 a101 0100 7152 640d  |.|.|.......qRd.
-00004080: 7d09 0900 740e 740f a010 7c00 6a11 a101  }...t.t...|.j...
-00004090: 7c04 7c07 740f a010 7c09 a101 740f a010  |.|.t...|...t...
-000040a0: 7c00 6a12 a101 740f a010 7c00 6a13 a101  |.j...t...|.j...
-000040b0: 740f a010 7c00 6a05 a101 8307 7d0a 7c02  t...|.j.....}.|.
-000040c0: 7289 7c02 a014 7400 6a15 7c0a a102 7d09  r.|...t.j.|...}.
-000040d0: 6e09 7402 740f a014 7400 6a15 7c0a a102  n.t.t...t.j.|...
-000040e0: 8301 7d09 7416 7c09 8301 72cf 7a07 7c09  ..}.t.|...r.z.|.
-000040f0: a017 6400 a101 0100 5700 6e09 0400 7418  ..d.....W.n...t.
-00004100: 79a6 0100 0100 0100 5900 6e01 7700 7c09  y.......Y.n.w.|.
-00004110: 6a19 640f 6410 8400 6411 8d01 0100 7c00  j.d.d...d.....|.
-00004120: 6a05 6a08 72c8 7409 6412 741a 7c09 6413  j.j.r.t.d.t.|.d.
-00004130: 1900 6414 1900 8301 9b00 6415 7c09 6413  ..d.......d.|.d.
-00004140: 1900 6416 1900 9b00 6417 9d05 8301 0100  ..d.....d.......
-00004150: 7c09 6413 1900 6414 1900 7d09 6e02 6400  |.d...d...}.n.d.
-00004160: 5300 7162 2918 4e7a 1246 6967 7572 6573  S.qb).Nz.Figures
-00004170: 2f48 6973 746f 6772 616d 7372 f000 0000  /Histogramsr....
-00004180: 722c 0000 0072 3a01 0000 7a1c 536b 6970  r,...r:...z.Skip
-00004190: 7069 6e67 2068 6973 746f 6772 616d 2063  ping histogram c
-000041a0: 7265 6174 696f 6e2e 7a1b 0a2d 2d2d 2048  reation.z..--- H
-000041b0: 6973 746f 6772 616d 2063 7265 6174 696f  istogram creatio
-000041c0: 6e20 2d2d 2d63 0100 0000 0000 0000 0000  n ---c..........
-000041d0: 0000 0200 0000 0500 0000 5300 0000 731e  ..........S...s.
-000041e0: 0000 0067 007c 005d 0b7d 0174 00a0 01a1  ...g.|.].}.t....
-000041f0: 009b 0064 007c 019b 009d 0391 0271 0253  ...d.|.......q.S
-00004200: 0029 017a 152f 4f76 6572 616c 6c2f 5261  .).z./Overall/Ra
-00004210: 775f 7265 7375 6c74 732f 2902 7215 0000  w_results/).r...
-00004220: 0072 1600 0000 7298 0000 0072 3500 0000  .r....r....r5...
-00004230: 7235 0000 0072 3600 0000 729c 0000 0071  r5...r6...r....q
-00004240: 0200 0073 0200 0000 1e00 7a23 4869 7374  ...s......z#Hist
-00004250: 6f67 7261 6d2e 7365 7475 702e 3c6c 6f63  ogram.setup.<loc
-00004260: 616c 733e 2e3c 6c69 7374 636f 6d70 3e7a  als>.<listcomp>z
-00004270: 134f 7665 7261 6c6c 2f52 6177 5f72 6573  .Overall/Raw_res
-00004280: 756c 7473 726f 0000 0072 0500 0000 2901  ultsro...r....).
-00004290: 727f 0000 0072 0100 0000 5463 0100 0000  r....r....Tc....
-000042a0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-000042b0: 5300 0000 723d 0100 0072 3e01 0000 7235  S...r=...r>...r5
-000042c0: 0000 0072 0701 0000 7235 0000 0072 3500  ...r....r5...r5.
-000042d0: 0000 7236 0000 0072 0901 0000 8b02 0000  ..r6...r........
-000042e0: 723f 0100 007a 2148 6973 746f 6772 616d  r?...z!Histogram
-000042f0: 2e73 6574 7570 2e3c 6c6f 6361 6c73 3e2e  .setup.<locals>.
-00004300: 3c6c 616d 6264 613e 7240 0100 007a 144d  <lambda>r@...z.M
-00004310: 6178 696d 756d 2078 206c 696d 6974 206f  aximum x limit o
-00004320: 663a 2072 a400 0000 7208 0000 0072 4101  f: r....r....rA.
-00004330: 0000 725f 0000 007a 262e 2043 7265 6174  ..r_...z&. Creat
-00004340: 696e 6720 6669 6775 7265 7320 7769 7468  ing figures with
-00004350: 2074 6869 7320 7820 6c69 6d69 742e 0a29   this x limit..)
-00004360: 1b72 0900 0000 7228 0000 0072 6800 0000  .r....r(...rh...
-00004370: 72a6 0000 0072 4401 0000 7213 0000 0072  r....rD...r....r
-00004380: 4501 0000 7246 0100 0072 1e00 0000 721f  E...rF...r....r.
-00004390: 0000 00da 0a66 696e 645f 6669 6c65 7372  .....find_filesr
-000043a0: 8600 0000 72da 0000 00da 2767 6574 5f6d  ....r.....'get_m
-000043b0: 6561 6e5f 616e 645f 6d65 6469 616e 5f66  ean_and_median_f
-000043c0: 6f72 5f65 6163 685f 6368 6f73 656e 5f72  or_each_chosen_r
-000043d0: 6f69 7247 0100 0072 4801 0000 7249 0100  oirG...rH...rI..
-000043e0: 0072 2600 0000 7256 0000 0072 4300 0000  .r&...rV...rC...
-000043f0: 724a 0100 0072 4b01 0000 724c 0100 00da  rJ...rK...rL....
-00004400: 0672 656d 6f76 65da 0a56 616c 7565 4572  .remove..ValueEr
-00004410: 726f 7272 4d01 0000 72ae 0000 0029 0b72  rorrM...r....).r
-00004420: 2f00 0000 727e 0000 0072 3400 0000 724e  /...r~...r4...rN
-00004430: 0100 0072 4f01 0000 727d 0000 0072 8000  ...rO...r}...r..
-00004440: 0000 5a10 636f 6d62 696e 6564 5f72 6177  ..Z.combined_raw
-00004450: 5f64 6673 da03 726f 6972 2b01 0000 7250  _dfs..roir+...rP
-00004460: 0100 0072 3500 0000 7235 0000 0072 3600  ...r5...r5...r6.
-00004470: 0000 722b 0000 005f 0200 0073 5800 0000  ..r+..._...sX...
-00004480: 0a02 1002 0801 0601 06ff 0203 0801 0c01  ................
-00004490: 0801 0e01 06ff 02ff 0804 0801 0603 0a01  ................
-000044a0: 06ff 1402 0402 0801 0401 0c01 06ff 0403  ................
-000044b0: 0201 1001 1201 1401 04fe 0404 1001 1202  ................
-000044c0: 0802 0201 0e01 0c01 0401 02ff 1003 0802  ................
-000044d0: 2a01 0e03 0402 02e8 7a0f 4869 7374 6f67  *.......z.Histog
-000044e0: 7261 6d2e 7365 7475 7063 0400 0000 0000  ram.setupc......
-000044f0: 0000 0000 0000 0800 0000 0700 0000 4300  ..............C.
-00004500: 0000 732a 0100 007c 0164 016b 0272 0874  ..s*...|.d.k.r.t
-00004510: 00a0 01a1 0053 007c 0164 026b 0272 157c  .....S.|.d.k.r.|
-00004520: 02a0 02a1 007d 0464 027c 0464 033c 006e  .....}.d.|.d.<.n
-00004530: 0a7c 027c 0264 0319 007c 016b 0219 00a0  .|.|.d...|.k....
-00004540: 02a1 007d 047c 04a0 03a1 007d 047c 036a  ...}.|.....}.|.j
-00004550: 0464 0464 0369 0164 058d 017d 0374 0574  .d.d.i.d...}.t.t
-00004560: 0664 007c 006a 076a 087c 006a 076a 0967  .d.|.j.j.|.j.j.g
-00004570: 0283 0283 017d 057c 046a 0a7c 0364 0367  .....}.|.j.|.d.g
-00004580: 017c 05a2 0164 0664 078d 037d 0467 007c  .|...d.d...}.g.|
-00004590: 05a2 0164 0391 0164 0891 0164 0991 0164  ...d...d...d...d
-000045a0: 0a91 017d 067c 046a 0b44 005d 0c7d 077c  ...}.|.j.D.].}.|
-000045b0: 077c 0676 0172 5e7c 046a 0c7c 0764 058d  .|.v.r^|.j.|.d..
-000045c0: 017d 0471 5274 006a 0d7c 047c 0664 0064  .}.qRt.j.|.|.d.d
-000045d0: 0b85 0219 0064 0c64 0964 0a67 0264 0d64  .....d.d.d.g.d.d
-000045e0: 0e8d 057d 047c 006a 076a 0e72 827c 006a  ...}.|.j.j.r.|.j
-000045f0: 076a 0f73 827c 046a 107c 0464 0c19 0064  .j.s.|.j.|.d...d
-00004600: 096b 0219 007d 047c 0453 007c 006a 076a  .k...}.|.S.|.j.j
-00004610: 0f72 937c 006a 076a 0e73 937c 046a 107c  .r.|.j.j.s.|.j.|
-00004620: 0464 0c19 0064 0a6b 0219 007d 047c 0453  .d...d.k...}.|.S
-00004630: 0029 0f4e 7202 0100 0072 0101 0000 7260  .).Nr....r....r`
-00004640: 0000 0072 f000 0000 2901 7276 0000 0072  ...r....).rv...r
-00004650: f900 0000 2902 da02 6f6e da03 686f 7772  ....)...on..howr
-00004660: 6100 0000 725b 0000 0072 a100 0000 e9fe  a...r[...r......
-00004670: ffff ffda 0953 7461 7469 7374 6963 da0a  .....Statistic..
-00004680: 7374 6174 5f76 616c 7565 2904 7262 0000  stat_value).rb..
-00004690: 0072 6300 0000 da0a 7661 6c75 655f 7661  .rc.....value_va
-000046a0: 7273 7264 0000 0029 1172 6600 0000 7267  rsrd...).rf...rg
-000046b0: 0000 0072 1e01 0000 727c 0000 00da 0672  ...r....r|.....r
-000046c0: 656e 616d 6572 6800 0000 7269 0000 0072  enamerh...ri...r
-000046d0: 1300 0000 726b 0000 0072 6c00 0000 da05  ....rk...rl.....
-000046e0: 6d65 7267 6572 7600 0000 720c 0100 0072  mergerv...r....r
-000046f0: 7b00 0000 da13 6869 7374 6f67 7261 6d5f  {.....histogram_
-00004700: 7368 6f77 5f6d 6561 6eda 1568 6973 746f  show_mean..histo
-00004710: 6772 616d 5f73 686f 775f 6d65 6469 616e  gram_show_median
-00004720: 7271 0000 0029 0872 2f00 0000 723e 0000  rq...).r/...r>..
-00004730: 0072 8000 0000 727e 0000 0072 7b01 0000  .r....r~...r{...
-00004740: 7281 0000 0072 ed00 0000 7285 0000 0072  r....r....r....r
-00004750: 3500 0000 7235 0000 0072 3600 0000 727d  5...r5...r6...r}
-00004760: 0100 0095 0200 0073 3a00 0000 0804 0801  .......s:.......
-00004770: 0801 0801 0a01 1402 0802 0403 0601 06ff  ................
-00004780: 1a04 0601 0801 0201 06fe 1805 0a02 0801  ................
-00004790: 0c01 0280 1202 0801 06ff 1003 1201 0404  ................
-000047a0: 10fd 1201 0402 7a31 4869 7374 6f67 7261  ......z1Histogra
-000047b0: 6d2e 6765 745f 6d65 616e 5f61 6e64 5f6d  m.get_mean_and_m
-000047c0: 6564 6961 6e5f 666f 725f 6561 6368 5f63  edian_for_each_c
-000047d0: 686f 7365 6e5f 726f 6963 0600 0000 0000  hosen_roic......
-000047e0: 0000 0000 0000 0900 0000 1000 0000 4300  ..............C.
-000047f0: 0000 73f8 0100 007c 016a 0072 0c7c 056a  ..s....|.j.r.|.j
-00004800: 0172 0a74 0264 0183 0101 0064 0053 0074  .r.t.d.....d.S.t
-00004810: 03a0 047c 0174 036a 0564 0264 038d 01a1  ...|.t.j.d.d....
-00004820: 0274 03a0 06a1 0017 0074 036a 077c 056a  .t.......t.j.|.j
-00004830: 087c 056a 0964 0464 0564 068d 0417 0074  .|.j.d.d.d.....t
-00004840: 036a 0a7c 056a 0b9b 0064 077c 056a 0c9b  .j.|.j...d.|.j..
-00004850: 009d 0364 0564 0864 098d 0317 0074 036a  ...d.d.d.....t.j
-00004860: 0d7c 056a 0e7c 056a 0f64 0a8d 0217 0074  .|.j.|.j.d.....t
-00004870: 036a 1074 036a 116a 1264 0464 0b8d 0174  .j.t.j.j.d.d...t
-00004880: 036a 116a 1264 0c64 0b8d 0174 036a 1264  .j.j.d.d...t.j.d
-00004890: 0464 0b8d 0174 036a 1364 0d64 0e8d 0174  .d...t.j.d.d...t
-000048a0: 036a 1364 0f64 1064 118d 0274 036a 1464  .j.d.d.d...t.j.d
-000048b0: 1264 1364 1464 158d 0374 036a 1464 1264  .d.d.d...t.j.d.d
-000048c0: 1364 1464 158d 0374 036a 1464 1264 1664  .d.d...t.j.d.d.d
-000048d0: 1364 178d 0374 036a 1464 1264 1664 1364  .d...t.j.d.d.d.d
-000048e0: 178d 0374 036a 1464 1664 1364 188d 0274  ...t.j.d.d.d...t
-000048f0: 036a 1464 1664 1364 188d 027c 056a 1564  .j.d.d.d...|.j.d
-00004900: 198d 0c17 007d 067c 056a 1673 8e7c 056a  .....}.|.j.s.|.j
-00004910: 1772 ad7c 0674 036a 1874 036a 0564 1a64  .r.|.t.j.t.j.d.d
-00004920: 1b64 1c8d 027c 056a 1964 1d8d 0237 007d  .d...|.j.d...7.}
-00004930: 067c 0674 036a 1a7c 056a 1b64 1e19 007c  .|.t.j.|.j.d...|
-00004940: 056a 1b64 0c19 0067 0264 1f8d 0137 007d  .j.d...g.d...7.}
-00004950: 067c 056a 1c73 b87c 0674 036a 1064 2064  .|.j.s.|.t.j.d d
-00004960: 218d 0137 007d 067c 0272 c77c 0674 03a0  !..7.}.|.r.|.t..
-00004970: 1d64 227c 02a1 0237 007d 067c 0064 2337  .d"|...7.}.|.d#7
-00004980: 007d 006e 087c 0674 03a0 1d64 2264 00a1  .}.n.|.t...d"d..
-00004990: 0237 007d 0664 047d 077c 0264 046b 0272  .7.}.d.}.|.d.k.r
-000049a0: de7c 047c 007c 0664 2483 037d 0764 257d  .|.|.|.d$..}.d%}
-000049b0: 086e 067c 0264 046b 0372 e464 267d 0874  .n.|.d.k.r.d&}.t
-000049c0: 1e6a 1f64 2774 2064 288d 0201 007c 037c  .j.d't d(....|.|
-000049d0: 067c 007c 0864 297c 0583 0501 0074 1e6a  .|.|.d)|.....t.j
-000049e0: 1f64 2a74 2064 288d 0201 007c 0753 0029  .d*t d(....|.S.)
-000049f0: 2b4e 7a38 494e 464f 3a20 4869 7374 6f67  +Nz8INFO: Histog
-00004a00: 7261 6d73 2063 616e 6e6f 7420 6265 206d  rams cannot be m
-00004a10: 6164 6520 666f 7220 7468 6520 4e6f 2052  ade for the No R
-00004a20: 4f49 2063 6174 6567 6f72 792e 7261 0000  OI category.ra..
-00004a30: 0072 0701 0000 7201 0000 0054 2904 da08  .r....r....T)...
-00004a40: 6269 6e77 6964 7468 7212 0100 00da 0862  binwidthr......b
-00004a50: 6f75 6e64 6172 7972 1001 0000 7213 0100  oundaryr....r...
-00004a60: 0072 1401 0000 7215 0100 0072 0e01 0000  .r....r....r....
-00004a70: 7216 0100 0072 0800 0000 7259 0100 00a9  r....r....rY....
-00004a80: 0172 1201 0000 7218 0100 0072 a000 0000  .r....r....r....
-00004a90: 7219 0100 0072 5a01 0000 725b 0100 0072  r....rZ...r[...r
-00004aa0: 5c01 0000 725d 0100 0072 6501 0000 a903  \...r]...re.....
-00004ab0: 725e 0100 0072 e600 0000 725f 0100 0072  r^...r....r_...r
-00004ac0: 6001 0000 a90c 5a12 7061 6e65 6c5f 6772  `.....Z.panel_gr
-00004ad0: 6964 5f6d 696e 6f72 5f78 721b 0100 0072  id_minor_xr....r
-00004ae0: 1a01 0000 5a0f 706c 6f74 5f62 6163 6b67  ....Z.plot_backg
-00004af0: 726f 756e 6472 1c01 0000 7267 0100 0072  roundr....rg...r
-00004b00: 6801 0000 5a0c 7374 7269 705f 7465 7874  h...Z.strip_text
-00004b10: 5f78 5a0c 7374 7269 705f 7465 7874 5f79  _xZ.strip_text_y
-00004b20: 721d 0100 0072 6901 0000 72c0 0000 0072  r....ri...r....r
-00004b30: 8501 0000 7284 0100 0029 025a 0a78 696e  ....r....).Z.xin
-00004b40: 7465 7263 6570 7472 5f01 0000 2901 72e6  terceptr_...).r.
-00004b50: 0000 0072 4800 0000 726e 0100 00da 046e  ...rH...rn.....n
-00004b60: 6f6e 6529 0172 6b01 0000 72a4 0000 005a  one).rk...r....Z
-00004b70: 0a5f 7361 6d65 5f78 6c69 6d72 3800 0000  ._same_xlimr8...
-00004b80: 5a0f 4469 6666 6572 656e 745f 7861 7869  Z.Different_xaxi
-00004b90: 735a 0a53 616d 655f 7861 7869 73da 0669  sZ.Same_xaxis..i
-00004ba0: 676e 6f72 6529 02da 0661 6374 696f 6eda  gnore)...action.
-00004bb0: 0863 6174 6567 6f72 79da 0968 6973 746f  .category..histo
-00004bc0: 6772 616d da07 6465 6661 756c 7429 21da  gram..default)!.
-00004bd0: 0565 6d70 7479 721e 0000 0072 1f00 0000  .emptyr....r....
-00004be0: 7225 0100 0072 2801 0000 7226 0100 0072  r%...r(...r&...r
-00004bf0: 2f01 0000 5a0e 6765 6f6d 5f68 6973 746f  /...Z.geom_histo
-00004c00: 6772 616d da12 6869 7374 6f67 7261 6d5f  gram..histogram_
-00004c10: 6269 6e77 6964 7468 da14 6869 7374 6f67  binwidth..histog
-00004c20: 7261 6d5f 6669 675f 636f 6c6f 7572 722e  ram_fig_colourr.
-00004c30: 0100 0072 6c00 0000 726b 0000 0072 7601  ...rl...rk...rv.
-00004c40: 0000 da15 6869 7374 6f67 7261 6d5f 6669  ....histogram_fi
-00004c50: 675f 6c61 6265 6c5f 78da 1568 6973 746f  g_label_x..histo
-00004c60: 6772 616d 5f66 6967 5f6c 6162 656c 5f79  gram_fig_label_y
-00004c70: 7230 0100 0072 3101 0000 7232 0100 0072  r0...r1...r2...r
-00004c80: 3301 0000 7274 0100 0072 d200 0000 7289  3...rt...r....r.
-00004c90: 0100 0072 8a01 0000 5a0a 6765 6f6d 5f76  ...r....Z.geom_v
-00004ca0: 6c69 6e65 da18 6869 7374 6f67 7261 6d5f  line..histogram_
-00004cb0: 7374 6174 5f6c 696e 655f 7369 7a65 5a12  stat_line_sizeZ.
-00004cc0: 7363 616c 655f 636f 6c6f 725f 6d61 6e75  scale_color_manu
-00004cd0: 616c 7275 0100 00da 1568 6973 746f 6772  alru.....histogr
-00004ce0: 616d 5f73 686f 775f 6c65 6765 6e64 722b  am_show_legendr+
-00004cf0: 0100 00da 0877 6172 6e69 6e67 73da 0c73  .....warnings..s
-00004d00: 696d 706c 6566 696c 7465 72da 0d46 7574  implefilter..Fut
-00004d10: 7572 6557 6172 6e69 6e67 2909 723e 0000  ureWarning).r>..
-00004d20: 0072 8000 0000 5a06 786c 696d 6974 727a  .r....Z.xlimitrz
-00004d30: 0100 005a 1266 696e 645f 786c 696d 5f66  ...Z.find_xlim_f
-00004d40: 756e 6374 696f 6e72 1300 0000 723f 0000  unctionr....r?..
-00004d50: 005a 0d72 6574 7572 6e65 645f 786c 696d  .Z.returned_xlim
-00004d60: 7252 0000 0072 3500 0000 7235 0000 0072  rR...r5...r5...r
-00004d70: 3600 0000 7226 0000 00be 0200 0073 7200  6...r&.......sr.
-00004d80: 0000 0602 0601 0801 0401 1203 0601 02ff  ................
-00004d90: 0c02 0201 0201 04fe 02fe 1405 0401 04ff  ................
-00004da0: 02fb 1007 02f9 0408 0c01 0c01 0a01 0a01  ................
-00004db0: 0c01 0e01 0e01 0e01 0e01 0c01 0c01 0401  ................
-00004dc0: 04f4 02f8 02ff 0c1a 1201 0401 08ff 0e02  ................
-00004dd0: 0801 0aff 0604 1001 0402 1002 0a01 1002  ................
-00004de0: 0402 0801 0c01 0601 0801 0401 0e03 1002  ................
-00004df0: 0e02 0402 7a0e 4869 7374 6f67 7261 6d2e  ....z.Histogram.
-00004e00: 6d61 6b65 4e29 0872 8700 0000 7288 0000  makeN).r....r...
-00004e10: 0072 8900 0000 728a 0000 0072 2b00 0000  .r....r....r+...
-00004e20: 727d 0100 0072 8b00 0000 7226 0000 0072  r}...r....r&...r
-00004e30: 3500 0000 7235 0000 0072 3500 0000 7236  5...r5...r5...r6
-00004e40: 0000 0072 2c00 0000 5e02 0000 730e 0000  ...r,...^...s...
-00004e50: 0008 0002 010a 0102 350a 0102 280e 0172  ........5...(..r
-00004e60: 2c00 0000 6300 0000 0000 0000 0000 0000  ,...c...........
-00004e70: 0000 0000 0003 0000 0040 0000 0073 3400  .........@...s4.
-00004e80: 0000 6500 5a01 6400 5a02 6401 5a03 6504  ..e.Z.d.Z.d.Z.e.
-00004e90: 6402 6403 8400 8301 5a05 6504 6404 6405  d.d.....Z.e.d.d.
-00004ea0: 8400 8301 5a06 6504 6406 6407 8400 8301  ....Z.e.d.d.....
-00004eb0: 5a07 6401 5300 2908 da0e 436f 6d70 6172  Z.d.S.)...Compar
-00004ec0: 654f 7574 7075 7473 4e63 0200 0000 0000  eOutputsNc......
-00004ed0: 0000 0000 0000 0400 0000 0500 0000 4300  ..............C.
-00004ee0: 0000 7320 0000 007c 00a0 007c 01a1 015c  ..s ...|...|...\
-00004ef0: 027d 027d 037c 00a0 017c 027c 037c 01a1  .}.}.|...|.|.|..
-00004f00: 0301 0064 0053 0029 014e 2902 da08 7365  ...d.S.).N)...se
-00004f10: 7475 705f 6466 da0c 4d61 6b65 5f73 6361  tup_df..Make_sca
-00004f20: 7474 6572 2904 722f 0000 0072 1300 0000  tter).r/...r....
-00004f30: 72af 0000 0072 5801 0000 7235 0000 0072  r....rX...r5...r
-00004f40: 3500 0000 7236 0000 00da 0372 756e 0403  5...r6.....run..
-00004f50: 0000 7304 0000 000e 0212 017a 1243 6f6d  ..s........z.Com
-00004f60: 7061 7265 4f75 7470 7574 732e 7275 6e63  pareOutputs.runc
-00004f70: 0200 0000 0000 0000 0000 0000 0a00 0000  ................
-00004f80: 0900 0000 4300 0000 73b8 0000 0069 007d  ....C...s....i.}
-00004f90: 0267 007d 0374 0064 0183 0144 005d 3e7d  .g.}.t.d...D.]>}
-00004fa0: 0474 016a 0264 0264 038d 017d 0574 037c  .t.j.d.d...}.t.|
-00004fb0: 059b 0064 049d 0264 0583 028f 267d 0674  ...d...d....&}.t
-00004fc0: 04a0 057c 06a1 017d 0774 06a0 077c 07a1  ...|...}.t...|..
-00004fd0: 017c 027c 043c 007c 03a0 0874 096a 0aa0  .|.|.<.|...t.j..
-00004fe0: 0b7c 05a1 01a1 0101 0074 0c64 0664 0784  .|.......t.d.d..
-00004ff0: 007c 0744 0083 0183 017d 0857 0064 0004  .|.D.....}.W.d..
-00005000: 0004 0083 0301 0071 0831 0073 4177 0101  .......q.1.sAw..
-00005010: 0001 0001 0059 0001 0071 087c 0264 0819  .....Y...q.|.d..
-00005020: 006a 0d7c 0264 0919 0064 0a64 0b7c 016a  .j.|.d...d.d.|.j
-00005030: 0e7c 016a 0f67 0364 0c8d 037d 097c 097c  .|.j.g.d...}.|.|
-00005040: 0366 0253 0029 0d4e 725f 0000 007a 2753  .f.S.).Nr_...z'S
-00005050: 656c 6563 7420 7468 6520 6469 7265 6374  elect the direct
-00005060: 6f72 7920 6f75 7470 7574 2062 7920 7468  ory output by th
-00005070: 6520 6652 4154 2901 724f 0000 007a 292f  e fRAT).rO...z)/
-00005080: 5375 6d6d 6172 6973 6564 5f72 6573 756c  Summarised_resul
-00005090: 7473 2f63 6f6d 6269 6e65 645f 7265 7375  ts/combined_resu
-000050a0: 6c74 732e 6a73 6f6e 725a 0000 0063 0100  lts.jsonrZ...c..
-000050b0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-000050c0: 0000 5300 0000 7314 0000 0068 007c 005d  ..S...s....h.|.]
-000050d0: 067d 017c 0164 0019 0092 0271 0253 0029  .}.|.d.....q.S.)
-000050e0: 0172 f000 0000 7235 0000 0029 0272 9900  .r....r5...).r..
-000050f0: 0000 da01 6472 3500 0000 7235 0000 0072  ....dr5...r5...r
-00005100: 3600 0000 da09 3c73 6574 636f 6d70 3e15  6.....<setcomp>.
-00005110: 0300 0072 eb00 0000 7a2a 436f 6d70 6172  ...r....z*Compar
-00005120: 654f 7574 7075 7473 2e73 6574 7570 5f64  eOutputs.setup_d
-00005130: 662e 3c6c 6f63 616c 733e 2e3c 7365 7463  f.<locals>.<setc
-00005140: 6f6d 703e 7201 0000 0072 0800 0000 da05  omp>r....r......
-00005150: 6f75 7465 7272 f000 0000 2902 7282 0100  outerr....).r...
-00005160: 0072 8101 0000 2910 da05 7261 6e67 6572  .r....)...ranger
-00005170: 0900 0000 da0c 6669 6c65 5f62 726f 7773  ......file_brows
-00005180: 6572 726d 0000 0072 6f00 0000 7270 0000  errm...ro...rp..
-00005190: 0072 6600 0000 7267 0000 0072 da00 0000  .rf...rg...r....
-000051a0: 7215 0000 0072 1800 0000 7273 0000 0072  r....r....rs...r
-000051b0: ad00 0000 7288 0100 0072 6c00 0000 726b  ....r....rl...rk
-000051c0: 0000 0029 0a72 2f00 0000 7213 0000 00da  ...).r/...r.....
-000051d0: 0364 6673 7258 0100 0072 0801 0000 da09  .dfsrX...r......
-000051e0: 6469 7265 6374 6f72 79da 0772 6573 756c  directory..resul
-000051f0: 7473 da04 6461 7461 5a04 726f 6973 5a03  ts..dataZ.roisZ.
-00005200: 6466 6d72 3500 0000 7235 0000 0072 3600  dfmr5...r5...r6.
-00005210: 0000 72a1 0100 0009 0300 0073 1c00 0000  ..r........s....
-00005220: 0402 0401 0c01 0c01 1202 0a01 0e01 1201  ................
-00005230: 1402 1efb 1007 0c01 06ff 0803 7a17 436f  ............z.Co
-00005240: 6d70 6172 654f 7574 7075 7473 2e73 6574  mpareOutputs.set
-00005250: 7570 5f64 6663 0400 0000 0000 0000 0000  up_dfc..........
-00005260: 0000 0500 0000 1000 0000 4300 0000 731c  ..........C...s.
-00005270: 0100 0074 00a0 017c 0174 006a 0264 0164  ...t...|.t.j.d.d
-00005280: 0264 038d 02a1 0274 00a0 03a1 0017 0074  .d.....t.......t
-00005290: 00a0 04a1 0017 0074 006a 057c 036a 069b  .......t.j.|.j..
-000052a0: 0064 047c 036a 079b 009d 0364 0564 0664  .d.|.j.....d.d.d
-000052b0: 078d 0317 0074 006a 0864 0864 098d 0117  .....t.j.d.d....
-000052c0: 0074 006a 097c 0264 0a19 007c 0264 0b19  .t.j.|.d...|.d..
-000052d0: 0064 038d 0217 0074 006a 0a74 006a 0b6a  .d.....t.j.t.j.j
-000052e0: 0c64 0b64 0c8d 0174 006a 0b6a 0c64 0a64  .d.d...t.j.j.d.d
-000052f0: 0c8d 0174 006a 0c64 0b64 0c8d 0174 006a  ...t.j.d.d...t.j
-00005300: 0d64 0d64 0e8d 0174 006a 0d64 0f64 1064  .d.d...t.j.d.d.d
-00005310: 118d 0274 006a 0e64 1264 1364 1464 158d  ...t.j.d.d.d.d..
-00005320: 0374 006a 0e64 1264 1364 1464 158d 0374  .t.j.d.d.d.d...t
-00005330: 006a 0e64 1264 1664 1364 178d 0374 006a  .j.d.d.d.d...t.j
-00005340: 0e64 1264 1664 1364 178d 0374 006a 0e64  .d.d.d.d...t.j.d
-00005350: 1664 1364 188d 0274 006a 0e64 1664 1364  .d.d...t.j.d.d.d
-00005360: 188d 027c 036a 0f64 198d 0c17 007d 047c  ...|.j.d.....}.|
-00005370: 046a 1064 1a7c 036a 117c 036a 1164 1b14  .j.d.|.j.|.j.d..
-00005380: 0064 1c64 1c64 1d8d 0501 0064 0053 0029  .d.d.d.....d.S.)
-00005390: 1e4e 5a06 4d65 616e 5f78 5a06 4d65 616e  .NZ.Mean_xZ.Mean
-000053a0: 5f79 720e 0100 0072 1301 0000 5472 1401  _yr....r....Tr..
-000053b0: 0000 7215 0100 00da 026c 6d29 01da 066d  ..r......lm)...m
-000053c0: 6574 686f 6472 0800 0000 7201 0000 0072  ethodr....r....r
-000053d0: 1601 0000 7259 0100 0072 8d01 0000 7218  ....rY...r....r.
-000053e0: 0100 0072 a000 0000 7219 0100 0072 5a01  ...r....r....rZ.
-000053f0: 0000 725b 0100 0072 5c01 0000 725d 0100  ..r[...r\...r]..
-00005400: 0072 6501 0000 728e 0100 0072 6001 0000  .re...r....r`...
-00005410: 728f 0100 007a 0854 4553 542e 706e 6772  r....z.TEST.pngr
-00005420: 4800 0000 4672 4900 0000 2912 7225 0100  H...FrI...).r%..
-00005430: 0072 2801 0000 7226 0100 0072 2f01 0000  .r(...r&...r/...
-00005440: 7236 0100 0072 2e01 0000 726c 0000 0072  r6...r....rl...r
-00005450: 6b00 0000 5a0b 6765 6f6d 5f73 6d6f 6f74  k...Z.geom_smoot
-00005460: 6872 7601 0000 7230 0100 0072 3101 0000  hrv...r0...r1...
-00005470: 7232 0100 0072 3301 0000 7274 0100 0072  r2...r3...rt...r
-00005480: d200 0000 7250 0000 0072 5100 0000 2905  ....rP...rQ...).
-00005490: 722f 0000 0072 af00 0000 7258 0100 0072  r/...r....rX...r
-000054a0: 1300 0000 723f 0000 0072 3500 0000 7235  ....r?...r5...r5
-000054b0: 0000 0072 3600 0000 72a2 0100 001c 0300  ...r6...r.......
-000054c0: 0073 4200 0000 1403 0601 02ff 0602 02fe  .sB.............
-000054d0: 1403 0401 04ff 02fd 0a05 02fb 1406 02fa  ................
-000054e0: 0407 0c01 0c01 0a01 0a01 0c01 0e01 0e01  ................
-000054f0: 0e01 0e01 0c01 0c01 0401 04f4 02f9 02ff  ................
-00005500: 0a18 0801 0401 0afe 7a1b 436f 6d70 6172  ........z.Compar
-00005510: 654f 7574 7075 7473 2e4d 616b 655f 7363  eOutputs.Make_sc
-00005520: 6174 7465 7229 0872 8700 0000 7288 0000  atter).r....r...
-00005530: 0072 8900 0000 727b 0100 0072 8a00 0000  .r....r{...r....
-00005540: 72a3 0100 0072 a101 0000 72a2 0100 0072  r....r....r....r
-00005550: 3500 0000 7235 0000 0072 3500 0000 7236  5...r5...r5...r6
-00005560: 0000 0072 a001 0000 0103 0000 7310 0000  ...r........s...
-00005570: 0008 0004 0102 020a 0102 040a 0102 120e  ................
-00005580: 0172 a001 0000 2924 721e 0100 0072 4801  .r....)$r....rH.
-00005590: 0000 7215 0000 0072 4d00 0000 729d 0100  ..r....rM...r...
-000055a0: 0072 0300 0000 da07 7061 7468 6c69 6272  .r......pathlibr
-000055b0: 0400 0000 da10 6d61 7470 6c6f 746c 6962  ......matplotlib
-000055c0: 2e69 6d61 6765 da05 696d 6167 6572 c300  .image..imager..
-000055d0: 0000 da05 6e75 6d70 7972 de00 0000 da07  ....numpyr......
-000055e0: 6e69 6261 6265 6c72 dc00 0000 da06 7061  nibabelr......pa
-000055f0: 6e64 6173 7266 0000 005a 0870 6c6f 746e  ndasrf...Z.plotn
-00005600: 696e 6572 2501 0000 da0a 7369 6d70 6c65  iner%.....simple
-00005610: 6a73 6f6e 726f 0000 00da 076e 696c 6561  jsonro.....nilea
-00005620: 726e 7205 0000 00da 0a6d 6174 706c 6f74  rnr......matplot
-00005630: 6c69 6272 0600 0000 72a8 0000 00da 0350  libr....r......P
-00005640: 494c 7207 0000 00da 0575 7469 6c73 7209  ILr......utilsr.
-00005650: 0000 0072 0a00 0000 7225 0000 0072 2900  ...r....r%...r).
-00005660: 0000 722a 0000 0072 2c00 0000 72a0 0100  ..r*...r,...r...
-00005670: 0072 3500 0000 7235 0000 0072 3500 0000  .r5...r5...r5...
-00005680: 7236 0000 00da 083c 6d6f 6475 6c65 3e01  r6.....<module>.
-00005690: 0000 0073 3600 0000 0800 0801 0801 0801  ...s6...........
-000056a0: 0801 0c01 0c01 0c02 0801 0801 0801 0801  ................
-000056b0: 0801 0c01 0c01 0c01 0c02 0e03 007f 1012  ................
-000056c0: 007f 007f 100b 103f 106f 007f 1424       .......?.o...$
+00001e30: 0ea0 12a1 0001 0074 13a0 147c 0aa1 018f  .......t...|....
+00001e40: 0d7d 0f7c 0f6a 155c 027d 107d 1157 0064  .}.|.j.\.}.}.W.d
+00001e50: 0004 0004 0083 0301 006e 0831 0073 8777  .........n.1.s.w
+00001e60: 0101 0001 0001 0059 0001 007c 0a7c 077c  .......Y...|.|.|
+00001e70: 107c 1166 0266 0353 0029 0e4e 720e 0000  .|.f.f.S.).Nr...
+00001e80: 0072 4700 0000 728c 0000 0072 4600 0000  .rG...r....rF...
+00001e90: 728e 0000 0072 a300 0000 72a4 0000 0046  r....r....r....F
+00001ea0: 54da 0278 7ada 0769 6e66 6572 6e6f 2908  T..xz..inferno).
+00001eb0: 5a0a 6472 6177 5f63 726f 7373 5a08 616e  Z.draw_crossZ.an
+00001ec0: 6e6f 7461 7465 da08 636f 6c6f 7262 6172  notate..colorbar
+00001ed0: 5a0c 6469 7370 6c61 795f 6d6f 6465 72b8  Z.display_moder.
+00001ee0: 0000 0072 b600 0000 5a0a 6375 745f 636f  ...r....Z.cut_co
+00001ef0: 6f72 6473 da04 636d 6170 2901 72c0 0000  ords..cmap).r...
+00001f00: 0029 16da 0661 7070 656e 64da 0466 696e  .)...append..fin
+00001f10: 64da 036e 6962 7270 0000 00da 0967 6574  d..nibrp.....get
+00001f20: 5f66 6461 7461 da02 6e70 da06 6e61 6e6d  _fdata..np..nanm
+00001f30: 6178 da0b 4e69 6674 6931 496d 6167 65da  ax..Nifti1Image.
+00001f40: 0a6e 616e 5f74 6f5f 6e75 6dda 0661 6666  .nan_to_num..aff
+00001f50: 696e 65da 0668 6561 6465 7272 0500 0000  ine..headerr....
+00001f60: 5a09 706c 6f74 5f61 6e61 7472 1300 0000  Z.plot_anatr....
+00001f70: da0d 6272 6169 6e5f 785f 636f 6f72 64da  ..brain_x_coord.
+00001f80: 0d62 7261 696e 5f7a 5f63 6f6f 7264 72d1  .brain_z_coordr.
+00001f90: 0000 0072 d200 0000 722d 0000 0072 0700  ...r....r-...r..
+00001fa0: 0000 726d 0000 00da 0473 697a 6529 1272  ..rm.....size).r
+00001fb0: 2f00 0000 726f 0000 0072 b000 0000 7295  /...ro...r....r.
+00001fc0: 0000 0072 b600 0000 72b7 0000 0072 b800  ...r....r....r..
+00001fd0: 0000 7296 0000 0072 9400 0000 7293 0000  ..r....r....r...
+00001fe0: 005a 0870 6e67 5f70 6174 685a 0a6e 6966  .Z.png_pathZ.nif
+00001ff0: 7469 5f70 6174 68da 0562 7261 696e 7297  ti_path..brainr.
+00002000: 0000 00da 0470 6c6f 74da 0269 6d72 4b00  .....plot..imrK.
+00002010: 0000 724a 0000 0072 3500 0000 7235 0000  ..rJ...r5...r5..
+00002020: 0072 3600 0000 72c2 0000 0035 0100 0073  .r6...r....5...s
+00002030: 2c00 0000 1004 0a01 1402 1e02 0a02 0801  ,...............
+00002040: 0a02 1404 0a03 1c01 0602 0801 0401 0e01  ................
+00002050: 0201 06fc 1205 0801 0c02 0c01 1cff 0e03  ................
+00002060: 7a19 4272 6169 6e47 7269 642e 7361 7665  z.BrainGrid.save
+00002070: 5f62 7261 696e 5f69 6d67 7363 0200 0000  _brain_imgsc....
+00002080: 0000 0000 0000 0000 1100 0000 0800 0000  ................
+00002090: 4300 0000 73be 0100 0067 007d 0267 007d  C...s....g.}.g.}
+000020a0: 037c 006a 006a 0144 005d 187d 0474 0274  .|.j.j.D.].}.t.t
+000020b0: 037c 017c 0419 00a0 04a1 0083 0183 017d  .|.|...........}
+000020c0: 0564 0164 0284 007c 0544 0083 017d 057c  .d.d...|.D...}.|
+000020d0: 02a0 057c 05a1 0101 0071 087c 027d 0674  ...|.....q.|.}.t
+000020e0: 037c 006a 006a 01a0 06a1 0083 017d 077c  .|.j.j.......}.|
+000020f0: 006a 006a 0764 0367 0167 0064 049c 037c  .j.j.d.g.g.d...|
+00002100: 006a 006a 0864 0367 0167 0064 049c 0364  .j.j.d.g.g.d...d
+00002110: 059c 027d 087c 0844 005d 1a7d 097c 087c  ...}.|.D.].}.|.|
+00002120: 0919 0064 0619 0064 076b 0272 4b71 407c  ...d...d.k.rKq@|
+00002130: 067c 07a0 097c 087c 0919 0064 0619 00a1  .|...|.|...d....
+00002140: 0119 007c 087c 0919 0064 083c 0071 4074  ...|.|...d.<.q@t
+00002150: 0a7c 0864 0919 0064 0819 0083 017d 0a74  .|.d...d.....}.t
+00002160: 0a7c 0864 0a19 0064 0819 0083 017d 0b74  .|.d...d.....}.t
+00002170: 0b7c 0164 0b19 00a0 04a1 0083 0144 005d  .|.d.........D.]
+00002180: 655c 027d 0c7d 0d67 007d 0e7c 017c 0164  e\.}.}.g.}.|.|.d
+00002190: 0b19 007c 0d6b 0219 006a 0c64 0319 007d  ...|.k...j.d...}
+000021a0: 0f7c 0844 005d 407d 097c 087c 0919 0064  .|.D.]@}.|.|...d
+000021b0: 0819 0064 0367 016b 0372 b874 0d7c 0f7c  ...d.g.k.r.t.|.|
+000021c0: 087c 0919 0064 0619 0019 0083 017d 107c  .|...d.......}.|
+000021d0: 087c 0919 0064 0c19 00a0 057c 087c 0919  .|...d.....|.|..
+000021e0: 0064 0819 00a0 097c 10a1 01a1 0101 007c  .d.....|.......|
+000021f0: 0ea0 057c 087c 0919 0064 0819 00a0 097c  ...|.|...d.....|
+00002200: 10a1 01a1 0101 0071 867c 087c 0919 0064  .......q.|.|...d
+00002210: 0c19 00a0 0564 03a1 0101 007c 0ea0 0564  .....d.....|...d
+00002220: 03a1 0101 0071 867c 03a0 0574 0ea0 0f7c  .....q.|...t...|
+00002230: 0e64 0d19 007c 0e64 0319 0066 027c 0b7c  .d...|.d...f.|.|
+00002240: 0a66 02a1 02a1 0101 0071 737c 087c 037c  .f.......qs|.|.|
+00002250: 0b7c 0a66 0453 0029 0e4e 6301 0000 0000  .|.f.S.).Nc.....
+00002260: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
+00002270: 0000 0073 1400 0000 6700 7c00 5d06 7d01  ...s....g.|.].}.
+00002280: 7400 7c01 8301 9102 7102 5300 7235 0000  t.|.....q.S.r5..
+00002290: 0029 0172 7500 0000 2902 7299 0000 00da  .).ru...).r.....
+000022a0: 0570 6172 616d 7235 0000 0072 3500 0000  .paramr5...r5...
+000022b0: 7236 0000 0072 9c00 0000 6101 0000 f302  r6...r....a.....
+000022c0: 0000 0014 007a 2942 7261 696e 4772 6964  .....z)BrainGrid
+000022d0: 2e74 6162 6c65 5f73 6574 7570 2e3c 6c6f  .table_setup.<lo
+000022e0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+000022f0: 7201 0000 0029 0372 ea00 0000 72bc 0000  r....).r....r...
+00002300: 0072 ba00 0000 2902 72bb 0000 0072 b900  .r....).r....r..
+00002310: 0000 72ea 0000 0072 4400 0000 72bc 0000  ..r....rD...r...
+00002320: 0072 bb00 0000 72b9 0000 0072 5800 0000  .r....r....rX...
+00002330: 72ba 0000 0072 0800 0000 2910 7213 0000  r....r....).r...
+00002340: 00da 0e70 6172 616d 6574 6572 5f64 6963  ...parameter_dic
+00002350: 7472 ad00 0000 7268 0000 0072 a600 0000  tr....rh...r....
+00002360: 72da 0000 00da 046b 6579 73da 1062 7261  r......keys..bra
+00002370: 696e 5f74 6162 6c65 5f63 6f6c 73da 1062  in_table_cols..b
+00002380: 7261 696e 5f74 6162 6c65 5f72 6f77 73da  rain_table_rows.
+00002390: 0569 6e64 6578 72c9 0000 0072 c100 0000  .indexr....r....
+000023a0: 7277 0000 0072 7500 0000 72de 0000 00da  rw...ru...r.....
+000023b0: 1172 6176 656c 5f6d 756c 7469 5f69 6e64  .ravel_multi_ind
+000023c0: 6578 2911 722f 0000 0072 af00 0000 5a0d  ex).r/...r....Z.
+000023d0: 756e 6971 7565 5f70 6172 616d 7372 b300  unique_paramsr..
+000023e0: 0000 da03 6b65 79da 0670 6172 616d 735a  ....key..paramsZ
+000023f0: 0b70 6c6f 745f 7661 6c75 6573 5a0b 6178  .plot_valuesZ.ax
+00002400: 6973 5f74 6974 6c65 7372 b200 0000 7240  is_titlesr....r@
+00002410: 0000 0072 b500 0000 72b4 0000 0072 d300  ...r....r....r..
+00002420: 0000 da09 6669 6c65 5f6e 616d 655a 1074  ....file_nameZ.t
+00002430: 656d 705f 6f72 6465 725f 7374 6f72 655a  emp_order_storeZ
+00002440: 0d66 696c 655f 6e61 6d65 5f72 6f77 5a0a  .file_name_rowZ.
+00002450: 6669 6c65 5f70 6172 616d 7235 0000 0072  file_paramr5...r
+00002460: 3500 0000 7236 0000 0072 a700 0000 5a01  5...r6...r....Z.
+00002470: 0000 7342 0000 0004 0204 010c 0214 010e  ..sB............
+00002480: 010c 0104 0210 0110 0210 0106 ff08 0310  ................
+00002490: 0102 0102 0210 010e ff10 0310 0118 0204  ................
+000024a0: 0116 0108 0212 0114 0220 021a 0112 020c  ......... ......
+000024b0: 0116 0206 0108 ff0c 037a 1542 7261 696e  .........z.Brain
+000024c0: 4772 6964 2e74 6162 6c65 5f73 6574 7570  Grid.table_setup
+000024d0: 6306 0000 0000 0000 0000 0000 000b 0000  c...............
+000024e0: 0007 0000 0043 0000 0073 4801 0000 7400  .....C...sH...t.
+000024f0: a001 6401 7c05 6402 1900 7c05 6403 1900  ..d.|.d...|.d...
+00002500: 6602 6404 a103 7d06 7402 7c01 6405 1900  f.d...}.t.|.d...
+00002510: 6406 1900 8301 4400 5d4c 5c02 7d07 7d08  d.....D.]L\.}.}.
+00002520: 7403 a004 6402 7c07 6602 7c04 7c03 6602  t...d.|.f.|.|.f.
+00002530: a102 7d09 7c09 7c02 7601 7261 7405 a006  ..}.|.|.v.rat...
+00002540: 7c04 7c03 7c09 6403 1700 a103 0100 7405  |.|.|.d.......t.
+00002550: a007 7c06 a101 0100 7c00 a008 a100 0100  ..|.....|.......
+00002560: 7405 6a09 7c00 6a0a 6a0b 6407 1700 7c08  t.j.|.j.j.d...|.
+00002570: 1700 7c00 6a0a 6a0c 6408 8d02 0100 7c09  ..|.j.j.d.....|.
+00002580: 6402 6b02 7261 7405 6a0d 7c00 6a0a 6a0e  d.k.rat.j.|.j.j.
+00002590: 6407 1700 7c01 6409 1900 6406 1900 6402  d...|.d...d...d.
+000025a0: 1900 1700 7c00 6a0a 6a0c 6408 8d02 0100  ....|.j.j.d.....
+000025b0: 7115 7402 7c01 6409 1900 6406 1900 8301  q.t.|.d...d.....
+000025c0: 4400 5d37 5c02 7d07 7d0a 7403 a004 7c07  D.]7\.}.}.t...|.
+000025d0: 6402 6602 7c04 7c03 6602 a102 7d09 7c09  d.f.|.|.f...}.|.
+000025e0: 7c02 7601 72a1 7c09 6402 6b03 72a1 7405  |.v.r.|.d.k.r.t.
+000025f0: a006 7c04 7c03 7c09 6403 1700 a103 0100  ..|.|.|.d.......
+00002600: 7405 a007 7c06 a101 0100 7c00 a008 a100  t...|.....|.....
+00002610: 0100 7405 6a0d 7c00 6a0a 6a0e 6407 1700  ..t.j.|.j.j.d...
+00002620: 7c0a 1700 7c00 6a0a 6a0c 6408 8d02 0100  |...|.j.j.d.....
+00002630: 716a 6400 5300 290a 4eda 0352 4742 7201  qjd.S.).N..RGBr.
+00002640: 0000 0072 0800 0000 2903 e9ff 0000 0072  ...r....)......r
+00002650: f600 0000 72f6 0000 0072 bb00 0000 72bc  ....r....r....r.
+00002660: 0000 0072 0d00 0000 72bd 0000 0072 b900  ...r....r....r..
+00002670: 0000 290f 7207 0000 0072 5500 0000 72c1  ..).r....rU...r.
+00002680: 0000 0072 de00 0000 72f1 0000 0072 a800  ...r....r....r..
+00002690: 0000 72c5 0000 0072 c600 0000 da13 6d61  ..r....r......ma
+000026a0: 6b65 5f63 656c 6c5f 696e 7669 7369 626c  ke_cell_invisibl
+000026b0: 6572 4f00 0000 7213 0000 0072 ca00 0000  erO...r....r....
+000026c0: 72cb 0000 0072 cc00 0000 72cd 0000 0029  r....r....r....)
+000026d0: 0b72 2f00 0000 72b2 0000 0072 b300 0000  .r/...r....r....
+000026e0: 72b5 0000 0072 b400 0000 72d4 0000 0072  r....r....r....r
+000026f0: 9700 0000 da07 636f 756e 7465 725a 0778  ......counterZ.x
+00002700: 5f74 6974 6c65 5a0b 6869 6464 656e 5f63  _titleZ.hidden_c
+00002710: 656c 6c5a 0779 5f74 6974 6c65 7235 0000  ellZ.y_titler5..
+00002720: 0072 3500 0000 7236 0000 0072 ce00 0000  .r5...r6...r....
+00002730: 8801 0000 732c 0000 001a 0318 0214 0108  ....s,..........
+00002740: 0212 010a 0108 011e 0208 021e 0106 0106  ................
+00002750: ff02 8018 0314 0110 0212 010a 0108 011e  ................
+00002760: 0202 8004 f87a 1f42 7261 696e 4772 6964  .....z.BrainGrid
+00002770: 2e6c 6162 656c 5f62 6c61 6e6b 5f63 656c  .label_blank_cel
+00002780: 6c5f 6178 6573 6300 0000 0000 0000 0000  l_axesc.........
+00002790: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
+000027a0: 6c00 0000 7400 a001 a100 7d00 7c00 6a02  l...t.....}.|.j.
+000027b0: a003 a100 a004 6700 a101 0100 7c00 6a02  ......g.....|.j.
+000027c0: a005 a100 a004 6700 a101 0100 7c00 6a06  ......g.....|.j.
+000027d0: 6401 1900 a007 6402 a101 0100 7c00 6a06  d.....d.....|.j.
+000027e0: 6403 1900 a007 6402 a101 0100 7c00 6a06  d.....d.....|.j.
+000027f0: 6404 1900 a007 6402 a101 0100 7c00 6a06  d.....d.....|.j.
+00002800: 6405 1900 a007 6402 a101 0100 6400 5300  d.....d.....d.S.
+00002810: 2906 4eda 046c 6566 7446 da05 7269 6768  ).N..leftF..righ
+00002820: 74da 0662 6f74 746f 6dda 0374 6f70 2908  t..bottom..top).
+00002830: 72a8 0000 0072 c700 0000 723b 0000 00da  r....r....r;....
+00002840: 0967 6574 5f78 6178 6973 5a09 7365 745f  .get_xaxisZ.set_
+00002850: 7469 636b 73da 0967 6574 5f79 6178 6973  ticks..get_yaxis
+00002860: 5a06 7370 696e 6573 da0b 7365 745f 7669  Z.spines..set_vi
+00002870: 7369 626c 6529 01da 0566 7261 6d65 7235  sible)...framer5
+00002880: 0000 0072 3500 0000 7236 0000 0072 f700  ...r5...r6...r..
+00002890: 0000 a501 0000 730e 0000 0008 0210 0110  ......s.........
+000028a0: 0110 0110 0110 0114 017a 1d42 7261 696e  .........z.Brain
+000028b0: 4772 6964 2e6d 616b 655f 6365 6c6c 5f69  Grid.make_cell_i
+000028c0: 6e76 6973 6962 6c65 4e29 0c72 8700 0000  nvisibleN).r....
+000028d0: 7288 0000 0072 8900 0000 728a 0000 0072  r....r....r....r
+000028e0: 2600 0000 722b 0000 0072 ac00 0000 72c2  &...r+...r....r.
+000028f0: 0000 0072 a700 0000 72ce 0000 0072 8b00  ...r....r....r..
+00002900: 0000 72f7 0000 0072 3500 0000 7235 0000  ..r....r5...r5..
+00002910: 0072 3500 0000 7236 0000 0072 2500 0000  .r5...r6...r%...
+00002920: a700 0000 731e 0000 0008 0002 010a 0102  ....s...........
+00002930: 220a 0102 3e0a 0102 2a0a 0102 240a 0102  "...>...*...$...
+00002940: 2d0a 0102 1c0e 0172 2500 0000 6300 0000  -......r%...c...
+00002950: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+00002960: 0040 0000 0073 1800 0000 6500 5a01 6400  .@...s....e.Z.d.
+00002970: 5a02 6503 6401 6402 8400 8301 5a04 6403  Z.e.d.d.....Z.d.
+00002980: 5300 2904 7229 0000 0063 0200 0000 0000  S.).r)...c......
+00002990: 0000 0000 0000 0700 0000 0800 0000 4300  ..............C.
+000029a0: 0000 7364 0200 0074 00a0 017c 01a1 017d  ..sd...t...|...}
+000029b0: 027c 027c 0264 0119 0064 026b 037c 0264  .|.|.d...d.k.|.d
+000029c0: 0119 0064 036b 0340 0019 007d 027c 027c  ...d.k.@...}.|.|
+000029d0: 0264 0419 0064 056b 0419 007d 027c 006a  .d...d.k...}.|.j
+000029e0: 026a 0364 066b 0273 387c 006a 026a 0464  .j.d.k.s8|.j.j.d
+000029f0: 066b 0273 387c 02a0 057c 006a 026a 037c  .k.s8|...|.j.j.|
+00002a00: 006a 026a 0467 02a1 01a0 0664 0764 0884  .j.j.g.....d.d..
+00002a10: 00a1 017d 026e 257c 006a 026a 0364 066b  ...}.n%|.j.j.d.k
+00002a20: 0273 4b7c 02a0 057c 006a 026a 03a1 01a0  .sK|...|.j.j....
+00002a30: 0664 0964 0884 00a1 017d 026e 127c 006a  .d.d.....}.n.|.j
+00002a40: 026a 0464 066b 0273 5d7c 02a0 057c 006a  .j.d.k.s]|...|.j
+00002a50: 026a 04a1 01a0 0664 0a64 0884 00a1 017d  .j.....d.d.....}
+00002a60: 027c 026a 0764 0b64 0c8d 017d 0264 0d7c  .|.j.d.d...}.d.|
+00002a70: 0264 0e3c 0064 0f7d 0374 086a 0974 086a  .d.<.d.}.t.j.t.j
+00002a80: 0a64 0e64 1064 118d 0264 128d 017d 0474  .d.d.d...d...}.t
+00002a90: 086a 0974 086a 0a64 0e64 1364 118d 0264  .j.t.j.d.d.d...d
+00002aa0: 128d 017d 0574 08a0 0b7c 02a1 0174 086a  ...}.t...|...t.j
+00002ab0: 0964 0e64 0464 148d 0217 0074 086a 0c7c  .d.d.d.....t.j.|
+00002ac0: 0564 0b64 157c 006a 026a 0d64 1664 178d  .d.d.|.j.j.d.d..
+00002ad0: 0517 0074 086a 0e64 0f64 057c 006a 026a  ...t.j.d.d.|.j.j
+00002ae0: 0f64 1664 188d 0417 0074 08a0 1064 1964  .d.d.....t...d.d
+00002af0: 1aa1 0217 0074 08a0 1164 0564 00a1 0217  .....t...d.d....
+00002b00: 0074 08a0 127c 006a 026a 13a1 0117 0074  .t...|.j.j.....t
+00002b10: 08a0 1464 06a1 0117 0074 086a 157c 006a  ...d.....t.j.|.j
+00002b20: 026a 049b 0064 1b7c 006a 026a 039b 009d  .j...d.|.j.j....
+00002b30: 0364 0b64 1c64 1d8d 0317 0074 08a0 16a1  .d.d.d.....t....
+00002b40: 0017 0074 086a 1774 086a 186a 1964 0d64  ...t.j.t.j.j.d.d
+00002b50: 1e8d 0174 086a 186a 1964 0564 1e8d 0174  ...t.j.j.d.d...t
+00002b60: 086a 1a64 1f64 0f64 208d 0274 08a0 1ba1  .j.d.d.d ..t....
+00002b70: 007c 006a 026a 1c64 218d 0517 007d 067c  .|.j.j.d!....}.|
+00002b80: 006a 026a 1d90 0172 057c 006a 026a 1e72  .j.j...r.|.j.j.r
+00002b90: ff7c 0674 086a 1f64 2264 0564 238d 0237  .|.t.j.d"d.d#..7
+00002ba0: 007d 066e 067c 0674 08a0 20a1 0037 007d  .}.n.|.t.. ..7.}
+00002bb0: 067c 066a 2164 247c 006a 026a 227c 006a  .|.j!d$|.j.j"|.j
+00002bc0: 026a 2264 2514 0064 2664 2664 278d 0501  .j"d%..d&d&d'...
+00002bd0: 007c 066a 2164 287c 006a 026a 227c 006a  .|.j!d(|.j.j"|.j
+00002be0: 026a 2264 2514 0064 2664 2664 278d 0501  .j"d%..d&d&d'...
+00002bf0: 007c 006a 026a 2390 0172 3074 2464 2983  .|.j.j#..r0t$d).
+00002c00: 0101 0064 0053 0064 0053 0029 2a4e 72f0  ...d.S.d.S.)*Nr.
+00002c10: 0000 00da 074f 7665 7261 6c6c fa06 4e6f  .....Overall..No
+00002c20: 2052 4f49 725b 0000 0072 0100 0000 7244   ROIr[...r....rD
+00002c30: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00002c40: 0100 0000 0300 0000 5300 0000 f30c 0000  ........S.......
+00002c50: 007c 00a0 0064 0167 01a1 0153 00a9 024e  .|...d.g...S...N
+00002c60: 725b 0000 00a9 01da 0b73 6f72 745f 7661  r[.......sort_va
+00002c70: 6c75 6573 a901 da01 7872 3500 0000 7235  lues....xr5...r5
+00002c80: 0000 0072 3600 0000 da08 3c6c 616d 6264  ...r6.....<lambd
+00002c90: 613e ba01 0000 f302 0000 000c 007a 2156  a>...........z!V
+00002ca0: 696f 6c69 6e50 6c6f 742e 6d61 6b65 2e3c  iolinPlot.make.<
+00002cb0: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
+00002cc0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00002cd0: 0003 0000 0053 0000 0072 0301 0000 7204  .....S...r....r.
+00002ce0: 0100 0072 0501 0000 7207 0100 0072 3500  ...r....r....r5.
+00002cf0: 0000 7235 0000 0072 3600 0000 7209 0100  ..r5...r6...r...
+00002d00: 00bd 0100 0072 0a01 0000 6301 0000 0000  .....r....c.....
+00002d10: 0000 0000 0000 0001 0000 0003 0000 0053  ...............S
+00002d20: 0000 0072 0301 0000 7204 0100 0072 0501  ...r....r....r..
+00002d30: 0000 7207 0100 0072 3500 0000 7235 0000  ..r....r5...r5..
+00002d40: 0072 3600 0000 7209 0100 00c0 0100 0072  .r6...r........r
+00002d50: 0a01 0000 54a9 01da 0464 726f 7072 0800  ....T....dropr..
+00002d60: 0000 da08 636f 6e73 7461 6e74 72a0 0000  ....constantr...
+00002d70: 007a 0778 2b73 6869 6674 2901 5a0b 6166  .z.x+shift).Z.af
+00002d80: 7465 725f 7363 616c 6572 0701 0000 7a07  ter_scaler....z.
+00002d90: 782d 7368 6966 74a9 0272 0801 0000 da01  x-shift..r......
+00002da0: 7972 f900 0000 6733 3333 3333 33e3 3f29  yr....g333333.?)
+00002db0: 04da 056e 615f 726d da05 7374 796c 65da  ...na_rm..style.
+00002dc0: 0466 696c 6c72 e600 0000 2904 724b 0000  .fillr....).rK..
+00002dd0: 005a 0d6f 7574 6c69 6572 5f61 6c70 6861  .Z.outlier_alpha
+00002de0: 7212 0100 0072 e600 0000 679a 9999 9999  r....r....g.....
+00002df0: 99d9 3f67 6666 6666 6666 f63f da01 7eda  ..?gffffff.?..~.
+00002e00: 0a6c 6162 656c 5f62 6f74 68a9 0272 0c01  .label_both..r..
+00002e10: 0000 5a08 6c61 6265 6c6c 6572 a901 da05  ..Z.labeller....
+00002e20: 616c 7068 61da 0467 7261 79a9 0272 1201  alpha..gray..r..
+00002e30: 0000 7217 0100 0029 05da 1270 616e 656c  ..r....)...panel
+00002e40: 5f67 7269 645f 6d61 6a6f 725f 79da 1270  _grid_major_y..p
+00002e50: 616e 656c 5f67 7269 645f 6d61 6a6f 725f  anel_grid_major_
+00002e60: 78da 1070 616e 656c 5f62 6163 6b67 726f  x..panel_backgro
+00002e70: 756e 64da 0b61 7869 735f 7465 7874 5f78  und..axis_text_x
+00002e80: 72c0 0000 0067 7b14 ae47 e17a a43f 2902  r....g{..G.z.?).
+00002e90: 724b 0000 0072 4a00 0000 7a23 4669 6775  rK...rJ...z#Figu
+00002ea0: 7265 732f 5669 6f6c 696e 5f70 6c6f 7473  res/Violin_plots
+00002eb0: 2f76 696f 6c69 6e70 6c6f 742e 706e 6772  /violinplot.pngr
+00002ec0: 4800 0000 4672 4900 0000 7a23 4669 6775  H...FrI...z#Figu
+00002ed0: 7265 732f 5669 6f6c 696e 5f70 6c6f 7473  res/Violin_plots
+00002ee0: 2f76 696f 6c69 6e70 6c6f 742e 7376 677a  /violinplot.svgz
+00002ef0: 1253 6176 6564 2076 696f 6c69 6e20 706c  .Saved violin pl
+00002f00: 6f74 2129 25da 0463 6f70 79da 0864 6565  ot!)%..copy..dee
+00002f10: 7063 6f70 7972 1300 0000 da0a 7461 626c  pcopyr......tabl
+00002f20: 655f 636f 6c73 da0a 7461 626c 655f 726f  e_cols..table_ro
+00002f30: 7773 da07 6772 6f75 7062 79da 0561 7070  ws..groupby..app
+00002f40: 6c79 da0b 7265 7365 745f 696e 6465 78da  ly..reset_index.
+00002f50: 0470 6c74 6eda 0361 6573 da05 7374 6167  .pltn..aes..stag
+00002f60: 65da 0667 6770 6c6f 745a 0b67 656f 6d5f  e..ggplotZ.geom_
+00002f70: 7669 6f6c 696e da0d 7669 6f6c 696e 5f63  violin..violin_c
+00002f80: 6f6c 6f75 725a 0c67 656f 6d5f 626f 7870  olourZ.geom_boxp
+00002f90: 6c6f 74da 0e62 6f78 706c 6f74 5f63 6f6c  lot..boxplot_col
+00002fa0: 6f75 72da 0478 6c69 6dda 0479 6c69 6d5a  our..xlim..ylimZ
+00002fb0: 0479 6c61 62da 0d74 6162 6c65 5f78 5f6c  .ylab..table_x_l
+00002fc0: 6162 656c 5a04 786c 6162 da0a 6661 6365  abelZ.xlab..face
+00002fd0: 745f 6772 6964 da09 7468 656d 655f 3533  t_grid..theme_53
+00002fe0: 38da 0574 6865 6d65 da06 7468 656d 6573  8..theme..themes
+00002ff0: da0c 656c 656d 656e 745f 6c69 6e65 da0c  ..element_line..
+00003000: 656c 656d 656e 745f 7265 6374 5a0d 656c  element_rectZ.el
+00003010: 656d 656e 745f 626c 616e 6b72 d200 0000  ement_blankr....
+00003020: da10 7669 6f6c 696e 5f73 686f 775f 6461  ..violin_show_da
+00003030: 7461 da0d 7669 6f6c 696e 5f6a 6974 7465  ta..violin_jitte
+00003040: 725a 0b67 656f 6d5f 6a69 7474 6572 da0a  rZ.geom_jitter..
+00003050: 6765 6f6d 5f70 6f69 6e74 7250 0000 0072  geom_pointrP...r
+00003060: 5100 0000 721e 0000 0072 1f00 0000 2907  Q...r....r....).
+00003070: 722f 0000 005a 076f 7269 675f 6466 72af  r/...Z.orig_dfr.
+00003080: 0000 00da 0573 6869 6674 da0b 7269 6768  .....shift..righ
+00003090: 745f 7368 6966 74da 0a6c 6566 745f 7368  t_shift..left_sh
+000030a0: 6966 7472 3f00 0000 7235 0000 0072 3500  iftr?...r5...r5.
+000030b0: 0000 7236 0000 0072 2600 0000 b101 0000  ..r6...r&.......
+000030c0: 7372 0000 000a 021c 0210 0118 0222 020c  sr..........."..
+000030d0: 021a 010c 0218 010c 0208 0204 0316 0216  ................
+000030e0: 0108 020c 0102 ff16 0202 fe14 0302 fd0a  ................
+000030f0: 0402 fc0a 0502 fb0c 0602 fa08 0702 f91a  ................
+00003100: 0802 0104 ff02 f806 0a02 f610 0b0c 010c  ................
+00003110: 0106 0106 0104 fc04 f50a 1108 0114 010c  ................
+00003120: 020c 020a 0104 0106 fe0c 040a 0104 0106  ................
+00003130: fe0a 040c 0104 ff7a 0f56 696f 6c69 6e50  .......z.ViolinP
+00003140: 6c6f 742e 6d61 6b65 4e29 0572 8700 0000  lot.makeN).r....
+00003150: 7288 0000 0072 8900 0000 728a 0000 0072  r....r....r....r
+00003160: 2600 0000 7235 0000 0072 3500 0000 7235  &...r5...r5...r5
+00003170: 0000 0072 3600 0000 7229 0000 00b0 0100  ...r6...r)......
+00003180: 0073 0600 0000 0800 0201 0e01 7229 0000  .s..........r)..
+00003190: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+000031a0: 0000 0300 0000 4000 0000 7324 0000 0065  ......@...s$...e
+000031b0: 005a 0164 005a 0265 0364 0164 0284 0083  .Z.d.Z.e.d.d....
+000031c0: 015a 0465 0564 0364 0484 0083 015a 0664  .Z.e.d.d.....Z.d
+000031d0: 0553 0029 0672 2a00 0000 6303 0000 0000  .S.).r*...c.....
+000031e0: 0000 0000 0000 0007 0000 000a 0000 0043  ...............C
+000031f0: 0000 0073 5001 0000 7c00 6a00 6a01 6401  ...sP...|.j.j.d.
+00003200: 6b02 720a 7402 6402 8301 8201 7403 a004  k.r.t.d.....t...
+00003210: 6403 a101 0100 7405 7c01 6404 1900 a006  d.....t.|.d.....
+00003220: a100 8301 7d03 7403 6a07 7c03 6405 7c00  ....}.t.j.|.d.|.
+00003230: 6a00 6a08 6406 8d03 7d04 7a04 7c04 0100  j.j.d...}.z.|...
+00003240: 5700 6e15 0400 7409 793a 0100 0100 0100  W.n...t.y:......
+00003250: 7c00 6a00 6a0a 7237 740b 6407 8301 0100  |.j.j.r7t.d.....
+00003260: 5900 6400 5300 5900 6400 5300 7700 7c00  Y.d.S.Y.d.S.w.|.
+00003270: 6a00 6a0a 7243 740b 6408 8301 0100 6409  j.j.rCt.d.....d.
+00003280: 7d05 0900 740c 740d a00e 7c00 6a0f a101  }...t.t...|.j...
+00003290: 7c04 740d a00e 7c01 a101 740d a00e 7c05  |.t...|...t...|.
+000032a0: a101 740d a00e 7c00 6a10 a101 740d a00e  ..t...|.j...t...
+000032b0: 7c00 6a11 a101 740d a00e 7c00 6a00 a101  |.j...t...|.j...
+000032c0: 8307 7d06 7c02 7270 7c02 a012 7403 6a13  ..}.|.rp|...t.j.
+000032d0: 7c06 a102 7d05 6e09 7405 740d a012 7403  |...}.n.t.t...t.
+000032e0: 6a13 7c06 a102 8301 7d05 7414 7c05 8301  j.|.....}.t.|...
+000032f0: 72a5 7c05 6a15 640b 640c 8400 640d 8d01  r.|.j.d.d...d...
+00003300: 0100 7c00 6a00 6a0a 729e 740b 640e 7416  ..|.j.j.r.t.d.t.
+00003310: 7c05 640f 1900 6410 1900 8301 9b00 6411  |.d...d.......d.
+00003320: 7c05 640f 1900 6412 1900 9b00 6413 9d05  |.d...d.....d...
+00003330: 8301 0100 7c05 640f 1900 6410 1900 7d05  ....|.d...d...}.
+00003340: 6e02 6400 5300 7146 2914 4e72 4400 0000  n.d.S.qF).NrD...
+00003350: 7a45 5061 7261 6d65 7465 7220 746f 2070  zEParameter to p
+00003360: 6c6f 7420 616c 6f6e 6720 7468 6520 782d  lot along the x-
+00003370: 6178 6573 206f 6620 7468 6520 6261 7263  axes of the barc
+00003380: 6861 7274 7320 6861 7320 6e6f 7420 6265  harts has not be
+00003390: 656e 2073 6574 2e7a 1146 6967 7572 6573  en set.z.Figures
+000033a0: 2f42 6172 6368 6172 7473 72f0 0000 007a  /Barchartsr....z
+000033b0: 144f 6e65 2072 6567 696f 6e20 6261 7220  .One region bar 
+000033c0: 6368 6172 74a9 02da 0966 756e 635f 6e61  chart....func_na
+000033d0: 6d65 da11 636f 6e66 6967 5f72 6567 696f  me..config_regio
+000033e0: 6e5f 7661 727a 1b53 6b69 7070 696e 6720  n_varz.Skipping 
+000033f0: 6261 7263 6861 7274 2063 7265 6174 696f  barchart creatio
+00003400: 6e2e 7a1a 0a2d 2d2d 2042 6172 6368 6172  n.z..--- Barchar
+00003410: 7420 6372 6561 7469 6f6e 202d 2d2d 7201  t creation ---r.
+00003420: 0000 0054 6301 0000 0000 0000 0000 0000  ...Tc...........
+00003430: 0001 0000 0002 0000 0053 0000 00f3 0800  .........S......
+00003440: 0000 7c00 6401 1900 5300 a902 4e72 0800  ..|.d...S...Nr..
+00003450: 0000 7235 0000 0072 0701 0000 7235 0000  ..r5...r....r5..
+00003460: 0072 3500 0000 7236 0000 0072 0901 0000  .r5...r6...r....
+00003470: 1002 0000 f302 0000 0008 007a 2042 6172  ...........z Bar
+00003480: 6368 6172 742e 7365 7475 702e 3c6c 6f63  chart.setup.<loc
+00003490: 616c 733e 2e3c 6c61 6d62 6461 3ea9 0172  als>.<lambda>..r
+000034a0: f200 0000 7a14 4d61 7869 6d75 6d20 7920  ....z.Maximum y 
+000034b0: 6c69 6d69 7420 6f66 3a20 72a4 0000 0072  limit of: r....r
+000034c0: 0800 0000 fa10 2073 6565 6e20 7769 7468  ...... seen with
+000034d0: 2052 4f49 3a20 725f 0000 007a 262e 2043   ROI: r_...z&. C
+000034e0: 7265 6174 696e 6720 6669 6775 7265 7320  reating figures 
+000034f0: 7769 7468 2074 6869 7320 7920 6c69 6d69  with this y limi
+00003500: 742e 0a29 1772 1300 0000 da15 7369 6e67  t..).r......sing
+00003510: 6c65 5f72 6f69 5f66 6967 5f78 5f61 7869  le_roi_fig_x_axi
+00003520: 73da 0945 7863 6570 7469 6f6e 7209 0000  s..Exceptionr...
+00003530: 0072 2800 0000 7268 0000 0072 a600 0000  .r(...rh...r....
+00003540: da10 6669 6e64 5f63 686f 7365 6e5f 726f  ..find_chosen_ro
+00003550: 6973 da11 7265 6769 6f6e 616c 5f66 6967  is..regional_fig
+00003560: 5f72 6f69 73da 094e 616d 6545 7272 6f72  _rois..NameError
+00003570: 721e 0000 0072 1f00 0000 da03 7a69 70da  r....r......zip.
+00003580: 0969 7465 7274 6f6f 6c73 da06 7265 7065  .itertools..repe
+00003590: 6174 7226 0000 0072 5600 0000 7243 0000  atr&...rV...rC..
+000035a0: 00da 0773 7461 726d 6170 da14 636c 6173  ...starmap..clas
+000035b0: 735f 6d65 7468 6f64 5f68 616e 646c 6572  s_method_handler
+000035c0: da03 616e 79da 0473 6f72 7472 ae00 0000  ..any..sortr....
+000035d0: 2907 722f 0000 0072 af00 0000 7234 0000  ).r/...r....r4..
+000035e0: 00da 096c 6973 745f 726f 6973 da0b 6368  ...list_rois..ch
+000035f0: 6f73 656e 5f72 6f69 7372 2c01 0000 da08  osen_roisr,.....
+00003600: 6974 6572 6162 6c65 7235 0000 0072 3500  iterabler5...r5.
+00003610: 0000 7236 0000 0072 2b00 0000 f001 0000  ..r6...r+.......
+00003620: 7340 0000 000c 0208 010a 0210 0208 0106  s@..............
+00003630: 0106 ff02 0208 010c 0108 010e 0106 ff02  ................
+00003640: ff08 0408 0104 0202 0116 0112 0114 0104  ................
+00003650: fe04 0410 0112 0308 0210 0108 022a 010e  .............*..
+00003660: 0304 0202 ec7a 0e42 6172 6368 6172 742e  .....z.Barchart.
+00003670: 7365 7475 7063 0600 0000 0000 0000 0000  setupc..........
+00003680: 0000 0b00 0000 0f00 0000 4300 0000 736c  ..........C...sl
+00003690: 0200 007c 016a 007c 0164 0119 007c 006b  ...|.j.|.d...|.k
+000036a0: 0219 007d 067c 06a0 017c 056a 0267 01a1  ...}.|...|.j.g..
+000036b0: 017d 067c 066a 0364 0264 038d 017d 0674  .}.|.j.d.d...}.t
+000036c0: 046a 057c 067c 056a 0219 007c 067c 056a  .j.|.|.j...|.|.j
+000036d0: 0219 00a0 06a1 0064 048d 027c 067c 056a  .......d...|.|.j
+000036e0: 023c 0064 0564 0684 007c 066a 0744 0083  .<.d.d...|.j.D..
+000036f0: 017c 065f 077c 056a 02a0 0864 0764 08a1  .|._.|.j...d.d..
+00003700: 027c 055f 027c 056a 09a0 0864 0764 08a1  .|._.|.j...d.d..
+00003710: 027c 055f 0974 0aa0 0b7c 06a1 0174 0aa0  .|._.t...|...t..
+00003720: 0ca1 0017 0074 0a6a 0d74 0a6a 0e64 0964  .....t.j.t.j.d.d
+00003730: 0a64 0b8d 0264 0a64 0264 0c8d 0317 0074  .d...d.d.d.....t
+00003740: 0a6a 0f64 0d74 0a6a 0e64 0964 0a64 0b8d  .j.d.t.j.d.d.d..
+00003750: 0264 0e8d 0217 0074 0a6a 1067 0064 0f8d  .d.....t.j.g.d..
+00003760: 0117 0074 0a6a 1174 0a6a 1264 1064 118d  ...t.j.t.j.d.d..
+00003770: 0174 0a6a 1364 1264 1364 148d 0274 0a6a  .t.j.d.d.d...t.j
+00003780: 1464 1564 1664 1764 188d 0374 0a6a 1464  .d.d.d.d...t.j.d
+00003790: 1564 1664 1764 188d 0374 0a6a 1464 1764  .d.d.d...t.j.d.d
+000037a0: 1664 198d 0274 0a6a 1464 1764 1564 1664  .d...t.j.d.d.d.d
+000037b0: 1a64 1769 0164 1b8d 0474 0a6a 1464 1764  .d.i.d...t.j.d.d
+000037c0: 1664 1c64 1d69 0164 1e8d 0364 1f64 2064  .d.d.i.d...d.d d
+000037d0: 2164 2269 0164 237c 056a 1564 248d 0c17  !d"i.d#|.j.d$...
+000037e0: 0074 0a6a 1674 0a6a 1764 257c 056a 0264  .t.j.t.j.d%|.j.d
+000037f0: 268d 0264 1664 1764 2764 288d 0417 0074  &..d.d.d'd(....t
+00003800: 0a6a 187c 056a 1964 298d 0117 007d 0764  .j.|.j.d)....}.d
+00003810: 2a64 0684 007c 06a0 1aa1 0044 0083 0164  *d...|.....D...d
+00003820: 1019 007d 087c 056a 0964 2b6b 0273 e77c  ...}.|.j.d+k.s.|
+00003830: 0774 0a6a 177c 056a 0264 2c64 2d7c 089b  .t.j.|.j.d,d-|..
+00003840: 009d 0264 2e7c 089b 009d 0264 2f7c 056a  ...d.|.....d/|.j
+00003850: 099b 0064 309d 0364 318d 0537 007d 076e  ...d0..d1..7.}.n
+00003860: 127c 0774 0a6a 177c 056a 0264 2c64 2d7c  .|.t.j.|.j.d,d-|
+00003870: 089b 009d 0264 2e7c 089b 009d 0264 328d  .....d.|.....d2.
+00003880: 0437 007d 077c 0774 0a6a 1b7c 056a 1c7c  .7.}.|.t.j.|.j.|
+00003890: 056a 1d7c 056a 1e64 338d 0337 007d 077c  .j.|.j.d3..7.}.|
+000038a0: 0290 0172 157c 0774 0aa0 1f64 007c 02a1  ...r.|.t...d.|..
+000038b0: 0237 007d 077c 0064 3437 007d 0064 107d  .7.}.|.d47.}.d.}
+000038c0: 097c 0264 106b 0290 0172 257c 047c 007c  .|.d.k...r%|.|.|
+000038d0: 0764 3583 037d 0964 367d 0a6e 077c 0264  .d5..}.d6}.n.|.d
+000038e0: 106b 0390 0172 2c64 377d 0a7c 037c 077c  .k...r,d7}.|.|.|
+000038f0: 007c 0a64 387c 0583 0501 007c 0953 0029  .|.d8|.....|.S.)
+00003900: 394e 72f0 0000 0054 720b 0100 0029 01da  9Nr....Tr....)..
+00003910: 0a63 6174 6567 6f72 6965 7363 0100 0000  .categoriesc....
+00003920: 0000 0000 0000 0000 0200 0000 0600 0000  ................
+00003930: 5300 0000 7318 0000 0067 007c 005d 087d  S...s....g.|.].}
+00003940: 017c 01a0 0064 0064 01a1 0291 0271 0253  .|...d.d.....q.S
+00003950: 0029 0272 0d00 0000 720e 0000 0029 0172  .).r....r....).r
+00003960: 1c00 0000 2902 7299 0000 00da 0163 7235  ....).r......cr5
+00003970: 0000 0072 3500 0000 7236 0000 0072 9c00  ...r5...r6...r..
+00003980: 0000 2402 0000 f302 0000 0018 007a 2142  ..$..........z!B
+00003990: 6172 6368 6172 742e 6d61 6b65 2e3c 6c6f  archart.make.<lo
+000039a0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+000039b0: 720d 0000 0072 0e00 0000 da06 7369 6e67  r....r......sing
+000039c0: 6c65 e79a 9999 9999 99e9 3f29 02da 0870  le........?)...p
+000039d0: 7265 7365 7276 6572 4b00 0000 2903 da08  reserverK...)...
+000039e0: 706f 7369 7469 6f6e 724b 0000 0072 1001  positionrK...r..
+000039f0: 0000 7208 0000 0029 0272 e600 0000 7257  ..r....).r....rW
+00003a00: 0100 0029 01da 066c 6162 656c 7372 0100  ...)...labelsr..
+00003a10: 0000 7216 0100 00da 0577 6869 7465 679a  ..r......whiteg.
+00003a20: 9999 9999 99c9 3f72 1901 0000 da04 626f  ......?r......bo
+00003a30: 6c64 da05 626c 6163 6be9 1400 0000 a903  ld..black.......
+00003a40: da06 7765 6967 6874 da05 636f 6c6f 7272  ..weight..colorr
+00003a50: e600 0000 a902 72e6 0000 0072 5f01 0000  ......r....r_...
+00003a60: da01 6229 0472 e600 0000 725e 0100 0072  ..b).r....r^...r
+00003a70: 5f01 0000 da06 6d61 7267 696e da01 6ce9  _.....margin..l.
+00003a80: 0500 0000 2903 72e6 0000 0072 5f01 0000  ....).r....r_...
+00003a90: 7262 0100 00e9 0a00 0000 e91e 0000 0072  rb.............r
+00003aa0: fa00 0000 6733 3333 3333 33eb 3f29 0267  ....g333333.?).g
+00003ab0: cdcc cccc cccc ec3f 7255 0100 0029 0c72  .......?rU...).r
+00003ac0: 1b01 0000 721c 0100 00da 0c61 7869 735f  ....r......axis_
+00003ad0: 7469 746c 655f 78da 0c61 7869 735f 7469  title_x..axis_ti
+00003ae0: 746c 655f 79da 0b61 7869 735f 7465 7874  tle_y..axis_text
+00003af0: 5f79 5a0c 6c65 6765 6e64 5f74 6974 6c65  _yZ.legend_title
+00003b00: 5a0b 6c65 6765 6e64 5f74 6578 745a 146c  Z.legend_textZ.l
+00003b10: 6567 656e 645f 656e 7472 795f 7370 6163  egend_entry_spac
+00003b20: 696e 675a 0f6c 6567 656e 645f 6b65 795f  ingZ.legend_key_
+00003b30: 7369 7a65 da0f 7375 6270 6c6f 7473 5f61  size..subplots_a
+00003b40: 646a 7573 74da 0f6c 6567 656e 645f 706f  djust..legend_po
+00003b50: 7369 7469 6f6e 72c0 0000 0067 6666 6666  sitionr....gffff
+00003b60: 6666 e6bf 2902 720f 0100 00da 056c 6162  ff..).r......lab
+00003b70: 656c 72fc 0000 0029 0372 5f01 0000 72e6  elr....).r_...r.
+00003b80: 0000 00da 0276 61a9 0172 bc00 0000 6301  .....va..r....c.
+00003b90: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00003ba0: 0000 0053 0000 0073 1800 0000 6700 7c00  ...S...s....g.|.
+00003bb0: 5d08 7d01 6400 7c01 7600 7202 7c01 9102  ].}.d.|.v.r.|...
+00003bc0: 7102 5300 2901 5a08 436f 6e66 5f49 6e74  q.S.).Z.Conf_Int
+00003bd0: 7235 0000 0029 0272 9900 0000 7208 0100  r5...).r....r...
+00003be0: 0072 3500 0000 7235 0000 0072 3600 0000  .r5...r5...r6...
+00003bf0: 729c 0000 0040 0200 0072 5301 0000 7244  r....@...rS...rD
+00003c00: 0000 0072 5b00 0000 7a05 4d65 616e 2d7a  ...r[...z.Mean-z
+00003c10: 054d 6561 6e2b 7a07 6661 6374 6f72 28fa  .Mean+z.factor(.
+00003c20: 0129 2905 7208 0100 0072 0f01 0000 da04  .)).r....r......
+00003c30: 796d 696e da04 796d 6178 7212 0100 0029  ymin..ymaxr....)
+00003c40: 0472 0801 0000 720f 0100 0072 7001 0000  .r....r....rp...
+00003c50: 7271 0100 0029 0372 0801 0000 720f 0100  rq...).r....r...
+00003c60: 0072 1201 0000 5a0a 5f73 616d 655f 796c  .r....Z._same_yl
+00003c70: 696d 7239 0000 005a 0f44 6966 6665 7265  imr9...Z.Differe
+00003c80: 6e74 5f79 6178 6973 5a0a 5361 6d65 5f79  nt_yaxisZ.Same_y
+00003c90: 6178 6973 5a08 6261 7263 6861 7274 2920  axisZ.barchart) 
+00003ca0: 7271 0000 0072 0601 0000 7242 0100 0072  rq...r....rB...r
+00003cb0: 2401 0000 7266 0000 00da 0b43 6174 6567  $...rf.....Categ
+00003cc0: 6f72 6963 616c 72a6 0000 0072 7600 0000  oricalr....rv...
+00003cd0: 721c 0000 00da 1573 696e 676c 655f 726f  r......single_ro
+00003ce0: 695f 6669 675f 636f 6c6f 7572 7225 0100  i_fig_colourr%..
+00003cf0: 0072 2801 0000 722f 0100 005a 0867 656f  .r(...r/...Z.geo
+00003d00: 6d5f 636f 6c5a 0e70 6f73 6974 696f 6e5f  m_colZ.position_
+00003d10: 646f 6467 655a 0d67 656f 6d5f 6572 726f  dodgeZ.geom_erro
+00003d20: 7262 6172 5a10 7363 616c 655f 785f 6469  rbarZ.scale_x_di
+00003d30: 7363 7265 7465 7230 0100 0072 3201 0000  screter0...r2...
+00003d40: 7233 0100 00da 0c65 6c65 6d65 6e74 5f74  r3.....element_t
+00003d50: 6578 7472 d200 0000 5a09 6765 6f6d 5f74  extr....Z.geom_t
+00003d60: 6578 7472 2601 0000 5a11 7363 616c 655f  extr&...Z.scale_
+00003d70: 6669 6c6c 5f6d 616e 7561 6cda 2063 6f6c  fill_manual. col
+00003d80: 6f72 626c 696e 645f 6672 6965 6e64 6c79  orblind_friendly
+00003d90: 5f70 6c6f 745f 636f 6c6f 7572 7372 ed00  _plot_coloursr..
+00003da0: 0000 da04 6c61 6273 da16 7369 6e67 6c65  ....labs..single
+00003db0: 5f72 6f69 5f66 6967 5f6c 6162 656c 5f78  _roi_fig_label_x
+00003dc0: da16 7369 6e67 6c65 5f72 6f69 5f66 6967  ..single_roi_fig
+00003dd0: 5f6c 6162 656c 5f79 da19 7369 6e67 6c65  _label_y..single
+00003de0: 5f72 6f69 5f66 6967 5f6c 6162 656c 5f66  _roi_fig_label_f
+00003df0: 696c 6c72 2c01 0000 290b 723e 0000 0072  illr,...).r>...r
+00003e00: af00 0000 5a06 796c 696d 6974 da0d 7361  ....Z.ylimit..sa
+00003e10: 7665 5f66 756e 6374 696f 6e5a 1266 696e  ve_functionZ.fin
+00003e20: 645f 796c 696d 5f66 756e 6374 696f 6e72  d_ylim_functionr
+00003e30: 1300 0000 da0a 6375 7272 656e 745f 6466  ......current_df
+00003e40: 723f 0000 005a 0f63 6f6e 665f 696e 745f  r?...Z.conf_int_
+00003e50: 7374 7269 6e67 5a0d 7265 7475 726e 6564  stringZ.returned
+00003e60: 5f79 6c69 6d72 5200 0000 7235 0000 0072  _ylimrR...r5...r
+00003e70: 3500 0000 7236 0000 0072 2600 0000 1a02  5...r6...r&.....
+00003e80: 0000 7382 0000 0012 020e 020c 010c 0102  ..s.............
+00003e90: 0104 0102 ff04 010c fe12 0410 0110 0108  ................
+00003ea0: 0306 0102 ff18 0202 fe16 0302 fd0a 0402  ................
+00003eb0: fc0e 050c 010e 010e 010c 0114 0112 0102  ................
+00003ec0: 0102 0106 0102 0104 0104 f502 fb12 1206  ................
+00003ed0: 0104 ff02 ee0c 1402 ec02 ff16 180a 020c  ................
+00003ee0: 0110 010c 010a fe0c 0410 0108 ff0e 0304  ................
+00003ef0: 0108 ff06 0310 0208 0104 020a 010c 0106  ................
+00003f00: 010a 0104 0110 0204 027a 0d42 6172 6368  .........z.Barch
+00003f10: 6172 742e 6d61 6b65 4e29 0772 8700 0000  art.makeN).r....
+00003f20: 7288 0000 0072 8900 0000 728a 0000 0072  r....r....r....r
+00003f30: 2b00 0000 728b 0000 0072 2600 0000 7235  +...r....r&...r5
+00003f40: 0000 0072 3500 0000 7235 0000 0072 3600  ...r5...r5...r6.
+00003f50: 0000 722a 0000 00ef 0100 0073 0a00 0000  ..r*.......s....
+00003f60: 0800 0201 0a01 0229 0e01 722a 0000 0063  .......)..r*...c
+00003f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003f80: 0300 0000 4000 0000 7330 0000 0065 005a  ....@...s0...e.Z
+00003f90: 0164 005a 0265 0364 0164 0284 0083 015a  .d.Z.e.d.d.....Z
+00003fa0: 0465 0364 0364 0484 0083 015a 0565 0664  .e.d.d.....Z.e.d
+00003fb0: 0564 0684 0083 015a 0764 0753 0029 0872  .d.....Z.d.S.).r
+00003fc0: 2c00 0000 6303 0000 0000 0000 0000 0000  ,...c...........
+00003fd0: 000b 0000 000a 0000 0043 0000 0073 a401  .........C...s..
+00003fe0: 0000 7400 a001 6401 a101 0100 7402 7c01  ..t...d.....t.|.
+00003ff0: 6402 1900 a003 a100 8301 7d03 7400 6a04  d.........}.t.j.
+00004000: 7c03 6403 7c00 6a05 6a06 6404 8d03 7d04  |.d.|.j.j.d...}.
+00004010: 7a04 7c04 0100 5700 6e15 0400 7407 7930  z.|...W.n...t.y0
+00004020: 0100 0100 0100 7c00 6a05 6a08 722d 7409  ......|.j.j.r-t.
+00004030: 6405 8301 0100 5900 6400 5300 5900 6400  d.....Y.d.S.Y.d.
+00004040: 5300 7700 7c00 6a05 6a08 7239 7409 6406  S.w.|.j.j.r9t.d.
+00004050: 8301 0100 6407 6408 8400 7400 a00a 6409  ....d.d...t...d.
+00004060: 640a a102 4400 8301 7d05 7c00 6a0b 7c00  d...D...}.|.j.|.
+00004070: 6a05 7c05 7c01 640b 640c 8d04 7d06 6700  j.|.|.d.d...}.g.
+00004080: 7d07 7c04 4400 5d0c 7d08 7c07 a00c 7c00  }.|.D.].}.|...|.
+00004090: a00d 7c08 7c06 7c01 a103 a101 0100 7152  ..|.|.|.......qR
+000040a0: 640d 7d09 0900 740e 740f a010 7c00 6a11  d.}...t.t...|.j.
+000040b0: a101 7c04 7c07 740f a010 7c09 a101 740f  ..|.|.t...|...t.
+000040c0: a010 7c00 6a12 a101 740f a010 7c00 6a13  ..|.j...t...|.j.
+000040d0: a101 740f a010 7c00 6a05 a101 8307 7d0a  ..t...|.j.....}.
+000040e0: 7c02 7289 7c02 a014 7400 6a15 7c0a a102  |.r.|...t.j.|...
+000040f0: 7d09 6e09 7402 740f a014 7400 6a15 7c0a  }.n.t.t...t.j.|.
+00004100: a102 8301 7d09 7416 7c09 8301 72cf 7a07  ....}.t.|...r.z.
+00004110: 7c09 a017 6400 a101 0100 5700 6e09 0400  |...d.....W.n...
+00004120: 7418 79a6 0100 0100 0100 5900 6e01 7700  t.y.......Y.n.w.
+00004130: 7c09 6a19 640f 6410 8400 6411 8d01 0100  |.j.d.d...d.....
+00004140: 7c00 6a05 6a08 72c8 7409 6412 741a 7c09  |.j.j.r.t.d.t.|.
+00004150: 6413 1900 6414 1900 8301 9b00 6415 7c09  d...d.......d.|.
+00004160: 6413 1900 6416 1900 9b00 6417 9d05 8301  d...d.....d.....
+00004170: 0100 7c09 6413 1900 6414 1900 7d09 6e02  ..|.d...d...}.n.
+00004180: 6400 5300 7162 2918 4e7a 1246 6967 7572  d.S.qb).Nz.Figur
+00004190: 6573 2f48 6973 746f 6772 616d 7372 f000  es/Histogramsr..
+000041a0: 0000 722c 0000 0072 3a01 0000 7a1c 536b  ..r,...r:...z.Sk
+000041b0: 6970 7069 6e67 2068 6973 746f 6772 616d  ipping histogram
+000041c0: 2063 7265 6174 696f 6e2e 7a1b 0a2d 2d2d   creation.z..---
+000041d0: 2048 6973 746f 6772 616d 2063 7265 6174   Histogram creat
+000041e0: 696f 6e20 2d2d 2d63 0100 0000 0000 0000  ion ---c........
+000041f0: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
+00004200: 731e 0000 0067 007c 005d 0b7d 0174 00a0  s....g.|.].}.t..
+00004210: 01a1 009b 0064 007c 019b 009d 0391 0271  .....d.|.......q
+00004220: 0253 0029 017a 152f 4f76 6572 616c 6c2f  .S.).z./Overall/
+00004230: 5261 775f 7265 7375 6c74 732f 2902 7215  Raw_results/).r.
+00004240: 0000 0072 1600 0000 7298 0000 0072 3500  ...r....r....r5.
+00004250: 0000 7235 0000 0072 3600 0000 729c 0000  ..r5...r6...r...
+00004260: 0071 0200 0073 0200 0000 1e00 7a23 4869  .q...s......z#Hi
+00004270: 7374 6f67 7261 6d2e 7365 7475 702e 3c6c  stogram.setup.<l
+00004280: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00004290: 3e7a 134f 7665 7261 6c6c 2f52 6177 5f72  >z.Overall/Raw_r
+000042a0: 6573 756c 7473 726f 0000 0072 0500 0000  esultsro...r....
+000042b0: 2901 727f 0000 0072 0100 0000 5463 0100  ).r....r....Tc..
+000042c0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+000042d0: 0000 5300 0000 723d 0100 0072 3e01 0000  ..S...r=...r>...
+000042e0: 7235 0000 0072 0701 0000 7235 0000 0072  r5...r....r5...r
+000042f0: 3500 0000 7236 0000 0072 0901 0000 8b02  5...r6...r......
+00004300: 0000 723f 0100 007a 2148 6973 746f 6772  ..r?...z!Histogr
+00004310: 616d 2e73 6574 7570 2e3c 6c6f 6361 6c73  am.setup.<locals
+00004320: 3e2e 3c6c 616d 6264 613e 7240 0100 007a  >.<lambda>r@...z
+00004330: 144d 6178 696d 756d 2078 206c 696d 6974  .Maximum x limit
+00004340: 206f 663a 2072 a400 0000 7208 0000 0072   of: r....r....r
+00004350: 4101 0000 725f 0000 007a 262e 2043 7265  A...r_...z&. Cre
+00004360: 6174 696e 6720 6669 6775 7265 7320 7769  ating figures wi
+00004370: 7468 2074 6869 7320 7820 6c69 6d69 742e  th this x limit.
+00004380: 0a29 1b72 0900 0000 7228 0000 0072 6800  .).r....r(...rh.
+00004390: 0000 72a6 0000 0072 4401 0000 7213 0000  ..r....rD...r...
+000043a0: 0072 4501 0000 7246 0100 0072 1e00 0000  .rE...rF...r....
+000043b0: 721f 0000 00da 0a66 696e 645f 6669 6c65  r......find_file
+000043c0: 7372 8600 0000 72da 0000 00da 2767 6574  sr....r.....'get
+000043d0: 5f6d 6561 6e5f 616e 645f 6d65 6469 616e  _mean_and_median
+000043e0: 5f66 6f72 5f65 6163 685f 6368 6f73 656e  _for_each_chosen
+000043f0: 5f72 6f69 7247 0100 0072 4801 0000 7249  _roirG...rH...rI
+00004400: 0100 0072 2600 0000 7256 0000 0072 4300  ...r&...rV...rC.
+00004410: 0000 724a 0100 0072 4b01 0000 724c 0100  ..rJ...rK...rL..
+00004420: 00da 0672 656d 6f76 65da 0a56 616c 7565  ...remove..Value
+00004430: 4572 726f 7272 4d01 0000 72ae 0000 0029  ErrorrM...r....)
+00004440: 0b72 2f00 0000 727e 0000 0072 3400 0000  .r/...r~...r4...
+00004450: 724e 0100 0072 4f01 0000 727d 0000 0072  rN...rO...r}...r
+00004460: 8000 0000 5a10 636f 6d62 696e 6564 5f72  ....Z.combined_r
+00004470: 6177 5f64 6673 da03 726f 6972 2b01 0000  aw_dfs..roir+...
+00004480: 7250 0100 0072 3500 0000 7235 0000 0072  rP...r5...r5...r
+00004490: 3600 0000 722b 0000 005f 0200 0073 5800  6...r+..._...sX.
+000044a0: 0000 0a02 1002 0801 0601 06ff 0203 0801  ................
+000044b0: 0c01 0801 0e01 06ff 02ff 0804 0801 0603  ................
+000044c0: 0a01 06ff 1402 0402 0801 0401 0c01 06ff  ................
+000044d0: 0403 0201 1001 1201 1401 04fe 0404 1001  ................
+000044e0: 1202 0802 0201 0e01 0c01 0401 02ff 1003  ................
+000044f0: 0802 2a01 0e03 0402 02e8 7a0f 4869 7374  ..*.......z.Hist
+00004500: 6f67 7261 6d2e 7365 7475 7063 0400 0000  ogram.setupc....
+00004510: 0000 0000 0000 0000 0800 0000 0700 0000  ................
+00004520: 4300 0000 732a 0100 007c 0164 016b 0272  C...s*...|.d.k.r
+00004530: 0874 00a0 01a1 0053 007c 0164 026b 0272  .t.....S.|.d.k.r
+00004540: 157c 02a0 02a1 007d 0464 027c 0464 033c  .|.....}.d.|.d.<
+00004550: 006e 0a7c 027c 0264 0319 007c 016b 0219  .n.|.|.d...|.k..
+00004560: 00a0 02a1 007d 047c 04a0 03a1 007d 047c  .....}.|.....}.|
+00004570: 036a 0464 0464 0369 0164 058d 017d 0374  .j.d.d.i.d...}.t
+00004580: 0574 0664 007c 006a 076a 087c 006a 076a  .t.d.|.j.j.|.j.j
+00004590: 0967 0283 0283 017d 057c 046a 0a7c 0364  .g.....}.|.j.|.d
+000045a0: 0367 017c 05a2 0164 0664 078d 037d 0467  .g.|...d.d...}.g
+000045b0: 007c 05a2 0164 0391 0164 0891 0164 0991  .|...d...d...d..
+000045c0: 0164 0a91 017d 067c 046a 0b44 005d 0c7d  .d...}.|.j.D.].}
+000045d0: 077c 077c 0676 0172 5e7c 046a 0c7c 0764  .|.|.v.r^|.j.|.d
+000045e0: 058d 017d 0471 5274 006a 0d7c 047c 0664  ...}.qRt.j.|.|.d
+000045f0: 0064 0b85 0219 0064 0c64 0964 0a67 0264  .d.....d.d.d.g.d
+00004600: 0d64 0e8d 057d 047c 006a 076a 0e72 827c  .d...}.|.j.j.r.|
+00004610: 006a 076a 0f73 827c 046a 107c 0464 0c19  .j.j.s.|.j.|.d..
+00004620: 0064 096b 0219 007d 047c 0453 007c 006a  .d.k...}.|.S.|.j
+00004630: 076a 0f72 937c 006a 076a 0e73 937c 046a  .j.r.|.j.j.s.|.j
+00004640: 107c 0464 0c19 0064 0a6b 0219 007d 047c  .|.d...d.k...}.|
+00004650: 0453 0029 0f4e 7202 0100 0072 0101 0000  .S.).Nr....r....
+00004660: 7260 0000 0072 f000 0000 2901 7276 0000  r`...r....).rv..
+00004670: 0072 f900 0000 2902 da02 6f6e da03 686f  .r....)...on..ho
+00004680: 7772 6100 0000 725b 0000 0072 a100 0000  wra...r[...r....
+00004690: e9fe ffff ffda 0953 7461 7469 7374 6963  .......Statistic
+000046a0: da0a 7374 6174 5f76 616c 7565 2904 7262  ..stat_value).rb
+000046b0: 0000 0072 6300 0000 da0a 7661 6c75 655f  ...rc.....value_
+000046c0: 7661 7273 7264 0000 0029 1172 6600 0000  varsrd...).rf...
+000046d0: 7267 0000 0072 1e01 0000 727c 0000 00da  rg...r....r|....
+000046e0: 0672 656e 616d 6572 6800 0000 7269 0000  .renamerh...ri..
+000046f0: 0072 1300 0000 726b 0000 0072 6c00 0000  .r....rk...rl...
+00004700: da05 6d65 7267 6572 7600 0000 720c 0100  ..mergerv...r...
+00004710: 0072 7b00 0000 da13 6869 7374 6f67 7261  .r{.....histogra
+00004720: 6d5f 7368 6f77 5f6d 6561 6eda 1568 6973  m_show_mean..his
+00004730: 746f 6772 616d 5f73 686f 775f 6d65 6469  togram_show_medi
+00004740: 616e 7271 0000 0029 0872 2f00 0000 723e  anrq...).r/...r>
+00004750: 0000 0072 8000 0000 727e 0000 0072 7b01  ...r....r~...r{.
+00004760: 0000 7281 0000 0072 ed00 0000 7285 0000  ..r....r....r...
+00004770: 0072 3500 0000 7235 0000 0072 3600 0000  .r5...r5...r6...
+00004780: 727d 0100 0095 0200 0073 3a00 0000 0804  r}.......s:.....
+00004790: 0801 0801 0801 0a01 1402 0802 0403 0601  ................
+000047a0: 06ff 1a04 0601 0801 0201 06fe 1805 0a02  ................
+000047b0: 0801 0c01 0280 1202 0801 06ff 1003 1201  ................
+000047c0: 0404 10fd 1201 0402 7a31 4869 7374 6f67  ........z1Histog
+000047d0: 7261 6d2e 6765 745f 6d65 616e 5f61 6e64  ram.get_mean_and
+000047e0: 5f6d 6564 6961 6e5f 666f 725f 6561 6368  _median_for_each
+000047f0: 5f63 686f 7365 6e5f 726f 6963 0600 0000  _chosen_roic....
+00004800: 0000 0000 0000 0000 0900 0000 1000 0000  ................
+00004810: 4300 0000 73f8 0100 007c 016a 0072 0c7c  C...s....|.j.r.|
+00004820: 056a 0172 0a74 0264 0183 0101 0064 0053  .j.r.t.d.....d.S
+00004830: 0074 03a0 047c 0174 036a 0564 0264 038d  .t...|.t.j.d.d..
+00004840: 01a1 0274 03a0 06a1 0017 0074 036a 077c  ...t.......t.j.|
+00004850: 056a 087c 056a 0964 0464 0564 068d 0417  .j.|.j.d.d.d....
+00004860: 0074 036a 0a7c 056a 0b9b 0064 077c 056a  .t.j.|.j...d.|.j
+00004870: 0c9b 009d 0364 0564 0864 098d 0317 0074  .....d.d.d.....t
+00004880: 036a 0d7c 056a 0e7c 056a 0f64 0a8d 0217  .j.|.j.|.j.d....
+00004890: 0074 036a 1074 036a 116a 1264 0464 0b8d  .t.j.t.j.j.d.d..
+000048a0: 0174 036a 116a 1264 0c64 0b8d 0174 036a  .t.j.j.d.d...t.j
+000048b0: 1264 0464 0b8d 0174 036a 1364 0d64 0e8d  .d.d...t.j.d.d..
+000048c0: 0174 036a 1364 0f64 1064 118d 0274 036a  .t.j.d.d.d...t.j
+000048d0: 1464 1264 1364 1464 158d 0374 036a 1464  .d.d.d.d...t.j.d
+000048e0: 1264 1364 1464 158d 0374 036a 1464 1264  .d.d.d...t.j.d.d
+000048f0: 1664 1364 178d 0374 036a 1464 1264 1664  .d.d...t.j.d.d.d
+00004900: 1364 178d 0374 036a 1464 1664 1364 188d  .d...t.j.d.d.d..
+00004910: 0274 036a 1464 1664 1364 188d 027c 056a  .t.j.d.d.d...|.j
+00004920: 1564 198d 0c17 007d 067c 056a 1673 8e7c  .d.....}.|.j.s.|
+00004930: 056a 1772 ad7c 0674 036a 1874 036a 0564  .j.r.|.t.j.t.j.d
+00004940: 1a64 1b64 1c8d 027c 056a 1964 1d8d 0237  .d.d...|.j.d...7
+00004950: 007d 067c 0674 036a 1a7c 056a 1b64 1e19  .}.|.t.j.|.j.d..
+00004960: 007c 056a 1b64 0c19 0067 0264 1f8d 0137  .|.j.d...g.d...7
+00004970: 007d 067c 056a 1c73 b87c 0674 036a 1064  .}.|.j.s.|.t.j.d
+00004980: 2064 218d 0137 007d 067c 0272 c77c 0674   d!..7.}.|.r.|.t
+00004990: 03a0 1d64 227c 02a1 0237 007d 067c 0064  ...d"|...7.}.|.d
+000049a0: 2337 007d 006e 087c 0674 03a0 1d64 2264  #7.}.n.|.t...d"d
+000049b0: 00a1 0237 007d 0664 047d 077c 0264 046b  ...7.}.d.}.|.d.k
+000049c0: 0272 de7c 047c 007c 0664 2483 037d 0764  .r.|.|.|.d$..}.d
+000049d0: 257d 086e 067c 0264 046b 0372 e464 267d  %}.n.|.d.k.r.d&}
+000049e0: 0874 1e6a 1f64 2774 2064 288d 0201 007c  .t.j.d't d(....|
+000049f0: 037c 067c 007c 0864 297c 0583 0501 0074  .|.|.|.d)|.....t
+00004a00: 1e6a 1f64 2a74 2064 288d 0201 007c 0753  .j.d*t d(....|.S
+00004a10: 0029 2b4e 7a38 494e 464f 3a20 4869 7374  .)+Nz8INFO: Hist
+00004a20: 6f67 7261 6d73 2063 616e 6e6f 7420 6265  ograms cannot be
+00004a30: 206d 6164 6520 666f 7220 7468 6520 4e6f   made for the No
+00004a40: 2052 4f49 2063 6174 6567 6f72 792e 7261   ROI category.ra
+00004a50: 0000 0072 0701 0000 7201 0000 0054 2904  ...r....r....T).
+00004a60: da08 6269 6e77 6964 7468 7212 0100 00da  ..binwidthr.....
+00004a70: 0862 6f75 6e64 6172 7972 1001 0000 7213  .boundaryr....r.
+00004a80: 0100 0072 1401 0000 7215 0100 0072 0e01  ...r....r....r..
+00004a90: 0000 7216 0100 0072 0800 0000 7259 0100  ..r....r....rY..
+00004aa0: 00a9 0172 1201 0000 7218 0100 0072 a000  ...r....r....r..
+00004ab0: 0000 7219 0100 0072 5a01 0000 725b 0100  ..r....rZ...r[..
+00004ac0: 0072 5c01 0000 725d 0100 0072 6501 0000  .r\...r]...re...
+00004ad0: a903 725e 0100 0072 e600 0000 725f 0100  ..r^...r....r_..
+00004ae0: 0072 6001 0000 a90c 5a12 7061 6e65 6c5f  .r`.....Z.panel_
+00004af0: 6772 6964 5f6d 696e 6f72 5f78 721b 0100  grid_minor_xr...
+00004b00: 0072 1a01 0000 5a0f 706c 6f74 5f62 6163  .r....Z.plot_bac
+00004b10: 6b67 726f 756e 6472 1c01 0000 7267 0100  kgroundr....rg..
+00004b20: 0072 6801 0000 5a0c 7374 7269 705f 7465  .rh...Z.strip_te
+00004b30: 7874 5f78 5a0c 7374 7269 705f 7465 7874  xt_xZ.strip_text
+00004b40: 5f79 721d 0100 0072 6901 0000 72c0 0000  _yr....ri...r...
+00004b50: 0072 8501 0000 7284 0100 0029 025a 0a78  .r....r....).Z.x
+00004b60: 696e 7465 7263 6570 7472 5f01 0000 2901  interceptr_...).
+00004b70: 72e6 0000 0072 4800 0000 726e 0100 00da  r....rH...rn....
+00004b80: 046e 6f6e 6529 0172 6b01 0000 72a4 0000  .none).rk...r...
+00004b90: 005a 0a5f 7361 6d65 5f78 6c69 6d72 3800  .Z._same_xlimr8.
+00004ba0: 0000 5a0f 4469 6666 6572 656e 745f 7861  ..Z.Different_xa
+00004bb0: 7869 735a 0a53 616d 655f 7861 7869 73da  xisZ.Same_xaxis.
+00004bc0: 0669 676e 6f72 6529 02da 0661 6374 696f  .ignore)...actio
+00004bd0: 6eda 0863 6174 6567 6f72 79da 0968 6973  n..category..his
+00004be0: 746f 6772 616d da07 6465 6661 756c 7429  togram..default)
+00004bf0: 21da 0565 6d70 7479 721e 0000 0072 1f00  !..emptyr....r..
+00004c00: 0000 7225 0100 0072 2801 0000 7226 0100  ..r%...r(...r&..
+00004c10: 0072 2f01 0000 5a0e 6765 6f6d 5f68 6973  .r/...Z.geom_his
+00004c20: 746f 6772 616d da12 6869 7374 6f67 7261  togram..histogra
+00004c30: 6d5f 6269 6e77 6964 7468 da14 6869 7374  m_binwidth..hist
+00004c40: 6f67 7261 6d5f 6669 675f 636f 6c6f 7572  ogram_fig_colour
+00004c50: 722e 0100 0072 6c00 0000 726b 0000 0072  r....rl...rk...r
+00004c60: 7601 0000 da15 6869 7374 6f67 7261 6d5f  v.....histogram_
+00004c70: 6669 675f 6c61 6265 6c5f 78da 1568 6973  fig_label_x..his
+00004c80: 746f 6772 616d 5f66 6967 5f6c 6162 656c  togram_fig_label
+00004c90: 5f79 7230 0100 0072 3101 0000 7232 0100  _yr0...r1...r2..
+00004ca0: 0072 3301 0000 7274 0100 0072 d200 0000  .r3...rt...r....
+00004cb0: 7289 0100 0072 8a01 0000 5a0a 6765 6f6d  r....r....Z.geom
+00004cc0: 5f76 6c69 6e65 da18 6869 7374 6f67 7261  _vline..histogra
+00004cd0: 6d5f 7374 6174 5f6c 696e 655f 7369 7a65  m_stat_line_size
+00004ce0: 5a12 7363 616c 655f 636f 6c6f 725f 6d61  Z.scale_color_ma
+00004cf0: 6e75 616c 7275 0100 00da 1568 6973 746f  nualru.....histo
+00004d00: 6772 616d 5f73 686f 775f 6c65 6765 6e64  gram_show_legend
+00004d10: 722b 0100 00da 0877 6172 6e69 6e67 73da  r+.....warnings.
+00004d20: 0c73 696d 706c 6566 696c 7465 72da 0d46  .simplefilter..F
+00004d30: 7574 7572 6557 6172 6e69 6e67 2909 723e  utureWarning).r>
+00004d40: 0000 0072 8000 0000 5a06 786c 696d 6974  ...r....Z.xlimit
+00004d50: 727a 0100 005a 1266 696e 645f 786c 696d  rz...Z.find_xlim
+00004d60: 5f66 756e 6374 696f 6e72 1300 0000 723f  _functionr....r?
+00004d70: 0000 005a 0d72 6574 7572 6e65 645f 786c  ...Z.returned_xl
+00004d80: 696d 7252 0000 0072 3500 0000 7235 0000  imrR...r5...r5..
+00004d90: 0072 3600 0000 7226 0000 00be 0200 0073  .r6...r&.......s
+00004da0: 7200 0000 0602 0601 0801 0401 1203 0601  r...............
+00004db0: 02ff 0c02 0201 0201 04fe 02fe 1405 0401  ................
+00004dc0: 04ff 02fb 1007 02f9 0408 0c01 0c01 0a01  ................
+00004dd0: 0a01 0c01 0e01 0e01 0e01 0e01 0c01 0c01  ................
+00004de0: 0401 04f4 02f8 02ff 0c1a 1201 0401 08ff  ................
+00004df0: 0e02 0801 0aff 0604 1001 0402 1002 0a01  ................
+00004e00: 1002 0402 0801 0c01 0601 0801 0401 0e03  ................
+00004e10: 1002 0e02 0402 7a0e 4869 7374 6f67 7261  ......z.Histogra
+00004e20: 6d2e 6d61 6b65 4e29 0872 8700 0000 7288  m.makeN).r....r.
+00004e30: 0000 0072 8900 0000 728a 0000 0072 2b00  ...r....r....r+.
+00004e40: 0000 727d 0100 0072 8b00 0000 7226 0000  ..r}...r....r&..
+00004e50: 0072 3500 0000 7235 0000 0072 3500 0000  .r5...r5...r5...
+00004e60: 7236 0000 0072 2c00 0000 5e02 0000 730e  r6...r,...^...s.
+00004e70: 0000 0008 0002 010a 0102 350a 0102 280e  ..........5...(.
+00004e80: 0172 2c00 0000 6300 0000 0000 0000 0000  .r,...c.........
+00004e90: 0000 0000 0000 0003 0000 0040 0000 0073  ...........@...s
+00004ea0: 3400 0000 6500 5a01 6400 5a02 6401 5a03  4...e.Z.d.Z.d.Z.
+00004eb0: 6504 6402 6403 8400 8301 5a05 6504 6404  e.d.d.....Z.e.d.
+00004ec0: 6405 8400 8301 5a06 6504 6406 6407 8400  d.....Z.e.d.d...
+00004ed0: 8301 5a07 6401 5300 2908 da0e 436f 6d70  ..Z.d.S.)...Comp
+00004ee0: 6172 654f 7574 7075 7473 4e63 0200 0000  areOutputsNc....
+00004ef0: 0000 0000 0000 0000 0400 0000 0500 0000  ................
+00004f00: 4300 0000 7320 0000 007c 00a0 007c 01a1  C...s ...|...|..
+00004f10: 015c 027d 027d 037c 00a0 017c 027c 037c  .\.}.}.|...|.|.|
+00004f20: 01a1 0301 0064 0053 0029 014e 2902 da08  .....d.S.).N)...
+00004f30: 7365 7475 705f 6466 da0c 4d61 6b65 5f73  setup_df..Make_s
+00004f40: 6361 7474 6572 2904 722f 0000 0072 1300  catter).r/...r..
+00004f50: 0000 72af 0000 0072 5801 0000 7235 0000  ..r....rX...r5..
+00004f60: 0072 3500 0000 7236 0000 00da 0372 756e  .r5...r6.....run
+00004f70: 0403 0000 7304 0000 000e 0212 017a 1243  ....s........z.C
+00004f80: 6f6d 7061 7265 4f75 7470 7574 732e 7275  ompareOutputs.ru
+00004f90: 6e63 0200 0000 0000 0000 0000 0000 0a00  nc..............
+00004fa0: 0000 0900 0000 4300 0000 73b8 0000 0069  ......C...s....i
+00004fb0: 007d 0267 007d 0374 0064 0183 0144 005d  .}.g.}.t.d...D.]
+00004fc0: 3e7d 0474 016a 0264 0264 038d 017d 0574  >}.t.j.d.d...}.t
+00004fd0: 037c 059b 0064 049d 0264 0583 028f 267d  .|...d...d....&}
+00004fe0: 0674 04a0 057c 06a1 017d 0774 06a0 077c  .t...|...}.t...|
+00004ff0: 07a1 017c 027c 043c 007c 03a0 0874 096a  ...|.|.<.|...t.j
+00005000: 0aa0 0b7c 05a1 01a1 0101 0074 0c64 0664  ...|.......t.d.d
+00005010: 0784 007c 0744 0083 0183 017d 0857 0064  ...|.D.....}.W.d
+00005020: 0004 0004 0083 0301 0071 0831 0073 4177  .........q.1.sAw
+00005030: 0101 0001 0001 0059 0001 0071 087c 0264  .......Y...q.|.d
+00005040: 0819 006a 0d7c 0264 0919 0064 0a64 0b7c  ...j.|.d...d.d.|
+00005050: 016a 0e7c 016a 0f67 0364 0c8d 037d 097c  .j.|.j.g.d...}.|
+00005060: 097c 0366 0253 0029 0d4e 725f 0000 007a  .|.f.S.).Nr_...z
+00005070: 2753 656c 6563 7420 7468 6520 6469 7265  'Select the dire
+00005080: 6374 6f72 7920 6f75 7470 7574 2062 7920  ctory output by 
+00005090: 7468 6520 6652 4154 2901 724f 0000 007a  the fRAT).rO...z
+000050a0: 292f 5375 6d6d 6172 6973 6564 5f72 6573  )/Summarised_res
+000050b0: 756c 7473 2f63 6f6d 6269 6e65 645f 7265  ults/combined_re
+000050c0: 7375 6c74 732e 6a73 6f6e 725a 0000 0063  sults.jsonrZ...c
+000050d0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+000050e0: 0400 0000 5300 0000 7314 0000 0068 007c  ....S...s....h.|
+000050f0: 005d 067d 017c 0164 0019 0092 0271 0253  .].}.|.d.....q.S
+00005100: 0029 0172 f000 0000 7235 0000 0029 0272  .).r....r5...).r
+00005110: 9900 0000 da01 6472 3500 0000 7235 0000  ......dr5...r5..
+00005120: 0072 3600 0000 da09 3c73 6574 636f 6d70  .r6.....<setcomp
+00005130: 3e15 0300 0072 eb00 0000 7a2a 436f 6d70  >....r....z*Comp
+00005140: 6172 654f 7574 7075 7473 2e73 6574 7570  areOutputs.setup
+00005150: 5f64 662e 3c6c 6f63 616c 733e 2e3c 7365  _df.<locals>.<se
+00005160: 7463 6f6d 703e 7201 0000 0072 0800 0000  tcomp>r....r....
+00005170: da05 6f75 7465 7272 f000 0000 2902 7282  ..outerr....).r.
+00005180: 0100 0072 8101 0000 2910 da05 7261 6e67  ...r....)...rang
+00005190: 6572 0900 0000 da0c 6669 6c65 5f62 726f  er......file_bro
+000051a0: 7773 6572 726d 0000 0072 6f00 0000 7270  wserrm...ro...rp
+000051b0: 0000 0072 6600 0000 7267 0000 0072 da00  ...rf...rg...r..
+000051c0: 0000 7215 0000 0072 1800 0000 7273 0000  ..r....r....rs..
+000051d0: 0072 ad00 0000 7288 0100 0072 6c00 0000  .r....r....rl...
+000051e0: 726b 0000 0029 0a72 2f00 0000 7213 0000  rk...).r/...r...
+000051f0: 00da 0364 6673 7258 0100 0072 0801 0000  ...dfsrX...r....
+00005200: da09 6469 7265 6374 6f72 79da 0772 6573  ..directory..res
+00005210: 756c 7473 da04 6461 7461 5a04 726f 6973  ults..dataZ.rois
+00005220: 5a03 6466 6d72 3500 0000 7235 0000 0072  Z.dfmr5...r5...r
+00005230: 3600 0000 72a1 0100 0009 0300 0073 1c00  6...r........s..
+00005240: 0000 0402 0401 0c01 0c01 1202 0a01 0e01  ................
+00005250: 1201 1402 1efb 1007 0c01 06ff 0803 7a17  ..............z.
+00005260: 436f 6d70 6172 654f 7574 7075 7473 2e73  CompareOutputs.s
+00005270: 6574 7570 5f64 6663 0400 0000 0000 0000  etup_dfc........
+00005280: 0000 0000 0500 0000 1000 0000 4300 0000  ............C...
+00005290: 731c 0100 0074 00a0 017c 0174 006a 0264  s....t...|.t.j.d
+000052a0: 0164 0264 038d 02a1 0274 00a0 03a1 0017  .d.d.....t......
+000052b0: 0074 00a0 04a1 0017 0074 006a 057c 036a  .t.......t.j.|.j
+000052c0: 069b 0064 047c 036a 079b 009d 0364 0564  ...d.|.j.....d.d
+000052d0: 0664 078d 0317 0074 006a 0864 0864 098d  .d.....t.j.d.d..
+000052e0: 0117 0074 006a 097c 0264 0a19 007c 0264  ...t.j.|.d...|.d
+000052f0: 0b19 0064 038d 0217 0074 006a 0a74 006a  ...d.....t.j.t.j
+00005300: 0b6a 0c64 0b64 0c8d 0174 006a 0b6a 0c64  .j.d.d...t.j.j.d
+00005310: 0a64 0c8d 0174 006a 0c64 0b64 0c8d 0174  .d...t.j.d.d...t
+00005320: 006a 0d64 0d64 0e8d 0174 006a 0d64 0f64  .j.d.d...t.j.d.d
+00005330: 1064 118d 0274 006a 0e64 1264 1364 1464  .d...t.j.d.d.d.d
+00005340: 158d 0374 006a 0e64 1264 1364 1464 158d  ...t.j.d.d.d.d..
+00005350: 0374 006a 0e64 1264 1664 1364 178d 0374  .t.j.d.d.d.d...t
+00005360: 006a 0e64 1264 1664 1364 178d 0374 006a  .j.d.d.d.d...t.j
+00005370: 0e64 1664 1364 188d 0274 006a 0e64 1664  .d.d.d...t.j.d.d
+00005380: 1364 188d 027c 036a 0f64 198d 0c17 007d  .d...|.j.d.....}
+00005390: 047c 046a 1064 1a7c 036a 117c 036a 1164  .|.j.d.|.j.|.j.d
+000053a0: 1b14 0064 1c64 1c64 1d8d 0501 0064 0053  ...d.d.d.....d.S
+000053b0: 0029 1e4e 5a06 4d65 616e 5f78 5a06 4d65  .).NZ.Mean_xZ.Me
+000053c0: 616e 5f79 720e 0100 0072 1301 0000 5472  an_yr....r....Tr
+000053d0: 1401 0000 7215 0100 00da 026c 6d29 01da  ....r......lm)..
+000053e0: 066d 6574 686f 6472 0800 0000 7201 0000  .methodr....r...
+000053f0: 0072 1601 0000 7259 0100 0072 8d01 0000  .r....rY...r....
+00005400: 7218 0100 0072 a000 0000 7219 0100 0072  r....r....r....r
+00005410: 5a01 0000 725b 0100 0072 5c01 0000 725d  Z...r[...r\...r]
+00005420: 0100 0072 6501 0000 728e 0100 0072 6001  ...re...r....r`.
+00005430: 0000 728f 0100 007a 0854 4553 542e 706e  ..r....z.TEST.pn
+00005440: 6772 4800 0000 4672 4900 0000 2912 7225  grH...FrI...).r%
+00005450: 0100 0072 2801 0000 7226 0100 0072 2f01  ...r(...r&...r/.
+00005460: 0000 7236 0100 0072 2e01 0000 726c 0000  ..r6...r....rl..
+00005470: 0072 6b00 0000 5a0b 6765 6f6d 5f73 6d6f  .rk...Z.geom_smo
+00005480: 6f74 6872 7601 0000 7230 0100 0072 3101  othrv...r0...r1.
+00005490: 0000 7232 0100 0072 3301 0000 7274 0100  ..r2...r3...rt..
+000054a0: 0072 d200 0000 7250 0000 0072 5100 0000  .r....rP...rQ...
+000054b0: 2905 722f 0000 0072 af00 0000 7258 0100  ).r/...r....rX..
+000054c0: 0072 1300 0000 723f 0000 0072 3500 0000  .r....r?...r5...
+000054d0: 7235 0000 0072 3600 0000 72a2 0100 001c  r5...r6...r.....
+000054e0: 0300 0073 4200 0000 1403 0601 02ff 0602  ...sB...........
+000054f0: 02fe 1403 0401 04ff 02fd 0a05 02fb 1406  ................
+00005500: 02fa 0407 0c01 0c01 0a01 0a01 0c01 0e01  ................
+00005510: 0e01 0e01 0e01 0c01 0c01 0401 04f4 02f9  ................
+00005520: 02ff 0a18 0801 0401 0afe 7a1b 436f 6d70  ..........z.Comp
+00005530: 6172 654f 7574 7075 7473 2e4d 616b 655f  areOutputs.Make_
+00005540: 7363 6174 7465 7229 0872 8700 0000 7288  scatter).r....r.
+00005550: 0000 0072 8900 0000 727b 0100 0072 8a00  ...r....r{...r..
+00005560: 0000 72a3 0100 0072 a101 0000 72a2 0100  ..r....r....r...
+00005570: 0072 3500 0000 7235 0000 0072 3500 0000  .r5...r5...r5...
+00005580: 7236 0000 0072 a001 0000 0103 0000 7310  r6...r........s.
+00005590: 0000 0008 0004 0102 020a 0102 040a 0102  ................
+000055a0: 120e 0172 a001 0000 2924 721e 0100 0072  ...r....)$r....r
+000055b0: 4801 0000 7215 0000 0072 4d00 0000 729d  H...r....rM...r.
+000055c0: 0100 0072 0300 0000 da07 7061 7468 6c69  ...r......pathli
+000055d0: 6272 0400 0000 da10 6d61 7470 6c6f 746c  br......matplotl
+000055e0: 6962 2e69 6d61 6765 da05 696d 6167 6572  ib.image..imager
+000055f0: c300 0000 da05 6e75 6d70 7972 de00 0000  ......numpyr....
+00005600: da07 6e69 6261 6265 6c72 dc00 0000 da06  ..nibabelr......
+00005610: 7061 6e64 6173 7266 0000 005a 0870 6c6f  pandasrf...Z.plo
+00005620: 746e 696e 6572 2501 0000 da0a 7369 6d70  tniner%.....simp
+00005630: 6c65 6a73 6f6e 726f 0000 00da 076e 696c  lejsonro.....nil
+00005640: 6561 726e 7205 0000 00da 0a6d 6174 706c  earnr......matpl
+00005650: 6f74 6c69 6272 0600 0000 72a8 0000 00da  otlibr....r.....
+00005660: 0350 494c 7207 0000 00da 0575 7469 6c73  .PILr......utils
+00005670: 7209 0000 0072 0a00 0000 7225 0000 0072  r....r....r%...r
+00005680: 2900 0000 722a 0000 0072 2c00 0000 72a0  )...r*...r,...r.
+00005690: 0100 0072 3500 0000 7235 0000 0072 3500  ...r5...r5...r5.
+000056a0: 0000 7236 0000 00da 083c 6d6f 6475 6c65  ..r6.....<module
+000056b0: 3e01 0000 0073 3600 0000 0800 0801 0801  >....s6.........
+000056c0: 0801 0801 0c01 0c01 0c02 0801 0801 0801  ................
+000056d0: 0801 0801 0c01 0c01 0c01 0c02 0e03 007f  ................
+000056e0: 1012 007f 007f 100b 103f 106f 007f 1424  .........?.o...$
```

### Comparing `frat_brain-1.3.5/fRAT/utils/__pycache__/html_report.cpython-310.pyc` & `frat_brain-1.3.6/fRAT/utils/__pycache__/html_report.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/utils/__pycache__/printResults.cpython-310.pyc` & `frat_brain-1.3.6/fRAT/utils/__pycache__/printResults.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/utils/__pycache__/statistics.cpython-310.pyc` & `frat_brain-1.3.6/fRAT/utils/__pycache__/statistics.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/utils/__pycache__/statmap.cpython-310.pyc` & `frat_brain-1.3.6/fRAT/utils/__pycache__/statmap.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc` & `frat_brain-1.3.6/fRAT/utils/__pycache__/statmap_config_setup.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/utils/__pycache__/utils.cpython-310.pyc` & `frat_brain-1.3.6/fRAT/utils/__pycache__/utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Mar 30 14:24:26 2023 UTC, .py size: 18878 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9a9b 2564 be49 0000  o.........%d.I..
+00000000: 6f0d 0d0a 0000 0000 6e13 4164 c349 0000  o.......n.Ad.I..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6402 6c06 6d06 5a06 0100 6400 6403 6c07  d.l.m.Z...d.d.l.
 00000070: 6d08 5a08 0100 6400 6404 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
@@ -266,15 +266,15 @@
 00001090: 0a72 5b00 0000 fa01 237a 0223 2372 2300  .r[.....#z.##r#.
 000010a0: 0000 721e 0000 00e9 ffff ffff 7261 0000  ..r.........ra..
 000010b0: 0029 05da 046f 7065 6e72 5c00 0000 da07  .)...openr\.....
 000010c0: 7665 7273 696f 6eda 0a73 7461 7274 7377  version..startsw
 000010d0: 6974 6872 2a00 0000 290a 5a06 6e65 7764  ithr*...).Z.newd
 000010e0: 6972 da0b 636f 6e66 6967 5f70 6174 68da  ir..config_path.
 000010f0: 0f63 6f6e 6669 675f 6669 6c65 6e61 6d65  .config_filename
-00001100: 5a0f 6164 6469 7469 6f6e 616c 5f69 6e66  Z.additional_inf
+00001100: da0f 6164 6469 7469 6f6e 616c 5f69 6e66  ..additional_inf
 00001110: 6fda 1172 656c 6576 616e 745f 7365 6374  o..relevant_sect
 00001120: 696f 6e73 da0f 6e65 775f 636f 6e66 6967  ions..new_config
 00001130: 5f6e 616d 6572 3800 0000 7265 0000 0072  _namer8...re...r
 00001140: 5f00 0000 5a0f 6375 7272 656e 745f 7365  _...Z.current_se
 00001150: 6374 696f 6e72 1400 0000 7214 0000 0072  ctionr....r....r
 00001160: 1500 0000 da0b 7361 7665 5f63 6f6e 6669  ......save_confi
 00001170: 6788 0000 0073 2c00 0000 2e02 0601 0201  g....s,.........
@@ -295,15 +295,15 @@
 00001260: 9d02 7c02 9b00 7c06 9b00 9d02 a102 0100  ..|...|.........
 00001270: 6400 5300 2904 4e72 6300 0000 7a0f 7061  d.S.).Nrc...z.pa
 00001280: 7261 6d56 616c 7565 732e 6373 765a 0563  ramValues.csvZ.c
 00001290: 6f70 795f 2905 da08 656e 6473 7769 7468  opy_)...endswith
 000012a0: da06 7368 7574 696c da04 636f 7079 7234  ..shutil..copyr4
 000012b0: 0000 00da 0672 656e 616d 6529 07da 086f  .....rename)...o
 000012c0: 6c64 5f6e 616d 655a 0c6f 7269 6769 6e61  ld_nameZ.origina
-000012d0: 6c5f 6469 725a 076e 6577 5f64 6972 7272  l_dirZ.new_dirrr
+000012d0: 6c5f 6469 725a 076e 6577 5f64 6972 7273  l_dirZ.new_dirrs
 000012e0: 0000 00da 0b72 656e 616d 655f 636f 7079  .....rename_copy
 000012f0: da0e 7061 7261 6d65 7465 725f 6669 6c65  ..parameter_file
 00001300: da08 6e65 775f 6e61 6d65 7214 0000 0072  ..new_namer....r
 00001310: 1400 0000 7215 0000 00da 096d 6f76 655f  ....r......move_
 00001320: 6669 6c65 a100 0000 7318 0000 000a 0208  file....s.......
 00001330: 010a 0208 0104 0206 0104 0204 0204 0122  ..............."
 00001340: 0120 0220 027a 0f55 7469 6c73 2e6d 6f76  . . .z.Utils.mov
@@ -311,15 +311,15 @@
 00001360: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
 00001370: 4600 0000 7c01 7214 7400 6a01 a002 7c00  F...|.r.t.j...|.
 00001380: a101 7214 7403 a004 7c00 a101 0100 7405  ..r.t...|.....t.
 00001390: a006 7c00 a101 0100 6400 5300 7400 6a01  ..|.....d.S.t.j.
 000013a0: a002 7c00 a101 7321 7405 a006 7c00 a101  ..|...s!t...|...
 000013b0: 0100 6400 5300 6400 5300 7241 0000 0029  ..d.S.d.S.rA...)
 000013c0: 0772 3400 0000 7235 0000 00da 0665 7869  .r4...r5.....exi
-000013d0: 7374 7372 7100 0000 da06 726d 7472 6565  stsrq.....rmtree
+000013d0: 7374 7372 7200 0000 da06 726d 7472 6565  stsrr.....rmtree
 000013e0: 7208 0000 00da 066d 6b5f 6469 7229 0272  r......mk_dir).r
 000013f0: 3500 0000 da0a 6465 6c65 7465 5f6f 6c64  5.....delete_old
 00001400: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
 00001410: 1263 6865 636b 5f61 6e64 5f6d 616b 655f  .check_and_make_
 00001420: 6469 72b6 0000 0073 0c00 0000 1002 0a01  dir....s........
 00001430: 0e01 0c02 0e01 04ff 7a18 5574 696c 732e  ........z.Utils.
 00001440: 6368 6563 6b5f 616e 645f 6d61 6b65 5f64  check_and_make_d
@@ -377,25 +377,25 @@
 00001780: 6567 6572 732e 0a63 0100 0000 0000 0000  egers..c........
 00001790: 0000 0000 0200 0000 0400 0000 1300 0000  ................
 000017a0: 7314 0000 0067 007c 005d 067d 0188 007c  s....g.|.].}...|
 000017b0: 0119 0091 0271 0253 0072 1400 0000 7214  .....q.S.r....r.
 000017c0: 0000 0029 0272 3700 0000 5a0a 726f 695f  ...).r7...Z.roi_
 000017d0: 6e75 6d62 6572 a901 da08 616c 6c5f 726f  number....all_ro
 000017e0: 6973 7214 0000 0072 1500 0000 7239 0000  isr....r....r9..
-000017f0: 00ea 0000 0072 8400 0000 290e 7258 0000  .....r....).rX..
+000017f0: 00ea 0000 0072 8500 0000 290e 7258 0000  .....r....).rX..
 00001800: 00da 0965 6e75 6d65 7261 7465 da06 666f  ...enumerate..fo
 00001810: 726d 6174 da05 696e 7075 74da 056c 6f77  rmat..input..low
 00001820: 6572 7210 0000 00da 0572 616e 6765 da03  err......range..
 00001830: 6c65 6eda 0573 706c 6974 da03 6d61 70da  len..split..map.
 00001840: 0369 6e74 7211 0000 0072 0e00 0000 725d  .intr....r....r]
-00001850: 0000 0029 0772 8700 0000 da09 6675 6e63  ...).r......func
+00001850: 0000 0029 0772 8800 0000 da09 6675 6e63  ...).r......func
 00001860: 5f6e 616d 655a 1163 6f6e 6669 675f 7265  _nameZ.config_re
 00001870: 6769 6f6e 5f76 6172 5a0b 6368 6f73 656e  gion_varZ.chosen
-00001880: 5f72 6f69 7372 7f00 0000 7280 0000 005a  _roisr....r....Z
-00001890: 0772 6f69 5f61 6e73 7214 0000 0072 8600  .roi_ansr....r..
+00001880: 5f72 6f69 7372 8000 0000 7281 0000 005a  _roisr....r....Z
+00001890: 0772 6f69 5f61 6e73 7214 0000 0072 8700  .roi_ansr....r..
 000018a0: 0000 7215 0000 00da 1066 696e 645f 6368  ..r......find_ch
 000018b0: 6f73 656e 5f72 6f69 73bf 0000 0073 4400  osen_rois....sD.
 000018c0: 0000 0802 0401 0801 1002 1401 0402 1001  ................
 000018d0: 0201 0201 04ff 0c04 1401 0c02 1401 0202  ................
 000018e0: 1201 0c01 0801 0801 02fe 0405 0201 04ec  ................
 000018f0: 0280 1817 0e01 02ff 1402 0402 0a02 0801  ................
 00001900: 0802 1202 0402 7a16 5574 696c 732e 6669  ......z.Utils.fi
@@ -426,15 +426,15 @@
 00001a90: 5f72 6573 756c 7473 2e6a 736f 6e20 6e6f  _results.json no
 00001aa0: 7420 666f 756e 6420 696e 207a 0820 666f  t found in z. fo
 00001ab0: 6c64 6572 2e72 4a00 0000 2908 724c 0000  lder.rJ...).rL..
 00001ac0: 0072 4d00 0000 da09 7265 6164 5f6a 736f  .rM.....read_jso
 00001ad0: 6e72 1100 0000 da09 4578 6365 7074 696f  nr......Exceptio
 00001ae0: 6e72 5600 0000 da0e 6176 6572 6167 696e  nrV.....averagin
 00001af0: 675f 7479 7065 da0b 736f 7274 5f76 616c  g_type..sort_val
-00001b00: 7565 7329 04da 0666 6f6c 6465 7272 9700  ues)...folderr..
+00001b00: 7565 7329 04da 0666 6f6c 6465 7272 9800  ues)...folderr..
 00001b10: 0000 da02 6466 7235 0000 0072 1400 0000  ....dfr5...r....
 00001b20: 7214 0000 0072 1500 0000 da15 7265 6164  r....r......read
 00001b30: 5f63 6f6d 6269 6e65 645f 7265 7375 6c74  _combined_result
 00001b40: 73ee 0000 0073 1e00 0000 0802 0401 0202  s....s..........
 00001b50: 0801 0a01 0c01 0802 0a01 0a01 0480 0c02  ................
 00001b60: 1201 02ff 0a03 0802 7a1b 5574 696c 732e  ........z.Utils.
 00001b70: 7265 6164 5f63 6f6d 6269 6e65 645f 7265  read_combined_re
@@ -450,18 +450,18 @@
 00001c10: 0066 0164 0964 0484 0874 027c 006a 0083  .f.d.d...t.|.j..
 00001c20: 0144 0083 0164 0583 027d 047c 0472 4c7c  .D...d...}.|.rL|
 00001c30: 03a0 077c 04a1 0101 0071 3374 0864 0a88  ...|.....q3t.d..
 00001c40: 009b 0064 0b74 046a 059b 0064 0c74 046a  ...d.t.j...d.t.j
 00001c50: 059b 0064 0d9d 0783 0182 017c 017c 037c  ...d.......|.|.|
 00001c60: 0266 0353 0029 0e4e 6301 0000 0000 0000  .f.S.).Nc.......
 00001c70: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
-00001c80: 0072 8100 0000 7214 0000 00a9 0172 8b00  .r....r......r..
-00001c90: 0000 7283 0000 0072 1400 0000 7214 0000  ..r....r....r...
+00001c80: 0072 8200 0000 7214 0000 00a9 0172 8c00  .r....r......r..
+00001c90: 0000 7284 0000 0072 1400 0000 7214 0000  ..r....r....r...
 00001ca0: 0072 1500 0000 7239 0000 0005 0100 0072  .r....r9.......r
-00001cb0: 8400 0000 7a2a 5574 696c 732e 6669 6e64  ....z*Utils.find
+00001cb0: 8500 0000 7a2a 5574 696c 732e 6669 6e64  ....z*Utils.find
 00001cc0: 5f63 6f6c 756d 6e5f 6c6f 6373 2e3c 6c6f  _column_locs.<lo
 00001cd0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
 00001ce0: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
 00001cf0: 0003 0000 0073 0000 00f3 2000 0000 8100  .....s.... .....
 00001d00: 7c00 5d0b 5c02 7d01 7d02 6400 7c02 7600  |.].\.}.}.d.|.v.
 00001d10: 7202 7c01 5600 0100 7102 6401 5300 2902  r.|.V...q.d.S.).
 00001d20: 7a0b 6967 6e6f 7265 2066 696c 654e 7214  z.ignore fileNr.
@@ -469,48 +469,48 @@
 00001d40: 7465 7272 4800 0000 7214 0000 0072 1400  terrH...r....r..
 00001d50: 0000 7215 0000 00da 093c 6765 6e65 7870  ..r......<genexp
 00001d60: 723e 0701 0000 7304 0000 0002 801e 007a  r>....s........z
 00001d70: 2955 7469 6c73 2e66 696e 645f 636f 6c75  )Utils.find_colu
 00001d80: 6d6e 5f6c 6f63 732e 3c6c 6f63 616c 733e  mn_locs.<locals>
 00001d90: 2e3c 6765 6e65 7870 723e 4663 0100 0000  .<genexpr>Fc....
 00001da0: 0000 0000 0000 0000 0300 0000 0300 0000  ................
-00001db0: 7300 0000 729d 0000 0029 02da 0862 6173  s...r....)...bas
-00001dc0: 656c 696e 654e 7214 0000 0072 9e00 0000  elineNr....r....
+00001db0: 7300 0000 729e 0000 0029 02da 0862 6173  s...r....)...bas
+00001dc0: 656c 696e 654e 7214 0000 0072 9f00 0000  elineNr....r....
 00001dd0: 7214 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
-00001de0: a000 0000 0a01 0000 7308 0000 0002 800a  ........s.......
+00001de0: a100 0000 0a01 0000 7308 0000 0002 800a  ........s.......
 00001df0: 0006 010e ff7a 1c4e 6f20 6261 7365 6c69  .....z.No baseli
 00001e00: 6e65 2063 6f6c 756d 6e20 666f 756e 6420  ne column found 
 00001e10: 696e 2072 3300 0000 6301 0000 0000 0000  in r3...c.......
 00001e20: 0000 0000 0003 0000 0003 0000 0033 0000  .............3..
 00001e30: 0073 2400 0000 8100 7c00 5d0d 5c02 7d01  .s$.....|.].\.}.
 00001e40: 7d02 8800 a000 a100 7c02 6b02 7202 7c01  }.......|.k.r.|.
 00001e50: 5600 0100 7102 6400 5300 7241 0000 0072  V...q.d.S.rA...r
-00001e60: 9c00 0000 729e 0000 00a9 01da 036b 6579  ....r........key
-00001e70: 7214 0000 0072 1500 0000 72a0 0000 0011  r....r....r.....
+00001e60: 9d00 0000 729f 0000 00a9 01da 036b 6579  ....r........key
+00001e70: 7214 0000 0072 1500 0000 72a1 0000 0011  r....r....r.....
 00001e80: 0100 0073 0400 0000 0280 2200 7a05 4b65  ...s......".z.Ke
 00001e90: 7920 227a 0f22 206e 6f74 2066 6f75 6e64  y "z." not found
 00001ea0: 2069 6e20 7a76 2e20 4368 6563 6b20 7468   in zv. Check th
 00001eb0: 6520 4372 6974 6963 616c 2050 6172 616d  e Critical Param
 00001ec0: 6574 6572 7320 6f70 7469 6f6e 2069 6e20  eters option in 
 00001ed0: 7468 6520 5061 7273 696e 6720 6d65 6e75  the Parsing menu
 00001ee0: 2028 7061 7261 6d65 7465 725f 6469 6374   (parameter_dict
 00001ef0: 3120 6966 206e 6f74 2075 7369 6e67 2074  1 if not using t
 00001f00: 6865 2047 5549 2920 636f 7272 6563 746c  he GUI) correctl
 00001f10: 7920 6d61 7463 6820 7468 6520 7a09 2068  y match the z. h
 00001f20: 6561 6465 7273 2e29 0972 4200 0000 da04  eaders.).rB.....
-00001f30: 6e65 7874 7288 0000 00da 094e 616d 6545  nextr......NameE
-00001f40: 7272 6f72 7256 0000 0072 7600 0000 da0e  rrorrV...rv.....
+00001f30: 6e65 7874 7289 0000 00da 094e 616d 6545  nextr......NameE
+00001f40: 7272 6f72 7256 0000 0072 7700 0000 da0e  rrorrV...rw.....
 00001f50: 7061 7261 6d65 7465 725f 6469 6374 da06  parameter_dict..
-00001f60: 6170 7065 6e64 7296 0000 0029 05da 0574  appendr....)...t
+00001f60: 6170 7065 6e64 7297 0000 0029 05da 0574  appendr....)...t
 00001f70: 6162 6c65 da11 6967 6e6f 7265 5f63 6f6c  able..ignore_col
 00001f80: 756d 6e5f 6c6f 635a 1362 6173 656c 696e  umn_locZ.baselin
 00001f90: 655f 636f 6c75 6d6e 5f6c 6f63 da14 6372  e_column_loc..cr
 00001fa0: 6974 6963 616c 5f63 6f6c 756d 6e5f 6c6f  itical_column_lo
 00001fb0: 6373 5a0a 636f 6c75 6d6e 5f6c 6f63 7214  csZ.column_locr.
-00001fc0: 0000 0072 a200 0000 7215 0000 00da 1066  ...r....r......f
+00001fc0: 0000 0072 a300 0000 7215 0000 00da 1066  ...r....r......f
 00001fd0: 696e 645f 636f 6c75 6d6e 5f6c 6f63 7303  ind_column_locs.
 00001fe0: 0100 0073 2400 0000 1202 1402 0201 04ff  ...s$...........
 00001ff0: 1403 0201 04ff 0402 1201 0402 0a01 1e01  ................
 00002000: 0402 0c01 1202 0402 0afe 0a04 7a16 5574  ............z.Ut
 00002010: 696c 732e 6669 6e64 5f63 6f6c 756d 6e5f  ils.find_column_
 00002020: 6c6f 6373 6301 0000 0000 0000 0000 0000  locsc...........
 00002030: 0004 0000 0008 0000 0043 0000 0073 8200  .........C...s..
@@ -535,33 +535,33 @@
 00002160: 7220 636f 6e74 6169 6e73 2061 6c6c 2074  r contains all t
 00002170: 6865 2070 6172 7469 6369 7061 6e74 2064  he participant d
 00002180: 6972 6563 746f 7269 6573 2069 6e20 7468  irectories in th
 00002190: 6520 6e65 6365 7373 6172 7920 4249 4453  e necessary BIDS
 000021a0: 2066 6f72 6d61 7420 652e 672e 2073 7562   format e.g. sub
 000021b0: 2d30 312e 290a 7234 0000 00da 0667 6574  -01.).r4.....get
 000021c0: 6377 6472 3500 0000 da06 6973 6669 6c65  cwdr5.....isfile
-000021d0: 7256 0000 0072 7600 0000 724c 0000 00da  rV...rv...rL....
-000021e0: 0872 6561 645f 6373 7672 5400 0000 7296  .read_csvrT...r.
-000021f0: 0000 0029 0472 3c00 0000 7299 0000 0072  ...).r<...r....r
-00002200: a800 0000 da0b 666f 6c64 6572 5f74 7970  ......folder_typ
+000021d0: 7256 0000 0072 7700 0000 724c 0000 00da  rV...rw...rL....
+000021e0: 0872 6561 645f 6373 7672 5400 0000 7297  .read_csvrT...r.
+000021f0: 0000 0029 0472 3c00 0000 729a 0000 0072  ...).r<...r....r
+00002200: a900 0000 da0b 666f 6c64 6572 5f74 7970  ......folder_typ
 00002210: 6572 1400 0000 7214 0000 0072 1500 0000  er....r....r....
 00002220: da15 6c6f 6164 5f70 6172 616d 5661 6c75  ..load_paramValu
 00002230: 6573 5f66 696c 651c 0100 0073 1c00 0000  es_file....s....
 00002240: 0402 0601 0802 1802 1601 0401 080c 02f7  ................
 00002250: 1001 0601 0807 0cfb 0801 02ff 7a1b 5574  ............z.Ut
 00002260: 696c 732e 6c6f 6164 5f70 6172 616d 5661  ils.load_paramVa
 00002270: 6c75 6573 5f66 696c 6563 0100 0000 0000  lues_filec......
 00002280: 0000 0000 0000 0100 0000 0800 0000 4300  ..............C.
 00002290: 0000 7326 0000 007a 0874 00a0 017c 00a1  ..s&...z.t...|..
 000022a0: 0101 0057 0064 0053 0004 0074 0279 1201  ...W.d.S...t.y..
 000022b0: 0001 0001 0059 0064 0053 0077 0072 4100  .....Y.d.S.w.rA.
 000022c0: 0000 2903 7234 0000 00da 056d 6b64 6972  ..).r4.....mkdir
 000022d0: da0f 4669 6c65 4578 6973 7473 4572 726f  ..FileExistsErro
 000022e0: 7229 0172 3500 0000 7214 0000 0072 1400  r).r5...r....r..
-000022f0: 0000 7215 0000 0072 7b00 0000 3301 0000  ..r....r{...3...
+000022f0: 0000 7215 0000 0072 7c00 0000 3301 0000  ..r....r|...3...
 00002300: 730a 0000 0002 0210 010c 0106 0102 ff7a  s..............z
 00002310: 0c55 7469 6c73 2e6d 6b5f 6469 7263 0000  .Utils.mk_dirc..
 00002320: 0000 0000 0000 0000 0000 0100 0000 0400  ................
 00002330: 0000 4700 0000 731e 0000 0074 007c 0064  ..G...s....t.|.d
 00002340: 0119 007c 0064 0219 0083 027c 0064 0364  ...|.d.....|.d.d
 00002350: 0085 0219 008e 0053 0029 044e 7201 0000  .......S.).Nr...
 00002360: 0072 1e00 0000 e902 0000 0029 01da 0767  .r.........)...g
@@ -571,366 +571,366 @@
 000023a0: 616e 646c 6572 3a01 0000 7302 0000 001e  andler:...s.....
 000023b0: 027a 1d55 7469 6c73 2e69 6e73 7461 6e63  .z.Utils.instanc
 000023c0: 655f 6d65 7468 6f64 5f68 616e 646c 6572  e_method_handler
 000023d0: 6300 0000 0000 0000 0000 0000 0001 0000  c...............
 000023e0: 0004 0000 0047 0000 0073 1400 0000 7c00  .....G...s....|.
 000023f0: 6401 1900 7c00 6402 6400 8502 1900 8e00  d...|.d.d.......
 00002400: 5300 2903 4e72 0100 0000 721e 0000 0072  S.).Nr....r....r
-00002410: 1400 0000 72b7 0000 0072 1400 0000 7214  ....r....r....r.
+00002410: 1400 0000 72b8 0000 0072 1400 0000 7214  ....r....r....r.
 00002420: 0000 0072 1500 0000 da14 636c 6173 735f  ...r......class_
 00002430: 6d65 7468 6f64 5f68 616e 646c 6572 3e01  method_handler>.
 00002440: 0000 7251 0000 007a 1a55 7469 6c73 2e63  ..rQ...z.Utils.c
 00002450: 6c61 7373 5f6d 6574 686f 645f 6861 6e64  lass_method_hand
 00002460: 6c65 7263 0100 0000 0000 0000 0000 0000  lerc............
-00002470: 0300 0000 0400 0000 4300 0000 734a 0000  ........C...sJ..
+00002470: 0300 0000 0400 0000 4300 0000 734e 0000  ........C...sN..
 00002480: 0074 006a 0164 016b 0272 0a74 02a0 03a1  .t.j.d.k.r.t....
-00002490: 007d 016e 0374 006a 017d 0174 02a0 0464  .}.n.t.j.}.t...d
-000024a0: 02a1 017d 0274 006a 0572 1f7c 0073 1f74  ...}.t.j.r.|.s.t
-000024b0: 0664 037c 019b 0064 049d 0383 0101 007c  .d.|...d.......|
-000024c0: 026a 077c 0164 058d 0153 0029 064e da03  .j.|.d...S.).N..
-000024d0: 6d61 78da 0a66 6f72 6b73 6572 7665 727a  max..forkserverz
-000024e0: 200a 5374 6172 7469 6e67 2070 726f 6365   .Starting proce
-000024f0: 7373 696e 6720 706f 6f6c 2075 7369 6e67  ssing pool using
-00002500: 207a 0720 636f 7265 732e 2901 da09 7072   z. cores.)...pr
-00002510: 6f63 6573 7365 7329 0872 5600 0000 5a0e  ocesses).rV...Z.
-00002520: 6d61 785f 636f 7265 5f75 7361 6765 da02  max_core_usage..
-00002530: 6d70 da09 6370 755f 636f 756e 74da 0b67  mp..cpu_count..g
-00002540: 6574 5f63 6f6e 7465 7874 7257 0000 0072  et_contextrW...r
-00002550: 5800 0000 da04 506f 6f6c 2903 da07 7265  X.....Pool)...re
-00002560: 7374 6172 74da 0777 6f72 6b65 7273 da03  start..workers..
-00002570: 6374 7872 1400 0000 7214 0000 0072 1500  ctxr....r....r..
-00002580: 0000 da15 7374 6172 745f 7072 6f63 6573  ....start_proces
-00002590: 7369 6e67 5f70 6f6f 6c42 0100 0073 0e00  sing_poolB...s..
-000025a0: 0000 0a02 0a01 0602 0a02 0a02 1001 0c02  ................
-000025b0: 7a1b 5574 696c 732e 7374 6172 745f 7072  z.Utils.start_pr
-000025c0: 6f63 6573 7369 6e67 5f70 6f6f 6c63 0200  ocessing_poolc..
-000025d0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-000025e0: 0000 4300 0000 7324 0000 007c 00a0 00a1  ..C...s$...|....
-000025f0: 0001 007c 00a0 01a1 0001 007c 0172 1074  ...|.......|.r.t
-00002600: 026a 0364 0164 028d 017d 007c 0053 0029  .j.d.d...}.|.S.)
-00002610: 034e 5429 0172 c200 0000 2904 da05 636c  .NT).r....)...cl
-00002620: 6f73 65da 046a 6f69 6e72 0800 0000 72c5  ose..joinr....r.
-00002630: 0000 0029 02da 0470 6f6f 6c72 c200 0000  ...)...poolr....
-00002640: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
-00002650: 146a 6f69 6e5f 7072 6f63 6573 7369 6e67  .join_processing
-00002660: 5f70 6f6f 6c50 0100 0073 0a00 0000 0802  _poolP...s......
-00002670: 0801 0402 0c01 0402 7a1a 5574 696c 732e  ........z.Utils.
-00002680: 6a6f 696e 5f70 726f 6365 7373 696e 675f  join_processing_
-00002690: 706f 6f6c 6305 0000 0000 0000 0000 0000  poolc...........
-000026a0: 0008 0000 000a 0000 0043 0000 0073 1801  .........C...s..
-000026b0: 0000 7400 7c01 9b00 6401 7c02 9b00 9d03  ..t.|...d.|.....
-000026c0: 6402 8302 8f78 7d05 7a67 7c05 a001 a100  d....x}.zg|.....
-000026d0: 7d06 7402 a003 6403 a004 7c06 a101 a101  }.t...d...|.....
-000026e0: 7d06 7c06 4400 5d0c 7d07 7c06 7c07 1900  }.|.D.].}.|.|...
-000026f0: 6404 6b02 7226 6400 7c06 7c07 3c00 711a  d.k.r&d.|.|.<.q.
-00002700: 7c03 7229 7405 6410 6900 7c06 a401 8e01  |.r)t.d.i.|.....
-00002710: 6106 7407 6a08 a009 7c01 a101 6405 1900  a.t.j...|...d...
-00002720: 6406 6b02 7256 6700 6407 a201 6700 6408  d.k.rVg.d...g.d.
-00002730: a201 6409 9c02 7406 5f0a 640a 640b 8400  ..d...t._.d.d...
-00002740: 740b 740c 7406 6a0d 8301 8301 4400 8301  t.t.t.j.....D...
-00002750: 7406 5f0e 740f a010 7406 a101 0100 7c02  t._.t...t.....|.
-00002760: 640c 6b02 7269 7c04 7406 5f11 7c04 7406  d.k.ri|.t._.|.t.
-00002770: 5f12 640d 7406 5f13 640e 7406 5f14 640e  _.d.t._.d.t._.d.
-00002780: 7406 5f15 7406 5700 5700 0200 6400 0400  t._.t.W.W...d...
-00002790: 0400 8303 0100 5300 0400 7402 6a16 6a17  ......S...t.j.j.
-000027a0: 7418 6602 7981 0100 0100 0100 7419 640f  t.f.y.......t.d.
-000027b0: 8301 8201 7700 3100 7385 7701 0100 0100  ....w.1.s.w.....
-000027c0: 0100 5900 0100 6400 5300 2911 4e72 6300  ..Y...d.S.).Nrc.
-000027d0: 0000 7265 0000 0072 2300 0000 da04 4e6f  ..re...r#.....No
-000027e0: 6e65 7267 0000 005a 0c72 6f69 5f61 6e61  nerg...Z.roi_ana
-000027f0: 6c79 7369 7329 0b7a 0c54 6f74 616c 2076  lysis).z.Total v
-00002800: 6f78 656c 737a 0f45 7863 6c75 6465 6420  oxelsz.Excluded 
-00002810: 766f 7865 6c73 7a1a 4176 6572 6167 6520  voxelsz.Average 
-00002820: 766f 7865 6c73 2070 6572 2073 6573 7369  voxels per sessi
-00002830: 6f6e da04 4d65 616e da07 5374 645f 6465  on..Mean..Std_de
-00002840: 76da 1343 6f6e 6669 6465 6e63 655f 696e  v..Confidence_in
-00002850: 7465 7276 616c da06 4d65 6469 616e da07  terval..Median..
-00002860: 4d69 6e69 6d75 6dda 074d 6178 696d 756d  Minimum..Maximum
-00002870: da0c 5061 7274 6963 6970 616e 7473 da08  ..Participants..
-00002880: 5365 7373 696f 6e73 290a 5a0c 566f 7865  Sessions).Z.Voxe
-00002890: 6c5f 616d 6f75 6e74 da16 4578 636c 7564  l_amount..Exclud
-000028a0: 6564 5f76 6f78 656c 735f 616d 6f75 6e74  ed_voxels_amount
-000028b0: 5a0e 4176 6572 6167 655f 766f 7865 6c73  Z.Average_voxels
-000028c0: 72cb 0000 005a 1253 7461 6e64 6172 645f  r....Z.Standard_
-000028d0: 6465 7669 6174 696f 6e72 cd00 0000 72ce  deviationr....r.
-000028e0: 0000 0072 cf00 0000 72d0 0000 0072 d200  ...r....r....r..
-000028f0: 0000 2902 7294 0000 0072 9300 0000 6301  ..).r....r....c.
-00002900: 0000 0000 0000 0000 0000 0002 0000 0005  ................
-00002910: 0000 0053 0000 0073 1e00 0000 6900 7c00  ...S...s....i.|.
-00002920: 5d0b 7d01 7400 6a01 7c01 1900 7400 6a02  ].}.t.j.|...t.j.
-00002930: 7c01 1900 9302 7102 5300 7214 0000 0029  |.....q.S.r....)
-00002940: 0372 5600 0000 da0f 7061 7261 6d65 7465  .rV.....paramete
-00002950: 725f 6469 6374 31da 0f70 6172 616d 6574  r_dict1..paramet
-00002960: 6572 5f64 6963 7432 2902 7237 0000 00da  er_dict2).r7....
-00002970: 0169 7214 0000 0072 1400 0000 7215 0000  .ir....r....r...
-00002980: 00da 0a3c 6469 6374 636f 6d70 3e84 0100  ...<dictcomp>...
-00002990: 0073 0a00 0000 0600 0201 08ff 0801 06ff  .s..............
-000029a0: 7a25 5574 696c 732e 6c6f 6164 5f63 6f6e  z%Utils.load_con
-000029b0: 6669 672e 3c6c 6f63 616c 733e 2e3c 6469  fig.<locals>.<di
-000029c0: 6374 636f 6d70 3e7a 1074 6573 745f 636f  ctcomp>z.test_co
-000029d0: 6e66 6967 2e74 6f6d 6c5a 0f74 6573 745f  nfig.tomlZ.test_
-000029e0: 524f 495f 7265 706f 7274 5a09 7465 7374  ROI_reportZ.test
-000029f0: 5f6d 6170 737a 3543 6f6e 6669 6720 6669  _mapsz5Config fi
-00002a00: 6c65 206e 6f74 2069 6e20 636f 7272 6563  le not in correc
-00002a10: 7420 666f 726d 6174 206f 7220 6d69 7373  t format or miss
-00002a20: 696e 6720 656e 7472 6965 732e 7214 0000  ing entries.r...
-00002a30: 0029 1a72 6800 0000 da09 7265 6164 6c69  .).rh.....readli
-00002a40: 6e65 73da 0474 6f6d 6cda 056c 6f61 6473  nes..toml..loads
-00002a50: 72c7 0000 0072 0600 0000 7256 0000 0072  r....r....rV...r
-00002a60: 3400 0000 7235 0000 0072 8e00 0000 da11  4...r5...r......
-00002a70: 7374 6174 6973 7469 635f 6f70 7469 6f6e  statistic_option
-00002a80: 7372 8c00 0000 728d 0000 0072 d400 0000  sr....r....r....
-00002a90: 72a6 0000 0072 0800 0000 da14 636c 6561  r....r......clea
-00002aa0: 6e5f 636f 6e66 6967 5f6f 7074 696f 6e73  n_config_options
-00002ab0: da0e 6272 6169 6e5f 6669 6c65 5f6c 6f63  ..brain_file_loc
-00002ac0: 72ac 0000 00da 0d6f 7574 7075 745f 666f  r......output_fo
-00002ad0: 6c64 6572 5a12 6f75 7470 7574 5f66 6f6c  lderZ.output_fol
-00002ae0: 6465 725f 6e61 6d65 da0f 7374 6174 5f6d  der_name..stat_m
-00002af0: 6170 5f66 6f6c 6465 72da 0764 6563 6f64  ap_folder..decod
-00002b00: 6572 da0f 546f 6d6c 4465 636f 6465 4572  er..TomlDecodeEr
-00002b10: 726f 72da 0e41 7474 7269 6275 7465 4572  ror..AttributeEr
-00002b20: 726f 7272 9600 0000 2908 da03 636c 7372  rorr....)...clsr
-00002b30: 6b00 0000 da08 6669 6c65 6e61 6d65 da04  k.....filename..
-00002b40: 7361 7665 7235 0000 00da 0874 6f6d 6c66  saver5.....tomlf
-00002b50: 696c 65da 0570 6172 7365 72a3 0000 0072  ile..parser....r
-00002b60: 1400 0000 7214 0000 0072 1500 0000 da0b  ....r....r......
-00002b70: 6c6f 6164 5f63 6f6e 6669 675a 0100 0073  load_configZ...s
-00002b80: 3c00 0000 1602 0201 0801 1001 0802 0c01  <...............
-00002b90: 0801 0280 0402 0e03 1402 0602 060c 08f3  ................
-00002ba0: 0619 0c01 08ff 0a03 0802 0602 0601 0601  ................
-00002bb0: 0601 0601 0402 10cb 1437 0801 02ff 14c9  .........7......
-00002bc0: 7a11 5574 696c 732e 6c6f 6164 5f63 6f6e  z.Utils.load_con
-00002bd0: 6669 6763 0100 0000 0000 0000 0000 0000  figc............
-00002be0: 0300 0000 0700 0000 4300 0000 736e 0000  ........C...sn..
-00002bf0: 0067 0064 01a2 017d 0174 007c 006a 0183  .g.d...}.t.|.j..
-00002c00: 0174 0275 0172 127c 01a0 037c 006a 01a1  .t.u.r.|...|.j..
-00002c10: 017c 005f 0167 0064 02a2 017d 0274 007c  .|._.g.d...}.t.|
-00002c20: 006a 0483 0174 0275 0172 3564 0374 0564  .j...t.u.r5d.t.d
-00002c30: 0474 06a0 0764 057c 006a 04a1 0264 0619  .t...d.|.j...d..
-00002c40: 009b 009d 0283 0118 007c 005f 087c 02a0  .........|._.|..
-00002c50: 037c 006a 04a1 017c 005f 047c 0053 0029  .|.j...|._.|.S.)
-00002c60: 074e 290d 7a13 4365 7265 6265 6c6c 756d  .N).z.Cerebellum
-00002c70: 2d4d 4e49 666c 6972 747a 1343 6572 6562  -MNIflirtz.Cereb
-00002c80: 656c 6c75 6d2d 4d4e 4966 6e69 7274 7a12  ellum-MNIfnirtz.
-00002c90: 4861 7276 6172 644f 7866 6f72 642d 636f  HarvardOxford-co
-00002ca0: 7274 7a11 4861 7276 6172 644f 7866 6f72  rtz.HarvardOxfor
-00002cb0: 642d 7375 627a 0f4a 4855 2d49 4342 4d2d  d-subz.JHU-ICBM-
-00002cc0: 6c61 6265 6c73 7a0f 4a48 552d 4943 424d  labelsz.JHU-ICBM
-00002cd0: 2d74 7261 6374 735a 076a 7565 6c69 6368  -tractsZ.juelich
-00002ce0: da03 4d4e 497a 0c53 4d41 5454 2d6c 6162  ..MNIz.SMATT-lab
-00002cf0: 656c 73da 0353 544e 7a13 7374 7269 6174  els..STNz.striat
-00002d00: 756d 2d73 7472 7563 7475 7261 6c7a 1054  um-structuralz.T
-00002d10: 616c 6169 7261 6368 2d6c 6162 656c 73da  alairach-labels.
-00002d20: 0854 6861 6c61 6d75 7329 067a 0938 3025  .Thalamus).z.80%
-00002d30: 2c20 312e 3238 7a09 3835 252c 2031 2e34  , 1.28z.85%, 1.4
-00002d40: 347a 0939 3025 2c20 312e 3634 7a09 3935  4z.90%, 1.64z.95
-00002d50: 252c 2031 2e39 367a 0939 3825 2c20 322e  %, 1.96z.98%, 2.
-00002d60: 3333 7a09 3939 252c 2032 2e35 3872 1e00  33z.99%, 2.58r..
-00002d70: 0000 7a02 302e 7222 0000 0072 0100 0000  ..z.0.r"...r....
-00002d80: 2909 721f 0000 00da 0c61 746c 6173 5f6e  ).r......atlas_n
-00002d90: 756d 6265 7272 9000 0000 724a 0000 00da  umberr....rJ....
-00002da0: 1163 6f6e 665f 6c65 7665 6c5f 6e75 6d62  .conf_level_numb
-00002db0: 6572 da05 666c 6f61 74da 0272 6572 8e00  er..float..rer..
-00002dc0: 0000 da0f 626f 6f74 7374 7261 705f 616c  ....bootstrap_al
-00002dd0: 7068 6129 0372 5600 0000 da0d 6174 6c61  pha).rV.....atla
-00002de0: 735f 6f70 7469 6f6e 735a 1263 6f6e 665f  s_optionsZ.conf_
-00002df0: 6c65 7665 6c5f 6f70 7469 6f6e 7372 1400  level_optionsr..
-00002e00: 0000 7214 0000 0072 1500 0000 72dc 0000  ..r....r....r...
-00002e10: 0096 0100 0073 1000 0000 0802 0e05 0e01  .....s..........
-00002e20: 0802 0e02 2201 0e01 0402 7a1a 5574 696c  ....".....z.Util
-00002e30: 732e 636c 6561 6e5f 636f 6e66 6967 5f6f  s.clean_config_o
-00002e40: 7074 696f 6e73 6301 0000 0000 0000 0000  ptionsc.........
-00002e50: 0000 0003 0000 0003 0000 0043 0000 0073  ...........C...s
-00002e60: 2000 0000 7400 a001 7c00 a101 7d01 7c01   ...t...|...}.|.
-00002e70: 6a02 7d02 7c01 a003 a100 7d01 7c01 7c02  j.}.|.....}.|.|.
-00002e80: 6602 5300 7241 0000 0029 04da 036e 6962  f.S.rA...)...nib
-00002e90: da04 6c6f 6164 da06 6865 6164 6572 da09  ..load..header..
-00002ea0: 6765 745f 6664 6174 6129 03da 0966 696c  get_fdata)...fil
-00002eb0: 655f 7061 7468 da04 6461 7461 72f4 0000  e_path..datar...
-00002ec0: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
-00002ed0: da0a 6c6f 6164 5f62 7261 696e a801 0000  ..load_brain....
-00002ee0: 7308 0000 000a 0206 0208 0108 027a 1055  s............z.U
-00002ef0: 7469 6c73 2e6c 6f61 645f 6272 6169 6e63  tils.load_brainc
-00002f00: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00002f10: 0500 0000 4300 0000 7322 0000 0067 0064  ....C...s"...g.d
-00002f20: 01a2 017d 017c 0144 005d 087d 027c 00a0  ...}.|.D.].}.|..
-00002f30: 007c 0264 02a1 027d 0071 067c 0053 0029  .|.d...}.q.|.S.)
-00002f40: 034e 2904 7a07 2e6e 6969 2e67 7a7a 042e  .N).z..nii.gzz..
-00002f50: 6e69 697a 042e 6864 727a 052e 6a73 6f6e  niiz..hdrz..json
-00002f60: 7223 0000 0029 0172 2a00 0000 2903 7235  r#...).r*...).r5
-00002f70: 0000 0072 3d00 0000 723f 0000 0072 1400  ...r=...r?...r..
-00002f80: 0000 7214 0000 0072 1500 0000 da09 7374  ..r....r......st
-00002f90: 7269 705f 6578 74b1 0100 0073 0800 0000  rip_ext....s....
-00002fa0: 0802 0802 0e01 0402 7a0f 5574 696c 732e  ........z.Utils.
-00002fb0: 7374 7269 705f 6578 7463 0100 0000 0000  strip_extc......
-00002fc0: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
-00002fd0: 0000 735c 0000 0064 0164 0284 0074 007c  ..s\...d.d...t.|
-00002fe0: 009b 0064 039d 0283 0144 0083 017d 0164  ...d.....D...}.d
-00002ff0: 0464 0284 007c 0144 0083 017d 0274 017c  .d...|.D...}.t.|
-00003000: 0183 0164 056b 0272 1d74 0264 0683 0182  ...d.k.r.t.d....
-00003010: 0174 036a 0472 2a74 0564 0774 017c 0183  .t.j.r*t.d.t.|..
-00003020: 019b 0064 089d 0383 0101 007c 017c 0266  ...d.......|.|.f
-00003030: 0253 0029 094e 6301 0000 0000 0000 0000  .S.).Nc.........
-00003040: 0000 0002 0000 0006 0000 0053 0000 0073  ...........S...s
-00003050: 1c00 0000 6700 7c00 5d0a 7d01 7400 a001  ....g.|.].}.t...
-00003060: 6400 7c01 a102 7202 7c01 9102 7102 5300  d.|...r.|...q.S.
-00003070: 2901 7a0b 7375 622d 5b30 2d39 5d2b 2429  ).z.sub-[0-9]+$)
-00003080: 0272 ef00 0000 da06 7365 6172 6368 2902  .r......search).
-00003090: 7237 0000 00da 0564 6972 6563 7214 0000  r7.....direcr...
-000030a0: 0072 1400 0000 7215 0000 0072 3900 0000  .r....r....r9...
-000030b0: bd01 0000 7302 0000 001c 007a 2f55 7469  ....s......z/Uti
-000030c0: 6c73 2e66 696e 645f 7061 7274 6963 6970  ls.find_particip
-000030d0: 616e 745f 6469 7273 2e3c 6c6f 6361 6c73  ant_dirs.<locals
-000030e0: 3e2e 3c6c 6973 7463 6f6d 703e 7a02 2f2a  >.<listcomp>z./*
-000030f0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00003100: 0005 0000 0053 0000 0073 1a00 0000 6700  .....S...s....g.
-00003110: 7c00 5d09 7d01 7c01 a000 6400 a101 6401  |.].}.|...d...d.
-00003120: 1900 9102 7102 5300 2902 7263 0000 0072  ....q.S.).rc...r
-00003130: 6700 0000 2901 728e 0000 0029 0272 3700  g...).r....).r7.
-00003140: 0000 da0b 7061 7274 6963 6970 616e 7472  ....participantr
-00003150: 1400 0000 7214 0000 0072 1500 0000 7239  ....r....r....r9
-00003160: 0000 00be 0100 0073 0200 0000 1a00 7201  .......s......r.
-00003170: 0000 007a 9e50 6172 7469 6369 7061 6e74  ...z.Participant
-00003180: 2064 6972 6563 746f 7269 6573 206e 6f74   directories not
-00003190: 2066 6f75 6e64 2e0a 4d61 6b65 2073 7572   found..Make sur
-000031a0: 6520 7061 7274 6963 6970 616e 7420 6469  e participant di
-000031b0: 7265 6374 6f72 6965 7320 6172 6520 6c61  rectories are la
-000031c0: 6265 6c6c 6564 2065 2e67 2e20 7375 622d  belled e.g. sub-
-000031d0: 3031 2061 6e64 2074 6865 2073 656c 6563  01 and the selec
-000031e0: 7465 6420 6469 7265 6374 6f72 7920 636f  ted directory co
-000031f0: 6e74 6169 6e73 2061 6c6c 2070 6172 7469  ntains all parti
-00003200: 6369 7061 6e74 2064 6972 6563 746f 7269  cipant directori
-00003210: 6573 2e7a 0646 6f75 6e64 207a 1520 7061  es.z.Found z. pa
-00003220: 7274 6963 6970 616e 7420 666f 6c64 6572  rticipant folder
-00003230: 732e 2906 7202 0000 0072 8d00 0000 7254  s.).r....r....rT
-00003240: 0000 0072 5600 0000 7257 0000 0072 5800  ...rV...rW...rX.
-00003250: 0000 2903 723c 0000 005a 1170 6172 7469  ..).r<...Z.parti
-00003260: 6369 7061 6e74 5f70 6174 6873 da11 7061  cipant_paths..pa
-00003270: 7274 6963 6970 616e 745f 6e61 6d65 7372  rticipant_namesr
-00003280: 1400 0000 7214 0000 0072 1500 0000 da15  ....r....r......
-00003290: 6669 6e64 5f70 6172 7469 6369 7061 6e74  find_participant
-000032a0: 5f64 6972 73ba 0100 0073 0e00 0000 1803  _dirs....s......
-000032b0: 0e01 0c02 0801 0603 1401 0802 7a1b 5574  ............z.Ut
-000032c0: 696c 732e 6669 6e64 5f70 6172 7469 6369  ils.find_partici
-000032d0: 7061 6e74 5f64 6972 7363 0100 0000 0000  pant_dirsc......
-000032e0: 0000 0000 0000 0400 0000 0800 0000 4300  ..............C.
-000032f0: 0000 73a4 0000 007c 0061 0064 017d 0164  ..s....|.a.d.}.d
-00003300: 027d 0274 0164 037c 009b 0064 0474 027c  .}.t.d.|...d.t.|
-00003310: 0183 019b 0064 0574 027c 0283 019b 0064  .....d.t.|.....d
-00003320: 069d 0783 0101 0074 036a 0464 0064 0785  .......t.j.d.d..
-00003330: 0219 007c 017c 0266 026b 0372 5074 0274  ...|.|.f.k.rPt.t
-00003340: 036a 0464 0819 0083 019b 0064 0574 0274  .j.d.......d.t.t
-00003350: 036a 0464 0919 0083 019b 0064 0574 0274  .j.d.......d.t.t
-00003360: 036a 0464 0719 0083 019b 009d 057d 0374  .j.d.........}.t
-00003370: 0164 0a7c 039b 0064 0b74 027c 0183 019b  .d.|...d.t.|....
-00003380: 0064 0574 027c 0283 019b 0064 0c9d 0783  .d.t.|.....d....
-00003390: 0101 0064 0053 0064 0053 0029 0d4e e903  ...d.S.d.S.).N..
-000033a0: 0000 00e9 0a00 0000 7a06 0a66 5241 5420  ........z..fRAT 
-000033b0: 7a25 2069 7320 6465 7665 6c6f 7065 6420  z% is developed 
-000033c0: 616e 6420 7465 7374 6564 2077 6974 6820  and tested with 
-000033d0: 5079 7468 6f6e 2072 3300 0000 7a02 2e0a  Python r3...z...
-000033e0: 72b5 0000 0072 0100 0000 721e 0000 007a  r....r....r....z
-000033f0: 1549 4e46 4f3a 2050 7974 686f 6e20 7665  .INFO: Python ve
-00003400: 7273 696f 6e20 7a2b 2069 7320 756e 7465  rsion z+ is unte
-00003410: 7374 6564 2e20 436f 6e73 6964 6572 2063  sted. Consider c
-00003420: 6861 6e67 696e 6720 746f 2076 6572 7369  hanging to versi
-00003430: 6f6e 207a 2220 6966 2074 6865 7265 2061  on z" if there a
-00003440: 7265 2065 7272 6f72 7320 7275 6e6e 696e  re errors runnin
-00003450: 6720 6652 4154 2e29 0572 6900 0000 7258  g fRAT.).ri...rX
-00003460: 0000 0072 5d00 0000 da03 7379 73da 0c76  ...r].....sys..v
-00003470: 6572 7369 6f6e 5f69 6e66 6f29 045a 0c66  ersion_info).Z.f
-00003480: 7261 745f 7665 7273 696f 6e5a 0c65 7870  rat_versionZ.exp
-00003490: 6563 745f 6d61 6a6f 725a 0c65 7870 6563  ect_majorZ.expec
-000034a0: 745f 6d69 6e6f 725a 0f63 7572 7265 6e74  t_minorZ.current
-000034b0: 5f76 6572 7369 6f6e 7214 0000 0072 1400  _versionr....r..
-000034c0: 0000 7215 0000 00da 0c63 6865 636b 7665  ..r......checkve
-000034d0: 7273 696f 6ec9 0100 0073 1800 0000 0403  rsion....s......
-000034e0: 0403 0401 2402 1601 3201 0a01 0601 04ff  ....$...2.......
-000034f0: 0601 0eff 04fe 7a12 5574 696c 732e 6368  ......z.Utils.ch
-00003500: 6563 6b76 6572 7369 6f6e 6302 0000 0000  eckversionc.....
-00003510: 0000 0000 0000 0004 0000 0008 0000 0043  ...............C
-00003520: 0000 0073 ae00 0000 7c00 6401 6b02 7209  ...s....|.d.k.r.
-00003530: 7c01 6a00 7209 6400 5300 7c01 6a01 7223  |.j.r.d.S.|.j.r#
-00003540: 6402 6403 6c02 6d03 7d02 0100 7404 a005  d.d.l.m.}...t...
-00003550: a100 9b00 6404 7c02 6a06 9b00 9d03 7d03  ....d.|.j.....}.
-00003560: 7404 a007 7c03 a101 0100 7c03 5300 7c01  t...|.....|.S.|.
-00003570: 6a08 6405 7600 7235 7409 6406 8301 0100  j.d.v.r5t.d.....
-00003580: 740a 6a0b 6407 6408 6409 8d02 7d03 7c03  t.j.d.d.d...}.|.
-00003590: 5300 7c01 6a08 7d03 7a07 7404 a007 7c03  S.|.j.}.z.t...|.
-000035a0: a101 0100 5700 6e0b 0400 740c 794a 0100  ....W.n...t.yJ..
-000035b0: 0100 0100 740c 640a 8301 8201 7700 7c01  ....t.d.....w.|.
-000035c0: 6a0d 7255 7409 640b 7c03 9b00 9d02 8301  j.rUt.d.|.......
-000035d0: 0100 7c03 5300 290c 4eda 0a53 7461 7469  ..|.S.).N..Stati
-000035e0: 7374 6963 7372 1e00 0000 2901 da11 456e  sticsr....)...En
-000035f0: 7669 726f 6e6d 656e 745f 5365 7475 7072  vironment_Setupr
-00003600: 6300 0000 2902 7223 0000 00fa 0120 7a28  c...).r#..... z(
-00003610: 5365 6c65 6374 2074 6865 2064 6972 6563  Select the direc
-00003620: 746f 7279 206f 7574 7075 7420 6279 2074  tory output by t
-00003630: 6865 2066 5241 542e 7a27 5365 6c65 6374  he fRAT.z'Select
-00003640: 2074 6865 2064 6972 6563 746f 7279 206f   the directory o
-00003650: 7574 7075 7420 6279 2074 6865 2066 5241  utput by the fRA
-00003660: 5454 2902 720b 0000 0072 5500 0000 7a4e  TT).r....rU...zN
-00003670: 4f75 7470 7574 2066 6f6c 6465 7220 6c6f  Output folder lo
-00003680: 6361 7469 6f6e 2028 6652 4154 206f 7574  cation (fRAT out
-00003690: 7075 7420 666f 6c64 6572 206c 6f63 6174  put folder locat
-000036a0: 696f 6e29 2069 7320 6e6f 7420 6120 7661  ion) is not a va
-000036b0: 6c69 6420 6469 7265 6374 6f72 792e 7a19  lid directory.z.
-000036c0: 4f75 7470 7574 2066 6f6c 6465 7220 7365  Output folder se
-000036d0: 6c65 6374 696f 6e3a 2029 0eda 0c72 756e  lection: )...run
-000036e0: 5f70 6c6f 7474 696e 67da 0c72 756e 5f61  _plotting..run_a
-000036f0: 6e61 6c79 7369 73da 0861 6e61 6c79 7369  nalysis..analysi
-00003700: 7372 0501 0000 7234 0000 0072 ae00 0000  sr....r4...r....
-00003710: da0d 7361 7665 5f6c 6f63 6174 696f 6e72  ..save_locationr
-00003720: 5500 0000 5a14 7265 706f 7274 5f6f 7574  U...Z.report_out
-00003730: 7075 745f 666f 6c64 6572 7258 0000 0072  put_folderrX...r
-00003740: 0800 0000 725a 0000 0072 5400 0000 7257  ....rZ...rT...rW
-00003750: 0000 0029 045a 0c63 7572 7265 6e74 5f73  ...).Z.current_s
-00003760: 7465 7072 5600 0000 7205 0100 005a 0e6a  teprV...r....Z.j
-00003770: 736f 6e5f 6469 7265 6374 6f72 7972 1400  son_directoryr..
-00003780: 0000 7214 0000 0072 1500 0000 da19 6368  ..r....r......ch
-00003790: 6469 725f 746f 5f6f 7574 7075 745f 6469  dir_to_output_di
-000037a0: 7265 6374 6f72 79d8 0100 0073 2c00 0000  rectory....s,...
-000037b0: 0e02 0401 0602 0c01 1401 0a02 0412 0af0  ................
-000037c0: 0801 0e01 040e 06f5 0202 0e01 0c01 0201  ................
-000037d0: 0201 04ff 02ff 0604 0e01 0402 7a1f 5574  ............z.Ut
-000037e0: 696c 732e 6368 6469 725f 746f 5f6f 7574  ils.chdir_to_out
-000037f0: 7075 745f 6469 7265 6374 6f72 7929 0272  put_directory).r
-00003800: 2300 0000 4629 034e 7261 0000 0072 6200  #...F).Nra...rb.
-00003810: 0000 2903 4654 4629 0146 2901 7223 0000  ..).FTF).F).r#..
-00003820: 0029 0254 4e29 1fda 085f 5f6e 616d 655f  .).TN)...__name_
-00003830: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00003840: 5f71 7561 6c6e 616d 655f 5fda 0c73 7461  _qualname__..sta
-00003850: 7469 636d 6574 686f 6472 1600 0000 7232  ticmethodr....r2
-00003860: 0000 0072 4000 0000 7249 0000 0072 5000  ...r@...rI...rP.
-00003870: 0000 725a 0000 0072 6000 0000 726f 0000  ..rZ...r`...ro..
-00003880: 0072 7800 0000 727d 0000 0072 9200 0000  .rx...r}...r....
-00003890: 729b 0000 0072 ab00 0000 72b2 0000 0072  r....r....r....r
-000038a0: 7b00 0000 72b9 0000 0072 ba00 0000 72c5  {...r....r....r.
-000038b0: 0000 0072 c900 0000 da0b 636c 6173 736d  ...r......classm
-000038c0: 6574 686f 6472 e800 0000 72dc 0000 0072  ethodr....r....r
-000038d0: f800 0000 72f9 0000 0072 fe00 0000 7203  ....r....r....r.
-000038e0: 0100 0072 0b01 0000 7214 0000 0072 1400  ...r....r....r..
-000038f0: 0000 7214 0000 0072 1500 0000 7208 0000  ..r....r....r...
-00003900: 0017 0000 0073 6a00 0000 0800 0201 0a01  .....sj.........
-00003910: 020f 0a01 022a 0a01 020d 0a01 0207 0a01  .....*..........
-00003920: 0203 0c01 0213 0a01 0206 0c01 0218 0c01  ................
-00003930: 0214 0c01 0208 0a01 022e 0a01 0214 0a01  ................
-00003940: 0218 0c01 0216 0a01 0206 0a01 0203 0a01  ................
-00003950: 0203 0c01 020d 0a01 0209 0c01 023b 0a01  .............;..
-00003960: 0211 0a01 0208 0a01 0208 0a01 020e 0a01  ................
-00003970: 020e 0e01 7208 0000 0029 1972 2500 0000  ....r....).r%...
-00003980: 720c 0000 0072 3400 0000 72ef 0000 0072  r....r4...r....r
-00003990: 7100 0000 7201 0100 0072 0200 0000 da07  q...r....r......
-000039a0: 7061 7468 6c69 6272 0300 0000 da07 746b  pathlibr......tk
-000039b0: 696e 7465 7272 0400 0000 7205 0000 00da  interr....r.....
-000039c0: 0574 7970 6573 7206 0000 005a 0c6d 756c  .typesr....Z.mul
-000039d0: 7469 7072 6f63 6573 7372 be00 0000 da07  tiprocessr......
-000039e0: 6e69 6261 6265 6c72 f200 0000 da06 7061  nibabelr......pa
-000039f0: 6e64 6173 724c 0000 0072 d900 0000 da1c  ndasrL...r......
-00003a00: 6652 4154 2e75 7469 6c73 2e66 5241 545f  fRAT.utils.fRAT_
-00003a10: 636f 6e66 6967 5f73 6574 7570 7256 0000  config_setuprV..
-00003a20: 0072 6900 0000 7208 0000 0072 1400 0000  .ri...r....r....
-00003a30: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
-00003a40: 083c 6d6f 6475 6c65 3e01 0000 0073 2400  .<module>....s$.
-00003a50: 0000 0800 0801 0801 0801 0801 0801 0c01  ................
-00003a60: 0c01 1001 0c01 0802 0801 0801 0801 0802  ................
-00003a70: 0402 0401 1203                           ......
+00002490: 007d 016e 0574 0474 006a 0183 017d 0174  .}.n.t.t.j...}.t
+000024a0: 02a0 0564 02a1 017d 0274 006a 0672 217c  ...d...}.t.j.r!|
+000024b0: 0073 2174 0764 037c 019b 0064 049d 0383  .s!t.d.|...d....
+000024c0: 0101 007c 026a 087c 0164 058d 0153 0029  ...|.j.|.d...S.)
+000024d0: 064e da03 6d61 78da 0a66 6f72 6b73 6572  .N..max..forkser
+000024e0: 7665 727a 200a 5374 6172 7469 6e67 2070  verz .Starting p
+000024f0: 726f 6365 7373 696e 6720 706f 6f6c 2075  rocessing pool u
+00002500: 7369 6e67 207a 0720 636f 7265 732e 2901  sing z. cores.).
+00002510: da09 7072 6f63 6573 7365 7329 0972 5600  ..processes).rV.
+00002520: 0000 5a0e 6d61 785f 636f 7265 5f75 7361  ..Z.max_core_usa
+00002530: 6765 da02 6d70 da09 6370 755f 636f 756e  ge..mp..cpu_coun
+00002540: 7472 9100 0000 da0b 6765 745f 636f 6e74  tr......get_cont
+00002550: 6578 7472 5700 0000 7258 0000 00da 0450  extrW...rX.....P
+00002560: 6f6f 6c29 03da 0772 6573 7461 7274 da07  ool)...restart..
+00002570: 776f 726b 6572 73da 0363 7478 7214 0000  workers..ctxr...
+00002580: 0072 1400 0000 7215 0000 00da 1573 7461  .r....r......sta
+00002590: 7274 5f70 726f 6365 7373 696e 675f 706f  rt_processing_po
+000025a0: 6f6c 4201 0000 730e 0000 000a 020a 010a  olB...s.........
+000025b0: 020a 020a 0210 010c 027a 1b55 7469 6c73  .........z.Utils
+000025c0: 2e73 7461 7274 5f70 726f 6365 7373 696e  .start_processin
+000025d0: 675f 706f 6f6c 6302 0000 0000 0000 0000  g_poolc.........
+000025e0: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
+000025f0: 2400 0000 7c00 a000 a100 0100 7c00 a001  $...|.......|...
+00002600: a100 0100 7c01 7210 7402 6a03 6401 6402  ....|.r.t.j.d.d.
+00002610: 8d01 7d00 7c00 5300 2903 4e54 2901 72c3  ..}.|.S.).NT).r.
+00002620: 0000 0029 04da 0563 6c6f 7365 da04 6a6f  ...)...close..jo
+00002630: 696e 7208 0000 0072 c600 0000 2902 da04  inr....r....)...
+00002640: 706f 6f6c 72c3 0000 0072 1400 0000 7214  poolr....r....r.
+00002650: 0000 0072 1500 0000 da14 6a6f 696e 5f70  ...r......join_p
+00002660: 726f 6365 7373 696e 675f 706f 6f6c 5001  rocessing_poolP.
+00002670: 0000 730a 0000 0008 0208 0104 020c 0104  ..s.............
+00002680: 027a 1a55 7469 6c73 2e6a 6f69 6e5f 7072  .z.Utils.join_pr
+00002690: 6f63 6573 7369 6e67 5f70 6f6f 6c63 0500  ocessing_poolc..
+000026a0: 0000 0000 0000 0000 0000 0800 0000 0a00  ................
+000026b0: 0000 4300 0000 7318 0100 0074 007c 019b  ..C...s....t.|..
+000026c0: 0064 017c 029b 009d 0364 0283 028f 787d  .d.|.....d....x}
+000026d0: 057a 677c 05a0 01a1 007d 0674 02a0 0364  .zg|.....}.t...d
+000026e0: 03a0 047c 06a1 01a1 017d 067c 0644 005d  ...|.....}.|.D.]
+000026f0: 0c7d 077c 067c 0719 0064 046b 0272 2664  .}.|.|...d.k.r&d
+00002700: 007c 067c 073c 0071 1a7c 0372 2974 0564  .|.|.<.q.|.r)t.d
+00002710: 1069 007c 06a4 018e 0161 0674 076a 08a0  .i.|.....a.t.j..
+00002720: 097c 01a1 0164 0519 0064 066b 0272 5667  .|...d...d.k.rVg
+00002730: 0064 07a2 0167 0064 08a2 0164 099c 0274  .d...g.d...d...t
+00002740: 065f 0a64 0a64 0b84 0074 0b74 0c74 066a  ._.d.d...t.t.t.j
+00002750: 0d83 0183 0144 0083 0174 065f 0e74 0fa0  .....D...t._.t..
+00002760: 1074 06a1 0101 007c 0264 0c6b 0272 697c  .t.....|.d.k.ri|
+00002770: 0474 065f 117c 0474 065f 1264 0d74 065f  .t._.|.t._.d.t._
+00002780: 1364 0e74 065f 1464 0e74 065f 1574 0657  .d.t._.d.t._.t.W
+00002790: 0057 0002 0064 0004 0004 0083 0301 0053  .W...d.........S
+000027a0: 0004 0074 026a 166a 1774 1866 0279 8101  ...t.j.j.t.f.y..
+000027b0: 0001 0001 0074 1964 0f83 0182 0177 0031  .....t.d.....w.1
+000027c0: 0073 8577 0101 0001 0001 0059 0001 0064  .s.w.......Y...d
+000027d0: 0053 0029 114e 7263 0000 0072 6500 0000  .S.).Nrc...re...
+000027e0: 7223 0000 00da 044e 6f6e 6572 6700 0000  r#.....Nonerg...
+000027f0: 5a0c 726f 695f 616e 616c 7973 6973 290b  Z.roi_analysis).
+00002800: 7a0c 546f 7461 6c20 766f 7865 6c73 7a0f  z.Total voxelsz.
+00002810: 4578 636c 7564 6564 2076 6f78 656c 737a  Excluded voxelsz
+00002820: 1a41 7665 7261 6765 2076 6f78 656c 7320  .Average voxels 
+00002830: 7065 7220 7365 7373 696f 6eda 044d 6561  per session..Mea
+00002840: 6eda 0753 7464 5f64 6576 da13 436f 6e66  n..Std_dev..Conf
+00002850: 6964 656e 6365 5f69 6e74 6572 7661 6cda  idence_interval.
+00002860: 064d 6564 6961 6eda 074d 696e 696d 756d  .Median..Minimum
+00002870: da07 4d61 7869 6d75 6dda 0c50 6172 7469  ..Maximum..Parti
+00002880: 6369 7061 6e74 73da 0853 6573 7369 6f6e  cipants..Session
+00002890: 7329 0a5a 0c56 6f78 656c 5f61 6d6f 756e  s).Z.Voxel_amoun
+000028a0: 74da 1645 7863 6c75 6465 645f 766f 7865  t..Excluded_voxe
+000028b0: 6c73 5f61 6d6f 756e 745a 0e41 7665 7261  ls_amountZ.Avera
+000028c0: 6765 5f76 6f78 656c 7372 cc00 0000 5a12  ge_voxelsr....Z.
+000028d0: 5374 616e 6461 7264 5f64 6576 6961 7469  Standard_deviati
+000028e0: 6f6e 72ce 0000 0072 cf00 0000 72d0 0000  onr....r....r...
+000028f0: 0072 d100 0000 72d3 0000 0029 0272 9500  .r....r....).r..
+00002900: 0000 7294 0000 0063 0100 0000 0000 0000  ..r....c........
+00002910: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
+00002920: 731e 0000 0069 007c 005d 0b7d 0174 006a  s....i.|.].}.t.j
+00002930: 017c 0119 0074 006a 027c 0119 0093 0271  .|...t.j.|.....q
+00002940: 0253 0072 1400 0000 2903 7256 0000 00da  .S.r....).rV....
+00002950: 0f70 6172 616d 6574 6572 5f64 6963 7431  .parameter_dict1
+00002960: da0f 7061 7261 6d65 7465 725f 6469 6374  ..parameter_dict
+00002970: 3229 0272 3700 0000 da01 6972 1400 0000  2).r7.....ir....
+00002980: 7214 0000 0072 1500 0000 da0a 3c64 6963  r....r......<dic
+00002990: 7463 6f6d 703e 8401 0000 730a 0000 0006  tcomp>....s.....
+000029a0: 0002 0108 ff08 0106 ff7a 2555 7469 6c73  .........z%Utils
+000029b0: 2e6c 6f61 645f 636f 6e66 6967 2e3c 6c6f  .load_config.<lo
+000029c0: 6361 6c73 3e2e 3c64 6963 7463 6f6d 703e  cals>.<dictcomp>
+000029d0: 7a10 7465 7374 5f63 6f6e 6669 672e 746f  z.test_config.to
+000029e0: 6d6c 5a0f 7465 7374 5f52 4f49 5f72 6570  mlZ.test_ROI_rep
+000029f0: 6f72 745a 0974 6573 745f 6d61 7073 7a35  ortZ.test_mapsz5
+00002a00: 436f 6e66 6967 2066 696c 6520 6e6f 7420  Config file not 
+00002a10: 696e 2063 6f72 7265 6374 2066 6f72 6d61  in correct forma
+00002a20: 7420 6f72 206d 6973 7369 6e67 2065 6e74  t or missing ent
+00002a30: 7269 6573 2e72 1400 0000 291a 7268 0000  ries.r....).rh..
+00002a40: 00da 0972 6561 646c 696e 6573 da04 746f  ...readlines..to
+00002a50: 6d6c da05 6c6f 6164 7372 c800 0000 7206  ml..loadsr....r.
+00002a60: 0000 0072 5600 0000 7234 0000 0072 3500  ...rV...r4...r5.
+00002a70: 0000 728f 0000 00da 1173 7461 7469 7374  ..r......statist
+00002a80: 6963 5f6f 7074 696f 6e73 728d 0000 0072  ic_optionsr....r
+00002a90: 8e00 0000 72d5 0000 0072 a700 0000 7208  ....r....r....r.
+00002aa0: 0000 00da 1463 6c65 616e 5f63 6f6e 6669  .....clean_confi
+00002ab0: 675f 6f70 7469 6f6e 73da 0e62 7261 696e  g_options..brain
+00002ac0: 5f66 696c 655f 6c6f 6372 ad00 0000 da0d  _file_locr......
+00002ad0: 6f75 7470 7574 5f66 6f6c 6465 725a 126f  output_folderZ.o
+00002ae0: 7574 7075 745f 666f 6c64 6572 5f6e 616d  utput_folder_nam
+00002af0: 65da 0f73 7461 745f 6d61 705f 666f 6c64  e..stat_map_fold
+00002b00: 6572 da07 6465 636f 6465 72da 0f54 6f6d  er..decoder..Tom
+00002b10: 6c44 6563 6f64 6545 7272 6f72 da0e 4174  lDecodeError..At
+00002b20: 7472 6962 7574 6545 7272 6f72 7297 0000  tributeErrorr...
+00002b30: 0029 08da 0363 6c73 726b 0000 00da 0866  .)...clsrk.....f
+00002b40: 696c 656e 616d 65da 0473 6176 6572 3500  ilename..saver5.
+00002b50: 0000 da08 746f 6d6c 6669 6c65 da05 7061  ....tomlfile..pa
+00002b60: 7273 6572 a400 0000 7214 0000 0072 1400  rser....r....r..
+00002b70: 0000 7215 0000 00da 0b6c 6f61 645f 636f  ..r......load_co
+00002b80: 6e66 6967 5a01 0000 733c 0000 0016 0202  nfigZ...s<......
+00002b90: 0108 0110 0108 020c 0108 0102 8004 020e  ................
+00002ba0: 0314 0206 0206 0c08 f306 190c 0108 ff0a  ................
+00002bb0: 0308 0206 0206 0106 0106 0106 0104 0210  ................
+00002bc0: cb14 3708 0102 ff14 c97a 1155 7469 6c73  ..7......z.Utils
+00002bd0: 2e6c 6f61 645f 636f 6e66 6967 6301 0000  .load_configc...
+00002be0: 0000 0000 0000 0000 0003 0000 0007 0000  ................
+00002bf0: 0043 0000 0073 6e00 0000 6700 6401 a201  .C...sn...g.d...
+00002c00: 7d01 7400 7c00 6a01 8301 7402 7501 7212  }.t.|.j...t.u.r.
+00002c10: 7c01 a003 7c00 6a01 a101 7c00 5f01 6700  |...|.j...|._.g.
+00002c20: 6402 a201 7d02 7400 7c00 6a04 8301 7402  d...}.t.|.j...t.
+00002c30: 7501 7235 6403 7405 6404 7406 a007 6405  u.r5d.t.d.t...d.
+00002c40: 7c00 6a04 a102 6406 1900 9b00 9d02 8301  |.j...d.........
+00002c50: 1800 7c00 5f08 7c02 a003 7c00 6a04 a101  ..|._.|...|.j...
+00002c60: 7c00 5f04 7c00 5300 2907 4e29 0d7a 1343  |._.|.S.).N).z.C
+00002c70: 6572 6562 656c 6c75 6d2d 4d4e 4966 6c69  erebellum-MNIfli
+00002c80: 7274 7a13 4365 7265 6265 6c6c 756d 2d4d  rtz.Cerebellum-M
+00002c90: 4e49 666e 6972 747a 1248 6172 7661 7264  NIfnirtz.Harvard
+00002ca0: 4f78 666f 7264 2d63 6f72 747a 1148 6172  Oxford-cortz.Har
+00002cb0: 7661 7264 4f78 666f 7264 2d73 7562 7a0f  vardOxford-subz.
+00002cc0: 4a48 552d 4943 424d 2d6c 6162 656c 737a  JHU-ICBM-labelsz
+00002cd0: 0f4a 4855 2d49 4342 4d2d 7472 6163 7473  .JHU-ICBM-tracts
+00002ce0: 5a07 6a75 656c 6963 68da 034d 4e49 7a0c  Z.juelich..MNIz.
+00002cf0: 534d 4154 542d 6c61 6265 6c73 da03 5354  SMATT-labels..ST
+00002d00: 4e7a 1373 7472 6961 7475 6d2d 7374 7275  Nz.striatum-stru
+00002d10: 6374 7572 616c 7a10 5461 6c61 6972 6163  cturalz.Talairac
+00002d20: 682d 6c61 6265 6c73 da08 5468 616c 616d  h-labels..Thalam
+00002d30: 7573 2906 7a09 3830 252c 2031 2e32 387a  us).z.80%, 1.28z
+00002d40: 0938 3525 2c20 312e 3434 7a09 3930 252c  .85%, 1.44z.90%,
+00002d50: 2031 2e36 347a 0939 3525 2c20 312e 3936   1.64z.95%, 1.96
+00002d60: 7a09 3938 252c 2032 2e33 337a 0939 3925  z.98%, 2.33z.99%
+00002d70: 2c20 322e 3538 721e 0000 007a 0230 2e72  , 2.58r....z.0.r
+00002d80: 2200 0000 7201 0000 0029 0972 1f00 0000  "...r....).r....
+00002d90: da0c 6174 6c61 735f 6e75 6d62 6572 7291  ..atlas_numberr.
+00002da0: 0000 0072 4a00 0000 da11 636f 6e66 5f6c  ...rJ.....conf_l
+00002db0: 6576 656c 5f6e 756d 6265 72da 0566 6c6f  evel_number..flo
+00002dc0: 6174 da02 7265 728f 0000 00da 0f62 6f6f  at..rer......boo
+00002dd0: 7473 7472 6170 5f61 6c70 6861 2903 7256  tstrap_alpha).rV
+00002de0: 0000 00da 0d61 746c 6173 5f6f 7074 696f  .....atlas_optio
+00002df0: 6e73 5a12 636f 6e66 5f6c 6576 656c 5f6f  nsZ.conf_level_o
+00002e00: 7074 696f 6e73 7214 0000 0072 1400 0000  ptionsr....r....
+00002e10: 7215 0000 0072 dd00 0000 9601 0000 7310  r....r........s.
+00002e20: 0000 0008 020e 050e 0108 020e 0222 010e  ............."..
+00002e30: 0104 027a 1a55 7469 6c73 2e63 6c65 616e  ...z.Utils.clean
+00002e40: 5f63 6f6e 6669 675f 6f70 7469 6f6e 7363  _config_optionsc
+00002e50: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+00002e60: 0300 0000 4300 0000 7320 0000 0074 00a0  ....C...s ...t..
+00002e70: 017c 00a1 017d 017c 016a 027d 027c 01a0  .|...}.|.j.}.|..
+00002e80: 03a1 007d 017c 017c 0266 0253 0072 4100  ...}.|.|.f.S.rA.
+00002e90: 0000 2904 da03 6e69 62da 046c 6f61 64da  ..)...nib..load.
+00002ea0: 0668 6561 6465 72da 0967 6574 5f66 6461  .header..get_fda
+00002eb0: 7461 2903 da09 6669 6c65 5f70 6174 68da  ta)...file_path.
+00002ec0: 0464 6174 6172 f500 0000 7214 0000 0072  .datar....r....r
+00002ed0: 1400 0000 7215 0000 00da 0a6c 6f61 645f  ....r......load_
+00002ee0: 6272 6169 6ea8 0100 0073 0800 0000 0a02  brain....s......
+00002ef0: 0602 0801 0802 7a10 5574 696c 732e 6c6f  ......z.Utils.lo
+00002f00: 6164 5f62 7261 696e 6301 0000 0000 0000  ad_brainc.......
+00002f10: 0000 0000 0003 0000 0005 0000 0043 0000  .............C..
+00002f20: 0073 2200 0000 6700 6401 a201 7d01 7c01  .s"...g.d...}.|.
+00002f30: 4400 5d08 7d02 7c00 a000 7c02 6402 a102  D.].}.|...|.d...
+00002f40: 7d00 7106 7c00 5300 2903 4e29 047a 072e  }.q.|.S.).N).z..
+00002f50: 6e69 692e 677a 7a04 2e6e 6969 7a04 2e68  nii.gzz..niiz..h
+00002f60: 6472 7a05 2e6a 736f 6e72 2300 0000 2901  drz..jsonr#...).
+00002f70: 722a 0000 0029 0372 3500 0000 723d 0000  r*...).r5...r=..
+00002f80: 0072 3f00 0000 7214 0000 0072 1400 0000  .r?...r....r....
+00002f90: 7215 0000 00da 0973 7472 6970 5f65 7874  r......strip_ext
+00002fa0: b101 0000 7308 0000 0008 0208 020e 0104  ....s...........
+00002fb0: 027a 0f55 7469 6c73 2e73 7472 6970 5f65  .z.Utils.strip_e
+00002fc0: 7874 6301 0000 0000 0000 0000 0000 0003  xtc.............
+00002fd0: 0000 0004 0000 0043 0000 0073 5c00 0000  .......C...s\...
+00002fe0: 6401 6402 8400 7400 7c00 9b00 6403 9d02  d.d...t.|...d...
+00002ff0: 8301 4400 8301 7d01 6404 6402 8400 7c01  ..D...}.d.d...|.
+00003000: 4400 8301 7d02 7401 7c01 8301 6405 6b02  D...}.t.|...d.k.
+00003010: 721d 7402 6406 8301 8201 7403 6a04 722a  r.t.d.....t.j.r*
+00003020: 7405 6407 7401 7c01 8301 9b00 6408 9d03  t.d.t.|.....d...
+00003030: 8301 0100 7c01 7c02 6602 5300 2909 4e63  ....|.|.f.S.).Nc
+00003040: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00003050: 0600 0000 5300 0000 731c 0000 0067 007c  ....S...s....g.|
+00003060: 005d 0a7d 0174 00a0 0164 007c 01a1 0272  .].}.t...d.|...r
+00003070: 027c 0191 0271 0253 0029 017a 0b73 7562  .|...q.S.).z.sub
+00003080: 2d5b 302d 395d 2b24 2902 72f0 0000 00da  -[0-9]+$).r.....
+00003090: 0673 6561 7263 6829 0272 3700 0000 da05  .search).r7.....
+000030a0: 6469 7265 6372 1400 0000 7214 0000 0072  direcr....r....r
+000030b0: 1500 0000 7239 0000 00bd 0100 0073 0200  ....r9.......s..
+000030c0: 0000 1c00 7a2f 5574 696c 732e 6669 6e64  ....z/Utils.find
+000030d0: 5f70 6172 7469 6369 7061 6e74 5f64 6972  _participant_dir
+000030e0: 732e 3c6c 6f63 616c 733e 2e3c 6c69 7374  s.<locals>.<list
+000030f0: 636f 6d70 3e7a 022f 2a63 0100 0000 0000  comp>z./*c......
+00003100: 0000 0000 0000 0200 0000 0500 0000 5300  ..............S.
+00003110: 0000 731a 0000 0067 007c 005d 097d 017c  ..s....g.|.].}.|
+00003120: 01a0 0064 00a1 0164 0119 0091 0271 0253  ...d...d.....q.S
+00003130: 0029 0272 6300 0000 7267 0000 0029 0172  .).rc...rg...).r
+00003140: 8f00 0000 2902 7237 0000 00da 0b70 6172  ....).r7.....par
+00003150: 7469 6369 7061 6e74 7214 0000 0072 1400  ticipantr....r..
+00003160: 0000 7215 0000 0072 3900 0000 be01 0000  ..r....r9.......
+00003170: 7302 0000 001a 0072 0100 0000 7a9e 5061  s......r....z.Pa
+00003180: 7274 6963 6970 616e 7420 6469 7265 6374  rticipant direct
+00003190: 6f72 6965 7320 6e6f 7420 666f 756e 642e  ories not found.
+000031a0: 0a4d 616b 6520 7375 7265 2070 6172 7469  .Make sure parti
+000031b0: 6369 7061 6e74 2064 6972 6563 746f 7269  cipant directori
+000031c0: 6573 2061 7265 206c 6162 656c 6c65 6420  es are labelled 
+000031d0: 652e 672e 2073 7562 2d30 3120 616e 6420  e.g. sub-01 and 
+000031e0: 7468 6520 7365 6c65 6374 6564 2064 6972  the selected dir
+000031f0: 6563 746f 7279 2063 6f6e 7461 696e 7320  ectory contains 
+00003200: 616c 6c20 7061 7274 6963 6970 616e 7420  all participant 
+00003210: 6469 7265 6374 6f72 6965 732e 7a06 466f  directories.z.Fo
+00003220: 756e 6420 7a15 2070 6172 7469 6369 7061  und z. participa
+00003230: 6e74 2066 6f6c 6465 7273 2e29 0672 0200  nt folders.).r..
+00003240: 0000 728e 0000 0072 5400 0000 7256 0000  ..r....rT...rV..
+00003250: 0072 5700 0000 7258 0000 0029 0372 3c00  .rW...rX...).r<.
+00003260: 0000 5a11 7061 7274 6963 6970 616e 745f  ..Z.participant_
+00003270: 7061 7468 73da 1170 6172 7469 6369 7061  paths..participa
+00003280: 6e74 5f6e 616d 6573 7214 0000 0072 1400  nt_namesr....r..
+00003290: 0000 7215 0000 00da 1566 696e 645f 7061  ..r......find_pa
+000032a0: 7274 6963 6970 616e 745f 6469 7273 ba01  rticipant_dirs..
+000032b0: 0000 730e 0000 0018 030e 010c 0208 0106  ..s.............
+000032c0: 0314 0108 027a 1b55 7469 6c73 2e66 696e  .....z.Utils.fin
+000032d0: 645f 7061 7274 6963 6970 616e 745f 6469  d_participant_di
+000032e0: 7273 6301 0000 0000 0000 0000 0000 0004  rsc.............
+000032f0: 0000 0008 0000 0043 0000 0073 a400 0000  .......C...s....
+00003300: 7c00 6100 6401 7d01 6402 7d02 7401 6403  |.a.d.}.d.}.t.d.
+00003310: 7c00 9b00 6404 7402 7c01 8301 9b00 6405  |...d.t.|.....d.
+00003320: 7402 7c02 8301 9b00 6406 9d07 8301 0100  t.|.....d.......
+00003330: 7403 6a04 6400 6407 8502 1900 7c01 7c02  t.j.d.d.....|.|.
+00003340: 6602 6b03 7250 7402 7403 6a04 6408 1900  f.k.rPt.t.j.d...
+00003350: 8301 9b00 6405 7402 7403 6a04 6409 1900  ....d.t.t.j.d...
+00003360: 8301 9b00 6405 7402 7403 6a04 6407 1900  ....d.t.t.j.d...
+00003370: 8301 9b00 9d05 7d03 7401 640a 7c03 9b00  ......}.t.d.|...
+00003380: 640b 7402 7c01 8301 9b00 6405 7402 7c02  d.t.|.....d.t.|.
+00003390: 8301 9b00 640c 9d07 8301 0100 6400 5300  ....d.......d.S.
+000033a0: 6400 5300 290d 4ee9 0300 0000 e90a 0000  d.S.).N.........
+000033b0: 007a 060a 6652 4154 207a 2520 6973 2064  .z..fRAT z% is d
+000033c0: 6576 656c 6f70 6564 2061 6e64 2074 6573  eveloped and tes
+000033d0: 7465 6420 7769 7468 2050 7974 686f 6e20  ted with Python 
+000033e0: 7233 0000 007a 022e 0a72 b600 0000 7201  r3...z...r....r.
+000033f0: 0000 0072 1e00 0000 7a15 494e 464f 3a20  ...r....z.INFO: 
+00003400: 5079 7468 6f6e 2076 6572 7369 6f6e 207a  Python version z
+00003410: 2b20 6973 2075 6e74 6573 7465 642e 2043  + is untested. C
+00003420: 6f6e 7369 6465 7220 6368 616e 6769 6e67  onsider changing
+00003430: 2074 6f20 7665 7273 696f 6e20 7a22 2069   to version z" i
+00003440: 6620 7468 6572 6520 6172 6520 6572 726f  f there are erro
+00003450: 7273 2072 756e 6e69 6e67 2066 5241 542e  rs running fRAT.
+00003460: 2905 7269 0000 0072 5800 0000 725d 0000  ).ri...rX...r]..
+00003470: 00da 0373 7973 da0c 7665 7273 696f 6e5f  ...sys..version_
+00003480: 696e 666f 2904 5a0c 6672 6174 5f76 6572  info).Z.frat_ver
+00003490: 7369 6f6e 5a0c 6578 7065 6374 5f6d 616a  sionZ.expect_maj
+000034a0: 6f72 5a0c 6578 7065 6374 5f6d 696e 6f72  orZ.expect_minor
+000034b0: 5a0f 6375 7272 656e 745f 7665 7273 696f  Z.current_versio
+000034c0: 6e72 1400 0000 7214 0000 0072 1500 0000  nr....r....r....
+000034d0: da0c 6368 6563 6b76 6572 7369 6f6e c901  ..checkversion..
+000034e0: 0000 7318 0000 0004 0304 0304 0124 0216  ..s..........$..
+000034f0: 0132 010a 0106 0104 ff06 010e ff04 fe7a  .2.............z
+00003500: 1255 7469 6c73 2e63 6865 636b 7665 7273  .Utils.checkvers
+00003510: 696f 6e63 0200 0000 0000 0000 0000 0000  ionc............
+00003520: 0400 0000 0800 0000 4300 0000 73ae 0000  ........C...s...
+00003530: 007c 0064 016b 0272 097c 016a 0072 0964  .|.d.k.r.|.j.r.d
+00003540: 0053 007c 016a 0172 2364 0264 036c 026d  .S.|.j.r#d.d.l.m
+00003550: 037d 0201 0074 04a0 05a1 009b 0064 047c  .}...t.......d.|
+00003560: 026a 069b 009d 037d 0374 04a0 077c 03a1  .j.....}.t...|..
+00003570: 0101 007c 0353 007c 016a 0864 0576 0072  ...|.S.|.j.d.v.r
+00003580: 3574 0964 0683 0101 0074 0a6a 0b64 0764  5t.d.....t.j.d.d
+00003590: 0864 098d 027d 037c 0353 007c 016a 087d  .d...}.|.S.|.j.}
+000035a0: 037a 0774 04a0 077c 03a1 0101 0057 006e  .z.t...|.....W.n
+000035b0: 0b04 0074 0c79 4a01 0001 0001 0074 0c64  ...t.yJ......t.d
+000035c0: 0a83 0182 0177 007c 016a 0d72 5574 0964  .....w.|.j.rUt.d
+000035d0: 0b7c 039b 009d 0283 0101 007c 0353 0029  .|.........|.S.)
+000035e0: 0c4e da0a 5374 6174 6973 7469 6373 721e  .N..Statisticsr.
+000035f0: 0000 0029 01da 1145 6e76 6972 6f6e 6d65  ...)...Environme
+00003600: 6e74 5f53 6574 7570 7263 0000 0029 0272  nt_Setuprc...).r
+00003610: 2300 0000 fa01 207a 2853 656c 6563 7420  #..... z(Select 
+00003620: 7468 6520 6469 7265 6374 6f72 7920 6f75  the directory ou
+00003630: 7470 7574 2062 7920 7468 6520 6652 4154  tput by the fRAT
+00003640: 2e7a 2753 656c 6563 7420 7468 6520 6469  .z'Select the di
+00003650: 7265 6374 6f72 7920 6f75 7470 7574 2062  rectory output b
+00003660: 7920 7468 6520 6652 4154 5429 0272 0b00  y the fRATT).r..
+00003670: 0000 7255 0000 007a 4e4f 7574 7075 7420  ..rU...zNOutput 
+00003680: 666f 6c64 6572 206c 6f63 6174 696f 6e20  folder location 
+00003690: 2866 5241 5420 6f75 7470 7574 2066 6f6c  (fRAT output fol
+000036a0: 6465 7220 6c6f 6361 7469 6f6e 2920 6973  der location) is
+000036b0: 206e 6f74 2061 2076 616c 6964 2064 6972   not a valid dir
+000036c0: 6563 746f 7279 2e7a 194f 7574 7075 7420  ectory.z.Output 
+000036d0: 666f 6c64 6572 2073 656c 6563 7469 6f6e  folder selection
+000036e0: 3a20 290e da0c 7275 6e5f 706c 6f74 7469  : )...run_plotti
+000036f0: 6e67 da0c 7275 6e5f 616e 616c 7973 6973  ng..run_analysis
+00003700: da08 616e 616c 7973 6973 7206 0100 0072  ..analysisr....r
+00003710: 3400 0000 72af 0000 00da 0d73 6176 655f  4...r......save_
+00003720: 6c6f 6361 7469 6f6e 7255 0000 005a 1472  locationrU...Z.r
+00003730: 6570 6f72 745f 6f75 7470 7574 5f66 6f6c  eport_output_fol
+00003740: 6465 7272 5800 0000 7208 0000 0072 5a00  derrX...r....rZ.
+00003750: 0000 7254 0000 0072 5700 0000 2904 5a0c  ..rT...rW...).Z.
+00003760: 6375 7272 656e 745f 7374 6570 7256 0000  current_steprV..
+00003770: 0072 0601 0000 5a0e 6a73 6f6e 5f64 6972  .r....Z.json_dir
+00003780: 6563 746f 7279 7214 0000 0072 1400 0000  ectoryr....r....
+00003790: 7215 0000 00da 1963 6864 6972 5f74 6f5f  r......chdir_to_
+000037a0: 6f75 7470 7574 5f64 6972 6563 746f 7279  output_directory
+000037b0: d801 0000 732c 0000 000e 0204 0106 020c  ....s,..........
+000037c0: 0114 010a 0204 120a f008 010e 0104 0e06  ................
+000037d0: f502 020e 010c 0102 0102 0104 ff02 ff06  ................
+000037e0: 040e 0104 027a 1f55 7469 6c73 2e63 6864  .....z.Utils.chd
+000037f0: 6972 5f74 6f5f 6f75 7470 7574 5f64 6972  ir_to_output_dir
+00003800: 6563 746f 7279 2902 7223 0000 0046 2903  ectory).r#...F).
+00003810: 4e72 6100 0000 7262 0000 0029 0346 5446  Nra...rb...).FTF
+00003820: 2901 4629 0172 2300 0000 2902 544e 291f  ).F).r#...).TN).
+00003830: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00003840: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00003850: 6d65 5f5f da0c 7374 6174 6963 6d65 7468  me__..staticmeth
+00003860: 6f64 7216 0000 0072 3200 0000 7240 0000  odr....r2...r@..
+00003870: 0072 4900 0000 7250 0000 0072 5a00 0000  .rI...rP...rZ...
+00003880: 7260 0000 0072 7000 0000 7279 0000 0072  r`...rp...ry...r
+00003890: 7e00 0000 7293 0000 0072 9c00 0000 72ac  ~...r....r....r.
+000038a0: 0000 0072 b300 0000 727c 0000 0072 ba00  ...r....r|...r..
+000038b0: 0000 72bb 0000 0072 c600 0000 72ca 0000  ..r....r....r...
+000038c0: 00da 0b63 6c61 7373 6d65 7468 6f64 72e9  ...classmethodr.
+000038d0: 0000 0072 dd00 0000 72f9 0000 0072 fa00  ...r....r....r..
+000038e0: 0000 72ff 0000 0072 0401 0000 720c 0100  ..r....r....r...
+000038f0: 0072 1400 0000 7214 0000 0072 1400 0000  .r....r....r....
+00003900: 7215 0000 0072 0800 0000 1700 0000 736a  r....r........sj
+00003910: 0000 0008 0002 010a 0102 0f0a 0102 2a0a  ..............*.
+00003920: 0102 0d0a 0102 070a 0102 030c 0102 130a  ................
+00003930: 0102 060c 0102 180c 0102 140c 0102 080a  ................
+00003940: 0102 2e0a 0102 140a 0102 180c 0102 160a  ................
+00003950: 0102 060a 0102 030a 0102 030c 0102 0d0a  ................
+00003960: 0102 090c 0102 3b0a 0102 110a 0102 080a  ......;.........
+00003970: 0102 080a 0102 0e0a 0102 0e0e 0172 0800  .............r..
+00003980: 0000 2919 7225 0000 0072 0c00 0000 7234  ..).r%...r....r4
+00003990: 0000 0072 f000 0000 7272 0000 0072 0201  ...r....rr...r..
+000039a0: 0000 7202 0000 00da 0770 6174 686c 6962  ..r......pathlib
+000039b0: 7203 0000 00da 0774 6b69 6e74 6572 7204  r......tkinterr.
+000039c0: 0000 0072 0500 0000 da05 7479 7065 7372  ...r......typesr
+000039d0: 0600 0000 da0c 6d75 6c74 6970 726f 6365  ......multiproce
+000039e0: 7373 72bf 0000 00da 076e 6962 6162 656c  ssr......nibabel
+000039f0: 72f3 0000 00da 0670 616e 6461 7372 4c00  r......pandasrL.
+00003a00: 0000 72da 0000 00da 1c66 5241 542e 7574  ..r......fRAT.ut
+00003a10: 696c 732e 6652 4154 5f63 6f6e 6669 675f  ils.fRAT_config_
+00003a20: 7365 7475 7072 5600 0000 7269 0000 0072  setuprV...ri...r
+00003a30: 0800 0000 7214 0000 0072 1400 0000 7214  ....r....r....r.
+00003a40: 0000 0072 1500 0000 da08 3c6d 6f64 756c  ...r......<modul
+00003a50: 653e 0100 0000 7324 0000 0008 0008 0108  e>....s$........
+00003a60: 0108 0108 0108 010c 010c 0110 010c 0108  ................
+00003a70: 0208 0108 0108 0108 0204 0204 0112 03    ...............
```

### Comparing `frat_brain-1.3.5/fRAT/utils/analysis.py` & `frat_brain-1.3.6/fRAT/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/utils/bootstrap.css` & `frat_brain-1.3.6/fRAT/utils/bootstrap.css`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/utils/dash_report.py` & `frat_brain-1.3.6/fRAT/utils/dash_report.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/utils/directory_comparison.py` & `frat_brain-1.3.6/fRAT/utils/directory_comparison.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/utils/fRAT_config_setup.py` & `frat_brain-1.3.6/fRAT/utils/fRAT_config_setup.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/utils/figures.py` & `frat_brain-1.3.6/fRAT/utils/figures.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,16 +334,16 @@
                                   draw_cross=False, annotate=False, colorbar=True, display_mode='xz',
                                   vmin=vmin, vmax=vmax,
                                   cut_coords=(cls.config.brain_x_coord, cls.config.brain_z_coord),
                                   cmap='inferno')
         plot.savefig(png_path, dpi=cls.config.plot_dpi)
         plot.close()
 
-        im = Image.open(png_path)
-        width, height = im.size
+        with Image.open(png_path) as im:
+            width, height = im.size
 
         return png_path, indiv_brain_imgs, (width, height)
 
     @classmethod
     def table_setup(cls, df):
         unique_params = []
         cell_nums = []
```

### Comparing `frat_brain-1.3.5/fRAT/utils/html_report.py` & `frat_brain-1.3.6/fRAT/utils/html_report.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/utils/printResults.py` & `frat_brain-1.3.6/fRAT/utils/printResults.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/utils/statistics.py` & `frat_brain-1.3.6/fRAT/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/utils/statmap.py` & `frat_brain-1.3.6/fRAT/utils/statmap.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/utils/statmap_config_setup.py` & `frat_brain-1.3.6/fRAT/utils/statmap_config_setup.py`

 * *Files identical despite different names*

### Comparing `frat_brain-1.3.5/fRAT/utils/utils.py` & `frat_brain-1.3.6/fRAT/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,15 +320,15 @@
         return argv[0](*argv[1:])
 
     @staticmethod
     def start_processing_pool(restart=False):
         if config.max_core_usage == 'max':
             workers = mp.cpu_count()
         else:
-            workers = config.max_core_usage
+            workers = int(config.max_core_usage)
 
         ctx = mp.get_context('forkserver')  # This stops segmentation fault for MacOS
 
         if config.verbose and not restart:
             print(f"\nStarting processing pool using {workers} cores.")
 
         return ctx.Pool(processes=workers)
```

### Comparing `frat_brain-1.3.5/pyproject.toml` & `frat_brain-1.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "frat-brain"
-version = "1.3.5"
+version = "1.3.6"
 description = "Application for ROI fMRI data analysis."
 authors = ["Elliot Howley <elliohow@hotmail.com>"]
 readme = "README.md"
 homepage = "https://fmri-roi-analysis-tool.readthedocs.io/en/latest/"
 repository = "https://github.com/elliohow/fMRI_ROI_Analysis_Tool"
 packages = [{include = "fRAT"}]
```

### Comparing `frat_brain-1.3.5/setup.py` & `frat_brain-1.3.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,17 +108,17 @@
  'zope-interface==5.2.0']
 
 entry_points = \
 {'console_scripts': ['fRAT = fRAT.__main__:start_gui']}
 
 setup_kwargs = {
     'name': 'frat-brain',
-    'version': '1.3.5',
+    'version': '1.3.6',
     'description': 'Application for ROI fMRI data analysis.',
-    'long_description': '<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/fRAT.gif?raw=true" width=500>\n\n# fRAT - fMRI ROI Analysis Tool\n[![status](https://joss.theoj.org/papers/cc9c0cb3b12abaf30c8381728d3229d7/status.svg)](https://joss.theoj.org/papers/cc9c0cb3b12abaf30c8381728d3229d7)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) \n[![GitHub license](https://img.shields.io/hexpm/l/plug?style=flat-square)](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/LICENSE)\n[![Github release (latest by date)](https://img.shields.io/github/v/release/elliohow/fmri_roi_analysis_tool?style=flat-square)](https://github.com/elliohow/fmri_roi_analysis_tool/releases/latest)\n[![Github issues](https://img.shields.io/github/issues/elliohow/fmri_roi_analysis_tool?style=flat-square)](https://github.com/elliohow/fmri_roi_analysis_tool/issues)\n[![Documentation](https://img.shields.io/readthedocs/fmri-roi-analysis-tool)](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/)\n\nfRAT is an open-source python-based GUI application used to simplify the processing and analysis of fMRI data by\nconverting voxelwise maps into ROI-wise maps. An installation of FSL is required in order to use fRAT.\n\n> fRAT is written using **Python** for **MacOS, Linux and WSL2**.\n\nDocumentation:\n\n[Home page](https://fmri-roi-analysis-tool.readthedocs.io)\n\n[Installation instructions](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/installation.html)\n\n[ROI analysis tutorial](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/tutorials/Basic-ROI-analysis.html)\n\n## Reporting bugs\n\nTo report a bug, please go to [fRAT\'s Issues](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/issues/new).\n\nFor other questions, issues or discussion please go to [fRAT\'s Discussions](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/discussions).\n\n## Contributing with development\n\nThe [Fork & Pull Request Workflow](https://docs.github.com/en/get-started/quickstart/contributing-to-projects) is used for contributing. Below is a summary of the necessary steps for this workflow:\n\n1. Fork this repository.\n2. Clone the repository at your machine.\n3. Add your changes in a branch named after the feature (`lower-case-with-hyphens`).\n4. Make a pull request to `fRAT`, targeting the `master` branch.\n\n## Images\n<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/GUI.png?raw=true" title="Example of the fRAT GUI" width=700>\n\n<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/ROI_example.png?raw=true" \n  title="A region of interest map created using fRAT, showing the mean temporal Signal-to-Noise for each region. Data is displayed in MNI152 standard space and combines data from multiple subjects." \nwidth=700>\n\n<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/HTML_report.png?raw=true" title="Example of a HTML report output by fRAT" width=600>\n\n## Versioning\nWe use [Semantic versioning](http://semver.org/) for versioning. For the versions available, see the\n[tag list](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/tags) for this project.\n\n## Licensing\nThis project uses the Apache 2.0 license. For the text version of the license see\n[here](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/LICENSE). \nPrior to version 1.0.0, this project used an MIT license.\n',
+    'long_description': '<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/fRAT.gif?raw=true" width=500>\n\n# fRAT - fMRI ROI Analysis Tool\n[![status](https://joss.theoj.org/papers/cc9c0cb3b12abaf30c8381728d3229d7/status.svg)](https://joss.theoj.org/papers/cc9c0cb3b12abaf30c8381728d3229d7)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com) \n[![GitHub license](https://img.shields.io/hexpm/l/plug?style=flat-square)](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/LICENSE)\n[![Github release (latest by date)](https://img.shields.io/github/v/release/elliohow/fmri_roi_analysis_tool?style=flat-square)](https://github.com/elliohow/fmri_roi_analysis_tool/releases/latest)\n[![Github issues](https://img.shields.io/github/issues/elliohow/fmri_roi_analysis_tool?style=flat-square)](https://github.com/elliohow/fmri_roi_analysis_tool/issues)\n[![Documentation](https://img.shields.io/readthedocs/fmri-roi-analysis-tool)](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/)\n\nfRAT is an open-source python-based GUI application used to simplify the processing and analysis of fMRI data by\nconverting voxelwise maps into ROI-wise maps. An installation of FSL is required in order to use fRAT.\n\n> fRAT is written using **Python** for **MacOS, Linux and WSL2**.\n\nDocumentation:\n\n[Home page](https://fmri-roi-analysis-tool.readthedocs.io)\n\n[Installation instructions](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/installation.html)\n\n[ROI analysis tutorial](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/tutorials/Basic-ROI-analysis.html)\n\n## Reporting bugs\n\nTo report a bug or suggest a new feature, please go to [fRAT\'s Issues](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/issues/new/choose).\n\nFor other questions, issues or discussion please go to [fRAT\'s Discussions](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/discussions).\n\n## Contributing to the project\n\nIf you\'d like to contribute to the project please read our [contributing guidelines](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/CONTRIBUTING.md). Please also read through our [code of conduct](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/CODE_OF_CONDUCT.md).\n\n## Versioning\nWe use [Semantic versioning](http://semver.org/) for versioning. For the versions available, see the\n[tag list](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/tags) for this project.\n\n## Licensing\nThis project uses the Apache 2.0 license. For the text version of the license see\n[here](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/LICENSE). \nPrior to version 1.0.0, this project used an MIT license.\n\n## Images\n<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/GUI.png?raw=true" title="Example of the fRAT GUI" width=700>\n\n<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/HTML_report.png?raw=true" title="Example of a HTML report output by fRAT" width=600>\n',
     'author': 'Elliot Howley',
     'author_email': 'elliohow@hotmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://fmri-roi-analysis-tool.readthedocs.io/en/latest/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `frat_brain-1.3.5/PKG-INFO` & `frat_brain-1.3.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frat-brain
-Version: 1.3.5
+Version: 1.3.6
 Summary: Application for ROI fMRI data analysis.
 Home-page: https://fmri-roi-analysis-tool.readthedocs.io/en/latest/
 Author: Elliot Howley
 Author-email: elliohow@hotmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -126,38 +126,29 @@
 
 [Installation instructions](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/installation.html)
 
 [ROI analysis tutorial](https://fmri-roi-analysis-tool.readthedocs.io/en/latest/tutorials/Basic-ROI-analysis.html)
 
 ## Reporting bugs
 
-To report a bug, please go to [fRAT's Issues](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/issues/new).
+To report a bug or suggest a new feature, please go to [fRAT's Issues](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/issues/new/choose).
 
 For other questions, issues or discussion please go to [fRAT's Discussions](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/discussions).
 
-## Contributing with development
+## Contributing to the project
 
-The [Fork & Pull Request Workflow](https://docs.github.com/en/get-started/quickstart/contributing-to-projects) is used for contributing. Below is a summary of the necessary steps for this workflow:
-
-1. Fork this repository.
-2. Clone the repository at your machine.
-3. Add your changes in a branch named after the feature (`lower-case-with-hyphens`).
-4. Make a pull request to `fRAT`, targeting the `master` branch.
-
-## Images
-<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/GUI.png?raw=true" title="Example of the fRAT GUI" width=700>
-
-<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/ROI_example.png?raw=true" 
-  title="A region of interest map created using fRAT, showing the mean temporal Signal-to-Noise for each region. Data is displayed in MNI152 standard space and combines data from multiple subjects." 
-width=700>
-
-<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/HTML_report.png?raw=true" title="Example of a HTML report output by fRAT" width=600>
+If you'd like to contribute to the project please read our [contributing guidelines](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/CONTRIBUTING.md). Please also read through our [code of conduct](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/CODE_OF_CONDUCT.md).
 
 ## Versioning
 We use [Semantic versioning](http://semver.org/) for versioning. For the versions available, see the
 [tag list](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/tags) for this project.
 
 ## Licensing
 This project uses the Apache 2.0 license. For the text version of the license see
 [here](https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/LICENSE). 
 Prior to version 1.0.0, this project used an MIT license.
 
+## Images
+<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/GUI.png?raw=true" title="Example of the fRAT GUI" width=700>
+
+<img src="https://github.com/elliohow/fMRI_ROI_Analysis_Tool/blob/master/docs/images/HTML_report.png?raw=true" title="Example of a HTML report output by fRAT" width=600>
+
```

