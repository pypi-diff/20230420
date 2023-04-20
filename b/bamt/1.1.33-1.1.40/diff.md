# Comparing `tmp/BAMT-1.1.33.tar.gz` & `tmp/BAMT-1.1.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BAMT-1.1.33.tar", max compression
+gzip compressed data, was "BAMT-1.1.40.tar", max compression
```

## Comparing `BAMT-1.1.33.tar` & `BAMT-1.1.40.tar`

### file list

```diff
@@ -1,189 +1,162 @@
--rw-r--r--   0        0        0        0 2022-10-18 09:46:52.969462 BAMT-1.1.33/bamt/__init__.py
--rw-r--r--   0        0        0    14711 2023-03-22 10:19:54.123390 BAMT-1.1.33/bamt/builders.py
--rw-r--r--   0        0        0      795 2023-03-17 12:29:52.730830 BAMT-1.1.33/bamt/config.py
--rw-r--r--   0        0        0        0 2022-07-18 14:22:44.582873 BAMT-1.1.33/bamt/external/__init__.py
--rw-r--r--   0        0        0      232 2022-07-18 14:22:44.582873 BAMT-1.1.33/bamt/external/libpgm/__init__.py
--rw-r--r--   0        0        0     3856 2022-07-18 14:22:44.583870 BAMT-1.1.33/bamt/external/libpgm/crazy.py
--rw-r--r--   0        0        0     4129 2022-07-18 14:22:44.583870 BAMT-1.1.33/bamt/external/libpgm/dictionary.py
--rw-r--r--   0        0        0     4731 2022-07-18 14:22:44.583870 BAMT-1.1.33/bamt/external/libpgm/discrete.py
--rw-r--r--   0        0        0    11303 2022-07-18 14:22:44.583870 BAMT-1.1.33/bamt/external/libpgm/discretebayesiannetwork.py
--rw-r--r--   0        0        0     9680 2022-07-18 14:22:44.584867 BAMT-1.1.33/bamt/external/libpgm/dyndiscbayesiannetwork.py
--rw-r--r--   0        0        0     6035 2022-07-18 14:22:44.584867 BAMT-1.1.33/bamt/external/libpgm/graphskeleton.py
--rw-r--r--   0        0        0     8107 2022-07-18 14:22:44.584867 BAMT-1.1.33/bamt/external/libpgm/hybayesiannetwork.py
--rw-r--r--   0        0        0    11987 2022-07-18 14:22:44.584867 BAMT-1.1.33/bamt/external/libpgm/lg.py
--rw-r--r--   0        0        0    13081 2022-07-18 14:22:44.585863 BAMT-1.1.33/bamt/external/libpgm/lgandd.py
--rw-r--r--   0        0        0     8886 2022-07-18 14:22:44.585863 BAMT-1.1.33/bamt/external/libpgm/lgbayesiannetwork.py
--rw-r--r--   0        0        0     5129 2022-07-18 14:22:44.585863 BAMT-1.1.33/bamt/external/libpgm/logit.py
--rw-r--r--   0        0        0     6096 2022-07-18 14:22:44.585863 BAMT-1.1.33/bamt/external/libpgm/logitandd.py
--rw-r--r--   0        0        0     7208 2022-07-18 14:22:44.586860 BAMT-1.1.33/bamt/external/libpgm/nodedata.py
--rw-r--r--   0        0        0     2633 2022-07-18 14:22:44.586860 BAMT-1.1.33/bamt/external/libpgm/orderedskeleton.py
--rw-r--r--   0        0        0    46978 2022-07-18 14:22:44.586860 BAMT-1.1.33/bamt/external/libpgm/pgmlearner.py
--rw-r--r--   0        0        0     4947 2022-07-18 14:22:44.587857 BAMT-1.1.33/bamt/external/libpgm/sampleaggregator.py
--rw-r--r--   0        0        0    12100 2022-07-18 14:22:44.587857 BAMT-1.1.33/bamt/external/libpgm/tablecpdfactor.py
--rw-r--r--   0        0        0    19760 2022-07-18 14:22:44.587857 BAMT-1.1.33/bamt/external/libpgm/tablecpdfactorization.py
--rw-r--r--   0        0        0      292 2022-07-18 14:22:44.587857 BAMT-1.1.33/bamt/external/pyBN/__init__.py
--rw-r--r--   0        0        0      186 2022-07-18 14:22:44.588854 BAMT-1.1.33/bamt/external/pyBN/classes/__init__.py
--rw-r--r--   0        0        0        0 2022-07-18 14:22:44.588854 BAMT-1.1.33/bamt/external/pyBN/classes/_tests/__init__.py
--rw-r--r--   0        0        0      174 2022-12-24 09:53:41.854845 BAMT-1.1.33/bamt/external/pyBN/classes/_tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5230 2022-12-24 09:53:41.861558 BAMT-1.1.33/bamt/external/pyBN/classes/_tests/__pycache__/test_bayesnet.cpython-310.pyc
--rw-r--r--   0        0        0     6379 2022-12-24 09:53:41.867553 BAMT-1.1.33/bamt/external/pyBN/classes/_tests/__pycache__/test_factor.cpython-310.pyc
--rw-r--r--   0        0        0     4162 2022-07-18 14:22:44.588854 BAMT-1.1.33/bamt/external/pyBN/classes/_tests/test_bayesnet.py
--rw-r--r--   0        0        0     4451 2022-07-18 14:22:44.588854 BAMT-1.1.33/bamt/external/pyBN/classes/_tests/test_factor.py
--rw-r--r--   0        0        0    10932 2022-07-18 14:22:44.589850 BAMT-1.1.33/bamt/external/pyBN/classes/bayesnet.py
--rw-r--r--   0        0        0    11827 2022-07-18 14:22:44.589850 BAMT-1.1.33/bamt/external/pyBN/classes/cliquetree.py
--rw-r--r--   0        0        0     5847 2022-07-18 14:22:44.589850 BAMT-1.1.33/bamt/external/pyBN/classes/clustergraph.py
--rw-r--r--   0        0        0     5341 2022-07-18 14:22:44.590847 BAMT-1.1.33/bamt/external/pyBN/classes/empiricaldistribution.py
--rw-r--r--   0        0        0    18529 2022-07-18 14:22:44.590847 BAMT-1.1.33/bamt/external/pyBN/classes/factor.py
--rw-r--r--   0        0        0     3747 2022-07-18 14:22:44.590847 BAMT-1.1.33/bamt/external/pyBN/classes/factorization.py
--rw-r--r--   0        0        0      129 2022-07-18 14:22:44.590847 BAMT-1.1.33/bamt/external/pyBN/classification/__init__.py
--rw-r--r--   0        0        0     3227 2022-07-18 14:22:44.591843 BAMT-1.1.33/bamt/external/pyBN/classification/classification.py
--rw-r--r--   0        0        0     3329 2022-07-18 14:22:44.591843 BAMT-1.1.33/bamt/external/pyBN/classification/feature_selection.py
--rw-r--r--   0        0        0      171 2022-07-18 14:22:44.591843 BAMT-1.1.33/bamt/external/pyBN/inference/__init__.py
--rw-r--r--   0        0        0        0 2022-07-18 14:22:44.591843 BAMT-1.1.33/bamt/external/pyBN/inference/_tests/__init__.py
--rw-r--r--   0        0        0      176 2022-12-24 09:53:41.870556 BAMT-1.1.33/bamt/external/pyBN/inference/_tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1060 2022-12-24 09:53:41.876256 BAMT-1.1.33/bamt/external/pyBN/inference/_tests/__pycache__/test_map_exact.cpython-310.pyc
--rw-r--r--   0        0        0     2776 2022-12-24 09:53:41.882205 BAMT-1.1.33/bamt/external/pyBN/inference/_tests/__pycache__/test_marginal_approx.cpython-310.pyc
--rw-r--r--   0        0        0     2251 2022-12-24 09:53:41.886925 BAMT-1.1.33/bamt/external/pyBN/inference/_tests/__pycache__/test_marginal_exact.cpython-310.pyc
--rw-r--r--   0        0        0      915 2022-07-18 14:22:44.592840 BAMT-1.1.33/bamt/external/pyBN/inference/_tests/test_map_exact.py
--rw-r--r--   0        0        0     2170 2022-07-18 14:22:44.592840 BAMT-1.1.33/bamt/external/pyBN/inference/_tests/test_marginal_approx.py
--rw-r--r--   0        0        0     2340 2022-07-18 14:22:44.592840 BAMT-1.1.33/bamt/external/pyBN/inference/_tests/test_marginal_exact.py
--rw-r--r--   0        0        0      121 2022-07-18 14:22:44.593837 BAMT-1.1.33/bamt/external/pyBN/inference/map_exact/__init__.py
--rw-r--r--   0        0        0      299 2022-07-18 14:38:07.206669 BAMT-1.1.33/bamt/external/pyBN/inference/map_exact/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2653 2022-07-18 14:38:07.207666 BAMT-1.1.33/bamt/external/pyBN/inference/map_exact/__pycache__/ilp_map.cpython-310.pyc
--rw-r--r--   0        0        0     1077 2022-07-18 14:38:07.208663 BAMT-1.1.33/bamt/external/pyBN/inference/map_exact/__pycache__/ve_map.cpython-310.pyc
--rw-r--r--   0        0        0     3333 2022-07-18 14:22:44.593837 BAMT-1.1.33/bamt/external/pyBN/inference/map_exact/ilp_map.py
--rw-r--r--   0        0        0     1342 2022-07-18 14:22:44.593837 BAMT-1.1.33/bamt/external/pyBN/inference/map_exact/ve_map.py
--rw-r--r--   0        0        0      285 2022-07-18 14:22:44.594833 BAMT-1.1.33/bamt/external/pyBN/inference/marginal_approx/__init__.py
--rw-r--r--   0        0        0      461 2022-07-18 14:38:07.209659 BAMT-1.1.33/bamt/external/pyBN/inference/marginal_approx/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2050 2022-07-18 14:38:07.210656 BAMT-1.1.33/bamt/external/pyBN/inference/marginal_approx/__pycache__/forward_sample.cpython-310.pyc
--rw-r--r--   0        0        0     1553 2022-07-18 14:38:07.213646 BAMT-1.1.33/bamt/external/pyBN/inference/marginal_approx/__pycache__/gibbs_sample.cpython-310.pyc
--rw-r--r--   0        0        0     1783 2022-07-18 14:38:07.214643 BAMT-1.1.33/bamt/external/pyBN/inference/marginal_approx/__pycache__/loopy_bp.cpython-310.pyc
--rw-r--r--   0        0        0     1613 2022-07-18 14:38:07.215639 BAMT-1.1.33/bamt/external/pyBN/inference/marginal_approx/__pycache__/lw_sample.cpython-310.pyc
--rw-r--r--   0        0        0     2067 2022-07-18 14:22:44.594833 BAMT-1.1.33/bamt/external/pyBN/inference/marginal_approx/forward_sample.py
--rw-r--r--   0        0        0     1963 2022-07-18 14:22:44.594833 BAMT-1.1.33/bamt/external/pyBN/inference/marginal_approx/gibbs_sample.py
--rw-r--r--   0        0        0     1861 2022-07-18 14:22:44.595830 BAMT-1.1.33/bamt/external/pyBN/inference/marginal_approx/loopy_bp.py
--rw-r--r--   0        0        0     2216 2022-07-18 14:22:44.595830 BAMT-1.1.33/bamt/external/pyBN/inference/marginal_approx/lw_sample.py
--rw-r--r--   0        0        0      137 2022-07-18 14:22:44.595830 BAMT-1.1.33/bamt/external/pyBN/inference/marginal_exact/__init__.py
--rw-r--r--   0        0        0      320 2022-07-18 14:38:07.216636 BAMT-1.1.33/bamt/external/pyBN/inference/marginal_exact/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2054 2022-07-18 14:38:07.217632 BAMT-1.1.33/bamt/external/pyBN/inference/marginal_exact/__pycache__/exact_bp.cpython-310.pyc
--rw-r--r--   0        0        0     1432 2022-07-18 14:38:07.218629 BAMT-1.1.33/bamt/external/pyBN/inference/marginal_exact/__pycache__/ve_marginal.cpython-310.pyc
--rw-r--r--   0        0        0     2813 2022-07-18 14:22:44.607908 BAMT-1.1.33/bamt/external/pyBN/inference/marginal_exact/exact_bp.py
--rw-r--r--   0        0        0     1307 2022-07-18 14:22:44.611364 BAMT-1.1.33/bamt/external/pyBN/inference/marginal_exact/ve_marginal.py
--rw-r--r--   0        0        0       83 2022-07-18 14:22:44.612080 BAMT-1.1.33/bamt/external/pyBN/io/__init__.py
--rw-r--r--   0        0        0        0 2022-07-18 14:22:44.619060 BAMT-1.1.33/bamt/external/pyBN/io/_tests/__init__.py
--rw-r--r--   0        0        0      169 2022-12-24 09:53:41.889932 BAMT-1.1.33/bamt/external/pyBN/io/_tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1451 2022-12-24 09:53:41.894772 BAMT-1.1.33/bamt/external/pyBN/io/_tests/__pycache__/test_reading.cpython-310.pyc
--rw-r--r--   0        0        0      888 2022-12-24 09:53:41.899461 BAMT-1.1.33/bamt/external/pyBN/io/_tests/__pycache__/test_writing.cpython-310.pyc
--rw-r--r--   0        0        0      791 2022-07-18 14:22:44.639075 BAMT-1.1.33/bamt/external/pyBN/io/_tests/test_reading.py
--rw-r--r--   0        0        0      341 2022-07-18 14:22:44.640134 BAMT-1.1.33/bamt/external/pyBN/io/_tests/test_writing.py
--rw-r--r--   0        0        0     6379 2022-07-18 14:22:44.640134 BAMT-1.1.33/bamt/external/pyBN/io/read.py
--rw-r--r--   0        0        0     1442 2022-07-18 14:22:44.641075 BAMT-1.1.33/bamt/external/pyBN/io/write.py
--rw-r--r--   0        0        0      104 2022-07-18 14:22:44.641075 BAMT-1.1.33/bamt/external/pyBN/learning/__init__.py
--rw-r--r--   0        0        0      114 2022-07-18 14:22:44.645468 BAMT-1.1.33/bamt/external/pyBN/learning/parameter/__init__.py
--rw-r--r--   0        0        0      291 2022-07-18 14:38:07.221620 BAMT-1.1.33/bamt/external/pyBN/learning/parameter/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3832 2022-07-18 14:38:07.222616 BAMT-1.1.33/bamt/external/pyBN/learning/parameter/__pycache__/bayes.cpython-310.pyc
--rw-r--r--   0        0        0     5978 2022-07-18 14:38:07.223613 BAMT-1.1.33/bamt/external/pyBN/learning/parameter/__pycache__/mle.cpython-310.pyc
--rw-r--r--   0        0        0        0 2022-07-18 14:22:44.667314 BAMT-1.1.33/bamt/external/pyBN/learning/parameter/_tests/__init__.py
--rw-r--r--   0        0        0      185 2022-12-24 09:53:41.900463 BAMT-1.1.33/bamt/external/pyBN/learning/parameter/_tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3566 2022-07-18 14:22:44.667314 BAMT-1.1.33/bamt/external/pyBN/learning/parameter/bayes.py
--rw-r--r--   0        0        0     5579 2022-07-18 14:22:44.667314 BAMT-1.1.33/bamt/external/pyBN/learning/parameter/mle.py
--rw-r--r--   0        0        0      417 2022-07-18 14:22:44.668316 BAMT-1.1.33/bamt/external/pyBN/learning/structure/__init__.py
--rw-r--r--   0        0        0      572 2022-07-18 14:38:07.224609 BAMT-1.1.33/bamt/external/pyBN/learning/structure/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3770 2022-07-18 14:38:07.248168 BAMT-1.1.33/bamt/external/pyBN/learning/structure/__pycache__/mdbn.cpython-310.pyc
--rw-r--r--   0        0        0        0 2022-07-18 14:22:44.668316 BAMT-1.1.33/bamt/external/pyBN/learning/structure/_tests/__init__.py
--rw-r--r--   0        0        0      185 2022-12-24 09:53:41.902496 BAMT-1.1.33/bamt/external/pyBN/learning/structure/_tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1821 2022-12-24 09:53:41.905088 BAMT-1.1.33/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_chow_liu.cpython-310.pyc
--rw-r--r--   0        0        0     2139 2022-12-24 09:53:41.908341 BAMT-1.1.33/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_grow_shrink.cpython-310.pyc
--rw-r--r--   0        0        0     1713 2022-12-24 09:53:41.910390 BAMT-1.1.33/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_orient_edges.cpython-310.pyc
--rw-r--r--   0        0        0     1744 2022-12-24 09:53:41.915718 BAMT-1.1.33/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_pc.cpython-310.pyc
--rw-r--r--   0        0        0     1031 2022-07-18 14:22:44.669313 BAMT-1.1.33/bamt/external/pyBN/learning/structure/_tests/test_chow_liu.py
--rw-r--r--   0        0        0     1207 2022-07-18 14:22:44.669313 BAMT-1.1.33/bamt/external/pyBN/learning/structure/_tests/test_grow_shrink.py
--rw-r--r--   0        0        0      965 2022-07-18 14:22:44.670311 BAMT-1.1.33/bamt/external/pyBN/learning/structure/_tests/test_orient_edges.py
--rw-r--r--   0        0        0      988 2022-07-18 14:22:44.670311 BAMT-1.1.33/bamt/external/pyBN/learning/structure/_tests/test_pc.py
--rw-r--r--   0        0        0      372 2022-07-18 14:22:44.674300 BAMT-1.1.33/bamt/external/pyBN/learning/structure/constraint/__init__.py
--rw-r--r--   0        0        0      548 2022-07-18 14:38:07.225606 BAMT-1.1.33/bamt/external/pyBN/learning/structure/constraint/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4331 2022-07-18 14:38:07.226602 BAMT-1.1.33/bamt/external/pyBN/learning/structure/constraint/__pycache__/fast_iamb.cpython-310.pyc
--rw-r--r--   0        0        0     4034 2022-07-18 14:38:07.227599 BAMT-1.1.33/bamt/external/pyBN/learning/structure/constraint/__pycache__/grow_shrink.cpython-310.pyc
--rw-r--r--   0        0        0     4359 2022-07-18 14:38:07.228596 BAMT-1.1.33/bamt/external/pyBN/learning/structure/constraint/__pycache__/iamb.cpython-310.pyc
--rw-r--r--   0        0        0     2892 2022-07-18 14:38:07.229592 BAMT-1.1.33/bamt/external/pyBN/learning/structure/constraint/__pycache__/lambda_iamb.cpython-310.pyc
--rw-r--r--   0        0        0     3783 2022-07-18 14:38:07.231586 BAMT-1.1.33/bamt/external/pyBN/learning/structure/constraint/__pycache__/path_condition.cpython-310.pyc
--rw-r--r--   0        0        0     4530 2022-07-18 14:22:44.675300 BAMT-1.1.33/bamt/external/pyBN/learning/structure/constraint/fast_iamb.py
--rw-r--r--   0        0        0     4648 2022-07-18 14:22:44.694145 BAMT-1.1.33/bamt/external/pyBN/learning/structure/constraint/grow_shrink.py
--rw-r--r--   0        0        0     4714 2022-07-18 14:22:44.694145 BAMT-1.1.33/bamt/external/pyBN/learning/structure/constraint/iamb.py
--rw-r--r--   0        0        0     3170 2022-07-18 14:22:44.695786 BAMT-1.1.33/bamt/external/pyBN/learning/structure/constraint/lambda_iamb.py
--rw-r--r--   0        0        0     3561 2022-07-18 14:22:44.695786 BAMT-1.1.33/bamt/external/pyBN/learning/structure/constraint/path_condition.py
--rw-r--r--   0        0        0       65 2022-07-18 14:22:44.696785 BAMT-1.1.33/bamt/external/pyBN/learning/structure/exact/__init__.py
--rw-r--r--   0        0        0      252 2022-07-18 14:38:07.231586 BAMT-1.1.33/bamt/external/pyBN/learning/structure/exact/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1743 2022-07-18 14:38:07.232582 BAMT-1.1.33/bamt/external/pyBN/learning/structure/exact/__pycache__/gobnilp.cpython-310.pyc
--rw-r--r--   0        0        0     1533 2022-07-18 14:22:44.696785 BAMT-1.1.33/bamt/external/pyBN/learning/structure/exact/gobnilp.py
--rw-r--r--   0        0        0       63 2022-07-18 14:22:44.697781 BAMT-1.1.33/bamt/external/pyBN/learning/structure/hybrid/__init__.py
--rw-r--r--   0        0        0      251 2022-07-18 14:38:07.233579 BAMT-1.1.33/bamt/external/pyBN/learning/structure/hybrid/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2480 2022-07-18 14:38:07.234575 BAMT-1.1.33/bamt/external/pyBN/learning/structure/hybrid/__pycache__/mmpc.cpython-310.pyc
--rw-r--r--   0        0        0     1527 2022-07-18 14:22:44.697781 BAMT-1.1.33/bamt/external/pyBN/learning/structure/hybrid/mmhc.py
--rw-r--r--   0        0        0     2471 2022-07-18 14:22:44.697781 BAMT-1.1.33/bamt/external/pyBN/learning/structure/hybrid/mmpc.py
--rw-r--r--   0        0        0     3604 2022-07-18 14:22:44.698778 BAMT-1.1.33/bamt/external/pyBN/learning/structure/mdbn.py
--rw-r--r--   0        0        0      132 2022-07-18 14:22:44.698778 BAMT-1.1.33/bamt/external/pyBN/learning/structure/naive/__init__.py
--rw-r--r--   0        0        0      315 2022-07-18 14:38:07.235572 BAMT-1.1.33/bamt/external/pyBN/learning/structure/naive/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2312 2022-07-18 14:38:07.236569 BAMT-1.1.33/bamt/external/pyBN/learning/structure/naive/__pycache__/naive_bayes.cpython-310.pyc
--rw-r--r--   0        0        0      870 2022-07-18 14:38:07.236569 BAMT-1.1.33/bamt/external/pyBN/learning/structure/naive/__pycache__/TAN.cpython-310.pyc
--rw-r--r--   0        0        0     1838 2022-07-18 14:22:44.699775 BAMT-1.1.33/bamt/external/pyBN/learning/structure/naive/naive_bayes.py
--rw-r--r--   0        0        0      637 2022-07-18 14:22:44.698778 BAMT-1.1.33/bamt/external/pyBN/learning/structure/naive/TAN.py
--rw-r--r--   0        0        0      353 2022-07-18 14:22:44.699775 BAMT-1.1.33/bamt/external/pyBN/learning/structure/score/__init__.py
--rw-r--r--   0        0        0      524 2022-07-18 14:38:07.237566 BAMT-1.1.33/bamt/external/pyBN/learning/structure/score/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3803 2022-07-18 14:38:07.238562 BAMT-1.1.33/bamt/external/pyBN/learning/structure/score/__pycache__/bayes_scores.cpython-310.pyc
--rw-r--r--   0        0        0     6763 2022-07-18 14:38:07.242186 BAMT-1.1.33/bamt/external/pyBN/learning/structure/score/__pycache__/hill_climbing.cpython-310.pyc
--rw-r--r--   0        0        0     5042 2022-07-18 14:38:07.243185 BAMT-1.1.33/bamt/external/pyBN/learning/structure/score/__pycache__/info_scores.cpython-310.pyc
--rw-r--r--   0        0        0     6013 2022-07-18 14:38:07.244181 BAMT-1.1.33/bamt/external/pyBN/learning/structure/score/__pycache__/random_restarts.cpython-310.pyc
--rw-r--r--   0        0        0     4959 2022-07-18 14:38:07.246175 BAMT-1.1.33/bamt/external/pyBN/learning/structure/score/__pycache__/tabu.cpython-310.pyc
--rw-r--r--   0        0        0     3797 2022-07-18 14:22:44.699775 BAMT-1.1.33/bamt/external/pyBN/learning/structure/score/bayes_scores.py
--rw-r--r--   0        0        0    11653 2022-07-18 14:22:44.699775 BAMT-1.1.33/bamt/external/pyBN/learning/structure/score/hill_climbing.py
--rw-r--r--   0        0        0     4754 2022-07-18 14:22:44.700771 BAMT-1.1.33/bamt/external/pyBN/learning/structure/score/info_scores.py
--rw-r--r--   0        0        0    10519 2022-07-18 14:22:44.700771 BAMT-1.1.33/bamt/external/pyBN/learning/structure/score/random_restarts.py
--rw-r--r--   0        0        0     6771 2022-07-18 14:22:44.700771 BAMT-1.1.33/bamt/external/pyBN/learning/structure/score/tabu.py
--rw-r--r--   0        0        0       65 2022-07-18 14:22:44.701768 BAMT-1.1.33/bamt/external/pyBN/learning/structure/tree/__init__.py
--rw-r--r--   0        0        0      251 2022-07-18 14:38:07.246175 BAMT-1.1.33/bamt/external/pyBN/learning/structure/tree/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2067 2022-07-18 14:38:07.247171 BAMT-1.1.33/bamt/external/pyBN/learning/structure/tree/__pycache__/chow_liu.cpython-310.pyc
--rw-r--r--   0        0        0     1636 2022-07-18 14:22:44.701768 BAMT-1.1.33/bamt/external/pyBN/learning/structure/tree/chow_liu.py
--rw-r--r--   0        0        0       46 2022-07-18 14:22:44.701768 BAMT-1.1.33/bamt/external/pyBN/plotting/__init__.py
--rw-r--r--   0        0        0     2546 2022-07-18 14:22:44.701768 BAMT-1.1.33/bamt/external/pyBN/plotting/plot.py
--rw-r--r--   0        0        0      593 2022-07-18 14:22:44.702765 BAMT-1.1.33/bamt/external/pyBN/utils/__init__.py
--rw-r--r--   0        0        0        0 2022-07-18 14:22:44.702765 BAMT-1.1.33/bamt/external/pyBN/utils/_tests/__init__.py
--rw-r--r--   0        0        0      172 2022-12-24 09:53:42.684367 BAMT-1.1.33/bamt/external/pyBN/utils/_tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2656 2022-12-24 09:53:42.690369 BAMT-1.1.33/bamt/external/pyBN/utils/_tests/__pycache__/test_independence_tests.cpython-310.pyc
--rw-r--r--   0        0        0     1462 2022-12-24 09:53:42.696862 BAMT-1.1.33/bamt/external/pyBN/utils/_tests/__pycache__/test_markov_blanket.cpython-310.pyc
--rw-r--r--   0        0        0     1700 2022-12-24 09:53:42.699046 BAMT-1.1.33/bamt/external/pyBN/utils/_tests/__pycache__/test_orient_edges.cpython-310.pyc
--rw-r--r--   0        0        0     1483 2022-12-24 09:53:42.704515 BAMT-1.1.33/bamt/external/pyBN/utils/_tests/__pycache__/test_random_sample.cpython-310.pyc
--rw-r--r--   0        0        0     1464 2022-07-18 14:22:44.702765 BAMT-1.1.33/bamt/external/pyBN/utils/_tests/test_independence_tests.py
--rw-r--r--   0        0        0      894 2022-07-18 14:22:44.703761 BAMT-1.1.33/bamt/external/pyBN/utils/_tests/test_markov_blanket.py
--rw-r--r--   0        0        0      965 2022-07-18 14:22:44.703761 BAMT-1.1.33/bamt/external/pyBN/utils/_tests/test_orient_edges.py
--rw-r--r--   0        0        0      776 2022-07-18 14:22:44.703761 BAMT-1.1.33/bamt/external/pyBN/utils/_tests/test_random_sample.py
--rw-r--r--   0        0        0      816 2022-07-18 14:22:44.703761 BAMT-1.1.33/bamt/external/pyBN/utils/class_equivalence.py
--rw-r--r--   0        0        0     1199 2022-07-18 14:22:44.704758 BAMT-1.1.33/bamt/external/pyBN/utils/data.py
--rw-r--r--   0        0        0     3302 2022-07-18 14:22:44.704758 BAMT-1.1.33/bamt/external/pyBN/utils/discretize.py
--rw-r--r--   0        0        0     5231 2022-07-18 14:22:44.704758 BAMT-1.1.33/bamt/external/pyBN/utils/graph.py
--rw-r--r--   0        0        0      779 2022-07-18 14:22:44.704758 BAMT-1.1.33/bamt/external/pyBN/utils/hybrid_distance.py
--rw-r--r--   0        0        0    14362 2022-07-18 14:22:44.705754 BAMT-1.1.33/bamt/external/pyBN/utils/independence_tests.py
--rw-r--r--   0        0        0     4541 2022-07-18 14:22:44.705754 BAMT-1.1.33/bamt/external/pyBN/utils/markov_blanket.py
--rw-r--r--   0        0        0     4823 2022-07-18 14:22:44.705754 BAMT-1.1.33/bamt/external/pyBN/utils/orient_edges.py
--rw-r--r--   0        0        0     3730 2022-07-18 14:22:44.706751 BAMT-1.1.33/bamt/external/pyBN/utils/parameter_distance.py
--rw-r--r--   0        0        0     1659 2022-07-18 14:22:44.706751 BAMT-1.1.33/bamt/external/pyBN/utils/random_sample.py
--rw-r--r--   0        0        0     2745 2022-07-18 14:22:44.706751 BAMT-1.1.33/bamt/external/pyBN/utils/structure_distance.py
--rw-r--r--   0        0        0      979 2023-03-17 12:29:52.731831 BAMT-1.1.33/bamt/log.py
--rw-r--r--   0        0        0     1090 2022-08-01 09:44:45.658643 BAMT-1.1.33/bamt/logging.conf
--rw-r--r--   0        0        0    10943 2023-03-17 12:29:52.731831 BAMT-1.1.33/bamt/mi_entropy_gauss.py
--rw-r--r--   0        0        0    35209 2023-03-22 10:23:08.167146 BAMT-1.1.33/bamt/networks.py
--rw-r--r--   0        0        0    50481 2023-03-22 09:31:51.375608 BAMT-1.1.33/bamt/nodes.py
--rw-r--r--   0        0        0        0 2022-07-18 14:22:44.707748 BAMT-1.1.33/bamt/preprocess/__init__.py
--rw-r--r--   0        0        0     5449 2023-03-17 12:29:52.733830 BAMT-1.1.33/bamt/preprocess/discretization.py
--rw-r--r--   0        0        0      871 2023-03-17 12:29:52.734830 BAMT-1.1.33/bamt/preprocess/graph.py
--rw-r--r--   0        0        0     1904 2023-03-17 12:29:52.734830 BAMT-1.1.33/bamt/preprocess/numpy_pandas.py
--rw-r--r--   0        0        0     4363 2023-03-17 12:29:52.735830 BAMT-1.1.33/bamt/preprocessors.py
--rw-r--r--   0        0        0    13188 2023-03-17 12:29:52.736830 BAMT-1.1.33/bamt/redef_HC.py
--rw-r--r--   0        0        0     6572 2023-03-17 12:29:52.736830 BAMT-1.1.33/bamt/redef_info_scores.py
--rw-r--r--   0        0        0        0 2022-07-18 14:22:44.709741 BAMT-1.1.33/bamt/utils/__init__.py
--rw-r--r--   0        0        0     2407 2023-03-22 09:31:51.375608 BAMT-1.1.33/bamt/utils/GraphUtils.py
--rw-r--r--   0        0        0     7658 2023-03-17 12:29:52.737830 BAMT-1.1.33/bamt/utils/MathUtils.py
--rw-r--r--   0        0        0     1168 2023-03-23 13:55:37.753597 BAMT-1.1.33/pyproject.toml
--rw-r--r--   0        0        0     8820 2023-03-17 18:51:26.332933 BAMT-1.1.33/README.rst
--rw-r--r--   0        0        0    10804 2023-03-23 14:04:11.848250 BAMT-1.1.33/setup.py
--rw-r--r--   0        0        0     9711 2023-03-23 14:04:11.848250 BAMT-1.1.33/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-10-18 09:46:52.969462 BAMT-1.1.40/bamt/__init__.py
+-rw-r--r--   0        0        0    14998 2023-04-10 14:01:43.784052 BAMT-1.1.40/bamt/builders.py
+-rw-r--r--   0        0        0      688 2023-04-10 14:01:43.785048 BAMT-1.1.40/bamt/config.py
+-rw-r--r--   0        0        0        0 2022-07-18 14:22:44.582873 BAMT-1.1.40/bamt/external/__init__.py
+-rw-r--r--   0        0        0      154 2023-03-22 08:13:29.970622 BAMT-1.1.40/bamt/external/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      373 2022-12-24 09:53:39.265727 BAMT-1.1.40/bamt/external/libpgm/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0       82 2023-04-10 14:01:43.785048 BAMT-1.1.40/bamt/external/pyBN/__init__.py
+-rw-r--r--   0        0        0      238 2023-03-27 20:03:35.633736 BAMT-1.1.40/bamt/external/pyBN/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2023-04-10 14:01:43.785048 BAMT-1.1.40/bamt/external/pyBN/classes/__init__.py
+-rw-r--r--   0        0        0      167 2023-03-27 20:03:35.635733 BAMT-1.1.40/bamt/external/pyBN/classes/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    12842 2023-03-27 20:03:35.673859 BAMT-1.1.40/bamt/external/pyBN/classes/__pycache__/bayesnet.cpython-310.pyc
+-rw-r--r--   0        0        0    10770 2023-03-27 08:04:03.587482 BAMT-1.1.40/bamt/external/pyBN/classes/__pycache__/cliquetree.cpython-310.pyc
+-rw-r--r--   0        0        0     4738 2023-03-27 08:04:03.584486 BAMT-1.1.40/bamt/external/pyBN/classes/__pycache__/clustergraph.cpython-310.pyc
+-rw-r--r--   0        0        0     5165 2023-03-27 08:04:03.681327 BAMT-1.1.40/bamt/external/pyBN/classes/__pycache__/empiricaldistribution.cpython-310.pyc
+-rw-r--r--   0        0        0    17971 2023-03-27 08:04:03.593487 BAMT-1.1.40/bamt/external/pyBN/classes/__pycache__/factor.cpython-310.pyc
+-rw-r--r--   0        0        0     4873 2023-03-27 08:04:03.590484 BAMT-1.1.40/bamt/external/pyBN/classes/__pycache__/factorization.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2022-07-18 14:22:44.588854 BAMT-1.1.40/bamt/external/pyBN/classes/_tests/__init__.py
+-rw-r--r--   0        0        0      174 2022-12-24 09:53:41.854845 BAMT-1.1.40/bamt/external/pyBN/classes/_tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5230 2022-12-24 09:53:41.861558 BAMT-1.1.40/bamt/external/pyBN/classes/_tests/__pycache__/test_bayesnet.cpython-310.pyc
+-rw-r--r--   0        0        0     6379 2022-12-24 09:53:41.867553 BAMT-1.1.40/bamt/external/pyBN/classes/_tests/__pycache__/test_factor.cpython-310.pyc
+-rw-r--r--   0        0        0     5520 2023-04-10 14:01:43.786046 BAMT-1.1.40/bamt/external/pyBN/classes/_tests/test_bayesnet.py
+-rw-r--r--   0        0        0    11006 2023-04-10 14:01:43.787042 BAMT-1.1.40/bamt/external/pyBN/classes/bayesnet.py
+-rw-r--r--   0        0        0      302 2023-03-27 08:04:03.623486 BAMT-1.1.40/bamt/external/pyBN/classification/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3370 2023-03-27 08:04:03.624483 BAMT-1.1.40/bamt/external/pyBN/classification/__pycache__/classification.cpython-310.pyc
+-rw-r--r--   0        0        0     3432 2023-03-27 08:04:03.647079 BAMT-1.1.40/bamt/external/pyBN/classification/__pycache__/feature_selection.cpython-310.pyc
+-rw-r--r--   0        0        0      335 2023-03-27 08:04:03.626130 BAMT-1.1.40/bamt/external/pyBN/inference/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      176 2022-12-24 09:53:41.870556 BAMT-1.1.40/bamt/external/pyBN/inference/_tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1060 2022-12-24 09:53:41.876256 BAMT-1.1.40/bamt/external/pyBN/inference/_tests/__pycache__/test_map_exact.cpython-310.pyc
+-rw-r--r--   0        0        0     2776 2022-12-24 09:53:41.882205 BAMT-1.1.40/bamt/external/pyBN/inference/_tests/__pycache__/test_marginal_approx.cpython-310.pyc
+-rw-r--r--   0        0        0     2251 2022-12-24 09:53:41.886925 BAMT-1.1.40/bamt/external/pyBN/inference/_tests/__pycache__/test_marginal_exact.cpython-310.pyc
+-rw-r--r--   0        0        0      299 2023-03-27 08:04:03.628136 BAMT-1.1.40/bamt/external/pyBN/inference/map_exact/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2653 2023-03-27 08:04:03.630137 BAMT-1.1.40/bamt/external/pyBN/inference/map_exact/__pycache__/ilp_map.cpython-310.pyc
+-rw-r--r--   0        0        0     1077 2023-03-27 08:04:03.631117 BAMT-1.1.40/bamt/external/pyBN/inference/map_exact/__pycache__/ve_map.cpython-310.pyc
+-rw-r--r--   0        0        0      461 2023-03-27 08:04:03.632119 BAMT-1.1.40/bamt/external/pyBN/inference/marginal_approx/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2050 2023-03-27 08:04:03.634118 BAMT-1.1.40/bamt/external/pyBN/inference/marginal_approx/__pycache__/forward_sample.cpython-310.pyc
+-rw-r--r--   0        0        0     1553 2023-03-27 08:04:03.639077 BAMT-1.1.40/bamt/external/pyBN/inference/marginal_approx/__pycache__/gibbs_sample.cpython-310.pyc
+-rw-r--r--   0        0        0     1783 2023-03-27 08:04:03.641082 BAMT-1.1.40/bamt/external/pyBN/inference/marginal_approx/__pycache__/loopy_bp.cpython-310.pyc
+-rw-r--r--   0        0        0     1613 2023-03-27 08:04:03.642078 BAMT-1.1.40/bamt/external/pyBN/inference/marginal_approx/__pycache__/lw_sample.cpython-310.pyc
+-rw-r--r--   0        0        0      320 2023-03-27 08:04:03.643078 BAMT-1.1.40/bamt/external/pyBN/inference/marginal_exact/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2054 2023-03-27 08:04:03.645083 BAMT-1.1.40/bamt/external/pyBN/inference/marginal_exact/__pycache__/exact_bp.cpython-310.pyc
+-rw-r--r--   0        0        0     1432 2023-03-27 08:04:03.646078 BAMT-1.1.40/bamt/external/pyBN/inference/marginal_exact/__pycache__/ve_marginal.cpython-310.pyc
+-rw-r--r--   0        0        0      244 2023-03-27 08:04:03.695089 BAMT-1.1.40/bamt/external/pyBN/io/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5673 2023-03-27 08:04:03.697093 BAMT-1.1.40/bamt/external/pyBN/io/__pycache__/read.cpython-310.pyc
+-rw-r--r--   0        0        0     1690 2023-03-27 08:04:03.699093 BAMT-1.1.40/bamt/external/pyBN/io/__pycache__/write.cpython-310.pyc
+-rw-r--r--   0        0        0      169 2022-12-24 09:53:41.889932 BAMT-1.1.40/bamt/external/pyBN/io/_tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1451 2022-12-24 09:53:41.894772 BAMT-1.1.40/bamt/external/pyBN/io/_tests/__pycache__/test_reading.cpython-310.pyc
+-rw-r--r--   0        0        0      888 2022-12-24 09:53:41.899461 BAMT-1.1.40/bamt/external/pyBN/io/_tests/__pycache__/test_writing.cpython-310.pyc
+-rw-r--r--   0        0        0      271 2023-03-27 08:04:03.649082 BAMT-1.1.40/bamt/external/pyBN/learning/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      291 2023-03-27 08:04:03.650078 BAMT-1.1.40/bamt/external/pyBN/learning/parameter/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3832 2023-03-27 08:04:03.652079 BAMT-1.1.40/bamt/external/pyBN/learning/parameter/__pycache__/bayes.cpython-310.pyc
+-rw-r--r--   0        0        0     5978 2023-03-27 08:04:03.654087 BAMT-1.1.40/bamt/external/pyBN/learning/parameter/__pycache__/mle.cpython-310.pyc
+-rw-r--r--   0        0        0      185 2022-12-24 09:53:41.900463 BAMT-1.1.40/bamt/external/pyBN/learning/parameter/_tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      572 2023-03-27 08:04:03.655095 BAMT-1.1.40/bamt/external/pyBN/learning/structure/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3770 2023-03-27 08:04:03.694090 BAMT-1.1.40/bamt/external/pyBN/learning/structure/__pycache__/mdbn.cpython-310.pyc
+-rw-r--r--   0        0        0      185 2022-12-24 09:53:41.902496 BAMT-1.1.40/bamt/external/pyBN/learning/structure/_tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1821 2022-12-24 09:53:41.905088 BAMT-1.1.40/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_chow_liu.cpython-310.pyc
+-rw-r--r--   0        0        0     2139 2022-12-24 09:53:41.908341 BAMT-1.1.40/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_grow_shrink.cpython-310.pyc
+-rw-r--r--   0        0        0     1713 2022-12-24 09:53:41.910390 BAMT-1.1.40/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_orient_edges.cpython-310.pyc
+-rw-r--r--   0        0        0     1744 2022-12-24 09:53:41.915718 BAMT-1.1.40/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_pc.cpython-310.pyc
+-rw-r--r--   0        0        0      548 2023-03-27 08:04:03.657092 BAMT-1.1.40/bamt/external/pyBN/learning/structure/constraint/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4331 2023-03-27 08:04:03.659096 BAMT-1.1.40/bamt/external/pyBN/learning/structure/constraint/__pycache__/fast_iamb.cpython-310.pyc
+-rw-r--r--   0        0        0     4034 2023-03-27 08:04:03.660092 BAMT-1.1.40/bamt/external/pyBN/learning/structure/constraint/__pycache__/grow_shrink.cpython-310.pyc
+-rw-r--r--   0        0        0     4359 2023-03-27 08:04:03.662095 BAMT-1.1.40/bamt/external/pyBN/learning/structure/constraint/__pycache__/iamb.cpython-310.pyc
+-rw-r--r--   0        0        0     2892 2023-03-27 08:04:03.663691 BAMT-1.1.40/bamt/external/pyBN/learning/structure/constraint/__pycache__/lambda_iamb.cpython-310.pyc
+-rw-r--r--   0        0        0     3783 2023-03-27 08:04:03.665697 BAMT-1.1.40/bamt/external/pyBN/learning/structure/constraint/__pycache__/path_condition.cpython-310.pyc
+-rw-r--r--   0        0        0      252 2023-03-27 08:04:03.666694 BAMT-1.1.40/bamt/external/pyBN/learning/structure/exact/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1743 2023-03-27 08:04:03.668693 BAMT-1.1.40/bamt/external/pyBN/learning/structure/exact/__pycache__/gobnilp.cpython-310.pyc
+-rw-r--r--   0        0        0      251 2023-03-27 08:04:03.669694 BAMT-1.1.40/bamt/external/pyBN/learning/structure/hybrid/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2480 2023-03-27 08:04:03.671004 BAMT-1.1.40/bamt/external/pyBN/learning/structure/hybrid/__pycache__/mmpc.cpython-310.pyc
+-rw-r--r--   0        0        0      315 2023-03-27 08:04:03.672006 BAMT-1.1.40/bamt/external/pyBN/learning/structure/naive/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2312 2023-03-27 08:04:03.674010 BAMT-1.1.40/bamt/external/pyBN/learning/structure/naive/__pycache__/naive_bayes.cpython-310.pyc
+-rw-r--r--   0        0        0      870 2023-03-27 08:04:03.675322 BAMT-1.1.40/bamt/external/pyBN/learning/structure/naive/__pycache__/TAN.cpython-310.pyc
+-rw-r--r--   0        0        0      524 2023-03-27 08:04:03.676326 BAMT-1.1.40/bamt/external/pyBN/learning/structure/score/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3803 2023-03-27 08:04:03.678326 BAMT-1.1.40/bamt/external/pyBN/learning/structure/score/__pycache__/bayes_scores.cpython-310.pyc
+-rw-r--r--   0        0        0     6763 2023-03-27 08:04:03.683330 BAMT-1.1.40/bamt/external/pyBN/learning/structure/score/__pycache__/hill_climbing.cpython-310.pyc
+-rw-r--r--   0        0        0     5042 2023-03-27 08:04:03.684326 BAMT-1.1.40/bamt/external/pyBN/learning/structure/score/__pycache__/info_scores.cpython-310.pyc
+-rw-r--r--   0        0        0     6013 2023-03-27 08:04:03.687330 BAMT-1.1.40/bamt/external/pyBN/learning/structure/score/__pycache__/random_restarts.cpython-310.pyc
+-rw-r--r--   0        0        0     4959 2023-03-27 08:04:03.689330 BAMT-1.1.40/bamt/external/pyBN/learning/structure/score/__pycache__/tabu.cpython-310.pyc
+-rw-r--r--   0        0        0      251 2023-03-27 08:04:03.691046 BAMT-1.1.40/bamt/external/pyBN/learning/structure/tree/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2067 2023-03-27 08:04:03.692088 BAMT-1.1.40/bamt/external/pyBN/learning/structure/tree/__pycache__/chow_liu.cpython-310.pyc
+-rw-r--r--   0        0        0      217 2022-12-24 09:53:41.922124 BAMT-1.1.40/bamt/external/pyBN/plotting/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2504 2022-12-24 09:53:41.930964 BAMT-1.1.40/bamt/external/pyBN/plotting/__pycache__/plot.cpython-310.pyc
+-rw-r--r--   0        0        0      208 2023-04-10 14:01:43.787042 BAMT-1.1.40/bamt/external/pyBN/utils/__init__.py
+-rw-r--r--   0        0        0      362 2023-03-27 20:03:35.640736 BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      948 2023-03-27 20:03:35.646737 BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/class_equivalence.cpython-310.pyc
+-rw-r--r--   0        0        0      840 2023-03-27 20:03:35.653137 BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/data.cpython-310.pyc
+-rw-r--r--   0        0        0     3156 2023-03-27 08:04:03.602487 BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/discretize.cpython-310.pyc
+-rw-r--r--   0        0        0     1274 2023-03-27 20:03:35.658779 BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/graph.cpython-310.pyc
+-rw-r--r--   0        0        0      973 2023-03-27 08:04:03.606486 BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/hybrid_distance.cpython-310.pyc
+-rw-r--r--   0        0        0     4392 2023-03-27 20:03:35.665794 BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/independence_tests.cpython-310.pyc
+-rw-r--r--   0        0        0     4723 2023-03-27 08:04:03.612483 BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/markov_blanket.cpython-310.pyc
+-rw-r--r--   0        0        0     4640 2023-03-27 08:04:03.615487 BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/orient_edges.cpython-310.pyc
+-rw-r--r--   0        0        0     3492 2023-03-27 08:04:03.617486 BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/parameter_distance.cpython-310.pyc
+-rw-r--r--   0        0        0     1943 2023-03-27 08:04:03.619487 BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/random_sample.cpython-310.pyc
+-rw-r--r--   0        0        0     2896 2023-03-27 08:04:03.621487 BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/structure_distance.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2022-07-18 14:22:44.702765 BAMT-1.1.40/bamt/external/pyBN/utils/_tests/__init__.py
+-rw-r--r--   0        0        0      172 2022-12-24 09:53:42.684367 BAMT-1.1.40/bamt/external/pyBN/utils/_tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2656 2022-12-24 09:53:42.690369 BAMT-1.1.40/bamt/external/pyBN/utils/_tests/__pycache__/test_independence_tests.cpython-310.pyc
+-rw-r--r--   0        0        0     1462 2022-12-24 09:53:42.696862 BAMT-1.1.40/bamt/external/pyBN/utils/_tests/__pycache__/test_markov_blanket.cpython-310.pyc
+-rw-r--r--   0        0        0     1700 2022-12-24 09:53:42.699046 BAMT-1.1.40/bamt/external/pyBN/utils/_tests/__pycache__/test_orient_edges.cpython-310.pyc
+-rw-r--r--   0        0        0     1483 2022-12-24 09:53:42.704515 BAMT-1.1.40/bamt/external/pyBN/utils/_tests/__pycache__/test_random_sample.cpython-310.pyc
+-rw-r--r--   0        0        0     1788 2023-04-10 14:01:43.787042 BAMT-1.1.40/bamt/external/pyBN/utils/_tests/test_independence_tests.py
+-rw-r--r--   0        0        0     1155 2023-04-10 14:01:43.788038 BAMT-1.1.40/bamt/external/pyBN/utils/_tests/test_markov_blanket.py
+-rw-r--r--   0        0        0     1205 2023-04-10 14:01:43.788038 BAMT-1.1.40/bamt/external/pyBN/utils/_tests/test_orient_edges.py
+-rw-r--r--   0        0        0      970 2023-04-10 14:01:43.788038 BAMT-1.1.40/bamt/external/pyBN/utils/_tests/test_random_sample.py
+-rw-r--r--   0        0        0      907 2023-04-10 14:01:43.789035 BAMT-1.1.40/bamt/external/pyBN/utils/class_equivalence.py
+-rw-r--r--   0        0        0      626 2023-04-10 14:01:43.789035 BAMT-1.1.40/bamt/external/pyBN/utils/data.py
+-rw-r--r--   0        0        0     1386 2023-04-10 14:01:43.790031 BAMT-1.1.40/bamt/external/pyBN/utils/graph.py
+-rw-r--r--   0        0        0     6222 2023-04-10 14:01:43.790031 BAMT-1.1.40/bamt/external/pyBN/utils/independence_tests.py
+-rw-r--r--   0        0        0      979 2023-03-17 12:29:52.731831 BAMT-1.1.40/bamt/log.py
+-rw-r--r--   0        0        0     1090 2022-08-01 09:44:45.658643 BAMT-1.1.40/bamt/logging.conf
+-rw-r--r--   0        0        0    10778 2023-04-10 14:01:43.791028 BAMT-1.1.40/bamt/mi_entropy_gauss.py
+-rw-r--r--   0        0        0      119 2023-04-10 14:01:43.791028 BAMT-1.1.40/bamt/networks/__init__.py
+-rw-r--r--   0        0        0      229 2023-03-27 20:16:49.956781 BAMT-1.1.40/bamt/networks/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    26367 2023-03-31 13:44:44.700941 BAMT-1.1.40/bamt/networks/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     1115 2023-03-28 14:57:14.478682 BAMT-1.1.40/bamt/networks/__pycache__/hybrid_bn.cpython-310.pyc
+-rw-r--r--   0        0        0    31404 2023-04-10 14:01:43.792025 BAMT-1.1.40/bamt/networks/base.py
+-rw-r--r--   0        0        0     1704 2023-04-10 14:01:43.792025 BAMT-1.1.40/bamt/networks/big_brave_bn.py
+-rw-r--r--   0        0        0      422 2023-04-10 14:01:43.792025 BAMT-1.1.40/bamt/networks/continuous_bn.py
+-rw-r--r--   0        0        0      392 2023-04-10 14:01:43.792025 BAMT-1.1.40/bamt/networks/discrete_bn.py
+-rw-r--r--   0        0        0      737 2023-04-10 14:01:43.793022 BAMT-1.1.40/bamt/networks/hybrid_bn.py
+-rw-r--r--   0        0        0      223 2023-04-10 14:01:43.793022 BAMT-1.1.40/bamt/nodes/__init__.py
+-rw-r--r--   0        0        0      324 2023-03-25 11:38:48.177276 BAMT-1.1.40/bamt/nodes/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2653 2023-03-31 13:44:42.957971 BAMT-1.1.40/bamt/nodes/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     4702 2023-03-27 08:25:39.343392 BAMT-1.1.40/bamt/nodes/__pycache__/conditional_gaussian_node.cpython-310.pyc
+-rw-r--r--   0        0        0     4717 2023-03-27 08:25:39.380393 BAMT-1.1.40/bamt/nodes/__pycache__/conditional_logit_node.cpython-310.pyc
+-rw-r--r--   0        0        0     5041 2023-03-25 11:38:48.587289 BAMT-1.1.40/bamt/nodes/__pycache__/conditional_mixture_gaussian_node.cpython-310.pyc
+-rw-r--r--   0        0        0     4095 2023-03-25 11:38:49.014930 BAMT-1.1.40/bamt/nodes/__pycache__/discrete_node.cpython-310.pyc
+-rw-r--r--   0        0        0     3396 2023-03-27 08:25:39.477816 BAMT-1.1.40/bamt/nodes/__pycache__/gaussian_node.cpython-310.pyc
+-rw-r--r--   0        0        0     3270 2023-03-27 08:25:39.475813 BAMT-1.1.40/bamt/nodes/__pycache__/logit_node.cpython-310.pyc
+-rw-r--r--   0        0        0     3723 2023-03-25 11:38:49.780249 BAMT-1.1.40/bamt/nodes/__pycache__/mixture_gaussian_node.cpython-310.pyc
+-rw-r--r--   0        0        0     1796 2023-03-25 11:16:57.986776 BAMT-1.1.40/bamt/nodes/__pycache__/schema.cpython-310.pyc
+-rw-r--r--   0        0        0     2685 2023-04-10 14:01:43.793022 BAMT-1.1.40/bamt/nodes/base.py
+-rw-r--r--   0        0        0     7951 2023-04-10 14:01:43.793022 BAMT-1.1.40/bamt/nodes/conditional_gaussian_node.py
+-rw-r--r--   0        0        0     6920 2023-04-10 14:01:43.794018 BAMT-1.1.40/bamt/nodes/conditional_logit_node.py
+-rw-r--r--   0        0        0     8119 2023-04-10 14:01:43.794018 BAMT-1.1.40/bamt/nodes/conditional_mixture_gaussian_node.py
+-rw-r--r--   0        0        0     4064 2023-04-10 14:01:43.794018 BAMT-1.1.40/bamt/nodes/discrete_node.py
+-rw-r--r--   0        0        0     4424 2023-04-10 14:01:43.795015 BAMT-1.1.40/bamt/nodes/gaussian_node.py
+-rw-r--r--   0        0        0     4026 2023-04-10 14:01:43.795015 BAMT-1.1.40/bamt/nodes/logit_node.py
+-rw-r--r--   0        0        0     5476 2023-04-10 14:01:43.795015 BAMT-1.1.40/bamt/nodes/mixture_gaussian_node.py
+-rw-r--r--   0        0        0     1034 2023-04-10 14:01:43.795015 BAMT-1.1.40/bamt/nodes/schema.py
+-rw-r--r--   0        0        0        0 2022-07-18 14:22:44.707748 BAMT-1.1.40/bamt/preprocess/__init__.py
+-rw-r--r--   0        0        0      156 2023-03-22 08:13:30.026531 BAMT-1.1.40/bamt/preprocess/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5287 2023-03-22 08:13:30.040531 BAMT-1.1.40/bamt/preprocess/__pycache__/discretization.cpython-310.pyc
+-rw-r--r--   0        0        0     1292 2023-03-22 08:13:30.056531 BAMT-1.1.40/bamt/preprocess/__pycache__/graph.cpython-310.pyc
+-rw-r--r--   0        0        0     1993 2023-03-22 08:13:30.051545 BAMT-1.1.40/bamt/preprocess/__pycache__/numpy_pandas.cpython-310.pyc
+-rw-r--r--   0        0        0     5449 2023-03-17 12:29:52.733830 BAMT-1.1.40/bamt/preprocess/discretization.py
+-rw-r--r--   0        0        0      871 2023-03-17 12:29:52.734830 BAMT-1.1.40/bamt/preprocess/graph.py
+-rw-r--r--   0        0        0     1904 2023-03-17 12:29:52.734830 BAMT-1.1.40/bamt/preprocess/numpy_pandas.py
+-rw-r--r--   0        0        0     4363 2023-03-17 12:29:52.735830 BAMT-1.1.40/bamt/preprocessors.py
+-rw-r--r--   0        0        0    12521 2023-04-10 14:01:43.796011 BAMT-1.1.40/bamt/redef_HC.py
+-rw-r--r--   0        0        0     6177 2023-04-10 14:01:43.797008 BAMT-1.1.40/bamt/redef_info_scores.py
+-rw-r--r--   0        0        0        0 2022-07-18 14:22:44.709741 BAMT-1.1.40/bamt/utils/__init__.py
+-rw-r--r--   0        0        0      151 2023-03-22 08:13:30.083531 BAMT-1.1.40/bamt/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2543 2023-03-27 08:04:04.969879 BAMT-1.1.40/bamt/utils/__pycache__/GraphUtils.cpython-310.pyc
+-rw-r--r--   0        0        0     6440 2023-03-22 08:14:15.703888 BAMT-1.1.40/bamt/utils/__pycache__/MathUtils.cpython-310.pyc
+-rw-r--r--   0        0        0     2412 2023-04-10 14:01:43.797008 BAMT-1.1.40/bamt/utils/GraphUtils.py
+-rw-r--r--   0        0        0     7658 2023-03-17 12:29:52.737830 BAMT-1.1.40/bamt/utils/MathUtils.py
+-rw-r--r--   0        0        0     1188 2023-04-20 12:46:05.088240 BAMT-1.1.40/pyproject.toml
+-rw-r--r--   0        0        0     8820 2023-03-17 18:51:26.332933 BAMT-1.1.40/README.rst
+-rw-r--r--   0        0        0     9963 2023-04-20 12:56:36.209555 BAMT-1.1.40/setup.py
+-rw-r--r--   0        0        0     9711 2023-04-20 12:56:36.210555 BAMT-1.1.40/PKG-INFO
```

### Comparing `BAMT-1.1.33/bamt/builders.py` & `BAMT-1.1.40/bamt/builders.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 import itertools
 
 from pgmpy.base import DAG
 from pgmpy.estimators import HillClimbSearch
 from bamt.redef_HC import hc as hc_method
 
-from bamt import nodes
+from bamt.nodes.discrete_node import DiscreteNode
+from bamt.nodes.gaussian_node import GaussianNode
+from bamt.nodes.conditional_logit_node import ConditionalLogitNode
+from bamt.nodes.logit_node import LogitNode
+from bamt.nodes.mixture_gaussian_node import MixtureGaussianNode
+from bamt.nodes.conditional_mixture_gaussian_node import ConditionalMixtureGaussianNode
+from bamt.nodes.conditional_gaussian_node import ConditionalGaussianNode
+
 from bamt.log import logger_builder
 from pandas import DataFrame
 from bamt.utils import GraphUtils as gru
 
-from typing import Dict, List, Optional, Tuple, Callable, TypedDict, Union
+from typing import Dict, List, Optional, Tuple, Callable, TypedDict, Union, Sequence
 
 
 class ParamDict(TypedDict, total=False):
-    init_edges: Optional[Tuple[str, str]]
+    init_edges: Optional[Sequence[str]]
     init_nodes: Optional[List[str]]
     remove_init_edges: bool
     white_list: Optional[Tuple[str, str]]
     bl_add: Optional[List[str]]
 
 
 class StructureBuilder(object):
@@ -26,19 +33,18 @@
     It can restrict nodes defined by RESTRICTIONS
     """
 
     def __init__(self, descriptor: Dict[str, Dict[str, str]]):
         """
         :param descriptor: a dict with types and signs of nodes
         Attributes:
-        Skeleton: dict;
         black_list: a list with restricted connections;
         """
-        self.skeleton = {'V': None,
-                         'E': None}
+        self.skeleton = {'V': [],
+                         'E': []}
         self.descriptor = descriptor
 
         self.has_logit = bool
 
         self.black_list = None
 
     def restrict(self, data: DataFrame,
@@ -50,15 +56,14 @@
         :param bl_add: additional vertices
         """
         node_type = self.descriptor['types']
         blacklist = []
         datacol = data.columns.to_list()
 
         if not self.has_logit:
-
             # Has_logit flag allows BN building edges between cont and disc
             RESTRICTIONS = [('cont', 'disc'), ('cont', 'disc_num')]
             for x, y in itertools.product(datacol, repeat=2):
                 if x != y:
                     if (node_type[x], node_type[y]) in RESTRICTIONS:
                         blacklist.append((x, y))
         else:
@@ -120,28 +125,28 @@
         """
         Automatically creates a list of nodes
         """
         super(VerticesDefiner, self).__init__(descriptor=descriptor)
         # Notice that vertices are used only by Builders
         self.vertices = []
 
-        Node = None
+        node = None
         # LEVEL 1: Define a general type of node: Discrete or Gaussian
         for vertex, type in self.descriptor['types'].items():
             if type in ['disc_num', 'disc']:
-                Node = nodes.DiscreteNode(name=vertex)
+                node = DiscreteNode(name=vertex)
             elif type == 'cont':
-                Node = nodes.GaussianNode(name=vertex, regressor=regressor)
+                node = GaussianNode(name=vertex, regressor=regressor)
             else:
                 msg = f"""First stage of automatic vertex detection failed on {vertex} due TypeError ({type}).
                 Set vertex manually (by calling set_nodes()) or investigate the error."""
                 logger_builder.error(msg)
                 continue
 
-            self.vertices.append(Node)
+            self.vertices.append(node)
 
     def overwrite_vertex(
             self,
             has_logit: bool,
             use_mixture: bool,
             classifier: Optional[Callable],
             regressor: Optional[Callable]):
@@ -149,52 +154,52 @@
         Level 2: Redefined nodes according structure (parents)
         :param classifier: an object to pass into logit, condLogit nodes
         :param regressor: an object to pass into gaussianish nodes
         :param has_logit allows edges from cont to disc nodes
         :param use_mixture allows using Mixture
         """
         for node_instance in self.vertices:
-            Node = node_instance
+            node = node_instance
             if has_logit:
                 if 'Discrete' in node_instance.type:
                     if node_instance.cont_parents:
                         if not node_instance.disc_parents:
-                            Node = nodes.LogitNode(
+                            node = LogitNode(
                                 name=node_instance.name, classifier=classifier)
 
                         elif node_instance.disc_parents:
-                            Node = nodes.ConditionalLogitNode(
+                            node = ConditionalLogitNode(
                                 name=node_instance.name, classifier=classifier)
 
             if use_mixture:
                 if 'Gaussian' in node_instance.type:
                     if not node_instance.disc_parents:
-                        Node = nodes.MixtureGaussianNode(
+                        node = MixtureGaussianNode(
                             name=node_instance.name)
                     elif node_instance.disc_parents:
-                        Node = nodes.ConditionalMixtureGaussianNode(
+                        node = ConditionalMixtureGaussianNode(
                             name=node_instance.name)
                     else:
                         continue
             else:
                 if 'Gaussian' in node_instance.type:
                     if node_instance.disc_parents:
-                        Node = nodes.ConditionalGaussianNode(
+                        node = ConditionalGaussianNode(
                             name=node_instance.name, regressor=regressor)
                     else:
                         continue
 
-            if node_instance == Node:
+            if node_instance == node:
                 continue
 
             id = self.skeleton['V'].index(node_instance)
-            Node.disc_parents = node_instance.disc_parents
-            Node.cont_parents = node_instance.cont_parents
-            Node.children = node_instance.children
-            self.skeleton['V'][id] = Node
+            node.disc_parents = node_instance.disc_parents
+            node.cont_parents = node_instance.cont_parents
+            node.children = node_instance.children
+            self.skeleton['V'][id] = node
 
 
 class EdgesDefiner(StructureBuilder):
     def __init__(self, descriptor: Dict[str, Dict[str, str]]):
         super(EdgesDefiner, self).__init__(descriptor)
 
 
@@ -205,44 +210,42 @@
 
     def __init__(self, data: DataFrame, descriptor: Dict[str, Dict[str, str]],
                  scoring_function: Union[Tuple[str, Callable], Tuple[str]],
                  regressor: Optional[object] = None):
         """
         :param scoring_function: a tuple with following format (Name, scoring_function)
         """
-        # if len(scoring_function) == 2:
-        #     if callable(scoring_function[1]):
-        #         logger_builder.error("Cannot call scoring function")
 
         self.scoring_function = scoring_function
         self.optimizer = HillClimbSearch(data)
         self.params = {'init_edges': None,
                        'init_nodes': None,
                        'remove_init_edges': True,
                        'white_list': None,
                        'bl_add': None}
         super(HillClimbDefiner, self).__init__(descriptor, regressor=regressor)
 
     def apply_K2(self,
                  data: DataFrame,
                  init_edges: Optional[List[Tuple[str,
-                                                 str]]],
+                 str]]],
                  progress_bar: bool,
                  remove_init_edges: bool,
                  white_list: Optional[List[Tuple[str,
-                                                 str]]]):
+                 str]]]):
         """
         :param init_edges: list of tuples, a graph to start learning with
-        :param remove_init_edges: allows changes in model defined by user
+        :param remove_init_edges: allows changes in a model defined by user
+        :param data: user's data
         :param progress_bar: verbose regime
         :param white_list: list of allowed edges
         """
         import bamt.utils.GraphUtils as gru
         if not all([i in ['disc', 'disc_num']
-                   for i in gru.nodes_types(data).values()]):
+                    for i in gru.nodes_types(data).values()]):
             logger_builder.error(
                 f"K2 deals only with discrete data. Continuous data: {[col for col, type in gru.nodes_types(data).items() if type not in ['disc', 'disc_num']]}")
             return None
 
         if len(self.scoring_function) != 2:
             from pgmpy.estimators import K2Score
             scoring_function = K2Score
@@ -278,21 +281,28 @@
         structure = [list(x) for x in list(best_model.edges())]
         self.skeleton['E'] = structure
 
     def apply_group1(self,
                      data: DataFrame,
                      progress_bar: bool,
                      init_edges: Optional[List[Tuple[str,
-                                                     str]]],
+                     str]]],
                      remove_init_edges: bool,
                      white_list: Optional[List[Tuple[str,
-                                                     str]]]):
-        # (score == "MI") | (score == "LL") | (score == "BIC") | (score == "AIC")
+                     str]]]):
+        """
+        This method implements the group of scoring functions.
+        Group:
+        "MI" - Mutual Information,
+        "LL" - Log Likelihood,
+        "BIC" - Bayess Information Criteria,
+        "AIC" - Akaike information Criteria.
+        """
         column_name_dict = dict([(n.name, i)
-                                for i, n in enumerate(self.vertices)])
+                                 for i, n in enumerate(self.vertices)])
         blacklist_new = []
         for pair in self.black_list:
             blacklist_new.append(
                 (column_name_dict[pair[0]], column_name_dict[pair[1]]))
         if white_list:
             white_list_old = white_list[:]
             white_list = []
```

### Comparing `BAMT-1.1.33/bamt/config.py` & `BAMT-1.1.40/bamt/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 CONFIGFILE = path.join(path.dirname(path.abspath(__file__)), 'selbst.ini')
 
 if path.isfile(CONFIGFILE) and stat(CONFIGFILE).st_size != 0:
     config.read(CONFIGFILE)
 else:
     open(CONFIGFILE, 'a').close()
-    # config['NODES'] = {'models_storage': path.join(path.dirname(path.abspath(__file__)), 'Nodes_data')}
     config['NODES'] = {
         'models_storage': path.join(
             path.expanduser("~"),
             'BAMT',
             'Nodes_data')}
     config['LOG'] = {
         "log_conf_loc": path.join(
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/classes/_tests/__pycache__/test_bayesnet.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/classes/_tests/__pycache__/test_bayesnet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.33/bamt/external/pyBN/classes/_tests/__pycache__/test_factor.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/classes/_tests/__pycache__/test_factor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.33/bamt/external/pyBN/classes/bayesnet.py` & `BAMT-1.1.40/bamt/external/pyBN/classes/bayesnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,63 +26,64 @@
     - E -
         key:
             - rv -
         values:
             - list of rv's children -
 Notes
 -----
-- Edges can be inferred from Factorization, but Vertex values 
+- Edges can be inferred from Factorization, but Vertex values
     must be specified.
 """
 
 __author__ = """Nicholas Cullen <ncullen.th@dartmouth.edu>"""
 
-from copy import copy, deepcopy
+from copy import deepcopy
 
 import numpy as np
 from bamt.external.pyBN.utils.class_equivalence import are_class_equivalent
 from bamt.external.pyBN.utils.graph import topsort
 
+
 class BayesNet(object):
     """
     Overarching class for Bayesian Networks
 
     """
 
     def __init__(self, E=None, value_dict=None, file=None):
         """
         Initialize the BayesNet class.
 
         Arguments
         ---------
         *V* : a list of strings - vertices in topsort order
         *E* : a dict, where key = vertex, val = list of its children
-        *F* : a dict, 
-            where key = rv, 
+        *F* : a dict,
+            where key = rv,
             val = another dict with
-                keys = 
-                    'parents', 
-                    'values', 
+                keys =
+                    'parents',
+                    'values',
                     'cpt'
 
-        *V* : a dict        
+        *V* : a dict
 
         Notes
         -----
-        
+
         """
         if file is not None:
             import pyBN.io.read as ior
             bn = ior.read_bn(file)
             self.V = bn.V
             self.E = bn.E
-            self.F = bn.F        
+            self.F = bn.F
         else:
             if E is not None:
-                #assert (value_dict is not None), 'Must set values if E is set.'
+                # assert (value_dict is not None), 'Must set values if E is set.'
                 self.set_structure(E, value_dict)
             else:
                 self.V = []
                 self.E = {}
                 self.F = {}
 
     def __eq__(self, y):
@@ -95,15 +96,15 @@
         return are_class_equivalent(self, y)
 
     def __hash__(self):
         """
         Allows BayesNet objects to be used
         as keys in a dictionary (i.e. hashable)
         """
-        return hash((str(self.V),str(self.E)))
+        return hash((str(self.V), str(self.E)))
 
     def copy(self):
         V = deepcopy(self.V)
         E = deepcopy(self.E)
         F = {}
         for v in V:
             F[v] = {}
@@ -115,36 +116,35 @@
         bn.E = E
         bn.F = F
 
         return bn
 
     def add_node(self, rv, cpt=[], parents=[], values=[]):
         self.V.append(rv)
-        self.F[rv] = {'cpt':cpt,'parents':parents,'values':values}
+        self.F[rv] = {'cpt': cpt, 'parents': parents, 'values': values}
 
     def add_edge(self, u, v):
         if not self.has_node(u):
             self.add_node(u)
         if not self.has_node(v):
             self.add_node(v)
-        if self.has_edge(u,v):
+        if self.has_edge(u, v):
             print('Edge already exists')
         else:
             self.E[u].append(v)
             self.F[v]['parents'].append(u)
-        #self.V = topsort(self.E)
+        # self.V = topsort(self.E)
         # HOW DO I RECALCULATE CPT?
 
-
     def remove_edge(self, u, v):
         self.E[u].remove(v)
         self.F[v]['parents'].remove(u)
 
     def reverse_arc(self, u, v):
-        if self.has_edge(u,v):
+        if self.has_edge(u, v):
             self.E[u].remove(v)
             self.E[v].append(u)
 
     def set_data(self, rv, data):
         assert (isinstance(data, dict)), 'data must be dictionary'
         self.F[rv] = data
 
@@ -172,29 +172,30 @@
 
     def has_edge(self, u, v):
         return v in self.E[u]
 
     def edges(self):
         for u in self.nodes():
             for v in self.E[u]:
-                yield (u,v)
+                yield (u, v)
+
     def num_edges(self):
         num = 0
         for u in self.nodes():
             num += len(self.E[u])
         return num
 
     def num_params(self):
         num = 0
         for u in self.nodes():
             num += len(self.F[u]['cpt'])
         return num
 
     def scope_size(self, rv):
-        return len(self.F[rv]['parents'])+1
+        return len(self.F[rv]['parents']) + 1
 
     def num_nodes(self):
         return len(self.V)
 
     def cpt(self, rv):
         return self.F[rv]['cpt']
 
@@ -215,22 +216,22 @@
     def degree(self, rv):
         return len(self.parents(rv)) + len(self.children(rv))
 
     def values(self, rv):
         return self.F[rv]['values']
 
     def value_idx(self, rv, val):
-        try:   
+        try:
             return self.F[rv]['values'].index(val)
         except ValueError:
             print("Value Index Error")
             return -1
 
     def stride(self, rv, n):
-        if n==rv:
+        if n == rv:
             return 1
         else:
             card_list = [self.card(rv)]
             card_list.extend([self.card(p) for p in self.parents(rv)])
             n_idx = self.parents(rv).index(n) + 1
             return int(np.prod(card_list[0:n_idx]))
 
@@ -238,17 +239,19 @@
         """
         Return all cpt values in the BN as a flattened
         numpy array ordered by bn.nodes() - i.e. topsort
         """
         if by_var:
             cpt = np.array([sum(self.cpt(rv)) for rv in self.nodes()])
         elif by_parents:
-            cpt = np.array([sum(self.cpt(rv)[i:(i+self.card(rv))]) for rv in self.nodes() for i in range(len(self.cpt(rv))/self.card(rv))])
+            cpt = np.array([sum(self.cpt(rv)[i:(i + self.card(rv))])
+                           for rv in self.nodes() for i in range(len(self.cpt(rv)) / self.card(rv))])
         else:
-            cpt = np.array([val for rv in self.nodes() for val in self.cpt(rv)])
+            cpt = np.array([val for rv in self.nodes()
+                           for val in self.cpt(rv)])
         return cpt
 
     def cpt_indices(self, target, val_dict):
         """
         Get the index of the CPT which corresponds
         to a dictionary of rv=val sets. This can be
         used for parameter learning to increment the
@@ -263,51 +266,50 @@
         *target* : a string
             Main RV
 
         *val_dict* : a dictionary, where
             key=rv,val=rv value
 
         """
-        stride = dict([(n,self.stride(target,n)) for n in self.scope(target)])
-        #if len(val_dict)==len(self.parents(target)):
+        stride = dict([(n, self.stride(target, n))
+                      for n in self.scope(target)])
+        # if len(val_dict)==len(self.parents(target)):
         #    idx = sum([self.value_idx(rv,val)*stride[rv] \
         #            for rv,val in val_dict.items()])
-        #else:
+        # else:
         card = dict([(n, self.card(n)) for n in self.scope(target)])
         idx = set(range(len(self.cpt(target))))
         for rv, val in val_dict.items():
-            val_idx = self.value_idx(rv,val)
+            val_idx = self.value_idx(rv, val)
             rv_idx = []
-            s_idx = val_idx*stride[rv]
+            s_idx = val_idx * stride[rv]
             while s_idx < len(self.cpt(target)):
-                rv_idx.extend(range(s_idx,(s_idx+stride[rv])))
-                s_idx += stride[rv]*card[rv]
+                rv_idx.extend(range(s_idx, (s_idx + stride[rv])))
+                s_idx += stride[rv] * card[rv]
             idx = idx.intersection(set(rv_idx))
 
         return list(idx)
 
     def cpt_str_idx(self, rv, idx):
         """
         Return string representation of RV=VAL and
         Parents=Val for the given idx of the given rv's cpt.
         """
         rv_val = self.values(rv)[idx % self.card(rv)]
-        s = str(rv)+'='+str(rv_val) + '|'
-        _idx=1
+        s = str(rv) + '=' + str(rv_val) + '|'
+        _idx = 1
         for parent in self.parents(rv):
             for val in self.values(parent):
-                if idx in self.cpt_indices(rv,{rv:rv_val,parent:val}):
-                    s += str(parent)+'='+str(val)
+                if idx in self.cpt_indices(rv, {rv: rv_val, parent: val}):
+                    s += str(parent) + '=' + str(val)
                     if _idx < len(self.parents(rv)):
                         s += ','
-                    _idx+=1
+                    _idx += 1
         return s
 
-
-
     def set_structure(self, edge_dict, value_dict=None):
         """
         Set the structure of a BayesNet object. This
         function is mostly used to instantiate a BN
         skeleton after structure learning algorithms.
 
         See "structure_learn" folder & algorithms
@@ -336,33 +338,33 @@
         Notes
         -----
 
         """
 
         self.V = topsort(edge_dict)
         self.E = edge_dict
-        self.F = dict([(rv,{}) for rv in self.nodes()])
+        self.F = dict([(rv, {}) for rv in self.nodes()])
         for rv in self.nodes():
             self.F[rv] = {
-                'parents':[p for p in self.nodes() if rv in self.children(p)],
+                'parents': [p for p in self.nodes() if rv in self.children(p)],
                 'cpt': [],
                 'values': []
             }
             if value_dict is not None:
                 self.F[rv]['values'] = value_dict[rv]
 
     def adj_list(self):
         """
         Returns adjacency list of lists, where
         each list element is a vertex, and each sub-list is
         a list of that vertex's neighbors.
         """
         adj_list = [[] for _ in self.V]
-        vi_map = dict((self.V[i],i) for i in range(len(self.V)))
-        for u,v in self.edges():
+        vi_map = dict((self.V[i], i) for i in range(len(self.V)))
+        for u, v in self.edges():
             adj_list[vi_map[u]].append(vi_map[v])
         return adj_list
 
     def moralized_edges(self):
         """
         Moralized graph is the original graph PLUS
         an edge between every set of common effect
@@ -375,18 +377,12 @@
         -------
         *e* : a python list of parent-child tuples.
 
         """
         e = set()
         for u in self.nodes():
             for p1 in self.parents(u):
-                e.add((p1,u))
+                e.add((p1, u))
                 for p2 in self.parents(u):
-                    if p1!=p2 and (p2,p1) not in e:
-                        e.add((p1,p2))
+                    if p1 != p2 and (p2, p1) not in e:
+                        e.add((p1, p2))
         return list(e)
-
-
-    
-
-
-
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/classes/cliquetree.py` & `BAMT-1.1.40/bamt/external/pyBN/classes/__pycache__/cliquetree.cpython-310.pyc`

 * *Files 27% similar despite different names*

```diff
@@ -1,740 +1,674 @@
-00000000: 2222 220d 0a2a 2a2a 2a2a 2a2a 2a2a 2a2a  """..***********
-00000010: 2a2a 2a2a 2a2a 2a0d 0a43 6c69 7175 6554  *******..CliqueT
-00000020: 7265 6520 436c 6173 7320 0d0a 260d 0a43  ree Class ..&..C
-00000030: 6c69 7175 6520 436c 6173 730d 0a2a 2a2a  lique Class..***
-00000040: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a0d  ***************.
-00000050: 0a0d 0a54 6869 7320 6973 2061 2063 6c61  ...This is a cla
-00000060: 7373 2066 6f72 2063 7265 6174 696e 672f  ss for creating/
-00000070: 6d61 6e69 7075 6c61 7469 6e67 204a 756e  manipulating Jun
-00000080: 6374 696f 6e20 2843 6c69 7175 6529 2054  ction (Clique) T
-00000090: 7265 6573 2c0d 0a61 6e64 2070 6572 666f  rees,..and perfo
-000000a0: 726d 696e 6720 696e 6665 7265 6e63 6520  rming inference 
-000000b0: 6f76 6572 2074 6865 6d2e 2054 6865 2061  over them. The a
-000000c0: 6476 616e 7461 6765 206f 6620 636c 6971  dvantage of cliq
-000000d0: 7565 2074 7265 6573 0d0a 6f76 6572 2074  ue trees..over t
-000000e0: 7261 6469 7469 6f6e 616c 2076 6172 6961  raditional varia
-000000f0: 626c 6520 656c 696d 696e 6174 696f 6e20  ble elimination 
-00000100: 6f76 6572 2074 6865 206f 7269 6769 6e61  over the origina
-00000110: 6c20 4261 7965 7369 616e 200d 0a6e 6574  l Bayesian ..net
-00000120: 776f 726b 2069 7320 7468 6174 2063 6c69  work is that cli
-00000130: 7175 6520 7472 6565 7320 616c 6c6f 7720  que trees allow 
-00000140: 796f 7520 746f 2063 6f6d 7075 7465 206d  you to compute m
-00000150: 6172 6769 6e61 6c0d 0a70 726f 6261 6269  arginal..probabi
-00000160: 6c69 7469 6573 206f 6620 4d55 4c54 4950  lities of MULTIP
-00000170: 4c45 2076 6172 6961 626c 6573 2077 6974  LE variables wit
-00000180: 686f 7574 2068 6176 696e 6720 746f 2072  hout having to r
-00000190: 756e 2074 6865 0d0a 656e 7469 7265 2061  un the..entire a
-000001a0: 6c67 6f72 6974 686d 206f 7665 722e 200d  lgorithm over. .
-000001b0: 0a0d 0a54 6865 7265 666f 7265 2c20 6966  ...Therefore, if
-000001c0: 2079 6f75 2068 6176 6520 746f 2071 7565   you have to que
-000001d0: 7279 2074 6865 2042 6179 6573 6961 6e20  ry the Bayesian 
-000001e0: 6e65 7477 6f72 6b20 6d61 6e79 2074 696d  network many tim
-000001f0: 6573 200d 0a2d 2d20 616e 6420 796f 7520  es ..-- and you 
-00000200: 7761 6e74 2074 6865 2065 7861 6374 206d  want the exact m
-00000210: 6172 6769 6e61 6c20 7661 6c75 6573 202d  arginal values -
-00000220: 2d20 7468 656e 2069 7420 6d69 6768 7420  - then it might 
-00000230: 6265 200d 0a62 6573 7420 746f 2075 7365  be ..best to use
-00000240: 2074 6865 2063 6c69 7175 6520 7472 6565   the clique tree
-00000250: 2064 6174 6120 7374 7275 6374 7572 6520   data structure 
-00000260: 666f 7220 696e 6665 7265 6e63 652e 0d0a  for inference...
-00000270: 4966 2079 6f75 206e 6565 6420 746f 2063  If you need to c
-00000280: 6f6d 7075 7465 2074 6865 206d 6172 6769  ompute the margi
-00000290: 6e61 6c20 6469 7374 7269 6275 7469 6f6e  nal distribution
-000002a0: 2066 6f72 2061 6c6c 2076 6172 6961 626c   for all variabl
-000002b0: 6573 2c0d 0a62 7574 2079 6f75 2064 6f6e  es,..but you don
-000002c0: 7420 6d69 6e64 2061 6e20 6170 7072 6f78  t mind an approx
-000002d0: 696d 6174 652c 2061 2073 616d 706c 696e  imate, a samplin
-000002e0: 6720 616c 676f 7269 7468 6d20 6973 2070  g algorithm is p
-000002f0: 726f 6261 626c 790d 0a74 6865 2077 6179  robably..the way
-00000300: 2074 6f20 676f 2e0d 0a0d 0a49 6e20 6765   to go.....In ge
-00000310: 6e65 7261 6c2c 2074 6865 206a 756e 6374  neral, the junct
-00000320: 696f 6e20 7472 6565 2061 6c67 6f72 6974  ion tree algorit
-00000330: 686d 7320 6765 6e65 7261 6c69 7a65 200d  hms generalize .
-00000340: 0a56 6172 6961 626c 6520 456c 696d 696e  .Variable Elimin
-00000350: 6174 696f 6e20 746f 2074 6865 2065 6666  ation to the eff
-00000360: 6963 6965 6e74 2c20 7369 6d75 6c74 616e  icient, simultan
-00000370: 656f 7573 2065 7865 6375 7469 6f6e 200d  eous execution .
-00000380: 0a6f 6620 6120 6c61 7267 6520 636c 6173  .of a large clas
-00000390: 7320 6f66 2071 7565 7269 6573 2e0d 0a0d  s of queries....
-000003a0: 0a4e 4f54 453a 2041 2063 6c75 7374 6572  .NOTE: A cluster
-000003b0: 2067 7261 7068 2069 7320 6120 6765 6e65   graph is a gene
-000003c0: 7261 6c69 7a61 7469 6f6e 206f 6620 7468  ralization of th
-000003d0: 6520 636c 6971 7565 2074 7265 650d 0a64  e clique tree..d
-000003e0: 6174 6120 7374 7275 6374 7572 6520 2d20  ata structure - 
-000003f0: 746f 2067 656e 6572 6174 6520 6120 636c  to generate a cl
-00000400: 6971 7565 2074 7265 652c 2079 6f75 2066  ique tree, you f
-00000410: 6972 7374 2067 656e 6572 6174 650d 0a61  irst generate..a
-00000420: 2063 6c75 7374 6572 2067 7261 7068 2c20   cluster graph, 
-00000430: 7468 656e 2073 696d 706c 7920 6361 6c63  then simply calc
-00000440: 756c 6174 6520 6120 6d61 7869 6d75 6d20  ulate a maximum 
-00000450: 7370 616e 6e69 6e67 2074 7265 652e 0d0a  spanning tree...
-00000460: 496e 206f 7468 6572 2077 6f72 6473 2c20  In other words, 
-00000470: 6120 636c 6971 7565 2074 7265 6520 6361  a clique tree ca
-00000480: 6e20 6265 2063 6f6e 7369 6465 7265 6420  n be considered 
-00000490: 6173 2061 2073 7065 6369 616c 0d0a 7479  as a special..ty
-000004a0: 7065 206f 6620 636c 7573 7465 7220 6772  pe of cluster gr
-000004b0: 6170 682e 0d0a 0d0a 2222 220d 0a0d 0a5f  aph....."""...._
-000004c0: 5f61 7574 686f 725f 5f20 3d20 2222 224e  _author__ = """N
-000004d0: 6963 686f 6c61 7320 4375 6c6c 656e 203c  icholas Cullen <
-000004e0: 6e63 756c 6c65 6e2e 7468 4064 6172 746d  ncullen.th@dartm
-000004f0: 6f75 7468 2e65 6475 3e22 2222 0d0a 0d0a  outh.edu>"""....
-00000500: 696d 706f 7274 206e 6574 776f 726b 7820  import networkx 
-00000510: 6173 206e 780d 0a66 726f 6d20 636f 7079  as nx..from copy
-00000520: 2069 6d70 6f72 7420 636f 7079 0d0a 0d0a   import copy....
-00000530: 6672 6f6d 2062 616d 742e 6578 7465 726e  from bamt.extern
-00000540: 616c 2e70 7942 4e2e 636c 6173 7365 732e  al.pyBN.classes.
-00000550: 6661 6374 6f72 697a 6174 696f 6e20 696d  factorization im
-00000560: 706f 7274 2046 6163 746f 7269 7a61 7469  port Factorizati
-00000570: 6f6e 0d0a 0d0a 6672 6f6d 2062 616d 742e  on....from bamt.
-00000580: 6578 7465 726e 616c 2e70 7942 4e2e 7574  external.pyBN.ut
-00000590: 696c 732e 6772 6170 6820 696d 706f 7274  ils.graph import
-000005a0: 202a 0d0a 0d0a 0d0a 0d0a 636c 6173 7320   *........class 
-000005b0: 436c 6971 7565 5472 6565 286f 626a 6563  CliqueTree(objec
-000005c0: 7429 3a0d 0a20 2020 2022 2222 0d0a 2020  t):..    """..  
-000005d0: 2020 436c 6971 7565 5472 6565 2043 6c61    CliqueTree Cla
-000005e0: 7373 0d0a 0d0a 2020 2020 4c65 7420 4720  ss....    Let G 
-000005f0: 6265 2061 2063 686f 7264 616c 2067 7261  be a chordal gra
-00000600: 7068 2028 6965 2e20 6120 6772 6170 6820  ph (ie. a graph 
-00000610: 7375 6368 2074 6861 7420 6e6f 2063 7963  such that no cyc
-00000620: 6c65 2069 6e63 6c75 6465 7320 6d6f 7265  le includes more
-00000630: 0d0a 2020 2020 7468 616e 2074 6872 6565  ..    than three
-00000640: 206e 6f64 6573 292c 2074 6865 6e20 6120   nodes), then a 
-00000650: 436c 6971 7565 5472 6565 2069 7320 6120  CliqueTree is a 
-00000660: 7472 6565 2048 2073 7563 6820 7468 6174  tree H such that
-00000670: 2065 6163 680d 0a20 2020 206d 6178 696d   each..    maxim
-00000680: 616c 2063 6c69 7175 6520 4320 696e 2047  al clique C in G
-00000690: 2069 7320 6120 6e6f 6465 2069 6e20 482e   is a node in H.
-000006a0: 0d0a 0d0a 2020 2020 4174 7472 6962 7574  ....    Attribut
-000006b0: 6573 0d0a 2020 2020 2d2d 2d2d 2d2d 2d2d  es..    --------
-000006c0: 2d2d 0d0a 2020 2020 2d20 626e 200d 0a20  --..    - bn .. 
-000006d0: 2020 2020 2020 202d 2042 6179 6573 4e65         - BayesNe
-000006e0: 7420 6f62 6a65 6374 0d0a 0d0a 2020 2020  t object....    
-000006f0: 2d20 560d 0a20 2020 2020 2020 202d 2056  - V..        - V
-00000700: 6572 7469 6365 7320 2d3e 206c 6973 740d  ertices -> list.
-00000710: 0a0d 0a20 2020 202d 2045 0d0a 2020 2020  ...    - E..    
-00000720: 2020 2020 2d20 4564 6765 7320 2d3e 2064      - Edges -> d
-00000730: 6963 7469 6f6e 6172 790d 0a0d 0a20 2020  ictionary....   
-00000740: 202d 2043 0d0a 2020 2020 2020 2020 2d20   - C..        - 
-00000750: 436c 6971 7565 7320 2d3e 2061 2064 6963  Cliques -> a dic
-00000760: 7469 6f6e 6172 7920 7768 6572 6520 6b65  tionary where ke
-00000770: 7920 3d20 7665 7274 6578 2069 6478 2c0d  y = vertex idx,.
-00000780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000790: 2076 616c 7565 203d 2043 6c69 7175 6520   value = Clique 
-000007a0: 6f62 6a65 6374 0d0a 0d0a 2020 2020 2222  object....    ""
-000007b0: 220d 0a0d 0a20 2020 2064 6566 205f 5f69  "....    def __i
-000007c0: 6e69 745f 5f28 7365 6c66 2c20 626e 293a  nit__(self, bn):
-000007d0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-000007e0: 2020 2020 2020 2049 6e73 7461 6e74 6961         Instantia
-000007f0: 7465 2061 2043 6c69 7175 6554 7265 6520  te a CliqueTree 
-00000800: 6f62 6a65 6374 2e0d 0a0d 0a20 2020 2020  object.....     
-00000810: 2020 2041 7267 756d 656e 7473 0d0a 2020     Arguments..  
-00000820: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d0d        ---------.
-00000830: 0a20 2020 2020 2020 202a 626e 2a3a 2061  .        *bn*: a
-00000840: 2042 6179 6573 4e65 7420 6f62 6a65 6374   BayesNet object
-00000850: 0d0a 0d0a 2020 2020 2020 2020 4e6f 7465  ....        Note
-00000860: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
-00000870: 0d0a 2020 2020 2020 2020 4964 6561 6c6c  ..        Ideall
-00000880: 792c 2074 6865 2046 6163 746f 7220 636c  y, the Factor cl
-00000890: 6173 7320 7368 6f75 6c64 2062 6520 7573  ass should be us
-000008a0: 6564 2061 7320 7468 650d 0a20 2020 2020  ed as the..     
-000008b0: 2020 2063 6c69 7175 6573 2069 6e73 7465     cliques inste
-000008c0: 6164 206f 6620 7468 6520 436c 6971 7565  ad of the Clique
-000008d0: 2063 6c61 7373 2028 6265 6361 7573 6520   class (because 
-000008e0: 6974 2773 0d0a 2020 2020 2020 2020 6a75  it's..        ju
-000008f0: 7374 2061 2077 6174 6572 6564 2064 6f77  st a watered dow
-00000900: 6e20 7665 7273 696f 6e20 6f66 2074 6865  n version of the
-00000910: 2046 6163 746f 7220 636c 6173 7329 2020   Factor class)  
-00000920: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00000930: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00000940: 2020 2020 2020 2023 2323 230d 0a20 2020         ####..   
-00000950: 2020 2020 2073 656c 662e 5620 3d20 4e6f       self.V = No
-00000960: 6e65 0d0a 2020 2020 2020 2020 7365 6c66  ne..        self
-00000970: 2e45 203d 204e 6f6e 650d 0a20 2020 2020  .E = None..     
-00000980: 2020 2073 656c 662e 4320 3d20 4e6f 6e65     self.C = None
-00000990: 0d0a 2020 2020 2020 2020 2323 230d 0a0d  ..        ###...
-000009a0: 0a20 2020 2020 2020 2073 656c 662e 626e  .        self.bn
-000009b0: 203d 2062 6e0d 0a20 2020 2020 2020 2073   = bn..        s
-000009c0: 656c 662e 5f46 203d 2046 6163 746f 7269  elf._F = Factori
-000009d0: 7a61 7469 6f6e 2862 6e29 0d0a 2020 2020  zation(bn)..    
-000009e0: 2020 2020 7365 6c66 2e69 6e69 7469 616c      self.initial
-000009f0: 697a 655f 7472 6565 2829 0d0a 0d0a 2020  ize_tree()....  
-00000a00: 2020 2020 2020 0d0a 0d0a 2020 2020 2364        ....    #d
-00000a10: 6566 205f 5f72 6570 725f 5f28 7365 6c66  ef __repr__(self
-00000a20: 293a 0d0a 2020 2020 2020 2023 2072 6574  ):..       # ret
-00000a30: 7572 6e20 7365 6c66 2e43 0d0a 0d0a 2020  urn self.C....  
-00000a40: 2020 6465 6620 5f5f 6974 6572 5f5f 2873    def __iter__(s
-00000a50: 656c 6629 3a0d 0a20 2020 2020 2020 2066  elf):..        f
-00000a60: 6f72 2063 6c69 7175 6520 696e 2073 656c  or clique in sel
-00000a70: 662e 432e 7661 6c75 6573 2829 3a0d 0a20  f.C.values():.. 
-00000a80: 2020 2020 2020 2020 2020 2079 6965 6c64             yield
-00000a90: 2063 6c69 7175 650d 0a0d 0a20 2020 2064   clique....    d
-00000aa0: 6566 205f 5f67 6574 6974 656d 5f5f 2873  ef __getitem__(s
-00000ab0: 656c 662c 2072 7629 3a0d 0a20 2020 2020  elf, rv):..     
-00000ac0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00000ad0: 5265 7475 726e 7320 436c 6971 7565 206f  Returns Clique o
-00000ae0: 6620 7061 7373 6564 2d69 6e20 7276 0d0a  f passed-in rv..
-00000af0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00000b00: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00000b10: 2e43 5b72 765d 0d0a 0d0a 2020 2020 6465  .C[rv]....    de
-00000b20: 6620 7061 7265 6e74 7328 7365 6c66 2c20  f parents(self, 
-00000b30: 7629 3a0d 0a20 2020 2020 2020 2070 203d  v):..        p =
-00000b40: 205b 5d0d 0a20 2020 2020 2020 2066 6f72   []..        for
-00000b50: 2072 7620 696e 2073 656c 662e 563a 0d0a   rv in self.V:..
-00000b60: 2020 2020 2020 2020 2020 2020 6966 2076              if v
-00000b70: 2069 6e20 7365 6c66 2e45 5b72 765d 3a0d   in self.E[rv]:.
-00000b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000b90: 2070 2e61 7070 656e 6428 7629 0d0a 2020   p.append(v)..  
-00000ba0: 2020 2020 2020 7265 7475 726e 2070 0d0a        return p..
-00000bb0: 0d0a 2020 2020 6465 6620 6368 696c 6472  ..    def childr
-00000bc0: 656e 2873 656c 662c 206e 293a 0d0a 2020  en(self, n):..  
-00000bd0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00000be0: 662e 455b 6e5d 0d0a 0d0a 2020 2020 6465  f.E[n]....    de
-00000bf0: 6620 6466 735f 706f 7374 6f72 6465 7228  f dfs_postorder(
-00000c00: 7365 6c66 2c20 726f 6f74 293a 0d0a 2020  self, root):..  
-00000c10: 2020 2020 2020 4720 3d20 6e78 2e47 7261        G = nx.Gra
-00000c20: 7068 2873 656c 662e 4529 0d0a 2020 2020  ph(self.E)..    
-00000c30: 2020 2020 7472 6565 5f67 7261 7068 203d      tree_graph =
-00000c40: 206e 782e 6466 735f 7472 6565 2847 2c72   nx.dfs_tree(G,r
-00000c50: 6f6f 7429 0d0a 2020 2020 2020 2020 636c  oot)..        cl
-00000c60: 6971 7565 5f6f 7264 6572 696e 6720 3d20  ique_ordering = 
-00000c70: 6c69 7374 286e 782e 6466 735f 706f 7374  list(nx.dfs_post
-00000c80: 6f72 6465 725f 6e6f 6465 7328 7472 6565  order_nodes(tree
-00000c90: 5f67 7261 7068 2c72 6f6f 7429 290d 0a20  _graph,root)).. 
-00000ca0: 2020 2020 2020 2072 6574 7572 6e20 636c         return cl
-00000cb0: 6971 7565 5f6f 7264 6572 696e 670d 0a0d  ique_ordering...
-00000cc0: 0a20 2020 2064 6566 2069 6e69 7469 616c  .    def initial
-00000cd0: 697a 655f 7472 6565 2873 656c 6629 3a0d  ize_tree(self):.
-00000ce0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00000cf0: 2020 2020 2020 496e 6974 6961 6c69 7a65        Initialize
-00000d00: 2074 6865 2073 7472 7563 7475 7265 206f   the structure o
-00000d10: 6620 6120 636c 6971 7565 2074 7265 652c  f a clique tree,
-00000d20: 2075 7369 6e67 0d0a 2020 2020 2020 2020   using..        
-00000d30: 7468 6520 666f 6c6c 6f77 696e 6720 7374  the following st
-00000d40: 6570 733a 0d0a 2020 2020 2020 2020 2020  eps:..          
-00000d50: 2020 2d20 4d6f 7261 6c69 7a65 2067 7261    - Moralize gra
-00000d60: 7068 2028 692e 652e 206d 6172 7279 2070  ph (i.e. marry p
-00000d70: 6172 656e 7473 290d 0a20 2020 2020 2020  arents)..       
-00000d80: 2020 2020 202d 2054 7269 616e 6775 6c61       - Triangula
-00000d90: 7465 2067 7261 7068 2028 692e 652e 206d  te graph (i.e. m
-00000da0: 616b 6520 6772 6170 6820 6368 6f72 6461  ake graph chorda
-00000db0: 6c29 0d0a 2020 2020 2020 2020 2020 2020  l)..            
-00000dc0: 2d20 4765 7420 6d61 7820 636c 6971 7565  - Get max clique
-00000dd0: 7320 2869 2e65 2e20 636f 6d6d 756e 6974  s (i.e. communit
-00000de0: 792f 636c 6971 7565 2064 6574 6563 7469  y/clique detecti
-00000df0: 6f6e 290d 0a20 2020 2020 2020 2020 2020  on)..           
-00000e00: 202d 204d 6178 2073 7061 6e6e 696e 6720   - Max spanning 
-00000e10: 7472 6565 206f 7665 7220 7365 7073 6574  tree over sepset
-00000e20: 2063 6172 6469 6e61 6c69 7479 2028 692e   cardinality (i.
-00000e30: 652e 2063 7265 6174 6520 7472 6565 290d  e. create tree).
-00000e40: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00000e50: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
-00000e60: 2323 2320 4d4f 5241 4c49 5a45 2047 5241  ### MORALIZE GRA
-00000e70: 5048 2026 204d 414b 4520 4954 2043 484f  PH & MAKE IT CHO
-00000e80: 5244 414c 2023 2323 0d0a 2020 2020 2020  RDAL ###..      
-00000e90: 2020 6368 6f72 6461 6c5f 4720 3d20 6d61    chordal_G = ma
-00000ea0: 6b65 5f63 686f 7264 616c 2873 656c 662e  ke_chordal(self.
-00000eb0: 626e 2920 2320 6d75 7374 2072 6574 7572  bn) # must retur
-00000ec0: 6e20 6120 6e65 7477 6f72 6b78 206f 626a  n a networkx obj
-00000ed0: 6563 740d 0a20 2020 2020 2020 2056 203d  ect..        V =
-00000ee0: 2063 686f 7264 616c 5f47 2e6e 6f64 6573   chordal_G.nodes
-00000ef0: 2829 0d0a 0d0a 2020 2020 2020 2020 2323  ()....        ##
-00000f00: 2320 4745 5420 4d41 5820 434c 4951 5545  # GET MAX CLIQUE
-00000f10: 5320 4652 4f4d 2043 484f 5244 414c 2047  S FROM CHORDAL G
-00000f20: 5241 5048 2023 2323 0d0a 2020 2020 2020  RAPH ###..      
-00000f30: 2020 4320 3d20 7b7d 2023 206b 6579 203d    C = {} # key =
-00000f40: 2076 6572 7465 782c 2076 616c 7565 203d   vertex, value =
-00000f50: 2063 6c69 7175 6520 6f62 6a65 6374 0d0a   clique object..
-00000f60: 2020 2020 2020 2020 6d61 785f 636c 6971          max_cliq
-00000f70: 7565 7320 3d20 7265 7665 7273 6564 286c  ues = reversed(l
-00000f80: 6973 7428 6e78 2e63 686f 7264 616c 5f67  ist(nx.chordal_g
-00000f90: 7261 7068 5f63 6c69 7175 6573 2863 686f  raph_cliques(cho
-00000fa0: 7264 616c 5f47 2929 290d 0a20 2020 2020  rdal_G)))..     
-00000fb0: 2020 2066 6f72 2076 5f69 6478 2c63 6c69     for v_idx,cli
-00000fc0: 7175 6520 696e 2065 6e75 6d65 7261 7465  que in enumerate
-00000fd0: 286d 6178 5f63 6c69 7175 6573 293a 0d0a  (max_cliques):..
-00000fe0: 2020 2020 2020 2020 2020 2020 435b 765f              C[v_
-00000ff0: 6964 785d 203d 2043 6c69 7175 6528 7365  idx] = Clique(se
-00001000: 7428 636c 6971 7565 2929 0d0a 0d0a 2020  t(clique))....  
-00001010: 2020 2020 2020 2323 2320 4d41 5849 4d55        ### MAXIMU
-00001020: 4d20 5350 414e 4e49 4e47 2054 5245 4520  M SPANNING TREE 
-00001030: 4f56 4552 2043 4f4d 504c 4554 4520 4752  OVER COMPLETE GR
-00001040: 4150 4820 544f 204d 414b 4520 4120 5452  APH TO MAKE A TR
-00001050: 4545 2023 2323 0d0a 2020 2020 2020 2020  EE ###..        
-00001060: 7765 6967 6874 6564 5f65 6467 655f 6469  weighted_edge_di
-00001070: 6374 203d 2064 6963 7428 5b28 635f 6964  ct = dict([(c_id
-00001080: 782c 7b7d 2920 666f 7220 635f 6964 7820  x,{}) for c_idx 
-00001090: 696e 2072 616e 6765 286c 656e 2843 2929  in range(len(C))
-000010a0: 5d29 0d0a 2020 2020 2020 2020 666f 7220  ])..        for 
-000010b0: 6920 696e 2072 616e 6765 286c 656e 2843  i in range(len(C
-000010c0: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-000010d0: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
-000010e0: 6c65 6e28 4329 293a 0d0a 2020 2020 2020  len(C)):..      
-000010f0: 2020 2020 2020 2020 2020 6966 2069 213d            if i!=
-00001100: 6a3a 0d0a 2020 2020 2020 2020 2020 2020  j:..            
-00001110: 2020 2020 2020 2020 696e 7465 7273 6563          intersec
-00001120: 745f 6361 7264 696e 616c 6974 7920 3d20  t_cardinality = 
-00001130: 6c65 6e28 435b 695d 2e73 6570 7365 7428  len(C[i].sepset(
-00001140: 435b 6a5d 2929 0d0a 2020 2020 2020 2020  C[j]))..        
-00001150: 2020 2020 2020 2020 2020 2020 7765 6967              weig
-00001160: 6874 6564 5f65 6467 655f 6469 6374 5b69  hted_edge_dict[i
-00001170: 5d5b 6a5d 203d 202d 312a 696e 7465 7273  ][j] = -1*inters
-00001180: 6563 745f 6361 7264 696e 616c 6974 790d  ect_cardinality.
-00001190: 0a20 2020 2020 2020 206d 7374 5f47 203d  .        mst_G =
-000011a0: 206d 7374 2877 6569 6768 7465 645f 6564   mst(weighted_ed
-000011b0: 6765 5f64 6963 7429 0d0a 2020 2020 2020  ge_dict)..      
-000011c0: 2020 2323 2320 5345 5420 562c 452c 4320    ### SET V,E,C 
-000011d0: 2323 230d 0a20 2020 2020 2020 2073 656c  ###..        sel
-000011e0: 662e 4520 3d20 6d73 745f 4720 2320 6469  f.E = mst_G # di
-000011f0: 6374 696f 6e61 7279 0d0a 2020 2020 2020  ctionary..      
-00001200: 2020 7365 6c66 2e56 203d 206d 7374 5f47    self.V = mst_G
-00001210: 2e6b 6579 7328 2920 2320 6c69 7374 0d0a  .keys() # list..
-00001220: 2020 2020 2020 2020 7365 6c66 2e43 203d          self.C =
-00001230: 2043 0d0a 0d0a 2020 2020 2020 2020 0d0a   C....        ..
-00001240: 2020 2020 2020 2020 2323 2320 4153 5349          ### ASSI
-00001250: 474e 2045 4143 4820 4641 4354 4f52 2054  GN EACH FACTOR T
-00001260: 4f20 4f4e 4520 434c 4951 5545 204f 4e4c  O ONE CLIQUE ONL
-00001270: 5920 2323 230d 0a20 2020 2020 2020 2076  Y ###..        v
-00001280: 5f61 203d 2064 6963 7428 5b28 7276 2c20  _a = dict([(rv, 
-00001290: 4661 6c73 6529 2066 6f72 2072 7620 696e  False) for rv in
-000012a0: 2073 656c 662e 626e 2e6e 6f64 6573 2829   self.bn.nodes()
-000012b0: 5d29 0d0a 2020 2020 2020 2020 666f 7220  ])..        for 
-000012c0: 636c 6971 7565 2069 6e20 7365 6c66 2e43  clique in self.C
-000012d0: 2e76 616c 7565 7328 293a 0d0a 2020 2020  .values():..    
-000012e0: 2020 2020 2020 2020 7465 6d70 5f73 636f          temp_sco
-000012f0: 7065 203d 205b 5d0d 0a20 2020 2020 2020  pe = []..       
-00001300: 2020 2020 2066 6f72 2076 6172 2069 6e20       for var in 
-00001310: 765f 613a 0d0a 2020 2020 2020 2020 2020  v_a:..          
-00001320: 2020 2020 2020 6966 2076 5f61 5b76 6172        if v_a[var
-00001330: 5d20 3d3d 2046 616c 7365 2061 6e64 2073  ] == False and s
-00001340: 6574 2873 656c 662e 626e 2e73 636f 7065  et(self.bn.scope
-00001350: 2876 6172 2929 2e69 7373 7562 7365 7428  (var)).issubset(
-00001360: 636c 6971 7565 2e73 636f 7065 293a 0d0a  clique.scope):..
-00001370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001380: 2020 2020 7465 6d70 5f73 636f 7065 2e61      temp_scope.a
-00001390: 7070 656e 6428 7661 7229 0d0a 2020 2020  ppend(var)..    
-000013a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013b0: 765f 615b 7661 725d 203d 2054 7275 650d  v_a[var] = True.
-000013c0: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
-000013d0: 7175 652e 5f46 203d 2046 6163 746f 7269  que._F = Factori
-000013e0: 7a61 7469 6f6e 2873 656c 662e 626e 2c20  zation(self.bn, 
-000013f0: 7465 6d70 5f73 636f 7065 290d 0a0d 0a20  temp_scope).... 
-00001400: 2020 2020 2020 2023 2323 2043 4f4d 5055         ### COMPU
-00001410: 5445 2049 4e49 5449 414c 2050 4f54 454e  TE INITIAL POTEN
-00001420: 5449 414c 2046 4f52 2045 4143 4820 4641  TIAL FOR EACH FA
-00001430: 4354 4f52 2023 2323 0d0a 2020 2020 2020  CTOR ###..      
-00001440: 2020 2320 2d20 692e 652e 206d 756c 7469    # - i.e. multi
-00001450: 706c 7920 616c 6c20 6f66 2069 7473 2061  ply all of its a
-00001460: 7373 6967 6e65 6420 6661 6374 6f72 7320  ssigned factors 
-00001470: 746f 6765 7468 6572 0d0a 2020 2020 2020  together..      
-00001480: 2020 666f 7220 692c 2063 6c69 7175 6520    for i, clique 
-00001490: 696e 2073 656c 662e 432e 6974 656d 7328  in self.C.items(
-000014a0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000014b0: 6966 206c 656e 2873 656c 662e 7061 7265  if len(self.pare
-000014c0: 6e74 7328 6929 2920 3d3d 2030 3a0d 0a20  nts(i)) == 0:.. 
-000014d0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000014e0: 6c69 7175 652e 6973 5f72 6561 6479 203d  lique.is_ready =
-000014f0: 2054 7275 650d 0a20 2020 2020 2020 2020   True..         
-00001500: 2020 2063 6c69 7175 652e 696e 6974 6961     clique.initia
-00001510: 6c69 7a65 5f70 7369 2829 0d0a 0d0a 0d0a  lize_psi()......
-00001520: 636c 6173 7320 436c 6971 7565 286f 626a  class Clique(obj
-00001530: 6563 7429 3a0d 0a20 2020 2022 2222 0d0a  ect):..    """..
-00001540: 2020 2020 436c 6971 7565 2043 6c61 7373      Clique Class
-00001550: 0d0a 0d0a 2020 2020 2a73 636f 7065 2a20  ....    *scope* 
-00001560: 3a20 6120 7365 7420 6f66 2076 6172 6961  : a set of varia
-00001570: 626c 6573 2069 6e20 7468 6520 636c 6971  bles in the cliq
-00001580: 7565 2773 2073 636f 7065 0d0a 0d0a 2020  ue's scope....  
-00001590: 2020 2a5f 662a 203a 2061 2066 6163 746f    *_f* : a facto
-000015a0: 7269 7a61 7469 6f6e 206f 626a 6563 7420  rization object 
-000015b0: 7468 6174 2063 6f6e 7461 696e 7320 6f6e  that contains on
-000015c0: 6c79 2074 6865 0d0a 2020 2020 2020 2020  ly the..        
-000015d0: 6661 6374 6f72 7320 6f66 2076 6172 6961  factors of varia
-000015e0: 626c 6573 2069 6e20 7468 6520 636c 6971  bles in the cliq
-000015f0: 7565 2773 2073 636f 7065 0d0a 0d0a 2020  ue's scope....  
-00001600: 2020 2a70 7369 2a20 3a20 6120 6661 6374    *psi* : a fact
-00001610: 6f72 0d0a 2020 2020 2020 2020 5468 6520  or..        The 
-00001620: 706f 7465 6e74 6961 6c20 6f66 2074 6865  potential of the
-00001630: 2063 6c69 7175 652e 0d0a 0d0a 2020 2020   clique.....    
-00001640: 2a62 656c 6965 662a 203a 2061 2066 6163  *belief* : a fac
-00001650: 746f 720d 0a20 2020 2020 2020 2054 6865  tor..        The
-00001660: 2066 6163 746f 7220 7768 6963 6820 686f   factor which ho
-00001670: 6c64 7320 7468 6520 6d61 7267 696e 616c  lds the marginal
-00001680: 2f63 6f6e 6469 7469 6f6e 616c 0d0a 2020  /conditional..  
-00001690: 2020 2020 2020 7072 6f62 6162 696c 6974        probabilit
-000016a0: 6965 7320 6f66 2074 6865 2072 656c 6576  ies of the relev
-000016b0: 616e 7420 6e6f 6465 7320 6166 7465 7220  ant nodes after 
-000016c0: 0d0a 2020 2020 2020 2020 6265 6c69 6566  ..        belief
-000016d0: 2070 726f 7061 6761 7469 6f6e 2c20 6574   propagation, et
-000016e0: 630d 0a0d 0a20 2020 202a 6d65 7373 6167  c....    *messag
-000016f0: 6573 5f72 6563 6569 7665 642a 203a 2061  es_received* : a
-00001700: 206c 6973 7420 6f66 2046 6163 746f 7273   list of Factors
-00001710: 0d0a 2020 2020 2020 2020 5468 6520 6d65  ..        The me
-00001720: 7373 6167 6573 2074 6865 2063 6c69 7175  ssages the cliqu
-00001730: 6520 6861 7320 7265 6365 6976 6564 2066  e has received f
-00001740: 726f 6d20 6974 7320 6e65 6967 6862 6f72  rom its neighbor
-00001750: 7320 2d0d 0a20 2020 2020 2020 2073 746f  s -..        sto
-00001760: 7265 6420 736f 2074 6861 7420 7468 6520  red so that the 
-00001770: 6265 6c69 6566 7320 6361 6e20 6265 2063  beliefs can be c
-00001780: 616c 6375 6c61 7465 6420 6166 7465 720d  alculated after.
-00001790: 0a20 2020 2020 2020 2062 656c 6965 6620  .        belief 
-000017a0: 7072 6f70 6167 6174 696f 6e2c 2065 7463  propagation, etc
-000017b0: 2e0d 0a0d 0a20 2020 202a 6973 5f72 6561  .....    *is_rea
-000017c0: 6479 2a20 3a20 6120 626f 6f6c 6561 6e0d  dy* : a boolean.
-000017d0: 0a20 2020 2020 2020 2057 6865 7468 6572  .        Whether
-000017e0: 2074 6865 2063 6c69 7175 6520 6973 2072   the clique is r
-000017f0: 6561 6479 2074 6f20 7365 6e64 2061 206d  eady to send a m
-00001800: 6573 7361 6765 202d 3e20 6d75 7374 0d0a  essage -> must..
-00001810: 2020 2020 2020 2020 6861 7665 2052 4543          have REC
-00001820: 4549 5645 4420 6d65 7373 6167 6573 2066  EIVED messages f
-00001830: 726f 6d20 616c 6c20 6f66 2069 7473 206e  rom all of its n
-00001840: 6569 6768 626f 7273 2066 6972 7374 2e0d  eighbors first..
-00001850: 0a0d 0a20 2020 2022 2222 0d0a 0d0a 2020  ...    """....  
-00001860: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00001870: 656c 662c 2073 636f 7065 293a 0d0a 2020  elf, scope):..  
-00001880: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00001890: 2020 2049 6e73 7461 6e74 6961 7465 2061     Instantiate a
-000018a0: 2063 6c69 7175 6520 6f62 6a65 6374 0d0a   clique object..
-000018b0: 0d0a 2020 2020 2020 2020 4172 6775 6d65  ..        Argume
-000018c0: 6e74 730d 0a20 2020 2020 2020 202d 2d2d  nts..        ---
-000018d0: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
-000018e0: 2a73 636f 7065 2a20 3a20 6120 7079 7468  *scope* : a pyth
-000018f0: 6f6e 2073 6574 0d0a 2020 2020 2020 2020  on set..        
-00001900: 2020 2020 5468 6520 7365 7420 6f66 2076      The set of v
-00001910: 6172 6961 626c 6573 2069 6e20 7468 6520  ariables in the 
-00001920: 636c 6971 7565 7320 7363 6f70 652c 0d0a  cliques scope,..
-00001930: 2020 2020 2020 2020 2020 2020 692e 652e              i.e.
-00001940: 2074 6865 206d 6169 6e20 7661 7220 616e   the main var an
-00001950: 6420 6974 7320 7061 7265 6e74 730d 0a0d  d its parents...
-00001960: 0a0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
-00001970: 2020 2020 2020 2020 7365 6c66 2e73 636f          self.sco
-00001980: 7065 203d 2073 636f 7065 0d0a 2020 2020  pe = scope..    
-00001990: 2020 2020 7365 6c66 2e5f 4620 3d20 4e6f      self._F = No
-000019a0: 6e65 0d0a 2020 2020 2020 2020 0d0a 2020  ne..        ..  
-000019b0: 2020 2020 2020 7365 6c66 2e70 7369 203d        self.psi =
-000019c0: 204e 6f6e 6520 2320 5073 6920 7368 6f75   None # Psi shou
-000019d0: 6c64 206e 6576 6572 2063 6861 6e67 6520  ld never change 
-000019e0: 2d3e 2046 6163 746f 7220 6f62 6a65 6374  -> Factor object
-000019f0: 0d0a 2020 2020 2020 2020 7365 6c66 2e62  ..        self.b
-00001a00: 656c 6965 6620 3d20 4e6f 6e65 0d0a 2020  elief = None..  
-00001a10: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00001a20: 7365 6c66 2e6d 6573 7361 6765 735f 7265  self.messages_re
-00001a30: 6365 6976 6564 203d 205b 5d0d 0a20 2020  ceived = []..   
-00001a40: 2020 2020 2073 656c 662e 6973 5f72 6561       self.is_rea
-00001a50: 6479 203d 2046 616c 7365 0d0a 0d0a 2020  dy = False....  
-00001a60: 2020 6465 6620 5f5f 7265 7072 5f5f 2873    def __repr__(s
-00001a70: 656c 6629 3a0d 0a20 2020 2020 2020 2072  elf):..        r
-00001a80: 6574 7572 6e20 7374 7228 7365 6c66 2e73  eturn str(self.s
-00001a90: 636f 7065 290d 0a0d 0a20 2020 2064 6566  cope)....    def
-00001aa0: 205f 5f72 7368 6966 745f 5f28 7365 6c66   __rshift__(self
-00001ab0: 2c20 6f74 6865 725f 636c 6971 7565 293a  , other_clique):
-00001ac0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00001ad0: 2020 2020 2020 2053 656e 6420 6120 6d65         Send a me
-00001ae0: 7373 6167 6520 6672 6f6d 2073 656c 6620  ssage from self 
-00001af0: 746f 206f 7468 6572 5f63 6c69 7175 650d  to other_clique.
-00001b00: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00001b10: 2020 2020 2020 7365 6c66 2e73 656e 645f        self.send_
-00001b20: 6d65 7373 6167 6528 6f74 6865 725f 636c  message(other_cl
-00001b30: 6971 7565 290d 0a0d 0a20 2020 2064 6566  ique)....    def
-00001b40: 205f 5f6c 7368 6966 745f 5f28 7365 6c66   __lshift__(self
-00001b50: 2c20 6f74 6865 725f 636c 6971 7565 293a  , other_clique):
-00001b60: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00001b70: 2020 2020 2020 2053 656e 6420 6120 6d65         Send a me
-00001b80: 7373 6167 6520 6672 6f6d 206f 7468 6572  ssage from other
-00001b90: 5f63 6c69 7175 6520 746f 2073 656c 660d  _clique to self.
-00001ba0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00001bb0: 2020 2020 2020 6f74 6865 725f 636c 6971        other_cliq
-00001bc0: 7565 2e73 656e 645f 6d65 7373 6167 6528  ue.send_message(
-00001bd0: 7365 6c66 290d 0a0d 0a20 2020 2064 6566  self)....    def
-00001be0: 2073 656e 645f 6d65 7373 6167 6528 7365   send_message(se
-00001bf0: 6c66 2c20 7061 7265 6e74 293a 0d0a 2020  lf, parent):..  
-00001c00: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00001c10: 2020 2053 656e 6420 6120 6d65 7373 6167     Send a messag
-00001c20: 6520 746f 2074 6865 2070 6172 656e 7420  e to the parent 
-00001c30: 636c 6971 7565 2e0d 0a0d 0a20 2020 2020  clique.....     
-00001c40: 2020 2054 6f20 7365 6e64 2061 206d 6573     To send a mes
-00001c50: 7361 6765 2066 726f 6d20 5820 746f 2059  sage from X to Y
-00001c60: 2c20 796f 750d 0a20 2020 2020 2020 206d  , you..        m
-00001c70: 7573 7420 6669 7273 7420 7461 6b65 2074  ust first take t
-00001c80: 6865 2070 6f74 656e 7469 616c 2028 7365  he potential (se
-00001c90: 6c66 2e70 7369 2920 6f66 0d0a 2020 2020  lf.psi) of..    
-00001ca0: 2020 2020 5820 616e 6420 7375 6d20 6f75      X and sum ou
-00001cb0: 7420 7468 6520 7661 7269 6162 6c65 7320  t the variables 
-00001cc0: 4e4f 5420 696e 2074 6865 2073 6570 7365  NOT in the sepse
-00001cd0: 740d 0a20 2020 2020 2020 206f 6620 592e  t..        of Y.
-00001ce0: 0d0a 0d0a 2020 2020 2020 2020 5448 454e  ....        THEN
-00001cf0: 2c20 6966 2058 2068 6173 2072 6563 6569  , if X has recei
-00001d00: 7665 6420 616e 7920 6d65 7373 6167 6573  ved any messages
-00001d10: 2c20 7468 650d 0a20 2020 2020 2020 2070  , the..        p
-00001d20: 6f74 656e 7469 616c 2028 7365 6c66 2e70  otential (self.p
-00001d30: 7369 2920 6d75 7374 2062 6520 6d75 6c74  si) must be mult
-00001d40: 6970 6c69 6564 2062 790d 0a20 2020 2020  iplied by..     
-00001d50: 2020 2061 6c6c 206f 6620 7468 6520 7265     all of the re
-00001d60: 6365 6976 6564 206d 6573 7361 6765 642e  ceived messaged.
-00001d70: 0d0a 0d0a 2020 2020 2020 2020 4172 6775  ....        Argu
-00001d80: 6d65 6e74 730d 0a20 2020 2020 2020 202d  ments..        -
-00001d90: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
-00001da0: 2020 2a70 6172 656e 742a 203a 2061 2073    *parent* : a s
-00001db0: 7472 696e 670d 0a20 2020 2020 2020 2020  tring..         
-00001dc0: 2020 2054 6865 2070 6172 656e 7420 746f     The parent to
-00001dd0: 2077 6869 6368 2074 6865 206d 6573 7361   which the messa
-00001de0: 6765 2077 696c 6c0d 0a20 2020 2020 2020  ge will..       
-00001df0: 2020 2020 2062 6520 7365 6e74 2e0d 0a0d       be sent....
-00001e00: 0a20 2020 2020 2020 2022 2222 0d0a 0d0a  .        """....
-00001e10: 0d0a 2020 2020 2020 2020 2320 4669 7273  ..        # Firs
-00001e20: 7420 6765 6e65 7261 7465 2042 656c 6965  t generate Belie
-00001e30: 6620 3d20 4f72 6967 696e 616c 5f50 7369  f = Original_Psi
-00001e40: 202a 2061 6c6c 2072 6563 6569 7665 6420   * all received 
-00001e50: 6d65 7373 6167 6573 0d0a 2020 2020 2020  messages..      
-00001e60: 2020 6966 206c 656e 2873 656c 662e 6d65    if len(self.me
-00001e70: 7373 6167 6573 5f72 6563 6569 7665 6429  ssages_received)
-00001e80: 203e 2030 3a0d 0a20 2020 2020 2020 2020   > 0:..         
-00001e90: 2020 2023 2069 6620 7468 6572 6520 6172     # if there ar
-00001ea0: 6520 6d65 7373 6167 6573 2072 6563 6569  e messages recei
-00001eb0: 7665 642c 206d 7574 6c69 706c 7920 7468  ved, mutliply th
-00001ec0: 656d 2069 6e20 746f 2070 7369 2066 6972  em in to psi fir
-00001ed0: 7374 0d0a 2020 2020 2020 2020 2020 2020  st..            
-00001ee0: 6966 206e 6f74 2073 656c 662e 6265 6c69  if not self.beli
-00001ef0: 6566 3a0d 0a20 2020 2020 2020 2020 2020  ef:..           
-00001f00: 2020 2020 2073 656c 662e 6265 6c69 6566       self.belief
-00001f10: 203d 2063 6f70 7928 7365 6c66 2e70 7369   = copy(self.psi
-00001f20: 290d 0a20 2020 2020 2020 2020 2020 2066  )..            f
-00001f30: 6f72 206d 7367 2069 6e20 7365 6c66 2e6d  or msg in self.m
-00001f40: 6573 7361 6765 735f 7265 6365 6976 6564  essages_received
-00001f50: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00001f60: 2020 2073 656c 662e 6265 6c69 6566 202a     self.belief *
-00001f70: 3d20 6d73 670d 0a20 2020 2020 2020 2020  = msg..         
-00001f80: 2020 2023 7365 6c66 2e62 656c 6965 662e     #self.belief.
-00001f90: 6d65 7267 655f 6d75 6c74 6970 6c79 2873  merge_multiply(s
-00001fa0: 656c 662e 6d65 7373 6167 6573 5f72 6563  elf.messages_rec
-00001fb0: 6569 7665 6429 0d0a 2020 2020 2020 2020  eived)..        
-00001fc0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-00001fd0: 2020 2023 2069 6620 7468 6572 6520 6172     # if there ar
-00001fe0: 6520 6e6f 206d 6573 7361 6765 7320 7265  e no messages re
-00001ff0: 6365 6976 6564 2c20 7369 6d70 6c79 206d  ceived, simply m
-00002000: 6f76 6520 6f6e 2077 6974 6820 7073 690d  ove on with psi.
-00002010: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00002020: 6e6f 7420 7365 6c66 2e62 656c 6965 663a  not self.belief:
-00002030: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002040: 2020 7365 6c66 2e62 656c 6965 6620 3d20    self.belief = 
-00002050: 636f 7079 2873 656c 662e 7073 6929 0d0a  copy(self.psi)..
-00002060: 2020 2020 2020 2020 2320 6765 6e65 7261          # genera
-00002070: 7465 206d 6573 7361 6765 2061 7320 6265  te message as be
-00002080: 6c69 6566 2077 6974 6820 4369 202d 2053  lief with Ci - S
-00002090: 696a 2076 6172 7320 7375 6d6d 6564 206f  ij vars summed o
-000020a0: 7574 0d0a 2020 2020 2020 2020 2376 6172  ut..        #var
-000020b0: 735f 746f 5f73 756d 6f75 7420 3d20 6c69  s_to_sumout = li
-000020c0: 7374 2873 656c 662e 7363 6f70 652e 6469  st(self.scope.di
-000020d0: 6666 6572 656e 6365 2873 656c 662e 7365  fference(self.se
-000020e0: 7073 6574 2870 6172 656e 7429 2929 0d0a  pset(parent)))..
-000020f0: 2020 2020 2020 2020 6d73 675f 746f 5f73          msg_to_s
-00002100: 656e 6420 3d20 636f 7079 2873 656c 662e  end = copy(self.
-00002110: 6265 6c69 6566 290d 0a20 2020 2020 2020  belief)..       
-00002120: 2066 6f72 2076 6172 5f74 6f5f 7375 6d6f   for var_to_sumo
-00002130: 7574 2069 6e20 7365 6c66 2e73 636f 7065  ut in self.scope
-00002140: 2e64 6966 6665 7265 6e63 6528 7365 6c66  .difference(self
-00002150: 2e73 6570 7365 7428 7061 7265 6e74 2929  .sepset(parent))
-00002160: 3a0d 0a20 2020 2020 2020 2020 2020 206d  :..            m
-00002170: 7367 5f74 6f5f 7365 6e64 202f 3d20 7661  sg_to_send /= va
-00002180: 725f 746f 5f73 756d 6f75 740d 0a20 2020  r_to_sumout..   
-00002190: 2020 2020 2023 6d65 7373 6167 655f 746f       #message_to
-000021a0: 5f73 656e 6420 3d20 636f 7079 2873 656c  _send = copy(sel
-000021b0: 662e 6265 6c69 6566 290d 0a20 2020 2020  f.belief)..     
-000021c0: 2020 2023 6d65 7373 6167 655f 746f 5f73     #message_to_s
-000021d0: 656e 642e 7375 6d6f 7574 5f76 6172 5f6c  end.sumout_var_l
-000021e0: 6973 7428 7661 7273 5f74 6f5f 7375 6d6f  ist(vars_to_sumo
-000021f0: 7574 290d 0a20 2020 2020 2020 2070 6172  ut)..        par
-00002200: 656e 742e 6d65 7373 6167 6573 5f72 6563  ent.messages_rec
-00002210: 6569 7665 642e 6170 7065 6e64 286d 7367  eived.append(msg
-00002220: 5f74 6f5f 7365 6e64 290d 0a0d 0a20 2020  _to_send)....   
-00002230: 2064 6566 2069 6e69 7469 616c 697a 655f   def initialize_
-00002240: 7073 6928 7365 6c66 293a 0d0a 2020 2020  psi(self):..    
-00002250: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00002260: 2043 6f6d 7075 7465 2061 206e 6577 2070   Compute a new p
-00002270: 7369 2028 6370 7429 2069 6e20 6f72 6465  si (cpt) in orde
-00002280: 7220 746f 200d 0a20 2020 2020 2020 2073  r to ..        s
-00002290: 6574 2074 6865 2063 6c69 7175 6527 7320  et the clique's 
-000022a0: 6265 6c69 6566 2e20 5468 6973 2069 6e76  belief. This inv
-000022b0: 6f6c 7665 730d 0a20 2020 2020 2020 206d  olves..        m
-000022c0: 756c 7469 706c 7969 6e67 2074 6865 2066  ultiplying the f
-000022d0: 6163 746f 7273 2069 6e20 7468 6520 436c  actors in the Cl
-000022e0: 6971 7565 2074 6f67 6574 6865 722e 0d0a  ique together...
-000022f0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00002300: 2020 2020 2061 7373 6572 7420 286c 656e       assert (len
-00002310: 2873 656c 662e 5f46 2920 213d 2030 292c  (self._F) != 0),
-00002320: 2027 4e6f 2046 6163 746f 7273 2061 7373   'No Factors ass
-00002330: 6967 6e65 6420 746f 2074 6869 7320 636c  igned to this cl
-00002340: 6971 7565 2e27 0d0a 0d0a 2020 2020 2020  ique.'....      
-00002350: 2020 6966 206c 656e 2873 656c 662e 5f46    if len(self._F
-00002360: 2920 3d3d 2031 3a0d 0a20 2020 2020 2020  ) == 1:..       
-00002370: 2020 2020 2073 656c 662e 7073 6920 3d20       self.psi = 
-00002380: 636f 7079 2873 656c 662e 5f46 5b30 5d29  copy(self._F[0])
-00002390: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-000023a0: 6c66 2e62 656c 6965 6620 3d20 636f 7079  lf.belief = copy
-000023b0: 2873 656c 662e 7073 6929 0d0a 2020 2020  (self.psi)..    
-000023c0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-000023d0: 2020 2020 2020 2073 656c 662e 7073 6920         self.psi 
-000023e0: 3d20 6d61 7828 7365 6c66 2e5f 462c 206b  = max(self._F, k
-000023f0: 6579 3d6c 616d 6264 6120 783a 206c 656e  ey=lambda x: len
-00002400: 2878 2e63 7074 2929 0d0a 2020 2020 2020  (x.cpt))..      
-00002410: 2020 2020 2020 666f 7220 6620 696e 2073        for f in s
-00002420: 656c 662e 5f46 3a0d 0a20 2020 2020 2020  elf._F:..       
-00002430: 2020 2020 2020 2020 2073 656c 662e 7073           self.ps
-00002440: 6920 2a3d 2066 0d0a 2020 2020 2020 2020  i *= f..        
-00002450: 2020 2020 7365 6c66 2e62 656c 6965 6620      self.belief 
-00002460: 3d20 636f 7079 2873 656c 662e 7073 6929  = copy(self.psi)
-00002470: 0d0a 0d0a 2020 2020 6465 6620 7365 6e64  ....    def send
-00002480: 5f69 6e69 7469 616c 5f6d 6573 7361 6765  _initial_message
-00002490: 2873 656c 662c 206f 7468 6572 5f63 6c69  (self, other_cli
-000024a0: 7175 6529 3a0d 0a20 2020 2020 2020 2022  que):..        "
-000024b0: 2222 0d0a 2020 2020 2020 2020 4e4f 5420  ""..        NOT 
-000024c0: 5355 5245 2049 4620 5448 4953 2049 5320  SURE IF THIS IS 
-000024d0: 4e45 4544 4544 2e0d 0a0d 0a20 2020 2020  NEEDED.....     
-000024e0: 2020 2053 656e 6420 7468 6520 6669 7273     Send the firs
-000024f0: 7420 6d65 7373 6167 6520 746f 2061 6e6f  t message to ano
-00002500: 7468 6572 2063 6c69 7175 652e 0d0a 0d0a  ther clique.....
-00002510: 2020 2020 2020 2020 4172 6775 6d65 6e74          Argument
-00002520: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
-00002530: 2d2d 2d2d 0d0a 2020 2020 2020 2020 2a6f  ----..        *o
-00002540: 7468 6572 5f63 6c69 7175 652a 203a 2061  ther_clique* : a
-00002550: 2064 6966 6665 7265 6e74 2043 6c69 7175   different Cliqu
-00002560: 6520 6f62 6a65 6374 0d0a 0d0a 2020 2020  e object....    
-00002570: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00002580: 2070 7369 5f63 6f70 7920 3d20 636f 7079   psi_copy = copy
-00002590: 2873 656c 662e 7073 6929 0d0a 2020 2020  (self.psi)..    
-000025a0: 2020 2020 7365 7073 6574 203d 2073 656c      sepset = sel
-000025b0: 662e 7365 7073 6574 286f 7468 6572 5f63  f.sepset(other_c
-000025c0: 6c69 7175 6529 0d0a 2020 2020 2020 2020  lique)..        
-000025d0: 7375 6d6f 7574 5f76 6172 7320 3d20 7365  sumout_vars = se
-000025e0: 6c66 2e73 636f 7065 2e64 6966 6665 7265  lf.scope.differe
-000025f0: 6e63 6528 7365 7073 6574 290d 0a20 2020  nce(sepset)..   
-00002600: 2020 2020 2023 2073 756d 206f 7574 2076       # sum out v
-00002610: 6172 6961 626c 6573 206e 6f74 2069 6e20  ariables not in 
-00002620: 7468 6520 7365 7073 6574 206f 6620 6f74  the sepset of ot
-00002630: 6865 725f 636c 6971 7565 0d0a 2020 2020  her_clique..    
-00002640: 2020 2020 7073 695f 636f 7079 2e73 756d      psi_copy.sum
-00002650: 6f75 745f 7661 725f 6c69 7374 286c 6973  out_var_list(lis
-00002660: 7428 7375 6d6f 7574 5f76 6172 7329 290d  t(sumout_vars)).
-00002670: 0a0d 0a0d 0a20 2020 2020 2020 2023 7073  .....        #ps
-00002680: 695f 636f 7079 2e63 7074 203d 2070 7369  i_copy.cpt = psi
-00002690: 5f63 6f70 792e 6370 742e 6c6f 635b 3a2c  _copy.cpt.loc[:,
-000026a0: 5b63 2066 6f72 2063 2069 6e20 7073 695f  [c for c in psi_
-000026b0: 636f 7079 2e63 7074 2e63 6f6c 756d 6e73  copy.cpt.columns
-000026c0: 2069 6620 2750 726f 6227 206e 6f74 2069   if 'Prob' not i
-000026d0: 6e20 635d 5d0d 0a20 2020 2020 2020 2023  n c]]..        #
-000026e0: 7073 695f 636f 7079 2e63 7074 5b73 7472  psi_copy.cpt[str
-000026f0: 2827 5072 6f62 2d56 616c 2d27 202b 2073  ('Prob-Val-' + s
-00002700: 7472 286e 702e 7261 6e64 6f6d 2e72 616e  tr(np.random.ran
-00002710: 6469 6e74 2830 2c31 3030 3030 3030 2929  dint(0,1000000))
-00002720: 295d 203d 2031 0d0a 2020 2020 2020 2020  )] = 1..        
-00002730: 7072 696e 7428 2749 6e69 7420 4d73 673a  print('Init Msg:
-00002740: 205c 6e27 2c20 7073 695f 636f 7079 2e63   \n', psi_copy.c
-00002750: 7074 290d 0a20 2020 2020 2020 206f 7468  pt)..        oth
-00002760: 6572 5f63 6c69 7175 652e 6d65 7373 6167  er_clique.messag
-00002770: 6573 5f72 6563 6569 7665 642e 6170 7065  es_received.appe
-00002780: 6e64 2870 7369 5f63 6f70 7929 0d0a 0d0a  nd(psi_copy)....
-00002790: 2020 2020 2020 2020 7365 6c66 2e62 656c          self.bel
-000027a0: 6965 6620 3d20 636f 7079 2873 656c 662e  ief = copy(self.
-000027b0: 7073 6929 0d0a 0d0a 2020 2020 6465 6620  psi)....    def 
-000027c0: 636f 6c6c 6563 745f 6265 6c69 6566 7328  collect_beliefs(
-000027d0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-000027e0: 2222 220d 0a20 2020 2020 2020 2043 6f6c  """..        Col
-000027f0: 6c65 6374 696e 6720 6265 6c69 6566 7320  lecting beliefs 
-00002800: 6973 2064 6f6e 6520 6279 2074 616b 696e  is done by takin
-00002810: 6720 7468 650d 0a20 2020 2020 2020 2070  g the..        p
-00002820: 6f74 656e 7469 616c 2028 7365 6c66 2e70  otential (self.p
-00002830: 7369 2920 6f66 2058 2061 6e64 206d 756c  si) of X and mul
-00002840: 7469 706c 7969 6e67 2062 7920 616c 6c20  tiplying by all 
-00002850: 6f66 0d0a 2020 2020 2020 2020 7468 6520  of..        the 
-00002860: 6d65 7373 6167 6573 2077 6869 6368 2058  messages which X
-00002870: 2068 6173 2072 6563 6569 7665 642e 0d0a   has received...
-00002880: 0d0a 2020 2020 2020 2020 4e4f 5445 3a20  ..        NOTE: 
-00002890: 6f6e 6365 2062 656c 6965 6673 2061 7265  once beliefs are
-000028a0: 2063 6f6c 6c65 6374 6564 2c20 7468 6520   collected, the 
-000028b0: 6d65 7373 6167 6573 0d0a 2020 2020 2020  messages..      
-000028c0: 2020 7768 6963 6820 7468 6520 436c 6971    which the Cliq
-000028d0: 7565 2068 6173 2072 6563 6569 7665 6420  ue has received 
-000028e0: 6172 6520 636c 6561 7265 6420 6f75 742e  are cleared out.
-000028f0: 0d0a 0d0a 2020 2020 2020 2020 4e6f 7465  ....        Note
-00002900: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
-00002910: 0d0a 2020 2020 2020 2020 4120 726f 6f74  ..        A root
-00002920: 206e 6f64 6520 2869 2e65 2e20 6f6e 6520   node (i.e. one 
-00002930: 7468 6174 2064 6f65 736e 2774 2073 656e  that doesn't sen
-00002940: 6420 6120 6d65 7373 6167 6529 206d 7573  d a message) mus
-00002950: 7420 7275 6e20 636f 6c6c 6563 745f 6265  t run collect_be
-00002960: 6c69 6566 730d 0a20 2020 2020 2020 2073  liefs..        s
-00002970: 696e 6365 2074 6865 7920 6172 6520 6f6e  ince they are on
-00002980: 6c79 2063 6f6c 6c65 6374 6564 2061 7420  ly collected at 
-00002990: 7365 6e64 5f6d 6573 7361 6765 2829 0d0a  send_message()..
-000029a0: 0d0a 2020 2020 2020 2020 416c 736f 2c20  ..        Also, 
-000029b0: 7765 2063 6f6c 6c65 6374 2062 656c 6965  we collect belie
-000029c0: 6673 2061 7420 7468 6520 656e 6420 6f66  fs at the end of
-000029d0: 206c 6f6f 7079 2062 656c 6965 6620 7072   loopy belief pr
-000029e0: 6f70 6167 6174 696f 6e20 2861 7070 726f  opagation (appro
-000029f0: 782e 2069 6e66 6572 656e 6365 290d 0a20  x. inference).. 
-00002a00: 2020 2020 2020 2073 696e 6365 2074 6865         since the
-00002a10: 206d 6169 6e20 616c 676f 7269 7468 6d20   main algorithm 
-00002a20: 6973 206a 7573 7420 7365 6e64 696e 6720  is just sending 
-00002a30: 6d65 7373 6167 6573 2066 6f72 2061 2077  messages for a w
-00002a40: 6869 6c65 2e0d 0a20 2020 2020 2020 2022  hile...        "
-00002a50: 2222 0d0a 2020 2020 2020 2020 6966 206c  ""..        if l
-00002a60: 656e 2873 656c 662e 6d65 7373 6167 6573  en(self.messages
-00002a70: 5f72 6563 6569 7665 6429 203e 2030 3a0d  _received) > 0:.
-00002a80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00002a90: 662e 6265 6c69 6566 203d 2063 6f70 7928  f.belief = copy(
-00002aa0: 7365 6c66 2e70 7369 290d 0a20 2020 2020  self.psi)..     
-00002ab0: 2020 2020 2020 2066 6f72 206d 7367 2069         for msg i
-00002ac0: 6e20 7365 6c66 2e6d 6573 7361 6765 735f  n self.messages_
-00002ad0: 7265 6365 6976 6564 3a0d 0a20 2020 2020  received:..     
-00002ae0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00002af0: 6265 6c69 6566 202a 3d20 6d73 670d 0a20  belief *= msg.. 
-00002b00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00002b10: 6265 6c69 6566 200d 0a20 2020 2020 2020  belief ..       
-00002b20: 2020 2020 2073 656c 662e 6d65 7373 6167       self.messag
-00002b30: 6573 5f72 6563 6569 7665 6420 3d20 5b5d  es_received = []
-00002b40: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-00002b50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00002b60: 662e 6265 6c69 6566 203d 2063 6f70 7928  f.belief = copy(
-00002b70: 7365 6c66 2e62 656c 6965 6629 0d0a 0d0a  self.belief)....
-00002b80: 2020 2020 6465 6620 7365 7073 6574 2873      def sepset(s
-00002b90: 656c 662c 206f 7468 6572 5f63 6c69 7175  elf, other_cliqu
-00002ba0: 6529 3a0d 0a20 2020 2020 2020 2022 2222  e):..        """
-00002bb0: 0d0a 2020 2020 2020 2020 5468 6520 7365  ..        The se
-00002bc0: 7073 6574 206f 6620 7477 6f20 636c 6971  pset of two cliq
-00002bd0: 7565 7320 6973 2074 6865 2073 6574 206f  ues is the set o
-00002be0: 660d 0a20 2020 2020 2020 2076 6172 6961  f..        varia
-00002bf0: 626c 6573 2069 6e20 7468 6520 696e 7465  bles in the inte
-00002c00: 7273 6563 7469 6f6e 206f 6620 7468 6520  rsection of the 
-00002c10: 7477 6f0d 0a20 2020 2020 2020 2063 6c69  two..        cli
-00002c20: 7175 6573 2720 7363 6f70 6573 2e0d 0a0d  ques' scopes....
-00002c30: 0a20 2020 2020 2020 2041 7267 756d 656e  .        Argumen
-00002c40: 7473 0d0a 2020 2020 2020 2020 2d2d 2d2d  ts..        ----
-00002c50: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 202a  -----..        *
-00002c60: 6f74 6865 725f 636c 6971 7565 2a20 3a20  other_clique* : 
-00002c70: 6120 436c 6971 7565 206f 626a 6563 740d  a Clique object.
-00002c80: 0a0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
-00002c90: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00002ca0: 656c 662e 7363 6f70 652e 696e 7465 7273  elf.scope.inters
-00002cb0: 6563 7469 6f6e 286f 7468 6572 5f63 6c69  ection(other_cli
-00002cc0: 7175 652e 7363 6f70 6529 0d0a 0d0a 2020  que.scope)....  
-00002cd0: 2020 6465 6620 6d61 7267 696e 616c 697a    def marginaliz
-00002ce0: 655f 6f76 6572 2873 656c 662c 2074 6172  e_over(self, tar
-00002cf0: 6765 7429 3a0d 0a20 2020 2020 2020 2022  get):..        "
-00002d00: 2222 0d0a 2020 2020 2020 2020 4d61 7267  ""..        Marg
-00002d10: 696e 616c 697a 6520 7468 6520 6370 7420  inalize the cpt 
-00002d20: 2862 656c 6965 6629 206f 7665 7220 6120  (belief) over a 
-00002d30: 7461 7267 6574 2076 6172 6961 626c 652e  target variable.
-00002d40: 0d0a 0d0a 2020 2020 2020 2020 4172 6775  ....        Argu
-00002d50: 6d65 6e74 730d 0a20 2020 2020 2020 202d  ments..        -
-00002d60: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
-00002d70: 2020 2a74 6172 6765 742a 203a 2061 2073    *target* : a s
-00002d80: 7472 696e 670d 0a20 2020 2020 2020 2020  tring..         
-00002d90: 2020 2054 6865 2074 6172 6765 7420 7261     The target ra
-00002da0: 6e64 6f6d 2076 6172 6961 626c 652e 0d0a  ndom variable...
-00002db0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00002dc0: 2020 2020 2020 2062 6c66 203d 2063 6f70         blf = cop
-00002dd0: 7928 7365 6c66 2e62 656c 6965 6629 0d0a  y(self.belief)..
-00002de0: 2020 2020 2020 2020 626c 662e 7375 6d6f          blf.sumo
-00002df0: 7665 725f 7661 7228 7461 7267 6574 290d  ver_var(target).
-00002e00: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00002e10: 626c 660d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d  blf.............
-00002e20: 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d 0a0d  ................
-00002e30: 0a0d 0a                                  ...
+00000000: 6f0d 0d0a 0000 0000 904d 2164 332e 0000  o........M!d3...
+00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
+00000020: 0004 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
+00000030: 5a00 6401 5a01 6402 6403 6c02 5a03 6402  Z.d.Z.d.d.l.Z.d.
+00000040: 6404 6c04 6d04 5a04 0100 6402 6405 6c05  d.l.m.Z...d.d.l.
+00000050: 6d06 5a06 0100 6402 6406 6c07 5400 4700  m.Z...d.d.l.T.G.
+00000060: 6407 6408 8400 6408 6508 8303 5a09 4700  d.d...d.e...Z.G.
+00000070: 6409 640a 8400 640a 6508 8303 5a0a 6403  d.d...d.e...Z.d.
+00000080: 5300 290b 6196 0400 000a 2a2a 2a2a 2a2a  S.).a.....******
+00000090: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 0a43 6c69  ************.Cli
+000000a0: 7175 6554 7265 6520 436c 6173 7320 0a26  queTree Class .&
+000000b0: 0a43 6c69 7175 6520 436c 6173 730a 2a2a  .Clique Class.**
+000000c0: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
+000000d0: 0a0a 5468 6973 2069 7320 6120 636c 6173  ..This is a clas
+000000e0: 7320 666f 7220 6372 6561 7469 6e67 2f6d  s for creating/m
+000000f0: 616e 6970 756c 6174 696e 6720 4a75 6e63  anipulating Junc
+00000100: 7469 6f6e 2028 436c 6971 7565 2920 5472  tion (Clique) Tr
+00000110: 6565 732c 0a61 6e64 2070 6572 666f 726d  ees,.and perform
+00000120: 696e 6720 696e 6665 7265 6e63 6520 6f76  ing inference ov
+00000130: 6572 2074 6865 6d2e 2054 6865 2061 6476  er them. The adv
+00000140: 616e 7461 6765 206f 6620 636c 6971 7565  antage of clique
+00000150: 2074 7265 6573 0a6f 7665 7220 7472 6164   trees.over trad
+00000160: 6974 696f 6e61 6c20 7661 7269 6162 6c65  itional variable
+00000170: 2065 6c69 6d69 6e61 7469 6f6e 206f 7665   elimination ove
+00000180: 7220 7468 6520 6f72 6967 696e 616c 2042  r the original B
+00000190: 6179 6573 6961 6e20 0a6e 6574 776f 726b  ayesian .network
+000001a0: 2069 7320 7468 6174 2063 6c69 7175 6520   is that clique 
+000001b0: 7472 6565 7320 616c 6c6f 7720 796f 7520  trees allow you 
+000001c0: 746f 2063 6f6d 7075 7465 206d 6172 6769  to compute margi
+000001d0: 6e61 6c0a 7072 6f62 6162 696c 6974 6965  nal.probabilitie
+000001e0: 7320 6f66 204d 554c 5449 504c 4520 7661  s of MULTIPLE va
+000001f0: 7269 6162 6c65 7320 7769 7468 6f75 7420  riables without 
+00000200: 6861 7669 6e67 2074 6f20 7275 6e20 7468  having to run th
+00000210: 650a 656e 7469 7265 2061 6c67 6f72 6974  e.entire algorit
+00000220: 686d 206f 7665 722e 200a 0a54 6865 7265  hm over. ..There
+00000230: 666f 7265 2c20 6966 2079 6f75 2068 6176  fore, if you hav
+00000240: 6520 746f 2071 7565 7279 2074 6865 2042  e to query the B
+00000250: 6179 6573 6961 6e20 6e65 7477 6f72 6b20  ayesian network 
+00000260: 6d61 6e79 2074 696d 6573 200a 2d2d 2061  many times .-- a
+00000270: 6e64 2079 6f75 2077 616e 7420 7468 6520  nd you want the 
+00000280: 6578 6163 7420 6d61 7267 696e 616c 2076  exact marginal v
+00000290: 616c 7565 7320 2d2d 2074 6865 6e20 6974  alues -- then it
+000002a0: 206d 6967 6874 2062 6520 0a62 6573 7420   might be .best 
+000002b0: 746f 2075 7365 2074 6865 2063 6c69 7175  to use the cliqu
+000002c0: 6520 7472 6565 2064 6174 6120 7374 7275  e tree data stru
+000002d0: 6374 7572 6520 666f 7220 696e 6665 7265  cture for infere
+000002e0: 6e63 652e 0a49 6620 796f 7520 6e65 6564  nce..If you need
+000002f0: 2074 6f20 636f 6d70 7574 6520 7468 6520   to compute the 
+00000300: 6d61 7267 696e 616c 2064 6973 7472 6962  marginal distrib
+00000310: 7574 696f 6e20 666f 7220 616c 6c20 7661  ution for all va
+00000320: 7269 6162 6c65 732c 0a62 7574 2079 6f75  riables,.but you
+00000330: 2064 6f6e 7420 6d69 6e64 2061 6e20 6170   dont mind an ap
+00000340: 7072 6f78 696d 6174 652c 2061 2073 616d  proximate, a sam
+00000350: 706c 696e 6720 616c 676f 7269 7468 6d20  pling algorithm 
+00000360: 6973 2070 726f 6261 626c 790a 7468 6520  is probably.the 
+00000370: 7761 7920 746f 2067 6f2e 0a0a 496e 2067  way to go...In g
+00000380: 656e 6572 616c 2c20 7468 6520 6a75 6e63  eneral, the junc
+00000390: 7469 6f6e 2074 7265 6520 616c 676f 7269  tion tree algori
+000003a0: 7468 6d73 2067 656e 6572 616c 697a 6520  thms generalize 
+000003b0: 0a56 6172 6961 626c 6520 456c 696d 696e  .Variable Elimin
+000003c0: 6174 696f 6e20 746f 2074 6865 2065 6666  ation to the eff
+000003d0: 6963 6965 6e74 2c20 7369 6d75 6c74 616e  icient, simultan
+000003e0: 656f 7573 2065 7865 6375 7469 6f6e 200a  eous execution .
+000003f0: 6f66 2061 206c 6172 6765 2063 6c61 7373  of a large class
+00000400: 206f 6620 7175 6572 6965 732e 0a0a 4e4f   of queries...NO
+00000410: 5445 3a20 4120 636c 7573 7465 7220 6772  TE: A cluster gr
+00000420: 6170 6820 6973 2061 2067 656e 6572 616c  aph is a general
+00000430: 697a 6174 696f 6e20 6f66 2074 6865 2063  ization of the c
+00000440: 6c69 7175 6520 7472 6565 0a64 6174 6120  lique tree.data 
+00000450: 7374 7275 6374 7572 6520 2d20 746f 2067  structure - to g
+00000460: 656e 6572 6174 6520 6120 636c 6971 7565  enerate a clique
+00000470: 2074 7265 652c 2079 6f75 2066 6972 7374   tree, you first
+00000480: 2067 656e 6572 6174 650a 6120 636c 7573   generate.a clus
+00000490: 7465 7220 6772 6170 682c 2074 6865 6e20  ter graph, then 
+000004a0: 7369 6d70 6c79 2063 616c 6375 6c61 7465  simply calculate
+000004b0: 2061 206d 6178 696d 756d 2073 7061 6e6e   a maximum spann
+000004c0: 696e 6720 7472 6565 2e0a 496e 206f 7468  ing tree..In oth
+000004d0: 6572 2077 6f72 6473 2c20 6120 636c 6971  er words, a cliq
+000004e0: 7565 2074 7265 6520 6361 6e20 6265 2063  ue tree can be c
+000004f0: 6f6e 7369 6465 7265 6420 6173 2061 2073  onsidered as a s
+00000500: 7065 6369 616c 0a74 7970 6520 6f66 2063  pecial.type of c
+00000510: 6c75 7374 6572 2067 7261 7068 2e0a 0a7a  luster graph...z
+00000520: 2a4e 6963 686f 6c61 7320 4375 6c6c 656e  *Nicholas Cullen
+00000530: 203c 6e63 756c 6c65 6e2e 7468 4064 6172   <ncullen.th@dar
+00000540: 746d 6f75 7468 2e65 6475 3ee9 0000 0000  tmouth.edu>.....
+00000550: 4e29 01da 0463 6f70 7929 01da 0d46 6163  N)...copy)...Fac
+00000560: 746f 7269 7a61 7469 6f6e 2901 da01 2a63  torization)...*c
+00000570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000580: 0200 0000 4000 0000 7348 0000 0065 005a  ....@...sH...e.Z
+00000590: 0164 005a 0264 015a 0364 0264 0384 005a  .d.Z.d.Z.d.d...Z
+000005a0: 0464 0464 0584 005a 0564 0664 0784 005a  .d.d...Z.d.d...Z
+000005b0: 0664 0864 0984 005a 0764 0a64 0b84 005a  .d.d...Z.d.d...Z
+000005c0: 0864 0c64 0d84 005a 0964 0e64 0f84 005a  .d.d...Z.d.d...Z
+000005d0: 0a64 1053 0029 11da 0a43 6c69 7175 6554  .d.S.)...CliqueT
+000005e0: 7265 6561 cc01 0000 0a20 2020 2043 6c69  reea.....    Cli
+000005f0: 7175 6554 7265 6520 436c 6173 730a 0a20  queTree Class.. 
+00000600: 2020 204c 6574 2047 2062 6520 6120 6368     Let G be a ch
+00000610: 6f72 6461 6c20 6772 6170 6820 2869 652e  ordal graph (ie.
+00000620: 2061 2067 7261 7068 2073 7563 6820 7468   a graph such th
+00000630: 6174 206e 6f20 6379 636c 6520 696e 636c  at no cycle incl
+00000640: 7564 6573 206d 6f72 650a 2020 2020 7468  udes more.    th
+00000650: 616e 2074 6872 6565 206e 6f64 6573 292c  an three nodes),
+00000660: 2074 6865 6e20 6120 436c 6971 7565 5472   then a CliqueTr
+00000670: 6565 2069 7320 6120 7472 6565 2048 2073  ee is a tree H s
+00000680: 7563 6820 7468 6174 2065 6163 680a 2020  uch that each.  
+00000690: 2020 6d61 7869 6d61 6c20 636c 6971 7565    maximal clique
+000006a0: 2043 2069 6e20 4720 6973 2061 206e 6f64   C in G is a nod
+000006b0: 6520 696e 2048 2e0a 0a20 2020 2041 7474  e in H...    Att
+000006c0: 7269 6275 7465 730a 2020 2020 2d2d 2d2d  ributes.    ----
+000006d0: 2d2d 2d2d 2d2d 0a20 2020 202d 2062 6e20  ------.    - bn 
+000006e0: 0a20 2020 2020 2020 202d 2042 6179 6573  .        - Bayes
+000006f0: 4e65 7420 6f62 6a65 6374 0a0a 2020 2020  Net object..    
+00000700: 2d20 560a 2020 2020 2020 2020 2d20 5665  - V.        - Ve
+00000710: 7274 6963 6573 202d 3e20 6c69 7374 0a0a  rtices -> list..
+00000720: 2020 2020 2d20 450a 2020 2020 2020 2020      - E.        
+00000730: 2d20 4564 6765 7320 2d3e 2064 6963 7469  - Edges -> dicti
+00000740: 6f6e 6172 790a 0a20 2020 202d 2043 0a20  onary..    - C. 
+00000750: 2020 2020 2020 202d 2043 6c69 7175 6573         - Cliques
+00000760: 202d 3e20 6120 6469 6374 696f 6e61 7279   -> a dictionary
+00000770: 2077 6865 7265 206b 6579 203d 2076 6572   where key = ver
+00000780: 7465 7820 6964 782c 0a20 2020 2020 2020  tex idx,.       
+00000790: 2020 2020 2020 2020 2076 616c 7565 203d           value =
+000007a0: 2043 6c69 7175 6520 6f62 6a65 6374 0a0a   Clique object..
+000007b0: 2020 2020 6302 0000 0000 0000 0000 0000      c...........
+000007c0: 0002 0000 0002 0000 0043 0000 0073 2e00  .........C...s..
+000007d0: 0000 6401 7c00 5f00 6401 7c00 5f01 6401  ..d.|._.d.|._.d.
+000007e0: 7c00 5f02 7c01 7c00 5f03 7404 7c01 8301  |._.|.|._.t.|...
+000007f0: 7c00 5f05 7c00 a006 a100 0100 6401 5300  |._.|.......d.S.
+00000800: 2902 6150 0100 000a 2020 2020 2020 2020  ).aP....        
+00000810: 496e 7374 616e 7469 6174 6520 6120 436c  Instantiate a Cl
+00000820: 6971 7565 5472 6565 206f 626a 6563 742e  iqueTree object.
+00000830: 0a0a 2020 2020 2020 2020 4172 6775 6d65  ..        Argume
+00000840: 6e74 730a 2020 2020 2020 2020 2d2d 2d2d  nts.        ----
+00000850: 2d2d 2d2d 2d0a 2020 2020 2020 2020 2a62  -----.        *b
+00000860: 6e2a 3a20 6120 4261 7965 734e 6574 206f  n*: a BayesNet o
+00000870: 626a 6563 740a 0a20 2020 2020 2020 204e  bject..        N
+00000880: 6f74 6573 0a20 2020 2020 2020 202d 2d2d  otes.        ---
+00000890: 2d2d 0a20 2020 2020 2020 2049 6465 616c  --.        Ideal
+000008a0: 6c79 2c20 7468 6520 4661 6374 6f72 2063  ly, the Factor c
+000008b0: 6c61 7373 2073 686f 756c 6420 6265 2075  lass should be u
+000008c0: 7365 6420 6173 2074 6865 0a20 2020 2020  sed as the.     
+000008d0: 2020 2063 6c69 7175 6573 2069 6e73 7465     cliques inste
+000008e0: 6164 206f 6620 7468 6520 436c 6971 7565  ad of the Clique
+000008f0: 2063 6c61 7373 2028 6265 6361 7573 6520   class (because 
+00000900: 6974 2773 0a20 2020 2020 2020 206a 7573  it's.        jus
+00000910: 7420 6120 7761 7465 7265 6420 646f 776e  t a watered down
+00000920: 2076 6572 7369 6f6e 206f 6620 7468 6520   version of the 
+00000930: 4661 6374 6f72 2063 6c61 7373 2920 2020  Factor class)   
+00000940: 2020 2020 200a 2020 2020 2020 2020 0a20       .        . 
+00000950: 2020 2020 2020 204e 2907 da01 56da 0145         N)...V..E
+00000960: da01 43da 0262 6e72 0300 0000 da02 5f46  ..C..bnr......_F
+00000970: da0f 696e 6974 6961 6c69 7a65 5f74 7265  ..initialize_tre
+00000980: 6529 02da 0473 656c 6672 0900 0000 a900  e)...selfr......
+00000990: 720d 0000 00fa 4c43 3a5c 5573 6572 735c  r.....LC:\Users\
+000009a0: 526f 6d61 6e5c 4465 736b 746f 705c 4769  Roman\Desktop\Gi
+000009b0: 7442 616d 745c 4241 4d54 5c62 616d 745c  tBamt\BAMT\bamt\
+000009c0: 6578 7465 726e 616c 5c70 7942 4e5c 636c  external\pyBN\cl
+000009d0: 6173 7365 735c 636c 6971 7565 7472 6565  asses\cliquetree
+000009e0: 2e70 79da 085f 5f69 6e69 745f 5f46 0000  .py..__init__F..
+000009f0: 0073 0c00 0000 0610 0601 0601 0603 0a01  .s..............
+00000a00: 0c01 7a13 436c 6971 7565 5472 6565 2e5f  ..z.CliqueTree._
+00000a10: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
+00000a20: 0000 0000 0200 0000 0200 0000 6300 0000  ............c...
+00000a30: 731c 0000 0081 007c 006a 00a0 01a1 0044  s......|.j.....D
+00000a40: 005d 057d 017c 0156 0001 0071 0664 0053  .].}.|.V...q.d.S
+00000a50: 00a9 014e 2902 7208 0000 00da 0676 616c  ...N).r......val
+00000a60: 7565 7329 0272 0c00 0000 da06 636c 6971  ues).r......cliq
+00000a70: 7565 720d 0000 0072 0d00 0000 720e 0000  uer....r....r...
+00000a80: 00da 085f 5f69 7465 725f 5f64 0000 0073  ...__iter__d...s
+00000a90: 0800 0000 0280 0e01 0801 04ff 7a13 436c  ............z.Cl
+00000aa0: 6971 7565 5472 6565 2e5f 5f69 7465 725f  iqueTree.__iter_
+00000ab0: 5f63 0200 0000 0000 0000 0000 0000 0200  _c..............
+00000ac0: 0000 0200 0000 4300 0000 f30a 0000 007c  ......C........|
+00000ad0: 006a 007c 0119 0053 0029 017a 300a 2020  .j.|...S.).z0.  
+00000ae0: 2020 2020 2020 5265 7475 726e 7320 436c        Returns Cl
+00000af0: 6971 7565 206f 6620 7061 7373 6564 2d69  ique of passed-i
+00000b00: 6e20 7276 0a20 2020 2020 2020 2029 0172  n rv.        ).r
+00000b10: 0800 0000 2902 720c 0000 00da 0272 7672  ....).r......rvr
+00000b20: 0d00 0000 720d 0000 0072 0e00 0000 da0b  ....r....r......
+00000b30: 5f5f 6765 7469 7465 6d5f 5f68 0000 0073  __getitem__h...s
+00000b40: 0200 0000 0a04 7a16 436c 6971 7565 5472  ......z.CliqueTr
+00000b50: 6565 2e5f 5f67 6574 6974 656d 5f5f 6302  ee.__getitem__c.
+00000b60: 0000 0000 0000 0000 0000 0004 0000 0004  ................
+00000b70: 0000 0043 0000 0073 2c00 0000 6700 7d02  ...C...s,...g.}.
+00000b80: 7c00 6a00 4400 5d0e 7d03 7c01 7c00 6a01  |.j.D.].}.|.|.j.
+00000b90: 7c03 1900 7600 7213 7c02 a002 7c01 a101  |...v.r.|...|...
+00000ba0: 0100 7105 7c02 5300 7210 0000 0029 0372  ..q.|.S.r....).r
+00000bb0: 0600 0000 7207 0000 00da 0661 7070 656e  ....r......appen
+00000bc0: 6429 0472 0c00 0000 da01 76da 0170 7215  d).r......v..pr.
+00000bd0: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+00000be0: 0000 da07 7061 7265 6e74 736e 0000 0073  ....parentsn...s
+00000bf0: 0c00 0000 0401 0a01 0e01 0a01 0280 0401  ................
+00000c00: 7a12 436c 6971 7565 5472 6565 2e70 6172  z.CliqueTree.par
+00000c10: 656e 7473 6302 0000 0000 0000 0000 0000  entsc...........
+00000c20: 0002 0000 0002 0000 0043 0000 0072 1400  .........C...r..
+00000c30: 0000 7210 0000 0029 0172 0700 0000 2902  ..r....).r....).
+00000c40: 720c 0000 00da 016e 720d 0000 0072 0d00  r......nr....r..
+00000c50: 0000 720e 0000 00da 0863 6869 6c64 7265  ..r......childre
+00000c60: 6e75 0000 00f3 0200 0000 0a01 7a13 436c  nu..........z.Cl
+00000c70: 6971 7565 5472 6565 2e63 6869 6c64 7265  iqueTree.childre
+00000c80: 6e63 0200 0000 0000 0000 0000 0000 0500  nc..............
+00000c90: 0000 0500 0000 4300 0000 732c 0000 0074  ......C...s,...t
+00000ca0: 00a0 017c 006a 02a1 017d 0274 00a0 037c  ...|.j...}.t...|
+00000cb0: 027c 01a1 027d 0374 0474 00a0 057c 037c  .|...}.t.t...|.|
+00000cc0: 01a1 0283 017d 047c 0453 0072 1000 0000  .....}.|.S.r....
+00000cd0: 2906 da02 6e78 da05 4772 6170 6872 0700  )...nx..Graphr..
+00000ce0: 0000 da08 6466 735f 7472 6565 da04 6c69  ....dfs_tree..li
+00000cf0: 7374 da13 6466 735f 706f 7374 6f72 6465  st..dfs_postorde
+00000d00: 725f 6e6f 6465 7329 0572 0c00 0000 da04  r_nodes).r......
+00000d10: 726f 6f74 da01 47da 0a74 7265 655f 6772  root..G..tree_gr
+00000d20: 6170 685a 0f63 6c69 7175 655f 6f72 6465  aphZ.clique_orde
+00000d30: 7269 6e67 720d 0000 0072 0d00 0000 720e  ringr....r....r.
+00000d40: 0000 00da 0d64 6673 5f70 6f73 746f 7264  .....dfs_postord
+00000d50: 6572 7800 0000 7308 0000 000c 010c 0110  erx...s.........
+00000d60: 0104 017a 1843 6c69 7175 6554 7265 652e  ...z.CliqueTree.
+00000d70: 6466 735f 706f 7374 6f72 6465 7263 0100  dfs_postorderc..
+00000d80: 0000 0000 0000 0000 0000 0f00 0000 0700  ................
+00000d90: 0000 4300 0000 7386 0100 0074 007c 006a  ..C...s....t.|.j
+00000da0: 0183 017d 017c 01a0 02a1 007d 0269 007d  ...}.|.....}.i.}
+00000db0: 0374 0374 0474 05a0 067c 01a1 0183 0183  .t.t.t...|......
+00000dc0: 017d 0474 077c 0483 0144 005d 0c5c 027d  .}.t.|...D.].\.}
+00000dd0: 057d 0674 0874 097c 0683 0183 017c 037c  .}.t.t.|.....|.|
+00000de0: 053c 0071 1874 0a64 0164 0284 0074 0b74  .<.q.t.d.d...t.t
+00000df0: 0c7c 0383 0183 0144 0083 0183 017d 0774  .|.....D.....}.t
+00000e00: 0b74 0c7c 0383 0183 0144 005d 227d 0874  .t.|.....D.]"}.t
+00000e10: 0b74 0c7c 0383 0183 0144 005d 197d 097c  .t.|.....D.].}.|
+00000e20: 087c 096b 0372 5974 0c7c 037c 0819 00a0  .|.k.rYt.|.|....
+00000e30: 0d7c 037c 0919 00a1 0183 017d 0a64 037c  .|.|.......}.d.|
+00000e40: 0a14 007c 077c 0819 007c 093c 0071 4071  ...|.|...|.<.q@q
+00000e50: 3874 0e7c 0783 017d 0b7c 0b7c 005f 0f7c  8t.|...}.|.|._.|
+00000e60: 0ba0 10a1 007c 005f 117c 037c 005f 1274  .....|._.|.|._.t
+00000e70: 0a64 0464 0284 007c 006a 01a0 02a1 0044  .d.d...|.j.....D
+00000e80: 0083 0183 017d 0c7c 006a 12a0 13a1 0044  .....}.|.j.....D
+00000e90: 005d 2b7d 0667 007d 0d7c 0c44 005d 1d7d  .]+}.g.}.|.D.].}
+00000ea0: 0e7c 0c7c 0e19 0064 056b 0272 9e74 097c  .|.|...d.k.r.t.|
+00000eb0: 006a 01a0 147c 0ea1 0183 01a0 157c 066a  .j...|.......|.j
+00000ec0: 14a1 0172 9e7c 0da0 167c 0ea1 0101 0064  ...r.|...|.....d
+00000ed0: 067c 0c7c 0e3c 0071 8174 177c 006a 017c  .|.|.<.q.t.|.j.|
+00000ee0: 0d83 027c 065f 1871 7b7c 006a 12a0 19a1  ...|._.q{|.j....
+00000ef0: 0044 005d 145c 027d 087d 0674 0c7c 00a0  .D.].\.}.}.t.|..
+00000f00: 1a7c 08a1 0183 0164 076b 0272 bc64 067c  .|.....d.k.r.d.|
+00000f10: 065f 1b7c 06a0 1ca1 0001 0071 ac64 0853  ._.|.......q.d.S
+00000f20: 0029 0961 5f01 0000 0a20 2020 2020 2020  .).a_....       
+00000f30: 2049 6e69 7469 616c 697a 6520 7468 6520   Initialize the 
+00000f40: 7374 7275 6374 7572 6520 6f66 2061 2063  structure of a c
+00000f50: 6c69 7175 6520 7472 6565 2c20 7573 696e  lique tree, usin
+00000f60: 670a 2020 2020 2020 2020 7468 6520 666f  g.        the fo
+00000f70: 6c6c 6f77 696e 6720 7374 6570 733a 0a20  llowing steps:. 
+00000f80: 2020 2020 2020 2020 2020 202d 204d 6f72             - Mor
+00000f90: 616c 697a 6520 6772 6170 6820 2869 2e65  alize graph (i.e
+00000fa0: 2e20 6d61 7272 7920 7061 7265 6e74 7329  . marry parents)
+00000fb0: 0a20 2020 2020 2020 2020 2020 202d 2054  .            - T
+00000fc0: 7269 616e 6775 6c61 7465 2067 7261 7068  riangulate graph
+00000fd0: 2028 692e 652e 206d 616b 6520 6772 6170   (i.e. make grap
+00000fe0: 6820 6368 6f72 6461 6c29 0a20 2020 2020  h chordal).     
+00000ff0: 2020 2020 2020 202d 2047 6574 206d 6178         - Get max
+00001000: 2063 6c69 7175 6573 2028 692e 652e 2063   cliques (i.e. c
+00001010: 6f6d 6d75 6e69 7479 2f63 6c69 7175 6520  ommunity/clique 
+00001020: 6465 7465 6374 696f 6e29 0a20 2020 2020  detection).     
+00001030: 2020 2020 2020 202d 204d 6178 2073 7061         - Max spa
+00001040: 6e6e 696e 6720 7472 6565 206f 7665 7220  nning tree over 
+00001050: 7365 7073 6574 2063 6172 6469 6e61 6c69  sepset cardinali
+00001060: 7479 2028 692e 652e 2063 7265 6174 6520  ty (i.e. create 
+00001070: 7472 6565 290a 2020 2020 2020 2020 0a20  tree).        . 
+00001080: 2020 2020 2020 2063 0100 0000 0000 0000         c........
+00001090: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
+000010a0: 7314 0000 0067 007c 005d 067d 017c 0169  s....g.|.].}.|.i
+000010b0: 0066 0291 0271 0253 0072 0d00 0000 720d  .f...q.S.r....r.
+000010c0: 0000 0029 02da 022e 30da 0563 5f69 6478  ...)....0..c_idx
+000010d0: 720d 0000 0072 0d00 0000 720e 0000 00da  r....r....r.....
+000010e0: 0a3c 6c69 7374 636f 6d70 3e93 0000 00f3  .<listcomp>.....
+000010f0: 0200 0000 1400 7a2e 436c 6971 7565 5472  ......z.CliqueTr
+00001100: 6565 2e69 6e69 7469 616c 697a 655f 7472  ee.initialize_tr
+00001110: 6565 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  ee.<locals>.<lis
+00001120: 7463 6f6d 703e e9ff ffff ff63 0100 0000  tcomp>.....c....
+00001130: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00001140: 5300 0000 7314 0000 0067 007c 005d 067d  S...s....g.|.].}
+00001150: 017c 0164 0066 0291 0271 0253 0029 0146  .|.d.f...q.S.).F
+00001160: 720d 0000 0029 0272 2700 0000 7215 0000  r....).r'...r...
+00001170: 0072 0d00 0000 720d 0000 0072 0e00 0000  .r....r....r....
+00001180: 7229 0000 00a1 0000 0072 2a00 0000 4654  r).......r*...FT
+00001190: 7201 0000 004e 291d 5a0c 6d61 6b65 5f63  r....N).Z.make_c
+000011a0: 686f 7264 616c 7209 0000 00da 056e 6f64  hordalr......nod
+000011b0: 6573 da08 7265 7665 7273 6564 7221 0000  es..reversedr!..
+000011c0: 0072 1e00 0000 da15 6368 6f72 6461 6c5f  .r......chordal_
+000011d0: 6772 6170 685f 636c 6971 7565 73da 0965  graph_cliques..e
+000011e0: 6e75 6d65 7261 7465 da06 436c 6971 7565  numerate..Clique
+000011f0: da03 7365 74da 0464 6963 74da 0572 616e  ..set..dict..ran
+00001200: 6765 da03 6c65 6eda 0673 6570 7365 74da  ge..len..sepset.
+00001210: 036d 7374 7207 0000 00da 046b 6579 7372  .mstr......keysr
+00001220: 0600 0000 7208 0000 0072 1100 0000 da05  ....r....r......
+00001230: 7363 6f70 65da 0869 7373 7562 7365 7472  scope..issubsetr
+00001240: 1700 0000 7203 0000 0072 0a00 0000 da05  ....r....r......
+00001250: 6974 656d 7372 1a00 0000 da08 6973 5f72  itemsr......is_r
+00001260: 6561 6479 da0e 696e 6974 6961 6c69 7a65  eady..initialize
+00001270: 5f70 7369 290f 720c 0000 005a 0963 686f  _psi).r....Z.cho
+00001280: 7264 616c 5f47 7206 0000 0072 0800 0000  rdal_Gr....r....
+00001290: 5a0b 6d61 785f 636c 6971 7565 735a 0576  Z.max_cliquesZ.v
+000012a0: 5f69 6478 7212 0000 005a 1277 6569 6768  _idxr....Z.weigh
+000012b0: 7465 645f 6564 6765 5f64 6963 74da 0169  ted_edge_dict..i
+000012c0: da01 6a5a 1569 6e74 6572 7365 6374 5f63  ..jZ.intersect_c
+000012d0: 6172 6469 6e61 6c69 7479 5a05 6d73 745f  ardinalityZ.mst_
+000012e0: 475a 0376 5f61 5a0a 7465 6d70 5f73 636f  GZ.v_aZ.temp_sco
+000012f0: 7065 da03 7661 7272 0d00 0000 720d 0000  pe..varr....r...
+00001300: 0072 0e00 0000 720b 0000 007e 0000 0073  .r....r....~...s
+00001310: 4000 0000 0a0b 0801 0403 1201 1001 1201  @...............
+00001320: 1a03 1001 1001 0801 1601 1001 0280 02fd  ................
+00001330: 0804 0602 0a01 0601 1804 0e01 0401 0801  ................
+00001340: 2401 0a01 0801 0280 1001 1204 1201 0601  $...............
+00001350: 0a01 04fd 7a1a 436c 6971 7565 5472 6565  ....z.CliqueTree
+00001360: 2e69 6e69 7469 616c 697a 655f 7472 6565  .initialize_tree
+00001370: 4e29 0bda 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00001380: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00001390: 6c6e 616d 655f 5fda 075f 5f64 6f63 5f5f  lname__..__doc__
+000013a0: 720f 0000 0072 1300 0000 7216 0000 0072  r....r....r....r
+000013b0: 1a00 0000 721c 0000 0072 2600 0000 720b  ....r....r&...r.
+000013c0: 0000 0072 0d00 0000 720d 0000 0072 0d00  ...r....r....r..
+000013d0: 0000 720e 0000 0072 0500 0000 2d00 0000  ..r....r....-...
+000013e0: 7312 0000 0008 0004 0108 1808 1e08 0408  s...............
+000013f0: 0608 0708 030c 0672 0500 0000 6300 0000  .......r....c...
+00001400: 0000 0000 0000 0000 0000 0000 0002 0000  ................
+00001410: 0040 0000 0073 6000 0000 6500 5a01 6400  .@...s`...e.Z.d.
+00001420: 5a02 6401 5a03 6402 6403 8400 5a04 6404  Z.d.Z.d.d...Z.d.
+00001430: 6405 8400 5a05 6406 6407 8400 5a06 6408  d...Z.d.d...Z.d.
+00001440: 6409 8400 5a07 640a 640b 8400 5a08 640c  d...Z.d.d...Z.d.
+00001450: 640d 8400 5a09 640e 640f 8400 5a0a 6410  d...Z.d.d...Z.d.
+00001460: 6411 8400 5a0b 6412 6413 8400 5a0c 6414  d...Z.d.d...Z.d.
+00001470: 6415 8400 5a0d 6416 5300 2917 7230 0000  d...Z.d.S.).r0..
+00001480: 0061 0003 0000 0a20 2020 2043 6c69 7175  .a.....    Cliqu
+00001490: 6520 436c 6173 730a 0a20 2020 202a 7363  e Class..    *sc
+000014a0: 6f70 652a 203a 2061 2073 6574 206f 6620  ope* : a set of 
+000014b0: 7661 7269 6162 6c65 7320 696e 2074 6865  variables in the
+000014c0: 2063 6c69 7175 6527 7320 7363 6f70 650a   clique's scope.
+000014d0: 0a20 2020 202a 5f66 2a20 3a20 6120 6661  .    *_f* : a fa
+000014e0: 6374 6f72 697a 6174 696f 6e20 6f62 6a65  ctorization obje
+000014f0: 6374 2074 6861 7420 636f 6e74 6169 6e73  ct that contains
+00001500: 206f 6e6c 7920 7468 650a 2020 2020 2020   only the.      
+00001510: 2020 6661 6374 6f72 7320 6f66 2076 6172    factors of var
+00001520: 6961 626c 6573 2069 6e20 7468 6520 636c  iables in the cl
+00001530: 6971 7565 2773 2073 636f 7065 0a0a 2020  ique's scope..  
+00001540: 2020 2a70 7369 2a20 3a20 6120 6661 6374    *psi* : a fact
+00001550: 6f72 0a20 2020 2020 2020 2054 6865 2070  or.        The p
+00001560: 6f74 656e 7469 616c 206f 6620 7468 6520  otential of the 
+00001570: 636c 6971 7565 2e0a 0a20 2020 202a 6265  clique...    *be
+00001580: 6c69 6566 2a20 3a20 6120 6661 6374 6f72  lief* : a factor
+00001590: 0a20 2020 2020 2020 2054 6865 2066 6163  .        The fac
+000015a0: 746f 7220 7768 6963 6820 686f 6c64 7320  tor which holds 
+000015b0: 7468 6520 6d61 7267 696e 616c 2f63 6f6e  the marginal/con
+000015c0: 6469 7469 6f6e 616c 0a20 2020 2020 2020  ditional.       
+000015d0: 2070 726f 6261 6269 6c69 7469 6573 206f   probabilities o
+000015e0: 6620 7468 6520 7265 6c65 7661 6e74 206e  f the relevant n
+000015f0: 6f64 6573 2061 6674 6572 200a 2020 2020  odes after .    
+00001600: 2020 2020 6265 6c69 6566 2070 726f 7061      belief propa
+00001610: 6761 7469 6f6e 2c20 6574 630a 0a20 2020  gation, etc..   
+00001620: 202a 6d65 7373 6167 6573 5f72 6563 6569   *messages_recei
+00001630: 7665 642a 203a 2061 206c 6973 7420 6f66  ved* : a list of
+00001640: 2046 6163 746f 7273 0a20 2020 2020 2020   Factors.       
+00001650: 2054 6865 206d 6573 7361 6765 7320 7468   The messages th
+00001660: 6520 636c 6971 7565 2068 6173 2072 6563  e clique has rec
+00001670: 6569 7665 6420 6672 6f6d 2069 7473 206e  eived from its n
+00001680: 6569 6768 626f 7273 202d 0a20 2020 2020  eighbors -.     
+00001690: 2020 2073 746f 7265 6420 736f 2074 6861     stored so tha
+000016a0: 7420 7468 6520 6265 6c69 6566 7320 6361  t the beliefs ca
+000016b0: 6e20 6265 2063 616c 6375 6c61 7465 6420  n be calculated 
+000016c0: 6166 7465 720a 2020 2020 2020 2020 6265  after.        be
+000016d0: 6c69 6566 2070 726f 7061 6761 7469 6f6e  lief propagation
+000016e0: 2c20 6574 632e 0a0a 2020 2020 2a69 735f  , etc...    *is_
+000016f0: 7265 6164 792a 203a 2061 2062 6f6f 6c65  ready* : a boole
+00001700: 616e 0a20 2020 2020 2020 2057 6865 7468  an.        Wheth
+00001710: 6572 2074 6865 2063 6c69 7175 6520 6973  er the clique is
+00001720: 2072 6561 6479 2074 6f20 7365 6e64 2061   ready to send a
+00001730: 206d 6573 7361 6765 202d 3e20 6d75 7374   message -> must
+00001740: 0a20 2020 2020 2020 2068 6176 6520 5245  .        have RE
+00001750: 4345 4956 4544 206d 6573 7361 6765 7320  CEIVED messages 
+00001760: 6672 6f6d 2061 6c6c 206f 6620 6974 7320  from all of its 
+00001770: 6e65 6967 6862 6f72 7320 6669 7273 742e  neighbors first.
+00001780: 0a0a 2020 2020 6302 0000 0000 0000 0000  ..    c.........
+00001790: 0000 0002 0000 0002 0000 0043 0000 0073  ...........C...s
+000017a0: 2800 0000 7c01 7c00 5f00 6401 7c00 5f01  (...|.|._.d.|._.
+000017b0: 6401 7c00 5f02 6401 7c00 5f03 6700 7c00  d.|._.d.|._.g.|.
+000017c0: 5f04 6402 7c00 5f05 6401 5300 2903 7ad8  _.d.|._.d.S.).z.
+000017d0: 0a20 2020 2020 2020 2049 6e73 7461 6e74  .        Instant
+000017e0: 6961 7465 2061 2063 6c69 7175 6520 6f62  iate a clique ob
+000017f0: 6a65 6374 0a0a 2020 2020 2020 2020 4172  ject..        Ar
+00001800: 6775 6d65 6e74 730a 2020 2020 2020 2020  guments.        
+00001810: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+00001820: 2020 2a73 636f 7065 2a20 3a20 6120 7079    *scope* : a py
+00001830: 7468 6f6e 2073 6574 0a20 2020 2020 2020  thon set.       
+00001840: 2020 2020 2054 6865 2073 6574 206f 6620       The set of 
+00001850: 7661 7269 6162 6c65 7320 696e 2074 6865  variables in the
+00001860: 2063 6c69 7175 6573 2073 636f 7065 2c0a   cliques scope,.
+00001870: 2020 2020 2020 2020 2020 2020 692e 652e              i.e.
+00001880: 2074 6865 206d 6169 6e20 7661 7220 616e   the main var an
+00001890: 6420 6974 7320 7061 7265 6e74 730a 0a0a  d its parents...
+000018a0: 2020 2020 2020 2020 4e46 2906 7238 0000          NF).r8..
+000018b0: 0072 0a00 0000 da03 7073 69da 0662 656c  .r......psi..bel
+000018c0: 6965 66da 116d 6573 7361 6765 735f 7265  ief..messages_re
+000018d0: 6365 6976 6564 723b 0000 0029 0272 0c00  ceivedr;...).r..
+000018e0: 0000 7238 0000 0072 0d00 0000 720d 0000  ..r8...r....r...
+000018f0: 0072 0e00 0000 720f 0000 00ce 0000 0073  .r....r........s
+00001900: 0c00 0000 060c 0601 0602 0601 0602 0a01  ................
+00001910: 7a0f 436c 6971 7565 2e5f 5f69 6e69 745f  z.Clique.__init_
+00001920: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
+00001930: 0000 0200 0000 4300 0000 f30a 0000 0074  ......C........t
+00001940: 007c 006a 0183 0153 0072 1000 0000 2902  .|.j...S.r....).
+00001950: da03 7374 7272 3800 0000 2901 720c 0000  ..strr8...).r...
+00001960: 0072 0d00 0000 720d 0000 0072 0e00 0000  .r....r....r....
+00001970: da08 5f5f 7265 7072 5f5f e300 0000 721d  ..__repr__....r.
+00001980: 0000 007a 0f43 6c69 7175 652e 5f5f 7265  ...z.Clique.__re
+00001990: 7072 5f5f 6302 0000 0000 0000 0000 0000  pr__c...........
+000019a0: 0002 0000 0003 0000 0043 0000 0073 0e00  .........C...s..
+000019b0: 0000 7c00 a000 7c01 a101 0100 6401 5300  ..|...|.....d.S.
+000019c0: 2902 7a3a 0a20 2020 2020 2020 2053 656e  ).z:.        Sen
+000019d0: 6420 6120 6d65 7373 6167 6520 6672 6f6d  d a message from
+000019e0: 2073 656c 6620 746f 206f 7468 6572 5f63   self to other_c
+000019f0: 6c69 7175 650a 2020 2020 2020 2020 4ea9  lique.        N.
+00001a00: 01da 0c73 656e 645f 6d65 7373 6167 65a9  ...send_message.
+00001a10: 0272 0c00 0000 da0c 6f74 6865 725f 636c  .r......other_cl
+00001a20: 6971 7565 720d 0000 0072 0d00 0000 720e  iquer....r....r.
+00001a30: 0000 00da 0a5f 5f72 7368 6966 745f 5fe6  .....__rshift__.
+00001a40: 0000 00f3 0200 0000 0e04 7a11 436c 6971  ..........z.Cliq
+00001a50: 7565 2e5f 5f72 7368 6966 745f 5f63 0200  ue.__rshift__c..
+00001a60: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00001a70: 0000 4300 0000 730e 0000 007c 01a0 007c  ..C...s....|...|
+00001a80: 00a1 0101 0064 0153 0029 027a 3a0a 2020  .....d.S.).z:.  
+00001a90: 2020 2020 2020 5365 6e64 2061 206d 6573        Send a mes
+00001aa0: 7361 6765 2066 726f 6d20 6f74 6865 725f  sage from other_
+00001ab0: 636c 6971 7565 2074 6f20 7365 6c66 0a20  clique to self. 
+00001ac0: 2020 2020 2020 204e 724a 0000 0072 4c00         NrJ...rL.
+00001ad0: 0000 720d 0000 0072 0d00 0000 720e 0000  ..r....r....r...
+00001ae0: 00da 0a5f 5f6c 7368 6966 745f 5fec 0000  ...__lshift__...
+00001af0: 0072 4f00 0000 7a11 436c 6971 7565 2e5f  .rO...z.Clique._
+00001b00: 5f6c 7368 6966 745f 5f63 0200 0000 0000  _lshift__c......
+00001b10: 0000 0000 0000 0500 0000 0500 0000 4300  ..............C.
+00001b20: 0000 7388 0000 0074 007c 006a 0183 0164  ..s....t.|.j...d
+00001b30: 016b 0472 1e7c 006a 0273 1074 037c 006a  .k.r.|.j.s.t.|.j
+00001b40: 0483 017c 005f 027c 006a 0144 005d 097d  ...|._.|.j.D.].}
+00001b50: 027c 0004 006a 027c 0239 0002 005f 0271  .|...j.|.9..._.q
+00001b60: 136e 097c 006a 0273 2774 037c 006a 0483  .n.|.j.s't.|.j..
+00001b70: 017c 005f 0274 037c 006a 0283 017d 037c  .|._.t.|.j...}.|
+00001b80: 006a 05a0 067c 00a0 077c 01a1 01a1 0144  .j...|...|.....D
+00001b90: 005d 067d 047c 037c 041d 007d 0371 357c  .].}.|.|...}.q5|
+00001ba0: 016a 01a0 087c 03a1 0101 0064 0253 0029  .j...|.....d.S.)
+00001bb0: 0361 ee01 0000 0a20 2020 2020 2020 2053  .a.....        S
+00001bc0: 656e 6420 6120 6d65 7373 6167 6520 746f  end a message to
+00001bd0: 2074 6865 2070 6172 656e 7420 636c 6971   the parent cliq
+00001be0: 7565 2e0a 0a20 2020 2020 2020 2054 6f20  ue...        To 
+00001bf0: 7365 6e64 2061 206d 6573 7361 6765 2066  send a message f
+00001c00: 726f 6d20 5820 746f 2059 2c20 796f 750a  rom X to Y, you.
+00001c10: 2020 2020 2020 2020 6d75 7374 2066 6972          must fir
+00001c20: 7374 2074 616b 6520 7468 6520 706f 7465  st take the pote
+00001c30: 6e74 6961 6c20 2873 656c 662e 7073 6929  ntial (self.psi)
+00001c40: 206f 660a 2020 2020 2020 2020 5820 616e   of.        X an
+00001c50: 6420 7375 6d20 6f75 7420 7468 6520 7661  d sum out the va
+00001c60: 7269 6162 6c65 7320 4e4f 5420 696e 2074  riables NOT in t
+00001c70: 6865 2073 6570 7365 740a 2020 2020 2020  he sepset.      
+00001c80: 2020 6f66 2059 2e0a 0a20 2020 2020 2020    of Y...       
+00001c90: 2054 4845 4e2c 2069 6620 5820 6861 7320   THEN, if X has 
+00001ca0: 7265 6365 6976 6564 2061 6e79 206d 6573  received any mes
+00001cb0: 7361 6765 732c 2074 6865 0a20 2020 2020  sages, the.     
+00001cc0: 2020 2070 6f74 656e 7469 616c 2028 7365     potential (se
+00001cd0: 6c66 2e70 7369 2920 6d75 7374 2062 6520  lf.psi) must be 
+00001ce0: 6d75 6c74 6970 6c69 6564 2062 790a 2020  multiplied by.  
+00001cf0: 2020 2020 2020 616c 6c20 6f66 2074 6865        all of the
+00001d00: 2072 6563 6569 7665 6420 6d65 7373 6167   received messag
+00001d10: 6564 2e0a 0a20 2020 2020 2020 2041 7267  ed...        Arg
+00001d20: 756d 656e 7473 0a20 2020 2020 2020 202d  uments.        -
+00001d30: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00001d40: 202a 7061 7265 6e74 2a20 3a20 6120 7374   *parent* : a st
+00001d50: 7269 6e67 0a20 2020 2020 2020 2020 2020  ring.           
+00001d60: 2054 6865 2070 6172 656e 7420 746f 2077   The parent to w
+00001d70: 6869 6368 2074 6865 206d 6573 7361 6765  hich the message
+00001d80: 2077 696c 6c0a 2020 2020 2020 2020 2020   will.          
+00001d90: 2020 6265 2073 656e 742e 0a0a 2020 2020    be sent...    
+00001da0: 2020 2020 7201 0000 004e 2909 7234 0000      r....N).r4..
+00001db0: 0072 4600 0000 7245 0000 0072 0200 0000  .rF...rE...r....
+00001dc0: 7244 0000 0072 3800 0000 da0a 6469 6666  rD...r8.....diff
+00001dd0: 6572 656e 6365 7235 0000 0072 1700 0000  erencer5...r....
+00001de0: 2905 720c 0000 00da 0670 6172 656e 74da  ).r......parent.
+00001df0: 036d 7367 5a0b 6d73 675f 746f 5f73 656e  .msgZ.msg_to_sen
+00001e00: 645a 0d76 6172 5f74 6f5f 7375 6d6f 7574  dZ.var_to_sumout
+00001e10: 720d 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
+00001e20: 4b00 0000 f200 0000 7318 0000 000e 1706  K.......s.......
+00001e30: 020c 010a 0110 0102 ff06 050c 010a 0316  ................
+00001e40: 010a 0110 037a 1343 6c69 7175 652e 7365  .....z.Clique.se
+00001e50: 6e64 5f6d 6573 7361 6765 6301 0000 0000  nd_messagec.....
+00001e60: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+00001e70: 0000 0073 8200 0000 7400 7c00 6a01 8301  ...s....t.|.j...
+00001e80: 6401 6b03 730b 4a00 6402 8301 8201 7400  d.k.s.J.d.....t.
+00001e90: 7c00 6a01 8301 6403 6b02 7222 7402 7c00  |.j...d.k.r"t.|.
+00001ea0: 6a01 6401 1900 8301 7c00 5f03 7402 7c00  j.d.....|._.t.|.
+00001eb0: 6a03 8301 7c00 5f04 6407 5300 7405 7c00  j...|._.d.S.t.|.
+00001ec0: 6a01 6404 6405 8400 6406 8d02 7c00 5f03  j.d.d...d...|._.
+00001ed0: 7c00 6a01 4400 5d09 7d01 7c00 0400 6a03  |.j.D.].}.|...j.
+00001ee0: 7c01 3900 0200 5f03 712f 7402 7c00 6a03  |.9..._.q/t.|.j.
+00001ef0: 8301 7c00 5f04 6407 5300 2908 7a9d 0a20  ..|._.d.S.).z.. 
+00001f00: 2020 2020 2020 2043 6f6d 7075 7465 2061         Compute a
+00001f10: 206e 6577 2070 7369 2028 6370 7429 2069   new psi (cpt) i
+00001f20: 6e20 6f72 6465 7220 746f 200a 2020 2020  n order to .    
+00001f30: 2020 2020 7365 7420 7468 6520 636c 6971      set the cliq
+00001f40: 7565 2773 2062 656c 6965 662e 2054 6869  ue's belief. Thi
+00001f50: 7320 696e 766f 6c76 6573 0a20 2020 2020  s involves.     
+00001f60: 2020 206d 756c 7469 706c 7969 6e67 2074     multiplying t
+00001f70: 6865 2066 6163 746f 7273 2069 6e20 7468  he factors in th
+00001f80: 6520 436c 6971 7565 2074 6f67 6574 6865  e Clique togethe
+00001f90: 722e 0a20 2020 2020 2020 2072 0100 0000  r..        r....
+00001fa0: 7a23 4e6f 2046 6163 746f 7273 2061 7373  z#No Factors ass
+00001fb0: 6967 6e65 6420 746f 2074 6869 7320 636c  igned to this cl
+00001fc0: 6971 7565 2ee9 0100 0000 6301 0000 0000  ique......c.....
+00001fd0: 0000 0000 0000 0001 0000 0002 0000 0053  ...............S
+00001fe0: 0000 0072 4700 0000 7210 0000 0029 0272  ...rG...r....).r
+00001ff0: 3400 0000 da03 6370 7429 01da 0178 720d  4.....cpt)...xr.
+00002000: 0000 0072 0d00 0000 720e 0000 00da 083c  ...r....r......<
+00002010: 6c61 6d62 6461 3e29 0100 0073 0200 0000  lambda>)...s....
+00002020: 0a00 7a27 436c 6971 7565 2e69 6e69 7469  ..z'Clique.initi
+00002030: 616c 697a 655f 7073 692e 3c6c 6f63 616c  alize_psi.<local
+00002040: 733e 2e3c 6c61 6d62 6461 3e29 01da 036b  s>.<lambda>)...k
+00002050: 6579 4e29 0672 3400 0000 720a 0000 0072  eyN).r4...r....r
+00002060: 0200 0000 7244 0000 0072 4500 0000 da03  ....rD...rE.....
+00002070: 6d61 7829 0272 0c00 0000 da01 6672 0d00  max).r......fr..
+00002080: 0000 720d 0000 0072 0e00 0000 723c 0000  ..r....r....r<..
+00002090: 001d 0100 0073 1000 0000 1606 0e02 1001  .....s..........
+000020a0: 1001 1402 0a01 1001 1001 7a15 436c 6971  ..........z.Cliq
+000020b0: 7565 2e69 6e69 7469 616c 697a 655f 7073  ue.initialize_ps
+000020c0: 6963 0200 0000 0000 0000 0000 0000 0500  ic..............
+000020d0: 0000 0400 0000 4300 0000 7356 0000 0074  ......C...sV...t
+000020e0: 007c 006a 0183 017d 027c 00a0 027c 01a1  .|.j...}.|...|..
+000020f0: 017d 037c 006a 03a0 047c 03a1 017d 047c  .}.|.j...|...}.|
+00002100: 02a0 0574 067c 0483 01a1 0101 0074 0764  ...t.|.......t.d
+00002110: 017c 026a 0883 0201 007c 016a 09a0 0a7c  .|.j.....|.j...|
+00002120: 02a1 0101 0074 007c 006a 0183 017c 005f  .....t.|.j...|._
+00002130: 0b64 0253 0029 037a b90a 2020 2020 2020  .d.S.).z..      
+00002140: 2020 4e4f 5420 5355 5245 2049 4620 5448    NOT SURE IF TH
+00002150: 4953 2049 5320 4e45 4544 4544 2e0a 0a20  IS IS NEEDED... 
+00002160: 2020 2020 2020 2053 656e 6420 7468 6520         Send the 
+00002170: 6669 7273 7420 6d65 7373 6167 6520 746f  first message to
+00002180: 2061 6e6f 7468 6572 2063 6c69 7175 652e   another clique.
+00002190: 0a0a 2020 2020 2020 2020 4172 6775 6d65  ..        Argume
+000021a0: 6e74 730a 2020 2020 2020 2020 2d2d 2d2d  nts.        ----
+000021b0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 2a6f  -----.        *o
+000021c0: 7468 6572 5f63 6c69 7175 652a 203a 2061  ther_clique* : a
+000021d0: 2064 6966 6665 7265 6e74 2043 6c69 7175   different Cliqu
+000021e0: 6520 6f62 6a65 6374 0a0a 2020 2020 2020  e object..      
+000021f0: 2020 7a0b 496e 6974 204d 7367 3a20 0a4e    z.Init Msg: .N
+00002200: 290c 7202 0000 0072 4400 0000 7235 0000  ).r....rD...r5..
+00002210: 0072 3800 0000 7251 0000 005a 0f73 756d  .r8...rQ...Z.sum
+00002220: 6f75 745f 7661 725f 6c69 7374 7221 0000  out_var_listr!..
+00002230: 00da 0570 7269 6e74 7255 0000 0072 4600  ...printrU...rF.
+00002240: 0000 7217 0000 0072 4500 0000 2905 720c  ..r....rE...).r.
+00002250: 0000 0072 4d00 0000 5a08 7073 695f 636f  ...rM...Z.psi_co
+00002260: 7079 7235 0000 005a 0b73 756d 6f75 745f  pyr5...Z.sumout_
+00002270: 7661 7273 720d 0000 0072 0d00 0000 720e  varsr....r....r.
+00002280: 0000 00da 1473 656e 645f 696e 6974 6961  .....send_initia
+00002290: 6c5f 6d65 7373 6167 652e 0100 0073 0e00  l_message....s..
+000022a0: 0000 0a0b 0a01 0c01 0e02 0c05 0c01 1002  ................
+000022b0: 7a1b 436c 6971 7565 2e73 656e 645f 696e  z.Clique.send_in
+000022c0: 6974 6961 6c5f 6d65 7373 6167 6563 0100  itial_messagec..
+000022d0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+000022e0: 0000 4300 0000 7354 0000 0074 007c 006a  ..C...sT...t.|.j
+000022f0: 0183 0164 016b 0472 2274 027c 006a 0383  ...d.k.r"t.|.j..
+00002300: 017c 005f 047c 006a 0144 005d 097d 017c  .|._.|.j.D.].}.|
+00002310: 0004 006a 047c 0139 0002 005f 0471 107c  ...j.|.9..._.q.|
+00002320: 006a 0401 0067 007c 005f 0164 0253 0074  .j...g.|._.d.S.t
+00002330: 027c 006a 0483 017c 005f 0464 0253 0029  .|.j...|._.d.S.)
+00002340: 0361 5d02 0000 0a20 2020 2020 2020 2043  .a]....        C
+00002350: 6f6c 6c65 6374 696e 6720 6265 6c69 6566  ollecting belief
+00002360: 7320 6973 2064 6f6e 6520 6279 2074 616b  s is done by tak
+00002370: 696e 6720 7468 650a 2020 2020 2020 2020  ing the.        
+00002380: 706f 7465 6e74 6961 6c20 2873 656c 662e  potential (self.
+00002390: 7073 6929 206f 6620 5820 616e 6420 6d75  psi) of X and mu
+000023a0: 6c74 6970 6c79 696e 6720 6279 2061 6c6c  ltiplying by all
+000023b0: 206f 660a 2020 2020 2020 2020 7468 6520   of.        the 
+000023c0: 6d65 7373 6167 6573 2077 6869 6368 2058  messages which X
+000023d0: 2068 6173 2072 6563 6569 7665 642e 0a0a   has received...
+000023e0: 2020 2020 2020 2020 4e4f 5445 3a20 6f6e          NOTE: on
+000023f0: 6365 2062 656c 6965 6673 2061 7265 2063  ce beliefs are c
+00002400: 6f6c 6c65 6374 6564 2c20 7468 6520 6d65  ollected, the me
+00002410: 7373 6167 6573 0a20 2020 2020 2020 2077  ssages.        w
+00002420: 6869 6368 2074 6865 2043 6c69 7175 6520  hich the Clique 
+00002430: 6861 7320 7265 6365 6976 6564 2061 7265  has received are
+00002440: 2063 6c65 6172 6564 206f 7574 2e0a 0a20   cleared out... 
+00002450: 2020 2020 2020 204e 6f74 6573 0a20 2020         Notes.   
+00002460: 2020 2020 202d 2d2d 2d2d 0a20 2020 2020       -----.     
+00002470: 2020 2041 2072 6f6f 7420 6e6f 6465 2028     A root node (
+00002480: 692e 652e 206f 6e65 2074 6861 7420 646f  i.e. one that do
+00002490: 6573 6e27 7420 7365 6e64 2061 206d 6573  esn't send a mes
+000024a0: 7361 6765 2920 6d75 7374 2072 756e 2063  sage) must run c
+000024b0: 6f6c 6c65 6374 5f62 656c 6965 6673 0a20  ollect_beliefs. 
+000024c0: 2020 2020 2020 2073 696e 6365 2074 6865         since the
+000024d0: 7920 6172 6520 6f6e 6c79 2063 6f6c 6c65  y are only colle
+000024e0: 6374 6564 2061 7420 7365 6e64 5f6d 6573  cted at send_mes
+000024f0: 7361 6765 2829 0a0a 2020 2020 2020 2020  sage()..        
+00002500: 416c 736f 2c20 7765 2063 6f6c 6c65 6374  Also, we collect
+00002510: 2062 656c 6965 6673 2061 7420 7468 6520   beliefs at the 
+00002520: 656e 6420 6f66 206c 6f6f 7079 2062 656c  end of loopy bel
+00002530: 6965 6620 7072 6f70 6167 6174 696f 6e20  ief propagation 
+00002540: 2861 7070 726f 782e 2069 6e66 6572 656e  (approx. inferen
+00002550: 6365 290a 2020 2020 2020 2020 7369 6e63  ce).        sinc
+00002560: 6520 7468 6520 6d61 696e 2061 6c67 6f72  e the main algor
+00002570: 6974 686d 2069 7320 6a75 7374 2073 656e  ithm is just sen
+00002580: 6469 6e67 206d 6573 7361 6765 7320 666f  ding messages fo
+00002590: 7220 6120 7768 696c 652e 0a20 2020 2020  r a while..     
+000025a0: 2020 2072 0100 0000 4e29 0572 3400 0000     r....N).r4...
+000025b0: 7246 0000 0072 0200 0000 7244 0000 0072  rF...r....rD...r
+000025c0: 4500 0000 2902 720c 0000 0072 5300 0000  E...).r....rS...
+000025d0: 720d 0000 0072 0d00 0000 720e 0000 00da  r....r....r.....
+000025e0: 0f63 6f6c 6c65 6374 5f62 656c 6965 6673  .collect_beliefs
+000025f0: 4701 0000 730e 0000 000e 110c 010a 0110  G...s...........
+00002600: 0106 010a 0110 027a 1643 6c69 7175 652e  .......z.Clique.
+00002610: 636f 6c6c 6563 745f 6265 6c69 6566 7363  collect_beliefsc
+00002620: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00002630: 0300 0000 4300 0000 730e 0000 007c 006a  ....C...s....|.j
+00002640: 00a0 017c 016a 00a1 0153 0029 017a d20a  ...|.j...S.).z..
+00002650: 2020 2020 2020 2020 5468 6520 7365 7073          The seps
+00002660: 6574 206f 6620 7477 6f20 636c 6971 7565  et of two clique
+00002670: 7320 6973 2074 6865 2073 6574 206f 660a  s is the set of.
+00002680: 2020 2020 2020 2020 7661 7269 6162 6c65          variable
+00002690: 7320 696e 2074 6865 2069 6e74 6572 7365  s in the interse
+000026a0: 6374 696f 6e20 6f66 2074 6865 2074 776f  ction of the two
+000026b0: 0a20 2020 2020 2020 2063 6c69 7175 6573  .        cliques
+000026c0: 2720 7363 6f70 6573 2e0a 0a20 2020 2020  ' scopes...     
+000026d0: 2020 2041 7267 756d 656e 7473 0a20 2020     Arguments.   
+000026e0: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 0a20       ---------. 
+000026f0: 2020 2020 2020 202a 6f74 6865 725f 636c         *other_cl
+00002700: 6971 7565 2a20 3a20 6120 436c 6971 7565  ique* : a Clique
+00002710: 206f 626a 6563 740a 0a20 2020 2020 2020   object..       
+00002720: 2029 0272 3800 0000 da0c 696e 7465 7273   ).r8.....inters
+00002730: 6563 7469 6f6e 724c 0000 0072 0d00 0000  ectionrL...r....
+00002740: 720d 0000 0072 0e00 0000 7235 0000 0061  r....r....r5...a
+00002750: 0100 0073 0200 0000 0e0b 7a0d 436c 6971  ...s......z.Cliq
+00002760: 7565 2e73 6570 7365 7463 0200 0000 0000  ue.sepsetc......
+00002770: 0000 0000 0000 0300 0000 0300 0000 4300  ..............C.
+00002780: 0000 7318 0000 0074 007c 006a 0183 017d  ..s....t.|.j...}
+00002790: 027c 02a0 027c 01a1 0101 007c 0253 0029  .|...|.....|.S.)
+000027a0: 017a b00a 2020 2020 2020 2020 4d61 7267  .z..        Marg
+000027b0: 696e 616c 697a 6520 7468 6520 6370 7420  inalize the cpt 
+000027c0: 2862 656c 6965 6629 206f 7665 7220 6120  (belief) over a 
+000027d0: 7461 7267 6574 2076 6172 6961 626c 652e  target variable.
+000027e0: 0a0a 2020 2020 2020 2020 4172 6775 6d65  ..        Argume
+000027f0: 6e74 730a 2020 2020 2020 2020 2d2d 2d2d  nts.        ----
+00002800: 2d2d 2d2d 2d0a 2020 2020 2020 2020 2a74  -----.        *t
+00002810: 6172 6765 742a 203a 2061 2073 7472 696e  arget* : a strin
+00002820: 670a 2020 2020 2020 2020 2020 2020 5468  g.            Th
+00002830: 6520 7461 7267 6574 2072 616e 646f 6d20  e target random 
+00002840: 7661 7269 6162 6c65 2e0a 0a20 2020 2020  variable...     
+00002850: 2020 2029 0372 0200 0000 7245 0000 005a     ).r....rE...Z
+00002860: 0b73 756d 6f76 6572 5f76 6172 2903 720c  .sumover_var).r.
+00002870: 0000 00da 0674 6172 6765 745a 0362 6c66  .....targetZ.blf
+00002880: 720d 0000 0072 0d00 0000 720e 0000 00da  r....r....r.....
+00002890: 106d 6172 6769 6e61 6c69 7a65 5f6f 7665  .marginalize_ove
+000028a0: 726e 0100 0073 0600 0000 0a0a 0a01 0401  rn...s..........
+000028b0: 7a17 436c 6971 7565 2e6d 6172 6769 6e61  z.Clique.margina
+000028c0: 6c69 7a65 5f6f 7665 724e 290e 7240 0000  lize_overN).r@..
+000028d0: 0072 4100 0000 7242 0000 0072 4300 0000  .rA...rB...rC...
+000028e0: 720f 0000 0072 4900 0000 724e 0000 0072  r....rI...rN...r
+000028f0: 5000 0000 724b 0000 0072 3c00 0000 725c  P...rK...r<...r\
+00002900: 0000 0072 5d00 0000 7235 0000 0072 6000  ...r]...r5...r`.
+00002910: 0000 720d 0000 0072 0d00 0000 720d 0000  ..r....r....r...
+00002920: 0072 0e00 0000 7230 0000 00b2 0000 0073  .r....r0.......s
+00002930: 1800 0000 0800 0401 081b 0815 0803 0806  ................
+00002940: 0806 082b 0811 0819 081a 0c0d 7230 0000  ...+........r0..
+00002950: 0029 0b72 4300 0000 da0a 5f5f 6175 7468  .).rC.....__auth
+00002960: 6f72 5f5f da08 6e65 7477 6f72 6b78 721e  or__..networkxr.
+00002970: 0000 0072 0200 0000 da28 6261 6d74 2e65  ...r.....(bamt.e
+00002980: 7874 6572 6e61 6c2e 7079 424e 2e63 6c61  xternal.pyBN.cla
+00002990: 7373 6573 2e66 6163 746f 7269 7a61 7469  sses.factorizati
+000029a0: 6f6e 7203 0000 00da 1e62 616d 742e 6578  onr......bamt.ex
+000029b0: 7465 726e 616c 2e70 7942 4e2e 7574 696c  ternal.pyBN.util
+000029c0: 732e 6772 6170 68da 066f 626a 6563 7472  s.graph..objectr
+000029d0: 0500 0000 7230 0000 0072 0d00 0000 720d  ....r0...r....r.
+000029e0: 0000 0072 0d00 0000 720e 0000 00da 083c  ...r....r......<
+000029f0: 6d6f 6475 6c65 3e01 0000 0073 1200 0000  module>....s....
+00002a00: 0400 0421 0802 0c01 0c02 0802 1004 007f  ...!............
+00002a10: 1406                                     ..
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/inference/_tests/__pycache__/test_map_exact.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/inference/_tests/__pycache__/test_map_exact.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.33/bamt/external/pyBN/inference/_tests/__pycache__/test_marginal_approx.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/inference/_tests/__pycache__/test_marginal_approx.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.33/bamt/external/pyBN/inference/_tests/__pycache__/test_marginal_exact.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/inference/_tests/__pycache__/test_marginal_exact.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.33/bamt/external/pyBN/inference/map_exact/__pycache__/ilp_map.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/inference/map_exact/__pycache__/ilp_map.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 3333 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 050d 0000  o........l.b....
+00000000: 6f0d 0d0a 0000 0000 904d 2164 050d 0000  o........M!d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 5a03 6401 6404 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 0100 6900  ..d.d.l.m.Z...i.
 00000060: 6601 6406 6407 8401 5a08 6403 5300 2908  f.d.d...Z.d.S.).
 00000070: 7a24 4e2e 2043 756c 6c65 6e20 3c6e 6375  z$N. Cullen <ncu
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/inference/map_exact/__pycache__/ve_map.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/inference/map_exact/__pycache__/ve_map.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 1342 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 3e05 0000  o........l.b>...
+00000000: 6f0d 0d0a 0000 0000 904d 2164 3e05 0000  o........M!d>...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 5a00 6401 6402 6c01 6d01 5a01 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c02 5a03 6401 6404 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6401 6405 6c06 6d07 5a07 0100 6900  ..d.d.l.m.Z...i.
 00000060: 6403 6406 6603 6407 6408 8401 5a08 6403  d.d.f.d.d...Z.d.
 00000070: 5300 2909 7a24 4e2e 2043 756c 6c65 6e20  S.).z$N. Cullen
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/inference/marginal_approx/__pycache__/forward_sample.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/inference/marginal_approx/__pycache__/forward_sample.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 2067 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 1308 0000  o........l.b....
+00000000: 6f0d 0d0a 0000 0000 904d 2164 1308 0000  o........M!d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 5a07 6405 5a08 6409  ..d.d.l.Z.d.Z.d.
 00000060: 6407 6408 8401 5a09 6404 5300 290a e900  d.d...Z.d.S.)...
 00000070: 0000 0029 01da 0842 6179 6573 4e65 7429  ...)...BayesNet)
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/inference/marginal_approx/__pycache__/gibbs_sample.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/inference/marginal_approx/__pycache__/gibbs_sample.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 1963 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 ab07 0000  o........l.b....
+00000000: 6f0d 0d0a 0000 0000 904d 2164 ab07 0000  o........M!d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a04 6408 6406 6407 8401 5a05  d.l.Z.d.d.d...Z.
 00000050: 6403 5300 2909 7a24 4e2e 2043 756c 6c65  d.S.).z$N. Culle
 00000060: 6e20 3c6e 6375 6c6c 656e 2e74 6840 6461  n <ncullen.th@da
 00000070: 7274 6d6f 7574 682e 6564 753e e900 0000  rtmouth.edu>....
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/inference/marginal_approx/__pycache__/loopy_bp.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/inference/marginal_approx/__pycache__/loopy_bp.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 1861 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 4507 0000  o........l.bE...
+00000000: 6f0d 0d0a 0000 0000 904d 2164 4507 0000  o........M!dE...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1a00 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a02 6406 6404 6405  Z.d.d.l.Z.d.d.d.
 00000040: 8401 5a03 6402 5300 2907 7a24 4e2e 2043  ..Z.d.S.).z$N. C
 00000050: 756c 6c65 6e20 3c6e 6375 6c6c 656e 2e74  ullen <ncullen.t
 00000060: 6840 6461 7274 6d6f 7574 682e 6564 753e  h@dartmouth.edu>
 00000070: e900 0000 004e e964 0000 0063 0300 0000  .....N.d...c....
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/inference/marginal_approx/__pycache__/lw_sample.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/inference/marginal_approx/__pycache__/lw_sample.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 2216 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 a808 0000  o........l.b....
+00000000: 6f0d 0d0a 0000 0000 904d 2164 a808 0000  o........M!d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a04 6900 6403 6404 6603 6405  d.l.Z.i.d.d.f.d.
 00000050: 6406 8401 5a05 6403 5300 2907 7a24 4e2e  d...Z.d.S.).z$N.
 00000060: 2043 756c 6c65 6e20 3c6e 6375 6c6c 656e   Cullen <ncullen
 00000070: 2e74 6840 6461 7274 6d6f 7574 682e 6564  .th@dartmouth.ed
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/inference/marginal_exact/__pycache__/exact_bp.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/inference/marginal_exact/__pycache__/exact_bp.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 2813 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 fd0a 0000  o........l.b....
+00000000: 6f0d 0d0a 0000 0000 904d 2164 fd0a 0000  o........M!d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 5400 6401 6405 6c06 6d07 5a07 6d06 5a06  T.d.d.l.m.Z.m.Z.
 00000060: 0100 6401 6406 6c08 5a09 6401 6406 6c0a  ..d.d.l.Z.d.d.l.
 00000070: 5a0a 640a 6408 6409 8401 5a0b 6406 5300  Z.d.d.d...Z.d.S.
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/inference/marginal_exact/__pycache__/ve_marginal.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/inference/marginal_exact/__pycache__/ve_marginal.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 1307 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 1b05 0000  o........l.b....
+00000000: 6f0d 0d0a 0000 0000 904d 2164 1b05 0000  o........M!d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5400 0000 6400  .....@...sT...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 6d04 5a04 0100 6401 6404 6c05  d.l.m.Z...d.d.l.
 00000050: 5400 6401 6405 6c06 6d07 5a07 6d06 5a06  T.d.d.l.m.Z.m.Z.
 00000060: 0100 6401 6406 6c08 5a09 6401 6406 6c0a  ..d.d.l.Z.d.d.l.
 00000070: 5a0a 6900 6601 6407 6408 8401 5a0b 6406  Z.i.f.d.d...Z.d.
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/io/_tests/__pycache__/test_reading.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/io/_tests/__pycache__/test_reading.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.33/bamt/external/pyBN/io/_tests/__pycache__/test_writing.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/io/_tests/__pycache__/test_writing.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/parameter/__pycache__/bayes.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/parameter/__pycache__/bayes.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 3566 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 ee0d 0000  o........l.b....
+00000000: 6f0d 0d0a 0000 0000 904d 2164 ee0d 0000  o........M!d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6403  Z.d.d.l.m.Z...d.
 00000040: 5a03 6401 6404 6c04 5a05 6407 6405 6406  Z.d.d.l.Z.d.d.d.
 00000050: 8401 5a06 6404 5300 2908 7a51 0a2a 2a2a  ..Z.d.S.).zQ.***
 00000060: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
 00000070: 0a42 6179 6573 6961 6e20 4573 7469 6d61  .Bayesian Estima
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/parameter/__pycache__/mle.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/parameter/__pycache__/mle.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 5579 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 cb15 0000  o........l.b....
+00000000: 6f0d 0d0a 0000 0000 904d 2164 cb15 0000  o........M!d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6403  Z.d.d.l.m.Z...d.
 00000040: 5a03 6401 6404 6c04 5a05 640a 6406 6407  Z.d.d.l.Z.d.d.d.
 00000050: 8401 5a06 640b 6408 6409 8401 5a07 6404  ..Z.d.d.d...Z.d.
 00000060: 5300 290c 7a6f 0a2a 2a2a 2a2a 2a2a 2a2a  S.).zo.*********
 00000070: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ****************
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/__pycache__/__init__.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/structure/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 417 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 a101 0000  o........l.b....
+00000000: 6f0d 0d0a 0000 0000 904d 2164 a101 0000  o........M!d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 5400 6400 6401 6c01 5400 6400  d.l.T.d.d.l.T.d.
 00000040: 6401 6c02 5400 6400 6401 6c03 5400 6400  d.l.T.d.d.l.T.d.
 00000050: 6401 6c04 5400 6400 6401 6c05 5400 6400  d.l.T.d.d.l.T.d.
 00000060: 6401 6c06 5400 6402 5300 2903 e900 0000  d.l.T.d.S.).....
 00000070: 0029 01da 012a 4e29 07da 3062 616d 742e  .)...*N)..0bamt.
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/__pycache__/mdbn.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/structure/__pycache__/mdbn.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 3604 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 140e 0000  o........l.b....
+00000000: 6f0d 0d0a 0000 0000 904d 2164 140e 0000  o........M!d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 5a00 6401 5a01 6402 6403 6c02 6d03 5a03  Z.d.Z.d.d.l.m.Z.
 00000040: 0100 6402 6404 6c04 6d05 5a05 0100 6405  ..d.d.l.m.Z...d.
 00000050: 6406 8400 5a06 640c 6409 640a 8401 5a07  d...Z.d.d.d...Z.
 00000060: 640b 5300 290d 616c 0600 000a 4c65 6172  d.S.).al....Lear
 00000070: 6e20 6120 4d75 6c74 692d 4469 6d65 6e73  n a Multi-Dimens
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_chow_liu.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_chow_liu.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_grow_shrink.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_grow_shrink.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_orient_edges.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_orient_edges.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_pc.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_pc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/_tests/test_orient_edges.py` & `BAMT-1.1.40/bamt/external/pyBN/utils/_tests/test_orient_edges.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,26 +13,32 @@
 import numpy as np
 
 from external.pyBN.structure_learn.orient_edges import orient_edges_gs, orient_edges_pc
 
 
 class OrientEdgesTestCase(unittest.TestCase):
 
-	def setUp(self):
-		pass
-	def tearDown(self):
-		pass
-
-	def test_orient_edges_pc(self):
-		e = {0:[1,2],1:[0],2:[0]}
-		b = {0: [], 1: {2: (0,)}, 2: {1: (0,)}}
-		self.assertDictEqual(orient_edges_pc(e,b),
-			{0: [1, 2], 1: [], 2: []})
-
-	def test_orient_edges_gs(self):
-		e = {0: [1, 2], 1: [0], 2: [0]}
-		b = {0: [1, 2], 1: [0], 2: [0]}
-		dpath = os.path.join(dirname(dirname(dirname(dirname(__file__)))),'data')	
-		path = (os.path.join(dpath,'lizards.csv'))
-		data = np.loadtxt(path, dtype='int32',skiprows=1,delimiter=',')
-		self.assertDictEqual(orient_edges_gs(e,b,data,0.05),
-			{0: [1, 2], 1: [], 2: []})
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def test_orient_edges_pc(self):
+        e = {0: [1, 2], 1: [0], 2: [0]}
+        b = {0: [], 1: {2: (0,)}, 2: {1: (0,)}}
+        self.assertDictEqual(orient_edges_pc(e, b),
+                             {0: [1, 2], 1: [], 2: []})
+
+    def test_orient_edges_gs(self):
+        e = {0: [1, 2], 1: [0], 2: [0]}
+        b = {0: [1, 2], 1: [0], 2: [0]}
+        dpath = os.path.join(
+            dirname(
+                dirname(
+                    dirname(
+                        dirname(__file__)))),
+            'data')
+        path = (os.path.join(dpath, 'lizards.csv'))
+        data = np.loadtxt(path, dtype='int32', skiprows=1, delimiter=',')
+        self.assertDictEqual(orient_edges_gs(e, b, data, 0.05),
+                             {0: [1, 2], 1: [], 2: []})
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/constraint/__pycache__/__init__.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/structure/constraint/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 372 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 7401 0000  o........l.bt...
+00000000: 6f0d 0d0a 0000 0000 904d 2164 7401 0000  o........M!dt...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 5400 6400 6401 6c01 5400 6400  d.l.T.d.d.l.T.d.
 00000040: 6401 6c02 5400 6400 6401 6c03 5400 6400  d.l.T.d.d.l.T.d.
 00000050: 6401 6c04 5400 6402 5300 2903 e900 0000  d.l.T.d.S.).....
 00000060: 0029 01da 012a 4e29 055a 3a62 616d 742e  .)...*N).Z:bamt.
 00000070: 6578 7465 726e 616c 2e70 7942 4e2e 6c65  external.pyBN.le
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/constraint/__pycache__/fast_iamb.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/structure/constraint/__pycache__/fast_iamb.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 4530 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 b211 0000  o........l.b....
+00000000: 6f0d 0d0a 0000 0000 904d 2164 b211 0000  o........M!d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4600 0000 6400  .....@...sF...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a04 6401 6404 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000050: 6d07 5a07 0100 6401 6405 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 6d0a 5a0a 0100 640b 6409 640a 8401 5a0b  m.Z...d.d.d...Z.
 00000070: 6403 5300 290c 6184 0400 000a 2a2a 2a2a  d.S.).a.....****
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/constraint/__pycache__/grow_shrink.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/structure/constraint/__pycache__/grow_shrink.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 4648 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 2812 0000  o........l.b(...
+00000000: 6f0d 0d0a 0000 0000 904d 2164 2812 0000  o........M!d(...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5e00 0000 6400  .....@...s^...d.
 00000030: 5a00 6401 5a01 6402 6403 6c02 6d03 5a03  Z.d.Z.d.d.l.m.Z.
 00000040: 0100 6402 6404 6c04 6d05 5a05 0100 6402  ..d.d.l.m.Z...d.
 00000050: 6405 6c06 6d07 5a07 0100 6402 6406 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6402 6407 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6402 6408 6c0c 6d0c 5a0c 0100 640e  ..d.d.l.m.Z...d.
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/constraint/__pycache__/iamb.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/structure/constraint/__pycache__/iamb.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 4714 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 6a12 0000  o........l.bj...
+00000000: 6f0d 0d0a 0000 0000 904d 2164 6a12 0000  o........M!dj...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 5a00 6401 5a01 6402 6403 6c02 5a03 6402  Z.d.Z.d.d.l.Z.d.
 00000040: 6404 6c04 6d05 5a05 6d06 5a06 0100 6402  d.l.m.Z.m.Z...d.
 00000050: 6405 6c07 6d08 5a08 0100 6402 6406 6c09  d.l.m.Z...d.d.l.
 00000060: 6d0a 5a0a 0100 6402 6407 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 0100 640c 640a 640b 8401 5a0d 6403 5300  ..d.d.d...Z.d.S.
@@ -235,39 +235,39 @@
 00000ea0: 74da 0373 7472 da06 7265 6d6f 7665 7205  t..str..remover.
 00000eb0: 0000 0072 0400 0000 da03 7a69 70da 0154  ...r......zip..T
 00000ec0: 7206 0000 0029 13da 0464 6174 61da 0561  r....)...data..a
 00000ed0: 6c70 6861 da11 6665 6174 7572 655f 7365  lpha..feature_se
 00000ee0: 6c65 6374 696f 6eda 0564 6562 7567 da04  lection..debug..
 00000ef0: 6e5f 7276 da02 4d62 da02 5f54 721f 0000  n_rv..Mb.._Tr...
 00000f00: 00da 0156 5a09 4d62 5f63 6861 6e67 65da  ...VZ.Mb_change.
-00000f10: 076d 6178 5f76 616c da05 6d61 785f 78da  .max_val..max_x.
+00000f10: 076d 6178 5f76 616c 5a05 6d61 785f 78da  .max_valZ.max_x.
 00000f20: 0158 da04 636f 6c73 5a06 6d69 5f76 616c  .X..colsZ.mi_val
 00000f30: da09 6564 6765 5f64 6963 74da 126f 7269  ..edge_dict..ori
 00000f40: 656e 7465 645f 6564 6765 5f64 6963 74da  ented_edge_dict.
 00000f50: 0a76 616c 7565 5f64 6963 74da 0262 6e72  .value_dict..bnr
 00000f60: 0900 0000 7209 0000 0072 0c00 0000 da04  ....r....r......
 00000f70: 6961 6d62 3700 0000 7362 0000 000a 2116  iamb7...sb....!.
 00000f80: 0108 020a 0112 0206 0108 0312 0204 0104  ................
 00000f90: 0304 0104 0404 011a 0114 0118 0108 0104  ................
 00000fa0: 0104 0102 8014 021c 010e 0104 0104 0118  ................
 00000fb0: 0104 ed0c 161e 0216 010e 0104 0118 0102  ................
 00000fc0: 8002 fa0a 080a 0204 0110 0110 010e 0204  ................
 00000fd0: 0110 0110 030e 0106 ff0a 0204 0208 0272  ...............r
-00000fe0: 3000 0000 2903 7207 0000 004e 4629 0eda  0...).r....NF)..
+00000fe0: 2f00 0000 2903 7207 0000 004e 4629 0eda  /...).r....NF)..
 00000ff0: 075f 5f64 6f63 5f5f da0a 5f5f 6175 7468  .__doc__..__auth
 00001000: 6f72 5f5f da05 6e75 6d70 7972 1100 0000  or__..numpyr....
 00001010: da2b 6261 6d74 2e65 7874 6572 6e61 6c2e  .+bamt.external.
 00001020: 7079 424e 2e75 7469 6c73 2e69 6e64 6570  pyBN.utils.indep
 00001030: 656e 6465 6e63 655f 7465 7374 7372 0200  endence_testsr..
 00001040: 0000 7203 0000 00da 2562 616d 742e 6578  ..r.....%bamt.ex
 00001050: 7465 726e 616c 2e70 7942 4e2e 7574 696c  ternal.pyBN.util
 00001060: 732e 6f72 6965 6e74 5f65 6467 6573 7204  s.orient_edgesr.
 00001070: 0000 00da 2762 616d 742e 6578 7465 726e  ....'bamt.extern
 00001080: 616c 2e70 7942 4e2e 7574 696c 732e 6d61  al.pyBN.utils.ma
 00001090: 726b 6f76 5f62 6c61 6e6b 6574 7205 0000  rkov_blanketr...
 000010a0: 00da 2362 616d 742e 6578 7465 726e 616c  ..#bamt.external
 000010b0: 2e70 7942 4e2e 636c 6173 7365 732e 6261  .pyBN.classes.ba
-000010c0: 7965 736e 6574 7206 0000 0072 3000 0000  yesnetr....r0...
+000010c0: 7965 736e 6574 7206 0000 0072 2f00 0000  yesnetr....r/...
 000010d0: 7209 0000 0072 0900 0000 7209 0000 0072  r....r....r....r
 000010e0: 0c00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
 000010f0: 0000 7310 0000 0004 0004 2d08 0210 010c  ..s.......-.....
 00001100: 010c 010c 010e 03                        .......
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/constraint/__pycache__/lambda_iamb.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/structure/constraint/__pycache__/lambda_iamb.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 3170 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 620c 0000  o........l.bb...
+00000000: 6f0d 0d0a 0000 0000 904d 2164 620c 0000  o........M!db...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 5a04 6d05 5a05 0100 6408 6406 6407  m.Z.m.Z...d.d.d.
 00000050: 8401 5a06 6402 5300 2909 7a74 0a4c 616d  ..Z.d.S.).zt.Lam
 00000060: 6264 6120 4941 4d42 2043 6f64 650a 0a52  bda IAMB Code..R
 00000070: 6566 6572 656e 6365 730a 2d2d 2d2d 2d2d  eferences.------
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/constraint/__pycache__/path_condition.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/structure/constraint/__pycache__/path_condition.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 3561 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 e90d 0000  o........l.b....
+00000000: 6f0d 0d0a 0000 0000 904d 2164 e90d 0000  o........M!d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 5a00 6401 5a01 6402 6403 6c02 5a02 6402  Z.d.Z.d.d.l.Z.d.
 00000040: 6403 6c03 5a04 6402 6404 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6402 6405 6c07 6d08 5a08 0100 6402  ..d.d.l.m.Z...d.
 00000060: 6406 6c09 6d0a 5a0a 0100 640a 6408 6409  d.l.m.Z...d.d.d.
 00000070: 8401 5a0b 6403 5300 290b 61e2 0300 000a  ..Z.d.S.).a.....
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/exact/__pycache__/gobnilp.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/structure/exact/__pycache__/gobnilp.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 1533 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 fd05 0000  o........l.b....
+00000000: 6f0d 0d0a 0000 0000 904d 2164 fd05 0000  o........M!d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 5a01 6405 6403 6404 8401 5a02  Z.d.Z.d.d.d...Z.
 00000040: 6402 5300 2906 618d 0300 000a 474f 424e  d.S.).a.....GOBN
 00000050: 494c 5020 536f 6c76 6572 2066 6f72 2045  ILP Solver for E
 00000060: 7861 6374 2042 6179 6573 6961 6e20 6e65  xact Bayesian ne
 00000070: 7477 6f72 6b0a 5374 7275 6374 7572 6520  twork.Structure
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/hybrid/__pycache__/mmpc.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/structure/hybrid/__pycache__/mmpc.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 2471 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 a709 0000  o........l.b....
+00000000: 6f0d 0d0a 0000 0000 904d 2164 a709 0000  o........M!d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 5a04 0100 6407 6405 6406 8401 5a05  m.Z...d.d.d...Z.
 00000050: 6402 5300 2908 6100 0200 000a 4d61 782d  d.S.).a.....Max-
 00000060: 4d69 6e20 5061 7265 6e74 7320 616e 6420  Min Parents and 
 00000070: 4368 696c 6472 656e 2041 6c67 6f72 6974  Children Algorit
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/naive/__pycache__/naive_bayes.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/structure/naive/__pycache__/naive_bayes.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 1838 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 2e07 0000  o........l.b....
+00000000: 6f0d 0d0a 0000 0000 904d 2164 2e07 0000  o........M!d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 5a00 6401 5a01 6402 6403 6c02 5a03 6402  Z.d.Z.d.d.l.Z.d.
 00000040: 6404 6c04 6d05 5a05 0100 6402 6405 6c06  d.l.m.Z...d.d.l.
 00000050: 6d07 5a07 0100 6402 6406 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 640a 6408 6409 8401 5a0a 6403 5300  ..d.d.d...Z.d.S.
 00000070: 290b 7a70 0a2a 2a2a 2a2a 2a2a 2a2a 2a2a  ).zp.***********
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/naive/__pycache__/TAN.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/structure/naive/__pycache__/TAN.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 637 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 7d02 0000  o........l.b}...
+00000000: 6f0d 0d0a 0000 0000 904d 2164 7d02 0000  o........M!d}...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1000 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 8400 5a01 6403 5300 2904  Z.d.d...Z.d.S.).
 00000040: 7a84 0a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a  z..*************
 00000050: 2a0a 5472 6565 2041 7567 6d65 6e74 6564  *.Tree Augmented
 00000060: 200a 4e61 6976 6520 4261 7965 730a 2a2a   .Naive Bayes.**
 00000070: 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 0a0a 5441  ************..TA
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/score/__pycache__/__init__.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/structure/score/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 353 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 6101 0000  o........l.ba...
+00000000: 6f0d 0d0a 0000 0000 904d 2164 6101 0000  o........M!da...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 5400 6400 6401 6c01 5400 6400  d.l.T.d.d.l.T.d.
 00000040: 6401 6c02 5400 6400 6401 6c03 5400 6400  d.l.T.d.d.l.T.d.
 00000050: 6401 6c04 5400 6402 5300 2903 e900 0000  d.l.T.d.S.).....
 00000060: 0029 01da 012a 4e29 055a 3862 616d 742e  .)...*N).Z8bamt.
 00000070: 6578 7465 726e 616c 2e70 7942 4e2e 6c65  external.pyBN.le
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/score/__pycache__/bayes_scores.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/structure/score/__pycache__/bayes_scores.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 3797 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 d50e 0000  o........l.b....
+00000000: 6f0d 0d0a 0000 0000 904d 2164 d50e 0000  o........M!d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a04 6401 6404 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000050: 6d07 5a07 0100 6401 6405 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 6d0a 5a0a 0100 6401 6406 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
 00000070: 0100 640e 6408 6409 8401 5a0d 640e 640a  ..d.d.d...Z.d.d.
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/score/__pycache__/hill_climbing.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/structure/score/__pycache__/hill_climbing.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 11653 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 852d 0000  o........l.b.-..
+00000000: 6f0d 0d0a 0000 0000 904d 2164 852d 0000  o........M!d.-..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 6600 0000 6400  .....@...sf...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d04 5a04 0100 6401 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6405 6c07 6d08 5a08 0100 6401  ..d.d.l.m.Z...d.
 00000060: 6406 6c09 6d0a 5a0a 6d0b 5a0b 0100 6401  d.l.m.Z.m.Z...d.
 00000070: 6407 6c0c 6d0d 5a0d 0100 6401 6408 6c0e  d.l.m.Z...d.d.l.
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/score/__pycache__/info_scores.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/structure/score/__pycache__/info_scores.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 4754 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 9212 0000  o........l.b....
+00000000: 6f0d 0d0a 0000 0000 904d 2164 9212 0000  o........M!d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a04 6401 6404 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000050: 6d07 5a07 0100 640f 6406 6407 8401 5a08  m.Z...d.d.d...Z.
 00000060: 6408 6409 8400 5a09 640a 640b 8400 5a0a  d.d...Z.d.d...Z.
 00000070: 640c 6405 8400 5a0b 640d 640e 8400 5a0c  d.d...Z.d.d...Z.
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/score/__pycache__/random_restarts.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/structure/score/__pycache__/random_restarts.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 10519 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 1729 0000  o........l.b.)..
+00000000: 6f0d 0d0a 0000 0000 904d 2164 1729 0000  o........M!d.)..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7600 0000 6400  .....@...sv...d.
 00000030: 5a00 6401 5a01 6402 6403 6c02 5a03 6402  Z.d.Z.d.d.l.Z.d.
 00000040: 6404 6c04 6d04 5a04 6d05 5a05 0100 6402  d.l.m.Z.m.Z...d.
 00000050: 6405 6c06 6d07 5a07 0100 6402 6406 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6402 6407 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
 00000070: 0100 6402 6408 6c0c 6d0d 5a0d 0100 6402  ..d.d.l.m.Z...d.
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/score/__pycache__/tabu.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/structure/score/__pycache__/tabu.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 6771 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 731a 0000  o........l.bs...
+00000000: 6f0d 0d0a 0000 0000 904d 2164 731a 0000  o........M!ds...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
 00000030: 5a00 6401 6402 6c01 5a02 6401 6403 6c03  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6401 6404 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6401 6405 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6401 6406 6c09 6d0a 5a0a 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6407 6c0b 6d0c 5a0c 0100 6401 6408 6c0d  d.l.m.Z...d.d.l.
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/score/hill_climbing.py` & `BAMT-1.1.40/bamt/redef_HC.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 for Structure Learning
 **********************
 
 Code for Searching through the space of
 possible Bayesian Network structures.
 
 Various optimization procedures are employed,
-from greedy search to simulated annealing, and 
+from greedy search to simulated annealing, and
 so on - mostly using scipy.optimize.
 
 Local search - possible moves:
 - Add edge
 - Delete edge
 - Invert edge
 
@@ -22,59 +22,62 @@
     random steps and then start climbing again.
 - Tabu List
     - keep a list of the K steps most recently taken,
     and say that the search cannt reverse (undo) any
     of these steps.
 """
 
-#from scipy.optimize import *
-import numpy as np
-#from heapq import *
-
 from bamt.external.pyBN.classes.bayesnet import BayesNet
-from bamt.external.pyBN.learning.parameter.mle import mle_estimator
-from bamt.external.pyBN.learning.parameter.bayes import bayes_estimator
-from bamt.external.pyBN.utils.independence_tests import mutual_information, entropy
 from bamt.external.pyBN.utils.graph import would_cause_cycle
-from bamt.external.pyBN.learning.structure.score.info_scores import info_score
+from bamt.redef_info_scores import log_lik_local, BIC_local, AIC_local
+from bamt.mi_entropy_gauss import mi_gauss
 
 
-def hc(data, metric='LL', max_iter=100, debug=False, init_nodes=None, restriction=None, init_edges=None, remove_geo_edges=True, black_list=None):
+def hc(
+        data,
+        metric='MI',
+        max_iter=200,
+        debug=False,
+        init_nodes=None,
+        restriction=None,
+        init_edges=None,
+        remove_geo_edges=True,
+        black_list=None):
     """
     Greedy Hill Climbing search proceeds by choosing the move
     which maximizes the increase in fitness of the
     network at the current step. It continues until
     it reaches a point where there does not exist any
     feasible single move that increases the network fitness.
 
     It is called "greedy" because it simply does what is
     best at the current iteration only, and thus does not
     look ahead to what may be better later on in the search.
 
-    For computational saving, a Priority Queue (python's heapq) 
+    For computational saving, a Priority Queue (python's heapq)
     can be used	to maintain the best operators and reduce the
     complexity of picking the best operator from O(n^2) to O(nlogn).
     This works by maintaining the heapq of operators sorted by their
     delta score, and each time a move is made, we only have to recompute
     the O(n) delta-scores which were affected by the move. The rest of
     the operator delta-scores are not affected.
 
     For additional computational efficiency, we can cache the
-    sufficient statistics for various families of distributions - 
+    sufficient statistics for various families of distributions -
     therefore, computing the mutual information for a given family
     only needs to happen once.
 
     The possible moves are the following:
         - add edge
         - delete edge
         - invert edge
 
     Arguments
     ---------
-    *data* : a nested numpy array
+    *data* : pd.DataFrame
         The data from which the Bayesian network
         structure will be learned.
 
     *metric* : a string
         Which score metric to use.
         Options:
             - AIC
@@ -99,203 +102,213 @@
     Returns
     -------
     *bn* : a BayesNet object
 
     """
     nrow = data.shape[0]
     ncol = data.shape[1]
-    
+
     names = range(ncol)
 
     # INITIALIZE NETWORK W/ NO EDGES
     # maintain children and parents dict for fast lookups
-    c_dict = dict([(n,[]) for n in names])
-    p_dict = dict([(n,[]) for n in names])
+    c_dict = dict([(n, []) for n in names])
+    p_dict = dict([(n, []) for n in names])
     if init_edges:
         for edge in init_edges:
             c_dict[edge[0]].append(edge[1])
             p_dict[edge[1]].append(edge[0])
 
-    score_list = []
-    # COMPUTE INITIAL LIKELIHOOD SCORE	
-    value_dict = dict([(n, np.unique(data[:,i])) for i,n in enumerate(names)])
     bn = BayesNet(c_dict)
-    mle_estimator(bn, data)
-    max_score = info_score(bn, data, metric)
-    
 
-    # CREATE EMPIRICAL DISTRIBUTION OBJECT FOR CACHING
-    #ED = EmpiricalDistribution(data,names)
+    mutual_information = mi_gauss
+    if metric == 'BIC':
+        mutual_information = BIC_local
+    if metric == 'AIC':
+        mutual_information = AIC_local
+    if metric == 'LL':
+        mutual_information = log_lik_local
 
-    
+    data = data.values
+
+    cache = dict()
 
     _iter = 0
     improvement = True
 
     while improvement:
         improvement = False
         max_delta = 0
 
         if debug:
-            print('ITERATION: ' , _iter)
+            print('ITERATION: ', _iter)
 
         ### TEST ARC ADDITIONS ###
         for u in bn.nodes():
             for v in bn.nodes():
-                if v not in c_dict[u] and u!=v and not would_cause_cycle(c_dict, u, v) and len(p_dict[v]) != 3:
+                if v not in c_dict[u] and u != v and not would_cause_cycle(
+                        c_dict, u, v) and len(p_dict[v]) != 3:
                     # FOR MMHC ALGORITHM -> Edge Restrictions
-                    if (init_nodes is None or  not(v in init_nodes)) and (restriction is None or (u,v) in restriction) and (black_list is None or not((u,v) in black_list)):
+                    if (init_nodes is None or not (v in init_nodes)) and (
+                            restriction is None or (u, v) in restriction) and (
+                            black_list is None or not ((u, v) in black_list)):
                         # SCORE FOR 'V' -> gaining a parent
-                        old_cols = (v,) + tuple(p_dict[v]) # without 'u' as parent
-                        mi_old = mutual_information(data[:,old_cols])
-                        new_cols = old_cols + (u,) # with'u' as parent
-                        mi_new = mutual_information(data[:,new_cols])
+                        # without 'u' as parent
+                        old_cols = (v,) + tuple(p_dict[v])
+                        if old_cols not in cache:
+                            cache[old_cols] = mutual_information(
+                                data[:, old_cols])
+                        mi_old = cache[old_cols]
+                        new_cols = old_cols + (u,)  # with'u' as parent
+                        if new_cols not in cache:
+                            cache[new_cols] = mutual_information(
+                                data[:, new_cols])
+                        mi_new = cache[new_cols]
                         delta_score = nrow * (mi_old - mi_new)
-                        
+
                         if delta_score > max_delta:
                             if debug:
-                                print('Improved Arc Addition: ' , (u,v))
-                                print('Delta Score: ' , delta_score)
+                                print('Improved Arc Addition: ', (u, v))
+                                print('Delta Score: ', delta_score)
                             max_delta = delta_score
                             max_operation = 'Addition'
-                            max_arc = (u,v)
-                            
+                            max_arc = (u, v)
 
         # ### TEST ARC DELETIONS ###
         for u in bn.nodes():
             for v in bn.nodes():
                 if v in c_dict[u]:
                     # SCORE FOR 'V' -> losing a parent
-                    old_cols = (v,) + tuple(p_dict[v]) # with 'u' as parent
-                    mi_old = mutual_information(data[:,old_cols])
-                    new_cols = tuple([i for i in old_cols if i != u]) # without 'u' as parent
-                    mi_new = mutual_information(data[:,new_cols])
+                    old_cols = (v,) + tuple(p_dict[v])  # with 'u' as parent
+                    if old_cols not in cache:
+                        cache[old_cols] = mutual_information(data[:, old_cols])
+                    mi_old = cache[old_cols]
+                    new_cols = tuple([i for i in old_cols if i != u])
+                    if new_cols not in cache:
+                        cache[new_cols] = mutual_information(data[:, new_cols])
+                    mi_new = cache[new_cols]
                     delta_score = nrow * (mi_old - mi_new)
 
                     if (delta_score > max_delta):
-                        if init_edges == None:
+                        if init_edges is None:
                             if debug:
-                                print('Improved Arc Deletion: ' , (u,v))
-                                print('Delta Score: ' , delta_score)
+                                print('Improved Arc Deletion: ', (u, v))
+                                print('Delta Score: ', delta_score)
                             max_delta = delta_score
                             max_operation = 'Deletion'
-                            max_arc = (u,v)
+                            max_arc = (u, v)
                         else:
                             if (u, v) in init_edges:
                                 if remove_geo_edges:
                                     if debug:
-                                        print('Improved Arc Deletion: ' , (u,v))
-                                        print('Delta Score: ' , delta_score)
+                                        print(
+                                            'Improved Arc Deletion: ', (u, v))
+                                        print('Delta Score: ', delta_score)
                                     max_delta = delta_score
                                     max_operation = 'Deletion'
-                                    max_arc = (u,v)
+                                    max_arc = (u, v)
                             else:
                                 if debug:
-                                    print('Improved Arc Deletion: ' , (u,v))
-                                    print('Delta Score: ' , delta_score)
+                                    print('Improved Arc Deletion: ', (u, v))
+                                    print('Delta Score: ', delta_score)
                                 max_delta = delta_score
                                 max_operation = 'Deletion'
-                                max_arc = (u,v)
+                                max_arc = (u, v)
 
         # ### TEST ARC REVERSALS ###
         for u in bn.nodes():
             for v in bn.nodes():
-                if v in c_dict[u] and not would_cause_cycle(c_dict,v,u, reverse=True) and len(p_dict[u])!=3 and (init_nodes is None or not (u in init_nodes)) and (restriction is None or (v,u) in restriction) and (black_list is None or not((v,u) in black_list)):
-                    # SCORE FOR 'U' -> gaining 'v' as parent
-                    old_cols = (u,) + tuple(p_dict[v]) # without 'v' as parent
-                    mi_old = mutual_information(data[:,old_cols])
-                    new_cols = old_cols + (v,) # with 'v' as parent
-                    mi_new = mutual_information(data[:,new_cols])
-                    delta1 = -1* nrow * (mi_old - mi_new)
+                if v in c_dict[u] and not would_cause_cycle(
+                    c_dict, v, u, reverse=True) and len(
+                    p_dict[u]) != 3 and (
+                    init_nodes is None or not (
+                        u in init_nodes)) and (
+                    restriction is None or (
+                        v, u) in restriction) and (
+                            black_list is None or not (
+                                (v, u) in black_list)):
+                    old_cols = (u,) + tuple(p_dict[v])  # without 'v' as parent
+                    if old_cols not in cache:
+                        cache[old_cols] = mutual_information(data[:, old_cols])
+                    mi_old = cache[old_cols]
+                    new_cols = old_cols + (v,)  # with 'v' as parent
+                    if new_cols not in cache:
+                        cache[new_cols] = mutual_information(data[:, new_cols])
+                    mi_new = cache[new_cols]
+                    delta1 = -1 * nrow * (mi_old - mi_new)
                     # SCORE FOR 'V' -> losing 'u' as parent
-                    old_cols = (v,) + tuple(p_dict[v]) # with 'u' as parent
-                    mi_old = mutual_information(data[:,old_cols])
-                    new_cols = tuple([u for i in old_cols if i != u]) # without 'u' as parent
-                    mi_new = mutual_information(data[:,new_cols])
+                    old_cols = (v,) + tuple(p_dict[v])  # with 'u' as parent
+                    if old_cols not in cache:
+                        cache[old_cols] = mutual_information(data[:, old_cols])
+                    mi_old = cache[old_cols]
+                    # without 'u' as parent
+                    new_cols = tuple([u for i in old_cols if i != u])
+                    if new_cols not in cache:
+                        cache[new_cols] = mutual_information(data[:, new_cols])
+                    mi_new = cache[new_cols]
                     delta2 = nrow * (mi_old - mi_new)
                     # COMBINED DELTA-SCORES
                     delta_score = delta1 + delta2
 
                     if (delta_score > max_delta):
-                        if init_edges == None:
+                        if init_edges is None:
                             if debug:
-                                print('Improved Arc Reversal: ' , (u,v))
-                                print('Delta Score: ' , delta_score)
+                                print('Improved Arc Reversal: ', (u, v))
+                                print('Delta Score: ', delta_score)
                             max_delta = delta_score
                             max_operation = 'Reversal'
-                            max_arc = (u,v)
+                            max_arc = (u, v)
                         else:
                             if (u, v) in init_edges:
                                 if remove_geo_edges:
                                     if debug:
-                                        print('Improved Arc Reversal: ' , (u,v))
-                                        print('Delta Score: ' , delta_score)
+                                        print(
+                                            'Improved Arc Reversal: ', (u, v))
+                                        print('Delta Score: ', delta_score)
                                     max_delta = delta_score
                                     max_operation = 'Reversal'
-                                    max_arc = (u,v)
+                                    max_arc = (u, v)
                             else:
                                 if debug:
-                                    print('Improved Arc Reversal: ' , (u,v))
-                                    print('Delta Score: ' , delta_score)
+                                    print('Improved Arc Reversal: ', (u, v))
+                                    print('Delta Score: ', delta_score)
                                 max_delta = delta_score
                                 max_operation = 'Reversal'
-                                max_arc = (u,v)
-
-
-
-
-
-
-                        
+                                max_arc = (u, v)
 
         if max_delta != 0:
             improvement = True
-            u,v = max_arc
+            u, v = max_arc
             if max_operation == 'Addition':
                 if debug:
-                    print('ADDING: ' , max_arc , '\n')
+                    print('ADDING: ', max_arc, '\n')
                 c_dict[u].append(v)
                 p_dict[v].append(u)
-                
+
             elif max_operation == 'Deletion':
                 if debug:
-                    print('DELETING: ' , max_arc , '\n')
+                    print('DELETING: ', max_arc, '\n')
                 c_dict[u].remove(v)
                 p_dict[v].remove(u)
-                
+
             elif max_operation == 'Reversal':
                 if debug:
-                    print('REVERSING: ' , max_arc, '\n')
+                    print('REVERSING: ', max_arc, '\n')
                 c_dict[u].remove(v)
                 p_dict[v].remove(u)
                 c_dict[v].append(u)
                 p_dict[u].append(v)
-            
+
         else:
             if debug:
-                print('No Improvement on Iter: ' , _iter)
+                print('No Improvement on Iter: ', _iter)
 
         ### TEST FOR MAX ITERATION ###
         _iter += 1
         if _iter > max_iter:
             if debug:
                 print('Max Iteration Reached')
             break
 
-    
     bn = BayesNet(c_dict)
-    
-    
-    return bn
-
-
-
-
-
-
-
-
-
-
-
-
 
+    return bn
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/learning/structure/tree/__pycache__/chow_liu.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/learning/structure/tree/__pycache__/chow_liu.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 18 14:22:44 2022 UTC, .py size: 1636 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b46c d562 6406 0000  o........l.bd...
+00000000: 6f0d 0d0a 0000 0000 904d 2164 6406 0000  o........M!dd...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 5a00 6401 5a01 6402 6403 6c02 6d03 5a03  Z.d.Z.d.d.l.m.Z.
 00000040: 0100 6402 6404 6c04 6d05 5a05 0100 6402  ..d.d.l.m.Z...d.
 00000050: 6405 6c06 5a06 6402 6405 6c07 5a08 6409  d.l.Z.d.d.l.Z.d.
 00000060: 6407 6408 8401 5a09 6405 5300 290a 7ad5  d.d...Z.d.S.).z.
 00000070: 0a2a 2a2a 2a2a 2a2a 2a2a 2a2a 2a2a 0a43  .*************.C
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/utils/_tests/__pycache__/test_independence_tests.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/utils/_tests/__pycache__/test_independence_tests.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.33/bamt/external/pyBN/utils/_tests/__pycache__/test_markov_blanket.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/utils/_tests/__pycache__/test_markov_blanket.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.33/bamt/external/pyBN/utils/_tests/__pycache__/test_orient_edges.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/utils/_tests/__pycache__/test_orient_edges.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.33/bamt/external/pyBN/utils/_tests/__pycache__/test_random_sample.cpython-310.pyc` & `BAMT-1.1.40/bamt/external/pyBN/utils/_tests/__pycache__/test_random_sample.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.33/bamt/external/pyBN/utils/class_equivalence.py` & `BAMT-1.1.40/bamt/external/pyBN/utils/class_equivalence.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,24 +9,25 @@
 edges when viewed as undirected graphs.
 
 Also, this code is for actually generating
 equivalent Bayesian networks from a given BN.
 
 """
 
-def are_class_equivalent(x,y):
-	"""
-	Check whether two Bayesian networks belong
-	to the same equivalence class.
-	"""
-	are_equivalent = True
 
-	if set(list(x.nodes())) != set(list(y.nodes())):
-		are_equivalent = False
-	else:
-		for rv in x.nodes():
-			rv_x_neighbors = set(x.parents(rv)) + set(y.children(rv))
-			rv_y_neighbors = set(y.parents(rv)) + set(y.children(rv))
-			if rv_x_neighbors != rv_y_neighbors:
-				are_equivalent =  False
-				break
-	return are_equivalent
+def are_class_equivalent(x, y):
+    """
+    Check whether two Bayesian networks belong
+    to the same equivalence class.
+    """
+    are_equivalent = True
+
+    if set(list(x.nodes())) != set(list(y.nodes())):
+        are_equivalent = False
+    else:
+        for rv in x.nodes():
+            rv_x_neighbors = set(x.parents(rv)) + set(y.children(rv))
+            rv_y_neighbors = set(y.parents(rv)) + set(y.children(rv))
+            if rv_x_neighbors != rv_y_neighbors:
+                are_equivalent = False
+                break
+    return are_equivalent
```

### Comparing `BAMT-1.1.33/bamt/external/pyBN/utils/structure_distance.py` & `BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/structure_distance.cpython-310.pyc`

 * *Files 23% similar despite different names*

```diff
@@ -1,172 +1,181 @@
-00000000: 2222 220d 0a2a 2a2a 2a2a 2a2a 2a2a 2a2a  """..***********
-00000010: 2a2a 2a2a 2a0d 0a42 4e20 5374 7275 6374  *****..BN Struct
-00000020: 7572 6520 0d0a 4469 7374 616e 6365 204d  ure ..Distance M
-00000030: 6574 7269 6373 0d0a 2a2a 2a2a 2a2a 2a2a  etrics..********
-00000040: 2a2a 2a2a 2a2a 2a2a 0d0a 0d0a 436f 6465  ********....Code
-00000050: 2066 6f72 2063 6f6d 7075 7469 6e67 2074   for computing t
-00000060: 6865 2073 7472 7563 7475 7261 6c20 4469  he structural Di
-00000070: 7374 616e 6365 0d0a 6265 7477 6565 6e20  stance..between 
-00000080: 322b 2042 6179 6573 6961 6e20 6e65 7477  2+ Bayesian netw
-00000090: 6f72 6b73 2e20 4e6f 7465 2c20 7468 6973  orks. Note, this
-000000a0: 0d0a 636f 6465 2063 6f6d 7061 7265 7320  ..code compares 
-000000b0: 6f6e 6c79 2073 7472 7563 7475 7265 202d  only structure -
-000000c0: 2069 2e65 2e20 7468 650d 0a63 6f6e 6469   i.e. the..condi
-000000d0: 7469 6f6e 616c 2028 696e 2964 6570 656e  tional (in)depen
-000000e0: 6465 6e63 6965 732e 2046 6f72 2061 2063  dencies. For a c
-000000f0: 6f6d 7061 7269 736f 6e0d 0a6f 6620 636f  omparison..of co
-00000100: 6e64 6974 696f 6e61 6c20 7072 6f62 6162  nditional probab
-00000110: 696c 6974 7920 7661 6c75 6573 206f 6620  ility values of 
-00000120: 322b 2042 4e73 2c0d 0a73 6565 2022 7061  2+ BNs,..see "pa
-00000130: 7261 6d65 7465 725f 6469 7374 616e 6365  rameter_distance
-00000140: 2e70 7922 0d0a 0d0a 466f 7220 636f 6d70  .py"....For comp
-00000150: 7574 696e 6720 6469 7374 616e 6365 206d  uting distance m
-00000160: 6574 7269 6373 2074 6861 7420 696e 636c  etrics that incl
-00000170: 7564 650d 0a62 6f74 6820 7374 7275 6374  ude..both struct
-00000180: 7572 6520 414e 4420 7061 7261 6d65 7465  ure AND paramete
-00000190: 7273 2c20 7365 6520 2268 7962 7269 645f  rs, see "hybrid_
-000001a0: 6469 7374 616e 6365 2e70 7922 0d0a 0d0a  distance.py"....
-000001b0: 4d65 7472 6963 730d 0a2d 2d2d 2d2d 2d2d  Metrics..-------
-000001c0: 0d0a 312e 204d 6973 7369 6e67 2045 6467  ..1. Missing Edg
-000001d0: 6573 3a20 0d0a 0963 6f75 6e74 7320 6564  es: ...counts ed
-000001e0: 6765 7320 7468 6174 2061 7265 2070 7265  ges that are pre
-000001f0: 7365 6e74 2069 6e20 7468 6520 6f72 6967  sent in the orig
-00000200: 696e 616c 2073 7472 7563 7475 7265 2062  inal structure b
-00000210: 7574 0d0a 0961 7265 206d 6973 7369 6e67  ut...are missing
-00000220: 2069 6e20 7468 6520 6c65 6172 6e65 6420   in the learned 
-00000230: 7374 7275 6374 7572 652e 2028 6c6f 7765  structure. (lowe
-00000240: 7220 6973 2062 6574 7465 7229 205b 315d  r is better) [1]
-00000250: 0d0a 0d0a 322e 2045 7874 7261 2045 6467  ....2. Extra Edg
-00000260: 6573 3a20 0d0a 0963 6f75 6e74 7320 6564  es: ...counts ed
-00000270: 6765 7320 7468 6174 2061 7265 2066 6f75  ges that are fou
-00000280: 6e64 2069 6e20 7468 6520 6c65 6172 6e65  nd in the learne
-00000290: 6420 7374 7275 6374 7572 6520 6275 7420  d structure but 
-000002a0: 6172 650d 0a09 6e6f 7420 7072 6573 656e  are...not presen
-000002b0: 7420 696e 2074 6865 206f 7269 6769 6e61  t in the origina
-000002c0: 6c20 7374 7275 6374 7572 652e 2028 6c6f  l structure. (lo
-000002d0: 7765 7220 6973 2062 6574 7465 7229 205b  wer is better) [
-000002e0: 315d 0d0a 0d0a 332e 2049 6e63 6f72 7265  1]....3. Incorre
-000002f0: 6374 2045 6467 6520 4469 7265 6374 696f  ct Edge Directio
-00000300: 6e3a 200d 0a09 636f 756e 7473 2064 6972  n: ...counts dir
-00000310: 6563 7465 6420 6564 6765 7320 696e 2074  ected edges in t
-00000320: 6865 206c 6561 726e 6564 2073 7472 7563  he learned struc
-00000330: 7475 7265 0d0a 0974 6861 7420 6172 6520  ture...that are 
-00000340: 6f72 6965 6e74 6564 2069 6e63 6f72 7265  oriented incorre
-00000350: 6374 6c79 2e20 286c 6f77 6572 2069 7320  ctly. (lower is 
-00000360: 6265 7474 6572 2920 5b31 5d0d 0a0d 0a34  better) [1]....4
-00000370: 2e20 4861 6d6d 696e 6720 4469 7374 616e  . Hamming Distan
-00000380: 6365 3a20 0d0a 0944 6573 6372 6962 6573  ce: ...Describes
-00000390: 2074 6865 206e 756d 6265 7220 6f66 2063   the number of c
-000003a0: 6861 6e67 6573 2074 6861 7420 6861 7665  hanges that have
-000003b0: 2074 6f20 6265 206d 6164 650d 0a09 746f   to be made...to
-000003c0: 2061 206e 6574 776f 726b 2066 6f72 2069   a network for i
-000003d0: 7420 746f 2074 7572 6e20 696e 746f 2074  t to turn into t
-000003e0: 6865 206f 6e65 2074 6861 7420 6974 2069  he one that it i
-000003f0: 7320 6265 696e 6720 636f 6d70 6172 6564  s being compared
-00000400: 2077 6974 682e 2049 7420 6973 2074 6865   with. It is the
-00000410: 0d0a 0973 756d 206f 6620 6d65 6173 7572  ...sum of measur
-00000420: 6573 2031 2c20 322c 2061 6e64 2033 2e20  es 1, 2, and 3. 
-00000430: 5665 7273 696f 6e73 206f 6620 7468 6520  Versions of the 
-00000440: 4861 6d6d 696e 6720 6469 7374 616e 6365  Hamming distance
-00000450: 206d 6574 7269 6320 6861 7665 0d0a 0962   metric have...b
-00000460: 6565 6e20 7072 6f70 6f73 6564 2062 7920  een proposed by 
-00000470: 4163 6964 2061 6e64 2064 6520 4361 6d70  Acid and de Camp
-00000480: 6f73 2028 3230 3033 292c 2054 7361 6d61  os (2003), Tsama
-00000490: 7264 696e 6f73 2065 7420 616c 2e20 2832  rdinos et al. (2
-000004a0: 3030 3629 2c20 616e 640d 0a09 5065 7272  006), and...Perr
-000004b0: 6965 7220 6574 2061 6c2e 2028 3230 3038  ier et al. (2008
-000004c0: 292e 2028 6c6f 7765 7220 6973 2062 6574  ). (lower is bet
-000004d0: 7465 7229 205b 315d 0d0a 0d0a 0d0a 5265  ter) [1]......Re
-000004e0: 6665 7265 6e63 6573 0d0a 2d2d 2d2d 2d2d  ferences..------
-000004f0: 2d2d 2d2d 0d0a 5b31 5d20 4d61 7274 696a  ----..[1] Martij
-00000500: 6e20 6465 204a 6f6e 6768 2061 6e64 204d  n de Jongh and M
-00000510: 6172 656b 204a 2e20 4472 757a 647a 656c  arek J. Druzdzel
-00000520: 0d0a 0922 4120 436f 6d70 6172 6973 6f6e  ..."A Comparison
-00000530: 206f 6620 5374 7275 6374 7572 616c 2044   of Structural D
-00000540: 6973 7461 6e63 6520 4d65 6173 7572 6573  istance Measures
-00000550: 0d0a 0966 6f72 2043 6175 7361 6c20 4261  ...for Causal Ba
-00000560: 7965 7369 616e 204e 6574 776f 726b 204d  yesian Network M
-00000570: 6f64 656c 7322 0d0a 0d0a 0d0a 2222 220d  odels"......""".
-00000580: 0a0d 0a5f 5f61 7574 686f 725f 5f20 3d20  ...__author__ = 
-00000590: 2222 224e 6963 686f 6c61 7320 4375 6c6c  """Nicholas Cull
-000005a0: 656e 203c 6e63 756c 6c65 6e2e 7468 4064  en <ncullen.th@d
-000005b0: 6172 746d 6f75 7468 2e65 6475 3e22 2222  artmouth.edu>"""
-000005c0: 0d0a 0d0a 696d 706f 7274 206e 756d 7079  ....import numpy
-000005d0: 2061 7320 6e70 0d0a 0d0a 6465 6620 6d69   as np....def mi
-000005e0: 7373 696e 675f 6564 6765 7328 782c 7929  ssing_edges(x,y)
-000005f0: 3a0d 0a09 2222 220d 0a09 436f 756e 7473  :..."""...Counts
-00000600: 2065 6467 6573 2074 6861 7420 6172 6520   edges that are 
-00000610: 7072 6573 656e 7420 696e 2074 6865 206f  present in the o
-00000620: 7269 6769 6e61 6c20 7374 7275 6374 7572  riginal structur
-00000630: 6520 2878 2920 6275 740d 0a09 6172 6520  e (x) but...are 
-00000640: 6d69 7373 696e 6720 696e 2074 6865 206c  missing in the l
-00000650: 6561 726e 6564 2073 7472 7563 7475 7265  earned structure
-00000660: 2028 7929 2e20 286c 6f77 6572 2069 7320   (y). (lower is 
-00000670: 6265 7474 6572 290d 0a09 2222 220d 0a09  better)..."""...
-00000680: 6d69 7373 696e 6720 3d20 300d 0a09 666f  missing = 0...fo
-00000690: 7220 7276 2069 6e20 782e 6e6f 6465 7328  r rv in x.nodes(
-000006a0: 293a 0d0a 0909 6966 206e 6f74 2079 2e68  ):....if not y.h
-000006b0: 6173 5f6e 6f64 6528 7276 293a 0d0a 0909  as_node(rv):....
-000006c0: 096d 6973 7369 6e67 202b 3d20 782e 6465  .missing += x.de
-000006d0: 6772 6565 2872 7629 0d0a 0909 656c 7365  gree(rv)....else
-000006e0: 3a0d 0a09 0909 666f 7220 6368 696c 6420  :.....for child 
-000006f0: 696e 2078 2e63 6869 6c64 7265 6e28 7276  in x.children(rv
-00000700: 293a 0d0a 0909 0909 6966 2063 6869 6c64  ):......if child
-00000710: 206e 6f74 2069 6e20 792e 6368 696c 6472   not in y.childr
-00000720: 656e 2872 7629 3a0d 0a09 0909 0909 6d69  en(rv):.......mi
-00000730: 7373 696e 6720 2b3d 2031 0d0a 0972 6574  ssing += 1...ret
-00000740: 7572 6e20 6d69 7373 696e 670d 0a0d 0a64  urn missing....d
-00000750: 6566 2065 7874 7261 5f65 6467 6573 2878  ef extra_edges(x
-00000760: 2c79 293a 0d0a 0922 2222 0d0a 0943 6f75  ,y):..."""...Cou
-00000770: 6e74 7320 6564 6765 7320 7468 6174 2061  nts edges that a
-00000780: 7265 2066 6f75 6e64 2069 6e20 7468 6520  re found in the 
-00000790: 6c65 6172 6e65 6420 7374 7275 6374 7572  learned structur
-000007a0: 6520 6275 7420 6172 650d 0a09 6e6f 7420  e but are...not 
-000007b0: 7072 6573 656e 7420 696e 2074 6865 206f  present in the o
-000007c0: 7269 6769 6e61 6c20 7374 7275 6374 7572  riginal structur
-000007d0: 652e 2028 6c6f 7765 7220 6973 2062 6574  e. (lower is bet
-000007e0: 7465 7229 0d0a 0922 2222 0d0a 0965 7874  ter)..."""...ext
-000007f0: 7261 203d 2030 0d0a 0966 6f72 2072 7620  ra = 0...for rv 
-00000800: 696e 2079 2e6e 6f64 6573 2829 3a0d 0a09  in y.nodes():...
-00000810: 0969 6620 6e6f 7420 782e 6861 735f 6e6f  .if not x.has_no
-00000820: 6465 2872 7629 3a0d 0a09 0909 6578 7472  de(rv):.....extr
-00000830: 6120 2b3d 2079 2e64 6567 7265 6528 7276  a += y.degree(rv
-00000840: 290d 0a09 0965 6c73 653a 0d0a 0909 0966  )....else:.....f
-00000850: 6f72 2063 6869 6c64 2069 6e20 792e 6368  or child in y.ch
-00000860: 696c 6472 656e 2872 7629 3a0d 0a09 0909  ildren(rv):.....
-00000870: 0969 6620 6368 696c 6420 6e6f 7420 696e  .if child not in
-00000880: 2078 2e63 6869 6c64 7265 6e28 7276 293a   x.children(rv):
-00000890: 0d0a 0909 0909 0965 7874 7261 202b 3d20  .......extra += 
-000008a0: 310d 0a09 7265 7475 726e 2065 7874 7261  1...return extra
-000008b0: 0d0a 0d0a 6465 6620 696e 636f 7272 6563  ....def incorrec
-000008c0: 745f 6469 7265 6374 696f 6e5f 6564 6765  t_direction_edge
-000008d0: 7328 782c 7929 3a0d 0a09 2222 220d 0a09  s(x,y):..."""...
-000008e0: 436f 756e 7473 2064 6972 6563 7465 6420  Counts directed 
-000008f0: 6564 6765 7320 696e 2074 6865 206c 6561  edges in the lea
-00000900: 726e 6564 2073 7472 7563 7475 7265 0d0a  rned structure..
-00000910: 0974 6861 7420 6172 6520 6f72 6965 6e74  .that are orient
-00000920: 6564 2069 6e63 6f72 7265 6374 6c79 2e20  ed incorrectly. 
-00000930: 286c 6f77 6572 2069 7320 6265 7474 6572  (lower is better
-00000940: 290d 0a09 2222 220d 0a09 696e 636f 7272  )..."""...incorr
-00000950: 6563 745f 6469 7265 6374 696f 6e20 3d20  ect_direction = 
-00000960: 300d 0a09 666f 7220 7276 2069 6e20 782e  0...for rv in x.
-00000970: 6e6f 6465 7328 293a 0d0a 0909 6966 2078  nodes():....if x
-00000980: 2e68 6173 5f6e 6f64 6528 7276 293a 0d0a  .has_node(rv):..
-00000990: 0909 0966 6f72 2063 6869 6c64 2069 6e20  ...for child in 
-000009a0: 782e 6368 696c 6472 656e 2872 7629 3a20  x.children(rv): 
-000009b0: 2320 6368 696c 6420 6973 2072 7627 7320  # child is rv's 
-000009c0: 6368 696c 6420 696e 2078 0d0a 0909 0909  child in x......
-000009d0: 6966 2072 7620 696e 2079 2e70 6172 656e  if rv in y.paren
-000009e0: 7473 2872 7629 3a20 2320 6368 696c 6420  ts(rv): # child 
-000009f0: 6973 2072 7627 7320 7061 7265 6e74 2069  is rv's parent i
-00000a00: 6e20 790d 0a09 0909 0909 696e 636f 7272  n y.......incorr
-00000a10: 6563 745f 6469 7265 6374 696f 6e20 2b3d  ect_direction +=
-00000a20: 2031 0d0a 0972 6574 7572 6e20 696e 636f   1...return inco
-00000a30: 7272 6563 745f 6469 7265 6374 696f 6e0d  rrect_direction.
-00000a40: 0a0d 0a64 6566 2068 616d 6d69 6e67 2878  ...def hamming(x
-00000a50: 2c79 293a 0d0a 0972 6574 7572 6e20 6d69  ,y):...return mi
-00000a60: 7373 696e 675f 6564 6765 7328 782c 7929  ssing_edges(x,y)
-00000a70: 202b 2065 7874 7261 5f65 6467 6573 2878   + extra_edges(x
-00000a80: 2c79 2920 2b20 696e 636f 7272 6563 745f  ,y) + incorrect_
-00000a90: 6469 7265 6374 696f 6e5f 6564 6765 7328  direction_edges(
-00000aa0: 782c 7929 0d0a 090d 0a0d 0a0d 0a0d 0a0d  x,y)............
-00000ab0: 0a0d 0a0d 0a0d 0a0d 0a                   .........
+00000000: 6f0d 0d0a 0000 0000 904d 2164 b90a 0000  o........M!d....
+00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
+00000020: 0002 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
+00000030: 5a00 6401 5a01 6402 6403 6c02 5a03 6404  Z.d.Z.d.d.l.Z.d.
+00000040: 6405 8400 5a04 6406 6407 8400 5a05 6408  d...Z.d.d...Z.d.
+00000050: 6409 8400 5a06 640a 640b 8400 5a07 6403  d...Z.d.d...Z.d.
+00000060: 5300 290c 614c 0500 000a 2a2a 2a2a 2a2a  S.).aL....******
+00000070: 2a2a 2a2a 2a2a 2a2a 2a2a 0a42 4e20 5374  **********.BN St
+00000080: 7275 6374 7572 6520 0a44 6973 7461 6e63  ructure .Distanc
+00000090: 6520 4d65 7472 6963 730a 2a2a 2a2a 2a2a  e Metrics.******
+000000a0: 2a2a 2a2a 2a2a 2a2a 2a2a 0a0a 436f 6465  **********..Code
+000000b0: 2066 6f72 2063 6f6d 7075 7469 6e67 2074   for computing t
+000000c0: 6865 2073 7472 7563 7475 7261 6c20 4469  he structural Di
+000000d0: 7374 616e 6365 0a62 6574 7765 656e 2032  stance.between 2
+000000e0: 2b20 4261 7965 7369 616e 206e 6574 776f  + Bayesian netwo
+000000f0: 726b 732e 204e 6f74 652c 2074 6869 730a  rks. Note, this.
+00000100: 636f 6465 2063 6f6d 7061 7265 7320 6f6e  code compares on
+00000110: 6c79 2073 7472 7563 7475 7265 202d 2069  ly structure - i
+00000120: 2e65 2e20 7468 650a 636f 6e64 6974 696f  .e. the.conditio
+00000130: 6e61 6c20 2869 6e29 6465 7065 6e64 656e  nal (in)dependen
+00000140: 6369 6573 2e20 466f 7220 6120 636f 6d70  cies. For a comp
+00000150: 6172 6973 6f6e 0a6f 6620 636f 6e64 6974  arison.of condit
+00000160: 696f 6e61 6c20 7072 6f62 6162 696c 6974  ional probabilit
+00000170: 7920 7661 6c75 6573 206f 6620 322b 2042  y values of 2+ B
+00000180: 4e73 2c0a 7365 6520 2270 6172 616d 6574  Ns,.see "paramet
+00000190: 6572 5f64 6973 7461 6e63 652e 7079 220a  er_distance.py".
+000001a0: 0a46 6f72 2063 6f6d 7075 7469 6e67 2064  .For computing d
+000001b0: 6973 7461 6e63 6520 6d65 7472 6963 7320  istance metrics 
+000001c0: 7468 6174 2069 6e63 6c75 6465 0a62 6f74  that include.bot
+000001d0: 6820 7374 7275 6374 7572 6520 414e 4420  h structure AND 
+000001e0: 7061 7261 6d65 7465 7273 2c20 7365 6520  parameters, see 
+000001f0: 2268 7962 7269 645f 6469 7374 616e 6365  "hybrid_distance
+00000200: 2e70 7922 0a0a 4d65 7472 6963 730a 2d2d  .py"..Metrics.--
+00000210: 2d2d 2d2d 2d0a 312e 204d 6973 7369 6e67  -----.1. Missing
+00000220: 2045 6467 6573 3a20 0a09 636f 756e 7473   Edges: ..counts
+00000230: 2065 6467 6573 2074 6861 7420 6172 6520   edges that are 
+00000240: 7072 6573 656e 7420 696e 2074 6865 206f  present in the o
+00000250: 7269 6769 6e61 6c20 7374 7275 6374 7572  riginal structur
+00000260: 6520 6275 740a 0961 7265 206d 6973 7369  e but..are missi
+00000270: 6e67 2069 6e20 7468 6520 6c65 6172 6e65  ng in the learne
+00000280: 6420 7374 7275 6374 7572 652e 2028 6c6f  d structure. (lo
+00000290: 7765 7220 6973 2062 6574 7465 7229 205b  wer is better) [
+000002a0: 315d 0a0a 322e 2045 7874 7261 2045 6467  1]..2. Extra Edg
+000002b0: 6573 3a20 0a09 636f 756e 7473 2065 6467  es: ..counts edg
+000002c0: 6573 2074 6861 7420 6172 6520 666f 756e  es that are foun
+000002d0: 6420 696e 2074 6865 206c 6561 726e 6564  d in the learned
+000002e0: 2073 7472 7563 7475 7265 2062 7574 2061   structure but a
+000002f0: 7265 0a09 6e6f 7420 7072 6573 656e 7420  re..not present 
+00000300: 696e 2074 6865 206f 7269 6769 6e61 6c20  in the original 
+00000310: 7374 7275 6374 7572 652e 2028 6c6f 7765  structure. (lowe
+00000320: 7220 6973 2062 6574 7465 7229 205b 315d  r is better) [1]
+00000330: 0a0a 332e 2049 6e63 6f72 7265 6374 2045  ..3. Incorrect E
+00000340: 6467 6520 4469 7265 6374 696f 6e3a 200a  dge Direction: .
+00000350: 0963 6f75 6e74 7320 6469 7265 6374 6564  .counts directed
+00000360: 2065 6467 6573 2069 6e20 7468 6520 6c65   edges in the le
+00000370: 6172 6e65 6420 7374 7275 6374 7572 650a  arned structure.
+00000380: 0974 6861 7420 6172 6520 6f72 6965 6e74  .that are orient
+00000390: 6564 2069 6e63 6f72 7265 6374 6c79 2e20  ed incorrectly. 
+000003a0: 286c 6f77 6572 2069 7320 6265 7474 6572  (lower is better
+000003b0: 2920 5b31 5d0a 0a34 2e20 4861 6d6d 696e  ) [1]..4. Hammin
+000003c0: 6720 4469 7374 616e 6365 3a20 0a09 4465  g Distance: ..De
+000003d0: 7363 7269 6265 7320 7468 6520 6e75 6d62  scribes the numb
+000003e0: 6572 206f 6620 6368 616e 6765 7320 7468  er of changes th
+000003f0: 6174 2068 6176 6520 746f 2062 6520 6d61  at have to be ma
+00000400: 6465 0a09 746f 2061 206e 6574 776f 726b  de..to a network
+00000410: 2066 6f72 2069 7420 746f 2074 7572 6e20   for it to turn 
+00000420: 696e 746f 2074 6865 206f 6e65 2074 6861  into the one tha
+00000430: 7420 6974 2069 7320 6265 696e 6720 636f  t it is being co
+00000440: 6d70 6172 6564 2077 6974 682e 2049 7420  mpared with. It 
+00000450: 6973 2074 6865 0a09 7375 6d20 6f66 206d  is the..sum of m
+00000460: 6561 7375 7265 7320 312c 2032 2c20 616e  easures 1, 2, an
+00000470: 6420 332e 2056 6572 7369 6f6e 7320 6f66  d 3. Versions of
+00000480: 2074 6865 2048 616d 6d69 6e67 2064 6973   the Hamming dis
+00000490: 7461 6e63 6520 6d65 7472 6963 2068 6176  tance metric hav
+000004a0: 650a 0962 6565 6e20 7072 6f70 6f73 6564  e..been proposed
+000004b0: 2062 7920 4163 6964 2061 6e64 2064 6520   by Acid and de 
+000004c0: 4361 6d70 6f73 2028 3230 3033 292c 2054  Campos (2003), T
+000004d0: 7361 6d61 7264 696e 6f73 2065 7420 616c  samardinos et al
+000004e0: 2e20 2832 3030 3629 2c20 616e 640a 0950  . (2006), and..P
+000004f0: 6572 7269 6572 2065 7420 616c 2e20 2832  errier et al. (2
+00000500: 3030 3829 2e20 286c 6f77 6572 2069 7320  008). (lower is 
+00000510: 6265 7474 6572 2920 5b31 5d0a 0a0a 5265  better) [1]...Re
+00000520: 6665 7265 6e63 6573 0a2d 2d2d 2d2d 2d2d  ferences.-------
+00000530: 2d2d 2d0a 5b31 5d20 4d61 7274 696a 6e20  ---.[1] Martijn 
+00000540: 6465 204a 6f6e 6768 2061 6e64 204d 6172  de Jongh and Mar
+00000550: 656b 204a 2e20 4472 757a 647a 656c 0a09  ek J. Druzdzel..
+00000560: 2241 2043 6f6d 7061 7269 736f 6e20 6f66  "A Comparison of
+00000570: 2053 7472 7563 7475 7261 6c20 4469 7374   Structural Dist
+00000580: 616e 6365 204d 6561 7375 7265 730a 0966  ance Measures..f
+00000590: 6f72 2043 6175 7361 6c20 4261 7965 7369  or Causal Bayesi
+000005a0: 616e 204e 6574 776f 726b 204d 6f64 656c  an Network Model
+000005b0: 7322 0a0a 0a7a 2a4e 6963 686f 6c61 7320  s"...z*Nicholas 
+000005c0: 4375 6c6c 656e 203c 6e63 756c 6c65 6e2e  Cullen <ncullen.
+000005d0: 7468 4064 6172 746d 6f75 7468 2e65 6475  th@dartmouth.edu
+000005e0: 3ee9 0000 0000 4e63 0200 0000 0000 0000  >.....Nc........
+000005f0: 0000 0000 0500 0000 0600 0000 4300 0000  ............C...
+00000600: 7356 0000 0064 017d 027c 00a0 00a1 0044  sV...d.}.|.....D
+00000610: 005d 227d 037c 01a0 017c 03a1 0173 157c  .]"}.|...|...s.|
+00000620: 027c 00a0 027c 03a1 0137 007d 0271 067c  .|...|...7.}.q.|
+00000630: 00a0 037c 03a1 0144 005d 0d7d 047c 047c  ...|...D.].}.|.|
+00000640: 01a0 037c 03a1 0176 0172 277c 0264 0237  ...|...v.r'|.d.7
+00000650: 007d 0271 1a71 067c 0253 0029 037a 800a  .}.q.q.|.S.).z..
+00000660: 0943 6f75 6e74 7320 6564 6765 7320 7468  .Counts edges th
+00000670: 6174 2061 7265 2070 7265 7365 6e74 2069  at are present i
+00000680: 6e20 7468 6520 6f72 6967 696e 616c 2073  n the original s
+00000690: 7472 7563 7475 7265 2028 7829 2062 7574  tructure (x) but
+000006a0: 0a09 6172 6520 6d69 7373 696e 6720 696e  ..are missing in
+000006b0: 2074 6865 206c 6561 726e 6564 2073 7472   the learned str
+000006c0: 7563 7475 7265 2028 7929 2e20 286c 6f77  ucture (y). (low
+000006d0: 6572 2069 7320 6265 7474 6572 290a 0972  er is better)..r
+000006e0: 0100 0000 e901 0000 00a9 04da 056e 6f64  .............nod
+000006f0: 6573 da08 6861 735f 6e6f 6465 da06 6465  es..has_node..de
+00000700: 6772 6565 da08 6368 696c 6472 656e 2905  gree..children).
+00000710: da01 78da 0179 da07 6d69 7373 696e 67da  ..x..y..missing.
+00000720: 0272 76da 0563 6869 6c64 a900 720d 0000  .rv..child..r...
+00000730: 00fa 5243 3a5c 5573 6572 735c 526f 6d61  ..RC:\Users\Roma
+00000740: 6e5c 4465 736b 746f 705c 4769 7442 616d  n\Desktop\GitBam
+00000750: 745c 4241 4d54 5c62 616d 745c 6578 7465  t\BAMT\bamt\exte
+00000760: 726e 616c 5c70 7942 4e5c 7574 696c 735c  rnal\pyBN\utils\
+00000770: 7374 7275 6374 7572 655f 6469 7374 616e  structure_distan
+00000780: 6365 2e70 79da 0d6d 6973 7369 6e67 5f65  ce.py..missing_e
+00000790: 6467 6573 3400 0000 f314 0000 0004 050c  dges4...........
+000007a0: 010a 0110 010e 020e 0108 0102 8002 fe04  ................
+000007b0: 0372 0f00 0000 6302 0000 0000 0000 0000  .r....c.........
+000007c0: 0000 0005 0000 0006 0000 0043 0000 0073  ...........C...s
+000007d0: 5600 0000 6401 7d02 7c01 a000 a100 4400  V...d.}.|.....D.
+000007e0: 5d22 7d03 7c00 a001 7c03 a101 7315 7c02  ]"}.|...|...s.|.
+000007f0: 7c01 a002 7c03 a101 3700 7d02 7106 7c01  |...|...7.}.q.|.
+00000800: a003 7c03 a101 4400 5d0d 7d04 7c04 7c00  ..|...D.].}.|.|.
+00000810: a003 7c03 a101 7601 7227 7c02 6402 3700  ..|...v.r'|.d.7.
+00000820: 7d02 711a 7106 7c02 5300 2903 7a7a 0a09  }.q.q.|.S.).zz..
+00000830: 436f 756e 7473 2065 6467 6573 2074 6861  Counts edges tha
+00000840: 7420 6172 6520 666f 756e 6420 696e 2074  t are found in t
+00000850: 6865 206c 6561 726e 6564 2073 7472 7563  he learned struc
+00000860: 7475 7265 2062 7574 2061 7265 0a09 6e6f  ture but are..no
+00000870: 7420 7072 6573 656e 7420 696e 2074 6865  t present in the
+00000880: 206f 7269 6769 6e61 6c20 7374 7275 6374   original struct
+00000890: 7572 652e 2028 6c6f 7765 7220 6973 2062  ure. (lower is b
+000008a0: 6574 7465 7229 0a09 7201 0000 0072 0200  etter)..r....r..
+000008b0: 0000 7203 0000 0029 0572 0800 0000 7209  ..r....).r....r.
+000008c0: 0000 00da 0565 7874 7261 720b 0000 0072  .....extrar....r
+000008d0: 0c00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
+000008e0: 0000 00da 0b65 7874 7261 5f65 6467 6573  .....extra_edges
+000008f0: 4300 0000 7210 0000 0072 1200 0000 6302  C...r....r....c.
+00000900: 0000 0000 0000 0000 0000 0005 0000 0006  ................
+00000910: 0000 0043 0000 0073 4600 0000 6401 7d02  ...C...sF...d.}.
+00000920: 7c00 a000 a100 4400 5d1a 7d03 7c00 a001  |.....D.].}.|...
+00000930: 7c03 a101 7220 7c00 a002 7c03 a101 4400  |...r |...|...D.
+00000940: 5d0d 7d04 7c03 7c01 a003 7c03 a101 7600  ].}.|.|...|...v.
+00000950: 721f 7c02 6402 3700 7d02 7112 7106 7c02  r.|.d.7.}.q.q.|.
+00000960: 5300 2903 7a64 0a09 436f 756e 7473 2064  S.).zd..Counts d
+00000970: 6972 6563 7465 6420 6564 6765 7320 696e  irected edges in
+00000980: 2074 6865 206c 6561 726e 6564 2073 7472   the learned str
+00000990: 7563 7475 7265 0a09 7468 6174 2061 7265  ucture..that are
+000009a0: 206f 7269 656e 7465 6420 696e 636f 7272   oriented incorr
+000009b0: 6563 746c 792e 2028 6c6f 7765 7220 6973  ectly. (lower is
+000009c0: 2062 6574 7465 7229 0a09 7201 0000 0072   better)..r....r
+000009d0: 0200 0000 2904 7204 0000 0072 0500 0000  ....).r....r....
+000009e0: 7207 0000 00da 0770 6172 656e 7473 2905  r......parents).
+000009f0: 7208 0000 0072 0900 0000 5a13 696e 636f  r....r....Z.inco
+00000a00: 7272 6563 745f 6469 7265 6374 696f 6e72  rrect_directionr
+00000a10: 0b00 0000 720c 0000 0072 0d00 0000 720d  ....r....r....r.
+00000a20: 0000 0072 0e00 0000 da19 696e 636f 7272  ...r......incorr
+00000a30: 6563 745f 6469 7265 6374 696f 6e5f 6564  ect_direction_ed
+00000a40: 6765 7352 0000 0073 1000 0000 0405 0c01  gesR...s........
+00000a50: 0a01 0e01 0e01 0801 0480 0401 7214 0000  ............r...
+00000a60: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
+00000a70: 0000 0400 0000 4300 0000 731e 0000 0074  ......C...s....t
+00000a80: 007c 007c 0183 0274 017c 007c 0183 0217  .|.|...t.|.|....
+00000a90: 0074 027c 007c 0183 0217 0053 0029 014e  .t.|.|.....S.).N
+00000aa0: 2903 720f 0000 0072 1200 0000 7214 0000  ).r....r....r...
+00000ab0: 0029 0272 0800 0000 7209 0000 0072 0d00  .).r....r....r..
+00000ac0: 0000 720d 0000 0072 0e00 0000 da07 6861  ..r....r......ha
+00000ad0: 6d6d 696e 675f 0000 0073 0200 0000 1e01  mming_...s......
+00000ae0: 7215 0000 0029 08da 075f 5f64 6f63 5f5f  r....)...__doc__
+00000af0: da0a 5f5f 6175 7468 6f72 5f5f da05 6e75  ..__author__..nu
+00000b00: 6d70 79da 026e 7072 0f00 0000 7212 0000  mpy..npr....r...
+00000b10: 0072 1400 0000 7215 0000 0072 0d00 0000  .r....r....r....
+00000b20: 720d 0000 0072 0d00 0000 720e 0000 00da  r....r....r.....
+00000b30: 083c 6d6f 6475 6c65 3e01 0000 0073 0e00  .<module>....s..
+00000b40: 0000 0400 042f 0802 0802 080f 080f 0c0d  ...../..........
```

### Comparing `BAMT-1.1.33/bamt/log.py` & `BAMT-1.1.40/bamt/log.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.33/bamt/logging.conf` & `BAMT-1.1.40/bamt/logging.conf`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.33/bamt/mi_entropy_gauss.py` & `BAMT-1.1.40/bamt/mi_entropy_gauss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import os
 import sys
 import inspect
-# currentdir = os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
-# parentdir = os.path.dirname(currentdir)
-# sys.path.insert(0,parentdir)
 
 
 from copy import copy
 import math
 from typing import List
 import numpy as np
 import pandas as pd
```

### Comparing `BAMT-1.1.33/bamt/networks.py` & `BAMT-1.1.40/bamt/networks/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,47 +4,43 @@
 import matplotlib
 import matplotlib.pyplot as plt
 import pandas as pd
 import numpy as np
 import json
 import os
 
-# from sklearn import preprocessing as pp
 from tqdm import tqdm
 from concurrent.futures import ThreadPoolExecutor
 from pyvis.network import Network
 from pyitlib import discrete_random_variable as drv
-from typing import Dict, Tuple, List, Callable, Optional, Type, Union, Any, Sequence
 
 from bamt.builders import ParamDict
 from bamt.log import logger_network
 from bamt.config import config
-from bamt.utils.MathUtils import get_brave_matrix, get_proximity_matrix
-# from bamt import Builders, Nodes
+
+from bamt.nodes.base import BaseNode
 
 import bamt.builders as Builders
-import bamt.nodes as Nodes
 
-# from bamt.Preprocessors import Preprocessor
+from typing import Dict, Tuple, List, Callable, Optional, Type, Union, Any, Sequence
 
 STORAGE = config.get('NODES', 'models_storage',
                      fallback='models_storage is not defined')
 
 
 class BaseNetwork(object):
     """
     Base class for Bayesian Network
     """
 
     def __init__(self):
         """
-        Attributes:
-            nodes: a list of nodes instances
-            edges: a list of edges
-            distributions: dict
+        nodes: a list of nodes instances
+        edges: a list of edges
+        distributions: dict
         """
         self.type = 'Abstract'
         self._allowed_dtypes = ['Abstract']
         self.nodes = []
         self.edges = []
         self.weights = {}
         self.descriptor = {"types": {},
@@ -53,15 +49,15 @@
         self.has_logit = False
         self.use_mixture = False
 
     @property
     def nodes_names(self) -> List[str]:
         return [node.name for node in self.nodes]
 
-    def __getitem__(self, node_name: str) -> Type[Nodes.BaseNode]:
+    def __getitem__(self, node_name: str) -> Type[BaseNode]:
         if node_name in self.nodes_names:
             index = self.nodes_names.index(node_name)
             return self.nodes[index]
 
     def validate(self, descriptor: Dict[str, Dict[str, str]]) -> bool:
         types = descriptor['types']
         return True if all(
@@ -97,16 +93,16 @@
         # LEVEL 1
         worker_1 = Builders.VerticesDefiner(descriptor, regressor=None)
         self.nodes = worker_1.vertices
 
     def add_edges(self,
                   data: pd.DataFrame,
                   scoring_function: Union[Tuple[str,
-                                                Callable],
-                                          Tuple[str]],
+                  Callable],
+                  Tuple[str]],
                   progress_bar: bool = True,
                   classifier: Optional[object] = None,
                   regressor: Optional[object] = None,
                   params: Optional[ParamDict] = None,
                   optimizer: str = 'HC'):
         """
         Base function for Structure learning
@@ -126,17 +122,17 @@
             # init_edges validation
             if not self.has_logit and "init_edges" in params.keys():
                 type_map = np.array([
                     [self.descriptor["types"][node1], self.descriptor["types"][node2]] for node1, node2 in
                     params["init_edges"]]
                 )
                 failed = (
-                    (type_map[:, 0] == "cont") &
-                    ((type_map[:, 1] == "disc") |
-                     (type_map[:, 1] == "disc_num"))
+                        (type_map[:, 0] == "cont") &
+                        ((type_map[:, 1] == "disc") |
+                         (type_map[:, 1] == "disc_num"))
                 )
                 if sum(failed):
                     logger_network.warning(
                         f"Edges between continuous nodes and disc nodes are forbidden (has_logit = {self.has_logit}), "
                         f"they will be ignored. Indexes: {np.where(failed)[0]}")
                     params["init_edges"] = [params["init_edges"][i] for i in range(
                         len(params["init_edges"])) if i not in np.where(failed)[0]]
@@ -168,19 +164,19 @@
             self.edges = worker.skeleton['E']
 
     def calculate_weights(self, discretized_data: pd.DataFrame):
         """
         Provide calculation of link strength according mutual information between node and its parent(-s) values.
         """
         import bamt.utils.GraphUtils as gru
-        if not all([i in ['disc', 'disc_num']
-                   for i in gru.nodes_types(discretized_data).values()]):
+        data_descriptor = gru.nodes_types(discretized_data)
+        if not all([i in ['disc', 'disc_num'] for i in data_descriptor.values()]):
             logger_network.error(
                 f"calculate_weghts() method deals only with discrete data. Continuous data: " +
-                f"{[col for col, type in gru.nodes_types(discretized_data).items() if type not in ['disc', 'disc_num']]}")
+                f"{[col for col, type in data_descriptor.items() if type not in ['disc', 'disc_num']]}")
         if not self.edges:
             logger_network.error(
                 "Bayesian Network hasn't fitted yet. Please add edges with add_edges() method")
         if not self.nodes:
             logger_network.error(
                 "Bayesian Network hasn't fitted yet. Please add nodes with add_nodes() method")
         weights = dict()
@@ -188,65 +184,62 @@
         for node in self.nodes:
             parents = node.cont_parents + node.disc_parents
             if parents is None:
                 continue
             y = discretized_data[node.name].values
             if len(parents) == 1:
                 x = discretized_data[parents[0]].values
-                LS_true = drv.information_mutual(X=y, Y=x)
+                ls_true = drv.information_mutual(X=y, Y=x)
                 entropy = drv.entropy(X=y)
-                weight = LS_true / entropy
+                weight = ls_true / entropy
                 weights[(parents[0], node.name)] = weight
             else:
                 for parent_node in parents:
                     x = discretized_data[parent_node].values
                     other_parents = [
                         tmp for tmp in parents if tmp != parent_node]
                     z = list()
                     for other_parent in other_parents:
                         z.append(list(discretized_data[other_parent].values))
-                    LS_true = np.average(drv.information_mutual_conditional(
+                    ls_true = np.average(drv.information_mutual_conditional(
                         X=y, Y=x, Z=z, cartesian_product=True))
                     entropy = np.average(drv.entropy_conditional(
                         X=y, Y=z, cartesian_product=True)) + 1e-8
-                    weight = LS_true / entropy
+                    weight = ls_true / entropy
                     weights[(parent_node, node.name)] = weight
         self.weights = weights
 
     def set_nodes(self, nodes: List, info: Optional[Dict] = None):
         """
         additional function to set nodes manually. User should be aware that
         nodes must be a subclass of BaseNode.
-        :param nodes dict with name and node (if a lot of nodes should be added)
+        Params:
+            nodes: dict with name and node (if a lot of nodes should be added)
+            info: descriptor
         """
         if not info and not self.descriptor["types"]:
             logger_network.error(
                 "In case of manual setting nodes user should set map for them as well.")
             return
         self.nodes = []
         for node in nodes:
-            try:
-                assert issubclass(type(node), Nodes.BaseNode)
+            if issubclass(type(node), BaseNode):
                 self.nodes.append(node)
-                continue
-            except AssertionError:
+            else:
                 logger_network.error(
-                    f"{node} is not an instance of {Nodes.BaseNode}")
-                continue
-            except TypeError:
-                logger_network.error(f"TypeError : {node.__class__}")
-                continue
+                    f"{node} is not an instance of {BaseNode}")
+
         if info:
             self.descriptor = info
 
     def set_edges(self, edges: Optional[List[Sequence[str]]] = None):
         """
         additional function to set edges manually. User should be aware that
         nodes must be a subclass of BaseNode.
-        :param edges dict with name and node (if a lot of nodes should be added)
+        param: edges dict with name and node (if a lot of nodes should be added)
         """
 
         if not self.nodes:
             logger_network.error("Graph without nodes")
         self.edges = []
         for node1, node2 in edges:
             if isinstance(node1, str) and isinstance(node2, str):
@@ -273,31 +266,34 @@
                       nodes: Optional[List] = None,
                       edges: Optional[List[Sequence[str]]] = None,
                       overwrite: bool = True):
         """
         Function to set structure manually
         info: Descriptor
         nodes, edges:
-        overwrite: use 2 stage of defining or not
+        overwrite: use 2nd stage of defining or not
         """
         if nodes and (
-            info or (
+                info or (
                 self.descriptor["types"] and self.descriptor["signs"])):
             self.set_nodes(nodes=nodes, info=info)
         if edges:
             self.set_edges(edges=edges)
             if overwrite:
                 builder = Builders.VerticesDefiner(
                     descriptor=self.descriptor, regressor=None)  # init worker
                 builder.skeleton['V'] = builder.vertices  # 1 stage
                 builder.skeleton['E'] = self.edges
                 builder.get_family()
                 if self.edges:
                     builder.overwrite_vertex(
-                        has_logit=self.has_logit, use_mixture=self.use_mixture, classifier=None, regressor=None)
+                        has_logit=self.has_logit,
+                        use_mixture=self.use_mixture,
+                        classifier=None,
+                        regressor=None)
                     self.set_nodes(nodes=builder.skeleton['V'])
                 else:
                     logger_network.error("Empty set of edges")
 
     def _param_validation(self, params: Dict[str, Any]) -> bool:
         if all(self[i] for i in params.keys()):
             for name, info in params.items():
@@ -311,22 +307,19 @@
             logger_network.error(
                 "Param validation failed due to unknown nodes.")
             return False
 
     def set_parameters(self, parameters: Dict):
         if not self.nodes:
             logger_network.error("Failed on search of BN's nodes.")
-        # elif self._param_validation(parameters):
-        # pass
 
         self.distributions = parameters
 
         for node, data in self.distributions.items():
             if "hybcprob" in data.keys():
-                # first_item = next(iter(data["hybcprob"].values()))
                 if "mixture" in self[node].type.lower():
                     continue
                 else:
                     if "gaussian" in self[node].type.lower():
                         model_type = "regressor"
                     else:
                         model_type = "classifier"
@@ -411,25 +404,26 @@
             for node_data in input_dict['parameters'].values():
                 if 'hybcprob' not in node_data.keys():
                     continue
                 else:
                     # Since we don't have information about types of nodes, we
                     # should derive it from parameters.
                     if any(list(node_keys.keys()) == ["covars", "mean", "coef"]
-                            for node_keys in node_data['hybcprob'].values()):
+                           for node_keys in node_data['hybcprob'].values()):
                         raise CompatibilityError("use_mixture")
 
+        # check if edges before and after are the same.They can be different in the case when user sets forbidden edges.
         if not self.has_logit:
             if not all(
-                ob1 == [
-                    ob2[0],
-                    ob2[1]] for ob1,
-                ob2 in zip(
-                    input_dict['edges'],
-                    self.edges)):
+                    edges_before == [
+                        edges_after[0],
+                        edges_after[1]] for edges_before,
+                    edges_after in zip(
+                        input_dict['edges'],
+                        self.edges)):
                 raise CompatibilityError("has_logit")
 
         self.set_parameters(parameters=input_dict['parameters'])
         str_keys = list(input_dict['weights'].keys())
         tuple_keys = [eval(key) for key in str_keys]
         weights = {}
         for tuple_key in tuple_keys:
@@ -440,15 +434,14 @@
         """
         Base function for parameter learning
         """
         if dropna:
             data = data.dropna()
             data.reset_index(inplace=True, drop=True)
 
-
         if not os.path.isdir(STORAGE):
             os.makedirs(STORAGE)
 
         # init folder
         if not os.listdir(STORAGE):
             os.makedirs(os.path.join(STORAGE, "0"))
 
@@ -548,17 +541,17 @@
                         for obj, obj_data in node_data["hybcprob"].items():
                             if "serialization" in obj_data.keys():
                                 if "gaussian" in node.type.lower():
                                     model_type = "regressor"
                                 else:
                                     model_type = "classifier"
                                 if obj_data["serialization"] == 'joblib' and obj_data[
-                                        f"{model_type}_obj"]:
+                                    f"{model_type}_obj"]:
                                     new_path = models_dir + \
-                                        f"\\{node.name.replace(' ', '_')}\\{obj}.joblib.compressed"
+                                               f"\\{node.name.replace(' ', '_')}\\{obj}.joblib.compressed"
                                     node_data["hybcprob"][obj][f"{model_type}_obj"] = new_path
 
                     if predict:
                         output[node.name] = \
                             node.predict(node_data, pvals=pvals)
                     else:
                         output[node.name] = \
@@ -591,36 +584,37 @@
         else:
             return seq
 
     def predict(self,
                 test: pd.DataFrame,
                 parall_count: int = 1,
                 progress_bar: bool = True) -> Dict[str,
-                                                   Union[List[str],
-                                                         List[int],
-                                                         List[float]]]:
+    Union[List[str],
+    List[int],
+    List[float]]]:
         """
         Function to predict columns from given data.
         Note that train data and test data must have different columns.
         Both train and test datasets must be cleaned from NaNs.
 
         Args:
             test (pd.DataFrame): test dataset
             parall_count (int, optional):number of threads. Defaults to 1.
+            progress_bar: verbose mode.
 
         Returns:
             predicted data (dict): dict with column as key and predicted data as value
         """
         if test.isnull().any().any():
             logger_network.error("Test data contains NaN values.")
             return {}
 
         from joblib import Parallel, delayed
 
-        def wrapper(bn: HybridBN, test: pd.DataFrame, columns: List[str]):
+        def wrapper(bn, test: pd.DataFrame, columns: List[str]):
             preds = {column_name: list() for column_name in columns}
 
             if len(test) == 1:
                 for i in range(test.shape[0]):
                     test_row = dict(test.iloc[i, :])
                     for n, key in enumerate(columns):
                         try:
@@ -650,33 +644,26 @@
         columns = list(set(self.nodes_names) - set(test.columns.to_list()))
         if not columns:
             logger_network.error("Test data is the same as train.")
             return {}
 
         preds = {column_name: list() for column_name in columns}
 
-        # processed_list = Parallel(n_jobs=parall_count)(
-        # delayed(wrapper)(self, test.loc[[i]], columns) for i in
-        # tqdm(test.index, position=0, leave=True))
-
         if progress_bar:
             processed_list = Parallel(n_jobs=parall_count)(delayed(wrapper)(
                 self, test.loc[[i]], columns) for i in tqdm(test.index, position=0, leave=True))
         else:
             processed_list = Parallel(n_jobs=parall_count)(
                 delayed(wrapper)(self, test.loc[[i]], columns) for i in test.index)
 
         for i in range(test.shape[0]):
             curr_pred = processed_list[i]
             for n, key in enumerate(columns):
                 preds[key].append(curr_pred[key][0])
 
-        # for column in columns:
-        #     preds[column] = [k for k in preds[column] if not pd.isna(k)]
-
         return preds
 
     def set_classifiers(self, classifiers: Dict[str, object]):
         """
         Set classifiers for logit nodes.
         classifiers: dict with node_name and Classifier
         """
@@ -774,104 +761,18 @@
 
         for level in range(len(nodes_sorted)):
             for node_i in range(len(nodes_sorted[level])):
                 name = nodes_sorted[level][node_i]
                 cls = name2class[name]
                 color = class2color[cls]
                 network.add_node(name, label=name, color=color, size=45, level=level, font={
-                                 'size': 36}, title=f'Узел байесовской сети {name} ({cls})')
+                    'size': 36}, title=f'Узел байесовской сети {name} ({cls})')
 
         for edge in G.edges:
             network.add_edge(edge[0], edge[1])
 
         network.hrepulsion(node_distance=300, central_gravity=0.5)
 
         if not (os.path.exists('visualization_result')):
             os.mkdir("visualization_result")
 
         return network.show(f'visualization_result/' + output)
-
-
-class DiscreteBN(BaseNetwork):
-    """
-    Bayesian Network with Discrete Types of Nodes
-    """
-
-    def __init__(self):
-        super(DiscreteBN, self).__init__()
-        self.type = 'Discrete'
-        self.scoring_function = ""
-        self._allowed_dtypes = ['disc', 'disc_num']
-        self.has_logit = None
-        self.use_mixture = None
-
-
-class ContinuousBN(BaseNetwork):
-    """
-    Bayesian Network with Continuous Types of Nodes
-    """
-
-    def __init__(self, use_mixture: bool = False):
-        super(ContinuousBN, self).__init__()
-        self.type = 'Continuous'
-        self._allowed_dtypes = ['cont']
-        self.has_logit = None
-        self.use_mixture = use_mixture
-        self.scoring_function = ""
-
-
-class HybridBN(BaseNetwork):
-    """
-    Bayesian Network with Mixed Types of Nodes
-    """
-
-    def __init__(self, has_logit: bool = False, use_mixture: bool = False):
-        super(HybridBN, self).__init__()
-        self._allowed_dtypes = ['cont', 'disc', 'disc_num']
-        self.type = 'Hybrid'
-        self.has_logit = has_logit
-        self.use_mixture = use_mixture
-
-    def validate(self, descriptor: Dict[str, Dict[str, str]]) -> bool:
-        types = descriptor['types']
-        s = set(types.values())
-        return True if ({'cont', 'disc', 'disc_num'} == s) or (
-            {'cont', 'disc'} == s) or ({'cont', 'disc_num'} == s) else False
-
-
-class BigBraveBN:
-
-    def __init__(self, n_nearest=5, threshold=.3, proximity_metric='MI'):
-        self.n_nearest = n_nearest
-        self.threshold = threshold
-        self.proximity_metric = proximity_metric
-        self.possible_edges = []
-
-    def set_possible_edges_by_brave(self, df):
-        """Returns list of possible edges for structure learning
-
-        Args:
-            df (DataFrame): data
-            proximity_matrix (DataFrame): might be generated by get_mutual_info_score_matrix() function,
-                                                                                                        correlation etc.
-            n_nearest (int, optional): Number of Nearest neighbors, hyperparameter. Defaults to 5.
-            threshold (float, optional): Threshold for edge candidates to be passed to possible edges, threshold.
-                                                                                                Defaults to 0.3 [0;1].
-
-        Returns:
-            Possible edges: list of possible edges
-        """
-
-        proximity_matrix = get_proximity_matrix(
-            df, proximity_metric=self.proximity_metric)
-        brave_matrix = get_brave_matrix(
-            df.columns, proximity_matrix, self.n_nearest)
-
-        possible_edges_list = []
-
-        for c1 in df.columns:
-            for c2 in df.columns:
-                if brave_matrix.loc[c1, c2] > brave_matrix.max(
-                        numeric_only='true').max() * self.threshold:
-                    possible_edges_list.append((c1, c2))
-
-        self.possible_edges = possible_edges_list
```

### Comparing `BAMT-1.1.33/bamt/preprocess/discretization.py` & `BAMT-1.1.40/bamt/preprocess/discretization.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.33/bamt/preprocess/graph.py` & `BAMT-1.1.40/bamt/preprocess/graph.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.33/bamt/preprocess/numpy_pandas.py` & `BAMT-1.1.40/bamt/preprocess/numpy_pandas.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.33/bamt/preprocessors.py` & `BAMT-1.1.40/bamt/preprocessors.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.33/bamt/redef_info_scores.py` & `BAMT-1.1.40/bamt/redef_info_scores.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-# from bayesian.redef_info_scores import BIC_local
-# import os,sys,inspect
-# currentdir = os.path.dirname(os.path.abspath(inspect.getfile(inspect.currentframe())))
-# parentdir = os.path.dirname(currentdir)
-# sys.path.insert(0,parentdir)
 import sys
 import numpy as np
 import pandas as pd
 from copy import copy
 import warnings
 from bamt.mi_entropy_gauss import mi_gauss as mutual_information, entropy_all as entropy
 from bamt.preprocess.numpy_pandas import get_type_numpy
@@ -97,15 +92,14 @@
     mi_scores = [mutual_information(data[:,
                                          (bn.V.index(rv),
                                           ) + tuple([bn.V.index(p) for p in bn.parents(rv)])],
                                     method=method) for rv in bn.nodes()]
     ent_scores = [entropy(data[:, bn.V.index(rv)], method=method)
                   for rv in bn.nodes()]
     return NROW * (sum(mi_scores) - sum(ent_scores))
-    # return ((1/nrow)*(np.sum(np.log((1e+7+bn.flat_cpt())))))
 
 
 def log_lik_local(data, method='LL'):
     NROW = data.shape[0]
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         if isinstance(data, pd.DataFrame):
@@ -113,24 +107,21 @@
                     entropy(data.iloc[:, 0], method=method)))
         elif isinstance(data, pd.Series):
             return 0.0
         elif isinstance(data, np.ndarray):
             return (NROW * (mutual_information(data, method=method) -
                     entropy(data[:, 0], method=method)))
 
-    # return ((1/nrow)*(np.sum(np.log((1e+7+bn.flat_cpt())))))
-
 
 def BIC_local(data, method='BIC'):
     NROW = data.shape[0]
     log_score = log_lik_local(data, method=method)
     try:
         penalty = 0.5 * num_params(data) * np.log(NROW)
     except OverflowError as err:
-        # print(data)
         penalty = sys.float_info.max
     return log_score - penalty
 
 
 def num_params(data):
     # Convert pandas DataFrame to numpy array
     if isinstance(data, pd.DataFrame):
```

### Comparing `BAMT-1.1.33/bamt/utils/GraphUtils.py` & `BAMT-1.1.40/bamt/utils/GraphUtils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import networkx as nx
 from bamt.log import logger_preprocessor
 from pandas import DataFrame
-from bamt.nodes import BaseNode
+from bamt.nodes.base import BaseNode
 
 from typing import Dict, List, Tuple, Type
 
 
 def nodes_types(data: DataFrame) -> Dict[str, str]:
     """
     Function to define the type of the node
```

### Comparing `BAMT-1.1.33/bamt/utils/MathUtils.py` & `BAMT-1.1.40/bamt/utils/MathUtils.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.33/pyproject.toml` & `BAMT-1.1.40/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "BAMT"
-version = "1.1.33"
+version = "1.1.40"
 description = "data modeling and analysis tool based on Bayesian networks"
 authors = ["Roman Netrogolov <romius2001@gmail.com>",
 	   "Irina Deeva <iriny.deeva@gmail.com>",
 	   "Karine Shakhkyan <kshahkyan@yandex.ru>",
 	   "Nikita Kovalev Yasen <Nikitoskova123@gmail.com>",
 	   "Anna Bubnova <banuba313@gmail.com>",
 	   "Yury Kaminsky <jkaminski@niuitmo.ru>"]
@@ -33,11 +33,12 @@
 pyvis = ">=0.2.1"
 missingno = "^0.5.1"
 pgmpy = "0.1.20"
 pyitlib = "0.2.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "7.1.3"
+catboost = "1.1.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `BAMT-1.1.33/README.rst` & `BAMT-1.1.40/README.rst`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.33/setup.py` & `BAMT-1.1.40/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,20 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['bamt',
  'bamt.external',
- 'bamt.external.libpgm',
  'bamt.external.pyBN',
  'bamt.external.pyBN.classes',
  'bamt.external.pyBN.classes._tests',
- 'bamt.external.pyBN.classification',
- 'bamt.external.pyBN.inference',
- 'bamt.external.pyBN.inference._tests',
- 'bamt.external.pyBN.inference.map_exact',
- 'bamt.external.pyBN.inference.marginal_approx',
- 'bamt.external.pyBN.inference.marginal_exact',
- 'bamt.external.pyBN.io',
- 'bamt.external.pyBN.io._tests',
- 'bamt.external.pyBN.learning',
- 'bamt.external.pyBN.learning.parameter',
- 'bamt.external.pyBN.learning.parameter._tests',
- 'bamt.external.pyBN.learning.structure',
- 'bamt.external.pyBN.learning.structure._tests',
- 'bamt.external.pyBN.learning.structure.constraint',
- 'bamt.external.pyBN.learning.structure.exact',
- 'bamt.external.pyBN.learning.structure.hybrid',
- 'bamt.external.pyBN.learning.structure.naive',
- 'bamt.external.pyBN.learning.structure.score',
- 'bamt.external.pyBN.learning.structure.tree',
- 'bamt.external.pyBN.plotting',
  'bamt.external.pyBN.utils',
  'bamt.external.pyBN.utils._tests',
+ 'bamt.networks',
+ 'bamt.nodes',
  'bamt.preprocess',
  'bamt.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
@@ -48,15 +29,15 @@
  'pyvis>=0.2.1',
  'scikit-learn==1.2.0',
  'scipy>=1.8.0,<2.0.0',
  'setuptools==65.6.3']
 
 setup_kwargs = {
     'name': 'bamt',
-    'version': '1.1.33',
+    'version': '1.1.40',
     'description': 'data modeling and analysis tool based on Bayesian networks',
     'long_description': ".. image:: /docs/images/BAMT_white_bg.png\n   :align: center\n   :alt: BAMT framework logo\n\n.. start-badges\n.. list-table::\n   :stub-columns: 1\n\n   * - package\n     - | |pypi| |py_8| |py_9| |py_10|\n   * - tests\n     - | |Build| |coverage|\n   * - docs\n     - |docs|\n   * - license\n     - | |license|\n   * - stats\n     - | |downloads_stats| |downloads_monthly| |downloads_weekly|\n\nRepository of a data modeling and analysis tool based on Bayesian networks\n\nBAMT - Bayesian Analytical and Modelling Toolkit. This repository contains a data modeling and analysis tool based on Bayesian networks. It can be divided into two main parts - algorithms for constructing and training Bayesian networks on data and algorithms for applying Bayesian networks for filling gaps, generating synthetic data, assessing edges strength e.t.c.\n\n.. image:: docs/images/bamt_readme_scheme.png\n     :target: docs/images/bamt_readme_scheme.png\n     :align: center\n     :alt: bamt readme scheme\n\nInstallation\n^^^^^^^^^^^^\n\nBAMT package is available via PyPi:\n\n.. code-block:: bash\n\n   pip install bamt\n\nBAMT Features\n^^^^^^^^^^^^^\n\nThe following algorithms for Bayesian Networks learning are implemented:\n\n\n* Building the structure of a Bayesian network based on expert knowledge by directly specifying the structure of the network;\n* Building the structure of a Bayesian network on data using three algorithms - Hill Climbing, evolutionary and PC (evolutionary and PC are currently under development). For Hill Climbing, the following score functions are implemented - MI, K2, BIC, AIC. The algorithms work on both discrete and mixed data.\n* Learning the parameters of distributions in the nodes of the network based on Gaussian distribution and Mixture Gaussian distribution with automatic selection of the number of components.\n* Non-parametric learning of distributions at nodes using classification and regression models.\n* BigBraveBN - algorithm for structural learning of Bayesian networks with a large number of nodes. Tested on networks with up to 500 nodes.\n\nDifference from existing implementations:\n\n\n* Algorithms work on mixed data;\n* Structural learning implements score-functions for mixed data;\n* Parametric learning implements the use of a mixture of Gaussian distributions to approximate continuous distributions;\n* Non-parametric learning of distributions with various user-specified regression and classification models;\n* The algorithm for structural training of large Bayesian networks (> 10 nodes) is based on local training of small networks with their subsequent algorithmic connection.\n\n.. image:: img/BN_gif.gif\n     :target: img/BN_gif.gif\n     :align: center\n     :alt: bn example gif\n\nFor example, in terms of data analysis and modeling using Bayesian networks, a pipeline has been implemented to generate synthetic data by sampling from Bayesian networks.\n\n\n\n.. image:: img/synth_gen.png\n   :target: img/synth_gen.png\n   :align: center\n   :height: 300px\n   :width: 600px\n   :alt: synthetics generation\n\n\nHow to use\n^^^^^^^^^^\n\nThen the necessary classes are imported from the library:\n\n.. code-block:: python\n\n   import bamt.networks as Nets\n\nNext, a network instance is created and training (structure and parameters) is performed:\n\n.. code-block:: python\n\n   bn = Nets.HybridBN(has_logit=False, use_mixture=True)\n   bn.add_edges(discretized_data, scoring_function=('K2',K2Score))\n   bn.fit_parameters(data)\n\n\n\nExamples & Tutorials\n^^^^^^^^^^^^^^^^^^^^^^\n\nMore examples can be found in `tutorials <https://github.com/ITMO-NSS-team/BAMT/tree/master/tutorials>`__  and `Documentation <https://bamt.readthedocs.io/en/latest/examples/learn_save.html>`__.\n\nPublications about BAMT\n^^^^^^^^^^^^^^^^^^^^^^^\n\nWe have published several articles about BAMT:\n\n* `Advanced Approach for Distributions Parameters Learning in Bayesian Networks with Gaussian Mixture Models and Discriminative Models <https://www.mdpi.com/2227-7390/11/2/343>`__ (2023)\n* `BigBraveBN: algorithm of structural learning for bayesian networks with a large number of nodes <https://www.sciencedirect.com/science/article/pii/S1877050922016945>`__ (2022)\n* `MIxBN: Library for learning Bayesian networks from mixed data <https://www.sciencedirect.com/science/article/pii/S1877050921020925>`__ (2021)\n* `Oil and Gas Reservoirs Parameters Analysis Using Mixed Learning of Bayesian Networks <https://link.springer.com/chapter/10.1007/978-3-030-77961-0_33>`__ (2021)\n* `Bayesian Networks-based personal data synthesis <https://dl.acm.org/doi/abs/10.1145/3411170.3411243>`__ (2020)\n\n\nProject structure\n^^^^^^^^^^^^^^^^^\n\nThe latest stable version of the library is available in the master branch.\n\nIt includes the following modules and direcotries:\n\n* `bamt <https://github.com/ITMO-NSS-team/BAMT/tree/master/bamt>`__ - directory with the framework code:\n    * Preprocessing - module for data preprocessing\n    * Networks - module for building and training Bayesian networks\n    * Nodes - module for nodes support of Bayesian networks\n    * Utilities - module for mathematical and graph utilities\n* `data <https://github.com/ITMO-NSS-team/BAMT/tree/master/data>`__  - directory with data for experiments and tests\n* `tests <https://github.com/ITMO-NSS-team/BAMT/tree/master/tests>`__  - directory with unit and integration tests\n* `tutorials <https://github.com/ITMO-NSS-team/BAMT/tree/master/tutorials>`__  - directory with tutorials\n* `docs <https://github.com/ITMO-NSS-team/BAMT/tree/master/docs>`__ - directory with RTD documentation\n\nPreprocessing\n=============\n\nPreprocessor module allows user to transform data according pipeline (similar to pipeline in scikit-learn).\n\nNetworks\n========\n\nThree types of networks are implemented:\n\n* HybridBN - Bayesian network with mixed data\n* DiscreteBN - Bayesian network with discrete data\n* ContinuousBN - Bayesian network with continuous data\n\nThey are inherited from the abstract class BaseNetwork.\n\nNodes\n=====\n\nContains classes for nodes of Bayesian networks.\n\nUtilities\n=========\n\nUtilities module contains mathematical and graph utilities to support the main functionality of the library.\n\n\nWeb-BAMT\n^^^^^^^^\n\nA web interface for BAMT is currently under development.\nThe repository is available at `web-BAMT <https://github.com/aimclub/Web-BAMT>`__\n\nContacts\n^^^^^^^^\n\nIf you have questions or suggestions, you can contact us at the following address: ideeva@itmo.ru (Irina Deeva)\n\nOur resources:\n\n* `Natural Systems Simulation Team <https://itmo-nss-team.github.io/>`__\n* `NSS team Telegram channel <https://t.me/NSS_group>`__\n* `NSS lab YouTube channel <https://www.youtube.com/@nsslab/videos>`__\n\n.. |docs| image:: https://readthedocs.org/projects/bamt/badge/?version=latest\n    :target: https://bamt.readthedocs.io/en/latest/?badge=latest\n    :alt: Documentation Status\n\n.. |pypi| image:: https://badge.fury.io/py/bamt.svg\n    :target: https://badge.fury.io/py/bamt\n\n.. |py_10| image:: https://img.shields.io/badge/python_3.10-passing-success\n   :alt: Supported Python Versions\n   :target: https://img.shields.io/badge/python_3.10-passing-success\n\n.. |py_8| image:: https://img.shields.io/badge/python_3.8-passing-success\n   :alt: Supported Python Versions\n   :target: https://img.shields.io/badge/python_3.8-passing-success\n\n.. |py_9| image:: https://img.shields.io/badge/python_3.9-passing-success\n   :alt: Supported Python Versions\n   :target: https://img.shields.io/badge/python_3.9-passing-success\n\n.. |license| image:: https://img.shields.io/github/license/ITMO-NSS-team/BAMT\n   :alt: Supported Python Versions\n   :target: https://github.com/ITMO-NSS-team/BAMT/blob/master/LICENCE\n\n.. |downloads_stats| image:: https://static.pepy.tech/personalized-badge/bamt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads\n :target: https://pepy.tech/project/bamt\n\n.. |downloads_monthly| image:: https://static.pepy.tech/personalized-badge/bamt?period=month&units=international_system&left_color=grey&right_color=blue&left_text=downloads/month\n :target: https://pepy.tech/project/bamt\n\n.. |downloads_weekly| image:: https://static.pepy.tech/personalized-badge/bamt?period=week&units=international_system&left_color=grey&right_color=blue&left_text=downloads/week\n :target: https://pepy.tech/project/bamt\n\n.. |Build| image:: https://github.com/ITMO-NSS-team/BAMT/actions/workflows/bamtcodecov.yml/badge.svg\n   :target: https://github.com/ITMO-NSS-team/BAMT/actions/workflows/bamtcodecov.yml\n\n.. |coverage| image:: https://codecov.io/github/ITMO-NSS-team/BAMT/branch/master/graph/badge.svg?token=9ZX37JNIYZ\n   :target: https://codecov.io/github/ITMO-NSS-team/BAMT\n",
     'author': 'Roman Netrogolov',
     'author_email': 'romius2001@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/ITMO-NSS-team/BAMT',
```

### Comparing `BAMT-1.1.33/PKG-INFO` & `BAMT-1.1.40/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bamt
-Version: 1.1.33
+Version: 1.1.40
 Summary: data modeling and analysis tool based on Bayesian networks
 Home-page: https://github.com/ITMO-NSS-team/BAMT
 License: BSD-3-Clause
 Author: Roman Netrogolov
 Author-email: romius2001@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: Development Status :: 3 - Alpha
```

