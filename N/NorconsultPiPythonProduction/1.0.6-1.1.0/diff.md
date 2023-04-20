# Comparing `tmp/NorconsultPiPythonProduction-1.0.6-py3-none-any.whl.zip` & `tmp/NorconsultPiPythonProduction-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6275 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat     3531 b- defN 23-Mar-30 07:45 NorconsultPiPythonProduction/copyFiles.py
--rw-rw-rw-  2.0 fat     1741 b- defN 23-Mar-06 09:52 NorconsultPiPythonProduction/generateDocs.py
--rw-rw-rw-  2.0 fat     2325 b- defN 23-Mar-30 07:45 NorconsultPiPythonProduction/init.py
--rw-rw-rw-  2.0 fat     2964 b- defN 23-Mar-06 09:52 NorconsultPiPythonProduction/serverPaths.py
--rw-rw-rw-  2.0 fat      522 b- defN 23-Mar-30 07:47 NorconsultPiPythonProduction-1.0.6.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      495 b- defN 23-Mar-30 07:47 NorconsultPiPythonProduction-1.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Mar-30 07:47 NorconsultPiPythonProduction-1.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       29 b- defN 23-Mar-30 07:47 NorconsultPiPythonProduction-1.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      885 b- defN 23-Mar-30 07:47 NorconsultPiPythonProduction-1.0.6.dist-info/RECORD
-9 files, 12589 bytes uncompressed, 4705 bytes compressed:  62.6%
+Zip file size: 6354 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat     3875 b- defN 23-Apr-20 10:36 NorconsultPiPythonProduction/copyFiles.py
+-rw-rw-rw-  2.0 fat     1741 b- defN 23-Apr-19 11:35 NorconsultPiPythonProduction/generateDocs.py
+-rw-rw-rw-  2.0 fat     2462 b- defN 23-Apr-20 10:36 NorconsultPiPythonProduction/init.py
+-rw-rw-rw-  2.0 fat     2964 b- defN 23-Apr-19 11:35 NorconsultPiPythonProduction/serverPaths.py
+-rw-rw-rw-  2.0 fat      522 b- defN 23-Apr-20 10:38 NorconsultPiPythonProduction-1.1.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      484 b- defN 23-Apr-20 10:38 NorconsultPiPythonProduction-1.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-20 10:38 NorconsultPiPythonProduction-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       29 b- defN 23-Apr-20 10:38 NorconsultPiPythonProduction-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      885 b- defN 23-Apr-20 10:38 NorconsultPiPythonProduction-1.1.0.dist-info/RECORD
+9 files, 13054 bytes uncompressed, 4784 bytes compressed:  63.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: NorconsultPiPythonProduction/init.py
 Comment: 
 
 Filename: NorconsultPiPythonProduction/serverPaths.py
 Comment: 
 
-Filename: NorconsultPiPythonProduction-1.0.6.dist-info/LICENSE.txt
+Filename: NorconsultPiPythonProduction-1.1.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: NorconsultPiPythonProduction-1.0.6.dist-info/METADATA
+Filename: NorconsultPiPythonProduction-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: NorconsultPiPythonProduction-1.0.6.dist-info/WHEEL
+Filename: NorconsultPiPythonProduction-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: NorconsultPiPythonProduction-1.0.6.dist-info/top_level.txt
+Filename: NorconsultPiPythonProduction-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: NorconsultPiPythonProduction-1.0.6.dist-info/RECORD
+Filename: NorconsultPiPythonProduction-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## NorconsultPiPythonProduction/copyFiles.py

```diff
@@ -22,59 +22,65 @@
     try:
         analysisPath = serverPaths["Analysis"]
         modellingPath = serverPaths["Modelling"]
         modelBuilderFEMPath = serverPaths['ModelBuilder_FEM']
         modelBuilderRobotPath = serverPaths["ModelBuilder_Robot"]
         auth_python_Path = serverPaths["auth_python"]
         stubsPath = serverPaths["stubs"]
+        femIntegratedPath = serverPaths["FemIntegrated"]
     except Exception as e: 
         raise e
     
     filesToCopyAnalysis = os.listdir(analysisPath)
     filesToCopyModelling = os.listdir(modellingPath)
     filesToCopyFEM = os.listdir(modelBuilderFEMPath)
     filesToCopyRobot = os.listdir(modelBuilderRobotPath)
     filesToCopy_auth_python = os.listdir(auth_python_Path)
     filesToCopyStubs = os.listdir(stubsPath)
+    filesToCopyFemIntegrated = os.listdir(femIntegratedPath)
 
     
     directoryPiPython = os.path.dirname(os.path.abspath(__file__))
     #check for multiple stubs file in the folder (in case we change the name of the stub file) and select the newest
     if len(filesToCopyStubs) > 0: 
         # get all files in the folder that end with '.pyi'
         files = glob.glob(os.path.join(stubsPath, '*.pyi'))
         # sort the files by creation time and get the newest one
         stubsFileToCopy = max(files, key=os.path.getctime)
         stubsFileDestination = os.path.join(directoryPiPython, "init.pyi")
         shutil.copy2(stubsFileToCopy, stubsFileDestination)
     else: 
         print("Could not locate any stub-file to copy.")
 
-
-    for file in filesToCopyAnalysis: 
-        if requiresUpdate(analysisPath + file, destinationFolder + file): 
-            shutil.copyfile(analysisPath + file, destinationFolder + file)
+    for file in filesToCopyFemIntegrated: 
+        if requiresUpdate(femIntegratedPath + file, destinationFolder + file): 
+            shutil.copyfile(femIntegratedPath + file, destinationFolder + file)
             
-    for file in filesToCopyModelling: 
-        if requiresUpdate(modellingPath + file, destinationFolder + file): 
-            shutil.copyfile(modellingPath + file, destinationFolder + file)
-
     for file in filesToCopyFEM: 
         if requiresUpdate(modelBuilderFEMPath + file, destinationFolder + file): 
             shutil.copyfile(modelBuilderFEMPath + file, destinationFolder + file)
-            
+                
     for file in filesToCopyRobot: 
         if requiresUpdate(modelBuilderRobotPath + file, destinationFolder + file): 
             shutil.copyfile(modelBuilderRobotPath + file, destinationFolder + file)
     
     for file in filesToCopy_auth_python:
         if requiresUpdate(auth_python_Path + file, destinationFolderAuth + file):
             shutil.copyfile(auth_python_Path + file, destinationFolderAuth + file)
     
 
+    for file in filesToCopyAnalysis: 
+        if requiresUpdate(analysisPath + file, destinationFolder + file): 
+            shutil.copyfile(analysisPath + file, destinationFolder + file)
+            
+    for file in filesToCopyModelling: 
+        if requiresUpdate(modellingPath + file, destinationFolder + file): 
+            shutil.copyfile(modellingPath + file, destinationFolder + file)
+
+
 def requiresUpdate(serverFilePath, destFilePath):
     if not os.path.isfile(destFilePath): 
         return True 
     
     serverFilePathCreatedDate = os.path.getmtime(serverFilePath)
     destFilePathCreatedDate = os.path.getmtime(destFilePath)
     if serverFilePathCreatedDate >  destFilePathCreatedDate:
```

## NorconsultPiPythonProduction/init.py

```diff
@@ -16,20 +16,22 @@
 ##Importing PI libraries and dependencies
 referenceFolder = "C:\\Users\\" + os.getlogin() + "\\AppData\\Roaming\\Norconsult\\NorconsultPiPythonProduction"
 modellingDllPath = referenceFolder + "\\APIClientModelling.dll" 
 analysisDllPath = referenceFolder + "\\APIClientAnalysis.dll" 
 commonDllPath = referenceFolder + "\\Norconsult.PI.Common.dll"
 FEMmodelBuilderPath = referenceFolder + "\\ModelBuilder_FEM_Design.dll";
 RobotModelBuilderPath = referenceFolder + "\\ModelBuilder_Robot.dll"
+FemIntegratedPath = referenceFolder + "\\FemIntegrated.dll"
 
 clr.AddReference(modellingDllPath)
 clr.AddReference(analysisDllPath)
 clr.AddReference(commonDllPath)
 clr.AddReference(FEMmodelBuilderPath)
 clr.AddReference(RobotModelBuilderPath)
+clr.AddReference(FemIntegratedPath)
 
 
 #Imports 
 import Norconsult.PI.APIConnect.Analysis as aapi 
 import Norconsult.PI.Common.API.Models.Analysis as adto
 import Norconsult.PI.APIConnect.Analysis.Extensions as aext
 import Norconsult.PI.APIConnect.Helpers.Analysis as ahel
@@ -38,24 +40,26 @@
 import Norconsult.PI.Common.API.Models.Modelling as mdto
 import Norconsult.PI.APIConnect.Modelling.Extensions as mext
 import Norconsult.PI.APIConnect.Helpers.Modelling as mhel
 import Norconsult.PI.Common.API.Models.Common as cdto
 
 import FEMDesign as fem
 import Robot as robot
+import FEMIntegrated as fi 
 
 adto.__dict__['AdministrativeUnits'] = cdto.AdministrativeUnits
 mdto.__dict__['AdministrativeUnits'] = cdto.AdministrativeUnits
 
 #Apperently we have to import clr twice so add Norconsult namespace in clr
 import clr
 documentationPath = authPath = "C:\\Users\\" + os.getlogin() + "\\AppData\\Roaming\\Norconsult\\NorconsultPiPythonDocumentation\\README.html"
 print('Welcome to PiPython!')
 print('This is the main version of our package, this means all request will be sent to our production database.')
 print('If you need startup help, check out https://norconsult365.sharepoint.com/sites/pamintegrated')
+print() 
 
 import os
 from colorama import Fore, Style
 import inspect
 import clr
```

## Comparing `NorconsultPiPythonProduction-1.0.6.dist-info/LICENSE.txt` & `NorconsultPiPythonProduction-1.1.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `NorconsultPiPythonProduction-1.0.6.dist-info/RECORD` & `NorconsultPiPythonProduction-1.1.0.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-NorconsultPiPythonProduction/copyFiles.py,sha256=_gNuNPQsgTqsAeFaInivC_jviUutKkdIW_CzDp2-cwk,3531
+NorconsultPiPythonProduction/copyFiles.py,sha256=O3lNWBjxhD7dqz__gMV1GczFHn52GdCAHOz6ARmp4yc,3875
 NorconsultPiPythonProduction/generateDocs.py,sha256=atYapsXS7otjHYqrPT2Q1R0Xd9dl3H1BSBube2TOCy8,1741
-NorconsultPiPythonProduction/init.py,sha256=_KSrnH3wW8zn8mj9orP1IdwyF51bUBKHsdvGHG6O0zI,2325
+NorconsultPiPythonProduction/init.py,sha256=6aFMNS7quza0rDydiNo0e_K5X-1SkM6MUnrTCIJv-gs,2462
 NorconsultPiPythonProduction/serverPaths.py,sha256=llo0qxApr20l2W8w8uU0g7XsC1TDA-n5SO9Xg3C8xo0,2964
-NorconsultPiPythonProduction-1.0.6.dist-info/LICENSE.txt,sha256=xP8JWp8KEvQSDKceBSItrPKJW4UXslBffo0IdDoGcN4,522
-NorconsultPiPythonProduction-1.0.6.dist-info/METADATA,sha256=CLKCcP-SN9ja8KCKPbZ2yj5JY-eNYeHp5HlbIAOelHg,495
-NorconsultPiPythonProduction-1.0.6.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
-NorconsultPiPythonProduction-1.0.6.dist-info/top_level.txt,sha256=dYiigbRKWMSRQvM7xEMKSdFuaQhyyhOfSR7BqUJdn_w,29
-NorconsultPiPythonProduction-1.0.6.dist-info/RECORD,,
+NorconsultPiPythonProduction-1.1.0.dist-info/LICENSE.txt,sha256=xP8JWp8KEvQSDKceBSItrPKJW4UXslBffo0IdDoGcN4,522
+NorconsultPiPythonProduction-1.1.0.dist-info/METADATA,sha256=SCjAVWOGrljbP7V6tg-MKxfheV7KX4C_mAmaMiDmOuE,484
+NorconsultPiPythonProduction-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+NorconsultPiPythonProduction-1.1.0.dist-info/top_level.txt,sha256=dYiigbRKWMSRQvM7xEMKSdFuaQhyyhOfSR7BqUJdn_w,29
+NorconsultPiPythonProduction-1.1.0.dist-info/RECORD,,
```

