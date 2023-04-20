# Comparing `tmp/kui-1.3.6.tar.gz` & `tmp/kui-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kui-1.3.6.tar", last modified: Sun Feb 26 18:47:17 2023, max compression
+gzip compressed data, was "kui-1.3.7.tar", last modified: Thu Apr 20 06:02:16 2023, max compression
```

## Comparing `kui-1.3.6.tar` & `kui-1.3.7.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0    11341 2023-02-26 18:47:01.574059 kui-1.3.6/LICENSE
--rw-r--r--   0        0        0      440 2023-02-26 18:47:01.574059 kui-1.3.6/README.md
--rw-r--r--   0        0        0        0 2023-02-26 18:47:01.574059 kui-1.3.6/kui/__init__.py
--rw-r--r--   0        0        0       63 2023-02-26 18:47:01.574059 kui-1.3.6/kui/__version__.py
--rw-r--r--   0        0        0     1754 2023-02-26 18:47:01.574059 kui-1.3.6/kui/asgi/__init__.py
--rw-r--r--   0        0        0     8139 2023-02-26 18:47:01.574059 kui-1.3.6/kui/asgi/applications.py
--rw-r--r--   0        0        0     2090 2023-02-26 18:47:01.574059 kui-1.3.6/kui/asgi/cors.py
--rw-r--r--   0        0        0     2366 2023-02-26 18:47:01.574059 kui-1.3.6/kui/asgi/exceptions.py
--rw-r--r--   0        0        0     1470 2023-02-26 18:47:01.574059 kui-1.3.6/kui/asgi/openapi.py
--rw-r--r--   0        0        0     5502 2023-02-26 18:47:01.574059 kui-1.3.6/kui/asgi/parameters.py
--rw-r--r--   0        0        0     3754 2023-02-26 18:47:01.574059 kui-1.3.6/kui/asgi/requests.py
--rw-r--r--   0        0        0     2906 2023-02-26 18:47:01.574059 kui-1.3.6/kui/asgi/responses.py
--rw-r--r--   0        0        0      972 2023-02-26 18:47:01.574059 kui-1.3.6/kui/asgi/routing.py
--rw-r--r--   0        0        0     3177 2023-02-26 18:47:01.574059 kui-1.3.6/kui/asgi/templates.py
--rw-r--r--   0        0        0     4614 2023-02-26 18:47:01.574059 kui-1.3.6/kui/asgi/views.py
--rw-r--r--   0        0        0     3849 2023-02-26 18:47:01.574059 kui-1.3.6/kui/exceptions.py
--rw-r--r--   0        0        0      123 2023-02-26 18:47:01.574059 kui-1.3.6/kui/openapi/__init__.py
--rw-r--r--   0        0        0     9465 2023-02-26 18:47:01.574059 kui-1.3.6/kui/openapi/application.py
--rw-r--r--   0        0        0     1565 2023-02-26 18:47:01.574059 kui-1.3.6/kui/openapi/extra_docs.py
--rw-r--r--   0        0        0     1632 2023-02-26 18:47:01.574059 kui-1.3.6/kui/openapi/schema.py
--rw-r--r--   0        0        0     7726 2023-02-26 18:47:01.574059 kui-1.3.6/kui/openapi/specification.py
--rw-r--r--   0        0        0      224 2023-02-26 18:47:01.574059 kui-1.3.6/kui/openapi/templates/rapidoc.html
--rw-r--r--   0        0        0      743 2023-02-26 18:47:01.574059 kui-1.3.6/kui/openapi/templates/redoc.html
--rw-r--r--   0        0        0     1522 2023-02-26 18:47:01.574059 kui-1.3.6/kui/openapi/templates/swagger.html
--rw-r--r--   0        0        0      586 2023-02-26 18:47:01.574059 kui-1.3.6/kui/openapi/types.py
--rw-r--r--   0        0        0    15327 2023-02-26 18:47:01.574059 kui-1.3.6/kui/parameters/__init__.py
--rw-r--r--   0        0        0     9051 2023-02-26 18:47:01.574059 kui-1.3.6/kui/parameters/field_functions.py
--rw-r--r--   0        0        0     2219 2023-02-26 18:47:01.574059 kui-1.3.6/kui/parameters/fields.py
--rw-r--r--   0        0        0        0 2023-02-26 18:47:01.574059 kui-1.3.6/kui/py.typed
--rw-r--r--   0        0        0     7375 2023-02-26 18:47:01.574059 kui-1.3.6/kui/responses.py
--rw-r--r--   0        0        0      429 2023-02-26 18:47:01.574059 kui-1.3.6/kui/routing/__init__.py
--rw-r--r--   0        0        0       82 2023-02-26 18:47:01.574059 kui-1.3.6/kui/routing/__main__.py
--rw-r--r--   0        0        0     1402 2023-02-26 18:47:01.574059 kui-1.3.6/kui/routing/commands.py
--rw-r--r--   0        0        0      130 2023-02-26 18:47:01.574059 kui-1.3.6/kui/routing/extensions/__init__.py
--rw-r--r--   0        0        0     2551 2023-02-26 18:47:01.574059 kui-1.3.6/kui/routing/extensions/file.py
--rw-r--r--   0        0        0     2982 2023-02-26 18:47:01.578059 kui-1.3.6/kui/routing/extensions/multimethod.py
--rw-r--r--   0        0        0    17789 2023-02-26 18:47:01.578059 kui-1.3.6/kui/routing/routers.py
--rw-r--r--   0        0        0     3040 2023-02-26 18:47:01.578059 kui-1.3.6/kui/routing/routes.py
--rw-r--r--   0        0        0     6234 2023-02-26 18:47:01.578059 kui-1.3.6/kui/routing/tree.py
--rw-r--r--   0        0        0      273 2023-02-26 18:47:01.578059 kui-1.3.6/kui/routing/typing.py
--rw-r--r--   0        0        0     2538 2023-02-26 18:47:01.578059 kui-1.3.6/kui/security.py
--rw-r--r--   0        0        0     2783 2023-02-26 18:47:01.578059 kui-1.3.6/kui/status.py
--rw-r--r--   0        0        0     1250 2023-02-26 18:47:01.578059 kui-1.3.6/kui/templates.py
--rw-r--r--   0        0        0      757 2023-02-26 18:47:01.578059 kui-1.3.6/kui/utils/__init__.py
--rw-r--r--   0        0        0      856 2023-02-26 18:47:01.578059 kui-1.3.6/kui/utils/contextvars.py
--rw-r--r--   0        0        0     1576 2023-02-26 18:47:01.578059 kui-1.3.6/kui/utils/importer.py
--rw-r--r--   0        0        0     1907 2023-02-26 18:47:01.578059 kui-1.3.6/kui/utils/inspect.py
--rw-r--r--   0        0        0     1647 2023-02-26 18:47:01.578059 kui-1.3.6/kui/utils/objects.py
--rw-r--r--   0        0        0      530 2023-02-26 18:47:01.578059 kui-1.3.6/kui/utils/pipe.py
--rw-r--r--   0        0        0     1123 2023-02-26 18:47:01.578059 kui-1.3.6/kui/utils/state.py
--rw-r--r--   0        0        0     1603 2023-02-26 18:47:01.578059 kui-1.3.6/kui/wsgi/__init__.py
--rw-r--r--   0        0        0     5249 2023-02-26 18:47:01.578059 kui-1.3.6/kui/wsgi/applications.py
--rw-r--r--   0        0        0     2067 2023-02-26 18:47:01.578059 kui-1.3.6/kui/wsgi/cors.py
--rw-r--r--   0        0        0     2309 2023-02-26 18:47:01.578059 kui-1.3.6/kui/wsgi/exceptions.py
--rw-r--r--   0        0        0     1428 2023-02-26 18:47:01.578059 kui-1.3.6/kui/wsgi/openapi.py
--rw-r--r--   0        0        0     4204 2023-02-26 18:47:01.578059 kui-1.3.6/kui/wsgi/parameters.py
--rw-r--r--   0        0        0     1833 2023-02-26 18:47:01.578059 kui-1.3.6/kui/wsgi/requests.py
--rw-r--r--   0        0        0     2906 2023-02-26 18:47:01.578059 kui-1.3.6/kui/wsgi/responses.py
--rw-r--r--   0        0        0      966 2023-02-26 18:47:01.578059 kui-1.3.6/kui/wsgi/routing.py
--rw-r--r--   0        0        0     2884 2023-02-26 18:47:01.578059 kui-1.3.6/kui/wsgi/templates.py
--rw-r--r--   0        0        0     2281 2023-02-26 18:47:01.578059 kui-1.3.6/kui/wsgi/views.py
--rw-r--r--   0        0        0     2208 2023-02-26 18:47:01.578059 kui-1.3.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-26 18:47:01.578059 kui-1.3.6/tests/asgi/__init__.py
--rw-r--r--   0        0        0     2416 2023-02-26 18:47:01.578059 kui-1.3.6/tests/asgi/test_application.py
--rw-r--r--   0        0        0      689 2023-02-26 18:47:01.578059 kui-1.3.6/tests/asgi/test_cors.py
--rw-r--r--   0        0        0     7058 2023-02-26 18:47:01.578059 kui-1.3.6/tests/asgi/test_parameters.py
--rw-r--r--   0        0        0      535 2023-02-26 18:47:01.578059 kui-1.3.6/tests/asgi/test_views.py
--rw-r--r--   0        0        0    32402 2023-02-26 18:47:01.578059 kui-1.3.6/tests/openapi/test_application.py
--rw-r--r--   0        0        0      429 2023-02-26 18:47:01.578059 kui-1.3.6/tests/openapi/test_extra_docs.py
--rw-r--r--   0        0        0      247 2023-02-26 18:47:01.578059 kui-1.3.6/tests/routing/extensions/test_fileroutes.py
--rw-r--r--   0        0        0     3155 2023-02-26 18:47:01.578059 kui-1.3.6/tests/routing/extensions/test_multimethod.py
--rw-r--r--   0        0        0       88 2023-02-26 18:47:01.578059 kui-1.3.6/tests/routing/test_commands.py
--rw-r--r--   0        0        0     3788 2023-02-26 18:47:01.578059 kui-1.3.6/tests/routing/test_routes.py
--rw-r--r--   0        0        0     2444 2023-02-26 18:47:01.578059 kui-1.3.6/tests/routing/test_tree.py
--rw-r--r--   0        0        0      242 2023-02-26 18:47:01.578059 kui-1.3.6/tests/test_export_all.py
--rw-r--r--   0        0        0     4505 2023-02-26 18:47:01.578059 kui-1.3.6/tests/test_responses.py
--rw-r--r--   0        0        0     3032 2023-02-26 18:47:01.578059 kui-1.3.6/tests/test_security.py
--rw-r--r--   0        0        0        0 2023-02-26 18:47:01.578059 kui-1.3.6/tests/utils/__init__.py
--rw-r--r--   0        0        0      722 2023-02-26 18:47:01.578059 kui-1.3.6/tests/utils/test_importer.py
--rw-r--r--   0        0        0      170 2023-02-26 18:47:01.578059 kui-1.3.6/tests/utils/test_objects.py
--rw-r--r--   0        0        0      426 2023-02-26 18:47:01.578059 kui-1.3.6/tests/utils/test_state.py
--rw-r--r--   0        0        0      648 2023-02-26 18:47:01.578059 kui-1.3.6/tests/wsgi/test_cors.py
--rw-r--r--   0        0        0     6790 2023-02-26 18:47:01.578059 kui-1.3.6/tests/wsgi/test_parameters.py
--rw-r--r--   0        0        0      453 2023-02-26 18:47:01.578059 kui-1.3.6/tests/wsgi/test_views.py
--rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 kui-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-04-20 06:01:59.028175 kui-1.3.7/LICENSE
+-rw-r--r--   0        0        0      440 2023-04-20 06:01:59.028175 kui-1.3.7/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 06:01:59.032175 kui-1.3.7/kui/__init__.py
+-rw-r--r--   0        0        0       63 2023-04-20 06:01:59.032175 kui-1.3.7/kui/__version__.py
+-rw-r--r--   0        0        0     1754 2023-04-20 06:01:59.032175 kui-1.3.7/kui/asgi/__init__.py
+-rw-r--r--   0        0        0     8139 2023-04-20 06:01:59.032175 kui-1.3.7/kui/asgi/applications.py
+-rw-r--r--   0        0        0     2090 2023-04-20 06:01:59.032175 kui-1.3.7/kui/asgi/cors.py
+-rw-r--r--   0        0        0     2366 2023-04-20 06:01:59.032175 kui-1.3.7/kui/asgi/exceptions.py
+-rw-r--r--   0        0        0     1470 2023-04-20 06:01:59.032175 kui-1.3.7/kui/asgi/openapi.py
+-rw-r--r--   0        0        0     5502 2023-04-20 06:01:59.032175 kui-1.3.7/kui/asgi/parameters.py
+-rw-r--r--   0        0        0     3754 2023-04-20 06:01:59.032175 kui-1.3.7/kui/asgi/requests.py
+-rw-r--r--   0        0        0     2879 2023-04-20 06:01:59.032175 kui-1.3.7/kui/asgi/responses.py
+-rw-r--r--   0        0        0      972 2023-04-20 06:01:59.032175 kui-1.3.7/kui/asgi/routing.py
+-rw-r--r--   0        0        0     3177 2023-04-20 06:01:59.032175 kui-1.3.7/kui/asgi/templates.py
+-rw-r--r--   0        0        0     4614 2023-04-20 06:01:59.032175 kui-1.3.7/kui/asgi/views.py
+-rw-r--r--   0        0        0     3849 2023-04-20 06:01:59.032175 kui-1.3.7/kui/exceptions.py
+-rw-r--r--   0        0        0      123 2023-04-20 06:01:59.032175 kui-1.3.7/kui/openapi/__init__.py
+-rw-r--r--   0        0        0     9465 2023-04-20 06:01:59.032175 kui-1.3.7/kui/openapi/application.py
+-rw-r--r--   0        0        0     1565 2023-04-20 06:01:59.032175 kui-1.3.7/kui/openapi/extra_docs.py
+-rw-r--r--   0        0        0     1632 2023-04-20 06:01:59.032175 kui-1.3.7/kui/openapi/schema.py
+-rw-r--r--   0        0        0     7726 2023-04-20 06:01:59.032175 kui-1.3.7/kui/openapi/specification.py
+-rw-r--r--   0        0        0      224 2023-04-20 06:01:59.032175 kui-1.3.7/kui/openapi/templates/rapidoc.html
+-rw-r--r--   0        0        0      743 2023-04-20 06:01:59.032175 kui-1.3.7/kui/openapi/templates/redoc.html
+-rw-r--r--   0        0        0     1522 2023-04-20 06:01:59.032175 kui-1.3.7/kui/openapi/templates/swagger.html
+-rw-r--r--   0        0        0      586 2023-04-20 06:01:59.032175 kui-1.3.7/kui/openapi/types.py
+-rw-r--r--   0        0        0    15327 2023-04-20 06:01:59.032175 kui-1.3.7/kui/parameters/__init__.py
+-rw-r--r--   0        0        0     9051 2023-04-20 06:01:59.032175 kui-1.3.7/kui/parameters/field_functions.py
+-rw-r--r--   0        0        0     2219 2023-04-20 06:01:59.032175 kui-1.3.7/kui/parameters/fields.py
+-rw-r--r--   0        0        0        0 2023-04-20 06:01:59.032175 kui-1.3.7/kui/py.typed
+-rw-r--r--   0        0        0     7577 2023-04-20 06:01:59.032175 kui-1.3.7/kui/responses.py
+-rw-r--r--   0        0        0      429 2023-04-20 06:01:59.032175 kui-1.3.7/kui/routing/__init__.py
+-rw-r--r--   0        0        0       82 2023-04-20 06:01:59.032175 kui-1.3.7/kui/routing/__main__.py
+-rw-r--r--   0        0        0     1402 2023-04-20 06:01:59.032175 kui-1.3.7/kui/routing/commands.py
+-rw-r--r--   0        0        0      130 2023-04-20 06:01:59.032175 kui-1.3.7/kui/routing/extensions/__init__.py
+-rw-r--r--   0        0        0     2551 2023-04-20 06:01:59.032175 kui-1.3.7/kui/routing/extensions/file.py
+-rw-r--r--   0        0        0     2982 2023-04-20 06:01:59.032175 kui-1.3.7/kui/routing/extensions/multimethod.py
+-rw-r--r--   0        0        0    17789 2023-04-20 06:01:59.032175 kui-1.3.7/kui/routing/routers.py
+-rw-r--r--   0        0        0     3040 2023-04-20 06:01:59.032175 kui-1.3.7/kui/routing/routes.py
+-rw-r--r--   0        0        0     6234 2023-04-20 06:01:59.032175 kui-1.3.7/kui/routing/tree.py
+-rw-r--r--   0        0        0      273 2023-04-20 06:01:59.032175 kui-1.3.7/kui/routing/typing.py
+-rw-r--r--   0        0        0     2825 2023-04-20 06:01:59.032175 kui-1.3.7/kui/security.py
+-rw-r--r--   0        0        0     2783 2023-04-20 06:01:59.032175 kui-1.3.7/kui/status.py
+-rw-r--r--   0        0        0     1250 2023-04-20 06:01:59.032175 kui-1.3.7/kui/templates.py
+-rw-r--r--   0        0        0      757 2023-04-20 06:01:59.032175 kui-1.3.7/kui/utils/__init__.py
+-rw-r--r--   0        0        0      856 2023-04-20 06:01:59.032175 kui-1.3.7/kui/utils/contextvars.py
+-rw-r--r--   0        0        0     1576 2023-04-20 06:01:59.032175 kui-1.3.7/kui/utils/importer.py
+-rw-r--r--   0        0        0     1907 2023-04-20 06:01:59.032175 kui-1.3.7/kui/utils/inspect.py
+-rw-r--r--   0        0        0     1647 2023-04-20 06:01:59.032175 kui-1.3.7/kui/utils/objects.py
+-rw-r--r--   0        0        0      530 2023-04-20 06:01:59.032175 kui-1.3.7/kui/utils/pipe.py
+-rw-r--r--   0        0        0     1123 2023-04-20 06:01:59.032175 kui-1.3.7/kui/utils/state.py
+-rw-r--r--   0        0        0     1603 2023-04-20 06:01:59.032175 kui-1.3.7/kui/wsgi/__init__.py
+-rw-r--r--   0        0        0     5249 2023-04-20 06:01:59.032175 kui-1.3.7/kui/wsgi/applications.py
+-rw-r--r--   0        0        0     2067 2023-04-20 06:01:59.032175 kui-1.3.7/kui/wsgi/cors.py
+-rw-r--r--   0        0        0     2309 2023-04-20 06:01:59.032175 kui-1.3.7/kui/wsgi/exceptions.py
+-rw-r--r--   0        0        0     1428 2023-04-20 06:01:59.032175 kui-1.3.7/kui/wsgi/openapi.py
+-rw-r--r--   0        0        0     4204 2023-04-20 06:01:59.032175 kui-1.3.7/kui/wsgi/parameters.py
+-rw-r--r--   0        0        0     1833 2023-04-20 06:01:59.032175 kui-1.3.7/kui/wsgi/requests.py
+-rw-r--r--   0        0        0     2879 2023-04-20 06:01:59.032175 kui-1.3.7/kui/wsgi/responses.py
+-rw-r--r--   0        0        0      966 2023-04-20 06:01:59.032175 kui-1.3.7/kui/wsgi/routing.py
+-rw-r--r--   0        0        0     2884 2023-04-20 06:01:59.032175 kui-1.3.7/kui/wsgi/templates.py
+-rw-r--r--   0        0        0     2281 2023-04-20 06:01:59.032175 kui-1.3.7/kui/wsgi/views.py
+-rw-r--r--   0        0        0     2208 2023-04-20 06:01:59.036175 kui-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-20 06:01:59.036175 kui-1.3.7/tests/asgi/__init__.py
+-rw-r--r--   0        0        0     2416 2023-04-20 06:01:59.036175 kui-1.3.7/tests/asgi/test_application.py
+-rw-r--r--   0        0        0      689 2023-04-20 06:01:59.036175 kui-1.3.7/tests/asgi/test_cors.py
+-rw-r--r--   0        0        0     7058 2023-04-20 06:01:59.036175 kui-1.3.7/tests/asgi/test_parameters.py
+-rw-r--r--   0        0        0      535 2023-04-20 06:01:59.036175 kui-1.3.7/tests/asgi/test_views.py
+-rw-r--r--   0        0        0    32402 2023-04-20 06:01:59.036175 kui-1.3.7/tests/openapi/test_application.py
+-rw-r--r--   0        0        0      429 2023-04-20 06:01:59.036175 kui-1.3.7/tests/openapi/test_extra_docs.py
+-rw-r--r--   0        0        0      247 2023-04-20 06:01:59.036175 kui-1.3.7/tests/routing/extensions/test_fileroutes.py
+-rw-r--r--   0        0        0     3155 2023-04-20 06:01:59.036175 kui-1.3.7/tests/routing/extensions/test_multimethod.py
+-rw-r--r--   0        0        0       88 2023-04-20 06:01:59.036175 kui-1.3.7/tests/routing/test_commands.py
+-rw-r--r--   0        0        0     3788 2023-04-20 06:01:59.036175 kui-1.3.7/tests/routing/test_routes.py
+-rw-r--r--   0        0        0     2444 2023-04-20 06:01:59.036175 kui-1.3.7/tests/routing/test_tree.py
+-rw-r--r--   0        0        0      242 2023-04-20 06:01:59.036175 kui-1.3.7/tests/test_export_all.py
+-rw-r--r--   0        0        0     4505 2023-04-20 06:01:59.036175 kui-1.3.7/tests/test_responses.py
+-rw-r--r--   0        0        0     3032 2023-04-20 06:01:59.036175 kui-1.3.7/tests/test_security.py
+-rw-r--r--   0        0        0        0 2023-04-20 06:01:59.036175 kui-1.3.7/tests/utils/__init__.py
+-rw-r--r--   0        0        0      722 2023-04-20 06:01:59.036175 kui-1.3.7/tests/utils/test_importer.py
+-rw-r--r--   0        0        0      170 2023-04-20 06:01:59.036175 kui-1.3.7/tests/utils/test_objects.py
+-rw-r--r--   0        0        0      426 2023-04-20 06:01:59.036175 kui-1.3.7/tests/utils/test_state.py
+-rw-r--r--   0        0        0      648 2023-04-20 06:01:59.036175 kui-1.3.7/tests/wsgi/test_cors.py
+-rw-r--r--   0        0        0     6790 2023-04-20 06:01:59.036175 kui-1.3.7/tests/wsgi/test_parameters.py
+-rw-r--r--   0        0        0      453 2023-04-20 06:01:59.036175 kui-1.3.7/tests/wsgi/test_views.py
+-rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 kui-1.3.7/PKG-INFO
```

### Comparing `kui-1.3.6/LICENSE` & `kui-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/asgi/__init__.py` & `kui-1.3.7/kui/asgi/__init__.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/asgi/applications.py` & `kui-1.3.7/kui/asgi/applications.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/asgi/cors.py` & `kui-1.3.7/kui/asgi/cors.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/asgi/exceptions.py` & `kui-1.3.7/kui/asgi/exceptions.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/asgi/openapi.py` & `kui-1.3.7/kui/asgi/openapi.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/asgi/parameters.py` & `kui-1.3.7/kui/asgi/parameters.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/asgi/requests.py` & `kui-1.3.7/kui/asgi/requests.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/asgi/responses.py` & `kui-1.3.7/kui/asgi/responses.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 import typing
 
 from baize import asgi as baize_asgi
 from baize.typing import ServerSentEvent
-from pydantic.json import pydantic_encoder
 
 from ..responses import (
     FileResponseMixin,
     HTMLResponseMixin,
     JSONResponseMixin,
     PlainTextResponseMixin,
     RedirectResponseMixin,
     SendEventResponseMixin,
     StreamResponseMixin,
+    _json_encoder,
 )
 from .requests import request
 
 __all__ = [
     "convert_response",
     "HttpResponse",
     "FileResponse",
@@ -39,15 +39,15 @@
         self,
         content: typing.Any,
         status_code: int = 200,
         headers: typing.Optional[typing.Mapping[str, str]] = None,
         **kwargs: typing.Any,
     ) -> None:
         json_kwargs: typing.Dict[str, typing.Any] = {
-            "default": pydantic_encoder,
+            "default": _json_encoder,
         }
         json_kwargs.update(**kwargs)
         super().__init__(
             content, status_code=status_code, headers=headers, **json_kwargs
         )
```

### Comparing `kui-1.3.6/kui/asgi/routing.py` & `kui-1.3.7/kui/asgi/routing.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/asgi/templates.py` & `kui-1.3.7/kui/asgi/templates.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/asgi/views.py` & `kui-1.3.7/kui/asgi/views.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/exceptions.py` & `kui-1.3.7/kui/exceptions.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/openapi/application.py` & `kui-1.3.7/kui/openapi/application.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/openapi/extra_docs.py` & `kui-1.3.7/kui/openapi/extra_docs.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/openapi/schema.py` & `kui-1.3.7/kui/openapi/schema.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/openapi/specification.py` & `kui-1.3.7/kui/openapi/specification.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/openapi/templates/redoc.html` & `kui-1.3.7/kui/openapi/templates/redoc.html`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/openapi/templates/swagger.html` & `kui-1.3.7/kui/openapi/templates/swagger.html`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/openapi/types.py` & `kui-1.3.7/kui/openapi/types.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/parameters/__init__.py` & `kui-1.3.7/kui/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/parameters/field_functions.py` & `kui-1.3.7/kui/parameters/field_functions.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/parameters/fields.py` & `kui-1.3.7/kui/parameters/fields.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/responses.py` & `kui-1.3.7/kui/responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 from __future__ import annotations
 
 import typing
 from http import HTTPStatus
 
 from pydantic import BaseModel, create_model
+from pydantic.json import pydantic_encoder
 from pydantic.typing import display_as_type
 
 from .openapi import specification as spec
 from .utils import safe_issubclass
 
 
+def _json_encoder(obj: typing.Any) -> typing.Any:
+    if isinstance(obj, BaseModel):
+        return obj.dict(by_alias=True)
+    return pydantic_encoder(obj)
+
+
 class JSONResponseMixin:
     def __class_getitem__(
         cls,
         parameters: typing.Tuple[
             int,
             typing.Dict[str, spec.Header | spec.Reference],
             typing.Type[BaseModel] | spec.Schema | type,
```

### Comparing `kui-1.3.6/kui/routing/commands.py` & `kui-1.3.7/kui/routing/commands.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/routing/extensions/file.py` & `kui-1.3.7/kui/routing/extensions/file.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/routing/extensions/multimethod.py` & `kui-1.3.7/kui/routing/extensions/multimethod.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/routing/routers.py` & `kui-1.3.7/kui/routing/routers.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/routing/routes.py` & `kui-1.3.7/kui/routing/routes.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/routing/tree.py` & `kui-1.3.7/kui/routing/tree.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/security.py` & `kui-1.3.7/kui/security.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,21 @@
     Bearer token authentication.
     """
     if authorization is None:
         raise HTTPException(
             401,
             headers={"WWW-Authenticate": "Bearer"},
         )
-    type, token = authorization.strip().split(" ", maxsplit=1)
+    try:
+        type, token = authorization.strip().split(" ", maxsplit=1)
+    except ValueError:
+        raise HTTPException(
+            401,
+            headers={"WWW-Authenticate": "Bearer"},
+        )
     if type != "Bearer":
         raise HTTPException(
             401,
             headers={"WWW-Authenticate": "Bearer"},
         )
     return token
 
@@ -69,15 +75,21 @@
     Basic authentication.
     """
     if authorization is None:
         raise HTTPException(
             401,
             headers={"WWW-Authenticate": "Basic"},
         )
-    type, token = authorization.strip().split(" ", maxsplit=1)
+    try:
+        type, token = authorization.strip().split(" ", maxsplit=1)
+    except ValueError:
+        raise HTTPException(
+            401,
+            headers={"WWW-Authenticate": "Basic"},
+        )
     if type != "Basic":
         raise HTTPException(
             401,
             headers={"WWW-Authenticate": "Basic"},
         )
     username, password = base64.b64decode(token).decode("utf8").split(":")
     return username, password
```

### Comparing `kui-1.3.6/kui/status.py` & `kui-1.3.7/kui/status.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/templates.py` & `kui-1.3.7/kui/templates.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/utils/__init__.py` & `kui-1.3.7/kui/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/utils/contextvars.py` & `kui-1.3.7/kui/utils/contextvars.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/utils/importer.py` & `kui-1.3.7/kui/utils/importer.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/utils/inspect.py` & `kui-1.3.7/kui/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/utils/objects.py` & `kui-1.3.7/kui/utils/objects.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/utils/pipe.py` & `kui-1.3.7/kui/utils/pipe.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/utils/state.py` & `kui-1.3.7/kui/utils/state.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/wsgi/__init__.py` & `kui-1.3.7/kui/wsgi/__init__.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/wsgi/applications.py` & `kui-1.3.7/kui/wsgi/applications.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/wsgi/cors.py` & `kui-1.3.7/kui/wsgi/cors.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/wsgi/exceptions.py` & `kui-1.3.7/kui/wsgi/exceptions.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/wsgi/openapi.py` & `kui-1.3.7/kui/wsgi/openapi.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/wsgi/parameters.py` & `kui-1.3.7/kui/wsgi/parameters.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/wsgi/requests.py` & `kui-1.3.7/kui/wsgi/requests.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/wsgi/responses.py` & `kui-1.3.7/kui/wsgi/responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from __future__ import annotations
 
 import typing
 
 from baize import wsgi as baize_wsgi
 from baize.typing import ServerSentEvent
-from pydantic.json import pydantic_encoder
 
 from ..responses import (
     FileResponseMixin,
     HTMLResponseMixin,
     JSONResponseMixin,
     PlainTextResponseMixin,
     RedirectResponseMixin,
     SendEventResponseMixin,
     StreamResponseMixin,
+    _json_encoder,
 )
 from .requests import request
 
 __all__ = [
     "convert_response",
     "HttpResponse",
     "FileResponse",
@@ -39,15 +39,15 @@
         self,
         content: typing.Any,
         status_code: int = 200,
         headers: typing.Optional[typing.Mapping[str, str]] = None,
         **kwargs: typing.Any,
     ) -> None:
         json_kwargs: typing.Dict[str, typing.Any] = {
-            "default": pydantic_encoder,
+            "default": _json_encoder,
         }
         json_kwargs.update(**kwargs)
         super().__init__(
             content, status_code=status_code, headers=headers, **json_kwargs
         )
```

### Comparing `kui-1.3.6/kui/wsgi/routing.py` & `kui-1.3.7/kui/wsgi/routing.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/wsgi/templates.py` & `kui-1.3.7/kui/wsgi/templates.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/kui/wsgi/views.py` & `kui-1.3.7/kui/wsgi/views.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/pyproject.toml` & `kui-1.3.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kui"
-version = "1.3.6"
+version = "1.3.7"
 description = "An easy-to-use web framework."
 authors = [
     { name = "abersheeran", email = "me@abersheeran.com" },
 ]
 dependencies = [
     "baize<0.21.0,>=0.20.0",
     "pydantic<2.0,>=1.8",
```

### Comparing `kui-1.3.6/tests/asgi/test_application.py` & `kui-1.3.7/tests/asgi/test_application.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/tests/asgi/test_cors.py` & `kui-1.3.7/tests/asgi/test_cors.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/tests/asgi/test_parameters.py` & `kui-1.3.7/tests/asgi/test_parameters.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/tests/asgi/test_views.py` & `kui-1.3.7/tests/asgi/test_views.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/tests/openapi/test_application.py` & `kui-1.3.7/tests/openapi/test_application.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/tests/routing/extensions/test_multimethod.py` & `kui-1.3.7/tests/routing/extensions/test_multimethod.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/tests/routing/test_routes.py` & `kui-1.3.7/tests/routing/test_routes.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/tests/routing/test_tree.py` & `kui-1.3.7/tests/routing/test_tree.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/tests/test_responses.py` & `kui-1.3.7/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/tests/test_security.py` & `kui-1.3.7/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/tests/utils/test_importer.py` & `kui-1.3.7/tests/utils/test_importer.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/tests/wsgi/test_cors.py` & `kui-1.3.7/tests/wsgi/test_cors.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/tests/wsgi/test_parameters.py` & `kui-1.3.7/tests/wsgi/test_parameters.py`

 * *Files identical despite different names*

### Comparing `kui-1.3.6/PKG-INFO` & `kui-1.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kui
-Version: 1.3.6
+Version: 1.3.7
 Summary: An easy-to-use web framework.
 License: Apache-2.0
 Author-email: abersheeran <me@abersheeran.com>
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

