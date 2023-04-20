# Comparing `tmp/notifator-0.2.8.tar.gz` & `tmp/notifator-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/notifator-0.2.8.tar", last modified: Fri Mar 12 09:53:59 2021, max compression
+gzip compressed data, was "dist/notifator-0.2.9.tar", last modified: Wed Apr 28 12:34:02 2021, max compression
```

## Comparing `notifator-0.2.8.tar` & `notifator-0.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2021-03-12 09:53:59.523255 notifator-0.2.8/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      628 2021-03-12 09:53:59.523255 notifator-0.2.8/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      198 2021-01-13 13:04:43.000000 notifator-0.2.8/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2021-03-12 09:53:59.519255 notifator-0.2.8/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6106 2021-03-12 09:50:21.000000 notifator-0.2.8/bin/checkbtrfs
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1407 2020-09-02 14:01:18.000000 notifator-0.2.8/bin/login-notify.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      759 2021-02-09 13:53:43.000000 notifator-0.2.8/bin/notifator
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5442 2020-09-16 16:26:19.000000 notifator-0.2.8/bin/teleg_bot.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2021-03-12 09:53:59.523255 notifator-0.2.8/notifator/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2020-09-02 12:30:38.000000 notifator-0.2.8/notifator/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     7342 2021-03-01 09:28:48.000000 notifator-0.2.8/notifator/notify.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     7468 2021-02-09 13:56:07.000000 notifator-0.2.8/notifator/notihat.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4215 2021-03-11 09:02:22.000000 notifator-0.2.8/notifator/telegram.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       20 2021-03-12 09:53:59.000000 notifator-0.2.8/notifator/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2021-03-12 09:53:59.523255 notifator-0.2.8/notifator.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      628 2021-03-12 09:53:59.000000 notifator-0.2.8/notifator.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      322 2021-03-12 09:53:59.000000 notifator-0.2.8/notifator.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2021-03-12 09:53:59.000000 notifator-0.2.8/notifator.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2021-03-12 09:53:59.000000 notifator-0.2.8/notifator.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2021-03-12 09:53:59.523255 notifator-0.2.8/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1746 2020-11-03 18:17:44.000000 notifator-0.2.8/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2021-04-28 12:34:02.905717 notifator-0.2.9/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      628 2021-04-28 12:34:02.905717 notifator-0.2.9/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      198 2021-01-13 13:04:43.000000 notifator-0.2.9/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2021-04-28 12:34:02.905717 notifator-0.2.9/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     7709 2021-04-28 12:33:02.000000 notifator-0.2.9/bin/checkbtrfs
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1407 2020-09-02 14:01:18.000000 notifator-0.2.9/bin/login-notify.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      759 2021-02-09 13:53:43.000000 notifator-0.2.9/bin/notifator
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5442 2020-09-16 16:26:19.000000 notifator-0.2.9/bin/teleg_bot.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2021-04-28 12:34:02.905717 notifator-0.2.9/notifator/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2020-09-02 12:30:38.000000 notifator-0.2.9/notifator/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     7342 2021-03-01 09:28:48.000000 notifator-0.2.9/notifator/notify.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     7468 2021-02-09 13:56:07.000000 notifator-0.2.9/notifator/notihat.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4215 2021-03-11 09:02:22.000000 notifator-0.2.9/notifator/telegram.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       20 2021-04-28 12:34:02.000000 notifator-0.2.9/notifator/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2021-04-28 12:34:02.905717 notifator-0.2.9/notifator.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      628 2021-04-28 12:34:02.000000 notifator-0.2.9/notifator.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      322 2021-04-28 12:34:02.000000 notifator-0.2.9/notifator.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2021-04-28 12:34:02.000000 notifator-0.2.9/notifator.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2021-04-28 12:34:02.000000 notifator-0.2.9/notifator.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2021-04-28 12:34:02.905717 notifator-0.2.9/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1746 2020-11-03 18:17:44.000000 notifator-0.2.9/setup.py
```

### Comparing `notifator-0.2.8/PKG-INFO` & `notifator-0.2.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notifator
-Version: 0.2.8
+Version: 0.2.9
 Summary: Automatically created environment for python package
 Home-page: UNKNOWN
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description: # Project: notifator
```

### Comparing `notifator-0.2.8/bin/checkbtrfs` & `notifator-0.2.9/bin/checkbtrfs`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,43 @@
 #!/usr/bin/python3
 
+"""
+ When btrfs RAID collapses:
+
+btrfs fi sh
+
+mount -o degraded /mnt/sdc1 /mnt/raid
+
+#-----------IF PROBLEM WITH SIZE----------
+# check the sizes of the raid components
+ blockdev --getsize64 /dev/sdb1
+ blockdev --getsize64 /dev/sdc1
+
+ btrfs fi res 1:... /mnt/usb_raid/
+
+# 39998980096   i f-uped the size
+# 500106788864  sdb1 degraded
+# 480102055936  sdc1 empty
+# resize
+btrfs fi res 1:480102055936 /mnt/usb_raid/
+
+
+sudo btrfs replace start 7 /dev/sdf1 /mnt
+"""
+
+
 logfile="/tmp/btrfscheck.log"
 with open(logfile,"a") as f:
     f.write("Ahoj1-----------------------------------\n")
 
 import os
 import socket
 import requests
 import subprocess as sp
-
+import sys
 
 from notifator import telegram
 from fire import Fire
 
 
 def btrfssh():
     """
@@ -26,121 +51,157 @@
     # #print(r)
     # r=r.split("\n")
     # r=[ x for x in r if x.find("uuid:")>0 ]
     # uuids=[ x.split()[-1] for x in r ]
     # #print(uuids)
 
     #==========mounted?
+    print("D... MOUNTED")
     CMD='mount'
     r=sp.check_output(CMD.split()).decode("utf8")
     #print(r)
     r=r.split("\n")
     r=[ x for x in r if x.find("type btrfs")>0 ]
     #print(r)
     devs=[ x.split()[0] for x in r ]
     mpoints=[ x.split()[2] for x in r ]
     for i in range(len(devs)):
         output.append( "{:14s} : {}".format(devs[i],mpoints[i])  )
-        #print()
+        # print("D...    ",devs[i])
 
     #print()
     # #=========== datafree: data for each mount
     # for i in range(len(mpoints)):
     #     print("===={}====".format(devs[i]))
     #     CMD='sudo btrfs fi df '+mpoints[i]
     #     r=sp.check_output(CMD.split()).decode("utf8")
     #     #r=r.split("\n")
     #     print(r)
 
     #========== USAGE
+    print("D... btrfs FI SHOW")
     CMD="sudo btrfs fi show"
-    r=sp.check_output(CMD.split()).decode("utf8").split("\n")
+    quitme =  False
+    try:
+        r=sp.check_output(CMD.split()).decode("utf8").split("\n")
+    except Exception as e:
+        quitme = True
+    if quitme:
+        print("D... error on  BTRFS FI SH: No btrfs?")
+        sys.exit(0)
     activeuuid=""
+    if len(r)==0:
+        print("D... NO BTRFS partitions found mounted.")
+        sys.exit(0)
+
     for i in r:
         if i.find("uuid:")>0:
             activeuuid=i.split()[-1]
         if activeuuid=="":
             continue
         else:
             if i.find("size")>0 and i.find("used")>0:
                 size=i.strip().split()[3]
                 used=i.strip().split()[5]
                 path=i.strip().split()[-1]
                 #print()
                 output.append("{:14s} {} / {}".format(path,used,size))
+                print("D...    ",path)
     #print(r)
     #print()
     output.append("")
 
+    print("D... DEV STAT","_"*30)
     #=========== ERRORCHECK
     for i in range(len(mpoints)):
         #print()
         output.append("===={}====".format(devs[i]) )
         CMD='sudo btrfs device stats '+mpoints[i]
         r=sp.check_output(CMD.split()).decode("utf8")
         #r=r.split("\n")
         #print(r)
         for i in r.split("\n"):
             output.append(i)
+    # print("D...         ","_"*30)
+    return output,mpoints,devs
 
+
+
+
+def smartctl(output):
     #print()
+    print("D... SMARTCTL","_"*30)
     output.append("######## SMARTCTL ######")
     #=========smartctl - look at df first
     CMD="df"
     # can happen that pcloud is not connected... error...
     #try:
     #r=sp.check_output(CMD, shell=True).decode("utf8")
     er, r = sp.getstatusoutput(CMD)
     #except:
     #    print("X... there was an error in '{}' ... maybe pcloud mount?".format(CMD))
     # print("D... result = /{}/".format(r) )
     r = r.rstrip().split("\n")
     root=[x for x in r if x.split()[-1]=="/"]
+    #print("D...    root==", root)
     home=[x for x in r if x.split()[-1]=="/home"]
+    #print("D...    home==", home)
     roothome=[root[0].split()[0],home[0].split()[0]]
-    #print()
+    print("D...    roothome==", roothome)
     output.append("root/home: {}".format(roothome))
 
     #============ smartctl: i had -l error -H .... not enough i think
     #
     for i in roothome:
-        #print()
+        print("D...    i == root or home==",i)
         output.append("====={}======".format(i) )
         CMD="sudo smartctl -l error -H "+i
         r=sp.check_output(CMD.split()).decode("utf8").strip().split("\n")
         r=[x for x in r if x.find("smartctl ")<0]
         r=[x for x in r if x.find("Copyright")<0]
         r=[x for x in r if x.find("START OF READ")<0]
         r=[x for x in r if x.find("SMART Error Log Version")<0]
         r=[x.replace("overall-health self-assessment","") for x in r if len(x)>0]
         r=[x.replace("Error Information","") for x in r ]
         for j in r:
             output.append(j)
 
+        print("D...    -t LONG",i)
         CMD="sudo smartctl -t long "+i
         try:
             r=sp.check_output(CMD.split()).decode("utf8").strip().split("\n")
         except:
             print("X.. long test may be running")
+
+        print("D...    -l error -l selftest",i)
         CMD="sudo smartctl -l error -l selftest "+i
         try:
             r=sp.check_output(CMD.split()).decode("utf8").strip().split("\n")
         except sp.CalledProcessError as grepexc:
             print("X... ERROR DETECTED in  l error l selftest")
             r = grepexc.output.decode("utf8").strip().split("\n")
         r = [x for x in r if x.find("#")==0 ]
         r = [x for x in r if x.find("Completed without error")<0 ]
 
         for j in r:
             output.append(j)
         #print("\n".join(r) )
+    return output
 
 
+def scrub(output,mpoints,devs):
+    print("D... SCRUB","_"*30)
     # ------------scrub------------------
     output.append("######## BTRFS SCRUB ######")
+    if len(mpoints)==0:
+        print("X... no mountpoints for scrub")
+        return output
+    if len(devs)==0:
+        print("X... no devs        for scrub")
+        return output
      #=========== ERRORCHECK
     for i in range(len(mpoints)):
         output.append("===={}====".format(devs[i]) )
         CMD='sudo btrfs scrub start -Bd -c 3 '+mpoints[i]
         r  ="no scrub happened"
         try:
             r=sp.check_output(CMD.split()).decode("utf8").strip().split("\n")
@@ -161,17 +222,21 @@
     rhost="?"
     user="?"
 
     #r=sp.check_output( "/usr/local/bin/btrfs.sh" ).decode("utf8")
     #r=r.split("\n")
     #print(r)
     #out="\n".join(r)
-    out=btrfssh()
+
+    out,mountpoints,devs = btrfssh()
+    out = smartctl(out)
+    out = scrub(out, mountpoints,devs)
+
     out="\n".join(out)
-    print(out)
+    print("D...","_"*40)
 
     # out=out.replace("\t"," ")
     # out=out.replace("_","\_")
     # out=out.replace("total=","T=")
     # out=out.replace("used=","U=")
     # out=out.replace(".00GiB","G")
     # out=out.replace(".00MiB","M")
@@ -188,14 +253,15 @@
     # out=out.replace("devid","#")
     # out=out.replace("path","")
     # out=out.replace("size","")
     # out=out.replace("used","u:")
 
 
     #bot_send( "@"+host+": "+out)
+    print(out)
     if tele:
         print("D... SENDING TELEGRAM BOT")
         telegram.bot_send("Btrfs", "@"+host+": "+out)
 
     with open(logfile,"a") as f:
         f.write(user+host+rhost+"FINALE===============\n")
```

### Comparing `notifator-0.2.8/bin/login-notify.py` & `notifator-0.2.9/bin/login-notify.py`

 * *Files identical despite different names*

### Comparing `notifator-0.2.8/bin/notifator` & `notifator-0.2.9/bin/notifator`

 * *Files identical despite different names*

### Comparing `notifator-0.2.8/bin/teleg_bot.py` & `notifator-0.2.9/bin/teleg_bot.py`

 * *Files identical despite different names*

### Comparing `notifator-0.2.8/notifator/notify.py` & `notifator-0.2.9/notifator/notify.py`

 * *Files identical despite different names*

### Comparing `notifator-0.2.8/notifator/notihat.py` & `notifator-0.2.9/notifator/notihat.py`

 * *Files identical despite different names*

### Comparing `notifator-0.2.8/notifator/telegram.py` & `notifator-0.2.9/notifator/telegram.py`

 * *Files identical despite different names*

### Comparing `notifator-0.2.8/notifator.egg-info/PKG-INFO` & `notifator-0.2.9/notifator.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notifator
-Version: 0.2.8
+Version: 0.2.9
 Summary: Automatically created environment for python package
 Home-page: UNKNOWN
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description: # Project: notifator
```

### Comparing `notifator-0.2.8/setup.py` & `notifator-0.2.9/setup.py`

 * *Files identical despite different names*

