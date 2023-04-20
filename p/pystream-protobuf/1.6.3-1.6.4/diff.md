# Comparing `tmp/pystream-protobuf-1.6.3.tar.gz` & `tmp/pystream-protobuf-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pystream-protobuf-1.6.3.tar", last modified: Thu Jan 28 11:13:45 2021, max compression
+gzip compressed data, was "pystream-protobuf-1.6.4.tar", last modified: Thu Apr 20 17:35:24 2023, max compression
```

## Comparing `pystream-protobuf-1.6.3.tar` & `pystream-protobuf-1.6.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 cartoonist  (1000) cartoonist  (1001)        0 2021-01-28 11:13:45.828936 pystream-protobuf-1.6.3/
--rw-r--r--   0 cartoonist  (1000) cartoonist  (1001)     1070 2020-08-10 11:08:21.000000 pystream-protobuf-1.6.3/LICENSE
--rw-r--r--   0 cartoonist  (1000) cartoonist  (1001)      127 2020-08-10 11:08:21.000000 pystream-protobuf-1.6.3/MANIFEST.in
--rw-r--r--   0 cartoonist  (1000) cartoonist  (1001)     4774 2021-01-28 11:13:45.828936 pystream-protobuf-1.6.3/PKG-INFO
--rw-r--r--   0 cartoonist  (1000) cartoonist  (1001)     3325 2021-01-28 11:05:39.000000 pystream-protobuf-1.6.3/README.md
-drwxr-xr-x   0 cartoonist  (1000) cartoonist  (1001)        0 2021-01-28 11:13:45.828936 pystream-protobuf-1.6.3/pystream_protobuf.egg-info/
--rw-r--r--   0 cartoonist  (1000) cartoonist  (1001)     4774 2021-01-28 11:13:45.000000 pystream-protobuf-1.6.3/pystream_protobuf.egg-info/PKG-INFO
--rw-r--r--   0 cartoonist  (1000) cartoonist  (1001)      367 2021-01-28 11:13:45.000000 pystream-protobuf-1.6.3/pystream_protobuf.egg-info/SOURCES.txt
--rw-r--r--   0 cartoonist  (1000) cartoonist  (1001)        1 2021-01-28 11:13:45.000000 pystream-protobuf-1.6.3/pystream_protobuf.egg-info/dependency_links.txt
--rw-r--r--   0 cartoonist  (1000) cartoonist  (1001)       44 2021-01-28 11:13:45.000000 pystream-protobuf-1.6.3/pystream_protobuf.egg-info/entry_points.txt
--rw-r--r--   0 cartoonist  (1000) cartoonist  (1001)       85 2021-01-28 11:13:45.000000 pystream-protobuf-1.6.3/pystream_protobuf.egg-info/requires.txt
--rw-r--r--   0 cartoonist  (1000) cartoonist  (1001)        7 2021-01-28 11:13:45.000000 pystream-protobuf-1.6.3/pystream_protobuf.egg-info/top_level.txt
--rw-r--r--   0 cartoonist  (1000) cartoonist  (1001)      156 2021-01-28 11:13:45.828936 pystream-protobuf-1.6.3/setup.cfg
--rw-r--r--   0 cartoonist  (1000) cartoonist  (1001)     1670 2020-08-10 11:08:21.000000 pystream-protobuf-1.6.3/setup.py
-drwxr-xr-x   0 cartoonist  (1000) cartoonist  (1001)        0 2021-01-28 11:13:45.828936 pystream-protobuf-1.6.3/stream/
--rw-r--r--   0 cartoonist  (1000) cartoonist  (1001)      502 2020-08-10 11:08:22.000000 pystream-protobuf-1.6.3/stream/__init__.py
--rw-r--r--   0 cartoonist  (1000) cartoonist  (1001)     1974 2021-01-28 11:05:39.000000 pystream-protobuf-1.6.3/stream/release.py
--rw-r--r--   0 cartoonist  (1000) cartoonist  (1001)    13483 2021-01-28 11:05:39.000000 pystream-protobuf-1.6.3/stream/stream.py
--rw-r--r--   0 cartoonist  (1000) cartoonist  (1001)     1366 2020-08-10 11:08:22.000000 pystream-protobuf-1.6.3/stream/varint.py
+drwxr-xr-x   0 cartoonist   (501) staff       (20)        0 2023-04-20 17:35:24.458869 pystream-protobuf-1.6.4/
+-rw-r--r--   0 cartoonist   (501) staff       (20)     1070 2021-10-26 13:51:37.000000 pystream-protobuf-1.6.4/LICENSE
+-rw-r--r--   0 cartoonist   (501) staff       (20)      127 2021-10-26 13:51:37.000000 pystream-protobuf-1.6.4/MANIFEST.in
+-rw-r--r--   0 cartoonist   (501) staff       (20)     4202 2023-04-20 17:35:24.458928 pystream-protobuf-1.6.4/PKG-INFO
+-rw-r--r--   0 cartoonist   (501) staff       (20)     3354 2023-04-20 17:17:04.000000 pystream-protobuf-1.6.4/README.md
+drwxr-xr-x   0 cartoonist   (501) staff       (20)        0 2023-04-20 17:35:24.457971 pystream-protobuf-1.6.4/pystream_protobuf.egg-info/
+-rw-r--r--   0 cartoonist   (501) staff       (20)     4202 2023-04-20 17:35:24.000000 pystream-protobuf-1.6.4/pystream_protobuf.egg-info/PKG-INFO
+-rw-r--r--   0 cartoonist   (501) staff       (20)      367 2023-04-20 17:35:24.000000 pystream-protobuf-1.6.4/pystream_protobuf.egg-info/SOURCES.txt
+-rw-r--r--   0 cartoonist   (501) staff       (20)        1 2023-04-20 17:35:24.000000 pystream-protobuf-1.6.4/pystream_protobuf.egg-info/dependency_links.txt
+-rw-r--r--   0 cartoonist   (501) staff       (20)       45 2023-04-20 17:35:24.000000 pystream-protobuf-1.6.4/pystream_protobuf.egg-info/entry_points.txt
+-rw-r--r--   0 cartoonist   (501) staff       (20)       85 2023-04-20 17:35:24.000000 pystream-protobuf-1.6.4/pystream_protobuf.egg-info/requires.txt
+-rw-r--r--   0 cartoonist   (501) staff       (20)        7 2023-04-20 17:35:24.000000 pystream-protobuf-1.6.4/pystream_protobuf.egg-info/top_level.txt
+-rw-r--r--   0 cartoonist   (501) staff       (20)      156 2023-04-20 17:35:24.459136 pystream-protobuf-1.6.4/setup.cfg
+-rw-r--r--   0 cartoonist   (501) staff       (20)     1670 2021-10-26 13:51:37.000000 pystream-protobuf-1.6.4/setup.py
+drwxr-xr-x   0 cartoonist   (501) staff       (20)        0 2023-04-20 17:35:24.458728 pystream-protobuf-1.6.4/stream/
+-rw-r--r--   0 cartoonist   (501) staff       (20)      502 2021-10-26 13:51:37.000000 pystream-protobuf-1.6.4/stream/__init__.py
+-rw-r--r--   0 cartoonist   (501) staff       (20)     1974 2023-04-20 17:21:37.000000 pystream-protobuf-1.6.4/stream/release.py
+-rw-r--r--   0 cartoonist   (501) staff       (20)    13797 2023-04-20 17:17:04.000000 pystream-protobuf-1.6.4/stream/stream.py
+-rw-r--r--   0 cartoonist   (501) staff       (20)     1366 2021-10-26 13:51:37.000000 pystream-protobuf-1.6.4/stream/varint.py
```

### Comparing `pystream-protobuf-1.6.3/LICENSE` & `pystream-protobuf-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pystream-protobuf-1.6.3/PKG-INFO` & `pystream-protobuf-1.6.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,96 +1,97 @@
 Metadata-Version: 2.1
 Name: pystream-protobuf
-Version: 1.6.3
+Version: 1.6.4
 Summary: Python implementation of stream library
 Home-page: https://github.com/cartoonist/pystream-protobuf
+Download-URL: https://github.com/cartoonist/pystream-protobuf/tarball/1.6.4
 Author: Ali Ghaffaari
 Author-email: ali.ghaffaari@mpi-inf.mpg.de
 License: MIT
-Download-URL: https://github.com/cartoonist/pystream-protobuf/tarball/1.6.3
-Description: [![Build Status](https://img.shields.io/travis/cartoonist/pystream-protobuf.svg?style=flat-square)](https://travis-ci.org/cartoonist/pystream-protobuf)
-        [![PyPI Release](https://img.shields.io/pypi/v/pystream-protobuf.svg?style=flat-square)](https://pypi.python.org/pypi/pystream-protobuf)
-        [![PyPI Status](https://img.shields.io/pypi/status/pystream-protobuf.svg?style=flat-square)](https://pypi.python.org/pypi/pystream-protobuf)
-        [![Python](https://img.shields.io/pypi/pyversions/pystream-protobuf.svg?style=flat-square)](https://www.python.org/download/releases/3.0/)
-        [![License](https://img.shields.io/pypi/l/pystream-protobuf.svg?style=flat-square)](https://github.com/cartoonist/pystream-protobuf/blob/master/LICENSE)
-        
-        # pyStream
-        Python implementation of [stream library](https://github.com/vgteam/stream).
-        
-        ## Introduction
-        This library enables _stream processing_ of protobuf messages (or any serializable
-        objects since v1.6.3); i.e. multiple protobuf messages can be written/read into/from a
-        single stream or file.
-        
-        It was originally developed to parse/write [vg](https://github.com/vgteam/vg)
-        file formats (`.vg`, `.gam`, etc). However, it can be used for any arbitrary
-        protocol buffer messages.
-        
-        Refer to the C++ [stream library](https://github.com/vgteam/stream) for more
-        details.
-        
-        ---
-        **NOTE**
-        
-        **@vg users:** The new version of stream library, now as a part of
-        [libvgio](https://github.com/vgteam/libvgio), writes a header at the start of
-        the stream depending on the output format. For example, headers like `b'GAM'`
-        or `b'VG'` can be found before the actual protobuf messages in GAM and VG files
-        repectively. In this case, you should provide the expected value using `header`
-        keyword argument; e.g.
-        `stream.parse('file.gam', vg_pb2.Alignment, header=b'GAM')`
-        for GAM files (since version v1.6.2).
-        
-        ---
-        
-        ## Encoding
-        The encoding is simple. Messages are written in groups of different sizes. Each
-        group starts with its size; i.e. the number of messages in that group. Then, the
-        size of each message is followed by the encoded message itself. Quoted from
-        [Google Protobuf Developer Guide](https://developers.google.com/protocol-buffers/docs/techniques#streaming):
-        
-        > The Protocol Buffer wire format is not self-delimiting, so protocol buffer
-        > parsers cannot determine where a message ends on their own. The easiest way to
-        > solve this problem is to write the size of each message before you write the
-        > message itself. When you read the messages back in, you read the size, then
-        > read the bytes into a separate buffer, then parse from that buffer.
-        
-        By default, the stream is considered compressed by GZip. However, uncompressed
-        stream processing is possible by passing `gzip=False` to any API calls.
-        
-        ## Installation
-        You can install pyStream using `pip`:
-        
-            pip install pystream-protobuf
-        
-        ## Usage
-        See [Wiki](https://github.com/cartoonist/pystream-protobuf/wiki) for usage documentation.
-        
-        ## Development
-        In case, you work with the source code and need to build the package:
-        
-            python setup.py build
-        
-        The proto files in the test module required to be compiled before running test
-        cases. To do so, it is required to have Google protobuf compiler (>=3.0.2)
-        installed. After installing protobuf compiler, run:
-        
-            make init
-        
-        to compile proto files required for test module and then:
-        
-            make test
-        
-        to run tests.
-        
 Keywords: stream protocol buffer protobuf
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
+
+[![Build Status](https://img.shields.io/travis/cartoonist/pystream-protobuf.svg?style=flat-square)](https://travis-ci.org/cartoonist/pystream-protobuf)
+[![PyPI Release](https://img.shields.io/pypi/v/pystream-protobuf.svg?style=flat-square)](https://pypi.python.org/pypi/pystream-protobuf)
+[![PyPI Status](https://img.shields.io/pypi/status/pystream-protobuf.svg?style=flat-square)](https://pypi.python.org/pypi/pystream-protobuf)
+[![Python](https://img.shields.io/pypi/pyversions/pystream-protobuf.svg?style=flat-square)](https://www.python.org/download/releases/3.0/)
+[![License](https://img.shields.io/pypi/l/pystream-protobuf.svg?style=flat-square)](https://github.com/cartoonist/pystream-protobuf/blob/master/LICENSE)
+
+# pyStream
+Python implementation of [stream library](https://github.com/vgteam/stream).
+
+## Introduction
+This library enables _stream processing_ of protobuf messages (or any serializable
+objects since v1.6.3); i.e. multiple protobuf messages can be written/read into/from a
+single stream or file.
+
+It was originally developed to parse/write [vg](https://github.com/vgteam/vg)
+file formats (`.vg`, `.gam`, etc). However, it can be used for any arbitrary
+protocol buffer messages.
+
+Refer to the C++ [stream library](https://github.com/vgteam/stream) for more
+details.
+
+---
+
+**NOTE**
+
+**@vg users:** The new version of stream library, now as a part of
+[libvgio](https://github.com/vgteam/libvgio), writes a header tag at the start of
+the stream depending on the output format. For example, headers like `b'GAM'`
+or `b'VG'` can be found before the actual protobuf messages in GAM and VG files
+repectively. In this case, you should provide the expected value using `header`
+keyword argument; e.g.
+`stream.parse('file.gam', vg_pb2.Alignment, header=b'GAM', persistent_header=True)`
+for GAM files (since version v1.6.2).
+
+---
+
+## Encoding
+The encoding is simple. Messages are written in groups of different sizes. Each
+group starts with its size; i.e. the number of messages in that group. Then, the
+size of each message is followed by the encoded message itself. Quoted from
+[Google Protobuf Developer Guide](https://developers.google.com/protocol-buffers/docs/techniques#streaming):
+
+> The Protocol Buffer wire format is not self-delimiting, so protocol buffer
+> parsers cannot determine where a message ends on their own. The easiest way to
+> solve this problem is to write the size of each message before you write the
+> message itself. When you read the messages back in, you read the size, then
+> read the bytes into a separate buffer, then parse from that buffer.
+
+By default, the stream is considered compressed by GZip. However, uncompressed
+stream processing is possible by passing `gzip=False` to any API calls.
+
+## Installation
+You can install pyStream using `pip`:
+
+    pip install pystream-protobuf
+
+## Usage
+See [Wiki](https://github.com/cartoonist/pystream-protobuf/wiki) for usage documentation.
+
+## Development
+In case, you work with the source code and need to build the package:
+
+    python setup.py build
+
+The proto files in the test module required to be compiled before running test
+cases. To do so, it is required to have Google protobuf compiler (>=3.0.2)
+installed. After installing protobuf compiler, run:
+
+    make init
+
+to compile proto files required for test module and then:
+
+    make test
+
+to run tests.
```

### Comparing `pystream-protobuf-1.6.3/README.md` & `pystream-protobuf-1.6.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -16,23 +16,24 @@
 file formats (`.vg`, `.gam`, etc). However, it can be used for any arbitrary
 protocol buffer messages.
 
 Refer to the C++ [stream library](https://github.com/vgteam/stream) for more
 details.
 
 ---
+
 **NOTE**
 
 **@vg users:** The new version of stream library, now as a part of
-[libvgio](https://github.com/vgteam/libvgio), writes a header at the start of
+[libvgio](https://github.com/vgteam/libvgio), writes a header tag at the start of
 the stream depending on the output format. For example, headers like `b'GAM'`
 or `b'VG'` can be found before the actual protobuf messages in GAM and VG files
 repectively. In this case, you should provide the expected value using `header`
 keyword argument; e.g.
-`stream.parse('file.gam', vg_pb2.Alignment, header=b'GAM')`
+`stream.parse('file.gam', vg_pb2.Alignment, header=b'GAM', persistent_header=True)`
 for GAM files (since version v1.6.2).
 
 ---
 
 ## Encoding
 The encoding is simple. Messages are written in groups of different sizes. Each
 group starts with its size; i.e. the number of messages in that group. Then, the
```

### Comparing `pystream-protobuf-1.6.3/pystream_protobuf.egg-info/PKG-INFO` & `pystream-protobuf-1.6.4/pystream_protobuf.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,96 +1,97 @@
 Metadata-Version: 2.1
 Name: pystream-protobuf
-Version: 1.6.3
+Version: 1.6.4
 Summary: Python implementation of stream library
 Home-page: https://github.com/cartoonist/pystream-protobuf
+Download-URL: https://github.com/cartoonist/pystream-protobuf/tarball/1.6.4
 Author: Ali Ghaffaari
 Author-email: ali.ghaffaari@mpi-inf.mpg.de
 License: MIT
-Download-URL: https://github.com/cartoonist/pystream-protobuf/tarball/1.6.3
-Description: [![Build Status](https://img.shields.io/travis/cartoonist/pystream-protobuf.svg?style=flat-square)](https://travis-ci.org/cartoonist/pystream-protobuf)
-        [![PyPI Release](https://img.shields.io/pypi/v/pystream-protobuf.svg?style=flat-square)](https://pypi.python.org/pypi/pystream-protobuf)
-        [![PyPI Status](https://img.shields.io/pypi/status/pystream-protobuf.svg?style=flat-square)](https://pypi.python.org/pypi/pystream-protobuf)
-        [![Python](https://img.shields.io/pypi/pyversions/pystream-protobuf.svg?style=flat-square)](https://www.python.org/download/releases/3.0/)
-        [![License](https://img.shields.io/pypi/l/pystream-protobuf.svg?style=flat-square)](https://github.com/cartoonist/pystream-protobuf/blob/master/LICENSE)
-        
-        # pyStream
-        Python implementation of [stream library](https://github.com/vgteam/stream).
-        
-        ## Introduction
-        This library enables _stream processing_ of protobuf messages (or any serializable
-        objects since v1.6.3); i.e. multiple protobuf messages can be written/read into/from a
-        single stream or file.
-        
-        It was originally developed to parse/write [vg](https://github.com/vgteam/vg)
-        file formats (`.vg`, `.gam`, etc). However, it can be used for any arbitrary
-        protocol buffer messages.
-        
-        Refer to the C++ [stream library](https://github.com/vgteam/stream) for more
-        details.
-        
-        ---
-        **NOTE**
-        
-        **@vg users:** The new version of stream library, now as a part of
-        [libvgio](https://github.com/vgteam/libvgio), writes a header at the start of
-        the stream depending on the output format. For example, headers like `b'GAM'`
-        or `b'VG'` can be found before the actual protobuf messages in GAM and VG files
-        repectively. In this case, you should provide the expected value using `header`
-        keyword argument; e.g.
-        `stream.parse('file.gam', vg_pb2.Alignment, header=b'GAM')`
-        for GAM files (since version v1.6.2).
-        
-        ---
-        
-        ## Encoding
-        The encoding is simple. Messages are written in groups of different sizes. Each
-        group starts with its size; i.e. the number of messages in that group. Then, the
-        size of each message is followed by the encoded message itself. Quoted from
-        [Google Protobuf Developer Guide](https://developers.google.com/protocol-buffers/docs/techniques#streaming):
-        
-        > The Protocol Buffer wire format is not self-delimiting, so protocol buffer
-        > parsers cannot determine where a message ends on their own. The easiest way to
-        > solve this problem is to write the size of each message before you write the
-        > message itself. When you read the messages back in, you read the size, then
-        > read the bytes into a separate buffer, then parse from that buffer.
-        
-        By default, the stream is considered compressed by GZip. However, uncompressed
-        stream processing is possible by passing `gzip=False` to any API calls.
-        
-        ## Installation
-        You can install pyStream using `pip`:
-        
-            pip install pystream-protobuf
-        
-        ## Usage
-        See [Wiki](https://github.com/cartoonist/pystream-protobuf/wiki) for usage documentation.
-        
-        ## Development
-        In case, you work with the source code and need to build the package:
-        
-            python setup.py build
-        
-        The proto files in the test module required to be compiled before running test
-        cases. To do so, it is required to have Google protobuf compiler (>=3.0.2)
-        installed. After installing protobuf compiler, run:
-        
-            make init
-        
-        to compile proto files required for test module and then:
-        
-            make test
-        
-        to run tests.
-        
 Keywords: stream protocol buffer protobuf
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
+
+[![Build Status](https://img.shields.io/travis/cartoonist/pystream-protobuf.svg?style=flat-square)](https://travis-ci.org/cartoonist/pystream-protobuf)
+[![PyPI Release](https://img.shields.io/pypi/v/pystream-protobuf.svg?style=flat-square)](https://pypi.python.org/pypi/pystream-protobuf)
+[![PyPI Status](https://img.shields.io/pypi/status/pystream-protobuf.svg?style=flat-square)](https://pypi.python.org/pypi/pystream-protobuf)
+[![Python](https://img.shields.io/pypi/pyversions/pystream-protobuf.svg?style=flat-square)](https://www.python.org/download/releases/3.0/)
+[![License](https://img.shields.io/pypi/l/pystream-protobuf.svg?style=flat-square)](https://github.com/cartoonist/pystream-protobuf/blob/master/LICENSE)
+
+# pyStream
+Python implementation of [stream library](https://github.com/vgteam/stream).
+
+## Introduction
+This library enables _stream processing_ of protobuf messages (or any serializable
+objects since v1.6.3); i.e. multiple protobuf messages can be written/read into/from a
+single stream or file.
+
+It was originally developed to parse/write [vg](https://github.com/vgteam/vg)
+file formats (`.vg`, `.gam`, etc). However, it can be used for any arbitrary
+protocol buffer messages.
+
+Refer to the C++ [stream library](https://github.com/vgteam/stream) for more
+details.
+
+---
+
+**NOTE**
+
+**@vg users:** The new version of stream library, now as a part of
+[libvgio](https://github.com/vgteam/libvgio), writes a header tag at the start of
+the stream depending on the output format. For example, headers like `b'GAM'`
+or `b'VG'` can be found before the actual protobuf messages in GAM and VG files
+repectively. In this case, you should provide the expected value using `header`
+keyword argument; e.g.
+`stream.parse('file.gam', vg_pb2.Alignment, header=b'GAM', persistent_header=True)`
+for GAM files (since version v1.6.2).
+
+---
+
+## Encoding
+The encoding is simple. Messages are written in groups of different sizes. Each
+group starts with its size; i.e. the number of messages in that group. Then, the
+size of each message is followed by the encoded message itself. Quoted from
+[Google Protobuf Developer Guide](https://developers.google.com/protocol-buffers/docs/techniques#streaming):
+
+> The Protocol Buffer wire format is not self-delimiting, so protocol buffer
+> parsers cannot determine where a message ends on their own. The easiest way to
+> solve this problem is to write the size of each message before you write the
+> message itself. When you read the messages back in, you read the size, then
+> read the bytes into a separate buffer, then parse from that buffer.
+
+By default, the stream is considered compressed by GZip. However, uncompressed
+stream processing is possible by passing `gzip=False` to any API calls.
+
+## Installation
+You can install pyStream using `pip`:
+
+    pip install pystream-protobuf
+
+## Usage
+See [Wiki](https://github.com/cartoonist/pystream-protobuf/wiki) for usage documentation.
+
+## Development
+In case, you work with the source code and need to build the package:
+
+    python setup.py build
+
+The proto files in the test module required to be compiled before running test
+cases. To do so, it is required to have Google protobuf compiler (>=3.0.2)
+installed. After installing protobuf compiler, run:
+
+    make init
+
+to compile proto files required for test module and then:
+
+    make test
+
+to run tests.
```

### Comparing `pystream-protobuf-1.6.3/setup.py` & `pystream-protobuf-1.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `pystream-protobuf-1.6.3/stream/release.py` & `pystream-protobuf-1.6.4/stream/release.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 __title__ = 'stream'
 __description__ = 'Python implementation of stream library'
 __author__ = 'Ali Ghaffaari'
 __email__ = 'ali.ghaffaari@mpi-inf.mpg.de'
 __license__ = 'MIT'
 
 # Release
-__version__ = '1.6.3'
+__version__ = '1.6.4'
 __status__ = DS_STABLE
 
 # PyPI-related information
 __keywords__ = 'stream protocol buffer protobuf'
 __classifiers__ = [
     # Development status
     DS_STRING[__status__],
```

### Comparing `pystream-protobuf-1.6.3/stream/stream.py` & `pystream-protobuf-1.6.4/stream/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,28 +132,31 @@
                 in one group upon `flush` or `close` events.
             group_delimiter (boolean): indicate the end of a message group if
                 True by yielding a delimiter after reading each group.
             delimiter_cls (class): delimiter class.
             gzip (bool): Whether or not to use gzip compression on the given
                 file. (default is True)
             header (bytes): the header which is expected to read or write.
+            persistent_header (bool): whether headers occur before any data
+                blob. (default is False)
             serialize (function): serialising an input object to byte string.
                 If `None`, input objects are assumed to be protobuf messages.
         """
         self._myfd = None
         if fileobj is None:
             if kwargs.get('gzip', True):
                 self._fd = gzip.open(filename, mode)
             else:
                 import builtins
                 self._fd = builtins.open(filename, mode)
             self._myfd = self._fd
         else:
             self._fd = fileobj
         self._header = kwargs.pop('header', b'')
+        self._pers_header = kwargs.pop('persistent_header', False)
         if not mode.startswith('r'):
             self._buffer_size = kwargs.pop('buffer_size', 0)
             self._serialize = kwargs.pop('serialize', self.serialize_to_string)
             self._write_buff = []
         else:
             self._group_delim = kwargs.pop('group_delimiter', False)
             self._delimiter = kwargs.pop('delimiter_cls', None)
@@ -265,27 +268,29 @@
     def __next__(self):
         """Get the next protobuf object data in a sync stream and check the
         header.
         """
         val = self._next()
         if self._header:
             if val == self._header:
-                self._header = b''
+                if not self._pers_header:
+                    self._header = b''
                 return self._next()
             raise RuntimeError("mismatch header (fetched {v})".format(v=val))
         return val
 
     async def __anext__(self):
         """Get the next protobuf object data in an async stream and check the
         header.
         """
         val = await self._anext()
         if self._header:
             if val == self._header:
-                self._header = b''
+                if not self._pers_header:
+                    self._header = b''
                 return await self._anext()
             raise RuntimeError("mismatch header (fetched {v})".format(v=val))
         return val
 
     def delimiter_class(self):
         """Return group delimiter class."""
         return type(None) if self._delimiter is None else self._delimiter
@@ -345,15 +350,16 @@
             self.flush()
 
     def _write_header(self):
         """Write the header into the stream."""
         assert self._header
         encodeVarint(self._fd.write, len(self._header), True)
         self._fd.write(self._header)
-        self._header = b''
+        if not self._pers_header:
+            self._header = b''
 
     def flush(self):
         """Write down buffer to the file."""
         if not self.is_output():
             return
 
         count = len(self._write_buff) + int(bool(self._header))
```

### Comparing `pystream-protobuf-1.6.3/stream/varint.py` & `pystream-protobuf-1.6.4/stream/varint.py`

 * *Files identical despite different names*

