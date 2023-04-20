# Comparing `tmp/wcommon-1.3.8.tar.gz` & `tmp/wcommon-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wcommon-1.3.8.tar", last modified: Mon Feb 27 09:52:10 2023, max compression
+gzip compressed data, was "wcommon-1.5.1.tar", last modified: Thu Apr 20 05:49:05 2023, max compression
```

## Comparing `wcommon-1.3.8.tar` & `wcommon-1.5.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2023-02-27 09:52:10.187886 wcommon-1.3.8/
--rw-r--r--   0 wangjunbo   (502) staff       (20)     1725 2023-02-27 09:52:10.187522 wcommon-1.3.8/PKG-INFO
--rw-r--r--   0 wangjunbo   (502) staff       (20)     1331 2023-02-27 09:51:48.000000 wcommon-1.3.8/README.md
--rw-r--r--   0 wangjunbo   (502) staff       (20)       38 2023-02-27 09:52:10.188022 wcommon-1.3.8/setup.cfg
--rw-r--r--   0 wangjunbo   (502) staff       (20)     1400 2023-02-27 09:48:39.000000 wcommon-1.3.8/setup.py
-drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2023-02-27 09:52:10.182530 wcommon-1.3.8/wcommon/
--rw-r--r--   0 wangjunbo   (502) staff       (20)    23389 2023-02-27 09:47:17.000000 wcommon-1.3.8/wcommon/__init__.py
-drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2023-02-27 09:52:10.186917 wcommon-1.3.8/wcommon.egg-info/
--rw-r--r--   0 wangjunbo   (502) staff       (20)     1725 2023-02-27 09:52:09.000000 wcommon-1.3.8/wcommon.egg-info/PKG-INFO
--rw-r--r--   0 wangjunbo   (502) staff       (20)      192 2023-02-27 09:52:09.000000 wcommon-1.3.8/wcommon.egg-info/SOURCES.txt
--rw-r--r--   0 wangjunbo   (502) staff       (20)        1 2023-02-27 09:52:09.000000 wcommon-1.3.8/wcommon.egg-info/dependency_links.txt
--rw-r--r--   0 wangjunbo   (502) staff       (20)       37 2023-02-27 09:52:09.000000 wcommon-1.3.8/wcommon.egg-info/requires.txt
--rw-r--r--   0 wangjunbo   (502) staff       (20)        8 2023-02-27 09:52:09.000000 wcommon-1.3.8/wcommon.egg-info/top_level.txt
+drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2023-04-20 05:49:05.039326 wcommon-1.5.1/
+-rw-r--r--   0 wangjunbo   (502) staff       (20)     1725 2023-04-20 05:49:05.039050 wcommon-1.5.1/PKG-INFO
+-rw-r--r--   0 wangjunbo   (502) staff       (20)     1331 2023-02-27 09:51:48.000000 wcommon-1.5.1/README.md
+-rw-r--r--   0 wangjunbo   (502) staff       (20)       38 2023-04-20 05:49:05.039493 wcommon-1.5.1/setup.cfg
+-rw-r--r--   0 wangjunbo   (502) staff       (20)     1400 2023-04-20 05:48:43.000000 wcommon-1.5.1/setup.py
+drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2023-04-20 05:49:05.036929 wcommon-1.5.1/wcommon/
+-rw-r--r--   0 wangjunbo   (502) staff       (20)    24125 2023-04-20 05:48:12.000000 wcommon-1.5.1/wcommon/__init__.py
+drwxr-xr-x   0 wangjunbo   (502) staff       (20)        0 2023-04-20 05:49:05.038661 wcommon-1.5.1/wcommon.egg-info/
+-rw-r--r--   0 wangjunbo   (502) staff       (20)     1725 2023-04-20 05:49:04.000000 wcommon-1.5.1/wcommon.egg-info/PKG-INFO
+-rw-r--r--   0 wangjunbo   (502) staff       (20)      192 2023-04-20 05:49:04.000000 wcommon-1.5.1/wcommon.egg-info/SOURCES.txt
+-rw-r--r--   0 wangjunbo   (502) staff       (20)        1 2023-04-20 05:49:04.000000 wcommon-1.5.1/wcommon.egg-info/dependency_links.txt
+-rw-r--r--   0 wangjunbo   (502) staff       (20)       37 2023-04-20 05:49:04.000000 wcommon-1.5.1/wcommon.egg-info/requires.txt
+-rw-r--r--   0 wangjunbo   (502) staff       (20)        8 2023-04-20 05:49:04.000000 wcommon-1.5.1/wcommon.egg-info/top_level.txt
```

### Comparing `wcommon-1.3.8/PKG-INFO` & `wcommon-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcommon
-Version: 1.3.8
+Version: 1.5.1
 Summary: 常用工具类方法集合
 Home-page: http://www.hohode.com
 Author: WangJunbo
 Author-email: wjbhnu@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wcommon-1.3.8/README.md` & `wcommon-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `wcommon-1.3.8/setup.py` & `wcommon-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     # 项目的名称 一般在同级目录中有个同名的文件夹
     name="wcommon",
     # 项目的版本
-    version="1.3.8",
+    version="1.5.1",
     # 项目的作者
     author="WangJunbo",
     # 作者的邮箱
     author_email="wjbhnu@gmail.com",
     # 项目描述
     description="常用工具类方法集合",
     # 项目的长描述
```

### Comparing `wcommon-1.3.8/wcommon/__init__.py` & `wcommon-1.5.1/wcommon/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import warnings
 
 # from Crypto.Cipher import AES
 # from binascii import b2a_hex
 
 # reload(sys)
 # sys.setdefaultencoding('utf8')
-# print("WARN:please configuration the configuraion_file variable")
+# logger.info("WARN:please configuration the configuraion_file variable")
 
 configuration_file = "/data/apps/public/conf.ini"
 configuration_path_prefix = "/data"
 system = platform.system()
 if system == "Darwin":
     configuration_path_prefix = os.path.expanduser("~")
 configuration_file = "{}/apps/public/conf.ini".format(configuration_path_prefix)
@@ -41,15 +41,15 @@
     warnings.warn("此方法已废弃，不推荐使用，请使用 command 替换。", DeprecationWarning)
     return command(cmd)
 
 
 def get_config(config_file=None):
     if config_file is None:
         config_file = configuration_file
-    print(configuration_file)
+    logger.info(configuration_file)
     import configparser
     config = configparser.ConfigParser()
     config.read(config_file)
     return config
 
 
 # for python2
@@ -134,50 +134,50 @@
     handler_id = logger.add(sys.stderr, level=level)
     return handler_id
 
 
 def parseCommandArguments(args):
     arg_dict = {}
     for argument in args:
-        print("argument:" + argument)
+        logger.debug("argument:" + argument)
         if argument.startswith("-D"):
             arg = argument[2:]
 
             idx = arg.find("=")
 
             k = arg[0:idx]
             v = arg[idx + 1:]
             arg_dict[k] = v
     return arg_dict
 
 
 def wait_until(future_timestamp):
-    print("futureTimestamp %s " % future_timestamp)
+    logger.debug("futureTimestamp %s " % future_timestamp)
 
     now = datetime_tool.datetime.now()
     now_timestamp = timestamp(now)
 
-    print("nowTimestamp %s " % now_timestamp)
+    logger.debug("nowTimestamp %s " % now_timestamp)
 
     if now_timestamp < future_timestamp:
         d = future_timestamp - now_timestamp
         timetool.sleep(d)
 
 
 # 获取redisCluster的对象
 # def getRedisCluster(redisClusterStr):
 #     from rediscluster import StrictRedisCluster
-#     print(redisClusterStr)
+#     logger.debug(redisClusterStr)
 #     redisCluster = []
 #     for nodePort in redisClusterStr.split(","):
 #         kv = nodePort.split(":")
 #         node = {"host": kv[0], "port": kv[1]}
 #         redisCluster.append(node)
 #
-#     print(redisCluster)
+#     logger.debug(redisCluster)
 #     rc = StrictRedisCluster(startup_nodes=redisCluster, decode_responses=True)
 #     return rc
 
 # mysql some operations
 def getDatabase(section="mysql"):
     try:
         import configparser
@@ -192,71 +192,75 @@
         charset = config.get(section, "charset")
 
         db = pymysql.connect(host=host, port=port, user=user, passwd=password, db=database, charset=charset,
                              autocommit=True,
                              cursorclass=pymysql.cursors.DictCursor)
         return db
     except ImportError:
-        print("Error: configparser or pymysql module not exists")
+        logger.error("Error: configparser or pymysql module not exists")
     except Exception as e:
         logger.error(e)
         traceback.print_exc()
 
     return None
 
 
-def query(database, sql, argumentTuple=(), timestamp2str=True, debug=True):
+def query(database, sql, argumentTuple=(), timestamp2str=True):
     import pymysql
     cursor = database.cursor()
-    if debug:
-        print("query sql:\t%s, arguments: %s" % (sql, argumentTuple))
+    logger.debug("query sql:\t%s, arguments: %s" % (sql, argumentTuple))
     if len(argumentTuple) == 0:
         cursor.execute(sql)
     else:
         cursor.execute(sql, argumentTuple)
     rows = []
 
     if timestamp2str:
         timestamp_field_array = []
+        date_field_array = []
         for tp in cursor.description:
             if tp[1] == pymysql.constants.FIELD_TYPE.TIMESTAMP or tp[1] == pymysql.constants.FIELD_TYPE.DATETIME:
                 timestamp_field_array.append(tp[0])
+            elif tp[1] == pymysql.constants.FIELD_TYPE.DATE:
+                date_field_array.append(tp[0])
 
         for row in cursor:
             for field in timestamp_field_array:
                 if row[field] is not None:
                     tmp_value = row[field].strftime("%Y-%m-%d %H:%M:%S")
                     row[field] = tmp_value
-                else:
-                    row[field] = ""
+
+            for field in date_field_array:
+                if row[field] is not None:
+                    tmp_value = row[field].strftime("%Y-%m-%d")
+                    row[field] = tmp_value
             rows.append(row)
     else:
         for row in cursor:
             rows.append(row)
     return rows
 
 
-def insert(database, tableName, dic, commit=True, debug=True):
+def insert(database, tableName, dic, commit=True):
     cursor = database.cursor()
     cols = []
     vals = []
     placeholders = []
     doc_id = ""
     for key in dic.keys():
         val = dic[key]
         if val is not None:
             cols.append(key)
             placeholders.append("%s")
             vals.append(val)
     insert_sql = "INSERT INTO " + tableName + " ( %s ) VALUES ( %s )" % (",".join(cols), ",".join(placeholders))
-    if debug:
-        print(insert_sql)
+    logger.debug(insert_sql)
 
     if commit:
-        print(tuple(vals))
+        logger.info(tuple(vals))
         cursor.execute(insert_sql, tuple(vals))
         doc_id = cursor.lastrowid
     if commit:
         database.commit()
 
     return doc_id
 
@@ -269,36 +273,35 @@
         val = dic[key]
         if val is not None:
             placeholders.append("{} = %s ".format(key))
             vals.append(val)
     setting = " , ".join(placeholders)
     vals.append(id)
     update_sql = "update {0} set {1} where {2} = %s ".format(tableName, setting, idFieldName)
-    print(update_sql)
+    logger.debug(update_sql)
 
     if commit:
-        print(tuple(vals))
+        logger.debug(tuple(vals))
         cursor.execute(update_sql, tuple(vals))
     if commit:
         database.commit()
 
 
-def execute(database, sql, argumentTuple=(), debug=True):
+def execute(database, sql, argumentTuple=()):
     cursor = database.cursor()
-    if debug:
-        print("query sql:\t%s, arguments: %s" % (sql, argumentTuple))
+    logger.debug("query sql:\t%s, arguments: %s" % (sql, argumentTuple))
     if len(argumentTuple) == 0:
         cursor.execute(sql)
     else:
         cursor.execute(sql, argumentTuple)
 
 
 def delete(database, sql, commit=True):
     cursor = database.cursor()
-    print("delete sql:\t" + sql)
+    logger.debug("delete sql:\t" + sql)
     if commit:
         cursor.execute(sql)
         database.commit()
 
 
 def mysql_execute(database, sql, argumentTuple, commit=True):
     cursor = database.cursor()
@@ -479,25 +482,25 @@
 
     Args:
         requirement_list: 依赖包list
     """
     for package in requirement_list:
         try:
             exec("import {0}".format(package))
-            print("Requirement {} already!".format(package))
+            logger.info("Requirement {} already!".format(package))
         except ModuleNotFoundError:
             inquiry = input("This script requires {0}. Do you want to install {0}? [y/n]".format(package))
             while (inquiry != "y") and (inquiry != "n"):
                 inquiry = input("This script requires {0}. Do you want to install {0}? [y/n]".format(package))
             if inquiry == "y":
                 import os
-                print("Execute command: pip3 install {0}".format(package))
+                logger.info("Execute command: pip3 install {0}".format(package))
                 os.system("pip3 install {0}".format(package))
             else:
-                print("{0} is missing, so the program exits!".format(package))
+                logger.info("{0} is missing, so the program exits!".format(package))
                 exit(-1)
 
 
 # reconnecting mysql , 参考 https://www.kingname.info/2017/04/17/decorate-for-method/
 def pingmysql(original_function):
     def wrapper(self, *args, **kwargs):
         try:
@@ -540,15 +543,15 @@
 
             self.database = pymysql.connect(host=host, port=port, user=user, passwd=password,
                                             db=self.default_database_name,
                                             charset=charset, autocommit=True,
                                             cursorclass=pymysql.cursors.DictCursor)
 
         except ImportError:
-            print("Error: configparser or pymysql module not exists")
+            logger.error("Error: configparser or pymysql module not exists")
         except Exception as e:
             logger.error(e)
             traceback.print_exc()
 
     def is_legal_value(self, table_name, column_name, val):
         if val is None:
             return True
@@ -583,25 +586,35 @@
             cursor.execute(sql)
         else:
             cursor.execute(sql, argumentTuple)
         rows = []
 
         if timestamp2str:
             timestamp_field_array = []
+            date_field_array = []
             for tp in cursor.description:
                 if tp[1] == pymysql.constants.FIELD_TYPE.TIMESTAMP or tp[1] == pymysql.constants.FIELD_TYPE.DATETIME:
                     timestamp_field_array.append(tp[0])
+                elif tp[1] == pymysql.constants.FIELD_TYPE.DATE:
+                    date_field_array.append(tp[0])
 
             for row in cursor:
                 for field in timestamp_field_array:
-                    if row[field] is not None:
+                    if row[field] is None:
+                        row[field] = ""
+                    else:
                         tmp_value = row[field].strftime("%Y-%m-%d %H:%M:%S")
                         row[field] = tmp_value
-                    else:
+
+                for field in date_field_array:
+                    if row[field] is None:
                         row[field] = ""
+                    else:
+                        tmp_value = row[field].strftime("%Y-%m-%d")
+                        row[field] = tmp_value
                 rows.append(row)
         else:
             for row in cursor:
                 rows.append(row)
         return rows
 
     @pingmysql
@@ -718,13 +731,13 @@
         values_array = []
         for row in data:
             tmp_ar = []
             for i in field_array:
                 val = row.get(i)
                 tmp_ar.append(val)
             values_array.append(tmp_ar)
-        print(values_array)
+        logger.debug(values_array)
         cursor = self.database.cursor()
         for start in range(0, len(values_array), batch_size):
             logger.debug(values_array[start:start + batch_size])
             cursor.executemany(ql, values_array[start:start + batch_size])
             self.database.commit()
```

### Comparing `wcommon-1.3.8/wcommon.egg-info/PKG-INFO` & `wcommon-1.5.1/wcommon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wcommon
-Version: 1.3.8
+Version: 1.5.1
 Summary: 常用工具类方法集合
 Home-page: http://www.hohode.com
 Author: WangJunbo
 Author-email: wjbhnu@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

