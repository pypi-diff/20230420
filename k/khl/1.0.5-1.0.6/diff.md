# Comparing `tmp/khl-1.0.5.tar.gz` & `tmp/khl-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khl-1.0.5.tar", max compression
+gzip compressed data, was "khl-1.0.6.tar", max compression
```

## Comparing `khl-1.0.5.tar` & `khl-1.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2023-03-05 17:17:58.027493 khl-1.0.5/LICENSE
--rw-r--r--   0        0        0     5528 2023-03-05 17:17:58.027493 khl-1.0.5/README.md
--rw-r--r--   0        0        0     2297 2023-03-10 18:06:18.347868 khl-1.0.5/khl/__init__.py
--rw-r--r--   0        0        0     8829 2023-03-10 16:38:07.463209 khl-1.0.5/khl/preprocess.py
--rw-r--r--   0        0        0     2426 2023-03-10 17:49:51.106914 khl-1.0.5/khl/stop_words.py
--rw-r--r--   0        0        0     3274 2023-03-10 16:26:00.431309 khl-1.0.5/khl/teams_orgs.py
--rw-r--r--   0        0        0    29283 2023-03-10 18:03:30.155086 khl-1.0.5/khl/utils.py
--rw-r--r--   0        0        0     8346 2023-03-05 17:17:58.031493 khl-1.0.5/khl/wrong_lemmas.py
--rw-r--r--   0        0        0     1557 2023-03-10 18:06:18.347868 khl-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     6469 1970-01-01 00:00:00.000000 khl-1.0.5/setup.py
--rw-r--r--   0        0        0     6251 1970-01-01 00:00:00.000000 khl-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-03-05 17:17:58.027493 khl-1.0.6/LICENSE
+-rw-r--r--   0        0        0     5528 2023-03-05 17:17:58.027493 khl-1.0.6/README.md
+-rw-r--r--   0        0        0     2297 2023-04-20 19:36:25.798785 khl-1.0.6/khl/__init__.py
+-rw-r--r--   0        0        0     8829 2023-03-10 16:38:07.463209 khl-1.0.6/khl/preprocess.py
+-rw-r--r--   0        0        0     2426 2023-03-10 17:49:51.106914 khl-1.0.6/khl/stop_words.py
+-rw-r--r--   0        0        0     3274 2023-03-10 16:26:00.431309 khl-1.0.6/khl/teams_orgs.py
+-rw-r--r--   0        0        0    30765 2023-04-20 19:34:54.754745 khl-1.0.6/khl/utils.py
+-rw-r--r--   0        0        0     8346 2023-03-05 17:17:58.031493 khl-1.0.6/khl/wrong_lemmas.py
+-rw-r--r--   0        0        0     1589 2023-04-20 19:36:32.994513 khl-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     6469 1970-01-01 00:00:00.000000 khl-1.0.6/setup.py
+-rw-r--r--   0        0        0     6251 1970-01-01 00:00:00.000000 khl-1.0.6/PKG-INFO
```

### Comparing `khl-1.0.5/LICENSE` & `khl-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `khl-1.0.5/README.md` & `khl-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `khl-1.0.5/khl/__init__.py` & `khl-1.0.6/khl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Подготовка русскоязычных текстов хоккейных новостей для обучения нейронных сетей."""
 
-__version__ = "1.0.5"
+__version__ = "1.0.6"
 
 from typing import Dict, List, Optional
 
 from khl import preprocess, utils
 from khl.stop_words import stop_words
```

### Comparing `khl-1.0.5/khl/preprocess.py` & `khl-1.0.6/khl/preprocess.py`

 * *Files identical despite different names*

### Comparing `khl-1.0.5/khl/stop_words.py` & `khl-1.0.6/khl/stop_words.py`

 * *Files identical despite different names*

### Comparing `khl-1.0.5/khl/teams_orgs.py` & `khl-1.0.6/khl/teams_orgs.py`

 * *Files identical despite different names*

### Comparing `khl-1.0.5/khl/utils.py` & `khl-1.0.6/khl/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,23 +44,14 @@
         .replace("ё", "ё")
         .replace("…", "...")
     )
     text = re.sub(r"[^ А-Яа-яЁёA-Za-z0-9',.\[\]{}()/=+%№#@!?;:-]", " ", text)
     return merge_spaces(text).strip()
 
 
-def _find_ners(text: str) -> List[Span]:
-    """Нахождение именованных сущностей."""
-    doc = Doc(text)
-    doc.segment(segmenter)
-    doc.tag_ner(ner_tagger)
-    ners: List[Span] = doc.ner.spans
-    return ners
-
-
 def _fix_quotes(text: str) -> str:
     """Исправление дублирующихся ординарных кавычек "''" -> "'"."""
     return re.sub(r"\'{2,}", "'", text)
 
 
 def _surround_with_quotes(match_object: re.Match) -> str:  # type: ignore
     """Окружение кавычками."""
@@ -79,14 +70,34 @@
 
 
 def delete_quotes_around_orgs(text: str) -> str:
     """Удаление кавычек вокруг org."""
     return re.sub(r"\'?org\'?", "org", text)
 
 
+def fix_bug_5(func: Callable[[str], str]) -> Callable[[str], str]:
+    """
+    Natasha не всегда правильно распознает названия организаций.
+
+    Например,
+    replace_ners("Сегодня в КХЛе пройдет матч") -> "Сегодня в loc пройдет матч".
+    Данный декоратор - попытка исправить данное поведение,
+    путем оборачивания заданных названий команд/организаций в кавычки
+    перед тем как распознавать ner'ы, а потом удаление кавычек вокруг org.
+    """
+
+    def wrapper(text: str) -> str:
+        """Функция wrapper."""
+        text = surround_concrete_orgs_with_quotes(text)
+        text = func(text)
+        return delete_quotes_around_orgs(text)
+
+    return wrapper
+
+
 def fix_bug_14(func: Callable[[str], str]) -> Callable[[str], str]:
     """
     Почему-то natasha ошибается на коротких названиях новостей.
 
     Например, replace_ners("Уральская проверка") -> "org".
     Данный декоратор - попытка исправить данное поведение,
     путем добавления в конец текста восклицательного знака
@@ -99,31 +110,40 @@
         text += "!"
         text = func(text)
         return re.sub(r"\!$", "", text)
 
     return wrapper
 
 
+def _find_ners(text: str) -> List[Span]:
+    """Нахождение именованных сущностей."""
+    doc = Doc(text)
+    doc.segment(segmenter)
+    doc.tag_ner(ner_tagger)
+    ners: List[Span] = doc.ner.spans
+    return ners
+
+
 @fix_bug_14
+@fix_bug_5
 def replace_ners(text: str) -> str:
     """
     Заменяет именованные сущности на их тип.
 
     'Иванов Иван'  -> 'per'
     'Магнитогорск' -> 'loc'
     'Ак Барс'      -> 'org'
     """
-    text = surround_concrete_orgs_with_quotes(text)
     ners_spans = _find_ners(text)
     for ner_span in reversed(ners_spans):
         text = text[: ner_span.start] + ner_span.type.lower() + text[ner_span.stop :]
     text = replace_concrete_orgs(text)
     text = handwritten_replace_orgs(text)
     text = handwritten_replace_per(text)
-    return delete_quotes_around_orgs(text)
+    return text
 
 
 def _find_dates(text: str) -> List[NatashaMatch]:
     """Нахождение дат."""
     dates_extractor = DatesExtractor(morph_vocab)
     return [match_ for match_ in dates_extractor(text)]
 
@@ -200,14 +220,27 @@
 def replace_dash_between_ners(text: str) -> str:
     """Замена тире между ner'ами на пробел."""
     pattern = r"(?:per|org|loc|date|pen)(?:\s*-+\s*(?:per|org|loc|date|pen))+"
     result = re.sub(pattern, _replace_dash_with_space, text)
     return result
 
 
+def _delete_with_and(match_object: re.Match) -> str:  # type: ignore
+    """Удаление предлога 'с' и союза 'и'."""
+    text: str = match_object.group(0)
+    pattern = r"\s+(?:с|со|и)\s+"
+    return re.sub(pattern, " ", text, flags=re.IGNORECASE)
+
+
+def fix_ner_with_and_ner(text: str) -> str:
+    """Удаление предлога 'с' и союза 'и', которые располагатся между ner'ами."""
+    pattern = r"(?:per|org|loc|date)(?:\s+(?i:с|со|и)\s+(?:per|org|loc|date))+"
+    return re.sub(pattern, _delete_with_and, text)
+
+
 def merge_spaces(text: str) -> str:
     """'Схлопывает' все соседние пробельные символы в один пробел."""
     return re.sub(r"\s{2,}", " ", text)
 
 
 def leave_only_significant_symbols(text: str) -> str:
     """
@@ -782,14 +815,15 @@
     text = delete_play_format(text)
     text = replace_exclamation_mark_with_dot(text)
     text = leave_only_significant_symbols(text)
     text = fix_org_loc(text)
     text = merge_spaces(text)
     text = merge_dashes(text)
     text = replace_dash_between_ners(text)
+    text = fix_ner_with_and_ner(text)
     text = delete_beginning_ending_dashes_in_words(text)
     text = fix_dots(text)
     text = fix_question_marks(text)
     text = fix_question_dot(text)
     text = fix_dot_question(text)
     text = delete_ending_colon_dash(text)
     text = fix_colons(text)
```

### Comparing `khl-1.0.5/khl/wrong_lemmas.py` & `khl-1.0.6/khl/wrong_lemmas.py`

 * *Files identical despite different names*

### Comparing `khl-1.0.5/pyproject.toml` & `khl-1.0.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "khl"
-version = "1.0.5"
+version = "1.0.6"
 description = "Preparing russian hockey news for machine learning"
 readme = "README.md"
 license = "MIT"
 authors = ["Rishat Fayzullin <nilluziaf@gmail.com>"]
 repository = "https://github.com/Rishat-F/khl"
 keywords = ["khl", "news", "nlp", "preprocessing", "ml"]
 
@@ -65,8 +65,9 @@
     "bug_4: test for bug #4",
     "bug_5: test for bug #5",
     "bug_6: test for bug #6",
     "bug_14: test for bug #14",
     "bug_17: test for bug #17",
     "bug_20: test for bug #20",
     "bug_21: test for bug #21",
+    "bug_26: test for bug #26",
 ]
```

### Comparing `khl-1.0.5/setup.py` & `khl-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['natasha==1.4.0']
 
 setup_kwargs = {
     'name': 'khl',
-    'version': '1.0.5',
+    'version': '1.0.6',
     'description': 'Preparing russian hockey news for machine learning',
     'long_description': '![Khl Logo](https://raw.githubusercontent.com/Rishat-F/khl/master/data/logo.png)\n\n<h1 align="center">No Water - Ice Only</h1>\n\nPreparing russian hockey news for machine learning.\n\n**Unify -> Simplify -> Preprocess** text and feed your neural model.\n\n## Installation\n\n*Khl* is available on PyPI:\n\n```console\n$ pip install khl\n```\nIt requires Python 3.8+ to run.\n\n## Usage\n\nTo get started right away with basic usage:\n\n```python\nfrom khl import text_to_codes\n\nlemmas_coder = {\n    \'\': 0,     # placeholder\n    \'???\': 1,  # unknown\n    \'.\': 2,\n    \'и\': 3,\n    \'в\': 4,\n    \'-\': 5,\n    \':\': 6,\n    \'матч\': 7,\n    \'за\': 8,\n    \'забить\': 9,\n    \'гол\': 10,\n    \'per\': 11,   # person entity\n    \'org\': 12,   # organization entity\n    \'loc\': 13,   # location entity\n    \'date\': 14,  # date entity\n    \'против\': 15,\n    \'год\': 16,\n    \'pers\': 17,  # few persons entity\n    \'orgs\': 18,  # few organizations entity\n    \'свой\': 19\n}\n\ntext = """\n    1 апреля 2023 года в Москве в матче ⅛ финала против „Спартака” Иван Иванов забил свой 100—й гол за карьеру.\n    «Динамо Мск» - «Спартак» 2:1 ОТ (1:0 0:1 0:0 1:0) Голы забили: Иванов, Петров и Сидоров.\n"""\n\ncodes = text_to_codes(\n    text=text,\n    lemmas_coder=lemmas_coder,\n    stop_words_=["в", "за", "и", "свой"],  # stop words to drop\n    replace_ners_=True,                    # replace named entities ("Иван Иванов" -> "per", "Спартак" -> "org", "Москва" -> "loc")\n    replace_dates_=True,                   # replace dates ("1 апреля 2023 года" -> "date")\n    replace_penalties_=True,               # replace penalties ("5+20" -> "pen")\n    exclude_unknown=True,                  # drop lemma that not presented in lemmas_coder\n    max_len=20,                            # get sequence of codes of length 20\n)\n# codes = [0, 0, 0, 0, 0, 14, 13, 7, 15, 12, 11, 9, 10, 2, 18, 10, 9, 6, 17, 2]\n```\n\n```text_to_codes``` is a very high level function. What\'s happens under hood see in [Lower level usage](#lower-level-usage).\n\n## What is `lemmas_coder`?\n`lemmas_coder` is just a dictionary where each lemma is represented with unique integer code.\nNote that first two elements are reserved for *placeholder* and *unknown* elements.\n\nIt is possible to get `lemmas_coder` from frequency dictionary file (see in [Get lemmas coder](#2-get-lemmas-coder)).\nFrequency dictionary file is a **json**-file with dictionary where key is lemma and value is how many times this lemma occurred in your whole dataset.\nPreferably it should be sorted in descending order of values.  \n`example_frequency_dictionary.json`:\n\n```json\n{\n  ".": 1000,\n  "и": 500,\n  "в": 400,\n  "-": 300,\n  ":": 300,\n  "матч": 290,\n  "за": 250,\n  "забить": 240,\n  "гол": 230,\n  "per": 200,\n  "org": 150,\n  "loc": 150,\n  "date": 100,\n  "против": 90,\n  "год": 70,\n  "pers": 40,\n  "orgs": 30,\n  "свой": 20\n}\n```\n\nYou could make and use your own frequency dictionary or download [this dictionary](https://github.com/Rishat-F/khl/blob/master/data/frequency_dictionary.json) created by myself.\n\n## Lower level usage<a id="lower-level-usage"></a>\n\n#### 1. Make imports\n```python\nfrom khl import stop_words\nfrom khl import utils\nfrom khl import preprocess\n```\n\n#### 2. Get lemmas coder<a id="2-get-lemmas-coder"></a>\n```python\nlemmas_coder = preprocess.get_lemmas_coder("example_frequency_dictionary.json")\n```\n\n#### 3. Define text\n```python\ntext = """\n    1 апреля 2023 года в Москве в матче ⅛ финала против „Спартака” Иван Иванов забил свой 100—й гол за карьеру.\n    «Динамо Мск» - «Спартак» 2:1 ОТ (1:0 0:1 0:0 1:0) Голы забили: Иванов, Петров и Сидоров.\n"""\n```\n\n#### 4. Unify\n```python\nunified_text = utils.unify_text(text)\n# "1 апреля 2023 года в Москве в матче 1/8 финала против \'Спартака\' Иван Иванов забил свой 100-й гол за карьеру. \'Динамо Мск\' - \'Спартак\' 2:1 ОТ (1:0 0:1 0:0 1:0) Голы забили: Иванов, Петров и Сидоров."\n```\n\n#### 5. Simplify\n```python\nsimplified_text = utils.simplify_text(\n    text=unified_text,\n    replace_ners_=True,\n    replace_dates_=True,\n    replace_penalties_=True,\n)\n# \'date в loc в матче финала против org per забил свой гол за карьеру. org org Голы забили: per per и per.\'\n```\n\n#### 6. Lemmatize\n```python\nlemmas = preprocess.lemmatize(text=simplified_text, stop_words_=stop_words)\n# [\'date\', \'loc\', \'матч\', \'финал\', \'против\', \'org\', \'per\', \'забить\', \'гол\', \'карьера\', \'.\', \'orgs\', \'гол\', \'забить\', \':\', \'pers\', \'.\']\n```\n\n#### 7. Transform to codes\n```python\ncodes = preprocess.lemmas_to_codes(\n    lemmas=lemmas,\n    lemmas_coder=lemmas_coder,\n    exclude_unknown=True,\n    max_len=20,\n)\n# [0, 0, 0, 0, 0, 14, 13, 7, 15, 12, 11, 9, 10, 2, 18, 10, 9, 6, 17, 2]\n```\n\n#### 8. Transform to lemmas back (just to look which lemmas are presented in codes sequence)\n```python\nprint(\n    preprocess.codes_to_lemmas(codes=codes, lemmas_coder=lemmas_coder)\n)\n# [\'\', \'\', \'\', \'\', \'\', \'date\', \'loc\', \'матч\', \'против\', \'org\', \'per\', \'забить\', \'гол\', \'.\', \'orgs\', \'гол\', \'забить\', \':\', \'pers\', \'.\']\n```\n',
     'author': 'Rishat Fayzullin',
     'author_email': 'nilluziaf@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Rishat-F/khl',
```

### Comparing `khl-1.0.5/PKG-INFO` & `khl-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khl
-Version: 1.0.5
+Version: 1.0.6
 Summary: Preparing russian hockey news for machine learning
 Home-page: https://github.com/Rishat-F/khl
 License: MIT
 Keywords: khl,news,nlp,preprocessing,ml
 Author: Rishat Fayzullin
 Author-email: nilluziaf@gmail.com
 Requires-Python: >=3.8,<4.0
```

