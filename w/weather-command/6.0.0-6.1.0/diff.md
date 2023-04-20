# Comparing `tmp/weather_command-6.0.0.tar.gz` & `tmp/weather_command-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weather_command-6.0.0.tar", max compression
+gzip compressed data, was "weather_command-6.1.0.tar", max compression
```

## Comparing `weather_command-6.0.0.tar` & `weather_command-6.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1069 2023-04-15 18:13:07.333191 weather_command-6.0.0/LICENSE
--rw-r--r--   0        0        0     2849 2023-04-15 18:13:07.333191 weather_command-6.0.0/README.md
--rw-r--r--   0        0        0     1841 2023-04-15 18:13:07.333191 weather_command-6.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/__init__.py
--rw-r--r--   0        0        0       95 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/__main__.py
--rw-r--r--   0        0        0    18640 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/_builder.py
--rw-r--r--   0        0        0     5260 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/_cache.py
--rw-r--r--   0        0        0     5262 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/_config.py
--rw-r--r--   0        0        0     2546 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/_location.py
--rw-r--r--   0        0        0      473 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/_utils.py
--rw-r--r--   0        0        0     2921 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/_weather.py
--rw-r--r--   0        0        0      459 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/errors.py
--rw-r--r--   0        0        0     9000 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/main.py
--rw-r--r--   0        0        0        0 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/models/__init__.py
--rw-r--r--   0        0        0      133 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/models/location.py
--rw-r--r--   0        0        0     3053 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/models/weather.py
--rw-r--r--   0        0        0        0 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/py.typed
--rw-r--r--   0        0        0     2816 2023-04-15 18:13:07.337191 weather_command-6.0.0/weather_command/settings_commands.py
--rw-r--r--   0        0        0     3896 1970-01-01 00:00:00.000000 weather_command-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-20 09:12:21.835913 weather_command-6.1.0/LICENSE
+-rw-r--r--   0        0        0     3015 2023-04-20 09:12:21.835913 weather_command-6.1.0/README.md
+-rw-r--r--   0        0        0     1841 2023-04-20 09:12:21.839913 weather_command-6.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-20 09:12:21.839913 weather_command-6.1.0/weather_command/__init__.py
+-rw-r--r--   0        0        0       95 2023-04-20 09:12:21.839913 weather_command-6.1.0/weather_command/__main__.py
+-rw-r--r--   0        0        0    18650 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/_builder.py
+-rw-r--r--   0        0        0     5268 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/_cache.py
+-rw-r--r--   0        0        0     5262 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/_config.py
+-rw-r--r--   0        0        0     2667 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/_location.py
+-rw-r--r--   0        0        0      473 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/_utils.py
+-rw-r--r--   0        0        0     2849 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/_weather.py
+-rw-r--r--   0        0        0      459 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/errors.py
+-rw-r--r--   0        0        0     9084 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/main.py
+-rw-r--r--   0        0        0        0 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/models/__init__.py
+-rw-r--r--   0        0        0      133 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/models/location.py
+-rw-r--r--   0        0        0     3053 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/models/weather.py
+-rw-r--r--   0        0        0        0 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/py.typed
+-rw-r--r--   0        0        0     2816 2023-04-20 09:12:21.843913 weather_command-6.1.0/weather_command/settings_commands.py
+-rw-r--r--   0        0        0     4062 1970-01-01 00:00:00.000000 weather_command-6.1.0/PKG-INFO
```

### Comparing `weather_command-6.0.0/LICENSE` & `weather_command-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `weather_command-6.0.0/README.md` & `weather_command-6.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -76,10 +76,16 @@
 
 ![Hourly weather](./assets/hourly.png)
 
 - Hourly Weather Temp Only
 
 ![Hourl weather temp only](./assets/hourly_temp_only.png)
 
+## Settings
+weather now has the ability to save settings to default certain flags. The list of possible settings can be seen with:
+
+```sh
+weather settings --help
+```
 ## Contributing
 
 Contributions to this project are welcome. If you are interesting in contributing please see our [contributing guide](CONTRIBUTING.md)
```

### Comparing `weather_command-6.0.0/pyproject.toml` & `weather_command-6.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weather-command"
-version = "6.0.0"
+version = "6.1.0"
 description = "Command line weather app"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/weather-command"
 homepage = "https://github.com/sanders41/weather-command"
 documentation = "https://github.com/sanders41/weather-command"
@@ -23,15 +23,15 @@
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 mypy = "1.2.0"
 pre-commit = "2.21.0"
 pytest = "7.3.1"
 pytest-cov = "4.0.0"
 tox = "4.4.12"
-ruff = "0.0.261"
+ruff = "0.0.262"
 tomli = {version = "2.0.1", python = "<3.11"}
 types-pyyaml = "6.0.12.9"
 pytest-asyncio = "0.21.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `weather_command-6.0.0/weather_command/_builder.py` & `weather_command-6.1.0/weather_command/_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from functools import lru_cache
 
 from rich.style import Style
 from rich.table import Table
 
 from weather_command._cache import Cache
 from weather_command._config import console
-from weather_command._location import get_location_details
+from weather_command._location import build_location_url, get_location_details
 from weather_command._utils import build_weather_url
 from weather_command._weather import get_current_weather, get_icon, get_one_call_weather
 from weather_command.models.location import Location
 from weather_command.models.weather import CurrentWeather, OneCallWeather
 
 HEADER_ROW_STYLE = Style(color="sky_blue2", bold=True)
 
@@ -444,84 +444,86 @@
     how: str,
     city_zip: str,
     *,
     state_code: str | None,
     country_code: str | None,
     units: str,
 ) -> tuple[CurrentWeather, Location]:
-    if how == "zip":
-        cache = Cache()
-        cache_hit = cache.get(city_zip)
-        if cache_hit:
-            if cache_hit.location:
-                location = cache_hit.location
-            else:
-                location = get_location_details(
-                    how=how, city_zip=city_zip, state=state_code, country=country_code
-                )
-            if cache_hit.current_weather:
-                current_weather = cache_hit.current_weather.current_weather
-                return cache_hit.current_weather.current_weather, location
-            else:
-                url = build_weather_url(
-                    forecast_type="current",
-                    units=units,
-                    lon=location.lon,
-                    lat=location.lat,
-                )
-                current_weather = await get_current_weather(url, how, city_zip)
-                return current_weather, location
+    location_url = build_location_url(how, city_zip, state_code, country_code)
+    cache = Cache()
+    cache_hit = cache.get(location_url)
+    if cache_hit:
+        if cache_hit.location:
+            location = cache_hit.location
+        else:
+            location = get_location_details(
+                how=how, city_zip=city_zip, state=state_code, country=country_code
+            )
+        if cache_hit.current_weather:
+            current_weather = cache_hit.current_weather.current_weather
+            return cache_hit.current_weather.current_weather, location
+        else:
+            url = build_weather_url(
+                forecast_type="current",
+                units=units,
+                lon=location.lon,
+                lat=location.lat,
+            )
+            current_weather = await get_current_weather(url, cache_key=location_url)
+            return current_weather, location
 
     location = get_location_details(
         how=how, city_zip=city_zip, state=state_code, country=country_code
     )
 
     url = build_weather_url(
         forecast_type="current",
         units=units,
         lon=location.lon,
         lat=location.lat,
     )
-    current_weather = await get_current_weather(url, how, city_zip)
+    current_weather = await get_current_weather(url, cache_key=location_url)
+
     return current_weather, location
 
 
 async def _gather_one_call_weather(
     how: str,
     city_zip: str,
     *,
     state_code: str | None,
     country_code: str | None,
     units: str,
 ) -> tuple[OneCallWeather, Location]:
-    if how == "zip":
-        cache = Cache()
-        cache_hit = cache.get(city_zip)
-        if cache_hit:
-            if cache_hit.location:
-                location = cache_hit.location
-            else:
-                location = get_location_details(
-                    how=how, city_zip=city_zip, state=state_code, country=country_code
-                )
-            if cache_hit.one_call_weather:
-                return cache_hit.one_call_weather.one_call_weather, location
-            else:
-                url = build_weather_url(
-                    forecast_type="daily", units=units, lon=location.lon, lat=location.lat
-                )
-                weather = await get_one_call_weather(url, how, city_zip)
-                return weather, location
+    location_url = build_location_url(how, city_zip, state_code, country_code)
+    cache = Cache()
+    cache_hit = cache.get(location_url)
+    if cache_hit:
+        if cache_hit.location:
+            location = cache_hit.location
+        else:
+            location = get_location_details(
+                how=how, city_zip=city_zip, state=state_code, country=country_code
+            )
+        if cache_hit.one_call_weather:
+            return cache_hit.one_call_weather.one_call_weather, location
+        else:
+            url = build_weather_url(
+                forecast_type="daily", units=units, lon=location.lon, lat=location.lat
+            )
+            weather = await get_one_call_weather(url, location_url)
+            return weather, location
 
     location = get_location_details(
         how=how, city_zip=city_zip, state=state_code, country=country_code
     )
 
     url = build_weather_url(forecast_type="daily", units=units, lon=location.lon, lat=location.lat)
-    weather = await get_one_call_weather(url, how, city_zip)
+    weather = await get_one_call_weather(url, location_url)
+
     return weather, location
 
 
 def _hourly_temp_only(
     weather: OneCallWeather, units: str, am_pm: bool, location: Location
 ) -> Table:
     _, _, _, temp_units = _get_units(units)
```

### Comparing `weather_command-6.0.0/weather_command/_cache.py` & `weather_command-6.1.0/weather_command/_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             self.cache_dir.mkdir(parents=True)
 
         self._cache: dict[str, CacheItem] | None = self._load()
 
     def add(
         self,
         *,
-        city_zip: str,
+        cache_key: str,
         location: Location | None = None,
         current_weather: CurrentWeather | None = None,
         one_call_weather: OneCallWeather | None = None,
         cache_size: int = 5,
     ) -> None:
         def save_cache() -> None:
             cache: dict[str, Any] = {}
@@ -84,38 +84,38 @@
                 OneCallWeatherCache(
                     date_time_saved=datetime.utcnow(), one_call_weather=one_call_weather
                 ).dict()
                 if one_call_weather
                 else None
             )
 
-            cache_hit = self.get(city_zip)
+            cache_hit = self.get(cache_key)
 
             if cache_hit:
-                cache[city_zip.lower()] = {
+                cache[cache_key.lower()] = {
                     "location": cache_hit.location.dict()
                     if cache_hit.location and not location_cache
                     else location_cache,
                     "currentWeather": cache_hit.current_weather.dict()
                     if cache_hit.current_weather and not current_weather_cache
                     else current_weather_cache,
                     "oneCallWeather": cache_hit.one_call_weather.dict()
                     if cache_hit.one_call_weather and not one_call_weather_cache
                     else one_call_weather_cache,
                 }
             else:
-                cache[city_zip.lower()] = {
+                cache[cache_key.lower()] = {
                     "location": location_cache,
                     "currentWeather": current_weather_cache,
                     "oneCallWeather": one_call_weather_cache,
                 }
 
             if self._cache:
                 for key in self._cache:
-                    if key != city_zip:
+                    if key != cache_key:
                         saved_cache = self._cache[key]
                         cache[key] = saved_cache.dict()
 
             with open(self._cache_file, "w") as f:
                 json.dump(cache, f, cls=DateTimeEncoder)
 
         if not self._cache or len(self._cache.keys()) < cache_size:
@@ -125,19 +125,19 @@
             del self._cache[last_key]
             save_cache()
 
     def clear(self) -> None:
         if self._cache_file.exists():
             self._cache_file.unlink()
 
-    def get(self, city_zip: str) -> CacheItem | None:
-        if not self._cache or not self._cache.get(city_zip):
+    def get(self, cache_key: str) -> CacheItem | None:
+        if not self._cache or not self._cache.get(cache_key):
             return None
 
-        cache = self._cache[city_zip.lower()]
+        cache = self._cache[cache_key.lower()]
         if cache.current_weather:
             time_diff = datetime.utcnow() - cache.current_weather.date_time_saved
             if (time_diff.total_seconds() / 60) > cache.current_weather.cache_duration_minutes:
                 cache.current_weather = None
 
         if cache.one_call_weather:
             time_diff = datetime.utcnow() - cache.one_call_weather.date_time_saved
```

### Comparing `weather_command-6.0.0/weather_command/_config.py` & `weather_command-6.1.0/weather_command/_config.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.0.0/weather_command/_location.py` & `weather_command-6.1.0/weather_command/_location.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,50 +30,49 @@
     country: str | None = None,
 ) -> Location:
     if how not in ("city", "zip"):
         raise UnknownSearchTypeError(f"{type} is not a valid type")
 
     cache = Cache()
 
-    if how == "zip":
-        cache_hit = cache.get(city_zip)
-        if cache_hit and cache_hit.location:
-            return cache_hit.location
-
-    base_url = _build_url(how, city_zip, state, country)
+    base_url = build_location_url(how, city_zip, state, country)
+    cache_hit = cache.get(base_url)
+    if cache_hit and cache_hit.location:
+        return cache_hit.location
 
     response = httpx.get(base_url, headers={"user-agent": "weather-command"})
     try:
         response.raise_for_status()
     except httpx.HTTPStatusError as e:
         check_status_error(e, console)
 
     if not response.json():
         _print_location_not_found_error()
         sys.exit(1)
 
     response_json = response.json()
 
     try:
+        # Sometimes the response comes back as a single location and sometimes it is a list of
+        # locations. The if/else here is to handle both of these cases.
         if isinstance(response_json, list):
             location = Location(**response_json[0])
         else:
             location = Location(**response_json)
 
-        if how == "zip":
-            cache.add(city_zip=city_zip, location=location)
+        cache.add(cache_key=base_url, location=location)
     except ValidationError:
         _print_location_not_found_error()
         sys.exit(1)
 
     return location
 
 
 @lru_cache(maxsize=1)
-def _build_url(how: str, city_zip: str, state: str | None, country: str | None) -> str:
+def build_location_url(how: str, city_zip: str, state: str | None, country: str | None) -> str:
     """Cache so if retries are needed the url only needs to be built once."""
     if how == "zip":
         base_url = f"{LOCATION_BASE_URL}&postalcode={city_zip}"
     else:
         base_url = f"{LOCATION_BASE_URL}&city={city_zip}"
 
     if state:
```

### Comparing `weather_command-6.0.0/weather_command/_weather.py` & `weather_command-6.1.0/weather_command/_weather.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,51 +13,49 @@
 from weather_command._cache import Cache
 from weather_command._config import console
 from weather_command.errors import check_status_error
 from weather_command.models.weather import CurrentWeather, OneCallWeather
 
 
 @retry(stop=stop_after_attempt(5), wait=wait_fixed(0.5), reraise=True)
-async def get_current_weather(url: str, how: str, city_zip: str) -> CurrentWeather:
+async def get_current_weather(url: str, cache_key: str) -> CurrentWeather:
     try:
         async with AsyncClient() as client:
             response = await client.get(url)
 
         response.raise_for_status()
     except HTTPStatusError as e:
         check_status_error(e, console)
 
     try:
         weather = CurrentWeather(**response.json())
     except ValidationError:
         _print_validation_error()
 
-    if how == "zip":
-        cache = Cache()
-        cache.add(city_zip=city_zip, current_weather=weather)
+    cache = Cache()
+    cache.add(cache_key=cache_key, current_weather=weather)
     return weather
 
 
 @retry(stop=stop_after_attempt(5), wait=wait_fixed(0.5), reraise=True)
-async def get_one_call_weather(url: str, how: str, city_zip: str) -> OneCallWeather:
+async def get_one_call_weather(url: str, cache_key: str) -> OneCallWeather:
     async with AsyncClient() as client:
         response = await client.get(url)
     try:
         response.raise_for_status()
     except HTTPStatusError as e:
         check_status_error(e, console)
 
     try:
         weather = OneCallWeather(**response.json())
     except ValidationError:
         _print_validation_error()
 
-    if how == "zip":
-        cache = Cache()
-        cache.add(city_zip=city_zip, one_call_weather=weather)
+    cache = Cache()
+    cache.add(cache_key=cache_key, one_call_weather=weather)
 
     return weather
 
 
 class WeatherIcons(Enum):
     BROKEN_CLOUDS = ":sun_behind_cloud:"
     CLEAR_SKY = ":sun:"
```

### Comparing `weather_command-6.0.0/weather_command/main.py` & `weather_command-6.1.0/weather_command/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 from typer import Argument, Exit, Option, Typer, echo
 
 from weather_command import settings_commands
 from weather_command._builder import show_current, show_daily, show_hourly
 from weather_command._cache import Cache
 from weather_command._config import console, load_settings
-from weather_command._location import get_location_details
+from weather_command._location import build_location_url, get_location_details
 from weather_command._utils import build_weather_url
 from weather_command._weather import get_current_weather, get_one_call_weather
 
-__version__ = "6.0.0"
+__version__ = "6.1.0"
 
 app = Typer()
 app.add_typer(settings_commands.app, name="settings", help="Manage saved settings.")
 
 
 class ForecastType(str, Enum):
     CURRENT = "current"
@@ -34,16 +34,17 @@
     city_zip: str,
     state_code: Union[str, None],
     country_code: Union[str, None],
     units: str,
 ) -> None:
     with console.status("Getting weather..."):
         retrieve: List[Coroutine] = []
+        location_url = build_location_url(how, city_zip, state_code, country_code)
         cache = Cache()
-        cache_hit = cache.get(city_zip)
+        cache_hit = cache.get(location_url)
         if cache_hit:
             if cache_hit.location:
                 location = cache_hit.location
             else:  # pragma: no cover
                 # This is a fail safe. It should only be possible to get here if someone manually
                 # modified the cache file.
                 location = get_location_details(
@@ -53,34 +54,34 @@
             if not cache_hit.current_weather:
                 url = build_weather_url(
                     forecast_type="current",
                     units=units,
                     lon=location.lon,
                     lat=location.lat,
                 )
-                retrieve.append(get_current_weather(url, how, city_zip))
+                retrieve.append(get_current_weather(url, location_url))
             if not cache_hit.one_call_weather:
                 url = build_weather_url(
                     forecast_type="daily", units=units, lon=location.lon, lat=location.lat
                 )
-                retrieve.append(get_one_call_weather(url, how, city_zip))
+                retrieve.append(get_one_call_weather(url, location_url))
         else:
             location = get_location_details(
-                how="zip", city_zip=city_zip, state=state_code, country=country_code
+                how=how, city_zip=city_zip, state=state_code, country=country_code
             )
 
             url = build_weather_url(
                 forecast_type="current", units=units, lon=location.lon, lat=location.lat
             )
-            retrieve.append(get_current_weather(url, how, city_zip))
+            retrieve.append(get_current_weather(url, location_url))
 
             url = build_weather_url(
                 forecast_type="daily", units=units, lon=location.lon, lat=location.lat
             )
-            retrieve.append(get_one_call_weather(url, how, city_zip))
+            retrieve.append(get_one_call_weather(url, location_url))
 
         if retrieve:
             await asyncio.gather(*retrieve)
 
 
 async def _runner(
     how: str,
@@ -112,15 +113,15 @@
     else:
         am_pm_choice = am_pm
 
     if clear_cache:
         cache = Cache()
         cache.clear()
 
-    if not clear_cache and how == "zip":
+    if not clear_cache:
         await _preload_cache(how, city_zip, state_code, country_code, units)
 
     if forecast_type == "current":
         await show_current(
             how=how,
             city_zip=city_zip,
             units=units,
```

### Comparing `weather_command-6.0.0/weather_command/models/weather.py` & `weather_command-6.1.0/weather_command/models/weather.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.0.0/weather_command/settings_commands.py` & `weather_command-6.1.0/weather_command/settings_commands.py`

 * *Files identical despite different names*

### Comparing `weather_command-6.0.0/PKG-INFO` & `weather_command-6.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weather-command
-Version: 6.0.0
+Version: 6.1.0
 Summary: Command line weather app
 Home-page: https://github.com/sanders41/weather-command
 License: MIT
 Keywords: weather,cli
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -104,11 +104,17 @@
 
 ![Hourly weather](./assets/hourly.png)
 
 - Hourly Weather Temp Only
 
 ![Hourl weather temp only](./assets/hourly_temp_only.png)
 
+## Settings
+weather now has the ability to save settings to default certain flags. The list of possible settings can be seen with:
+
+```sh
+weather settings --help
+```
 ## Contributing
 
 Contributions to this project are welcome. If you are interesting in contributing please see our [contributing guide](CONTRIBUTING.md)
```

