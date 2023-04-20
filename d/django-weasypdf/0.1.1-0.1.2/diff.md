# Comparing `tmp/django_weasypdf-0.1.1-py2.py3-none-any.whl.zip` & `tmp/django_weasypdf-0.1.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 35195 bytes, number of entries: 22
--rw-r--r--  2.0 unx       22 b- defN 23-Apr-20 09:49 weasypdf/__init__.py
+Zip file size: 35230 bytes, number of entries: 22
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-20 10:18 weasypdf/__init__.py
 -rw-r--r--  2.0 unx       91 b- defN 23-Apr-20 08:59 weasypdf/apps.py
 -rw-r--r--  2.0 unx    12626 b- defN 23-Apr-20 07:37 weasypdf/plot.py
 -rw-r--r--  2.0 unx      324 b- defN 23-Apr-20 09:00 weasypdf/urls.py
 -rw-r--r--  2.0 unx     5556 b- defN 23-Apr-20 09:00 weasypdf/utils.py
--rw-r--r--  2.0 unx     6009 b- defN 23-Apr-20 09:02 weasypdf/views.py
+-rw-r--r--  2.0 unx     6029 b- defN 23-Apr-20 10:06 weasypdf/views.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-20 07:37 weasypdf/management/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-20 07:37 weasypdf/management/commands/__init__.py
 -rw-r--r--  2.0 unx     7055 b- defN 23-Apr-20 09:02 weasypdf/management/commands/build_test_pdf.py
 -rw-r--r--  2.0 unx    13320 b- defN 23-Apr-20 07:37 weasypdf/static/weasypdf/images/header_left.png
 -rw-r--r--  2.0 unx      707 b- defN 23-Apr-20 07:37 weasypdf/templates/weasypdf/base.html
 -rw-r--r--  2.0 unx      707 b- defN 23-Apr-20 07:37 weasypdf/templates/weasypdf/base_nomargins.html
 -rw-r--r--  2.0 unx      536 b- defN 23-Apr-20 07:37 weasypdf/templates/weasypdf/footer.html
 -rw-r--r--  2.0 unx      810 b- defN 23-Apr-20 09:05 weasypdf/templates/weasypdf/header.html
 -rw-r--r--  2.0 unx      890 b- defN 23-Apr-20 07:37 weasypdf/templates/weasypdf/styles.css
 -rw-r--r--  2.0 unx       26 b- defN 23-Apr-20 07:37 weasypdf/templates/weasypdf/pages/test.css
 -rw-r--r--  2.0 unx      481 b- defN 23-Apr-20 09:03 weasypdf/templates/weasypdf/pages/test.html
--rw-r--r--  2.0 unx     1065 b- defN 23-Apr-20 09:53 django_weasypdf-0.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    15439 b- defN 23-Apr-20 09:53 django_weasypdf-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-20 09:53 django_weasypdf-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Apr-20 09:53 django_weasypdf-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1930 b- defN 23-Apr-20 09:53 django_weasypdf-0.1.1.dist-info/RECORD
-22 files, 67713 bytes uncompressed, 32001 bytes compressed:  52.7%
+-rw-r--r--  2.0 unx     1065 b- defN 23-Apr-20 10:19 django_weasypdf-0.1.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    15745 b- defN 23-Apr-20 10:19 django_weasypdf-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-20 10:19 django_weasypdf-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-20 10:19 django_weasypdf-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1930 b- defN 23-Apr-20 10:19 django_weasypdf-0.1.2.dist-info/RECORD
+22 files, 68039 bytes uncompressed, 32036 bytes compressed:  52.9%
```

## zipnote {}

```diff
@@ -45,23 +45,23 @@
 
 Filename: weasypdf/templates/weasypdf/pages/test.css
 Comment: 
 
 Filename: weasypdf/templates/weasypdf/pages/test.html
 Comment: 
 
-Filename: django_weasypdf-0.1.1.dist-info/LICENSE
+Filename: django_weasypdf-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: django_weasypdf-0.1.1.dist-info/METADATA
+Filename: django_weasypdf-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: django_weasypdf-0.1.1.dist-info/WHEEL
+Filename: django_weasypdf-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: django_weasypdf-0.1.1.dist-info/top_level.txt
+Filename: django_weasypdf-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: django_weasypdf-0.1.1.dist-info/RECORD
+Filename: django_weasypdf-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## weasypdf/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '0.1.1'
+__version__ = '0.1.2'
```

## weasypdf/views.py

```diff
@@ -8,17 +8,17 @@
 from django.db import connection
 
 from .utils import get_pdf_styles
 from .utils import build_pdf_document
 from .utils import Counter
 
 ################################################################################
-# Base PdfView
+# Base WeasypdfView
 
-class PdfView(TemplateView):
+class WeasypdfView(TemplateView):
 
     body_template_name = 'weasypdf/base.html'
     styles_template_name = ''
     header_template_name = 'weasypdf/header.html'
     footer_template_name = 'weasypdf/footer.html'
     title = "Title"
     for_download = False
@@ -42,15 +42,15 @@
             self.debug = bool(int(self.request.GET.get('debug')))
         except:
             self.debug = False
         try:
             self.format = self.request.GET.get('format')
         except:
             self.format = 'pdf'
-        context = super(PdfView, self).get_context_data(**kwargs)
+        context = super(WeasypdfView, self).get_context_data(**kwargs)
         self.for_download = context.pop('for_download', False)
         #self.print_date = timezone.now()
 
         # Remove <view> from context to make sure all templates are generic
         context.pop('view', None)
 
         return context
@@ -145,15 +145,15 @@
             format=self.format,
         )
 
 
 ################################################################################
 # Pages
 
-class PdfTestView(PdfView):
+class PdfTestView(WeasypdfView):
 
     """
     Per il fine-tuning del css conviene invocare direttamente la view dal browser
     e selezionando "format=html",
     al fine di ottenere la pagina HTML che verrebbe utilizzata per il rendering
     del documento PDF.
```

## Comparing `django_weasypdf-0.1.1.dist-info/LICENSE` & `django_weasypdf-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `django_weasypdf-0.1.1.dist-info/METADATA` & `django_weasypdf-0.1.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: django-weasypdf
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Django class-based view helper to generate PDF with WeasyPrint
 Home-page: http://github.com/morlandi/django-weasypdf
 Author: Mario Orlandi
 Author-email: morlandi@brainstorm.it
 License: MIT
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
-django-pdf
-==========
+django-weasypdf
+===============
 
 A Django class-based view helper to generate PDF with WeasyPrint.
 
 Requires: `WeasyPrint <https://github.com/Kozea/WeasyPrint>`_
 
 Optional requirements:
 
@@ -34,104 +34,116 @@
 
     pip install django-weasypdf
 
 or:
 
 .. code:: bash
 
-    pip install git+https://github.com/morlandi/django-pdf
+    pip install git+https://github.com/morlandi/django-weasypdf
 
 
-You will probably build you own app in the project to provide derived Views
-and custom templates; for example:
+You will probably build your own app, for example `reports`, to provide custom derived Views
+and templates:
 
 .. code:: bash
 
     python manage.py startapp reports
 
 In your settings, add:
 
 .. code:: python
 
     INSTALLED_APPS = [
         ...
         'reports',
-        'pdf',
+        'weasypdf',
     ]
 
-Note that `reports` is listed before `pdf` to make sure you can possibly
+Note that `reports` is listed before `weasypdf` to make sure you can possibly
 override any template.
 
 In your urls, add:
 
 .. code:: python
 
+    from django.urls import path, include
+
     urlpatterns = [
         ...
         path('reports/', include('reports.urls', namespace='reports')),
         ...
 
-You might want to copy the default templates from 'pdf/templates/pdf' to 'reports/templates/reports'
+Optionally, you might want to copy the default templates from 'weasypdf/templates/weasypdf' to 'reports/templates/reports'
 for any required customization; see `Customizing the templates`_ below
 
 A sample report
 ---------------
 
-A test view has been provided to render a sample report for demonstration purposes.
+A test view has already been included in the `weasypdf` app
+to render a sample document for demonstration purposes.
+
+To use it, add the following to your urls:
+
+.. code:: python
+
+    path('weasypdf/', include('weasypdf.urls', namespace='weasypdf')),
 
-In your main urls, include pdf/urls.py, where the required end-point have been
-mapped to the PdfTestView; then, visit:
+then, visit:
 
     http://127.0.0.1:8000/weasypdf/test/print/
 
-You can copy the following to your own app to have an initial working view
+
+Usage
+-----
+
+You can copy the following to your `reports` app to have a sample view
 to start working with:
 
 file `reports/urls.py`:
 
 .. code:: python
 
     from django.urls import path
     from . import views
 
-    app_name = 'pdf'
+    app_name = 'weasypdf'
 
     urlpatterns = [
         path('test/print/', views.ReportTestView.as_view(), {'for_download': False, 'lines': 200, }, name="test-print"),
         path('test/download/', views.ReportTestView.as_view(), {'for_download': True, 'lines': 200, }, name="test-download"),
     ]
 
 
 file `reports/views.py`:
 
 .. code:: python
 
-    from pdf.views import PdfView
+    from weasypdf.views import WeasypdfView
 
 
-    class ReportView(PdfView):
+    class ReportView(WeasypdfView):
 
         #my_custom_data = None
-        header_template_name = 'pdf/header.html'
-        footer_template_name = 'pdf/footer.html'
-        styles_template_name = 'pdf/styles.css'
+        header_template_name = 'weasypdf/header.html'
+        footer_template_name = 'weasypdf/footer.html'
+        styles_template_name = 'weasypdf/styles.css'
 
         def get_context_data(self, **kwargs):
             context = super(ReportView, self).get_context_data(**kwargs)
             #self.my_custom_data = context.pop('my_custom_data', None)
             # context.update({
             #     'footer_line_1': config.REPORT_FOOTER_LINE_1,
             #     'footer_line_2': config.REPORT_FOOTER_LINE_2,
             # })
             return context
 
 
     class ReportTestView(ReportView):
-        body_template_name = 'pdf/pages/test.html'
-        styles_template_name = 'pdf/pages/test.css'
+        body_template_name = 'weasypdf/pages/test.html'
+        styles_template_name = 'weasypdf/pages/test.css'
         # header_template_name = None
         # footer_template_name = None
         title = "Report Test"
 
         def get_context_data(self, **kwargs):
             context = super().get_context_data(**kwargs)
 
@@ -149,22 +161,22 @@
             context.update({
                 ...
             })
 
             return context
 
 
-or **replace `pdf/header.html` with `reports/header.html`**, etc ... when using
+or **replace `weasypdf/header.html` with `reports/header.html`**, etc ... when using
 custom templates.
 
 file `reports/pages/test.html`:
 
 .. code:: html
 
-    {% extends "pdf/base.html" %}
+    {% extends "weasypdf/base.html" %}
 
     {% block content %}
 
         <h1>Test PDF</h1>
 
         {% if plot_image %}
             <img class="plot" src="data:image/png;base64,{{plot_image}}">
@@ -193,15 +205,15 @@
 
 .. image:: screenshots/pdf_sample.png
 
 
 Building a PDF document from a background process
 -------------------------------------------------
 
-A `PdfView.render_as_pdf_to_stream(self, base_url, extra_context, output)` method is supplied for this purpose:
+A `WeasypdfView.render_as_pdf_to_stream(self, base_url, extra_context, output)` method is supplied for this purpose:
 
 .. code:: python
 
     def render_as_pdf_to_stream(self, base_url, extra_context, output):
         """
         Build the PDF document and save in into "ouput" stream.
 
@@ -213,15 +225,15 @@
             with open(filepath, 'wb') as f:
                 view.render_as_pdf_to_stream('', context, f)
         """
 
 A sample management command to build a PDF document outside the HTML request/response
 cycle is available here:
 
-`pdf/management/commands/build_test_pdf.py <./pdf/management/commands/build_test_pdf.py>`_
+`weasypdf/management/commands/build_test_pdf.py <./weasypdf/management/commands/build_test_pdf.py>`_
 
 
 Providing "extra_context" parameters
 ------------------------------------
 
 Supply context parameters either in the urlpattern, or invoking get_context_data():
 
@@ -243,36 +255,36 @@
     from reports.views import ReportDailyView
     view = ReportDailyView()
     context = view.get_context_data(
         exclude_inactives=task.exclude_inactives,
     )
 
     # Create empty file as result
-    filename = view.build_filename(extension="pdf")
+    filename = view.build_filename(extension="weasypdf")
     task.result.save(filename, ContentFile(''))
 
     # Open and write result
     filepath = task.result.path
 
     with open(filepath, 'wb') as f:
         view.render_as_pdf_to_stream('', context, f)
 
 
 Customizing the templates
 -------------------------
 
 These sample files::
 
-    pdf
+    weasypdf
     ├── static
-    │   └── pdf
+    │   └── weasypdf
     │       └── images
     │           └── header_left.png
     └── templates
-        └── pdf
+        └── weasypdf
             ├── base.html
             ├── base_nomargins.html
             ├── styles.css
             ├── footer.html
             ├── header.html
             └── pages
                 ├── test.css
@@ -280,15 +292,15 @@
 
 
 can be copied into your app's local folder `reports/templates/reports`,
 and used for any required customization:
 
 .. code:: python
 
-    class ReportView(PdfView):
+    class ReportView(WeasypdfView):
 
         header_template_name = 'reports/header.html'
         footer_template_name = 'reports/footer.html'
         styles_template_name = 'reports/styles.css'
 
 How to insert a page break
 --------------------------
@@ -436,15 +448,15 @@
 This doesn't help you in embedding a plot in a PDF documents built offline, however;
 in this case, you need to build an image server side.
 
 An helper function has been included in this app for that purpose; to use it, **matplotlib**
 must be installed.
 
 At the moment, it is more a POC then a complete solution; you can either use it
-from the package, or copy the source file `pdf/plot.py` in your project and use
+from the package, or copy the source file `weasypdf/plot.py` in your project and use
 `build_plot_from_data()` as a starting point:
 
 .. code:: python
 
     def build_plot_from_data(data, chart_type='line', as_base64=False, dpi=300, ylabel=''):
         """
         Build a plot from given "data";
@@ -548,14 +560,18 @@
 
 
 
 
 History
 =======
 
+v0.1.2
+------
+* PdfView renamed as WeasypdfView
+
 v0.1.1
 ------
 * Rename "pdf" module as "weasypdf"
 * Sample project added
 
 v0.1.0
 ------
```

## Comparing `django_weasypdf-0.1.1.dist-info/RECORD` & `django_weasypdf-0.1.2.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-weasypdf/__init__.py,sha256=ls1camlIoMxEZz9gSkZ1OJo-MXqHWwKPtdPbZJmwp7E,22
+weasypdf/__init__.py,sha256=mdp2CftfqYbdKtP-eWv1z7rAUycYv6X1ntXSMUf8Kss,22
 weasypdf/apps.py,sha256=960x1-198ek9ycxaM08KYdYpvOISIqskricbfEyhDVc,91
 weasypdf/plot.py,sha256=B1PsWQMBJt0QSucb3uFVDM3sviqBl6ui9O3mT7w9-kc,12626
 weasypdf/urls.py,sha256=xkY4ylMWUViN-NI97bWEKwylOw6j8-lDzb9nPSA1Yws,324
 weasypdf/utils.py,sha256=p6qRmaCxBfUPVZZhckMVlgUgAkAq64II0d4-AO3TllA,5556
-weasypdf/views.py,sha256=ti5t_BpFe6MUYx-TEb6zXzUIy6IcqdNli7aRHnaRqp4,6009
+weasypdf/views.py,sha256=TK9NsRG8eO-Zsh5zm0_8XLjyqxRKtgRuqZNpFdz552Y,6029
 weasypdf/management/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 weasypdf/management/commands/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 weasypdf/management/commands/build_test_pdf.py,sha256=HhGlnxo8IqKQvhpZ1QelRz-eQPlO0lNuF5bXzrLuF8E,7055
 weasypdf/static/weasypdf/images/header_left.png,sha256=HuJkygMqahGPGBedtlUG3ja7N19zI-eowQVv8Yfk3PM,13320
 weasypdf/templates/weasypdf/base.html,sha256=xJvIafKRl1h0ApHCwV7hOlDxSEoHY47LDL4M31r14cw,707
 weasypdf/templates/weasypdf/base_nomargins.html,sha256=_3fWaIlg6exEZReQ3fkkf_ifnxSUL_NjIldlXZoswDk,707
 weasypdf/templates/weasypdf/footer.html,sha256=mwLlOzuLY1Jo8f5iagzHHSZgKb8mtkGCrGBNutm-d5A,536
 weasypdf/templates/weasypdf/header.html,sha256=VN9wfIFiCRiX7rFauWMTljLZ72-nzRTmfXBOcyDh8lE,810
 weasypdf/templates/weasypdf/styles.css,sha256=Q56icgKW0EDZfgrMTY0EqUoUtaQrHxNvrB1KhgDkMuk,890
 weasypdf/templates/weasypdf/pages/test.css,sha256=15R5nH8khpS05pw2uvYP73CH_aUSiU1tHueANH71kPI,26
 weasypdf/templates/weasypdf/pages/test.html,sha256=g3lZl9W5eAJJOKlp7M24MDIDsURP2Q1VTP9Y1z3A2Iw,481
-django_weasypdf-0.1.1.dist-info/LICENSE,sha256=SJoJwqjgSuZlqj4Y9yX-Fmk68xeWaxN6RTOjWWuuoy4,1065
-django_weasypdf-0.1.1.dist-info/METADATA,sha256=Snj9uU3dLjYIHb5uJvOT_U8X6B0wRGkYS8QWRGKHHGg,15439
-django_weasypdf-0.1.1.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-django_weasypdf-0.1.1.dist-info/top_level.txt,sha256=DIwLfV9Jp6icEYW8F_r6wmy8E6mL6Fmp-Day1AeG_Dw,9
-django_weasypdf-0.1.1.dist-info/RECORD,,
+django_weasypdf-0.1.2.dist-info/LICENSE,sha256=SJoJwqjgSuZlqj4Y9yX-Fmk68xeWaxN6RTOjWWuuoy4,1065
+django_weasypdf-0.1.2.dist-info/METADATA,sha256=s44_6HmG_hbPbGwXi1rB4XObuigrpIl1K2bzAFt-I-k,15745
+django_weasypdf-0.1.2.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+django_weasypdf-0.1.2.dist-info/top_level.txt,sha256=DIwLfV9Jp6icEYW8F_r6wmy8E6mL6Fmp-Day1AeG_Dw,9
+django_weasypdf-0.1.2.dist-info/RECORD,,
```

