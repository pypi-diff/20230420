# Comparing `tmp/lumeny-0.1.2.tar.gz` & `tmp/lumeny-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumeny-0.1.2.tar", max compression
+gzip compressed data, was "lumeny-0.2.0.tar", max compression
```

## Comparing `lumeny-0.1.2.tar` & `lumeny-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      652 2023-04-13 12:21:17.181246 lumeny-0.1.2/README.md
--rw-r--r--   0        0        0     4712 2023-04-12 16:47:14.787304 lumeny-0.1.2/lumeny/CaldavConnector.py
--rw-r--r--   0        0        0     1590 2023-04-13 12:16:45.567741 lumeny-0.1.2/lumeny/ConfigLoader.py
--rw-r--r--   0        0        0     2068 2023-03-26 21:54:13.154345 lumeny-0.1.2/lumeny/EmbeddingGenerator.py
--rw-r--r--   0        0        0     3001 2023-04-13 12:18:41.544232 lumeny-0.1.2/lumeny/MinifluxConnector.py
--rw-r--r--   0        0        0        0 2023-03-26 11:54:25.500396 lumeny-0.1.2/lumeny/QdrantConnector.py
--rw-r--r--   0        0        0        0 2023-03-26 11:44:08.561839 lumeny-0.1.2/lumeny/__init__.py
--rw-r--r--   0        0        0     1675 2023-04-14 22:04:00.264026 lumeny-0.1.2/lumeny/ai.py
--rw-r--r--   0        0        0     4864 2023-04-14 21:57:36.895011 lumeny-0.1.2/lumeny/calendar.py
--rw-r--r--   0        0        0     1992 2023-04-14 12:09:46.339099 lumeny-0.1.2/lumeny/cli.py
--rw-r--r--   0        0        0     1839 2023-04-13 12:08:33.198863 lumeny-0.1.2/lumeny/tui.py
--rw-r--r--   0        0        0      912 2023-04-12 20:24:12.954146 lumeny-0.1.2/lumeny/utils.py
--rw-r--r--   0        0        0      645 2023-04-14 22:02:47.742081 lumeny-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 lumeny-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      652 2023-04-13 12:21:17.181246 lumeny-0.2.0/README.md
+-rw-r--r--   0        0        0     4712 2023-04-12 16:47:14.787304 lumeny-0.2.0/lumeny/CaldavConnector.py
+-rw-r--r--   0        0        0     1590 2023-04-13 12:16:45.567741 lumeny-0.2.0/lumeny/ConfigLoader.py
+-rw-r--r--   0        0        0     2068 2023-03-26 21:54:13.154345 lumeny-0.2.0/lumeny/EmbeddingGenerator.py
+-rw-r--r--   0        0        0     3001 2023-04-13 12:18:41.544232 lumeny-0.2.0/lumeny/MinifluxConnector.py
+-rw-r--r--   0        0        0        0 2023-03-26 11:54:25.500396 lumeny-0.2.0/lumeny/QdrantConnector.py
+-rw-r--r--   0        0        0        0 2023-03-26 11:44:08.561839 lumeny-0.2.0/lumeny/__init__.py
+-rw-r--r--   0        0        0     1684 2023-04-20 01:43:03.801671 lumeny-0.2.0/lumeny/ai_utils.py
+-rw-r--r--   0        0        0     6002 2023-04-20 02:17:32.419822 lumeny-0.2.0/lumeny/calendar.py
+-rw-r--r--   0        0        0     2802 2023-04-20 02:06:59.785132 lumeny-0.2.0/lumeny/cli.py
+-rw-r--r--   0        0        0     1839 2023-04-13 12:08:33.198863 lumeny-0.2.0/lumeny/tui.py
+-rw-r--r--   0        0        0     1046 2023-04-20 02:04:35.099308 lumeny-0.2.0/lumeny/utils.py
+-rw-r--r--   0        0        0      645 2023-04-20 02:19:05.031699 lumeny-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 lumeny-0.2.0/PKG-INFO
```

### Comparing `lumeny-0.1.2/README.md` & `lumeny-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lumeny-0.1.2/lumeny/CaldavConnector.py` & `lumeny-0.2.0/lumeny/CaldavConnector.py`

 * *Files identical despite different names*

### Comparing `lumeny-0.1.2/lumeny/ConfigLoader.py` & `lumeny-0.2.0/lumeny/ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `lumeny-0.1.2/lumeny/EmbeddingGenerator.py` & `lumeny-0.2.0/lumeny/EmbeddingGenerator.py`

 * *Files identical despite different names*

### Comparing `lumeny-0.1.2/lumeny/MinifluxConnector.py` & `lumeny-0.2.0/lumeny/MinifluxConnector.py`

 * *Files identical despite different names*

### Comparing `lumeny-0.1.2/lumeny/ai.py` & `lumeny-0.2.0/lumeny/ai_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 config = ConfigLoader().get_config()
 
 openai.api_key = config["openai"]["api"]
 
 # Function to interact with the chatcompletion API
 
 
-def chat(the_conversation: List[Dict], model: str = "gpt-4", temperature: float = 0.1):
+def chat_with_gpt(the_conversation: List[Dict], model: str = "gpt-4", temperature: float = 0.1):
     """
 
     The function to interact with the chatcompletion API
 
     :param the_conversation: conversation stored in list of dictionaries
     :param model: gpt3.5-turbo, gpt-4
     :param temperature: from 0 to 1, control the randomness of the response
```

### Comparing `lumeny-0.1.2/lumeny/calendar.py` & `lumeny-0.2.0/lumeny/calendar.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,46 @@
 """Define the commands that generate commands correspoends to the calendar manipulation"""
 
 from typing import Dict, List
 import datetime
 
-from lumeny.ai import chat, create_system_msg, create_user_msg
+from datetime import datetime, timedelta
+
+from lumeny.ai_utils import chat_with_gpt, create_system_msg, create_user_msg
+
+
+def repeat_learn(the_topic: str, repeat_days: List[int], start_day: int = 0) -> str:
+    """
+    the functions to create an event that follows the forgetting curves.
+    The default is to repeat at 2, 5, 14, 30 days after.
+
+    :param the_topic: What event it is
+    :param repeat_days: the scheme to repeat an tpoic
+    :param start_date int: the date you viewed/learnt this topic, relative to today. Default is 0
+    :return: the command
+    """
+
+    if repeat_days is None:
+        repeat_days = [2, 5, 14, 30]
+
+    today: datetime = datetime.today()
+
+    start_date: datetime = today - timedelta(days=start_day)
+
+    repeat_dates: List[datetime] = [
+        start_date + timedelta(days=day) for day in repeat_days
+    ]
+
+    repeat_commands: str = ""
+
+    for i, day in enumerate(repeat_dates):
+        date_str: str = day.strftime("%d.%m.%Y")
+        repeat_commands += f"khal new -a personal {date_str} {date_str} {the_topic} :: {the_topic} for the {i+1}th time ; "
+
+    return repeat_commands
 
 
 def generate_command_with_gpt4(the_instruction: str) -> str:
     """
     Generate a khal command to add an event to the calendar with the gpt4 model.
 
     :param instruction: The natural language instruction
@@ -41,15 +74,15 @@
 
     # get the date of today in the format DD-MM-YYYY
     custom_system_prompt: Dict[str, str] = create_system_msg(prompt_content)
 
     conversation: List[Dict] = [custom_system_prompt]
     user_message = create_user_msg(the_instruction)
     conversation.append(user_message)
-    response = chat(conversation, model="gpt-4")
+    response = chat_with_gpt(conversation, model="gpt-4")
     return response
 
 
 # def is_period_of_time(instruct: str) -> str:
 #     prompt_content: str = "Your task is to classify a sentence. You will receive a sentence that contains a reference to either a specific time point or a time interval. Determine if it is a time interval mentioned in the sentence, e.g. 'for 1 hour' 'for 20 mins' 'half an hour' '2 hours' are time intervals. Simply reply 'yes' or 'no' without further explanation."
 #     sys_msg = create_system_msg(prompt_content)
 
@@ -112,27 +145,28 @@
 #             if ans == "False":
 #                 print("correct, false")
 #             else:
 #                 print("error with the instruction", instruction)
 
 
 if __name__ == "__main__":
+    # list_of_instructions = [
+    #     "Ride bike tomorrow at 8pm for 1 hour",
+    #     "Write thesis for 2 hours at 10pm",
+    #     "meeting with lina next wednesday at 11:30",
+    #     "Learn python for 2 hours in three weeks at 7pm",
+    #     "Go to gym at 7pm",
+    #     "Meditation at 1am",
+    #     "A one hour meeting at 7",
+    # ]
 
-    list_of_instructions = [
-        "Ride bike tomorrow at 8pm for 1 hour",
-        "Write thesis for 2 hours at 10pm",
-        "meeting with lina next wednesday at 11:30",
-        "Learn python for 2 hours in three weeks at 7pm",
-        "Go to gym at 7pm",
-        "Meditation at 1am",
-        "A one hour meeting at 7",
-    ]
+    # answers = ["True", "True", "False", "True", "False", "False", "True"]
 
-    answers = ["True", "True", "False", "True", "False", "False", "True"]
+    # for instruction in list_of_instructions:
+    #     command = generate_command_with_gpt4(instruction)
 
-    for instruction in list_of_instructions:
-        command = generate_command_with_gpt4(instruction)
+    #     print(command)
 
-        print(command)
+    repeat_learn("Learn the MMK chapter 1")
 
     # print(generate_command_with_gpt4( "Learn python for 2 hours in three weeks at 7pm"))
     # print(generate_command_with_gpt4("meeting with lina next wednesday at 11:30"))
```

### Comparing `lumeny-0.1.2/lumeny/cli.py` & `lumeny-0.2.0/lumeny/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,48 +1,86 @@
 # cli.py
 import os
 import questionary as q
 import click
 from prompt_toolkit.lexers import PygmentsLexer
-from lumeny.utils import InputLexer
+from lumeny.utils import InputLexer, print_green
+
 # from lumen.tui import launch_tui
-from lumeny.calendar import generate_command_with_gpt4
+from lumeny.calendar import generate_command_with_gpt4, repeat_learn
 
 
 @click.group()
 def cli():
     pass
 
+
 @click.command()
 def add():
-    """Interactively add events to your calendar. 
-    """
+    """Interactively add events to your calendar."""
 
     def add_one_event() -> None:
-        request: str = q.text("What you will do (enter to abort): ", qmark="",
-                              lexer=PygmentsLexer(InputLexer)).ask()
+        request: str = q.text(
+            "What you will do (enter to abort): ",
+            qmark="",
+            lexer=PygmentsLexer(InputLexer),
+        ).ask()
 
         if request == "":
             return
-        
+
         command = generate_command_with_gpt4(request)
         if q.confirm(f"Execute: {command}", qmark="?").ask():
             try:
                 os.system(command)
                 # print in green: command executed
-                print(f"\033[1;32mEvent Added!\033[0m")
+                print_green("Event Added!")
             except Exception as e:
                 print(e)
                 print("Error executing command")
-    
-    while True:
-        add_one_event()
-        if not q.confirm("Add another event?", qmark="").ask():
-            break
-    
+
+        while True:
+            add_one_event()
+            if not q.confirm("Add another event?", qmark="").ask():
+                break
+
+        return
+
+
+@click.command()
+@click.option("-t", "--topic", type=str, help="Specify the topic.")
+@click.option(
+    "-r",
+    "--repeat_days",
+    type=int,
+    multiple=True,
+    default=(2, 5, 14, 30),
+    help="repeat this event in these days",
+)
+@click.option(
+    "-s",
+    "--start_date",
+    type=int,
+    default=0,
+    help="Specify a start date as an integer.",
+)
+def repeat(topic, repeat_days, start_date):
+
+    format_str = "%d-%m-%Y"
+
+    command: str = repeat_learn(topic, repeat_days, start_date)
+    if q.confirm(f"Execute: {command}", qmark="?").ask():
+        try:
+            os.system(command)
+            print_green("Event Added!")
+
+        except Exception as e:
+            print(e)
+            print("Error executing command")
+
 
 @click.command()
 @click.argument("input", nargs=-1)
 def will(input):
     """
     Add events to the calendar. Accept any number of arguments and treat them as one string.
     """
@@ -70,10 +108,11 @@
 
     # launch_tui()
 
 
 cli.add_command(will)
 cli.add_command(show)
 cli.add_command(add)
+cli.add_command(repeat)
 
 if __name__ == "__main__":
     cli()
```

### Comparing `lumeny-0.1.2/lumeny/tui.py` & `lumeny-0.2.0/lumeny/tui.py`

 * *Files identical despite different names*

### Comparing `lumeny-0.1.2/pyproject.toml` & `lumeny-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lumeny"
-version = "0.1.2"
+version = "0.2.0"
 description = "A cli and tui based personal management app for Lumen Young"
 authors = ["Lumen Young <pip@lumeny.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 caldav = "^1.2.1"
```

### Comparing `lumeny-0.1.2/PKG-INFO` & `lumeny-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumeny
-Version: 0.1.2
+Version: 0.2.0
 Summary: A cli and tui based personal management app for Lumen Young
 Author: Lumen Young
 Author-email: pip@lumeny.io
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

