# Comparing `tmp/NorconsultPiPythonDevelop-1.0.9-py3-none-any.whl.zip` & `tmp/NorconsultPiPythonDevelop-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 5828 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat     3174 b- defN 22-Sep-23 12:06 NorconsultPiPythonDevelop/copyFiles.py
--rw-rw-rw-  2.0 fat     1736 b- defN 22-Sep-23 09:46 NorconsultPiPythonDevelop/generateDocs.py
--rw-rw-rw-  2.0 fat     2046 b- defN 22-Sep-23 09:55 NorconsultPiPythonDevelop/init.py
--rw-rw-rw-  2.0 fat     2955 b- defN 22-Sep-23 09:56 NorconsultPiPythonDevelop/serverPaths.py
--rw-rw-rw-  2.0 fat      522 b- defN 22-Sep-23 12:06 NorconsultPiPythonDevelop-1.0.9.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      523 b- defN 22-Sep-23 12:06 NorconsultPiPythonDevelop-1.0.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 22-Sep-23 12:06 NorconsultPiPythonDevelop-1.0.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       26 b- defN 22-Sep-23 12:06 NorconsultPiPythonDevelop-1.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      858 b- defN 22-Sep-23 12:06 NorconsultPiPythonDevelop-1.0.9.dist-info/RECORD
-9 files, 11937 bytes uncompressed, 4312 bytes compressed:  63.9%
+Zip file size: 52812 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat     3895 b- defN 23-Apr-20 10:25 NorconsultPiPythonDevelop/copyFiles.py
+-rw-rw-rw-  2.0 fat     1741 b- defN 23-Apr-19 11:35 NorconsultPiPythonDevelop/generateDocs.py
+-rw-rw-rw-  2.0 fat     2441 b- defN 23-Apr-20 10:30 NorconsultPiPythonDevelop/init.py
+-rw-rw-rw-  2.0 fat   856957 b- defN 23-Apr-20 10:25 NorconsultPiPythonDevelop/init.pyi
+-rw-rw-rw-  2.0 fat     2955 b- defN 23-Apr-19 11:35 NorconsultPiPythonDevelop/serverPaths.py
+-rw-rw-rw-  2.0 fat      522 b- defN 23-Apr-20 10:33 NorconsultPiPythonDevelop-1.1.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      478 b- defN 23-Apr-20 10:33 NorconsultPiPythonDevelop-1.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-20 10:33 NorconsultPiPythonDevelop-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       26 b- defN 23-Apr-20 10:33 NorconsultPiPythonDevelop-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      951 b- defN 23-Apr-20 10:33 NorconsultPiPythonDevelop-1.1.0.dist-info/RECORD
+10 files, 870058 bytes uncompressed, 51152 bytes compressed:  94.1%
```

## zipnote {}

```diff
@@ -3,26 +3,29 @@
 
 Filename: NorconsultPiPythonDevelop/generateDocs.py
 Comment: 
 
 Filename: NorconsultPiPythonDevelop/init.py
 Comment: 
 
+Filename: NorconsultPiPythonDevelop/init.pyi
+Comment: 
+
 Filename: NorconsultPiPythonDevelop/serverPaths.py
 Comment: 
 
-Filename: NorconsultPiPythonDevelop-1.0.9.dist-info/LICENSE.txt
+Filename: NorconsultPiPythonDevelop-1.1.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: NorconsultPiPythonDevelop-1.0.9.dist-info/METADATA
+Filename: NorconsultPiPythonDevelop-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: NorconsultPiPythonDevelop-1.0.9.dist-info/WHEEL
+Filename: NorconsultPiPythonDevelop-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: NorconsultPiPythonDevelop-1.0.9.dist-info/top_level.txt
+Filename: NorconsultPiPythonDevelop-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: NorconsultPiPythonDevelop-1.0.9.dist-info/RECORD
+Filename: NorconsultPiPythonDevelop-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## NorconsultPiPythonDevelop/copyFiles.py

```diff
@@ -1,68 +1,88 @@
 
 import os 
 from serverPaths import getServerPaths
 import shutil
+import glob
 
 def copyAllFiles(): 
-    serverPaths = getServerPaths()
+    try: 
+        serverPaths = getServerPaths()
+    except Exception as e: 
+        print("Could not get server paths. Check that you are connected to Norconsult VPN")
+        raise e
 
     destinationFolder = "C:\\Users\\" + os.getlogin() + "\\AppData\\Roaming\\Norconsult\\NorconsultPiPythonDevelop\\"
-    destinationFolderAuth =  "C:\\Users\\" + os.getlogin() + "\\AppData\\Roaming\\Norconsult\\NorconsultPiPythonDevelopAuth\\"
-    destinationFolderDocumentation =  "C:\\Users\\" + os.getlogin() + "\\AppData\\Roaming\\Norconsult\\NorconsultPiPythonDevelopDocumentation\\"
-
+    destinationFolderAuth =  "C:\\Users\\" + os.getlogin() + "\\AppData\\Roaming\\Norconsult\\NorconsultPiPython_auth\\"
 
     if not os.path.exists(destinationFolder):
         os.makedirs(destinationFolder)
         
     if not os.path.exists(destinationFolderAuth):
         os.makedirs(destinationFolderAuth)
-
-    if not os.path.exists(destinationFolderAuth):
-        os.makedirs(destinationFolderDocumentation)
         
-    analysisPath = serverPaths["Analysis"]
-    modellingPath = serverPaths["Modelling"]
-    modelBuilderFEMPath = serverPaths['ModelBuilder_FEM']
-    modelBuilderRobotPath = serverPaths["ModelBuilder_Robot"]
-    auth_python_Path = serverPaths["auth_python"]
-    documentationPath = serverPaths["documentation"]
+
+    try: 
+        analysisPath = serverPaths["Analysis"]
+        modellingPath = serverPaths["Modelling"]
+        modelBuilderFEMPath = serverPaths['ModelBuilder_FEM']
+        modelBuilderRobotPath = serverPaths["ModelBuilder_Robot"]
+        auth_python_Path = serverPaths["auth_python"]
+        stubsPath = serverPaths["stubs"]
+        femIntegratedPath = serverPaths["FemIntegrated"]
+    except Exception as e: 
+        raise e
+
 
     filesToCopyAnalysis = os.listdir(analysisPath)
     filesToCopyModelling = os.listdir(modellingPath)
     filesToCopyFEM = os.listdir(modelBuilderFEMPath)
     filesToCopyRobot = os.listdir(modelBuilderRobotPath)
     filesToCopy_auth_python = os.listdir(auth_python_Path)
-    filesToCopyDocumentation = os.listdir(documentationPath)
+    filesToCopyStubs = os.listdir(stubsPath)
+    filesToCopyFemIntegrated = os.listdir(femIntegratedPath)
+    
+    
+    directoryPiPython = os.path.dirname(os.path.abspath(__file__))
+    #check for multiple stubs file in the folder (in case we change the name of the stub file) and select the newest
+    if len(filesToCopyStubs) > 0: 
+        # get all files in the folder that end with '.pyi'
+        files = glob.glob(os.path.join(stubsPath, '*.pyi'))
+        # sort the files by creation time and get the newest one
+        stubsFileToCopy = max(files, key=os.path.getctime)
+        stubsFileDestination = os.path.join(directoryPiPython, "init.pyi")
+        shutil.copy2(stubsFileToCopy, stubsFileDestination)
+    else: 
+        print("Could not locate any stub-file to copy.")
 
-    for file in filesToCopyAnalysis: 
-        if requiresUpdate(analysisPath + file, destinationFolder + file): 
-            shutil.copyfile(analysisPath + file, destinationFolder + file)
+    
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
             
     for file in filesToCopyRobot: 
         if requiresUpdate(modelBuilderRobotPath + file, destinationFolder + file): 
             shutil.copyfile(modelBuilderRobotPath + file, destinationFolder + file)
     
     for file in filesToCopy_auth_python:
         if requiresUpdate(auth_python_Path + file, destinationFolderAuth + file):
             shutil.copyfile(auth_python_Path + file, destinationFolderAuth + file)
-    
-    for file in filesToCopyDocumentation:
-        if file.endswith(".html"): 
-            if requiresUpdate(documentationPath + file, destinationFolderDocumentation + file):
-                shutil.copyfile(documentationPath + file, destinationFolderDocumentation + file)
-    
+            
+    for file in filesToCopyAnalysis: 
+        if requiresUpdate(analysisPath + file, destinationFolder + file): 
+            shutil.copyfile(analysisPath + file, destinationFolder + file)
+            
+    for file in filesToCopyModelling: 
+        if requiresUpdate(modellingPath + file, destinationFolder + file): 
+            shutil.copyfile(modellingPath + file, destinationFolder + file)
+
 
 def requiresUpdate(serverFilePath, destFilePath):
     if not os.path.isfile(destFilePath): 
         return True 
     
     serverFilePathCreatedDate = os.path.getmtime(serverFilePath)
     destFilePathCreatedDate = os.path.getmtime(destFilePath)
```

## NorconsultPiPythonDevelop/generateDocs.py

```diff
@@ -9,20 +9,17 @@
     
 def getModuleDocumentation(norconsultModule):
     """
 
     Args:
         norconsultModule (object): c# namespace of module imported from Norconsult
         Options: 
-            - mapi
-            - api
-            - mext
-            - aext
-            - fem
-            - robot
+            - Norconsult.PI.APIConnect.Analysis
+            - Norconsult.PI.APIConnect.Modelling
+            - FEMDesign
 
     """
     #for discpiline, bar, node etc
     for moduleName, module in inspect.getmembers(norconsultModule):
         if not moduleName.startswith('__'):
             print()
             print(Fore.CYAN + moduleName)
```

## NorconsultPiPythonDevelop/init.py

```diff
@@ -1,50 +1,64 @@
 import subprocess
 import os
+import os
 import clr
 import sys
 file_dir = os.path.dirname(__file__)
 sys.path.append(file_dir)
 from copyFiles import copyAllFiles
-from generateDocs import getModuleDocumentation
 #Copy All Files
 copyAllFiles()
 
 #Authentificate
-authPath = "C:\\Users\\" + os.getlogin() + "\\AppData\\Roaming\\Norconsult\\NorconsultPiPythonDevelop_auth\\PiPython.exe"
+authPath = "C:\\Users\\" + os.getlogin() + "\\AppData\\Roaming\\Norconsult\\NorconsultPiPython_auth\\PiPython.exe"
 subprocess.check_call([authPath])
 
 ##Importing PI libraries and dependencies
 referenceFolder = "C:\\Users\\" + os.getlogin() + "\\AppData\\Roaming\\Norconsult\\NorconsultPiPythonDevelop"
 modellingDllPath = referenceFolder + "\\APIClientModelling.dll" 
 analysisDllPath = referenceFolder + "\\APIClientAnalysis.dll" 
 commonDllPath = referenceFolder + "\\Norconsult.PI.Common.dll"
 FEMmodelBuilderPath = referenceFolder + "\\ModelBuilder_FEM_Design.dll";
 RobotModelBuilderPath = referenceFolder + "\\ModelBuilder_Robot.dll"
+FemIntegratedPath = referenceFolder + "\\FEMIntegrated.dll"
 
 clr.AddReference(modellingDllPath)
 clr.AddReference(analysisDllPath)
 clr.AddReference(commonDllPath)
 clr.AddReference(FEMmodelBuilderPath)
 clr.AddReference(RobotModelBuilderPath)
+clr.AddReference(FemIntegratedPath)
+
 
 #Imports 
 import Norconsult.PI.APIConnect.Analysis as aapi 
 import Norconsult.PI.Common.API.Models.Analysis as adto
 import Norconsult.PI.APIConnect.Analysis.Extensions as aext
 import Norconsult.PI.APIConnect.Helpers.Analysis as ahel
 
 import Norconsult.PI.APIConnect.Modelling as mapi 
 import Norconsult.PI.Common.API.Models.Modelling as mdto
 import Norconsult.PI.APIConnect.Modelling.Extensions as mext
 import Norconsult.PI.APIConnect.Helpers.Modelling as mhel
+import Norconsult.PI.Common.API.Models.Common as cdto
 
 import FEMDesign as fem
 import Robot as robot
 
+import FEMIntegrated as fi
+
+adto.__dict__['AdministrativeUnits'] = cdto.AdministrativeUnits
+mdto.__dict__['AdministrativeUnits'] = cdto.AdministrativeUnits
+
 #Apperently we have to import clr twice so add Norconsult namespace in clr
 import clr
-print("Welcome to PiPython!")
-print("This is the develop version of our package, this means all request will be sent to our test database.")
-print("If you need startup help, check the documentation file: " + str("C:\\Users\\" + os.getlogin() + "\\AppData\\Roaming\\Norconsult\\NorconsultPiPythonDevelopDocumentation\\README.html"))
-
+documentationPath = "C:\\Users\\" + os.getlogin() + "\\AppData\\Roaming\\Norconsult\\NorconsultPiPythonDocumentation\\README.html"
+print('Welcome to PiPython!')
+print('This is the develop version of our package, this means all request will be sent to our test database.')
+print('If you need startup help, check out https://norconsult365.sharepoint.com/sites/pamintegrated')
+print()
 
+import os
+from colorama import Fore, Style
+import inspect
+import clr
```

## Comparing `NorconsultPiPythonDevelop-1.0.9.dist-info/LICENSE.txt` & `NorconsultPiPythonDevelop-1.1.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `NorconsultPiPythonDevelop-1.0.9.dist-info/RECORD` & `NorconsultPiPythonDevelop-1.1.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-NorconsultPiPythonDevelop/copyFiles.py,sha256=trq28FBJ4Z_allJGvfMMj4-XQs-eDRARptPfsnichac,3174
-NorconsultPiPythonDevelop/generateDocs.py,sha256=5J3m-Nkfa8YMZBIdpKgkahPDcFWcKzPxOCZ6KBnKJrw,1736
-NorconsultPiPythonDevelop/init.py,sha256=1LmfX_-9GNzZn_dDDAthgHFXix_Tj2ikyU9y_vSmyq4,2046
+NorconsultPiPythonDevelop/copyFiles.py,sha256=g7nRHb6sIIm1rducvWuTX7ndQrYBWta2Y_WBvYKHrD8,3895
+NorconsultPiPythonDevelop/generateDocs.py,sha256=atYapsXS7otjHYqrPT2Q1R0Xd9dl3H1BSBube2TOCy8,1741
+NorconsultPiPythonDevelop/init.py,sha256=_HwA_t6oQCnCBPcRHzQdSuTzdjzvQzPvgc-Yp0lljGw,2441
+NorconsultPiPythonDevelop/init.pyi,sha256=-mNnRFl-WT4J3dxqCERkTCK7hKrYMDO-jWDcaYaAstM,856957
 NorconsultPiPythonDevelop/serverPaths.py,sha256=w7rBDb_5WJQ9py7gFPoFqFVEVdVByAzHU1MactsVrdM,2955
-NorconsultPiPythonDevelop-1.0.9.dist-info/LICENSE.txt,sha256=xP8JWp8KEvQSDKceBSItrPKJW4UXslBffo0IdDoGcN4,522
-NorconsultPiPythonDevelop-1.0.9.dist-info/METADATA,sha256=pV3A5J6AqSeUlmu_ZSdmdwWGKEAw0BvjdzYX8ynj114,523
-NorconsultPiPythonDevelop-1.0.9.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
-NorconsultPiPythonDevelop-1.0.9.dist-info/top_level.txt,sha256=mk9Yv7wHxSidak7AkcDC4Y_x3WUYO-sSBAQG5ycMGg8,26
-NorconsultPiPythonDevelop-1.0.9.dist-info/RECORD,,
+NorconsultPiPythonDevelop-1.1.0.dist-info/LICENSE.txt,sha256=xP8JWp8KEvQSDKceBSItrPKJW4UXslBffo0IdDoGcN4,522
+NorconsultPiPythonDevelop-1.1.0.dist-info/METADATA,sha256=UgaH7mazegsT8YNZ6LeTWI1iey887IUEYLcv7jlWbjw,478
+NorconsultPiPythonDevelop-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+NorconsultPiPythonDevelop-1.1.0.dist-info/top_level.txt,sha256=mk9Yv7wHxSidak7AkcDC4Y_x3WUYO-sSBAQG5ycMGg8,26
+NorconsultPiPythonDevelop-1.1.0.dist-info/RECORD,,
```

