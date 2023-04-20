# Comparing `tmp/apimoex-1.2.0.tar.gz` & `tmp/apimoex-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apimoex-1.2.0.tar", last modified: Mon Feb  3 12:34:31 2020, max compression
+gzip compressed data, was "apimoex-1.3.0.tar", last modified: Thu Apr 20 17:12:22 2023, max compression
```

## Comparing `apimoex-1.2.0.tar` & `apimoex-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 WLMike     (501) staff       (20)        0 2020-02-03 12:34:31.000000 apimoex-1.2.0/
--rw-r--r--   0 WLMike     (501) staff       (20)     7364 2020-02-03 12:34:31.000000 apimoex-1.2.0/PKG-INFO
--rwxr-xr-x   0 WLMike     (501) staff       (20)     5352 2020-02-03 10:38:39.000000 apimoex-1.2.0/README.rst
-drwxr-xr-x   0 WLMike     (501) staff       (20)        0 2020-02-03 12:34:31.000000 apimoex-1.2.0/apimoex/
--rwxr-xr-x   0 WLMike     (501) staff       (20)      704 2020-02-03 12:32:32.000000 apimoex-1.2.0/apimoex/__init__.py
--rwxr-xr-x   0 WLMike     (501) staff       (20)     7207 2020-02-03 10:38:39.000000 apimoex-1.2.0/apimoex/client.py
--rwxr-xr-x   0 WLMike     (501) staff       (20)    23582 2020-02-03 12:26:26.000000 apimoex-1.2.0/apimoex/requests.py
-drwxr-xr-x   0 WLMike     (501) staff       (20)        0 2020-02-03 12:34:31.000000 apimoex-1.2.0/apimoex.egg-info/
--rw-r--r--   0 WLMike     (501) staff       (20)     7364 2020-02-03 12:34:31.000000 apimoex-1.2.0/apimoex.egg-info/PKG-INFO
--rw-r--r--   0 WLMike     (501) staff       (20)      231 2020-02-03 12:34:31.000000 apimoex-1.2.0/apimoex.egg-info/SOURCES.txt
--rw-r--r--   0 WLMike     (501) staff       (20)        1 2020-02-03 12:34:31.000000 apimoex-1.2.0/apimoex.egg-info/dependency_links.txt
--rw-r--r--   0 WLMike     (501) staff       (20)        9 2020-02-03 12:34:31.000000 apimoex-1.2.0/apimoex.egg-info/requires.txt
--rw-r--r--   0 WLMike     (501) staff       (20)        8 2020-02-03 12:34:31.000000 apimoex-1.2.0/apimoex.egg-info/top_level.txt
--rw-r--r--   0 WLMike     (501) staff       (20)       38 2020-02-03 12:34:31.000000 apimoex-1.2.0/setup.cfg
--rwxr-xr-x   0 WLMike     (501) staff       (20)     1698 2020-02-03 10:38:39.000000 apimoex-1.2.0/setup.py
+drwxr-xr-x   0 WLMike     (501) staff       (20)        0 2023-04-20 17:12:22.385852 apimoex-1.3.0/
+-rwxr-xr-x   0 WLMike     (501) staff       (20)     1210 2023-04-20 16:20:52.000000 apimoex-1.3.0/LICENSE
+-rw-r--r--   0 WLMike     (501) staff       (20)     6415 2023-04-20 17:12:22.385480 apimoex-1.3.0/PKG-INFO
+-rwxr-xr-x   0 WLMike     (501) staff       (20)     5456 2023-04-20 16:20:52.000000 apimoex-1.3.0/README.rst
+drwxr-xr-x   0 WLMike     (501) staff       (20)        0 2023-04-20 17:12:22.380989 apimoex-1.3.0/apimoex/
+-rwxr-xr-x   0 WLMike     (501) staff       (20)      704 2023-04-20 16:58:58.000000 apimoex-1.3.0/apimoex/__init__.py
+-rwxr-xr-x   0 WLMike     (501) staff       (20)     7207 2023-04-20 16:20:52.000000 apimoex-1.3.0/apimoex/client.py
+-rwxr-xr-x   0 WLMike     (501) staff       (20)    26012 2023-04-20 16:38:22.000000 apimoex-1.3.0/apimoex/requests.py
+drwxr-xr-x   0 WLMike     (501) staff       (20)        0 2023-04-20 17:12:22.384997 apimoex-1.3.0/apimoex.egg-info/
+-rw-r--r--   0 WLMike     (501) staff       (20)     6415 2023-04-20 17:12:22.000000 apimoex-1.3.0/apimoex.egg-info/PKG-INFO
+-rw-r--r--   0 WLMike     (501) staff       (20)      239 2023-04-20 17:12:22.000000 apimoex-1.3.0/apimoex.egg-info/SOURCES.txt
+-rw-r--r--   0 WLMike     (501) staff       (20)        1 2023-04-20 17:12:22.000000 apimoex-1.3.0/apimoex.egg-info/dependency_links.txt
+-rw-r--r--   0 WLMike     (501) staff       (20)        9 2023-04-20 17:12:22.000000 apimoex-1.3.0/apimoex.egg-info/requires.txt
+-rw-r--r--   0 WLMike     (501) staff       (20)        8 2023-04-20 17:12:22.000000 apimoex-1.3.0/apimoex.egg-info/top_level.txt
+-rw-r--r--   0 WLMike     (501) staff       (20)       38 2023-04-20 17:12:22.385948 apimoex-1.3.0/setup.cfg
+-rwxr-xr-x   0 WLMike     (501) staff       (20)     1698 2023-04-20 16:20:53.000000 apimoex-1.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `apimoex-1.2.0/PKG-INFO` & `apimoex-1.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,150 +1,16 @@
 Metadata-Version: 2.1
 Name: apimoex
-Version: 1.2.0
+Version: 1.3.0
 Summary: MOEX ISS API
 Home-page: https://wlm1ke.github.io/apimoex/
 Author: Mikhail Korotkov aka WLMike
 Author-email: wlmike@gmail.com
 License: http://unlicense.org
 Project-URL: Source, https://github.com/WLM1ke/apimoex
-Description: MOEX ISS API
-        ====================
-        .. image:: https://github.com/WLM1ke/apimoex/workflows/tests/badge.svg
-            :target: https://github.com/WLM1ke/apimoex/actions
-        .. image:: https://codecov.io/gh/WLM1ke/apimoex/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/WLM1ke/apimoex
-        .. image:: https://badge.fury.io/py/apimoex.svg
-            :target: https://badge.fury.io/py/apimoex
-        
-        Реализация части  запросов к `MOEX Informational & Statistical Server <https://www.moex.com/a2193>`_.
-        
-        Документация
-        ------------
-        https://wlm1ke.github.io/apimoex/
-        
-        Основные возможности
-        --------------------
-        Реализовано несколько функций-запросов информации о торгуемых акциях и их исторических котировках, результаты которых
-        напрямую конвертируются в pandas.DataFrame.
-        
-        Работа функций базируется на универсальном клиенте, позволяющем осуществлять произвольные запросы к MOEX ISS, поэтому
-        перечень доступных функций-запросов может быть легко расширен. При необходимости добавления функций воспользуйтесь
-        `Issues <https://github.com/WLM1ke/apimoex/issues>`_ на GitHub с указанием ссылки на описание запроса:
-        
-        * Полный перечень возможных `запросов <https://iss.moex.com/iss/reference/>`_ к MOEX ISS
-        * Официальное `Руководство разработчика <https://fs.moex.com/files/6523>`_ с дополнительной информацией
-        
-        Начало работы
-        =============
-        Установка
-        ---------
-        
-        .. code-block:: Bash
-        
-           $ pip install apimoex
-        
-        Пример использования реализованных запросов
-        -------------------------------------------
-        История котировок SNGSP в режиме TQBR::
-        
-           import requests
-        
-           import apimoex
-           import pandas as pd
-        
-        
-           with requests.Session() as session:
-               data = apimoex.get_board_history(session, 'SNGSP')
-               df = pd.DataFrame(data)
-               df.set_index('TRADEDATE', inplace=True)
-               print(df.head(), '\n')
-               print(df.tail(), '\n')
-               df.info()
-        
-        .. code-block::
-        
-                       BOARDID  CLOSE    VOLUME         VALUE
-            TRADEDATE
-            2014-06-09    TQBR  27.48  12674200  3.484352e+08
-            2014-06-10    TQBR  27.55  14035900  3.856417e+08
-            2014-06-11    TQBR  28.15  27208800  7.602146e+08
-            2014-06-16    TQBR  28.27  68059900  1.913160e+09
-            2014-06-17    TQBR  28.20  22101600  6.292844e+08
-        
-                       BOARDID   CLOSE     VOLUME         VALUE
-            TRADEDATE
-            2019-09-04    TQBR  38.060  243010500  9.348435e+09
-            2019-09-05    TQBR  36.140  129366600  4.704949e+09
-            2019-09-06    TQBR  35.475   62389000  2.201887e+09
-            2019-09-09    TQBR  34.570   54331300  1.905837e+09
-            2019-09-10    TQBR  35.250   45966000  1.605849e+09
-        
-            <class 'pandas.core.frame.DataFrame'>
-            Index: 1326 entries, 2014-06-09 to 2019-09-10
-            Data columns (total 4 columns):
-            BOARDID    1326 non-null object
-            CLOSE      1326 non-null float64
-            VOLUME     1326 non-null int64
-            VALUE      1326 non-null float64
-            dtypes: float64(2), int64(1), object(1)
-            memory usage: 51.8+ KB
-        
-        Пример реализации запроса с помощью клиента
-        -------------------------------------------
-        Перечень акций, торгующихся в режиме TQBR (`описание запроса <https://iss.moex.com/iss/reference/32>`_)::
-        
-           import requests
-        
-           import apimoex
-           import pandas as pd
-        
-        
-           request_url = ('https://iss.moex.com/iss/engines/stock/'
-                          'markets/shares/boards/TQBR/securities.json')
-           arguments = {'securities.columns': ('SECID,'
-                                               'REGNUMBER,'
-                                               'LOTSIZE,'
-                                               'SHORTNAME')}
-           with requests.Session() as session:
-               iss = apimoex.ISSClient(session, request_url, arguments)
-               data = iss.get()
-               df = pd.DataFrame(data['securities'])
-               df.set_index('SECID', inplace=True)
-               print(df.head(), '\n')
-               print(df.tail(), '\n')
-               df.info()
-        
-        .. code-block::
-        
-                      REGNUMBER  LOTSIZE   SHORTNAME
-            SECID
-            ABRD   1-02-12500-A       10  АбрауДюрсо
-            AFKS   1-05-01669-A      100  Система ао
-            AFLT   1-01-00010-A       10    Аэрофлот
-            AGRO           None        1    AGRO-гдр
-            AKRN   1-03-00207-A        1       Акрон
-        
-                      REGNUMBER  LOTSIZE   SHORTNAME
-            SECID
-            YNDX           None        1  Yandex clA
-            YRSB   1-01-50099-A       10     ТНСэнЯр
-            YRSBP  2-01-50099-A       10   ТНСэнЯр-п
-            ZILL   1-02-00036-A        1      ЗИЛ ао
-            ZVEZ   1-01-00169-D     1000   ЗВЕЗДА ао
-        
-            <class 'pandas.core.frame.DataFrame'>
-            Index: 264 entries, ABRD to ZVEZ
-            Data columns (total 3 columns):
-            REGNUMBER    255 non-null object
-            LOTSIZE      264 non-null int64
-            SHORTNAME    264 non-null object
-            dtypes: int64(1), object(2)
-            memory usage: 8.2+ KB
-        
 Keywords: moex iss api
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: Public Domain
 Classifier: Natural Language :: Russian
@@ -153,7 +19,153 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+MOEX ISS API
+============
+
+.. image:: https://github.com/WLM1ke/apimoex/workflows/tests/badge.svg
+    :target: https://github.com/WLM1ke/apimoex/actions
+.. image:: https://codecov.io/gh/WLM1ke/apimoex/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/WLM1ke/apimoex
+.. image:: https://badge.fury.io/py/apimoex.svg
+    :target: https://badge.fury.io/py/apimoex
+
+Реализация части запросов к `MOEX Informational & Statistical Server <https://www.moex.com/a2193>`_.
+
+Документация
+------------
+
+https://wlm1ke.github.io/apimoex/
+
+Основные возможности
+--------------------
+
+Реализовано несколько функций-запросов информации о торгуемых акциях и их исторических котировках, результаты которых
+напрямую конвертируются в pandas.DataFrame.
+
+Работа функций базируется на универсальном клиенте, позволяющем осуществлять произвольные запросы к MOEX ISS, поэтому
+перечень доступных функций-запросов может быть легко расширен. При необходимости добавления функций воспользуйтесь
+`Issues <https://github.com/WLM1ke/apimoex/issues>`_ на GitHub с указанием ссылки на описание запроса:
+
+* Полный перечень возможных `запросов <https://iss.moex.com/iss/reference/>`_ к MOEX ISS
+* Официальное `Руководство разработчика <https://fs.moex.com/files/6523>`_ с дополнительной информацией
+
+Начало работы
+=============
+
+Установка
+---------
+
+.. code-block:: Bash
+
+   $ pip install apimoex
+
+Пример использования реализованных запросов
+-------------------------------------------
+
+История котировок `SNGSP в режиме TQBR <https://www.moex.com/ru/issue.aspx?board=TQBR&code=SNGSP>`_:
+
+.. code-block:: python
+
+   import requests
+
+   import apimoex
+   import pandas as pd
+
+   with requests.Session() as session:
+       data = apimoex.get_board_history(session, 'SNGSP')
+       df = pd.DataFrame(data)
+       df.set_index('TRADEDATE', inplace=True)
+       print(df.head(), '\n')
+       print(df.tail(), '\n')
+       df.info()
+
+.. code-block::
+
+               BOARDID  CLOSE    VOLUME         VALUE
+    TRADEDATE
+    2014-06-09    TQBR  27.48  12674200  3.484352e+08
+    2014-06-10    TQBR  27.55  14035900  3.856417e+08
+    2014-06-11    TQBR  28.15  27208800  7.602146e+08
+    2014-06-16    TQBR  28.27  68059900  1.913160e+09
+    2014-06-17    TQBR  28.20  22101600  6.292844e+08
+
+               BOARDID   CLOSE     VOLUME         VALUE
+    TRADEDATE
+    2019-09-04    TQBR  38.060  243010500  9.348435e+09
+    2019-09-05    TQBR  36.140  129366600  4.704949e+09
+    2019-09-06    TQBR  35.475   62389000  2.201887e+09
+    2019-09-09    TQBR  34.570   54331300  1.905837e+09
+    2019-09-10    TQBR  35.250   45966000  1.605849e+09
+
+    <class 'pandas.core.frame.DataFrame'>
+    Index: 1326 entries, 2014-06-09 to 2019-09-10
+    Data columns (total 4 columns):
+    BOARDID    1326 non-null object
+    CLOSE      1326 non-null float64
+    VOLUME     1326 non-null int64
+    VALUE      1326 non-null float64
+    dtypes: float64(2), int64(1), object(1)
+    memory usage: 51.8+ KB
+
+Пример реализации запроса с помощью клиента
+-------------------------------------------
+
+Перечень акций, торгующихся в режиме TQBR (`описание запроса <https://iss.moex.com/iss/reference/32>`_):
+
+.. code-block:: python
+
+   import requests
+
+   import apimoex
+   import pandas as pd
+
+
+   request_url = ('https://iss.moex.com/iss/engines/stock/'
+                  'markets/shares/boards/TQBR/securities.json')
+   arguments = {'securities.columns': ('SECID,'
+                                       'REGNUMBER,'
+                                       'LOTSIZE,'
+                                       'SHORTNAME')}
+   with requests.Session() as session:
+       iss = apimoex.ISSClient(session, request_url, arguments)
+       data = iss.get()
+       df = pd.DataFrame(data['securities'])
+       df.set_index('SECID', inplace=True)
+       print(df.head(), '\n')
+       print(df.tail(), '\n')
+       df.info()
+
+.. code-block::
+
+              REGNUMBER  LOTSIZE   SHORTNAME
+    SECID
+    ABRD   1-02-12500-A       10  АбрауДюрсо
+    AFKS   1-05-01669-A      100  Система ао
+    AFLT   1-01-00010-A       10    Аэрофлот
+    AGRO           None        1    AGRO-гдр
+    AKRN   1-03-00207-A        1       Акрон
+
+              REGNUMBER  LOTSIZE   SHORTNAME
+    SECID
+    YNDX           None        1  Yandex clA
+    YRSB   1-01-50099-A       10     ТНСэнЯр
+    YRSBP  2-01-50099-A       10   ТНСэнЯр-п
+    ZILL   1-02-00036-A        1      ЗИЛ ао
+    ZVEZ   1-01-00169-D     1000   ЗВЕЗДА ао
+
+    <class 'pandas.core.frame.DataFrame'>
+    Index: 264 entries, ABRD to ZVEZ
+    Data columns (total 3 columns):
+    REGNUMBER    255 non-null object
+    LOTSIZE      264 non-null int64
+    SHORTNAME    264 non-null object
+    dtypes: int64(1), object(2)
+    memory usage: 8.2+ KB
+
+
```

### Comparing `apimoex-1.2.0/README.rst` & `apimoex-1.3.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,53 +1,59 @@
 MOEX ISS API
-====================
+============
+
 .. image:: https://github.com/WLM1ke/apimoex/workflows/tests/badge.svg
     :target: https://github.com/WLM1ke/apimoex/actions
 .. image:: https://codecov.io/gh/WLM1ke/apimoex/branch/master/graph/badge.svg
     :target: https://codecov.io/gh/WLM1ke/apimoex
 .. image:: https://badge.fury.io/py/apimoex.svg
     :target: https://badge.fury.io/py/apimoex
 
-Реализация части  запросов к `MOEX Informational & Statistical Server <https://www.moex.com/a2193>`_.
+Реализация части запросов к `MOEX Informational & Statistical Server <https://www.moex.com/a2193>`_.
 
 Документация
 ------------
+
 https://wlm1ke.github.io/apimoex/
 
 Основные возможности
 --------------------
+
 Реализовано несколько функций-запросов информации о торгуемых акциях и их исторических котировках, результаты которых
 напрямую конвертируются в pandas.DataFrame.
 
 Работа функций базируется на универсальном клиенте, позволяющем осуществлять произвольные запросы к MOEX ISS, поэтому
 перечень доступных функций-запросов может быть легко расширен. При необходимости добавления функций воспользуйтесь
 `Issues <https://github.com/WLM1ke/apimoex/issues>`_ на GitHub с указанием ссылки на описание запроса:
 
 * Полный перечень возможных `запросов <https://iss.moex.com/iss/reference/>`_ к MOEX ISS
 * Официальное `Руководство разработчика <https://fs.moex.com/files/6523>`_ с дополнительной информацией
 
 Начало работы
 =============
+
 Установка
 ---------
 
 .. code-block:: Bash
 
    $ pip install apimoex
 
 Пример использования реализованных запросов
 -------------------------------------------
-История котировок SNGSP в режиме TQBR::
+
+История котировок `SNGSP в режиме TQBR <https://www.moex.com/ru/issue.aspx?board=TQBR&code=SNGSP>`_:
+
+.. code-block:: python
 
    import requests
 
    import apimoex
    import pandas as pd
 
-
    with requests.Session() as session:
        data = apimoex.get_board_history(session, 'SNGSP')
        df = pd.DataFrame(data)
        df.set_index('TRADEDATE', inplace=True)
        print(df.head(), '\n')
        print(df.tail(), '\n')
        df.info()
@@ -78,15 +84,18 @@
     VOLUME     1326 non-null int64
     VALUE      1326 non-null float64
     dtypes: float64(2), int64(1), object(1)
     memory usage: 51.8+ KB
 
 Пример реализации запроса с помощью клиента
 -------------------------------------------
-Перечень акций, торгующихся в режиме TQBR (`описание запроса <https://iss.moex.com/iss/reference/32>`_)::
+
+Перечень акций, торгующихся в режиме TQBR (`описание запроса <https://iss.moex.com/iss/reference/32>`_):
+
+.. code-block:: python
 
    import requests
 
    import apimoex
    import pandas as pd
```

### Comparing `apimoex-1.2.0/apimoex/__init__.py` & `apimoex-1.3.0/apimoex/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,8 +4,8 @@
 Работа функций базируется на универсальном клиенте, позволяющем осуществлять произвольные запросы к MOEX ISS, поэтому
 перечень доступных функций-запросов может быть легко расширен.
 """
 from .client import ISSClient
 
 from .requests import *
 
-__version__ = "1.2.0"
+__version__ = "1.3.0"
```

### Comparing `apimoex-1.2.0/apimoex/client.py` & `apimoex-1.3.0/apimoex/client.py`

 * *Files identical despite different names*

### Comparing `apimoex-1.2.0/apimoex/requests.py` & `apimoex-1.3.0/apimoex/requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,23 +22,25 @@
     "get_board_candle_borders",
     "get_market_candles",
     "get_board_candles",
     "get_board_dates",
     "get_board_securities",
     "get_market_history",
     "get_board_history",
+    "get_index_tickers",
 ]
 
 
 def _make_query(
     *,
     q: Optional[str] = None,
     interval: Optional[int] = None,
     start: Optional[str] = None,
     end: Optional[str] = None,
+    date: Optional[str] = None,
     table: Optional[str] = None,
     columns: Optional[Tuple[str, ...]] = None,
 ) -> Dict[str, Union[str, int]]:
     """Формирует дополнительные параметры запроса к MOEX ISS.
 
     В случае None значений не добавляются в запрос.
 
@@ -46,14 +48,16 @@
         Строка с частью характеристик бумаги для поиска.
     :param interval:
         Размер свечки.
     :param start:
         Начальная дата котировок.
     :param end:
         Конечная дата котировок.
+    :param date:
+        Точная дата (используется при получении тикеров в индексе).
     :param table:
         Таблица, которую нужно загрузить (для запросов, предполагающих наличие нескольких таблиц).
     :param columns:
         Кортеж столбцов, которые нужно загрузить.
 
     :return:
         Словарь с дополнительными параметрами запроса.
@@ -63,14 +67,16 @@
         query["q"] = q
     if interval:
         query["interval"] = interval
     if start:
         query["from"] = start
     if end:
         query["till"] = end
+    if date:
+        query["date"] = date
     if table:
         query["iss.only"] = f"{table},history.cursor"
     if columns:
         query[f"{table}.columns"] = ",".join(columns)
     return query
 
 
@@ -529,7 +535,52 @@
     url = (
         f"https://iss.moex.com/iss/history/engines/{engine}/markets/{market}/"
         f"boards/{board}/securities/{security}.json"
     )
     table = "history"
     query = _make_query(start=start, end=end, table=table, columns=columns)
     return _get_long_data(session, url, table, query)
+
+
+def get_index_tickers(
+    session: requests.Session,
+    index: str,
+    date: Optional[str] = None,
+    columns: Optional[Tuple[str, ...]] = (
+        "ticker",
+        "from",
+        "till",
+        "tradingsession",
+    ),
+    market: str = "index",
+    engine: str = "stock",
+):
+    """Получить информацию по составу указанного индекса за указанную дату.
+
+    Описание запроса - https://iss.moex.com/iss/reference/148
+
+    Список индексов - https://iss.moex.com/iss/statistics/engines/stock/markets/index/analytics
+
+    :param session:
+        Сессия интернет соединения.
+    :param index:
+        Название индекса. Например, IMOEX.
+    :param date:
+        Дата вида ГГГГ-ММ-ДД. Если указано, то будут показаны только активные инструменты, по которым тогда рассчитывалось значение индекса. Если в указанный день не было торгов, то вернёт пустой список! При отсутствии данные будут загружены с начала истории. 
+    :param columns:
+        Кортеж столбцов, которые нужно загрузить - по умолчанию режим торгов, дата торгов, цена закрытия и объем в
+        штуках и стоимости. Если пустой или None, то загружаются все столбцы.
+    :param market:
+        Рынок - по умолчанию индексы.
+    :param engine:
+        Движок - по умолчанию акции.
+
+    :return:
+        Список словарей, которые напрямую конвертируется в pandas.DataFrame.
+    """
+    url = (
+        f"https://iss.moex.com/iss/statistics/engines/{engine}/markets/{market}/"
+        f"analytics/{index}/tickers.json"
+    )
+    table = "tickers"
+    query = _make_query(date=date, table=table, columns=columns)
+    return _get_short_data(session, url, table, query)
```

### Comparing `apimoex-1.2.0/apimoex.egg-info/PKG-INFO` & `apimoex-1.3.0/apimoex.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,150 +1,16 @@
 Metadata-Version: 2.1
 Name: apimoex
-Version: 1.2.0
+Version: 1.3.0
 Summary: MOEX ISS API
 Home-page: https://wlm1ke.github.io/apimoex/
 Author: Mikhail Korotkov aka WLMike
 Author-email: wlmike@gmail.com
 License: http://unlicense.org
 Project-URL: Source, https://github.com/WLM1ke/apimoex
-Description: MOEX ISS API
-        ====================
-        .. image:: https://github.com/WLM1ke/apimoex/workflows/tests/badge.svg
-            :target: https://github.com/WLM1ke/apimoex/actions
-        .. image:: https://codecov.io/gh/WLM1ke/apimoex/branch/master/graph/badge.svg
-            :target: https://codecov.io/gh/WLM1ke/apimoex
-        .. image:: https://badge.fury.io/py/apimoex.svg
-            :target: https://badge.fury.io/py/apimoex
-        
-        Реализация части  запросов к `MOEX Informational & Statistical Server <https://www.moex.com/a2193>`_.
-        
-        Документация
-        ------------
-        https://wlm1ke.github.io/apimoex/
-        
-        Основные возможности
-        --------------------
-        Реализовано несколько функций-запросов информации о торгуемых акциях и их исторических котировках, результаты которых
-        напрямую конвертируются в pandas.DataFrame.
-        
-        Работа функций базируется на универсальном клиенте, позволяющем осуществлять произвольные запросы к MOEX ISS, поэтому
-        перечень доступных функций-запросов может быть легко расширен. При необходимости добавления функций воспользуйтесь
-        `Issues <https://github.com/WLM1ke/apimoex/issues>`_ на GitHub с указанием ссылки на описание запроса:
-        
-        * Полный перечень возможных `запросов <https://iss.moex.com/iss/reference/>`_ к MOEX ISS
-        * Официальное `Руководство разработчика <https://fs.moex.com/files/6523>`_ с дополнительной информацией
-        
-        Начало работы
-        =============
-        Установка
-        ---------
-        
-        .. code-block:: Bash
-        
-           $ pip install apimoex
-        
-        Пример использования реализованных запросов
-        -------------------------------------------
-        История котировок SNGSP в режиме TQBR::
-        
-           import requests
-        
-           import apimoex
-           import pandas as pd
-        
-        
-           with requests.Session() as session:
-               data = apimoex.get_board_history(session, 'SNGSP')
-               df = pd.DataFrame(data)
-               df.set_index('TRADEDATE', inplace=True)
-               print(df.head(), '\n')
-               print(df.tail(), '\n')
-               df.info()
-        
-        .. code-block::
-        
-                       BOARDID  CLOSE    VOLUME         VALUE
-            TRADEDATE
-            2014-06-09    TQBR  27.48  12674200  3.484352e+08
-            2014-06-10    TQBR  27.55  14035900  3.856417e+08
-            2014-06-11    TQBR  28.15  27208800  7.602146e+08
-            2014-06-16    TQBR  28.27  68059900  1.913160e+09
-            2014-06-17    TQBR  28.20  22101600  6.292844e+08
-        
-                       BOARDID   CLOSE     VOLUME         VALUE
-            TRADEDATE
-            2019-09-04    TQBR  38.060  243010500  9.348435e+09
-            2019-09-05    TQBR  36.140  129366600  4.704949e+09
-            2019-09-06    TQBR  35.475   62389000  2.201887e+09
-            2019-09-09    TQBR  34.570   54331300  1.905837e+09
-            2019-09-10    TQBR  35.250   45966000  1.605849e+09
-        
-            <class 'pandas.core.frame.DataFrame'>
-            Index: 1326 entries, 2014-06-09 to 2019-09-10
-            Data columns (total 4 columns):
-            BOARDID    1326 non-null object
-            CLOSE      1326 non-null float64
-            VOLUME     1326 non-null int64
-            VALUE      1326 non-null float64
-            dtypes: float64(2), int64(1), object(1)
-            memory usage: 51.8+ KB
-        
-        Пример реализации запроса с помощью клиента
-        -------------------------------------------
-        Перечень акций, торгующихся в режиме TQBR (`описание запроса <https://iss.moex.com/iss/reference/32>`_)::
-        
-           import requests
-        
-           import apimoex
-           import pandas as pd
-        
-        
-           request_url = ('https://iss.moex.com/iss/engines/stock/'
-                          'markets/shares/boards/TQBR/securities.json')
-           arguments = {'securities.columns': ('SECID,'
-                                               'REGNUMBER,'
-                                               'LOTSIZE,'
-                                               'SHORTNAME')}
-           with requests.Session() as session:
-               iss = apimoex.ISSClient(session, request_url, arguments)
-               data = iss.get()
-               df = pd.DataFrame(data['securities'])
-               df.set_index('SECID', inplace=True)
-               print(df.head(), '\n')
-               print(df.tail(), '\n')
-               df.info()
-        
-        .. code-block::
-        
-                      REGNUMBER  LOTSIZE   SHORTNAME
-            SECID
-            ABRD   1-02-12500-A       10  АбрауДюрсо
-            AFKS   1-05-01669-A      100  Система ао
-            AFLT   1-01-00010-A       10    Аэрофлот
-            AGRO           None        1    AGRO-гдр
-            AKRN   1-03-00207-A        1       Акрон
-        
-                      REGNUMBER  LOTSIZE   SHORTNAME
-            SECID
-            YNDX           None        1  Yandex clA
-            YRSB   1-01-50099-A       10     ТНСэнЯр
-            YRSBP  2-01-50099-A       10   ТНСэнЯр-п
-            ZILL   1-02-00036-A        1      ЗИЛ ао
-            ZVEZ   1-01-00169-D     1000   ЗВЕЗДА ао
-        
-            <class 'pandas.core.frame.DataFrame'>
-            Index: 264 entries, ABRD to ZVEZ
-            Data columns (total 3 columns):
-            REGNUMBER    255 non-null object
-            LOTSIZE      264 non-null int64
-            SHORTNAME    264 non-null object
-            dtypes: int64(1), object(2)
-            memory usage: 8.2+ KB
-        
 Keywords: moex iss api
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: Public Domain
 Classifier: Natural Language :: Russian
@@ -153,7 +19,153 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+MOEX ISS API
+============
+
+.. image:: https://github.com/WLM1ke/apimoex/workflows/tests/badge.svg
+    :target: https://github.com/WLM1ke/apimoex/actions
+.. image:: https://codecov.io/gh/WLM1ke/apimoex/branch/master/graph/badge.svg
+    :target: https://codecov.io/gh/WLM1ke/apimoex
+.. image:: https://badge.fury.io/py/apimoex.svg
+    :target: https://badge.fury.io/py/apimoex
+
+Реализация части запросов к `MOEX Informational & Statistical Server <https://www.moex.com/a2193>`_.
+
+Документация
+------------
+
+https://wlm1ke.github.io/apimoex/
+
+Основные возможности
+--------------------
+
+Реализовано несколько функций-запросов информации о торгуемых акциях и их исторических котировках, результаты которых
+напрямую конвертируются в pandas.DataFrame.
+
+Работа функций базируется на универсальном клиенте, позволяющем осуществлять произвольные запросы к MOEX ISS, поэтому
+перечень доступных функций-запросов может быть легко расширен. При необходимости добавления функций воспользуйтесь
+`Issues <https://github.com/WLM1ke/apimoex/issues>`_ на GitHub с указанием ссылки на описание запроса:
+
+* Полный перечень возможных `запросов <https://iss.moex.com/iss/reference/>`_ к MOEX ISS
+* Официальное `Руководство разработчика <https://fs.moex.com/files/6523>`_ с дополнительной информацией
+
+Начало работы
+=============
+
+Установка
+---------
+
+.. code-block:: Bash
+
+   $ pip install apimoex
+
+Пример использования реализованных запросов
+-------------------------------------------
+
+История котировок `SNGSP в режиме TQBR <https://www.moex.com/ru/issue.aspx?board=TQBR&code=SNGSP>`_:
+
+.. code-block:: python
+
+   import requests
+
+   import apimoex
+   import pandas as pd
+
+   with requests.Session() as session:
+       data = apimoex.get_board_history(session, 'SNGSP')
+       df = pd.DataFrame(data)
+       df.set_index('TRADEDATE', inplace=True)
+       print(df.head(), '\n')
+       print(df.tail(), '\n')
+       df.info()
+
+.. code-block::
+
+               BOARDID  CLOSE    VOLUME         VALUE
+    TRADEDATE
+    2014-06-09    TQBR  27.48  12674200  3.484352e+08
+    2014-06-10    TQBR  27.55  14035900  3.856417e+08
+    2014-06-11    TQBR  28.15  27208800  7.602146e+08
+    2014-06-16    TQBR  28.27  68059900  1.913160e+09
+    2014-06-17    TQBR  28.20  22101600  6.292844e+08
+
+               BOARDID   CLOSE     VOLUME         VALUE
+    TRADEDATE
+    2019-09-04    TQBR  38.060  243010500  9.348435e+09
+    2019-09-05    TQBR  36.140  129366600  4.704949e+09
+    2019-09-06    TQBR  35.475   62389000  2.201887e+09
+    2019-09-09    TQBR  34.570   54331300  1.905837e+09
+    2019-09-10    TQBR  35.250   45966000  1.605849e+09
+
+    <class 'pandas.core.frame.DataFrame'>
+    Index: 1326 entries, 2014-06-09 to 2019-09-10
+    Data columns (total 4 columns):
+    BOARDID    1326 non-null object
+    CLOSE      1326 non-null float64
+    VOLUME     1326 non-null int64
+    VALUE      1326 non-null float64
+    dtypes: float64(2), int64(1), object(1)
+    memory usage: 51.8+ KB
+
+Пример реализации запроса с помощью клиента
+-------------------------------------------
+
+Перечень акций, торгующихся в режиме TQBR (`описание запроса <https://iss.moex.com/iss/reference/32>`_):
+
+.. code-block:: python
+
+   import requests
+
+   import apimoex
+   import pandas as pd
+
+
+   request_url = ('https://iss.moex.com/iss/engines/stock/'
+                  'markets/shares/boards/TQBR/securities.json')
+   arguments = {'securities.columns': ('SECID,'
+                                       'REGNUMBER,'
+                                       'LOTSIZE,'
+                                       'SHORTNAME')}
+   with requests.Session() as session:
+       iss = apimoex.ISSClient(session, request_url, arguments)
+       data = iss.get()
+       df = pd.DataFrame(data['securities'])
+       df.set_index('SECID', inplace=True)
+       print(df.head(), '\n')
+       print(df.tail(), '\n')
+       df.info()
+
+.. code-block::
+
+              REGNUMBER  LOTSIZE   SHORTNAME
+    SECID
+    ABRD   1-02-12500-A       10  АбрауДюрсо
+    AFKS   1-05-01669-A      100  Система ао
+    AFLT   1-01-00010-A       10    Аэрофлот
+    AGRO           None        1    AGRO-гдр
+    AKRN   1-03-00207-A        1       Акрон
+
+              REGNUMBER  LOTSIZE   SHORTNAME
+    SECID
+    YNDX           None        1  Yandex clA
+    YRSB   1-01-50099-A       10     ТНСэнЯр
+    YRSBP  2-01-50099-A       10   ТНСэнЯр-п
+    ZILL   1-02-00036-A        1      ЗИЛ ао
+    ZVEZ   1-01-00169-D     1000   ЗВЕЗДА ао
+
+    <class 'pandas.core.frame.DataFrame'>
+    Index: 264 entries, ABRD to ZVEZ
+    Data columns (total 3 columns):
+    REGNUMBER    255 non-null object
+    LOTSIZE      264 non-null int64
+    SHORTNAME    264 non-null object
+    dtypes: int64(1), object(2)
+    memory usage: 8.2+ KB
+
+
```

### Comparing `apimoex-1.2.0/setup.py` & `apimoex-1.3.0/setup.py`

 * *Files identical despite different names*

