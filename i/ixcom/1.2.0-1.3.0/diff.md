# Comparing `tmp/ixcom-1.2.0.tar.gz` & `tmp/ixcom-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ixcom-1.2.0.tar", last modified: Tue Feb 23 16:09:25 2021, max compression
+gzip compressed data, was "ixcom-1.3.0.tar", last modified: Thu Apr 20 13:18:24 2023, max compression
```

## Comparing `ixcom-1.2.0.tar` & `ixcom-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2021-02-23 16:09:25.516922 ixcom-1.2.0/
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     1357 2021-02-23 16:09:25.516922 ixcom-1.2.0/PKG-INFO
--rw-rw-r--   0 sascha    (1000) sascha    (1000)      584 2021-01-27 12:16:10.000000 ixcom-1.2.0/README.md
-drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2021-02-23 16:09:25.516922 ixcom-1.2.0/ixcom/
--rw-rw-r--   0 sascha    (1000) sascha    (1000)      105 2021-01-27 12:16:10.000000 ixcom-1.2.0/ixcom/__init__.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     9303 2021-01-27 12:16:10.000000 ixcom-1.2.0/ixcom/cmdline.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     1462 2021-01-27 12:16:10.000000 ixcom-1.2.0/ixcom/commands.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     2557 2021-01-27 12:16:10.000000 ixcom-1.2.0/ixcom/crc16.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)      224 2021-01-27 12:16:10.000000 ixcom-1.2.0/ixcom/data.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)      361 2021-01-27 12:16:10.000000 ixcom-1.2.0/ixcom/exceptions.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     5096 2021-01-27 12:16:10.000000 ixcom-1.2.0/ixcom/grep.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    36568 2021-02-23 16:00:30.000000 ixcom-1.2.0/ixcom/messages.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    36427 2021-02-23 16:00:30.000000 ixcom-1.2.0/ixcom/parameters.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    66569 2021-02-23 16:00:30.000000 ixcom-1.2.0/ixcom/parser.py
--rw-rw-r--   0 sascha    (1000) sascha    (1000)    28034 2021-02-23 16:00:30.000000 ixcom-1.2.0/ixcom/protocol.py
-drwxrwxr-x   0 sascha    (1000) sascha    (1000)        0 2021-02-23 16:09:25.516922 ixcom-1.2.0/ixcom.egg-info/
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     1357 2021-02-23 16:09:25.000000 ixcom-1.2.0/ixcom.egg-info/PKG-INFO
--rw-rw-r--   0 sascha    (1000) sascha    (1000)      382 2021-02-23 16:09:25.000000 ixcom-1.2.0/ixcom.egg-info/SOURCES.txt
--rw-rw-r--   0 sascha    (1000) sascha    (1000)        1 2021-02-23 16:09:25.000000 ixcom-1.2.0/ixcom.egg-info/dependency_links.txt
--rw-rw-r--   0 sascha    (1000) sascha    (1000)      189 2021-02-23 16:09:25.000000 ixcom-1.2.0/ixcom.egg-info/entry_points.txt
--rw-rw-r--   0 sascha    (1000) sascha    (1000)       14 2021-02-23 16:09:25.000000 ixcom-1.2.0/ixcom.egg-info/requires.txt
--rw-rw-r--   0 sascha    (1000) sascha    (1000)        6 2021-02-23 16:09:25.000000 ixcom-1.2.0/ixcom.egg-info/top_level.txt
--rw-rw-r--   0 sascha    (1000) sascha    (1000)       38 2021-02-23 16:09:25.516922 ixcom-1.2.0/setup.cfg
--rw-rw-r--   0 sascha    (1000) sascha    (1000)     1807 2021-02-23 16:09:18.000000 ixcom-1.2.0/setup.py
+drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-04-20 13:18:24.358921 ixcom-1.3.0/
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1069 2023-04-20 13:09:22.000000 ixcom-1.3.0/LICENSE
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1272 2023-04-20 13:18:24.358921 ixcom-1.3.0/PKG-INFO
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      584 2023-04-20 13:09:22.000000 ixcom-1.3.0/README.md
+drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-04-20 13:18:24.354921 ixcom-1.3.0/ixcom/
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      105 2023-04-20 13:09:22.000000 ixcom-1.3.0/ixcom/__init__.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     9498 2023-04-20 13:09:22.000000 ixcom-1.3.0/ixcom/cmdline.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1462 2023-04-20 13:09:22.000000 ixcom-1.3.0/ixcom/commands.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     2780 2023-04-20 13:09:22.000000 ixcom-1.3.0/ixcom/crc16.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      304 2023-04-20 13:09:22.000000 ixcom-1.3.0/ixcom/data.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      401 2023-04-20 13:09:22.000000 ixcom-1.3.0/ixcom/exceptions.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     8142 2023-04-20 13:09:22.000000 ixcom-1.3.0/ixcom/grep.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    37317 2023-04-20 13:09:22.000000 ixcom-1.3.0/ixcom/messages.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    37288 2023-04-20 13:09:22.000000 ixcom-1.3.0/ixcom/parameters.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    70844 2023-04-20 13:09:22.000000 ixcom-1.3.0/ixcom/parser.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      273 2023-04-20 13:09:22.000000 ixcom-1.3.0/ixcom/plugin_messages.py
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)    42100 2023-04-20 13:09:22.000000 ixcom-1.3.0/ixcom/protocol.py
+drwxrwxr-x   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        0 2023-04-20 13:18:24.354921 ixcom-1.3.0/ixcom.egg-info/
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1272 2023-04-20 13:18:24.000000 ixcom-1.3.0/ixcom.egg-info/PKG-INFO
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      415 2023-04-20 13:18:24.000000 ixcom-1.3.0/ixcom.egg-info/SOURCES.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        1 2023-04-20 13:18:24.000000 ixcom-1.3.0/ixcom.egg-info/dependency_links.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)      189 2023-04-20 13:18:24.000000 ixcom-1.3.0/ixcom.egg-info/entry_points.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)       33 2023-04-20 13:18:24.000000 ixcom-1.3.0/ixcom.egg-info/requires.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)        6 2023-04-20 13:18:24.000000 ixcom-1.3.0/ixcom.egg-info/top_level.txt
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)       38 2023-04-20 13:18:24.358921 ixcom-1.3.0/setup.cfg
+-rw-rw-r--   0 maximilianrehermann  (1001) maximilianrehermann  (1001)     1890 2023-04-20 13:09:22.000000 ixcom-1.3.0/setup.py
```

### Comparing `ixcom-1.2.0/PKG-INFO` & `ixcom-1.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 Metadata-Version: 2.1
 Name: ixcom
-Version: 1.2.0
+Version: 1.3.0
 Summary: Library for communicating with xcom devices over network
 Home-page: http://www.imar-navigation.de
 Author: iMAR Navigation GmbH
 Author-email: support@imar-navigation.de
 License: UNKNOWN
 Project-URL: Documentation, https://ixcom.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/imar-navigation/ixcom-python
-Description: This library can be used to communicate with iMAR devices speaking the iXCOM protocol.
-        
-        Example usage:
-        ```python
-        import ixcom
-        
-        client = ixcom.Client('192.168.1.30')
-        client.open_last_free_channel()
-        client.realign()
-        ```
-        
-        Alongside this package, some command line tools will be installed in the user's path:
-        * configdump2txt: Converts a config.dump into a text form
-        * monitor2xcom: Converts iXCOM frames in a monitor.log into human readable format
-        * xcom_lookup: Looks for iXCOM devives on the local network
-        * split_config: Filters certain parameter IDs from a config.dump
 Keywords: XCOM,Inertial navigation,INS,iMAR,iNAT,GNSS,GPS,AHRS
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Provides-Extra: fastcrc
+License-File: LICENSE
+
+This library can be used to communicate with iMAR devices speaking the iXCOM protocol.
+
+Example usage:
+```python
+import ixcom
+
+client = ixcom.Client('192.168.1.30')
+client.open_last_free_channel()
+client.realign()
+```
+
+Alongside this package, some command line tools will be installed in the user's path:
+* configdump2txt: Converts a config.dump into a text form
+* monitor2xcom: Converts iXCOM frames in a monitor.log into human readable format
+* xcom_lookup: Looks for iXCOM devives on the local network
+* split_config: Filters certain parameter IDs from a config.dump
+
```

### Comparing `ixcom-1.2.0/README.md` & `ixcom-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ixcom-1.2.0/ixcom/cmdline.py` & `ixcom-1.3.0/ixcom/cmdline.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import sys
 import struct
 import argparse
 import socket
 
 
 class TextFileParser(ixcom.parser.MessageParser):
-    def __init__(self, outputfile, skip_parameter=None, print_request = True):
+    def __init__(self, outputfile, skip_parameter=list(), print_request = True):
         super().__init__()
+        self.ignore_output = False
         self.outputfile = outputfile
         self.print_request = print_request
         self.messageSearcher.disableCRC = False
         self._indent_level = 0
         self.add_subscriber(self)
         self.skipParameter = skip_parameter
         self.parameterList = list()
@@ -30,21 +31,21 @@
             self.write_output(zeile)
             self.write_output(f'divider: {log["divider"]}\n')
             self.write_output(f'running: {log["running"]}\n')
         self.write_output('\n\n')
     
     def handle_message(self, message, from_device):
         zeile = "Header Time: %.4f\n" % (message.header.get_time())
-        if self.skipParameter is None:
-            self.write_output(zeile)
-        elif message.data['parameterID'] in self.skipParameter:
-            return
         if message.header.msgID == ixcom.data.MessageID.PARAMETER:
-            self.parameterList.append((message.data['parameterID'], message))
-            return
+            parameter_id = message.data['parameterID']
+            if not (parameter_id in ixcom.data.ParameterPayloadDictionary) or \
+                parameter_id in self.skipParameter:
+                return
+            self.write_output(zeile)
+            self.parameterList.append((parameter_id, message))
             if message.payload.data["action"] == 0:
                 zeile = "Parameter: %s\n" % message.payload.get_name()
             else:
                 zeile = "Parameter request: %s\n" % message.payload.get_name()
                 if not self.print_request:
                     self.write_output(zeile+'\n')
                     return
@@ -102,15 +103,16 @@
             except:
                 zeile = "%s: %s\n" % (key, d[key])
         else:
             zeile = "%s: %s\n" % (key, d[key])
         self.write_output(zeile)
 
     def write_output(self, line):
-        self.outputfile.write('\t'*self._indent_level+line)
+        if not self.ignore_output:
+            self.outputfile.write('\t'*self._indent_level+line)
         
     def parse_file(self, inputfile):
         while True:
             tmpBuffer = inputfile.read(1024)
             if not tmpBuffer: 
                 break
             self.messageSearcher.process_bytes(tmpBuffer)
@@ -132,15 +134,15 @@
             data, (ip, _) = s.recvfrom(1024) # buffer size is 1024 bytes
             try:
                 client = ixcom.Client(ip, 3000)
                 client.open_last_free_channel()
                 sysname = client.get_parameter(19).payload.data['str'].decode('utf-8').split('\0')[0]
                 imutype = client.get_parameter(107).payload.data["type"]
                 fwversion = client.get_parameter(5).payload.data['str'].decode('utf-8').split('\0')[0]
-                if imutype is not 255:
+                if imutype != 255:
                     print("%s (%s, FW %s): ssh://root@%s, ftp://%s" % (data[:-1].decode('utf-8'), sysname, fwversion, ip, ip))
                 client.close_channel()
             except:
                 pass
         except (socket.timeout, OSError):
             try:
                 s.close()
@@ -151,22 +153,24 @@
 
 def configdump2txt(argv=None):
     parser = argparse.ArgumentParser(description='Converts xcom binary config dump files to other representations')
     parser.add_argument('input_file', metavar='', type=argparse.FileType('rb'), nargs='?', help='Name of the binary file', default='config.dump')
     parser.add_argument('-o', '--output', metavar='output_filename', type=argparse.FileType('wt'), help='Filename of the output file', default=sys.stdout)
     args = parser.parse_args(args=argv)
     xcomparser = TextFileParser(args.output, skip_parameter=[917])  # skip parxcom_loglist2(917)
+    xcomparser.ignore_output = True
     xcomparser.parse_file(args.input_file)
+    xcomparser.ignore_output = False
     xcomparser.write_parameter()
 
 
 def monitor2xcom(argv = None):
     import re
     import binascii
-    parser = argparse.ArgumentParser(description='Converts xcom binary config dump files to other representations')
+    parser = argparse.ArgumentParser(description='Converts raw messages in monitor log files to readable text')
     parser.add_argument('input_file', metavar='', type=argparse.FileType('rt'), nargs='?',
                        help='Name of the monitor file', default = 'monitor.log')
     parser.add_argument('-o', '--output', metavar='output_filename', type=argparse.FileType('wt'),
                        help='Filename of the output file', default = sys.stdout)
     args = parser.parse_args(args = argv)
     xcomparser = TextFileParser(args.output, print_request=False)
```

### Comparing `ixcom-1.2.0/ixcom/commands.py` & `ixcom-1.3.0/ixcom/commands.py`

 * *Files identical despite different names*

### Comparing `ixcom-1.2.0/ixcom/grep.py` & `ixcom-1.3.0/ixcom/grep.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import io
 
 import numpy as np
 from numpy.lib.recfunctions import append_fields
 
 from .parser import MessageParser, MessageSearcher
 from . import data
+from .exceptions import EndOfConfig
 
 def get_item_len(item):
     if isinstance(item, (list, tuple)):
         item_len = len(item)
     else:
         item_len = 1
     return item_len
@@ -40,23 +41,61 @@
     parser = MessageParser()
     parser.nothrow = True
     parser.add_callback(parameter_callback)
     with open(filename, 'rb') as f:
         parser.messageSearcher.process_bytes(f.read())
     return config
 
+def read_file_for_config(filename='iXCOMstream.bin'):
+    parameter_bytes = io.BytesIO(b'')
+    message_searcher = MessageSearcher(disable_crc = True)
+
+
+    def message_callback(in_bytes):
+        if not in_bytes:
+            return
+        message_id = int(in_bytes[1])
+        if message_id == data.MessageID.PARAMETER:
+            parameter_bytes.write(in_bytes)
+        else:
+            raise EndOfConfig()
+
+    config = {}
+    def parameter_callback(msg, from_device):
+        if msg.header.msgID == data.MessageID.PARAMETER:
+            config[msg.payload.get_name()] = msg.data
+
+
+    message_searcher.add_callback(message_callback)
+
+    with open(filename, 'rb') as f:
+        try:
+            message_searcher.process_buffer_unsafe(f.read())
+        except EndOfConfig:
+            pass
+    parameter_bytes.seek(0, os.SEEK_SET)
+    parser = MessageParser()
+    parser.nothrow = True
+    parser.add_callback(parameter_callback)
+    parser.messageSearcher.process_bytes(parameter_bytes.read())
+
+    return config
+
 def read_file(filename='iXCOMstream.bin'):
     message_bytes_dict = dict()
     result = dict()
     message_searcher = MessageSearcher(disable_crc = True)
 
     def message_callback(in_bytes):
         if not in_bytes:
             return
         message_id = int(in_bytes[1])
+        if message_id == data.MessageID.PLUGIN:
+            plugin_id = int(in_bytes[16]) + (int(in_bytes[17]) << 8)
+            message_id = 0x100 + plugin_id
         if message_id not in message_bytes_dict:
             message_bytes_dict[message_id] =  io.BytesIO(b'')
         message_bytes_dict[message_id].write(in_bytes)
 
     config = {}
     def parameter_callback(msg, from_device):
         if msg.header.msgID == data.MessageID.PARAMETER:
@@ -65,34 +104,48 @@
 
     message_searcher.add_callback(message_callback)
     with open(filename, 'rb') as f:
         message_searcher.process_buffer_unsafe(f.read())
 
     for msg_id in message_bytes_dict:
         message_bytes_dict[msg_id].seek(0, os.SEEK_SET)
-        
         if msg_id < 0xFD:
             msg = data.getMessageWithID(msg_id)
-            result[msg.payload.get_name()] = parse_message_from_buffer(msg_id, message_bytes_dict[msg_id])
+            try:
+                if msg:
+                    result[msg.payload.get_name()] = parse_message_from_buffer(msg_id, message_bytes_dict[msg_id])
+                else:
+                    data.handle_undefined_message(msg_id)
+            except:
+                print(f"Error: Message with ID: {msg_id} could not be parsed!")
         elif msg_id == data.MessageID.PARAMETER:
             parser = MessageParser()
             parser.nothrow = True
             parser.add_callback(parameter_callback)
             parser.messageSearcher.process_bytes(message_bytes_dict[msg_id].read())
             result['config'] = config
-
+        elif msg_id > 0xFF:
+                plugin_message_id = msg_id - 0x100
+                msg = data.getPluginMessageWithID(plugin_message_id)
+                try:
+                    if msg:
+                        result[msg.payload.get_name()] = parse_message_from_buffer(msg_id, message_bytes_dict[msg_id])
+                    else:
+                        data.handle_undefined_plugin_message(plugin_message_id)
+                except:
+                    print(f"Error: Plugin Message with ID: {plugin_message_id} could not be parsed!")
     return result
 
 def parse_message_from_file(messageID, filename = None):
     msg = data.getMessageWithID(messageID)
     if filename is None:
         fname = hex(messageID).upper()+'.bin'
     else:
         fname = filename
-    if messageID is not 0x19:
+    if messageID != 0x19:
         msg_size = msg.size()
     else:
         with open(fname, mode='rb') as f:
             msg_size = struct.unpack('=BBBBH', f.read(6))[4]
     
     with open(fname, mode='rb') as f:
         msg.from_bytes(f.read(msg_size))
@@ -116,31 +169,52 @@
             result_dict['globalstat'][idx] = msg.bottom.gStatus
             idx += 1
     return result_dict
 
 def parse_message_from_buffer(messageID, buffer):
  
     def add_time(ret):
-        return append_fields(ret, 'gpstime', ret['time_of_week_sec'] + 1e-6*ret['time_of_week_usec'], usemask=False)
-
-    msg = data.getMessageWithID(messageID)   
+        return append_fields(ret, 'gpstime', ret['time_of_week_sec'] + 1e-6 * ret['time_of_week_usec'], usemask=False)
+    if messageID > 0xFF:
+        plugin_message_id = messageID - 0x100
+        msg = data.getPluginMessageWithID(plugin_message_id)
+    else:
+        msg = data.getMessageWithID(messageID)   
     if not msg or get_item_len(msg) == 0:
-        print('ignored')
+        print(f'ignored Message with ID: {messageID}')
         return None
         
-    if messageID != data.SYSSTAT_Payload.message_id:   
+    if msg.payload.get_varsize_arg_from_bytes is None:
         dtype = np.dtype(msg.get_numpy_dtype())
         nlen = int(np.floor(len(buffer.getbuffer())/ dtype.itemsize))
-        return add_time(np.frombuffer(buffer.getbuffer(), dtype,count=nlen))
+        return add_time(np.frombuffer(buffer.getbuffer(), dtype, count=nlen))
     else:
+        _next_header = 0
+        _msg_length = 16
+        ret = []
+        while _next_header + _msg_length < len(buffer.getbuffer()):
+            buffer.seek(_next_header)
+            msg.header.from_bytes(buffer.read(16))
+            _msg_length = msg.header.msgLength
+            _varsize_arg = msg.payload.get_varsize_arg_from_bytes(buffer.read(_msg_length - 16 - 4))
+            if messageID > 0xFF:
+                msg = data.getPluginMessageWithID(plugin_message_id,_varsize_arg)
+            else:
+                msg = data.getMessageWithID(messageID,_varsize_arg) 
+            dtype = np.dtype(msg.get_numpy_dtype())
+            buffer.seek(_next_header)
+            ret.append(add_time(np.frombuffer(buffer.read(_msg_length), dtype, count=1)))
+            _next_header += _msg_length
+        return  ret  # normal ndarray not possible because of variable dtypes -> return list
+
         def iterate(buffer):
             start = 0
             while True:
                 try:
                     current = buffer.getbuffer()[start:]
                     msg.from_bytes(current)
                     dtype = msg.get_numpy_dtype()
                     start += msg.header.msgLength
-                    yield add_time(np.frombuffer(current, dtype, count=1))
+                    return add_time(np.frombuffer(current, dtype, count=1))
                 except:
                     return             
         return np.hstack(iterate(buffer))
```

### Comparing `ixcom-1.2.0/ixcom/messages.py` & `ixcom-1.3.0/ixcom/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,201 @@
 import struct
-from .protocol import message, ProtocolPayload, MessageID, PayloadItem, Message
+import os
+import json
+from .protocol import Message, PayloadItem, parse_messages_json_folder
+from .protocol import ProtocolPayload, message
+from .protocol import DefaultPluginMessagePayload, plugin_message
+from .protocol import MessageID
 
+def handle_undefined_message(*args):
+    pass
+
+def handle_undefined_plugin_message(*args):
+    pass
+
+"""
+PLUGIN MESSAGES
+"""
+class GenericPluginMessagePayload(DefaultPluginMessagePayload):
+    plugin_message_payload = Message([
+        PayloadItem(name = 'data', dimension = 4096-4, datatype = "B"),
+    ])
+
+"""
+MANUAL AND VARIABLE LENGTH MESSAGES
+"""
 @message(MessageID.RESPONSE)
 class ResponsePayload(ProtocolPayload):
     message_description = Message([
             PayloadItem(name = 'responseID', dimension = 1, datatype = 'H'),
             PayloadItem(name = 'repsonseLength', dimension = 1, datatype = 'H'),
-            ])
-    def __init__(self, msgLength):
+    ])
+
+    def get_varsize_item_list(self, payload_length):
+        _item_list = [
+            PayloadItem(name = 'responseID', dimension = 1, datatype = 'H'),
+            PayloadItem(name = 'repsonseLength', dimension = 1, datatype = 'H'),
+            PayloadItem(name = 'responseText', dimension = payload_length-4, datatype = 's'),
+        ]
+        return _item_list
+
+    def get_varsize_arg_from_bytes(self, inBytes):
+        payload_length = len(inBytes)
+        return payload_length
+
+    """def __init__(self, msgLength):
         self.message_description = Message([
             PayloadItem(name = 'responseID', dimension = 1, datatype = 'H'),
             PayloadItem(name = 'repsonseLength', dimension = 1, datatype = 'H'),
             PayloadItem(name = 'responseText', dimension = msgLength-24, datatype = 's'),
         ])
-        super().__init__()
+        super().__init__()"""
+
+
+@message(0x19)
+class SYSSTAT_Payload(ProtocolPayload):
+    message_description = Message([
+            PayloadItem(name = 'statMode', dimension = 1, datatype = 'I'),
+            PayloadItem(name = 'sysStat', dimension = 1, datatype = 'I'),
+    ])
+
+    @staticmethod
+    def get_varsize_item_list(stat_mode):
+        _item_list = [
+            PayloadItem(name = 'statMode', dimension = 1, datatype = 'I'),
+            PayloadItem(name = 'sysStat', dimension = 1, datatype = 'I')
+            ]
+        if(stat_mode & (1 << 0)):
+            _item_list += [PayloadItem(name = 'imuStat', dimension = 1, datatype = 'I')]
+        if(stat_mode & (1 << 1)):
+            _item_list += [PayloadItem(name = 'gnssStat', dimension = 1, datatype = 'I')]
+        if(stat_mode & (1 << 2)):
+            _item_list += [PayloadItem(name = 'magStat', dimension = 1, datatype = 'I')]
+        if(stat_mode & (1 << 3)):
+            _item_list += [PayloadItem(name = 'madcStat', dimension = 1, datatype = 'I')]
+        if(stat_mode & (1 << 4)):
+            _item_list += [PayloadItem(name = 'ekfStat', dimension = 2, datatype = 'I')]
+        if(stat_mode & (1 << 5)):
+            _item_list += [PayloadItem(name = 'ekfGeneralStat', dimension = 1, datatype = 'I')]
+        if(stat_mode & (1 << 6)):
+            _item_list += [PayloadItem(name = 'addStat', dimension = 4, datatype = 'I')]
+        if(stat_mode & (1 << 7)):
+            _item_list += [PayloadItem(name = 'serviceStat', dimension = 1, datatype = 'I')]
+        if(stat_mode & (1 << 8)):
+            _item_list += [PayloadItem(name = 'remainingAlignTime', dimension = 1, datatype = 'f')]
+        return _item_list
+
+    @staticmethod
+    def get_varsize_arg_from_bytes(inBytes):
+        stat_mode = struct.unpack('I', inBytes[:4])[0]
+        return stat_mode
+
+
+@message(0x57)
+class MONITOR_Payload(ProtocolPayload):
+    message_description = Message([
+        PayloadItem(name='log_level', dimension=1, datatype='B')
+    ])
+
+    def get_varsize_item_list(self, len_logmsg):
+        _item_list = [
+            PayloadItem(name='log_level', dimension=1, datatype='B'),
+            PayloadItem(name='logmsg', dimension=len_logmsg, datatype='s')
+            ]
+        return _item_list
+
+    def get_varsize_arg_from_bytes(self, inBytes):
+        len_logmsg = len(inBytes) - 1
+        return len_logmsg
+
+
+@message(0x91)
+class CANGATEWAY_Payload(ProtocolPayload):
+    message_description = Message([
+        PayloadItem(name='device', dimension=1, datatype='B'),
+        PayloadItem(name='reserved', dimension=3, datatype='B'),
+    ])
+
+    def get_varsize_item_list(self, num_frames):
+        _can_frame = Message([
+            PayloadItem(name='data', dimension=8, datatype='B'),
+            PayloadItem(name='length', dimension=1, datatype='B'),
+            PayloadItem(name='is_extended_mid', dimension=1, datatype='B'),
+            PayloadItem(name='is_remote_frame', dimension=1, datatype='B'),
+            PayloadItem(name='reserved', dimension=1, datatype='B'),
+            PayloadItem(name='mid', dimension=1, datatype='I'),
+            PayloadItem(name='timestamp', dimension=1, datatype='d')
+        ])
+        _item_list = [
+            PayloadItem(name='device', dimension=1, datatype='B'),
+            PayloadItem(name='reserved', dimension=3, datatype='B'),
+            PayloadItem(name='can_frames', dimension=num_frames, datatype=_can_frame)
+            ]
+        return _item_list
+
+    def get_varsize_arg_from_bytes(self, inBytes):
+        num_frames = (len(inBytes) - 4) / 24
+        return int(num_frames)
+
+
+class IMU_Payload(ProtocolPayload):
+    message_description = Message([
+        PayloadItem(name = 'acc', dimension = 3, datatype = 'f'),
+        PayloadItem(name = 'omg', dimension = 3, datatype = 'f'),
+    ])
+
+@message(0x00)
+class IMURAW_Payload(IMU_Payload):
+    pass
+
+
+@message(0x01)
+class IMUCORR_Payload(IMU_Payload):
+    pass
 
 
+@message(0x02)
+class IMUCOMP_Payload(IMU_Payload):
+    pass
+
+@message(0x03)
+class INSSOL_Payload(ProtocolPayload):
+    message_description = Message([
+        PayloadItem(name = 'acc', dimension = 3, datatype = 'f', unit = 'm/s²', description = 'Acceleration'),
+        PayloadItem(name = 'omg', dimension = 3, datatype = 'f', unit = 'rad/s', description = 'Specific force'),
+        PayloadItem(name = 'rpy', dimension = 3, datatype = 'f', unit = 'rad', description = 'Angle'),
+        PayloadItem(name = 'vel', dimension = 3, datatype = 'f', unit = 'm/s', description = 'Velocity'),
+        PayloadItem(name = 'lon', dimension = 1, datatype = 'd', unit = 'rad', description = 'Longitude'),
+        PayloadItem(name = 'lat', dimension = 1, datatype = 'd', unit = 'rad', description = 'Latitude'),
+        PayloadItem(name = 'alt', dimension = 1, datatype = 'f', unit = 'm', description = 'Altitude'),
+        PayloadItem(name = 'undulation', dimension = 1, datatype = 'h', unit = 'cm', description = 'Undulation'),
+        PayloadItem(name = 'DatSel', dimension = 1, datatype = 'H'),
+    ])
+
+@message(0x0D)
+class INSROTTEST_Payload(ProtocolPayload):
+    message_description = Message([
+        PayloadItem(name = 'accNED', dimension = 3, datatype = 'd'),
+    ])
+
+@message(0x20)
+class STATFPGA_Payload(ProtocolPayload):
+    message_description = Message([
+        PayloadItem(name = 'usParID', dimension = 1, datatype = 'H'),
+        PayloadItem(name = 'uReserved', dimension = 1, datatype = 'B'),
+        PayloadItem(name = 'ucAction', dimension = 1, datatype = 'B'),
+        PayloadItem(name = 'uiPowerStatLower', dimension = 1, datatype = 'I'),
+        PayloadItem(name = 'uiPowerStatUpper', dimension = 1, datatype = 'I'),
+        PayloadItem(name = 'usFpgaStatus', dimension = 1, datatype = 'H'),
+        PayloadItem(name = 'usSupervisorStatus', dimension = 1, datatype = 'H'),
+        PayloadItem(name = 'ucImuStatus', dimension = 1, datatype = 'B'),
+        PayloadItem(name = 'ucTempStatus', dimension = 1, datatype = 'B'),
+        PayloadItem(name = 'usRes', dimension = 1, datatype = 'H'),
+    ])
+
 @message(0x40)
 class POSTPROC_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'acc', dimension = 3, datatype = 'f', unit = 'm/s²', description = 'Specific force'),
         PayloadItem(name = 'omg', dimension = 3, datatype = 'f', unit = 'rad/s', description = 'Angular rate'),
         PayloadItem(name = 'delta_theta', dimension = 12, datatype = 'f'),
         PayloadItem(name = 'delta_v', dimension = 12, datatype = 'f'),
@@ -31,29 +207,14 @@
         PayloadItem(name = 'odoSpeed', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'odoTicks', dimension = 1, datatype = 'i'),
         PayloadItem(name = 'odoInterval', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'odoTrigEvent', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'odoNextEvent', dimension = 1, datatype = 'I'),
     ])
 
-
-@message(0x03)
-class INSSOL_Payload(ProtocolPayload):
-    message_description = Message([
-        PayloadItem(name = 'acc', dimension = 3, datatype = 'f', unit = 'm/s²', description = 'Acceleration'),
-        PayloadItem(name = 'omg', dimension = 3, datatype = 'f', unit = 'rad/s', description = 'Specific force'),
-        PayloadItem(name = 'rpy', dimension = 3, datatype = 'f', unit = 'rad', description = 'Angle'),
-        PayloadItem(name = 'vel', dimension = 3, datatype = 'f', unit = 'm/s', description = 'Velocity'),
-        PayloadItem(name = 'lon', dimension = 1, datatype = 'd', unit = 'rad', description = 'Longitude'),
-        PayloadItem(name = 'lat', dimension = 1, datatype = 'd', unit = 'rad', description = 'Latitude'),
-        PayloadItem(name = 'alt', dimension = 1, datatype = 'f', unit = 'm', description = 'Altitude'),
-        PayloadItem(name = 'undulation', dimension = 1, datatype = 'h', unit = 'cm', description = 'Undulation'),
-        PayloadItem(name = 'DatSel', dimension = 1, datatype = 'H'),
-    ])
-
 @message(0x47)
 class INSSOLECEF_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'acc', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'omg', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'pos_ecef', dimension = 3, datatype = 'd'),
         PayloadItem(name = 'vel_ecef', dimension = 3, datatype = 'f'),
@@ -89,84 +250,14 @@
 @message(0x56)
 class IMU_FILTERED_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'Omg', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'Acc', dimension = 3, datatype = 'f'),
     ])
 
-@message(0x65)
-class MAGDATA2_Payload(ProtocolPayload):
-    message_description = Message([
-        PayloadItem(name='rawx', dimension=1, datatype='i'),
-        PayloadItem(name='rawy', dimension=1, datatype='i'),
-        PayloadItem(name='rawz', dimension=1, datatype='i'),
-        PayloadItem(name='bit_error', dimension=1, datatype='B'),
-        PayloadItem(name='reserved', dimension=3, datatype='B'),
-    ])
-
-@message(0x66)
-class IPST_Payload(ProtocolPayload):
-    message_description = Message([
-        PayloadItem(name='omg', dimension=3, datatype='f'),
-        PayloadItem(name='acc', dimension=3, datatype='f'),
-        PayloadItem(name='system_status', dimension=1, datatype='I'),
-        PayloadItem(name='fpga_status', dimension=1, datatype='I'),
-        PayloadItem(name='odo_0_ticks', dimension=1, datatype='i'),
-        PayloadItem(name='odo_0_event', dimension=1, datatype='I'),
-        PayloadItem(name='odo_0_event_next', dimension=1, datatype='I'),
-        PayloadItem(name='odo_1_ticks', dimension=1, datatype='i'),
-        PayloadItem(name='odo_1_event', dimension=1, datatype='I'),
-        PayloadItem(name='odo_1_event_next', dimension=1, datatype='I'),
-        PayloadItem(name='odo_2_ticks', dimension=1, datatype='i'),
-        PayloadItem(name='odo_2_event', dimension=1, datatype='I'),
-        PayloadItem(name='odo_2_event_next', dimension=1, datatype='I'),
-    ])
-
-class IMU_Payload(ProtocolPayload):
-    message_description = Message([
-        PayloadItem(name = 'acc', dimension = 3, datatype = 'f'),
-        PayloadItem(name = 'omg', dimension = 3, datatype = 'f'),
-    ])
-
-
-@message(0x00)
-class IMURAW_Payload(IMU_Payload):
-    pass
-
-@message(0x01)
-class IMUCORR_Payload(IMU_Payload):
-    pass
-
-@message(0x02)
-class IMUCOMP_Payload(IMU_Payload):
-    pass
-
-@message(0x0D)
-class INSROTTEST_Payload(ProtocolPayload):
-    message_description = Message([
-        PayloadItem(name = 'accNED', dimension = 3, datatype = 'd'),
-    ])
-
-
-@message(0x20)
-class STATFPGA_Payload(ProtocolPayload):
-    message_description = Message([
-        PayloadItem(name = 'usParID', dimension = 1, datatype = 'H'),
-        PayloadItem(name = 'uReserved', dimension = 1, datatype = 'B'),
-        PayloadItem(name = 'ucAction', dimension = 1, datatype = 'B'),
-        PayloadItem(name = 'uiPowerStatLower', dimension = 1, datatype = 'I'),
-        PayloadItem(name = 'uiPowerStatUpper', dimension = 1, datatype = 'I'),
-        PayloadItem(name = 'usFpgaStatus', dimension = 1, datatype = 'H'),
-        PayloadItem(name = 'usSupervisorStatus', dimension = 1, datatype = 'H'),
-        PayloadItem(name = 'ucImuStatus', dimension = 1, datatype = 'B'),
-        PayloadItem(name = 'ucTempStatus', dimension = 1, datatype = 'B'),
-        PayloadItem(name = 'usRes', dimension = 1, datatype = 'H'),
-    ])
-
-
 @message(0x63)
 class PASSTHROUGH_Payload(ProtocolPayload):
     message_description = Message([
             PayloadItem(name = 'port', dimension = 1, datatype = 'B'),
             PayloadItem(name = 'reserved', dimension = 3, datatype = 'B'),
             PayloadItem(name='passthroughdata', dimension=256, datatype='B')
             ])
@@ -200,97 +291,51 @@
             item_list += [PayloadItem(name = 'addStat', dimension = 4, datatype = 'I')]
         if(stat_mode & (1 << 7)):
             item_list += [PayloadItem(name = 'serviceStat', dimension = 1, datatype = 'I')]
         if(stat_mode & (1 << 8)):
             item_list += [PayloadItem(name = 'remainingAlignTime', dimension = 1, datatype = 'f')]
         return item_list
 
-@message(0x19)
-class SYSSTAT_Payload(ProtocolPayload):
+@message(0x65)
+class MAGDATA2_Payload(ProtocolPayload):
     message_description = Message([
-            PayloadItem(name = 'statMode', dimension = 1, datatype = 'I'),
-            PayloadItem(name = 'sysStat', dimension = 1, datatype = 'I'),
-            ])
-
-    def _get_varsize_message_description(self, stat_mode):
-        _item_list = [
-            PayloadItem(name = 'statMode', dimension = 1, datatype = 'I'),
-            PayloadItem(name = 'sysStat', dimension = 1, datatype = 'I')
-            ]
-        if(stat_mode & (1 << 0)):
-            _item_list += [PayloadItem(name = 'imuStat', dimension = 1, datatype = 'I')]
-        if(stat_mode & (1 << 1)):
-            _item_list += [PayloadItem(name = 'gnssStat', dimension = 1, datatype = 'I')]
-        if(stat_mode & (1 << 2)):
-            _item_list += [PayloadItem(name = 'magStat', dimension = 1, datatype = 'I')]
-        if(stat_mode & (1 << 3)):
-            _item_list += [PayloadItem(name = 'madcStat', dimension = 1, datatype = 'I')]
-        if(stat_mode & (1 << 4)):
-            _item_list += [PayloadItem(name = 'ekfStat', dimension = 2, datatype = 'I')]
-        if(stat_mode & (1 << 5)):
-            _item_list += [PayloadItem(name = 'ekfGeneralStat', dimension = 1, datatype = 'I')]
-        if(stat_mode & (1 << 6)):
-            _item_list += [PayloadItem(name = 'addStat', dimension = 4, datatype = 'I')]
-        if(stat_mode & (1 << 7)):
-            _item_list += [PayloadItem(name = 'serviceStat', dimension = 1, datatype = 'I')]
-        if(stat_mode & (1 << 8)):
-            _item_list += [PayloadItem(name = 'remainingAlignTime', dimension = 1, datatype = 'f')]
-        self.message_description = Message(_item_list)
-        self.item_list = _item_list
-        self._structString = None
-
-
-    def from_bytes(self, inBytes):
-        item_list = [
-            PayloadItem(name = 'statMode', dimension = 1, datatype = 'I'),
-            PayloadItem(name = 'sysStat', dimension = 1, datatype = 'I'),
-        ]
-        stat_mode = struct.unpack('I', inBytes[:4])[0]
-        item_list += self._get_payload(stat_mode)
-        _msg = Message(item_list)
-        self.data = _msg.data
-        self.message_description = _msg
-        self.struct_inst = _msg.struct_inst
-        self._structString = _msg.struct_inst.format
-        super().from_bytes(inBytes)
+        PayloadItem(name='rawx', dimension=1, datatype='i'),
+        PayloadItem(name='rawy', dimension=1, datatype='i'),
+        PayloadItem(name='rawz', dimension=1, datatype='i'),
+        PayloadItem(name='bit_error', dimension=1, datatype='B'),
+        PayloadItem(name='reserved', dimension=3, datatype='B'),
+    ])
 
-#    def to_bytes(self):
-#        item_list = [
-#            PayloadItem(name = 'statMode', dimension = 1, datatype = 'I'),
-#            PayloadItem(name = 'sysStat', dimension = 1, datatype = 'I'),
-#        ]
-#        item_list += self._get_payload(self.data['statMode'])
-#        _msg = Message(item_list)
-#        self.data = _msg.data
-#        self.message_description = _msg
-#        self.struct_inst = _msg.struct_inst
-#        self._structString = _msg.struct_inst.format
-#        return super().to_bytes()
+@message(0x66)
+class IPST_Payload(ProtocolPayload):
+    message_description = Message([
+        PayloadItem(name='omg', dimension=3, datatype='f'),
+        PayloadItem(name='acc', dimension=3, datatype='f'),
+        PayloadItem(name='system_status', dimension=1, datatype='I'),
+        PayloadItem(name='fpga_status', dimension=1, datatype='I'),
+        PayloadItem(name='odo_0_ticks', dimension=1, datatype='i'),
+        PayloadItem(name='odo_0_event', dimension=1, datatype='I'),
+        PayloadItem(name='odo_0_event_next', dimension=1, datatype='I'),
+        PayloadItem(name='odo_1_ticks', dimension=1, datatype='i'),
+        PayloadItem(name='odo_1_event', dimension=1, datatype='I'),
+        PayloadItem(name='odo_1_event_next', dimension=1, datatype='I'),
+        PayloadItem(name='odo_2_ticks', dimension=1, datatype='i'),
+        PayloadItem(name='odo_2_event', dimension=1, datatype='I'),
+        PayloadItem(name='odo_2_event_next', dimension=1, datatype='I'),
+    ])
 
-    def _get_payload(self, stat_mode):
-        item_list = []
-        if(stat_mode & (1 << 0)):
-            item_list += [PayloadItem(name = 'imuStat', dimension = 1, datatype = 'I')]
-        if(stat_mode & (1 << 1)):
-            item_list += [PayloadItem(name = 'gnssStat', dimension = 1, datatype = 'I')]
-        if(stat_mode & (1 << 2)):
-            item_list += [PayloadItem(name = 'magStat', dimension = 1, datatype = 'I')]
-        if(stat_mode & (1 << 3)):
-            item_list += [PayloadItem(name = 'madcStat', dimension = 1, datatype = 'I')]
-        if(stat_mode & (1 << 4)):
-            item_list += [PayloadItem(name = 'ekfStat', dimension = 2, datatype = 'I')]
-        if(stat_mode & (1 << 5)):
-            item_list += [PayloadItem(name = 'ekfGeneralStat', dimension = 1, datatype = 'I')]
-        if(stat_mode & (1 << 6)):
-            item_list += [PayloadItem(name = 'addStat', dimension = 4, datatype = 'I')]
-        if(stat_mode & (1 << 7)):
-            item_list += [PayloadItem(name = 'serviceStat', dimension = 1, datatype = 'I')]
-        if(stat_mode & (1 << 8)):
-            item_list += [PayloadItem(name = 'remainingAlignTime', dimension = 1, datatype = 'f')]
-        return item_list
+@message(0x80)
+class ENCODERDAT_Payload(ProtocolPayload):
+    MAXENC = 3
+    message_description = Message([
+        PayloadItem(name='encoder_pos', dimension=MAXENC, datatype='d'),
+        PayloadItem(name='encoder_vel', dimension=MAXENC, datatype='d'),
+        PayloadItem(name='encoder_status', dimension=MAXENC, datatype='I'),
+        PayloadItem(name='nav_status', dimension=1, datatype='I'),
+    ])
 
 @message(0x1a)
 class MAGHDG_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'MagHdg', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'MagCOG', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'Deviation', dimension = 1, datatype = 'f'),
@@ -298,61 +343,54 @@
 
 @message(0x04)
 class INSRPY_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'rpy', dimension = 3, datatype = 'f'),
     ])
 
-
 @message(0x05)
 class INSDCM_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'DCM', dimension = 9, datatype = 'f'),
     ])
 
-
 @message(0x06)
 class INSQUAT_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'quat', dimension = 4, datatype = 'f'),
     ])
 
-
 @message(0x0A)
 class INSPOSLLH_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'lon', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'lat', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'alt', dimension = 1, datatype = 'f'),
     ])
 
-
 @message(0x0C)
 class INSPOSUTM_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'zone', dimension = 1, datatype = 'i'),
         PayloadItem(name = 'easting', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'northing', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'height', dimension = 1, datatype = 'f'),
     ])
 
-
 @message(0x0B)
 class INSPOSECEF_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'pos', dimension = 3, datatype = 'd'),
     ])
 
-
 class INSVEL_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'vel', dimension = 3, datatype = 'f'),
     ])
 
-
 @message(0x07)
 class INSVELNED_Payload(INSVEL_Payload):
     pass
 
 @message(0x08)
 class INSVELECEF_Payload(INSVEL_Payload):
     pass
@@ -372,15 +410,14 @@
         PayloadItem(name = 'magHdg', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'magBank', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'magElevation', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'magDeviation', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'status', dimension = 1, datatype = 'I'),
     ])
 
-
 @message(0x17)
 class AIRDATA_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'TAS', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'IAS', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'baroAlt', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'baroAltRate', dimension = 1, datatype = 'f'),
@@ -409,54 +446,50 @@
         PayloadItem(name = 'biasAcc', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'biasOmg', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'scfAcc', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'scfOmg', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'scfOdo', dimension = 1, datatype = 'f'),
     ])
 
-
 @message(0x28)
 class EKFSTDDEV2_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'pos', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'vel', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'rpy', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'biasAcc', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'biasOmg', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'fMaAcc', dimension = 9, datatype = 'f'),
         PayloadItem(name = 'fMaOmg', dimension = 9, datatype = 'f'),
         PayloadItem(name = 'scfOdo', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'fMaOdo', dimension = 2, datatype = 'f'),
     ])
 
-
 @message(0x27)
 class EKFERROR2_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'biasAcc', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'biasOmg', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'fMaAcc', dimension = 9, datatype = 'f'),
         PayloadItem(name = 'fMaOmg', dimension = 9, datatype = 'f'),
         PayloadItem(name = 'scfOdo', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'maOdo', dimension = 2, datatype = 'f'),
     ])
 
-
 @message(0x10)
 class EKFERROR_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'biasAcc', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'biasOmg', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'scfAcc', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'scfOmg', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'scfOdo', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'maOdo', dimension = 2, datatype = 'f'),
     ])
 
-
 @message(0x11)
 class EKFTIGHTLY_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'ucSatsAvailablePSR', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'ucSatsUsedPSR', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'ucSatsAvailableRR', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'ucSatsUsedRR', dimension = 1, datatype = 'B'),
@@ -474,44 +507,40 @@
         PayloadItem(name = 'uiOutlierSatsRR_GLONASS', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'uiUsedSatsTDCP_GPS', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'uiOutlierSatsTDCP_GPS', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'uiUsedSatsTDCP_GLONASS', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'uiOutlierSatsTDCP_GLONASS', dimension = 1, datatype = 'I'),
     ])
 
-
 @message(0x29)
 class EKFPOSCOVAR_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'fPosCovar', dimension = 9, datatype = 'f'),
     ])
 
-
 @message(0x21)
 class POWER_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'power', dimension = 32, datatype = 'f'),
     ])
 
-
 @message(0x22)
 class TEMP_Payload(ProtocolPayload):
     
     message_description = Message([
         PayloadItem(name = 'temp_power_pcb', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'temp_switcher', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'temp_oem628', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'temp_oem615', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'temp_cpu', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'temp_acc', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'temp_omg', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'temp_other', dimension = 5, datatype = 'f'),
     ])
 
-
 @message(0x1F)
 class HEAVE_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'StatFiltPos', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'AppliedFreqHz', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'AppliedAmplMeter', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'AppliedSigWaveHeightMeter', dimension = 1, datatype = 'd'),
@@ -520,46 +549,42 @@
         PayloadItem(name = 'ZDvel', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'AccZnavDown', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'HeavePosVelDown', dimension = 2, datatype = 'd'),
         PayloadItem(name = 'HeaveAlgoStatus1', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'HeaveAlgoStatus2', dimension = 1, datatype = 'I'),
     ])
 
-
 @message(0x24)
 class CANSTAT_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'uiErrorMask', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'ucControllerStatus', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'ucTransceiverStatus', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'ucProtocolStatus', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'ucProtocolLocation', dimension = 1, datatype = 'B'),
     ])
 
-
 @message(0x1D)
 class ARINC429STAT_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'uiStatus', dimension = 1, datatype = 'I'),
     ])
 
-
 @message(0x26)
 class TIME_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'sysTime', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'ImuInterval', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'TimeSincePPS', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'PPS_IMUtime', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'PPS_GNSStime', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'GNSSbias', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'GNSSbiasSmoothed', dimension = 1, datatype = 'd'),
     ])
 
-
 @message(0x12)
 class GNSSSOL_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'lon', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'lat', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'alt', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'undulation', dimension = 1, datatype = 'f'),
@@ -581,30 +606,28 @@
 class INSGNDSPEED_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'SOG', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'COG', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'VDown', dimension = 1, datatype = 'f'),
     ])
 
-
 @message(0x14)
 class GNSSTIME_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'utcOffset', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'offset', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'year', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'month', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'day', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'hour', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'minute', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'millisec', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'status', dimension = 1, datatype = 'I'),
     ])
 
-
 @message(0x15)
 class GNSSSOLCUST_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'dLon', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'dLat', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'fAlt', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'fUndulation', dimension = 1, datatype = 'f'),
@@ -620,15 +643,14 @@
         PayloadItem(name = 'ucSatsDisplacement', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'usReserved', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'fDiffAge', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'fSolAge', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'uiGnssStatus', dimension = 1, datatype = 'I'),
     ])
 
-
 @message(0x33)
 class GNSSHDG_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'hdg', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'stdDevHdg', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'pitch', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'stdDevPitch', dimension = 1, datatype = 'f'),
@@ -636,50 +658,42 @@
         PayloadItem(name = 'solType', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'res', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'satsUsed', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'satsTracked', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'gnssStatus', dimension = 1, datatype = 'I'),
     ])
 
-
 @message(0x1B)
 class GNSSLEVERARM_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'primary', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'stdDevPrimary', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'relative', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'stdDevRelative', dimension = 3, datatype = 'f'),
     ])
 
-
 @message(0x1C)
 class GNSSVOTER_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'ucSatsUsed_INT', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'ucSatsUsed_EXT', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'usReserved', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'fStdDevHDG_INT', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'fStdDevHDG_EXT', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'fStdDevPOS_INT', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'fStdDevPOS_EXT', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'uiStatus', dimension = 1, datatype = 'I'),
     ])
 
-
 @message(0x1E)
 class GNSSHWMON_Payload(ProtocolPayload):
-    message_description = Message([])
-    def __init__(self):
-        if type(self).message_description is None:
-            item_list = []
-            for idx in range(0, 16):
-                item_list += [PayloadItem(name = 'val %d' % idx, dimension = 1, datatype = 'f'),
-                              PayloadItem(name = 'status %d' % idx, dimension = 1, datatype = 'I')]
-            type(self).message_description = Message(item_list)
-
+    GnssHwMonitor = Message([PayloadItem(name = 'val' , dimension = 1, datatype = 'f'),
+                             PayloadItem(name = 'status' , dimension = 1, datatype = 'I')])
+    
+    message_description = Message([PayloadItem(name = 'GnssHwMonitor' , dimension = 16, datatype = GnssHwMonitor)])
 
 @message(0x38)
 class GNSSALIGNBSL_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'east', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'north', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'up', dimension = 1, datatype = 'd'),
@@ -690,69 +704,62 @@
         PayloadItem(name = 'posVelType', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'satsTracked', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'satsUsedInSolution', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'extSolStat', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'reserved', dimension = 1, datatype = 'B'),
     ])
 
-
 @message(0x16)
 class WHEELDATA_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'odoSpeed', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'ticks', dimension = 1, datatype = 'i'),
     ])
 
-
 @message(0x32)
 class WHEELDATADBG_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'odoSpeed', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'ticks', dimension = 1, datatype = 'i'),
         PayloadItem(name = 'interval', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'trigEvent', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'trigNextEvent', dimension = 1, datatype = 'I'),
     ])
 
-
 @message(0x34)
 class EVENTTIME_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'dGpsTime_EVENT_0', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'dGpsTime_EVENT_1', dimension = 1, datatype = 'd'),
     ])
 
-
 @message(0x35)
 class OMGINT_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'omgINT', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'omgINTtime', dimension = 1, datatype = 'f'),
     ])
 
-
 @message(0x36)
 class ADC24STATUS_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'uiRRidx', dimension = 4, datatype = 'I'),
         PayloadItem(name = 'uiRRvalue', dimension = 4, datatype = 'I'),
     ])
 
-
 @message(0x37)
 class ADC24DATA_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'acc', dimension = 3, datatype = 'I'),
         PayloadItem(name = 'frameCounter', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'temperature', dimension = 1, datatype = 'h'),
         PayloadItem(name = 'errorStatus', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'intervalCounter', dimension = 3, datatype = 'B'),
     ])
 
-
 @message(0x42)
 class CSACDATA_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'status', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'alarm', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'serialNum', dimension = 32, datatype = 's'),
         PayloadItem(name = 'mode', dimension = 1, datatype = 'I'),
@@ -776,20 +783,14 @@
 @message(0x46)
 class INSMGRS_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'Error Code', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'MGRS Position', dimension = 64, datatype = 's'),
     ])
 
-@message(0x57)
-class TAG_Payload(ProtocolPayload):
-    message_description = Message([
-        PayloadItem(name = 'tag', dimension = 128, datatype = 's')
-    ])
-
 @message(0x25)
 class GNSSSATINFO_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'SvID', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'PositionECEF', dimension = 3, datatype = 'd'),
         PayloadItem(name = 'VelocityECEF', dimension = 3, datatype = 'd'),
         PayloadItem(name = 'CN0', dimension = 3, datatype = 'f'),
@@ -804,7 +805,14 @@
 class NTRIPSTAT_Payload(ProtocolPayload):
     message_description = Message([
         PayloadItem(name = 'NtripStatus', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'LastErrorMsg', dimension = 256, datatype = 's'),
         PayloadItem(name = 'ErrorCounter', dimension = 1, datatype = 'I'),
     ])
 
+
+"""
+MESSAGES FROM JSON FILES
+"""
+path_json = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'json-files', 'messages')
+parse_messages_json_folder(path_json)
+
```

### Comparing `ixcom-1.2.0/ixcom/parameters.py` & `ixcom-1.3.0/ixcom/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,32 @@
-from .protocol import DefaultParameterPayload, Message, PayloadItem, parameter
+import os
+import json
+from .protocol import Message, PayloadItem, parse_parameter_json_folder
+from .protocol import DefaultParameterPayload, parameter
+from .protocol import DefaultPluginParameterPayload, plugin_parameter
+
+def handle_undefined_parameter(*args):
+    pass
+
+"""
+PLUGIN PARAMETER
+"""
+### ride_control plugin
+@plugin_parameter(10)
+class PARPLUGIN_IATANGLIM_Payload(DefaultPluginParameterPayload):
+    plugin_parameter_payload = Message([
+        PayloadItem(name = 'angLimLowMain', dimension = 4, datatype = 'f'),
+        PayloadItem(name = 'angLimUpMain', dimension = 4, datatype = 'f'),
+        PayloadItem(name = 'angLimLowAux', dimension = 4, datatype = 'f'),
+        PayloadItem(name = 'angLimUpAux', dimension = 4, datatype = 'f')
+    ])
 
 
 """
-PARSYS
+MANUAL AND VARIABLE LENGTH PARAMETER
 """
 class PARSYS_STRING_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'str', dimension = 32, datatype = 's')
     ])
 
 class PARSYS_STRING64_Payload(DefaultParameterPayload):
@@ -107,90 +127,75 @@
 class PARSYS_CONFIGCRC_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'romCRC', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'ramCRC', dimension = 1, datatype = 'H'),
     ])
 
 @parameter(18)
-class PARSYS_OSVERSION_Payload(PARSYS_STRING64_Payload):
+class PARSYS_OSVERSION_Payload(PARSYS_STRING_Payload):
     pass
 
 @parameter(19)
 class PARSYS_SYSNAME_Payload(PARSYS_STRING64_Payload):
     pass
 
-"""
-PARIMU
-"""
 @parameter(105)
 class PARIMU_MISALIGN_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'rpy', dimension = 3, datatype = 'f'),
     ])
 
-
 @parameter(112)
 class PARIMU_BANDSTOP_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'bandwidth', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'center', dimension = 1, datatype = 'f'),
     ])
 
 @parameter(117)
 class PARIMU_RANGE_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'range_accel', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'range_gyro', dimension = 1, datatype = 'f'),
     ])
 
-
-
-"""
-PARGNSS
-"""
-
-
-
 @parameter(203)
 class PARGNSS_LATENCY_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'baud', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'reserved2', dimension = 1, datatype = 'H'),
     ])
 
 @parameter(204)
 class PARGNSS_ANTOFFSET_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'antennaOffset', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'stdDev', dimension = 3, datatype = 'f'),
     ])
 
-    def get_name(self):
-        return super().get_name() + '_' + str(self.data.get('reserved_paramheader', ''))
+    def get_ant_number(self):
+        return self.data.get('reserved_paramheader', '')
 
 @parameter(212)
 class PARGNSS_LOCKOUTSYSTEM_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'lockoutMask', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'reserved2', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'reserved3', dimension = 1, datatype = 'H'),
     ])
 
-
 @parameter(213)
 class PARGNSS_RTCMV3CONFIG_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'port', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'enable', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'reserved2', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'baud', dimension = 1, datatype = 'I'),
     ])
 
-
-
 @parameter(217)
 class PARGNSS_MODEL_Payload(DefaultParameterPayload):
     __sub_payload = Message(
         [PayloadItem(name = f'modelName', dimension = 16, datatype = 's'),
         PayloadItem(name = f'year', dimension = 1, datatype = 'I'),
         PayloadItem(name = f'month', dimension = 1, datatype = 'I'),
         PayloadItem(name = f'day', dimension = 1, datatype = 'I')])
@@ -224,113 +229,92 @@
     ])
 
 @parameter(229)
 class PARGNSS_HDGOFFSET_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name='offset', dimension=1, datatype='f'),
     ])
-      
-"""
-PARMAG
-"""
+
 @parameter(300)
 class PARMAG_COM_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'port', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'reserved3', dimension = 3, datatype = 'B'),
         PayloadItem(name = 'baud', dimension = 1, datatype = 'I'),
     ])
 
 @parameter(304)
 class PARMAG_MISALIGN_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'rpy', dimension = 3, datatype = 'f'),
     ])
 
-
 @parameter(307)
 class PARMAG_CAL_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'C', dimension = 9, datatype = 'f'),
         PayloadItem(name = 'bias', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'valid', dimension = 1, datatype = 'I'),
     ])
 
-
 @parameter(308)
 class PARMAG_CALSTATE_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'calstate', dimension = 1, datatype = 'i'),
     ])
 
-
 @parameter(309)
 class PARMAG_FOM_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'FOM', dimension = 1, datatype = 'f'),
     ])
 
-
-"""
-PARMADC
-"""
 @parameter(400)
 class PARMADC_ENABLE_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'enable', dimension = 1, datatype = 'I'),
     ])
 
-
 @parameter(401)
 class PARMADC_LEVERARM_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'leverArm', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'leverArmStdDev', dimension = 3, datatype = 'f'),
     ])
 
-
-"""
-PARREC
-"""
 @parameter(600)
 class PARREC_CONFIG_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'channelNumber', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'autostart', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'reserved2', dimension = 1, datatype = 'H'),
     ])
 
-
 @parameter(603)
 class PARREC_START_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'str', dimension = 128, datatype = 's'),
     ])
 
-
 @parameter(604)
 class PARREC_STOP_Payload(DefaultParameterPayload):
     pass
 
 @parameter(606)
 class PARREC_SUFFIX_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'suffix', dimension = 128, datatype = 's'),
     ])
 
-
 @parameter(607)
 class PARREC_DISKSPACE_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'freespace', dimension = 1, datatype = 'd'),
     ])
-        
-"""
-PAREKF
-"""
+
 @parameter(700)
 class PAREKF_ALIGNMODE_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'alignmode', dimension = 1, datatype = 'I'),
     ])
 
 @parameter(701)
@@ -404,51 +388,28 @@
         PayloadItem(name = 'weightingFactor', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'timeConstant', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'delay', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'mask', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'autoZupt', dimension = 1, datatype = 'B'),
     ])
 
-
 @parameter(714)
 class PAREKF_DEFPOS_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'lon', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'lat', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'alt', dimension = 1, datatype = 'f'),
     ])
 
-
 @parameter(715)
 class PAREKF_DEFHDG_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'hdg', dimension = 1, datatype = 'f'),
     ])
 
-
-@parameter(731)
-class PAREKF_STARTUPV2_Payload(DefaultParameterPayload):
-    parameter_payload = Message([
-        PayloadItem(name = 'initLon', dimension = 1, datatype = 'd'),
-        PayloadItem(name = 'initLat', dimension = 1, datatype = 'd'),
-        PayloadItem(name = 'initAlt', dimension = 1, datatype = 'f'),
-        PayloadItem(name = 'stdDev', dimension = 3, datatype = 'f'),
-        PayloadItem(name = 'initHdg', dimension = 1, datatype = 'f'),
-        PayloadItem(name = 'stdDevHdg', dimension = 1, datatype = 'f'),
-        PayloadItem(name = 'leverArm', dimension = 3, datatype = 'f'),
-        PayloadItem(name = 'stdLeverArm', dimension = 3, datatype = 'f'),
-        PayloadItem(name = 'posMode', dimension = 1, datatype = 'B'),
-        PayloadItem(name = 'hdgMode', dimension = 1, datatype = 'B'),
-        PayloadItem(name = 'gnssTimeout', dimension = 1, datatype = 'H'),
-        PayloadItem(name = 'altMSL', dimension = 1, datatype = 'B'),
-        PayloadItem(name = 'realign', dimension = 1, datatype = 'B'),
-        PayloadItem(name = 'inMotion', dimension = 1, datatype = 'B'),
-        PayloadItem(name = 'autoRestart', dimension = 1, datatype = 'B'),
-    ])
-
 @parameter(717)
 class PAREKF_POWERDOWN_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'savestate', dimension = 1, datatype = 'I'),
     ])
 
 @parameter(719)
@@ -458,36 +419,32 @@
         PayloadItem(name = 'lat', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'alt', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'stdDevLon', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'stdDevLat', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'stdDevAlt', dimension = 1, datatype = 'd'),
     ])
 
-
-@parameter(723)
-class PAREKF_STOREDATT_Payload(DefaultParameterPayload):
-    parameter_payload = Message([
-        PayloadItem(name = 'rpy', dimension = 3, datatype = 'f'),
-        PayloadItem(name = 'stdDev', dimension = 3, datatype = 'f'),
-    ])
-
-
 @parameter(720)
 class PAREKF_ALIGNZUPTSTDDEV_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'zuptStdDev', dimension = 1, datatype = 'd'),
     ])
 
-
 @parameter(721)
 class PAREKF_POSAIDSTDDEVTHR_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'thr', dimension = 1, datatype = 'd'),
     ])
 
+@parameter(723)
+class PAREKF_STOREDATT_Payload(DefaultParameterPayload):
+    parameter_payload = Message([
+        PayloadItem(name = 'rpy', dimension = 3, datatype = 'f'),
+        PayloadItem(name = 'stdDev', dimension = 3, datatype = 'f'),
+    ])
 
 @parameter(724)
 class PAREKF_ODOMETER_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'sfError', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'sfStdDev', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'rwScalefactor', dimension = 1, datatype = 'f'),
@@ -499,81 +456,93 @@
         PayloadItem(name = 'rwMisalignmentZ', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'minVel', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'maxVel', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'useAvgInno', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'enableCoarseCal', dimension = 1, datatype = 'H'),
     ])
 
-
 @parameter(725)
 class PAREKF_ODOBOGIE_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'distance', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'enable', dimension = 1, datatype = 'I'),
     ])
 
-
 @parameter(726)
 class PAREKF_GNSSLEVERARMEST_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'primary', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'secondary', dimension = 1, datatype = 'H'),
     ])
 
-
 @parameter(727)
 class PAREKF_GNSSAIDINGRATE_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'psrpos', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'psrvel', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'rtk', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'rtktimeout', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'hdg', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'duringzupt', dimension = 1, datatype = 'H'),
     ])
 
-
 @parameter(728)
 class PAREKF_KINALIGNTHR_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'thr', dimension = 1, datatype = 'f'),
     ])
 
-
 @parameter(729)
 class PAREKF_PDOPTHR_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'thr', dimension = 1, datatype = 'f'),
     ])
 
-
 @parameter(730)
 class PAREKF_DUALANTAID_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'thrHdg', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'thrPitch', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'thrINSHdg', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'mode', dimension = 1, datatype = 'I'),
     ])
 
+@parameter(731)
+class PAREKF_STARTUPV2_Payload(DefaultParameterPayload):
+    parameter_payload = Message([
+        PayloadItem(name = 'initLon', dimension = 1, datatype = 'd'),
+        PayloadItem(name = 'initLat', dimension = 1, datatype = 'd'),
+        PayloadItem(name = 'initAlt', dimension = 1, datatype = 'f'),
+        PayloadItem(name = 'stdDev', dimension = 3, datatype = 'f'),
+        PayloadItem(name = 'initHdg', dimension = 1, datatype = 'f'),
+        PayloadItem(name = 'stdDevHdg', dimension = 1, datatype = 'f'),
+        PayloadItem(name = 'leverArm', dimension = 3, datatype = 'f'),
+        PayloadItem(name = 'stdLeverArm', dimension = 3, datatype = 'f'),
+        PayloadItem(name = 'posMode', dimension = 1, datatype = 'B'),
+        PayloadItem(name = 'hdgMode', dimension = 1, datatype = 'B'),
+        PayloadItem(name = 'gnssTimeout', dimension = 1, datatype = 'H'),
+        PayloadItem(name = 'altMSL', dimension = 1, datatype = 'B'),
+        PayloadItem(name = 'realign', dimension = 1, datatype = 'B'),
+        PayloadItem(name = 'inMotion', dimension = 1, datatype = 'B'),
+        PayloadItem(name = 'autoRestart', dimension = 1, datatype = 'B'),
+    ])
 
 @parameter(732)
 class PAREKF_MAGATTAID_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'samplePeriods', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'thrHdg', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'latency', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'thrINSHdg', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'aidingMode', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'updateMode', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'aidingInterval', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'magFieldStdDev', dimension = 3, datatype = 'f'),
     ])
 
-
 @parameter(733)
 class PAREKF_MADCAID_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'altStdDev', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'latency', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'aidInterval', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'reserved2', dimension = 1, datatype = 'H'),
@@ -581,15 +550,14 @@
         PayloadItem(name = 'sfStdDev', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'rwSf', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'bias', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'biasStdDev', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'rwBias', dimension = 1, datatype = 'f'),
     ])
 
-
 @parameter(734)
 class PAREKF_ALIGNMENT_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'method', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'levellingDuration', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'stationaryDuration', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'alignZuptStdDev', dimension = 1, datatype = 'd'),
@@ -597,145 +565,120 @@
         PayloadItem(name = 'enableTrackAlign', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'trackAlignThresh', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'trackAlignDirection', dimension = 3, datatype = 'f'),
         PayloadItem(name = 'reserved2', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'reserved3', dimension = 3, datatype = 'I'),
     ])
 
-
-
 @parameter(737)
 class PAREKF_ZARU_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'enable', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'reserved2', dimension = 3, datatype = 'B'),
     ])
 
 @parameter(739)
 class PAREKF_ZUPTCALIB_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'zuptCalibTime', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'reserved2', dimension = 1, datatype = 'H'),
     ])
 
-"""
-PARDAT
-"""
 @parameter(800)
 class PARDAT_POS_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'posMode', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'altMode', dimension = 1, datatype = 'H'),
     ])
 
-
 @parameter(801)
 class PARDAT_VEL_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'velMode', dimension = 1, datatype = 'I'),
     ])
 
-
 @parameter(802)
 class PARDAT_IMU_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'imuMode', dimension = 1, datatype = 'I'),
     ])
 
-
 @parameter(803)
 class PARDAT_SYSSTAT_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'statMode', dimension = 1, datatype = 'I'),
     ])
 
-
-class PARDAT_STATFPGA_Payload(DefaultParameterPayload):
-    parameter_payload = Message([
-        PayloadItem(name = 'powerStatLower', dimension = 1, datatype = 'I'),
-        PayloadItem(name = 'powerStatUpper', dimension = 1, datatype = 'I'),
-        PayloadItem(name = 'fpgaStatus', dimension = 1, datatype = 'H'),
-        PayloadItem(name = 'supervisorStatus', dimension = 1, datatype = 'H'),
-        PayloadItem(name = 'imuStatus', dimension = 1, datatype = 'B'),
-        PayloadItem(name = 'tempStatus', dimension = 1, datatype = 'B'),
-        PayloadItem(name = 'reserved2', dimension = 1, datatype = 'H'),
-    ])
-
-
-"""
-PARXCOM
-"""
 @parameter(902)
 class PARXCOM_SERIALPORT_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'port', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'switch', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'reserved2', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'baudRate', dimension = 1, datatype = 'I'),
     ])
 
-    def get_name(self):
-        return super().get_name() + '_COM' + str(self.data.get('port'))
-
+    def get_port_number(self):
+        return self.data.get('port')
 
 @parameter(903)
 class PARXCOM_NETCONFIG_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'mode', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'protocol', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'interface', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'speed', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'port', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'ip', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'subnetmask', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'gateway', dimension = 1, datatype = 'I'),
     ])
 
-    def get_name(self):
-        if 0 == self.data.get('interface'):
-            return super().get_name() + '_ETH'
-        else:
-            return super().get_name() + '_USB'
+    def get_name(self = None):
+        if self:
+            if hasattr(self,'data'):
+                if 0 == self.data.get('interface'):
+                    return super().get_name() + '_ETH'
+                else:
+                    return super().get_name() + '_USB'
+        return 'PARXCOM_NETCONFIG'
 
 @parameter(905)
 class PARXCOM_LOGLIST_Payload(DefaultParameterPayload):
     __sub_payload = Message([
-        PayloadItem(name = f'divider', dimension = 1, datatype = 'H'), 
+        PayloadItem(name = f'divider', dimension = 1, datatype = 'H'),
         PayloadItem(name = f'msgid', dimension = 1, datatype = 'H')
         ])
 
     parameter_payload = Message([
         PayloadItem(name = 'logs', dimension = 16, datatype = __sub_payload)
     ])
 
-
 @parameter(906)
 class PARXCOM_AUTOSTART_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'channelNumber', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'autoStart', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'port', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'reserved2', dimension = 1, datatype = 'H'),
     ])
 
-
 @parameter(907)
 class PARXCOM_NTRIP_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'stream', dimension = 128, datatype = 's'),
         PayloadItem(name = 'user', dimension = 128, datatype = 's'),
         PayloadItem(name = 'password', dimension = 128, datatype = 's'),
         PayloadItem(name = 'server', dimension = 128, datatype = 's'),
         PayloadItem(name = 'send_pos_on_login', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'enable', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'remote_port', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'gga_send_period', dimension = 1, datatype = 'I'),
     ])
 
-
 @parameter(908)
 class PARXCOM_POSTPROC_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'enable', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'channel', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'reserved2', dimension = 1, datatype = 'H'),
     ])
@@ -756,143 +699,124 @@
     parameter_payload = Message([
         PayloadItem(name = 'defaultAddress', dimension = 1, datatype = 'I'),
     ])
 
 @parameter(917)
 class PARXCOM_LOGLIST2_Payload(DefaultParameterPayload):
     __sub_payload = Message([
-            PayloadItem(name = f'divider', dimension = 1, datatype = 'H'), 
+            PayloadItem(name = f'divider', dimension = 1, datatype = 'H'),
             PayloadItem(name = f'msgid', dimension = 1, datatype = 'H'),
             PayloadItem(name = f'running', dimension = 1, datatype = 'B'),
             PayloadItem(name = f'reserved2', dimension = 1, datatype = 'B'),
             PayloadItem(name = f'reserved3', dimension = 1, datatype = 'H')
         ])
     parameter_payload = Message([
         PayloadItem(name = 'loglist', dimension = 16, datatype = __sub_payload)
     ])
 
-    def get_name(self):
-        return super().get_name() + '_Channel' + str(self.data.get('reserved_paramheader'))
+    def get_name(self = None):
+        if self:
+            if hasattr(self,"data"):
+                return super().get_name() + '_Channel' + str(self.data.get('reserved_paramheader'))
+        return "PARXCOM_LOGLIST2"            
 
-
-"""
-PARODO
-"""
 @parameter(1100)
 class PARODO_SCF_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'scfOdo', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'scfEst', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'selection', dimension = 1, datatype = 'I'),
     ])
 
-
 @parameter(1101)
 class PARODO_TIMEOUT_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'timeout', dimension = 1, datatype = 'f'),
     ])
 
-
 @parameter(1102)
 class PARODO_MODE_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'enable', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'mode', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'deglitcherA', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'deglitcherB', dimension = 1, datatype = 'H'),
     ])
 
-
 @parameter(1103)
 class PARODO_LEVERARM_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'leverArm', dimension = 3, datatype = 'f'),
     ])
 
-
 @parameter(1104)
 class PARODO_VELSTDDEV_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'stdDev', dimension = 1, datatype = 'f'),
     ])
 
-
 @parameter(1105)
 class PARODO_DIRECTION_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'direction', dimension = 3, datatype = 'f'),
     ])
 
-
 @parameter(1106)
 class PARODO_CONSTRAINTS_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'enable', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'reserved2', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'reserved3', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'stdDev', dimension = 1, datatype = 'f'),
     ])
 
-
 @parameter(1107)
 class PARODO_RATE_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'rate', dimension = 1, datatype = 'f'),
     ])
 
-
 @parameter(1108)
 class PARODO_THR_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'thrAcc', dimension = 1, datatype = 'f'),
         PayloadItem(name = 'thrOmg', dimension = 1, datatype = 'f'),
     ])
 
-
-
-
-
-"""
-PARARINC
-"""
 @parameter(1200)
 class PARARINC825_PORT_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'port', dimension = 1, datatype = 'I'),
     ])
 
-
 @parameter(1201)
 class PARARINC825_BAUD_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'baud', dimension = 1, datatype = 'I'),
     ])
 
-
 @parameter(1202)
 class PARARINC825_ENABLE_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'reserved2', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'enable', dimension = 1, datatype = 'H'),
     ])
 
 @parameter(1204)
 class PARARINC825_LOGLIST_Payload(DefaultParameterPayload):
     __sub_payload = Message([
-            PayloadItem(name = f'divider', dimension = 1, datatype = 'H'), 
-            PayloadItem(name = f'reserved', dimension = 1, datatype = 'H'), 
+            PayloadItem(name = f'divider', dimension = 1, datatype = 'H'),
+            PayloadItem(name = f'reserved', dimension = 1, datatype = 'H'),
             PayloadItem(name = f'docnumber', dimension = 1, datatype = 'I')
             ])
 
     parameter_payload = Message([
         PayloadItem(name = 'logs', dimension = 30, datatype = __sub_payload)
     ])
 
-
 @parameter(1205)
 class PARARINC825_BUSRECOVERY_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'enable', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'reserved2', dimension = 1, datatype = 'H'),
     ])
 
@@ -908,74 +832,67 @@
         PayloadItem(name = 'ScfRPYStdDev', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'ScfInsPosStdDev', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'ScfVelStdDev', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'ScfGnssPosStdDev', dimension = 1, datatype = 'd'),
         PayloadItem(name = 'ScfSideSlip', dimension = 1, datatype = 'd'),
     ])
 
-
 @parameter(1208)
 class PARARINC825_EVENTMASK_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'eventMask', dimension = 1, datatype = 'I'),
     ])
 
-
-
-"""
-PARNMEA
-"""
 @parameter(1300)
 class PARNMEA_COM_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'port', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'enable', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'reserved3', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'baud', dimension = 1, datatype = 'I'),
     ])
 
-    def get_name(self):
-        return super().get_name() + '_COM' + str(self.data.get('port'))
+    def get_name(self = None):
+        if self:
+            if hasattr(self,"data"):
+                return super().get_name() + '_COM' + str(self.data.get('port'))
+        return "PARNMEA_COM"
 
 
 @parameter(1301)
 class PARNMEA_ENABLE_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'reserved2', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'qualityMode', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'selectionSwitch', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'reserved4', dimension = 1, datatype = 'B'),
     ])
 
-
 @parameter(1302)
 class PARNMEA_TXMASK_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'txMask', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'txMaskUDP', dimension = 1, datatype = 'I'),
     ])
 
-
 @parameter(1303)
 class PARNMEA_DECPLACES_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'digitsPos', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'digitsHdg', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'reserved2', dimension = 1, datatype = 'H'),
     ])
 
-
 @parameter(1304)
 class PARNMEA_RATE_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'divisor', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'divisorUDP', dimension = 1, datatype = 'I'),
     ])
 
-
 @parameter(1305)
 class PARNMEA_UDP_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'serverAddress', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'port', dimension = 1, datatype = 'I'),
         PayloadItem(name = 'enable', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'reserved2', dimension = 1, datatype = 'B'),
@@ -984,30 +901,45 @@
 
 @parameter(1306)
 class PARNMEA_VTGSELECT_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'Selector', dimension = 1, datatype = 'I'),
     ])
 
+@parameter(1307)
+class PARNMEA_PRECISION_Payload(DefaultParameterPayload):
+    parameter_payload = Message([
+        PayloadItem(name = 'messageSelect', dimension = 1, datatype = 'B'),
+        PayloadItem(name = 'latitudePrecision', dimension = 1, datatype = 'B'),
+        PayloadItem(name = 'longitudePrecision', dimension = 1, datatype = 'B'),
+        PayloadItem(name = 'undulationPrecision', dimension = 1, datatype = 'B'),
+        PayloadItem(name = 'diffagePrecision', dimension = 1, datatype = 'B'),
+        PayloadItem(name = 'Reserved', dimension = 3, datatype = 'B'),
+    ])
+
 @parameter(1402)
 class PARARINC429_CFG_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'Divisor', dimension = 1, datatype = 'H'),
         PayloadItem(name = 'Channel', dimension = 1, datatype = 'B'),
         PayloadItem(name = 'High Speed', dimension = 1, datatype = 'B'),
     ])
 
-"""
-IO
-"""
 @parameter(1500)
 class PARIO_HW245_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'configIO', dimension = 1, datatype = 'I'),
     ])
 
-
 @parameter(1501)
 class PARIO_HW288_Payload(DefaultParameterPayload):
     parameter_payload = Message([
         PayloadItem(name = 'toDef', dimension = 1, datatype = 'I'),
     ])
+
+
+"""
+PARAMETER FROM JSON FILES
+"""
+path_json = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'json-files', 'parameters')
+parse_parameter_json_folder(path_json)
+
```

### Comparing `ixcom-1.2.0/ixcom/parser.py` & `ixcom-1.3.0/ixcom/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,62 @@
 import collections
 import math
+import numpy
 import queue
 import select
 import socket
 import struct
 import threading
 import time
 from enum import IntEnum
 from typing import Sequence
 
 from . import crc16, data, protocol
 from .data import (BROADCAST_PORT, GENERAL_PORT, LAST_CHANNEL_NUMBER,
                    SYNC_BYTE, WAIT_TIME_FOR_RESPONSE)
 from .exceptions import (ClientTimeoutError, CommunicationError, ParseError,
                          ResponseError)
+from .protocol import ParamID, ProtocolHeader, ProtocolBottom
 
 PositionTuple = collections.namedtuple('PositionTuple', 'Lon Lat Alt')
 
 class MessageSearcherState(IntEnum):
     waiting_for_sync = 0
     waiting_for_msglength = 1
     fetching_bytes = 2
 
+XCOM_MAX_MESSAGE_LENGTH = 4096
+XCOM_HEADER_LENGTH = ProtocolHeader().size()
+XCOM_BOTTOM_LENGTH = ProtocolBottom().size()
+TOTAL_MAX_MESSAGE_LENGTH = XCOM_MAX_MESSAGE_LENGTH + XCOM_HEADER_LENGTH + XCOM_BOTTOM_LENGTH
 
 class MessageSearcher:
     def __init__(self, parserDelegate = None, disable_crc = False):
         self.searcherState = MessageSearcherState.waiting_for_sync
         self.currentBytes = bytearray(512)
         self.currentByteIdx = 0
         self.remainingByteCount = 0
         self.msgLength = 0
         self.disableCRC = disable_crc
         self.callbacks = []
         if parserDelegate is not None:
             self.callbacks.append(parserDelegate.parse)
 
+    def handle_v5_json(self, inBytes):
+        if inBytes[0] == SYNC_BYTE:
+            return 0
+        else:
+            json_hdr_len_pos = 7*4
+            return int.from_bytes(inBytes[json_hdr_len_pos:json_hdr_len_pos+4], byteorder='little')
+
     def process_buffer_unsafe(self, buffer):
         current_msg_start_idx = 0
         inBytes = memoryview(buffer)
         inbytelen = len(inBytes)
+        current_msg_start_idx = self.handle_v5_json(inBytes)
         while current_msg_start_idx + 5 < inbytelen:
             current_msg_length = inBytes[current_msg_start_idx + 4] + 256*inBytes[current_msg_start_idx + 5]
             if current_msg_start_idx + current_msg_length > inbytelen: # Message nicht mehr komplett
                 break
             self.publish(inBytes[current_msg_start_idx:current_msg_start_idx+current_msg_length])
             current_msg_start_idx += current_msg_length
 
@@ -62,16 +76,15 @@
                 inByteIdx += 1
                 self.currentBytes[self.currentByteIdx] = poppedByte
                 self.currentByteIdx += 1
                 self.remainingByteCount -= 1
                 if self.remainingByteCount == 0:
                     self.msgLength = self.currentBytes[self.currentByteIdx - 1] * 256 + self.currentBytes[self.currentByteIdx - 2]
                     self.remainingByteCount = self.msgLength - 6
-                    # 4096 should be replaced if greater messages would be defined
-                    if self.remainingByteCount < 4096 and self.remainingByteCount > 0:
+                    if self.remainingByteCount < TOTAL_MAX_MESSAGE_LENGTH and self.remainingByteCount > 0:
                         self.searcherState = MessageSearcherState.fetching_bytes
                     else:
                         self.searcherState = MessageSearcherState.waiting_for_sync
             elif self.searcherState == MessageSearcherState.fetching_bytes:
                 if len(inBytes) - 1 >= self.remainingByteCount + inByteIdx - 1:  # Der Buffer ist Länger als der Rest der Nachricht.
                     self.currentBytes[self.currentByteIdx:self.currentByteIdx + self.remainingByteCount] = inBytes[inByteIdx:inByteIdx + self.remainingByteCount]
                     self.currentByteIdx = self.currentByteIdx + self.remainingByteCount
@@ -117,43 +130,62 @@
         message.header.from_bytes(inBytes[:16])
         message.payload = data.ResponsePayload(message.header.msgLength)
         message.from_bytes(inBytes)
         self.publish(message)
 
     def parse_parameter(self, inBytes):
         parameterID = inBytes[16] + (inBytes[17] << 8)
-        message = data.getParameterWithID(parameterID)
+        if parameterID != ParamID.PARPLUGIN:
+            message = data.getParameterWithID(parameterID)
+        else:
+            pluginParameterID = inBytes[22] + (inBytes[23] << 8)
+            message = data.getPluginParameterWithID(pluginParameterID)
         if message is not None:
             try:
                 message.from_bytes(inBytes)
                 self.publish(message)
             except Exception:
                 print('Error: Parameter with ID: {} ({}) could not be parsed!'.format(parameterID, message.payload.get_name()))
         else:
-            print('Warning: Parameter with ID: {} not handled!'.format(parameterID))
+            data.handle_undefined_parameter(parameterID)
 
     def parse_command(self, inBytes):
         cmdID = inBytes[16] + (inBytes[17] << 8)
         message = data.getCommandWithID(cmdID)
         if message is not None:
             message.from_bytes(inBytes)
             self.publish(message)
         else:
             pass
 
+    def parse_plugin_message(self, inBytes):
+        plugin_message_id = inBytes[16] + (inBytes[17] << 8)
+        message = data.getPluginMessageWithID(plugin_message_id)
+        if message is not None:
+            try:
+                message.from_bytes(inBytes)
+                self.publish(message)
+            except Exception:
+                print('Error: Plugin Message with ID: {} ({}) could not be parsed!'.format(plugin_message_id, message.payload.get_name()))
+        else:
+            data.handle_undefined_plugin_message(plugin_message_id)
+
+
     def parse(self, inBytes):
         header = data.ProtocolHeader()
         header.from_bytes(inBytes)
         try:
             if header.msgID == data.MessageID.RESPONSE:
                 self.parse_response(inBytes)
             elif header.msgID == data.MessageID.PARAMETER:
                 self.parse_parameter(inBytes)
             elif header.msgID == data.MessageID.COMMAND:
                 self.parse_command(inBytes)
+            elif header.msgID == data.MessageID.PLUGIN:
+                self.parse_plugin_message(inBytes)
             else:
                 message = data.getMessageWithID(header.msgID)
                 if message is not None:
                     message.from_bytes(inBytes)
                     self.publish(message)
         except ParseError as err:
             if self.nothrow:
@@ -236,14 +268,20 @@
         Blocks the calling location until the communications thread terminates.
         Can e.g. be used if callbacks have been set up, logs have been requested and we just want to
         leave the program running like this until the communications with the device stop.
         Args:
             self
         '''
         self._comm_thread.join()
+    
+    def get_commthread_handler(self):
+        return self._comm_thread
+
+    def get_callbackthread_handler(self):
+        return self._callback_thread
 
     def stop(self):
         self._stop_event.set()
         self._comm_thread.join()
         self._callback_thread.join()
 
     def publish(self, message):
@@ -436,14 +474,35 @@
         
         '''
         msgToSend = data.getParameterWithID(parameterID)
         msgToSend.payload.data['action'] = data.ParameterAction.REQUESTING
         self.send_msg_and_waitfor_okay(msgToSend)
         return self.wait_for_parameter()
 
+    def get_plugin_parameter(self, parameterID: int):
+        '''Gets plugin parameter from device with specified ID
+
+        Gets the specified plugin parameter. Blocks until parameter is retrieved.
+
+        Args:
+            parameterID: ID of the plugin parameter to retrieve
+
+        Returns:
+            An XcomMessage object containing the parameter
+
+        Raises:
+            ClientTimeoutError: Timeout while waiting for response or parameter from the XCOM server
+            ResponseError: The response from the system was not 'OK'
+
+        '''
+        msgToSend = data.getPluginParameterWithID(parameterID)
+        msgToSend.payload.data['action'] = data.ParameterAction.REQUESTING
+        self.send_msg_and_waitfor_okay(msgToSend)
+        return self.wait_for_parameter()
+
     def set_aligncomplete(self):
         '''Completes the alignment
 
         Completes system alignment by sending the EKF ALIGN_COMPLETE command. Blocks until system
         repsonse is received.
 
  
@@ -1425,49 +1484,87 @@
 
         '''
         msgToSend = data.getParameterWithID(data.PARODO_LEVERARM_Payload.parameter_id)
         msgToSend.payload.data['action'] = data.ParameterAction.CHANGING
         msgToSend.payload.data['leverArm'] = offset
         self.send_msg_and_waitfor_okay(msgToSend)
 
-    def get_virtual_meas_pt(self):
+    def get_virtual_meas_pt(self, channel=0):
         '''Convenience getter for virtual measpoint offset
 
         Gets the virtual measpoint offset for the output values defined with the mask #
+
+        Args:
+            channel: get parameter for the desired channel (not available in older software versions)
                 
         Raises:
             ClientTimeoutError: Timeout while waiting for response or parameter from the XCOM server
             ResponseError: The response from the system was not 'OK'.
         
         '''
-        return self.get_parameter(data.PAREKF_VMP_Payload.parameter_id)
+        msgToSend = data.getParameterWithID(data.PAREKF_VMP_Payload.parameter_id)
+        msgToSend.payload.data['action'] = data.ParameterAction.REQUESTING
+        msgToSend.payload.data['reserved_paramheader'] = channel
+        self.send_msg_and_waitfor_okay(msgToSend)
+
+        return self.wait_for_parameter()
 
-    def set_virtual_meas_pt(self, offset=[0, 0, 0], activationMask=0, cutOffFreq=0):
+    def set_virtual_meas_pt(self, offset=[0, 0, 0], activationMask=0, cutOffFreq=0, channel=0xFF):
         '''Convenience setter for virtual measpoint offset
 
         Sets the virtual measpoint offset #
         
         Args:
             offset: Distance between INS center of measurement and virtual measurement point [m, m, m].
             activationMask: Bit 0 -> INS/GNSS Position, Bit 1 -> INS/GNSS Velocity, Bit 2 -> Specific Force, Bit 3 -> Angular Rate
             cutOffFreq: The parameter CUTOFF-FREQ specifies the cut-off 1st frequency in [Hz] of the 1 order low pass. The low pass
                         is used to filter ω for the transformation. Due to the noise, the derivation of ω will not be transformed.
+            channel: Set the settings to a specific channel or all channels (0xFF) (not available in older software versions)
         
         Raises:
             ClientTimeoutError: Timeout while waiting for response or parameter from the XCOM server
             ResponseError: The response from the system was not 'OK'.
         
         '''
         msgToSend = data.getParameterWithID(data.PAREKF_VMP_Payload.parameter_id)
         msgToSend.payload.data['action'] = data.ParameterAction.CHANGING
+        msgToSend.payload.data['reserved_paramheader'] = channel
         msgToSend.payload.data['leverArm'] = offset
         msgToSend.payload.data['mask'] = activationMask
         msgToSend.payload.data['cutoff'] = cutOffFreq
         self.send_msg_and_waitfor_okay(msgToSend)
 
+### ride_control Plugin parameters
+    ANGLIM_DEFAULT = numpy.deg2rad(10.0)
+    def set_PARPLUGIN_IATANGLIM(
+            self,
+            angLimLowMain: Sequence[float] = [-ANGLIM_DEFAULT, -ANGLIM_DEFAULT, -ANGLIM_DEFAULT, -ANGLIM_DEFAULT],
+            angLimUpMain: Sequence[float] = [ANGLIM_DEFAULT, ANGLIM_DEFAULT, ANGLIM_DEFAULT, ANGLIM_DEFAULT],
+            angLimLowAux: Sequence[float] = [-ANGLIM_DEFAULT, -ANGLIM_DEFAULT, -ANGLIM_DEFAULT, -ANGLIM_DEFAULT],
+            angLimUpAux: Sequence[float] = [ANGLIM_DEFAULT, ANGLIM_DEFAULT, ANGLIM_DEFAULT, ANGLIM_DEFAULT]):
+        '''Change angulare limits of actuators
+
+        Changes the angular limits of the actuators. Blocks until system
+        repsonse is received.
+
+
+        Raises:
+            ClientTimeoutError: Timeout while waiting for response from the XCOM server
+            ResponseError: The response from the system was not 'OK'
+
+        '''
+        msgToSend = data.getPluginParameterWithID(data.PARPLUGIN_IATANGLIM_Payload.plugin_parameter_id)
+        msgToSend.payload.data['angLimLowMain'] = angLimLowMain
+        msgToSend.payload.data['angLimUpMain'] = angLimUpMain
+        msgToSend.payload.data['angLimLowAux'] = angLimLowAux
+        msgToSend.payload.data['angLimUpAux'] = angLimUpAux
+
+        msgToSend.payload.data['action'] = data.ParameterAction.CHANGING
+        self.send_msg_and_waitfor_okay(msgToSend)
+
 def broadcast_search(timeout=0.1, port=BROADCAST_PORT, addr='<broadcast>'):
     s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
     s.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, True)
     s.settimeout(timeout)
 
     s.sendto('hello'.encode('utf-8'), (addr, port))
     time.sleep(timeout)
```

### Comparing `ixcom-1.2.0/ixcom.egg-info/PKG-INFO` & `ixcom-1.3.0/ixcom.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 Metadata-Version: 2.1
 Name: ixcom
-Version: 1.2.0
+Version: 1.3.0
 Summary: Library for communicating with xcom devices over network
 Home-page: http://www.imar-navigation.de
 Author: iMAR Navigation GmbH
 Author-email: support@imar-navigation.de
 License: UNKNOWN
 Project-URL: Documentation, https://ixcom.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/imar-navigation/ixcom-python
-Description: This library can be used to communicate with iMAR devices speaking the iXCOM protocol.
-        
-        Example usage:
-        ```python
-        import ixcom
-        
-        client = ixcom.Client('192.168.1.30')
-        client.open_last_free_channel()
-        client.realign()
-        ```
-        
-        Alongside this package, some command line tools will be installed in the user's path:
-        * configdump2txt: Converts a config.dump into a text form
-        * monitor2xcom: Converts iXCOM frames in a monitor.log into human readable format
-        * xcom_lookup: Looks for iXCOM devives on the local network
-        * split_config: Filters certain parameter IDs from a config.dump
 Keywords: XCOM,Inertial navigation,INS,iMAR,iNAT,GNSS,GPS,AHRS
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+Provides-Extra: fastcrc
+License-File: LICENSE
+
+This library can be used to communicate with iMAR devices speaking the iXCOM protocol.
+
+Example usage:
+```python
+import ixcom
+
+client = ixcom.Client('192.168.1.30')
+client.open_last_free_channel()
+client.realign()
+```
+
+Alongside this package, some command line tools will be installed in the user's path:
+* configdump2txt: Converts a config.dump into a text form
+* monitor2xcom: Converts iXCOM frames in a monitor.log into human readable format
+* xcom_lookup: Looks for iXCOM devives on the local network
+* split_config: Filters certain parameter IDs from a config.dump
+
```

### Comparing `ixcom-1.2.0/setup.py` & `ixcom-1.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 if __name__ == '__main__':
 
     readmePath = os.path.join(os.path.dirname(__file__), 'README.md')
     long_description = open(readmePath, "rt").read()
 
     setup(name='ixcom',
-          version='1.2.0',
+          version='1.3.0',
           description='Library for communicating with xcom devices over network',
           author='iMAR Navigation GmbH',
           author_email='support@imar-navigation.de',
           url='http://www.imar-navigation.de',
           keywords=['XCOM', 'Inertial navigation', 'INS', 'iMAR', 'iNAT', 'GNSS', 'GPS', 'AHRS'],
           packages=['ixcom'],
           entry_points={
@@ -28,14 +28,17 @@
                         'xcom_lookup = ixcom.cmdline:xcom_lookup',
                         'split_config = ixcom.cmdline:split_config',
                                 ],
                         },
           install_requires=[
                     'numpy>=1.16.2',
                 ],
+          extras_require={
+                    'fastcrc': ['fastcrc']
+          },
           classifiers=[
                 "Programming Language :: Python :: 3.6",
                 "License :: OSI Approved :: MIT License",
                 "Operating System :: OS Independent",
                 ],
           long_description=long_description,
           long_description_content_type="text/markdown",
```

