# Comparing `tmp/falcon-ml-xgboost-0.1.0.tar.gz` & `tmp/falcon-ml-xgboost-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcon-ml-xgboost-0.1.0.tar", last modified: Mon Apr 10 18:49:26 2023, max compression
+gzip compressed data, was "falcon-ml-xgboost-0.2.0.tar", last modified: Thu Apr 20 16:48:08 2023, max compression
```

## Comparing `falcon-ml-xgboost-0.1.0.tar` & `falcon-ml-xgboost-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-10 18:49:26.792279 falcon-ml-xgboost-0.1.0/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      474 2023-04-10 18:49:26.792279 falcon-ml-xgboost-0.1.0/PKG-INFO
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-10 18:49:26.792279 falcon-ml-xgboost-0.1.0/falcon_ml_xgboost/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       74 2023-03-06 15:23:05.000000 falcon-ml-xgboost-0.1.0/falcon_ml_xgboost/__init__.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     6970 2023-03-10 15:17:08.000000 falcon-ml-xgboost-0.1.0/falcon_ml_xgboost/model.py
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     1624 2023-04-06 14:16:04.000000 falcon-ml-xgboost-0.1.0/falcon_ml_xgboost/task_configs.py
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-10 18:49:26.792279 falcon-ml-xgboost-0.1.0/falcon_ml_xgboost.egg-info/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      474 2023-04-10 18:49:26.000000 falcon-ml-xgboost-0.1.0/falcon_ml_xgboost.egg-info/PKG-INFO
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      327 2023-04-10 18:49:26.000000 falcon-ml-xgboost-0.1.0/falcon_ml_xgboost.egg-info/SOURCES.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)        1 2023-04-10 18:49:26.000000 falcon-ml-xgboost-0.1.0/falcon_ml_xgboost.egg-info/dependency_links.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       52 2023-04-10 18:49:26.000000 falcon-ml-xgboost-0.1.0/falcon_ml_xgboost.egg-info/requires.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       18 2023-04-10 18:49:26.000000 falcon-ml-xgboost-0.1.0/falcon_ml_xgboost.egg-info/top_level.txt
--rw-rw-r--   0 oleg      (1000) oleg      (1000)      752 2023-03-06 15:23:21.000000 falcon-ml-xgboost-0.1.0/pyproject.toml
--rw-rw-r--   0 oleg      (1000) oleg      (1000)       38 2023-04-10 18:49:26.792279 falcon-ml-xgboost-0.1.0/setup.cfg
-drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-10 18:49:26.792279 falcon-ml-xgboost-0.1.0/tests/
--rw-rw-r--   0 oleg      (1000) oleg      (1000)     2761 2023-03-06 15:23:05.000000 falcon-ml-xgboost-0.1.0/tests/test_xgb.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-20 16:48:08.834436 falcon-ml-xgboost-0.2.0/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      474 2023-04-20 16:48:08.834436 falcon-ml-xgboost-0.2.0/PKG-INFO
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-20 16:48:08.830436 falcon-ml-xgboost-0.2.0/falcon_ml_xgboost/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       97 2023-04-20 16:47:15.000000 falcon-ml-xgboost-0.2.0/falcon_ml_xgboost/__init__.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     6567 2023-04-20 16:17:20.000000 falcon-ml-xgboost-0.2.0/falcon_ml_xgboost/model.py
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     1624 2023-04-06 14:16:04.000000 falcon-ml-xgboost-0.2.0/falcon_ml_xgboost/task_configs.py
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-20 16:48:08.830436 falcon-ml-xgboost-0.2.0/falcon_ml_xgboost.egg-info/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      474 2023-04-20 16:48:08.000000 falcon-ml-xgboost-0.2.0/falcon_ml_xgboost.egg-info/PKG-INFO
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      327 2023-04-20 16:48:08.000000 falcon-ml-xgboost-0.2.0/falcon_ml_xgboost.egg-info/SOURCES.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)        1 2023-04-20 16:48:08.000000 falcon-ml-xgboost-0.2.0/falcon_ml_xgboost.egg-info/dependency_links.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       52 2023-04-20 16:48:08.000000 falcon-ml-xgboost-0.2.0/falcon_ml_xgboost.egg-info/requires.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       18 2023-04-20 16:48:08.000000 falcon-ml-xgboost-0.2.0/falcon_ml_xgboost.egg-info/top_level.txt
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)      752 2023-04-20 16:47:17.000000 falcon-ml-xgboost-0.2.0/pyproject.toml
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)       38 2023-04-20 16:48:08.834436 falcon-ml-xgboost-0.2.0/setup.cfg
+drwxrwxr-x   0 oleg      (1000) oleg      (1000)        0 2023-04-20 16:48:08.834436 falcon-ml-xgboost-0.2.0/tests/
+-rw-rw-r--   0 oleg      (1000) oleg      (1000)     2761 2023-03-06 15:23:05.000000 falcon-ml-xgboost-0.2.0/tests/test_xgb.py
```

### Comparing `falcon-ml-xgboost-0.1.0/falcon_ml_xgboost/model.py` & `falcon-ml-xgboost-0.2.0/falcon_ml_xgboost/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,32 +20,29 @@
 from falcon.config import ONNX_OPSET_VERSION, ML_ONNX_OPSET_VERSION
 
 
 class _XGBoostBase(Model, ONNXConvertible, OptunaMixin):
     def __init__(
         self,
         verbosity: int = 0,
-        objective: Optional[str] = None,
         tree_method: str = "auto",
         booster: str = "dart",
         reg_lambda: float = 1.0,
         reg_alpha: float = 0.0,
         *args,
         **kwargs,
     ):
 
         params = kwargs
         params["verbosity"] = verbosity
-        params["objective"] = objective
         params["tree_method"] = tree_method
         params["booster"] = booster
         params["reg_lambda"] = reg_lambda
         params["reg_alpha"] = reg_alpha
         self.params = params
-        self.objective = "multi:softmax"
 
     def predict(self, X: npt.NDArray, *args: Any, **kwargs: Any) -> npt.NDArray:
         preds = self.bst.predict(X)
         return preds
 
     def to_onnx(self) -> SerializedModelRepr:
         """
@@ -84,32 +81,29 @@
         reg_lambda: float = 1.0,
         reg_alpha: float = 0.0,
         *args,
         **kwargs,
     ):
         super().__init__(
             verbosity=verbosity,
-            objective="multi:softmax",
             tree_method=tree_method,
             booster=booster,
             reg_lambda=reg_lambda,
             reg_alpha=reg_alpha,
             **kwargs,
         )
 
     def fit(self, X: npt.NDArray, y: npt.NDArray, *args: Any, **kwargs: Any) -> None:
         self._shape = [None, *X.shape[1:]]
-        self.params["num_class"] = len(np.unique(y))
-        self.bst = xgboost.XGBClassifier(**self.params)
+        self.bst = xgboost.XGBClassifier(random_state = 42, **self.params)
         self.bst.fit(X, y)
 
     @classmethod
     def get_search_space(cls, X: npt.NDArray, y: npt.NDArray) -> Callable:
-        obj_ = "multi:softmax"
-
+        obj_ = "clf"
         def _objective_fn(trial, X, Xt, y, yt):
             return _objective(trial, X, Xt, y, yt, obj_)
 
         return _objective_fn
 
 
 class FalconXGBoostRegressor(_XGBoostBase):
@@ -121,15 +115,14 @@
         reg_lambda: float = 1.0,
         reg_alpha: float = 0.0,
         *args,
         **kwargs,
     ):
         super().__init__(
             verbosity=verbosity,
-            objective="reg:squarederror",
             tree_method=tree_method,
             booster=booster,
             reg_lambda=reg_lambda,
             reg_alpha=reg_alpha,
             **kwargs,
         )
 
@@ -138,40 +131,34 @@
         def _objective_fn(trial, X, Xt, y, yt):
             return _objective(trial, X, Xt, y, yt, "reg:squarederror")
 
         return _objective_fn
 
     def fit(self, X: npt.NDArray, y: npt.NDArray, *args: Any, **kwargs: Any) -> None:
         self._shape = [None, *X.shape[1:]]
-        self.bst = xgboost.XGBRegressor(**self.params)
+        self.bst = xgboost.XGBRegressor(random_state = 42, **self.params)
         self.bst.fit(X, y)
 
 
 def _objective(trial, X, Xt, y, yt, _objective):
     with xgboost.config_context(verbosity=0):
-        n_targets = len(np.unique(y))
-
         param = {
             "verbosity": 0,
-            "objective": _objective,
             "tree_method": "auto",
             "booster": trial.suggest_categorical("booster", ["gbtree", "dart"]),
             "reg_lambda": trial.suggest_float("reg_lambda", 1e-8, 1.0),
             "reg_alpha": trial.suggest_float("reg_alpha", 1e-8, 1.0, log=True),
             "subsample": trial.suggest_float("subsample", 0.5, 1.0),
             "colsample_bytree": trial.suggest_float("colsample_bytree", 0.5, 1.0),
             "random_state": 42,
             "n_estimators": trial.suggest_int("n_estimators", 10, 500, step=10),
         }
 
-        if _objective == "multi:softmax":
-            param["num_class"] = n_targets
-
         if param["booster"] in ["gbtree", "dart"]:
-            param["max_depth"] = trial.suggest_int("max_depth", 2, 10, step=2)
+            param["max_depth"] = trial.suggest_int("max_depth", 3, 10)
             param["min_child_weight"] = trial.suggest_int("min_child_weight", 1, 10)
             param["eta"] = trial.suggest_float("eta", 0.01, 1.0)  # lr
             param["gamma"] = trial.suggest_float("gamma", 1e-8, 1.0, log=True)
             param["grow_policy"] = trial.suggest_categorical(
                 "grow_policy", ["depthwise"]  # , "lossguide"]        
              )
 
@@ -181,17 +168,17 @@
             )
             param["normalize_type"] = trial.suggest_categorical(
                 "normalize_type", ["tree", "forest"]
             )
             param["rate_drop"] = trial.suggest_float("rate_drop", 1e-8, 1.0, log=True)
             param["skip_drop"] = trial.suggest_float("skip_drop", 1e-8, 1.0, log=True)
         if _objective == "reg:squarederror":
-            bst = xgboost.XGBRFRegressor(**param)
+            bst = xgboost.XGBRegressor(**param)
         else:
-            bst = xgboost.XGBRFClassifier(**param)
+            bst = xgboost.XGBClassifier(**param)
         bst.fit(X, y)
         preds = bst.predict(Xt)
         return {"predictions": preds, "loss": None}
 
 
 update_registered_converter(
     xgboost.XGBRegressor,
```

### Comparing `falcon-ml-xgboost-0.1.0/falcon_ml_xgboost/task_configs.py` & `falcon-ml-xgboost-0.2.0/falcon_ml_xgboost/task_configs.py`

 * *Files identical despite different names*

### Comparing `falcon-ml-xgboost-0.1.0/pyproject.toml` & `falcon-ml-xgboost-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [project]
 dependencies = [
 "falcon-ml>=0.6.0",
 "xgboost>=1.7.0",
 "onnxmltools>=1.11.0",
 ]
 name = "falcon-ml-xgboost"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="Oleg Kostromin", email="kostromin97@gmail.com" },
   { name="Iryna Kondrashchenko", email="iryna230520@gmail.com" },
   { name="Marco Pasini", email="marco.pasini.98@gmail.com" },
 ]
 description = "XGBoost extension for falcon-ml library."
 readme = "README.md"
```

### Comparing `falcon-ml-xgboost-0.1.0/tests/test_xgb.py` & `falcon-ml-xgboost-0.2.0/tests/test_xgb.py`

 * *Files identical despite different names*

