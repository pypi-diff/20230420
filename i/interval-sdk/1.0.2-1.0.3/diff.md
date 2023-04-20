# Comparing `tmp/interval_sdk-1.0.2.tar.gz` & `tmp/interval_sdk-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interval_sdk-1.0.2.tar", max compression
+gzip compressed data, was "interval_sdk-1.0.3.tar", max compression
```

## Comparing `interval_sdk-1.0.2.tar` & `interval_sdk-1.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     2968 2023-02-09 22:23:52.939868 interval_sdk-1.0.2/README.md
--rw-r--r--   0        0        0     1890 2023-04-07 20:59:55.559775 interval_sdk-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      331 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/classes/__init__.py
--rw-r--r--   0        0        0      422 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/classes/action.py
--rw-r--r--   0        0        0     7024 2023-04-07 20:59:44.056525 interval_sdk-1.0.2/src/interval_sdk/classes/component.py
--rw-r--r--   0        0        0      931 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/classes/interval_file.py
--rw-r--r--   0        0        0    57515 2023-03-01 18:41:20.060651 interval_sdk-1.0.2/src/interval_sdk/classes/io.py
--rw-r--r--   0        0        0     8151 2023-04-07 20:59:44.056525 interval_sdk-1.0.2/src/interval_sdk/classes/io_client.py
--rw-r--r--   0        0        0      348 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/classes/io_error.py
--rw-r--r--   0        0        0    35098 2023-04-07 20:59:44.056525 interval_sdk-1.0.2/src/interval_sdk/classes/io_promise.py
--rw-r--r--   0        0        0     7766 2023-04-07 16:54:29.430443 interval_sdk-1.0.2/src/interval_sdk/classes/isocket.py
--rw-r--r--   0        0        0     1290 2023-04-07 16:54:29.430443 interval_sdk-1.0.2/src/interval_sdk/classes/layout.py
--rw-r--r--   0        0        0     3458 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/classes/logger.py
--rw-r--r--   0        0        0     2993 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/classes/page.py
--rw-r--r--   0        0        0     6040 2023-04-07 16:54:29.430443 interval_sdk-1.0.2/src/interval_sdk/classes/rpc.py
--rw-r--r--   0        0        0     2968 2023-03-27 15:09:45.572798 interval_sdk-1.0.2/src/interval_sdk/classes/transaction_loading_state.py
--rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/components/__init__.py
--rw-r--r--   0        0        0     1704 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/components/grid.py
--rw-r--r--   0        0        0     6090 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/components/table.py
--rw-r--r--   0        0        0      771 2023-04-06 18:28:22.682795 interval_sdk-1.0.2/src/interval_sdk/handlers.py
--rw-r--r--   0        0        0    13565 2023-04-07 16:54:29.430443 interval_sdk-1.0.2/src/interval_sdk/internal_rpc_schema.py
--rw-r--r--   0        0        0    25561 2023-04-07 16:54:29.430443 interval_sdk-1.0.2/src/interval_sdk/io_schema.py
--rw-r--r--   0        0        0    55271 2023-04-07 16:54:29.430443 interval_sdk-1.0.2/src/interval_sdk/main.py
--rw-r--r--   0        0        0       41 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/superjson/__init__.py
--rw-r--r--   0        0        0     1081 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/superjson/main.py
--rw-r--r--   0        0        0     3810 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/superjson/plainer.py
--rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/superjson/tests/__init__.py
--rw-r--r--   0        0        0      188 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/superjson/tests/node-only-types.js
--rw-r--r--   0        0        0      416 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/superjson/tests/round-trip-superjson.js
--rw-r--r--   0        0        0     3385 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/superjson/tests/test_superjson.py
--rw-r--r--   0        0        0     5790 2023-02-09 22:23:52.943201 interval_sdk-1.0.2/src/interval_sdk/superjson/transformer.py
--rw-r--r--   0        0        0     4550 2023-04-07 16:54:29.430443 interval_sdk-1.0.2/src/interval_sdk/types.py
--rw-r--r--   0        0        0     7193 2023-04-07 16:54:29.430443 interval_sdk-1.0.2/src/interval_sdk/util.py
--rw-r--r--   0        0        0     4207 1970-01-01 00:00:00.000000 interval_sdk-1.0.2/setup.py
--rw-r--r--   0        0        0     4051 1970-01-01 00:00:00.000000 interval_sdk-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2968 2023-02-09 22:23:52.939868 interval_sdk-1.0.3/README.md
+-rw-r--r--   0        0        0     1890 2023-04-20 18:41:38.393235 interval_sdk-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      331 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/classes/__init__.py
+-rw-r--r--   0        0        0      422 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/classes/action.py
+-rw-r--r--   0        0        0     7024 2023-04-20 18:40:02.490552 interval_sdk-1.0.3/src/interval_sdk/classes/component.py
+-rw-r--r--   0        0        0      931 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/classes/interval_file.py
+-rw-r--r--   0        0        0    57635 2023-04-20 18:41:38.393235 interval_sdk-1.0.3/src/interval_sdk/classes/io.py
+-rw-r--r--   0        0        0     8151 2023-04-20 18:40:02.490552 interval_sdk-1.0.3/src/interval_sdk/classes/io_client.py
+-rw-r--r--   0        0        0      348 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/classes/io_error.py
+-rw-r--r--   0        0        0    35098 2023-04-20 18:40:02.493885 interval_sdk-1.0.3/src/interval_sdk/classes/io_promise.py
+-rw-r--r--   0        0        0     7891 2023-04-20 18:40:02.493885 interval_sdk-1.0.3/src/interval_sdk/classes/isocket.py
+-rw-r--r--   0        0        0     1290 2023-04-14 17:16:59.713107 interval_sdk-1.0.3/src/interval_sdk/classes/layout.py
+-rw-r--r--   0        0        0     3458 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/classes/logger.py
+-rw-r--r--   0        0        0     2993 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/classes/page.py
+-rw-r--r--   0        0        0     6155 2023-04-20 18:40:02.493885 interval_sdk-1.0.3/src/interval_sdk/classes/rpc.py
+-rw-r--r--   0        0        0     2968 2023-03-27 15:09:45.572798 interval_sdk-1.0.3/src/interval_sdk/classes/transaction_loading_state.py
+-rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/components/__init__.py
+-rw-r--r--   0        0        0     1704 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/components/grid.py
+-rw-r--r--   0        0        0     6090 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/components/table.py
+-rw-r--r--   0        0        0      810 2023-04-20 18:40:02.493885 interval_sdk-1.0.3/src/interval_sdk/handlers.py
+-rw-r--r--   0        0        0    13589 2023-04-20 18:40:02.493885 interval_sdk-1.0.3/src/interval_sdk/internal_rpc_schema.py
+-rw-r--r--   0        0        0    25561 2023-04-17 13:45:05.449358 interval_sdk-1.0.3/src/interval_sdk/io_schema.py
+-rw-r--r--   0        0        0    56972 2023-04-20 18:40:02.493885 interval_sdk-1.0.3/src/interval_sdk/main.py
+-rw-r--r--   0        0        0       41 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/superjson/__init__.py
+-rw-r--r--   0        0        0     1081 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/superjson/main.py
+-rw-r--r--   0        0        0     3810 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/superjson/plainer.py
+-rw-r--r--   0        0        0        0 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/superjson/tests/__init__.py
+-rw-r--r--   0        0        0      188 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/superjson/tests/node-only-types.js
+-rw-r--r--   0        0        0      416 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/superjson/tests/round-trip-superjson.js
+-rw-r--r--   0        0        0     3385 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/superjson/tests/test_superjson.py
+-rw-r--r--   0        0        0     5790 2023-02-09 22:23:52.943201 interval_sdk-1.0.3/src/interval_sdk/superjson/transformer.py
+-rw-r--r--   0        0        0     4550 2023-04-14 17:16:59.716440 interval_sdk-1.0.3/src/interval_sdk/types.py
+-rw-r--r--   0        0        0     7193 2023-04-14 17:16:59.716440 interval_sdk-1.0.3/src/interval_sdk/util.py
+-rw-r--r--   0        0        0     4207 1970-01-01 00:00:00.000000 interval_sdk-1.0.3/setup.py
+-rw-r--r--   0        0        0     4051 1970-01-01 00:00:00.000000 interval_sdk-1.0.3/PKG-INFO
```

### Comparing `interval_sdk-1.0.2/README.md` & `interval_sdk-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.2/pyproject.toml` & `interval_sdk-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "interval-sdk"
-version = "1.0.2"
+version = "1.0.3"
 description = "The frontendless framework for high growth companies. Interval automatically generates apps by inlining the UI in your backend code. It's a faster and more maintainable way to build internal tools, rapid prototypes, and more."
 authors = [
 	"Jacob Mischka <jacob@interval.com>",
 	"Ryan Coppolo <ryan@interval.com>",
 ]
 maintainers = [
 	"Jacob Mischka <jacob@interval.com>",
```

### Comparing `interval_sdk-1.0.2/src/interval_sdk/classes/component.py` & `interval_sdk-1.0.3/src/interval_sdk/classes/component.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.2/src/interval_sdk/classes/interval_file.py` & `interval_sdk-1.0.3/src/interval_sdk/classes/interval_file.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.2/src/interval_sdk/classes/io.py` & `interval_sdk-1.0.3/src/interval_sdk/classes/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -1073,15 +1073,17 @@
             )
 
             async def handle_state_change(
                 state: DisplayTableState,
                 props: DisplayTableProps,
             ) -> DisplayTableProps:
                 if get_data is not None:
-                    fetched = await get_data(TableDataFetcherState(**state.dict()))
+                    fetched = await get_data(
+                        TableDataFetcherState(**state.dict(by_alias=False))
+                    )
                     if isinstance(fetched, list):
                         fetched = FetchedTableData(fetched)
                     elif isinstance(fetched, tuple):
                         fetched = FetchedTableData(*fetched)
 
                     built_columns = columns_builder(data=fetched.data, columns=columns)
                     props.data = [
@@ -1192,15 +1194,17 @@
             )
 
             async def handle_state_change(
                 state: DisplayGridState,
                 props: DisplayGridProps,
             ) -> DisplayGridProps:
                 if get_data is not None:
-                    fetched = await get_data(GridDataFetcherState(**state.dict()))
+                    fetched = await get_data(
+                        GridDataFetcherState(**state.dict(by_alias=False))
+                    )
                     if isinstance(fetched, list):
                         fetched = FetchedGridData(fetched)
                     elif isinstance(fetched, tuple):
                         fetched = FetchedGridData(*fetched)
 
                     props.data = [
                         serialize_grid_item(
```

### Comparing `interval_sdk-1.0.2/src/interval_sdk/classes/io_client.py` & `interval_sdk-1.0.3/src/interval_sdk/classes/io_client.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.2/src/interval_sdk/classes/io_promise.py` & `interval_sdk-1.0.3/src/interval_sdk/classes/io_promise.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.2/src/interval_sdk/classes/isocket.py` & `interval_sdk-1.0.3/src/interval_sdk/classes/isocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,29 +178,32 @@
                     self._logger.print_exception(e)
                 finally:
                     self._out_queue.task_done()
             except Exception as e:
                 self._logger.error("Error getting message from queue?", e)
                 self._logger.print_exception(e)
 
-    async def send(self, data: str) -> None:
+    async def send(self, data: str, *, timeout_factor: Optional[int] = None) -> None:
         if self._ws is None:
             raise NotConnectedError
 
+        if timeout_factor is None:
+            timeout_factor = 1
+
         loop = asyncio.get_running_loop()
 
         id = uuid4()
         fut = loop.create_future()
         message = Message(id=id, data=data, type="MESSAGE")
         self._pending_messages[message.id] = PendingMessage(
             message=message, on_ack_received=fut
         )
         await self._out_queue.put(message)
 
-        await asyncio.wait_for(fut, self._send_timeout)
+        await asyncio.wait_for(fut, self._send_timeout * timeout_factor)
 
     async def _handle_close(self, code: int, reason: str):
         self.is_closed = True
 
         if not self.on_authenticated.done():
             self.on_authenticated.cancel()
```

### Comparing `interval_sdk-1.0.2/src/interval_sdk/classes/layout.py` & `interval_sdk-1.0.3/src/interval_sdk/classes/layout.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.2/src/interval_sdk/classes/logger.py` & `interval_sdk-1.0.3/src/interval_sdk/classes/logger.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.2/src/interval_sdk/classes/page.py` & `interval_sdk-1.0.3/src/interval_sdk/classes/page.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.2/src/interval_sdk/classes/rpc.py` & `interval_sdk-1.0.3/src/interval_sdk/classes/rpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,24 +126,29 @@
         message = DuplexMessage(
             id=parsed.id,
             method_name=method_name,
             data=return_value,
             kind="RESPONSE",
         )
         prepared_response_text = message.json()
-        print(prepared_response_text)
 
         try:
             await self._communicator.send(prepared_response_text)
         except Exception as err:
             self._logger.error("Failed sending response", message, err)
             self._logger.print_exception(err)
             raise err
 
-    async def send(self, method_name: CallerSchemaMethodName, inputs: dict[str, Any]):
+    async def send(
+        self,
+        method_name: CallerSchemaMethodName,
+        inputs: dict[str, Any],
+        *,
+        timeout_factor: Optional[int] = None
+    ):
         id = generate_id()
 
         message = DuplexMessage(
             id=id,
             data=inputs,
             method_name=method_name,
             kind="CALL",
@@ -155,14 +160,17 @@
 
         def handle_exceptions(task: asyncio.Task):
             try:
                 task.result()
             except BaseException as err:
                 self._logger.error("Error sending message", err)
 
-        task = loop.create_task(self._communicator.send(message.json()), name="send")
+        task = loop.create_task(
+            self._communicator.send(message.json(), timeout_factor=timeout_factor),
+            name="send",
+        )
         task.add_done_callback(handle_exceptions)
 
         raw_response_text = await fut
         parsed = parse_obj_as(self._can_call[method_name].returns, raw_response_text)
 
         return parsed
```

### Comparing `interval_sdk-1.0.2/src/interval_sdk/classes/transaction_loading_state.py` & `interval_sdk-1.0.3/src/interval_sdk/classes/transaction_loading_state.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.2/src/interval_sdk/components/grid.py` & `interval_sdk-1.0.3/src/interval_sdk/components/grid.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.2/src/interval_sdk/components/table.py` & `interval_sdk-1.0.3/src/interval_sdk/components/table.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.2/src/interval_sdk/handlers.py` & `interval_sdk-1.0.3/src/interval_sdk/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 IntervalActionHandler: TypeAlias = Union[
     Callable[[], Awaitable[IOFunctionReturnType]],
     Callable[[IO], Awaitable[IOFunctionReturnType]],
     Callable[[IO, ActionContext], Awaitable[IOFunctionReturnType]],
 ]
 
 IntervalPageHandler: TypeAlias = Union[
-    Callable[[], Awaitable[Layout]],
-    Callable[[IO.Display], Awaitable[Layout]],
-    Callable[[IO.Display, PageContext], Awaitable[Layout]],
+    Callable[[], Awaitable[Union[Layout, None]]],
+    Callable[[IO.Display], Awaitable[Union[Layout, None]]],
+    Callable[[IO.Display, PageContext], Awaitable[Union[Layout, None]]],
 ]
 
 IOResponseHandler: TypeAlias = Callable[[IOResponse], Awaitable[None]]
```

### Comparing `interval_sdk-1.0.2/src/interval_sdk/internal_rpc_schema.py` & `interval_sdk-1.0.3/src/interval_sdk/internal_rpc_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,16 +51,16 @@
 class SendIOCallInputs(BaseModel):
     transaction_id: str
     io_call: str
 
 
 class SendPageInputs(BaseModel):
     page_key: str
-    # stringified page
-    page: str
+    # stringified page layout
+    page: Optional[str] = None
 
 
 class LeavePageInputs(BaseModel):
     page_key: str
 
 
 class SendLoadingCallInputs(LoadingState):
```

### Comparing `interval_sdk-1.0.2/src/interval_sdk/io_schema.py` & `interval_sdk-1.0.3/src/interval_sdk/io_schema.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.2/src/interval_sdk/main.py` & `interval_sdk-1.0.3/src/interval_sdk/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,14 +134,16 @@
 
     _logger: Logger
     _endpoint: str = "wss://interval.com/websocket"
     _http_endpoint: str
     _api_key: str
 
     _retry_interval_seconds: float = 3
+    _max_resend_attempts: int = 10
+    _send_timeout_seconds: float = 5
     _ping_timeout_seconds: float = 5
     _ping_interval_seconds: float = 30
     _close_unresponsive_connection_timeout_seconds: float = 180
     _reinitialize_batch_timeout_seconds: float = 0.2
     _num_isocket_producers: int
 
     _io_clients: dict[str, IOClient]
@@ -174,14 +176,16 @@
     def __init__(
         self,
         api_key: str,
         *,
         endpoint: Optional[str] = None,
         log_level: LogLevel = "info",
         retry_interval: float = 3,
+        max_resend_attempts: int = 10,
+        send_timeout: float = 5,
         ping_timeout: float = 5,
         ping_interval: float = 30,
         close_unresponsive_connection_timeout: float = 180,
         reinitialize_batch_timeout: float = 0.2,
         num_message_producers: int = 1,
     ):
         self._api_key = api_key
@@ -190,14 +194,16 @@
 
         url = urlparse(self._endpoint)
         self._http_endpoint = urlunparse(
             url._replace(scheme=url.scheme.replace("ws", "http"), path="/api")
         )
 
         self._retry_interval_seconds = retry_interval
+        self._max_resend_attempts = max_resend_attempts
+        self._send_timeout_seconds = send_timeout
         self._ping_timeout_seconds = ping_timeout
         self._ping_interval_seconds = ping_interval
         self._close_unresponsive_connection_timeout_seconds = (
             close_unresponsive_connection_timeout
         )
         self._reinitialize_batch_timeout_seconds = reinitialize_batch_timeout
         self._num_isocket_producers = num_message_producers
@@ -366,24 +372,35 @@
         self,
         method_name: WSServerSchemaMethodName,
         inputs: dict[str, Any],
     ):
         if self._server_rpc is None:
             raise NotInitializedError("server_rpc not initialized")
 
-        while True:
+        for attempt_index in range(self._max_resend_attempts):
+            attempt_number = attempt_index + 1
+            sleep_time_before_retrying = self._retry_interval_seconds * attempt_number
             if self._is_connected:
                 try:
-                    return await self._server_rpc.send(method_name, inputs)
+                    return await self._server_rpc.send(
+                        method_name, inputs, timeout_factor=attempt_number
+                    )
                 except Exception as err:
-                    self._log.debug("RPC call timed out, retrying in 3s...", err)
+                    self._log.debug(
+                        f"RPC call timed out, retrying in {sleep_time_before_retrying}s...",
+                        err,
+                    )
             else:
-                self._log.debug("Not connected, retrying again in 3s...")
+                self._log.debug(
+                    f"Not connected, retrying again in {sleep_time_before_retrying}s..."
+                )
 
-            await asyncio.sleep(self._retry_interval_seconds)
+            await asyncio.sleep(sleep_time_before_retrying)
+
+        raise IntervalError("Maximum failed resend attempts reached, aborting.")
 
     async def _send_log(self, transaction_id: str, index: int, *args):
         if len(args) == 0:
             return
 
         data = " ".join([str(arg) for arg in args])
         if len(data) > 10000:
@@ -526,15 +543,16 @@
             to_resend: dict[str, str] = {}
             for id in ids_to_resend:
                 try:
                     to_resend[id] = self._pending_io_calls[id]
                 except KeyError:
                     pass
 
-        while len(to_resend) > 0:
+        attempt_number = 0
+        while len(to_resend) > 0 and attempt_number <= self._max_resend_attempts:
             items = list(to_resend.items())
             responses = await asyncio.gather(
                 *(
                     self._send(
                         "SEND_IO_CALL",
                         SendIOCallInputs(
                             transaction_id=transaction_id,
@@ -569,19 +587,20 @@
                     if not response:
                         # Unsuccessful, don't retry again
                         try:
                             del self._pending_io_calls[transaction_id]
                         except KeyError:
                             pass
 
-            if len(to_resend) > 0:
-                self._logger.debug(
-                    f"Trying again in {self._retry_interval_seconds}s..."
-                )
-                await asyncio.sleep(self._retry_interval_seconds)
+            attempt_number += 1
+
+            if len(to_resend) > 0 and attempt_number <= self._max_resend_attempts:
+                retry_sleep_seconds = self._retry_interval_seconds * attempt_number
+                self._logger.debug(f"Trying again in {retry_sleep_seconds}s...")
+                await asyncio.sleep(retry_sleep_seconds)
 
     async def _resend_pending_page_layouts(
         self, page_keys_to_resend: Optional[list[str]] = None
     ):
         if not self._is_connected:
             return
 
@@ -591,15 +610,16 @@
             to_resend: dict[str, str] = {}
             for id in page_keys_to_resend:
                 try:
                     to_resend[id] = self._pending_page_layouts[id]
                 except KeyError:
                     pass
 
-        while len(to_resend) > 0:
+        attempt_number = 1
+        while len(to_resend) > 0 and attempt_number <= self._max_resend_attempts:
             items = list(to_resend.items())
             responses = await asyncio.gather(
                 *(
                     self._send(
                         "SEND_PAGE",
                         SendPageInputs(
                             page_key=page_key,
@@ -634,19 +654,20 @@
                     if not response:
                         # Unsuccessful, don't retry again
                         try:
                             del self._pending_page_layouts[page_key]
                         except KeyError:
                             pass
 
-            if len(to_resend) > 0:
-                self._logger.debug(
-                    f"Trying again in {self._retry_interval_seconds}s..."
-                )
-                await asyncio.sleep(self._retry_interval_seconds)
+            attempt_number += 1
+
+            if len(to_resend) > 0 and attempt_number <= self._max_resend_attempts:
+                retry_sleep_seconds = self._retry_interval_seconds * attempt_number
+                self._logger.debug(f"Trying again in {retry_sleep_seconds}s...")
+                await asyncio.sleep(retry_sleep_seconds)
 
     async def _resend_transaction_loading_states(
         self, ids_to_resend: Optional[list[str]] = None
     ):
         if not self._is_connected:
             return
 
@@ -656,15 +677,16 @@
             to_resend: dict[str, LoadingState] = {}
             for id in ids_to_resend:
                 try:
                     to_resend[id] = self._transaction_loading_states[id]
                 except KeyError:
                     pass
 
-        while len(to_resend) > 0:
+        attempt_number = 1
+        while len(to_resend) > 0 and attempt_number <= self._retry_interval_seconds:
             items = list(to_resend.items())
             responses = await asyncio.gather(
                 (
                     self._send(
                         "SEND_LOADING_CALL",
                         SendLoadingCallInputs(
                             transaction_id=transaction_id,
@@ -705,19 +727,20 @@
                     if not response:
                         # Unsuccessful, don't retry again
                         try:
                             del self._transaction_loading_states[transaction_id]
                         except KeyError:
                             pass
 
-            if len(to_resend) > 0:
-                self._logger.debug(
-                    f"Trying again in {self._retry_interval_seconds}s..."
-                )
-                await asyncio.sleep(self._retry_interval_seconds)
+            attempt_number += 1
+
+            if len(to_resend) > 0 and attempt_number <= self._max_resend_attempts:
+                retry_sleep_seconds = self._retry_interval_seconds * attempt_number
+                self._logger.debug(f"Trying again in {retry_sleep_seconds}s...")
+                await asyncio.sleep(retry_sleep_seconds)
 
     def _close_transaction(self, transaction_id: str):
         self._logger.debug("Closing transaction", transaction_id)
         try:
             del self._pending_io_calls[transaction_id]
         except KeyError:
             pass
@@ -795,14 +818,15 @@
 
         self._isocket = ISocket(
             id=instance_id,
             ws=ws,
             on_close=on_close,
             log_level=self._logger.log_level,
             num_producers=self._num_isocket_producers,
+            send_timeout=self._send_timeout_seconds,
         )
 
         await self._isocket.connect()
         self._is_connected = True
 
         if self._server_rpc is None:
             return
@@ -1033,14 +1057,15 @@
                 try:
                     task.result()
                     send_page_task = None
                 except BaseException as e:
                     self._logger.error(e)
 
             async def send_page():
+                page_layout = None
                 if page is not None:
                     page_layout = BasicLayoutModel(
                         kind="BASIC",
                         errors=errors,
                     )
 
                     if page.title is not None:
@@ -1057,39 +1082,40 @@
 
                     if render_instruction is not None:
                         page_layout.children = render_instruction
 
                     if menu_items is not None:
                         page_layout.menu_items = menu_items
 
-                    for _ in range(MAX_PAGE_RETRIES):
-                        try:
-                            serialized_page = page_layout.json(
-                                exclude_unset=True,
-                            )
+                for _ in range(MAX_PAGE_RETRIES):
+                    try:
+                        serialized_page = (
+                            page_layout.json(exclude_unset=True, by_alias=True)
+                            if page_layout is not None
+                            else None
+                        )
+                        if serialized_page is not None:
                             self._pending_page_layouts[
                                 inputs.page_key
                             ] = serialized_page
-                            await self._send(
-                                "SEND_PAGE",
-                                SendPageInputs(
-                                    page_key=inputs.page_key,
-                                    page=serialized_page,
-                                ).dict(),
-                            )
-                            return
-                        except Exception as err:
-                            self._logger.debug("Failed sending page", err)
-                            self._logger.debug(
-                                "Retrying in", self._retry_interval_seconds, "seconds"
-                            )
-                            await asyncio.sleep(self._retry_interval_seconds)
-                    raise IntervalError(
-                        "Unsuccessful sending page, max retries exceeded."
-                    )
+                        await self._send(
+                            "SEND_PAGE",
+                            SendPageInputs(
+                                page_key=inputs.page_key,
+                                page=serialized_page,
+                            ).dict(),
+                        )
+                        return
+                    except Exception as err:
+                        self._logger.debug("Failed sending page", err)
+                        self._logger.debug(
+                            "Retrying in", self._retry_interval_seconds, "seconds"
+                        )
+                        await asyncio.sleep(self._retry_interval_seconds)
+                raise IntervalError("Unsuccessful sending page, max retries exceeded.")
 
             async def handle_send(instruction: IORender):
                 nonlocal render_instruction
                 render_instruction = instruction
                 if send_page_task is None:
                     await send_page()
 
@@ -1125,14 +1151,20 @@
                     else:
                         raise IntervalError(
                             "handler accepts invalid number of arguments"
                         )
 
                     page = resp
 
+                    if page is None:
+                        if send_page_task is None:
+                            send_page_task = loop.create_task(send_page())
+                            send_page_task.add_done_callback(on_page_sent)
+                        return
+
                     if page.title is not None:
                         if isfunction(page.title):
                             try:
                                 page.title = page.title()
                             except Exception as err:
                                 self._logger.error(err)
                                 errors.append(page_error(err, "title"))
```

### Comparing `interval_sdk-1.0.2/src/interval_sdk/superjson/main.py` & `interval_sdk-1.0.3/src/interval_sdk/superjson/main.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.2/src/interval_sdk/superjson/plainer.py` & `interval_sdk-1.0.3/src/interval_sdk/superjson/plainer.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.2/src/interval_sdk/superjson/tests/test_superjson.py` & `interval_sdk-1.0.3/src/interval_sdk/superjson/tests/test_superjson.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.2/src/interval_sdk/superjson/transformer.py` & `interval_sdk-1.0.3/src/interval_sdk/superjson/transformer.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.2/src/interval_sdk/types.py` & `interval_sdk-1.0.3/src/interval_sdk/types.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.2/src/interval_sdk/util.py` & `interval_sdk-1.0.3/src/interval_sdk/util.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.0.2/setup.py` & `interval_sdk-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ['aiohttp>=3.8.1,<4.0.0',
  'pydantic>=1.9.0,<2.0.0',
  'typing-extensions>=4.4.0,<5.0.0',
  'websockets>=10.1,<11.0']
 
 setup_kwargs = {
     'name': 'interval-sdk',
-    'version': '1.0.2',
+    'version': '1.0.3',
     'description': "The frontendless framework for high growth companies. Interval automatically generates apps by inlining the UI in your backend code. It's a faster and more maintainable way to build internal tools, rapid prototypes, and more.",
     'long_description': '# interval-sdk\n\n## Installation\n\nInstall using pip, (or your python package manager of choice):\n\n```\npip install interval-sdk\n```\n\n## API\n\n*Note:* Proper documentation is in progress!\n\nSee `src/demos/basic.py` and `src/tests` for a better overview, but in short:\n\n```python\nfrom interval_sdk import Interval, IO\n\n# Initialize Interval\ninterval = Interval("API_KEY")\n\n# Add an action using the function name as the slug\n@interval.action\nasync def hello_interval():\n    return {"hello": "from python!"}\n\n# Add an action using a custom slug (can contain hyphens) and additional configuration\n@interval.action(slug=\'echo-message\', unlisted=True)\nasync def echo_message(io: IO):\n    [message] = await io.group(io.input.text("Hello!", help_text="From python!"))\n\n    return {"message": message}\n\n\n# Synchronously listen, blocking forever\ninterval.listen()\n```\n\nTo not block, interval can also be run asynchronously using\n`interval.listen_async()`. You must provide your own event loop.\n\nThe task will complete as soon as connection to Interval completes, so you\nlikely want to run forever or run alongside another permanent task.\n\n```python\nimport asyncio\n\n# This is what synchronous `listen()` does under the hood\nloop = asyncio.get_event_loop()\ntask = loop.create_task(interval.listen_async())\ndef handle_done(task: asyncio.Task[None]):\n    try:\n        task.result()\n    except:\n        loop.stop()\n\ntask.add_done_callback(handle_done)\nloop.run_forever()\n```\n\nIf you are using `run_forever()`, you\'ll probably want to add signal handlers\nto close the loop gracefully on process termination:\n\n```python\nimport asyncio, signal\n\nloop = asyncio.get_event_loop()\ntask = loop.create_task(interval.listen_async())\ndef handle_done(task: asyncio.Task[None]):\n    try:\n        task.result()\n    except:\n        loop.stop()\n\ntask.add_done_callback(handle_done)\nfor sig in {signal.SIGINT, signal.SIGTERM}:\n    loop.add_signal_handler(sig, loop.stop)\nloop.run_forever()\n```\n\n\n## Contributing\n\nThis project uses [Poetry](https://python-poetry.org/) for dependency\nmanagement\n\n1. `poetry install` to install dependencies\n2. `poetry shell` to activate the virtual environment\n\nTasks are configured using [poethepoet](https://github.com/nat-n/poethepoet)\n(installed as a dev dependency).\n\n- `poe demo [demo_name]` to run a demo (`basic` by default if `demo_name` omitted)\n- `poe test` to run `pytest` (can also run `pytest` directly in virtual env)\n\nCode is formatted using [Black](https://github.com/psf/black). Please configure\nyour editor to format on save using Black, or run `poe format` to format the\ncode before committing changes.\n\n## Tests\n\n*Note:* Tests currently require a local instance of the Interval backend.\n\nTests use [pytest](https://docs.pytest.org/en/7.1.x/) and\n[playwright](https://playwright.dev/python/).\n\nCurrently assumes the `test-runner@interval.com` user exists already.\nRun `yarn test` in the `web` directory at least once to create it before\nrunning these.\n',
     'author': 'Jacob Mischka',
     'author_email': 'jacob@interval.com',
     'maintainer': 'Jacob Mischka',
     'maintainer_email': 'jacob@interval.com',
     'url': 'https://interval.com',
```

### Comparing `interval_sdk-1.0.2/PKG-INFO` & `interval_sdk-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interval-sdk
-Version: 1.0.2
+Version: 1.0.3
 Summary: The frontendless framework for high growth companies. Interval automatically generates apps by inlining the UI in your backend code. It's a faster and more maintainable way to build internal tools, rapid prototypes, and more.
 Home-page: https://interval.com
 Keywords: internal tool,app,ui,ui builder
 Author: Jacob Mischka
 Author-email: jacob@interval.com
 Maintainer: Jacob Mischka
 Maintainer-email: jacob@interval.com
```

