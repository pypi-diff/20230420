# Comparing `tmp/bovine-0.1.1.tar.gz` & `tmp/bovine-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine-0.1.1.tar", max compression
+gzip compressed data, was "bovine-0.1.2.tar", max compression
```

## Comparing `bovine-0.1.1.tar` & `bovine-0.1.2.tar`

### file list

```diff
@@ -1,96 +1,104 @@
--rw-r--r--   0        0        0      627 2023-04-15 18:19:16.463381 bovine-0.1.1/README.md
--rw-r--r--   0        0        0     8584 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 18:19:16.587382 bovine-0.1.1/bovine/activitypub/__init__.py
--rw-r--r--   0        0        0      173 2023-04-15 18:19:52.807613 bovine-0.1.1/bovine/activitypub/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3092 2023-04-15 18:19:52.807613 bovine-0.1.1/bovine/activitypub/__pycache__/authorization_wrapper.cpython-310.pyc
--rw-r--r--   0        0        0     2477 2023-04-15 18:19:53.195615 bovine-0.1.1/bovine/activitypub/__pycache__/collection_helper.cpython-310.pyc
--rw-r--r--   0        0        0      906 2023-04-15 18:19:53.303616 bovine-0.1.1/bovine/activitypub/__pycache__/collection_iterator.cpython-310.pyc
--rw-r--r--   0        0        0     3638 2023-04-15 18:19:53.311616 bovine-0.1.1/bovine/activitypub/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     2736 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitypub/authorization_wrapper.py
--rw-r--r--   0        0        0     2219 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitypub/collection_helper.py
--rw-r--r--   0        0        0      429 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitypub/collection_iterator.py
--rw-r--r--   0        0        0     2757 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitypub/test_actor.py
--rw-r--r--   0        0        0     4623 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitystreams/__init__.py
--rw-r--r--   0        0        0     4224 2023-04-15 18:19:53.295616 bovine-0.1.1/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4093 2023-04-15 18:19:53.295616 bovine-0.1.1/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc
--rw-r--r--   0        0        0     4086 2023-04-15 18:19:53.299616 bovine-0.1.1/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc
--rw-r--r--   0        0        0     4560 2023-04-15 18:19:53.343616 bovine-0.1.1/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     3305 2023-04-15 18:19:53.351616 bovine-0.1.1/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     3168 2023-04-15 18:19:53.359616 bovine-0.1.1/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     1929 2023-04-15 18:19:53.363616 bovine-0.1.1/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     1368 2023-04-15 18:19:53.367616 bovine-0.1.1/bovine/activitystreams/__pycache__/test_ordered_collection_page.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     4012 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitystreams/activity_factory.py
--rw-r--r--   0        0        0     4240 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitystreams/object_factory.py
--rw-r--r--   0        0        0     2163 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitystreams/test_activity_factory.py
--rw-r--r--   0        0        0     1418 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitystreams/test_actor.py
--rw-r--r--   0        0        0     1381 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitystreams/test_object_factory.py
--rw-r--r--   0        0        0     1010 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitystreams/test_ordered_collection_builder.py
--rw-r--r--   0        0        0      809 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitystreams/test_ordered_collection_page.py
--rw-r--r--   0        0        0     2354 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitystreams/utils/__init__.py
--rw-r--r--   0        0        0     2836 2023-04-15 18:19:53.299616 bovine-0.1.1/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      908 2023-04-15 18:19:53.303616 bovine-0.1.1/bovine/activitystreams/utils/__pycache__/print.cpython-310.pyc
--rw-r--r--   0        0        0     4763 2023-04-15 18:19:53.375616 bovine-0.1.1/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0      787 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitystreams/utils/print.py
--rw-r--r--   0        0        0     2266 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/activitystreams/utils/test_utils.py
--rw-r--r--   0        0        0     2081 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/__init__.py
--rw-r--r--   0        0        0     2209 2023-04-15 18:19:53.011614 bovine-0.1.1/bovine/clients/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      268 2023-04-15 18:19:53.011614 bovine-0.1.1/bovine/clients/__pycache__/consts.cpython-310.pyc
--rw-r--r--   0        0        0     1472 2023-04-15 18:19:53.191615 bovine-0.1.1/bovine/clients/__pycache__/event_source.cpython-310.pyc
--rw-r--r--   0        0        0     1014 2023-04-15 18:19:53.011614 bovine-0.1.1/bovine/clients/__pycache__/lookup_account.cpython-310.pyc
--rw-r--r--   0        0        0     2508 2023-04-15 18:19:53.015614 bovine-0.1.1/bovine/clients/__pycache__/moo_auth_client.cpython-310.pyc
--rw-r--r--   0        0        0     1237 2023-04-15 18:19:53.015614 bovine-0.1.1/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc
--rw-r--r--   0        0        0     2471 2023-04-15 18:19:53.191615 bovine-0.1.1/bovine/clients/__pycache__/signed_http.cpython-310.pyc
--rw-r--r--   0        0        0     1471 2023-04-15 18:19:53.191615 bovine-0.1.1/bovine/clients/__pycache__/signed_http_client.cpython-310.pyc
--rw-r--r--   0        0        0     1352 2023-04-15 18:19:53.383616 bovine-0.1.1/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     1576 2023-04-15 18:19:53.383616 bovine-0.1.1/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     1217 2023-04-15 18:19:53.387616 bovine-0.1.1/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     2094 2023-04-15 18:19:53.391616 bovine-0.1.1/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0      821 2023-04-15 18:19:53.391616 bovine-0.1.1/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0       91 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/consts.py
--rw-r--r--   0        0        0     1106 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/event_source.py
--rw-r--r--   0        0        0      787 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/lookup_account.py
--rw-r--r--   0        0        0     3176 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/moo_auth_client.py
--rw-r--r--   0        0        0      948 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/nodeinfo.py
--rw-r--r--   0        0        0     3278 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/signed_http.py
--rw-r--r--   0        0        0     1074 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/signed_http_client.py
--rw-r--r--   0        0        0      609 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/test_event_source.py
--rw-r--r--   0        0        0      624 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/test_lookup_account.py
--rw-r--r--   0        0        0      319 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/test_nodeinfo.py
--rw-r--r--   0        0        0     1145 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/test_signed_http.py
--rw-r--r--   0        0        0      529 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/clients/test_signed_http_client.py
--rw-r--r--   0        0        0     3999 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/crypto/__init__.py
--rw-r--r--   0        0        0     3634 2023-04-15 18:19:53.015614 bovine-0.1.1/bovine/crypto/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2863 2023-04-15 18:19:53.147615 bovine-0.1.1/bovine/crypto/__pycache__/helper.cpython-310.pyc
--rw-r--r--   0        0        0     2909 2023-04-15 18:19:53.151615 bovine-0.1.1/bovine/crypto/__pycache__/http_signature.cpython-310.pyc
--rw-r--r--   0        0        0     2257 2023-04-15 18:19:53.151615 bovine-0.1.1/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc
--rw-r--r--   0        0        0     1784 2023-04-15 18:19:53.191615 bovine-0.1.1/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc
--rw-r--r--   0        0        0     2363 2023-04-15 18:19:53.331616 bovine-0.1.1/bovine/crypto/__pycache__/test.cpython-310.pyc
--rw-r--r--   0        0        0     5810 2023-04-15 18:19:53.399617 bovine-0.1.1/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     2742 2023-04-15 18:19:53.403617 bovine-0.1.1/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     7454 2023-04-15 18:19:53.415617 bovine-0.1.1/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     2674 2023-04-15 18:19:53.423617 bovine-0.1.1/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     2664 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/crypto/helper.py
--rw-r--r--   0        0        0     2112 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/crypto/http_signature.py
--rw-r--r--   0        0        0     2942 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/crypto/signature_checker.py
--rw-r--r--   0        0        0     1266 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/crypto/signature_parser.py
--rw-r--r--   0        0        0     2199 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/crypto/test.py
--rw-r--r--   0        0        0     4989 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/crypto/test_crypto.py
--rw-r--r--   0        0        0      896 2023-04-15 18:19:16.463381 bovine-0.1.1/bovine/crypto/test_helper.py
--rw-r--r--   0        0        0     5081 2023-04-15 18:19:16.467381 bovine-0.1.1/bovine/crypto/test_http_signature.py
--rw-r--r--   0        0        0     1207 2023-04-15 18:19:16.467381 bovine-0.1.1/bovine/crypto/test_signature_parser.py
--rw-r--r--   0        0        0      178 2023-04-15 18:19:16.467381 bovine-0.1.1/bovine/test_bovine_client.py
--rw-r--r--   0        0        0      282 2023-04-15 18:19:16.467381 bovine-0.1.1/bovine/test_types.py
--rw-r--r--   0        0        0     2397 2023-04-15 18:19:16.467381 bovine-0.1.1/bovine/types.py
--rw-r--r--   0        0        0      667 2023-04-15 18:19:16.467381 bovine-0.1.1/bovine/utils/__init__.py
--rw-r--r--   0        0        0      848 2023-04-15 18:19:53.011614 bovine-0.1.1/bovine/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      877 2023-04-15 18:19:53.151615 bovine-0.1.1/bovine/utils/__pycache__/date.cpython-310.pyc
--rw-r--r--   0        0        0     3443 2023-04-15 18:19:53.431617 bovine-0.1.1/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0     1662 2023-04-15 18:19:53.435617 bovine-0.1.1/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0      973 2023-04-15 18:19:53.439617 bovine-0.1.1/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.0.pyc
--rw-r--r--   0        0        0      519 2023-04-15 18:19:16.467381 bovine-0.1.1/bovine/utils/date.py
--rw-r--r--   0        0        0      181 2023-04-15 18:19:16.467381 bovine-0.1.1/bovine/utils/test.py
--rw-r--r--   0        0        0      737 2023-04-15 18:19:16.467381 bovine-0.1.1/bovine/utils/test_date.py
--rw-r--r--   0        0        0      452 2023-04-15 18:19:16.467381 bovine-0.1.1/bovine/utils/test_parse.py
--rw-r--r--   0        0        0      191 2023-04-15 18:19:16.467381 bovine-0.1.1/bovine/utils/test_webfinger.py
--rw-r--r--   0        0        0     1178 2023-04-15 18:19:16.467381 bovine-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1523 1970-01-01 00:00:00.000000 bovine-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1364 2023-04-20 10:27:12.601485 bovine-0.1.2/README.md
+-rw-r--r--   0        0        0     8584 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-20 10:27:12.733486 bovine-0.1.2/bovine/activitypub/__init__.py
+-rw-r--r--   0        0        0      173 2023-04-20 10:27:49.365802 bovine-0.1.2/bovine/activitypub/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3092 2023-04-20 10:27:49.365802 bovine-0.1.2/bovine/activitypub/__pycache__/authorization_wrapper.cpython-310.pyc
+-rw-r--r--   0        0        0     2477 2023-04-20 10:27:49.785805 bovine-0.1.2/bovine/activitypub/__pycache__/collection_helper.cpython-310.pyc
+-rw-r--r--   0        0        0      906 2023-04-20 10:27:49.893806 bovine-0.1.2/bovine/activitypub/__pycache__/collection_iterator.cpython-310.pyc
+-rw-r--r--   0        0        0     3638 2023-04-20 10:27:49.901806 bovine-0.1.2/bovine/activitypub/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2736 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/activitypub/authorization_wrapper.py
+-rw-r--r--   0        0        0     2219 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/activitypub/collection_helper.py
+-rw-r--r--   0        0        0      429 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/activitypub/collection_iterator.py
+-rw-r--r--   0        0        0     2757 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/activitypub/test_actor.py
+-rw-r--r--   0        0        0     4682 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/activitystreams/__init__.py
+-rw-r--r--   0        0        0     4268 2023-04-20 10:27:49.885806 bovine-0.1.2/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4249 2023-04-20 10:27:49.885806 bovine-0.1.2/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc
+-rw-r--r--   0        0        0     4086 2023-04-20 10:27:49.889806 bovine-0.1.2/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc
+-rw-r--r--   0        0        0     4560 2023-04-20 10:27:50.065808 bovine-0.1.2/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     3305 2023-04-20 10:27:50.073808 bovine-0.1.2/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     3168 2023-04-20 10:27:50.077808 bovine-0.1.2/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1929 2023-04-20 10:27:50.081808 bovine-0.1.2/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1368 2023-04-20 10:27:50.085808 bovine-0.1.2/bovine/activitystreams/__pycache__/test_ordered_collection_page.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     4195 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/activitystreams/activity_factory.py
+-rw-r--r--   0        0        0     4240 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/activitystreams/object_factory.py
+-rw-r--r--   0        0        0     2163 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/activitystreams/test_activity_factory.py
+-rw-r--r--   0        0        0     1418 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/activitystreams/test_actor.py
+-rw-r--r--   0        0        0     1381 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/activitystreams/test_object_factory.py
+-rw-r--r--   0        0        0     1010 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/activitystreams/test_ordered_collection_builder.py
+-rw-r--r--   0        0        0      809 2023-04-20 10:27:12.601485 bovine-0.1.2/bovine/activitystreams/test_ordered_collection_page.py
+-rw-r--r--   0        0        0     2354 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/activitystreams/utils/__init__.py
+-rw-r--r--   0        0        0     2836 2023-04-20 10:27:49.889806 bovine-0.1.2/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      908 2023-04-20 10:27:49.893806 bovine-0.1.2/bovine/activitystreams/utils/__pycache__/print.cpython-310.pyc
+-rw-r--r--   0        0        0     4763 2023-04-20 10:27:50.093808 bovine-0.1.2/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0      787 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/activitystreams/utils/print.py
+-rw-r--r--   0        0        0     2266 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/activitystreams/utils/test_utils.py
+-rw-r--r--   0        0        0     2081 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/__init__.py
+-rw-r--r--   0        0        0     2209 2023-04-20 10:27:49.605804 bovine-0.1.2/bovine/clients/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      268 2023-04-20 10:27:49.605804 bovine-0.1.2/bovine/clients/__pycache__/consts.cpython-310.pyc
+-rw-r--r--   0        0        0     1472 2023-04-20 10:27:49.781805 bovine-0.1.2/bovine/clients/__pycache__/event_source.cpython-310.pyc
+-rw-r--r--   0        0        0     1014 2023-04-20 10:27:49.605804 bovine-0.1.2/bovine/clients/__pycache__/lookup_account.cpython-310.pyc
+-rw-r--r--   0        0        0     2508 2023-04-20 10:27:49.605804 bovine-0.1.2/bovine/clients/__pycache__/moo_auth_client.cpython-310.pyc
+-rw-r--r--   0        0        0     1237 2023-04-20 10:27:49.605804 bovine-0.1.2/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc
+-rw-r--r--   0        0        0     2471 2023-04-20 10:27:49.781805 bovine-0.1.2/bovine/clients/__pycache__/signed_http.cpython-310.pyc
+-rw-r--r--   0        0        0     1471 2023-04-20 10:27:49.781805 bovine-0.1.2/bovine/clients/__pycache__/signed_http_client.cpython-310.pyc
+-rw-r--r--   0        0        0     1352 2023-04-20 10:27:50.101808 bovine-0.1.2/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1576 2023-04-20 10:27:50.101808 bovine-0.1.2/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1217 2023-04-20 10:27:50.105808 bovine-0.1.2/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2094 2023-04-20 10:27:50.109808 bovine-0.1.2/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0      821 2023-04-20 10:27:50.109808 bovine-0.1.2/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0       91 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/consts.py
+-rw-r--r--   0        0        0     1106 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/event_source.py
+-rw-r--r--   0        0        0      787 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/lookup_account.py
+-rw-r--r--   0        0        0     3176 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/moo_auth_client.py
+-rw-r--r--   0        0        0      948 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/nodeinfo.py
+-rw-r--r--   0        0        0     3278 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/signed_http.py
+-rw-r--r--   0        0        0     1074 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/signed_http_client.py
+-rw-r--r--   0        0        0      609 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/test_event_source.py
+-rw-r--r--   0        0        0      624 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/test_lookup_account.py
+-rw-r--r--   0        0        0      319 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/test_nodeinfo.py
+-rw-r--r--   0        0        0     1145 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/test_signed_http.py
+-rw-r--r--   0        0        0      529 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/clients/test_signed_http_client.py
+-rw-r--r--   0        0        0     3999 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/crypto/__init__.py
+-rw-r--r--   0        0        0     3634 2023-04-20 10:27:49.609804 bovine-0.1.2/bovine/crypto/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2863 2023-04-20 10:27:49.741805 bovine-0.1.2/bovine/crypto/__pycache__/helper.cpython-310.pyc
+-rw-r--r--   0        0        0     2909 2023-04-20 10:27:49.741805 bovine-0.1.2/bovine/crypto/__pycache__/http_signature.cpython-310.pyc
+-rw-r--r--   0        0        0     2257 2023-04-20 10:27:49.741805 bovine-0.1.2/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc
+-rw-r--r--   0        0        0     1784 2023-04-20 10:27:49.781805 bovine-0.1.2/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc
+-rw-r--r--   0        0        0     2363 2023-04-20 10:27:50.053808 bovine-0.1.2/bovine/crypto/__pycache__/test.cpython-310.pyc
+-rw-r--r--   0        0        0     5810 2023-04-20 10:27:50.125808 bovine-0.1.2/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2742 2023-04-20 10:27:50.133808 bovine-0.1.2/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     7454 2023-04-20 10:27:50.145808 bovine-0.1.2/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2674 2023-04-20 10:27:50.153808 bovine-0.1.2/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     2664 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/crypto/helper.py
+-rw-r--r--   0        0        0     2112 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/crypto/http_signature.py
+-rw-r--r--   0        0        0     2942 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/crypto/signature_checker.py
+-rw-r--r--   0        0        0     1266 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/crypto/signature_parser.py
+-rw-r--r--   0        0        0     2199 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/crypto/test.py
+-rw-r--r--   0        0        0     4989 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/crypto/test_crypto.py
+-rw-r--r--   0        0        0      896 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/crypto/test_helper.py
+-rw-r--r--   0        0        0     5081 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/crypto/test_http_signature.py
+-rw-r--r--   0        0        0     1207 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/crypto/test_signature_parser.py
+-rw-r--r--   0        0        0      302 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/ed25519_key.py
+-rw-r--r--   0        0        0      864 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/msg.py
+-rw-r--r--   0        0        0      178 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/test_bovine_client.py
+-rw-r--r--   0        0        0      282 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/test_types.py
+-rw-r--r--   0        0        0     2397 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/types.py
+-rw-r--r--   0        0        0      667 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/utils/__init__.py
+-rw-r--r--   0        0        0      848 2023-04-20 10:27:49.605804 bovine-0.1.2/bovine/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      877 2023-04-20 10:27:49.741805 bovine-0.1.2/bovine/utils/__pycache__/date.cpython-310.pyc
+-rw-r--r--   0        0        0     3443 2023-04-20 10:27:50.161809 bovine-0.1.2/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0     1662 2023-04-20 10:27:50.165809 bovine-0.1.2/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0      973 2023-04-20 10:27:50.165809 bovine-0.1.2/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0      519 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/utils/date.py
+-rw-r--r--   0        0        0     1159 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/utils/msg/__init__.py
+-rw-r--r--   0        0        0     1722 2023-04-20 10:27:50.169809 bovine-0.1.2/bovine/utils/msg/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1922 2023-04-20 10:27:50.173809 bovine-0.1.2/bovine/utils/msg/__pycache__/test_validation.cpython-310-pytest-7.3.0.pyc
+-rw-r--r--   0        0        0      622 2023-04-20 10:27:50.169809 bovine-0.1.2/bovine/utils/msg/__pycache__/validation.cpython-310.pyc
+-rw-r--r--   0        0        0      557 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/utils/msg/test_validation.py
+-rw-r--r--   0        0        0      243 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/utils/msg/validation.py
+-rw-r--r--   0        0        0      181 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/utils/test.py
+-rw-r--r--   0        0        0      737 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/utils/test_date.py
+-rw-r--r--   0        0        0      452 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/utils/test_parse.py
+-rw-r--r--   0        0        0      191 2023-04-20 10:27:12.605485 bovine-0.1.2/bovine/utils/test_webfinger.py
+-rw-r--r--   0        0        0     1211 2023-04-20 10:27:12.605485 bovine-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2260 1970-01-01 00:00:00.000000 bovine-0.1.2/PKG-INFO
```

### Comparing `bovine-0.1.1/bovine/__init__.py` & `bovine-0.1.2/bovine/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/activitypub/__pycache__/authorization_wrapper.cpython-310.pyc` & `bovine-0.1.2/bovine/activitypub/__pycache__/authorization_wrapper.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 2736 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 b00a 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 b00a 0000  o.........Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6403 6c04  ..d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0a 6d0b 5a0b 0100 6500 a00c 650d  d.l.m.Z...e...e.
```

### Comparing `bovine-0.1.1/bovine/activitypub/__pycache__/collection_helper.cpython-310.pyc` & `bovine-0.1.2/bovine/activitypub/__pycache__/collection_helper.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 2219 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 ab08 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 ab08 0000  o.........Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 6c03 6d04 5a04 0100 6405  ..d.d.l.m.Z...d.
 00000050: 6406 8400 5a05 4700 6407 6408 8400 6408  d...Z.G.d.d...d.
 00000060: 8302 5a06 6401 5300 2909 e900 0000 004e  ..Z.d.S.)......N
 00000070: 2901 da0e 7072 696e 745f 6163 7469 7669  )...print_activi
```

### Comparing `bovine-0.1.1/bovine/activitypub/__pycache__/collection_iterator.cpython-310.pyc` & `bovine-0.1.2/bovine/activitypub/__pycache__/collection_iterator.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 429 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 ad01 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 ad01 0000  o.........Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1200 0000 4700  .....@...s....G.
 00000030: 6400 6401 8400 6401 8302 5a00 6402 5300  d.d...d...Z.d.S.
 00000040: 2903 6300 0000 0000 0000 0000 0000 0000  ).c.............
 00000050: 0000 0002 0000 0040 0000 0073 2400 0000  .......@...s$...
 00000060: 6500 5a01 6400 5a02 6401 6402 8400 5a03  e.Z.d.Z.d.d...Z.
 00000070: 6403 6404 8400 5a04 6405 6406 8400 5a05  d.d...Z.d.d...Z.
```

### Comparing `bovine-0.1.1/bovine/activitypub/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.2/bovine/activitypub/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 2757 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 c50a 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 c50a 0000  o.........Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 6d09 5a09 0100  d.d.l.m.Z.m.Z...
 00000060: 6400 6401 6c0a 5a0a 6400 6403 6c0b 6d0c  d.d.l.Z.d.d.l.m.
 00000070: 5a0c 0100 6400 6404 6c0d 6d0e 5a0e 6d0f  Z...d.d.l.m.Z.m.
```

### Comparing `bovine-0.1.1/bovine/activitypub/authorization_wrapper.py` & `bovine-0.1.2/bovine/activitypub/authorization_wrapper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/activitypub/collection_helper.py` & `bovine-0.1.2/bovine/activitypub/collection_helper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/activitypub/test_actor.py` & `bovine-0.1.2/bovine/activitypub/test_actor.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/activitystreams/__init__.py` & `bovine-0.1.2/bovine/activitystreams/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     public_key: Optional[str] = None
     public_key_name: Optional[str] = None
     event_source: Optional[str] = None
     proxy_url: Optional[str] = None
 
     summary: Optional[str] = None
     icon: Optional[dict] = None
+    url: Optional[str] = None
 
     def build(self, visibility=Visibility.PUBLIC):
         """Creates the json-ld representation of the actor."""
         result = {
             "@context": self._build_context(),
             "id": self.id,
             "type": self.type,
@@ -54,14 +55,15 @@
             result["name"] = self.name
         elif self.preferred_username:
             result["name"] = self.preferred_username
 
         for key, value in {
             "summary": self.summary,
             "icon": self.icon,
+            "url": self.url,
         }.items():
             if value is not None:
                 result[key] = value
 
         return result
 
     def _build_context(self):
```

### Comparing `bovine-0.1.1/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc` & `bovine-0.1.2/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 4623 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 0f12 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 4a12 0000  o.........AdJ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6404 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6404 6406 6c09 6d0a 5a0a 0100 6407  ..d.d.l.m.Z...d.
 00000070: 650b 6408 6504 6508 650a 6602 1900 6604  e.d.e.e.e.f...f.
@@ -32,233 +32,236 @@
 000001f0: 7669 6e65 2f62 6f76 696e 652f 626f 7669  vine/bovine/bovi
 00000200: 6e65 2f62 6f76 696e 652f 6163 7469 7669  ne/bovine/activi
 00000210: 7479 7374 7265 616d 732f 5f5f 696e 6974  tystreams/__init
 00000220: 5f5f 2e70 79da 1a66 6163 746f 7269 6573  __.py..factories
 00000230: 5f66 6f72 5f61 6374 6f72 5f6f 626a 6563  _for_actor_objec
 00000240: 740a 0000 0073 0200 0000 1204 720d 0000  t....s......r...
 00000250: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000260: 0000 0300 0000 4000 0000 7314 0100 0065  ......@...s....e
+00000260: 0000 0300 0000 4000 0000 7324 0100 0065  ......@...s$...e
 00000270: 005a 0164 005a 0255 0064 015a 0365 0465  .Z.d.Z.U.d.Z.e.e
 00000280: 0564 023c 0064 035a 0665 0465 0564 043c  .d.<.d.Z.e.e.d.<
 00000290: 0064 055a 0765 0865 0419 0065 0564 063c  .d.Z.e.e...e.d.<
 000002a0: 0064 055a 0965 0865 0419 0065 0564 073c  .d.Z.e.e...e.d.<
 000002b0: 0064 055a 0a65 0865 0419 0065 0564 083c  .d.Z.e.e...e.d.<
 000002c0: 0064 055a 0b65 0865 0419 0065 0564 093c  .d.Z.e.e...e.d.<
 000002d0: 0064 055a 0c65 0865 0419 0065 0564 0a3c  .d.Z.e.e...e.d.<
 000002e0: 0064 055a 0d65 0865 0419 0065 0564 0b3c  .d.Z.e.e...e.d.<
 000002f0: 0064 055a 0e65 0865 0419 0065 0564 0c3c  .d.Z.e.e...e.d.<
 00000300: 0064 055a 0f65 0865 0419 0065 0564 0d3c  .d.Z.e.e...e.d.<
 00000310: 0064 055a 1065 0865 0419 0065 0564 0e3c  .d.Z.e.e...e.d.<
 00000320: 0064 055a 1165 0865 0419 0065 0564 0f3c  .d.Z.e.e...e.d.<
 00000330: 0064 055a 1265 0865 0419 0065 0564 103c  .d.Z.e.e...e.d.<
 00000340: 0064 055a 1365 0865 1419 0065 0564 113c  .d.Z.e.e...e.d.<
-00000350: 0065 156a 1666 0164 1264 1384 015a 1764  .e.j.f.d.d...Z.d
-00000360: 1464 1584 005a 1864 1664 1784 005a 1964  .d...Z.d.d...Z.d
-00000370: 1864 1984 005a 1a64 1a64 1b84 005a 1b64  .d...Z.d.d...Z.d
-00000380: 0553 0029 1cda 0541 6374 6f72 7a37 4163  .S.)...Actorz7Ac
-00000390: 746f 7220 636c 6173 7320 7265 7072 6573  tor class repres
-000003a0: 656e 7473 2074 6865 2062 6173 6963 2041  ents the basic A
-000003b0: 6374 6976 6974 7953 7472 6561 6d73 2061  ctivityStreams a
-000003c0: 6374 6f72 2eda 0269 645a 0650 6572 736f  ctor...idZ.Perso
-000003d0: 6eda 0474 7970 654e da04 6e61 6d65 da12  n..typeN..name..
-000003e0: 7072 6566 6572 7265 645f 7573 6572 6e61  preferred_userna
-000003f0: 6d65 da05 696e 626f 78da 066f 7574 626f  me..inbox..outbo
-00000400: 78da 0966 6f6c 6c6f 7765 7273 da09 666f  x..followers..fo
-00000410: 6c6c 6f77 696e 67da 0a70 7562 6c69 635f  llowing..public_
-00000420: 6b65 79da 0f70 7562 6c69 635f 6b65 795f  key..public_key_
-00000430: 6e61 6d65 da0c 6576 656e 745f 736f 7572  name..event_sour
-00000440: 6365 da09 7072 6f78 795f 7572 6cda 0773  ce..proxy_url..s
-00000450: 756d 6d61 7279 da04 6963 6f6e 6302 0000  ummary..iconc...
-00000460: 0000 0000 0000 0000 0005 0000 0004 0000  ................
-00000470: 0043 0000 0073 9800 0000 7c00 a000 a100  .C...s....|.....
-00000480: 7c00 6a01 7c00 6a02 6401 9c03 7c00 a003  |.j.|.j.d...|...
-00000490: a100 a501 7c00 6a04 7c01 6402 8d01 a501  ....|.j.|.d.....
-000004a0: 7d02 7c00 6a05 721c 7c00 6a05 7c02 6403  }.|.j.r.|.j.|.d.
-000004b0: 3c00 7c01 7406 6a07 6b02 7223 7c02 5300  <.|.t.j.k.r#|.S.
-000004c0: 7c00 6a08 722c 7c00 6a08 7c02 6404 3c00  |.j.r,|.j.|.d.<.
-000004d0: 6e08 7c00 6a05 7234 7c00 6a05 7c02 6404  n.|.j.r4|.j.|.d.
-000004e0: 3c00 7c00 6a09 7c00 6a0a 6405 9c02 a00b  <.|.j.|.j.d.....
-000004f0: a100 4400 5d0c 5c02 7d03 7d04 7c04 6406  ..D.].\.}.}.|.d.
-00000500: 7501 7249 7c04 7c02 7c03 3c00 713d 7c02  u.rI|.|.|.<.q=|.
-00000510: 5300 2907 7a30 4372 6561 7465 7320 7468  S.).z0Creates th
-00000520: 6520 6a73 6f6e 2d6c 6420 7265 7072 6573  e json-ld repres
-00000530: 656e 7461 7469 6f6e 206f 6620 7468 6520  entation of the 
-00000540: 6163 746f 722e 2903 fa08 4063 6f6e 7465  actor.)...@conte
-00000550: 7874 720f 0000 0072 1000 0000 2901 da0a  xtr....r....)...
-00000560: 7669 7369 6269 6c69 7479 5a11 7072 6566  visibilityZ.pref
-00000570: 6572 7265 6455 7365 726e 616d 6572 1100  erredUsernamer..
-00000580: 0000 2902 721b 0000 0072 1c00 0000 4e29  ..).r....r....N)
-00000590: 0cda 0e5f 6275 696c 645f 636f 6e74 6578  ..._build_contex
-000005a0: 7472 0f00 0000 7210 0000 00da 115f 6275  tr....r......_bu
-000005b0: 696c 645f 7075 626c 6963 5f6b 6579 da10  ild_public_key..
-000005c0: 5f62 7569 6c64 5f65 6e64 706f 696e 7473  _build_endpoints
-000005d0: 7212 0000 0072 0500 0000 da03 5745 4272  r....r......WEBr
-000005e0: 1100 0000 721b 0000 0072 1c00 0000 da05  ....r....r......
-000005f0: 6974 656d 7329 05da 0473 656c 6672 1e00  items)...selfr..
-00000600: 0000 da06 7265 7375 6c74 da03 6b65 79da  ....result..key.
-00000610: 0576 616c 7565 720b 0000 0072 0b00 0000  .valuer....r....
-00000620: 720c 0000 00da 0562 7569 6c64 2500 0000  r......build%...
-00000630: 7332 0000 0006 0304 0104 0104 fd06 0402  s2..............
-00000640: fc0a 0504 fb06 080a 010a 0204 0106 020c  ................
-00000650: 0106 010a 0104 0304 0104 fe04 030a fd08  ................
-00000660: 0408 0102 8004 027a 0b41 6374 6f72 2e62  .......z.Actor.b
-00000670: 7569 6c64 6301 0000 0000 0000 0000 0000  uildc...........
-00000680: 0001 0000 0002 0000 0043 0000 0073 1200  .........C...s..
-00000690: 0000 7c00 6a00 7207 6401 6402 6702 5300  ..|.j.r.d.d.g.S.
-000006a0: 6401 5300 2903 4efa 2568 7474 7073 3a2f  d.S.).N.%https:/
-000006b0: 2f77 7777 2e77 332e 6f72 672f 6e73 2f61  /www.w3.org/ns/a
-000006c0: 6374 6976 6974 7973 7472 6561 6d73 7a1c  ctivitystreamsz.
-000006d0: 6874 7470 733a 2f2f 7733 6964 2e6f 7267  https://w3id.org
-000006e0: 2f73 6563 7572 6974 792f 7631 2901 7217  /security/v1).r.
-000006f0: 0000 00a9 0172 2400 0000 720b 0000 0072  .....r$...r....r
-00000700: 0b00 0000 720c 0000 0072 1f00 0000 4300  ....r....r....C.
-00000710: 0000 730a 0000 0006 0102 0202 0104 fe04  ..s.............
-00000720: 057a 1441 6374 6f72 2e5f 6275 696c 645f  .z.Actor._build_
-00000730: 636f 6e74 6578 7463 0100 0000 0000 0000  contextc........
-00000740: 0000 0000 0100 0000 0500 0000 4300 0000  ............C...
-00000750: 732c 0000 007c 006a 0072 1464 017c 006a  s,...|.j.r.d.|.j
-00000760: 019b 0064 027c 006a 029b 009d 037c 006a  ...d.|.j.....|.j
-00000770: 017c 006a 0064 039c 0369 0153 0069 0053  .|.j.d...i.S.i.S
-00000780: 0029 044e 5a09 7075 626c 6963 4b65 79fa  .).NZ.publicKey.
-00000790: 0123 2903 720f 0000 00da 056f 776e 6572  .#).r......owner
-000007a0: 5a0c 7075 626c 6963 4b65 7950 656d 2903  Z.publicKeyPem).
-000007b0: 7217 0000 0072 0f00 0000 7218 0000 0072  r....r....r....r
-000007c0: 2a00 0000 720b 0000 0072 0b00 0000 720c  *...r....r....r.
-000007d0: 0000 0072 2000 0000 4c00 0000 7310 0000  ...r ...L...s...
-000007e0: 0006 0102 0210 0104 0104 0104 fd04 ff04  ................
-000007f0: 077a 1741 6374 6f72 2e5f 6275 696c 645f  .z.Actor._build_
-00000800: 7075 626c 6963 5f6b 6579 6302 0000 0000  public_keyc.....
-00000810: 0000 0000 0000 0004 0000 0003 0000 0043  ...............C
-00000820: 0000 0073 9000 0000 6900 7d02 7c01 7400  ...s....i.}.|.t.
-00000830: 6a01 6b02 7209 7c02 5300 7c00 6a02 7212  j.k.r.|.S.|.j.r.
-00000840: 7c00 6a02 7c02 6401 3c00 6e05 7c00 6a03  |.j.|.d.<.n.|.j.
-00000850: 7c02 6401 3c00 7c00 6a04 7220 7c00 6a04  |.d.<.|.j.r |.j.
-00000860: 7c02 6402 3c00 6e05 7c00 6a03 7c02 6402  |.d.<.n.|.j.|.d.
-00000870: 3c00 7c01 7400 6a05 6b03 722c 7c02 5300  <.|.t.j.k.r,|.S.
-00000880: 7c00 a006 a100 7d03 7c03 7236 7c03 7c02  |.....}.|.r6|.|.
-00000890: 6403 3c00 7c00 6a07 723e 7c00 6a07 7c02  d.<.|.j.r>|.j.|.
-000008a0: 6404 3c00 7c00 6a08 7246 7c00 6a08 7c02  d.<.|.j.rF|.j.|.
-000008b0: 6405 3c00 7c02 5300 2906 4e72 1300 0000  d.<.|.S.).Nr....
-000008c0: 7214 0000 00da 0965 6e64 706f 696e 7473  r......endpoints
-000008d0: 7215 0000 0072 1600 0000 2909 7205 0000  r....r....).r...
-000008e0: 0072 2200 0000 7213 0000 0072 0f00 0000  .r"...r....r....
-000008f0: 7214 0000 00da 054f 574e 4552 da15 5f62  r......OWNER.._b
-00000900: 7569 6c64 5f75 7365 725f 656e 6470 6f69  uild_user_endpoi
-00000910: 6e74 7372 1500 0000 7216 0000 0029 0472  ntsr....r....).r
-00000920: 2400 0000 721e 0000 0072 2500 0000 722d  $...r....r%...r-
-00000930: 0000 0072 0b00 0000 720b 0000 0072 0c00  ...r....r....r..
-00000940: 0000 7221 0000 0057 0000 0073 2600 0000  ..r!...W...s&...
-00000950: 0401 0a02 0401 0602 0c01 0a02 0602 0c01  ................
-00000960: 0a02 0a02 0401 0802 0401 0801 0602 0a01  ................
-00000970: 0601 0a01 0402 7a16 4163 746f 722e 5f62  ......z.Actor._b
-00000980: 7569 6c64 5f65 6e64 706f 696e 7473 6301  uild_endpointsc.
-00000990: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-000009a0: 0000 0043 0000 0073 2800 0000 6900 7d01  ...C...s(...i.}.
-000009b0: 7c00 6a00 720a 7c00 6a00 7c01 6401 3c00  |.j.r.|.j.|.d.<.
-000009c0: 7c00 6a01 7212 7c00 6a01 7c01 6402 3c00  |.j.r.|.j.|.d.<.
-000009d0: 7c01 5300 2903 4eda 0b65 7665 6e74 536f  |.S.).N..eventSo
-000009e0: 7572 6365 da08 7072 6f78 7955 726c 2902  urce..proxyUrl).
-000009f0: 7219 0000 0072 1a00 0000 2902 7224 0000  r....r....).r$..
-00000a00: 0072 2d00 0000 720b 0000 0072 0b00 0000  .r-...r....r....
-00000a10: 720c 0000 0072 2f00 0000 7500 0000 730c  r....r/...u...s.
-00000a20: 0000 0004 0106 010a 0106 010a 0104 017a  ...............z
-00000a30: 1b41 6374 6f72 2e5f 6275 696c 645f 7573  .Actor._build_us
-00000a40: 6572 5f65 6e64 706f 696e 7473 291c da08  er_endpoints)...
-00000a50: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00000a60: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00000a70: 5f5f da07 5f5f 646f 635f 5fda 0373 7472  __..__doc__..str
-00000a80: da0f 5f5f 616e 6e6f 7461 7469 6f6e 735f  ..__annotations_
-00000a90: 5f72 1000 0000 7211 0000 0072 0300 0000  _r....r....r....
-00000aa0: 7212 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
-00000ab0: 1500 0000 7216 0000 0072 1700 0000 7218  ....r....r....r.
-00000ac0: 0000 0072 1900 0000 721a 0000 0072 1b00  ...r....r....r..
-00000ad0: 0000 721c 0000 00da 0464 6963 7472 0500  ..r......dictr..
-00000ae0: 0000 da06 5055 424c 4943 7228 0000 0072  ....PUBLICr(...r
-00000af0: 1f00 0000 7220 0000 0072 2100 0000 722f  ....r ...r!...r/
-00000b00: 0000 0072 0b00 0000 720b 0000 0072 0b00  ...r....r....r..
-00000b10: 0000 720c 0000 0072 0e00 0000 1100 0000  ..r....r........
-00000b20: 732a 0000 000a 0004 0208 020c 0110 0110  s*..............
-00000b30: 0110 0110 0110 0110 0110 0110 0110 0110  ................
-00000b40: 0110 0210 010e 0208 1e08 0908 0b0c 1e72  ...............r
-00000b50: 0e00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-00000b60: 0000 0000 0003 0000 0040 0000 0073 6000  .........@...s`.
-00000b70: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
-00000b80: 6401 3c00 6402 5a05 6506 6402 4200 6504  d.<.d.Z.e.d.B.e.
-00000b90: 6403 3c00 6404 5a07 6508 6504 6405 3c00  d.<.d.Z.e.e.d.<.
-00000ba0: 6402 5a09 6503 6402 4200 6504 6406 3c00  d.Z.e.d.B.e.d.<.
-00000bb0: 6402 5a0a 6503 6402 4200 6504 6407 3c00  d.Z.e.d.B.e.d.<.
-00000bc0: 6408 650b 6602 6409 640a 8404 5a0c 6402  d.e.f.d.d...Z.d.
-00000bd0: 5300 290b da11 4f72 6465 7265 6443 6f6c  S.)...OrderedCol
-00000be0: 6c65 6374 696f 6e72 0f00 0000 4e72 2300  lectionr....Nr#.
-00000bf0: 0000 7201 0000 00da 0563 6f75 6e74 da05  ..r......count..
-00000c00: 6669 7273 74da 046c 6173 7472 0a00 0000  first..lastr....
-00000c10: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000c20: 0005 0000 0043 0000 0073 4600 0000 6401  .....C...sF...d.
-00000c30: 7c00 6a00 7c00 6a01 6402 6403 9c04 7d01  |.j.|.j.d.d...}.
-00000c40: 7c00 6a02 7211 7c00 6a02 7c01 6404 3c00  |.j.r.|.j.|.d.<.
-00000c50: 7c00 6a03 7219 7c00 6a03 7c01 6405 3c00  |.j.r.|.j.|.d.<.
-00000c60: 7c00 6a04 7221 7c00 6a04 7c01 6406 3c00  |.j.r!|.j.|.d.<.
-00000c70: 7c01 5300 2907 4e72 2900 0000 723a 0000  |.S.).Nr)...r:..
-00000c80: 0029 0472 1d00 0000 720f 0000 00da 0a74  .).r....r......t
-00000c90: 6f74 616c 4974 656d 7372 1000 0000 da0c  otalItemsr......
-00000ca0: 6f72 6465 7265 6449 7465 6d73 723c 0000  orderedItemsr<..
-00000cb0: 0072 3d00 0000 2905 720f 0000 0072 3b00  .r=...).r....r;.
-00000cc0: 0000 7223 0000 0072 3c00 0000 723d 0000  ..r#...r<...r=..
-00000cd0: 00a9 0272 2400 0000 7225 0000 0072 0b00  ...r$...r%...r..
-00000ce0: 0000 720b 0000 0072 0c00 0000 7228 0000  ..r....r....r(..
-00000cf0: 0086 0000 0073 1800 0000 0202 0401 0401  .....s..........
-00000d00: 0201 06fc 0607 0a01 0602 0a01 0602 0a01  ................
-00000d10: 0402 7a17 4f72 6465 7265 6443 6f6c 6c65  ..z.OrderedColle
-00000d20: 6374 696f 6e2e 6275 696c 6429 0d72 3200  ction.build).r2.
-00000d30: 0000 7233 0000 0072 3400 0000 7236 0000  ..r3...r4...r6..
-00000d40: 0072 3700 0000 7223 0000 00da 046c 6973  .r7...r#.....lis
-00000d50: 7472 3b00 0000 da03 696e 7472 3c00 0000  tr;.....intr<...
-00000d60: 723d 0000 0072 3800 0000 7228 0000 0072  r=...r8...r(...r
-00000d70: 0b00 0000 720b 0000 0072 0b00 0000 720c  ....r....r....r.
-00000d80: 0000 0072 3a00 0000 7e00 0000 730e 0000  ...r:...~...s...
-00000d90: 000a 0008 0210 010c 0110 0110 0112 0272  ...............r
-00000da0: 3a00 0000 6300 0000 0000 0000 0000 0000  :...c...........
-00000db0: 0000 0000 0003 0000 0040 0000 0073 5400  .........@...sT.
-00000dc0: 0000 6500 5a01 6400 5a02 5500 6503 6504  ..e.Z.d.Z.U.e.e.
-00000dd0: 6401 3c00 6505 6504 6402 3c00 6503 6504  d.<.e.e.d.<.e.e.
-00000de0: 6403 3c00 6404 5a06 6503 6404 4200 6504  d.<.d.Z.e.d.B.e.
-00000df0: 6405 3c00 6404 5a07 6503 6404 4200 6504  d.<.d.Z.e.d.B.e.
-00000e00: 6406 3c00 6407 6508 6602 6408 6409 8404  d.<.d.e.f.d.d...
-00000e10: 5a09 6404 5300 290a da15 4f72 6465 7265  Z.d.S.)...Ordere
-00000e20: 6443 6f6c 6c65 6374 696f 6e50 6167 6572  dCollectionPager
-00000e30: 0f00 0000 7223 0000 00da 0770 6172 745f  ....r#.....part_
-00000e40: 6f66 4eda 046e 6578 74da 0470 7265 7672  ofN..next..prevr
-00000e50: 0a00 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00000e60: 0002 0000 0006 0000 0043 0000 0073 3a00  .........C...s:.
-00000e70: 0000 6401 7c00 6a00 7c00 6a01 7c00 6a02  ..d.|.j.|.j.|.j.
-00000e80: 6402 6403 9c05 7d01 7c00 6a03 7213 7c00  d.d...}.|.j.r.|.
-00000e90: 6a03 7c01 6404 3c00 7c00 6a04 721b 7c00  j.|.d.<.|.j.r.|.
-00000ea0: 6a04 7c01 6405 3c00 7c01 5300 2906 4e72  j.|.d.<.|.S.).Nr
-00000eb0: 2900 0000 7243 0000 0029 0572 1d00 0000  )...rC...).r....
-00000ec0: 720f 0000 005a 0670 6172 744f 6672 3f00  r....Z.partOfr?.
-00000ed0: 0000 7210 0000 0072 4500 0000 7246 0000  ..r....rE...rF..
-00000ee0: 0029 0572 0f00 0000 7244 0000 0072 2300  .).r....rD...r#.
-00000ef0: 0000 7245 0000 0072 4600 0000 7240 0000  ..rE...rF...r@..
-00000f00: 0072 0b00 0000 720b 0000 0072 0c00 0000  .r....r....r....
-00000f10: 7228 0000 00a2 0000 0073 1600 0000 0202  r(.......s......
-00000f20: 0401 0401 0401 0201 06fb 0608 0a01 0602  ................
-00000f30: 0a01 0402 7a1b 4f72 6465 7265 6443 6f6c  ....z.OrderedCol
-00000f40: 6c65 6374 696f 6e50 6167 652e 6275 696c  lectionPage.buil
-00000f50: 6429 0a72 3200 0000 7233 0000 0072 3400  d).r2...r3...r4.
-00000f60: 0000 7236 0000 0072 3700 0000 7241 0000  ..r6...r7...rA..
-00000f70: 0072 4500 0000 7246 0000 0072 3800 0000  .rE...rF...r8...
-00000f80: 7228 0000 0072 0b00 0000 720b 0000 0072  r(...r....r....r
-00000f90: 0b00 0000 720c 0000 0072 4300 0000 9a00  ....r....rC.....
-00000fa0: 0000 730e 0000 000a 0008 0208 0108 0110  ..s.............
-00000fb0: 0110 0112 0272 4300 0000 4e29 10da 0b64  .....rC...N)...d
-00000fc0: 6174 6163 6c61 7373 6573 7202 0000 00da  ataclassesr.....
-00000fd0: 0674 7970 696e 6772 0300 0000 7204 0000  .typingr....r...
-00000fe0: 00da 0c62 6f76 696e 652e 7479 7065 7372  ...bovine.typesr
-00000ff0: 0500 0000 da10 6163 7469 7669 7479 5f66  ......activity_f
-00001000: 6163 746f 7279 7207 0000 00da 0e6f 626a  actoryr......obj
-00001010: 6563 745f 6661 6374 6f72 7972 0800 0000  ect_factoryr....
-00001020: 7238 0000 0072 0d00 0000 720e 0000 0072  r8...r....r....r
-00001030: 3a00 0000 7243 0000 0072 0b00 0000 720b  :...rC...r....r.
-00001040: 0000 0072 0b00 0000 720c 0000 00da 083c  ...r....r......<
-00001050: 6d6f 6475 6c65 3e01 0000 0073 2000 0000  module>....s ...
-00001060: 0c00 1001 0c02 0c02 0c01 0203 0201 02ff  ................
-00001070: 0a02 0afe 0207 1001 026c 1001 021b 1401  .........l......
+00000350: 0064 055a 1565 0865 0419 0065 0564 123c  .d.Z.e.e...e.d.<
+00000360: 0065 166a 1766 0164 1364 1484 015a 1864  .e.j.f.d.d...Z.d
+00000370: 1564 1684 005a 1964 1764 1884 005a 1a64  .d...Z.d.d...Z.d
+00000380: 1964 1a84 005a 1b64 1b64 1c84 005a 1c64  .d...Z.d.d...Z.d
+00000390: 0553 0029 1dda 0541 6374 6f72 7a37 4163  .S.)...Actorz7Ac
+000003a0: 746f 7220 636c 6173 7320 7265 7072 6573  tor class repres
+000003b0: 656e 7473 2074 6865 2062 6173 6963 2041  ents the basic A
+000003c0: 6374 6976 6974 7953 7472 6561 6d73 2061  ctivityStreams a
+000003d0: 6374 6f72 2eda 0269 645a 0650 6572 736f  ctor...idZ.Perso
+000003e0: 6eda 0474 7970 654e da04 6e61 6d65 da12  n..typeN..name..
+000003f0: 7072 6566 6572 7265 645f 7573 6572 6e61  preferred_userna
+00000400: 6d65 da05 696e 626f 78da 066f 7574 626f  me..inbox..outbo
+00000410: 78da 0966 6f6c 6c6f 7765 7273 da09 666f  x..followers..fo
+00000420: 6c6c 6f77 696e 67da 0a70 7562 6c69 635f  llowing..public_
+00000430: 6b65 79da 0f70 7562 6c69 635f 6b65 795f  key..public_key_
+00000440: 6e61 6d65 da0c 6576 656e 745f 736f 7572  name..event_sour
+00000450: 6365 da09 7072 6f78 795f 7572 6cda 0773  ce..proxy_url..s
+00000460: 756d 6d61 7279 da04 6963 6f6e da03 7572  ummary..icon..ur
+00000470: 6c63 0200 0000 0000 0000 0000 0000 0500  lc..............
+00000480: 0000 0400 0000 4300 0000 739c 0000 007c  ......C...s....|
+00000490: 00a0 00a1 007c 006a 017c 006a 0264 019c  .....|.j.|.j.d..
+000004a0: 037c 00a0 03a1 00a5 017c 006a 047c 0164  .|.......|.j.|.d
+000004b0: 028d 01a5 017d 027c 006a 0572 1c7c 006a  .....}.|.j.r.|.j
+000004c0: 057c 0264 033c 007c 0174 066a 076b 0272  .|.d.<.|.t.j.k.r
+000004d0: 237c 0253 007c 006a 0872 2c7c 006a 087c  #|.S.|.j.r,|.j.|
+000004e0: 0264 043c 006e 087c 006a 0572 347c 006a  .d.<.n.|.j.r4|.j
+000004f0: 057c 0264 043c 007c 006a 097c 006a 0a7c  .|.d.<.|.j.|.j.|
+00000500: 006a 0b64 059c 03a0 0ca1 0044 005d 0c5c  .j.d.......D.].\
+00000510: 027d 037d 047c 0464 0675 0172 4b7c 047c  .}.}.|.d.u.rK|.|
+00000520: 027c 033c 0071 3f7c 0253 0029 077a 3043  .|.<.q?|.S.).z0C
+00000530: 7265 6174 6573 2074 6865 206a 736f 6e2d  reates the json-
+00000540: 6c64 2072 6570 7265 7365 6e74 6174 696f  ld representatio
+00000550: 6e20 6f66 2074 6865 2061 6374 6f72 2e29  n of the actor.)
+00000560: 03fa 0840 636f 6e74 6578 7472 0f00 0000  ...@contextr....
+00000570: 7210 0000 0029 01da 0a76 6973 6962 696c  r....)...visibil
+00000580: 6974 795a 1170 7265 6665 7272 6564 5573  ityZ.preferredUs
+00000590: 6572 6e61 6d65 7211 0000 0029 0372 1b00  ernamer....).r..
+000005a0: 0000 721c 0000 0072 1d00 0000 4e29 0dda  ..r....r....N)..
+000005b0: 0e5f 6275 696c 645f 636f 6e74 6578 7472  ._build_contextr
+000005c0: 0f00 0000 7210 0000 00da 115f 6275 696c  ....r......_buil
+000005d0: 645f 7075 626c 6963 5f6b 6579 da10 5f62  d_public_key.._b
+000005e0: 7569 6c64 5f65 6e64 706f 696e 7473 7212  uild_endpointsr.
+000005f0: 0000 0072 0500 0000 da03 5745 4272 1100  ...r......WEBr..
+00000600: 0000 721b 0000 0072 1c00 0000 721d 0000  ..r....r....r...
+00000610: 00da 0569 7465 6d73 2905 da04 7365 6c66  ...items)...self
+00000620: 721f 0000 00da 0672 6573 756c 74da 036b  r......result..k
+00000630: 6579 da05 7661 6c75 6572 0b00 0000 720b  ey..valuer....r.
+00000640: 0000 0072 0c00 0000 da05 6275 696c 6426  ...r......build&
+00000650: 0000 0073 3400 0000 0603 0401 0401 04fd  ...s4...........
+00000660: 0604 02fc 0a05 04fb 0608 0a01 0a02 0401  ................
+00000670: 0602 0c01 0601 0a01 0403 0401 0401 04fd  ................
+00000680: 0404 0afc 0805 0801 0280 0402 7a0b 4163  ............z.Ac
+00000690: 746f 722e 6275 696c 6463 0100 0000 0000  tor.buildc......
+000006a0: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
+000006b0: 0000 7312 0000 007c 006a 0072 0764 0164  ..s....|.j.r.d.d
+000006c0: 0267 0253 0064 0153 0029 034e fa25 6874  .g.S.d.S.).N.%ht
+000006d0: 7470 733a 2f2f 7777 772e 7733 2e6f 7267  tps://www.w3.org
+000006e0: 2f6e 732f 6163 7469 7669 7479 7374 7265  /ns/activitystre
+000006f0: 616d 737a 1c68 7474 7073 3a2f 2f77 3369  amsz.https://w3i
+00000700: 642e 6f72 672f 7365 6375 7269 7479 2f76  d.org/security/v
+00000710: 3129 0172 1700 0000 a901 7225 0000 0072  1).r......r%...r
+00000720: 0b00 0000 720b 0000 0072 0c00 0000 7220  ....r....r....r 
+00000730: 0000 0045 0000 0073 0a00 0000 0601 0202  ...E...s........
+00000740: 0201 04fe 0405 7a14 4163 746f 722e 5f62  ......z.Actor._b
+00000750: 7569 6c64 5f63 6f6e 7465 7874 6301 0000  uild_contextc...
+00000760: 0000 0000 0000 0000 0001 0000 0005 0000  ................
+00000770: 0043 0000 0073 2c00 0000 7c00 6a00 7214  .C...s,...|.j.r.
+00000780: 6401 7c00 6a01 9b00 6402 7c00 6a02 9b00  d.|.j...d.|.j...
+00000790: 9d03 7c00 6a01 7c00 6a00 6403 9c03 6901  ..|.j.|.j.d...i.
+000007a0: 5300 6900 5300 2904 4e5a 0970 7562 6c69  S.i.S.).NZ.publi
+000007b0: 634b 6579 fa01 2329 0372 0f00 0000 da05  cKey..#).r......
+000007c0: 6f77 6e65 725a 0c70 7562 6c69 634b 6579  ownerZ.publicKey
+000007d0: 5065 6d29 0372 1700 0000 720f 0000 0072  Pem).r....r....r
+000007e0: 1800 0000 722b 0000 0072 0b00 0000 720b  ....r+...r....r.
+000007f0: 0000 0072 0c00 0000 7221 0000 004e 0000  ...r....r!...N..
+00000800: 0073 1000 0000 0601 0202 1001 0401 0401  .s..............
+00000810: 04fd 04ff 0407 7a17 4163 746f 722e 5f62  ......z.Actor._b
+00000820: 7569 6c64 5f70 7562 6c69 635f 6b65 7963  uild_public_keyc
+00000830: 0200 0000 0000 0000 0000 0000 0400 0000  ................
+00000840: 0300 0000 4300 0000 7390 0000 0069 007d  ....C...s....i.}
+00000850: 027c 0174 006a 016b 0272 097c 0253 007c  .|.t.j.k.r.|.S.|
+00000860: 006a 0272 127c 006a 027c 0264 013c 006e  .j.r.|.j.|.d.<.n
+00000870: 057c 006a 037c 0264 013c 007c 006a 0472  .|.j.|.d.<.|.j.r
+00000880: 207c 006a 047c 0264 023c 006e 057c 006a   |.j.|.d.<.n.|.j
+00000890: 037c 0264 023c 007c 0174 006a 056b 0372  .|.d.<.|.t.j.k.r
+000008a0: 2c7c 0253 007c 00a0 06a1 007d 037c 0372  ,|.S.|.....}.|.r
+000008b0: 367c 037c 0264 033c 007c 006a 0772 3e7c  6|.|.d.<.|.j.r>|
+000008c0: 006a 077c 0264 043c 007c 006a 0872 467c  .j.|.d.<.|.j.rF|
+000008d0: 006a 087c 0264 053c 007c 0253 0029 064e  .j.|.d.<.|.S.).N
+000008e0: 7213 0000 0072 1400 0000 da09 656e 6470  r....r......endp
+000008f0: 6f69 6e74 7372 1500 0000 7216 0000 0029  ointsr....r....)
+00000900: 0972 0500 0000 7223 0000 0072 1300 0000  .r....r#...r....
+00000910: 720f 0000 0072 1400 0000 da05 4f57 4e45  r....r......OWNE
+00000920: 52da 155f 6275 696c 645f 7573 6572 5f65  R.._build_user_e
+00000930: 6e64 706f 696e 7473 7215 0000 0072 1600  ndpointsr....r..
+00000940: 0000 2904 7225 0000 0072 1f00 0000 7226  ..).r%...r....r&
+00000950: 0000 0072 2e00 0000 720b 0000 0072 0b00  ...r....r....r..
+00000960: 0000 720c 0000 0072 2200 0000 5900 0000  ..r....r"...Y...
+00000970: 7326 0000 0004 010a 0204 0106 020c 010a  s&..............
+00000980: 0206 020c 010a 020a 0204 0108 0204 0108  ................
+00000990: 0106 020a 0106 010a 0104 027a 1641 6374  ...........z.Act
+000009a0: 6f72 2e5f 6275 696c 645f 656e 6470 6f69  or._build_endpoi
+000009b0: 6e74 7363 0100 0000 0000 0000 0000 0000  ntsc............
+000009c0: 0200 0000 0300 0000 4300 0000 7328 0000  ........C...s(..
+000009d0: 0069 007d 017c 006a 0072 0a7c 006a 007c  .i.}.|.j.r.|.j.|
+000009e0: 0164 013c 007c 006a 0172 127c 006a 017c  .d.<.|.j.r.|.j.|
+000009f0: 0164 023c 007c 0153 0029 034e da0b 6576  .d.<.|.S.).N..ev
+00000a00: 656e 7453 6f75 7263 65da 0870 726f 7879  entSource..proxy
+00000a10: 5572 6c29 0272 1900 0000 721a 0000 0029  Url).r....r....)
+00000a20: 0272 2500 0000 722e 0000 0072 0b00 0000  .r%...r....r....
+00000a30: 720b 0000 0072 0c00 0000 7230 0000 0077  r....r....r0...w
+00000a40: 0000 0073 0c00 0000 0401 0601 0a01 0601  ...s............
+00000a50: 0a01 0401 7a1b 4163 746f 722e 5f62 7569  ....z.Actor._bui
+00000a60: 6c64 5f75 7365 725f 656e 6470 6f69 6e74  ld_user_endpoint
+00000a70: 7329 1dda 085f 5f6e 616d 655f 5fda 0a5f  s)...__name__.._
+00000a80: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000a90: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
+00000aa0: da03 7374 72da 0f5f 5f61 6e6e 6f74 6174  ..str..__annotat
+00000ab0: 696f 6e73 5f5f 7210 0000 0072 1100 0000  ions__r....r....
+00000ac0: 7203 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+00000ad0: 1400 0000 7215 0000 0072 1600 0000 7217  ....r....r....r.
+00000ae0: 0000 0072 1800 0000 7219 0000 0072 1a00  ...r....r....r..
+00000af0: 0000 721b 0000 0072 1c00 0000 da04 6469  ..r....r......di
+00000b00: 6374 721d 0000 0072 0500 0000 da06 5055  ctr....r......PU
+00000b10: 424c 4943 7229 0000 0072 2000 0000 7221  BLICr)...r ...r!
+00000b20: 0000 0072 2200 0000 7230 0000 0072 0b00  ...r"...r0...r..
+00000b30: 0000 720b 0000 0072 0b00 0000 720c 0000  ..r....r....r...
+00000b40: 0072 0e00 0000 1100 0000 732c 0000 000a  .r........s,....
+00000b50: 0004 0208 020c 0110 0110 0110 0110 0110  ................
+00000b60: 0110 0110 0110 0110 0110 0110 0210 0110  ................
+00000b70: 010e 0208 1f08 0908 0b0c 1e72 0e00 0000  ...........r....
+00000b80: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000b90: 0003 0000 0040 0000 0073 6000 0000 6500  .....@...s`...e.
+00000ba0: 5a01 6400 5a02 5500 6503 6504 6401 3c00  Z.d.Z.U.e.e.d.<.
+00000bb0: 6402 5a05 6506 6402 4200 6504 6403 3c00  d.Z.e.d.B.e.d.<.
+00000bc0: 6404 5a07 6508 6504 6405 3c00 6402 5a09  d.Z.e.e.d.<.d.Z.
+00000bd0: 6503 6402 4200 6504 6406 3c00 6402 5a0a  e.d.B.e.d.<.d.Z.
+00000be0: 6503 6402 4200 6504 6407 3c00 6408 650b  e.d.B.e.d.<.d.e.
+00000bf0: 6602 6409 640a 8404 5a0c 6402 5300 290b  f.d.d...Z.d.S.).
+00000c00: da11 4f72 6465 7265 6443 6f6c 6c65 6374  ..OrderedCollect
+00000c10: 696f 6e72 0f00 0000 4e72 2400 0000 7201  ionr....Nr$...r.
+00000c20: 0000 00da 0563 6f75 6e74 da05 6669 7273  .....count..firs
+00000c30: 74da 046c 6173 7472 0a00 0000 6301 0000  t..lastr....c...
+00000c40: 0000 0000 0000 0000 0002 0000 0005 0000  ................
+00000c50: 0043 0000 0073 4600 0000 6401 7c00 6a00  .C...sF...d.|.j.
+00000c60: 7c00 6a01 6402 6403 9c04 7d01 7c00 6a02  |.j.d.d...}.|.j.
+00000c70: 7211 7c00 6a02 7c01 6404 3c00 7c00 6a03  r.|.j.|.d.<.|.j.
+00000c80: 7219 7c00 6a03 7c01 6405 3c00 7c00 6a04  r.|.j.|.d.<.|.j.
+00000c90: 7221 7c00 6a04 7c01 6406 3c00 7c01 5300  r!|.j.|.d.<.|.S.
+00000ca0: 2907 4e72 2a00 0000 723b 0000 0029 0472  ).Nr*...r;...).r
+00000cb0: 1e00 0000 720f 0000 00da 0a74 6f74 616c  ....r......total
+00000cc0: 4974 656d 7372 1000 0000 da0c 6f72 6465  Itemsr......orde
+00000cd0: 7265 6449 7465 6d73 723d 0000 0072 3e00  redItemsr=...r>.
+00000ce0: 0000 2905 720f 0000 0072 3c00 0000 7224  ..).r....r<...r$
+00000cf0: 0000 0072 3d00 0000 723e 0000 00a9 0272  ...r=...r>.....r
+00000d00: 2500 0000 7226 0000 0072 0b00 0000 720b  %...r&...r....r.
+00000d10: 0000 0072 0c00 0000 7229 0000 0088 0000  ...r....r)......
+00000d20: 0073 1800 0000 0202 0401 0401 0201 06fc  .s..............
+00000d30: 0607 0a01 0602 0a01 0602 0a01 0402 7a17  ..............z.
+00000d40: 4f72 6465 7265 6443 6f6c 6c65 6374 696f  OrderedCollectio
+00000d50: 6e2e 6275 696c 6429 0d72 3300 0000 7234  n.build).r3...r4
+00000d60: 0000 0072 3500 0000 7237 0000 0072 3800  ...r5...r7...r8.
+00000d70: 0000 7224 0000 00da 046c 6973 7472 3c00  ..r$.....listr<.
+00000d80: 0000 da03 696e 7472 3d00 0000 723e 0000  ....intr=...r>..
+00000d90: 0072 3900 0000 7229 0000 0072 0b00 0000  .r9...r)...r....
+00000da0: 720b 0000 0072 0b00 0000 720c 0000 0072  r....r....r....r
+00000db0: 3b00 0000 8000 0000 730e 0000 000a 0008  ;.......s.......
+00000dc0: 0210 010c 0110 0110 0112 0272 3b00 0000  ...........r;...
+00000dd0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00000de0: 0003 0000 0040 0000 0073 5400 0000 6500  .....@...sT...e.
+00000df0: 5a01 6400 5a02 5500 6503 6504 6401 3c00  Z.d.Z.U.e.e.d.<.
+00000e00: 6505 6504 6402 3c00 6503 6504 6403 3c00  e.e.d.<.e.e.d.<.
+00000e10: 6404 5a06 6503 6404 4200 6504 6405 3c00  d.Z.e.d.B.e.d.<.
+00000e20: 6404 5a07 6503 6404 4200 6504 6406 3c00  d.Z.e.d.B.e.d.<.
+00000e30: 6407 6508 6602 6408 6409 8404 5a09 6404  d.e.f.d.d...Z.d.
+00000e40: 5300 290a da15 4f72 6465 7265 6443 6f6c  S.)...OrderedCol
+00000e50: 6c65 6374 696f 6e50 6167 6572 0f00 0000  lectionPager....
+00000e60: 7224 0000 00da 0770 6172 745f 6f66 4eda  r$.....part_ofN.
+00000e70: 046e 6578 74da 0470 7265 7672 0a00 0000  .next..prevr....
+00000e80: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000e90: 0006 0000 0043 0000 0073 3a00 0000 6401  .....C...s:...d.
+00000ea0: 7c00 6a00 7c00 6a01 7c00 6a02 6402 6403  |.j.|.j.|.j.d.d.
+00000eb0: 9c05 7d01 7c00 6a03 7213 7c00 6a03 7c01  ..}.|.j.r.|.j.|.
+00000ec0: 6404 3c00 7c00 6a04 721b 7c00 6a04 7c01  d.<.|.j.r.|.j.|.
+00000ed0: 6405 3c00 7c01 5300 2906 4e72 2a00 0000  d.<.|.S.).Nr*...
+00000ee0: 7244 0000 0029 0572 1e00 0000 720f 0000  rD...).r....r...
+00000ef0: 005a 0670 6172 744f 6672 4000 0000 7210  .Z.partOfr@...r.
+00000f00: 0000 0072 4600 0000 7247 0000 0029 0572  ...rF...rG...).r
+00000f10: 0f00 0000 7245 0000 0072 2400 0000 7246  ....rE...r$...rF
+00000f20: 0000 0072 4700 0000 7241 0000 0072 0b00  ...rG...rA...r..
+00000f30: 0000 720b 0000 0072 0c00 0000 7229 0000  ..r....r....r)..
+00000f40: 00a4 0000 0073 1600 0000 0202 0401 0401  .....s..........
+00000f50: 0401 0201 06fb 0608 0a01 0602 0a01 0402  ................
+00000f60: 7a1b 4f72 6465 7265 6443 6f6c 6c65 6374  z.OrderedCollect
+00000f70: 696f 6e50 6167 652e 6275 696c 6429 0a72  ionPage.build).r
+00000f80: 3300 0000 7234 0000 0072 3500 0000 7237  3...r4...r5...r7
+00000f90: 0000 0072 3800 0000 7242 0000 0072 4600  ...r8...rB...rF.
+00000fa0: 0000 7247 0000 0072 3900 0000 7229 0000  ..rG...r9...r)..
+00000fb0: 0072 0b00 0000 720b 0000 0072 0b00 0000  .r....r....r....
+00000fc0: 720c 0000 0072 4400 0000 9c00 0000 730e  r....rD.......s.
+00000fd0: 0000 000a 0008 0208 0108 0110 0110 0112  ................
+00000fe0: 0272 4400 0000 4e29 10da 0b64 6174 6163  .rD...N)...datac
+00000ff0: 6c61 7373 6573 7202 0000 00da 0674 7970  lassesr......typ
+00001000: 696e 6772 0300 0000 7204 0000 00da 0c62  ingr....r......b
+00001010: 6f76 696e 652e 7479 7065 7372 0500 0000  ovine.typesr....
+00001020: da10 6163 7469 7669 7479 5f66 6163 746f  ..activity_facto
+00001030: 7279 7207 0000 00da 0e6f 626a 6563 745f  ryr......object_
+00001040: 6661 6374 6f72 7972 0800 0000 7239 0000  factoryr....r9..
+00001050: 0072 0d00 0000 720e 0000 0072 3b00 0000  .r....r....r;...
+00001060: 7244 0000 0072 0b00 0000 720b 0000 0072  rD...r....r....r
+00001070: 0b00 0000 720c 0000 00da 083c 6d6f 6475  ....r......<modu
+00001080: 6c65 3e01 0000 0073 2000 0000 0c00 1001  le>....s .......
+00001090: 0c02 0c02 0c01 0203 0201 02ff 0a02 0afe  ................
+000010a0: 0207 1001 026e 1001 021b 1401            .....n......
```

### Comparing `bovine-0.1.1/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc` & `bovine-0.1.2/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 4012 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 ac0f 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 6310 0000  o.........Adc...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 6d05 5a05 0100 6501  d.l.m.Z.m.Z...e.
 00000050: 4700 6403 6404 8400 6404 8302 8301 5a06  G.d.d...d.....Z.
 00000060: 4700 6405 6406 8400 6406 8302 5a07 6407  G.d.d...d...Z.d.
 00000070: 5300 2908 e900 0000 0029 02da 0964 6174  S.)......)...dat
@@ -127,130 +127,140 @@
 000007e0: 0072 1a00 0000 721b 0000 0072 2200 0000  .r....r....r"...
 000007f0: 7218 0000 0072 1800 0000 7218 0000 0072  r....r....r....r
 00000800: 1900 0000 7206 0000 0005 0000 0073 2200  ....r........s".
 00000810: 0000 0a00 0402 0803 1001 1001 1001 1001  ................
 00000820: 1601 1601 1002 1001 1001 1002 1001 0802  ................
 00000830: 0807 0c07 7206 0000 0063 0000 0000 0000  ....r....c......
 00000840: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
-00000850: 0000 7350 0000 0065 005a 0164 005a 0264  ..sP...e.Z.d.Z.d
+00000850: 0000 7358 0000 0065 005a 0164 005a 0264  ..sX...e.Z.d.Z.d
 00000860: 015a 0364 0264 0384 005a 0464 0464 0584  .Z.d.d...Z.d.d..
 00000870: 005a 0564 0664 0784 005a 0664 0864 0984  .Z.d.d...Z.d.d..
 00000880: 005a 0764 0a64 0b84 005a 0864 0c64 0d84  .Z.d.d...Z.d.d..
 00000890: 005a 0964 0e64 0f84 005a 0a64 1064 1184  .Z.d.d...Z.d.d..
-000008a0: 005a 0b64 1253 0029 13da 0f41 6374 6976  .Z.d.S.)...Activ
-000008b0: 6974 7946 6163 746f 7279 7a49 4261 7369  ityFactoryzIBasi
-000008c0: 6320 6661 6374 6f72 7920 666f 7220 4163  c factory for Ac
-000008d0: 7469 7669 7479 206f 626a 6563 7473 2e0a  tivity objects..
-000008e0: 0a20 2020 2055 7361 6c6c 7920 6372 6561  .    Usally crea
-000008f0: 7465 6420 6279 2061 2042 6f76 696e 6543  ted by a BovineC
-00000900: 6c69 656e 7463 0200 0000 0000 0000 0000  lientc..........
-00000910: 0000 0200 0000 0200 0000 4300 0000 730a  ..........C...s.
-00000920: 0000 007c 017c 005f 0064 0053 0029 014e  ...|.|._.d.S.).N
-00000930: 2901 da0b 696e 666f 726d 6174 696f 6e29  )...information)
-00000940: 0272 1700 0000 da11 6163 746f 725f 696e  .r......actor_in
-00000950: 666f 726d 6174 696f 6e72 1800 0000 7218  formationr....r.
-00000960: 0000 0072 1900 0000 da08 5f5f 696e 6974  ...r......__init
-00000970: 5f5f 4c00 0000 7302 0000 000a 017a 1841  __L...s......z.A
-00000980: 6374 6976 6974 7946 6163 746f 7279 2e5f  ctivityFactory._
-00000990: 5f69 6e69 745f 5f63 0200 0000 0000 0000  _init__c........
-000009a0: 0000 0000 0300 0000 0a00 0000 4b00 0000  ............K...
-000009b0: f336 0000 0074 0064 0764 017c 0164 0219  .6...t.d.d.|.d..
-000009c0: 0074 017c 01a0 0264 0367 00a1 0283 0174  .t.|...d.g.....t
-000009d0: 017c 01a0 0264 0467 00a1 0283 017c 0164  .|...d.g.....|.d
-000009e0: 059c 057c 02a4 018e 0153 0029 087a 2341  ...|.....S.).z#A
-000009f0: 6374 6976 6974 7920 6f66 2074 7970 6520  ctivity of type 
-00000a00: 4372 6561 7465 2066 726f 6d20 4f62 6a65  Create from Obje
-00000a10: 6374 5a06 4372 6561 7465 da0c 6174 7472  ctZ.Create..attr
-00000a20: 6962 7574 6564 546f 720e 0000 0072 0d00  ibutedTor....r..
-00000a30: 0000 a905 7207 0000 0072 0800 0000 720e  ....r....r....r.
-00000a40: 0000 0072 0d00 0000 7213 0000 004e 7218  ...r....r....Nr.
-00000a50: 0000 00a9 0372 0600 0000 7229 0000 00da  .....r....r)....
-00000a60: 0367 6574 a903 7217 0000 00da 036f 626a  .get..r......obj
-00000a70: da06 6b77 6172 6773 7218 0000 0072 1800  ..kwargsr....r..
-00000a80: 0000 7219 0000 00da 0663 7265 6174 654f  ..r......createO
-00000a90: 0000 00f3 1200 0000 0402 0201 0601 0e01  ................
-00000aa0: 0e01 0201 04fb 0206 06fa 7a16 4163 7469  ..........z.Acti
-00000ab0: 7669 7479 4661 6374 6f72 792e 6372 6561  vityFactory.crea
-00000ac0: 7465 6302 0000 0000 0000 0000 0000 0003  tec.............
-00000ad0: 0000 000a 0000 004b 0000 0072 2e00 0000  .......K...r....
-00000ae0: 2908 7a23 4163 7469 7669 7479 206f 6620  ).z#Activity of 
-00000af0: 7479 7065 2055 7064 6174 6520 6672 6f6d  type Update from
-00000b00: 204f 626a 6563 745a 0655 7064 6174 6572   ObjectZ.Updater
-00000b10: 2f00 0000 720e 0000 0072 0d00 0000 7230  /...r....r....r0
-00000b20: 0000 004e 7218 0000 0072 3100 0000 7233  ...Nr....r1...r3
-00000b30: 0000 0072 1800 0000 7218 0000 0072 1900  ...r....r....r..
-00000b40: 0000 da06 7570 6461 7465 5a00 0000 7237  ....updateZ...r7
-00000b50: 0000 007a 1641 6374 6976 6974 7946 6163  ...z.ActivityFac
-00000b60: 746f 7279 2e75 7064 6174 6563 0200 0000  tory.updatec....
-00000b70: 0000 0000 0000 0000 0300 0000 0600 0000  ................
-00000b80: 4b00 0000 f31c 0000 0074 0064 0564 017c  K........t.d.d.|
-00000b90: 006a 0164 0219 007c 0164 039c 037c 02a4  .j.d...|.d...|..
-00000ba0: 018e 0153 0029 067a 0f4c 696b 6520 666f  ...S.).z.Like fo
-00000bb0: 7220 7461 7267 6574 5a04 4c69 6b65 720a  r targetZ.Liker.
-00000bc0: 0000 00a9 0372 0700 0000 7208 0000 0072  .....r....r....r
-00000bd0: 1300 0000 4e72 1800 0000 a902 7206 0000  ....Nr......r...
-00000be0: 0072 2b00 0000 a903 7217 0000 0072 1200  .r+.....r....r..
-00000bf0: 0000 7235 0000 0072 1800 0000 7218 0000  ..r5...r....r...
-00000c00: 0072 1900 0000 da04 6c69 6b65 6500 0000  .r......likee...
-00000c10: f30a 0000 0004 020c 0104 ff02 0106 ff7a  ...............z
-00000c20: 1441 6374 6976 6974 7946 6163 746f 7279  .ActivityFactory
-00000c30: 2e6c 696b 6563 0200 0000 0000 0000 0000  .likec..........
-00000c40: 0000 0300 0000 0600 0000 4b00 0000 7239  ..........K...r9
-00000c50: 0000 0029 067a 1144 656c 6574 6520 666f  ...).z.Delete fo
-00000c60: 7220 7461 7267 6574 da06 4465 6c65 7465  r target..Delete
-00000c70: 720a 0000 0072 3a00 0000 4e72 1800 0000  r....r:...Nr....
-00000c80: 723b 0000 0072 3c00 0000 7218 0000 0072  r;...r<...r....r
-00000c90: 1800 0000 7219 0000 00da 0664 656c 6574  ....r......delet
-00000ca0: 656b 0000 0072 3e00 0000 7a16 4163 7469  ek...r>...z.Acti
-00000cb0: 7669 7479 4661 6374 6f72 792e 6465 6c65  vityFactory.dele
-00000cc0: 7465 6302 0000 0000 0000 0000 0000 0003  tec.............
-00000cd0: 0000 0006 0000 004b 0000 0072 3900 0000  .......K...r9...
-00000ce0: 2906 7a11 4163 6365 7074 2066 6f72 206f  ).z.Accept for o
-00000cf0: 626a 6563 74da 0641 6363 6570 7472 0a00  bject..Acceptr..
-00000d00: 0000 723a 0000 004e 7218 0000 0072 3b00  ..r:...Nr....r;.
-00000d10: 0000 7233 0000 0072 1800 0000 7218 0000  ..r3...r....r...
-00000d20: 0072 1900 0000 da06 6163 6365 7074 7100  .r......acceptq.
-00000d30: 0000 723e 0000 007a 1641 6374 6976 6974  ..r>...z.Activit
-00000d40: 7946 6163 746f 7279 2e61 6363 6570 7463  yFactory.acceptc
-00000d50: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-00000d60: 0900 0000 4b00 0000 7328 0000 0074 0064  ....K...s(...t.d
-00000d70: 0664 017c 006a 0164 0219 007c 017c 006a  .d.|.j.d...|.|.j
-00000d80: 01a0 0264 0367 00a1 0264 049c 047c 02a4  ...d.g...d...|..
-00000d90: 018e 0153 0029 077a 1341 6e6e 6f75 6e63  ...S.).z.Announc
-00000da0: 6520 666f 7220 6f62 6a65 6374 5a08 416e  e for objectZ.An
-00000db0: 6e6f 756e 6365 720a 0000 0072 0900 0000  nouncer....r....
-00000dc0: 2904 7207 0000 0072 0800 0000 7213 0000  ).r....r....r...
-00000dd0: 0072 0900 0000 4e72 1800 0000 2903 7206  .r....Nr....).r.
-00000de0: 0000 0072 2b00 0000 7232 0000 0072 3300  ...r+...r2...r3.
-00000df0: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
-00000e00: 00da 0861 6e6e 6f75 6e63 6577 0000 0073  ...announcew...s
-00000e10: 1000 0000 0402 0201 0801 0201 0c01 04fc  ................
-00000e20: 0205 06fb 7a18 4163 7469 7669 7479 4661  ....z.ActivityFa
-00000e30: 6374 6f72 792e 616e 6e6f 756e 6365 6302  ctory.announcec.
-00000e40: 0000 0000 0000 0000 0000 0003 0000 0007  ................
-00000e50: 0000 004b 0000 0073 2400 0000 7400 6405  ...K...s$...t.d.
-00000e60: 6401 7c00 6a01 6402 1900 7c01 7402 7c01  d.|.j.d...|.t.|.
-00000e70: 6701 8301 6403 9c04 7c02 a401 8e01 5300  g...d...|.....S.
-00000e80: 2906 7a11 466f 6c6c 6f77 2066 6f72 206f  ).z.Follow for o
-00000e90: 626a 6563 745a 0646 6f6c 6c6f 7772 0a00  bjectZ.Followr..
-00000ea0: 0000 2904 7207 0000 0072 0800 0000 7213  ..).r....r....r.
-00000eb0: 0000 0072 0d00 0000 4e72 1800 0000 2903  ...r....Nr....).
-00000ec0: 7206 0000 0072 2b00 0000 7229 0000 0072  r....r+...r)...r
-00000ed0: 3300 0000 7218 0000 0072 1800 0000 7219  3...r....r....r.
-00000ee0: 0000 00da 0666 6f6c 6c6f 7781 0000 0073  .....follow....s
-00000ef0: 1000 0000 0402 0201 0801 0201 0801 04fc  ................
-00000f00: 0205 06fb 7a16 4163 7469 7669 7479 4661  ....z.ActivityFa
-00000f10: 6374 6f72 792e 666f 6c6c 6f77 4e29 0c72  ctory.followN).r
-00000f20: 2300 0000 7224 0000 0072 2500 0000 7226  #...r$...r%...r&
-00000f30: 0000 0072 2d00 0000 7236 0000 0072 3800  ...r-...r6...r8.
-00000f40: 0000 723d 0000 0072 4000 0000 7242 0000  ..r=...r@...rB..
-00000f50: 0072 4300 0000 7244 0000 0072 1800 0000  .rC...rD...r....
-00000f60: 7218 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
-00000f70: 2a00 0000 4700 0000 7314 0000 0008 0004  *...G...s.......
-00000f80: 0108 0408 0308 0b08 0b08 0608 0608 060c  ................
-00000f90: 0a72 2a00 0000 4e29 08da 0b64 6174 6163  .r*...N)...datac
-00000fa0: 6c61 7373 6573 7202 0000 0072 0300 0000  lassesr....r....
-00000fb0: da06 7479 7069 6e67 7204 0000 0072 0500  ..typingr....r..
-00000fc0: 0000 7206 0000 0072 2a00 0000 7218 0000  ..r....r*...r...
-00000fd0: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00000fe0: da08 3c6d 6f64 756c 653e 0100 0000 730a  ..<module>....s.
-00000ff0: 0000 0010 0010 0102 0310 0112 41         ............A
+000008a0: 005a 0b64 1264 1384 005a 0c64 1453 0029  .Z.d.d...Z.d.S.)
+000008b0: 15da 0f41 6374 6976 6974 7946 6163 746f  ...ActivityFacto
+000008c0: 7279 7a49 4261 7369 6320 6661 6374 6f72  ryzIBasic factor
+000008d0: 7920 666f 7220 4163 7469 7669 7479 206f  y for Activity o
+000008e0: 626a 6563 7473 2e0a 0a20 2020 2055 7361  bjects...    Usa
+000008f0: 6c6c 7920 6372 6561 7465 6420 6279 2061  lly created by a
+00000900: 2042 6f76 696e 6543 6c69 656e 7463 0200   BovineClientc..
+00000910: 0000 0000 0000 0000 0000 0200 0000 0200  ................
+00000920: 0000 4300 0000 730a 0000 007c 017c 005f  ..C...s....|.|._
+00000930: 0064 0053 0029 014e 2901 da0b 696e 666f  .d.S.).N)...info
+00000940: 726d 6174 696f 6e29 0272 1700 0000 da11  rmation).r......
+00000950: 6163 746f 725f 696e 666f 726d 6174 696f  actor_informatio
+00000960: 6e72 1800 0000 7218 0000 0072 1900 0000  nr....r....r....
+00000970: da08 5f5f 696e 6974 5f5f 4c00 0000 7302  ..__init__L...s.
+00000980: 0000 000a 017a 1841 6374 6976 6974 7946  .....z.ActivityF
+00000990: 6163 746f 7279 2e5f 5f69 6e69 745f 5f63  actory.__init__c
+000009a0: 0200 0000 0000 0000 0000 0000 0300 0000  ................
+000009b0: 0a00 0000 4b00 0000 f336 0000 0074 0064  ....K....6...t.d
+000009c0: 0764 017c 0164 0219 0074 017c 01a0 0264  .d.|.d...t.|...d
+000009d0: 0367 00a1 0283 0174 017c 01a0 0264 0467  .g.....t.|...d.g
+000009e0: 00a1 0283 017c 0164 059c 057c 02a4 018e  .....|.d...|....
+000009f0: 0153 0029 087a 2341 6374 6976 6974 7920  .S.).z#Activity 
+00000a00: 6f66 2074 7970 6520 4372 6561 7465 2066  of type Create f
+00000a10: 726f 6d20 4f62 6a65 6374 5a06 4372 6561  rom ObjectZ.Crea
+00000a20: 7465 da0c 6174 7472 6962 7574 6564 546f  te..attributedTo
+00000a30: 720e 0000 0072 0d00 0000 a905 7207 0000  r....r......r...
+00000a40: 0072 0800 0000 720e 0000 0072 0d00 0000  .r....r....r....
+00000a50: 7213 0000 004e 7218 0000 00a9 0372 0600  r....Nr......r..
+00000a60: 0000 7229 0000 00da 0367 6574 a903 7217  ..r).....get..r.
+00000a70: 0000 00da 036f 626a da06 6b77 6172 6773  .....obj..kwargs
+00000a80: 7218 0000 0072 1800 0000 7219 0000 00da  r....r....r.....
+00000a90: 0663 7265 6174 654f 0000 00f3 1200 0000  .createO........
+00000aa0: 0402 0201 0601 0e01 0e01 0201 04fb 0206  ................
+00000ab0: 06fa 7a16 4163 7469 7669 7479 4661 6374  ..z.ActivityFact
+00000ac0: 6f72 792e 6372 6561 7465 6302 0000 0000  ory.createc.....
+00000ad0: 0000 0000 0000 0003 0000 000a 0000 004b  ...............K
+00000ae0: 0000 0072 2e00 0000 2908 7a23 4163 7469  ...r....).z#Acti
+00000af0: 7669 7479 206f 6620 7479 7065 2055 7064  vity of type Upd
+00000b00: 6174 6520 6672 6f6d 204f 626a 6563 745a  ate from ObjectZ
+00000b10: 0655 7064 6174 6572 2f00 0000 720e 0000  .Updater/...r...
+00000b20: 0072 0d00 0000 7230 0000 004e 7218 0000  .r....r0...Nr...
+00000b30: 0072 3100 0000 7233 0000 0072 1800 0000  .r1...r3...r....
+00000b40: 7218 0000 0072 1900 0000 da06 7570 6461  r....r......upda
+00000b50: 7465 5a00 0000 7237 0000 007a 1641 6374  teZ...r7...z.Act
+00000b60: 6976 6974 7946 6163 746f 7279 2e75 7064  ivityFactory.upd
+00000b70: 6174 6563 0200 0000 0000 0000 0000 0000  atec............
+00000b80: 0300 0000 0600 0000 4b00 0000 f31c 0000  ........K.......
+00000b90: 0074 0064 0564 017c 006a 0164 0219 007c  .t.d.d.|.j.d...|
+00000ba0: 0164 039c 037c 02a4 018e 0153 0029 067a  .d...|.....S.).z
+00000bb0: 0f4c 696b 6520 666f 7220 7461 7267 6574  .Like for target
+00000bc0: 5a04 4c69 6b65 720a 0000 00a9 0372 0700  Z.Liker......r..
+00000bd0: 0000 7208 0000 0072 1300 0000 4e72 1800  ..r....r....Nr..
+00000be0: 0000 a902 7206 0000 0072 2b00 0000 a903  ....r....r+.....
+00000bf0: 7217 0000 0072 1200 0000 7235 0000 0072  r....r....r5...r
+00000c00: 1800 0000 7218 0000 0072 1900 0000 da04  ....r....r......
+00000c10: 6c69 6b65 6500 0000 f30a 0000 0004 020c  likee...........
+00000c20: 0104 ff02 0106 ff7a 1441 6374 6976 6974  .......z.Activit
+00000c30: 7946 6163 746f 7279 2e6c 696b 6563 0200  yFactory.likec..
+00000c40: 0000 0000 0000 0000 0000 0300 0000 0600  ................
+00000c50: 0000 4b00 0000 7239 0000 0029 067a 1144  ..K...r9...).z.D
+00000c60: 656c 6574 6520 666f 7220 7461 7267 6574  elete for target
+00000c70: da06 4465 6c65 7465 720a 0000 0072 3a00  ..Deleter....r:.
+00000c80: 0000 4e72 1800 0000 723b 0000 0072 3c00  ..Nr....r;...r<.
+00000c90: 0000 7218 0000 0072 1800 0000 7219 0000  ..r....r....r...
+00000ca0: 00da 0664 656c 6574 656b 0000 0072 3e00  ...deletek...r>.
+00000cb0: 0000 7a16 4163 7469 7669 7479 4661 6374  ..z.ActivityFact
+00000cc0: 6f72 792e 6465 6c65 7465 6302 0000 0000  ory.deletec.....
+00000cd0: 0000 0000 0000 0003 0000 0006 0000 004b  ...............K
+00000ce0: 0000 0072 3900 0000 2906 7a11 4163 6365  ...r9...).z.Acce
+00000cf0: 7074 2066 6f72 206f 626a 6563 74da 0641  pt for object..A
+00000d00: 6363 6570 7472 0a00 0000 723a 0000 004e  cceptr....r:...N
+00000d10: 7218 0000 0072 3b00 0000 7233 0000 0072  r....r;...r3...r
+00000d20: 1800 0000 7218 0000 0072 1900 0000 da06  ....r....r......
+00000d30: 6163 6365 7074 7100 0000 723e 0000 007a  acceptq...r>...z
+00000d40: 1641 6374 6976 6974 7946 6163 746f 7279  .ActivityFactory
+00000d50: 2e61 6363 6570 7463 0200 0000 0000 0000  .acceptc........
+00000d60: 0000 0000 0300 0000 0600 0000 4b00 0000  ............K...
+00000d70: 7239 0000 0029 067a 1152 656a 6563 7420  r9...).z.Reject 
+00000d80: 666f 7220 6f62 6a65 6374 5a06 5265 6a65  for objectZ.Reje
+00000d90: 6374 720a 0000 0072 3a00 0000 4e72 1800  ctr....r:...Nr..
+00000da0: 0000 723b 0000 0072 3300 0000 7218 0000  ..r;...r3...r...
+00000db0: 0072 1800 0000 7219 0000 00da 0672 656a  .r....r......rej
+00000dc0: 6563 7477 0000 0072 3e00 0000 7a16 4163  ectw...r>...z.Ac
+00000dd0: 7469 7669 7479 4661 6374 6f72 792e 7265  tivityFactory.re
+00000de0: 6a65 6374 6302 0000 0000 0000 0000 0000  jectc...........
+00000df0: 0003 0000 0009 0000 004b 0000 0073 2800  .........K...s(.
+00000e00: 0000 7400 6406 6401 7c00 6a01 6402 1900  ..t.d.d.|.j.d...
+00000e10: 7c01 7c00 6a01 a002 6403 6700 a102 6404  |.|.j...d.g...d.
+00000e20: 9c04 7c02 a401 8e01 5300 2907 7a13 416e  ..|.....S.).z.An
+00000e30: 6e6f 756e 6365 2066 6f72 206f 626a 6563  nounce for objec
+00000e40: 745a 0841 6e6e 6f75 6e63 6572 0a00 0000  tZ.Announcer....
+00000e50: 7209 0000 0029 0472 0700 0000 7208 0000  r....).r....r...
+00000e60: 0072 1300 0000 7209 0000 004e 7218 0000  .r....r....Nr...
+00000e70: 0029 0372 0600 0000 722b 0000 0072 3200  .).r....r+...r2.
+00000e80: 0000 7233 0000 0072 1800 0000 7218 0000  ..r3...r....r...
+00000e90: 0072 1900 0000 da08 616e 6e6f 756e 6365  .r......announce
+00000ea0: 7d00 0000 7310 0000 0004 0202 0108 0102  }...s...........
+00000eb0: 010c 0104 fc02 0506 fb7a 1841 6374 6976  .........z.Activ
+00000ec0: 6974 7946 6163 746f 7279 2e61 6e6e 6f75  ityFactory.annou
+00000ed0: 6e63 6563 0200 0000 0000 0000 0000 0000  ncec............
+00000ee0: 0300 0000 0700 0000 4b00 0000 7324 0000  ........K...s$..
+00000ef0: 0074 0064 0564 017c 006a 0164 0219 007c  .t.d.d.|.j.d...|
+00000f00: 0174 027c 0167 0183 0164 039c 047c 02a4  .t.|.g...d...|..
+00000f10: 018e 0153 0029 067a 1146 6f6c 6c6f 7720  ...S.).z.Follow 
+00000f20: 666f 7220 6f62 6a65 6374 5a06 466f 6c6c  for objectZ.Foll
+00000f30: 6f77 720a 0000 0029 0472 0700 0000 7208  owr....).r....r.
+00000f40: 0000 0072 1300 0000 720d 0000 004e 7218  ...r....r....Nr.
+00000f50: 0000 0029 0372 0600 0000 722b 0000 0072  ...).r....r+...r
+00000f60: 2900 0000 7233 0000 0072 1800 0000 7218  )...r3...r....r.
+00000f70: 0000 0072 1900 0000 da06 666f 6c6c 6f77  ...r......follow
+00000f80: 8700 0000 7310 0000 0004 0202 0108 0102  ....s...........
+00000f90: 0108 0104 fc02 0506 fb7a 1641 6374 6976  .........z.Activ
+00000fa0: 6974 7946 6163 746f 7279 2e66 6f6c 6c6f  ityFactory.follo
+00000fb0: 774e 290d 7223 0000 0072 2400 0000 7225  wN).r#...r$...r%
+00000fc0: 0000 0072 2600 0000 722d 0000 0072 3600  ...r&...r-...r6.
+00000fd0: 0000 7238 0000 0072 3d00 0000 7240 0000  ..r8...r=...r@..
+00000fe0: 0072 4200 0000 7243 0000 0072 4400 0000  .rB...rC...rD...
+00000ff0: 7245 0000 0072 1800 0000 7218 0000 0072  rE...r....r....r
+00001000: 1800 0000 7219 0000 0072 2a00 0000 4700  ....r....r*...G.
+00001010: 0000 7316 0000 0008 0004 0108 0408 0308  ..s.............
+00001020: 0b08 0b08 0608 0608 0608 060c 0a72 2a00  .............r*.
+00001030: 0000 4e29 08da 0b64 6174 6163 6c61 7373  ..N)...dataclass
+00001040: 6573 7202 0000 0072 0300 0000 da06 7479  esr....r......ty
+00001050: 7069 6e67 7204 0000 0072 0500 0000 7206  pingr....r....r.
+00001060: 0000 0072 2a00 0000 7218 0000 0072 1800  ...r*...r....r..
+00001070: 0000 7218 0000 0072 1900 0000 da08 3c6d  ..r....r......<m
+00001080: 6f64 756c 653e 0100 0000 730a 0000 0010  odule>....s.....
+00001090: 0010 0102 0310 0112 41                   ........A
```

### Comparing `bovine-0.1.1/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc` & `bovine-0.1.2/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 4240 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 9010 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 9010 0000  o.........Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 6d06 5a06 6d07 5a07 0100 6404 6405 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6502 4700 6406 6407 8400  m.Z...e.G.d.d...
 00000070: 6407 8302 8301 5a0a 4700 6408 6409 8400  d.....Z.G.d.d...
```

### Comparing `bovine-0.1.1/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.2/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 2163 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 7308 0000  o.........:ds...
+00000000: 6f0d 0d0a 0000 0000 8013 4164 7308 0000  o.........Ads...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6402 6404 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
 00000060: 6405 6406 8400 5a0a 6407 6408 8400 5a0b  d.d...Z.d.d...Z.
 00000070: 6409 640a 8400 5a0c 640b 640c 8400 5a0d  d.d...Z.d.d...Z.
@@ -241,15 +241,15 @@
 00000f00: a00a 7c02 a101 7405 a00a 7c03 a101 7405  ..|...t...|...t.
 00000f10: a00a 7c04 a101 7405 a00a 7c05 a101 640a  ..|...t...|...d.
 00000f20: 9c06 1600 7d07 640b 640c 7c07 6901 1600  ....}.d.d.|.i...
 00000f30: 7d08 740b 7405 a00c 7c08 a101 8301 8201  }.t.t...|.......
 00000f40: 6400 0400 7d02 0400 7d03 0400 7d04 0400  d...}...}...}...
 00000f50: 7d06 7d05 6400 5300 290d 4e72 0500 0000  }.}.d.S.).Nr....
 00000f60: 7206 0000 0072 0700 0000 7209 0000 003e  r....r....r....>
-00000f70: 0400 0000 722f 0000 0072 0b00 0000 722e  ....r/...r....r.
+00000f70: 0400 0000 720b 0000 0072 2e00 0000 722f  ....r....r....r/
 00000f80: 0000 0072 1700 0000 720d 0000 0029 017a  ...r....r....).z
 00000f90: 6225 2870 7937 2973 0a7b 2528 7079 3729  b%(py7)s.{%(py7)
 00000fa0: 7320 3d20 2528 7079 3029 7328 2528 7079  s = %(py0)s(%(py
 00000fb0: 3529 730a 7b25 2870 7935 2973 203d 2025  5)s.{%(py5)s = %
 00000fc0: 2870 7933 2973 0a7b 2528 7079 3329 7320  (py3)s.{%(py3)s 
 00000fd0: 3d20 2528 7079 3129 732e 6b65 7973 0a7d  = %(py1)s.keys.}
 00000fe0: 2829 0a7d 290a 7d20 3d3d 2025 2870 7931  ().}).} == %(py1
```

### Comparing `bovine-0.1.1/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.2/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 1418 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 8a05 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 8a05 0000  o.........Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
 00000060: 6405 6406 8400 5a0a 6407 6408 8400 5a0b  d.d...Z.d.d...Z.
 00000070: 6409 640a 8400 5a0c 6401 5300 290b e900  d.d...Z.d.S.)...
@@ -61,35 +61,35 @@
 000003c0: a009 7c09 a101 7404 a009 7c0a a101 6414  ..|...t...|...d.
 000003d0: 9c02 1600 7d0b 6415 6416 7c0b 6901 1600  ....}.d.d.|.i...
 000003e0: 7d0c 740a 7404 a00b 7c0c a101 8301 8201  }.t.t...|.......
 000003f0: 6400 0400 7d09 0400 7d02 7d0a 6400 5300  d...}...}.}.d.S.
 00000400: 2917 4efa 1c68 7474 703a 2f2f 6578 616d  ).N..http://exam
 00000410: 706c 652e 636f 6d2f 6163 746f 722f 3132  ple.com/actor/12
 00000420: 3329 01da 0269 643e 0500 0000 da05 696e  3)...id>......in
-00000430: 626f 78fa 0840 636f 6e74 6578 7472 0600  box..@contextr..
-00000440: 0000 da04 7479 7065 da06 6f75 7462 6f78  ....type..outbox
+00000430: 626f 7872 0600 0000 da04 7479 7065 fa08  boxr......type..
+00000440: 4063 6f6e 7465 7874 da06 6f75 7462 6f78  @context..outbox
 00000450: a901 fa02 3d3d 2901 7a62 2528 7079 3729  ....==).zb%(py7)
 00000460: 730a 7b25 2870 7937 2973 203d 2025 2870  s.{%(py7)s = %(p
 00000470: 7930 2973 2825 2870 7935 2973 0a7b 2528  y0)s(%(py5)s.{%(
 00000480: 7079 3529 7320 3d20 2528 7079 3329 730a  py5)s = %(py3)s.
 00000490: 7b25 2870 7933 2973 203d 2025 2870 7931  {%(py3)s = %(py1
 000004a0: 2973 2e6b 6579 730a 7d28 290a 7d29 0a7d  )s.keys.}().}).}
 000004b0: 203d 3d20 2528 7079 3130 2973 da03 7365   == %(py10)s..se
 000004c0: 74da 0672 6573 756c 7429 06da 0370 7930  t..result)...py0
 000004d0: da03 7079 31da 0370 7933 da03 7079 35da  ..py1..py3..py5.
 000004e0: 0370 7937 da04 7079 3130 7a0f 6173 7365  .py7..py10z.asse
 000004f0: 7274 2025 2870 7931 3229 73da 0470 7931  rt %(py12)s..py1
 00000500: 327a 084a 6f68 6e20 446f 653e 0600 0000  2z.John Doe>....
-00000510: 7207 0000 0072 0800 0000 7206 0000 0072  r....r....r....r
-00000520: 0900 0000 720a 0000 00da 046e 616d 655a  ....r......nameZ
+00000510: da04 6e61 6d65 7206 0000 0072 0700 0000  ..namer....r....
+00000520: 7208 0000 0072 0900 0000 720a 0000 005a  r....r....r....Z
 00000530: 1130 3132 3334 3536 3738 3930 3132 3334  .012345678901234
-00000540: 3536 da03 6b65 793e 0700 0000 7207 0000  56..key>....r...
-00000550: 0072 0800 0000 da09 7075 626c 6963 4b65  .r......publicKe
-00000560: 7972 0600 0000 7209 0000 0072 0a00 0000  yr....r....r....
-00000570: 7216 0000 0072 1800 0000 7a04 236b 6579  r....r....z.#key
+00000540: 3536 da03 6b65 793e 0700 0000 7216 0000  56..key>....r...
+00000550: 0072 0600 0000 7207 0000 00da 0970 7562  .r....r......pub
+00000560: 6c69 634b 6579 7208 0000 0072 0900 0000  licKeyr....r....
+00000570: 720a 0000 0072 1800 0000 7a04 236b 6579  r....r....z.#key
 00000580: 2903 7206 0000 00da 056f 776e 6572 da0c  ).r......owner..
 00000590: 7075 626c 6963 4b65 7950 656d a901 7a12  publicKeyPem..z.
 000005a0: 2528 7079 3129 7320 3d3d 2025 2870 7934  %(py1)s == %(py4
 000005b0: 2973 a902 7210 0000 00da 0370 7934 fa0e  )s..r......py4..
 000005c0: 6173 7365 7274 2025 2870 7936 2973 da03  assert %(py6)s..
 000005d0: 7079 3629 1072 0400 0000 da05 6275 696c  py6).r......buil
 000005e0: 64da 046b 6579 7372 0d00 0000 da0a 4070  d..keysr......@p
@@ -181,15 +181,15 @@
 00000b40: 6b02 7d04 7c04 7341 7403 a004 6408 7c04  k.}.|.sAt...d.|.
 00000b50: 6601 6409 7c02 7c03 6602 a104 7403 a005  f.d.|.|.f...t...
 00000b60: 7c02 a101 7403 a005 7c03 a101 640a 9c02  |...t...|...d...
 00000b70: 1600 7d05 640b 640c 7c05 6901 1600 7d06  ..}.d.d.|.i...}.
 00000b80: 7406 7403 a007 7c06 a101 8301 8201 6400  t.t...|.......d.
 00000b90: 0400 7d02 0400 7d04 7d03 6400 5300 290d  ..}...}.}.d.S.).
 00000ba0: 4e72 0500 0000 7207 0000 0072 0a00 0000  Nr....r....r....
-00000bb0: 723b 0000 0072 0900 0000 5a05 496d 6167  r;...r....Z.Imag
+00000bb0: 723b 0000 0072 0800 0000 5a05 496d 6167  r;...r....Z.Imag
 00000bc0: 65da 0469 636f 6e72 0b00 0000 721b 0000  e..iconr....r...
 00000bd0: 0072 1c00 0000 721e 0000 0072 1f00 0000  .r....r....r....
 00000be0: 2908 7204 0000 0072 4300 0000 7220 0000  ).r....rC...r ..
 00000bf0: 0072 2200 0000 7223 0000 0072 2700 0000  .r"...r#...r'...
 00000c00: 7228 0000 0072 2900 0000 7241 0000 0072  r(...r)...rA...r
 00000c10: 3800 0000 7238 0000 0072 3900 0000 da14  8...r8...r9.....
 00000c20: 7465 7374 5f61 6374 6f72 5f77 6974 685f  test_actor_with_
```

### Comparing `bovine-0.1.1/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.2/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 1381 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 6505 0000  o.........:de...
+00000000: 6f0d 0d0a 0000 0000 8013 4164 6505 0000  o.........Ade...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6400 6402 6c07 6d08 5a08 0100 6403 6404  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 0100 6405 6406 8400 5a0b  l.m.Z...d.d...Z.
 00000070: 6407 6408 8400 5a0c 6401 5300 2909 e900  d.d...Z.d.S.)...
@@ -38,18 +38,18 @@
 00000250: 0366 0164 0f7c 0a7c 0b66 02a1 0474 07a0  .f.d.|.|.f...t..
 00000260: 0c7c 0aa1 0174 07a0 0c7c 0ba1 0164 109c  .|...t...|...d..
 00000270: 0216 007d 0c64 1164 127c 0c69 0116 007d  ...}.d.d.|.i...}
 00000280: 0d74 0d74 07a0 0e7c 0da1 0183 0182 0164  .t.t...|.......d
 00000290: 0004 007d 0a04 007d 037d 0b64 0053 0029  ...}...}.}.d.S.)
 000002a0: 144e da08 6163 746f 725f 6964 da09 666f  .N..actor_id..fo
 000002b0: 6c6c 6f77 6572 7329 02da 0269 6472 0600  llowers)...idr..
-000002c0: 0000 da04 7465 7874 3e06 0000 00da 0763  ....text>......c
-000002d0: 6f6e 7465 6e74 da02 6363 fa08 4063 6f6e  ontent..cc..@con
-000002e0: 7465 7874 da04 7479 7065 da0c 6174 7472  text..type..attr
-000002f0: 6962 7574 6564 546f da02 746f a901 fa02  ibutedTo..to....
+000002c0: 0000 da04 7465 7874 3e06 0000 00da 0263  ....text>......c
+000002d0: 63da 0763 6f6e 7465 6e74 da04 7479 7065  c..content..type
+000002e0: da0c 6174 7472 6962 7574 6564 546f fa08  ..attributedTo..
+000002f0: 4063 6f6e 7465 7874 da02 746f a901 fa02  @context..to....
 00000300: 3d3d a901 7a62 2528 7079 3729 730a 7b25  ==..zb%(py7)s.{%
 00000310: 2870 7937 2973 203d 2025 2870 7930 2973  (py7)s = %(py0)s
 00000320: 2825 2870 7935 2973 0a7b 2528 7079 3529  (%(py5)s.{%(py5)
 00000330: 7320 3d20 2528 7079 3329 730a 7b25 2870  s = %(py3)s.{%(p
 00000340: 7933 2973 203d 2025 2870 7931 2973 2e6b  y3)s = %(py1)s.k
 00000350: 6579 730a 7d28 290a 7d29 0a7d 203d 3d20  eys.}().}).} == 
 00000360: 2528 7079 3130 2973 da03 7365 74da 0672  %(py10)s..set..r
@@ -59,17 +59,17 @@
 000003a0: 2870 7931 3229 73da 0470 7931 3272 0e00  (py12)s..py12r..
 000003b0: 0000 7a2c 6874 7470 733a 2f2f 7777 772e  ..z,https://www.
 000003c0: 7733 2e6f 7267 2f6e 732f 6163 7469 7669  w3.org/ns/activi
 000003d0: 7479 7374 7265 616d 7323 5075 626c 6963  tystreams#Public
 000003e0: a901 7a12 2528 7079 3129 7320 3d3d 2025  ..z.%(py1)s == %
 000003f0: 2870 7934 2973 a902 7216 0000 00da 0370  (py4)s..r......p
 00000400: 7934 fa0e 6173 7365 7274 2025 2870 7936  y4..assert %(py6
-00000410: 2973 da03 7079 3672 0a00 0000 290f 7204  )s..py6r....).r.
+00000410: 2973 da03 7079 3672 0900 0000 290f 7204  )s..py6r....).r.
 00000420: 0000 00da 046e 6f74 65da 0961 735f 7075  .....note..as_pu
-00000430: 626c 6963 7209 0000 00da 0562 7569 6c64  blicr......build
+00000430: 626c 6963 720a 0000 00da 0562 7569 6c64  blicr......build
 00000440: da04 6b65 7973 7212 0000 00da 0a40 7079  ..keysr......@py
 00000450: 7465 7374 5f61 72da 115f 6361 6c6c 5f72  test_ar.._call_r
 00000460: 6570 7263 6f6d 7061 7265 da0c 4070 795f  eprcompare..@py_
 00000470: 6275 696c 7469 6e73 da06 6c6f 6361 6c73  builtins..locals
 00000480: da18 5f73 686f 756c 645f 7265 7072 5f67  .._should_repr_g
 00000490: 6c6f 6261 6c5f 6e61 6d65 da09 5f73 6166  lobal_name.._saf
 000004a0: 6572 6570 72da 0e41 7373 6572 7469 6f6e  erepr..Assertion
@@ -144,21 +144,21 @@
 000008f0: 7412 740c a013 7c10 a101 8301 8201 6400  t.t...|.......d.
 00000900: 0400 7d0d 0400 7d06 7d0e 6400 5300 291d  ..}...}.}.d.S.).
 00000910: 4e7a 1468 7474 7073 3a2f 2f72 656d 6f74  Nz.https://remot
 00000920: 652f 616c 6963 657a 2568 7474 7073 3a2f  e/alicez%https:/
 00000930: 2f77 7777 2e77 332e 6f72 672f 6e73 2f61  /www.w3.org/ns/a
 00000940: 6374 6976 6974 7973 7472 6561 6d73 da06  ctivitystreams..
 00000950: 5065 7273 6f6e 5a06 616c 7973 7361 2904  PersonZ.alyssa).
-00000960: 720b 0000 0072 0700 0000 720c 0000 00da  r....r....r.....
+00000960: 720d 0000 0072 0700 0000 720b 0000 00da  r....r....r.....
 00000970: 1170 7265 6665 7272 6564 5573 6572 6e61  .preferredUserna
 00000980: 6d65 2901 da06 636c 6965 6e74 3e04 0000  me)...client>...
-00000990: 0072 0b00 0000 da04 6e61 6d65 720c 0000  .r......namer...
+00000990: 0072 0d00 0000 da04 6e61 6d65 720b 0000  .r......namer...
 000009a0: 00da 0468 7265 6672 0f00 0000 7211 0000  ...hrefr....r...
 000009b0: 0072 1200 0000 da07 6d65 6e74 696f 6e72  .r......mentionr
-000009c0: 1400 0000 721b 0000 0072 1c00 0000 720c  ....r....r....r.
+000009c0: 1400 0000 721b 0000 0072 1c00 0000 720b  ....r....r....r.
 000009d0: 0000 00da 074d 656e 7469 6f6e 721d 0000  .....Mentionr...
 000009e0: 0072 1e00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
 000009f0: 7241 0000 0029 017a 1225 2870 7931 2973  rA...).z.%(py1)s
 00000a00: 203d 3d20 2528 7079 3329 73da 0a72 656d   == %(py3)s..rem
 00000a10: 6f74 655f 7572 6929 0272 1600 0000 7217  ote_uri).r....r.
 00000a20: 0000 007a 0e61 7373 6572 7420 2528 7079  ...z.assert %(py
 00000a30: 3529 7372 1800 0000 7240 0000 007a 0d61  5)sr....r@...z.a
```

### Comparing `bovine-0.1.1/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.2/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 1010 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 f203 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 f203 0000  o.........Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6404 6405 8400 5a08 6406 6407  Z...d.d...Z.d.d.
 00000060: 8400 5a09 6408 6409 8400 5a0a 6401 5300  ..Z.d.d...Z.d.S.
 00000070: 290a e900 0000 004e e901 0000 0029 01da  )......N.....)..
```

### Comparing `bovine-0.1.1/bovine/activitystreams/__pycache__/test_ordered_collection_page.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.2/bovine/activitystreams/__pycache__/test_ordered_collection_page.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 809 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 2903 0000  o.........:d)...
+00000000: 6f0d 0d0a 0000 0000 8013 4164 2903 0000  o.........Ad)...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6404 6405 8400 5a08 6401 5300  Z...d.d...Z.d.S.
 00000060: 2906 e900 0000 004e e901 0000 0029 01da  )......N.....)..
 00000070: 154f 7264 6572 6564 436f 6c6c 6563 7469  .OrderedCollecti
```

### Comparing `bovine-0.1.1/bovine/activitystreams/activity_factory.py` & `bovine-0.1.2/bovine/activitystreams/activity_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,20 @@
 
     def accept(self, obj, **kwargs):
         """Accept for object"""
         return Activity(
             type="Accept", actor=self.information["id"], object=obj, **kwargs
         )
 
+    def reject(self, obj, **kwargs):
+        """Reject for object"""
+        return Activity(
+            type="Reject", actor=self.information["id"], object=obj, **kwargs
+        )
+
     def announce(self, obj, **kwargs):
         """Announce for object"""
         return Activity(
             type="Announce",
             actor=self.information["id"],
             object=obj,
             followers=self.information.get("followers", []),
```

### Comparing `bovine-0.1.1/bovine/activitystreams/object_factory.py` & `bovine-0.1.2/bovine/activitystreams/object_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/activitystreams/test_activity_factory.py` & `bovine-0.1.2/bovine/activitystreams/test_activity_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/activitystreams/test_actor.py` & `bovine-0.1.2/bovine/activitystreams/test_actor.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/activitystreams/test_object_factory.py` & `bovine-0.1.2/bovine/activitystreams/test_object_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/activitystreams/test_ordered_collection_builder.py` & `bovine-0.1.2/bovine/activitystreams/test_ordered_collection_builder.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/activitystreams/test_ordered_collection_page.py` & `bovine-0.1.2/bovine/activitystreams/test_ordered_collection_page.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/activitystreams/utils/__init__.py` & `bovine-0.1.2/bovine/activitystreams/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc` & `bovine-0.1.2/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 2354 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 3209 0000  o.........:d2...
+00000000: 6f0d 0d0a 0000 0000 8013 4164 3209 0000  o.........Ad2...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6403 6504 6404 6505 6604  m.Z...d.e.d.e.f.
 00000050: 6405 6406 8404 5a06 6403 6501 6504 6505  d.d...Z.d.e.e.e.
 00000060: 4200 1900 6404 6501 6505 1900 6604 6407  B...d.e.e...f.d.
 00000070: 6408 8404 5a07 6409 640a 8400 5a08 6403  d...Z.d.d...Z.d.
```

### Comparing `bovine-0.1.1/bovine/activitystreams/utils/__pycache__/print.cpython-310.pyc` & `bovine-0.1.2/bovine/activitystreams/utils/__pycache__/print.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 787 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 1303 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 1303 0000  o.........Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1c00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6402 6403 8400 5a01 6404  d.l.Z.d.d...Z.d.
 00000040: 6405 8400 5a02 6401 5300 2906 e900 0000  d...Z.d.S.).....
 00000050: 004e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
 00000060: 0000 0007 0000 0043 0000 0073 6000 0000  .......C...s`...
 00000070: 6401 7c00 7600 7217 7400 6402 7c00 6401  d.|.v.r.t.d.|.d.
```

### Comparing `bovine-0.1.1/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.2/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 2266 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 da08 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 da08 0000  o.........Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 6d0a  Z...d.d.l.m.Z.m.
 00000060: 5a0a 6d0b 5a0b 6d0c 5a0c 0100 6405 6406  Z.m.Z.m.Z...d.d.
 00000070: 8400 5a0d 6407 6408 8400 5a0e 6409 640a  ..Z.d.d...Z.d.d.
```

### Comparing `bovine-0.1.1/bovine/activitystreams/utils/print.py` & `bovine-0.1.2/bovine/activitystreams/utils/print.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/activitystreams/utils/test_utils.py` & `bovine-0.1.2/bovine/activitystreams/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/clients/__init__.py` & `bovine-0.1.2/bovine/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/clients/__pycache__/__init__.cpython-310.pyc` & `bovine-0.1.2/bovine/clients/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 2081 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 2108 0000  o.........:d!...
+00000000: 6f0d 0d0a 0000 0000 8013 4164 2108 0000  o.........Ad!...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6403 6404 6c05 6d06 5a06 0100 6403  ..d.d.l.m.Z...d.
 00000060: 6405 6c07 6d08 5a08 6d09 5a09 0100 6500  d.l.m.Z.m.Z...e.
 00000070: a00a 650b a101 5a0c 6406 6502 6a0d 6407  ..e...Z.d.e.j.d.
```

### Comparing `bovine-0.1.1/bovine/clients/__pycache__/event_source.cpython-310.pyc` & `bovine-0.1.2/bovine/clients/__pycache__/event_source.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 1106 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 5204 0000  o.........:dR...
+00000000: 6f0d 0d0a 0000 0000 8013 4164 5204 0000  o.........AdR...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 8302 5a03  ..G.d.d...d...Z.
 00000050: 6401 5300 2905 e900 0000 004e 2901 da0f  d.S.)......N)...
 00000060: 5365 7276 6572 5365 6e74 4576 656e 7463  ServerSentEventc
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `bovine-0.1.1/bovine/clients/__pycache__/lookup_account.cpython-310.pyc` & `bovine-0.1.2/bovine/clients/__pycache__/lookup_account.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 787 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 1303 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 1303 0000  o.........Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6402 6403 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6501 a005 6506 a101 5a07 6404 6502  ..e...e...Z.d.e.
 00000060: 6a08 6405 6509 6406 650a 6606 6407 6408  j.d.e.d.e.f.d.d.
 00000070: 8404 5a0b 6401 5300 2909 e900 0000 004e  ..Z.d.S.)......N
```

### Comparing `bovine-0.1.1/bovine/clients/__pycache__/moo_auth_client.cpython-310.pyc` & `bovine-0.1.2/bovine/clients/__pycache__/moo_auth_client.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 3176 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 680c 0000  o.........:dh...
+00000000: 6f0d 0d0a 0000 0000 8013 4164 680c 0000  o.........Adh...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6405  ..d.d.l.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 6405 6407 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6408 6409 8400 5a0c 4700  m.Z...d.d...Z.G.
```

### Comparing `bovine-0.1.1/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc` & `bovine-0.1.2/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 948 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 b403 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 b403 0000  o.........Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6402  d.l.Z.d.d.l.Z.d.
 00000050: 6403 6c04 6d05 5a05 0100 6501 a006 6507  d.l.m.Z...e...e.
 00000060: a101 5a08 6404 6503 6a09 6405 650a 6406  ..Z.d.e.j.d.e.d.
 00000070: 650b 6606 6407 6408 8404 5a0c 6404 6503  e.f.d.d...Z.d.e.
```

### Comparing `bovine-0.1.1/bovine/clients/__pycache__/signed_http.cpython-310.pyc` & `bovine-0.1.2/bovine/clients/__pycache__/signed_http.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 3278 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 ce0c 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 ce0c 0000  o.........Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000f 0000 0040 0000 0073 e400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6403 6c04  ..d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6406  ..d.d.l.m.Z...d.
 00000070: 6407 6c0a 6d0b 5a0b 0100 6406 6408 6c0c  d.l.m.Z...d.d.l.
@@ -126,17 +126,17 @@
 000007d0: 0000 0072 2300 0000 7224 0000 00da 0b73  ...r#...r$.....s
 000007e0: 6967 6e65 645f 706f 7374 5000 0000 7330  igned_postP...s0
 000007f0: 0000 0002 8016 0908 0206 0106 0104 0208  ................
 00000800: 0204 0106 0108 020a 0308 0108 0108 0108  ................
 00000810: 0102 fb08 0808 0108 0108 0108 0108 0108  ................
 00000820: 0116 0272 2b00 0000 2918 da07 6c6f 6767  ...r+...)...logg
 00000830: 696e 67da 0c75 726c 6c69 622e 7061 7273  ing..urllib.pars
-00000840: 6572 0200 0000 da07 6169 6f68 7474 70da  er......aiohttp.
+00000840: 6572 0200 0000 da07 6169 6f68 7474 705a  er......aiohttpZ
 00000850: 1462 6f76 696e 652e 6372 7970 746f 2e68  .bovine.crypto.h
-00000860: 656c 7065 7272 0300 0000 da1c 626f 7669  elperr......bovi
+00000860: 656c 7065 7272 0300 0000 5a1c 626f 7669  elperr....Z.bovi
 00000870: 6e65 2e63 7279 7074 6f2e 6874 7470 5f73  ne.crypto.http_s
 00000880: 6967 6e61 7475 7265 7204 0000 00da 1162  ignaturer......b
 00000890: 6f76 696e 652e 7574 696c 732e 6461 7465  ovine.utils.date
 000008a0: 7205 0000 00da 0663 6f6e 7374 7372 0700  r......constsr..
 000008b0: 0000 da0c 6576 656e 745f 736f 7572 6365  ....event_source
 000008c0: 7208 0000 00da 0967 6574 4c6f 6767 6572  r......getLogger
 000008d0: da08 5f5f 6e61 6d65 5f5f 7219 0000 00da  ..__name__r.....
```

### Comparing `bovine-0.1.1/bovine/clients/__pycache__/signed_http_client.cpython-310.pyc` & `bovine-0.1.2/bovine/clients/__pycache__/signed_http_client.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 1074 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 3204 0000  o.........:d2...
+00000000: 6f0d 0d0a 0000 0000 8013 4164 3204 0000  o.........Ad2...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 8302 5a02 6401 5300 2904 e900 0000 004e  ..Z.d.S.)......N
 00000050: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00000060: 0003 0000 0040 0000 0073 4000 0000 6500  .....@...s@...e.
 00000070: 5a01 6400 5a02 640c 6402 6403 8401 5a03  Z.d.Z.d.d.d...Z.
```

### Comparing `bovine-0.1.1/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.2/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 609 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 6102 0000  o.........:da...
+00000000: 6f0d 0d0a 0000 0000 8013 4164 6102 0000  o.........Ada...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 0100  Z...d.d.l.m.Z...
 00000060: 6408 6406 6407 8404 5a0a 6401 5300 2909  d.d.d...Z.d.S.).
 00000070: e900 0000 004e 2901 da09 4173 796e 634d  .....N)...AsyncM
```

### Comparing `bovine-0.1.1/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.2/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 624 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 7002 0000  o.........:dp...
+00000000: 6f0d 0d0a 0000 0000 8013 4164 7002 0000  o.........Adp...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 6d09 5a09 0100  d.d.l.m.Z.m.Z...
 00000060: 6404 6405 8400 5a0a 6406 6407 8400 5a0b  d.d...Z.d.d...Z.
 00000070: 6401 5300 2908 e900 0000 004e e901 0000  d.S.)......N....
```

### Comparing `bovine-0.1.1/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.2/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 319 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 3f01 0000  o.........:d?...
+00000000: 6f0d 0d0a 0000 0000 8013 4164 3f01 0000  o.........Ad?...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 0100 6404 6405  d.d.l.m.Z...d.d.
 00000060: 8400 5a09 6401 5300 2906 e900 0000 004e  ..Z.d.S.)......N
 00000070: e901 0000 0029 01da 0e66 6574 6368 5f6e  .....)...fetch_n
```

### Comparing `bovine-0.1.1/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.2/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 1145 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 7904 0000  o.........:dy...
+00000000: 6f0d 0d0a 0000 0000 8013 4164 7904 0000  o.........Ady...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 6d08 5a08 0100 6400 6401 6c09 5a09  Z.m.Z...d.d.l.Z.
 00000060: 6400 6403 6c0a 6d0b 5a0b 0100 6400 6404  d.d.l.m.Z...d.d.
 00000070: 6c0c 6d0d 5a0d 6d0e 5a0e 0100 6405 6406  l.m.Z.m.Z...d.d.
```

### Comparing `bovine-0.1.1/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.2/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 529 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 1102 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 1102 0000  o.........Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6400 6401 6c08 5a08 6400 6403  Z...d.d.l.Z.d.d.
 00000060: 6c09 6d0a 5a0a 0100 6404 6405 6c0b 6d0c  l.m.Z...d.d.l.m.
 00000070: 5a0c 0100 6406 6407 8400 5a0d 6401 5300  Z...d.d...Z.d.S.
```

### Comparing `bovine-0.1.1/bovine/clients/event_source.py` & `bovine-0.1.2/bovine/clients/event_source.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/clients/lookup_account.py` & `bovine-0.1.2/bovine/clients/lookup_account.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/clients/moo_auth_client.py` & `bovine-0.1.2/bovine/clients/moo_auth_client.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/clients/nodeinfo.py` & `bovine-0.1.2/bovine/clients/nodeinfo.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/clients/signed_http.py` & `bovine-0.1.2/bovine/clients/signed_http.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/clients/signed_http_client.py` & `bovine-0.1.2/bovine/clients/signed_http_client.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/clients/test_event_source.py` & `bovine-0.1.2/bovine/clients/test_event_source.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/clients/test_lookup_account.py` & `bovine-0.1.2/bovine/clients/test_lookup_account.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/clients/test_signed_http.py` & `bovine-0.1.2/bovine/clients/test_signed_http.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/clients/test_signed_http_client.py` & `bovine-0.1.2/bovine/clients/test_signed_http_client.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/crypto/__init__.py` & `bovine-0.1.2/bovine/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/crypto/__pycache__/__init__.cpython-310.pyc` & `bovine-0.1.2/bovine/crypto/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 3999 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 9f0f 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 9f0f 0000  o.........Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 c400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 6d07 5a07 0100 6400 6404 6c08  m.Z.m.Z...d.d.l.
 00000060: 6d09 5a09 6d0a 5a0a 0100 6400 6405 6c0b  m.Z.m.Z...d.d.l.
 00000070: 5a0b 6406 6407 6c0c 6d0d 5a0d 6d0e 5a0e  Z.d.d.l.m.Z.m.Z.
```

### Comparing `bovine-0.1.1/bovine/crypto/__pycache__/helper.cpython-310.pyc` & `bovine-0.1.2/bovine/crypto/__pycache__/helper.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 2664 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 680a 0000  o.........:dh...
+00000000: 6f0d 0d0a 0000 0000 8013 4164 680a 0000  o.........Adh...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 d800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6402 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 6d07 5a07  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6400 6404 6c08 6d09 5a09 6d0a 5a0a  ..d.d.l.m.Z.m.Z.
 00000070: 6d0b 5a0b 0100 6400 6405 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `bovine-0.1.1/bovine/crypto/__pycache__/http_signature.cpython-310.pyc` & `bovine-0.1.2/bovine/crypto/__pycache__/http_signature.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 2112 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 4008 0000  o.........:d@...
+00000000: 6f0d 0d0a 0000 0000 8013 4164 4008 0000  o.........Ad@...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 0100 6405  d.l.m.Z.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 0100 6500 a00c 650d a101 5a0e 6407 6408  ..e...e...Z.d.d.
```

### Comparing `bovine-0.1.1/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc` & `bovine-0.1.2/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 2942 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 7e0b 0000  o.........:d~...
+00000000: 6f0d 0d0a 0000 0000 8013 4164 7e0b 0000  o.........Ad~...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6401 6c04  d.l.m.Z...d.d.l.
 00000050: 5a05 6400 6403 6c04 6d06 5a06 0100 6404  Z.d.d.l.m.Z...d.
 00000060: 6405 6c07 6d08 5a08 0100 6404 6406 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6404 6407 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
```

### Comparing `bovine-0.1.1/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc` & `bovine-0.1.2/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 1266 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 f204 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 f204 0000  o.........Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 5a00 6500 a001 6502 a101 5a03  d.l.Z.e...e...Z.
 00000040: 4700 6402 6403 8400 6403 8302 5a04 6404  G.d.d...d...Z.d.
 00000050: 6405 8400 5a05 6401 5300 2906 e900 0000  d...Z.d.S.).....
 00000060: 004e 6300 0000 0000 0000 0000 0000 0000  .Nc.............
 00000070: 0000 0003 0000 0040 0000 0073 2800 0000  .......@...s(...
```

### Comparing `bovine-0.1.1/bovine/crypto/__pycache__/test.cpython-310.pyc` & `bovine-0.1.2/bovine/crypto/__pycache__/test.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 2199 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 9708 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 9708 0000  o.........Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0001 0000 0040 0000 0073 0c00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 5a01 6402 5300 2903 61c4 0100  Z.d.Z.d.S.).a...
 00000040: 000a 2d2d 2d2d 2d42 4547 494e 2050 5542  ..-----BEGIN PUB
 00000050: 4c49 4320 4b45 592d 2d2d 2d2d 0a4d 4949  LIC KEY-----.MII
 00000060: 4249 6a41 4e42 676b 7168 6b69 4739 7730  BIjANBgkqhkiG9w0
 00000070: 4241 5145 4641 414f 4341 5138 414d 4949  BAQEFAAOCAQ8AMII
```

### Comparing `bovine-0.1.1/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.2/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 4989 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 7d13 0000  o.........:d}...
+00000000: 6f0d 0d0a 0000 0000 8013 4164 7d13 0000  o.........Ad}...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 a600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 6d08 5a08 6d09 5a09 0100 6403 6404  Z.m.Z.m.Z...d.d.
 00000060: 6c0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e  l.m.Z.m.Z.m.Z.m.
 00000070: 5a0e 0100 6403 6405 6c0f 6d10 5a10 0100  Z...d.d.l.m.Z...
```

### Comparing `bovine-0.1.1/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.2/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 896 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 8003 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 8003 0000  o.........Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6403 6404 6c08 6d09 5a09 6d0a  Z...d.d.l.m.Z.m.
 00000060: 5a0a 6d0b 5a0b 6d0c 5a0c 0100 6403 6405  Z.m.Z.m.Z...d.d.
 00000070: 6c0d 6d0e 5a0e 6d0f 5a0f 0100 6406 6407  l.m.Z.m.Z...d.d.
```

### Comparing `bovine-0.1.1/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.2/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 5081 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 d913 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 d913 0000  o.........Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
 00000050: 6402 6403 6c07 6d08 5a08 0100 6402 6404  d.d.l.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 6d0b 5a0b 0100 6402 6405  l.m.Z.m.Z...d.d.
 00000070: 6c0c 6d0d 5a0d 0100 6406 6407 8400 5a0e  l.m.Z...d.d...Z.
```

### Comparing `bovine-0.1.1/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.2/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 1207 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 b704 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 b704 0000  o.........Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6404 6405 8400 5a08 6406 6407  Z...d.d...Z.d.d.
 00000060: 8400 5a09 6401 5300 2908 e900 0000 004e  ..Z.d.S.)......N
 00000070: e901 0000 0029 01da 0953 6967 6e61 7475  .....)...Signatu
```

### Comparing `bovine-0.1.1/bovine/crypto/helper.py` & `bovine-0.1.2/bovine/crypto/helper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/crypto/http_signature.py` & `bovine-0.1.2/bovine/crypto/http_signature.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/crypto/signature_checker.py` & `bovine-0.1.2/bovine/crypto/signature_checker.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/crypto/signature_parser.py` & `bovine-0.1.2/bovine/crypto/signature_parser.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/crypto/test.py` & `bovine-0.1.2/bovine/crypto/test.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/crypto/test_crypto.py` & `bovine-0.1.2/bovine/crypto/test_crypto.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/crypto/test_helper.py` & `bovine-0.1.2/bovine/crypto/test_helper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/crypto/test_http_signature.py` & `bovine-0.1.2/bovine/crypto/test_http_signature.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/crypto/test_signature_parser.py` & `bovine-0.1.2/bovine/crypto/test_signature_parser.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/types.py` & `bovine-0.1.2/bovine/types.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/utils/__init__.py` & `bovine-0.1.2/bovine/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/utils/__pycache__/__init__.cpython-310.pyc` & `bovine-0.1.2/bovine/utils/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 667 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 9b02 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 9b02 0000  o.........Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6402  d.l.m.Z.m.Z...d.
 00000040: 6503 6403 6503 6404 6503 6405 6504 6608  e.d.e.d.e.d.e.f.
 00000050: 6406 6407 8404 5a05 6408 6503 6405 6502  d.d...Z.d.e.d.e.
 00000060: 6503 6501 6503 1900 6602 1900 6604 6409  e.e.e...f...f.d.
 00000070: 640a 8404 5a06 640b 5300 290c e900 0000  d...Z.d.S.).....
```

### Comparing `bovine-0.1.1/bovine/utils/__pycache__/date.cpython-310.pyc` & `bovine-0.1.2/bovine/utils/__pycache__/date.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 519 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 0702 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 0702 0000  o.........Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 6d00 5a00 6d01 5a01 6d02 5a02  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c03 6d04 5a04 0100 6403  ..d.d.l.m.Z...d.
 00000050: 6505 6602 6404 6405 8404 5a06 6406 6505  e.f.d.d...Z.d.e.
 00000060: 6403 6500 6604 6407 6408 8404 5a07 640f  d.e.f.d.d...Z.d.
 00000070: 640a 6500 640b 6508 6403 6509 6606 640c  d.e.d.e.d.e.f.d.
```

### Comparing `bovine-0.1.1/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.2/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 737 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 e102 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 e102 0000  o.........Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6400 6402 6c06 6d06  ..m.Z...d.d.l.m.
 00000050: 5a06 6d07 5a07 6d08 5a08 0100 6403 6404  Z.m.Z.m.Z...d.d.
 00000060: 6c09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 0100  l.m.Z.m.Z.m.Z...
 00000070: 6405 6406 8400 5a0d 6407 6408 8400 5a0e  d.d...Z.d.d...Z.
```

### Comparing `bovine-0.1.1/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.2/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 452 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 c401 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 c401 0000  o.........Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6404 6405 8400 5a08 6401 5300  Z...d.d...Z.d.S.
 00000060: 2906 e900 0000 004e e901 0000 0029 01da  )......N.....)..
 00000070: 1670 6172 7365 5f66 6564 6976 6572 7365  .parse_fediverse
```

### Comparing `bovine-0.1.1/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.0.pyc` & `bovine-0.1.2/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.0.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Apr 15 18:19:16 2023 UTC, .py size: 191 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4ea 3a64 bf00 0000  o.........:d....
+00000000: 6f0d 0d0a 0000 0000 8013 4164 bf00 0000  o.........Ad....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
 00000040: 0100 6d04 5a05 0100 6402 6403 6c06 6d07  ..m.Z...d.d.l.m.
 00000050: 5a07 0100 6404 6405 8400 5a08 6401 5300  Z...d.d...Z.d.S.
 00000060: 2906 e900 0000 004e e901 0000 0029 01da  )......N.....)..
 00000070: 1777 6562 6669 6e67 6572 5f72 6573 706f  .webfinger_respo
```

### Comparing `bovine-0.1.1/bovine/utils/date.py` & `bovine-0.1.2/bovine/utils/date.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/bovine/utils/test_date.py` & `bovine-0.1.2/bovine/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `bovine-0.1.1/pyproject.toml` & `bovine-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bovine"
-version = "0.1.1"
+version = "0.1.2"
 description = "Core functionality of bovine needed to build FediVerse applications"
 authors = ["Helge <helge.krueger@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bovine" }]
 repository = "https://codeberg.org/bovine/bovine"
 documentation = "https://bovine.readthedocs.io/en/latest/"
@@ -24,27 +24,29 @@
 pytest-cov = "^4.0.0"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 mypy = "^0.991"
 types-python-dateutil = "^2.8.19.6"
 black = "*"
-flake8 = "*"
-flake8-black = "*"
 ptpython = "^3.0.23"
 jupyter = "^1.0.0"
-sphinx = "^6.1.3"
-sphinx-rtd-theme = "^1.2.0"
-sphinxcontrib-napoleon = "^0.7"
 rich = "^13.3.2"
-aiohttp = "^3.8.4"
 types-bleach = "^6.0.0.2"
 reload = "^0.9"
 quart = "^0.18.3"
 rdflib = "^6.3.2"
+ruff = "^0.0.261"
+
+[tool.poetry.group.doc.dependencies]
+sphinx = "^6.1.3"
+sphinx-rtd-theme = "^1.2.0"
+sphinxcontrib-napoleon = "^0.7"
+sphinx-argparse = "^0.4.0"
+
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 asyncio_mode="auto"
```

### Comparing `bovine-0.1.1/PKG-INFO` & `bovine-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bovine
-Version: 0.1.1
+Version: 0.1.2
 Summary: Core functionality of bovine needed to build FediVerse applications
 Home-page: https://codeberg.org/bovine/bovine
 License: MIT
 Author: Helge
 Author-email: helge.krueger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -27,11 +27,25 @@
 
 The bovine library can just be installed via pip
 
 ```bash
 pip install bovine
 ```
 
-Documentation including tutorials is available at [ReadTheDocs](https://bovine.readthedocs.io/en/latest/)
-
+Documentation including tutorials is available at [ReadTheDocs](https://bovine.readthedocs.io/en/latest/).
 An entire working ActivityPub server can be found in the [bovine repository](https://codeberg.org/bovine/bovine/).
 
+## Feedback
+
+Issues about bovine should be filed as an [issue](https://codeberg.org/bovine/bovine/issues).
+
+## Contributing
+
+If you want to contribute, you can start by working on issues labeled [Good first issue](https://codeberg.org/bovine/bovine/issues?q=&type=all&state=open&labels=110885&milestone=0&assignee=0&poster=0). The tech stack is currently based on asynchronous python, using the following components:
+
+- [aiohttp](https://docs.aiohttp.org/en/stable/index.html) for http requests.
+- [quart](https://quart.palletsprojects.com/en/latest/) as a webserver.
+- [cryptography](https://cryptography.io/en/latest/).
+- [pytest](https://docs.pytest.org/en/7.3.x/) for testing.
+- [ruff](https://pypi.org/project/ruff/) for linting.
+
+
```

