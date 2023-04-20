# Comparing `tmp/forust-0.1.7.tar.gz` & `tmp/forust-0.2.0.tar.gz`

## Comparing `forust-0.1.7.tar` & `forust-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,41 @@
--rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 forust-0.1.7/local_dependencies/forust-ml/Cargo.toml
--rw-r--r--   0      501       20     5576 2022-08-20 19:35:59.000000 forust-0.1.7/local_dependencies/forust-ml/.github/workflows/CI.yml
--rw-r--r--   0      501       20      229 2022-08-20 19:35:59.000000 forust-0.1.7/local_dependencies/forust-ml/.gitignore
--rw-r--r--   0      501       20      320 2022-08-20 19:35:59.000000 forust-0.1.7/local_dependencies/forust-ml/.pre-commit-config.yaml
--rw-r--r--   0      501       20    11341 2022-08-20 19:35:59.000000 forust-0.1.7/local_dependencies/forust-ml/LICENSE
--rw-r--r--   0      501       20    10768 2022-08-20 19:35:59.000000 forust-0.1.7/local_dependencies/forust-ml/README.md
--rw-r--r--   0      501       20     3573 2022-08-20 19:35:59.000000 forust-0.1.7/local_dependencies/forust-ml/benches/forust_benchmarks.rs
--rw-r--r--   0      501       20   386602 2022-08-20 19:39:50.000000 forust-0.1.7/local_dependencies/forust-ml/dist/forust-0.1.7-cp310-cp310-macosx_10_7_x86_64.whl
--rw-r--r--   0      501       20   729080 2022-08-20 19:38:48.000000 forust-0.1.7/local_dependencies/forust-ml/dist/forust-0.1.7.tar.gz
--rw-r--r--   0      501       20     1179 2022-08-20 19:35:59.000000 forust-0.1.7/local_dependencies/forust-ml/resources/make_resources.py
--rw-r--r--   0      501       20    16121 2022-08-20 19:35:59.000000 forust-0.1.7/local_dependencies/forust-ml/resources/pdp_plot_age.png
--rw-r--r--   0      501       20    57018 2022-08-20 19:35:59.000000 forust-0.1.7/local_dependencies/forust-ml/resources/titanic.csv
--rw-r--r--   0      501       20   655700 2022-08-20 19:35:59.000000 forust-0.1.7/local_dependencies/forust-ml/resources/tree-image-crop.png
--rw-r--r--   0      501       20     5455 2022-08-20 19:35:59.000000 forust-0.1.7/local_dependencies/forust-ml/src/binning.rs
--rw-r--r--   0      501       20      248 2022-08-20 19:35:59.000000 forust-0.1.7/local_dependencies/forust-ml/src/constraints.rs
--rw-r--r--   0      501       20     7139 2022-08-20 19:35:59.000000 forust-0.1.7/local_dependencies/forust-ml/src/data.rs
--rw-r--r--   0      501       20      473 2022-08-20 19:35:59.000000 forust-0.1.7/local_dependencies/forust-ml/src/errors.rs
--rw-r--r--   0      501       20    12673 2022-08-20 19:35:59.000000 forust-0.1.7/local_dependencies/forust-ml/src/gradientbooster.rs
--rw-r--r--   0      501       20     6465 2022-08-20 19:35:59.000000 forust-0.1.7/local_dependencies/forust-ml/src/histogram.rs
--rw-r--r--   0      501       20      205 2022-08-20 19:35:59.000000 forust-0.1.7/local_dependencies/forust-ml/src/lib.rs
--rw-r--r--   0      501       20     5089 2022-08-20 19:35:59.000000 forust-0.1.7/local_dependencies/forust-ml/src/node.rs
--rw-r--r--   0      501       20     4125 2022-08-20 19:35:59.000000 forust-0.1.7/local_dependencies/forust-ml/src/objective.rs
--rw-r--r--   0      501       20     3812 2022-08-20 19:35:59.000000 forust-0.1.7/local_dependencies/forust-ml/src/partial_dependence.rs
--rw-r--r--   0      501       20    18393 2022-08-20 19:35:59.000000 forust-0.1.7/local_dependencies/forust-ml/src/splitter.rs
--rw-r--r--   0      501       20    15238 2022-08-20 19:35:59.000000 forust-0.1.7/local_dependencies/forust-ml/src/tree.rs
--rw-r--r--   0      501       20     9554 2022-08-20 19:35:59.000000 forust-0.1.7/local_dependencies/forust-ml/src/utils.rs
--rw-r--r--   0        0        0      393 1970-01-01 00:00:00.000000 forust-0.1.7/Cargo.toml
--rw-r--r--   0      501       20      685 2022-08-20 19:35:59.000000 forust-0.1.7/.gitignore
--rw-r--r--   0      501       20    10768 2022-08-20 19:36:32.000000 forust-0.1.7/README.md
--rw-r--r--   0      501       20    14396 2022-08-20 19:35:59.000000 forust-0.1.7/forust/__init__.py
--rw-r--r--   0      501       20      670 2022-08-20 19:35:59.000000 forust-0.1.7/pyproject.toml
--rw-r--r--   0      501       20     6905 2022-08-20 19:35:59.000000 forust-0.1.7/scratch.py
--rw-r--r--   0      501       20     8060 2022-08-20 19:35:59.000000 forust-0.1.7/src/lib.rs
--rw-r--r--   0      501       20     6632 2022-08-20 19:35:59.000000 forust-0.1.7/tests/test_booster.py
--rw-r--r--   0      501       20    11341 2022-08-20 19:36:32.000000 forust-0.1.7/LICENSE
--rw-r--r--   0      501       20    10768 2022-08-20 19:36:32.000000 forust-0.1.7/README.md
--rw-r--r--   0        0        0    11326 1970-01-01 00:00:00.000000 forust-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 forust-0.2.0/local_dependencies/forust-ml/Cargo.toml
+-rw-r--r--   0      501       20     5584 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      262 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/.gitignore
+-rw-r--r--   0      501       20      320 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/.pre-commit-config.yaml
+-rw-r--r--   0      501       20    11341 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/LICENSE
+-rw-r--r--   0      501       20    10117 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/README.md
+-rw-r--r--   0      501       20     3857 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/benches/forust_benchmarks.rs
+-rw-r--r--   0      501       20   403349 2023-04-20 00:37:01.000000 forust-0.2.0/local_dependencies/forust-ml/dist/forust-0.2.0-cp310-cp310-macosx_10_7_x86_64.whl
+-rw-r--r--   0      501       20   743715 2023-04-20 00:36:03.000000 forust-0.2.0/local_dependencies/forust-ml/dist/forust-0.2.0.tar.gz
+-rw-r--r--   0      501       20    16121 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/resources/pdp_plot_age.png
+-rw-r--r--   0      501       20    10758 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/resources/pdp_plot_age_mono.png
+-rw-r--r--   0      501       20    57018 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/resources/titanic.csv
+-rw-r--r--   0      501       20   655700 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/resources/tree-image-crop.png
+-rw-r--r--   0      501       20     2556 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/rs-example.md
+-rw-r--r--   0      501       20     1179 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/scripts/make_resources.py
+-rw-r--r--   0      501       20       53 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/scripts/run-python-tests.ps1
+-rw-r--r--   0      501       20       53 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/scripts/run-python-tests.sh
+-rw-r--r--   0      501       20     5456 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/binning.rs
+-rw-r--r--   0      501       20      248 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/constraints.rs
+-rw-r--r--   0      501       20     7196 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/data.rs
+-rw-r--r--   0      501       20      473 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/errors.rs
+-rw-r--r--   0      501       20    16106 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/gradientbooster.rs
+-rw-r--r--   0      501       20     8639 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/histogram.rs
+-rw-r--r--   0      501       20      318 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/lib.rs
+-rw-r--r--   0      501       20     5813 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/node.rs
+-rw-r--r--   0      501       20     4125 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/objective.rs
+-rw-r--r--   0      501       20     3650 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/partial_dependence.rs
+-rw-r--r--   0      501       20    27732 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/splitter.rs
+-rw-r--r--   0      501       20    10708 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/tree.rs
+-rw-r--r--   0      501       20    28270 2023-04-20 00:32:57.000000 forust-0.2.0/local_dependencies/forust-ml/src/utils.rs
+-rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 forust-0.2.0/Cargo.toml
+-rw-r--r--   0      501       20      685 2023-04-20 00:32:57.000000 forust-0.2.0/.gitignore
+-rw-r--r--   0      501       20    10117 2023-04-20 00:33:45.000000 forust-0.2.0/README.md
+-rw-r--r--   0      501       20    13982 2023-04-20 00:32:57.000000 forust-0.2.0/forust/__init__.py
+-rw-r--r--   0      501       20      785 2023-04-20 00:32:57.000000 forust-0.2.0/pyproject.toml
+-rw-r--r--   0      501       20     7353 2023-04-20 00:32:57.000000 forust-0.2.0/scratch.py
+-rw-r--r--   0      501       20     7927 2023-04-20 00:32:57.000000 forust-0.2.0/src/lib.rs
+-rw-r--r--   0      501       20     6632 2023-04-20 00:32:57.000000 forust-0.2.0/tests/test_booster.py
+-rw-r--r--   0      501       20    11341 2023-04-20 00:33:45.000000 forust-0.2.0/LICENSE
+-rw-r--r--   0      501       20    10117 2023-04-20 00:33:45.000000 forust-0.2.0/README.md
+-rw-r--r--   0        0        0    10901 1970-01-01 00:00:00.000000 forust-0.2.0/PKG-INFO
```

### Comparing `forust-0.1.7/local_dependencies/forust-ml/Cargo.toml` & `forust-0.2.0/local_dependencies/forust-ml/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "forust-ml"
-version = "0.1.7"
+version = "0.2.0"
 edition = "2021"
 authors = ["James Inlow <james.d.inlow@gmail.com>"]
 homepage = "https://github.com/jinlow/forust"
 description = "A lightweight gradient boosting implementation in Rust."
 license-file = "LICENSE"
 readme = "README.md"
 repository = "https://github.com/jinlow/forust"
@@ -14,12 +14,13 @@
 [dependencies]
 rayon = "1.5"
 thiserror = "1.0.31"
 serde_json = {version = "1.0", features = ["float_roundtrip"] }
 serde = { version = "1.0", features = ["derive"] }
 
 [dev-dependencies]
-criterion = "0.3"
+criterion = "0.4"
+rand = "0.8.5"
 
 [[bench]]
 name = "forust_benchmarks"
 harness = false
```

### Comparing `forust-0.1.7/local_dependencies/forust-ml/.github/workflows/CI.yml` & `forust-0.2.0/local_dependencies/forust-ml/.github/workflows/CI.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name: Test and Deploy
-on: [push]
+on: [pull_request, push]
 
 jobs:
   windows-build-tests:
     strategy:
       matrix:
         pyversion: ["3.8", "3.9", "3.10"]
     runs-on: "windows-latest"
@@ -20,15 +20,15 @@
           architecture: x64
       - name: Install deps
         run: pip install numpy pandas seaborn xgboost=='1.6.1' scikit-learn
       - run: |
           cp README.md py-forust/README.md
           cp LICENSE py-forust/LICENSE
       - name: Build test data
-        run: python resources/make_resources.py
+        run: python scripts/make_resources.py
       - name: Run Cargo tests
         uses: actions-rs/cargo@v1
         with:
           command: test
       - name: Build Wheels with maturin
         uses: messense/maturin-action@v1
         with:
@@ -73,15 +73,15 @@
           architecture: x64
       - name: Install deps
         run: pip install numpy pandas seaborn xgboost=='1.6.1' scikit-learn
       - run: |
           cp README.md py-forust/README.md
           cp LICENSE py-forust/LICENSE
       - name: Build test data
-        run: python resources/make_resources.py
+        run: python scripts/make_resources.py
       - name: Run Cargo tests
         uses: actions-rs/cargo@v1
         with:
           command: test
       - name: Build Wheels with maturin
         uses: messense/maturin-action@v1
         with:
@@ -128,15 +128,15 @@
           architecture: x64
       - name: Install deps
         run: pip install numpy pandas seaborn xgboost=='1.6.1' scikit-learn
       - run: |
           cp README.md py-forust/README.md
           cp LICENSE py-forust/LICENSE
       - name: Build test data
-        run: python resources/make_resources.py
+        run: python scripts/make_resources.py
       - name: Run Cargo tests
         uses: actions-rs/cargo@v1
         with:
           command: test
       - name: Build Wheels with maturin
         uses: messense/maturin-action@v1
         with:
```

### Comparing `forust-0.1.7/local_dependencies/forust-ml/LICENSE` & `forust-0.2.0/local_dependencies/forust-ml/LICENSE`

 * *Files identical despite different names*

### Comparing `forust-0.1.7/local_dependencies/forust-ml/README.md` & `forust-0.2.0/local_dependencies/forust-ml/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,29 +8,29 @@
   <a href="https://pypi.org/project/forust/">![PyPI](https://img.shields.io/pypi/v/forust?color=gr&style=for-the-badge)</a>
   <a href="https://crates.io/crates/forust-ml">![Crates.io](https://img.shields.io/crates/v/forust-ml?color=gr&style=for-the-badge)</a>
 
 </div>
 
 # Forust
 ## _A lightweight gradient boosting package_
-Forust, is a lightweight package for building gradient boosted decision tree ensembles. All of the algorithm code is written in [Rust](https://www.rust-lang.org/), with a python wrapper. The rust package can be used directly, however, most examples shown here will be for the python wrapper. It implements the same algorithm as the [XGBoost](https://xgboost.readthedocs.io/en/stable/) package, and in many cases will give nearly identical results.
+Forust, is a lightweight package for building gradient boosted decision tree ensembles. All of the algorithm code is written in [Rust](https://www.rust-lang.org/), with a python wrapper. The rust package can be used directly, however, most examples shown here will be for the python wrapper. For a self contained rust example, [see here](rs-example.md). It implements the same algorithm as the [XGBoost](https://xgboost.readthedocs.io/en/stable/) package, and in many cases will give nearly identical results.
 
 I developed this package for a few reasons, mainly to better understand the XGBoost algorithm, additionally to have a fun project to work on in rust, and because I wanted to be able to experiment with adding new features to the algorithm in a smaller simpler codebase.
 
 All of the rust code for the package can be found in the [src](src/) directory, while all of the python wrapper code is in the [py-forust](py-forust/) directory.
 
 ## Installation
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.1.7"
+forust-ml = "0.2.0"
 ```
 
 ## Usage
 The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
 
 It can be initialized with the following arguments.
 
@@ -57,15 +57,14 @@
  - `nbins` ***(int, optional)***: Number of bins to calculate to partition the data. Setting this to
     a smaller number, will result in faster training time, while potentially sacrificing
     accuracy. If there are more bins, than unique values in a column, all unique values
     will be used. Defaults to 256.
  - `parallel` ***(bool, optional)***: Should multiple cores be used when training and predicting
     with this model? Defaults to `True`.
  - `allow_missing_splits` ***(bool, optional)***: Allow for splits to be made such that all missing values go down one branch, and all non-missing values go down the other, if this results in the greatest reduction of loss. If this is false, splits will only be made on non missing values. Defaults to `True`.
- - `impute_missing` ***(bool, optional)***: Automatically impute missing values, such that at every split the model learns the best direction to send missing values. If this is false, all missing values will default to right branch. Defaults to `True`.
  - `monotone_constraints` ***(dict[Any, int], optional)***: Constraints that are used to enforce a specific relationship between the training features and the target variable. A dictionary should be provided where the keys are the feature index value if the model will be fit on a numpy array, or a feature name if it will be fit on a pandas Dataframe. The values of the dictionary should be an integer value of -1, 1, or 0 to specify the relationship that should be estimated between the respective feature and the target variable. Use a value of -1 to enforce a negative relationship, 1 a positive relationship, and 0 will enforce no specific relationship at all. Features not included in the mapping will not have any constraint applied. If `None` is passed no constraints will be enforced on any variable.  Defaults to `None`.
 
 ### Training and Predicting
 
 Once, the booster has been initialized, it can be fit on a provided dataset, and performance field. After fitting, the model can be used to predict on a dataset.
 In the case of this example, the predictions are the log odds of a given record being 1.
 
@@ -152,15 +151,15 @@
 ```python
 model = GradientBooster(
     objective_type="LogLoss",
     monotone_constraints={"age": -1},
 )
 model.fit(X, y)
 
-pd_values = model.partial_dependence(X=X, 1)
+pd_values = model.partial_dependence(X=X, feature="age")
 fig = lineplot(
     x=pd_values[:, 0],
     y=pd_values[:, 1],
 )
 plt.title("Partial Dependence Plot with Monotonicity")
 plt.xlabel("Age")
 plt.ylabel("Log Odds")
@@ -172,17 +171,7 @@
 
 ```python
 trained_model.save_booster("model_path.json")
 
 # To load a model from a json path.
 loaded_model = GradientBooster.load_model("model_path.json")
 ```
-
-## TODOs
-This is still a work in progress
-- [ ] Early stopping rounds
-    * We should be able to accept a validation dataset, and this should be able to be used to determine when to stop training.
-- [X] Monotonicity support
-    * Right now features are used in the model without any constraints.
-- [X] Ability to save a model.
-    * The way the underlying trees are structured, they would lend themselves to being saved as JSon objects.
-- [ ] Clean up the CICD pipeline.
```

#### html2text {}

```diff
@@ -2,60 +2,58 @@
  ![PyPI](https://img.shields.io/pypi/v/forust?color=gr&style=for-the-badge) !
  [Crates.io](https://img.shields.io/crates/v/forust-ml?color=gr&style=for-the-
                                     badge)
 # Forust ## _A lightweight gradient boosting package_ Forust, is a lightweight
 package for building gradient boosted decision tree ensembles. All of the
 algorithm code is written in [Rust](https://www.rust-lang.org/), with a python
 wrapper. The rust package can be used directly, however, most examples shown
-here will be for the python wrapper. It implements the same algorithm as the
-[XGBoost](https://xgboost.readthedocs.io/en/stable/) package, and in many cases
-will give nearly identical results. I developed this package for a few reasons,
-mainly to better understand the XGBoost algorithm, additionally to have a fun
-project to work on in rust, and because I wanted to be able to experiment with
-adding new features to the algorithm in a smaller simpler codebase. All of the
-rust code for the package can be found in the [src](src/) directory, while all
-of the python wrapper code is in the [py-forust](py-forust/) directory. ##
-Installation The package can be installed directly from [pypi](https://
-pypi.org/project/forust/). ```shell pip install forust ``` To use in a rust
-project add the following to your Cargo.toml file. ```toml forust-ml = "0.1.7"
-``` ## Usage The `GradientBooster` class is currently the only public facing
-class in the package, and can be used to train gradient boosted decision tree
-ensembles with multiple objective functions. It can be initialized with the
-following arguments. - `objective_type` ***(str, optional)***: The name of
-objective function used to optimize. Valid options include "LogLoss" to use
-logistic loss as the objective function (binary classification), or
-"SquaredLoss" to use Squared Error as the objective function (continuous
-regression). Defaults to "LogLoss". - `iterations` ***(int, optional)***: Total
-number of trees to train in the ensemble. Defaults to 100. - `learning_rate`
-***(float, optional)***: Step size to use at each iteration. Each leaf weight
-is multiplied by this number. The smaller the value, the more conservative the
-weights will be. Defaults to 0.3. - `max_depth` ***(int, optional)***: Maximum
-depth of an individual tree. Valid values are 0 to infinity. Defaults to 5. -
-`max_leaves` ***(int, optional)***: Maximum number of leaves allowed on a tree.
-Valid values are 0 to infinity. This is the total number of final nodes.
-Defaults to sys.maxsize. - `l2` ***(float, optional)***: L2 regularization term
-applied to the weights of the tree. Valid values are 0 to infinity. Defaults to
-1.0. - `gamma` ***(float, optional)***: The minimum amount of loss required to
-further split a node. Valid values are 0 to infinity. Defaults to 0.0. -
+here will be for the python wrapper. For a self contained rust example, [see
+here](rs-example.md). It implements the same algorithm as the [XGBoost](https:/
+/xgboost.readthedocs.io/en/stable/) package, and in many cases will give nearly
+identical results. I developed this package for a few reasons, mainly to better
+understand the XGBoost algorithm, additionally to have a fun project to work on
+in rust, and because I wanted to be able to experiment with adding new features
+to the algorithm in a smaller simpler codebase. All of the rust code for the
+package can be found in the [src](src/) directory, while all of the python
+wrapper code is in the [py-forust](py-forust/) directory. ## Installation The
+package can be installed directly from [pypi](https://pypi.org/project/forust/
+). ```shell pip install forust ``` To use in a rust project add the following
+to your Cargo.toml file. ```toml forust-ml = "0.2.0" ``` ## Usage The
+`GradientBooster` class is currently the only public facing class in the
+package, and can be used to train gradient boosted decision tree ensembles with
+multiple objective functions. It can be initialized with the following
+arguments. - `objective_type` ***(str, optional)***: The name of objective
+function used to optimize. Valid options include "LogLoss" to use logistic loss
+as the objective function (binary classification), or "SquaredLoss" to use
+Squared Error as the objective function (continuous regression). Defaults to
+"LogLoss". - `iterations` ***(int, optional)***: Total number of trees to train
+in the ensemble. Defaults to 100. - `learning_rate` ***(float, optional)***:
+Step size to use at each iteration. Each leaf weight is multiplied by this
+number. The smaller the value, the more conservative the weights will be.
+Defaults to 0.3. - `max_depth` ***(int, optional)***: Maximum depth of an
+individual tree. Valid values are 0 to infinity. Defaults to 5. - `max_leaves`
+***(int, optional)***: Maximum number of leaves allowed on a tree. Valid values
+are 0 to infinity. This is the total number of final nodes. Defaults to
+sys.maxsize. - `l2` ***(float, optional)***: L2 regularization term applied to
+the weights of the tree. Valid values are 0 to infinity. Defaults to 1.0. -
+`gamma` ***(float, optional)***: The minimum amount of loss required to further
+split a node. Valid values are 0 to infinity. Defaults to 0.0. -
 `min_leaf_weight` ***(float, optional)***: Minimum sum of the hessian values of
 the loss function required to be in a node. Defaults to 1.0. - `base_score` ***
 (float, optional)***: The initial prediction value of the model. Defaults to
 0.5. - `nbins` ***(int, optional)***: Number of bins to calculate to partition
 the data. Setting this to a smaller number, will result in faster training
 time, while potentially sacrificing accuracy. If there are more bins, than
 unique values in a column, all unique values will be used. Defaults to 256. -
 `parallel` ***(bool, optional)***: Should multiple cores be used when training
 and predicting with this model? Defaults to `True`. - `allow_missing_splits`
 ***(bool, optional)***: Allow for splits to be made such that all missing
 values go down one branch, and all non-missing values go down the other, if
 this results in the greatest reduction of loss. If this is false, splits will
-only be made on non missing values. Defaults to `True`. - `impute_missing` ***
-(bool, optional)***: Automatically impute missing values, such that at every
-split the model learns the best direction to send missing values. If this is
-false, all missing values will default to right branch. Defaults to `True`. -
+only be made on non missing values. Defaults to `True`. -
 `monotone_constraints` ***(dict[Any, int], optional)***: Constraints that are
 used to enforce a specific relationship between the training features and the
 target variable. A dictionary should be provided where the keys are the feature
 index value if the model will be fit on a numpy array, or a feature name if it
 will be fit on a pandas Dataframe. The values of the dictionary should be an
 integer value of -1, 1, or 0 to specify the relationship that should be
 estimated between the respective feature and the target variable. Use a value
@@ -114,22 +112,17 @@
 matplotlib.pyplot as plt pd_values = model.partial_dependence(X=X,
 feature="age") fig = lineplot(x=pd_values[:,0], y=pd_values[:,1],) plt.title
 ("Partial Dependence Plot") plt.xlabel("Age") plt.ylabel("Log Odds") ```
 [https://github.com/jinlow/forust/raw/main/resources/pdp_plot_age.png] We can
 see how this is impacted if a model is created, where a specific constraint is
 applied to the feature using the `monotone_constraint` parameter. ```python
 model = GradientBooster( objective_type="LogLoss", monotone_constraints={"age":
--1}, ) model.fit(X, y) pd_values = model.partial_dependence(X=X, 1) fig =
-lineplot( x=pd_values[:, 0], y=pd_values[:, 1], ) plt.title("Partial Dependence
-Plot with Monotonicity") plt.xlabel("Age") plt.ylabel("Log Odds") ``` [https://
-github.com/jinlow/forust/raw/main/resources/pdp_plot_age_mono.png] ### Saving
-the model To save and subsequently load a trained booster, the `save_booster`
-and `load_booster` methods can be used. Each accepts a path, which is used to
-write the model to. The model is saved and loaded as a json object. ```python
-trained_model.save_booster("model_path.json") # To load a model from a json
-path. loaded_model = GradientBooster.load_model("model_path.json") ``` ## TODOs
-This is still a work in progress - [ ] Early stopping rounds * We should be
-able to accept a validation dataset, and this should be able to be used to
-determine when to stop training. - [X] Monotonicity support * Right now
-features are used in the model without any constraints. - [X] Ability to save a
-model. * The way the underlying trees are structured, they would lend
-themselves to being saved as JSon objects. - [ ] Clean up the CICD pipeline.
+-1}, ) model.fit(X, y) pd_values = model.partial_dependence(X=X, feature="age")
+fig = lineplot( x=pd_values[:, 0], y=pd_values[:, 1], ) plt.title("Partial
+Dependence Plot with Monotonicity") plt.xlabel("Age") plt.ylabel("Log Odds")
+``` [https://github.com/jinlow/forust/raw/main/resources/pdp_plot_age_mono.png]
+### Saving the model To save and subsequently load a trained booster, the
+`save_booster` and `load_booster` methods can be used. Each accepts a path,
+which is used to write the model to. The model is saved and loaded as a json
+object. ```python trained_model.save_booster("model_path.json") # To load a
+model from a json path. loaded_model = GradientBooster.load_model
+("model_path.json") ```
```

### Comparing `forust-0.1.7/local_dependencies/forust-ml/benches/forust_benchmarks.rs` & `forust-0.2.0/local_dependencies/forust-ml/benches/forust_benchmarks.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 use criterion::{black_box, criterion_group, criterion_main, Criterion};
 use forust_ml::binning::bin_matrix;
 use forust_ml::constraints::ConstraintMap;
 use forust_ml::data::Matrix;
 use forust_ml::gradientbooster::GradientBooster;
 use forust_ml::objective::{LogLoss, ObjectiveFunction};
-use forust_ml::splitter::Splitter;
+use forust_ml::splitter::MissingImputerSplitter;
 use forust_ml::tree::Tree;
 use forust_ml::utils::{fast_f64_sum, fast_sum, naive_sum};
 use std::fs;
+use std::time::Duration;
 
 pub fn tree_benchmarks(c: &mut Criterion) {
     let file = fs::read_to_string("resources/contiguous_no_missing_100k_samp_seed0.csv")
         .expect("Something went wrong reading the file");
     let data_vec: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
     let file = fs::read_to_string("resources/performance_100k_samp_seed0.csv")
         .expect("Something went wrong reading the file");
@@ -31,21 +32,20 @@
     });
 
     c.bench_function("calc_hess", |b| {
         b.iter(|| LogLoss::calc_hess(black_box(&y), black_box(&yhat), black_box(&w)))
     });
 
     let data = Matrix::new(&data_vec, y.len(), 5);
-    let splitter = Splitter {
+    let splitter = MissingImputerSplitter {
         l2: 1.0,
         gamma: 3.0,
         min_leaf_weight: 1.0,
         learning_rate: 0.3,
         allow_missing_splits: true,
-        impute_missing: true,
         constraints_map: ConstraintMap::new(),
     };
     let mut tree = Tree::new();
 
     let bindata = bin_matrix(&data, &w, 300).unwrap();
     let bdata = Matrix::new(&bindata.binned_data, data.rows, data.cols);
 
@@ -66,38 +66,42 @@
             train_tree.fit(
                 black_box(&bdata),
                 black_box(&bindata.cuts),
                 black_box(&g),
                 black_box(&h),
                 black_box(&splitter),
                 black_box(usize::MAX),
-                black_box(5),
-                black_box(true),
+                black_box(10),
+                black_box(false),
             );
         })
     });
     c.bench_function("Tree Predict (Single Threaded)", |b| {
         b.iter(|| tree.predict(black_box(&data), black_box(false)))
     });
     c.bench_function("Tree Predict (Multi Threaded)", |b| {
         b.iter(|| tree.predict(black_box(&data), black_box(true)))
     });
 
     // Gradient Booster
     // Bench building
-    c.bench_function("Train Booster", |b| {
+    let mut booster_train = c.benchmark_group("train-booster");
+    booster_train.warm_up_time(Duration::from_secs(10));
+    booster_train.sample_size(50);
+    // booster_train.sampling_mode(SamplingMode::Linear);
+    booster_train.bench_function("Train Booster", |b| {
         b.iter(|| {
-            let mut booster = GradientBooster::default();
+            let mut booster = GradientBooster::default().set_parallel(false);
             booster
                 .fit(black_box(&data), black_box(&y), black_box(&w))
                 .unwrap();
         })
     });
     let mut booster = GradientBooster::default();
     booster.fit(&data, &y, &w).unwrap();
-    c.bench_function("Predict Booster", |b| {
-        b.iter(|| booster.predict(black_box(&data), true))
+    booster_train.bench_function("Predict Booster", |b| {
+        b.iter(|| booster.predict(black_box(&data), false))
     });
 }
 
 criterion_group!(benches, tree_benchmarks);
 criterion_main!(benches);
```

### Comparing `forust-0.1.7/local_dependencies/forust-ml/resources/make_resources.py` & `forust-0.2.0/local_dependencies/forust-ml/scripts/make_resources.py`

 * *Files identical despite different names*

### Comparing `forust-0.1.7/local_dependencies/forust-ml/resources/pdp_plot_age.png` & `forust-0.2.0/local_dependencies/forust-ml/resources/pdp_plot_age.png`

 * *Files identical despite different names*

### Comparing `forust-0.1.7/local_dependencies/forust-ml/resources/titanic.csv` & `forust-0.2.0/local_dependencies/forust-ml/resources/titanic.csv`

 * *Files identical despite different names*

### Comparing `forust-0.1.7/local_dependencies/forust-ml/resources/tree-image-crop.png` & `forust-0.2.0/local_dependencies/forust-ml/resources/tree-image-crop.png`

 * *Files identical despite different names*

### Comparing `forust-0.1.7/local_dependencies/forust-ml/src/binning.rs` & `forust-0.2.0/local_dependencies/forust-ml/src/binning.rs`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         v_u
     } else {
         percentiles(v, sample_weight, pcts)
     }
 }
 
 // We want to be able to bin our dataset into discrete buckets.
-// First we will calculate percentils and the number of unique values
+// First we will calculate percentiles and the number of unique values
 // for each feature.
 // Then we will bucket them into bins from 0 to N + 1 where N is the number
 // of unique bin values created from the percentiles, and the very last
 // bin is missing values.
 // For now, we will just use usize, although, it would be good to see if
 // we can use something smaller, u8 for instance.
 // If we generated these cuts:
```

### Comparing `forust-0.1.7/local_dependencies/forust-ml/src/data.rs` & `forust-0.2.0/local_dependencies/forust-ml/src/data.rs`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,15 @@
 
 impl<'a, T> fmt::Display for Matrix<'a, T>
 where
     T: FromStr + std::fmt::Display,
     <T as FromStr>::Err: 'static + std::error::Error,
 {
     // This trait requires `fmt` with this exact signature.
+    /// Format a Matrix.
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         let mut val = String::new();
         for i in 0..self.rows {
             for j in 0..self.cols {
                 val.push_str(self.get(i, j).to_string().as_str());
                 if j == (self.cols - 1) {
                     val.push('\n');
@@ -156,15 +157,14 @@
             }
         }
         write!(f, "{}", val)
     }
 }
 
 /// A jagged column aligned matrix, that owns it's data contents.
-
 #[derive(Debug, Deserialize, Serialize)]
 pub struct JaggedMatrix<T> {
     /// The contents of the matrix.
     pub data: Vec<T>,
     /// The end index's of the matrix.
     pub ends: Vec<usize>,
     /// Number of columns in the matrix
@@ -174,15 +174,15 @@
 }
 
 impl<T> JaggedMatrix<T>
 where
     T: Copy,
 {
     /// Generate a jagged array from a vector of vectors
-    pub fn from_vecs(vecs: &Vec<Vec<T>>) -> Self {
+    pub fn from_vecs(vecs: &[Vec<T>]) -> Self {
         let mut data = Vec::new();
         let mut ends = Vec::new();
         let mut e = 0;
         let mut n_records = 0;
         for vec in vecs {
             for v in vec {
                 data.push(*v);
@@ -199,14 +199,15 @@
             cols,
             n_records,
         }
     }
 }
 
 impl<T> JaggedMatrix<T> {
+    /// Create a new jagged matrix.
     pub fn new() -> Self {
         JaggedMatrix {
             data: Vec::new(),
             ends: Vec::new(),
             cols: 0,
             n_records: 0,
         }
```

### Comparing `forust-0.1.7/local_dependencies/forust-ml/src/gradientbooster.rs` & `forust-0.2.0/local_dependencies/forust-ml/src/gradientbooster.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use crate::binning::bin_matrix;
 use crate::constraints::ConstraintMap;
 use crate::data::Matrix;
 use crate::errors::ForustError;
 use crate::objective::{gradient_hessian_callables, ObjectiveType};
-use crate::splitter::Splitter;
+use crate::splitter::MissingImputerSplitter;
 use crate::tree::Tree;
 use serde::{Deserialize, Serialize};
 use std::fs;
 
 /// Gradient Booster object
 ///
 /// * `objective_type` - The name of objective function used to optimize.
@@ -32,32 +32,28 @@
 ///   a smaller number, will result in faster training time, while potentially sacrificing
 ///   accuracy. If there are more bins, than unique values in a column, all unique values
 ///   will be used.
 /// * `allow_missing_splits` - Allow for splits to be made such that all missing values go
 ///   down one branch, and all non-missing values go down the other, if this results
 ///   in the greatest reduction of loss. If this is false, splits will only be made on non
 ///   missing values.
-/// * `impute_missing` - Automatically impute missing values, such that at every split
-///   the model learns the best direction to send missing values. If this is false, all
-///   missing values will default to right branch.
 #[derive(Deserialize, Serialize)]
 pub struct GradientBooster {
     pub objective_type: ObjectiveType,
     pub iterations: usize,
     pub learning_rate: f32,
     pub max_depth: usize,
     pub max_leaves: usize,
     pub l2: f32,
     pub gamma: f32,
     pub min_leaf_weight: f32,
     pub base_score: f64,
     pub nbins: u16,
     pub parallel: bool,
     pub allow_missing_splits: bool,
-    pub impute_missing: bool,
     pub monotone_constraints: Option<ConstraintMap>,
     pub trees: Vec<Tree>,
 }
 
 impl Default for GradientBooster {
     fn default() -> Self {
         Self::new(
@@ -69,15 +65,14 @@
             1.,
             0.,
             1.,
             0.5,
             256,
             true,
             true,
-            true,
             None,
         )
     }
 }
 
 impl GradientBooster {
     /// Gradient Booster object
@@ -116,15 +111,14 @@
         l2: f32,
         gamma: f32,
         min_leaf_weight: f32,
         base_score: f64,
         nbins: u16,
         parallel: bool,
         allow_missing_splits: bool,
-        impute_missing: bool,
         monotone_constraints: Option<ConstraintMap>,
     ) -> Self {
         GradientBooster {
             objective_type,
             iterations,
             learning_rate,
             max_depth,
@@ -132,15 +126,14 @@
             l2,
             gamma,
             min_leaf_weight,
             base_score,
             nbins,
             parallel,
             allow_missing_splits,
-            impute_missing,
             monotone_constraints,
             trees: Vec::new(),
         }
     }
 
     /// Fit the gradient booster on a provided dataset.
     ///
@@ -155,29 +148,31 @@
         sample_weight: &[f64],
     ) -> Result<(), ForustError> {
         let constraints_map = self
             .monotone_constraints
             .as_ref()
             .unwrap_or(&ConstraintMap::new())
             .to_owned();
-        let splitter = Splitter {
+        let splitter = MissingImputerSplitter {
             l2: self.l2,
             gamma: self.gamma,
             min_leaf_weight: self.min_leaf_weight,
             learning_rate: self.learning_rate,
             allow_missing_splits: self.allow_missing_splits,
-            impute_missing: self.impute_missing,
             constraints_map,
         };
         let mut yhat = vec![self.base_score; y.len()];
         let (calc_grad, calc_hess) = gradient_hessian_callables(&self.objective_type);
         let mut grad = calc_grad(y, &yhat, sample_weight);
         let mut hess = calc_hess(y, &yhat, sample_weight);
 
         // Generate binned data
+        // TODO
+        // In scikit-learn, they sample 200_000 records for generating the bins.
+        // we could consier that, especially if this proved to be a large bottleneck...
         let binned_data = bin_matrix(data, sample_weight, self.nbins)?;
         let bdata = Matrix::new(&binned_data.binned_data, data.rows, data.cols);
 
         for _ in 0..self.iterations {
             let mut tree = Tree::new();
             tree.fit(
                 &bdata,
@@ -194,14 +189,23 @@
             self.trees.push(tree);
             grad = calc_grad(y, &yhat, sample_weight);
             hess = calc_hess(y, &yhat, sample_weight);
         }
         Ok(())
     }
 
+    /// Fit the gradient booster on a provided dataset without any weights.
+    ///
+    /// * `data` -  Either a pandas DataFrame, or a 2 dimensional numpy array.
+    /// * `y` - Either a pandas Series, or a 1 dimensional numpy array.
+    pub fn fit_unweighted(&mut self, data: &Matrix<f64>, y: &[f64]) -> Result<(), ForustError> {
+        let w = vec![1.0; data.rows];
+        self.fit(data, y, &w)
+    }
+
     /// Generate predictions on data using the gradient booster.
     ///
     /// * `data` -  Either a pandas DataFrame, or a 2 dimensional numpy array.
     pub fn predict(&self, data: &Matrix<f64>, parallel: bool) -> Vec<f64> {
         let mut init_preds = vec![self.base_score; data.rows];
         self.trees.iter().for_each(|tree| {
             for (p_, val) in init_preds.iter_mut().zip(tree.predict(data, parallel)) {
@@ -261,14 +265,107 @@
     pub fn load_booster(path: &str) -> Result<Self, ForustError> {
         let json_str = match fs::read_to_string(path) {
             Ok(s) => Ok(s),
             Err(e) => Err(ForustError::UnableToRead(e.to_string())),
         }?;
         Self::from_json(&json_str)
     }
+
+    // Set methods for paramters
+    /// Set the objective_type on the booster.
+    /// * `objective_type` - The objective type of the booster.
+    pub fn set_objective_type(mut self, objective_type: ObjectiveType) -> Self {
+        self.objective_type = objective_type;
+        self
+    }
+
+    /// Set the iterations on the booster.
+    /// * `iterations` - The number of iterations of the booster.
+    pub fn set_iterations(mut self, iterations: usize) -> Self {
+        self.iterations = iterations;
+        self
+    }
+
+    /// Set the learning_rate on the booster.
+    /// * `learning_rate` - The learning rate of the booster.
+    pub fn set_learning_rate(mut self, learning_rate: f32) -> Self {
+        self.learning_rate = learning_rate;
+        self
+    }
+
+    /// Set the max_depth on the booster.
+    /// * `max_depth` - The maximum tree depth of the booster.
+    pub fn set_max_depth(mut self, max_depth: usize) -> Self {
+        self.max_depth = max_depth;
+        self
+    }
+
+    /// Set the max_leaves on the booster.
+    /// * `max_leaves` - The maximum number of leaves of the booster.
+    pub fn set_max_leaves(mut self, max_leaves: usize) -> Self {
+        self.max_leaves = max_leaves;
+        self
+    }
+
+    /// Set the l2 on the booster.
+    /// * `l2` - The l2 regulation term of the booster.
+    pub fn set_l2(mut self, l2: f32) -> Self {
+        self.l2 = l2;
+        self
+    }
+
+    /// Set the gamma on the booster.
+    /// * `gamma` - The gamma value of the booster.
+    pub fn set_gamma(mut self, gamma: f32) -> Self {
+        self.gamma = gamma;
+        self
+    }
+
+    /// Set the min_leaf_weight on the booster.
+    /// * `min_leaf_weight` - The minimum sum of the hession values allowed in the
+    ///     node of a tree of the booster.
+    pub fn set_min_leaf_weight(mut self, min_leaf_weight: f32) -> Self {
+        self.min_leaf_weight = min_leaf_weight;
+        self
+    }
+
+    /// Set the base_score on the booster.
+    /// * `base_score` - The base score of the booster.
+    pub fn set_base_score(mut self, base_score: f64) -> Self {
+        self.base_score = base_score;
+        self
+    }
+
+    /// Set the nbins on the booster.
+    /// * `nbins` - The nummber of bins used for partitioning the data of the booster.
+    pub fn set_nbins(mut self, nbins: u16) -> Self {
+        self.nbins = nbins;
+        self
+    }
+
+    /// Set the parallel on the booster.
+    /// * `parallel` - Set if the booster should be trained in parallels.
+    pub fn set_parallel(mut self, parallel: bool) -> Self {
+        self.parallel = parallel;
+        self
+    }
+
+    /// Set the allow_missing_splits on the booster.
+    /// * `allow_missing_splits` - Set if missing splits are allowed for the booster.
+    pub fn set_allow_missing_splits(mut self, allow_missing_splits: bool) -> Self {
+        self.allow_missing_splits = allow_missing_splits;
+        self
+    }
+
+    /// Set the monotone_constraints on the booster.
+    /// * `monotone_constraints` - The monotone constraints of the booster.
+    pub fn set_monotone_constraints(mut self, monotone_constraints: Option<ConstraintMap>) -> Self {
+        self.monotone_constraints = monotone_constraints;
+        self
+    }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
     use std::fs;
```

### Comparing `forust-0.1.7/local_dependencies/forust-ml/src/node.rs` & `forust-0.2.0/local_dependencies/forust-ml/src/node.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,91 +1,119 @@
 use crate::data::FloatData;
 use crate::histogram::HistogramMatrix;
-use crate::splitter::SplitInfo;
+use crate::splitter::{MissingInfo, NodeInfo, SplitInfo};
 use serde::{Deserialize, Serialize};
 use std::fmt::{self, Debug};
 
 #[derive(Debug, Deserialize, Serialize)]
 pub struct SplittableNode {
     pub num: usize,
     pub histograms: HistogramMatrix,
     pub weight_value: f32,
     pub gain_value: f32,
-    pub grad_sum: f32,
-    pub hess_sum: f32,
+    pub gradient_sum: f32,
+    pub hessian_sum: f32,
     pub depth: usize,
     pub split_value: f64,
     pub split_feature: usize,
     pub split_gain: f32,
-    pub missing_right: bool,
+    pub missing_node: usize,
     pub left_child: usize,
     pub right_child: usize,
     pub start_idx: usize,
     pub stop_idx: usize,
     pub lower_bound: f32,
     pub upper_bound: f32,
 }
 
 #[derive(Deserialize, Serialize)]
 pub struct ParentNode {
     pub num: usize,
     pub weight_value: f32,
-    pub hess_sum: f32,
+    pub hessian_sum: f32,
     pub depth: usize,
     pub split_value: f64,
     pub split_feature: usize,
     pub split_gain: f32,
-    pub missing_right: bool,
+    pub missing_node: usize,
     pub left_child: usize,
     pub right_child: usize,
 }
 
 #[derive(Deserialize, Serialize)]
 pub struct LeafNode {
     pub num: usize,
     pub weight_value: f32,
-    pub hess_sum: f32,
+    pub hessian_sum: f32,
     pub depth: usize,
 }
 
 #[derive(Deserialize, Serialize)]
 pub enum TreeNode {
     Parent(ParentNode),
     Leaf(LeafNode),
     Splittable(SplittableNode),
 }
 
 impl SplittableNode {
+    pub fn from_node_info(
+        num: usize,
+        histograms: HistogramMatrix,
+        depth: usize,
+        start_idx: usize,
+        stop_idx: usize,
+        node_info: NodeInfo,
+    ) -> Self {
+        SplittableNode {
+            num,
+            histograms,
+            weight_value: node_info.weight,
+            gain_value: node_info.gain,
+            gradient_sum: node_info.grad,
+            hessian_sum: node_info.cover,
+            depth,
+            split_value: f64::ZERO,
+            split_feature: 0,
+            split_gain: f32::ZERO,
+            missing_node: 0,
+            left_child: 0,
+            right_child: 0,
+            start_idx,
+            stop_idx,
+            lower_bound: node_info.bounds.0,
+            upper_bound: node_info.bounds.1,
+        }
+    }
+
     #[allow(clippy::too_many_arguments)]
     pub fn new(
         num: usize,
         histograms: HistogramMatrix,
         weight_value: f32,
         gain_value: f32,
-        grad_sum: f32,
-        hess_sum: f32,
+        gradient_sum: f32,
+        hessian_sum: f32,
         depth: usize,
-        missing_right: bool,
         start_idx: usize,
         stop_idx: usize,
         lower_bound: f32,
         upper_bound: f32,
     ) -> Self {
         SplittableNode {
             num,
             histograms,
             weight_value,
             gain_value,
-            grad_sum,
-            hess_sum,
+            gradient_sum,
+            hessian_sum,
             depth,
             split_value: f64::ZERO,
             split_feature: 0,
             split_gain: f32::ZERO,
-            missing_right,
+            missing_node: 0,
             left_child: 0,
             right_child: 0,
             start_idx,
             stop_idx,
             lower_bound,
             upper_bound,
         }
@@ -96,33 +124,38 @@
         left_child: usize,
         right_child: usize,
         split_info: &SplitInfo,
     ) {
         self.left_child = left_child;
         self.right_child = right_child;
         self.split_feature = split_info.split_feature;
-        self.split_gain = split_info.left_gain + split_info.right_gain - self.gain_value;
+        self.split_gain = split_info.left_node.gain + split_info.right_node.gain - self.gain_value;
         self.split_value = split_info.split_value;
-        self.missing_right = split_info.missing_right;
+        self.missing_node = match split_info.missing_node {
+            MissingInfo::Left => left_child,
+            MissingInfo::Right => right_child,
+            MissingInfo::Branch(_) => todo!(),
+            MissingInfo::EmptyBranch => todo!(),
+        };
     }
     pub fn as_leaf_node(&self) -> TreeNode {
         TreeNode::Leaf(LeafNode {
             num: self.num,
             weight_value: self.weight_value,
-            hess_sum: self.hess_sum,
+            hessian_sum: self.hessian_sum,
             depth: self.depth,
         })
     }
     pub fn as_parent_node(&self) -> TreeNode {
         TreeNode::Parent(ParentNode {
             num: self.num,
             weight_value: self.weight_value,
-            hess_sum: self.hess_sum,
+            hessian_sum: self.hessian_sum,
             depth: self.depth,
-            missing_right: self.missing_right,
+            missing_node: self.missing_node,
             split_value: self.split_value,
             split_feature: self.split_feature,
             split_gain: self.split_gain,
             left_child: self.left_child,
             right_child: self.right_child,
         })
     }
@@ -131,50 +164,40 @@
 impl fmt::Display for TreeNode {
     // This trait requires `fmt` with this exact signature.
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         match self {
             TreeNode::Leaf(leaf) => write!(
                 f,
                 "{}:leaf={},cover={}",
-                leaf.num, leaf.weight_value, leaf.hess_sum
+                leaf.num, leaf.weight_value, leaf.hessian_sum
             ),
             TreeNode::Parent(parent) => {
-                let missing = if parent.missing_right {
-                    parent.right_child
-                } else {
-                    parent.left_child
-                };
                 write!(
                     f,
                     "{}:[{} < {}] yes={},no={},missing={},gain={},cover={}",
                     parent.num,
                     parent.split_feature,
                     parent.split_value,
                     parent.left_child,
                     parent.right_child,
-                    missing,
+                    parent.missing_node,
                     parent.split_gain,
-                    parent.hess_sum
+                    parent.hessian_sum
                 )
             }
             TreeNode::Splittable(node) => {
-                let missing = if node.missing_right {
-                    node.right_child
-                } else {
-                    node.left_child
-                };
                 write!(
                     f,
                     "SPLITTABLE - {}:[{} < {}] yes={},no={},missing={},gain={},cover={}",
                     node.num,
                     node.split_feature,
                     node.split_value,
-                    missing,
+                    node.missing_node,
                     node.left_child,
                     node.right_child,
                     node.split_gain,
-                    node.hess_sum
+                    node.hessian_sum
                 )
             }
         }
     }
 }
```

### Comparing `forust-0.1.7/local_dependencies/forust-ml/src/objective.rs` & `forust-0.2.0/local_dependencies/forust-ml/src/objective.rs`

 * *Files identical despite different names*

### Comparing `forust-0.1.7/local_dependencies/forust-ml/src/partial_dependence.rs` & `forust-0.2.0/local_dependencies/forust-ml/src/partial_dependence.rs`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 //     base_score: f64,
 //     tree_prediction: f64,
 
 // }
 
 fn get_node_cover(tree: &Tree, node_idx: usize) -> f32 {
     match &tree.nodes[node_idx] {
-        TreeNode::Leaf(n) => n.hess_sum,
-        TreeNode::Parent(n) => n.hess_sum,
+        TreeNode::Leaf(n) => n.hessian_sum,
+        TreeNode::Parent(n) => n.hessian_sum,
         TreeNode::Splittable(_) => unreachable!(),
     }
 }
 
 pub fn tree_partial_dependence(
     tree: &Tree,
     node_idx: usize,
@@ -26,27 +26,22 @@
 ) -> f64 {
     let node = &tree.nodes[node_idx];
     match node {
         TreeNode::Leaf(n) => f64::from(proportion * n.weight_value),
         TreeNode::Parent(n) => {
             if n.split_feature == feature {
                 let child = if value.is_nan() {
-                    if n.missing_right {
-                        n.right_child
-                    } else {
-                        n.left_child
-                    }
+                    n.missing_node
                 } else if value < n.split_value {
                     n.left_child
                 } else {
                     n.right_child
                 };
                 tree_partial_dependence(tree, child, feature, value, proportion)
             } else {
-                // Left cover
                 let left_cover = get_node_cover(tree, n.left_child);
                 let right_cover = get_node_cover(tree, n.right_child);
                 let total_cover = left_cover + right_cover;
 
                 tree_partial_dependence(
                     tree,
                     n.left_child,
@@ -69,15 +64,15 @@
 #[cfg(test)]
 mod tests {
     use super::*;
     use crate::binning::bin_matrix;
     use crate::constraints::ConstraintMap;
     use crate::data::Matrix;
     use crate::objective::{LogLoss, ObjectiveFunction};
-    use crate::splitter::Splitter;
+    use crate::splitter::MissingImputerSplitter;
     use crate::tree::Tree;
     use std::fs;
     #[test]
     fn test_partial_dependence() {
         let file = fs::read_to_string("resources/contiguous_no_missing.csv")
             .expect("Something went wrong reading the file");
         let data_vec: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
@@ -86,21 +81,20 @@
         let y: Vec<f64> = file.lines().map(|x| x.parse::<f64>().unwrap()).collect();
         let yhat = vec![0.5; y.len()];
         let w = vec![1.; y.len()];
         let g = LogLoss::calc_grad(&y, &yhat, &w);
         let h = LogLoss::calc_hess(&y, &yhat, &w);
 
         let data = Matrix::new(&data_vec, 891, 5);
-        let splitter = Splitter {
+        let splitter = MissingImputerSplitter {
             l2: 1.0,
             gamma: 3.0,
             min_leaf_weight: 1.0,
             learning_rate: 0.3,
             allow_missing_splits: true,
-            impute_missing: true,
             constraints_map: ConstraintMap::new(),
         };
         let mut tree = Tree::new();
 
         let b = bin_matrix(&data, &w, 300).unwrap();
         let bdata = Matrix::new(&b.binned_data, data.rows, data.cols);
```

### Comparing `forust-0.1.7/.gitignore` & `forust-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `forust-0.1.7/README.md` & `forust-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,29 +8,29 @@
   <a href="https://pypi.org/project/forust/">![PyPI](https://img.shields.io/pypi/v/forust?color=gr&style=for-the-badge)</a>
   <a href="https://crates.io/crates/forust-ml">![Crates.io](https://img.shields.io/crates/v/forust-ml?color=gr&style=for-the-badge)</a>
 
 </div>
 
 # Forust
 ## _A lightweight gradient boosting package_
-Forust, is a lightweight package for building gradient boosted decision tree ensembles. All of the algorithm code is written in [Rust](https://www.rust-lang.org/), with a python wrapper. The rust package can be used directly, however, most examples shown here will be for the python wrapper. It implements the same algorithm as the [XGBoost](https://xgboost.readthedocs.io/en/stable/) package, and in many cases will give nearly identical results.
+Forust, is a lightweight package for building gradient boosted decision tree ensembles. All of the algorithm code is written in [Rust](https://www.rust-lang.org/), with a python wrapper. The rust package can be used directly, however, most examples shown here will be for the python wrapper. For a self contained rust example, [see here](rs-example.md). It implements the same algorithm as the [XGBoost](https://xgboost.readthedocs.io/en/stable/) package, and in many cases will give nearly identical results.
 
 I developed this package for a few reasons, mainly to better understand the XGBoost algorithm, additionally to have a fun project to work on in rust, and because I wanted to be able to experiment with adding new features to the algorithm in a smaller simpler codebase.
 
 All of the rust code for the package can be found in the [src](src/) directory, while all of the python wrapper code is in the [py-forust](py-forust/) directory.
 
 ## Installation
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.1.7"
+forust-ml = "0.2.0"
 ```
 
 ## Usage
 The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
 
 It can be initialized with the following arguments.
 
@@ -57,15 +57,14 @@
  - `nbins` ***(int, optional)***: Number of bins to calculate to partition the data. Setting this to
     a smaller number, will result in faster training time, while potentially sacrificing
     accuracy. If there are more bins, than unique values in a column, all unique values
     will be used. Defaults to 256.
  - `parallel` ***(bool, optional)***: Should multiple cores be used when training and predicting
     with this model? Defaults to `True`.
  - `allow_missing_splits` ***(bool, optional)***: Allow for splits to be made such that all missing values go down one branch, and all non-missing values go down the other, if this results in the greatest reduction of loss. If this is false, splits will only be made on non missing values. Defaults to `True`.
- - `impute_missing` ***(bool, optional)***: Automatically impute missing values, such that at every split the model learns the best direction to send missing values. If this is false, all missing values will default to right branch. Defaults to `True`.
  - `monotone_constraints` ***(dict[Any, int], optional)***: Constraints that are used to enforce a specific relationship between the training features and the target variable. A dictionary should be provided where the keys are the feature index value if the model will be fit on a numpy array, or a feature name if it will be fit on a pandas Dataframe. The values of the dictionary should be an integer value of -1, 1, or 0 to specify the relationship that should be estimated between the respective feature and the target variable. Use a value of -1 to enforce a negative relationship, 1 a positive relationship, and 0 will enforce no specific relationship at all. Features not included in the mapping will not have any constraint applied. If `None` is passed no constraints will be enforced on any variable.  Defaults to `None`.
 
 ### Training and Predicting
 
 Once, the booster has been initialized, it can be fit on a provided dataset, and performance field. After fitting, the model can be used to predict on a dataset.
 In the case of this example, the predictions are the log odds of a given record being 1.
 
@@ -152,15 +151,15 @@
 ```python
 model = GradientBooster(
     objective_type="LogLoss",
     monotone_constraints={"age": -1},
 )
 model.fit(X, y)
 
-pd_values = model.partial_dependence(X=X, 1)
+pd_values = model.partial_dependence(X=X, feature="age")
 fig = lineplot(
     x=pd_values[:, 0],
     y=pd_values[:, 1],
 )
 plt.title("Partial Dependence Plot with Monotonicity")
 plt.xlabel("Age")
 plt.ylabel("Log Odds")
@@ -172,17 +171,7 @@
 
 ```python
 trained_model.save_booster("model_path.json")
 
 # To load a model from a json path.
 loaded_model = GradientBooster.load_model("model_path.json")
 ```
-
-## TODOs
-This is still a work in progress
-- [ ] Early stopping rounds
-    * We should be able to accept a validation dataset, and this should be able to be used to determine when to stop training.
-- [X] Monotonicity support
-    * Right now features are used in the model without any constraints.
-- [X] Ability to save a model.
-    * The way the underlying trees are structured, they would lend themselves to being saved as JSon objects.
-- [ ] Clean up the CICD pipeline.
```

#### html2text {}

```diff
@@ -2,60 +2,58 @@
  ![PyPI](https://img.shields.io/pypi/v/forust?color=gr&style=for-the-badge) !
  [Crates.io](https://img.shields.io/crates/v/forust-ml?color=gr&style=for-the-
                                     badge)
 # Forust ## _A lightweight gradient boosting package_ Forust, is a lightweight
 package for building gradient boosted decision tree ensembles. All of the
 algorithm code is written in [Rust](https://www.rust-lang.org/), with a python
 wrapper. The rust package can be used directly, however, most examples shown
-here will be for the python wrapper. It implements the same algorithm as the
-[XGBoost](https://xgboost.readthedocs.io/en/stable/) package, and in many cases
-will give nearly identical results. I developed this package for a few reasons,
-mainly to better understand the XGBoost algorithm, additionally to have a fun
-project to work on in rust, and because I wanted to be able to experiment with
-adding new features to the algorithm in a smaller simpler codebase. All of the
-rust code for the package can be found in the [src](src/) directory, while all
-of the python wrapper code is in the [py-forust](py-forust/) directory. ##
-Installation The package can be installed directly from [pypi](https://
-pypi.org/project/forust/). ```shell pip install forust ``` To use in a rust
-project add the following to your Cargo.toml file. ```toml forust-ml = "0.1.7"
-``` ## Usage The `GradientBooster` class is currently the only public facing
-class in the package, and can be used to train gradient boosted decision tree
-ensembles with multiple objective functions. It can be initialized with the
-following arguments. - `objective_type` ***(str, optional)***: The name of
-objective function used to optimize. Valid options include "LogLoss" to use
-logistic loss as the objective function (binary classification), or
-"SquaredLoss" to use Squared Error as the objective function (continuous
-regression). Defaults to "LogLoss". - `iterations` ***(int, optional)***: Total
-number of trees to train in the ensemble. Defaults to 100. - `learning_rate`
-***(float, optional)***: Step size to use at each iteration. Each leaf weight
-is multiplied by this number. The smaller the value, the more conservative the
-weights will be. Defaults to 0.3. - `max_depth` ***(int, optional)***: Maximum
-depth of an individual tree. Valid values are 0 to infinity. Defaults to 5. -
-`max_leaves` ***(int, optional)***: Maximum number of leaves allowed on a tree.
-Valid values are 0 to infinity. This is the total number of final nodes.
-Defaults to sys.maxsize. - `l2` ***(float, optional)***: L2 regularization term
-applied to the weights of the tree. Valid values are 0 to infinity. Defaults to
-1.0. - `gamma` ***(float, optional)***: The minimum amount of loss required to
-further split a node. Valid values are 0 to infinity. Defaults to 0.0. -
+here will be for the python wrapper. For a self contained rust example, [see
+here](rs-example.md). It implements the same algorithm as the [XGBoost](https:/
+/xgboost.readthedocs.io/en/stable/) package, and in many cases will give nearly
+identical results. I developed this package for a few reasons, mainly to better
+understand the XGBoost algorithm, additionally to have a fun project to work on
+in rust, and because I wanted to be able to experiment with adding new features
+to the algorithm in a smaller simpler codebase. All of the rust code for the
+package can be found in the [src](src/) directory, while all of the python
+wrapper code is in the [py-forust](py-forust/) directory. ## Installation The
+package can be installed directly from [pypi](https://pypi.org/project/forust/
+). ```shell pip install forust ``` To use in a rust project add the following
+to your Cargo.toml file. ```toml forust-ml = "0.2.0" ``` ## Usage The
+`GradientBooster` class is currently the only public facing class in the
+package, and can be used to train gradient boosted decision tree ensembles with
+multiple objective functions. It can be initialized with the following
+arguments. - `objective_type` ***(str, optional)***: The name of objective
+function used to optimize. Valid options include "LogLoss" to use logistic loss
+as the objective function (binary classification), or "SquaredLoss" to use
+Squared Error as the objective function (continuous regression). Defaults to
+"LogLoss". - `iterations` ***(int, optional)***: Total number of trees to train
+in the ensemble. Defaults to 100. - `learning_rate` ***(float, optional)***:
+Step size to use at each iteration. Each leaf weight is multiplied by this
+number. The smaller the value, the more conservative the weights will be.
+Defaults to 0.3. - `max_depth` ***(int, optional)***: Maximum depth of an
+individual tree. Valid values are 0 to infinity. Defaults to 5. - `max_leaves`
+***(int, optional)***: Maximum number of leaves allowed on a tree. Valid values
+are 0 to infinity. This is the total number of final nodes. Defaults to
+sys.maxsize. - `l2` ***(float, optional)***: L2 regularization term applied to
+the weights of the tree. Valid values are 0 to infinity. Defaults to 1.0. -
+`gamma` ***(float, optional)***: The minimum amount of loss required to further
+split a node. Valid values are 0 to infinity. Defaults to 0.0. -
 `min_leaf_weight` ***(float, optional)***: Minimum sum of the hessian values of
 the loss function required to be in a node. Defaults to 1.0. - `base_score` ***
 (float, optional)***: The initial prediction value of the model. Defaults to
 0.5. - `nbins` ***(int, optional)***: Number of bins to calculate to partition
 the data. Setting this to a smaller number, will result in faster training
 time, while potentially sacrificing accuracy. If there are more bins, than
 unique values in a column, all unique values will be used. Defaults to 256. -
 `parallel` ***(bool, optional)***: Should multiple cores be used when training
 and predicting with this model? Defaults to `True`. - `allow_missing_splits`
 ***(bool, optional)***: Allow for splits to be made such that all missing
 values go down one branch, and all non-missing values go down the other, if
 this results in the greatest reduction of loss. If this is false, splits will
-only be made on non missing values. Defaults to `True`. - `impute_missing` ***
-(bool, optional)***: Automatically impute missing values, such that at every
-split the model learns the best direction to send missing values. If this is
-false, all missing values will default to right branch. Defaults to `True`. -
+only be made on non missing values. Defaults to `True`. -
 `monotone_constraints` ***(dict[Any, int], optional)***: Constraints that are
 used to enforce a specific relationship between the training features and the
 target variable. A dictionary should be provided where the keys are the feature
 index value if the model will be fit on a numpy array, or a feature name if it
 will be fit on a pandas Dataframe. The values of the dictionary should be an
 integer value of -1, 1, or 0 to specify the relationship that should be
 estimated between the respective feature and the target variable. Use a value
@@ -114,22 +112,17 @@
 matplotlib.pyplot as plt pd_values = model.partial_dependence(X=X,
 feature="age") fig = lineplot(x=pd_values[:,0], y=pd_values[:,1],) plt.title
 ("Partial Dependence Plot") plt.xlabel("Age") plt.ylabel("Log Odds") ```
 [https://github.com/jinlow/forust/raw/main/resources/pdp_plot_age.png] We can
 see how this is impacted if a model is created, where a specific constraint is
 applied to the feature using the `monotone_constraint` parameter. ```python
 model = GradientBooster( objective_type="LogLoss", monotone_constraints={"age":
--1}, ) model.fit(X, y) pd_values = model.partial_dependence(X=X, 1) fig =
-lineplot( x=pd_values[:, 0], y=pd_values[:, 1], ) plt.title("Partial Dependence
-Plot with Monotonicity") plt.xlabel("Age") plt.ylabel("Log Odds") ``` [https://
-github.com/jinlow/forust/raw/main/resources/pdp_plot_age_mono.png] ### Saving
-the model To save and subsequently load a trained booster, the `save_booster`
-and `load_booster` methods can be used. Each accepts a path, which is used to
-write the model to. The model is saved and loaded as a json object. ```python
-trained_model.save_booster("model_path.json") # To load a model from a json
-path. loaded_model = GradientBooster.load_model("model_path.json") ``` ## TODOs
-This is still a work in progress - [ ] Early stopping rounds * We should be
-able to accept a validation dataset, and this should be able to be used to
-determine when to stop training. - [X] Monotonicity support * Right now
-features are used in the model without any constraints. - [X] Ability to save a
-model. * The way the underlying trees are structured, they would lend
-themselves to being saved as JSon objects. - [ ] Clean up the CICD pipeline.
+-1}, ) model.fit(X, y) pd_values = model.partial_dependence(X=X, feature="age")
+fig = lineplot( x=pd_values[:, 0], y=pd_values[:, 1], ) plt.title("Partial
+Dependence Plot with Monotonicity") plt.xlabel("Age") plt.ylabel("Log Odds")
+``` [https://github.com/jinlow/forust/raw/main/resources/pdp_plot_age_mono.png]
+### Saving the model To save and subsequently load a trained booster, the
+`save_booster` and `load_booster` methods can be used. Each accepts a path,
+which is used to write the model to. The model is saved and loaded as a json
+object. ```python trained_model.save_booster("model_path.json") # To load a
+model from a json path. loaded_model = GradientBooster.load_model
+("model_path.json") ```
```

### Comparing `forust-0.1.7/forust/__init__.py` & `forust-0.2.0/forust/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,14 @@
         l2: float = 1.0,
         gamma: float = 0.0,
         min_leaf_weight: float = 1.0,
         base_score: float = 0.5,
         nbins: int = 256,
         parallel: bool = True,
         allow_missing_splits: bool = True,
-        impute_missing: bool = True,
         monotone_constraints: Union[dict[Any, int], None] = None,
     ):
         """Gradient Booster Class, used to generate gradient boosted decision tree ensembles.
 
         Args:
             objective_type (str, optional): The name of objective function used to optimize.
                 Valid options include "LogLoss" to use logistic loss as the objective function
@@ -110,17 +109,14 @@
                 will be used. Defaults to 256.
             parallel (bool, optional): Should multiple cores be used when training and predicting
                 with this model? Defaults to `True`.
             allow_missing_splits (bool, optional): Allow for splits to be made such that all missing values go
                 down one branch, and all non-missing values go down the other, if this results
                 in the greatest reduction of loss. If this is false, splits will only be made on non
                 missing values. Defaults to `True`.
-            impute_missing (bool, optional): Automatically impute missing values, such that at every split
-                the model learns the best direction to send missing values. If this is false, all
-                missing values will default to right branch. Defaults to `True`.
             monotone_constraints (dict[Any, int], optional): Constraints that are used to enforce a
                 specific relationship between the training features and the target variable. A dictionary
                 should be provided where the keys are the feature index value if the model will be fit on
                 a numpy array, or a feature name if it will be fit on a pandas Dataframe. The values of
                 the dictionary should be an integer value of -1, 1, or 0 to specify the relationship
                 that should be estimated between the respective feature and the target variable.
                 Use a value of -1 to enforce a negative relationship, 1 a positive relationship,
@@ -140,15 +136,14 @@
             l2=l2,
             gamma=gamma,
             min_leaf_weight=min_leaf_weight,
             base_score=base_score,
             nbins=nbins,
             parallel=parallel,
             allow_missing_splits=allow_missing_splits,
-            impute_missing=impute_missing,
             monotone_constraints={},
         )
         monotone_constraints_ = (
             {} if monotone_constraints is None else monotone_constraints
         )
         self.booster = cast(BoosterType, booster)
         self.objective_type = objective_type
@@ -159,15 +154,14 @@
         self.l2 = l2
         self.gamma = gamma
         self.min_leaf_weight = min_leaf_weight
         self.base_score = base_score
         self.nbins = nbins
         self.parallel = parallel
         self.allow_missing_splits = (allow_missing_splits,)
-        self.impute_missing = (impute_missing,)
         self.monotone_constraints = monotone_constraints_
 
     def fit(
         self,
         X: FrameLike,
         y: ArrayLike,
         sample_weight: Union[ArrayLike, None] = None,
```

### Comparing `forust-0.1.7/src/lib.rs` & `forust-0.2.0/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,14 @@
         l2: f32,
         gamma: f32,
         min_leaf_weight: f32,
         base_score: f64,
         nbins: u16,
         parallel: bool,
         allow_missing_splits: bool,
-        impute_missing: bool,
         monotone_constraints: HashMap<usize, i8>,
     ) -> PyResult<Self> {
         let constraints = int_map_to_constraint_map(monotone_constraints)?;
         let objective_ = match objective_type {
             "LogLoss" => Ok(ObjectiveType::LogLoss),
             "SquaredLoss" => Ok(ObjectiveType::SquaredLoss),
             _ => Err(PyValueError::new_err(format!("Not a valid objective type passed, expected one of 'LogLoss', 'SquaredLoss', but '{}' was provided.", objective_type))),
@@ -66,15 +65,14 @@
             l2,
             gamma,
             min_leaf_weight,
             base_score,
             nbins,
             parallel,
             allow_missing_splits,
-            impute_missing,
             Some(constraints),
         );
         Ok(GradientBooster { booster })
     }
 
     #[setter]
     fn set_monotone_constraints(&mut self, value: HashMap<usize, i8>) -> PyResult<()> {
@@ -194,15 +192,14 @@
             ("base_score", self.booster.base_score.to_object(py)),
             ("nbins", self.booster.nbins.to_object(py)),
             ("parallel", self.booster.parallel.to_object(py)),
             (
                 "allow_missing_splits",
                 self.booster.allow_missing_splits.to_object(py),
             ),
-            ("impute_missing", self.booster.impute_missing.to_object(py)),
             ("monotone_constraints", constraints.to_object(py)),
         ];
         let dict = key_vals.into_py_dict(py);
         Ok(dict.to_object(py))
     }
 }
```

### Comparing `forust-0.1.7/tests/test_booster.py` & `forust-0.2.0/tests/test_booster.py`

 * *Files identical despite different names*

### Comparing `forust-0.1.7/LICENSE` & `forust-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `forust-0.1.7/PKG-INFO` & `forust-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 Metadata-Version: 2.1
 Name: forust
-Version: 0.1.7
+Version: 0.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: numpy>=1.21
 Requires-Dist: pandas>=1.3
+Requires-Dist: maturin; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: seaborn; extra == 'dev'
+Requires-Dist: xgboost==1.6.1; extra == 'dev'
+Requires-Dist: scikit-learn; extra == 'dev'
+Provides-Extra: dev
 License-File: LICENSE
 Summary: A lightweight gradient boosting implementation in Rust.
 Keywords: rust,forust,machine learning,xgboost,tree model,decision tree
 Author: James Inlow
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 <p align="center">
   <img  height="340" src="https://github.com/jinlow/forust/raw/main/resources/tree-image-crop.png">
 </p>
 
 
@@ -23,29 +29,29 @@
   <a href="https://pypi.org/project/forust/">![PyPI](https://img.shields.io/pypi/v/forust?color=gr&style=for-the-badge)</a>
   <a href="https://crates.io/crates/forust-ml">![Crates.io](https://img.shields.io/crates/v/forust-ml?color=gr&style=for-the-badge)</a>
 
 </div>
 
 # Forust
 ## _A lightweight gradient boosting package_
-Forust, is a lightweight package for building gradient boosted decision tree ensembles. All of the algorithm code is written in [Rust](https://www.rust-lang.org/), with a python wrapper. The rust package can be used directly, however, most examples shown here will be for the python wrapper. It implements the same algorithm as the [XGBoost](https://xgboost.readthedocs.io/en/stable/) package, and in many cases will give nearly identical results.
+Forust, is a lightweight package for building gradient boosted decision tree ensembles. All of the algorithm code is written in [Rust](https://www.rust-lang.org/), with a python wrapper. The rust package can be used directly, however, most examples shown here will be for the python wrapper. For a self contained rust example, [see here](rs-example.md). It implements the same algorithm as the [XGBoost](https://xgboost.readthedocs.io/en/stable/) package, and in many cases will give nearly identical results.
 
 I developed this package for a few reasons, mainly to better understand the XGBoost algorithm, additionally to have a fun project to work on in rust, and because I wanted to be able to experiment with adding new features to the algorithm in a smaller simpler codebase.
 
 All of the rust code for the package can be found in the [src](src/) directory, while all of the python wrapper code is in the [py-forust](py-forust/) directory.
 
 ## Installation
 The package can be installed directly from [pypi](https://pypi.org/project/forust/).
 ```shell
 pip install forust
 ```
 
 To use in a rust project add the following to your Cargo.toml file.
 ```toml
-forust-ml = "0.1.7"
+forust-ml = "0.2.0"
 ```
 
 ## Usage
 The `GradientBooster` class is currently the only public facing class in the package, and can be used to train gradient boosted decision tree ensembles with multiple objective functions.
 
 It can be initialized with the following arguments.
 
@@ -72,15 +78,14 @@
  - `nbins` ***(int, optional)***: Number of bins to calculate to partition the data. Setting this to
     a smaller number, will result in faster training time, while potentially sacrificing
     accuracy. If there are more bins, than unique values in a column, all unique values
     will be used. Defaults to 256.
  - `parallel` ***(bool, optional)***: Should multiple cores be used when training and predicting
     with this model? Defaults to `True`.
  - `allow_missing_splits` ***(bool, optional)***: Allow for splits to be made such that all missing values go down one branch, and all non-missing values go down the other, if this results in the greatest reduction of loss. If this is false, splits will only be made on non missing values. Defaults to `True`.
- - `impute_missing` ***(bool, optional)***: Automatically impute missing values, such that at every split the model learns the best direction to send missing values. If this is false, all missing values will default to right branch. Defaults to `True`.
  - `monotone_constraints` ***(dict[Any, int], optional)***: Constraints that are used to enforce a specific relationship between the training features and the target variable. A dictionary should be provided where the keys are the feature index value if the model will be fit on a numpy array, or a feature name if it will be fit on a pandas Dataframe. The values of the dictionary should be an integer value of -1, 1, or 0 to specify the relationship that should be estimated between the respective feature and the target variable. Use a value of -1 to enforce a negative relationship, 1 a positive relationship, and 0 will enforce no specific relationship at all. Features not included in the mapping will not have any constraint applied. If `None` is passed no constraints will be enforced on any variable.  Defaults to `None`.
 
 ### Training and Predicting
 
 Once, the booster has been initialized, it can be fit on a provided dataset, and performance field. After fitting, the model can be used to predict on a dataset.
 In the case of this example, the predictions are the log odds of a given record being 1.
 
@@ -167,15 +172,15 @@
 ```python
 model = GradientBooster(
     objective_type="LogLoss",
     monotone_constraints={"age": -1},
 )
 model.fit(X, y)
 
-pd_values = model.partial_dependence(X=X, 1)
+pd_values = model.partial_dependence(X=X, feature="age")
 fig = lineplot(
     x=pd_values[:, 0],
     y=pd_values[:, 1],
 )
 plt.title("Partial Dependence Plot with Monotonicity")
 plt.xlabel("Age")
 plt.ylabel("Log Odds")
@@ -188,17 +193,7 @@
 ```python
 trained_model.save_booster("model_path.json")
 
 # To load a model from a json path.
 loaded_model = GradientBooster.load_model("model_path.json")
 ```
 
-## TODOs
-This is still a work in progress
-- [ ] Early stopping rounds
-    * We should be able to accept a validation dataset, and this should be able to be used to determine when to stop training.
-- [X] Monotonicity support
-    * Right now features are used in the model without any constraints.
-- [X] Ability to save a model.
-    * The way the underlying trees are structured, they would lend themselves to being saved as JSon objects.
-- [ ] Clean up the CICD pipeline.
-
```

#### html2text {}

```diff
@@ -1,69 +1,70 @@
-Metadata-Version: 2.1 Name: forust Version: 0.1.7 Classifier: Programming
+Metadata-Version: 2.1 Name: forust Version: 0.2.0 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: numpy>=1.21 Requires-Dist: pandas>=1.3 License-File: LICENSE
-Summary: A lightweight gradient boosting implementation in Rust. Keywords:
+Requires-Dist: numpy>=1.21 Requires-Dist: pandas>=1.3 Requires-Dist: maturin;
+extra == 'dev' Requires-Dist: pytest; extra == 'dev' Requires-Dist: seaborn;
+extra == 'dev' Requires-Dist: xgboost==1.6.1; extra == 'dev' Requires-Dist:
+scikit-learn; extra == 'dev' Provides-Extra: dev License-File: LICENSE Summary:
+A lightweight gradient boosting implementation in Rust. Keywords:
 rust,forust,machine learning,xgboost,tree model,decision tree Author: James
-Inlow Requires-Python: >=3.7 Description-Content-Type: text/markdown;
+Inlow Requires-Python: >=3.8 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM
    [https://github.com/jinlow/forust/raw/main/resources/tree-image-crop.png]
  ![PyPI](https://img.shields.io/pypi/v/forust?color=gr&style=for-the-badge) !
  [Crates.io](https://img.shields.io/crates/v/forust-ml?color=gr&style=for-the-
                                     badge)
 # Forust ## _A lightweight gradient boosting package_ Forust, is a lightweight
 package for building gradient boosted decision tree ensembles. All of the
 algorithm code is written in [Rust](https://www.rust-lang.org/), with a python
 wrapper. The rust package can be used directly, however, most examples shown
-here will be for the python wrapper. It implements the same algorithm as the
-[XGBoost](https://xgboost.readthedocs.io/en/stable/) package, and in many cases
-will give nearly identical results. I developed this package for a few reasons,
-mainly to better understand the XGBoost algorithm, additionally to have a fun
-project to work on in rust, and because I wanted to be able to experiment with
-adding new features to the algorithm in a smaller simpler codebase. All of the
-rust code for the package can be found in the [src](src/) directory, while all
-of the python wrapper code is in the [py-forust](py-forust/) directory. ##
-Installation The package can be installed directly from [pypi](https://
-pypi.org/project/forust/). ```shell pip install forust ``` To use in a rust
-project add the following to your Cargo.toml file. ```toml forust-ml = "0.1.7"
-``` ## Usage The `GradientBooster` class is currently the only public facing
-class in the package, and can be used to train gradient boosted decision tree
-ensembles with multiple objective functions. It can be initialized with the
-following arguments. - `objective_type` ***(str, optional)***: The name of
-objective function used to optimize. Valid options include "LogLoss" to use
-logistic loss as the objective function (binary classification), or
-"SquaredLoss" to use Squared Error as the objective function (continuous
-regression). Defaults to "LogLoss". - `iterations` ***(int, optional)***: Total
-number of trees to train in the ensemble. Defaults to 100. - `learning_rate`
-***(float, optional)***: Step size to use at each iteration. Each leaf weight
-is multiplied by this number. The smaller the value, the more conservative the
-weights will be. Defaults to 0.3. - `max_depth` ***(int, optional)***: Maximum
-depth of an individual tree. Valid values are 0 to infinity. Defaults to 5. -
-`max_leaves` ***(int, optional)***: Maximum number of leaves allowed on a tree.
-Valid values are 0 to infinity. This is the total number of final nodes.
-Defaults to sys.maxsize. - `l2` ***(float, optional)***: L2 regularization term
-applied to the weights of the tree. Valid values are 0 to infinity. Defaults to
-1.0. - `gamma` ***(float, optional)***: The minimum amount of loss required to
-further split a node. Valid values are 0 to infinity. Defaults to 0.0. -
+here will be for the python wrapper. For a self contained rust example, [see
+here](rs-example.md). It implements the same algorithm as the [XGBoost](https:/
+/xgboost.readthedocs.io/en/stable/) package, and in many cases will give nearly
+identical results. I developed this package for a few reasons, mainly to better
+understand the XGBoost algorithm, additionally to have a fun project to work on
+in rust, and because I wanted to be able to experiment with adding new features
+to the algorithm in a smaller simpler codebase. All of the rust code for the
+package can be found in the [src](src/) directory, while all of the python
+wrapper code is in the [py-forust](py-forust/) directory. ## Installation The
+package can be installed directly from [pypi](https://pypi.org/project/forust/
+). ```shell pip install forust ``` To use in a rust project add the following
+to your Cargo.toml file. ```toml forust-ml = "0.2.0" ``` ## Usage The
+`GradientBooster` class is currently the only public facing class in the
+package, and can be used to train gradient boosted decision tree ensembles with
+multiple objective functions. It can be initialized with the following
+arguments. - `objective_type` ***(str, optional)***: The name of objective
+function used to optimize. Valid options include "LogLoss" to use logistic loss
+as the objective function (binary classification), or "SquaredLoss" to use
+Squared Error as the objective function (continuous regression). Defaults to
+"LogLoss". - `iterations` ***(int, optional)***: Total number of trees to train
+in the ensemble. Defaults to 100. - `learning_rate` ***(float, optional)***:
+Step size to use at each iteration. Each leaf weight is multiplied by this
+number. The smaller the value, the more conservative the weights will be.
+Defaults to 0.3. - `max_depth` ***(int, optional)***: Maximum depth of an
+individual tree. Valid values are 0 to infinity. Defaults to 5. - `max_leaves`
+***(int, optional)***: Maximum number of leaves allowed on a tree. Valid values
+are 0 to infinity. This is the total number of final nodes. Defaults to
+sys.maxsize. - `l2` ***(float, optional)***: L2 regularization term applied to
+the weights of the tree. Valid values are 0 to infinity. Defaults to 1.0. -
+`gamma` ***(float, optional)***: The minimum amount of loss required to further
+split a node. Valid values are 0 to infinity. Defaults to 0.0. -
 `min_leaf_weight` ***(float, optional)***: Minimum sum of the hessian values of
 the loss function required to be in a node. Defaults to 1.0. - `base_score` ***
 (float, optional)***: The initial prediction value of the model. Defaults to
 0.5. - `nbins` ***(int, optional)***: Number of bins to calculate to partition
 the data. Setting this to a smaller number, will result in faster training
 time, while potentially sacrificing accuracy. If there are more bins, than
 unique values in a column, all unique values will be used. Defaults to 256. -
 `parallel` ***(bool, optional)***: Should multiple cores be used when training
 and predicting with this model? Defaults to `True`. - `allow_missing_splits`
 ***(bool, optional)***: Allow for splits to be made such that all missing
 values go down one branch, and all non-missing values go down the other, if
 this results in the greatest reduction of loss. If this is false, splits will
-only be made on non missing values. Defaults to `True`. - `impute_missing` ***
-(bool, optional)***: Automatically impute missing values, such that at every
-split the model learns the best direction to send missing values. If this is
-false, all missing values will default to right branch. Defaults to `True`. -
+only be made on non missing values. Defaults to `True`. -
 `monotone_constraints` ***(dict[Any, int], optional)***: Constraints that are
 used to enforce a specific relationship between the training features and the
 target variable. A dictionary should be provided where the keys are the feature
 index value if the model will be fit on a numpy array, or a feature name if it
 will be fit on a pandas Dataframe. The values of the dictionary should be an
 integer value of -1, 1, or 0 to specify the relationship that should be
 estimated between the respective feature and the target variable. Use a value
@@ -122,22 +123,17 @@
 matplotlib.pyplot as plt pd_values = model.partial_dependence(X=X,
 feature="age") fig = lineplot(x=pd_values[:,0], y=pd_values[:,1],) plt.title
 ("Partial Dependence Plot") plt.xlabel("Age") plt.ylabel("Log Odds") ```
 [https://github.com/jinlow/forust/raw/main/resources/pdp_plot_age.png] We can
 see how this is impacted if a model is created, where a specific constraint is
 applied to the feature using the `monotone_constraint` parameter. ```python
 model = GradientBooster( objective_type="LogLoss", monotone_constraints={"age":
--1}, ) model.fit(X, y) pd_values = model.partial_dependence(X=X, 1) fig =
-lineplot( x=pd_values[:, 0], y=pd_values[:, 1], ) plt.title("Partial Dependence
-Plot with Monotonicity") plt.xlabel("Age") plt.ylabel("Log Odds") ``` [https://
-github.com/jinlow/forust/raw/main/resources/pdp_plot_age_mono.png] ### Saving
-the model To save and subsequently load a trained booster, the `save_booster`
-and `load_booster` methods can be used. Each accepts a path, which is used to
-write the model to. The model is saved and loaded as a json object. ```python
-trained_model.save_booster("model_path.json") # To load a model from a json
-path. loaded_model = GradientBooster.load_model("model_path.json") ``` ## TODOs
-This is still a work in progress - [ ] Early stopping rounds * We should be
-able to accept a validation dataset, and this should be able to be used to
-determine when to stop training. - [X] Monotonicity support * Right now
-features are used in the model without any constraints. - [X] Ability to save a
-model. * The way the underlying trees are structured, they would lend
-themselves to being saved as JSon objects. - [ ] Clean up the CICD pipeline.
+-1}, ) model.fit(X, y) pd_values = model.partial_dependence(X=X, feature="age")
+fig = lineplot( x=pd_values[:, 0], y=pd_values[:, 1], ) plt.title("Partial
+Dependence Plot with Monotonicity") plt.xlabel("Age") plt.ylabel("Log Odds")
+``` [https://github.com/jinlow/forust/raw/main/resources/pdp_plot_age_mono.png]
+### Saving the model To save and subsequently load a trained booster, the
+`save_booster` and `load_booster` methods can be used. Each accepts a path,
+which is used to write the model to. The model is saved and loaded as a json
+object. ```python trained_model.save_booster("model_path.json") # To load a
+model from a json path. loaded_model = GradientBooster.load_model
+("model_path.json") ```
```

