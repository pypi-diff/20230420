# Comparing `tmp/bitio-0.2.tar.gz` & `tmp/bitio-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bitio-0.2.tar", last modified: Sun May  1 10:17:01 2016, max compression
+gzip compressed data, was "bitio-0.3.0.tar", last modified: Thu Apr 20 13:33:48 2023, max compression
```

## Comparing `bitio-0.2.tar` & `bitio-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,14 @@
-drwxr-xr-x   0 daiju      (501) staff       (20)        0 2016-05-01 10:17:01.000000 bitio-0.2/
-drwxr-xr-x   0 daiju      (501) staff       (20)        0 2016-05-01 10:17:01.000000 bitio-0.2/bitio/
--rw-r--r--   0 daiju      (501) staff       (20)     1373 2016-05-01 09:44:10.000000 bitio-0.2/bitio/__init__.py
--rw-r--r--   0 daiju      (501) staff       (20)     2944 2016-05-01 08:22:37.000000 bitio-0.2/bitio/bit_file.py
--rw-r--r--   0 daiju      (501) staff       (20)      461 2016-05-01 09:34:04.000000 bitio-0.2/bitio/byte_wrapper.py
--rw-r--r--   0 daiju      (501) staff       (20)      470 2016-05-01 10:17:01.000000 bitio-0.2/PKG-INFO
--rw-r--r--   0 daiju      (501) staff       (20)      661 2016-05-01 09:48:41.000000 bitio-0.2/README.md
--rw-r--r--   0 daiju      (501) staff       (20)      566 2016-05-01 10:15:48.000000 bitio-0.2/setup.py
+drwxr-xr-x   0 daiju      (501) staff       (20)        0 2023-04-20 13:33:48.044688 bitio-0.3.0/
+-rw-r--r--   0 daiju      (501) staff       (20)     1158 2023-04-20 13:33:48.044475 bitio-0.3.0/PKG-INFO
+-rw-r--r--   0 daiju      (501) staff       (20)      687 2023-04-20 12:56:48.000000 bitio-0.3.0/README.md
+drwxr-xr-x   0 daiju      (501) staff       (20)        0 2023-04-20 13:33:48.042947 bitio-0.3.0/bitio/
+-rw-r--r--   0 daiju      (501) staff       (20)     1411 2023-04-20 13:32:53.000000 bitio-0.3.0/bitio/__init__.py
+-rw-r--r--   0 daiju      (501) staff       (20)     2900 2023-04-20 13:16:09.000000 bitio-0.3.0/bitio/bit_file.py
+-rw-r--r--   0 daiju      (501) staff       (20)      466 2023-04-20 13:16:00.000000 bitio-0.3.0/bitio/byte_wrapper.py
+drwxr-xr-x   0 daiju      (501) staff       (20)        0 2023-04-20 13:33:48.044220 bitio-0.3.0/bitio.egg-info/
+-rw-r--r--   0 daiju      (501) staff       (20)     1158 2023-04-20 13:33:48.000000 bitio-0.3.0/bitio.egg-info/PKG-INFO
+-rw-r--r--   0 daiju      (501) staff       (20)      192 2023-04-20 13:33:48.000000 bitio-0.3.0/bitio.egg-info/SOURCES.txt
+-rw-r--r--   0 daiju      (501) staff       (20)        1 2023-04-20 13:33:48.000000 bitio-0.3.0/bitio.egg-info/dependency_links.txt
+-rw-r--r--   0 daiju      (501) staff       (20)        6 2023-04-20 13:33:48.000000 bitio-0.3.0/bitio.egg-info/top_level.txt
+-rw-r--r--   0 daiju      (501) staff       (20)       38 2023-04-20 13:33:48.044747 bitio-0.3.0/setup.cfg
+-rw-r--r--   0 daiju      (501) staff       (20)      661 2023-04-20 13:32:58.000000 bitio-0.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bitio-0.2/bitio/__init__.py` & `bitio-0.3.0/bitio/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 #
 # bitio/bit_file.py
 #
-"""\
-Input/output utirites of a bit-basis file.
+"""
+Input/output utilities of a bit-basis file.
 
 ------------------------------------------
 how to use:
 
 from bitio import bit_open, bit_wrap, ByteWrapper
 
 f = bit_open(file_name, "r")
@@ -19,47 +19,44 @@
 f.write_bits(bits, count) # write 'count bits'
 f.close()
 
 l = []
 wrapper = ByteWrapper(l.append)
 f = bit_wrap(wrapper, "w")
 f.write_bits(0b110000101, 10)
-print l # ["a"]
+print(l)    # [b"a"]
 f.close()
-print l # ["a", "@"]
+print(l)    # [b"a", b"@"]
 """
 
-
 from .bit_file import BitFileReader, BitFileWriter
 from .byte_wrapper import ByteWrapper
 
-VERSION = (0, 2, 0)
+VERSION = (0, 3, 0)
 
 
 def bit_open(name, mode="r"):
-    """\
-name: file name
-mode: "r" -> read mode
-      "w" -> write mode
-"""
+    """
+    name: file name
+    mode: "r" -> read mode
+          "w" -> write mode
+    """
     if mode in ["w", "wb"]:
         return BitFileWriter(name)
     elif mode in ["r", "rb"]:
         return BitFileReader(name)
     else:
-        raise ValueError("Invalid bit-file mode '%s'"%(mode))
+        raise ValueError("Invalid bit-file mode '%s'" % mode)
+
 
 def bit_wrap(byte_file, mode="r"):
-    """\
-byte_file: byte basis file-like object
-mode: "r" -> read mode
-      "w" -> write mode
-"""
+    """
+    byte_file: byte basis file-like object
+    mode: "r" -> read mode
+          "w" -> write mode
+    """
     if mode in ["w", "wb"]:
         return BitFileWriter.from_file(byte_file)
     elif mode in ["r", "rb"]:
         return BitFileReader.from_file(byte_file)
     else:
-        raise ValueError("Invalid bit-file mode '%s'"%(mode))
-
-
-
+        raise ValueError("Invalid bit-file mode '%s'" % mode)
```

### Comparing `bitio-0.2/bitio/bit_file.py` & `bitio-0.3.0/bitio/bit_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # -*- coding: utf-8 -*-
 #
 # bitio/bit_file.py
 #
 class _BaseBitFile(object):
     def __enter__(self):
         return self
+
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
         return False
+
     def __del__(self):
         self.close()
 
+
 class BitFileReader(_BaseBitFile):
-    
+
     def __init__(self, name):
         self.name = name
         self.byte_file = open(name, "rb")
         self.rack = 0
         self.mask = 0
 
     @classmethod
@@ -25,33 +28,33 @@
             raise TypeError("must have 'read' method")
         reader = cls.__new__(cls)
         reader.name = None
         reader.byte_file = byte_file
         reader.rack = 0
         reader.mask = 0
         return reader
-    
+
     def close(self):
         if hasattr(self.byte_file, "close"):
             self.byte_file.close()
-    
+
     def _read_byte(self):
         c = self.byte_file.read(1)
-        if c == '':
-            raise IOError("Bit file is empty!")
+        if not c:
+            raise EOFError("Bit file is empty!")
         return ord(c)
-        
+
     def read(self):
         if self.mask == 0:
             self.mask = 0x80
             self.rack = self._read_byte()
         ret = 1 if (self.rack & self.mask) else 0
         self.mask >>= 1
         return ret
-    
+
     def read_bits(self, count):
         if count <= 0:
             return 0
         ret = 0
         mask = 1 << (count - 1)
         while mask > 0:
             if self.mask == 0:
@@ -61,50 +64,50 @@
                 ret |= mask
             self.mask >>= 1
             mask >>= 1
         return ret
 
 
 class BitFileWriter(_BaseBitFile):
-    
+
     def __init__(self, name):
         self.name = name
         self.byte_file = open(name, "wb")
         self.rack = 0
         self.mask = 0x80
-    
+
     @classmethod
     def from_file(cls, byte_file):
         if not hasattr(byte_file, "write"):
             raise TypeError("must have 'write' method")
         writer = cls.__new__(cls)
         writer.name = None
         writer.byte_file = byte_file
         writer.rack = 0
         writer.mask = 0x80
         return writer
 
     def _flush_byte(self):
-        self.byte_file.write(chr(self.rack))
+        self.byte_file.write(self.rack.to_bytes())
         self.rack = 0
         self.mask = 0x80
-        
+
     def close(self):
         if self.mask != 0x80:
             self._flush_byte()
         if hasattr(self.byte_file, "close"):
             self.byte_file.close()
-        
+
     def write(self, bit):
         if bit:
             self.rack |= self.mask
         self.mask >>= 1
         if self.mask == 0:
             self._flush_byte()
-    
+
     def write_bits(self, code, count):
         if count <= 0:
             return
         mask = 1 << (count - 1)
         while mask > 0:
             if code & mask:
                 self.rack |= self.mask
```

### Comparing `bitio-0.2/README.md` & `bitio-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # bitio
 
-Input/output utirites of bit basis file
+Utilities to read or write files by bit or bits
 
 ## How to use
 
 ```py
 from bitio import bit_open
 
 f = bit_open(file_name, "r")
@@ -13,30 +13,30 @@
 
 f = bit_open(file_name, "w")
 f.write(bit)              # write 1 if bit else 0
 f.write_bits(bits, count) # write 'count bits'
 f.close()
 ```
 
-These are same
+These are the same
 
 ```py
 f.write_bits(bits, count)
 
 for i in range(count-1, -1, -1):
   if bits & (1 << i):
     f.write(1)
   else:
     f.write(0)
 ```
 
-othe interface
+Another interface
 
 ```py
 l = []
 wrapper = ByteWrapper(l.append)
 f = bit_wrap(wrapper, "w")
 f.write_bits(0b110000101, 10)
-print l # ["a"]
+print(l)    # [b"a"]
 f.close()
-print l # ["a", "@"]
+print(l)    # [b"a", b"@"]
 ```
```

### Comparing `bitio-0.2/setup.py` & `bitio-0.3.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # -*- coding: utf-8 -*-
 #
 # setup.py
 #
-from distutils.core import setup
+from setuptools import setup
 
 setup(
-    name = "bitio",
-    packages = ["bitio"],
-    version = "0.2",
-    description = "Input/output utirites of a bit-basis file",
-    author = "Daiju Nakayama",
-    author_email = "42.daiju@gmail.com",
-    url = "https://github.com/hinohi/bitio",
-    classifiers = [
-        "Programming Language :: Python",
+    name="bitio",
+    packages=["bitio"],
+    version="0.3.0",
+    description="Input/output utilities of a bit-basis file",
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
+    author="Daiju Nakayama",
+    author_email="42.daiju@gmail.com",
+    url="https://github.com/hinohi/bitio",
+    classifiers=[
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Topic :: Utilities",
     ]
-)
+)
```

