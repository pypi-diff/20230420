# Comparing `tmp/market-data-transcoder-1.0.1.tar.gz` & `tmp/market-data-transcoder-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "market-data-transcoder-1.0.1.tar", last modified: Fri Mar 10 15:57:27 2023, max compression
+gzip compressed data, was "market-data-transcoder-1.0.2.tar", last modified: Thu Apr 20 20:42:58 2023, max compression
```

## Comparing `market-data-transcoder-1.0.1.tar` & `market-data-transcoder-1.0.2.tar`

### file list

```diff
@@ -1,116 +1,123 @@
-drwxr-xr-x   0 mservidio   (502) staff       (20)        0 2023-03-10 15:57:27.849214 market-data-transcoder-1.0.1/
--rw-r--r--   0 mservidio   (502) staff       (20)    11357 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/LICENSE
--rw-r--r--   0 mservidio   (502) staff       (20)    13254 2023-03-10 15:57:27.849598 market-data-transcoder-1.0.1/PKG-INFO
--rw-r--r--   0 mservidio   (502) staff       (20)    12376 2023-03-07 19:34:39.000000 market-data-transcoder-1.0.1/README.md
-drwxr-xr-x   0 mservidio   (502) staff       (20)        0 2023-03-10 15:57:26.493615 market-data-transcoder-1.0.1/market_data_transcoder.egg-info/
--rw-r--r--   0 mservidio   (502) staff       (20)    13254 2023-03-10 15:57:25.000000 market-data-transcoder-1.0.1/market_data_transcoder.egg-info/PKG-INFO
--rw-r--r--   0 mservidio   (502) staff       (20)     3967 2023-03-10 15:57:26.000000 market-data-transcoder-1.0.1/market_data_transcoder.egg-info/SOURCES.txt
--rw-r--r--   0 mservidio   (502) staff       (20)        1 2023-03-10 15:57:25.000000 market-data-transcoder-1.0.1/market_data_transcoder.egg-info/dependency_links.txt
--rw-r--r--   0 mservidio   (502) staff       (20)       48 2023-03-10 15:57:25.000000 market-data-transcoder-1.0.1/market_data_transcoder.egg-info/entry_points.txt
--rw-r--r--   0 mservidio   (502) staff       (20)        1 2023-03-10 15:57:24.000000 market-data-transcoder-1.0.1/market_data_transcoder.egg-info/not-zip-safe
--rw-r--r--   0 mservidio   (502) staff       (20)      149 2023-03-10 15:57:25.000000 market-data-transcoder-1.0.1/market_data_transcoder.egg-info/requires.txt
--rw-r--r--   0 mservidio   (502) staff       (20)       23 2023-03-10 15:57:25.000000 market-data-transcoder-1.0.1/market_data_transcoder.egg-info/top_level.txt
--rw-r--r--   0 mservidio   (502) staff       (20)      101 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/pyproject.toml
--rw-r--r--   0 mservidio   (502) staff       (20)     1263 2023-03-10 15:57:27.859830 market-data-transcoder-1.0.1/setup.cfg
-drwxr-xr-x   0 mservidio   (502) staff       (20)        0 2023-03-10 15:57:26.494789 market-data-transcoder-1.0.1/third_party/
--rw-r--r--   0 mservidio   (502) staff       (20)      846 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/third_party/__init__.py
-drwxr-xr-x   0 mservidio   (502) staff       (20)        0 2023-03-10 15:57:26.506154 market-data-transcoder-1.0.1/third_party/pyfixmsg/
--rw-r--r--   0 mservidio   (502) staff       (20)     6276 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/third_party/pyfixmsg/__init__.py
-drwxr-xr-x   0 mservidio   (502) staff       (20)        0 2023-03-10 15:57:26.509542 market-data-transcoder-1.0.1/third_party/pyfixmsg/codecs/
--rw-r--r--   0 mservidio   (502) staff       (20)      846 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/third_party/pyfixmsg/codecs/__init__.py
--rw-r--r--   0 mservidio   (502) staff       (20)    13965 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/third_party/pyfixmsg/codecs/stringfix.py
-drwxr-xr-x   0 mservidio   (502) staff       (20)        0 2023-03-10 15:57:26.512433 market-data-transcoder-1.0.1/third_party/pyfixmsg/exception/
--rw-r--r--   0 mservidio   (502) staff       (20)      945 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/third_party/pyfixmsg/exception/FixSchemaNotDefinedError.py
--rw-r--r--   0 mservidio   (502) staff       (20)      846 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/third_party/pyfixmsg/exception/__init__.py
--rw-r--r--   0 mservidio   (502) staff       (20)    18449 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/third_party/pyfixmsg/fixmessage.py
--rw-r--r--   0 mservidio   (502) staff       (20)     6964 2023-03-07 02:39:47.000000 market-data-transcoder-1.0.1/third_party/pyfixmsg/parser.py
--rw-r--r--   0 mservidio   (502) staff       (20)    18582 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/third_party/pyfixmsg/reference.py
--rw-r--r--   0 mservidio   (502) staff       (20)     1079 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/third_party/pyfixmsg/util.py
-drwxr-xr-x   0 mservidio   (502) staff       (20)        0 2023-03-10 15:57:26.523472 market-data-transcoder-1.0.1/third_party/sbedecoder/
--rw-r--r--   0 mservidio   (502) staff       (20)      154 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/third_party/sbedecoder/__init__.py
--rw-r--r--   0 mservidio   (502) staff       (20)    22959 2023-03-06 02:42:26.000000 market-data-transcoder-1.0.1/third_party/sbedecoder/message.py
--rw-r--r--   0 mservidio   (502) staff       (20)     5376 2023-03-07 19:34:39.000000 market-data-transcoder-1.0.1/third_party/sbedecoder/parser.py
--rw-r--r--   0 mservidio   (502) staff       (20)    27955 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/third_party/sbedecoder/schema.py
--rw-r--r--   0 mservidio   (502) staff       (20)     1326 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/third_party/sbedecoder/typemap.py
-drwxr-xr-x   0 mservidio   (502) staff       (20)        0 2023-03-10 15:57:26.846479 market-data-transcoder-1.0.1/transcoder/
--rw-r--r--   0 mservidio   (502) staff       (20)     1257 2023-03-10 15:56:07.000000 market-data-transcoder-1.0.1/transcoder/__init__.py
--rwxr-xr-x   0 mservidio   (502) staff       (20)    12590 2023-03-10 15:56:07.000000 market-data-transcoder-1.0.1/transcoder/main.py
-drwxr-xr-x   0 mservidio   (502) staff       (20)        0 2023-03-10 15:57:26.930898 market-data-transcoder-1.0.1/transcoder/message/
--rw-r--r--   0 mservidio   (502) staff       (20)     1709 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/message/DatacastField.py
--rw-r--r--   0 mservidio   (502) staff       (20)     2756 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/message/DatacastGroup.py
--rw-r--r--   0 mservidio   (502) staff       (20)     5360 2023-03-03 17:55:30.000000 market-data-transcoder-1.0.1/transcoder/message/DatacastParser.py
--rw-r--r--   0 mservidio   (502) staff       (20)     1163 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/message/DatacastSchema.py
--rw-r--r--   0 mservidio   (502) staff       (20)     3813 2023-03-07 02:11:02.000000 market-data-transcoder-1.0.1/transcoder/message/ErrorWriter.py
--rw-r--r--   0 mservidio   (502) staff       (20)    12954 2023-03-10 15:56:07.000000 market-data-transcoder-1.0.1/transcoder/message/MessageParser.py
--rw-r--r--   0 mservidio   (502) staff       (20)     2550 2023-03-03 17:55:30.000000 market-data-transcoder-1.0.1/transcoder/message/MessageUtil.py
--rw-r--r--   0 mservidio   (502) staff       (20)     1452 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/message/ParsedMessage.py
--rw-r--r--   0 mservidio   (502) staff       (20)      846 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/message/__init__.py
-drwxr-xr-x   0 mservidio   (502) staff       (20)        0 2023-03-10 15:57:27.165709 market-data-transcoder-1.0.1/transcoder/message/exception/
--rw-r--r--   0 mservidio   (502) staff       (20)      974 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/message/exception/MessageParserNotDefinedError.py
--rw-r--r--   0 mservidio   (502) staff       (20)      927 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/message/exception/ParserFunctionNotDefinedError.py
--rw-r--r--   0 mservidio   (502) staff       (20)      959 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/message/exception/__init__.py
-drwxr-xr-x   0 mservidio   (502) staff       (20)        0 2023-03-10 15:57:27.273685 market-data-transcoder-1.0.1/transcoder/message/factory/
--rw-r--r--   0 mservidio   (502) staff       (20)     1595 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/message/factory/CmeMessageFactory.py
--rw-r--r--   0 mservidio   (502) staff       (20)     1762 2023-03-10 15:56:07.000000 market-data-transcoder-1.0.1/transcoder/message/factory/ITCHMessageFactory.py
--rw-r--r--   0 mservidio   (502) staff       (20)     2001 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/message/factory/MDPMessageFactory.py
--rw-r--r--   0 mservidio   (502) staff       (20)     1576 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/message/factory/MemxMessageFactory.py
--rw-r--r--   0 mservidio   (502) staff       (20)     1687 2023-03-07 19:34:39.000000 market-data-transcoder-1.0.1/transcoder/message/factory/MessageFactory.py
--rw-r--r--   0 mservidio   (502) staff       (20)     1319 2023-03-07 19:34:39.000000 market-data-transcoder-1.0.1/transcoder/message/factory/__init__.py
-drwxr-xr-x   0 mservidio   (502) staff       (20)        0 2023-03-10 15:57:27.429472 market-data-transcoder-1.0.1/transcoder/message/factory/exception/
--rw-r--r--   0 mservidio   (502) staff       (20)      915 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/message/factory/exception/FactoryNotFoundError.py
--rw-r--r--   0 mservidio   (502) staff       (20)      946 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/message/factory/exception/TemplateSchemaNotDefinedError.py
--rw-r--r--   0 mservidio   (502) staff       (20)      920 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/message/factory/exception/__init__.py
-drwxr-xr-x   0 mservidio   (502) staff       (20)        0 2023-03-10 15:57:27.494350 market-data-transcoder-1.0.1/transcoder/message/handler/
--rw-r--r--   0 mservidio   (502) staff       (20)     2320 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/message/handler/CmeBinaryPacketHandler.py
--rw-r--r--   0 mservidio   (502) staff       (20)     1756 2023-03-07 02:39:47.000000 market-data-transcoder-1.0.1/transcoder/message/handler/MessageHandler.py
--rw-r--r--   0 mservidio   (502) staff       (20)     1423 2023-03-07 02:39:47.000000 market-data-transcoder-1.0.1/transcoder/message/handler/MessageHandlerFloatField.py
--rw-r--r--   0 mservidio   (502) staff       (20)     1417 2023-03-07 02:39:47.000000 market-data-transcoder-1.0.1/transcoder/message/handler/MessageHandlerIntField.py
--rw-r--r--   0 mservidio   (502) staff       (20)     1424 2023-03-07 02:39:47.000000 market-data-transcoder-1.0.1/transcoder/message/handler/MessageHandlerStringField.py
--rw-r--r--   0 mservidio   (502) staff       (20)     1876 2023-03-09 16:22:51.000000 market-data-transcoder-1.0.1/transcoder/message/handler/SequencerHandler.py
--rw-r--r--   0 mservidio   (502) staff       (20)     2182 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/message/handler/TimestampPullForwardHandler.py
--rw-r--r--   0 mservidio   (502) staff       (20)     1022 2023-03-09 02:24:09.000000 market-data-transcoder-1.0.1/transcoder/message/handler/__init__.py
-drwxr-xr-x   0 mservidio   (502) staff       (20)        0 2023-03-10 15:57:27.521357 market-data-transcoder-1.0.1/transcoder/output/
--rw-r--r--   0 mservidio   (502) staff       (20)     4536 2023-03-07 19:39:18.000000 market-data-transcoder-1.0.1/transcoder/output/OutputManager.py
--rw-r--r--   0 mservidio   (502) staff       (20)     4481 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/output/OutputUtil.py
--rw-r--r--   0 mservidio   (502) staff       (20)      935 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/output/__init__.py
-drwxr-xr-x   0 mservidio   (502) staff       (20)        0 2023-03-10 15:57:27.581621 market-data-transcoder-1.0.1/transcoder/output/avro/
--rw-r--r--   0 mservidio   (502) staff       (20)     1843 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/output/avro/AvroOutputManager.py
--rw-r--r--   0 mservidio   (502) staff       (20)     2736 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/output/avro/BaseAvroOutputManager.py
--rw-r--r--   0 mservidio   (502) staff       (20)     1756 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/output/avro/FastAvroOutputManager.py
--rw-r--r--   0 mservidio   (502) staff       (20)      953 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/output/avro/__init__.py
-drwxr-xr-x   0 mservidio   (502) staff       (20)        0 2023-03-10 15:57:27.608593 market-data-transcoder-1.0.1/transcoder/output/diag/
--rw-r--r--   0 mservidio   (502) staff       (20)     1158 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/output/diag/DiagnosticOutputManager.py
--rw-r--r--   0 mservidio   (502) staff       (20)      908 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/output/diag/__init__.py
-drwxr-xr-x   0 mservidio   (502) staff       (20)        0 2023-03-10 15:57:27.627307 market-data-transcoder-1.0.1/transcoder/output/exception/
--rw-r--r--   0 mservidio   (502) staff       (20)      983 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/output/exception/BigQueryTableSchemaOutOfSyncError.py
--rw-r--r--   0 mservidio   (502) staff       (20)      943 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/output/exception/OutputFunctionNotDefinedError.py
--rw-r--r--   0 mservidio   (502) staff       (20)      909 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/output/exception/OutputManagerSchemaError.py
--rw-r--r--   0 mservidio   (502) staff       (20)      953 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/output/exception/OutputNotAvailableError.py
--rw-r--r--   0 mservidio   (502) staff       (20)      979 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/output/exception/PubSubTopicSchemaOutOfSyncError.py
--rw-r--r--   0 mservidio   (502) staff       (20)     1202 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/output/exception/__init__.py
-drwxr-xr-x   0 mservidio   (502) staff       (20)        0 2023-03-10 15:57:27.634045 market-data-transcoder-1.0.1/transcoder/output/google_cloud/
--rw-r--r--   0 mservidio   (502) staff       (20)     6504 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/output/google_cloud/BigQueryOutputManager.py
--rw-r--r--   0 mservidio   (502) staff       (20)     1016 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/output/google_cloud/Constants.py
--rw-r--r--   0 mservidio   (502) staff       (20)    12040 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/output/google_cloud/PubSubOutputManager.py
--rw-r--r--   0 mservidio   (502) staff       (20)      957 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/output/google_cloud/__init__.py
-drwxr-xr-x   0 mservidio   (502) staff       (20)        0 2023-03-10 15:57:27.641864 market-data-transcoder-1.0.1/transcoder/output/google_cloud/terraform/
--rw-r--r--   0 mservidio   (502) staff       (20)     2792 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/output/google_cloud/terraform/BigQueryTerraformOutputManager.py
--rw-r--r--   0 mservidio   (502) staff       (20)     2118 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/output/google_cloud/terraform/GcpTerraformOutputManager.py
--rw-r--r--   0 mservidio   (502) staff       (20)     2892 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/output/google_cloud/terraform/PubSubTerraformOutputManager.py
--rw-r--r--   0 mservidio   (502) staff       (20)      993 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/output/google_cloud/terraform/__init__.py
-drwxr-xr-x   0 mservidio   (502) staff       (20)        0 2023-03-10 15:57:27.646003 market-data-transcoder-1.0.1/transcoder/output/json/
--rw-r--r--   0 mservidio   (502) staff       (20)     3559 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/output/json/JsonOutputManager.py
--rw-r--r--   0 mservidio   (502) staff       (20)      896 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/output/json/__init__.py
-drwxr-xr-x   0 mservidio   (502) staff       (20)        0 2023-03-10 15:57:27.652132 market-data-transcoder-1.0.1/transcoder/source/
--rw-r--r--   0 mservidio   (502) staff       (20)     1826 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/source/Source.py
--rw-r--r--   0 mservidio   (502) staff       (20)     3476 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/source/SourceUtil.py
--rw-r--r--   0 mservidio   (502) staff       (20)      894 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/source/__init__.py
-drwxr-xr-x   0 mservidio   (502) staff       (20)        0 2023-03-10 15:57:27.845228 market-data-transcoder-1.0.1/transcoder/source/file/
--rw-r--r--   0 mservidio   (502) staff       (20)     3971 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/source/file/CmeBinaryPacketFileMessageSource.py
--rw-r--r--   0 mservidio   (502) staff       (20)     3504 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/source/file/FileMessageSource.py
--rw-r--r--   0 mservidio   (502) staff       (20)     2496 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/source/file/LengthDelimitedFileMessageSource.py
--rw-r--r--   0 mservidio   (502) staff       (20)     2016 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/source/file/LineDelimitedFileMessageSource.py
--rw-r--r--   0 mservidio   (502) staff       (20)     2296 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/source/file/PcapFileMessageSource.py
--rw-r--r--   0 mservidio   (502) staff       (20)     1186 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/source/file/__init__.py
--rw-r--r--   0 mservidio   (502) staff       (20)     1624 2023-03-02 21:47:49.000000 market-data-transcoder-1.0.1/transcoder/test.py
--rw-r--r--   0 mservidio   (502) staff       (20)      837 2023-03-10 15:55:53.000000 market-data-transcoder-1.0.1/transcoder/version.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.637516 market-data-transcoder-1.0.2/
+-rw-r--r--   0 mservidio   (501) staff       (20)    11357 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/LICENSE
+-rw-r--r--   0 mservidio   (501) staff       (20)    13254 2023-04-20 20:42:58.637649 market-data-transcoder-1.0.2/PKG-INFO
+-rw-r--r--   0 mservidio   (501) staff       (20)    12376 2023-03-18 02:08:30.000000 market-data-transcoder-1.0.2/README.md
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.623352 market-data-transcoder-1.0.2/market_data_transcoder.egg-info/
+-rw-r--r--   0 mservidio   (501) staff       (20)    13254 2023-04-20 20:42:58.000000 market-data-transcoder-1.0.2/market_data_transcoder.egg-info/PKG-INFO
+-rw-r--r--   0 mservidio   (501) staff       (20)     4188 2023-04-20 20:42:58.000000 market-data-transcoder-1.0.2/market_data_transcoder.egg-info/SOURCES.txt
+-rw-r--r--   0 mservidio   (501) staff       (20)        1 2023-04-20 20:42:58.000000 market-data-transcoder-1.0.2/market_data_transcoder.egg-info/dependency_links.txt
+-rw-r--r--   0 mservidio   (501) staff       (20)       48 2023-04-20 20:42:58.000000 market-data-transcoder-1.0.2/market_data_transcoder.egg-info/entry_points.txt
+-rw-r--r--   0 mservidio   (501) staff       (20)        1 2023-04-20 20:22:51.000000 market-data-transcoder-1.0.2/market_data_transcoder.egg-info/not-zip-safe
+-rw-r--r--   0 mservidio   (501) staff       (20)      149 2023-04-20 20:42:58.000000 market-data-transcoder-1.0.2/market_data_transcoder.egg-info/requires.txt
+-rw-r--r--   0 mservidio   (501) staff       (20)       23 2023-04-20 20:42:58.000000 market-data-transcoder-1.0.2/market_data_transcoder.egg-info/top_level.txt
+-rw-r--r--   0 mservidio   (501) staff       (20)      101 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/pyproject.toml
+-rw-r--r--   0 mservidio   (501) staff       (20)     1263 2023-04-20 20:42:58.638472 market-data-transcoder-1.0.2/setup.cfg
+-rw-r--r--   0 mservidio   (501) staff       (20)     1075 2023-04-20 20:41:12.000000 market-data-transcoder-1.0.2/setup.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.623486 market-data-transcoder-1.0.2/third_party/
+-rw-r--r--   0 mservidio   (501) staff       (20)      846 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/third_party/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.624209 market-data-transcoder-1.0.2/third_party/pyfixmsg/
+-rw-r--r--   0 mservidio   (501) staff       (20)     6276 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/third_party/pyfixmsg/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.624449 market-data-transcoder-1.0.2/third_party/pyfixmsg/codecs/
+-rw-r--r--   0 mservidio   (501) staff       (20)      846 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/third_party/pyfixmsg/codecs/__init__.py
+-rw-r--r--   0 mservidio   (501) staff       (20)    13965 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/third_party/pyfixmsg/codecs/stringfix.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.624718 market-data-transcoder-1.0.2/third_party/pyfixmsg/exception/
+-rw-r--r--   0 mservidio   (501) staff       (20)      945 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/third_party/pyfixmsg/exception/FixSchemaNotDefinedError.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      846 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/third_party/pyfixmsg/exception/__init__.py
+-rw-r--r--   0 mservidio   (501) staff       (20)    18449 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/third_party/pyfixmsg/fixmessage.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     6960 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/third_party/pyfixmsg/parser.py
+-rw-r--r--   0 mservidio   (501) staff       (20)    18582 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/third_party/pyfixmsg/reference.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1079 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/third_party/pyfixmsg/util.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.625469 market-data-transcoder-1.0.2/third_party/sbedecoder/
+-rw-r--r--   0 mservidio   (501) staff       (20)      154 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/third_party/sbedecoder/__init__.py
+-rw-r--r--   0 mservidio   (501) staff       (20)    22959 2023-03-18 02:08:30.000000 market-data-transcoder-1.0.2/third_party/sbedecoder/message.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     5317 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/third_party/sbedecoder/parser.py
+-rw-r--r--   0 mservidio   (501) staff       (20)    27955 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/third_party/sbedecoder/schema.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1326 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/third_party/sbedecoder/typemap.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.626116 market-data-transcoder-1.0.2/transcoder/
+-rw-r--r--   0 mservidio   (501) staff       (20)    11989 2023-04-20 19:43:43.000000 market-data-transcoder-1.0.2/transcoder/Transcoder.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      915 2023-04-20 20:38:35.000000 market-data-transcoder-1.0.2/transcoder/__init__.py
+-rwxr-xr-x   0 mservidio   (501) staff       (20)    12218 2023-04-20 19:42:58.000000 market-data-transcoder-1.0.2/transcoder/main.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.627446 market-data-transcoder-1.0.2/transcoder/message/
+-rw-r--r--   0 mservidio   (501) staff       (20)     1709 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/DatacastField.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     2756 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/DatacastGroup.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     5117 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/message/DatacastParser.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1163 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/DatacastSchema.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     3775 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/message/ErrorWriter.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     3280 2023-04-20 19:45:10.000000 market-data-transcoder-1.0.2/transcoder/message/MessageUtil.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1335 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/message/NoParser.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1452 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/ParsedMessage.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      921 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/message/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.627881 market-data-transcoder-1.0.2/transcoder/message/exception/
+-rw-r--r--   0 mservidio   (501) staff       (20)      974 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/exception/MessageParserNotDefinedError.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      927 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/exception/ParserFunctionNotDefinedError.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      959 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/exception/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.628731 market-data-transcoder-1.0.2/transcoder/message/factory/
+-rw-r--r--   0 mservidio   (501) staff       (20)     1595 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/factory/CmeMessageFactory.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1762 2023-03-18 02:08:30.000000 market-data-transcoder-1.0.2/transcoder/message/factory/ITCHMessageFactory.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     2001 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/factory/MDPMessageFactory.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1576 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/factory/MemxMessageFactory.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1687 2023-03-18 02:08:30.000000 market-data-transcoder-1.0.2/transcoder/message/factory/MessageFactory.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1319 2023-03-18 02:08:30.000000 market-data-transcoder-1.0.2/transcoder/message/factory/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.629179 market-data-transcoder-1.0.2/transcoder/message/factory/exception/
+-rw-r--r--   0 mservidio   (501) staff       (20)      915 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/factory/exception/FactoryNotFoundError.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      946 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/factory/exception/TemplateSchemaNotDefinedError.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      920 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/message/factory/exception/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.630551 market-data-transcoder-1.0.2/transcoder/message/handler/
+-rw-r--r--   0 mservidio   (501) staff       (20)     2269 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/message/handler/CmeBinaryPacketHandler.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     2287 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/message/handler/FilterHandler.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1731 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/message/handler/MessageHandler.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1423 2023-03-18 02:08:30.000000 market-data-transcoder-1.0.2/transcoder/message/handler/MessageHandlerFloatField.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1417 2023-03-18 02:08:30.000000 market-data-transcoder-1.0.2/transcoder/message/handler/MessageHandlerIntField.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1424 2023-03-18 02:08:30.000000 market-data-transcoder-1.0.2/transcoder/message/handler/MessageHandlerStringField.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     2137 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/message/handler/SequencerHandler.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     2151 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/message/handler/TimestampPullForwardHandler.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1063 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/message/handler/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.630995 market-data-transcoder-1.0.2/transcoder/output/
+-rw-r--r--   0 mservidio   (501) staff       (20)     4536 2023-03-18 02:08:30.000000 market-data-transcoder-1.0.2/transcoder/output/OutputManager.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     4975 2023-04-20 20:10:00.000000 market-data-transcoder-1.0.2/transcoder/output/OutputUtil.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      955 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/output/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.631615 market-data-transcoder-1.0.2/transcoder/output/avro/
+-rw-r--r--   0 mservidio   (501) staff       (20)     1843 2023-04-20 20:30:03.000000 market-data-transcoder-1.0.2/transcoder/output/avro/AvroOutputManager.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     2736 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/avro/BaseAvroOutputManager.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1756 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/avro/FastAvroOutputManager.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      953 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/avro/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.631933 market-data-transcoder-1.0.2/transcoder/output/diag/
+-rw-r--r--   0 mservidio   (501) staff       (20)     1158 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/diag/DiagnosticOutputManager.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      908 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/diag/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.633464 market-data-transcoder-1.0.2/transcoder/output/exception/
+-rw-r--r--   0 mservidio   (501) staff       (20)      983 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/exception/BigQueryTableSchemaOutOfSyncError.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      943 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/exception/OutputFunctionNotDefinedError.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      909 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/exception/OutputManagerSchemaError.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      953 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/exception/OutputNotAvailableError.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      979 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/exception/PubSubTopicSchemaOutOfSyncError.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1202 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/exception/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.634238 market-data-transcoder-1.0.2/transcoder/output/google_cloud/
+-rw-r--r--   0 mservidio   (501) staff       (20)     6504 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/google_cloud/BigQueryOutputManager.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1016 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/google_cloud/Constants.py
+-rw-r--r--   0 mservidio   (501) staff       (20)    12040 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/google_cloud/PubSubOutputManager.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      957 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/google_cloud/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.634859 market-data-transcoder-1.0.2/transcoder/output/google_cloud/terraform/
+-rw-r--r--   0 mservidio   (501) staff       (20)     2792 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/google_cloud/terraform/BigQueryTerraformOutputManager.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     2118 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/google_cloud/terraform/GcpTerraformOutputManager.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     2892 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/google_cloud/terraform/PubSubTerraformOutputManager.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      993 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/google_cloud/terraform/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.635140 market-data-transcoder-1.0.2/transcoder/output/json/
+-rw-r--r--   0 mservidio   (501) staff       (20)     3559 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/json/JsonOutputManager.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      896 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/output/json/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.635435 market-data-transcoder-1.0.2/transcoder/output/length_delimited/
+-rw-r--r--   0 mservidio   (501) staff       (20)     1909 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/output/length_delimited/LengthDelimitedOutputManager.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      918 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/output/length_delimited/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.636011 market-data-transcoder-1.0.2/transcoder/source/
+-rw-r--r--   0 mservidio   (501) staff       (20)     1189 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/source/LineEncoding.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1826 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/source/Source.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     3776 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/source/SourceUtil.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      914 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/source/__init__.py
+drwxr-xr-x   0 mservidio   (501) staff       (20)        0 2023-04-20 20:42:58.637389 market-data-transcoder-1.0.2/transcoder/source/file/
+-rw-r--r--   0 mservidio   (501) staff       (20)     3867 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/source/file/CmeBinaryPacketFileMessageSource.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     2623 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/source/file/FileMessageSource.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     2630 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/source/file/LengthDelimitedFileMessageSource.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     2719 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/source/file/LineDelimitedFileMessageSource.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     2295 2023-04-20 19:33:29.000000 market-data-transcoder-1.0.2/transcoder/source/file/PcapFileMessageSource.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1186 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/source/file/__init__.py
+-rw-r--r--   0 mservidio   (501) staff       (20)     1624 2023-03-17 18:45:04.000000 market-data-transcoder-1.0.2/transcoder/test.py
+-rw-r--r--   0 mservidio   (501) staff       (20)      837 2023-04-20 19:51:40.000000 market-data-transcoder-1.0.2/transcoder/version.py
```

### Comparing `market-data-transcoder-1.0.1/LICENSE` & `market-data-transcoder-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/PKG-INFO` & `market-data-transcoder-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: market-data-transcoder
-Version: 1.0.1
+Version: 1.0.2
 Summary: Market Data Transcoder
 Home-page: https://github.com/GoogleCloudPlatform/market-data-transcoder
 Author: Google Cloud FSI Solutions
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/GoogleCloudPlatform/market-data-transcoder/issues
 Keywords: bigquery,devops,json,automation,schema,trading,avro,binary,transcoding,pubsub,fix,fixprotocol,google-cloud-platform,itch,sbe,simple-binary-encoding,exchanges,marketdata,binaryencoding
 Classifier: Programming Language :: Python :: 3
```

### Comparing `market-data-transcoder-1.0.1/README.md` & `market-data-transcoder-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/market_data_transcoder.egg-info/PKG-INFO` & `market-data-transcoder-1.0.2/market_data_transcoder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: market-data-transcoder
-Version: 1.0.1
+Version: 1.0.2
 Summary: Market Data Transcoder
 Home-page: https://github.com/GoogleCloudPlatform/market-data-transcoder
 Author: Google Cloud FSI Solutions
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/GoogleCloudPlatform/market-data-transcoder/issues
 Keywords: bigquery,devops,json,automation,schema,trading,avro,binary,transcoding,pubsub,fix,fixprotocol,google-cloud-platform,itch,sbe,simple-binary-encoding,exchanges,marketdata,binaryencoding
 Classifier: Programming Language :: Python :: 3
```

### Comparing `market-data-transcoder-1.0.1/market_data_transcoder.egg-info/SOURCES.txt` & `market-data-transcoder-1.0.2/market_data_transcoder.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
+setup.py
 market_data_transcoder.egg-info/PKG-INFO
 market_data_transcoder.egg-info/SOURCES.txt
 market_data_transcoder.egg-info/dependency_links.txt
 market_data_transcoder.egg-info/entry_points.txt
 market_data_transcoder.egg-info/not-zip-safe
 market_data_transcoder.egg-info/requires.txt
 market_data_transcoder.egg-info/top_level.txt
@@ -20,25 +21,26 @@
 third_party/pyfixmsg/exception/FixSchemaNotDefinedError.py
 third_party/pyfixmsg/exception/__init__.py
 third_party/sbedecoder/__init__.py
 third_party/sbedecoder/message.py
 third_party/sbedecoder/parser.py
 third_party/sbedecoder/schema.py
 third_party/sbedecoder/typemap.py
+transcoder/Transcoder.py
 transcoder/__init__.py
 transcoder/main.py
 transcoder/test.py
 transcoder/version.py
 transcoder/message/DatacastField.py
 transcoder/message/DatacastGroup.py
 transcoder/message/DatacastParser.py
 transcoder/message/DatacastSchema.py
 transcoder/message/ErrorWriter.py
-transcoder/message/MessageParser.py
 transcoder/message/MessageUtil.py
+transcoder/message/NoParser.py
 transcoder/message/ParsedMessage.py
 transcoder/message/__init__.py
 transcoder/message/exception/MessageParserNotDefinedError.py
 transcoder/message/exception/ParserFunctionNotDefinedError.py
 transcoder/message/exception/__init__.py
 transcoder/message/factory/CmeMessageFactory.py
 transcoder/message/factory/ITCHMessageFactory.py
@@ -46,14 +48,15 @@
 transcoder/message/factory/MemxMessageFactory.py
 transcoder/message/factory/MessageFactory.py
 transcoder/message/factory/__init__.py
 transcoder/message/factory/exception/FactoryNotFoundError.py
 transcoder/message/factory/exception/TemplateSchemaNotDefinedError.py
 transcoder/message/factory/exception/__init__.py
 transcoder/message/handler/CmeBinaryPacketHandler.py
+transcoder/message/handler/FilterHandler.py
 transcoder/message/handler/MessageHandler.py
 transcoder/message/handler/MessageHandlerFloatField.py
 transcoder/message/handler/MessageHandlerIntField.py
 transcoder/message/handler/MessageHandlerStringField.py
 transcoder/message/handler/SequencerHandler.py
 transcoder/message/handler/TimestampPullForwardHandler.py
 transcoder/message/handler/__init__.py
@@ -78,14 +81,17 @@
 transcoder/output/google_cloud/__init__.py
 transcoder/output/google_cloud/terraform/BigQueryTerraformOutputManager.py
 transcoder/output/google_cloud/terraform/GcpTerraformOutputManager.py
 transcoder/output/google_cloud/terraform/PubSubTerraformOutputManager.py
 transcoder/output/google_cloud/terraform/__init__.py
 transcoder/output/json/JsonOutputManager.py
 transcoder/output/json/__init__.py
+transcoder/output/length_delimited/LengthDelimitedOutputManager.py
+transcoder/output/length_delimited/__init__.py
+transcoder/source/LineEncoding.py
 transcoder/source/Source.py
 transcoder/source/SourceUtil.py
 transcoder/source/__init__.py
 transcoder/source/file/CmeBinaryPacketFileMessageSource.py
 transcoder/source/file/FileMessageSource.py
 transcoder/source/file/LengthDelimitedFileMessageSource.py
 transcoder/source/file/LineDelimitedFileMessageSource.py
```

### Comparing `market-data-transcoder-1.0.1/setup.cfg` & `market-data-transcoder-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/third_party/__init__.py` & `market-data-transcoder-1.0.2/third_party/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/third_party/pyfixmsg/__init__.py` & `market-data-transcoder-1.0.2/third_party/pyfixmsg/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/third_party/pyfixmsg/codecs/__init__.py` & `market-data-transcoder-1.0.2/third_party/pyfixmsg/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/third_party/pyfixmsg/codecs/stringfix.py` & `market-data-transcoder-1.0.2/third_party/pyfixmsg/codecs/stringfix.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/third_party/pyfixmsg/exception/FixSchemaNotDefinedError.py` & `market-data-transcoder-1.0.2/third_party/pyfixmsg/exception/FixSchemaNotDefinedError.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/third_party/pyfixmsg/exception/__init__.py` & `market-data-transcoder-1.0.2/third_party/pyfixmsg/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/third_party/pyfixmsg/fixmessage.py` & `market-data-transcoder-1.0.2/third_party/pyfixmsg/fixmessage.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/third_party/pyfixmsg/parser.py` & `market-data-transcoder-1.0.2/third_party/pyfixmsg/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed to the Apache Software Foundation (ASF) under one or more
 # contributor license agreements.  See the NOTICE file distributed with
 # this work for additional information regarding copyright ownership.
 # The ASF licenses this file to You under the Apache License, Version 2.0
 # (the "License"); you may not use this file except in compliance with
 # the License.  You may obtain a copy of the License at
@@ -36,18 +36,19 @@
 class FixParser(DatacastParser):
     """Fix message parser"""
 
     @staticmethod
     def supported_factory_types():
         return ['fix']
 
-    def __init__(self, schema_file_path: str, sampling_count: int = None, message_type_inclusions: str = None,
-                 message_type_exclusions: str = None, fix_header_tags: str = None, fix_separator: int = 1,
+    def __init__(self, schema_file_path: str,  # pylint: disable=too-many-arguments
+                 message_type_inclusions: str = None, message_type_exclusions: str = None,
+                 fix_header_tags: str = None, fix_separator: int = 1,
                  stats_only: bool = False):
-        super().__init__(sampling_count=sampling_count, message_type_inclusions=message_type_inclusions,
+        super().__init__(message_type_inclusions=message_type_inclusions,
                          message_type_exclusions=message_type_exclusions, stats_only=stats_only)
         self.schema_file_path = schema_file_path
         self.fix_header_tags = fix_header_tags
         self.fix_separator = fix_separator
         self.spec = FixSpec(schema_file_path)
 
         # The codec will use the given spec to find repeating groups
```

### Comparing `market-data-transcoder-1.0.1/third_party/pyfixmsg/reference.py` & `market-data-transcoder-1.0.2/third_party/pyfixmsg/reference.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/third_party/pyfixmsg/util.py` & `market-data-transcoder-1.0.2/third_party/pyfixmsg/util.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/third_party/sbedecoder/message.py` & `market-data-transcoder-1.0.2/third_party/sbedecoder/message.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/third_party/sbedecoder/parser.py` & `market-data-transcoder-1.0.2/third_party/sbedecoder/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 class SBEParser(DatacastParser):
     """SBE message parser"""
 
     @staticmethod
     def supported_factory_types():
         return ['cme', 'itch', 'memx']
 
-    def __init__(self, msg_factory, sampling_count: int = None, message_type_inclusions: str = None,
+    def __init__(self, msg_factory, message_type_inclusions: str = None,
                  message_type_exclusions: str = None, stats_only: bool = False):
-        super().__init__(sampling_count=sampling_count, message_type_inclusions=message_type_inclusions,
+        super().__init__(message_type_inclusions=message_type_inclusions,
                          message_type_exclusions=message_type_exclusions, stats_only=stats_only)
         self.factory = msg_factory
 
     def parse(self, message_buffer, offset=0):
         """Passes a message buffer to the factory for processing"""
         msg_offset = offset
         while msg_offset < len(message_buffer):
```

### Comparing `market-data-transcoder-1.0.1/third_party/sbedecoder/schema.py` & `market-data-transcoder-1.0.2/third_party/sbedecoder/schema.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/third_party/sbedecoder/typemap.py` & `market-data-transcoder-1.0.2/third_party/sbedecoder/typemap.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/__init__.py` & `market-data-transcoder-1.0.2/transcoder/source/LineEncoding.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,20 +15,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from enum import Enum
 
-from .version import __version__
-
-
-# pylint: disable=invalid-name
-
-
 class LineEncoding(Enum):
     """Line encoding types supported for individual message decoding before processing"""
     NONE = 0
     BASE_64 = 1
     BASE_64_URL_SAFE = 2
 
     @classmethod
```

### Comparing `market-data-transcoder-1.0.1/transcoder/main.py` & `market-data-transcoder-1.0.2/transcoder/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,40 +18,39 @@
 # limitations under the License.
 #
 
 # pylint: disable=invalid-name
 # pylint: disable=too-many-locals
 # pylint: disable=too-many-statements
 
-"""Datacast Transcoder
-This script provides a default implementation for the Datacast Transcoder MessageParser class.
+"""
+CLI entry point for the market data transcoding API
 """
 
 import argparse
 import logging
 import os
 
-from transcoder import __version__, LineEncoding
-from transcoder.message.MessageParser import MessageParser
 from transcoder.message.factory import all_supported_factory_types
 from transcoder.output import all_output_identifiers
 from transcoder.source import all_source_identifiers
+from transcoder import Transcoder, __version__
 
 script_dir = os.path.dirname(__file__)
 
 
 def main():
     """main entry point for Datacast Transcoder"""
     arg_parser = argparse.ArgumentParser(description='Datacast Transcoder process input arguments', allow_abbrev=False)
 
     source_options_group = arg_parser.add_argument_group('Input source arguments')
-    source_options_group.add_argument('--factory', required=True, choices=all_supported_factory_types(),
+    source_options_group.add_argument('--factory', choices=all_supported_factory_types(),
                                       help='Message factory for decoding')
-    source_options_group.add_argument('--schema_file', required=True, type=str, help='Path to the schema file')
-    source_options_group.add_argument('--source_file', required=False, type=str, help='Path to the source file')
+    source_options_group.add_argument('--schema_file', type=str, help='Path to the schema file')
+    source_options_group.add_argument('--source_file', type=str, help='Path to the source file')
     source_options_group.add_argument('--source_file_encoding', type=str, default='utf-8', help='The source file '
                                                                                                 'character encoding')
     source_options_group.add_argument('--source_file_format_type', required=True, choices=all_source_identifiers(),
                                       help='The source file format')
 
     base64_group = source_options_group.add_mutually_exclusive_group()
     base64_group.add_argument('--base64', action='store_true',
@@ -67,14 +66,17 @@
     source_options_group.add_argument('--message_handlers', type=str, help='Comma delimited list of message '
                                                                            'handlers in priority order')
     source_options_group.add_argument('--message_skip_bytes', type=int, default=0,
                                       help='Number of bytes to skip before processing individual messages within a '
                                            'repeated '
                                            'length delimited file message source')
 
+    source_options_group.add_argument('--prefix_length', type=int, default=2,
+                                      help='How many bytes to use for the length prefix of length-delimited binary '
+                                           'sources')
     message_filter_group = source_options_group.add_mutually_exclusive_group()
     message_filter_group.add_argument('--message_type_exclusions', type=str,
                                       help='Comma-delimited list of message types to exclude '
                                            'when processing')
     message_filter_group.add_argument('--message_type_inclusions', type=str,
                                       help='Comma-delimited list of message types to include '
                                            'when processing')
@@ -101,14 +103,17 @@
                                            'errorOut')
     output_options_group.add_argument('--lazy_create_resources', action='store_true',
                                       help='Flag indicating that output resources for message types '
                                            'should be only created as messages of each type are encountered in the '
                                            'source data. Default behavior is to create resources for each message '
                                            'type before messages are processed. Particularly useful when working with '
                                            'FIX but only processing a limited set of message types in the source data')
+    output_options_group.add_argument('--frame_only', action='store_true',
+                                      help='Flag indicating that transcoder should only frame messages to an output '
+                                           'source')
     output_options_group.add_argument('--stats_only', action='store_true',
                                       help='Flag indicating that transcoder should only report on message type counts '
                                            'without parsing messages further')
     output_options_group.add_argument('--create_schemas_only', action='store_true',
                                       help='Flag indicating that transcoder should only create output resource '
                                            'schemas and not output message data')
 
@@ -146,55 +151,47 @@
 
     factory = args.factory
     schema_file_path = os.path.expanduser(args.schema_file) if args.schema_file else None
     source_file_path = os.path.expanduser(args.source_file) if args.source_file else None
     source_file_encoding = args.source_file_encoding
     source_file_format_type = args.source_file_format_type
     source_file_endian = args.source_file_endian
+    prefix_length = args.prefix_length
     skip_lines = args.skip_lines
     skip_bytes = args.skip_bytes
     message_skip_bytes = args.message_skip_bytes
     quiet = args.quiet
     output_type = args.output_type
     output_encoding = args.output_encoding
     output_path = os.path.expanduser(args.output_path) if args.output_path is not None else None
     error_output_path = os.path.expanduser(args.error_output_path) if args.error_output_path is not None else None
     destination_project_id = args.destination_project_id
     destination_dataset_id = args.destination_dataset_id
     message_handlers = args.message_handlers
     lazy_create_resources = args.lazy_create_resources
+    frame_only = args.frame_only
     stats_only = args.stats_only
     create_schemas_only = args.create_schemas_only
     continue_on_error = args.continue_on_error
     create_schema_enforcing_topics = args.create_schema_enforcing_topics
     sampling_count = args.sampling_count
     message_type_inclusions = args.message_type_inclusions
     message_type_exclusions = args.message_type_exclusions
     fix_header_tags = args.fix_header_tags
     fix_separator = args.fix_separator
+    base64 = args.base64
+    base64_urlsafe = args.base64_urlsafe
 
-    line_encoding = None
-    if args.base64 is True:
-        line_encoding = LineEncoding.BASE_64
-    elif args.base64_urlsafe is True:
-        line_encoding = LineEncoding.BASE_64_URL_SAFE
-
-    message_parser = MessageParser(factory, schema_file_path,
-                                   source_file_path, source_file_encoding, source_file_format_type,
-                                   source_file_endian, skip_lines=skip_lines, skip_bytes=skip_bytes,
-                                   message_skip_bytes=message_skip_bytes, line_encoding=line_encoding,
-                                   output_type=output_type, output_path=output_path, output_encoding=output_encoding,
-                                   destination_project_id=destination_project_id,
-                                   destination_dataset_id=destination_dataset_id,
-                                   message_handlers=message_handlers, lazy_create_resources=lazy_create_resources,
-                                   stats_only=stats_only, create_schemas_only=create_schemas_only,
-                                   continue_on_error=continue_on_error, error_output_path=error_output_path,
-                                   quiet=quiet, create_schema_enforcing_topics=create_schema_enforcing_topics,
-                                   sampling_count=sampling_count, message_type_inclusions=message_type_inclusions,
-                                   message_type_exclusions=message_type_exclusions,
-                                   fix_header_tags=fix_header_tags, fix_separator=fix_separator)
+    txcode = Transcoder(factory, schema_file_path, source_file_path, source_file_encoding,
+                        source_file_format_type, source_file_endian, prefix_length, skip_lines,
+                        skip_bytes, message_skip_bytes, quiet, output_type, output_encoding,
+                        output_path, error_output_path, destination_project_id, destination_dataset_id,
+                        message_handlers, lazy_create_resources, frame_only, stats_only,
+                        create_schemas_only, continue_on_error, create_schema_enforcing_topics,
+                        sampling_count, message_type_inclusions, message_type_exclusions,
+                        fix_header_tags, fix_separator, base64, base64_urlsafe)
 
-    message_parser.process()
+    txcode.transcode()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `market-data-transcoder-1.0.1/transcoder/message/DatacastField.py` & `market-data-transcoder-1.0.2/transcoder/message/DatacastField.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/message/DatacastGroup.py` & `market-data-transcoder-1.0.2/transcoder/message/DatacastGroup.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/message/DatacastParser.py` & `market-data-transcoder-1.0.2/transcoder/message/DatacastParser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed to the Apache Software Foundation (ASF) under one or more
 # contributor license agreements.  See the NOTICE file distributed with
 # this work for additional information regarding copyright ownership.
 # The ASF licenses this file to You under the Apache License, Version 2.0
 # (the "License"); you may not use this file except in compliance with
 # the License.  You may obtain a copy of the License at
@@ -16,33 +16,31 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from transcoder.message import DatacastSchema, ParsedMessage
 from transcoder.message.exception import ParserFunctionNotDefinedError
 
-
 class DatacastParser:
     """Class encapsulating message parsing and processing functionality """
 
     @staticmethod
     def supported_factory_types():
         """Static method for retrieving list of provider-specific factory classes"""
         raise ParserFunctionNotDefinedError
 
-    def __init__(self, sampling_count: int = None, stats_only: bool = False,
+    def __init__(self, stats_only: bool = False,
                  message_type_inclusions: str = None, message_type_exclusions: str = None):
-        self.sampling_count = sampling_count
         self.stats_only = stats_only
         self.message_type_inclusions = message_type_inclusions.split(
             ',') if message_type_inclusions is not None else None
         self.message_type_exclusions = message_type_exclusions.split(
             ',') if message_type_exclusions is not None else None
         self.use_message_type_filtering = message_type_inclusions is not None or message_type_exclusions is not None
-        self.use_sampling = sampling_count is not None and sampling_count > 0
+
         self.record_count = 0
         self.summary_count = {}
         self.total_schema_count = 0
         self.error_summary_count = {}
 
     @property
     def record_type_count(self):
@@ -65,27 +63,25 @@
         filtered_list = list(filter(lambda x: self.__include_message_type(x.name), schema_list))
         self.total_schema_count = len(filtered_list)
         for name in list(map(lambda x: x.name, filtered_list)):
             self.summary_count[name] = 0
         return filtered_list
 
     def _process_schema(self) -> [DatacastSchema]:
+        """Function for sub-class to implement for processing schema"""
         raise ParserFunctionNotDefinedError
 
     def process_message(self, raw_msg) -> ParsedMessage:
         """Wraps _process_message with count and inclusion behavior"""
+
         message = self._process_message(raw_msg)
 
         if message is None:
             return None
 
-        if self.use_sampling is True and self.get_summary_count(message.name) >= self.sampling_count:
-            message.ignored = True
-            return message
-
         if self.__include_message_type(message.name) is False:
             message.ignored = True
             return message
 
         self.increment_summary_count(message.name)
 
         if self.stats_only is True:
```

### Comparing `market-data-transcoder-1.0.1/transcoder/message/DatacastSchema.py` & `market-data-transcoder-1.0.2/transcoder/message/DatacastSchema.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/message/ErrorWriter.py` & `market-data-transcoder-1.0.2/transcoder/message/ErrorWriter.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
 from transcoder.message import ParsedMessage
 
 
 class TranscodeStep(Enum):
     """Enum of steps at which an error may be encountered"""
     UNKNOWN = 'UNKNOWN'
-    DECODE_MESSAGE = 'decode_message'
     PARSE_MESSAGE = 'parse_message'
     EXECUTE_HANDLERS = 'execute_handlers'
     EXECUTE_HANDLER = 'execute_handler'
     WRITE_OUTPUT_RECORD = 'write_output_record'
 
     @classmethod
     def _missing_(cls, value):
```

### Comparing `market-data-transcoder-1.0.1/transcoder/message/MessageParser.py` & `market-data-transcoder-1.0.2/transcoder/Transcoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed to the Apache Software Foundation (ASF) under one or more
 # contributor license agreements.  See the NOTICE file distributed with
 # this work for additional information regarding copyright ownership.
 # The ASF licenses this file to You under the Apache License, Version 2.0
 # (the "License"); you may not use this file except in compliance with
 # the License.  You may obtain a copy of the License at
@@ -20,107 +20,155 @@
 # pylint: disable=broad-except
 
 import importlib
 import logging
 import os
 import signal
 import sys
+
 from datetime import datetime
 
-from transcoder import LineEncoding
-from transcoder.message import DatacastParser, ParsedMessage
+from transcoder.message.MessageUtil import get_message_parser, parse_handler_config
+from transcoder.message import DatacastParser, NoParser
 from transcoder.message.ErrorWriter import ErrorWriter, TranscodeStep
-from transcoder.message.MessageUtil import get_message_parser
-from transcoder.output import OutputManager
-from transcoder.output.OutputUtil import get_output_manager
-from transcoder.source import Source
-from transcoder.source.SourceUtil import get_message_source
+from transcoder.output import get_output_manager
+from transcoder.source import get_message_source
 
 
-class MessageParser:  # pylint: disable=too-many-instance-attributes
-    """Main entry point for message transcoding"""
+# pylint: disable=invalid-name
+class Transcoder:  # pylint: disable=too-many-instance-attributes
+    """ Main entry point for transcodihg sessions, bounded by a schema, source and parser """
 
     def __init__(self,  # pylint: disable=too-many-arguments),too-many-locals
-                 factory, schema_file_path: str,
-                 source_file_path: str, source_file_encoding: str, source_file_format_type: str,
-                 source_file_endian: str, skip_lines: int = 0, skip_bytes: int = 0, message_skip_bytes: int = 0,
-                 line_encoding: LineEncoding = None, output_type: str = None, output_path: str = None,
-                 output_encoding: str = None, destination_project_id: str = None, destination_dataset_id: str = None,
-                 message_handlers: str = None, lazy_create_resources: bool = False,
-                 stats_only: bool = False, create_schemas_only: bool = False,
-                 continue_on_error: bool = False, error_output_path: str = None, quiet: bool = False,
-                 create_schema_enforcing_topics: bool = True, sampling_count: int = None,
-                 message_type_inclusions: str = None, message_type_exclusions: str = None,
-                 fix_header_tags: str = None, fix_separator: int = 1):
+                 factory: str, schema_file_path: str, source_file_path: str, source_file_encoding: str,
+                 source_file_format_type: str, source_file_endian: str, prefix_length: int, skip_lines: int,
+                 skip_bytes: int, message_skip_bytes: int, quiet: bool, output_type: str, output_encoding: str,
+                 output_path: str, error_output_path: str, destination_project_id: str, destination_dataset_id: str,
+                 message_handlers: str, lazy_create_resources: bool, frame_only: bool, stats_only: bool,
+                 create_schemas_only: bool, continue_on_error: bool, create_schema_enforcing_topics: bool,
+                 sampling_count: int, message_type_inclusions: str, message_type_exclusions: str, fix_header_tags: str,
+                 fix_separator: int, base64: bool, base64_urlsafe: bool):
 
-        self.start_time = None
-        self.source = None
-        self.source_file_path = source_file_path
-        self.source_file_encoding = source_file_encoding
-        self.source_file_format_type = source_file_format_type
-        self.source_file_endian = source_file_endian
-        self.skip_lines = skip_lines
-        self.skip_bytes = skip_bytes
-        self.message_skip_bytes = message_skip_bytes
-        self.line_encoding = line_encoding
-        self.continue_on_error = continue_on_error
-        self.error_output_path = error_output_path
-        self.lazy_create_resources = lazy_create_resources
-        self.quiet = quiet
-        self.create_schema_enforcing_topics = create_schema_enforcing_topics
-        self.create_schemas_only = create_schemas_only
-        self.output_manager: OutputManager = None
+        signal.signal(signal.SIGINT, self.trap)
+
+        self.message_handler_spec = message_handlers
         self.message_handlers = {}
         self.all_message_type_handlers = []
         self.all_handlers = []
         self.handlers_enabled = False
-        self.file_name_without_extension = os.path.basename(
+        self.continue_on_error = continue_on_error
+        self.error_output_path = error_output_path
+        self.output_encoding = output_encoding
+        self.frame_only = frame_only
+        self.create_schemas_only = create_schemas_only
+        self.lazy_create_resources = lazy_create_resources
+        self.prefix_length = prefix_length
+        self.quiet = quiet
+        self.start_time = None
+        self.stats_only = stats_only
+        self.sampling_count = sampling_count
+
+        self.output_prefix = os.path.basename(
             os.path.splitext(source_file_path)[0]) if source_file_path else 'stdin'
 
-        self.error_writer = ErrorWriter(prefix=self.file_name_without_extension,
+        self.error_writer = ErrorWriter(prefix=self.output_prefix,
                                         output_path=self.error_output_path)
 
-        if output_type is not None:
-            self.output_manager = get_output_manager(output_type,
-                                                     output_prefix=self.file_name_without_extension,
-                                                     output_file_path=output_path,
-                                                     output_encoding=output_encoding,
-                                                     destination_project_id=destination_project_id,
-                                                     destination_dataset_id=destination_dataset_id,
-                                                     lazy_create_resources=lazy_create_resources,
-                                                     create_schema_enforcing_topics=create_schema_enforcing_topics)
+        self.output_manager = get_output_manager(output_type, self.output_prefix, output_path,
+                                                 output_encoding, self.prefix_length, destination_project_id,
+                                                 destination_dataset_id, lazy_create_resources,
+                                                 create_schema_enforcing_topics)
+
+        # TODO: think about this abstraction some more
+        if self.output_manager.supports_data_writing() is False:
+            self.create_schemas_only = True
+        else:
+            self.source = get_message_source(source_file_path, source_file_encoding,
+                                             source_file_format_type, source_file_endian,
+                                             skip_bytes, skip_lines, message_skip_bytes,
+                                             prefix_length, base64, base64_urlsafe)
+
+        self.message_parser: DatacastParser = NoParser() if self.frame_only else get_message_parser(
+            factory,
+            schema_file_path,
+            stats_only,
+            message_type_inclusions,
+            message_type_exclusions,
+            fix_header_tags,
+            fix_separator
+        )
+
+        self.setup_handlers()
 
-            if self.output_manager.supports_data_writing() is False:
-                self.create_schemas_only = True
+    def transcode(self):
+        """Entry point for transcoding session"""
+        self.start_time = datetime.now()
+        if self.frame_only is False:
+            self.process_schemas()
 
-        self.setup_handlers(message_handlers)
-        self.message_parser: DatacastParser = get_message_parser(factory, schema_file_path,
-                                                                 sampling_count=sampling_count,
-                                                                 stats_only=stats_only,
-                                                                 message_type_inclusions=message_type_inclusions,
-                                                                 message_type_exclusions=message_type_exclusions,
-                                                                 fix_header_tags=fix_header_tags,
-                                                                 fix_separator=fix_separator)
+        with self.source:
+            for raw_msg in self.source.get_message_iterator():
+                if self.frame_only:  # don't parse message
+                    self.message_parser.process_message(raw_msg)
+                    self.output_manager.write_record(None, raw_msg)
+                else:  # parse message
+                    if self.stats_only is False:  # output message
+                        self.transcode_message(raw_msg)
 
-        signal.signal(signal.SIGINT, self.trap)
+                if self.message_parser.record_count == self.sampling_count:
+                    break
+
+        self.print_summary()
 
-    def setup_handlers(self, message_handlers: str):
+    def transcode_message(self, raw):
+        """ Transcoding steps executed on each source message """
+        self.error_writer.set_step(TranscodeStep.PARSE_MESSAGE)
+        msg = None
+        try:
+            msg = self.message_parser.process_message(raw)
+
+            if msg.exception is not None:
+                self.handle_exception(raw, msg, msg.exception)
+
+            if msg.ignored is False:  # passed inclusions / exclusions
+                self.execute_handlers(msg)
+                if msg.ignored is False:  # passed filters
+                    self.error_writer.set_step(TranscodeStep.WRITE_OUTPUT_RECORD)
+                    self.output_manager.write_record(msg.name, msg.dictionary)
+        except Exception as ex:
+            self.handle_exception(raw, msg, ex)
+
+    def execute_handlers(self, message):
+        """ Executes in sequence the message handlers specified for this transcoding instance """
+        if self.handlers_enabled is True:  # execute handlers
+            self.error_writer.set_step(TranscodeStep.EXECUTE_HANDLERS)
+            for handler in self.all_message_type_handlers + self.message_handlers.get(message.type, []):
+                self.error_writer.set_step(TranscodeStep.EXECUTE_HANDLER, type(handler).__name__)
+                handler.handle(message)
+
+    def setup_handlers(self):
         """Initialize MessageHandler instances to employ at runtime"""
 
-        if message_handlers is None or message_handlers == "":
-            return
-        if self.create_schemas_only is True:
+        if self.message_handler_spec is None or self.message_handler_spec == "":
             return
 
         self.handlers_enabled = True
-        handler_strs = message_handlers.split()
-        for handler_cls_name in handler_strs:
+        handler_strs = self.message_handler_spec.split(',')
+        for handler_spec in handler_strs:
+            cls_name = None
+            config_dict = None
+            if handler_spec.find(':') == -1:  # no handler params
+                cls_name = handler_spec
+            else:
+                cls_name = handler_spec.split(':')[0]
+                config_dict = parse_handler_config(handler_spec)
+
             module = importlib.import_module('transcoder.message.handler')
-            class_ = getattr(module, handler_cls_name)
-            instance = class_(self)
+            class_ = getattr(module, cls_name)
+            instance = class_(config_dict)
             self.all_handlers.append(instance)
 
             if instance.supports_all_message_types is True:
                 self.all_message_type_handlers.append(instance)
                 continue
 
             supported_msg_types = instance.supported_message_types
@@ -128,65 +176,51 @@
                 if supported_type in self.message_handlers:
                     handler_list = self.message_handlers[supported_type]
                     if instance not in handler_list:
                         self.message_handlers[supported_type].append(instance)
                 else:
                     self.message_handlers[supported_type] = [instance]
 
-    def process(self):
-        """Entry point for individual message processing"""
-        self.start_time = datetime.now()
-        self.process_schemas()
-
-        if self.create_schemas_only is False:
-            self.source: Source = get_message_source(self.source_file_path, self.source_file_encoding,
-                                                     self.source_file_format_type, self.source_file_endian,
-                                                     skip_lines=self.skip_lines, skip_bytes=self.skip_bytes,
-                                                     message_skip_bytes=self.message_skip_bytes,
-                                                     line_encoding=self.line_encoding)
-
-            self.process_data()
-
-        if self.output_manager is not None:
-            self.output_manager.wait_for_completion()
-
-        self.print_summary()
-
     def print_summary(self):
         """Print summary of the messages that were processed"""
         if logging.getLogger().isEnabledFor(logging.INFO):
             end_time = datetime.now()
             time_diff = end_time - self.start_time
             total_seconds = time_diff.total_seconds()
 
             if self.create_schemas_only is True:
                 logging.info('Run in create_schemas_only mode')
 
             if self.output_manager.supports_data_writing() is False:
                 logging.info('Output manager \'%s\' does not support message writes',
                              self.output_manager.output_type_identifier())
 
-            if self.message_parser.stats_only is True:
-                logging.info('Run in stats_only mode')
+            if self.frame_only is False:
 
-            if self.message_parser.use_sampling is True:
-                logging.info('Sampling count: %s', self.message_parser.sampling_count)
+                if self.message_parser.stats_only is True:
+                    logging.info('Run in stats_only mode')
 
-            if self.message_parser.message_type_inclusions is not None:
-                logging.info('Message type inclusions: %s', self.message_parser.message_type_inclusions)
-            elif self.message_parser.message_type_exclusions is not None:
-                logging.info('Message type exclusions: %s', self.message_parser.message_type_exclusions)
+                if self.sampling_count is not None:
+                    logging.info('Sampled messages: %s', self.sampling_count)
 
-            if self.create_schemas_only is False:
+                if self.message_parser.message_type_inclusions is not None:
+                    logging.info('Message type inclusions: %s', self.message_parser.message_type_inclusions)
+                elif self.message_parser.message_type_exclusions is not None:
+                    logging.info('Message type exclusions: %s', self.message_parser.message_type_exclusions)
+
+                if self.create_schemas_only is False:
+                    logging.info('Source record count: %s', self.source.record_count)
+                    logging.info('Processed record count: %s', self.message_parser.record_count)
+                    logging.info('Processed schema count: %s', self.message_parser.total_schema_count)
+                    logging.info('Summary of message counts: %s', self.message_parser.record_type_count)
+                    logging.info('Summary of error message counts: %s', self.message_parser.error_record_type_count)
+                    logging.info('Message rate: %s per second', round(self.source.record_count / total_seconds, 6))
+
+            else:
                 logging.info('Source record count: %s', self.source.record_count)
-                logging.info('Processed record count: %s', self.message_parser.record_count)
-                logging.info('Processed schema count: %s', self.message_parser.total_schema_count)
-                logging.info('Summary of message counts: %s', self.message_parser.record_type_count)
-                logging.info('Summary of error message counts: %s', self.message_parser.error_record_type_count)
-                logging.info('Message rate: %s per second', round(self.source.record_count / total_seconds, 6))
 
             logging.info('Total runtime in seconds: %s', round(total_seconds, 6))
             logging.info('Total runtime in minutes: %s', round(total_seconds / 60, 6))
 
     def process_schemas(self):
         """Process the schema specified at runtime"""
         spec_schemas = self.message_parser.process_schema()
@@ -202,48 +236,14 @@
 
             self.output_manager.enqueue_schema(schema)
 
         # Only need to wait if lazy create is off, and you want to force creation before data is read
         if self.lazy_create_resources is False:
             self.output_manager.wait_for_schema_creation()
 
-    def process_data(self):
-        """Entry point for individual message processing"""
-        with self.source:
-            for raw_record in self.source.get_message_iterator():
-                message: ParsedMessage = None
-                try:
-                    self.error_writer.set_step(TranscodeStep.DECODE_MESSAGE)
-                    self.error_writer.set_step(TranscodeStep.PARSE_MESSAGE)
-                    message = self.message_parser.process_message(raw_record)
-
-                    if message is None:
-                        continue
-
-                    if message.exception is not None:
-                        self.handle_exception(raw_record, message, message.exception)
-
-                    # For messages that contain no fields, the dictionary will be empty.
-                    # Skip as no schema is created for these.
-                    if message.is_empty():
-                        continue
-
-                    if self.handlers_enabled is True:
-                        self.error_writer.set_step(TranscodeStep.EXECUTE_HANDLERS)
-                        for handler in self.all_message_type_handlers + self.message_handlers.get(message.type, []):
-                            self.error_writer.set_step(TranscodeStep.EXECUTE_HANDLER, type(handler).__name__)
-                            handler.handle(message)
-
-                    if self.output_manager is not None:
-                        self.error_writer.set_step(TranscodeStep.WRITE_OUTPUT_RECORD)
-                        self.output_manager.write_record(message.name, message.dictionary)
-
-                except Exception as ex:
-                    self.handle_exception(raw_record, message, ex)
-
     def handle_exception(self, raw_record, message, exception):
         """Process exceptions encountered in the message processing runtime"""
         if message is not None:
             self.message_parser.increment_error_summary_count(message.name)
         else:
             self.message_parser.increment_error_summary_count()
```

### Comparing `market-data-transcoder-1.0.1/transcoder/message/MessageUtil.py` & `market-data-transcoder-1.0.2/transcoder/message/MessageUtil.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed to the Apache Software Foundation (ASF) under one or more
 # contributor license agreements.  See the NOTICE file distributed with
 # this work for additional information regarding copyright ownership.
 # The ASF licenses this file to You under the Apache License, Version 2.0
 # (the "License"); you may not use this file except in compliance with
 # the License.  You may obtain a copy of the License at
@@ -20,29 +20,54 @@
 from third_party.pyfixmsg.parser import FixParser
 from third_party.sbedecoder import SBEParser
 from transcoder.message import DatacastParser
 from transcoder.message.exception import MessageParserNotDefinedError
 from transcoder.message.factory.MessageFactory import get_message_factory
 
 
-def get_message_parser(factory: str, schema_file_path: str,
-                       sampling_count: int = None, stats_only: bool = False,
+def get_message_parser(factory: str, schema_file_path: str,  # pylint: disable=too-many-arguments
+                       stats_only: bool = False,
                        message_type_inclusions: str = None, message_type_exclusions: str = None,
                        fix_header_tags: str = None, fix_separator: int = 1) -> DatacastParser:
     """Returns a DatacastParser instance based on the supplied factory name"""
     message_parser: DatacastParser = None
     if factory in SBEParser.supported_factory_types():
         message_factory = get_message_factory(factory, schema_file_path)
-        message_parser = SBEParser(message_factory, sampling_count=sampling_count,
+        message_parser = SBEParser(message_factory,
                                    message_type_inclusions=message_type_inclusions,
                                    message_type_exclusions=message_type_exclusions,
                                    stats_only=stats_only)
     elif factory in FixParser.supported_factory_types():
-        message_parser = FixParser(schema_file_path=schema_file_path, sampling_count=sampling_count,
+        message_parser = FixParser(schema_file_path=schema_file_path,
                                    message_type_inclusions=message_type_inclusions,
                                    message_type_exclusions=message_type_exclusions,
                                    fix_header_tags=fix_header_tags, fix_separator=fix_separator,
                                    stats_only=stats_only)
     else:
         raise MessageParserNotDefinedError
 
     return message_parser
+
+
+def parse_handler_config(handler_config_string: str) -> dict:
+    """
+    Extracts the configuration parameters attached to the CLI handler option,
+    in the format:
+
+    FirstHandler:<param>=<value>,SecondHandler:<param>=<value>
+
+    For example:
+
+    --message_handlers SequencerHandler,FilterHandler:field=value
+
+    would run a SequencerHandler without a config, then pass a single-element dict of field: value to FilterHandler via the config object.
+
+    This routine manufactures the configuration for the Handler from the CLI string
+
+    """
+    if handler_config_string.find(':') != -1:
+        config = {}
+        params = handler_config_string.split(':')[1]
+        keyval = params.split('=')
+        config[keyval[0]] = keyval[1]
+        return config
+    return None
```

### Comparing `market-data-transcoder-1.0.1/transcoder/message/ParsedMessage.py` & `market-data-transcoder-1.0.2/transcoder/message/ParsedMessage.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/message/__init__.py` & `market-data-transcoder-1.0.2/transcoder/source/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,7 +14,9 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 # pylint: disable=invalid-name
+
+from .SourceUtil import all_source_identifiers, get_message_source
```

### Comparing `market-data-transcoder-1.0.1/transcoder/message/exception/MessageParserNotDefinedError.py` & `market-data-transcoder-1.0.2/transcoder/message/exception/MessageParserNotDefinedError.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/message/exception/ParserFunctionNotDefinedError.py` & `market-data-transcoder-1.0.2/transcoder/message/exception/ParserFunctionNotDefinedError.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/message/exception/__init__.py` & `market-data-transcoder-1.0.2/transcoder/message/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/message/factory/CmeMessageFactory.py` & `market-data-transcoder-1.0.2/transcoder/message/factory/CmeMessageFactory.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/message/factory/ITCHMessageFactory.py` & `market-data-transcoder-1.0.2/transcoder/message/factory/ITCHMessageFactory.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/message/factory/MDPMessageFactory.py` & `market-data-transcoder-1.0.2/transcoder/message/factory/MDPMessageFactory.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/message/factory/MemxMessageFactory.py` & `market-data-transcoder-1.0.2/transcoder/message/factory/MemxMessageFactory.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/message/factory/MessageFactory.py` & `market-data-transcoder-1.0.2/transcoder/message/factory/MessageFactory.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/message/factory/__init__.py` & `market-data-transcoder-1.0.2/transcoder/message/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/message/factory/exception/FactoryNotFoundError.py` & `market-data-transcoder-1.0.2/transcoder/message/factory/exception/FactoryNotFoundError.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/message/factory/exception/TemplateSchemaNotDefinedError.py` & `market-data-transcoder-1.0.2/transcoder/message/factory/exception/TemplateSchemaNotDefinedError.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/message/factory/exception/__init__.py` & `market-data-transcoder-1.0.2/transcoder/message/factory/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/message/handler/CmeBinaryPacketHandler.py` & `market-data-transcoder-1.0.2/transcoder/message/handler/CmeBinaryPacketHandler.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import math
 
-from transcoder.message import MessageParser, ParsedMessage, DatacastSchema
+from transcoder.message import ParsedMessage, DatacastSchema
 from transcoder.message.handler.MessageHandler import MessageHandler
 from transcoder.message.handler.MessageHandlerFloatField import MessageHandlerFloatField
 
 
 class CmeBinaryPacketHandler(MessageHandler):
     """CME binary package message handler which appends and computes a new field md_entry_calculated_px"""
 
-    def __init__(self, parser: MessageParser):
-        super().__init__(parser=parser)
+    def __init__(self):
+        super().__init__()
 
     def append_manufactured_fields(self, schema: DatacastSchema):
         if schema.name != 'MDIncrementalRefreshOrderBook47':
             schema.fields.append(MessageHandlerFloatField('timestamp_seconds'))
 
     def handle(self, message: ParsedMessage):
         if message.name == 'MDIncrementalRefreshOrderBook47':  # pylint: disable=too-many-nested-blocks
```

### Comparing `market-data-transcoder-1.0.1/transcoder/message/handler/MessageHandler.py` & `market-data-transcoder-1.0.2/transcoder/message/handler/MessageHandler.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-from transcoder.message import MessageParser, ParsedMessage
+from transcoder.message import ParsedMessage
 
 
 class MessageHandler:
     """Base class for handlers of specific message types"""
 
-    def __init__(self, parser: MessageParser):
-        self.parser = parser
+    def __init__(self, config=None):
+        self.config = config
         self.all_value: str = '__ALL__'
 
     @property
     def supports_all_message_types(self):
         """Returns whether handler class supports all message types within a given source"""
         return True
```

### Comparing `market-data-transcoder-1.0.1/transcoder/message/handler/MessageHandlerFloatField.py` & `market-data-transcoder-1.0.2/transcoder/message/handler/MessageHandlerFloatField.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/message/handler/MessageHandlerIntField.py` & `market-data-transcoder-1.0.2/transcoder/message/handler/MessageHandlerIntField.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/message/handler/MessageHandlerStringField.py` & `market-data-transcoder-1.0.2/transcoder/message/handler/MessageHandlerStringField.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/message/handler/SequencerHandler.py` & `market-data-transcoder-1.0.2/transcoder/message/handler/TimestampPullForwardHandler.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2023 Google LLC
+# Copyright 2022 Google LLC
 #
 # Licensed to the Apache Software Foundation (ASF) under one or more
 # contributor license agreements.  See the NOTICE file distributed with
 # this work for additional information regarding copyright ownership.
 # The ASF licenses this file to You under the Apache License, Version 2.0
 # (the "License"); you may not use this file except in compliance with
 # the License.  You may obtain a copy of the License at
@@ -13,28 +13,35 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-from transcoder.message import MessageParser, ParsedMessage, DatacastSchema
+from transcoder.message import ParsedMessage, DatacastSchema
 from transcoder.message.handler.MessageHandler import MessageHandler
 from transcoder.message.handler.MessageHandlerIntField import MessageHandlerIntField
 
 
-class SequencerHandler(MessageHandler):
-    """ Message handler to append a sequencer number to all messages transcoded from an arbitrary source.
-    Particularly useful when transcoding messages encapsulated in POSIX files where the original sequence numbers
-    were found within the pocket header and not the message itself """
-
-    def __init__(self, parser: MessageParser):
-        super().__init__(parser=parser)
-        self.sequence_number = 0
-        self.sequence_number_field_name = 'sequence_number'
+class TimestampPullForwardHandler(MessageHandler):
+
+    """Custom message handler that stores the 'second' value from the last message of type 'time_message',
+    and carries it forward into other message types not of type 'time_message'"""
+
+    def __init__(self, config=None):
+        super().__init__(config)
+        self.last_timestamp_message = None
+        self.last_epoch_seconds = None
+        self.time_message_type_name = 'time_message'
+        self.time_value_field_name = 'second'
+        self.new_timestamp_field_name = 'timestamp_seconds'
 
     def append_manufactured_fields(self, schema: DatacastSchema):
-        schema.fields.append(MessageHandlerIntField(self.sequence_number_field_name))
+        if schema.name != self.time_message_type_name:
+            schema.fields.append(MessageHandlerIntField(self.new_timestamp_field_name))
 
     def handle(self, message: ParsedMessage):
-        self.sequence_number += 1
-        message.dictionary[self.sequence_number_field_name] = self.sequence_number
+        if message.name == self.time_message_type_name:
+            self.last_timestamp_message = message.dictionary
+            self.last_epoch_seconds = int(message.dictionary[self.time_value_field_name])
+        else:
+            message.dictionary[self.new_timestamp_field_name] = self.last_epoch_seconds
```

### Comparing `market-data-transcoder-1.0.1/transcoder/message/handler/TimestampPullForwardHandler.py` & `market-data-transcoder-1.0.2/transcoder/source/file/LengthDelimitedFileMessageSource.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,34 +13,58 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-from transcoder.message import MessageParser, ParsedMessage, DatacastSchema
-from transcoder.message.handler.MessageHandler import MessageHandler
-from transcoder.message.handler.MessageHandlerIntField import MessageHandlerIntField
-
-
-class TimestampPullForwardHandler(MessageHandler):
-    """Custom message handler that stores the 'second' value from the last message of type 'time_message',
-    and carries it forward into other message types not of type 'time_message'"""
-
-    def __init__(self, parser: MessageParser):
-        super().__init__(parser=parser)
-        self.last_timestamp_message = None
-        self.last_epoch_seconds = None
-        self.time_message_type_name = 'time_message'
-        self.time_value_field_name = 'second'
-        self.new_timestamp_field_name = 'timestamp_seconds'
-
-    def append_manufactured_fields(self, schema: DatacastSchema):
-        if schema.name != self.time_message_type_name:
-            schema.fields.append(MessageHandlerIntField(self.new_timestamp_field_name))
-
-    def handle(self, message: ParsedMessage):
-        if message.name == self.time_message_type_name:
-            self.last_timestamp_message = message.dictionary
-            self.last_epoch_seconds = int(message.dictionary[self.time_value_field_name])
-        else:
-            message.dictionary[self.new_timestamp_field_name] = self.last_epoch_seconds
+from transcoder.source.file.FileMessageSource import FileMessageSource
+
+
+class LengthDelimitedFileMessageSource(FileMessageSource):
+    """Reads length delimited files and yields individual records for message consumption"""
+
+    @staticmethod
+    def source_type_identifier():
+        return 'length_delimited'
+
+    def __init__(self, file_path: str, skip_bytes: int = 0, endian: str = 'big',
+                 message_skip_bytes: int = 0, prefix_length: int = 2):
+        super().__init__(file_path, file_open_mode='rb')
+
+        self.skip_bytes = skip_bytes
+        self.endian = endian
+        self.message_skip_bytes = message_skip_bytes
+        self.prefix_length = prefix_length
+
+    def prepare(self):
+        if self.skip_bytes > 0:
+            self.file_handle.read(self.skip_bytes)
+
+    def get_message_iterator(self):
+        # pylint: disable=duplicate-code
+        while True:
+
+            # Read the message length
+            msg_len_bytes = self.file_handle.read(self.prefix_length) #self.message_length_byte_length) #self.message_length_byte_length) #self.message_length_byte_length)
+
+            if not msg_len_bytes:
+                break
+
+            message_length = int.from_bytes(msg_len_bytes, self.endian)
+            self.increment_count()
+
+            # Get the message
+            msg_bytes = self.file_handle.read(message_length)
+            if not msg_bytes:
+                break
+
+            if self.message_skip_bytes > 0:
+                # Skip bytes based on the message_skip_bytes value
+                skipped_bytes = self.file_handle.read(self.message_skip_bytes)
+                if not skipped_bytes:
+                    break
+                yield msg_bytes[self.message_skip_bytes:]
+            else:
+                yield msg_bytes
+
+            self._log_percentage_read()
```

### Comparing `market-data-transcoder-1.0.1/transcoder/message/handler/__init__.py` & `market-data-transcoder-1.0.2/transcoder/message/handler/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,7 +18,8 @@
 #
 
 # pylint: disable=invalid-name
 
 from .SequencerHandler import SequencerHandler
 from .CmeBinaryPacketHandler import CmeBinaryPacketHandler
 from .TimestampPullForwardHandler import TimestampPullForwardHandler
+from .FilterHandler import FilterHandler
```

### Comparing `market-data-transcoder-1.0.1/transcoder/output/OutputManager.py` & `market-data-transcoder-1.0.2/transcoder/output/OutputManager.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/output/OutputUtil.py` & `market-data-transcoder-1.0.2/transcoder/output/OutputUtil.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,36 +17,40 @@
 # limitations under the License.
 #
 
 from transcoder.output import OutputManager
 from transcoder.output.avro import AvroOutputManager
 from transcoder.output.avro.FastAvroOutputManager import FastAvroOutputManager
 from transcoder.output.diag import DiagnosticOutputManager
+from transcoder.output.length_delimited import LengthDelimitedOutputManager
 from transcoder.output.google_cloud import PubSubOutputManager, BigQueryOutputManager
 from transcoder.output.google_cloud.terraform import BigQueryTerraformOutputManager, PubSubTerraformOutputManager
 from transcoder.output.json import JsonOutputManager
 
 
-
 def all_output_identifiers():
     """List of all available source identifiers"""
     return [
         DiagnosticOutputManager.output_type_identifier(),
         AvroOutputManager.output_type_identifier(),
         FastAvroOutputManager.output_type_identifier(),
         BigQueryOutputManager.output_type_identifier(),
         PubSubOutputManager.output_type_identifier(),
         BigQueryTerraformOutputManager.output_type_identifier(),
         PubSubTerraformOutputManager.output_type_identifier(),
-        JsonOutputManager.output_type_identifier()
+        JsonOutputManager.output_type_identifier(),
+        LengthDelimitedOutputManager.output_type_identifier()
     ]
 
 
-def get_output_manager(output_name: str, output_prefix: str = None, output_file_path: str = None,
+def get_output_manager(output_name: str,  # pylint: disable=too-many-arguments
+                       output_prefix: str = None,
+                       output_file_path: str = None,
                        output_encoding: str = None,
+                       prefix_length: int = 2,
                        destination_project_id: str = None,
                        destination_dataset_id: str = None,
                        lazy_create_resources: bool = False,
                        create_schema_enforcing_topics: bool = True):
     """Returns OutputManager instance based on the supplied name"""
     output: OutputManager = None
     if output_name == AvroOutputManager.output_type_identifier():
@@ -66,14 +70,17 @@
         output = PubSubTerraformOutputManager(destination_project_id, output_encoding=output_encoding,
                                               create_schema_enforcing_topics=create_schema_enforcing_topics,
                                               output_path=output_file_path)
     elif output_name == DiagnosticOutputManager.output_type_identifier():
         output = DiagnosticOutputManager()
     elif output_name == JsonOutputManager.output_type_identifier():
         output = JsonOutputManager(output_prefix, output_file_path, lazy_create_resources=lazy_create_resources)
+    elif output_name == LengthDelimitedOutputManager.output_type_identifier():
+        # TODO: pass through output endian specification from CLI args
+        output = LengthDelimitedOutputManager(prefix_length=prefix_length)
     else:
         raise UnsupportedOutputTypeError(f'Output {output_name} is not supported')
     return output
 
 
 class UnsupportedOutputTypeError(Exception):
     """Exception that is raised when an output name cannot resolve to a child OutputManager class"""
```

### Comparing `market-data-transcoder-1.0.1/transcoder/output/__init__.py` & `market-data-transcoder-1.0.2/transcoder/message/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 # pylint: disable=invalid-name
 
-from .OutputManager import OutputManager
-from .OutputUtil import all_output_identifiers
+from .NoParser import NoParser
+from .DatacastParser import DatacastParser
```

### Comparing `market-data-transcoder-1.0.1/transcoder/output/avro/AvroOutputManager.py` & `market-data-transcoder-1.0.2/transcoder/output/avro/AvroOutputManager.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/output/avro/BaseAvroOutputManager.py` & `market-data-transcoder-1.0.2/transcoder/output/avro/BaseAvroOutputManager.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/output/avro/FastAvroOutputManager.py` & `market-data-transcoder-1.0.2/transcoder/output/avro/FastAvroOutputManager.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/output/avro/__init__.py` & `market-data-transcoder-1.0.2/transcoder/output/avro/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/output/diag/DiagnosticOutputManager.py` & `market-data-transcoder-1.0.2/transcoder/output/diag/DiagnosticOutputManager.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/output/diag/__init__.py` & `market-data-transcoder-1.0.2/transcoder/output/diag/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/output/exception/BigQueryTableSchemaOutOfSyncError.py` & `market-data-transcoder-1.0.2/transcoder/output/exception/BigQueryTableSchemaOutOfSyncError.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/output/exception/OutputFunctionNotDefinedError.py` & `market-data-transcoder-1.0.2/transcoder/output/exception/OutputFunctionNotDefinedError.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/output/exception/OutputManagerSchemaError.py` & `market-data-transcoder-1.0.2/transcoder/output/exception/OutputManagerSchemaError.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/output/exception/OutputNotAvailableError.py` & `market-data-transcoder-1.0.2/transcoder/output/exception/OutputNotAvailableError.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/output/exception/PubSubTopicSchemaOutOfSyncError.py` & `market-data-transcoder-1.0.2/transcoder/output/exception/PubSubTopicSchemaOutOfSyncError.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/output/exception/__init__.py` & `market-data-transcoder-1.0.2/transcoder/output/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/output/google_cloud/BigQueryOutputManager.py` & `market-data-transcoder-1.0.2/transcoder/output/google_cloud/BigQueryOutputManager.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/output/google_cloud/Constants.py` & `market-data-transcoder-1.0.2/transcoder/output/google_cloud/Constants.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/output/google_cloud/PubSubOutputManager.py` & `market-data-transcoder-1.0.2/transcoder/output/google_cloud/PubSubOutputManager.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/output/google_cloud/__init__.py` & `market-data-transcoder-1.0.2/transcoder/output/google_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/output/google_cloud/terraform/BigQueryTerraformOutputManager.py` & `market-data-transcoder-1.0.2/transcoder/output/google_cloud/terraform/BigQueryTerraformOutputManager.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/output/google_cloud/terraform/GcpTerraformOutputManager.py` & `market-data-transcoder-1.0.2/transcoder/output/google_cloud/terraform/GcpTerraformOutputManager.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/output/google_cloud/terraform/PubSubTerraformOutputManager.py` & `market-data-transcoder-1.0.2/transcoder/output/google_cloud/terraform/PubSubTerraformOutputManager.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/output/google_cloud/terraform/__init__.py` & `market-data-transcoder-1.0.2/transcoder/output/google_cloud/terraform/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/output/json/JsonOutputManager.py` & `market-data-transcoder-1.0.2/transcoder/output/json/JsonOutputManager.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/output/json/__init__.py` & `market-data-transcoder-1.0.2/transcoder/output/json/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/source/Source.py` & `market-data-transcoder-1.0.2/transcoder/source/Source.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/source/SourceUtil.py` & `market-data-transcoder-1.0.2/transcoder/source/SourceUtil.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,51 +13,65 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-from transcoder import LineEncoding
 from transcoder.source import Source
+from transcoder.source.LineEncoding import LineEncoding
 from transcoder.source.file import PcapFileMessageSource, LengthDelimitedFileMessageSource, \
     LineDelimitedFileMessageSource, CmeBinaryPacketFileMessageSource
 
 
 def all_source_identifiers():
     """List of all available source identifiers"""
     return [
         PcapFileMessageSource.source_type_identifier(),
         LengthDelimitedFileMessageSource.source_type_identifier(),
         LineDelimitedFileMessageSource.source_type_identifier(),
         CmeBinaryPacketFileMessageSource.source_type_identifier()
     ]
 
 
-def get_message_source(source_name: str,  # pylint: disable=too-many-arguments
+def get_message_source(source_loc: str,  # pylint: disable=too-many-arguments
                        source_file_encoding: str, source_file_format_type: str,
                        endian: str, skip_bytes: int = 0, skip_lines: int = 0,
-                       message_skip_bytes: int = 0, message_length_byte_length: int = 2,
-                       line_encoding: LineEncoding = None) -> Source:
+                        message_skip_bytes: int = 0, prefix_length: int = 2,
+                        base64: bool = False, base64_urlsafe: bool = False) -> Source:
     """Returns a Source implementation instance based on the supplied source name"""
+
     source: Source = None
+
     if source_file_format_type == PcapFileMessageSource.source_type_identifier():
-        source = PcapFileMessageSource(source_name, message_skip_bytes=message_skip_bytes)
+        source = PcapFileMessageSource(source_loc, message_skip_bytes=message_skip_bytes)
     elif source_file_format_type == LengthDelimitedFileMessageSource.source_type_identifier():
-        source = LengthDelimitedFileMessageSource(source_name, skip_bytes=skip_bytes,
+
+        source = LengthDelimitedFileMessageSource(source_loc, skip_bytes=skip_bytes,
                                                   message_skip_bytes=message_skip_bytes,
-                                                  message_length_byte_length=message_length_byte_length)
+                                                  prefix_length=prefix_length)
+
     elif source_file_format_type == LineDelimitedFileMessageSource.source_type_identifier():
-        source = LineDelimitedFileMessageSource(source_name, encoding=source_file_encoding,
+
+        if base64 is True:
+            line_encoding = LineEncoding.BASE_64
+        elif base64_urlsafe is True:
+            line_encoding = LineEncoding.BASE_64_URL_SAFE
+        else:
+            line_encoding = LineEncoding.NONE
+
+        source = LineDelimitedFileMessageSource(source_loc,
+                                                encoding=source_file_encoding,
                                                 skip_lines=skip_lines,
-                                                line_encoding=line_encoding, message_skip_bytes=message_skip_bytes)
+                                                line_encoding=line_encoding,
+                                                message_skip_bytes=message_skip_bytes)
     elif source_file_format_type == CmeBinaryPacketFileMessageSource.source_type_identifier():
-        source = CmeBinaryPacketFileMessageSource(source_name, endian, skip_bytes=skip_bytes,
+        source = CmeBinaryPacketFileMessageSource(source_loc, endian, skip_bytes=skip_bytes,
                                                   message_skip_bytes=message_skip_bytes,
-                                                  message_length_byte_length=message_length_byte_length)
+                                                  prefix_length=prefix_length)
     else:
-        raise UnsupportedFileTypeError(f'Source {source_name} is not supported')
+        raise UnsupportedFileTypeError(f'Source {source_loc} is not supported')
     return source
 
 
 class UnsupportedFileTypeError(Exception):
     """Exception that is raised when a file source type name cannot resolve to a child Source class"""
```

### Comparing `market-data-transcoder-1.0.1/transcoder/source/__init__.py` & `market-data-transcoder-1.0.2/transcoder/output/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 # pylint: disable=invalid-name
 
-from .SourceUtil import all_source_identifiers
+from .OutputManager import OutputManager
+from .OutputUtil import all_output_identifiers, get_output_manager
```

### Comparing `market-data-transcoder-1.0.1/transcoder/source/file/FileMessageSource.py` & `market-data-transcoder-1.0.2/transcoder/source/file/FileMessageSource.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,39 +13,35 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-import base64
 import logging
 import os
 import sys
 from io import IOBase
 
-from transcoder import LineEncoding
+
 from transcoder.source.Source import Source, SourceFunctionNotDefinedError
 
 
 class FileMessageSource(Source):
     """Abstract file message source class"""
 
     @staticmethod
     def source_type_identifier():
         raise SourceFunctionNotDefinedError
 
-    def __init__(self, file_path: str, file_open_mode: str, file_encoding: str = None,
-                 message_skip_bytes: int = 0, line_encoding: LineEncoding = None):
+    def __init__(self, file_path: str, file_open_mode: str, file_encoding: str = None):
         super().__init__()
         self.path = file_path
         self.file_open_mode = file_open_mode
         self.file_encoding = file_encoding
-        self.message_skip_bytes = message_skip_bytes
-        self.line_encoding = line_encoding
         self.file_handle: IOBase = None
         self.file_size = 0
         self.log_percentage_read_enabled = logging.getLogger().isEnabledFor(logging.DEBUG)
 
     def open(self):
         if self.path is not None:
             self.file_size = os.path.getsize(self.path)
@@ -70,22 +66,7 @@
 
     def get_message_iterator(self):
         raise SourceFunctionNotDefinedError
 
     def _log_percentage_read(self):
         if self.file_size and self.log_percentage_read_enabled is True:
             logging.debug('Percentage read: %f%%', round((self.file_handle.tell() / self.file_size) * 100, 6))
-
-    def decode_message(self, record):
-        """Performs line decoding and message skip bytes for line encoded cases"""
-        message = record
-        if self.line_encoding is LineEncoding.BASE_64:
-            message = base64.b64decode(record)
-        elif self.line_encoding is LineEncoding.BASE_64_URL_SAFE:
-            message = base64.urlsafe_b64decode(record)
-
-        if self.message_skip_bytes > 0 and isinstance(message, bytes):
-            # print(''.join('{:02x}'.format(x) for x in message))
-            message = message[self.message_skip_bytes:]
-            # print(''.join('{:02x}'.format(x) for x in message))
-
-        return message
```

### Comparing `market-data-transcoder-1.0.1/transcoder/source/file/LengthDelimitedFileMessageSource.py` & `market-data-transcoder-1.0.2/transcoder/source/file/LineDelimitedFileMessageSource.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,52 +13,56 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-from transcoder.source.file.FileMessageSource import FileMessageSource
+import sys
+import base64
 
+from transcoder.source.LineEncoding import LineEncoding
+from transcoder.source.file import FileMessageSource
 
-class LengthDelimitedFileMessageSource(FileMessageSource):
-    """Reads length delimited files and yields individual records for message consumption"""
+class LineDelimitedFileMessageSource(FileMessageSource):
+    """Reads line delimited files and yields individual records for message consumption"""
 
     @staticmethod
     def source_type_identifier():
-        return 'length_delimited'
+        return 'line_delimited'
 
-    def __init__(self, file_path: str, skip_bytes: int = 0, endian: str = 'big',
-                 message_skip_bytes: int = 0, message_length_byte_length: int = 2):
-        super().__init__(file_path, file_open_mode='rb')
-        self.skip_bytes = skip_bytes
-        self.endian = endian
+    def __init__(self, file_path: str, encoding: str, skip_lines: int = 0,
+                 message_skip_bytes: int = 0, line_encoding: LineEncoding = None):
+
+        super().__init__(file_path, file_open_mode='rt', file_encoding=encoding)
         self.message_skip_bytes = message_skip_bytes
-        self.message_length_byte_length = message_length_byte_length
+        self.line_encoding = line_encoding
+        self.skip_lines = skip_lines
 
     def prepare(self):
-        if self.skip_bytes > 0:
-            self.file_handle.read(self.skip_bytes)
+        # file_size is only determinable on seekable input
+        if sys.stdin.seekable() is True and self.file_size == 0:
+            return
+        if self.skip_lines > 0:
+            for _ in range(self.skip_lines):
+                self.file_handle.readline()
 
     def get_message_iterator(self):
-        # pylint: disable=duplicate-code
-        while True:
-            if self.message_skip_bytes > 0:
-                # Skip bytes based on the message_skip_bytes value
-                skipped_bytes = self.file_handle.read(self.message_skip_bytes)
-                if not skipped_bytes:
-                    break
-
-            # Read the message length
-            msg_len_bytes = self.file_handle.read(self.message_length_byte_length)
-            if not msg_len_bytes:
-                break
-
-            message_length = int.from_bytes(msg_len_bytes, self.endian)
+        while line := self.file_handle.readline():
             self.increment_count()
-
-            # Get the message
-            msg_bytes = self.file_handle.read(message_length)
-            if not msg_bytes:
-                break
-            yield msg_bytes
+            yield self.decode_message(line)
             self._log_percentage_read()
+
+    def decode_message(self, record):
+        """Performs line decoding and message skip bytes for line encoded cases"""
+        message = record
+        if self.line_encoding == LineEncoding.BASE_64.value:
+            message = base64.b64decode(record)
+        elif self.line_encoding == LineEncoding.BASE_64_URL_SAFE.value:
+            message = base64.urlsafe_b64decode(record)
+
+        if self.message_skip_bytes > 0 and isinstance(message, bytes):
+            # print(''.join('{:02x}'.format(x) for x in message))
+            message = message[self.message_skip_bytes:]
+            # print(''.join('{:02x}'.format(x) for x in message))
+
+        return message
```

### Comparing `market-data-transcoder-1.0.1/transcoder/source/file/LineDelimitedFileMessageSource.py` & `market-data-transcoder-1.0.2/transcoder/test.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,39 +13,35 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-import sys
+# pylint: disable=invalid-name
 
-from transcoder import LineEncoding
-from transcoder.source.file import FileMessageSource
+import unittest
 
 
-class LineDelimitedFileMessageSource(FileMessageSource):
-    """Reads line delimited files and yields individual records for message consumption"""
+class TestStringMethods(unittest.TestCase):
+    """TestCase implementation testing string methods"""
 
-    @staticmethod
-    def source_type_identifier():
-        return 'line_delimited'
-
-    def __init__(self, file_path: str, encoding: str, skip_lines: int = 0,
-                 message_skip_bytes: int = 0, line_encoding: LineEncoding = None):
-        super().__init__(file_path, file_open_mode='rt', file_encoding=encoding,
-                         line_encoding=line_encoding, message_skip_bytes=message_skip_bytes)
-        self.skip_lines = skip_lines
-
-    def prepare(self):
-        # file_size is only determinable on seekable input
-        if sys.stdin.seekable() is True and self.file_size == 0:
-            return
-        if self.skip_lines > 0:
-            for _ in range(self.skip_lines):
-                self.file_handle.readline()
-
-    def get_message_iterator(self):
-        while line := self.file_handle.readline():
-            self.increment_count()
-            yield self.decode_message(line)
-            self._log_percentage_read()
+    def test_upper(self):
+        """Tests ability to uppercase string"""
+        self.assertEqual('foo'.upper(), 'FOO')
+
+    def test_isupper(self):
+        """Tests uppercase-ness of string"""
+        self.assertTrue('FOO'.isupper())
+        self.assertFalse('Foo'.isupper())
+
+    def test_split(self):
+        """Tests strings split method and expected exception case"""
+        s = 'hello world'
+        self.assertEqual(s.split(), ['hello', 'world'])
+        # check that s.split fails when the separator is not a string
+        with self.assertRaises(TypeError):
+            s.split(2)  # type: ignore
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `market-data-transcoder-1.0.1/transcoder/source/file/PcapFileMessageSource.py` & `market-data-transcoder-1.0.2/transcoder/source/file/PcapFileMessageSource.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 class PcapFileMessageSource(FileMessageSource):
     """Reads pcap files and yields individual records for message consumption"""
 
     @staticmethod
     def source_type_identifier():
         return 'pcap'
 
-    def __init__(self, file_path: str, message_skip_bytes: int = 0, length_threshold: int = 50):
+    def __init__(self, file_path: str, message_skip_bytes: int = 0, length_threshold: int = 0):
         super().__init__(file_path, file_open_mode='rb')
         self.message_skip_bytes = message_skip_bytes
         self.pcap_reader: dpkt.pcap.Reader = None
         self.length_threshold = length_threshold
 
     def prepare(self):
         self.pcap_reader = dpkt.pcap.Reader(self.file_handle)
```

### Comparing `market-data-transcoder-1.0.1/transcoder/source/file/__init__.py` & `market-data-transcoder-1.0.2/transcoder/source/file/__init__.py`

 * *Files identical despite different names*

### Comparing `market-data-transcoder-1.0.1/transcoder/test.py` & `market-data-transcoder-1.0.2/transcoder/message/NoParser.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed to the Apache Software Foundation (ASF) under one or more
 # contributor license agreements.  See the NOTICE file distributed with
 # this work for additional information regarding copyright ownership.
 # The ASF licenses this file to You under the Apache License, Version 2.0
 # (the "License"); you may not use this file except in compliance with
 # the License.  You may obtain a copy of the License at
@@ -13,35 +13,23 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-# pylint: disable=invalid-name
+from .DatacastParser import DatacastParser
 
-import unittest
-
-
-class TestStringMethods(unittest.TestCase):
-    """TestCase implementation testing string methods"""
-
-    def test_upper(self):
-        """Tests ability to uppercase string"""
-        self.assertEqual('foo'.upper(), 'FOO')
-
-    def test_isupper(self):
-        """Tests uppercase-ness of string"""
-        self.assertTrue('FOO'.isupper())
-        self.assertFalse('Foo'.isupper())
-
-    def test_split(self):
-        """Tests strings split method and expected exception case"""
-        s = 'hello world'
-        self.assertEqual(s.split(), ['hello', 'world'])
-        # check that s.split fails when the separator is not a string
-        with self.assertRaises(TypeError):
-            s.split(2)  # type: ignore
-
-
-if __name__ == '__main__':
-    unittest.main()
+class NoParser(DatacastParser):
+    """ NOOP parser that simply maintains a record count. Intended to be used with the frame-only option. """
+    # pylint: disable=super-init-not-called
+
+    def __init__(self):
+        self.record_count = 0
+        self.summary_count = 0
+
+    # pylint: disable=unused-argument
+    def process_message(self, raw_msg=None):
+        """ Update message counter """
+        self.record_count += 1
+        self.summary_count += 1
+        return {}
```

### Comparing `market-data-transcoder-1.0.1/transcoder/version.py` & `market-data-transcoder-1.0.2/transcoder/version.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = '1.0.1'
+__version__ = '1.0.2'
```

