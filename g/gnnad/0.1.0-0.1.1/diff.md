# Comparing `tmp/gnnad-0.1.0.tar.gz` & `tmp/gnnad-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnnad-0.1.0.tar", max compression
+gzip compressed data, was "gnnad-0.1.1.tar", max compression
```

## Comparing `gnnad-0.1.0.tar` & `gnnad-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-04-18 06:01:31.203385 gnnad-0.1.0/LICENSE
--rw-r--r--   0        0        0     3612 2023-04-18 06:01:31.203385 gnnad-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-04-18 06:01:31.215385 gnnad-0.1.0/gnnad/__init__.py
--rw-r--r--   0        0        0     6808 2023-04-18 06:01:31.215385 gnnad-0.1.0/gnnad/generate.py
--rw-r--r--   0        0        0    37868 2023-04-18 06:01:31.215385 gnnad-0.1.0/gnnad/graphanomaly.py
--rw-r--r--   0        0        0     4778 2023-04-18 06:01:31.215385 gnnad-0.1.0/gnnad/plot.py
--rw-r--r--   0        0        0      680 2023-04-18 06:01:31.215385 gnnad-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4638 1970-01-01 00:00:00.000000 gnnad-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-20 04:11:05.851883 gnnad-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4166 2023-04-20 04:11:05.851883 gnnad-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 04:11:05.859883 gnnad-0.1.1/gnnad/__init__.py
+-rw-r--r--   0        0        0     6808 2023-04-20 04:11:05.859883 gnnad-0.1.1/gnnad/generate.py
+-rw-r--r--   0        0        0    38009 2023-04-20 04:11:05.859883 gnnad-0.1.1/gnnad/graphanomaly.py
+-rw-r--r--   0        0        0     4778 2023-04-20 04:11:05.859883 gnnad-0.1.1/gnnad/plot.py
+-rw-r--r--   0        0        0      680 2023-04-20 04:11:05.859883 gnnad-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5192 1970-01-01 00:00:00.000000 gnnad-0.1.1/PKG-INFO
```

### Comparing `gnnad-0.1.0/LICENSE` & `gnnad-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gnnad-0.1.0/README.md` & `gnnad-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,73 +1,91 @@
 # Graph Neural Network-Based Anomaly Detection (GNNAD)
 
-gnnad is a package for anomaly detection on multivariate time series data. This model builds on the recently-proposed Graph Deviation Network (GDN) [2], a  graph neural network model that uses embeddings to capture inter-sensor relationships as a learned graph, and employs graph attention-based forecasting to predict future sensor behaviour. Anomalies are flagged when the error scores are above a calculated threshold value. By learning the interdependencies among variables and predicting based on the typical patterns of the system, this approach is able to detect deviations when the expected spatial dependencies are disrupted. As such, GDN offers the ability to detect even the small-deviation anomalies generally overlooked by other distance based and density based anomaly detection methods for time series.
+`gnnad` is a package for anomaly detection on multivariate time series data.
 
-This package accompanies work that further develops this model [1], and introduces an alternate anomaly threshold criteria based on the learned graph, with the improved ability to detect anomalies in multivariate timeseries data. The example we explore is of data collected within river network systems.
+This model builds on the recently-proposed Graph Deviation Network (GDN)[^2], a graph neural network model that uses embeddings to capture inter-sensor relationships as a learned graph, and employs graph attention-based forecasting to predict future sensor behaviour. Anomalies are flagged when the error scores are above a calculated threshold value. By learning the interdependencies among variables and predicting based on the typical patterns of the system, this approach is able to detect deviations when the expected spatial dependencies are disrupted. As such, GDN offers the ability to detect even the small-deviation anomalies generally overlooked by other distance based and density based anomaly detection methods for time series.
+
+This package accompanies work that further develops this model[^1], and introduces an alternate anomaly threshold criteria based on the learned graph, with the improved ability to detect anomalies in multivariate timeseries data.
 
 ## Quick start
 
-Consider data collected on the Herbert river network, at these sensor locations:
+As an example we'll explore data collected within river network system. In particular data collected on the Herbert river network, at these sensor locations:
 
+<p align="center">
 <img src="https://user-images.githubusercontent.com/34525024/232662278-bc6973ae-6ccf-443d-99d4-204eada127d6.JPG" width="35%" height="35%" alt="Herbert river sensor locations" title="">
+ </p>
 
 The sensors measure water level, from within the river. Assuming we have pre-processed the data, we instantiate and fit the model:
-```
+
+```python
+from gnnad.graphanomaly import GNNAD
+
 # run model
 model = GNNAD(threshold_type="max_validation", topk=6, slide_win=200)
 fitted_model = model.fit(X_train, X_test, y_test)
 
 # the predicted values can be accessed here
 test_predict = fitted_model.test_result[0, :, i]
 ```
 
 We can visualise the predicted values vs. actual values, with helper functions in the plot module.
-
+<p align="center">
 <img src="https://user-images.githubusercontent.com/34525024/232661014-99ebb7c0-7e4a-4f54-b09a-fedb5c5bbaf1.jpg" width="40%" height="40%" alt="Herbert river sensor locations" title="">
-
+</p>
+  
 Note that some locations closer to the outlet are influenced by tidal patterns. The error scores that are obtained from this forecasting model are then transformed and, if they exceed the calculated threshold, flagged as an anomaly. The bottom indicates if any sensor flagged an anomaly, and compares this to the ground truth labels, for the test data.
 
 The performance of the anomaly detection classification model can be analysed by:
-```
+
+```python
 fitted_model.print_eval_metrics()
 >>> recall: 30.4
 >>> precision: 59.3
 >>> accuracy: 49.7
 >>> specificity: 73.9
 >>> f1: 40.2
 ```
 
 Check out full details in the [example notebook](example_herbert.ipynb)
 
 ## Installation
 
+`gnnad` is compatible with python versions 3.8, 3.9, 3.10 and 3.11. You can install the latest release with pip: 
+
 ```bash
-pip install https://github.com/KatieBuc/gnnad.git
+pip install gnnad
 ```
 
-Once the project is release on PyPI it should be as simple as:
+If you would like the latest development version you can install directly from github:
 
 ```bash
-pip install gnnad
+pip install https://github.com/KatieBuc/gnnad.git
 ```
 
 ## Developer installation
 
 You'll need [poetry](https://python-poetry.org/docs/#installation). Once you have it installed and
 cloned the repo you can install with (from the repo directory):
 
 ```bash
 poetry install
 ```
 
-## References
-
-[1] Buchhorn, Katie, et al. "Graph Neural Network-Based Anomaly Detection for River Network Systems" Under review.
-
-[2] Deng, Ailin, and Bryan Hooi. "Graph neural network-based anomaly detection in multivariate time series." Proceedings of the AAAI conference on artificial intelligence. Vol. 35. No. 5. 2021.
+[^1]: Buchhorn, Katie, et al. _"Graph Neural Network-Based Anomaly Detection for River Network Systems"_ Under review.
+[^2]: Deng, Ailin, and Bryan Hooi. _"Graph neural network-based anomaly detection in multivariate time series."_ Proceedings of the AAAI conference on artificial intelligence. Vol. 35. No. 5. 2021.
 
 
 ## Citation
-
+MLA:
+```
+Buchhorn, Katie, et al. "Graph Neural Network-Based Anomaly Detection for River Network Systems"
+arXiv preprint arXiv:2304.09367 (2023).
+```
+BibTeX:
 ```
-Buchhorn, Katie, et al. "Graph Neural Network-Based Anomaly Detection for River Network Systems" Under review.
+@article{buchhorn2023graph,
+  title={Graph Neural Network-Based Anomaly Detection for River Network Systems},
+  author={Buchhorn, Katie and Mengersen, Kerrie and Santos-Fernandez, Edgar and Salomone, Robert},
+  journal={arXiv preprint arXiv:2304.09367},
+  year={2023}
+}
 ```
```

### Comparing `gnnad-0.1.0/gnnad/generate.py` & `gnnad-0.1.1/gnnad/generate.py`

 * *Files identical despite different names*

### Comparing `gnnad-0.1.0/gnnad/graphanomaly.py` & `gnnad-0.1.1/gnnad/graphanomaly.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 """
 Graph Neural Network-Based Anomaly Detection.
 
 References
 ----------
 [1] Deng, Ailin, and Bryan Hooi. "Graph neural network-based anomaly detection in multivariate time series."
 Proceedings of the AAAI conference on artificial intelligence. Vol. 35. No. 5. 2021.
+[2] Buchhorn, Katie, et al. "Graph Neural Network-Based Anomaly Detection for River Network Systems"
+arXiv preprint arXiv:2304.09367 (2023).
 """
 
 import math
 import os
 import random
 from datetime import datetime
 from pathlib import Path
```

### Comparing `gnnad-0.1.0/gnnad/plot.py` & `gnnad-0.1.1/gnnad/plot.py`

 * *Files identical despite different names*

### Comparing `gnnad-0.1.0/pyproject.toml` & `gnnad-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gnnad"
-version = "0.1.0"
+version = "0.1.1"
 description = "Graph Neural Network-Based Anomaly Detection (GNNAD)"
 authors = ["Katie Buchhorn"]
 maintainers = ["Katie Buchhorn"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/KatieBuc/gnnad"
```

### Comparing `gnnad-0.1.0/PKG-INFO` & `gnnad-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gnnad
-Version: 0.1.0
+Version: 0.1.1
 Summary: Graph Neural Network-Based Anomaly Detection (GNNAD)
 Home-page: https://github.com/KatieBuc/gnnad
 License: MIT
 Author: Katie Buchhorn
 Maintainer: Katie Buchhorn
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -23,79 +23,97 @@
 Requires-Dist: torch-geometric (>=2.3.0,<3.0.0)
 Requires-Dist: torchsummary (>=1.5.1,<2.0.0)
 Project-URL: Repository, https://github.com/KatieBuc/gnnad
 Description-Content-Type: text/markdown
 
 # Graph Neural Network-Based Anomaly Detection (GNNAD)
 
-gnnad is a package for anomaly detection on multivariate time series data. This model builds on the recently-proposed Graph Deviation Network (GDN) [2], a  graph neural network model that uses embeddings to capture inter-sensor relationships as a learned graph, and employs graph attention-based forecasting to predict future sensor behaviour. Anomalies are flagged when the error scores are above a calculated threshold value. By learning the interdependencies among variables and predicting based on the typical patterns of the system, this approach is able to detect deviations when the expected spatial dependencies are disrupted. As such, GDN offers the ability to detect even the small-deviation anomalies generally overlooked by other distance based and density based anomaly detection methods for time series.
+`gnnad` is a package for anomaly detection on multivariate time series data.
 
-This package accompanies work that further develops this model [1], and introduces an alternate anomaly threshold criteria based on the learned graph, with the improved ability to detect anomalies in multivariate timeseries data. The example we explore is of data collected within river network systems.
+This model builds on the recently-proposed Graph Deviation Network (GDN)[^2], a graph neural network model that uses embeddings to capture inter-sensor relationships as a learned graph, and employs graph attention-based forecasting to predict future sensor behaviour. Anomalies are flagged when the error scores are above a calculated threshold value. By learning the interdependencies among variables and predicting based on the typical patterns of the system, this approach is able to detect deviations when the expected spatial dependencies are disrupted. As such, GDN offers the ability to detect even the small-deviation anomalies generally overlooked by other distance based and density based anomaly detection methods for time series.
+
+This package accompanies work that further develops this model[^1], and introduces an alternate anomaly threshold criteria based on the learned graph, with the improved ability to detect anomalies in multivariate timeseries data.
 
 ## Quick start
 
-Consider data collected on the Herbert river network, at these sensor locations:
+As an example we'll explore data collected within river network system. In particular data collected on the Herbert river network, at these sensor locations:
 
+<p align="center">
 <img src="https://user-images.githubusercontent.com/34525024/232662278-bc6973ae-6ccf-443d-99d4-204eada127d6.JPG" width="35%" height="35%" alt="Herbert river sensor locations" title="">
+ </p>
 
 The sensors measure water level, from within the river. Assuming we have pre-processed the data, we instantiate and fit the model:
-```
+
+```python
+from gnnad.graphanomaly import GNNAD
+
 # run model
 model = GNNAD(threshold_type="max_validation", topk=6, slide_win=200)
 fitted_model = model.fit(X_train, X_test, y_test)
 
 # the predicted values can be accessed here
 test_predict = fitted_model.test_result[0, :, i]
 ```
 
 We can visualise the predicted values vs. actual values, with helper functions in the plot module.
-
+<p align="center">
 <img src="https://user-images.githubusercontent.com/34525024/232661014-99ebb7c0-7e4a-4f54-b09a-fedb5c5bbaf1.jpg" width="40%" height="40%" alt="Herbert river sensor locations" title="">
-
+</p>
+  
 Note that some locations closer to the outlet are influenced by tidal patterns. The error scores that are obtained from this forecasting model are then transformed and, if they exceed the calculated threshold, flagged as an anomaly. The bottom indicates if any sensor flagged an anomaly, and compares this to the ground truth labels, for the test data.
 
 The performance of the anomaly detection classification model can be analysed by:
-```
+
+```python
 fitted_model.print_eval_metrics()
 >>> recall: 30.4
 >>> precision: 59.3
 >>> accuracy: 49.7
 >>> specificity: 73.9
 >>> f1: 40.2
 ```
 
 Check out full details in the [example notebook](example_herbert.ipynb)
 
 ## Installation
 
+`gnnad` is compatible with python versions 3.8, 3.9, 3.10 and 3.11. You can install the latest release with pip: 
+
 ```bash
-pip install https://github.com/KatieBuc/gnnad.git
+pip install gnnad
 ```
 
-Once the project is release on PyPI it should be as simple as:
+If you would like the latest development version you can install directly from github:
 
 ```bash
-pip install gnnad
+pip install https://github.com/KatieBuc/gnnad.git
 ```
 
 ## Developer installation
 
 You'll need [poetry](https://python-poetry.org/docs/#installation). Once you have it installed and
 cloned the repo you can install with (from the repo directory):
 
 ```bash
 poetry install
 ```
 
-## References
-
-[1] Buchhorn, Katie, et al. "Graph Neural Network-Based Anomaly Detection for River Network Systems" Under review.
-
-[2] Deng, Ailin, and Bryan Hooi. "Graph neural network-based anomaly detection in multivariate time series." Proceedings of the AAAI conference on artificial intelligence. Vol. 35. No. 5. 2021.
+[^1]: Buchhorn, Katie, et al. _"Graph Neural Network-Based Anomaly Detection for River Network Systems"_ Under review.
+[^2]: Deng, Ailin, and Bryan Hooi. _"Graph neural network-based anomaly detection in multivariate time series."_ Proceedings of the AAAI conference on artificial intelligence. Vol. 35. No. 5. 2021.
 
 
 ## Citation
-
+MLA:
+```
+Buchhorn, Katie, et al. "Graph Neural Network-Based Anomaly Detection for River Network Systems"
+arXiv preprint arXiv:2304.09367 (2023).
+```
+BibTeX:
 ```
-Buchhorn, Katie, et al. "Graph Neural Network-Based Anomaly Detection for River Network Systems" Under review.
+@article{buchhorn2023graph,
+  title={Graph Neural Network-Based Anomaly Detection for River Network Systems},
+  author={Buchhorn, Katie and Mengersen, Kerrie and Santos-Fernandez, Edgar and Salomone, Robert},
+  journal={arXiv preprint arXiv:2304.09367},
+  year={2023}
+}
 ```
```

