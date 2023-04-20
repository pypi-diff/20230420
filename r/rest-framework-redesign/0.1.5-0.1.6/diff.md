# Comparing `tmp/rest_framework_redesign-0.1.5.tar.gz` & `tmp/rest_framework_redesign-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_framework_redesign-0.1.5.tar", max compression
+gzip compressed data, was "rest_framework_redesign-0.1.6.tar", max compression
```

## Comparing `rest_framework_redesign-0.1.5.tar` & `rest_framework_redesign-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1095 2023-04-17 08:21:25.010142 rest_framework_redesign-0.1.5/LICENSE
--rw-r--r--   0        0        0      570 2023-04-18 08:29:22.507759 rest_framework_redesign-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      792 2023-04-18 08:20:43.087539 rest_framework_redesign-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_redesign-0.1.5/rest_framework_redesign/__init__.py
--rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_redesign-0.1.5/rest_framework_redesign/admin.py
--rw-r--r--   0        0        0      248 2023-04-17 08:33:14.492981 rest_framework_redesign-0.1.5/rest_framework_redesign/apps.py
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_redesign-0.1.5/rest_framework_redesign/migrations/__init__.py
--rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_redesign-0.1.5/rest_framework_redesign/models.py
--rw-r--r--   0        0        0    22948 2023-04-18 08:45:22.244712 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/api.html
--rw-r--r--   0        0        0      744 2023-04-18 08:53:35.615309 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/filters/base.html
--rw-r--r--   0        0        0      700 2023-04-18 08:50:06.523205 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/filters/ordering.html
--rw-r--r--   0        0        0      608 2023-04-18 08:49:46.702650 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/filters/search.html
--rw-r--r--   0        0        0      835 2023-04-17 06:09:51.030141 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html
--rw-r--r--   0        0        0     1536 2023-04-17 06:10:08.352256 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/dict_field.html
--rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/fieldset.html
--rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/form.html
--rw-r--r--   0        0        0     1096 2023-04-17 06:10:16.889823 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/input.html
--rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/list_field.html
--rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/list_fieldset.html
--rw-r--r--   0        0        0     1448 2023-04-17 06:10:38.062218 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/radio.html
--rw-r--r--   0        0        0     1205 2023-04-17 06:11:00.824317 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/select.html
--rw-r--r--   0        0        0     1239 2023-04-17 06:12:33.906413 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html
--rw-r--r--   0        0        0      813 2023-04-17 06:12:09.013201 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html
--rw-r--r--   0        0        0     4375 2023-04-18 08:11:26.812363 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/login.html
--rw-r--r--   0        0        0     1715 2023-04-16 10:26:12.389947 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/pagination/numbers.html
--rw-r--r--   0        0        0      692 2023-04-16 10:31:24.701736 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html
--rw-r--r--   0        0        0      307 2023-04-18 06:07:45.314176 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/raw_data_form.html
--rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_redesign-0.1.5/rest_framework_redesign/tests.py
--rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_redesign-0.1.5/rest_framework_redesign/views.py
--rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 rest_framework_redesign-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-04-17 08:21:25.010142 rest_framework_redesign-0.1.6/LICENSE
+-rw-r--r--   0        0        0      570 2023-04-18 12:02:52.652114 rest_framework_redesign-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      792 2023-04-18 08:20:43.087539 rest_framework_redesign-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_redesign-0.1.6/rest_framework_redesign/__init__.py
+-rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_redesign-0.1.6/rest_framework_redesign/admin.py
+-rw-r--r--   0        0        0      248 2023-04-17 08:33:14.492981 rest_framework_redesign-0.1.6/rest_framework_redesign/apps.py
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_redesign-0.1.6/rest_framework_redesign/migrations/__init__.py
+-rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_redesign-0.1.6/rest_framework_redesign/models.py
+-rw-r--r--   0        0        0    23750 2023-04-20 09:09:17.444650 rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/api.html
+-rw-r--r--   0        0        0     1085 2023-04-20 09:11:06.989223 rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/filters/base.html
+-rw-r--r--   0        0        0      700 2023-04-18 08:50:06.523205 rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/filters/ordering.html
+-rw-r--r--   0        0        0      608 2023-04-18 08:49:46.702650 rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/filters/search.html
+-rw-r--r--   0        0        0      866 2023-04-19 11:57:00.707959 rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html
+-rw-r--r--   0        0        0     1567 2023-04-19 11:56:43.779104 rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/horizontal/dict_field.html
+-rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/horizontal/fieldset.html
+-rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/horizontal/form.html
+-rw-r--r--   0        0        0     1182 2023-04-19 11:59:11.581766 rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/horizontal/input.html
+-rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/horizontal/list_field.html
+-rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/horizontal/list_fieldset.html
+-rw-r--r--   0        0        0     1499 2023-04-19 11:58:53.030223 rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/horizontal/radio.html
+-rw-r--r--   0        0        0     1220 2023-04-19 11:59:53.039237 rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/horizontal/select.html
+-rw-r--r--   0        0        0     1254 2023-04-19 11:59:33.439478 rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html
+-rw-r--r--   0        0        0      828 2023-04-19 12:00:12.217896 rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html
+-rw-r--r--   0        0        0     4375 2023-04-18 08:11:26.812363 rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/login.html
+-rw-r--r--   0        0        0     1715 2023-04-16 10:26:12.389947 rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/pagination/numbers.html
+-rw-r--r--   0        0        0      692 2023-04-16 10:31:24.701736 rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html
+-rw-r--r--   0        0        0      307 2023-04-18 06:07:45.314176 rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/raw_data_form.html
+-rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_redesign-0.1.6/rest_framework_redesign/tests.py
+-rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_redesign-0.1.6/rest_framework_redesign/views.py
+-rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 rest_framework_redesign-0.1.6/PKG-INFO
```

### Comparing `rest_framework_redesign-0.1.5/LICENSE` & `rest_framework_redesign-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.5/pyproject.toml` & `rest_framework_redesign-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rest-framework-redesign"
-version = "0.1.5"
+version = "0.1.6"
 description = "Redesign of the browsable api of Django REST Framework"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rest_framework_redesign"}]
 homepage = "https://github.com/youzarsiph/rest-framework-redesign/"
 repository = "https://github.com/youzarsiph/rest-framework-redesign/"
```

### Comparing `rest_framework_redesign-0.1.5/README.md` & `rest_framework_redesign-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/api.html` & `rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/api.html`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,23 @@
   {% block bootstrap_theme %}
     <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/css/bootstrap.min.css" rel="stylesheet"
       integrity="sha384-KK94CHFLLe+nY2dmCWGMq91rCGa5gtU4mk92HdvYe+M/SXH301p5ILy+dN9+nJOZ" crossorigin="anonymous">
     <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.4/font/bootstrap-icons.css">
     <link rel="stylesheet" href="//cdn.jsdelivr.net/gh/highlightjs/cdn-release@11.7.0/build/styles/default.min.css">
   {% endblock %}
 
-  {% if code_style %}<style>{{ code_style }}</style>{% endif %}
+  <style>
+    {% if code_style %}
+      {{ code_style }}
+    {% endif %}
+
+    .dropdown-toggle::after {
+      content: none;
+    }
+  </style>
 {% endblock %}
 
 
 {% block navbar %}
   <header class="fixed-top">
     <div class="bg-danger py-2 shadow">
       <nav class="navbar navbar-expand-lg navbar-dark bg-dark {% block bootstrap_navbar_variant %}{% endblock %}"
@@ -59,21 +67,34 @@
                 <a href="https://github.com/encode/django-rest-framework/" class="nav-link">
                   <strong class="d-flex align-items-center gap-3">
                     <i class="bi bi-github"></i>
                     {% translate "Github" %}
                   </strong>
                 </a>
               </li>
+              <li class="nav-item">
+                <a href="https://github.com/youzarsiph/rest-framework-redesign/" class="nav-link">
+                  <strong class="d-flex align-items-center gap-3">
+                    <i class="bi bi-code-slash"></i>
+                    {% translate "Redesign" %}
+                  </strong>
+                </a>
+              </li>
             </ul>
             <ul class="navbar-nav">
               <li class="nav-item dropdown">
                 <a href="#" class="nav-link" data-bs-toggle="dropdown">
                   <strong class="d-flex align-items-center gap-3">
                     <i class="bi bi-person-fill"></i>
-                    {{ request.user|capfirst }}
+                    {% if user.is_authenticated %}
+                      {{ request.user|capfirst }}
+                    {% else %}
+                      {% translate "Account" %}
+                    {% endif %}
+                    <i class="bi bi-chevron-down"></i>
                   </strong>
                 </a>
                 <ul class="dropdown-menu dropdown-menu-dark dropdown-menu-end rounded-3 shadow">
                   <li>
                     {% if user.is_authenticated %}
                       <a class="dropdown-item" href="{% url 'rest_framework:logout' %}">
                         <strong class="d-flex align-items-center gap-3">
@@ -153,15 +174,17 @@
                     title="Make a GET request on the {{ name }} resource">
                     <strong class="d-flex align-items-center justify-content-center gap-3">
                       <i class="bi bi-arrow-clockwise"></i>
                       {% translate "GET" %}
                     </strong>
                   </a>
                   <button class="btn btn-lg btn-outline-primary dropdown-toggle" type="button" id="dropdownMenuButton"
-                    data-bs-toggle="dropdown" aria-expanded="false"></button>
+                    data-bs-toggle="dropdown" aria-expanded="false">
+                    <i class="bi bi-chevron-down"></i>
+                  </button>
                   <div class="dropdown">
                     <ul class="dropdown-menu dropdown-menu-end rounded-3 shadow" aria-labelledby="dropdownMenuButton">
                       <li>
                         <h6 class="dropdown-header">
                           {% translate 'Select a format' %}
                         </h6>
                       </li>
@@ -209,55 +232,55 @@
                 <i class="bi bi-trash"></i>
                 {% translate "DELETE" %}
               </strong>
             </button>
           </div>
 
           <div class="modal fade" id="deleteModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
-            <div class="modal-dialog">
-              <div class="modal-content p-4 rounded-3 shadow">
+            <div class="modal-dialog modal-dialog-centered">
+              <div class="modal-content p-md-3 p-lg-4 rounded-4 shadow">
                 <div class="modal-header border-bottom-0">
                   <h3 class="modal-title" id="exampleModalLabel">
                     {% translate 'Delete' %} {{ name }}
                   </h3>
                   <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                 </div>
                 <div class="modal-body">
-                  <p class="lead mb-4">
+                  <p class="mb-4">
                     {% translate "Are you sure you want to delete this" %} {{ name }}?
                   </p>
-                  <div class="d-grid gap-4">
-                    <button type="button" class="btn btn-lg btn-outline-secondary" data-bs-dismiss="modal">
-                      <strong class="d-flex align-item-center justify-content-center gap-3">
-                        <i class="bi bi-close"></i>
-                        {% translate "Cancel" %}
-                      </strong>
-                    </button>
-                    <form class="button-form" action="{{ request.get_full_path }}" data-method="DELETE">
-                      <button class="btn btn-lg btn-danger">
+                  <div class="d-grid d-lg-flex align-items-lg-center gap-4">
+                    <form class="button-form w-100" action="{{ request.get_full_path }}" data-method="DELETE">
+                      <button class="btn btn-lg btn-danger w-100">
                         <strong class="d-flex align-item-center justify-content-center gap-3">
                           <i class="bi bi-trash"></i>
                           {% translate "Delete" %}
                         </strong>
                       </button>
                     </form>
+                    <button type="button" class="btn btn-lg btn-outline-secondary w-100" data-bs-dismiss="modal">
+                      <strong class="d-flex align-item-center justify-content-center gap-3">
+                        <i class="bi bi-x-lg"></i>
+                        {% translate "Cancel" %}
+                      </strong>
+                    </button>
                   </div>
                 </div>
               </div>
             </div>
           </div>
         {% endif %}
 
         {% if extra_actions %}
-          <div class="dropdown" style="float: right; margin-right: 10px">
+          <div class="dropdown">
             <button class="btn btn-lg btn-info w-100" id="extra-actions-menu" data-bs-toggle="dropdown" aria-haspopup="true"
               aria-expanded="true">
               <strong class="d-flex align-items-center justify-content-center gap-3">
-                <i class="bi bi-three-dots"></i>
                 {% translate "Extra Actions" %}
+                <i class="bi bi-chevron-down"></i>
               </strong>
             </button>
             <ul class="dropdown-menu" aria-labelledby="extra-actions-menu">
               {% for action_name, url in extra_actions|items %}
                 <li>
                   <a class="dropdown-item" href="{{ url }}">
                     {{ action_name }}
```

#### html2text {}

```diff
@@ -1,19 +1,21 @@
 {% extends "rest_framework/base.html" %} {% load i18n static rest_framework %}
 {% block meta %} {{ block.super }}
  {% endblock %} {% block style %} {% block bootstrap_theme %}
 
 
- {% endblock %} {% if code_style %}
-{% endif %} {% endblock %} {% block navbar %}
+ {% endblock %}
+ {% endblock %} {% block navbar %}
 {% block branding %} {%_translate_'Django_REST_Framework'_%} {% endblock %}
     *  {%_translate_"Home"_%}
     *  {%_translate_"Tutorial"_%}
     *  {%_translate_"Github"_%}
-    *  {{_request.user|capfirst_}}
+    *  {%_translate_"Redesign"_%}
+    *  {%_if_user.is_authenticated_%}_{{_request.user|capfirst_}}_{%_else_%}_{%
+      translate_"Account"_%}_{%_endif_%}
           o {% if user.is_authenticated %}
              {%_translate_'Logout'_%}
              {% else %}
              {%_translate_'Login'_%}
              {% endif %}
  {% endblock %} {% block breadcrumbs %}
    1. {% for breadcrumb_name, breadcrumb_url in breadcrumblist %} {% if
@@ -46,22 +48,22 @@
 {% endif %} {% if delete_form %}
 
  {% translate "DELETE" %}
 
 **** {% translate 'Delete' %} {{ name }} ****
 {% translate "Are you sure you want to delete this" %} {{ name }}?
 
- {% translate "Cancel" %}
+ {% translate "Delete" %}
 
 
- {% translate "Delete" %}
+ {% translate "Cancel" %}
 
 {% endif %} {% if extra_actions %}
 
- {% translate "Extra Actions" %}
+{% translate "Extra Actions" %}
 
     * {% for action_name, url in extra_actions|items %}
     * {{_action_name_}}
     * {% endfor %}
 {% endif %} {% if filter_form %}
  {% translate "Filters" %}
   {% endif %}  {% endblock %}
```

### Comparing `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/filters/base.html` & `rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/filters/base.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 {% load i18n %}
 
 <div class="modal fade" id="filtersModal" tabindex="-1" aria-labelledby="filters" role="dialog" aria-hidden="true">
-  <div class="modal-dialog">
-    <div class="modal-content p-4 rounded-3 shadow">
+  <div class="modal-dialog modal-dialog-centered">
+    <div class="modal-content p-md-3 p-lg-4 rounded-4 shadow">
       <div class="modal-header border-bottom-0">
         <h3 class="modal-title" id="filters">
           {% translate "Filters" %}
         </h3>
         <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
       </div>
       <div class="modal-body">
         <div class="d-grid gap-4">
           {% for element in elements %}
             <div>
               {{ element }}
             </div>
           {% endfor %}
+          <button type="button" class="btn btn-lg btn-outline-secondary" data-bs-dismiss="modal">
+            <strong class="d-flex align-item-center justify-content-center gap-3">
+              <i class="bi bi-x-lg"></i>
+              {% translate "Cancel" %}
+            </strong>
+          </button>
         </div>
       </div>
     </div>
   </div>
 </div>
```

### Comparing `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/filters/ordering.html` & `rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/filters/ordering.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/filters/search.html` & `rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/filters/search.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html` & `rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html`

 * *Files 7% similar despite different names*

```diff
@@ -14,20 +14,21 @@
         for="{{ field.name }}"
         class="form-check-label {% if style.hide_label %}sr-only{% endif %}"
       >
         {{ field.label }}
       </label>
     {% endif %}
 
+    {% if field.help_text %}
+      <small class="d-block text-muted">{{ field.help_text|safe }}</small>
+    {% endif %}
+
     {% if field.errors %}
+      <div class="mt-3"></div>
       {% for error in field.errors %}
         <div role="alert" class="alert alert-warning mb-3">
           <p>{{ error }}</p>
         </div>
       {% endfor %}
     {% endif %}
-
-    {% if field.help_text %}
-      <small class="d-block text-muted">{{ field.help_text|safe }}</small>
-    {% endif %}
   </div>
 </div>
```

### Comparing `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html` & `rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html`

 * *Files 18% similar despite different names*

```diff
@@ -34,20 +34,21 @@
             {% if key|as_string in field.value|as_list_of_strings %}checked{% endif %}
           />
           <label class="form-check-label" for="{{ key }}"> {{ text }} </label>
         </div>
       {% endfor %}
     {% endif %}
 
+    {% if field.help_text %}
+      <small class="d-block text-muted">{{ field.help_text|safe }}</small>
+    {% endif %}
+
     {% if field.errors %}
+      <div class="mt-3"></div>
       {% for error in field.errors %}
         <div role="alert" class="alert alert-warning mb-3">
           <p>{{ error }}</p>
         </div>
       {% endfor %}
     {% endif %}
-
-    {% if field.help_text %}
-      <small class="d-block text-muted">{{ field.help_text|safe }}</small>
-    {% endif %}
   </div>
 </div>
```

### Comparing `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/input.html` & `rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/horizontal/input.html`

 * *Files 8% similar despite different names*

```diff
@@ -16,17 +16,20 @@
 
   {% if field.label and style.input_type != "file" %}
     <label class="form-label {% if style.hide_label %}sr-only{% endif %}">
       {{ field.label }}
     </label>
   {% endif %}
 
-  {% if field.help_text %}
-    <small class="d-block text-muted">{{ field.help_text|safe }}</small>
-  {% endif %}
+    {% if field.help_text %}
+      <small class="d-block text-muted">{{ field.help_text|safe }}</small>
+    {% endif %}
 
-  {% if field.errors %}
-    {% for error in field.errors %}
-      <div class="alert alert-warning mbb-3">{{ error }}</div>
-    {% endfor %}
-  {% endif %}
+    {% if field.errors %}
+      <div class="mt-3"></div>
+      {% for error in field.errors %}
+        <div role="alert" class="alert alert-warning mb-3">
+          <p>{{ error }}</p>
+        </div>
+      {% endfor %}
+    {% endif %}
 </div>
```

### Comparing `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/radio.html` & `rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/horizontal/radio.html`

 * *Files 3% similar despite different names*

```diff
@@ -37,19 +37,20 @@
         >
           {{ text }}
         </label>
       {% endif %}
     </div>
   {% endfor %}
 
-  {% if field.errors %}
-    {% for error in field.errors %}
-      <div role="alert" class="alert alert-warning mb-3">
-        <p>{{ error }}</p>
-      </div>
-    {% endfor %}
-  {% endif %}
+    {% if field.help_text %}
+      <small class="d-block text-muted">{{ field.help_text|safe }}</small>
+    {% endif %}
 
-  {% if field.help_text %}
-    <small class="d-block text-muted">{{ field.help_text|safe }}</small>
-  {% endif %}
+    {% if field.errors %}
+      <div class="mt-3"></div>
+      {% for error in field.errors %}
+        <div role="alert" class="alert alert-warning mb-3">
+          <p>{{ error }}</p>
+        </div>
+      {% endfor %}
+    {% endif %}
 </div>
```

### Comparing `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/select.html` & `rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,41 @@
+{% load i18n %}
 {% load rest_framework %}
 
+{% translate "No items to select." as no_items %}
+
 <div class="form-floating mb-4">
-  <select class="form-select" name="{{ field.name }}">
-    {% if field.allow_null or field.allow_blank %}
-      <option value="" {% if not field.value %}selected{% endif %}>--------</option>
-    {% endif %}
+  <select multiple {{ field.choices|yesno:",disabled" }} class="form-select" name="{{ field.name }}">
     {% for select in field.iter_options %}
       {% if select.start_option_group %}
         <optgroup label="{{ select.label }}">
       {% elif select.end_option_group %}
         </optgroup>
       {% else %}
-        <option value="{{ select.value }}" {% if select.value|as_string == field.value|as_string %}selected{% endif %}
-         {% if select.disabled %}disabled{% endif %}>{{ select.display_text }}</option>
+        <option value="{{ select.value }}"
+        {% if select.value|as_string in field.value|as_list_of_strings %}selected{% endif %}
+        {% if select.disabled %}disabled{% endif %}>{{ select.display_text }}</option>
       {% endif %}
+    {% empty %}
+        <option>{{ no_items }}</option>
     {% endfor %}
   </select>
 
   {% if field.label %}
     <label class="form-label {% if style.hide_label %}sr-only{% endif %}">
       {{ field.label }}
     </label>
   {% endif %}
 
   {% if field.help_text %}
-    <small class="d-block text-muted" class="invalid-feedback">
-      {{ field.help_text|safe }}
-    </small>
+    <small class="d-block text-muted">{{ field.help_text|safe }}</small>
   {% endif %}
 
   {% if field.errors %}
+    <div class="mt-3"></div>
     {% for error in field.errors %}
-      <div role="alert" class="alert alert-warning mb-3">{{ error }}</div>
+      <div role="alert" class="alert alert-warning mb-3">
+        <p>{{ error }}</p>
+      </div>
     {% endfor %}
   {% endif %}
 </div>
```

### Comparing `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html` & `rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/horizontal/select.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,38 @@
-{% load i18n %}
 {% load rest_framework %}
 
-{% translate "No items to select." as no_items %}
-
 <div class="form-floating mb-4">
-  <select multiple {{ field.choices|yesno:",disabled" }} class="form-select" name="{{ field.name }}">
+  <select class="form-select" name="{{ field.name }}">
+    {% if field.allow_null or field.allow_blank %}
+      <option value="" {% if not field.value %}selected{% endif %}>--------</option>
+    {% endif %}
     {% for select in field.iter_options %}
       {% if select.start_option_group %}
         <optgroup label="{{ select.label }}">
       {% elif select.end_option_group %}
         </optgroup>
       {% else %}
-        <option value="{{ select.value }}"
-        {% if select.value|as_string in field.value|as_list_of_strings %}selected{% endif %}
-        {% if select.disabled %}disabled{% endif %}>{{ select.display_text }}</option>
+        <option value="{{ select.value }}" {% if select.value|as_string == field.value|as_string %}selected{% endif %}
+         {% if select.disabled %}disabled{% endif %}>{{ select.display_text }}</option>
       {% endif %}
-    {% empty %}
-        <option>{{ no_items }}</option>
     {% endfor %}
   </select>
 
   {% if field.label %}
     <label class="form-label {% if style.hide_label %}sr-only{% endif %}">
       {{ field.label }}
     </label>
   {% endif %}
 
   {% if field.help_text %}
-    <small class="d-block text-muted" class="invalid-feedback">
-      {{ field.help_text|safe }}
-    </small>
+    <small class="d-block text-muted">{{ field.help_text|safe }}</small>
   {% endif %}
 
   {% if field.errors %}
+    <div class="mt-3"></div>
     {% for error in field.errors %}
-      <div role="alert" class="alert alert-warning mb-3">{{ error }}</div>
+      <div role="alert" class="alert alert-warning mb-3">
+        <p>{{ error }}</p>
+      </div>
     {% endfor %}
   {% endif %}
 </div>
```

### Comparing `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html` & `rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html`

 * *Files 14% similar despite different names*

```diff
@@ -8,18 +8,19 @@
   {% if field.label %}
     <label class="form-label {% if style.hide_label %}sr-only{% endif %}">
       {{ field.label }}
     </label>
   {% endif %}
 
   {% if field.help_text %}
-    <small class="d-block text-muted" class="invalid-feedback">
-      {{ field.help_text|safe }}
-    </small>
+    <small class="d-block text-muted">{{ field.help_text|safe }}</small>
   {% endif %}
 
   {% if field.errors %}
+    <div class="mt-3"></div>
     {% for error in field.errors %}
-      <div role="alert" class="alert alert-warning mb-3">{{ error }}</div>
+      <div role="alert" class="alert alert-warning mb-3">
+        <p>{{ error }}</p>
+      </div>
     {% endfor %}
   {% endif %}
 </div>
```

### Comparing `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/login.html` & `rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/login.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/pagination/numbers.html` & `rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/pagination/numbers.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html` & `rest_framework_redesign-0.1.6/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.5/PKG-INFO` & `rest_framework_redesign-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest-framework-redesign
-Version: 0.1.5
+Version: 0.1.6
 Summary: Redesign of the browsable api of Django REST Framework
 Home-page: https://github.com/youzarsiph/rest-framework-redesign/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

