# Comparing `tmp/HLR-0.1.4.tar.gz` & `tmp/HLR-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HLR-0.1.4.tar", last modified: Thu Mar  9 04:13:30 2023, max compression
+gzip compressed data, was "HLR-0.1.5.tar", last modified: Thu Apr 20 01:45:55 2023, max compression
```

## Comparing `HLR-0.1.4.tar` & `HLR-0.1.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 tanijarv   (501) staff       (20)        0 2023-03-09 04:13:30.007574 HLR-0.1.4/
--rw-r--r--   0 tanijarv   (501) staff       (20)      175 2023-03-09 04:12:33.000000 HLR-0.1.4/AUTHORS.rst
--rw-r--r--   0 tanijarv   (501) staff       (20)     3529 2023-03-02 22:44:09.000000 HLR-0.1.4/CONTRIBUTING.rst
--rw-r--r--   0 tanijarv   (501) staff       (20)      377 2023-03-09 04:12:33.000000 HLR-0.1.4/HISTORY.rst
-drwxr-xr-x   0 tanijarv   (501) staff       (20)        0 2023-03-09 04:13:30.002694 HLR-0.1.4/HLR/
--rw-r--r--   0 tanijarv   (501) staff       (20)      428 2023-03-02 22:44:09.000000 HLR-0.1.4/HLR/__init__.py
--rw-r--r--   0 tanijarv   (501) staff       (20)      387 2023-03-02 22:44:09.000000 HLR-0.1.4/HLR/cli.py
--rw-r--r--   0 tanijarv   (501) staff       (20)    20007 2023-03-09 04:12:33.000000 HLR-0.1.4/HLR/diagnostic_tests.py
--rw-r--r--   0 tanijarv   (501) staff       (20)     9766 2023-03-09 04:12:33.000000 HLR-0.1.4/HLR/hierarchical_regression.py
--rw-r--r--   0 tanijarv   (501) staff       (20)     7865 2023-03-02 22:44:09.000000 HLR-0.1.4/HLR/model.py
-drwxr-xr-x   0 tanijarv   (501) staff       (20)        0 2023-03-09 04:13:30.003945 HLR-0.1.4/HLR.egg-info/
--rw-r--r--   0 tanijarv   (501) staff       (20)     9915 2023-03-09 04:13:29.000000 HLR-0.1.4/HLR.egg-info/PKG-INFO
--rw-r--r--   0 tanijarv   (501) staff       (20)      617 2023-03-09 04:13:29.000000 HLR-0.1.4/HLR.egg-info/SOURCES.txt
--rw-r--r--   0 tanijarv   (501) staff       (20)        1 2023-03-09 04:13:29.000000 HLR-0.1.4/HLR.egg-info/dependency_links.txt
--rw-r--r--   0 tanijarv   (501) staff       (20)       37 2023-03-09 04:13:29.000000 HLR-0.1.4/HLR.egg-info/entry_points.txt
--rw-r--r--   0 tanijarv   (501) staff       (20)        1 2023-03-02 22:49:21.000000 HLR-0.1.4/HLR.egg-info/not-zip-safe
--rw-r--r--   0 tanijarv   (501) staff       (20)       88 2023-03-09 04:13:29.000000 HLR-0.1.4/HLR.egg-info/requires.txt
--rw-r--r--   0 tanijarv   (501) staff       (20)        4 2023-03-09 04:13:29.000000 HLR-0.1.4/HLR.egg-info/top_level.txt
--rw-r--r--   0 tanijarv   (501) staff       (20)     1570 2023-03-02 22:44:09.000000 HLR-0.1.4/LICENSE
--rw-r--r--   0 tanijarv   (501) staff       (20)      320 2023-03-02 22:44:09.000000 HLR-0.1.4/MANIFEST.in
--rw-r--r--   0 tanijarv   (501) staff       (20)     9915 2023-03-09 04:13:30.007686 HLR-0.1.4/PKG-INFO
--rw-r--r--   0 tanijarv   (501) staff       (20)     8744 2023-03-09 04:12:33.000000 HLR-0.1.4/README.md
-drwxr-xr-x   0 tanijarv   (501) staff       (20)        0 2023-03-09 04:13:30.005787 HLR-0.1.4/docs/
--rw-r--r--   0 tanijarv   (501) staff       (20)      604 2023-03-02 22:44:09.000000 HLR-0.1.4/docs/Makefile
--rw-r--r--   0 tanijarv   (501) staff       (20)       28 2023-03-02 22:44:09.000000 HLR-0.1.4/docs/authors.rst
--rwxr-xr-x   0 tanijarv   (501) staff       (20)     4882 2023-03-02 22:44:09.000000 HLR-0.1.4/docs/conf.py
--rw-r--r--   0 tanijarv   (501) staff       (20)       33 2023-03-02 22:44:09.000000 HLR-0.1.4/docs/contributing.rst
--rw-r--r--   0 tanijarv   (501) staff       (20)       28 2023-03-02 22:44:09.000000 HLR-0.1.4/docs/history.rst
--rw-r--r--   0 tanijarv   (501) staff       (20)      333 2023-03-02 22:44:09.000000 HLR-0.1.4/docs/index.rst
--rw-r--r--   0 tanijarv   (501) staff       (20)     1185 2023-03-02 22:44:09.000000 HLR-0.1.4/docs/installation.rst
--rw-r--r--   0 tanijarv   (501) staff       (20)      801 2023-03-02 22:44:09.000000 HLR-0.1.4/docs/make.bat
--rw-r--r--   0 tanijarv   (501) staff       (20)       27 2023-03-02 22:44:09.000000 HLR-0.1.4/docs/readme.rst
--rw-r--r--   0 tanijarv   (501) staff       (20)      870 2023-03-02 22:44:09.000000 HLR-0.1.4/docs/usage.rst
-drwxr-xr-x   0 tanijarv   (501) staff       (20)        0 2023-03-09 04:13:30.006259 HLR-0.1.4/example/
--rw-r--r--   0 tanijarv   (501) staff       (20)    86022 2023-03-02 22:44:09.000000 HLR-0.1.4/example/NBA_train.csv
--rw-r--r--   0 tanijarv   (501) staff       (20)  1391411 2023-03-09 04:12:33.000000 HLR-0.1.4/example/usage.ipynb
--rw-r--r--   0 tanijarv   (501) staff       (20)      420 2023-03-09 04:13:30.008190 HLR-0.1.4/setup.cfg
--rw-r--r--   0 tanijarv   (501) staff       (20)     1636 2023-03-09 04:12:33.000000 HLR-0.1.4/setup.py
-drwxr-xr-x   0 tanijarv   (501) staff       (20)        0 2023-03-09 04:13:30.007362 HLR-0.1.4/tests/
--rw-r--r--   0 tanijarv   (501) staff       (20)       33 2023-03-02 22:44:09.000000 HLR-0.1.4/tests/__init__.py
--rw-r--r--   0 tanijarv   (501) staff       (20)     1034 2023-03-02 22:44:09.000000 HLR-0.1.4/tests/test_HLR.py
+drwxr-xr-x   0 tanijarv   (501) staff       (20)        0 2023-04-20 01:45:55.732714 HLR-0.1.5/
+-rw-r--r--   0 tanijarv   (501) staff       (20)      221 2023-04-05 23:56:16.000000 HLR-0.1.5/AUTHORS.rst
+-rw-r--r--   0 tanijarv   (501) staff       (20)     3529 2023-03-02 22:44:09.000000 HLR-0.1.5/CONTRIBUTING.rst
+-rw-r--r--   0 tanijarv   (501) staff       (20)      636 2023-04-11 02:22:08.000000 HLR-0.1.5/HISTORY.rst
+drwxr-xr-x   0 tanijarv   (501) staff       (20)        0 2023-04-20 01:45:55.726359 HLR-0.1.5/HLR/
+-rw-r--r--   0 tanijarv   (501) staff       (20)      428 2023-03-02 22:44:09.000000 HLR-0.1.5/HLR/__init__.py
+-rw-r--r--   0 tanijarv   (501) staff       (20)      387 2023-03-02 22:44:09.000000 HLR-0.1.5/HLR/cli.py
+-rw-r--r--   0 tanijarv   (501) staff       (20)    20621 2023-04-05 23:56:16.000000 HLR-0.1.5/HLR/diagnostic_tests.py
+-rw-r--r--   0 tanijarv   (501) staff       (20)    13646 2023-04-11 02:22:08.000000 HLR-0.1.5/HLR/hierarchical_regression.py
+-rw-r--r--   0 tanijarv   (501) staff       (20)     7865 2023-03-02 22:44:09.000000 HLR-0.1.5/HLR/model.py
+drwxr-xr-x   0 tanijarv   (501) staff       (20)        0 2023-04-20 01:45:55.727508 HLR-0.1.5/HLR.egg-info/
+-rw-r--r--   0 tanijarv   (501) staff       (20)    10286 2023-04-20 01:45:55.000000 HLR-0.1.5/HLR.egg-info/PKG-INFO
+-rw-r--r--   0 tanijarv   (501) staff       (20)      617 2023-04-20 01:45:55.000000 HLR-0.1.5/HLR.egg-info/SOURCES.txt
+-rw-r--r--   0 tanijarv   (501) staff       (20)        1 2023-04-20 01:45:55.000000 HLR-0.1.5/HLR.egg-info/dependency_links.txt
+-rw-r--r--   0 tanijarv   (501) staff       (20)       37 2023-04-20 01:45:55.000000 HLR-0.1.5/HLR.egg-info/entry_points.txt
+-rw-r--r--   0 tanijarv   (501) staff       (20)        1 2023-03-02 22:49:21.000000 HLR-0.1.5/HLR.egg-info/not-zip-safe
+-rw-r--r--   0 tanijarv   (501) staff       (20)      104 2023-04-20 01:45:55.000000 HLR-0.1.5/HLR.egg-info/requires.txt
+-rw-r--r--   0 tanijarv   (501) staff       (20)        4 2023-04-20 01:45:55.000000 HLR-0.1.5/HLR.egg-info/top_level.txt
+-rw-r--r--   0 tanijarv   (501) staff       (20)     1570 2023-03-02 22:44:09.000000 HLR-0.1.5/LICENSE
+-rw-r--r--   0 tanijarv   (501) staff       (20)      320 2023-03-02 22:44:09.000000 HLR-0.1.5/MANIFEST.in
+-rw-r--r--   0 tanijarv   (501) staff       (20)    10286 2023-04-20 01:45:55.732854 HLR-0.1.5/PKG-INFO
+-rw-r--r--   0 tanijarv   (501) staff       (20)     8856 2023-04-11 02:22:08.000000 HLR-0.1.5/README.md
+drwxr-xr-x   0 tanijarv   (501) staff       (20)        0 2023-04-20 01:45:55.729445 HLR-0.1.5/docs/
+-rw-r--r--   0 tanijarv   (501) staff       (20)      604 2023-03-02 22:44:09.000000 HLR-0.1.5/docs/Makefile
+-rw-r--r--   0 tanijarv   (501) staff       (20)       28 2023-03-02 22:44:09.000000 HLR-0.1.5/docs/authors.rst
+-rwxr-xr-x   0 tanijarv   (501) staff       (20)     4882 2023-03-02 22:44:09.000000 HLR-0.1.5/docs/conf.py
+-rw-r--r--   0 tanijarv   (501) staff       (20)       33 2023-03-02 22:44:09.000000 HLR-0.1.5/docs/contributing.rst
+-rw-r--r--   0 tanijarv   (501) staff       (20)       28 2023-03-02 22:44:09.000000 HLR-0.1.5/docs/history.rst
+-rw-r--r--   0 tanijarv   (501) staff       (20)      333 2023-03-02 22:44:09.000000 HLR-0.1.5/docs/index.rst
+-rw-r--r--   0 tanijarv   (501) staff       (20)     1185 2023-03-02 22:44:09.000000 HLR-0.1.5/docs/installation.rst
+-rw-r--r--   0 tanijarv   (501) staff       (20)      801 2023-03-02 22:44:09.000000 HLR-0.1.5/docs/make.bat
+-rw-r--r--   0 tanijarv   (501) staff       (20)       27 2023-03-02 22:44:09.000000 HLR-0.1.5/docs/readme.rst
+-rw-r--r--   0 tanijarv   (501) staff       (20)      870 2023-03-02 22:44:09.000000 HLR-0.1.5/docs/usage.rst
+drwxr-xr-x   0 tanijarv   (501) staff       (20)        0 2023-04-20 01:45:55.730042 HLR-0.1.5/example/
+-rw-r--r--   0 tanijarv   (501) staff       (20)    86022 2023-03-02 22:44:09.000000 HLR-0.1.5/example/NBA_train.csv
+-rw-r--r--   0 tanijarv   (501) staff       (20)  1391411 2023-03-09 04:12:33.000000 HLR-0.1.5/example/usage.ipynb
+-rw-r--r--   0 tanijarv   (501) staff       (20)      420 2023-04-20 01:45:55.733463 HLR-0.1.5/setup.cfg
+-rw-r--r--   0 tanijarv   (501) staff       (20)     1671 2023-04-11 02:22:08.000000 HLR-0.1.5/setup.py
+drwxr-xr-x   0 tanijarv   (501) staff       (20)        0 2023-04-20 01:45:55.732487 HLR-0.1.5/tests/
+-rw-r--r--   0 tanijarv   (501) staff       (20)       33 2023-03-02 22:44:09.000000 HLR-0.1.5/tests/__init__.py
+-rw-r--r--   0 tanijarv   (501) staff       (20)     1034 2023-03-02 22:44:09.000000 HLR-0.1.5/tests/test_HLR.py
```

### Comparing `HLR-0.1.4/CONTRIBUTING.rst` & `HLR-0.1.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `HLR-0.1.4/HLR/diagnostic_tests.py` & `HLR-0.1.5/HLR/diagnostic_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
     ###### ASSUMPTION I - INDEPENDENCE OF RESIDUALS
 
     ### (1) Durbin-Watson stat (no autocorrelation)
 
     # Calculate the Durbin-Watson statistic
     diagnostics['durbin_watson_stat'] = sm_stats.stattools.durbin_watson(
-            model.resid, axis=0)
+           model.resid, axis=0)
     # If the statistic is between 1.5-2.5, the test is passed
     if diagnostics['durbin_watson_stat'] >= 1.5 and diagnostics[
             'durbin_watson_stat'] <= 2.5:
         diagnostics['durbin_watson_passed'] = 'Yes'
     else:
         diagnostics['durbin_watson_passed'] = 'No'
     # Link test to assumption
@@ -369,67 +369,81 @@
 
     # Save a CSV of pairwise correlations (only if there are multiple predictors)
     if len(X.columns) > 1:
         pairwiseCorrName = saveto + '/' + step + '_pairwise_correlations.csv'
         high_pairwise_corr.to_csv(pairwiseCorrName)
 
     ###### MAKE AND SAVE PLOTS
-
-    sns.set_theme(style="whitegrid")
-    fig, axs = plt.subplots(nrows=2, ncols=2, figsize=(15, 15))
-    suptitle = fig.suptitle('Diagnostic Plots for {} - {}'.format(step, X_names), y=0.92)
+    #29/03/2023 - 2 x 2 figure subplot removed and figures now saved individually
 
     ### PLOT 1 - STUDENTISED RESIDUALS VS FITTED VALUES 
     # Used to inspect linearity and homoscedasticity
     # Get values for the plot 1
     student_resid = influence_df['student_resid']
     fitted_vals = model.fittedvalues
     df_residfitted = pd.concat([student_resid, fitted_vals], axis=1)
     df_residfitted = df_residfitted.set_axis(['student_resid', 'fitted_vals'],
                                              axis=1)
     # Plot with a LOWESS (Locally Weighted Scatterplot Smoothing) line 
     # A relativelty straight LOWESS line indicates a linear model is reasonable
-    sns.residplot(ax=axs[0][0], data=df_residfitted,
+    fig, ax = plt.subplots()
+    sns.residplot(ax=ax, data=df_residfitted,
             x='fitted_vals', y='student_resid', lowess=True,
             scatter_kws={'alpha': 0.8},
             line_kws={'color': 'red', 'lw': 1, 'alpha': 1})
-    axs[0][0].set(ylim=(-3.5, 3.5))
-    axs[0][0].set_title('Residuals vs Fitted')
-    axs[0][0].set_xlabel('Fitted values')
-    axs[0][0].set_ylabel('Studentised Residuals')
+    ax.set(ylim=(-3.5, 3.5))
+    ax.set_title('Residuals vs Fitted')
+    ax.set_xlabel('Fitted values')
+    ax.set_ylabel('Studentised Residuals')
+
+    figName = saveto + '/' + step + '_studresid_plots.png'
+    plt.savefig(figName, dpi=300, bbox_inches="tight")
 
     ### PLOT 2 - NORMAL QQ PLOT OF RESIDUALS
     # Used to inspect normality
-    sm.qqplot(ax=axs[0][1], data=model.resid, fit=True, line='45')
-    axs[0][1].set_title('Normal QQ Plot of Residuals')
+    fig, ax = plt.subplots()
+    sm.qqplot(ax=ax, data=model.resid, fit=True, line='45')
+    ax.set_title('Normal QQ Plot of Residuals')
+    figName = saveto + '/' + step + '_QQ_plots.png'
+    plt.savefig(figName, dpi=300, bbox_inches="tight")
 
     ### PLOT 3 - INFLUENCE PLOT WITH COOK'S DISTANCE
     # Used to inspect influence
-    sm.graphics.influence_plot(model, ax=axs[1][0], criterion="cooks")
-    axs[1][0].set_title('Influence plot')
-    axs[1][0].set_xlabel('H leverage')
-    axs[1][0].set_ylabel('Studentised Residuals')
+    fig, ax = plt.subplots()
+    sm.graphics.influence_plot(model, ax=ax, criterion="cooks")
+    ax.set_title('Influence plot')
+    ax.set_xlabel('H leverage')
+    ax.set_ylabel('Studentised Residuals')
+    figName = saveto + '/' + step + '_influence_plots.png'
+    plt.savefig(figName, dpi=300, bbox_inches="tight")
 
     ### PLOT 4 - BOX PLOT OF STANDARDISED RESIDUALS
     # Used to inspect outliers (residuals)
-    outlier_fig = sns.boxplot(ax=axs[1][1], y=influence_df['standard_resid'])
-    outlier_fig = sns.swarmplot(ax=axs[1][1], y=influence_df['standard_resid'], color="red")
-    outlier_fig.axes.set(ylim=(-3.5, 3.5))
-    outlier_fig.axes.set_title('Boxplot of Standardised Residuals')
+    fig, ax = plt.subplots()
+    outlier_fig = sns.boxplot(ax=ax, y=influence_df['standard_resid'])
+    outlier_fig = sns.swarmplot(ax=ax, y=influence_df['standard_resid'], color="red")
+    outlier_fig.axes.set(title = 'Boxplot of  Standardised Residuals', ylabel='Standardized Residuals', ylim=(-3.5, 3.5))
     residBoxplot = outlier_fig.get_figure()  # get figure to save
-    
-    ### SAVE ALL THE PLOTS ABOVE AS A SUBPLOT
-    figName = saveto + '/' + step + '_diagnostictests_plots.png'
-    plt.savefig(figName, dpi=300, bbox_extra_artists=(suptitle,), bbox_inches="tight")
+    figName = saveto + '/' + step + '_box_plots.png'
+    plt.savefig(figName, dpi=300, bbox_inches="tight")
+    plt.show()  
+
+    ### PLOT 5 - HISTOGRAM OF STANDARDISED RESIDUAL
+    plot = sns.histplot(data=influence_df, x='standard_resid', kde=True, bins=16) # you may select the no. of bins
+    plot.set(title = 'Histogram of Standardised Residuals', xlabel='Standardized Residuals', ylabel='Frequency', xlim=(-3.5, 3.5))
+
+    figName = saveto + '/' + step + '_histogram_plots.png'
+    plt.savefig(figName, dpi=300, bbox_inches="tight")
+
     if showfig==True:
         plt.show()
     else:
         plt.close()
-
-    ### PLOT 5 - PARTIAL REGRESSION PLOTS
+    
+    ### PLOT 6 - PARTIAL REGRESSION PLOTS
     # Used to inspect linearity
     if len(X.columns) == 1:
         fig_partRegress = plt.figure(figsize=(15, 5))
     elif len(X.columns) <= 3:
         fig_partRegress = plt.figure(figsize=(15, 10))
     elif len(X.columns) <= 5:
         fig_partRegress = plt.figure(figsize=(15, 15))
@@ -446,8 +460,8 @@
         plt.show()
     else:
         plt.close()
 
     # Return list of assumptions that require further inspection (i.e. failed
     # at least 1 diagnostic test)
     assumptionsToCheck = list(set(violated))
-    return assumptionsToCheck
+    return assumptionsToCheck
```

### Comparing `HLR-0.1.4/HLR/model.py` & `HLR-0.1.5/HLR/model.py`

 * *Files identical despite different names*

### Comparing `HLR-0.1.4/HLR.egg-info/PKG-INFO` & `HLR-0.1.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,10 @@
-Metadata-Version: 2.1
-Name: HLR
-Version: 0.1.4
-Summary: HLR - Hierarchical Linear Regression for Python
-Home-page: https://github.com/teanijarv/HLR
-Author: Toomas Erik Anijärv
-Author-email: toomaserikanijarv@gmail.com
-License: GNU General Public License v3
-Keywords: HLR
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS.rst
-
 # HLR - Hierarchical Linear Regression in Python
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7683809.svg)](https://doi.org/10.5281/zenodo.7683809) [![image](https://img.shields.io/pypi/v/HLR.svg)](https://pypi.python.org/pypi/HLR) [![image](https://img.shields.io/travis/teanijarv/HLR.svg)](https://travis-ci.com/teanijarv/HLR) [![Documentation Status](https://readthedocs.org/projects/hlr-hierarchical-linear-regression/badge/?version=latest)](https://hlr-hierarchical-linear-regression.readthedocs.io/en/latest/?version=latest)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7683809.svg)](https://doi.org/10.5281/zenodo.7683809) [![image](https://img.shields.io/pypi/v/HLR.svg)](https://pypi.python.org/pypi/HLR) [![Build Status](https://app.travis-ci.com/teanijarv/HLR.svg?branch=main)](https://app.travis-ci.com/teanijarv/HLR) [![Documentation Status](https://readthedocs.org/projects/hlr-hierarchical-linear-regression/badge/?version=latest)](https://hlr-hierarchical-linear-regression.readthedocs.io/en/latest/?version=latest)
 
 HLR is a simple Python package for running hierarchical regression. It was created because there wasn't any good options to run hierarchical regression without using programs like SPSS.
 
 ## Features
 It is built to work with Pandas dataframes, uses SciPy and statsmodels for all statistics and regression functions, and runs diagnostic tests for testing assumptions while plotting figures with matplotlib and seaborn.
 - Easy model creation and initiation with input data as Pandas dataframes
 - Diagnostic tests and plots for checking assumptions:
@@ -59,14 +37,15 @@
 HLR is meant to be used with Python 3.x and has been tested on Python 3.7-3.9.
 
 #### Dependencies
 - [NumPy](https://numpy.org/)
 - [SciPy](https://www.scipy.org/)
 - [Pandas](https://pandas.pydata.org/)
 - [statsmodels](https://www.statsmodels.org/)
+- [pingouin](https://pingouin-stats.org/)
 - [matplotlib](https://matplotlib.org/)
 - [seaborn](https://seaborn.pydata.org/)
 
 #### User installation
 To install HLR, run this command in your terminal:
 
 `pip install hlr`
@@ -176,28 +155,11 @@
 Would be great if someone with more experience with packages would contribute with testing and the whole deployment process. Also, if someone would want to write documentation, that would be amazing.
 - Documentation
 - More thorough testing
 
 #### Contributors
 [Toomas Erik Anijärv](https://github.com/teanijarv)
 [Rory Boyle](https://github.com/rorytboyle)
+[Jules Mitchell](https://github.com/JulesMitchell)
 
 #### Credits
 This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage) project template.
-
-
-=======
-History
-=======
-
-0.1.0 (2023-02-24)
-------------------
-
-* First release on PyPI.
-
-0.1.4 (2023-03-9)
-------------------
-
-* Fixed pairwise correlations threshold for multicollinearity assumption testing (0.3 -> 0.7)
-* Fixed partial regression plots fixed figure size
-* Added titles to diagnostic plots
-* Fixed the VIF to match with SPSS output by adding the constant to X
```

### Comparing `HLR-0.1.4/HLR.egg-info/SOURCES.txt` & `HLR-0.1.5/HLR.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HLR-0.1.4/LICENSE` & `HLR-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `HLR-0.1.4/PKG-INFO` & `HLR-0.1.5/HLR.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HLR
-Version: 0.1.4
+Version: 0.1.5
 Summary: HLR - Hierarchical Linear Regression for Python
 Home-page: https://github.com/teanijarv/HLR
 Author: Toomas Erik Anijärv
 Author-email: toomaserikanijarv@gmail.com
 License: GNU General Public License v3
 Keywords: HLR
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -18,15 +18,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 # HLR - Hierarchical Linear Regression in Python
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7683809.svg)](https://doi.org/10.5281/zenodo.7683809) [![image](https://img.shields.io/pypi/v/HLR.svg)](https://pypi.python.org/pypi/HLR) [![image](https://img.shields.io/travis/teanijarv/HLR.svg)](https://travis-ci.com/teanijarv/HLR) [![Documentation Status](https://readthedocs.org/projects/hlr-hierarchical-linear-regression/badge/?version=latest)](https://hlr-hierarchical-linear-regression.readthedocs.io/en/latest/?version=latest)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7683809.svg)](https://doi.org/10.5281/zenodo.7683809) [![image](https://img.shields.io/pypi/v/HLR.svg)](https://pypi.python.org/pypi/HLR) [![Build Status](https://app.travis-ci.com/teanijarv/HLR.svg?branch=main)](https://app.travis-ci.com/teanijarv/HLR) [![Documentation Status](https://readthedocs.org/projects/hlr-hierarchical-linear-regression/badge/?version=latest)](https://hlr-hierarchical-linear-regression.readthedocs.io/en/latest/?version=latest)
 
 HLR is a simple Python package for running hierarchical regression. It was created because there wasn't any good options to run hierarchical regression without using programs like SPSS.
 
 ## Features
 It is built to work with Pandas dataframes, uses SciPy and statsmodels for all statistics and regression functions, and runs diagnostic tests for testing assumptions while plotting figures with matplotlib and seaborn.
 - Easy model creation and initiation with input data as Pandas dataframes
 - Diagnostic tests and plots for checking assumptions:
@@ -59,14 +59,15 @@
 HLR is meant to be used with Python 3.x and has been tested on Python 3.7-3.9.
 
 #### Dependencies
 - [NumPy](https://numpy.org/)
 - [SciPy](https://www.scipy.org/)
 - [Pandas](https://pandas.pydata.org/)
 - [statsmodels](https://www.statsmodels.org/)
+- [pingouin](https://pingouin-stats.org/)
 - [matplotlib](https://matplotlib.org/)
 - [seaborn](https://seaborn.pydata.org/)
 
 #### User installation
 To install HLR, run this command in your terminal:
 
 `pip install hlr`
@@ -176,14 +177,15 @@
 Would be great if someone with more experience with packages would contribute with testing and the whole deployment process. Also, if someone would want to write documentation, that would be amazing.
 - Documentation
 - More thorough testing
 
 #### Contributors
 [Toomas Erik Anijärv](https://github.com/teanijarv)
 [Rory Boyle](https://github.com/rorytboyle)
+[Jules Mitchell](https://github.com/JulesMitchell)
 
 #### Credits
 This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage) project template.
 
 
 =======
 History
@@ -197,7 +199,15 @@
 0.1.4 (2023-03-9)
 ------------------
 
 * Fixed pairwise correlations threshold for multicollinearity assumption testing (0.3 -> 0.7)
 * Fixed partial regression plots fixed figure size
 * Added titles to diagnostic plots
 * Fixed the VIF to match with SPSS output by adding the constant to X
+
+0.1.5 (2023-04-6)
+------------------
+
+* Added standardised beta coefficients to model output
+* Added partial and semi-partial correlations (unique variance) to model output
+* Fixed F-change degrees of freedom calculation
+* Fixed F-change p-value calculation
```

### Comparing `HLR-0.1.4/README.md` & `HLR-0.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,32 @@
+Metadata-Version: 2.1
+Name: HLR
+Version: 0.1.5
+Summary: HLR - Hierarchical Linear Regression for Python
+Home-page: https://github.com/teanijarv/HLR
+Author: Toomas Erik Anijärv
+Author-email: toomaserikanijarv@gmail.com
+License: GNU General Public License v3
+Keywords: HLR
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.rst
+
 # HLR - Hierarchical Linear Regression in Python
 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7683809.svg)](https://doi.org/10.5281/zenodo.7683809) [![image](https://img.shields.io/pypi/v/HLR.svg)](https://pypi.python.org/pypi/HLR) [![image](https://img.shields.io/travis/teanijarv/HLR.svg)](https://travis-ci.com/teanijarv/HLR) [![Documentation Status](https://readthedocs.org/projects/hlr-hierarchical-linear-regression/badge/?version=latest)](https://hlr-hierarchical-linear-regression.readthedocs.io/en/latest/?version=latest)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7683809.svg)](https://doi.org/10.5281/zenodo.7683809) [![image](https://img.shields.io/pypi/v/HLR.svg)](https://pypi.python.org/pypi/HLR) [![Build Status](https://app.travis-ci.com/teanijarv/HLR.svg?branch=main)](https://app.travis-ci.com/teanijarv/HLR) [![Documentation Status](https://readthedocs.org/projects/hlr-hierarchical-linear-regression/badge/?version=latest)](https://hlr-hierarchical-linear-regression.readthedocs.io/en/latest/?version=latest)
 
 HLR is a simple Python package for running hierarchical regression. It was created because there wasn't any good options to run hierarchical regression without using programs like SPSS.
 
 ## Features
 It is built to work with Pandas dataframes, uses SciPy and statsmodels for all statistics and regression functions, and runs diagnostic tests for testing assumptions while plotting figures with matplotlib and seaborn.
 - Easy model creation and initiation with input data as Pandas dataframes
 - Diagnostic tests and plots for checking assumptions:
@@ -37,14 +59,15 @@
 HLR is meant to be used with Python 3.x and has been tested on Python 3.7-3.9.
 
 #### Dependencies
 - [NumPy](https://numpy.org/)
 - [SciPy](https://www.scipy.org/)
 - [Pandas](https://pandas.pydata.org/)
 - [statsmodels](https://www.statsmodels.org/)
+- [pingouin](https://pingouin-stats.org/)
 - [matplotlib](https://matplotlib.org/)
 - [seaborn](https://seaborn.pydata.org/)
 
 #### User installation
 To install HLR, run this command in your terminal:
 
 `pip install hlr`
@@ -154,10 +177,37 @@
 Would be great if someone with more experience with packages would contribute with testing and the whole deployment process. Also, if someone would want to write documentation, that would be amazing.
 - Documentation
 - More thorough testing
 
 #### Contributors
 [Toomas Erik Anijärv](https://github.com/teanijarv)
 [Rory Boyle](https://github.com/rorytboyle)
+[Jules Mitchell](https://github.com/JulesMitchell)
 
 #### Credits
 This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage) project template.
+
+
+=======
+History
+=======
+
+0.1.0 (2023-02-24)
+------------------
+
+* First release on PyPI.
+
+0.1.4 (2023-03-9)
+------------------
+
+* Fixed pairwise correlations threshold for multicollinearity assumption testing (0.3 -> 0.7)
+* Fixed partial regression plots fixed figure size
+* Added titles to diagnostic plots
+* Fixed the VIF to match with SPSS output by adding the constant to X
+
+0.1.5 (2023-04-6)
+------------------
+
+* Added standardised beta coefficients to model output
+* Added partial and semi-partial correlations (unique variance) to model output
+* Fixed F-change degrees of freedom calculation
+* Fixed F-change p-value calculation
```

### Comparing `HLR-0.1.4/docs/Makefile` & `HLR-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `HLR-0.1.4/docs/conf.py` & `HLR-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `HLR-0.1.4/docs/installation.rst` & `HLR-0.1.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `HLR-0.1.4/docs/make.bat` & `HLR-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `HLR-0.1.4/docs/usage.rst` & `HLR-0.1.5/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `HLR-0.1.4/example/NBA_train.csv` & `HLR-0.1.5/example/NBA_train.csv`

 * *Files identical despite different names*

### Comparing `HLR-0.1.4/example/usage.ipynb` & `HLR-0.1.5/example/usage.ipynb`

 * *Files identical despite different names*

### Comparing `HLR-0.1.4/setup.py` & `HLR-0.1.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,16 @@
     history = history_file.read()
 
 requirements = ['Click>=7.0',
                 'scipy>=1.7.3',
                 'pandas>=1.3.5',
                 'matplotlib>=3.5.2',
                 'seaborn>=0.11',
-                'statsmodels>=0.13']
+                'statsmodels>=0.13',
+                'pingouin>=0.5.3']
 
 test_requirements = ['pytest>=3']
 
 setup(
     author="Toomas Erik Anijärv",
     author_email='toomaserikanijarv@gmail.com',
     python_requires='>=3.7',
@@ -46,10 +47,10 @@
     include_package_data=True,
     keywords='HLR',
     name='HLR',
     packages=find_packages(include=['HLR', 'HLR.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/teanijarv/HLR',
-    version='0.1.4',
+    version='0.1.5',
     zip_safe=False,
 )
```

### Comparing `HLR-0.1.4/tests/test_HLR.py` & `HLR-0.1.5/tests/test_HLR.py`

 * *Files identical despite different names*

