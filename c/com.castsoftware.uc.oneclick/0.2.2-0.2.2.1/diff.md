# Comparing `tmp/com.castsoftware.uc.oneclick-0.2.2.tar.gz` & `tmp/com.castsoftware.uc.oneclick-0.2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.castsoftware.uc.oneclick-0.2.2.tar", last modified: Thu Apr  6 16:41:00 2023, max compression
+gzip compressed data, was "com.castsoftware.uc.oneclick-0.2.2.1.tar", last modified: Thu Apr 20 16:06:03 2023, max compression
```

## Comparing `com.castsoftware.uc.oneclick-0.2.2.tar` & `com.castsoftware.uc.oneclick-0.2.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 16:41:00.293872 com.castsoftware.uc.oneclick-0.2.2/
--rw-rw-rw-   0        0        0      515 2023-04-06 16:41:00.284065 com.castsoftware.uc.oneclick-0.2.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-06 16:40:59.992482 com.castsoftware.uc.oneclick-0.2.2/com.castsoftware.uc.oneclick.egg-info/
--rw-rw-rw-   0        0        0      515 2023-04-06 16:40:59.000000 com.castsoftware.uc.oneclick-0.2.2/com.castsoftware.uc.oneclick.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      818 2023-04-06 16:40:59.000000 com.castsoftware.uc.oneclick-0.2.2/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 16:40:59.000000 com.castsoftware.uc.oneclick-0.2.2/com.castsoftware.uc.oneclick.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      136 2023-04-06 16:40:59.000000 com.castsoftware.uc.oneclick-0.2.2/com.castsoftware.uc.oneclick.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-06 16:40:59.000000 com.castsoftware.uc.oneclick-0.2.2/com.castsoftware.uc.oneclick.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-06 16:41:00.120456 com.castsoftware.uc.oneclick-0.2.2/oneclick/
--rw-rw-rw-   0        0        0        2 2023-03-27 13:09:22.000000 com.castsoftware.uc.oneclick-0.2.2/oneclick/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 16:41:00.175931 com.castsoftware.uc.oneclick-0.2.2/oneclick/analysis/
--rw-rw-rw-   0        0        0        0 2023-03-27 13:09:22.000000 com.castsoftware.uc.oneclick-0.2.2/oneclick/analysis/__init__.py
--rw-rw-rw-   0        0        0     2649 2023-04-06 16:17:36.000000 com.castsoftware.uc.oneclick-0.2.2/oneclick/analysis/aip_analysis.py
--rw-rw-rw-   0        0        0     1231 2023-03-27 13:09:22.000000 com.castsoftware.uc.oneclick-0.2.2/oneclick/analysis/analysis.py
--rw-rw-rw-   0        0        0     3446 2023-04-06 16:21:03.000000 com.castsoftware.uc.oneclick-0.2.2/oneclick/analysis/highlight_analysis.py
--rw-rw-rw-   0        0        0     4706 2023-03-27 13:09:22.000000 com.castsoftware.uc.oneclick-0.2.2/oneclick/analysis/trackAnalysis.py
--rw-rw-rw-   0        0        0    19538 2023-04-06 16:10:49.000000 com.castsoftware.uc.oneclick-0.2.2/oneclick/config.py
-drwxrwxrwx   0        0        0        0 2023-04-06 16:41:00.269643 com.castsoftware.uc.oneclick-0.2.2/oneclick/discovery/
--rw-rw-rw-   0        0        0        0 2023-03-27 13:09:22.000000 com.castsoftware.uc.oneclick-0.2.2/oneclick/discovery/__init__.py
--rw-rw-rw-   0        0        0     4429 2023-03-29 16:14:00.000000 com.castsoftware.uc.oneclick-0.2.2/oneclick/discovery/cleanup.py
--rw-rw-rw-   0        0        0     6391 2023-03-29 16:14:00.000000 com.castsoftware.uc.oneclick-0.2.2/oneclick/discovery/cloc.py
--rw-rw-rw-   0        0        0     8416 2023-03-29 16:14:00.000000 com.castsoftware.uc.oneclick-0.2.2/oneclick/discovery/discoveryReport.py
--rw-rw-rw-   0        0        0     3436 2023-03-29 16:14:00.000000 com.castsoftware.uc.oneclick-0.2.2/oneclick/discovery/prep.py
--rw-rw-rw-   0        0        0      491 2023-03-29 16:14:00.000000 com.castsoftware.uc.oneclick-0.2.2/oneclick/discovery/sourceValidation.py
--rw-rw-rw-   0        0        0     6023 2023-03-29 16:14:00.000000 com.castsoftware.uc.oneclick-0.2.2/oneclick/discovery/sqlDiscovery.py
--rw-rw-rw-   0        0        0     2251 2023-03-29 16:14:00.000000 com.castsoftware.uc.oneclick-0.2.2/oneclick/discovery/unzip.py
--rw-rw-rw-   0        0        0      305 2023-03-27 13:12:48.000000 com.castsoftware.uc.oneclick-0.2.2/oneclick/exceptions.py
--rw-rw-rw-   0        0        0    11263 2023-03-29 16:14:00.000000 com.castsoftware.uc.oneclick-0.2.2/oneclick/main.py
--rw-rw-rw-   0        0        0     1977 2023-03-28 19:09:20.000000 com.castsoftware.uc.oneclick-0.2.2/oneclick/runArg.py
--rw-rw-rw-   0        0        0     2098 2023-03-27 13:09:22.000000 com.castsoftware.uc.oneclick-0.2.2/oneclick/sendEmail.py
--rw-rw-rw-   0        0        0      705 2023-04-06 16:32:44.000000 com.castsoftware.uc.oneclick-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-06 16:41:00.294876 com.castsoftware.uc.oneclick-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-20 16:06:03.508230 com.castsoftware.uc.oneclick-0.2.2.1/
+-rw-rw-rw-   0        0        0      517 2023-04-20 16:06:03.497327 com.castsoftware.uc.oneclick-0.2.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-20 16:06:03.246193 com.castsoftware.uc.oneclick-0.2.2.1/com.castsoftware.uc.oneclick.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-04-20 16:06:03.000000 com.castsoftware.uc.oneclick-0.2.2.1/com.castsoftware.uc.oneclick.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      818 2023-04-20 16:06:03.000000 com.castsoftware.uc.oneclick-0.2.2.1/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 16:06:03.000000 com.castsoftware.uc.oneclick-0.2.2.1/com.castsoftware.uc.oneclick.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      162 2023-04-20 16:06:03.000000 com.castsoftware.uc.oneclick-0.2.2.1/com.castsoftware.uc.oneclick.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-20 16:06:03.000000 com.castsoftware.uc.oneclick-0.2.2.1/com.castsoftware.uc.oneclick.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-20 16:06:03.348967 com.castsoftware.uc.oneclick-0.2.2.1/oneclick/
+-rw-rw-rw-   0        0        0        2 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.1/oneclick/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:06:03.397307 com.castsoftware.uc.oneclick-0.2.2.1/oneclick/analysis/
+-rw-rw-rw-   0        0        0        0 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.1/oneclick/analysis/__init__.py
+-rw-rw-rw-   0        0        0     2736 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.1/oneclick/analysis/aip_analysis.py
+-rw-rw-rw-   0        0        0     1231 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.1/oneclick/analysis/analysis.py
+-rw-rw-rw-   0        0        0     3454 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.1/oneclick/analysis/highlight_analysis.py
+-rw-rw-rw-   0        0        0     4706 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.1/oneclick/analysis/trackAnalysis.py
+-rw-rw-rw-   0        0        0    19726 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.1/oneclick/config.py
+drwxrwxrwx   0        0        0        0 2023-04-20 16:06:03.480588 com.castsoftware.uc.oneclick-0.2.2.1/oneclick/discovery/
+-rw-rw-rw-   0        0        0        0 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.1/oneclick/discovery/__init__.py
+-rw-rw-rw-   0        0        0     4429 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.1/oneclick/discovery/cleanup.py
+-rw-rw-rw-   0        0        0     7040 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.1/oneclick/discovery/cloc.py
+-rw-rw-rw-   0        0        0     8416 2023-04-20 15:56:31.000000 com.castsoftware.uc.oneclick-0.2.2.1/oneclick/discovery/discoveryReport.py
+-rw-rw-rw-   0        0        0     3472 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.1/oneclick/discovery/prep.py
+-rw-rw-rw-   0        0        0      491 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.1/oneclick/discovery/sourceValidation.py
+-rw-rw-rw-   0        0        0     6803 2023-04-20 15:56:31.000000 com.castsoftware.uc.oneclick-0.2.2.1/oneclick/discovery/sqlDiscovery.py
+-rw-rw-rw-   0        0        0     2251 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.1/oneclick/discovery/unzip.py
+-rw-rw-rw-   0        0        0      305 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.1/oneclick/exceptions.py
+-rw-rw-rw-   0        0        0    11312 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.1/oneclick/main.py
+-rw-rw-rw-   0        0        0     2152 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.1/oneclick/runArg.py
+-rw-rw-rw-   0        0        0     2098 2023-04-20 12:19:52.000000 com.castsoftware.uc.oneclick-0.2.2.1/oneclick/sendEmail.py
+-rw-rw-rw-   0        0        0      737 2023-04-20 15:58:49.000000 com.castsoftware.uc.oneclick-0.2.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-20 16:06:03.508230 com.castsoftware.uc.oneclick-0.2.2.1/setup.cfg
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2/PKG-INFO` & `com.castsoftware.uc.oneclick-0.2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.oneclick
-Version: 0.2.2
+Version: 0.2.2.1
 Summary: Assessment Generator
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2/com.castsoftware.uc.oneclick.egg-info/PKG-INFO` & `com.castsoftware.uc.oneclick-0.2.2.1/com.castsoftware.uc.oneclick.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.oneclick
-Version: 0.2.2
+Version: 0.2.2.1
 Summary: Assessment Generator
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt` & `com.castsoftware.uc.oneclick-0.2.2.1/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2/oneclick/analysis/aip_analysis.py` & `com.castsoftware.uc.oneclick-0.2.2.1/oneclick/analysis/aip_analysis.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,49 +11,51 @@
 
     def __init__(cls, log_level:int):
         super().__init__(cls.__class__.__name__,log_level)
         pass
     
     def run(cls, config:Config):
         if not config.is_console_active:
-            cls._log.warning('Console active flag is set to false, skipping analysis')
-            return -1
+            cls._log.warning('AIP Console configuration is incomplete, analysis will not run')
+            return 0
 
         for appl in config.application:
 
             #has thi spplication already been run?
             aip_status = config.application[appl]['aip']
             if aip_status == '' or aip_status.startswith('Error'):
                 #add a new appication in AIP Console
                 cls._log.info(f'Running analysis for {config.project_name}\{appl}')
 
                 java_home = config.java_home
                 if len(java_home) > 0:
                     java_home = f'{java_home}/bin/'
-                
-                enable_security=''
-                if config.enable_security_assessment:
-                    enable_security='--enable-security-assessment'
 
-                blueprint=''
+                node_name = ""
+                if len(config.console_node) > 0:
+                    node_name=f'--node-name={config.console_node}'
+
+                security_assessment=""
+                if config.enable_security_assessment:
+                    security_assessment='--enable-security-assessment'
+                
+                blueprint=""
                 if config.blueprint:
                     blueprint='--blueprint'
 
                 args = [f'{java_home}java.exe',
                         '-jar',config.console_cli,
                         'add',
                         '-n',appl,
                         '-f', f'AIP/{config.project_name}/{appl}',
                         '-s',config.console_url,
                         '--apikey',config.console_key,
-                        '--verbose' , 'false',
+                        '--verbose',
                         '--auto-create',
-                        '--node-name',config.console_node,
-                        enable_security,
-                        blueprint
+                        node_name, security_assessment, blueprint
                         ]
                 cls._log.debug(dumps(args, indent=2))
 
                 try:
                     process = run_process(args,wait=False)
                 except FileNotFoundError as e:
                     cls._log.error(f'Unable to launch analysis process {e}')
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2/oneclick/analysis/analysis.py` & `com.castsoftware.uc.oneclick-0.2.2.1/oneclick/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2/oneclick/analysis/highlight_analysis.py` & `com.castsoftware.uc.oneclick-0.2.2.1/oneclick/analysis/highlight_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
     def __init__(cls, log_level:int):
         super().__init__(cls.__class__.__name__,log_level)
         pass
 
     def run(cls, config:Config):
         if not config.is_hl_active:
-            cls._log.warning(f'Highlight is not configured, analysis will not run')
-            return -1
+            cls._log.warning('Highlight configuration is incomplete, analysis will not run')
+            return 0
         
         rest = HLRestCall(config.hl_url,config.hl_user,config.hl_password,config.hl_instance)
 
         try:
             process = {}
             for appl in config.application:
                 hl_status = config.application[appl]['hl']
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2/oneclick/analysis/trackAnalysis.py` & `com.castsoftware.uc.oneclick-0.2.2.1/oneclick/analysis/trackAnalysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2/oneclick/config.py` & `com.castsoftware.uc.oneclick-0.2.2.1/oneclick/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,17 @@
 
     def validate_for_run(self):
         if self.cloc_version == '':
             raise InvalidConfiguration('Missing CLOC executable name')
         exec = f'{getcwd()}\\scripts\\{self.cloc_version}'
         if not exists(exec):
             raise InvalidConfiguration(f'CLOC executable not found: {exec}')
+        if not self.is_console_active and not self.is_hl_active:
+            raise InvalidConfiguration('Both Hightlight and AIP configureations are incomplete, at least one must be')
+
 
     def check_default(self,arg_value,cfg_value,default_value) -> bool:
         rtn =  False
         if arg_value is not None: 
             if (cfg_value is None or cfg_value=='') or arg_value != default_value:
                 rtn =  True
         return rtn
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2/oneclick/discovery/cleanup.py` & `com.castsoftware.uc.oneclick-0.2.2.1/oneclick/discovery/cleanup.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2/oneclick/discovery/cloc.py` & `com.castsoftware.uc.oneclick-0.2.2.1/oneclick/discovery/cloc.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,17 +38,17 @@
     def cloc_project(cls):
         return f'{cls.cloc_base}\\{cls.config.project_name}'
 
     @property
     def cloc_results(cls):
         return cls._df
 
-    def _run_cloc(cls,work_folder:str,cloc_output:str):
+    def _run_cloc(cls,work_folder:str,cloc_output:str,cloc_output_ignored:str):
         cloc_path=abspath(f'{getcwd()}\\scripts\\{cls.config.cloc_version}')
-        args = [cloc_path,work_folder,"--report-file",cloc_output,"--quiet"]
+        args = [cloc_path,work_folder,"--report-file",cloc_output,"--ignored",cloc_output_ignored,"--quiet"]
         proc = run_process(args,False)
 
         sleep(10)
         if proc.poll() is not None and exists(cloc_output):
             return 'DONE'
         else:
             return proc
@@ -66,32 +66,34 @@
 
         process = {}
         cloc_run=False
         for appl in config.application:
             cls._log.info(f'Running {config.project_name}/{appl}')
             create_folder(f'{config.report}/{config.project_name}/{appl}')
             cloc_output = abspath(f'{config.report}/{config.project_name}/{appl}/{appl}-cloc-{cls.phase}.txt')
+            cloc_output_ignored = abspath(f'{config.report}/{config.project_name}/{appl}/{appl}-cloc-ignored-{cls.phase}.txt')
             work_folder = abspath(f'{config.work}/AIP/{config.project_name}/{appl}')
 
             #if the report is already out there - no need to continue
             if exists(cloc_output):
                 process[appl]=None
                 continue 
             cloc_run=True
-            process[appl] = cls._run_cloc(work_folder,cloc_output)
+            process[appl] = cls._run_cloc(work_folder,cloc_output,cloc_output_ignored)
 
         #has all cloc processing completed
         all_done=False
         while (not all_done):
             all_done=True
             for p in process:
                 if process[p]=='DONE':
                     continue
                 all_done=False
                 cloc_output = abspath(f'{config.report}/{config.project_name}/{p}/{p}-cloc-{cls.phase}.txt')
+                cloc_output_ignored = abspath(f'{config.report}/{config.project_name}/{p}/{p}-cloc-ignored-{cls.phase}.txt')
                 if not process[p] is None:
                     cls._log.info(f'Checking results for {config.project_name}/{p}')
                     try:
                         ret,output = check_process(process[p],False)
                         if ret != 0 and not exists(cloc_output) and getsize(cloc_output) == 0:
                             cls._log.error(f'Error running cloc on {cloc_output} ({ret})')
                     except IOError:
@@ -102,26 +104,32 @@
                     process[p]='DONE'
             if cloc_run:
                 sleep(60)
 
         for appl in config.application:
             #reading cloc_output.txt file
             cloc_output = abspath(f'{config.report}/{config.project_name}/{appl}/{appl}-cloc-{cls.phase}.txt')
+            cloc_output_ignored = abspath(f'{config.report}/{config.project_name}/{appl}/{appl}-cloc-ignored-{cls.phase}.txt') 
             cls._log.info(f'Processing {cloc_output}')
             summary_list=[]   
             with open(cloc_output, 'r') as f:
                 content = f.read()
                 f.seek(0)
                 summary_list= [line.rstrip('\n').lstrip() for line in f]
                 #print(summary_list)
 
             #extracting required data from content of cloc_output.txt using python regex
             pattern='(\S{1,}|\w{1,}[:])\s{1,}(\d{1,})\s{1,}(\d{1,})\s{1,}(\d{1,})\s{1,}(\d{1,})'
             statistics_list=findall(pattern,content)
             statistics_list= statistics_list[:-1]
+            
+            with open(cloc_output_ignored, 'r') as fp:
+                lines = len(fp.readlines())
+            statistics_list.append(('Unknown Files',lines,'0','0','0'))
+
             df = DataFrame(statistics_list,columns=['LANGUAGE','FILES','BLANK','COMMENT','CODE'])
 
             #making technolgy check as case sensitive
             def all_lower(my_list):
                 return list(map(lambda x: x.lower(), my_list))
             tech_list = all_lower(tech_list)
             df['APPLICABLE']=df['LANGUAGE'].str.lower().isin(tech_list)
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2/oneclick/discovery/discoveryReport.py` & `com.castsoftware.uc.oneclick-0.2.2.1/oneclick/discovery/discoveryReport.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2/oneclick/discovery/prep.py` & `com.castsoftware.uc.oneclick-0.2.2.1/oneclick/discovery/prep.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         if not exists(config.deliver):
             raise ValueError(f'{config.deliver} does not exist')
 
         #scan delivery folder for application folders
         dir=[]
         for (dirpath,dirnames,filenames) in walk(config.deliver,topdown=False):
             dir.extend(dirnames)
+        config.application.clear()
         config.application=dirnames
 
         """create the application folders under 'work'
             base
             |-DELIVER
             |-STAGE
             | |-project
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2/oneclick/discovery/sqlDiscovery.py` & `com.castsoftware.uc.oneclick-0.2.2.1/oneclick/discovery/sqlDiscovery.py`

 * *Files 26% similar despite different names*

```diff
@@ -125,20 +125,35 @@
             tbl_list=findall(table_pattern,content)
             cls.table_list.extend(tbl_list)
 
             proc_pattern='[C|c][R|r][E|e][A|a][T|t][E|e]\s{1,}[P|p][R|r][O|o][C|c][E|e][D|d][U|u][R|r][E|e]\s{1,}([^\n|^\s|^\(]+)'
             proc_list=findall(proc_pattern,content)
             cls.procedure_list.extend(proc_list)
 
+            #regular expressions for PL/SQL
+            proc_pattern_2='[P|p][R|r][O|o][C|c][E|e][D|d][U|u][R|r][E|e]\s{1,}([^\n|^\s|^\(]+)'
+            proc_list_2=findall(proc_pattern_2,content)
+            cls.procedure_list.extend(proc_list_2)
+
             func_pattern='[C|c][R|r][E|e][A|a][T|t][E|e]\s{1,}[F|f][U|u][N|n][C|c][T|t][I|i][O|o][N|n]\s{1,}([^\n|^\s|^\(]+)'
             func_list=findall(func_pattern,content)
             cls.function_list.extend(func_list)
 
+            #regular expressions for PL/SQL
+            func_pattern_2='[F|f][U|u][N|n][C|c][T|t][I|i][O|o][N|n]\s{1,}([^\n|^\s|^\(]+)'
+            func_list_2=findall(func_pattern_2,content)
+            cls.function_list.extend(func_list_2)
+
             view_pattern='[C|c][R|r][E|e][A|a][T|t][E|e]\s{1,}[V|v][I|i][E|e][W|w]\s{1,}([^\n|^\s|^\(]+)'
             vi_list=findall(view_pattern,content)
             cls.view_list.extend(vi_list)
 
             trig_pattern='[C|c][R|r][E|e][A|a][T|t][E|e]\s{1,}[T|t][R|r][I|i][G|g][G|g][E|e][R|r]\s{1,}([^\n|^\s|^\(]+)'
             trig_list=findall(trig_pattern,content)
             cls.trigger_list.extend(trig_list)
+
+            #regular expressions for PL/SQL
+            trig_pattern_2='[C|c][R|r][E|e][A|a][T|t][E|e]\s{1,}[T|t][R|r][I|i][G|g][G|g][E|e][R|r]\s{1,}([^\n|^\s|^\(]+)'
+            trig_list_2=findall(trig_pattern_2,content)
+            cls.trigger_list.extend(trig_list_2)
             
             f.close()
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2/oneclick/discovery/unzip.py` & `com.castsoftware.uc.oneclick-0.2.2.1/oneclick/discovery/unzip.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2/oneclick/main.py` & `com.castsoftware.uc.oneclick-0.2.2.1/oneclick/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,16 @@
                     log.error('One or more analysis failed, review logs and restart')
                     break
                 elif status > 0:
                     break
 
 
         if args.end == 'Analysis':
-            break
+            if issubclass(type(p), RunARG):
+                break
 
         if args.start in ['Discovery','Analysis','Report']:
             if issubclass(type(p), RunARG):
                 status = p.run(config)
 
         # if issubclass(type(p), ActionPlan):
         #     for appl in config.application:
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2/oneclick/runArg.py` & `com.castsoftware.uc.oneclick-0.2.2.1/oneclick/runArg.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,18 @@
             log_name = cls.__class__.__name__
             
         cls._log = Logger(log_name,log_level)
         cls._config = config
         pass
 
     def run(cls,config:Config,appl_name:str=None,operation:str=None) -> bool:
+        if not config.is_aip_active:
+            cls._log.warning('Dashboard configureaton is incomplete, Assessment report will NOT be generated')
+            return -1
+
         if appl_name is None:
             appl_name = 'FULL'
         
         cfg = {}
         cfg['company']=config.company_name
         cfg['project']=config.project['name']
         cfg['template']=abspath(config.arg_template)
```

### Comparing `com.castsoftware.uc.oneclick-0.2.2/oneclick/sendEmail.py` & `com.castsoftware.uc.oneclick-0.2.2.1/oneclick/sendEmail.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.2/pyproject.toml` & `com.castsoftware.uc.oneclick-0.2.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [project]
 name='com.castsoftware.uc.oneclick'
 description="Assessment Generator"
-version='0.2.2' #prod version
+version='0.2.2.1' #prod version
 dependencies = [
-    'pandas','python-pptx==0.6.18','python-docx',
+    'pandas==1.4.0','python-pptx==0.6.18','python-docx','argparse_formatter',
     'com.castsoftware.uc.python.common>=0.1.6',
     'com.castsoftware.uc.action-plan',
     'com.castsoftware.uc.arg'
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
+
 requires-python = ">=3.10"
 readme = "README.md"
 [project.urls]
 "Homepage" = "https://github.com/CAST-Extend/com.castsoftware.uc.arg"
 "Bug Tracker" = "https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues"
```

