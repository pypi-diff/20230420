# Comparing `tmp/DigitalizationTools-0.2.6.tar.gz` & `tmp/DigitalizationTools-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DigitalizationTools-0.2.6.tar", last modified: Sun Feb 12 10:13:18 2023, max compression
+gzip compressed data, was "DigitalizationTools-0.2.7.tar", last modified: Fri Feb 24 12:11:26 2023, max compression
```

## Comparing `DigitalizationTools-0.2.6.tar` & `DigitalizationTools-0.2.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mklu       (501) staff       (20)        0 2023-02-12 10:13:18.925898 DigitalizationTools-0.2.6/
-drwxr-xr-x   0 mklu       (501) staff       (20)        0 2023-02-12 10:13:18.924864 DigitalizationTools-0.2.6/DigitalizationTools/
--rw-r--r--   0 mklu       (501) staff       (20)        0 2023-01-16 22:42:59.000000 DigitalizationTools-0.2.6/DigitalizationTools/__init__.py
--rw-r--r--   0 mklu       (501) staff       (20)    14545 2023-02-11 14:22:47.000000 DigitalizationTools-0.2.6/DigitalizationTools/components.py
--rw-r--r--   0 mklu       (501) staff       (20)     6317 2023-02-12 10:12:13.000000 DigitalizationTools-0.2.6/DigitalizationTools/mongodb_api.py
--rw-r--r--   0 mklu       (501) staff       (20)     9371 2023-02-12 10:08:34.000000 DigitalizationTools-0.2.6/DigitalizationTools/postgresql_api.py
--rw-r--r--   0 mklu       (501) staff       (20)     5460 2023-02-12 10:12:39.000000 DigitalizationTools-0.2.6/DigitalizationTools/sqlite3_api.py
-drwxr-xr-x   0 mklu       (501) staff       (20)        0 2023-02-12 10:13:18.925573 DigitalizationTools-0.2.6/DigitalizationTools.egg-info/
--rw-r--r--   0 mklu       (501) staff       (20)      681 2023-02-12 10:13:18.000000 DigitalizationTools-0.2.6/DigitalizationTools.egg-info/PKG-INFO
--rw-r--r--   0 mklu       (501) staff       (20)      377 2023-02-12 10:13:18.000000 DigitalizationTools-0.2.6/DigitalizationTools.egg-info/SOURCES.txt
--rw-r--r--   0 mklu       (501) staff       (20)        1 2023-02-12 10:13:18.000000 DigitalizationTools-0.2.6/DigitalizationTools.egg-info/dependency_links.txt
--rw-r--r--   0 mklu       (501) staff       (20)       20 2023-02-12 10:13:18.000000 DigitalizationTools-0.2.6/DigitalizationTools.egg-info/top_level.txt
--rw-r--r--   0 mklu       (501) staff       (20)     1065 2023-01-16 22:45:35.000000 DigitalizationTools-0.2.6/LICENSE
--rw-r--r--   0 mklu       (501) staff       (20)      681 2023-02-12 10:13:18.925769 DigitalizationTools-0.2.6/PKG-INFO
--rw-r--r--   0 mklu       (501) staff       (20)      103 2023-01-16 22:45:42.000000 DigitalizationTools-0.2.6/pyproject.toml
--rw-r--r--   0 mklu       (501) staff       (20)       38 2023-02-12 10:13:18.925938 DigitalizationTools-0.2.6/setup.cfg
--rw-r--r--   0 mklu       (501) staff       (20)      860 2023-02-12 10:12:41.000000 DigitalizationTools-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-24 12:11:26.525060 DigitalizationTools-0.2.7/
+drwxrwxrwx   0        0        0        0 2023-02-24 12:11:26.500060 DigitalizationTools-0.2.7/DigitalizationTools/
+-rw-rw-rw-   0        0        0        0 2023-01-17 08:16:10.000000 DigitalizationTools-0.2.7/DigitalizationTools/__init__.py
+-rw-rw-rw-   0        0        0    14929 2023-02-09 15:28:36.000000 DigitalizationTools-0.2.7/DigitalizationTools/components.py
+-rw-rw-rw-   0        0        0     6751 2023-02-24 12:07:41.000000 DigitalizationTools-0.2.7/DigitalizationTools/mongodb_api.py
+-rw-rw-rw-   0        0        0     9625 2023-02-12 15:35:49.000000 DigitalizationTools-0.2.7/DigitalizationTools/postgresql_api.py
+-rw-rw-rw-   0        0        0     5625 2023-01-18 08:04:02.000000 DigitalizationTools-0.2.7/DigitalizationTools/sqlite3_api.py
+drwxrwxrwx   0        0        0        0 2023-02-24 12:11:26.518059 DigitalizationTools-0.2.7/DigitalizationTools.egg-info/
+-rw-rw-rw-   0        0        0      698 2023-02-24 12:11:26.000000 DigitalizationTools-0.2.7/DigitalizationTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2023-02-24 12:11:26.000000 DigitalizationTools-0.2.7/DigitalizationTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-24 12:11:26.000000 DigitalizationTools-0.2.7/DigitalizationTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-02-24 12:11:26.000000 DigitalizationTools-0.2.7/DigitalizationTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2023-01-17 08:16:10.000000 DigitalizationTools-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0      698 2023-02-24 12:11:26.524058 DigitalizationTools-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2023-01-17 08:16:10.000000 DigitalizationTools-0.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-02-24 12:11:26.526062 DigitalizationTools-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      887 2023-02-24 12:10:37.000000 DigitalizationTools-0.2.7/setup.py
```

### Comparing `DigitalizationTools-0.2.6/DigitalizationTools/postgresql_api.py` & `DigitalizationTools-0.2.7/DigitalizationTools/postgresql_api.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,255 +1,255 @@
-import psycopg2
-from datetime import datetime
-import secrets
-import pandas as pd
-from beartype import beartype
-from typing import Optional, Union
-
-
-# sql_pass = "g5XSmIEJesgmR9uKvhdD"
-
-
-class database:
-    @beartype
-    def __init__(self, hostName:str, databaseName:str, userName:str, sqlPasswords:str):
-        self.hostName     = hostName
-        self.databaseName = databaseName
-        self.userName     = userName
-        self.sqlPasswords = sqlPasswords
-    
-    def get_table(self):
-        try:
-            conn = psycopg2.connect(host=self.hostName,database=self.databaseName,user=self.userName, password=self.sqlPasswords)
-            cur = conn.cursor()
-            cur.execute("SELECT table_name FROM information_schema.tables WHERE table_schema='public' AND table_type='BASE TABLE';")
-            tables = cur.fetchall()
-            columnsName = [i[0] for i in cur.description]
-            conn.commit()
-            conn.close()
-            df_tables = pd.DataFrame(tables, columns=columnsName)
-            return df_tables
-        except psycopg2.Error as err:
-            return err
-
-
-class databaseTable(database):
-    
-    @beartype
-    def __init__(self, hostName:str, databaseName:str, userName:str, sqlPasswords:str, tableName:str):
-        super().__init__(hostName, databaseName, userName, sqlPasswords)
-        self.tableName  = tableName
-    
-    @beartype
-    def create_table(self, keys:list, datatype:list):
-        """
-        keys: column names ["name1", "name2", ...]
-        datatype: type of columns ["text", "float", ...]
-        """
-        try:
-            conn = psycopg2.connect(host=self.hostName,database=self.databaseName,user=self.userName, password=self.sqlPasswords)
-            cur = conn.cursor()
-            # create table
-            create_table_sql = "CREATE TABLE IF NOT EXISTS {} ".format(self.tableName)
-            keys_datatype = [f"{keys[i]} {datatype[i]}," for i in range(len(keys))]
-            create_table_sql = create_table_sql + \
-                                "({} id text, date text);".format("".join(keys_datatype))
-            cur.execute(create_table_sql)
-            conn.commit()
-            conn.close()
-            self.keys = keys
-            self.datatype = datatype
-            return True
-        except psycopg2.Error as err:
-            return err
-    
-    @beartype
-    def insert_one_row(self, insert_data:list, with_id:Optional[bool]=False):
-        """
-        if with_id = True, 'id' should be the last element in 'insert_data'
-        """
-        try:
-            conn = psycopg2.connect(host=self.hostName,database=self.databaseName,user=self.userName, password=self.sqlPasswords)
-            cur  = conn.cursor()        
-            sql = "SELECT * FROM {};".format(self.tableName)
-            cur.execute(sql)
-            keys = [i[0] for i in cur.description][0:-2]
-            # insert data
-            qs = ",".join(["%s" for _ in range(len(keys)+2)])
-            insert = """INSERT INTO {} ({},id,date) 
-                    VALUES ({})""".format(self.tableName, ",".join(keys), qs)
-            # check if id is specified
-            if with_id: # true
-                insert_data.append(str(datetime.now())[0:19])
-            else: # false, no id specified
-                insert_data.append(secrets.token_hex(16))
-                insert_data.append(str(datetime.now())[0:19])
-            cur.execute(insert, tuple(insert_data))
-            conn.commit()
-            conn.close()
-            return True
-        except psycopg2.Error as err:
-            return err
-    
-    @beartype
-    def insert_multiple_rows(self, insert_df:pd.DataFrame): 
-        """
-        insert_data: list of lists, e.g.: [[1,2,3], [1,2,3]]
-        """
-        try:
-            conn = psycopg2.connect(host=self.hostName,database=self.databaseName,user=self.userName, password=self.sqlPasswords)
-            cur  = conn.cursor()        
-            sql = "SELECT * FROM {};".format(self.tableName)
-            cur.execute(sql)
-            keys = [i[0] for i in cur.description][0:-2]
-            # insert data
-            qs = ",".join(["%s" for _ in range(len(keys)+2)])
-            insert = """INSERT INTO {} ({},id,date) 
-                    VALUES ({})""".format(self.tableName, ",".join(keys), qs)
-            
-            id                 = secrets.token_hex(16)
-            date               = str(datetime.now())[0:19]
-            len_of_df          = len(insert_df)
-            insert_df["id"]    = [id for i in range(len_of_df)]
-            insert_df["date"]  = [date for i in range(len_of_df)]
-
-            sql_insert_data = []
-            for i in range(len(insert_df)):
-                sql_insert_data.append(tuple(insert_df.iloc[i].to_list()))
-
-            cur.executemany(insert, sql_insert_data)
-            conn.commit()
-            conn.close()
-            return True
-        except psycopg2.Error as err:
-            return err
-    
-    def get_all(self):
-        """
-        get all rows in table
-        """
-        try:
-            conn = psycopg2.connect(host=self.hostName,database=self.databaseName,user=self.userName, password=self.sqlPasswords)
-            cur = conn.cursor()
-            sql = "SELECT * FROM {};".format(self.tableName)
-            cur.execute(sql)
-            # get all rows
-            rows = cur.fetchall()
-            # keys
-            columnsName = [i[0] for i in cur.description]
-            conn.commit()
-            conn.close()
-            return pd.DataFrame(rows, columns=columnsName)
-        except psycopg2.Error as err:
-            return err
-    
-    @beartype
-    def get_one_row(self, id:str):
-        """
-        get one row based on id
-        """
-        try:
-            conn = psycopg2.connect(host=self.hostName,database=self.databaseName,user=self.userName, password=self.sqlPasswords)
-            cur = conn.cursor()
-            sql_select = "SELECT * FROM {} WHERE id=%s".format(self.tableName)
-            cur.execute(sql_select, (id,))
-            rows = cur.fetchone()
-            columnsName = [i[0] for i in cur.description]
-            conn.commit()
-            conn.close()
-            return pd.DataFrame([rows], columns=columnsName)
-        except psycopg2.Error as err:
-            return err
-
-    @beartype
-    def get_columns(self, columnNames:list):
-        """
-        get all columns based on the given column names,
-        columnNames = ["name1", "name2", ...]
-        """
-        if columnNames == []:
-            return "No column specified"
-        try:
-            df = self.get_all()
-            return df.loc[:, columnNames]
-        except psycopg2.Error as err:
-            return err
-    
-    @beartype
-    def delete_one_row(self, id:str):
-        """
-        delete one row from table
-        """
-        try:
-            conn = psycopg2.connect(host=self.hostName,database=self.databaseName,user=self.userName, password=self.sqlPasswords)
-            cur = conn.cursor()
-            sql_delete = 'DELETE FROM {} WHERE id=%s'.format(self.tableName)
-            cur.execute(sql_delete, (id,))  
-            conn.commit()
-            conn.close()
-            return True
-        except psycopg2.Error as err:
-            return err
-    
-    @beartype
-    def update_one_row(self, id:str, update_data:list):
-        """
-        update the whole row in table
-        """
-        try:
-            df = self.get_columns(["id"])
-            if id in df["id"].to_list():
-                # delete
-                self.delete_one_row(id)
-                # insert
-                update_data.append(id)
-                self.insert_one_row(insert_data=update_data, with_id=True)
-                return True
-            else:
-                return "no id matching."
-        except psycopg2.Error as err:
-            return err
-    
-    @beartype
-    def update_elements(self, id:str, update_dict=dict):
-        """
-        update_dict = {"text": text, "list": [1,2,3] }
-        """
-        keys    = tuple(update_dict.keys())
-        values  = tuple(update_dict.values()) 
-        try:
-            # get all ids in table
-            df = self.get_columns(["id"])
-            if id not in df["id"].to_list():
-                return "id does not exist..."
-            if len(values) > 1:
-                keys_s  = f"{keys}".replace("'", '')
-                sql = f"""UPDATE {self.tableName} SET {keys_s} = {values} WHERE id = '{id}';"""
-            else:
-
-                sql = f"""UPDATE {self.tableName} SET {keys[0]} = '{values[0]}' WHERE id = '{id}';"""
-
-            conn = psycopg2.connect(host=self.hostName,database=self.databaseName,user=self.userName, password=self.sqlPasswords)
-            cur = conn.cursor()
-            
-            cur.execute(sql)
-            conn.commit()
-            conn.close()
-            return True
-        except psycopg2.Error as err:
-            return err
-        
-
-    def delete_all_rows(self):
-        """
-        delete all rows from table
-        """
-        try:
-            conn = psycopg2.connect(host=self.hostName,database=self.databaseName,user=self.userName, password=self.sqlPasswords)
-            cur = conn.cursor()
-            sql_delete = 'DELETE FROM {};'.format(self.tableName)
-            cur.execute(sql_delete)  
-            conn.commit()
-            conn.close()
-            return True
-        except psycopg2.Error as err:
+import psycopg2
+from datetime import datetime
+import secrets
+import pandas as pd
+from beartype import beartype
+from typing import Optional, Union
+
+
+# sql_pass = "g5XSmIEJesgmR9uKvhdD"
+
+
+class database:
+    @beartype
+    def __init__(self, hostName:str, databaseName:str, userName:str, sqlPasswords:str):
+        self.hostName     = hostName
+        self.databaseName = databaseName
+        self.userName     = userName
+        self.sqlPasswords = sqlPasswords
+    
+    def get_table(self):
+        try:
+            conn = psycopg2.connect(host=self.hostName,database=self.databaseName,user=self.userName, password=self.sqlPasswords)
+            cur = conn.cursor()
+            cur.execute("SELECT table_name FROM information_schema.tables WHERE table_schema='public' AND table_type='BASE TABLE';")
+            tables = cur.fetchall()
+            columnsName = [i[0] for i in cur.description]
+            conn.commit()
+            conn.close()
+            df_tables = pd.DataFrame(tables, columns=columnsName)
+            return df_tables
+        except psycopg2.Error as err:
+            return err
+
+
+class databaseTable(database):
+    
+    @beartype
+    def __init__(self, hostName:str, databaseName:str, userName:str, sqlPasswords:str, tableName:str):
+        super().__init__(hostName, databaseName, userName, sqlPasswords)
+        self.tableName  = tableName
+    
+    @beartype
+    def create_table(self, keys:list, datatype:list):
+        """
+        keys: column names ["name1", "name2", ...]
+        datatype: type of columns ["text", "float", ...]
+        """
+        try:
+            conn = psycopg2.connect(host=self.hostName,database=self.databaseName,user=self.userName, password=self.sqlPasswords)
+            cur = conn.cursor()
+            # create table
+            create_table_sql = "CREATE TABLE IF NOT EXISTS {} ".format(self.tableName)
+            keys_datatype = [f"{keys[i]} {datatype[i]}," for i in range(len(keys))]
+            create_table_sql = create_table_sql + \
+                                "({} id text, date text);".format("".join(keys_datatype))
+            cur.execute(create_table_sql)
+            conn.commit()
+            conn.close()
+            self.keys = keys
+            self.datatype = datatype
+            return True
+        except psycopg2.Error as err:
+            return err
+    
+    @beartype
+    def insert_one_row(self, insert_data:list, with_id:Optional[bool]=False):
+        """
+        if with_id = True, 'id' should be the last element in 'insert_data'
+        """
+        try:
+            conn = psycopg2.connect(host=self.hostName,database=self.databaseName,user=self.userName, password=self.sqlPasswords)
+            cur  = conn.cursor()        
+            sql = "SELECT * FROM {};".format(self.tableName)
+            cur.execute(sql)
+            keys = [i[0] for i in cur.description][0:-2]
+            # insert data
+            qs = ",".join(["%s" for _ in range(len(keys)+2)])
+            insert = """INSERT INTO {} ({},id,date) 
+                    VALUES ({})""".format(self.tableName, ",".join(keys), qs)
+            # check if id is specified
+            if with_id: # true
+                insert_data.append(str(datetime.now())[0:19])
+            else: # false, no id specified
+                insert_data.append(secrets.token_hex(16))
+                insert_data.append(str(datetime.now())[0:19])
+            cur.execute(insert, tuple(insert_data))
+            conn.commit()
+            conn.close()
+            return True
+        except psycopg2.Error as err:
+            return err
+    
+    @beartype
+    def insert_multiple_rows(self, insert_df:pd.DataFrame): 
+        """
+        insert_data: list of lists, e.g.: [[1,2,3], [1,2,3]]
+        """
+        try:
+            conn = psycopg2.connect(host=self.hostName,database=self.databaseName,user=self.userName, password=self.sqlPasswords)
+            cur  = conn.cursor()        
+            sql = "SELECT * FROM {};".format(self.tableName)
+            cur.execute(sql)
+            keys = [i[0] for i in cur.description][0:-2]
+            # insert data
+            qs = ",".join(["%s" for _ in range(len(keys)+2)])
+            insert = """INSERT INTO {} ({},id,date) 
+                    VALUES ({})""".format(self.tableName, ",".join(keys), qs)
+            
+            id                 = secrets.token_hex(16)
+            date               = str(datetime.now())[0:19]
+            len_of_df          = len(insert_df)
+            insert_df["id"]    = [id for i in range(len_of_df)]
+            insert_df["date"]  = [date for i in range(len_of_df)]
+
+            sql_insert_data = []
+            for i in range(len(insert_df)):
+                sql_insert_data.append(tuple(insert_df.iloc[i].to_list()))
+
+            cur.executemany(insert, sql_insert_data)
+            conn.commit()
+            conn.close()
+            return True
+        except psycopg2.Error as err:
+            return err
+    
+    def get_all(self):
+        """
+        get all rows in table
+        """
+        try:
+            conn = psycopg2.connect(host=self.hostName,database=self.databaseName,user=self.userName, password=self.sqlPasswords)
+            cur = conn.cursor()
+            sql = "SELECT * FROM {};".format(self.tableName)
+            cur.execute(sql)
+            # get all rows
+            rows = cur.fetchall()
+            # keys
+            columnsName = [i[0] for i in cur.description]
+            conn.commit()
+            conn.close()
+            return pd.DataFrame(rows, columns=columnsName)
+        except psycopg2.Error as err:
+            return err
+    
+    @beartype
+    def get_one_row(self, id:str):
+        """
+        get one row based on id
+        """
+        try:
+            conn = psycopg2.connect(host=self.hostName,database=self.databaseName,user=self.userName, password=self.sqlPasswords)
+            cur = conn.cursor()
+            sql_select = "SELECT * FROM {} WHERE id=%s".format(self.tableName)
+            cur.execute(sql_select, (id,))
+            rows = cur.fetchone()
+            columnsName = [i[0] for i in cur.description]
+            conn.commit()
+            conn.close()
+            return pd.DataFrame([rows], columns=columnsName)
+        except psycopg2.Error as err:
+            return err
+
+    @beartype
+    def get_columns(self, columnNames:list):
+        """
+        get all columns based on the given column names,
+        columnNames = ["name1", "name2", ...]
+        """
+        if columnNames == []:
+            return "No column specified"
+        try:
+            df = self.get_all()
+            return df.loc[:, columnNames]
+        except psycopg2.Error as err:
+            return err
+    
+    @beartype
+    def delete_one_row(self, id:str):
+        """
+        delete one row from table
+        """
+        try:
+            conn = psycopg2.connect(host=self.hostName,database=self.databaseName,user=self.userName, password=self.sqlPasswords)
+            cur = conn.cursor()
+            sql_delete = 'DELETE FROM {} WHERE id=%s'.format(self.tableName)
+            cur.execute(sql_delete, (id,))  
+            conn.commit()
+            conn.close()
+            return True
+        except psycopg2.Error as err:
+            return err
+    
+    @beartype
+    def update_one_row(self, id:str, update_data:list):
+        """
+        update the whole row in table
+        """
+        try:
+            df = self.get_columns(["id"])
+            if id in df["id"].to_list():
+                # delete
+                self.delete_one_row(id)
+                # insert
+                update_data.append(id)
+                self.insert_one_row(insert_data=update_data, with_id=True)
+                return True
+            else:
+                return "no id matching."
+        except psycopg2.Error as err:
+            return err
+    
+    @beartype
+    def update_elements(self, id:str, update_dict=dict):
+        """
+        update_dict = {"text": text, "list": [1,2,3] }
+        """
+        keys    = tuple(update_dict.keys())
+        values  = tuple(update_dict.values()) 
+        try:
+            # get all ids in table
+            df = self.get_columns(["id"])
+            if id not in df["id"].to_list():
+                return "id does not exist..."
+            if len(values) > 1:
+                keys_s  = f"{keys}".replace("'", '')
+                sql = f"""UPDATE {self.tableName} SET {keys_s} = {values} WHERE id = '{id}';"""
+            else:
+
+                sql = f"""UPDATE {self.tableName} SET {keys[0]} = '{values[0]}' WHERE id = '{id}';"""
+
+            conn = psycopg2.connect(host=self.hostName,database=self.databaseName,user=self.userName, password=self.sqlPasswords)
+            cur = conn.cursor()
+            
+            cur.execute(sql)
+            conn.commit()
+            conn.close()
+            return True
+        except psycopg2.Error as err:
+            return err
+        
+
+    def delete_all_rows(self):
+        """
+        delete all rows from table
+        """
+        try:
+            conn = psycopg2.connect(host=self.hostName,database=self.databaseName,user=self.userName, password=self.sqlPasswords)
+            cur = conn.cursor()
+            sql_delete = 'DELETE FROM {};'.format(self.tableName)
+            cur.execute(sql_delete)  
+            conn.commit()
+            conn.close()
+            return True
+        except psycopg2.Error as err:
             return err
```

### Comparing `DigitalizationTools-0.2.6/DigitalizationTools.egg-info/PKG-INFO` & `DigitalizationTools-0.2.7/DigitalizationTools.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1
-Name: DigitalizationTools
-Version: 0.2.6
-Summary: A package that manages database through PostgreSQL and creates webapp through Dash plotly.
-Author: Mengke Lu
-Author-email: <mklu0611@gmail.com>
-Keywords: python,postgresql,dash
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-A package that manages database through PostgreSQL and creates webapp through Dash plotly.
+Metadata-Version: 2.1
+Name: DigitalizationTools
+Version: 0.2.7
+Summary: A package that manages database through PostgreSQL and creates webapp through Dash plotly.
+Author: Mengke Lu
+Author-email: <mklu0611@gmail.com>
+Keywords: python,postgresql,dash
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+A package that manages database through PostgreSQL and creates webapp through Dash plotly.
```

### Comparing `DigitalizationTools-0.2.6/PKG-INFO` & `DigitalizationTools-0.2.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1
-Name: DigitalizationTools
-Version: 0.2.6
-Summary: A package that manages database through PostgreSQL and creates webapp through Dash plotly.
-Author: Mengke Lu
-Author-email: <mklu0611@gmail.com>
-Keywords: python,postgresql,dash
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-A package that manages database through PostgreSQL and creates webapp through Dash plotly.
+Metadata-Version: 2.1
+Name: DigitalizationTools
+Version: 0.2.7
+Summary: A package that manages database through PostgreSQL and creates webapp through Dash plotly.
+Author: Mengke Lu
+Author-email: <mklu0611@gmail.com>
+Keywords: python,postgresql,dash
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+A package that manages database through PostgreSQL and creates webapp through Dash plotly.
```

### Comparing `DigitalizationTools-0.2.6/setup.py` & `DigitalizationTools-0.2.7/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,56 @@
-00000000: 0a66 726f 6d20 7365 7475 7074 6f6f 6c73  .from setuptools
-00000010: 2069 6d70 6f72 7420 7365 7475 702c 2066   import setup, f
-00000020: 696e 645f 7061 636b 6167 6573 0a0a 5645  ind_packages..VE
-00000030: 5253 494f 4e20 3d20 2730 2e32 2e36 270a  RSION = '0.2.6'.
-00000040: 4445 5343 5249 5054 494f 4e20 3d20 2741  DESCRIPTION = 'A
-00000050: 2070 6163 6b61 6765 2074 6861 7420 6d61   package that ma
-00000060: 6e61 6765 7320 6461 7461 6261 7365 2074  nages database t
-00000070: 6872 6f75 6768 2050 6f73 7467 7265 5351  hrough PostgreSQ
-00000080: 4c20 616e 6420 6372 6561 7465 7320 7765  L and creates we
-00000090: 6261 7070 2074 6872 6f75 6768 2044 6173  bapp through Das
-000000a0: 6820 706c 6f74 6c79 2e27 0a4c 4f4e 475f  h plotly.'.LONG_
-000000b0: 4445 5343 5249 5054 494f 4e20 3d20 4445  DESCRIPTION = DE
-000000c0: 5343 5249 5054 494f 4e0a 0a23 2053 6574  SCRIPTION..# Set
-000000d0: 7469 6e67 2075 700a 7365 7475 7028 0a20  ting up.setup(. 
-000000e0: 2020 206e 616d 653d 2244 6967 6974 616c     name="Digital
-000000f0: 697a 6174 696f 6e54 6f6f 6c73 222c 0a20  izationTools",. 
-00000100: 2020 2076 6572 7369 6f6e 3d56 4552 5349     version=VERSI
-00000110: 4f4e 2c0a 2020 2020 6175 7468 6f72 3d22  ON,.    author="
-00000120: 4d65 6e67 6b65 204c 7522 2c0a 2020 2020  Mengke Lu",.    
-00000130: 6175 7468 6f72 5f65 6d61 696c 3d22 3c6d  author_email="<m
-00000140: 6b6c 7530 3631 3140 676d 6169 6c2e 636f  klu0611@gmail.co
-00000150: 6d3e 222c 0a20 2020 2064 6573 6372 6970  m>",.    descrip
-00000160: 7469 6f6e 3d20 4445 5343 5249 5054 494f  tion= DESCRIPTIO
-00000170: 4e2c 0a20 2020 206c 6f6e 675f 6465 7363  N,.    long_desc
-00000180: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
-00000190: 7479 7065 3d22 7465 7874 2f6d 6172 6b64  type="text/markd
-000001a0: 6f77 6e22 2c0a 2020 2020 6c6f 6e67 5f64  own",.    long_d
-000001b0: 6573 6372 6970 7469 6f6e 3d4c 4f4e 475f  escription=LONG_
-000001c0: 4445 5343 5249 5054 494f 4e2c 0a20 2020  DESCRIPTION,.   
-000001d0: 2070 6163 6b61 6765 733d 6669 6e64 5f70   packages=find_p
-000001e0: 6163 6b61 6765 7328 292c 0a20 2020 2069  ackages(),.    i
-000001f0: 6e73 7461 6c6c 5f72 6571 7569 7265 733d  nstall_requires=
-00000200: 5b5d 2c0a 2020 2020 6b65 7977 6f72 6473  [],.    keywords
-00000210: 3d5b 2770 7974 686f 6e27 2c20 2770 6f73  =['python', 'pos
-00000220: 7467 7265 7371 6c27 2c20 2764 6173 6827  tgresql', 'dash'
-00000230: 5d2c 0a20 2020 2063 6c61 7373 6966 6965  ],.    classifie
-00000240: 7273 3d5b 0a20 2020 2020 2020 2022 4465  rs=[.        "De
-00000250: 7665 6c6f 706d 656e 7420 5374 6174 7573  velopment Status
-00000260: 203a 3a20 3120 2d20 506c 616e 6e69 6e67   :: 1 - Planning
-00000270: 222c 0a20 2020 2020 2020 2022 496e 7465  ",.        "Inte
-00000280: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
-00000290: 2044 6576 656c 6f70 6572 7322 2c0a 2020   Developers",.  
-000002a0: 2020 2020 2020 2250 726f 6772 616d 6d69        "Programmi
-000002b0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000002c0: 7974 686f 6e20 3a3a 2033 222c 0a20 2020  ython :: 3",.   
-000002d0: 2020 2020 2022 4f70 6572 6174 696e 6720       "Operating 
-000002e0: 5379 7374 656d 203a 3a20 556e 6978 222c  System :: Unix",
-000002f0: 0a20 2020 2020 2020 2022 4f70 6572 6174  .        "Operat
-00000300: 696e 6720 5379 7374 656d 203a 3a20 4d61  ing System :: Ma
-00000310: 634f 5320 3a3a 204d 6163 4f53 2058 222c  cOS :: MacOS X",
-00000320: 0a20 2020 2020 2020 2022 4f70 6572 6174  .        "Operat
-00000330: 696e 6720 5379 7374 656d 203a 3a20 4d69  ing System :: Mi
-00000340: 6372 6f73 6f66 7420 3a3a 2057 696e 646f  crosoft :: Windo
-00000350: 7773 222c 0a20 2020 205d 0a29            ws",.    ].)
+00000000: 0d0a 6672 6f6d 2073 6574 7570 746f 6f6c  ..from setuptool
+00000010: 7320 696d 706f 7274 2073 6574 7570 2c20  s import setup, 
+00000020: 6669 6e64 5f70 6163 6b61 6765 730d 0a0d  find_packages...
+00000030: 0a56 4552 5349 4f4e 203d 2027 302e 322e  .VERSION = '0.2.
+00000040: 3727 0d0a 4445 5343 5249 5054 494f 4e20  7'..DESCRIPTION 
+00000050: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
+00000060: 7420 6d61 6e61 6765 7320 6461 7461 6261  t manages databa
+00000070: 7365 2074 6872 6f75 6768 2050 6f73 7467  se through Postg
+00000080: 7265 5351 4c20 616e 6420 6372 6561 7465  reSQL and create
+00000090: 7320 7765 6261 7070 2074 6872 6f75 6768  s webapp through
+000000a0: 2044 6173 6820 706c 6f74 6c79 2e27 0d0a   Dash plotly.'..
+000000b0: 4c4f 4e47 5f44 4553 4352 4950 5449 4f4e  LONG_DESCRIPTION
+000000c0: 203d 2044 4553 4352 4950 5449 4f4e 0d0a   = DESCRIPTION..
+000000d0: 0d0a 2320 5365 7474 696e 6720 7570 0d0a  ..# Setting up..
+000000e0: 7365 7475 7028 0d0a 2020 2020 6e61 6d65  setup(..    name
+000000f0: 3d22 4469 6769 7461 6c69 7a61 7469 6f6e  ="Digitalization
+00000100: 546f 6f6c 7322 2c0d 0a20 2020 2076 6572  Tools",..    ver
+00000110: 7369 6f6e 3d56 4552 5349 4f4e 2c0d 0a20  sion=VERSION,.. 
+00000120: 2020 2061 7574 686f 723d 224d 656e 676b     author="Mengk
+00000130: 6520 4c75 222c 0d0a 2020 2020 6175 7468  e Lu",..    auth
+00000140: 6f72 5f65 6d61 696c 3d22 3c6d 6b6c 7530  or_email="<mklu0
+00000150: 3631 3140 676d 6169 6c2e 636f 6d3e 222c  611@gmail.com>",
+00000160: 0d0a 2020 2020 6465 7363 7269 7074 696f  ..    descriptio
+00000170: 6e3d 2044 4553 4352 4950 5449 4f4e 2c0d  n= DESCRIPTION,.
+00000180: 0a20 2020 206c 6f6e 675f 6465 7363 7269  .    long_descri
+00000190: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
+000001a0: 7065 3d22 7465 7874 2f6d 6172 6b64 6f77  pe="text/markdow
+000001b0: 6e22 2c0d 0a20 2020 206c 6f6e 675f 6465  n",..    long_de
+000001c0: 7363 7269 7074 696f 6e3d 4c4f 4e47 5f44  scription=LONG_D
+000001d0: 4553 4352 4950 5449 4f4e 2c0d 0a20 2020  ESCRIPTION,..   
+000001e0: 2070 6163 6b61 6765 733d 6669 6e64 5f70   packages=find_p
+000001f0: 6163 6b61 6765 7328 292c 0d0a 2020 2020  ackages(),..    
+00000200: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
+00000210: 3d5b 5d2c 0d0a 2020 2020 6b65 7977 6f72  =[],..    keywor
+00000220: 6473 3d5b 2770 7974 686f 6e27 2c20 2770  ds=['python', 'p
+00000230: 6f73 7467 7265 7371 6c27 2c20 2764 6173  ostgresql', 'das
+00000240: 6827 5d2c 0d0a 2020 2020 636c 6173 7369  h'],..    classi
+00000250: 6669 6572 733d 5b0d 0a20 2020 2020 2020  fiers=[..       
+00000260: 2022 4465 7665 6c6f 706d 656e 7420 5374   "Development St
+00000270: 6174 7573 203a 3a20 3120 2d20 506c 616e  atus :: 1 - Plan
+00000280: 6e69 6e67 222c 0d0a 2020 2020 2020 2020  ning",..        
+00000290: 2249 6e74 656e 6465 6420 4175 6469 656e  "Intended Audien
+000002a0: 6365 203a 3a20 4465 7665 6c6f 7065 7273  ce :: Developers
+000002b0: 222c 0d0a 2020 2020 2020 2020 2250 726f  ",..        "Pro
+000002c0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000002d0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000002e0: 222c 0d0a 2020 2020 2020 2020 224f 7065  ",..        "Ope
+000002f0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000300: 2055 6e69 7822 2c0d 0a20 2020 2020 2020   Unix",..       
+00000310: 2022 4f70 6572 6174 696e 6720 5379 7374   "Operating Syst
+00000320: 656d 203a 3a20 4d61 634f 5320 3a3a 204d  em :: MacOS :: M
+00000330: 6163 4f53 2058 222c 0d0a 2020 2020 2020  acOS X",..      
+00000340: 2020 224f 7065 7261 7469 6e67 2053 7973    "Operating Sys
+00000350: 7465 6d20 3a3a 204d 6963 726f 736f 6674  tem :: Microsoft
+00000360: 203a 3a20 5769 6e64 6f77 7322 2c0d 0a20   :: Windows",.. 
+00000370: 2020 205d 0d0a 29                           ]..)
```

