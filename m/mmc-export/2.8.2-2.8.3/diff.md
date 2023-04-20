# Comparing `tmp/mmc_export-2.8.2.tar.gz` & `tmp/mmc_export-2.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmc_export-2.8.2.tar", max compression
+gzip compressed data, was "mmc_export-2.8.3.tar", max compression
```

## Comparing `mmc_export-2.8.2.tar` & `mmc_export-2.8.3.tar`

### file list

```diff
@@ -1,27 +1,16 @@
--rw-r--r--   0        0        0     1066 2022-05-10 23:10:38.982236 mmc_export-2.8.2/LICENSE
--rw-r--r--   0        0        0     5545 2022-11-03 07:21:41.102451 mmc_export-2.8.2/README.md
--rw-r--r--   0        0        0     2825 2022-07-09 04:03:11.721431 mmc_export-2.8.2/mmc_export/Formats/__pycache__/curseforge.cpython-310.pyc
--rw-r--r--   0        0        0     5233 2022-11-20 23:46:59.078504 mmc_export-2.8.2/mmc_export/Formats/__pycache__/curseforge.cpython-311.pyc
--rw-r--r--   0        0        0     3872 2022-11-06 06:15:07.099438 mmc_export-2.8.2/mmc_export/Formats/__pycache__/modrinth.cpython-310.pyc
--rw-r--r--   0        0        0     7113 2022-11-20 23:46:59.038505 mmc_export-2.8.2/mmc_export/Formats/__pycache__/modrinth.cpython-311.pyc
--rw-r--r--   0        0        0     3743 2022-09-13 09:10:41.682987 mmc_export-2.8.2/mmc_export/Formats/__pycache__/packwiz.cpython-310.pyc
--rw-r--r--   0        0        0     2798 2022-07-09 04:02:46.858433 mmc_export-2.8.2/mmc_export/Formats/curseforge.py
--rw-r--r--   0        0        0     4094 2022-11-06 06:15:03.483584 mmc_export-2.8.2/mmc_export/Formats/modrinth.py
--rw-r--r--   0        0        0     4966 2022-09-13 09:13:46.482260 mmc_export-2.8.2/mmc_export/Formats/packwiz.py
--rw-r--r--   0        0        0    14391 2022-11-06 06:14:36.306681 mmc_export-2.8.2/mmc_export/Helpers/__pycache__/resourceAPI.cpython-310.pyc
--rw-r--r--   0        0        0    32927 2023-02-18 11:19:41.053374 mmc_export-2.8.2/mmc_export/Helpers/__pycache__/resourceAPI.cpython-311.pyc
--rw-r--r--   0        0        0     3660 2022-09-02 09:46:55.851465 mmc_export-2.8.2/mmc_export/Helpers/__pycache__/structures.cpython-310.pyc
--rw-r--r--   0        0        0     6219 2022-11-20 23:45:36.224296 mmc_export-2.8.2/mmc_export/Helpers/__pycache__/structures.cpython-311.pyc
--rw-r--r--   0        0        0    10793 2022-09-23 18:04:23.027960 mmc_export-2.8.2/mmc_export/Helpers/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0    22205 2023-01-23 22:02:48.082383 mmc_export-2.8.2/mmc_export/Helpers/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0    15932 2023-02-18 11:19:04.128890 mmc_export-2.8.2/mmc_export/Helpers/resourceAPI.py
--rw-r--r--   0        0        0     2396 2022-08-24 18:47:04.717746 mmc_export-2.8.2/mmc_export/Helpers/structures.py
--rw-r--r--   0        0        0    11683 2022-11-22 02:40:45.069285 mmc_export-2.8.2/mmc_export/Helpers/utils.py
--rw-r--r--   0        0        0       63 2022-07-09 03:47:00.282736 mmc_export-2.8.2/mmc_export/__init__.py
--rw-r--r--   0        0        0       61 2022-05-10 23:10:38.982236 mmc_export-2.8.2/mmc_export/__main__.py
--rw-r--r--   0        0        0      648 2022-09-12 09:19:59.859818 mmc_export-2.8.2/mmc_export/config.py
--rw-r--r--   0        0        0     2674 2023-02-12 11:44:09.333476 mmc_export-2.8.2/mmc_export/main.py
--rw-r--r--   0        0        0     3069 2023-01-23 19:06:35.936606 mmc_export-2.8.2/mmc_export/parser.py
--rw-r--r--   0        0        0      820 2023-02-18 11:03:16.903701 mmc_export-2.8.2/pyproject.toml
--rw-r--r--   0        0        0     6793 1970-01-01 00:00:00.000000 mmc_export-2.8.2/setup.py
--rw-r--r--   0        0        0     6514 1970-01-01 00:00:00.000000 mmc_export-2.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-05-10 23:10:38.982236 mmc_export-2.8.3/LICENSE
+-rw-r--r--   0        0        0     5545 2022-11-03 07:21:41.102451 mmc_export-2.8.3/README.md
+-rw-r--r--   0        0        0     2816 2023-04-20 09:34:24.580816 mmc_export-2.8.3/mmc_export/Formats/curseforge.py
+-rw-r--r--   0        0        0     4094 2022-11-06 06:15:03.483584 mmc_export-2.8.3/mmc_export/Formats/modrinth.py
+-rw-r--r--   0        0        0     4984 2023-04-20 09:34:42.212054 mmc_export-2.8.3/mmc_export/Formats/packwiz.py
+-rw-r--r--   0        0        0    15932 2023-04-20 09:36:54.618375 mmc_export-2.8.3/mmc_export/Helpers/resourceAPI.py
+-rw-r--r--   0        0        0     2396 2022-08-24 18:47:04.717746 mmc_export-2.8.3/mmc_export/Helpers/structures.py
+-rw-r--r--   0        0        0    11683 2022-11-22 02:40:45.069285 mmc_export-2.8.3/mmc_export/Helpers/utils.py
+-rw-r--r--   0        0        0       63 2022-07-09 03:47:00.282736 mmc_export-2.8.3/mmc_export/__init__.py
+-rw-r--r--   0        0        0       61 2022-05-10 23:10:38.982236 mmc_export-2.8.3/mmc_export/__main__.py
+-rw-r--r--   0        0        0      648 2022-09-12 09:19:59.859818 mmc_export-2.8.3/mmc_export/config.py
+-rw-r--r--   0        0        0     2788 2023-04-20 09:36:05.218485 mmc_export-2.8.3/mmc_export/main.py
+-rw-r--r--   0        0        0     3069 2023-01-23 19:06:35.936606 mmc_export-2.8.3/mmc_export/parser.py
+-rw-r--r--   0        0        0      844 2023-04-20 09:36:39.651014 mmc_export-2.8.3/pyproject.toml
+-rw-r--r--   0        0        0     6834 1970-01-01 00:00:00.000000 mmc_export-2.8.3/setup.py
+-rw-r--r--   0        0        0     6569 1970-01-01 00:00:00.000000 mmc_export-2.8.3/PKG-INFO
```

### Comparing `mmc_export-2.8.2/LICENSE` & `mmc_export-2.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mmc_export-2.8.2/README.md` & `mmc_export-2.8.3/README.md`

 * *Files identical despite different names*

### Comparing `mmc_export-2.8.2/mmc_export/Formats/curseforge.py` & `mmc_export-2.8.3/mmc_export/Formats/curseforge.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         for override in self.intermediate.overrides:
             self.add_override(override)
 
         from json import dump as write_json
         with open(self.temp_dir / "manifest.json", 'w') as file:
             write_json(self.manifest, file, indent=4)
 
-        with open(self.temp_dir / "modlist.html", 'w') as file:
+        with open(self.temp_dir / "modlist.html", 'w', encoding="utf-8") as file:
             self.modlist.insert(0, "<ul>\n")
             self.modlist.append("</ul>\n")
             file.writelines(self.modlist)
 
         from shutil import make_archive
         name = get_name_from_scheme("CF", "CurseForge", self.intermediate)
         make_archive((self.modpack_path / name).as_posix(), 'zip', self.temp_dir, '.')
```

### Comparing `mmc_export-2.8.2/mmc_export/Formats/modrinth.py` & `mmc_export-2.8.3/mmc_export/Formats/modrinth.py`

 * *Files identical despite different names*

### Comparing `mmc_export-2.8.2/mmc_export/Formats/packwiz.py` & `mmc_export-2.8.3/mmc_export/Formats/packwiz.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
         from werkzeug.utils import secure_filename
         if not slug: slug = secure_filename(resource.name)
 
         toml_path = self.temp_dir / resource.file.relativePath / (slug + ".pw.toml")
         toml_path.parent.mkdir(parents=True, exist_ok=True)
 
-        with open(toml_path, "w") as file:
+        with open(toml_path, "w", encoding="utf-8") as file:
 
             if not data['update']: del data['update']
             toml_data = encode_toml(data)
 
             with suppress(ValueError):
                 index = toml_data.index("[update")
                 toml_data = toml_data[:index] + "[update]\n" + toml_data[index:]
```

### Comparing `mmc_export-2.8.2/mmc_export/Helpers/resourceAPI.py` & `mmc_export-2.8.3/mmc_export/Helpers/resourceAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     excluded_providers: list[str]
 
     def __init__(self, session: CachedSession, intermediate: Intermediate) -> None:
 
         self.session = session
         self.intermediate = intermediate
 
-        self.session.headers["User-Agent"] = "RozeFound/mmc-export/2.8.2"
+        self.session.headers["User-Agent"] = "RozeFound/mmc-export/2.8.3"
         self.session.headers["X-Api-Key"] = config.CURSEFORGE_API_TOKEN
         self.session.headers["Content-Type"] = "application/json"
         self.session.headers["Accept"] = "application/json"
 
         self.github = "https://api.github.com"
         self.modrinth = "https://api.modrinth.com/v2"
         self.curseforge = "https://api.curseforge.com/v1"
```

### Comparing `mmc_export-2.8.2/mmc_export/Helpers/structures.py` & `mmc_export-2.8.3/mmc_export/Helpers/structures.py`

 * *Files identical despite different names*

### Comparing `mmc_export-2.8.2/mmc_export/Helpers/utils.py` & `mmc_export-2.8.3/mmc_export/Helpers/utils.py`

 * *Files identical despite different names*

### Comparing `mmc_export-2.8.2/mmc_export/config.py` & `mmc_export-2.8.3/mmc_export/config.py`

 * *Files identical despite different names*

### Comparing `mmc_export-2.8.2/mmc_export/main.py` & `mmc_export-2.8.3/mmc_export/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from importlib import import_module
 from json import dump as write_json
 from shutil import rmtree
 
+import ssl, certifi
 from aiohttp import TCPConnector
 from aiohttp_client_cache.backends.filesystem import FileBackend
 from aiohttp_client_cache.session import CachedSession
 
 from .Helpers.resourceAPI import ResourceAPI
 from .Helpers.utils import (JsonEncoder, add_github_token, parse_args,
                             parse_config, resolve_conflicts)
@@ -16,16 +17,17 @@
 async def program():
 
     args = parse_args()
 
     ResourceAPI.modrinth_search_type = args.modrinth_search
     ResourceAPI.excluded_providers = args.excluded_providers
 
+    ssl_context = ssl.create_default_context(cafile=certifi.where())
     cache = FileBackend("mmc-export", use_temp=True, urls_expire_after={'*.jar': -1}, allowed_methods=("GET", "POST", "HEAD"))
-    async with CachedSession(cache=cache, connector=TCPConnector(limit=0)) as session: 
+    async with CachedSession(cache=cache, connector=TCPConnector(limit=0, ssl_context=ssl_context)) as session: 
         if args.skip_cache: session.cache.disabled = True # type: ignore
 
         match args.cmd:
             case "gh-login": await add_github_token(); return
             case "gh-logout": 
                 url = f"https://github.com/settings/connections/applications/{config.OAUTH_GITHUB_CLIENT_ID}"
                 print(f"You can revoke your access token by the following link: \n{url}"); return
```

### Comparing `mmc_export-2.8.2/mmc_export/parser.py` & `mmc_export-2.8.3/mmc_export/parser.py`

 * *Files identical despite different names*

### Comparing `mmc_export-2.8.2/pyproject.toml` & `mmc_export-2.8.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mmc-export"
-version = "2.8.2"
+version = "2.8.3"
 description = "Export MMC modpack to other modpack formats"
 authors = ["RozeFound"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/RozeFound/mmc-export"
 
 keywords = [
@@ -22,19 +22,20 @@
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = "^3.8.3"
 aiohttp-client-cache = {extras = ["filesystem"], version = "^0.7.3"}
 murmurhash2 = "^0.2.10"
 tenacity = "^8.1.0"
 Werkzeug = "^2.2.2"
-cryptography = "38.0.3"
+cryptography = "^39.0.2"
 xxhash = "^3.1.0"
 gql-query-builder = "^0.1.7"
 keyring = "^23.11.0"
 tomli-w = "^1.0.0"
+certifi = "^2022.12.7"
 
 [tool.poetry.scripts]
 mmc-export = "mmc_export:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mmc_export-2.8.2/setup.py` & `mmc_export-2.8.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Werkzeug>=2.2.2,<3.0.0',
  'aiohttp-client-cache[filesystem]>=0.7.3,<0.8.0',
  'aiohttp>=3.8.3,<4.0.0',
- 'cryptography==38.0.3',
+ 'certifi>=2022.12.7,<2023.0.0',
+ 'cryptography>=39.0.2,<40.0.0',
  'gql-query-builder>=0.1.7,<0.2.0',
  'keyring>=23.11.0,<24.0.0',
  'murmurhash2>=0.2.10,<0.3.0',
  'tenacity>=8.1.0,<9.0.0',
  'tomli-w>=1.0.0,<2.0.0',
  'xxhash>=3.1.0,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['mmc-export = mmc_export:main']}
 
 setup_kwargs = {
     'name': 'mmc-export',
-    'version': '2.8.2',
+    'version': '2.8.3',
     'description': 'Export MMC modpack to other modpack formats',
     'long_description': '# MultiMC advanced exporter\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/mmc-export)](https://www.python.org)\n[![PyPI version](https://img.shields.io/pypi/v/mmc-export?label=mmc-export&color=%2347a637)](https://pypi.org/project/mmc-export)\n[![PyPI downloads](https://img.shields.io/pypi/dm/mmc-export?color=%23894bbf)](https://pypistats.org/packages/mmc-export)\n[![GitHub license](https://img.shields.io/github/license/RozeFound/mmc-export)](/LICENSE)\n\nSince MultiMC export features are very limited, I created a script that solves this problem, with this script you can export MultiMC pack to any popular format (e.g. curseforge, modrinth, packwiz). MultiMC forks which didn\'t changed export format much also supported.\n\n# Features\n\n- Support conversion to:\n    - CurseForge\n    - Modrinth\n    - packwiz\n- Detects downloadable resourcepacks and shaders\n- Supports github parsing[¹](#github-rate-limits)\n- Loose modrinth search\n- User friendly toml config\n- Multiple output formats at once\n\n---\n### GitHub rate limits\n\nGitHub has limited requests per hour (up to 60), this means that if you have more than 60 mods, the rest will be excluded from github search. \nIf you authenticate with GitHub using `mmc-export gh-login`, the limit will be removed and requests will be faster. You can always log out with `mmc-export gh-logout`.\n\nIf you don\'t want to use github search by some reason, you can specify `--exclude-providers GitHub` as argument.\n\n# How to Use\n```\nmmc-export -i modpack.zip -c config.toml -f Modrinth packwiz -o converted_modpacks\n```\nIt\'s recommended to fill config at least with basic info like name and version, some launchers can fail import if these values are empty.\n\n## Sub-commands\n\n`gh-login` - to authrize GitHub \\\n`gh-logout` - to get info how to deauthorize GitHub \n\n`purge-cache` - to purge cache. Available arguments:\n```\n--web: to delete requests cache and downloaded mods\n--files: to delete hashes cache\n--all: equivalent to --web --files, deletes all cache (default)\n```\n\n## Syntax\n```\nmmc-export [sub-command] [-h] [-c CONFIG] -i INPUT -f FORMAT [-o OUTPUT] [-v VERSION] [--modrinth-search SEARCH_TYPE] [--exclude-providers PROVIDERS]\n```\n\n### Explanation\n```\n-h --help: prints help\n-i --input: path to modpack, must be zip file exported from MultiMC.\n-c --config: path to config, used to fill the gaps like description or lost mods.\n-f --format: output formats, must be separated by spaces.\n-o --output: directory where converted zip files will be stored.\n-v --version: specify modpack version, will be overriden by config\'s value if exists\n--modrinth-search: modrinth search accuracy\n--exclude-providers: providers you wish to exclude from search\n--provider-priority: providers priority used for packwiz\n--skip-cache: don\'t use web cache in this run\n--scheme: output filename formatting scheme, more info in #scheme-formatting\n```\n> All paths can be relative to current working directory or absolute.\n\n`--format` options (case-sensitive): \n- `CurseForge`\n- `Modrinth`\n- `packwiz`\n- `Intermediate` (only for debugging, may contain sensitive data like username)\n\n`--exclude-providers` options (case-sensitive): \n- `CurseForge`\n- `Modrinth`\n- `GitHub`\n\n`--provider-priority` options (case-sensitive): \n- `CurseForge`\n- `Modrinth`\n- `Other` or `GitHub`\n\n`--modrinth-search` options:\n- `exact` - by hash (default)\n- `accurate` - by hash or slug\n- `loose` - by hash, slug or long name\n\nThe example for the optional `--config` file [can be found here](example_config.toml). \n\nFor example, if the script says\n\n> No config entry found for resource: ModName\n\nThen you should add **one** of the following entries to the end of the config:\n\n#### Specify source URL\n```\n[[Resource]]\nname = "ModName"\nfilename = "the_name_of_the.jar" \nurl = "https://cdn.modrinth.com/data/abcdefg/versions/1.0.0/the_name_of_the.jar"\n```\n#### Hide the warning\n```\n[[Resource]]\nname = "ModName"\nfilename = "the_name_of_the.jar" \naction = "ignore"\n```\n#### Explicitly move to overrides\n```\n[[Resource]]\nname = "ModName"\nfilename = "the_name_of_the.jar" \naction = "override"\n```\n#### Delete the file altogether\n```\n[[Resource]]\nname = "ModName"\nfilename = "the_name_of_the.jar" \naction = "remove"\n```\n#### Make the mod optional\nAppend `optional = true` to any of above\n\n#### Delete any file\nThis can be defined to delete any file that isn\'t downloadable from CurseForge/Modrinth, e.g. mod config or metadata file.\n```\n[[File]]\nname = "Useless file.txt"\naction = "remove"\n```\n\n> Also specifying both name and filename is optional but recommended, you can always leave only one of these\n\n## Scheme Formatting\n\nMust be used as `--scheme "{keyword}_Literally any text"` without file extension, follows python\'s [format string syntax](https://docs.python.org/3/library/string.html#format-string-syntax)\n\n#### Available keywords: \n- `abbr` - provider abbreviation, usually 2 capitals, e.g. `MR`, `CF`\n- `format` - full format name, e.g. `CurseForge`, `Packwiz`\n- `name` same as `pack.name` - modpack name\n- `version` same as `pack.version` - modpack version\n- `pack` - pointer to [Intermediate](mmc_export/Helpers/structures.py#L50-L66) structure\n\nDefault scheme is as simple as `{abbr}_{name}`\n\n***Caution: if you don\'t use any format specifc keywords, output files will overwrite the same file several times***, can be ignored if you output to only one format.\nAlso, be aware of your filesystem limitations, unsupported characters may lead to an error, or inaccesible file.\n\n# How to Install / Update\n```\npip install -U mmc-export\n```\n',
     'author': 'RozeFound',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/RozeFound/mmc-export',
```

### Comparing `mmc_export-2.8.2/PKG-INFO` & `mmc_export-2.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: mmc-export
-Version: 2.8.2
+Version: 2.8.3
 Summary: Export MMC modpack to other modpack formats
 Home-page: https://github.com/RozeFound/mmc-export
 License: MIT
 Keywords: minecraft,mods,modpack,converter,MultiMC
 Author: RozeFound
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Werkzeug (>=2.2.2,<3.0.0)
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: aiohttp-client-cache[filesystem] (>=0.7.3,<0.8.0)
-Requires-Dist: cryptography (==38.0.3)
+Requires-Dist: certifi (>=2022.12.7,<2023.0.0)
+Requires-Dist: cryptography (>=39.0.2,<40.0.0)
 Requires-Dist: gql-query-builder (>=0.1.7,<0.2.0)
 Requires-Dist: keyring (>=23.11.0,<24.0.0)
 Requires-Dist: murmurhash2 (>=0.2.10,<0.3.0)
 Requires-Dist: tenacity (>=8.1.0,<9.0.0)
 Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
 Requires-Dist: xxhash (>=3.1.0,<4.0.0)
 Project-URL: Repository, https://github.com/RozeFound/mmc-export
```

