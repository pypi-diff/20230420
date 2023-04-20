# Comparing `tmp/a2-0.3.tar.gz` & `tmp/a2-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a2-0.3.tar", max compression
+gzip compressed data, was "a2-0.3.2.tar", max compression
```

## Comparing `a2-0.3.tar` & `a2-0.3.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     3467 2023-03-27 12:15:56.086413 a2-0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-20 15:29:54.345253 a2-0.3/src/a2/__init__.py
--rw-r--r--   0        0        0       45 2023-01-13 09:43:31.404482 a2-0.3/src/a2/cli/__init__.py
--rw-r--r--   0        0        0       39 2023-01-13 09:45:19.522669 a2-0.3/src/a2/cli/cli_plotting/__init__.py
--rw-r--r--   0        0        0      107 2023-01-13 09:46:23.599985 a2-0.3/src/a2/cli/cli_plotting/plot.py
--rw-r--r--   0        0        0     2056 2023-02-16 10:12:08.320539 a2-0.3/src/a2/cli/cli_plotting/single_plots.py
--rw-r--r--   0        0        0       66 2023-01-13 09:36:10.235731 a2-0.3/src/a2/cli/main.py
--rw-r--r--   0        0        0        0 2022-11-01 14:44:14.720032 a2-0.3/src/a2/data/__init__.py
--rw-r--r--   0        0        0        0 2022-11-01 14:44:14.720032 a2-0.3/src/a2/data/emoji/__init__.py
--rw-r--r--   0        0        0   379747 2022-11-01 14:44:14.724032 a2-0.3/src/a2/data/emoji/emoji_df.csv
--rw-r--r--   0        0        0        0 2022-11-01 14:44:14.724032 a2-0.3/src/a2/data/vocabularies/__init__.py
--rw-r--r--   0        0        0     2789 2023-02-21 08:27:21.563839 a2-0.3/src/a2/data/vocabularies/weather_vocab_enchanted_learning_com.txt
--rw-r--r--   0        0        0      236 2023-02-21 08:27:21.563869 a2-0.3/src/a2/data/vocabularies/weather_vocab_enchanted_precipitation.txt
--rw-r--r--   0        0        0      188 2023-02-21 14:04:17.568649 a2-0.3/src/a2/dataset/__init__.py
--rw-r--r--   0        0        0      556 2023-01-30 14:59:51.635141 a2-0.3/src/a2/dataset/emojis.py
--rw-r--r--   0        0        0     7525 2023-02-20 13:53:30.152744 a2-0.3/src/a2/dataset/load_dataset.py
--rw-r--r--   0        0        0    50068 2023-01-30 14:59:51.635141 a2-0.3/src/a2/dataset/radar.py
--rw-r--r--   0        0        0    10354 2023-01-30 14:59:51.635141 a2-0.3/src/a2/dataset/stations.py
--rw-r--r--   0        0        0      699 2023-02-20 13:53:30.152744 a2-0.3/src/a2/dataset/tweets.py
--rw-r--r--   0        0        0     1464 2022-12-14 09:36:33.150856 a2-0.3/src/a2/dataset/units.py
--rw-r--r--   0        0        0    16914 2023-02-15 13:23:54.265629 a2-0.3/src/a2/dataset/utils_dataset.py
--rw-r--r--   0        0        0      191 2022-12-14 09:36:33.150856 a2-0.3/src/a2/plotting/__init__.py
--rw-r--r--   0        0        0     8266 2023-03-03 16:00:04.992588 a2-0.3/src/a2/plotting/analysis.py
--rw-r--r--   0        0        0     1964 2023-02-14 14:11:41.262470 a2-0.3/src/a2/plotting/axes_utils.py
--rw-r--r--   0        0        0    28393 2023-03-03 15:58:05.697968 a2-0.3/src/a2/plotting/histograms.py
--rw-r--r--   0        0        0     3007 2022-12-14 09:36:33.154856 a2-0.3/src/a2/plotting/parallel_plotting.py
--rw-r--r--   0        0        0     2809 2022-12-14 09:36:33.154856 a2-0.3/src/a2/plotting/timeseries.py
--rw-r--r--   0        0        0    16032 2023-03-03 15:56:41.072135 a2-0.3/src/a2/plotting/utils_plotting.py
--rw-r--r--   0        0        0    34741 2023-02-20 13:53:30.156744 a2-0.3/src/a2/plotting/weather_maps.py
--rw-r--r--   0        0        0       67 2022-11-01 14:44:14.724032 a2-0.3/src/a2/preprocess/__init__.py
--rw-r--r--   0        0        0     3645 2022-12-06 08:38:01.708129 a2-0.3/src/a2/preprocess/embedding.py
--rw-r--r--   0        0        0    29471 2022-12-06 08:38:01.708129 a2-0.3/src/a2/preprocess/normalize_text.py
--rw-r--r--   0        0        0      172 2023-03-03 15:56:22.067727 a2-0.3/src/a2/training/__init__.py
--rw-r--r--   0        0        0     3540 2023-03-27 11:05:29.221905 a2-0.3/src/a2/training/benchmarks.py
--rw-r--r--   0        0        0     2556 2022-12-14 09:36:33.154856 a2-0.3/src/a2/training/dataset_hugging.py
--rw-r--r--   0        0        0     4131 2023-02-02 13:31:55.647577 a2-0.3/src/a2/training/evaluate_hugging.py
--rw-r--r--   0        0        0     4311 2023-03-16 14:07:38.180150 a2-0.3/src/a2/training/tracking.py
--rw-r--r--   0        0        0     1721 2023-03-03 17:10:05.441361 a2-0.3/src/a2/training/tracking_hugging.py
--rw-r--r--   0        0        0     6390 2023-03-02 16:51:55.930811 a2-0.3/src/a2/training/training_deep500.py
--rw-r--r--   0        0        0     8656 2023-03-23 14:07:56.848122 a2-0.3/src/a2/training/training_hugging.py
--rw-r--r--   0        0        0       73 2023-01-30 14:59:51.639141 a2-0.3/src/a2/training/utils_training.py
--rw-r--r--   0        0        0       87 2022-11-01 14:44:14.728032 a2-0.3/src/a2/twitter/__init__.py
--rw-r--r--   0        0        0     4570 2023-02-20 13:53:30.156744 a2-0.3/src/a2/twitter/downloader.py
--rw-r--r--   0        0        0    11233 2023-02-20 13:53:30.156744 a2-0.3/src/a2/twitter/locations.py
--rw-r--r--   0        0        0     6765 2023-02-20 13:53:30.156744 a2-0.3/src/a2/twitter/twitter_api.py
--rw-r--r--   0        0        0      147 2022-12-14 09:36:33.154856 a2-0.3/src/a2/utils/__init__.py
--rw-r--r--   0        0        0      518 2022-12-14 09:36:33.154856 a2-0.3/src/a2/utils/checks.py
--rw-r--r--   0        0        0      362 2023-02-20 15:01:52.076201 a2-0.3/src/a2/utils/constants.py
--rw-r--r--   0        0        0     9177 2023-03-15 09:45:11.698161 a2-0.3/src/a2/utils/file_handling.py
--rw-r--r--   0        0        0     5220 2023-02-20 13:53:30.156744 a2-0.3/src/a2/utils/testing.py
--rw-r--r--   0        0        0      394 2022-12-14 09:36:33.154856 a2-0.3/src/a2/utils/times.py
--rw-r--r--   0        0        0     6044 2023-03-03 15:56:22.027726 a2-0.3/src/a2/utils/utils.py
--rw-r--r--   0        0        0     1874 1970-01-01 00:00:00.000000 a2-0.3/setup.py
--rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 a2-0.3/PKG-INFO
+-rw-r--r--   0        0        0     3769 2023-04-20 06:31:32.717643 a2-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-20 15:29:54.345253 a2-0.3.2/src/a2/__init__.py
+-rw-r--r--   0        0        0       45 2023-01-13 09:43:31.404482 a2-0.3.2/src/a2/cli/__init__.py
+-rw-r--r--   0        0        0       39 2023-01-13 09:45:19.522669 a2-0.3.2/src/a2/cli/cli_plotting/__init__.py
+-rw-r--r--   0        0        0      107 2023-01-13 09:46:23.599985 a2-0.3.2/src/a2/cli/cli_plotting/plot.py
+-rw-r--r--   0        0        0     2056 2023-02-16 10:12:08.320539 a2-0.3.2/src/a2/cli/cli_plotting/single_plots.py
+-rw-r--r--   0        0        0       66 2023-01-13 09:36:10.235731 a2-0.3.2/src/a2/cli/main.py
+-rw-r--r--   0        0        0        0 2022-11-01 14:44:14.720032 a2-0.3.2/src/a2/data/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-01 14:44:14.720032 a2-0.3.2/src/a2/data/emoji/__init__.py
+-rw-r--r--   0        0        0   379747 2022-11-01 14:44:14.724032 a2-0.3.2/src/a2/data/emoji/emoji_df.csv
+-rw-r--r--   0        0        0        0 2022-11-01 14:44:14.724032 a2-0.3.2/src/a2/data/vocabularies/__init__.py
+-rw-r--r--   0        0        0     2789 2023-02-21 08:27:21.563839 a2-0.3.2/src/a2/data/vocabularies/weather_vocab_enchanted_learning_com.txt
+-rw-r--r--   0        0        0      236 2023-02-21 08:27:21.563869 a2-0.3.2/src/a2/data/vocabularies/weather_vocab_enchanted_precipitation.txt
+-rw-r--r--   0        0        0      188 2023-02-21 14:04:17.568649 a2-0.3.2/src/a2/dataset/__init__.py
+-rw-r--r--   0        0        0      556 2023-01-30 14:59:51.635141 a2-0.3.2/src/a2/dataset/emojis.py
+-rw-r--r--   0        0        0     7525 2023-02-20 13:53:30.152744 a2-0.3.2/src/a2/dataset/load_dataset.py
+-rw-r--r--   0        0        0    50068 2023-01-30 14:59:51.635141 a2-0.3.2/src/a2/dataset/radar.py
+-rw-r--r--   0        0        0    10354 2023-01-30 14:59:51.635141 a2-0.3.2/src/a2/dataset/stations.py
+-rw-r--r--   0        0        0      699 2023-02-20 13:53:30.152744 a2-0.3.2/src/a2/dataset/tweets.py
+-rw-r--r--   0        0        0     1464 2022-12-14 09:36:33.150856 a2-0.3.2/src/a2/dataset/units.py
+-rw-r--r--   0        0        0    16914 2023-02-15 13:23:54.265629 a2-0.3.2/src/a2/dataset/utils_dataset.py
+-rw-r--r--   0        0        0      191 2022-12-14 09:36:33.150856 a2-0.3.2/src/a2/plotting/__init__.py
+-rw-r--r--   0        0        0     8266 2023-03-03 16:00:04.992588 a2-0.3.2/src/a2/plotting/analysis.py
+-rw-r--r--   0        0        0     1964 2023-02-14 14:11:41.262470 a2-0.3.2/src/a2/plotting/axes_utils.py
+-rw-r--r--   0        0        0    29338 2023-04-12 11:32:44.371869 a2-0.3.2/src/a2/plotting/histograms.py
+-rw-r--r--   0        0        0     3007 2022-12-14 09:36:33.154856 a2-0.3.2/src/a2/plotting/parallel_plotting.py
+-rw-r--r--   0        0        0     2809 2022-12-14 09:36:33.154856 a2-0.3.2/src/a2/plotting/timeseries.py
+-rw-r--r--   0        0        0    16032 2023-03-03 15:56:41.072135 a2-0.3.2/src/a2/plotting/utils_plotting.py
+-rw-r--r--   0        0        0    34741 2023-02-20 13:53:30.156744 a2-0.3.2/src/a2/plotting/weather_maps.py
+-rw-r--r--   0        0        0       67 2022-11-01 14:44:14.724032 a2-0.3.2/src/a2/preprocess/__init__.py
+-rw-r--r--   0        0        0     3645 2022-12-06 08:38:01.708129 a2-0.3.2/src/a2/preprocess/embedding.py
+-rw-r--r--   0        0        0    29471 2022-12-06 08:38:01.708129 a2-0.3.2/src/a2/preprocess/normalize_text.py
+-rw-r--r--   0        0        0      172 2023-03-03 15:56:22.067727 a2-0.3.2/src/a2/training/__init__.py
+-rw-r--r--   0        0        0     3618 2023-04-20 06:29:52.911455 a2-0.3.2/src/a2/training/benchmarks.py
+-rw-r--r--   0        0        0     2556 2022-12-14 09:36:33.154856 a2-0.3.2/src/a2/training/dataset_hugging.py
+-rw-r--r--   0        0        0     4131 2023-02-02 13:31:55.647577 a2-0.3.2/src/a2/training/evaluate_hugging.py
+-rw-r--r--   0        0        0     4421 2023-04-12 09:53:21.965604 a2-0.3.2/src/a2/training/tracking.py
+-rw-r--r--   0        0        0     1780 2023-04-12 09:29:10.503408 a2-0.3.2/src/a2/training/tracking_hugging.py
+-rw-r--r--   0        0        0     6390 2023-03-02 16:51:55.930811 a2-0.3.2/src/a2/training/training_deep500.py
+-rw-r--r--   0        0        0     8949 2023-04-12 09:53:21.577595 a2-0.3.2/src/a2/training/training_hugging.py
+-rw-r--r--   0        0        0     6821 2023-04-17 13:38:37.032507 a2-0.3.2/src/a2/training/training_performance.py
+-rw-r--r--   0        0        0       73 2023-01-30 14:59:51.639141 a2-0.3.2/src/a2/training/utils_training.py
+-rw-r--r--   0        0        0       87 2022-11-01 14:44:14.728032 a2-0.3.2/src/a2/twitter/__init__.py
+-rw-r--r--   0        0        0     4570 2023-02-20 13:53:30.156744 a2-0.3.2/src/a2/twitter/downloader.py
+-rw-r--r--   0        0        0    11233 2023-02-20 13:53:30.156744 a2-0.3.2/src/a2/twitter/locations.py
+-rw-r--r--   0        0        0     6765 2023-02-20 13:53:30.156744 a2-0.3.2/src/a2/twitter/twitter_api.py
+-rw-r--r--   0        0        0      147 2022-12-14 09:36:33.154856 a2-0.3.2/src/a2/utils/__init__.py
+-rw-r--r--   0        0        0      518 2022-12-14 09:36:33.154856 a2-0.3.2/src/a2/utils/checks.py
+-rw-r--r--   0        0        0      362 2023-02-20 15:01:52.076201 a2-0.3.2/src/a2/utils/constants.py
+-rw-r--r--   0        0        0     9181 2023-04-12 10:07:20.603125 a2-0.3.2/src/a2/utils/file_handling.py
+-rw-r--r--   0        0        0     5220 2023-04-19 06:56:16.631322 a2-0.3.2/src/a2/utils/testing.py
+-rw-r--r--   0        0        0      394 2022-12-14 09:36:33.154856 a2-0.3.2/src/a2/utils/times.py
+-rw-r--r--   0        0        0     6044 2023-03-03 15:56:22.027726 a2-0.3.2/src/a2/utils/utils.py
+-rw-r--r--   0        0        0     1887 1970-01-01 00:00:00.000000 a2-0.3.2/PKG-INFO
```

### Comparing `a2-0.3/pyproject.toml` & `a2-0.3.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,94 +1,100 @@
 [tool.poetry]
 name = "a2"
-version = "0.3"
+version = "0.3.2"
 description = "Package for predicting information about the weather from social media data as application 2 for maelstrom project"
 authors = ["Kristian Ehlert <kristian.ehlert@4-cast.de>"]
 packages = [{ include = "a2", from = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 jupyterlab = "^3.4.3"
 requests = "^2.28.1"
 pandas = "^1.4.2"
 DateTime = "^4.4"
 matplotlib = "^3.5.2"
 xarray = "^2022.3.0"
 emoji = "<1.0.0"
 dask = "^2022.6.1"
-pytest-recording = "^0.12.1"
 ipywidgets = "^7.7.1"
 spacymoji = "^3.0.1"
 wget = "^3.2"
 jsonlines = "^3.1.0"
 tweepy = "^4.10.0"
 Shapely = "^1.8.2"
 pyproj = "^3.3.1"
 h5py = "^3.7.0"
 netCDF4 = "^1.6.0"
 h5netcdf = "^1.0.1"
 mantik = "^0.1.0"
-pytest-xdist = "^2.5.0"
 urllib3 = "^1.26.12"
 scikit-learn = "^1.1.2"
 kaleido = "0.2.1"
 rioxarray = "^0.12.2"
 rasterio = "^1.3.3"
 convertbng = "^0.6.39"
 plotly = "^5.11.0"
 seaborn = "^0.12.1"
 geopy = "^2.3.0"
 click = "^8.1.3"
 ipython = "^8.7.0"
+llvmlite = "^0.39.1"
+datasets = "^2.11.0"
+#transformers = {git = "https://github.com/huggingface/transformers", branch = "main", optional = true }
+torch = {version = "^2.0.0", optional = true}
+sentencepiece = {version = "^0.1.98", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "^22.6.0"}
 mypy = "^0.971"
 reorder-python-imports = "^3.1.0"
 types-python-dateutil = "^2.8.18"
 types-requests = "^2.28.0"
 pandas-stubs = "^1.4.2"
 pytest = "^7.1.2"
 pytest-cov = "^3.0.0"
 pytest-cases = "^3.6.13"
+pytest-recording = "^0.12.1"
+pytest-xdist = "^2.5.0"
 types-tqdm = "^4.64.4"
 line-profiler = {extras = ["ipython"], version = "^3.5.1"}
 pyflakes = "^2.5.0"
 traceback-with-variables = "^2.0.4"
 sacremoses = "^0.0.53"
 deepdiff = "^5.8.1"
 guppy3 = "^3.1.2"
 memory-profiler = "^0.60.0"
 pre-commit = "^2.20.0"
 docformatter = "^1.5.0"
 pytest-mpl = "^0.16.1"
 responses = "0.18"
 pytest-mock = "^3.10.0"
 
+[tool.poetry.extras]
+llama-chatbot = ["transformers", "sentencepiece"]
+torch = ["torch"]
 
 [tool.poetry.group.parallel.dependencies]
 p-tqdm = "^1.4.0"
 
-
+[tool.poetry.group.train]
+optional = true
 [tool.poetry.group.train.dependencies]
 xgboost = "^1.6.2"
 catboost = "^1.1"
 nltk = "^3.7"
 sentence-transformers = "^2.2.2"
-datasets = "^2.7.1"
-transformers = {extras = ["torch"], version = "^4.25.1"}
-sentencepiece = "^0.1.97"
 ray = {extras = ["tune"], version = "^2.2.0"}
 tensorboard = "^2.11.0"
 
 
+[tool.poetry.group.benchmarking]
+optional = true
 [tool.poetry.group.benchmarking.dependencies]
-onnx = "^1.13.0"
 optimum = {extras = ["onnxruntime"], version = "^1.7.1", optional = true}
-transformers = {extras = ["onnx"], version = "^4.27.1"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 a2 = 'a2.cli.main:cli'
@@ -137,19 +143,20 @@
 line-length = 120
 
 [tool.flake8]
 max-line-length = 120
 per-file-ignores = [
     "__init__.py:F401,E501",
     "training_deep500.py:F403,F405",
+    "training_performance.py:F403,F405",
 ]
 
-[tool.poetry.extras]
-extend-exclude = [
-    "notebooks/training/helper_deep500.py"
-]
+# [tool.poetry.extras]
+# extend-exclude = [
+#     "notebooks/training/helper_deep500.py"
+# ]
 
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_level = "INFO"
 log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
 log_cli_date_format = "%Y-%m-%d %H:%M:%S"
```

### Comparing `a2-0.3/src/a2/cli/cli_plotting/single_plots.py` & `a2-0.3.2/src/a2/cli/cli_plotting/single_plots.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/data/emoji/emoji_df.csv` & `a2-0.3.2/src/a2/data/emoji/emoji_df.csv`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/data/vocabularies/weather_vocab_enchanted_learning_com.txt` & `a2-0.3.2/src/a2/data/vocabularies/weather_vocab_enchanted_learning_com.txt`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/dataset/emojis.py` & `a2-0.3.2/src/a2/dataset/emojis.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/dataset/load_dataset.py` & `a2-0.3.2/src/a2/dataset/load_dataset.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/dataset/radar.py` & `a2-0.3.2/src/a2/dataset/radar.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/dataset/stations.py` & `a2-0.3.2/src/a2/dataset/stations.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/dataset/tweets.py` & `a2-0.3.2/src/a2/dataset/tweets.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/dataset/units.py` & `a2-0.3.2/src/a2/dataset/units.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/dataset/utils_dataset.py` & `a2-0.3.2/src/a2/dataset/utils_dataset.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/plotting/analysis.py` & `a2-0.3.2/src/a2/plotting/analysis.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/plotting/axes_utils.py` & `a2-0.3.2/src/a2/plotting/axes_utils.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/plotting/histograms.py` & `a2-0.3.2/src/a2/plotting/histograms.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     ds: xarray.Dataset | None = None,
     bins: t.Sequence | None = None,
     xlim: t.Sequence | None = None,
     ylim: t.Sequence | None = None,
     ax: a2.utils.constants.TYPE_MATPLOTLIB_AXES | None = None,
     ax_colorbar: a2.utils.constants.TYPE_MATPLOTLIB_AXES | None = None,
     log: t.Union[bool, t.List[bool]] = False,
-    filename: t.Union[str, pathlib.Path] = None,
+    filename: str | pathlib.Path | None = None,
     fig: a2.utils.constants.TYPE_MATPLOTLIB_FIGURES | None = None,
     n_bins: t.Union[int, t.List[int]] = 60,
     norm: str | None = None,
     linear_thresh: t.Union[float, t.List[float]] = 1e-9,
     label_x: str | None = None,
     label_y: str | None = None,
     label_colorbar: str | None = None,
@@ -48,20 +48,74 @@
     marginal_y: str = "default",
     marginal_y_label_x: str = "N",
     marginal_y_label_y: bool = False,
     marginal_y_show_yticks: bool = False,
     marginal_color: str | None = "#1f77b4",
     figure_size: t.List[float] | None = None,
     colormap: str = "viridis",
-    colorbar_width=0.02,
-    spacing_x=0.03,
-    spacing_y=0.03,
-    spacing_colorbar=0.03,
+    colorbar_width: float = 0.02,
+    spacing_x: float = 0.03,
+    spacing_y: float = 0.03,
+    spacing_colorbar: float = 0.03,
     title: str = "",
 ):
+    """
+    Plots 2d histogram including histograms in margins
+
+    Log types included `False`, `log`/`True`, `symlog`.
+    Norm takes care of colorbar scale, so far included: `log`
+    Parameters:
+    ----------
+    x: values binned on x-axis
+    y: values binned on y-axis
+    bins: if None computed based on data provided, otherwise should
+          provide [x_edges, y_edges]
+    xlim: limits of x-axis and bin_edges, if None determined from x
+    ylim: limits of y-axis and bin_edges, if None determined from y
+    ax: matplotlib axes for histogram
+    ax_colorbar: matplotlib axes for colorbar
+    log: type of bins
+    filename: plot saved to file if provided
+    fig: matplotlib figure
+    n_bins: number of bins
+    norm: scaling of colorbar
+    linear_thresh: required if using log='symlog' to indicate
+                   where scale turns linear
+    label_x: label of x-axis
+    label_y: label of y-axis
+    label_colorbar: label of colorbar
+    font_size: size of font
+    overplot_values: show number of samples on plot
+    overplot_round_base: Round values to be overplotted to this base int
+    overplot_color: Color of samples to be overplotted
+    vmin: Minimum value of colormap
+    vmax: Maximum value of colormap
+    facet_column: Assign all samples belonging to unique value from this field to histogram as columns
+    facet_row: Assign all samples belonging to unique value from this field to histogram as rows
+    marginal_x: Add additional plot on top of histogram plot ("histogram"/None)
+    marginal_x_label_x: Label along x-axis for plot `marginal_x`
+    marginal_x_label_y: Label along y-axis for plot `marginal_x`
+    marginal_x_show_xticks: Wether to show ticks along the x-axis for plot `marginal_x`
+    marginal_y: Add additional plot on top of histogram plot ("histogram"/None)
+    marginal_y_label_x: Label along x-axis for plot `marginal_y`
+    marginal_y_label_y: Label along y-axis for plot `marginal_y`
+    marginal_y_show_yticks: Wether to show ticks along the y-axis for plot `marginal_y`
+    marginal_color: Color of histogram bars in marginal plots
+    figure_size: Size of figure (height, width), default (10, 6)
+    colormap: Matplotlib colormap name
+    colorbar_width: Width of the colorbars
+    spacing_x: Spacing between axes along horizontal direction
+    spacing_y: Spacing between axes along vertical direction
+    spacing_colorbar: Spacing between axes and colorbar axes
+    title: Title of figure
+
+    Returns
+    -------
+    axes, histogram values
+    """
     marginal_x, marginal_y = _resolve_defaults(facet_column, facet_row, marginal_x, marginal_y)
     _check_histogram_parameter_consistency(facet_column, facet_row, marginal_x, marginal_y, ds)
 
     facet_column_values, column_masks, n_facet_column_values, facet_column_title = prepare_facet(ds, facet_column)
     facet_row_values, row_masks, n_facet_row_values, facet_row_title = prepare_facet(ds, facet_row)
 
     n_columns = 1
@@ -255,61 +309,31 @@
     marginal_x_show_xticks: bool = False,
     marginal_y: str = "histogram",
     marginal_y_label_x: str = "N",
     marginal_y_label_y: bool = False,
     marginal_y_show_yticks: bool = False,
     marginal_color: str | None = None,
     colormap: str = "viridis",
+    title: None | str = None,
     axes_marginal: list | None = None,
     mask: np.ndarray | None = None,
-    title: None | str = None,
-) -> t.Union[plt.axes, t.Tuple[plt.axes, t.Sequence]]:
+) -> t.Tuple[plt.axes, t.Sequence]:
     """
-    plots 2d histogram
+    Plots 2d histogram
 
-    Log types included `False`, `log`/`True`, `symlog`.
-    Norm takes care of colorbar scale, so far included: `log`
     Parameters:
     ----------
-    x: values binned on x-axis
-    y: values binned on y-axis
-    bins: if None computed based on data provided, otherwise should
-          provide [x_edges, y_edges]
-    xlim: limits of x-axis and bin_edges, if None determined from x
-    ylim: limits of y-axis and bin_edges, if None determined from y
-    ax: matplotlib axes
-    log: type of bins
-    filename: plot saved to file if provided
-    fig: matplotlib figure
-    n_bins: number of bins
-    norm: scaling of colorbar
-    linear_thresh: required if using log='symlog' to indicate
-                   where scale turns linear
-    label_x: label of x-axis
-    label_y: label of y-axis
-    font_size: size of font
-    overplot_values: show number of samples on plot
-    overplot_round_base: Round values to be overplotted to this base int
-    marginal_x: Add additional plot on top of histogram plot ("histogram"/None)
-    marginal_x_label_x: Label along x-axis for plot `marginal_x`
-    marginal_x_label_y: Label along y-axis for plot `marginal_x`
-    marginal_x_show_xticks: Wether to show ticks along the x-axis for plot `marginal_x`
-    marginal_y: Add additional plot on top of histogram plot ("histogram"/None)
-    marginal_y_label_x: Label along x-axis for plot `marginal_y`
-    marginal_y_label_y: Label along y-axis for plot `marginal_y`
-    marginal_y_show_yticks: Wether to show ticks along the y-axis for plot `marginal_y`
-    figure_size: Size of figure (height, width), default (10, 6)
-    colormap: Matplotlib colormap name
+    axes_marginal: Matplotlib axes to plot margins into
     mask: Mask x/y values (required shape same as shape of x/y)
-    vmin: Minimum value of colormap
-    vmax: Maximum value of colormap
+
+    See definition of `plot_histogram_2d` for explanation of same parameters
 
     Returns
     -------
-    axes
+    axes, histogram values
     """
 
     def get_label(label):
         if label is not None and label:
             return label
         else:
             return ""
@@ -523,15 +547,14 @@
     filename: t.Union[str, pathlib.Path] = None,
     fig: t.Optional[plt.figure] = None,
     n_bins: int = 60,
     linear_thresh: t.Optional[float] = None,
     label_x: t.Optional[str] = None,
     label_y: t.Optional[str] = None,
     font_size: int = 12,
-    label: str = None,
     return_plot: bool = False,
     vertical: bool = False,
     alpha: float = 1,
     annotatations_bars: t.Optional[list] = None,
     color: str | None = None,
     min_counts: int = 0,
 ) -> t.Union[plt.axes, t.Tuple[plt.figure, plt.axes]]:
@@ -555,15 +578,14 @@
     norm: scaling of colorbar
     linear_thresh: required if using log='symlog' to indicate where
                    scale turns linear
     label_x: label of x-axis
     label_y: label of y-axis
     font_size: size of font
     alpha: alpha value of plot
-    label: Label of plot
     return_plot: return axes and bar plot object
 
     Returns
     -------
     axes
     """
     if all([isinstance(i, str) for i in x]):
```

### Comparing `a2-0.3/src/a2/plotting/parallel_plotting.py` & `a2-0.3.2/src/a2/plotting/parallel_plotting.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/plotting/timeseries.py` & `a2-0.3.2/src/a2/plotting/timeseries.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/plotting/utils_plotting.py` & `a2-0.3.2/src/a2/plotting/utils_plotting.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/plotting/weather_maps.py` & `a2-0.3.2/src/a2/plotting/weather_maps.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/preprocess/embedding.py` & `a2-0.3.2/src/a2/preprocess/embedding.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/preprocess/normalize_text.py` & `a2-0.3.2/src/a2/preprocess/normalize_text.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/training/benchmarks.py` & `a2-0.3.2/src/a2/training/benchmarks.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 
 
 def current_time():
     return time.time()
 
 
 class Timer:
+    """Interface has analagous implementation to deep500 timer. Therefore not all variables used"""
+
     def __init__(self, print_all_single_time_stats=True, debug=True):
         self.times_archive = {}
         self.times_running = {}
         self.TimeType = TimeType()
         self.debug = debug
         self.print_all_single_time_stats = print_all_single_time_stats
 
@@ -53,16 +55,14 @@
             self._archive_timing(time_type, duration=duration)
             if self.print_all_single_time_stats:
                 logging.info(f"{time_type:<10}: took {duration}")
         else:
             logging.warning(f"Attempting to finish timer type {time_type}, which was never started!")
 
     def complete_all(self):
-        # for _type in self.times_running.copy().keys():
-        #     self.end(_type)
         pass
 
     def print_all_time_stats(self):
         for _type, times in self.times_archive.items():
             print(
                 f"{_type:<15}; "
                 f"min: {min(times):.04e}, "
@@ -87,17 +87,18 @@
 
 
 def reset_cuda_memory_monitoring():
     for i_cuda in range(torch.cuda.device_count()):
         torch.cuda.reset_peak_memory_stats(i_cuda)
 
 
-def get_cuda_memory_usage(log_message):
+def get_cuda_memory_usage(log_message, style="verbose"):
     logging.info("CUDA memory logging....\n")
     for i_cuda in range(torch.cuda.device_count()):
-        logging.info(f"{log_message}: Cuda device {i_cuda} report:\n")
-        pprint.pprint(torch.cuda.memory_stats(i_cuda))
-        logging.info(f"Report done! for Cuda device {i_cuda}\n")
+        logging.info(f"{log_message}: Cuda device {i_cuda}, {style} report:\n")
+        if style =="verbose":
+            pprint.pprint(torch.cuda.memory_stats(i_cuda))
+            logging.info(f"Report done! for Cuda device {i_cuda}\n")
         logging.info(f"Gpu memory currently allocated: {torch.cuda.memory_allocated(i_cuda)/1e9} GB.")
         logging.info(f"Gpu max memory allocated: {torch.cuda.max_memory_allocated(i_cuda)/1e9} GB.")
         logging.info(f"Gpu memory currently reserved: {torch.cuda.memory_reserved(i_cuda)/1e9} GB.")
         logging.info(f"Gpu max memory reserved: {torch.cuda.max_memory_reserved(i_cuda)/1e9} GB.")
```

### Comparing `a2-0.3/src/a2/training/dataset_hugging.py` & `a2-0.3.2/src/a2/training/dataset_hugging.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/training/evaluate_hugging.py` & `a2-0.3.2/src/a2/training/evaluate_hugging.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/training/tracking.py` & `a2-0.3.2/src/a2/training/tracking.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,29 +16,29 @@
         mantik.init_tracking()
     except Exception as e:
         warnings.warn(f"{e}\nCannot initialize mantik!")
 
 
 def catch_mantik_exceptions(func):
     def wrapper_catch_exception(*args, **kwargs):
+        result = None
         try:
             if not args[0].ignore:
-                func(*args, **kwargs)
-            else:
-                lambda x: None
+                result = func(*args, **kwargs)
         except mlflow.exceptions.MlflowException as e:
             logging.info(f"Ignoring mlflow exception:\n{e}")
         except Exception as exc:
             raise ValueError("Tracking error!") from exc
+        return result
 
     return wrapper_catch_exception
 
 
 class Tracker:
-    def __init__(self, ignore=True) -> None:
+    def __init__(self, ignore=False) -> None:
         self.ignore = ignore
         if not self.ignore:
             initialize_mantik()
 
     @catch_mantik_exceptions
     def log_param(self, name, value):
         mlflow.log_param(name, value)
@@ -74,28 +74,30 @@
     def active_run(self, *args, **kwargs):
         return mlflow.active_run(*args, **kwargs)
 
     @catch_mantik_exceptions
     def local_file_uri_to_path(self, *args, **kwargs):
         return mlflow.utils.file_utils.local_file_uri_to_path(*args, **kwargs)
 
-    @catch_mantik_exceptions
+    # @catch_mantik_exceptions
     def set_tracking_uri(self, *args, **kwargs):
         mlflow.set_tracking_uri(*args, **kwargs)
 
     @catch_mantik_exceptions
     def get_tracking_uri(self, *args, **kwargs):
         return mlflow.get_tracking_uri(*args, **kwargs)
 
     @catch_mantik_exceptions
     def create_experiment(self, name, **kwargs):
         experiment_id = self.get_experiment_by_name(name)
         print(f"{experiment_id=}")
+        logging.info(f"{not experiment_id=}")
         if not experiment_id:
             experiment_id = mlflow.create_experiment(name, **kwargs)
+            logging.info(f"create new: {experiment_id}")
         return experiment_id
 
     @catch_mantik_exceptions
     def get_experiment_by_name(self, *args, **kwargs):
         return mlflow.get_experiment_by_name(*args, **kwargs)
```

### Comparing `a2-0.3/src/a2/training/tracking_hugging.py` & `a2-0.3.2/src/a2/training/tracking_hugging.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import transformers
 
 from . import tracking
 
 
 class LogCallback(transformers.TrainerCallback):
-    def __init__(self, tracker: tracking.Tracker, log_to_stdout=True):
+    def __init__(self, tracker: tracking.Tracker | None = None, log_to_stdout=True):
         self.tracker = tracker
         self.log_to_stdout = log_to_stdout
         self.steps_logged = {"train": [], "evaluate": []}
 
     def _log_metrics(self, state, which="train", prefix=""):
         logs = state.log_history
         evaluate_logs = [_l for _l in logs if "eval_loss" in _l]
@@ -25,15 +25,16 @@
             current_log = log[-1]
             if self.log_to_stdout:
                 logging.info(f"LogCallback: {prefix} {current_log}")
             step = current_log["step"]
             if step in self.steps_logged:
                 # do not log same step twice: may occur as `on_log` also called during evaluation
                 return
-            self.tracker.log_metrics({k: v for k, v in current_log.items() if k != "step"}, step=step)
+            if self.tracker is not None:
+                self.tracker.log_metrics({k: v for k, v in current_log.items() if k != "step"}, step=step)
             self.steps_logged[which].append(step)
 
     def on_evaluate(self, args, state, control, logs=None, **kwargs):
         if state.is_local_process_zero:
             self._log_metrics(state, which="evaluate", prefix="on_evaluate: ")
 
     def on_log(self, args, state, control, logs=None, **kwargs):
```

### Comparing `a2-0.3/src/a2/training/training_deep500.py` & `a2-0.3.2/src/a2/training/training_deep500.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/training/training_hugging.py` & `a2-0.3.2/src/a2/training/training_hugging.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,16 +96,16 @@
         if mantik:
             a2.training.tracking.initialize_mantik()
         return model
 
     def get_trainer(
         self,
         dataset: t.Union[datasets.Dataset, datasets.DatasetDict],
-        hyper_parameters: HyperParametersDebertaClassifier = None,
-        tokenizer: t.Optional[transformers.DebertaTokenizer] = None,
+        hyper_parameters: HyperParametersDebertaClassifier | None = None,
+        tokenizer: t.Optional[transformers.DebertaTokenizer] | None = None,
         folder_output: str = "output/",
         hyper_tuning: bool = False,
         fp16: bool = True,
         evaluate: bool = False,
         mantik: bool = True,
         disable_tqdm: bool = False,
         callbacks: list | None = None,
@@ -128,14 +128,18 @@
         tokenizer: Hugging Face tokenizer
         folder_output: Folder to save training outputs
         hyper_tuning: Whether trainer used for hyper tuning
         fp16: Whether to use fp16 16-bit (mixed) precision training
               instead of 32-bit training.
         evaluate: Whether trainer only used for evaluation
         mantik: Whether using mantik for tracking
+        disable_tqdm: Whether to disable progress bar used by `Transformer`
+        callbacks: Callbacks during training
+        base_model_trainable: Whether base model weights are trainable (not fixed)
+        trainer_class: Trainer class compatible with `transformer.Trainer`
         logging_steps: Number of steps before hugging face prints
         evaluation_strategy: When to evaluate, after "steps" or "epoch"
         eval_steps: Number of steps between evaluation (only used if `evaluation_strategy`="steps")
         save_strategy: When to save best model "steps" or "epoch"
         load_best_model_at_end: Load best model at end of training
 
         Returns
```

### Comparing `a2-0.3/src/a2/twitter/downloader.py` & `a2-0.3.2/src/a2/twitter/downloader.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/twitter/locations.py` & `a2-0.3.2/src/a2/twitter/locations.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/twitter/twitter_api.py` & `a2-0.3.2/src/a2/twitter/twitter_api.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/utils/checks.py` & `a2-0.3.2/src/a2/utils/checks.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/utils/file_handling.py` & `a2-0.3.2/src/a2/utils/file_handling.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,12 +296,12 @@
 
 
 def check_folder_exists(path, check_is_empty=False, raise_exception=False):
     if not os.path.isdir(path):
         if raise_exception:
             raise ValueError(f"{path=} doesn't exist!")
         return False
-    if check_is_empty and not os.path.getsize(path):
+    if check_is_empty and os.path.getsize(path) <= 4096:
         if raise_exception:
             raise ValueError(f"{path=} is empty!")
         return False
     return True
```

### Comparing `a2-0.3/src/a2/utils/testing.py` & `a2-0.3.2/src/a2/utils/testing.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/src/a2/utils/utils.py` & `a2-0.3.2/src/a2/utils/utils.py`

 * *Files identical despite different names*

### Comparing `a2-0.3/PKG-INFO` & `a2-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 Metadata-Version: 2.1
 Name: a2
-Version: 0.3
+Version: 0.3.2
 Summary: Package for predicting information about the weather from social media data as application 2 for maelstrom project
 Author: Kristian Ehlert
 Author-email: kristian.ehlert@4-cast.de
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: extend-exclude
+Provides-Extra: llama-chatbot
+Provides-Extra: torch
 Requires-Dist: DateTime (>=4.4,<5.0)
 Requires-Dist: Shapely (>=1.8.2,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: convertbng (>=0.6.39,<0.7.0)
 Requires-Dist: dask (>=2022.6.1,<2023.0.0)
+Requires-Dist: datasets (>=2.11.0,<3.0.0)
 Requires-Dist: emoji (<1.0.0)
 Requires-Dist: geopy (>=2.3.0,<3.0.0)
 Requires-Dist: h5netcdf (>=1.0.1,<2.0.0)
 Requires-Dist: h5py (>=3.7.0,<4.0.0)
 Requires-Dist: ipython (>=8.7.0,<9.0.0)
 Requires-Dist: ipywidgets (>=7.7.1,<8.0.0)
 Requires-Dist: jsonlines (>=3.1.0,<4.0.0)
 Requires-Dist: jupyterlab (>=3.4.3,<4.0.0)
 Requires-Dist: kaleido (==0.2.1)
+Requires-Dist: llvmlite (>=0.39.1,<0.40.0)
 Requires-Dist: mantik (>=0.1.0,<0.2.0)
 Requires-Dist: matplotlib (>=3.5.2,<4.0.0)
 Requires-Dist: netCDF4 (>=1.6.0,<2.0.0)
 Requires-Dist: pandas (>=1.4.2,<2.0.0)
 Requires-Dist: plotly (>=5.11.0,<6.0.0)
 Requires-Dist: pyproj (>=3.3.1,<4.0.0)
-Requires-Dist: pytest-recording (>=0.12.1,<0.13.0)
-Requires-Dist: pytest-xdist (>=2.5.0,<3.0.0)
 Requires-Dist: rasterio (>=1.3.3,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: rioxarray (>=0.12.2,<0.13.0)
 Requires-Dist: scikit-learn (>=1.1.2,<2.0.0)
 Requires-Dist: seaborn (>=0.12.1,<0.13.0)
+Requires-Dist: sentencepiece (>=0.1.98,<0.2.0) ; extra == "llama-chatbot"
 Requires-Dist: spacymoji (>=3.0.1,<4.0.0)
+Requires-Dist: torch (>=2.0.0,<3.0.0) ; extra == "torch"
 Requires-Dist: tweepy (>=4.10.0,<5.0.0)
 Requires-Dist: urllib3 (>=1.26.12,<2.0.0)
 Requires-Dist: wget (>=3.2,<4.0)
 Requires-Dist: xarray (>=2022.3.0,<2023.0.0)
```

