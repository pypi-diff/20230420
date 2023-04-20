# Comparing `tmp/robotframework_openapi_libcore-1.8.4.tar.gz` & `tmp/robotframework_openapi_libcore-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_openapi_libcore-1.8.4.tar", max compression
+gzip compressed data, was "robotframework_openapi_libcore-1.8.5.tar", max compression
```

## Comparing `robotframework_openapi_libcore-1.8.4.tar` & `robotframework_openapi_libcore-1.8.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     4693 2023-04-19 12:51:32.901466 robotframework_openapi_libcore-1.8.4/docs/README.md
--rw-r--r--   0        0        0    11558 2021-12-13 14:33:13.481598 robotframework_openapi_libcore-1.8.4/LICENSE
--rw-r--r--   0        0        0     2345 2023-04-19 11:35:09.393682 robotframework_openapi_libcore-1.8.4/pyproject.toml
--rw-r--r--   0        0        0     1297 2021-12-28 14:18:06.991167 robotframework_openapi_libcore-1.8.4/src/OpenApiLibCore/__init__.py
--rw-r--r--   0        0        0     8014 2023-02-17 14:58:53.541795 robotframework_openapi_libcore-1.8.4/src/OpenApiLibCore/dto_base.py
--rw-r--r--   0        0        0     2659 2023-02-17 14:58:53.542831 robotframework_openapi_libcore-1.8.4/src/OpenApiLibCore/dto_utils.py
--rw-r--r--   0        0        0      163 2023-04-19 06:55:56.561449 robotframework_openapi_libcore-1.8.4/src/OpenApiLibCore/oas_cache.py
--rw-r--r--   0        0        0    24298 2023-04-19 12:51:32.827552 robotframework_openapi_libcore-1.8.4/src/OpenApiLibCore/openapi_libcore.libspec
--rw-r--r--   0        0        0    59264 2023-04-19 12:11:03.596357 robotframework_openapi_libcore-1.8.4/src/OpenApiLibCore/openapi_libcore.py
--rw-r--r--   0        0        0    14713 2023-02-17 14:58:53.548382 robotframework_openapi_libcore-1.8.4/src/OpenApiLibCore/value_utils.py
--rw-r--r--   0        0        0     5656 1970-01-01 00:00:00.000000 robotframework_openapi_libcore-1.8.4/setup.py
--rw-r--r--   0        0        0     5867 1970-01-01 00:00:00.000000 robotframework_openapi_libcore-1.8.4/PKG-INFO
+-rw-r--r--   0        0        0     4693 2023-04-20 08:42:44.492938 robotframework_openapi_libcore-1.8.5/docs/README.md
+-rw-r--r--   0        0        0    11558 2021-12-13 14:33:13.481598 robotframework_openapi_libcore-1.8.5/LICENSE
+-rw-r--r--   0        0        0     2345 2023-04-20 08:33:33.956737 robotframework_openapi_libcore-1.8.5/pyproject.toml
+-rw-r--r--   0        0        0     1297 2021-12-28 14:18:06.991167 robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/__init__.py
+-rw-r--r--   0        0        0     8014 2023-02-17 14:58:53.541795 robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/dto_base.py
+-rw-r--r--   0        0        0     2659 2023-02-17 14:58:53.542831 robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/dto_utils.py
+-rw-r--r--   0        0        0      163 2023-04-20 07:55:08.986947 robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/oas_cache.py
+-rw-r--r--   0        0        0    24298 2023-04-20 08:42:44.415026 robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/openapi_libcore.libspec
+-rw-r--r--   0        0        0    59158 2023-04-20 08:42:16.575425 robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/openapi_libcore.py
+-rw-r--r--   0        0        0    14713 2023-02-17 14:58:53.548382 robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/value_utils.py
+-rw-r--r--   0        0        0     5656 1970-01-01 00:00:00.000000 robotframework_openapi_libcore-1.8.5/setup.py
+-rw-r--r--   0        0        0     5867 1970-01-01 00:00:00.000000 robotframework_openapi_libcore-1.8.5/PKG-INFO
```

### Comparing `robotframework_openapi_libcore-1.8.4/docs/README.md` & `robotframework_openapi_libcore-1.8.5/docs/README.md`

 * *Files identical despite different names*

### Comparing `robotframework_openapi_libcore-1.8.4/LICENSE` & `robotframework_openapi_libcore-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_openapi_libcore-1.8.4/pyproject.toml` & `robotframework_openapi_libcore-1.8.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="robotframework-openapi-libcore"
-version = "1.8.4"
+version = "1.8.5"
 description = "A Robot Framework library to facilitate library development for OpenAPI / Swagger APIs."
 license = "Apache-2.0"
 authors = ["Robin Mackaij <r.a.mackaij@gmail.com>"]
 maintainers = ["Robin Mackaij <r.a.mackaij@gmail.com>"]
 readme =  "./docs/README.md"
 homepage = "https://github.com/MarketSquare/robotframework-openapi-libcore"
 classifiers = [
```

### Comparing `robotframework_openapi_libcore-1.8.4/src/OpenApiLibCore/__init__.py` & `robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapi_libcore-1.8.4/src/OpenApiLibCore/dto_base.py` & `robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/dto_base.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapi_libcore-1.8.4/src/OpenApiLibCore/dto_utils.py` & `robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/dto_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapi_libcore-1.8.4/src/OpenApiLibCore/openapi_libcore.libspec` & `robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/openapi_libcore.libspec`

 * *Files 0% similar despite different names*

#### Comparing `robotframework_openapi_libcore-1.8.4/src/OpenApiLibCore/openapi_libcore.libspec` & `robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/openapi_libcore.libspec`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
-<keywordspec name="OpenApiLibCore" type="LIBRARY" format="HTML" scope="SUITE" generated="2023-04-19T12:51:33+00:00" specversion="4" source="C:\GitHub\robotframework-openapi-libcore\src\OpenApiLibCore\openapi_libcore.py" lineno="380">
-  <version>1.8.4</version>
+<keywordspec name="OpenApiLibCore" type="LIBRARY" format="HTML" scope="SUITE" generated="2023-04-20T08:42:44+00:00" specversion="4" source="C:\GitHub\robotframework-openapi-libcore\src\OpenApiLibCore\openapi_libcore.py" lineno="380">
+  <version>1.8.5</version>
   <doc>&lt;p&gt;Main class providing the keywords and core logic to interact with an OpenAPI server.&lt;/p&gt;
 &lt;p&gt;Visit the &lt;a href=&quot;https://github.com/MarketSquare/robotframework-openapi-libcore&quot;&gt;library page&lt;/a&gt; for an introduction.&lt;/p&gt;</doc>
   <tags/>
   <inits>
     <init name="__init__" lineno="388">
       <arguments repr="source: str, origin: str = , base_path: str = , mappings_path: str | Path = , username: str = , password: str = , security_token: str = , auth: AuthBase | None = None, cert: str | Tuple[str, str] | None = None, extra_headers: Dict[str, str] | None = None, invalid_property_default_response: int = 422, recursion_limit: int = 1, recursion_default: Any = {}, faker_locale: str | List[str] | None = None, default_id_property_name: str = id">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="source: str">
@@ -120,15 +120,15 @@
 &lt;h4&gt;default_id_property_name&lt;/h4&gt;
 &lt;p&gt;The default name for the property that identifies a resource (i.e. a unique entiry) within the API. The default value for this property name is &lt;span class=&quot;name&quot;&gt;id&lt;/span&gt;. If the target API uses a different name for all the resources within the API, you can configure it globally using this property.&lt;/p&gt;
 &lt;p&gt;If different property names are used for the unique identifier for different types of resources, an &lt;span class=&quot;name&quot;&gt;ID_MAPPING&lt;/span&gt; can be implemented in the &lt;span class=&quot;name&quot;&gt;mappings_path&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>=== source === An absolute path to an openapi.json or openapi.yaml file or an url to such a file.</shortdoc>
     </init>
   </inits>
   <keywords>
-    <kw name="Authorized Request" lineno="1363">
+    <kw name="Authorized Request" lineno="1360">
       <arguments repr="url: str, method: str, params: Dict[str, Any] | None = None, headers: Dict[str, str] | None = None, json_data: Dict[str, Any] | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -153,39 +153,39 @@
           <default>None</default>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Perform a request using the security token or authentication set in the library.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: provided username / password or auth objects take precedence over token based security&lt;/p&gt;</doc>
       <shortdoc>Perform a request using the security token or authentication set in the library.</shortdoc>
     </kw>
-    <kw name="Ensure In Use" lineno="1267">
+    <kw name="Ensure In Use" lineno="1264">
       <arguments repr="url: str, resource_relation: IdReference">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="resource_relation: IdReference">
           <name>resource_relation</name>
           <type>IdReference</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Ensure that the (right-most) &lt;span class=&quot;name&quot;&gt;id&lt;/span&gt; of the resource referenced by the &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt; is used by the resource defined by the &lt;span class=&quot;name&quot;&gt;resource_relation&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Ensure that the (right-most) `id` of the resource referenced by the `url` is used by the resource defined by the `resource_relation`.</shortdoc>
     </kw>
-    <kw name="Get Ids From Url" lineno="702">
+    <kw name="Get Ids From Url" lineno="699">
       <arguments repr="url: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Perform a GET request on the &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt; and return the list of resource &lt;span class=&quot;name&quot;&gt;ids&lt;/span&gt; from the response.&lt;/p&gt;</doc>
       <shortdoc>Perform a GET request on the `url` and return the list of resource `ids` from the response.</shortdoc>
     </kw>
-    <kw name="Get Invalid Json Data" lineno="1046">
+    <kw name="Get Invalid Json Data" lineno="1043">
       <arguments repr="url: str, method: str, status_code: int, request_data: RequestData">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -200,40 +200,40 @@
           <type>RequestData</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return &lt;span class=&quot;name&quot;&gt;json_data&lt;/span&gt; based on the &lt;span class=&quot;name&quot;&gt;dto&lt;/span&gt; on the &lt;span class=&quot;name&quot;&gt;request_data&lt;/span&gt; that will cause the provided &lt;span class=&quot;name&quot;&gt;status_code&lt;/span&gt; for the &lt;span class=&quot;name&quot;&gt;method&lt;/span&gt; operation on the &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt;.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: applicable UniquePropertyValueConstraint and IdReference Relations are considered before changes to &lt;span class=&quot;name&quot;&gt;json_data&lt;/span&gt; are made.&lt;/p&gt;</doc>
       <shortdoc>Return `json_data` based on the `dto` on the `request_data` that will cause the provided `status_code` for the `method` operation on the `url`.</shortdoc>
     </kw>
-    <kw name="Get Invalidated Parameters" lineno="1094">
+    <kw name="Get Invalidated Parameters" lineno="1091">
       <arguments repr="status_code: int, request_data: RequestData">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="status_code: int">
           <name>status_code</name>
           <type typedoc="integer">int</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="request_data: RequestData">
           <name>request_data</name>
           <type>RequestData</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Returns a version of &lt;span class=&quot;name&quot;&gt;params, headers&lt;/span&gt; as present on &lt;span class=&quot;name&quot;&gt;request_data&lt;/span&gt; that has been modified to cause the provided &lt;span class=&quot;name&quot;&gt;status_code&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Returns a version of `params, headers` as present on `request_data` that has been modified to cause the provided `status_code`.</shortdoc>
     </kw>
-    <kw name="Get Invalidated Url" lineno="1012">
+    <kw name="Get Invalidated Url" lineno="1009">
       <arguments repr="valid_url: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="valid_url: str">
           <name>valid_url</name>
           <type typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return an url with all the path parameters in the &lt;span class=&quot;name&quot;&gt;valid_url&lt;/span&gt; replaced by a random UUID.&lt;/p&gt;
 &lt;p&gt;Raises ValueError if the valid_url cannot be invalidated.&lt;/p&gt;</doc>
       <shortdoc>Return an url with all the path parameters in the `valid_url` replaced by a random UUID.</shortdoc>
     </kw>
-    <kw name="Get Json Data For Dto Class" lineno="922">
+    <kw name="Get Json Data For Dto Class" lineno="919">
       <arguments repr="schema: Dict[str, Any], dto_class: Dto | Type[Dto], operation_id: str = ">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="schema: Dict[str, Any]">
           <name>schema</name>
           <type typedoc="dictionary">Dict[str, Any]</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="dto_class: Dto | Type[Dto]">
           <name>dto_class</name>
@@ -245,15 +245,15 @@
           <type typedoc="string">str</type>
           <default/>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Generate a valid (json-compatible) dict for all the &lt;span class=&quot;name&quot;&gt;dto_class&lt;/span&gt; properties.&lt;/p&gt;</doc>
       <shortdoc>Generate a valid (json-compatible) dict for all the `dto_class` properties.</shortdoc>
     </kw>
-    <kw name="Get Json Data With Conflict" lineno="1311">
+    <kw name="Get Json Data With Conflict" lineno="1308">
       <arguments repr="url: str, method: str, dto: Dto, conflict_status_code: int">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -267,25 +267,25 @@
           <name>conflict_status_code</name>
           <type typedoc="integer">int</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return &lt;span class=&quot;name&quot;&gt;json_data&lt;/span&gt; based on the &lt;span class=&quot;name&quot;&gt;UniquePropertyValueConstraint&lt;/span&gt; that must be returned by the &lt;span class=&quot;name&quot;&gt;get_relations&lt;/span&gt; implementation on the &lt;span class=&quot;name&quot;&gt;dto&lt;/span&gt; for the given &lt;span class=&quot;name&quot;&gt;conflict_status_code&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Return `json_data` based on the `UniquePropertyValueConstraint` that must be returned by the `get_relations` implementation on the `dto` for the given `conflict_status_code`.</shortdoc>
     </kw>
-    <kw name="Get Parameterized Endpoint From Url" lineno="1034">
+    <kw name="Get Parameterized Endpoint From Url" lineno="1031">
       <arguments repr="url: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return the endpoint as found in the &lt;span class=&quot;name&quot;&gt;paths&lt;/span&gt; section based on the given &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Return the endpoint as found in the `paths` section based on the given `url`.</shortdoc>
     </kw>
-    <kw name="Get Request Data" lineno="742">
+    <kw name="Get Request Data" lineno="739">
       <arguments repr="endpoint: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="endpoint: str">
           <name>endpoint</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
```

### Comparing `robotframework_openapi_libcore-1.8.4/src/OpenApiLibCore/openapi_libcore.py` & `robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/openapi_libcore.py`

 * *Files 0% similar despite different names*

```diff
@@ -636,28 +636,25 @@
             id_property = mapping
             # set the transformer to a dummy callable that returns the original value so
             # the transformer can be applied on any returned id
             id_transformer = lambda x: x
         else:
             id_property, id_transformer = mapping
 
-        if response.status_code == 405:
-            # For endpoints that do no support POST, try to get an existing id using GET
+        if not response.ok:
+            # If a new resource cannot be created using POST, try to retrieve a
+            # valid id using a GET request.
             try:
                 valid_id = choice(run_keyword("get_ids_from_url", url))
                 return id_transformer(valid_id)
             except Exception as exception:
                 raise AssertionError(
                     f"Failed to get a valid id using GET on {url}"
                 ) from exception
 
-        assert (
-            response.ok
-        ), f"get_valid_id_for_endpoint received status_code {response.status_code}"
-
         response_data = response.json()
         if prepared_body := response.request.body:
             if isinstance(prepared_body, bytes):
                 send_json = _json.loads(prepared_body.decode("UTF-8"))
             else:
                 send_json = _json.loads(prepared_body)
         else:
```

### Comparing `robotframework_openapi_libcore-1.8.4/src/OpenApiLibCore/value_utils.py` & `robotframework_openapi_libcore-1.8.5/src/OpenApiLibCore/value_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapi_libcore-1.8.4/setup.py` & `robotframework_openapi_libcore-1.8.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'prance[cli]>=0.22,<0.23',
  'requests>=2.27,<3.0',
  'robotframework>=4',
  'rstr>=3,<4']
 
 setup_kwargs = {
     'name': 'robotframework-openapi-libcore',
-    'version': '1.8.4',
+    'version': '1.8.5',
     'description': 'A Robot Framework library to facilitate library development for OpenAPI / Swagger APIs.',
     'long_description': '---\n---\n\n# OpenApiLibCore for Robot Framework\n\nThe OpenApiLibCore library is a utility library that is meant to simplify creation\nof other Robot Framework libraries for API testing based on the information in\nan OpenAPI document (also known as Swagger document).\nThis document explains how to use the OpenApiLibCore library.\n\nMy RoboCon 2022 talk about OpenApiDriver and OpenApiLibCore can be found\n[here](https://www.youtube.com/watch?v=7YWZEHxk9Ps)\n\nFor more information about Robot Framework, see http://robotframework.org.\n\n---\n\n> Note: OpenApiLibCore is still being developed so there are currently\nrestrictions / limitations that you may encounter when using this library to run\ntests against an API. See [Limitations](#limitations) for details.\n\n---\n\n## Installation\n\nIf you already have Python >= 3.8 with pip installed, you can simply run:\n\n`pip install --upgrade robotframework-openapi-libcore`\n\n---\n\n## OpenAPI (aka Swagger)\n\nThe OpenAPI Specification (OAS) defines a standard, language-agnostic interface\nto RESTful APIs, see https://swagger.io/specification/\n\nThe OpenApiLibCore implements a number of Robot Framework keywords that make it\neasy to interact with an OpenAPI implementation by using the information in the\nopenapi document (Swagger file), for examply by automatic generation of valid values\nfor requests based on the schema information in the document.\n\n> Note: OpenApiLibCore is designed for APIs based on the OAS v3\nThe library has not been tested for APIs based on the OAS v2.\n\n---\n\n## Getting started\n\nBefore trying to use the keywords exposed by OpenApiLibCore on the target API\nit\'s recommended to first ensure that the openapi document for the API is valid\nunder the OpenAPI Specification.\n\nThis can be done using the command line interface of a package that is installed as\na prerequisite for OpenApiLibCore.\nBoth a local openapi.json or openapi.yaml file or one hosted by the API server\ncan be checked using the `prance validate <reference_to_file>` shell command:\n\n```shell\nprance validate http://localhost:8000/openapi.json\nProcessing "http://localhost:8000/openapi.json"...\n -> Resolving external references.\nValidates OK as OpenAPI 3.0.2!\n\nprance validate /tests/files/petstore_openapi.yaml\nProcessing "/tests/files/petstore_openapi.yaml"...\n -> Resolving external references.\nValidates OK as OpenAPI 3.0.2!\n```\n\nYou\'ll have to change the url or file reference to the location of the openapi\ndocument for your API.\n\n> Note: Although recursion is technically allowed under the OAS, tool support is limited\nand changing the API to not use recursion is recommended.\nAt present OpenApiLibCore has limited support for parsing OpenAPI documents with\nrecursion in them. See the `recursion_limit` and `recursion_default` parameters.\n\nIf the openapi document passes this validation, the next step is trying to do a test\nrun with a minimal test suite.\nThe example below can be used, with `source`, `origin` and \'endpoint\' altered to\nfit your situation.\n\n``` robotframework\n*** Settings ***\nLibrary            OpenApiLibCore\n...                    source=http://localhost:8000/openapi.json\n...                    origin=http://localhost:8000\n\n*** Test Cases ***\nGetting Started\n    ${url}=    Get Valid Url    endpoint=/employees/{employee_id}   method=get\n\n```\n\nRunning the above suite for the first time may result in an error / failed test.\nYou should look at the Robot Framework `log.html` to determine the reasons\nfor the failing tests.\nDepending on the reasons for the failures, different solutions are possible.\n\nDetails about the OpenApiLibCore library parameters and keywords that you may need can be found\n[here](https://marketsquare.github.io/robotframework-openapi-libcore/openapi_libcore.html).\n\nThe OpenApiLibCore also support handling of relations between resources within the scope\nof the API being validated as well as handling dependencies on resources outside the\nscope of the API. In addition there is support for handling restrictions on the values\nof parameters and properties.\n\nDetails about the `mappings_path` variable usage can be found\n[here](https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html).\n\n---\n\n## Limitations\n\nThere are currently a number of limitations to supported API structures, supported\ndata types and properties. The following list details the most important ones:\n- Only JSON request and response bodies are supported.\n- No support for per-endpoint authorization levels.\n- Parsing of OAS 3.1 documents is supported by the parsing tools, but runtime behavior is untested.\n\n',
     'author': 'Robin Mackaij',
     'author_email': 'r.a.mackaij@gmail.com',
     'maintainer': 'Robin Mackaij',
     'maintainer_email': 'r.a.mackaij@gmail.com',
     'url': 'https://github.com/MarketSquare/robotframework-openapi-libcore',
```

### Comparing `robotframework_openapi_libcore-1.8.4/PKG-INFO` & `robotframework_openapi_libcore-1.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-openapi-libcore
-Version: 1.8.4
+Version: 1.8.5
 Summary: A Robot Framework library to facilitate library development for OpenAPI / Swagger APIs.
 Home-page: https://github.com/MarketSquare/robotframework-openapi-libcore
 License: Apache-2.0
 Author: Robin Mackaij
 Author-email: r.a.mackaij@gmail.com
 Maintainer: Robin Mackaij
 Maintainer-email: r.a.mackaij@gmail.com
```

