# Comparing `tmp/socket_proxy-4.0.1-py3-none-any.whl.zip` & `tmp/socket_proxy-5.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,21 @@
-Zip file size: 33658 bytes, number of entries: 20
--rw-r--r--  2.0 unx      221 b- defN 22-Oct-27 15:59 socket_proxy/__init__.py
--rw-r--r--  2.0 unx    14221 b- defN 23-Jan-10 11:07 socket_proxy/__main__.py
--rw-r--r--  2.0 unx     3257 b- defN 23-Feb-25 11:55 socket_proxy/api.py
--rw-r--r--  2.0 unx     3036 b- defN 23-Jan-10 11:07 socket_proxy/base.py
--rw-rw-r--  2.0 unx     3277 b- defN 21-Apr-24 12:38 socket_proxy/config.py
--rw-r--r--  2.0 unx     2392 b- defN 22-Dec-01 18:01 socket_proxy/connection.py
--rw-rw-r--  2.0 unx    10869 b- defN 21-Apr-24 12:38 socket_proxy/main.py
--rw-r--r--  2.0 unx    12017 b- defN 23-Jan-10 11:07 socket_proxy/package.py
--rw-r--r--  2.0 unx    11053 b- defN 23-Jan-10 11:07 socket_proxy/proxy.py
--rw-r--r--  2.0 unx     6616 b- defN 22-Oct-28 20:56 socket_proxy/tunnel.py
--rw-r--r--  2.0 unx     7423 b- defN 23-Jan-10 11:07 socket_proxy/tunnel_client.py
--rw-r--r--  2.0 unx     4518 b- defN 22-Oct-28 20:25 socket_proxy/tunnel_gui.py
--rw-r--r--  2.0 unx     7314 b- defN 22-Dec-01 18:45 socket_proxy/tunnel_server.py
--rw-r--r--  2.0 unx    11024 b- defN 23-Jan-10 11:07 socket_proxy/utils.py
--rw-rw-r--  2.0 unx     1085 b- defN 23-Feb-25 11:58 socket_proxy-4.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3621 b- defN 23-Feb-25 11:58 socket_proxy-4.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-25 11:58 socket_proxy-4.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       60 b- defN 23-Feb-25 11:58 socket_proxy-4.0.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-Feb-25 11:58 socket_proxy-4.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1639 b- defN 23-Feb-25 11:58 socket_proxy-4.0.1.dist-info/RECORD
-20 files, 103748 bytes uncompressed, 31006 bytes compressed:  70.1%
+Zip file size: 30977 bytes, number of entries: 19
+-rw-r--r--  2.0 unx      240 b- defN 23-Apr-20 16:54 socket_proxy/__init__.py
+-rw-r--r--  2.0 unx    14803 b- defN 23-Apr-20 16:54 socket_proxy/__main__.py
+-rw-r--r--  2.0 unx     3314 b- defN 23-Apr-20 16:54 socket_proxy/api.py
+-rw-r--r--  2.0 unx     3096 b- defN 23-Apr-20 16:54 socket_proxy/base.py
+-rw-r--r--  2.0 unx     2392 b- defN 23-Apr-20 16:54 socket_proxy/connection.py
+-rw-r--r--  2.0 unx     2083 b- defN 23-Apr-20 16:54 socket_proxy/event.py
+-rw-r--r--  2.0 unx    12017 b- defN 23-Apr-20 16:54 socket_proxy/package.py
+-rw-r--r--  2.0 unx    11836 b- defN 23-Apr-20 16:54 socket_proxy/proxy.py
+-rw-r--r--  2.0 unx     6616 b- defN 23-Apr-20 16:54 socket_proxy/tunnel.py
+-rw-r--r--  2.0 unx     7307 b- defN 23-Apr-20 16:54 socket_proxy/tunnel_client.py
+-rw-r--r--  2.0 unx     4543 b- defN 23-Apr-20 16:54 socket_proxy/tunnel_gui.py
+-rw-r--r--  2.0 unx     7937 b- defN 23-Apr-20 16:54 socket_proxy/tunnel_server.py
+-rw-r--r--  2.0 unx    11183 b- defN 23-Apr-20 16:54 socket_proxy/utils.py
+-rw-r--r--  2.0 unx     1085 b- defN 23-Apr-20 16:55 socket_proxy-5.0.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3933 b- defN 23-Apr-20 16:55 socket_proxy-5.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 16:55 socket_proxy-5.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       60 b- defN 23-Apr-20 16:55 socket_proxy-5.0.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Apr-20 16:55 socket_proxy-5.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1560 b- defN 23-Apr-20 16:55 socket_proxy-5.0.0.dist-info/RECORD
+19 files, 94110 bytes uncompressed, 28443 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -6,21 +6,18 @@
 
 Filename: socket_proxy/api.py
 Comment: 
 
 Filename: socket_proxy/base.py
 Comment: 
 
-Filename: socket_proxy/config.py
-Comment: 
-
 Filename: socket_proxy/connection.py
 Comment: 
 
-Filename: socket_proxy/main.py
+Filename: socket_proxy/event.py
 Comment: 
 
 Filename: socket_proxy/package.py
 Comment: 
 
 Filename: socket_proxy/proxy.py
 Comment: 
@@ -36,26 +33,26 @@
 
 Filename: socket_proxy/tunnel_server.py
 Comment: 
 
 Filename: socket_proxy/utils.py
 Comment: 
 
-Filename: socket_proxy-4.0.1.dist-info/LICENSE
+Filename: socket_proxy-5.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: socket_proxy-4.0.1.dist-info/METADATA
+Filename: socket_proxy-5.0.0.dist-info/METADATA
 Comment: 
 
-Filename: socket_proxy-4.0.1.dist-info/WHEEL
+Filename: socket_proxy-5.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: socket_proxy-4.0.1.dist-info/entry_points.txt
+Filename: socket_proxy-5.0.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: socket_proxy-4.0.1.dist-info/top_level.txt
+Filename: socket_proxy-5.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: socket_proxy-4.0.1.dist-info/RECORD
+Filename: socket_proxy-5.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## socket_proxy/__init__.py

```diff
@@ -1,7 +1,9 @@
 from .base import config
 from .connection import Connection
 from .package import *
 from .proxy import ProxyServer
 from .tunnel import Tunnel
 from .tunnel_client import TunnelClient
 from .tunnel_server import TunnelServer
+
+VERSION = "5.0.0"
```

## socket_proxy/__main__.py

```diff
@@ -2,15 +2,15 @@
 import argparse
 import logging
 import os
 import sys
 from configparser import ConfigParser
 from typing import Tuple
 
-from . import api, base, utils
+from . import api, base, event, utils
 from .proxy import ProxyServer
 from .tunnel_client import TunnelClient
 from .tunnel_gui import GUIClient
 
 _logger = logging.getLogger(__name__)
 
 
@@ -254,14 +254,34 @@
         "--log-level",
         choices=sorted(base.LOG_LEVELS),
         default=base.DEFAULT_LOG_LEVEL,
         help="Set the log level to use. (default: %(default)s)",
     )
 
 
+def event_group(parser: argparse.ArgumentParser) -> None:
+    if not event.ClientSession:
+        return
+
+    group = parser.add_argument_group(
+        "Events and Hooks",
+        "Configure the event system and the hooks",
+    )
+    group.add_argument(
+        "--hook-url",
+        default=None,
+        help="Send events via an HTTP web hook as JSON data",
+    )
+    group.add_argument(
+        "--hook-token",
+        default=None,
+        help="Authentication token for the web hook. Uses bearer authentication",
+    )
+
+
 def option_group(parser: argparse.ArgumentParser, server: bool) -> None:
     group = parser.add_argument_group(
         "Additional options",
         "If the tunnel server and client set the options the minimal value will be "
         "used.",
     )
     group.add_argument(
@@ -356,25 +376,27 @@
         "client",
         formatter_class=CustomHelpFormatter,
         help="Enter client mode connect to a server building the tunnel.",
     )
     basic_group(client)
     security_group(client, False)
     connection_group(client, False)
+    event_group(client)
     option_group(client, False)
     logging_group(client)
 
     server = sub.add_parser(
         "server",
         formatter_class=CustomHelpFormatter,
         help="Enter server mode and listen for incoming clients to build the tunnels.",
     )
     basic_group(server, True)
     security_group(server, True)
     connection_group(server, True)
+    event_group(server)
     option_group(server, True)
     logging_group(server)
 
     parsed = parser.parse_args(args)
     if not getattr(parsed, "config", None) or not parsed.mode:
         return parsed
```

## socket_proxy/api.py

```diff
@@ -15,14 +15,16 @@
 
 class APIType(enum.IntEnum):
     Client = 0x01
     Server = 0x02
 
 
 class APIMixin:
+    """Mixin to define the basic API implementations"""
+
     def __init__(self, api_type: APIType):
         self.api_type = api_type
         self.api = self.api_ssl = None
         self.api_host = self.api_port = self.api_token = False
 
         if web is None:
             return
```

## socket_proxy/base.py

```diff
@@ -4,14 +4,15 @@
 import logging
 import os
 from typing import TypeVar, Union
 
 _logger = logging.getLogger(__name__)
 
 CLIENT_NAME_SIZE = 8
+EVENT_TIMEOUT = 0.5
 INTERVAL_TIME = 1
 DEFAULT_PORT = 2773
 DEFAULT_API_PORT = 7773
 DEFAULT_HTTP_PORT = 8773
 DEFAULT_LOG_LEVEL = "info"
 LOG_FORMAT = "{asctime} [{levelname:^8}] {message}"
 
@@ -105,14 +106,16 @@
     cipher=None,
     crl=None,
     connect=None,
     dst=None,
     http_domain=None,
     http_listen=("", DEFAULT_HTTP_PORT),
     http_ssl=False,
+    hook_token=None,
+    hook_url=None,
     idle_timeout=0,
     key=None,
     listen=("", DEFAULT_PORT),
     log_file=None,
     log_level=DEFAULT_LOG_LEVEL,
     max_clients=0,
     max_connects=0,
```

## socket_proxy/proxy.py

```diff
@@ -3,15 +3,15 @@
 import logging
 import re
 import uuid
 from asyncio import StreamReader, StreamWriter
 from datetime import datetime, timedelta
 from typing import Any, List, Tuple, Union
 
-from . import api, base, package, utils
+from . import api, base, event, package, utils
 from .tunnel_server import TunnelServer
 
 _logger = logging.getLogger(__name__)
 
 HTTPRequestStatus = re.compile(rb"^(\S+)\s+(\S+)\s+(\S+)$")
 
 
@@ -45,14 +45,19 @@
             crl=crl,
             server=True,
         )
         self.http_proxy = self.server = None
 
         self.authentication = authentication
         self.auth_timeout = auth_timeout
+        self.event = event.EventSystem(
+            event.EventType.Server,
+            url=base.config.hook_url,
+            token=base.config.hook_token,
+        )
 
         if isinstance(base.config.http_domain, str) and base.config.http_listen:
             self.http_host, self.http_port = base.config.http_listen
             self.http_domain = base.config.http_domain
             self.http_domain_regex = re.compile(
                 rb"^(.*)\.%s$" % self.http_domain.replace(".", r"\.").encode()
             )
@@ -99,33 +104,38 @@
         """This methods will get called regularly to apply timeouts"""
         dt = datetime.now() - timedelta(seconds=self.auth_timeout)
         changes = False
         for token, t in list(self.tokens.items()):
             if t and token and t < dt:
                 self.tokens.pop(token, None)
                 changes = True
-                _logger.info("Invalidated token %s", token)
+                _logger.info(f"Invalidated token {token}")
+                await self.event.send(msg="token_invalidate", token=token)
 
         if self.authentication and not self.tokens:
             self.generate_token()
         elif changes:
             self._persist_state()
 
+        # Flush the event queue
+        await self.event.flush()
+
     def generate_token(self, hotp: bool = False) -> str:
         """Generate a new authentication token"""
         if not self.authentication:
             return None
 
         token = str(uuid.uuid4())
         self.tokens[token] = None if hotp else datetime.now()
         _logger.info(
             "Generated authentication token %s [%s]",
             token,
             "hotp" if hotp else "totp",
         )
+        self.event.send_nowait(msg="token_generate", token=token, hotp=bool(hotp))
         self._persist_state()
         return token
 
     async def _api_handle(self, path: Tuple[str], request: api.Request) -> Any:
         """Handle api functions"""
         if ("token", "hotp") == path[:2]:
             return self.generate_token(True)
@@ -150,31 +160,39 @@
 
         # Limit the number of tunnels
         if 0 < self.max_tunnels <= len(self.tunnels):
             await self.close(reader, writer)
             return
 
         # Create the tunnel object and generate an unique token
-        tunnel = TunnelServer(reader, writer, domain=self.http_domain, **self.kwargs)
+        tunnel = TunnelServer(
+            reader,
+            writer,
+            event=self.event,
+            domain=self.http_domain,
+            **self.kwargs,
+        )
 
         if self.authentication:
             # Expect the token as first package
             pkg = await tunnel.tunnel.tun_read()
             if not isinstance(pkg, package.AuthPackage):
                 await self.close(reader, writer)
                 return
 
             if not self._verify_auth_token(pkg):
                 await self.close(reader, writer)
                 return
 
         self.tunnels[tunnel.uuid] = tunnel
+        await self.event.send(msg="tunnel_connect", tunnel=tunnel.uuid)
         try:
             await tunnel.loop()
         finally:
+            await self.event.send(msg="tunnel_disconnect", tunnel=tunnel.uuid)
             self.tunnels.pop(tunnel.uuid)
 
     async def _request(self, reader: StreamReader, writer: StreamWriter) -> None:
         """Handle http requests and try to proxy them to the specific tunnel"""
         buf = await reader.readline()
         status = buf.strip()
         match = HTTPRequestStatus.match(status)
@@ -224,15 +242,15 @@
             await writer.drain()
             await self.close(reader, writer)
 
     async def http_loop(self) -> None:
         """Main server loop for the http socket"""
         host = self.http_host
         for h in host if isinstance(host, list) else [host]:
-            _logger.info("Serving on %s:%s [HTTP]", h, self.http_port)
+            _logger.info(f"Serving on {h}:{self.http_port} [HTTP]")
 
         self.http_proxy = await asyncio.start_server(
             self._request,
             self.http_host,
             self.http_port,
             ssl=self.sc if self.http_ssl else None,
         )
@@ -240,29 +258,33 @@
         async with self.http_proxy:
             await self.http_proxy.serve_forever()
 
     async def loop(self) -> None:
         """Main server loop to wait for tunnels to open"""
         if self.http_domain_regex:
             asyncio.create_task(self.http_loop())
+            await self.event.send(msg="http_start")
 
         if self.api_port:
             asyncio.create_task(self.start_api())
+            await self.event.send(msg="api_start")
 
         asyncio.create_task(self._interval())
 
         self.server = await asyncio.start_server(
             self._accept,
             self.host,
             self.port,
             ssl=self.sc,
         )
 
         for host in self.host if isinstance(self.host, list) else [self.host]:
-            _logger.info("Serving on %s:%s", host, self.port)
+            _logger.info(f"Serving on {host}:{self.port}")
+
+        await self.event.send(msg="proxy_start")
 
         async with self.server:
             await self.server.serve_forever()
 
     def get_state_dict(self) -> dict:
         """Generate a dictionary which shows the current state of the server"""
         tunnels = {}
```

## socket_proxy/tunnel_client.py

```diff
@@ -44,17 +44,14 @@
 
     def info(self, msg: str, *args) -> None:
         _logger.info(msg.capitalize(), *args)
 
     def error(self, msg: str, *args) -> None:
         _logger.error(msg.capitalize(), *args)
 
-    def fmt_port(self, ip_type, ip, port):
-        return f"{'' if ip.is_unspecified else ip}:{port} [{ip_type.name}]"
-
     async def idle(self) -> None:
         await super().idle()
 
         if not self.ping_enabled:
             return
 
         # Break the connection if the last ping took too long
@@ -131,15 +128,15 @@
             self.tunnel.token = pkg.token
             self.addr = pkg.addresses
             self.domain = pkg.domain
 
             # Output the public addresses
             addr = [(base.InternetType.from_ip(ip), ip, port) for ip, port in self.addr]
             for a in sorted(addr):
-                self.info(f"open on {self.fmt_port(*a)}")
+                self.info(f"open on {utils.format_port(*a)}")
 
             if self.protocol == base.ProtocolType.HTTP:
                 self.info(f"domain: {self.domain}")
 
             # Send the configuration to the server for negotiation
             await self._send_config()
             return True
```

## socket_proxy/tunnel_gui.py

```diff
@@ -111,15 +111,15 @@
         self.logs = self.logs[-h - 2 :]
 
         self._draw_lines(win, self.logs)
 
         win.refresh()
         return win
 
-    def _draw_lines(self, win, lines: List[str]) -> None:
+    def _draw_lines(self, win, lines: List[str]) -> None:  # pylint: disable=R0201
         """Draw multiple lines in a window with some border"""
         h, w = [k - 2 for k in win.getmaxyx()]
         for y, line in enumerate(lines[:h]):
             win.addstr(y + 1, 2, line[:w])
 
     async def _handle(self) -> bool:
         """Handle the drawing after each package"""
```

## socket_proxy/tunnel_server.py

```diff
@@ -4,26 +4,28 @@
 import logging
 from asyncio import StreamReader, StreamWriter
 from datetime import datetime, timedelta
 from typing import List, Tuple
 
 from . import base, package, tunnel, utils
 from .connection import Connection
+from .event import EventSystem
 
 _logger = logging.getLogger(__name__)
 
 
 class TunnelServer(tunnel.Tunnel):
     """Server side of the tunnel to listen for external connections"""
 
     def __init__(
         self,
         reader: StreamReader,
         writer: StreamWriter,
         *,
+        event: EventSystem,
         domain: str = "",
         tunnel_host: str = None,
         ports: Tuple[int, int] = None,
         protocols: List[base.ProtocolType] = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
@@ -32,14 +34,15 @@
         self.host, self.port = writer.get_extra_info("peername")[:2]
         self.tunnel_host = tunnel_host.split(",") if tunnel_host else ""
         self.tunnel_port = None
         self.ports = ports
         self.server = None
         self.connections = collections.defaultdict(utils.Ban)
         self.protocols = protocols or utils.protocols()
+        self.event = event
 
     def block(self, ip: base.IPvXAddress) -> bool:
         """Decide whether the ip should be blocked"""
         if 0 < self.max_connects <= self.connections[ip].hits:
             return True
 
         if self.networks and not any(ip in n for n in self.networks):
@@ -70,23 +73,29 @@
         # Block connections using the networks
         if self.block(ip):
             reader.feed_eof()
             writer.close()
             await writer.wait_closed()
 
             _logger.info("Connection from %s blocked", ip)
+            await self.event.send(msg="client_blocked", tunnel=self.uuid, ip=str(ip))
             return
 
         self.connections[ip].hits += 1
 
         # Create the client object and generate an unique token
         client = Connection(reader, writer, self.protocol, utils.generate_token())
         self.add(client)
 
         _logger.info("Client %s connected on %s:%s", client.uuid, host, port)
+        await self.event.send(
+            msg="client_connect",
+            tunnel=self.uuid,
+            client=client.uuid,
+        )
 
         # Inform the tunnel about the new client
         pkg = package.ClientInitPackage(ip, port, client.token)
         await self.tunnel.tun_write(pkg)
 
         # Send the buffer read ahead of initialization through the tunnel
         if read_ahead:
@@ -103,14 +112,23 @@
 
         if self.server and self.server.is_serving():
             pkg = package.ClientClosePackage(client.token)
             await self.tunnel.tun_write(pkg)
 
         await self._disconnect_client(client.token)
 
+    async def _disconnect_client(self, token: bytes) -> None:
+        """Disconnect a client and generate an event"""
+        await self.event.send(
+            msg="client_disconnect",
+            tunnel=self.uuid,
+            client=token.hex(),
+        )
+        return await super()._disconnect_client(token)
+
     async def _open_server(self) -> bool:
         """Open the public server listener and start the main loop"""
 
         # Start to listen on an external port
         self.tunnel_port = utils.get_unused_port(*self.ports) if self.ports else 0
         if self.tunnel_port is None:
             self.error("All ports are blocked")
```

## socket_proxy/utils.py

```diff
@@ -88,14 +88,18 @@
     if log_file:
         handler = logging.FileHandler(log_file)
         handler.setLevel(logging.DEBUG)
         handler.setFormatter(logging.Formatter(base.LOG_FORMAT, style="{"))
         log.addHandler(handler)
 
 
+def format_port(ip_type: base.InternetType, ip: base.IPvXAddress, port: int) -> str:
+    return f"{'' if ip.is_unspecified else ip}:{port} [{ip_type.name}]"
+
+
 def format_transfer(b: int) -> str:
     """Format a number of bytes in a more human readable format"""
     symbols = [("T", 1 << 40), ("G", 1 << 30), ("M", 1 << 20), ("K", 1 << 10)]
 
     if b < 0:
         raise ValueError("Must be bigger than 0")
```

## Comparing `socket_proxy-4.0.1.dist-info/LICENSE` & `socket_proxy-5.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `socket_proxy-4.0.1.dist-info/METADATA` & `socket_proxy-5.0.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 Metadata-Version: 2.1
 Name: socket-proxy
-Version: 4.0.1
+Version: 5.0.0
 Summary: Proxy TCP ports of local systems
 Home-page: https://github.com/fkantelberg/socket-proxy
 Author: Florian Kantelberg
 Author-email: florian.kantelberg@mailbox.org
 License: MIT
 Keywords: proxy socket network
-Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: api
 Requires-Dist: aiohttp ; extra == 'api'
+Provides-Extra: event
+Requires-Dist: aiohttp ; extra == 'event'
 
+[![main](https://github.com/fkantelberg/socket-proxy/actions/workflows/main.yaml/badge.svg)](https://github.com/fkantelberg/socket-proxy/actions/workflows/main.yaml)
+![Coverage](https://github.com/fkantelberg/socket-proxy/blob/master/coverage.svg)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/socket-proxy)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # socket-proxy
 
 This tool allows to forward TCP or HTTP ports to a server and make them available through the server.
```

