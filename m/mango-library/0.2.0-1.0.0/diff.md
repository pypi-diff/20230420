# Comparing `tmp/mango-library-0.2.0.tar.gz` & `tmp/mango-library-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-library-0.2.0.tar", last modified: Wed Dec 14 13:13:19 2022, max compression
+gzip compressed data, was "mango-library-1.0.0.tar", last modified: Thu Apr 20 08:40:04 2023, max compression
```

## Comparing `mango-library-0.2.0.tar` & `mango-library-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 13:13:19.676003 mango-library-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2022-12-14 13:12:52.000000 mango-library-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      619 2022-12-14 13:13:19.675003 mango-library-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       17 2022-12-14 13:12:52.000000 mango-library-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 13:13:19.668002 mango-library-0.2.0/mango_library/
--rw-rw-rw-   0 root         (0) root         (0)       62 2022-12-14 13:12:52.000000 mango-library-0.2.0/mango_library/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 13:13:19.671002 mango-library-0.2.0/mango_library/coalition/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-14 13:12:52.000000 mango-library-0.2.0/mango_library/coalition/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11264 2022-12-14 13:12:52.000000 mango-library-0.2.0/mango_library/coalition/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 13:13:19.672003 mango-library-0.2.0/mango_library/negotiation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-14 13:12:52.000000 mango-library-0.2.0/mango_library/negotiation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 13:13:19.675003 mango-library-0.2.0/mango_library/negotiation/cohda/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-14 13:12:52.000000 mango-library-0.2.0/mango_library/negotiation/cohda/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4268 2022-12-14 13:12:52.000000 mango-library-0.2.0/mango_library/negotiation/cohda/cohda_messages.py
--rw-rw-rw-   0 root         (0) root         (0)    26985 2022-12-14 13:12:52.000000 mango-library-0.2.0/mango_library/negotiation/cohda/cohda_negotiation.py
--rw-rw-rw-   0 root         (0) root         (0)     7293 2022-12-14 13:12:52.000000 mango-library-0.2.0/mango_library/negotiation/cohda/cohda_solution_aggregation.py
--rw-rw-rw-   0 root         (0) root         (0)     3864 2022-12-14 13:12:52.000000 mango-library-0.2.0/mango_library/negotiation/cohda/cohda_starting.py
--rw-rw-rw-   0 root         (0) root         (0)     6674 2022-12-14 13:12:52.000000 mango-library-0.2.0/mango_library/negotiation/cohda/data_classes.py
--rw-rw-rw-   0 root         (0) root         (0)    10134 2022-12-14 13:12:52.000000 mango-library-0.2.0/mango_library/negotiation/termination.py
--rw-rw-rw-   0 root         (0) root         (0)     2244 2022-12-14 13:12:52.000000 mango-library-0.2.0/mango_library/negotiation/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-14 13:13:19.670003 mango-library-0.2.0/mango_library.egg-info/
--rw-r--r--   0 root         (0) root         (0)      619 2022-12-14 13:13:19.000000 mango-library-0.2.0/mango_library.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      770 2022-12-14 13:13:19.000000 mango-library-0.2.0/mango_library.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-14 13:13:19.000000 mango-library-0.2.0/mango_library.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-12-14 13:13:19.000000 mango-library-0.2.0/mango_library.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-12-14 13:13:19.000000 mango-library-0.2.0/mango_library.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-12-14 13:13:19.000000 mango-library-0.2.0/mango_library.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-14 13:13:19.676003 mango-library-0.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3914 2022-12-14 13:12:52.000000 mango-library-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:40:04.824620 mango-library-1.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-20 08:39:34.000000 mango-library-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      619 2023-04-20 08:40:04.824620 mango-library-1.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-04-20 08:39:34.000000 mango-library-1.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:40:04.816620 mango-library-1.0.0/mango_library/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-04-20 08:39:34.000000 mango-library-1.0.0/mango_library/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:40:04.820620 mango-library-1.0.0/mango_library/coalition/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 08:39:34.000000 mango-library-1.0.0/mango_library/coalition/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16643 2023-04-20 08:39:34.000000 mango-library-1.0.0/mango_library/coalition/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:40:04.821620 mango-library-1.0.0/mango_library/negotiation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 08:39:34.000000 mango-library-1.0.0/mango_library/negotiation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:40:04.823620 mango-library-1.0.0/mango_library/negotiation/cohda/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 08:39:34.000000 mango-library-1.0.0/mango_library/negotiation/cohda/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5395 2023-04-20 08:39:34.000000 mango-library-1.0.0/mango_library/negotiation/cohda/cohda_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)    29836 2023-04-20 08:39:34.000000 mango-library-1.0.0/mango_library/negotiation/cohda/cohda_negotiation.py
+-rw-rw-rw-   0 root         (0) root         (0)     9681 2023-04-20 08:39:34.000000 mango-library-1.0.0/mango_library/negotiation/cohda/cohda_solution_aggregation.py
+-rw-rw-rw-   0 root         (0) root         (0)     8844 2023-04-20 08:39:34.000000 mango-library-1.0.0/mango_library/negotiation/cohda/cohda_starting.py
+-rw-rw-rw-   0 root         (0) root         (0)     6674 2023-04-20 08:39:34.000000 mango-library-1.0.0/mango_library/negotiation/cohda/data_classes.py
+-rw-rw-rw-   0 root         (0) root         (0)    10570 2023-04-20 08:39:34.000000 mango-library-1.0.0/mango_library/negotiation/termination.py
+-rw-rw-rw-   0 root         (0) root         (0)     3278 2023-04-20 08:39:34.000000 mango-library-1.0.0/mango_library/negotiation/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 08:40:04.819620 mango-library-1.0.0/mango_library.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      619 2023-04-20 08:40:04.000000 mango-library-1.0.0/mango_library.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      770 2023-04-20 08:40:04.000000 mango-library-1.0.0/mango_library.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 08:40:04.000000 mango-library-1.0.0/mango_library.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-20 08:40:04.000000 mango-library-1.0.0/mango_library.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-20 08:40:04.000000 mango-library-1.0.0/mango_library.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-20 08:40:04.000000 mango-library-1.0.0/mango_library.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 08:40:04.824620 mango-library-1.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3892 2023-04-20 08:39:34.000000 mango-library-1.0.0/setup.py
```

### Comparing `mango-library-0.2.0/LICENSE` & `mango-library-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mango-library-0.2.0/PKG-INFO` & `mango-library-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-library
-Version: 0.2.0
+Version: 1.0.0
 Summary: Library for the Modular Python Agent Framework MANGO
 Author: Mango Team
 Author-email: mango@offis.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mango-library-0.2.0/mango_library/negotiation/cohda/cohda_messages.py` & `mango-library-1.0.0/mango_library/negotiation/cohda/cohda_messages.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,34 @@
 
 from mango.messages.codecs import json_serializable
 
 from mango_library.negotiation.cohda.data_classes import WorkingMemory, SolutionCandidate
 
 
 @json_serializable
+class StartCohdaNegotiationMessage:
+    """
+        Message to start a COHDA negotiation.
+        Contains the coalition_id of the associated coalition
+        and the target parameters that are necessary for the agents to calculate the performance.
+        """
+    def __init__(self, coalition_id, send_weight, target_params = None):
+        self.coalition_id = coalition_id
+        self._send_weight = send_weight
+        self._target_params = target_params
+
+    @property
+    def send_weight(self):
+        return self._send_weight
+
+    @property
+    def target_params(self):
+        return self._target_params
+
+@json_serializable
 class CohdaNegotiationMessage:
     """
     Message for a COHDA negotiation.
     Contains the working memory of an agent.
     """
 
     def __init__(self, working_memory: WorkingMemory, negotiation_id: UUID, coalition_id: UUID,
@@ -145,7 +165,25 @@
     @property
     def negotiation_id(self) -> UUID:
         """Return the negotiation_id of the corresponding solution
 
         :return: the negotiation_id
         """
         return self._negotiation_id
+
+
+@json_serializable
+class ConfirmCohdaSolutionMessage:
+    """
+    Message that is sent by unit Agents to the Aggregator Agent to confirm that they have received the final solution.
+    """
+
+    def __init__(self, negotiation_id: UUID):
+        self._negotiation_id = negotiation_id
+
+    @property
+    def negotiation_id(self) -> UUID:
+        """Return the negotiation_id of the solution that was received
+
+        :return: the negotiation_id
+        """
+        return self._negotiation_id
```

### Comparing `mango-library-0.2.0/mango_library/negotiation/cohda/cohda_negotiation.py` & `mango-library-1.0.0/mango_library/negotiation/cohda/cohda_negotiation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,67 +1,105 @@
 import asyncio
+import inspect
 import logging
 from typing import List, Dict, Optional, Tuple, Callable
 from uuid import UUID
+
 import numpy as np
 
+from mango import Role
 from mango_library.coalition.core import CoalitionAssignment, CoalitionModel
-from mango_library.negotiation.cohda.cohda_messages import CohdaNegotiationMessage, CohdaSolutionRequestMessage, \
-    CohdaProposedSolutionMessage, StopNegotiationMessage, CohdaFinalSolutionMessage
-from mango_library.negotiation.cohda.data_classes import WorkingMemory, SolutionCandidate, SystemConfig, \
-    ScheduleSelection
-from mango.role.api import Role
+from mango_library.negotiation.cohda.cohda_messages import (
+    CohdaNegotiationMessage,
+    CohdaSolutionRequestMessage,
+    CohdaProposedSolutionMessage,
+    StopNegotiationMessage,
+    CohdaFinalSolutionMessage,
+    ConfirmCohdaSolutionMessage,
+)
+from mango_library.negotiation.cohda.data_classes import (
+    WorkingMemory,
+    SolutionCandidate,
+    SystemConfig,
+    ScheduleSelection,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class COHDANegotiationRole(Role):
-    """Negotiation role for COHDA.
-    """
+    """Negotiation role for COHDA."""
 
-    def __init__(self, schedules_provider: Callable, local_acceptable_func: Callable = None, perf_func: Callable = None,
-                 check_inbox_interval: float = 0.1):
+    def __init__(
+        self,
+        schedules_provider: Callable,
+        local_acceptable_func: Callable = None,
+        perf_func: Callable = None,
+        check_inbox_interval: float = 0.1,
+    ):
         """
         Init of COHDANegotiationRole
-        :param schedules_provider: Function that takes no arguments and returns a list of schedules
+        :param schedules_provider: Function that takes either no arguments or "candidate" as an argument or
+        "system_config" as an argument or "candidate" and "system_config" as arguments and
+        provides a list of possible schedules
         :param local_acceptable_func: Function that takes a schedule as input and returns a boolean indicating,
         if the schedule is locally acceptable or not. Defaults to lambda x: True
         :param perf_func: performance function for the agent. Defaults to deviation_from_target_schedule
         :param check_inbox_interval: Duration of buffering the CohdaNegotiationMessages [s]
         """
         super().__init__()
 
         self._schedules_provider = schedules_provider
-        self._perf_func = perf_func if perf_func is not None else COHDANegotiation.deviation_to_target_schedule
+        self._perf_func = (
+            perf_func
+            if perf_func is not None
+            else COHDANegotiation.deviation_to_target_schedule
+        )
 
         if local_acceptable_func is None:
             # accept all schedules if not function is provided
             self._is_local_acceptable = lambda x: True
         else:
             self._is_local_acceptable = local_acceptable_func
 
-        self._cohda_msg_queues: Dict[UUID, List[WorkingMemory]] = {}     # stores the message queues
-        self._cohda_tasks: Dict[UUID, asyncio.Task] = {}          # stores the tasks that process the inbox
+        self._cohda_msg_queues: Dict[
+            UUID, List[WorkingMemory]
+        ] = {}  # stores the message queues
+        self._cohda_tasks: Dict[
+            UUID, asyncio.Task
+        ] = {}  # stores the tasks that process the inbox
         self.check_inbox_interval = check_inbox_interval
 
     def setup(self) -> None:
         super().setup()
 
         # negotiation message
-        self.context.subscribe_message(self, self.handle_neg_msg,
-                                       lambda c, _: isinstance(c, CohdaNegotiationMessage))
+        self.context.subscribe_message(
+            self,
+            self.handle_neg_msg,
+            lambda c, _: isinstance(c, CohdaNegotiationMessage),
+        )
         # stop negotiation message
-        self.context.subscribe_message(self, self.handle_neg_stop,
-                                       lambda c, _: isinstance(c, StopNegotiationMessage))
+        self.context.subscribe_message(
+            self,
+            self.handle_neg_stop,
+            lambda c, _: isinstance(c, StopNegotiationMessage),
+        )
         # solution request message
-        self.context.subscribe_message(self, self.handle_solution_request,
-                                       lambda c, _: isinstance(c, CohdaSolutionRequestMessage))
+        self.context.subscribe_message(
+            self,
+            self.handle_solution_request,
+            lambda c, _: isinstance(c, CohdaSolutionRequestMessage),
+        )
         # final solution message
-        self.context.subscribe_message(self, self.handle_cohda_solution_msg,
-                                       lambda c, _: isinstance(c, CohdaFinalSolutionMessage))
+        self.context.subscribe_message(
+            self,
+            self.handle_cohda_solution_msg,
+            lambda c, _: isinstance(c, CohdaFinalSolutionMessage),
+        )
 
     async def on_stop(self) -> None:
         """
         Will be called once the agent is shutdown
         """
         # cancel all cohda tasks
         for task in self._cohda_tasks.values():
@@ -73,105 +111,143 @@
 
     def handle_neg_msg(self, content: CohdaNegotiationMessage, _):
         """
         Will be called when a CohdaNegotiationMessage is received
         :param content: CohdaNegotiationMessage
         :param _: meta dict
         """
-
         # check if there is a Coalition with the coalition_ID
-        if not self.context.get_or_create_model(CoalitionModel).exists(content.coalition_id):
-            logger.warning(f'Received a CohdaNegotiationMessage with the coalition_id {content.coalition_id}'
-                           f'but there is no such Coalition known.')
+        if not self.context.get_or_create_model(CoalitionModel).exists(
+            content.coalition_id
+        ):
+            logger.warning(
+                f"Received a CohdaNegotiationMessage with the coalition_id {content.coalition_id}"
+                f"but there is no such Coalition known."
+            )
             return
 
         # get coalition_assignment
         coalition_assignment: CoalitionAssignment = self.context.get_or_create_model(
-            CoalitionModel).by_id(content.coalition_id)
+            CoalitionModel
+        ).by_id(content.coalition_id)
 
         # get negotiation model
-        cohda_negotiation_model: CohdaNegotiationModel = self.context.get_or_create_model(CohdaNegotiationModel)
+        cohda_negotiation_model: CohdaNegotiationModel = (
+            self.context.get_or_create_model(CohdaNegotiationModel)
+        )
         # add negotiation if it doesn't exist
         if not cohda_negotiation_model.exists(content.negotiation_id):
             cohda_negotiation_model.add(
                 negotiation_id=content.negotiation_id,
                 cohda_negotiation=COHDANegotiation(
                     part_id=coalition_assignment.part_id,
                     schedule_provider=self._schedules_provider,
                     is_local_acceptable=self._is_local_acceptable,
-                    perf_func=self._perf_func
-                ))
-        cohda_negotiation = cohda_negotiation_model.by_id(negotiation_id=content.negotiation_id)
+                    perf_func=self._perf_func,
+                ),
+            )
+        cohda_negotiation = cohda_negotiation_model.by_id(
+            negotiation_id=content.negotiation_id
+        )
 
         # add message to the queue if negotiation is not stopped
         if not cohda_negotiation.stopped:
             if content.negotiation_id in self._cohda_msg_queues.keys():
                 cohda_negotiation.active = True
-                self._cohda_msg_queues[content.negotiation_id].append(content.working_memory)
+                self._cohda_msg_queues[content.negotiation_id].append(
+                    content.working_memory
+                )
             else:
-                self._cohda_msg_queues[content.negotiation_id] = [content.working_memory]
-                self._cohda_tasks[content.negotiation_id] = self.context.schedule_periodic_task(
+                self._cohda_msg_queues[content.negotiation_id] = [
+                    content.working_memory
+                ]
+                self._cohda_tasks[
+                    content.negotiation_id
+                ] = self.context.schedule_periodic_task(
                     self.get_process_msg_queue_coro(
-                            cohda_negotiation=cohda_negotiation, negotiation_id=content.negotiation_id,
-                            coalition_assignment=coalition_assignment),
-                    delay=self.check_inbox_interval)
+                        cohda_negotiation=cohda_negotiation,
+                        negotiation_id=content.negotiation_id,
+                        coalition_assignment=coalition_assignment,
+                    ),
+                    delay=self.check_inbox_interval,
+                )
 
-    def get_process_msg_queue_coro(self, cohda_negotiation, coalition_assignment: CoalitionAssignment,
-                                   negotiation_id: UUID):
+    def get_process_msg_queue_coro(
+        self,
+        cohda_negotiation,
+        coalition_assignment: CoalitionAssignment,
+        negotiation_id: UUID,
+    ):
         """
         Method that returns a coroutine that process a message queue of a specific COHDA negotiation.
         :param cohda_negotiation: the COHDANegotiation instance
         :param coalition_assignment: the corresponding coalition assignment
         :param negotiation_id: the corresponding negotiation ID
         :return: a coroutine without arguments that can be scheduled as periodic task
         """
+
         async def process_msg():
-            if len(self._cohda_msg_queues[negotiation_id]) > 0 and not cohda_negotiation.stopped:
+            if (
+                len(self._cohda_msg_queues[negotiation_id]) > 0
+                and not cohda_negotiation.stopped
+            ):
                 # get queue
-                cohda_message_queue, self._cohda_msg_queues[negotiation_id] = \
-                    self._cohda_msg_queues[negotiation_id], []
+                cohda_message_queue, self._cohda_msg_queues[negotiation_id] = (
+                    self._cohda_msg_queues[negotiation_id],
+                    [],
+                )
 
                 wm_to_send = cohda_negotiation.handle_cohda_msgs(cohda_message_queue)
 
                 if wm_to_send is not None:
                     # send message to all neighbors
                     for neighbor in coalition_assignment.neighbors:
-                        self.context.schedule_instant_task(self.context.send_acl_message(
+                        self.context.schedule_instant_acl_message(
                             content=CohdaNegotiationMessage(
                                 negotiation_id=negotiation_id,
                                 coalition_id=coalition_assignment.coalition_id,
                                 working_memory=wm_to_send,
                             ),
-                            receiver_addr=neighbor[1], receiver_id=neighbor[2],
-                            acl_metadata={'sender_addr': self.context.addr, 'sender_id': self.context.aid})
+                            receiver_addr=neighbor[1],
+                            receiver_id=neighbor[2],
+                            acl_metadata={
+                                "sender_addr": self.context.addr,
+                                "sender_id": self.context.aid,
+                            },
                         )
 
             else:
                 # set the negotiation as inactive as no message has arrived
                 cohda_negotiation.active = False
+
         return process_msg
 
     def handle_neg_stop(self, content: StopNegotiationMessage, _):
-        """ Is called once a StopNegotiationMessage arrived
-        """
+        """Is called once a StopNegotiationMessage arrived"""
         if content.negotiation_id in self._cohda_tasks.keys():
             # get negotiation
-            cohda_negotiation_model: CohdaNegotiationModel = self.context.get_or_create_model(CohdaNegotiationModel)
+            cohda_negotiation_model: CohdaNegotiationModel = (
+                self.context.get_or_create_model(CohdaNegotiationModel)
+            )
             if not cohda_negotiation_model.exists(content.negotiation_id):
-                logger.warning(f'Received a stop message for a negotiation with id {content.negotiation_id} '
-                               'but no such negotiation is running.')
+                logger.warning(
+                    f"Received a stop message for a negotiation with id {content.negotiation_id} "
+                    "but no such negotiation is running."
+                )
                 return
             cohda_negotiation = cohda_negotiation_model.by_id(content.negotiation_id)
 
             cohda_negotiation.stopped = True
 
             # wait until current iteration of negotiation is done (in case it is still running)
-            self.context.schedule_conditional_task(self.stop_cohda_task(content.negotiation_id),
-                                                   condition_func=lambda: not cohda_negotiation.active,
-                                                   lookup_delay=0.05)
+            self.context.schedule_conditional_task(
+                self.stop_cohda_task(content.negotiation_id),
+                condition_func=lambda: not cohda_negotiation.active,
+                lookup_delay=0.05,
+            )
 
     async def stop_cohda_task(self, negotiation_id):
         """
         Will stop the process message task of a certain negotiation
         :param negotiation_id: ID of the negotiation
         """
         # cancel task
@@ -185,99 +261,142 @@
     def handle_solution_request(self, content: CohdaSolutionRequestMessage, meta):
         """
         Handles a solution request for a certain negotiation
         :param content: The CohdaSolutionRequestMessage
         :param meta: meta of the message
         """
         # get negotiation
-        cohda_negotiation_model: CohdaNegotiationModel = self.context.get_or_create_model(CohdaNegotiationModel)
+        cohda_negotiation_model: CohdaNegotiationModel = (
+            self.context.get_or_create_model(CohdaNegotiationModel)
+        )
         if not cohda_negotiation_model.exists(content.negotiation_id):
-            logger.warning(f'Received a solution request message for a negotiation with id {content.negotiation_id} '
-                           'but no such negotiation exists.')
+            logger.warning(
+                f"Received a solution request message for a negotiation with id {content.negotiation_id} "
+                "but no such negotiation exists."
+            )
             return
         cohda_negotiation = cohda_negotiation_model.by_id(content.negotiation_id)
 
         # get current solution candidate
         final_solution = cohda_negotiation._memory.solution_candidate
         # send CohdaProposedSolutionMessage
-        self.context.schedule_instant_task(
-            self.context.send_acl_message(content=CohdaProposedSolutionMessage(
-                solution_candidate=final_solution, negotiation_id=content.negotiation_id
-            ),
-                receiver_addr=meta['sender_addr'], receiver_id=meta['sender_id'],
-                acl_metadata={'sender_id': self.context.aid}
+        self.context.schedule_instant_acl_message(
+            content=CohdaProposedSolutionMessage(
+                solution_candidate=final_solution,
+                negotiation_id=content.negotiation_id,
             ),
+            receiver_addr=meta["sender_addr"],
+            receiver_id=meta["sender_id"],
+            acl_metadata={"sender_id": self.context.aid},
         )
 
-    def handle_cohda_solution_msg(self, content: CohdaFinalSolutionMessage, _):
+    def handle_cohda_solution_msg(self, content: CohdaFinalSolutionMessage, meta):
         """
         Is called once a CohdaFinalSolutionMessage arrives
         :param content: The CohdaFinalSolutionMessage
-        :param _: Meta dict
+        :param meta: Meta dict
         :return:
         """
         final_candidate = content.solution_candidate
         neg_id = content.negotiation_id
         # get part id from negotiation
-        part_id = self.context.get_or_create_model(CohdaNegotiationModel).by_id(neg_id)._part_id
+        part_id = (
+            self.context.get_or_create_model(CohdaNegotiationModel)
+            .by_id(neg_id)
+            ._part_id
+        )
         # get individual schedule from final candidate
         final_schedule = final_candidate.schedules[part_id]
         # add final schedule to CohdaSolutionModel
         self.context.get_or_create_model(CohdaSolutionModel).add(neg_id, final_schedule)
+        # reply with a confirmation
+        self.context.schedule_instant_acl_message(
+            content=ConfirmCohdaSolutionMessage(neg_id),
+            receiver_addr=meta["sender_addr"],
+            receiver_id=meta["sender_id"],
+            acl_metadata={"sender_id": self.context.aid},
+        )
 
 
 class COHDANegotiation:
-    """COHDA-decider
-    """
+    """COHDA-decider"""
 
-    def __init__(self, schedule_provider: Callable, is_local_acceptable: Callable,
-                 part_id: str, perf_func=None):
+    def __init__(
+        self,
+        schedule_provider: Callable,
+        is_local_acceptable: Callable,
+        part_id: str,
+        perf_func=None,
+    ):
         """
         Init of the CohdaNegotiation
-        :param schedule_provider: Function that takes no arguments and provides a list of possible schedules
+        :param schedule_provider: Function that takes either no arguments or "candidate" as an argument or
+        "system_config" as an argument or "candidate" and "system_config" as arguments and
+        provides a list of possible schedules
         :param is_local_acceptable: Function that defines whether a schedule is locally acceptable or not
         :param part_id: the part_id of the agent
         :param perf_func: The performance function, that takes one numpy array and target_params
         as input and returns a float
         """
         self._part_id = part_id
-        self._schedule_provider = schedule_provider
+
+        def complete_schedule_provider(
+            system_config: SystemConfig, candidate: SolutionCandidate
+        ):
+            schedule_provider_args = inspect.signature(
+                schedule_provider
+            ).parameters.keys()
+            args = {}
+            if "candidate" in schedule_provider_args:
+                args["candidate"] = candidate
+            if "system_config" in schedule_provider_args:
+                args["system_config"] = system_config
+            return schedule_provider(**args)
+
+        self._schedule_provider = complete_schedule_provider
+
         self._is_local_acceptable = is_local_acceptable
         # start with an empty WorkingMemory
-        self._memory = WorkingMemory(None, SystemConfig({}), SolutionCandidate(self._part_id, {}, float('-inf')))
-        self._counter = 0   # counter for ScheduleSelections
+        self._memory = WorkingMemory(
+            None, SystemConfig({}), SolutionCandidate(self._part_id, {}, float("-inf"))
+        )
+        self._counter = 0  # counter for ScheduleSelections
 
-        self._stopped = False   # is Ture once a StopNegotiationMessage is received for this negotiation
+        self._stopped = False  # is Ture once a StopNegotiationMessage is received for this negotiation
         # self._active is False once an iteration of the process_message_queue function has not received any message
         self._active = True
 
         if perf_func is None:
             # as a default performance function we take the deviation to a target schedule, which is defined in
             # target_params
             self._perf_func = self.deviation_to_target_schedule
         else:
             self._perf_func = perf_func
 
     @staticmethod
-    def deviation_to_target_schedule(cluster_schedule: np.array, target_parameters) -> float:
+    def deviation_to_target_schedule(
+        cluster_schedule: np.array, target_parameters
+    ) -> float:
         """Default Performance function for a cohda negotiation
         :param cluster_schedule: The cluster schedule to be evaluated
         :param target_parameters: The target parameters. In this case we expect a Tuple of target_schedule, weights
         :return: The performance
         """
         if cluster_schedule.size == 0:
             # we have no schedules, so return worst possible performance
-            return float('-inf')
+            return float("-inf")
         # we expect this input here
         target_schedule, weights = target_parameters
         sum_cs = cluster_schedule.sum(axis=0)  # sum for each interval
-        diff = np.abs(np.array(target_schedule) - sum_cs)  # deviation to the target schedule
+        diff = np.abs(
+            np.array(target_schedule) - sum_cs
+        )  # deviation to the target schedule
         w_diff = diff * np.array(weights)  # multiply with weight vector
         result = -np.sum(w_diff)
-        return float(result)        # cast to float, otherwise a numpy object is returned
+        return float(result)  # cast to float, otherwise a numpy object is returned
 
     @property
     def active(self) -> bool:
         """Is seen as active
 
         :return: True if active, False otherwise
         """
@@ -302,15 +421,17 @@
     def stopped(self, is_stopped) -> None:
         """
         Set is stopped
         :param is_stopped: stopped
         """
         self._stopped = is_stopped
 
-    def handle_cohda_msgs(self, messages: List[WorkingMemory]) -> Optional[WorkingMemory]:
+    def handle_cohda_msgs(
+        self, messages: List[WorkingMemory]
+    ) -> Optional[WorkingMemory]:
         """
         This is called by the COHDARole.
         It takes a List of WorkingMemories, executes perceive, decide, act and returns
         a new WorkingMemory in case the working memory has changed and None otherwise
         :param messages: The list of received WorkingMemories
         :return: The message to be sent to the neighbors, None if no message has to be sent
         """
@@ -327,103 +448,136 @@
             sysconf, candidate = self._decide(sysconfig=sysconf, candidate=candidate)
             # act
             return self._act(new_sysconfig=sysconf, new_candidate=candidate)
         else:
             # nothing has changed in perceive, so we return None
             return None
 
-    def _perceive(self, working_memories: List[WorkingMemory]) -> Tuple[SystemConfig, SolutionCandidate]:
+    def _perceive(
+        self, working_memories: List[WorkingMemory]
+    ) -> Tuple[SystemConfig, SolutionCandidate]:
         """
         Updates the current knowledge
         :param working_memories: The List of received WorkingMemories
         :return: a tuple of SystemConfig, Candidate as a result of perceive
         """
         current_sysconfig = None
         current_candidate = None
         for new_wm in working_memories:
             if self._memory.target_params is None:
                 # get target parameters if not known
                 self._memory.target_params = new_wm.target_params
-
             if current_sysconfig is None:
                 if self._part_id not in self._memory.system_config.schedule_choices:
                     # if you have not yet selected any schedule in the sysconfig, choose any to start with
                     schedule_choices = self._memory.system_config.schedule_choices
                     schedule_choices[self._part_id] = ScheduleSelection(
-                        np.array(self._schedule_provider()[0]), self._counter + 1)
+                        np.array(
+                            self._schedule_provider(
+                                candidate=self._memory.solution_candidate,
+                                system_config=self._memory.system_config,
+                            )[0]
+                        ),
+                        self._counter + 1,
+                    )
                     self._counter += 1
                     # we need to create a new instance of SystemConfig so the updates are
                     # recognized in handle_cohda_msgs()
                     current_sysconfig = SystemConfig(schedule_choices=schedule_choices)
                 else:
                     current_sysconfig = self._memory.system_config
 
             if current_candidate is None:
                 if self._part_id not in self._memory.solution_candidate.schedules:
                     # if you have not yet selected any schedule in the sysconfig, choose any to start with
                     schedules = self._memory.solution_candidate.schedules
-                    schedules[self._part_id] = self._schedule_provider()[0]
+                    schedules[self._part_id] = self._schedule_provider(
+                        candidate=self._memory.solution_candidate,
+                        system_config=self._memory.system_config,
+                    )[0]
                     # we need to create a new class of SolutionCandidate so the updates are
                     # recognized in handle_cohda_msgs()
-                    current_candidate = SolutionCandidate(agent_id=self._part_id, schedules=schedules, perf=None)
-                    current_candidate.perf = self._perf_func(current_candidate.cluster_schedule,
-                                                             self._memory.target_params)
+                    current_candidate = SolutionCandidate(
+                        agent_id=self._part_id, schedules=schedules, perf=None
+                    )
+                    current_candidate.perf = self._perf_func(
+                        current_candidate.cluster_schedule, self._memory.target_params
+                    )
                 else:
                     current_candidate = self._memory.solution_candidate
 
             new_sysconf = new_wm.system_config
             new_candidate = new_wm.solution_candidate
 
             # Merge new information into current_sysconfig and current_candidate
-            current_sysconfig = self._merge_sysconfigs(sysconfig_i=current_sysconfig, sysconfig_j=new_sysconf)
+            current_sysconfig = self._merge_sysconfigs(
+                sysconfig_i=current_sysconfig, sysconfig_j=new_sysconf
+            )
             current_candidate = self._merge_candidates(
                 candidate_i=current_candidate,
                 candidate_j=new_candidate,
                 agent_id=self._part_id,
                 perf_func=self._perf_func,
-                target_params=self._memory.target_params)
+                target_params=self._memory.target_params,
+            )
 
         return current_sysconfig, current_candidate
 
-    def _decide(self, sysconfig: SystemConfig, candidate: SolutionCandidate) -> Tuple[SystemConfig, SolutionCandidate]:
+    def _decide(
+        self, sysconfig: SystemConfig, candidate: SolutionCandidate
+    ) -> Tuple[SystemConfig, SolutionCandidate]:
         """
         Check whether a better SolutionCandidate can be created based on the current state of the negotiation
         :param sysconfig: Current SystemConfig
         :param candidate: Current SolutionCandidate
         :return: Tuple of SystemConfig, SolutionCandidate. Unchanged to parameters if no new SolutionCandidate was
         found. Else it consists of the new SolutionCandidate and an updated SystemConfig
         """
-        possible_schedules = self._schedule_provider()
+        possible_schedules = self._schedule_provider(
+            candidate=candidate, system_config=sysconfig
+        )
         current_best_candidate = candidate
         for schedule in possible_schedules:
             if self._is_local_acceptable(schedule):
                 # create new candidate from sysconfig
                 new_candidate = SolutionCandidate.create_from_updated_sysconf(
-                    agent_id=self._part_id, sysconfig=sysconfig, new_schedule=np.array(schedule)
+                    agent_id=self._part_id,
+                    sysconfig=sysconfig,
+                    new_schedule=np.array(schedule),
+                )
+                new_performance = self._perf_func(
+                    new_candidate.cluster_schedule, self._memory.target_params
                 )
-                new_performance = self._perf_func(new_candidate.cluster_schedule, self._memory.target_params)
                 # only keep new candidates that perform better than the current one
                 if new_performance > current_best_candidate.perf:
                     new_candidate.perf = new_performance
                     current_best_candidate = new_candidate
 
-        schedule_in_candidate = current_best_candidate.schedules.get(self._part_id, None)
-        schedule_choice_in_sysconfig = sysconfig.schedule_choices.get(self._part_id, None)
+        schedule_in_candidate = current_best_candidate.schedules.get(
+            self._part_id, None
+        )
+        schedule_choice_in_sysconfig = sysconfig.schedule_choices.get(
+            self._part_id, None
+        )
 
-        if schedule_choice_in_sysconfig is None or \
-                not np.array_equal(schedule_in_candidate, schedule_choice_in_sysconfig.schedule):
+        if schedule_choice_in_sysconfig is None or not np.array_equal(
+            schedule_in_candidate, schedule_choice_in_sysconfig.schedule
+        ):
             # update Sysconfig if your schedule in the current sysconf is different to the one in the candidate
             sysconfig.schedule_choices[self._part_id] = ScheduleSelection(
-                schedule=schedule_in_candidate, counter=self._counter + 1)
+                schedule=schedule_in_candidate, counter=self._counter + 1
+            )
             # update counter
             self._counter += 1
 
         return sysconfig, current_best_candidate
 
-    def _act(self, new_sysconfig: SystemConfig, new_candidate: SolutionCandidate) -> WorkingMemory:
+    def _act(
+        self, new_sysconfig: SystemConfig, new_candidate: SolutionCandidate
+    ) -> WorkingMemory:
         """
         Stores the new SystemConfig and SolutionCandidate in Memory and returns the new working Memory
         :param new_sysconfig: The SystemConfig as a result from perceive and decide
         :param new_candidate: The SolutionCandidate as a result from perceive and decide
         :return: The COHDA message that should be sent
         """
         # update memory
@@ -437,26 +591,32 @@
         """
         Merge *sysconf_i* and *sysconf_j* and return the result.
 
         Returns a merged SystemConfig. If the sysconfig_i remains unchanged, the same instance of sysconfig_i is
         returned, otherwise a new object is created.
         """
 
-        sysconfig_i_schedules: Dict[str, ScheduleSelection] = sysconfig_i.schedule_choices
-        sysconfig_j_schedules: Dict[str, ScheduleSelection] = sysconfig_j.schedule_choices
+        sysconfig_i_schedules: Dict[
+            str, ScheduleSelection
+        ] = sysconfig_i.schedule_choices
+        sysconfig_j_schedules: Dict[
+            str, ScheduleSelection
+        ] = sysconfig_j.schedule_choices
         key_set_i = set(sysconfig_i_schedules.keys())
         key_set_j = set(sysconfig_j_schedules.keys())
 
         new_sysconfig: Dict[str, ScheduleSelection] = {}
         modified = False
 
         for i, a in enumerate(sorted(key_set_i | key_set_j)):
             # An "a" might be in key_set_i, key_set_j or in both!
-            if a in key_set_i and \
-                    (a not in key_set_j or sysconfig_i_schedules[a].counter >= sysconfig_j_schedules[a].counter):
+            if a in key_set_i and (
+                a not in key_set_j
+                or sysconfig_i_schedules[a].counter >= sysconfig_j_schedules[a].counter
+            ):
                 # Use data of sysconfig_i
                 schedule_selection = sysconfig_i_schedules[a]
             else:
                 # Use data of sysconfig_j
                 schedule_selection = sysconfig_j_schedules[a]
                 modified = True
 
@@ -466,16 +626,21 @@
             sysconf = SystemConfig(new_sysconfig)
         else:
             sysconf = sysconfig_i
 
         return sysconf
 
     @staticmethod
-    def _merge_candidates(candidate_i: SolutionCandidate, candidate_j: SolutionCandidate,
-                          agent_id: str, perf_func: Callable, target_params):
+    def _merge_candidates(
+        candidate_i: SolutionCandidate,
+        candidate_j: SolutionCandidate,
+        agent_id: str,
+        perf_func: Callable,
+        target_params,
+    ):
         """
         Returns a merged Candidate. If the candidate_i remains unchanged, the same instance of candidate_i is
         returned, otherwise a new object is created with agent_id as candidate.agent_id
         :param candidate_i: The first candidate
         :param candidate_j: The second candidate
         :param agent_id: The agent_id that defines who is the creator of a new candidate
         :param perf_func: The performance function
@@ -506,23 +671,24 @@
                 if a in keyset_i:
                     schedule = candidate_i.schedules[a]
                 else:
                     schedule = candidate_j.schedules[a]
                 new_schedules[a] = schedule
 
             # create new SolutionCandidate
-            candidate = SolutionCandidate(agent_id=agent_id, schedules=new_schedules, perf=None)
+            candidate = SolutionCandidate(
+                agent_id=agent_id, schedules=new_schedules, perf=None
+            )
             candidate.perf = perf_func(candidate.cluster_schedule, target_params)
 
         return candidate
 
 
 class CohdaNegotiationModel:
-    """Model for storing all metadata regarding negotiations
-    """
+    """Model for storing all metadata regarding negotiations"""
 
     def __init__(self) -> None:
         self._negotiations: Dict[UUID, COHDANegotiation] = {}
 
     def by_id(self, negotiation_id: UUID) -> COHDANegotiation:
         """Get a negotiation by id
         :param negotiation_id: id of the negotiation
```

### Comparing `mango-library-0.2.0/mango_library/negotiation/cohda/data_classes.py` & `mango-library-1.0.0/mango_library/negotiation/cohda/data_classes.py`

 * *Files identical despite different names*

### Comparing `mango-library-0.2.0/mango_library/negotiation/termination.py` & `mango-library-1.0.0/mango_library/negotiation/termination.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,27 +13,30 @@
 considers itself as inactive.
 """
 import asyncio
 from fractions import Fraction
 from typing import Dict, Any, Union, Optional, Set, Tuple, Callable, List
 from uuid import UUID
 
-from .cohda.cohda_negotiation import CohdaNegotiationModel
+from mango.messages.codecs import json_serializable
+from mango import Role
+
+from mango_library.negotiation.cohda.cohda_messages import CohdaNegotiationMessage
 from .cohda.cohda_messages import StopNegotiationMessage
+from .cohda.cohda_negotiation import CohdaNegotiationModel
 from ..coalition.core import CoalitionModel, CoalitionAssignment
-from mango_library.negotiation.cohda.cohda_messages import CohdaNegotiationMessage
-from mango.role.api import Role
-from mango.messages.codecs import json_serializable
 
 
 @json_serializable
 class TerminationMessage:
-    """Message for sending the remaining weight to the controller
-    """
-    def __init__(self, weight: Fraction, coalition_id: UUID, negotiation_id: UUID) -> None:
+    """Message for sending the remaining weight to the controller"""
+
+    def __init__(
+        self, weight: Fraction, coalition_id: UUID, negotiation_id: UUID
+    ) -> None:
         self._weight = weight
         self._coalition_id = coalition_id
         self._negotiation_id = negotiation_id
 
     @property
     def weight(self) -> Fraction:
         """Return the remaining weight
@@ -60,14 +63,15 @@
 
 
 @json_serializable
 class InformAboutTerminationMessage:
     """
     Message that informs an agent that a negotiation should be stopped.
     """
+
     def __init__(self, negotiation_id: UUID, participants: List[Tuple]) -> None:
         self._negotiation_id = negotiation_id
         self._participants = participants
 
     @property
     def negotiation_id(self) -> UUID:
         """Return the negotiation id
@@ -86,50 +90,60 @@
 
 
 class NegotiationTerminationParticipantRole(Role):
     """Role for negotiation participants. Will add the weight attribute to every
     coalition related message send.
     """
 
-    def __init__(self, negotiation_model_class=CohdaNegotiationModel,
-                 negotiation_message_class=CohdaNegotiationMessage):
+    def __init__(
+        self,
+        negotiation_model_class=CohdaNegotiationModel,
+        negotiation_message_class=CohdaNegotiationMessage,
+    ):
         super().__init__()
         self._negotiation_message_class = negotiation_message_class
         self._negotiation_model_class = negotiation_model_class
-        self._negotiation_model = None  # will be defined in setup(), once the context exists
+        self._negotiation_model = (
+            None  # will be defined in setup(), once the context exists
+        )
         self._weight_map: Dict[UUID, Fraction] = {}
         self._termination_check_tasks: Dict[UUID, asyncio.Task] = {}
 
     def setup(self):
         super().setup()
-        self._negotiation_model = self.context.get_or_create_model(self._negotiation_model_class)
+        self._negotiation_model = self.context.get_or_create_model(
+            self._negotiation_model_class
+        )
         self.context.subscribe_send(self, self.on_send)
-        self.context.subscribe_message(self, self.handle_neg_msg,
-                                       lambda c, _: isinstance(c, self._negotiation_message_class))
-
-    def on_send(self, content,
-                receiver_addr: Union[str, Tuple[str, int]], *,
-                receiver_id: Optional[str] = None,
-                create_acl: bool = False,
-                acl_metadata: Optional[Dict[str, Any]] = None,
-                mqtt_kwargs: Dict[str, Any] = None):
+        self.context.subscribe_message(
+            self,
+            self.handle_neg_msg,
+            lambda c, _: isinstance(c, self._negotiation_message_class),
+        )
+
+    def on_send(
+        self,
+        content,
+        receiver_addr: Union[str, Tuple[str, int]],
+        *,
+        receiver_id: Optional[str] = None,
+        **kwargs
+    ):
         """Add the weight to every coalition related message
 
         :param content: content of the message
         :param receiver_addr: address
         :param receiver_id: id of the receiver. Defaults to None.
-        :param create_acl: If you want to wrap the message in an ACL. Defaults to False.
-        :param acl_metadata: ACL meta data. Defaults to None.
-        :param mqtt_kwargs: Args for MQTT. Defaults to None.
+        :param kwargs: additional parameters
         """
         if isinstance(content, self._negotiation_message_class):
 
             if content.negotiation_id not in self._weight_map:
                 self._weight_map[content.negotiation_id] = Fraction(0, 1)
-            if not hasattr(content, 'message_weight') or content.message_weight is None:
+            if not hasattr(content, "message_weight") or content.message_weight is None:
                 content.message_weight = self._weight_map[content.negotiation_id] / 2
             self._weight_map[content.negotiation_id] /= 2
 
     def handle_neg_msg(self, content, _: Dict[str, Any]) -> None:
         """Check whether a coalition related message has been received and manipulate the internal
         weight accordingly. Setup a conditional task that checks for termination.
 
@@ -137,105 +151,147 @@
         :param _: the meta data
         """
         if content.negotiation_id in self._weight_map:
             self._weight_map[content.negotiation_id] += content.message_weight
         else:
             self._weight_map[content.negotiation_id] = content.message_weight
 
-        coalition_assignment: CoalitionAssignment = \
-            self.context.get_or_create_model(CoalitionModel).by_id(content.coalition_id)
-
-        term_detector = coalition_assignment.controller_agent_addr, coalition_assignment.controller_agent_id
+        coalition_assignment: CoalitionAssignment = self.context.get_or_create_model(
+            CoalitionModel
+        ).by_id(content.coalition_id)
+
+        term_detector = (
+            coalition_assignment.controller_agent_addr,
+            coalition_assignment.controller_agent_id,
+        )
 
         def _check_weight_condition() -> bool:
             """
             Function that checks whether the negotiation has 'probably' terminated.
             :return: boolean
             """
-            return (not self._negotiation_model.by_id(negotiation_id=content.negotiation_id).active and
-                    self._weight_map[content.negotiation_id] != 0)
+            return (
+                not self._negotiation_model.by_id(
+                    negotiation_id=content.negotiation_id
+                ).active
+                and self._weight_map[content.negotiation_id] != 0
+            )
 
-        if (content.negotiation_id not in self._termination_check_tasks or
-                self._termination_check_tasks[content.negotiation_id].done()):
+        if (
+            content.negotiation_id not in self._termination_check_tasks
+            or self._termination_check_tasks[content.negotiation_id].done()
+        ):
             # create a new conditional task that checks for termination
-            self._termination_check_tasks[content.negotiation_id] = self.context.schedule_conditional_task(
+            self._termination_check_tasks[
+                content.negotiation_id
+            ] = self.context.schedule_conditional_task(
                 self._send_weight(term_detector, content),
-                condition_func=_check_weight_condition)
+                condition_func=_check_weight_condition,
+            )
 
     async def _send_weight(self, termination_detector: Tuple, content):
         """
         Sends the current weight to the termination controller
         :param termination_detector: Address (addr, aid) of the termination detector that should receive the
         weight message
         :param content: The NeogotiationMessage
 
         """
         # store weight
         current_weight = self._weight_map[content.negotiation_id]
         # reset weight
         self._weight_map[content.negotiation_id] = Fraction(0, 1)
         # Send weight
-        await(self.context.send_acl_message(
-            content=TerminationMessage(current_weight, content.coalition_id, content.negotiation_id),
-            receiver_addr=termination_detector[0],
-            receiver_id=termination_detector[1],
-            acl_metadata={'sender_addr': self.context.addr, 'sender_id': self.context.aid}
-        ))
+        await (
+            self.context.send_acl_message(
+                content=TerminationMessage(
+                    current_weight, content.coalition_id, content.negotiation_id
+                ),
+                receiver_addr=termination_detector[0],
+                receiver_id=termination_detector[1],
+                acl_metadata={
+                    "sender_addr": self.context.addr,
+                    "sender_id": self.context.aid,
+                },
+            )
+        )
 
 
 class NegotiationTerminationDetectorRole(Role):
-    """
+    """ """
 
-    """
-    def __init__(self, on_termination: Callable = None, aggregator_addr=None, aggregator_id: str = None):
+    def __init__(
+        self,
+        on_termination: Callable = None,
+        aggregator_addr=None,
+        aggregator_id: str = None,
+    ):
         super().__init__()
         self._weight_map: Dict[UUID, Fraction] = {}
         self._participant_map: Dict[UUID, Set[Tuple[Tuple, str]]] = {}
-        self._on_termination = on_termination if on_termination is not None else self._send_stop_and_inform
+        self._on_termination = (
+            on_termination if on_termination is not None else self._send_stop_and_inform
+        )
         self._aggregator_addr = aggregator_addr
         self._aggregator_id = aggregator_id
 
     def setup(self):
         super().setup()
-        self.context.subscribe_message(self, self.handle_term_msg, lambda c, _: isinstance(c, TerminationMessage))
+        self.context.subscribe_message(
+            self, self.handle_term_msg, lambda c, _: isinstance(c, TerminationMessage)
+        )
         if self._aggregator_addr is None and self._aggregator_id is None:
             self._aggregator_addr = self.context.addr
             self._aggregator_id = self.context.aid
 
     async def _send_stop_and_inform(self, negotiation_id):
         # send stopNegotiationMessage first
         for agent_addr, agent_id in self._participant_map[negotiation_id]:
             await self.context.send_acl_message(
                 content=StopNegotiationMessage(negotiation_id=negotiation_id),
                 receiver_addr=agent_addr,
                 receiver_id=agent_id,
-                acl_metadata={'sender_addr': self.context.addr, 'sender_id': self.context.aid},
+                acl_metadata={
+                    "sender_addr": self.context.addr,
+                    "sender_id": self.context.aid,
+                },
             )
 
         # now send message to aggregator
         if self._aggregator_addr is not None and self._aggregator_id is not None:
             await self.context.send_acl_message(
-                content=InformAboutTerminationMessage(negotiation_id=negotiation_id,
-                                                      participants=list(self._participant_map[negotiation_id])),
+                content=InformAboutTerminationMessage(
+                    negotiation_id=negotiation_id,
+                    participants=list(self._participant_map[negotiation_id]),
+                ),
                 receiver_addr=self._aggregator_addr,
                 receiver_id=self._aggregator_id,
-                acl_metadata={'sender_addr': self.context.addr, 'sender_id': self.context.aid},
+                acl_metadata={
+                    "sender_addr": self.context.addr,
+                    "sender_id": self.context.aid,
+                },
             )
 
-    def handle_term_msg(self, content: TerminationMessage, meta: Dict[str, Any]) -> None:
+    def handle_term_msg(
+        self, content: TerminationMessage, meta: Dict[str, Any]
+    ) -> None:
         """Handle the termination message.
 
         :param content: the message
         :param meta: meta data
         """
         neg_id = content.negotiation_id
-        if 'sender_addr' in meta and 'sender_id' in meta:
+        if "sender_addr" in meta and "sender_id" in meta:
+            sender_addr = meta["sender_addr"]
+            if isinstance(sender_addr, list):
+                sender_addr = tuple(sender_addr)
+
             if neg_id not in self._participant_map:
                 self._participant_map[neg_id] = set()
-            self._participant_map[neg_id].add((tuple(meta['sender_addr']), meta['sender_id']))
+            self._participant_map[neg_id].add((sender_addr, meta["sender_id"]))
 
         if neg_id not in self._weight_map:
             self._weight_map[neg_id] = content.weight
         else:
             self._weight_map[neg_id] += content.weight
 
         if self._weight_map[neg_id] == 1:
```

### Comparing `mango-library-0.2.0/mango_library/negotiation/util.py` & `mango-library-1.0.0/mango_library/negotiation/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import numpy as np
 import fractions
 import uuid
 import base64
-from mango_library.coalition.core import CoalitionInvite, CoaltitionResponse, CoalitionAssignment
+from mango_library.coalition.core import CoalitionInvite, CoaltitionResponse, CoalitionAssignment, \
+    CoalitionAssignmentConfirm, CoalitionBuildConfirm
 from mango_library.negotiation.cohda.data_classes import ScheduleSelection, \
     SystemConfig, SolutionCandidate, WorkingMemory
-
-from mango_library.negotiation.cohda.cohda_messages import CohdaNegotiationMessage, CohdaProposedSolutionMessage,\
-    CohdaSolutionRequestMessage, CohdaFinalSolutionMessage
-from mango_library.negotiation.termination import TerminationMessage, StopNegotiationMessage,\
+from mango_library.negotiation.cohda.cohda_messages import CohdaNegotiationMessage, CohdaProposedSolutionMessage, \
+    CohdaSolutionRequestMessage, CohdaFinalSolutionMessage, ConfirmCohdaSolutionMessage
+from mango_library.negotiation.multiobjective_cohda.cohda_messages import MoCohdaNegotiationMessage
+from mango_library.negotiation.multiobjective_cohda.data_classes import ScheduleSelections, \
+    SystemConfig as SystemConfig_m, SolutionCandidate as SolutionCandidate_m, WorkingMemory as WorkingMemory_m
+from mango_library.negotiation.termination import TerminationMessage, StopNegotiationMessage, \
     InformAboutTerminationMessage
 
 
 def get_np_serializer():
     """Return a tuple *(type, serialize(), deserialize())* for NumPy arrays
     """
     return np.ndarray, _serialize_ndarray, _deserialize_ndarray
@@ -59,20 +62,39 @@
 
 cohda_serializers = [
     get_np_serializer,
     get_uuid_serializer,
     CoalitionInvite.__serializer__,
     CoaltitionResponse.__serializer__,
     CoalitionAssignment.__serializer__,
+    CoalitionAssignmentConfirm.__serializer__,
+    CoalitionBuildConfirm.__serializer__,
     ScheduleSelection.__serializer__,
     SystemConfig.__serializer__,
     SolutionCandidate.__serializer__,
     WorkingMemory.__serializer__,
     CohdaNegotiationMessage.__serializer__,
     CohdaSolutionRequestMessage.__serializer__,
     CohdaProposedSolutionMessage.__serializer__,
     TerminationMessage.__serializer__,
     get_fraction_serializer,
     StopNegotiationMessage.__serializer__,
     InformAboutTerminationMessage.__serializer__,
     CohdaFinalSolutionMessage.__serializer__,
+    ConfirmCohdaSolutionMessage.__serializer__,
+]
+
+multi_objective_serializers = [
+    get_np_serializer,
+    get_uuid_serializer,
+    CoalitionInvite.__serializer__,
+    CoaltitionResponse.__serializer__,
+    CoalitionAssignment.__serializer__,
+    ScheduleSelections.__serializer__,
+    SystemConfig_m.__serializer__,
+    SolutionCandidate_m.__serializer__,
+    WorkingMemory_m.__serializer__,
+    MoCohdaNegotiationMessage.__serializer__,
+    TerminationMessage.__serializer__,
+    get_fraction_serializer,
+    StopNegotiationMessage.__serializer__,
 ]
```

### Comparing `mango-library-0.2.0/mango_library.egg-info/PKG-INFO` & `mango-library-1.0.0/mango_library.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-library
-Version: 0.2.0
+Version: 1.0.0
 Summary: Library for the Modular Python Agent Framework MANGO
 Author: Mango Team
 Author-email: mango@offis.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mango-library-0.2.0/mango_library.egg-info/SOURCES.txt` & `mango-library-1.0.0/mango_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mango-library-0.2.0/setup.py` & `mango-library-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,26 +8,24 @@
 import os
 import sys
 from shutil import rmtree
 
 from setuptools import find_packages, setup, Command
 
 # Package meta-data.
-NAME = 'mango-library'
-DESCRIPTION = 'Library for the Modular Python Agent Framework MANGO'
-URL = 'https://gitlab.com/mango-agents/mango-library'
-EMAIL = 'mango@offis.de'
-AUTHOR = 'Mango Team'
-REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '0.2.0'
+NAME = "mango-library"
+DESCRIPTION = "Library for the Modular Python Agent Framework MANGO"
+URL = "https://gitlab.com/mango-agents/mango-library"
+EMAIL = "mango@offis.de"
+AUTHOR = "Mango Team"
+REQUIRES_PYTHON = ">=3.7.0"
+VERSION = "1.0.0"
 
 # What packages are required for this module to be executed?
-REQUIRED = [
-     'numpy', 'mango-agents'
-]
+REQUIRED = ["numpy", "mango-agents==1.0.0"]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
@@ -36,99 +34,96 @@
 # If you do change the License, remember to change the Trove Classifier for that!
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import the README and use it as the long-description.
 # Note: this will only work if 'README.md' is present in your MANIFEST.in file!
 try:
-    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
-        long_description = '\n' + f.read()
+    with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
+        long_description = "\n" + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 # Load the package's __version__.py module as a dictionary.
 about = {}
 if not VERSION:
     project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
-    with open(os.path.join(here, project_slug, '__version__.py')) as f:
+    with open(os.path.join(here, project_slug, "__version__.py")) as f:
         exec(f.read(), about)
 else:
-    about['__version__'] = VERSION
+    about["__version__"] = VERSION
 
 
 class UploadCommand(Command):
     """Support setup.py upload."""
 
-    description = 'Build and publish the package.'
+    description = "Build and publish the package."
     user_options = []
 
     @staticmethod
     def status(s):
         """Prints things in bold."""
-        print('\033[1m{0}\033[0m'.format(s))
+        print("\033[1m{0}\033[0m".format(s))
 
     def initialize_options(self):
         pass
 
     def finalize_options(self):
         pass
 
     def run(self):
         try:
-            self.status('Removing previous builds…')
-            rmtree(os.path.join(here, 'dist'))
+            self.status("Removing previous builds…")
+            rmtree(os.path.join(here, "dist"))
         except OSError:
             pass
 
-        self.status('Building Source and Wheel (universal) distribution…')
-        os.system('{0} setup.py sdist bdist_wheel --universal'.format(
-            sys.executable))
-
-        self.status('Uploading the package to PyPI via Twine…')
-        os.system('twine upload dist/*')
-
-        self.status('Pushing git tags…')
-        os.system('git tag v{0}'.format(about['__version__']))
-        os.system('git push --tags')
+        self.status("Building Source and Wheel (universal) distribution…")
+        os.system("{0} setup.py sdist bdist_wheel --universal".format(sys.executable))
+
+        self.status("Uploading the package to PyPI via Twine…")
+        os.system("twine upload dist/*")
+
+        self.status("Pushing git tags…")
+        os.system("git tag v{0}".format(about["__version__"]))
+        os.system("git push --tags")
 
         sys.exit()
 
 
 # Where the magic happens:
 setup(
     name=NAME,
-    version=about['__version__'],
+    version=about["__version__"],
     description=DESCRIPTION,
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     # url=URL,
-    packages=find_packages(
-        exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
-    namespace_packages=['mango_library'],
+    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
+    namespace_packages=["mango_library"],
     # If your package is a single module, use this instead of 'packages':
     # py_modules=['mypackage'],
-
     # entry_points={
     #     'console_scripts': ['mycli=mymodule:cli'],
     # },
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
-    license='MIT',
+    license="MIT",
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: Implementation :: CPython',
-        'Programming Language :: Python :: Implementation :: PyPy'
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Programming Language :: Python :: Implementation :: PyPy",
     ],
     # $ setup.py publish support.
     cmdclass={
-        'upload': UploadCommand,
+        "upload": UploadCommand,
     },
 )
```

