# Comparing `tmp/unstructured_inference-0.4.0.tar.gz` & `tmp/unstructured_inference-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured_inference-0.4.0.tar", last modified: Fri Apr 14 21:36:53 2023, max compression
+gzip compressed data, was "unstructured_inference-0.4.1.tar", last modified: Thu Apr 20 17:38:11 2023, max compression
```

## Comparing `unstructured_inference-0.4.0.tar` & `unstructured_inference-0.4.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:36:53.257323 unstructured_inference-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-04-14 21:36:53.257323 unstructured_inference-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:36:53.253322 unstructured_inference-0.4.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-14 21:36:53.257323 unstructured_inference-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:36:53.253322 unstructured_inference-0.4.0/unstructured_inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:36:53.253322 unstructured_inference-0.4.0/unstructured_inference/inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/inference/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/inference/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/inference/layoutelement.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:36:53.257323 unstructured_inference-0.4.0/unstructured_inference/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/models/detectron2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/models/donut.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/models/paddle_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)    24106 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/models/table_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    23850 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/models/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/models/tesseract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/models/unstructuredmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/models/yolox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:36:53.253322 unstructured_inference-0.4.0/unstructured_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-04-14 21:36:53.000000 unstructured_inference-0.4.0/unstructured_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-14 21:36:53.000000 unstructured_inference-0.4.0/unstructured_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:36:53.000000 unstructured_inference-0.4.0/unstructured_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-14 21:36:53.000000 unstructured_inference-0.4.0/unstructured_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 21:36:53.000000 unstructured_inference-0.4.0/unstructured_inference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:38:11.517226 unstructured_inference-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-04-20 17:38:11.517226 unstructured_inference-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:38:11.513226 unstructured_inference-0.4.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-20 17:38:11.521226 unstructured_inference-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:38:11.513226 unstructured_inference-0.4.1/unstructured_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:38:11.517226 unstructured_inference-0.4.1/unstructured_inference/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/inference/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/inference/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/inference/layoutelement.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:38:11.517226 unstructured_inference-0.4.1/unstructured_inference/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/models/detectron2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/models/donut.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/models/paddle_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24106 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/models/table_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23850 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/models/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/models/tesseract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/models/unstructuredmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/models/yolox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-04-20 17:36:12.000000 unstructured_inference-0.4.1/unstructured_inference/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:38:11.513226 unstructured_inference-0.4.1/unstructured_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-04-20 17:38:11.000000 unstructured_inference-0.4.1/unstructured_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-20 17:38:11.000000 unstructured_inference-0.4.1/unstructured_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 17:38:11.000000 unstructured_inference-0.4.1/unstructured_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-20 17:38:11.000000 unstructured_inference-0.4.1/unstructured_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 17:38:11.000000 unstructured_inference-0.4.1/unstructured_inference.egg-info/top_level.txt
```

### Comparing `unstructured_inference-0.4.0/PKG-INFO` & `unstructured_inference-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured_inference
-Version: 0.4.0
+Version: 0.4.1
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

### Comparing `unstructured_inference-0.4.0/README.md` & `unstructured_inference-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.0/setup.py` & `unstructured_inference-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.0/unstructured_inference/api.py` & `unstructured_inference-0.4.1/unstructured_inference/api.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.0/unstructured_inference/inference/elements.py` & `unstructured_inference-0.4.1/unstructured_inference/inference/elements.py`

 * *Files 6% similar despite different names*

```diff
@@ -158,25 +158,26 @@
 
     def extract_text(
         self,
         objects: Optional[List[TextRegion]],
         image: Optional[Image.Image] = None,
         extract_tables: bool = False,
         ocr_strategy: str = "auto",
+        ocr_languages: str = "eng",
     ) -> str:
         """Extracts text contained in region."""
         if self.text is not None:
             # If block text is already populated, we'll assume it's correct
             text = self.text
         elif objects is not None:
             text = aggregate_by_block(self, image, objects, ocr_strategy)
         elif image is not None:
             if ocr_strategy != "never":
                 # We don't have anything to go on but the image itself, so we use OCR
-                text = ocr(self, image)
+                text = ocr(self, image, languages=ocr_languages)
             else:
                 text = ""
         else:
             raise ValueError(
                 "Got arguments image and layout as None, at least one must be populated to use for "
                 "text extraction."
             )
@@ -186,14 +187,15 @@
 class EmbeddedTextRegion(TextRegion):
     def extract_text(
         self,
         objects: Optional[List[TextRegion]],
         image: Optional[Image.Image] = None,
         extract_tables: bool = False,
         ocr_strategy: str = "auto",
+        ocr_languages: str = "eng",
     ) -> str:
         """Extracts text contained in region."""
         if self.text is None:
             return ""
         else:
             return self.text
 
@@ -201,32 +203,36 @@
 class ImageTextRegion(TextRegion):
     def extract_text(
         self,
         objects: Optional[List[TextRegion]],
         image: Optional[Image.Image] = None,
         extract_tables: bool = False,
         ocr_strategy: str = "auto",
+        ocr_languages: str = "eng",
     ) -> str:
         """Extracts text contained in region."""
         if self.text is None:
             if ocr_strategy == "never" or image is None:
                 return ""
             else:
-                return ocr(self, image)
+                return ocr(self, image, languages=ocr_languages)
         else:
             return super().extract_text(objects, image, extract_tables, ocr_strategy)
 
 
-def ocr(text_block: TextRegion, image: Image.Image) -> str:
+def ocr(text_block: TextRegion, image: Image.Image, languages: str = "eng") -> str:
     """Runs a cropped text block image through and OCR agent."""
     logger.debug("Running OCR on text block ...")
-    tesseract.load_agent()
+    tesseract.load_agent(languages=languages)
     padded_block = text_block.pad(12)
     cropped_image = image.crop((padded_block.x1, padded_block.y1, padded_block.x2, padded_block.y2))
-    return tesseract.ocr_agent.detect(cropped_image)
+    agent = tesseract.ocr_agents.get(languages)
+    if agent is None:
+        raise RuntimeError("OCR agent is not loaded for {languages}.")
+    return agent.detect(cropped_image)
 
 
 def needs_ocr(
     region: TextRegion,
     pdf_objects: List[TextRegion],
     ocr_strategy: str,
 ) -> bool:
@@ -259,24 +265,25 @@
 
 
 def aggregate_by_block(
     text_region: TextRegion,
     image: Optional[Image.Image],
     pdf_objects: List[TextRegion],
     ocr_strategy: str = "auto",
+    ocr_languages: str = "eng",
 ) -> str:
     """Extracts the text aggregated from the elements of the given layout that lie within the given
     block."""
     if image is not None and needs_ocr(text_region, pdf_objects, ocr_strategy):
-        text = ocr(text_region, image)
+        text = ocr(text_region, image, languages=ocr_languages)
     else:
         filtered_blocks = [obj for obj in pdf_objects if obj.is_in(text_region, error_margin=5)]
         for little_block in filtered_blocks:
             if image is not None and needs_ocr(little_block, pdf_objects, ocr_strategy):
-                little_block.text = ocr(little_block, image)
+                little_block.text = ocr(little_block, image, languages=ocr_languages)
         text = " ".join([x.text for x in filtered_blocks if x.text])
     text = remove_control_characters(text)
     return text
 
 
 def cid_ratio(text: str) -> float:
     """Gets ratio of unknown 'cid' characters extracted from text to all characters."""
```

### Comparing `unstructured_inference-0.4.0/unstructured_inference/inference/layout.py` & `unstructured_inference-0.4.1/unstructured_inference/inference/layout.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     @classmethod
     def from_file(
         cls,
         filename: str,
         model: Optional[UnstructuredModel] = None,
         fixed_layouts: Optional[List[Optional[List[TextRegion]]]] = None,
         ocr_strategy: str = "auto",
+        ocr_languages: str = "eng",
         extract_tables: bool = False,
     ) -> DocumentLayout:
         """Creates a DocumentLayout from a pdf file."""
         logger.info(f"Reading PDF for file: {filename} ...")
         layouts, images = load_pdf(filename)
         if len(layouts) > len(images):
             raise RuntimeError(
@@ -71,26 +72,28 @@
             # NOTE(robinson) - In the future, maybe we detect the page number and default
             # to the index if it is not detected
             page = PageLayout.from_image(
                 image,
                 model=model,
                 layout=layout,
                 ocr_strategy=ocr_strategy,
+                ocr_languages=ocr_languages,
                 fixed_layout=fixed_layout,
                 extract_tables=extract_tables,
             )
             pages.append(page)
         return cls.from_pages(pages)
 
     @classmethod
     def from_image_file(
         cls,
         filename: str,
         model: Optional[UnstructuredModel] = None,
         ocr_strategy: str = "auto",
+        ocr_languages: str = "eng",
         fixed_layout: Optional[List[TextRegion]] = None,
         extract_tables: bool = False,
     ) -> DocumentLayout:
         """Creates a DocumentLayout from an image file."""
         logger.info(f"Reading image file: {filename} ...")
         try:
             image = Image.open(filename).convert("RGB")
@@ -100,14 +103,15 @@
             else:
                 raise FileNotFoundError(f'File "{filename}" not found!') from e
         page = PageLayout.from_image(
             image,
             model=model,
             layout=None,
             ocr_strategy=ocr_strategy,
+            ocr_languages=ocr_languages,
             fixed_layout=fixed_layout,
             extract_tables=extract_tables,
         )
         return cls.from_pages([page])
 
 
 class PageLayout:
@@ -116,25 +120,27 @@
     def __init__(
         self,
         number: int,
         image: Image.Image,
         layout: Optional[List[TextRegion]],
         model: Optional[UnstructuredModel] = None,
         ocr_strategy: str = "auto",
+        ocr_languages: str = "eng",
         extract_tables: bool = False,
     ):
         self.image = image
         self.image_array: Union[np.ndarray, None] = None
         self.layout = layout
         self.number = number
         self.model = model
         self.elements: List[LayoutElement] = list()
         if ocr_strategy not in VALID_OCR_STRATEGIES:
             raise ValueError(f"ocr_strategy must be one of {VALID_OCR_STRATEGIES}.")
         self.ocr_strategy = ocr_strategy
+        self.ocr_languages = ocr_languages
         self.extract_tables = extract_tables
 
     def __str__(self) -> str:
         return "\n\n".join([str(element) for element in self.elements])
 
     def get_elements_with_model(self, inplace=True) -> Optional[List[LayoutElement]]:
         """Uses specified model to detect the elements on the page."""
@@ -155,15 +161,20 @@
         """Uses the given Layout to separate the page text into elements, either extracting the
         text from the discovered layout blocks or from the image using OCR."""
         # NOTE(robinson) - This orders the page from top to bottom. We'll need more
         # sophisticated ordering logic for more complicated layouts.
         layout.sort(key=lambda element: element.y1)
         elements = [
             get_element_from_block(
-                e, self.image, self.layout, self.ocr_strategy, self.extract_tables
+                block=e,
+                image=self.image,
+                pdf_objects=self.layout,
+                ocr_strategy=self.ocr_strategy,
+                ocr_languages=self.ocr_languages,
+                extract_tables=self.extract_tables,
             )
             for e in layout
         ]
         return elements
 
     def _get_image_array(self) -> Union[np.ndarray, None]:
         """Converts the raw image into a numpy array."""
@@ -174,96 +185,111 @@
     @classmethod
     def from_image(
         cls,
         image,
         model: Optional[UnstructuredModel] = None,
         layout: Optional[List[TextRegion]] = None,
         ocr_strategy: str = "auto",
+        ocr_languages: str = "eng",
         extract_tables: bool = False,
         fixed_layout: Optional[List[TextRegion]] = None,
     ):
         """Creates a PageLayout from an already-loaded PIL Image."""
         page = cls(
             number=0,
             image=image,
             layout=layout,
             model=model,
             ocr_strategy=ocr_strategy,
+            ocr_languages=ocr_languages,
             extract_tables=extract_tables,
         )
         if fixed_layout is None:
             page.get_elements_with_model()
         else:
             page.elements = page.get_elements_from_layout(fixed_layout)
         return page
 
 
 def process_data_with_model(
     data: BinaryIO,
     model_name: Optional[str],
     is_image: bool = False,
     ocr_strategy: str = "auto",
+    ocr_languages: str = "eng",
     fixed_layouts: Optional[List[Optional[List[TextRegion]]]] = None,
     extract_tables: bool = False,
 ) -> DocumentLayout:
     """Processes pdf file in the form of a file handler (supporting a read method) into a
     DocumentLayout by using a model identified by model_name."""
     with tempfile.NamedTemporaryFile() as tmp_file:
         tmp_file.write(data.read())
         layout = process_file_with_model(
             tmp_file.name,
             model_name,
             is_image=is_image,
             ocr_strategy=ocr_strategy,
+            ocr_languages=ocr_languages,
             fixed_layouts=fixed_layouts,
             extract_tables=extract_tables,
         )
 
     return layout
 
 
 def process_file_with_model(
     filename: str,
     model_name: Optional[str],
     is_image: bool = False,
     ocr_strategy: str = "auto",
+    ocr_languages: str = "eng",
     fixed_layouts: Optional[List[Optional[List[TextRegion]]]] = None,
     extract_tables: bool = False,
 ) -> DocumentLayout:
     """Processes pdf file with name filename into a DocumentLayout by using a model identified by
     model_name."""
     model = get_model(model_name)
     layout = (
         DocumentLayout.from_image_file(
-            filename, model=model, ocr_strategy=ocr_strategy, extract_tables=extract_tables
+            filename,
+            model=model,
+            ocr_strategy=ocr_strategy,
+            ocr_languages=ocr_languages,
+            extract_tables=extract_tables,
         )
         if is_image
         else DocumentLayout.from_file(
             filename,
             model=model,
             ocr_strategy=ocr_strategy,
+            ocr_languages=ocr_languages,
             fixed_layouts=fixed_layouts,
             extract_tables=extract_tables,
         )
     )
     return layout
 
 
 def get_element_from_block(
     block: TextRegion,
     image: Optional[Image.Image] = None,
     pdf_objects: Optional[List[TextRegion]] = None,
     ocr_strategy: str = "auto",
+    ocr_languages: str = "eng",
     extract_tables: bool = False,
 ) -> LayoutElement:
     """Creates a LayoutElement from a given layout or image by finding all the text that lies within
     a given block."""
     element = LayoutElement.from_region(block)
     element.text = block.extract_text(
-        objects=pdf_objects, image=image, extract_tables=extract_tables, ocr_strategy=ocr_strategy
+        objects=pdf_objects,
+        image=image,
+        extract_tables=extract_tables,
+        ocr_strategy=ocr_strategy,
+        ocr_languages=ocr_languages,
     )
     return element
 
 
 def load_pdf(
     filename: str,
     x_tolerance: Union[int, float] = 1.5,
```

### Comparing `unstructured_inference-0.4.0/unstructured_inference/inference/layoutelement.py` & `unstructured_inference-0.4.1/unstructured_inference/inference/layoutelement.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,27 +15,29 @@
 
     def extract_text(
         self,
         objects: Optional[List[TextRegion]],
         image: Optional[Image.Image] = None,
         extract_tables: bool = False,
         ocr_strategy: str = "auto",
+        ocr_languages: str = "eng",
     ):
         """Extracts text contained in region"""
         if self.text is not None:
             # If block text is already populated, we'll assume it's correct
             text = self.text
         elif extract_tables and isinstance(self, LayoutElement) and self.type == "Table":
             text = interprete_table_block(self, image)
         else:
             text = super().extract_text(
                 objects=objects,
                 image=image,
                 extract_tables=extract_tables,
                 ocr_strategy=ocr_strategy,
+                ocr_languages=ocr_languages,
             )
         return text
 
     def to_dict(self) -> dict:
         """Converts the class instance to dictionary form."""
         out_dict = {
             "coordinates": self.coordinates,
```

### Comparing `unstructured_inference-0.4.0/unstructured_inference/models/base.py` & `unstructured_inference-0.4.1/unstructured_inference/models/base.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.0/unstructured_inference/models/detectron2.py` & `unstructured_inference-0.4.1/unstructured_inference/models/detectron2.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.0/unstructured_inference/models/donut.py` & `unstructured_inference-0.4.1/unstructured_inference/models/donut.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.0/unstructured_inference/models/table_postprocess.py` & `unstructured_inference-0.4.1/unstructured_inference/models/table_postprocess.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.0/unstructured_inference/models/tables.py` & `unstructured_inference-0.4.1/unstructured_inference/models/tables.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.0/unstructured_inference/models/unstructuredmodel.py` & `unstructured_inference-0.4.1/unstructured_inference/models/unstructuredmodel.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.0/unstructured_inference/models/yolox.py` & `unstructured_inference-0.4.1/unstructured_inference/models/yolox.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.0/unstructured_inference/utils.py` & `unstructured_inference-0.4.1/unstructured_inference/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.0/unstructured_inference/visualize.py` & `unstructured_inference-0.4.1/unstructured_inference/visualize.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.0/unstructured_inference.egg-info/PKG-INFO` & `unstructured_inference-0.4.1/unstructured_inference.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured-inference
-Version: 0.4.0
+Version: 0.4.1
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

### Comparing `unstructured_inference-0.4.0/unstructured_inference.egg-info/SOURCES.txt` & `unstructured_inference-0.4.1/unstructured_inference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

