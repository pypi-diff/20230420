# Comparing `tmp/aiorocket-1.3.1b1.tar.gz` & `tmp/aiorocket-1.3.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiorocket-1.3.1b1.tar", last modified: Sat Mar 25 13:46:12 2023, max compression
+gzip compressed data, was "aiorocket-1.3.1b2.tar", last modified: Tue Apr  4 15:50:46 2023, max compression
```

## Comparing `aiorocket-1.3.1b1.tar` & `aiorocket-1.3.1b2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 owl       (1000) owl       (1000)        0 2023-03-25 13:46:12.373497 aiorocket-1.3.1b1/
--rw-r--r--   0 owl       (1000) owl       (1000)    35149 2023-03-25 07:32:30.000000 aiorocket-1.3.1b1/LICENSE.txt
--rw-r--r--   0 owl       (1000) owl       (1000)     4189 2023-03-25 13:46:12.373497 aiorocket-1.3.1b1/PKG-INFO
--rw-r--r--   0 owl       (1000) owl       (1000)     3636 2023-03-25 13:38:59.000000 aiorocket-1.3.1b1/README.md
-drwxr-xr-x   0 owl       (1000) owl       (1000)        0 2023-03-25 13:46:12.370164 aiorocket-1.3.1b1/aiorocket/
--rw-r--r--   0 owl       (1000) owl       (1000)     5918 2023-03-25 13:38:59.000000 aiorocket-1.3.1b1/aiorocket/__init__.py
--rw-r--r--   0 owl       (1000) owl       (1000)     4036 2023-03-25 06:41:43.000000 aiorocket-1.3.1b1/aiorocket/classes.py
-drwxr-xr-x   0 owl       (1000) owl       (1000)        0 2023-03-25 13:46:12.373497 aiorocket-1.3.1b1/aiorocket.egg-info/
--rw-r--r--   0 owl       (1000) owl       (1000)     4189 2023-03-25 13:46:12.000000 aiorocket-1.3.1b1/aiorocket.egg-info/PKG-INFO
--rw-r--r--   0 owl       (1000) owl       (1000)      243 2023-03-25 13:46:12.000000 aiorocket-1.3.1b1/aiorocket.egg-info/SOURCES.txt
--rw-r--r--   0 owl       (1000) owl       (1000)        1 2023-03-25 13:46:12.000000 aiorocket-1.3.1b1/aiorocket.egg-info/dependency_links.txt
--rw-r--r--   0 owl       (1000) owl       (1000)        8 2023-03-25 13:46:12.000000 aiorocket-1.3.1b1/aiorocket.egg-info/requires.txt
--rw-r--r--   0 owl       (1000) owl       (1000)       10 2023-03-25 13:46:12.000000 aiorocket-1.3.1b1/aiorocket.egg-info/top_level.txt
--rw-r--r--   0 owl       (1000) owl       (1000)      625 2023-03-25 13:38:59.000000 aiorocket-1.3.1b1/pyproject.toml
--rw-r--r--   0 owl       (1000) owl       (1000)       38 2023-03-25 13:46:12.373497 aiorocket-1.3.1b1/setup.cfg
+drwxr-xr-x   0 owl       (1000) owl       (1000)        0 2023-04-04 15:50:46.256376 aiorocket-1.3.1b2/
+-rw-r--r--   0 owl       (1000) owl       (1000)    35149 2023-03-25 07:32:30.000000 aiorocket-1.3.1b2/LICENSE.txt
+-rw-r--r--   0 owl       (1000) owl       (1000)     4711 2023-04-04 15:50:46.253042 aiorocket-1.3.1b2/PKG-INFO
+-rw-r--r--   0 owl       (1000) owl       (1000)     4158 2023-04-04 15:40:35.000000 aiorocket-1.3.1b2/README.md
+drwxr-xr-x   0 owl       (1000) owl       (1000)        0 2023-04-04 15:50:46.253042 aiorocket-1.3.1b2/aiorocket/
+-rw-r--r--   0 owl       (1000) owl       (1000)     5948 2023-04-04 13:33:11.000000 aiorocket-1.3.1b2/aiorocket/__init__.py
+-rw-r--r--   0 owl       (1000) owl       (1000)     4179 2023-04-04 13:30:48.000000 aiorocket-1.3.1b2/aiorocket/classes.py
+drwxr-xr-x   0 owl       (1000) owl       (1000)        0 2023-04-04 15:50:46.253042 aiorocket-1.3.1b2/aiorocket.egg-info/
+-rw-r--r--   0 owl       (1000) owl       (1000)     4711 2023-04-04 15:50:46.000000 aiorocket-1.3.1b2/aiorocket.egg-info/PKG-INFO
+-rw-r--r--   0 owl       (1000) owl       (1000)      243 2023-04-04 15:50:46.000000 aiorocket-1.3.1b2/aiorocket.egg-info/SOURCES.txt
+-rw-r--r--   0 owl       (1000) owl       (1000)        1 2023-04-04 15:50:46.000000 aiorocket-1.3.1b2/aiorocket.egg-info/dependency_links.txt
+-rw-r--r--   0 owl       (1000) owl       (1000)        8 2023-04-04 15:50:46.000000 aiorocket-1.3.1b2/aiorocket.egg-info/requires.txt
+-rw-r--r--   0 owl       (1000) owl       (1000)       10 2023-04-04 15:50:46.000000 aiorocket-1.3.1b2/aiorocket.egg-info/top_level.txt
+-rw-r--r--   0 owl       (1000) owl       (1000)      625 2023-04-04 15:49:24.000000 aiorocket-1.3.1b2/pyproject.toml
+-rw-r--r--   0 owl       (1000) owl       (1000)       38 2023-04-04 15:50:46.256376 aiorocket-1.3.1b2/setup.cfg
```

### Comparing `aiorocket-1.3.1b1/LICENSE.txt` & `aiorocket-1.3.1b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiorocket-1.3.1b1/PKG-INFO` & `aiorocket-1.3.1b2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,11 @@
-Metadata-Version: 2.1
-Name: aiorocket
-Version: 1.3.1b1
-Summary: Async Python SDK for TON Rocket
-Author-email: Sovenok-Hacker <artemka.hvostov@yandex.ru>
-Project-URL: homepage, https://github.com/Sovenok-Hacker/aiorocket
-Project-URL: repository, https://github.com/Sovenok-Hacker/aiorocket.git
-Keywords: ton,rocket,sdk,async,the open network,bot,telegram,crypto,cryptocurrency
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # SDK для работы с TON Rocket
 
+## Это ещё бета-версия, просьба сообщать о любых проблемах
+
 ## 🔐 Авторизация
 
 Как получить токен написано [тут](https://pay.ton-rocket.com/api/).
 
 Mainnet:
 
 ```python
@@ -70,15 +58,15 @@
 ```
 
 ### Создание чека
 Все параметры как в [документации](https://pay.ton-rocket.com/api/#/multi-cheques/ChequesController_createCheque)
 
 Пример:
 ```python
-api.create_cheque({
+await api.create_cheque({
     chequePerUser=0.005,
     usersNumber=100,
     refProgram=50,
     password="pwd",
     description="This cheque is the best",
     sendNotifications=True,
     enableCaptcha=True,
@@ -115,18 +103,18 @@
 ### Создание счёта
 Все параметры как в [документации](https://pay.ton-rocket.com/api/#/tg-invoices/InvoicesController_createInvoice)
 
 Пример:
 ```python
 await api.createInvoice(
     amount=1.23,
-    description="best thing in the world, 1 item",
-    hiddenMessage="thank you",
+    description="покупка лучшой вещи в мире",
+    hiddenMessage="спасибо",
     callbackUrl="https://t.me/ton_rocket",
-    payload="some custom payload I want to see in webhook or when I request invoice",
+    payload="полезна нагрузку, которую я хочу видеть в webhook или когда я запрашиваю счет-фактуру",
     expiredIn=10
 )
 ```
 
 ### Получение счетов
 [Документация](https://pay.ton-rocket.com/api/#/tg-invoices/InvoicesController_deleteInvoice)
 
@@ -154,7 +142,24 @@
 ### Доступные валюты
 [Документация](https://pay.ton-rocket.com/api/#/currencies/CurrenciesController_getCoins)
 
 Пример:
 ```python
 await api.available_currencies()
 ```
+
+## ⚠ Обработка ошибок
+
+```python
+try:
+    api.get_invoice(1234) # вызов метода
+except aiorocket.classes.RocketAPIError as err:
+    print(err.errors)
+```
+
+Результат:
+```json
+{
+    "property": "somePropertyName",
+    "error": "somePropertyName should be less than X"
+}
+```
```

### Comparing `aiorocket-1.3.1b1/README.md` & `aiorocket-1.3.1b2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,25 @@
+Metadata-Version: 2.1
+Name: aiorocket
+Version: 1.3.1b2
+Summary: Async Python SDK for TON Rocket
+Author-email: Sovenok-Hacker <artemka.hvostov@yandex.ru>
+Project-URL: homepage, https://github.com/Sovenok-Hacker/aiorocket
+Project-URL: repository, https://github.com/Sovenok-Hacker/aiorocket.git
+Keywords: ton,rocket,sdk,async,the open network,bot,telegram,crypto,cryptocurrency
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # SDK для работы с TON Rocket
 
+## Это ещё бета-версия, просьба сообщать о любых проблемах
+
 ## 🔐 Авторизация
 
 Как получить токен написано [тут](https://pay.ton-rocket.com/api/).
 
 Mainnet:
 
 ```python
@@ -56,15 +72,15 @@
 ```
 
 ### Создание чека
 Все параметры как в [документации](https://pay.ton-rocket.com/api/#/multi-cheques/ChequesController_createCheque)
 
 Пример:
 ```python
-api.create_cheque({
+await api.create_cheque({
     chequePerUser=0.005,
     usersNumber=100,
     refProgram=50,
     password="pwd",
     description="This cheque is the best",
     sendNotifications=True,
     enableCaptcha=True,
@@ -101,18 +117,18 @@
 ### Создание счёта
 Все параметры как в [документации](https://pay.ton-rocket.com/api/#/tg-invoices/InvoicesController_createInvoice)
 
 Пример:
 ```python
 await api.createInvoice(
     amount=1.23,
-    description="best thing in the world, 1 item",
-    hiddenMessage="thank you",
+    description="покупка лучшой вещи в мире",
+    hiddenMessage="спасибо",
     callbackUrl="https://t.me/ton_rocket",
-    payload="some custom payload I want to see in webhook or when I request invoice",
+    payload="полезна нагрузку, которую я хочу видеть в webhook или когда я запрашиваю счет-фактуру",
     expiredIn=10
 )
 ```
 
 ### Получение счетов
 [Документация](https://pay.ton-rocket.com/api/#/tg-invoices/InvoicesController_deleteInvoice)
 
@@ -139,8 +155,25 @@
 
 ### Доступные валюты
 [Документация](https://pay.ton-rocket.com/api/#/currencies/CurrenciesController_getCoins)
 
 Пример:
 ```python
 await api.available_currencies()
-```
+```
+
+## ⚠ Обработка ошибок
+
+```python
+try:
+    api.get_invoice(1234) # вызов метода
+except aiorocket.classes.RocketAPIError as err:
+    print(err.errors)
+```
+
+Результат:
+```json
+{
+    "property": "somePropertyName",
+    "error": "somePropertyName should be less than X"
+}
+```
```

### Comparing `aiorocket-1.3.1b1/aiorocket/__init__.py` & `aiorocket-1.3.1b2/aiorocket/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,129 +7,129 @@
 
 class Rocket:
     def __init__(self, api_key: str, testnet=False):
         self.BASE_URL = BASEURL_TESTNET if testnet else BASEURL_MAINNET
         self.api_key = api_key
         self._headers = {'Rocket-Pay-Key': self.api_key}
 
-    async def version(self):
+    async def version(self) -> str:
         async with aiohttp.request('GET', f'{self.BASE_URL}/version') as r:
             return (await r.json()).get('version')
 
-    async def info(self):
+    async def info(self) -> dict:
         async with aiohttp.request('GET', f'{self.BASE_URL}/app/info', headers=self._headers) as r:
             r = await r.json()
             if not r['success']:
                 raise RocketAPIError(r['message'])
             return {'name': r['data']['name'], 'feePercents': r['data']['feePercents']}
 
-    async def balance(self, only_positive=True):
+    async def balance(self, only_positive=True) -> dict:
         async with aiohttp.request('GET', f'{self.BASE_URL}/app/info', headers=self._headers) as r:
             r = await r.json()
             if not r['success']:
                 raise RocketAPIError(r['message'])
             result = {}
             for pair in r['data']['balances']:
                 if only_positive and not pair['balance']:
                     continue
                 result[pair['currency']] = pair['balance']
             return result
 
-    async def send(self, **params):
+    async def send(self, **params) -> int:
         async with aiohttp.request('POST', f'{self.BASE_URL}/app/transfer', json=params, headers=self._headers) as r:
             r = await r.json()
             if not r['success']:
                 raise RocketAPIError(r['message'])
             return r['data']['id']
 
-    async def withdraw(self, **params):
+    async def withdraw(self, **params) -> int:
         async with aiohttp.request('POST', f'{self.BASE_URL}/app/withdrawal', json=params, headers=self._headers) as r:
             r = await r.json()
             if not r['success']:
                 raise RocketAPIError(r['message'])
             return r['data']['id']
 
-    async def create_cheque(self, **params):
+    async def create_cheque(self, **params) -> Cheque:
         async with aiohttp.request('POST', f'{self.BASE_URL}/multi-cheques', json=params, headers=self._headers) as r:
             r = await r.json()
             if not r['success']:
                 raise RocketAPIError(r['message'])
             cheque = r['data']
         return Cheque.fromjson(cheque)
 
-    async def get_cheques(self, limit: int = 100, offset: int = 0):
+    async def get_cheques(self, limit: int = 100, offset: int = 0) -> list:
         async with aiohttp.request('GET', f'{self.BASE_URL}/multi-cheques', params={'limit': limit, 'offset': offset}, headers=self._headers) as r:
             r = await r.json()
             if not r['success']:
-                raise RocketAPIError(r['message'])
+                raise RocketAPIError(r)
             r = r['data']
         result = []
         for cheque in r['results']:
             result.append(Cheque.fromjson(cheque))
         return result
 
-    async def get_cheque(self, id: int):
+    async def get_cheque(self, id: int) -> Cheque:
         async with aiohttp.request('GET', f'{self.BASE_URL}/multi-cheques/{id}', headers=self._headers) as r:
             r = await r.json()
             if not r['success']:
-                raise RocketAPIError(r['message'])
+                raise RocketAPIError(r)
             cheque = r['data']
         return Cheque.fromjson(cheque)
 
-    async def edit_cheque(self, id: int, **params):
+    async def edit_cheque(self, id: int, **params) -> Cheque:
         async with aiohttp.request('PUT', f'{self.BASE_URL}/multi-cheques/{id}', headers=self._headers) as r:
             r = await r.json()
             if not r['success']:
-                raise RocketAPIError(r['message'])
+                raise RocketAPIError(r)
             return Cheque.fromjson(r)
 
-    async def delete_cheque(self, id: int):
+    async def delete_cheque(self, id: int) -> None:
         async with aiohttp.request('DELETE', f'{self.BASE_URL}/multi-cheques/{id}', headers=self._headers) as r:
             r = await r.json()
             if not r['success']:
-                raise RocketAPIError(r['message'])
+                raise RocketAPIError(r)
 
-    async def create_invoice(self, **params):
+    async def create_invoice(self, **params) -> Invoice:
         async with aiohttp.request('POST', f'{self.BASE_URL}/tg-invoices', json=params, headers=self._headers) as r:
             r = await r.json()
             if not r['success']:
-                raise RocketAPIError(r['message'])
+                raise RocketAPIError(r)
             r = r['data']
         return Invoice.fromjson(r)
 
-    async def get_invoices(self, limit: int = 100, offset: int = 0):
+    async def get_invoices(self, limit: int = 100, offset: int = 0) -> list:
         async with aiohttp.request('GET', f'{self.BASE_URL}/tg-invoices', params={'limit': limit, 'offset': offset}, headers=self._headers) as r:
             r = await r.json()
             if not r['success']:
-                raise RocketAPIError(r['message'])
+                raise RocketAPIError(r)
             r = r['data']
         result = []
         for invoice in r['results']:
             result.append(Invoice.fromjson(invoice))
         return result
 
-    async def get_invoice(self, id: int):
+    async def get_invoice(self, id: int) -> Invoice:
         async with aiohttp.request('GET', f'{self.BASE_URL}/tg-invoices/{id}', headers=self._headers) as r:
             r = await r.json()
             if not r['success']:
-                raise RocketAPIError(r['message'])
+                raise RocketAPIError(r)
             invoice = r['data']
         return Invoice.fromjson(invoice)
 
-    async def delete_cheque(self, id: int):
+    async def delete_cheque(self, id: int) -> None:
         async with aiohttp.request('DELETE', f'{self.BASE_URL}/tg-invoices/{id}', headers=self._headers) as r:
             r = await r.json()
             if not r['success']:
-                raise RocketAPIError(r['message'])
+                raise RocketAPIError(r)
 
-    async def available_currencies(self):
+    async def available_currencies(self) -> list:
         async with aiohttp.request('GET', f'{self.BASE_URL}/currencies/available') as r:
             r = await r.json()
             if not r['success']:
-                raise RocketAPIError(r['message'])
+                raise RocketAPIError(r)
         results = []
         for currency in r['data']['results']:
             results.append(Currency(
                 currency.get('currency'),
                 currency.get('name'),
                 currency.get('minTransfer'),
                 currency.get('minCheque'),
```

### Comparing `aiorocket-1.3.1b1/aiorocket/classes.py` & `aiorocket-1.3.1b2/aiorocket/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import aiohttp
 
-class RocketAPIError(BaseException):
-    pass
+class RocketAPIError(Exception):
+    def __init__(self, data):
+        self.message = data['message']
+        self.errors = data.get('errors') or []
+        super().__init__(self.message)
 
 class Cheque:
     def __init__(self, id: int, currency: str, total: int, users: int, password: str, description: str, noitifications: bool, captcha: bool, telegramResources: list, refPercents: int, state: str, link: str, activations: int, refRewards: int, disabledLangs: list, forPremium: bool, forNewUsers: bool, linkedWallet: bool):
         self.id = id
         self.currency = currency
         self.total = total
         self.users = users
@@ -99,8 +102,8 @@
         return self.currency
 
     async def get_price(self, currency: str = 'RUB', fiat: bool = True):
         async with aiohttp.request('GET', f'https://trade.ton-rocket.com/rates/{"fiat" if fiat else "crypto"}/{self.currency}/{currency}') as r:
             r = await r.json()
             if not r['success']:
                 raise RocketAPIError(r['message'])
-        return r['data'].get('rate')
+        return r['data'].get('rate')
```

### Comparing `aiorocket-1.3.1b1/aiorocket.egg-info/PKG-INFO` & `aiorocket-1.3.1b2/aiorocket.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: aiorocket
-Version: 1.3.1b1
+Version: 1.3.1b2
 Summary: Async Python SDK for TON Rocket
 Author-email: Sovenok-Hacker <artemka.hvostov@yandex.ru>
 Project-URL: homepage, https://github.com/Sovenok-Hacker/aiorocket
 Project-URL: repository, https://github.com/Sovenok-Hacker/aiorocket.git
 Keywords: ton,rocket,sdk,async,the open network,bot,telegram,crypto,cryptocurrency
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # SDK для работы с TON Rocket
 
+## Это ещё бета-версия, просьба сообщать о любых проблемах
+
 ## 🔐 Авторизация
 
 Как получить токен написано [тут](https://pay.ton-rocket.com/api/).
 
 Mainnet:
 
 ```python
@@ -70,15 +72,15 @@
 ```
 
 ### Создание чека
 Все параметры как в [документации](https://pay.ton-rocket.com/api/#/multi-cheques/ChequesController_createCheque)
 
 Пример:
 ```python
-api.create_cheque({
+await api.create_cheque({
     chequePerUser=0.005,
     usersNumber=100,
     refProgram=50,
     password="pwd",
     description="This cheque is the best",
     sendNotifications=True,
     enableCaptcha=True,
@@ -115,18 +117,18 @@
 ### Создание счёта
 Все параметры как в [документации](https://pay.ton-rocket.com/api/#/tg-invoices/InvoicesController_createInvoice)
 
 Пример:
 ```python
 await api.createInvoice(
     amount=1.23,
-    description="best thing in the world, 1 item",
-    hiddenMessage="thank you",
+    description="покупка лучшой вещи в мире",
+    hiddenMessage="спасибо",
     callbackUrl="https://t.me/ton_rocket",
-    payload="some custom payload I want to see in webhook or when I request invoice",
+    payload="полезна нагрузку, которую я хочу видеть в webhook или когда я запрашиваю счет-фактуру",
     expiredIn=10
 )
 ```
 
 ### Получение счетов
 [Документация](https://pay.ton-rocket.com/api/#/tg-invoices/InvoicesController_deleteInvoice)
 
@@ -154,7 +156,24 @@
 ### Доступные валюты
 [Документация](https://pay.ton-rocket.com/api/#/currencies/CurrenciesController_getCoins)
 
 Пример:
 ```python
 await api.available_currencies()
 ```
+
+## ⚠ Обработка ошибок
+
+```python
+try:
+    api.get_invoice(1234) # вызов метода
+except aiorocket.classes.RocketAPIError as err:
+    print(err.errors)
+```
+
+Результат:
+```json
+{
+    "property": "somePropertyName",
+    "error": "somePropertyName should be less than X"
+}
+```
```

### Comparing `aiorocket-1.3.1b1/pyproject.toml` & `aiorocket-1.3.1b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aiorocket"
-version = "1.3.1-b1"
+version = "1.3.1-b2"
 description = "Async Python SDK for TON Rocket"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
 readme = "README.md"
 dependencies = [
     "aiohttp"
 ]
```

