# Comparing `tmp/twitter-api-client-0.6.5.tar.gz` & `tmp/twitter-api-client-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.6.5.tar", last modified: Mon Apr 17 00:41:41 2023, max compression
+gzip compressed data, was "twitter-api-client-0.6.6.tar", last modified: Wed Apr 19 22:58:47 2023, max compression
```

## Comparing `twitter-api-client-0.6.5.tar` & `twitter-api-client-0.6.6.tar`

### file list

```diff
@@ -1,29 +1,24 @@
-drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-17 00:41:41.387368 twitter-api-client-0.6.5/
--rw-rw-r--   0 x         (1000) x         (1000)     1075 2023-04-14 02:53:18.000000 twitter-api-client-0.6.5/LICENSE
--rw-rw-r--   0 x         (1000) x         (1000)     6812 2023-04-17 00:41:41.387368 twitter-api-client-0.6.5/PKG-INFO
--rw-rw-r--   0 x         (1000) x         (1000)       38 2023-04-17 00:41:41.387368 twitter-api-client-0.6.5/setup.cfg
--rw-rw-r--   0 x         (1000) x         (1000)     7860 2023-04-17 00:37:33.000000 twitter-api-client-0.6.5/setup.py
-drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-17 00:41:41.383368 twitter-api-client-0.6.5/twitter/
--rw-rw-r--   0 x         (1000) x         (1000)        0 2023-04-14 02:53:18.000000 twitter-api-client-0.6.5/twitter/__init__.py
--rw-rw-r--   0 x         (1000) x         (1000)    26566 2023-04-16 14:27:37.000000 twitter-api-client-0.6.5/twitter/account.py
-drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-17 00:41:41.387368 twitter-api-client-0.6.5/twitter/config/
--rw-rw-r--   0 x         (1000) x         (1000)        0 2023-04-14 02:53:18.000000 twitter-api-client-0.6.5/twitter/config/__init__.py
--rw-rw-r--   0 x         (1000) x         (1000)      909 2023-04-14 02:53:18.000000 twitter-api-client-0.6.5/twitter/config/log.py
--rw-rw-r--   0 x         (1000) x         (1000)   147862 2023-04-14 21:16:39.000000 twitter-api-client-0.6.5/twitter/config/operations.py
--rw-rw-r--   0 x         (1000) x         (1000)     5859 2023-04-15 18:04:24.000000 twitter-api-client-0.6.5/twitter/config/settings.py
--rw-rw-r--   0 x         (1000) x         (1000)     2539 2023-04-14 21:53:11.000000 twitter-api-client-0.6.5/twitter/constants.py
--rw-rw-r--   0 x         (1000) x         (1000)     5259 2023-04-17 00:28:42.000000 twitter-api-client-0.6.5/twitter/login.py
-drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-17 00:41:41.387368 twitter-api-client-0.6.5/twitter/noauth/
--rw-rw-r--   0 x         (1000) x         (1000)        0 2023-04-16 21:57:30.000000 twitter-api-client-0.6.5/twitter/noauth/__init__.py
--rw-rw-r--   0 x         (1000) x         (1000)     2646 2023-04-16 23:55:48.000000 twitter-api-client-0.6.5/twitter/noauth/operation.py
--rw-rw-r--   0 x         (1000) x         (1000)     7400 2023-04-17 00:37:33.000000 twitter-api-client-0.6.5/twitter/noauth/scraper.py
--rw-rw-r--   0 x         (1000) x         (1000)     2852 2023-04-17 00:11:45.000000 twitter-api-client-0.6.5/twitter/noauth/util.py
--rw-rw-r--   0 x         (1000) x         (1000)    12836 2023-04-16 22:08:27.000000 twitter-api-client-0.6.5/twitter/scraper.py
--rw-rw-r--   0 x         (1000) x         (1000)     4998 2023-04-17 00:28:42.000000 twitter-api-client-0.6.5/twitter/search.py
--rw-rw-r--   0 x         (1000) x         (1000)     2256 2023-04-17 00:28:42.000000 twitter-api-client-0.6.5/twitter/utils.py
-drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-04-17 00:41:41.387368 twitter-api-client-0.6.5/twitter_api_client.egg-info/
--rw-rw-r--   0 x         (1000) x         (1000)     6812 2023-04-17 00:41:41.000000 twitter-api-client-0.6.5/twitter_api_client.egg-info/PKG-INFO
--rw-rw-r--   0 x         (1000) x         (1000)      565 2023-04-17 00:41:41.000000 twitter-api-client-0.6.5/twitter_api_client.egg-info/SOURCES.txt
--rw-rw-r--   0 x         (1000) x         (1000)        1 2023-04-17 00:41:41.000000 twitter-api-client-0.6.5/twitter_api_client.egg-info/dependency_links.txt
--rw-rw-r--   0 x         (1000) x         (1000)       82 2023-04-17 00:41:41.000000 twitter-api-client-0.6.5/twitter_api_client.egg-info/requires.txt
--rw-rw-r--   0 x         (1000) x         (1000)        8 2023-04-17 00:41:41.000000 twitter-api-client-0.6.5/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-19 22:58:47.565021 twitter-api-client-0.6.6/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-04-17 21:53:35.000000 twitter-api-client-0.6.6/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)     6857 2023-04-19 22:58:47.565021 twitter-api-client-0.6.6/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-04-19 22:58:47.565021 twitter-api-client-0.6.6/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)     8154 2023-04-19 22:52:46.000000 twitter-api-client-0.6.6/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-19 22:58:47.565021 twitter-api-client-0.6.6/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-17 21:53:35.000000 twitter-api-client-0.6.6/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    22355 2023-04-19 20:10:25.000000 twitter-api-client-0.6.6/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    27260 2023-04-19 22:52:46.000000 twitter-api-client-0.6.6/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     5527 2023-04-19 22:52:46.000000 twitter-api-client-0.6.6/twitter/login.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-19 22:58:47.565021 twitter-api-client-0.6.6/twitter/noauth/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-04-17 21:53:35.000000 twitter-api-client-0.6.6/twitter/noauth/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)     2567 2023-04-19 22:52:46.000000 twitter-api-client-0.6.6/twitter/noauth/operation.py
+-rw-r--r--   0 x         (1000) x         (1000)     7404 2023-04-19 19:28:54.000000 twitter-api-client-0.6.6/twitter/noauth/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     2852 2023-04-17 21:53:35.000000 twitter-api-client-0.6.6/twitter/noauth/util.py
+-rw-r--r--   0 x         (1000) x         (1000)    10521 2023-04-19 19:28:54.000000 twitter-api-client-0.6.6/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     4902 2023-04-19 22:46:55.000000 twitter-api-client-0.6.6/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     3269 2023-04-19 22:46:55.000000 twitter-api-client-0.6.6/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-04-19 22:58:47.565021 twitter-api-client-0.6.6/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)     6857 2023-04-19 22:58:47.000000 twitter-api-client-0.6.6/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      459 2023-04-19 22:58:47.000000 twitter-api-client-0.6.6/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-04-19 22:58:47.000000 twitter-api-client-0.6.6/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       82 2023-04-19 22:58:47.000000 twitter-api-client-0.6.6/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-04-19 22:58:47.000000 twitter-api-client-0.6.6/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.6.5/LICENSE` & `twitter-api-client-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.5/PKG-INFO` & `twitter-api-client-0.6.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,222 +1,258 @@
-Metadata-Version: 2.1
-Name: twitter-api-client
-Version: 0.6.5
-Summary: Twitter API
-Home-page: https://github.com/trevorhobenshield/twitter-api
-Author: Trevor Hobenshield
-Author-email: trevorhobenshield@gmail.com
-Keywords: twitter api client async search automation bot scrape
-Requires-Python: >=3.11.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
+from textwrap import dedent
 
+from setuptools import find_packages, setup
 
- Complete implementation of the undocumented Twitter API
-
- Includes tools to **scrape**, **automate**, and **search** twitter
-
- ### Installation
-
-```python
- from twitter.account import Account
-
- email, username, password = ..., ..., ...
- account = Account(email, username, password)
-
- account.create_poll('test poll 123', ['hello', 'world', 'foo', 'bar'], 10080)
-
- # DM 1 user
- account.dm([123], 'hello world', filename='test.png')
-
- # DM group of users
- account.dm([123, 234, 345], 'foo bar', filename='test.mp4')
-
- # schedule a tweet (date str or timestamp)
- account.schedule_tweet('scheduled hello', 1679912795, media=['test.jpg'])
-
- # schedule a reply tweet (date str or timestamp)
- account.schedule_tweet('scheduled world', '2023-03-25 19:11', media=['test.jpg'], reply_to=645)
-
- account.unschedule_tweet(321)
-
- # tweets
- account.tweet('test 123')
- account.tweet('test 234', media=['test.mp4'])
- account.tweet('test 345', media=['test.jpg', 'test.png', 'test.jpeg', 'test.jfif'])
- account.tweet('test 456', media=[{'file': 'test.jpeg', 'tagged_users': [123234345456], 'alt': 'some image'}])
- account.untweet(123)
- account.retweet(1633609779745820675)
- account.unretweet(1633609779745820675)
- account.quote(1633609779745820675, 'elonmusk', 'test 123')
- account.reply(1633609779745820675, 'test 123')
- account.like(1633609779745820675)
- account.unlike(1633609779745820675)
- account.bookmark(1633609779745820675)
- account.unbookmark(1633609779745820675)
- account.pin(1635479755364651008)
- account.unpin(1635479755364651008)
-
- # users
- account.follow(50393960)
- account.unfollow(50393960)
- account.mute(50393960)
- account.unmute(50393960)
- account.enable_notifications(50393960)
- account.disable_notifications(50393960)
- account.block(50393960)
- account.unblock(50393960)
-
- # other
- account.stats(50393960)
-
- # user profile
- account.update_profile_image('test.jpg')
- account.update_profile_banner('test.png')
- account.update_profile_info(name='Foo Bar', description='test 123', location='Victoria, BC')
-
- # topics
- account.follow_topic(808713037230157824)
- account.unfollow_topic(808713037230157824)
-
- # lists
- account.create_list('My List', 'description of my list', private=False)
- account.update_list(543, 'My Updated List', 'some updated description', private=False)
- account.update_list_banner(543, 'test.png')
- account.delete_list_banner(543)
- account.add_list_member(543, 50393960)
- account.remove_list_member(543, 50393960)
- account.delete_list(543)
- account.pin_list(543)
- account.unpin_list(543)
-
- # refresh all pinned lists in this order
- account.update_pinned_lists([543, 432, 321])
-
- # unpin all lists
- account.update_pinned_lists([])
-
- # get timelines
- timeline = account.home_timeline()
- latest_timeline = account.home_latest_timeline(limit=100)
-
- # example configuration
- account.update_settings({
-     "address_book_live_sync_enabled": False,
-     "allow_ads_personalization": False,
-     "allow_authenticated_periscope_requests": True,
-     "allow_dm_groups_from": "following",
-     "allow_dms_from": "following",
-     "allow_location_history_personalization": False,
-     "allow_logged_out_device_personalization": False,
-     "allow_media_tagging": "none",
-     "allow_sharing_data_for_third_party_personalization": False,
-     "alt_text_compose_enabled": None,
-     "always_use_https": True,
-     "autoplay_disabled": False,
-     "country_code": "us",
-     "discoverable_by_email": False,
-     "discoverable_by_mobile_phone": False,
-     "display_sensitive_media": False,
-     "dm_quality_filter": "enabled",
-     "dm_receipt_setting": "all_disabled",
-     "geo_enabled": False,
-     "include_alt_text_compose": True,
-     "include_mention_filter": True,
-     "include_nsfw_admin_flag": True,
-     "include_nsfw_user_flag": True,
-     "include_ranked_timeline": True,
-     "language": "en",
-     "mention_filter": "unfiltered",
-     "nsfw_admin": False,
-     "nsfw_user": False,
-     "personalized_trends": True,
-     "protected": False,
-     "ranked_timeline_eligible": None,
-     "ranked_timeline_setting": None,
-     "require_password_login": False,
-     "requires_login_verification": False,
-     "sleep_time": {
-         "enabled": False,
-         "end_time": None,
-         "start_time": None
-     },
-     "translator_type": "none",
-     "universal_quality_filtering_enabled": "enabled",
-     "use_cookie_personalization": False,
- })
-
- # example configuration
- account.update_search_settings({
-     "optInFiltering": True,  # filter out nsfw content
-     "optInBlocking": True,  # filter out blocked accounts
- })
-
- ## account.change_password('old password', 'new password')
- ## account.logout_all_sessions()
-
- ```
-
-
- ### Scraping
-
- #### Get all user/tweet data
-
- ```python
- from twitter.scraper import Scraper
-
- email, username, password = ..., ..., ...
- scraper = Scraper(email, username, password)  # session
-
- ####### User Data ########
- users = scraper.user_by_screen_name(['foo', 'bar', 'baz'])
- tweets = scraper.tweets([123, 234, 345])
- likes = scraper.likes([123, 234, 345])
- tweets_and_replies = scraper.tweets_and_replies([123, 234, 345])
- media = scraper.media([123, 234, 345])
- following = scraper.following([123, 234, 345])
- followers = scraper.followers([123, 234, 345])
-
- ######## Tweet Data ########
- tweets_by_ids = scraper.tweet_by_rest_id([456, 567, 678])
- tweets_details = scraper.tweets_details([456, 567, 678])
- retweeters = scraper.retweeters([456, 567, 678])
- favoriters = scraper.favoriters([456, 567, 678])
-
- scraper.download_media([456, 567, 678])
- ```
-
- #### Get user/tweet data (no auth)
-
- ```python
- from twitter.noauth.scraper import Scraper
-
- scraper = Scraper()
-
- users = scraper.user(['foo', 'bar', 'baz'])
- users = scraper.user_by_id([123, 234, 345])
- users = scraper.users_by_ids([123, 234, 345])  # special batch query
-
- tweets = scraper.tweet_by_id([987, 876, 765])  # condensed
- tweets = scraper.tweet_details([987, 876, 765])
-
- user_tweets = scraper.tweets([123, 234, 345])
- user_tweets_replies = scraper.tweets_and_replies([123, 234, 345])
- user_media = scraper.media([123, 234, 345])
- ```
-
- #### Search
-
- ```python   
- from twitter.search import search
-
- search(
-     '(#dogs OR #cats) min_retweets:500',
-     'min_faves:10000 @elonmusk until:2023-02-16 since:2023-02-01',
-     'brasil portugal -argentina',
-     'paperswithcode -tensorflow -tf',
-     'skateboarding baseball guitar',
-     'cheese bread butter',
-     'ios android',
-     # limit=1000, # optional limit
- )
- ```
+install_requires = [
+    "nest_asyncio",
+    "aiohttp",
+    "requests",
+    "tqdm",
+    "orjson",
+    'uvloop; platform_system != "Windows"',
+]
+
+setup(
+    name="twitter-api-client",
+    version="0.6.6",
+    python_requires=">=3.11.0",
+    description="Twitter API",
+    long_description=dedent('''
+    Complete implementation of the undocumented Twitter API
+    
+    Includes tools to **scrape**, **automate**, and **search** twitter
+    
+    * [Installation](#installation)
+    * [Automation](#automation)
+    * [Scraping](#scraping)
+      * [Get all user/tweet data](#get-all-usertweet-data)
+      * [Get user/tweet data (no auth)](#get-usertweet-data-no-auth)
+      * [Search](#search)
+    * [Notes](#notes)
+    
+    ### Automation
+    
+    ```python
+    from twitter.account import Account
+    
+    email, username, password = ..., ..., ...
+    account = Account(email, username, password, debug=2, save=True)
+    
+    account.tweet('test 123')
+    account.untweet(123456)
+    account.retweet(123456)
+    account.unretweet(123456)
+    account.reply('foo', tweet_id=123456)
+    account.quote('bar', tweet_id=123456)
+    account.schedule_tweet('schedule foo', 1681851240)
+    account.unschedule_tweet(123456)
+    
+    account.tweet('hello world', media=[
+        {'media': 'test.jpg', 'alt': 'some alt text', 'tagged_users': [123]},
+        {'media': 'test.jpeg', 'alt': 'some alt text', 'tagged_users': [123]},
+        {'media': 'test.png', 'alt': 'some alt text', 'tagged_users': [123]},
+        {'media': 'test.jfif', 'alt': 'some alt text', 'tagged_users': [123]},
+    ])
+    
+    account.schedule_tweet('foo bar', '2023-04-18 15:42', media=[
+        {'media': 'test.gif', 'alt': 'some alt text'},
+    ])
+    
+    account.schedule_reply('hello world', '2023-04-19 15:42', tweet_id=123456, media=[
+        {'media': 'test.gif', 'alt': 'some alt text'},
+    ])
+    
+    account.dm('my message', [1234], media='test.jpg')
+    
+    account.create_poll('test poll 123', ['hello', 'world', 'foo', 'bar'], 10080)
+    
+    # tweets
+    account.like(123456)
+    account.unlike(123456)
+    account.bookmark(123456)
+    account.unbookmark(123456)
+    account.pin(123456)
+    account.unpin(123456)
+    
+    # users
+    account.follow(1234)
+    account.unfollow(1234)
+    account.mute(1234)
+    account.unmute(1234)
+    account.enable_notifications(1234)
+    account.disable_notifications(1234)
+    account.block(1234)
+    account.unblock(1234)
+    
+    # user profile
+    account.update_profile_image('test.jpg')
+    account.update_profile_banner('test.png')
+    account.update_profile_info(name='Foo Bar', description='test 123', location='Victoria, BC')
+    
+    #  topics
+    account.follow_topic(111)
+    account.unfollow_topic(111)
+    
+    # lists
+    account.create_list('My List', 'description of my list', private=False)
+    account.update_list(222, 'My Updated List', 'some updated description', private=False)
+    account.update_list_banner(222, 'test.png')
+    account.delete_list_banner(222)
+    account.add_list_member(222, 1234)
+    account.remove_list_member(222, 1234)
+    account.delete_list(222)
+    account.pin_list(222)
+    account.unpin_list(222)
+    
+    # refresh all pinned lists in this order
+    account.update_pinned_lists([222, 111, 333])
+    
+    # unpin all lists
+    account.update_pinned_lists([])
+    
+    # get timelines
+    timeline = account.home_timeline()
+    latest_timeline = account.home_latest_timeline(limit=500)
+    
+    # get bookmarks
+    bookmarks = account.bookmarks()
+    
+    # example configuration
+    account.update_settings({
+        "address_book_live_sync_enabled": False,
+        "allow_ads_personalization": False,
+        "allow_authenticated_periscope_requests": True,
+        "allow_dm_groups_from": "following",
+        "allow_dms_from": "following",
+        "allow_location_history_personalization": False,
+        "allow_logged_out_device_personalization": False,
+        "allow_media_tagging": "none",
+        "allow_sharing_data_for_third_party_personalization": False,
+        "alt_text_compose_enabled": None,
+        "always_use_https": True,
+        "autoplay_disabled": False,
+        "country_code": "us",
+        "discoverable_by_email": False,
+        "discoverable_by_mobile_phone": False,
+        "display_sensitive_media": False,
+        "dm_quality_filter": "enabled",
+        "dm_receipt_setting": "all_disabled",
+        "geo_enabled": False,
+        "include_alt_text_compose": True,
+        "include_mention_filter": True,
+        "include_nsfw_admin_flag": True,
+        "include_nsfw_user_flag": True,
+        "include_ranked_timeline": True,
+        "language": "en",
+        "mention_filter": "unfiltered",
+        "nsfw_admin": False,
+        "nsfw_user": False,
+        "personalized_trends": True,
+        "protected": False,
+        "ranked_timeline_eligible": None,
+        "ranked_timeline_setting": None,
+        "require_password_login": False,
+        "requires_login_verification": False,
+        "sleep_time": {
+            "enabled": False,
+            "end_time": None,
+            "start_time": None
+        },
+        "translator_type": "none",
+        "universal_quality_filtering_enabled": "enabled",
+        "use_cookie_personalization": False,
+    })
+    
+    # example configuration
+    account.update_search_settings({
+        "optInFiltering": True,  # filter nsfw content
+        "optInBlocking": True,  # filter blocked accounts
+    })
+    
+    ## change_password('old pwd','new pwd)
+    
+    ```
+    
+    ### Scraping
+    
+    #### Get all user/tweet data
+    
+    ```python
+    from twitter.scraper import Scraper
+    
+    email, username, password = ..., ..., ...
+    scraper = Scraper(email, username, password, debug=1, save=True)
+    
+    # user data
+    users = scraper.users(['foo', 'bar', 'hello', 'world'])
+    users = scraper.users_by_ids([123, 234, 345])  # batch-request
+    tweets = scraper.tweets([123, 234, 345])
+    likes = scraper.likes([123, 234, 345])
+    tweets_and_replies = scraper.tweets_and_replies([123, 234, 345])
+    media = scraper.media([123, 234, 345])
+    following = scraper.following([123, 234, 345])
+    followers = scraper.followers([123, 234, 345])
+    scraper.tweet_stats([111111, 222222, 333333])
+    
+    
+    # tweet data
+    tweets_by_ids = scraper.tweets_by_id([987, 876, 754])
+    tweets_details = scraper.tweets_details([987, 876, 754])
+    retweeters = scraper.retweeters([987, 876, 754])
+    favoriters = scraper.favoriters([987, 876, 754])
+    
+    scraper.download_media([
+        111111,
+        222222,
+        333333,
+        444444,
+    ])
+    
+    # trends
+    scraper.trends()
+    ```
+    
+    #### Get user/tweet data (no auth)
+    
+    ```python
+    from twitter.noauth.scraper import Scraper
+    
+    scraper = Scraper()
+    
+    users = scraper.users(['foo', 'bar', 'baz'])
+    users = scraper.users_by_id([123, 234, 345])
+    users = scraper.users_by_ids([123, 234, 345])  # special batch query
+    
+    tweets = scraper.tweets_by_id([987, 876, 765])  # condensed
+    tweets = scraper.tweets_details([987, 876, 765])
+    
+    user_tweets = scraper.tweets([123, 234, 345])
+    user_tweets_replies = scraper.tweets_and_replies([123, 234, 345])
+    user_media = scraper.media([123, 234, 345])
+    ```
+    
+    #### Search
+    
+    ```python   
+    from twitter.search import search
+    
+    search(
+        '(#dogs OR #cats) min_retweets:500',
+        'min_faves:10000 @elonmusk until:2023-02-16 since:2023-02-01',
+        'brasil portugal -argentina',
+        'paperswithcode -tensorflow -tf',
+        'skateboarding baseball guitar',
+        'cheese bread butter',
+        'ios android',
+        # limit=1000, # optional limit
+    )
+    ```
+    '''),
+    long_description_content_type='text/markdown',
+    author="Trevor Hobenshield",
+    author_email="trevorhobenshield@gmail.com",
+    url="https://github.com/trevorhobenshield/twitter-api",
+    install_requires=install_requires,
+    keywords="twitter api client async search automation bot scrape",
+    packages=find_packages(),
+    include_package_data=True,
+)
```

### Comparing `twitter-api-client-0.6.5/twitter/account.py` & `twitter-api-client-0.6.6/twitter/account.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 import asyncio
 import hashlib
-import inspect
 import logging.config
+import math
 import mimetypes
 import platform
 import random
-import re
 import time
 from copy import deepcopy
 from datetime import datetime
-from functools import wraps, partial
 from pathlib import Path
 from urllib.parse import urlencode
 from uuid import uuid1, getnode
 
 import orjson
-from requests import Response, Session
+from requests import Response
 from tqdm import tqdm
 
-from .config.log import log_config
-from .config.operations import operations
-from .config.settings import *
 from .constants import *
 from .login import login
-from .utils import get_headers, build_query, find_key
+from .util import find_key, get_headers, fmt_status, get_cursor, save_data
 
 try:
     if get_ipython().__class__.__name__ == 'ZMQInteractiveShell':
         import nest_asyncio
 
         nest_asyncio.apply()
 except:
@@ -39,181 +34,71 @@
     asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
 else:
     asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
 
 logging.config.dictConfig(log_config)
 logger = logging.getLogger(__name__)
 
-ID = 'ID'
-DUP_LIMIT = 5
 
+class GraphQL:
+    def __init__(self, operation: tuple, variables: dict, features: dict = Operation.default_features):
+        self.operation = operation
+        self.variables = variables
+        self.features = features
 
-def log(fn=None, *, level: int = logging.DEBUG, info: list = None) -> callable:
-    if fn is None:
-        return partial(log, level=level, info=info)
-
-    @wraps(fn)
-    def wrapper(*args, **kwargs):
-        args_info = " ".join(
-            f'{k}={v}' for k, v in dict(zip(inspect.getfullargspec(fn)[0], args)).items()
-            if '_id' in k or '_name' in k or 'Id' in k or 'Name' in k
-        )
-        r = fn(*args, **kwargs)
-
-        limits = {k: v for k, v in r.headers.items() if 'x-rate-limit' in k}
-        current_time = int(time.time())
-        wait = int(r.headers.get('x-rate-limit-reset', current_time)) - current_time
-        logger.log(level, f'{wait // 60} minutes until rate-limit reset. {limits = }')
-
-        try:
-            data = {}
-            if 200 <= r.status_code < 300:
-                if 'json' in r.headers.get('content-type', ''):
-                    data = r.json()
-                    if data.get('errors'):
-                        logger.log(level, f'[{ERROR}error{RESET}] ({fn.__name__}) {args_info} {r.status_code} {r.text}')
-                        return r
-
-                typenames = find_key(data, '__typename')
-                # logger.log(level, f'{typenames = }')
-                errors = ','.join([t for t in typenames if re.search('fail|error', t, flags=re.I)])
-
-                if errors:
-                    message = f'[{ERROR}error{RESET}] {r.status_code} ({BOLD}{fn.__name__}{RESET}) {args_info} {WARN}{errors}{RESET}'
-                else:
-                    message = f'[{SUCCESS}success{RESET}] {r.status_code} ({BOLD}{fn.__name__}{RESET}) {args_info}'
-
-                if info:
-                    for k in info:
-                        if callable(k):
-                            logger.log(level, f'{message} {k(r)}')
-                        else:
-                            attr = getattr(r, k)
-                            v = attr() if callable(attr) else attr
-                            d = {f"{k}": v}
-                            logger.log(level, f'{message} {d}')
-                else:
-                    logger.log(level, f'{message}')
-            else:
-                logger.log(level, f'[{ERROR}error{RESET}] ({fn.__name__}) {args_info} {r.status_code} {r.text}')
-        except Exception as e:
-            logger.log(level, f'[{ERROR}error{RESET}] ({fn.__name__}) {args_info} {r.status_code} {e}')
-        return r
+    def get(self):
+        ...
 
-    return wrapper
+    def post(self):
+        ...
 
 
 class Account:
-    V1_URL = 'https://api.twitter.com/1.1'
-    V2_URL = 'https://api.twitter.com/2'  # /search
-    GRAPHQL_URL = 'https://api.twitter.com/graphql'
 
-    def __init__(self, email: str, username: str, password: str):
+    def __init__(self, email: str, username: str, password: str, *, save=True, debug: int = 0):
         self.session = login(email, username, password)
+        self.gql_url = 'https://twitter.com/i/api/graphql'
+        self.v1_url = 'https://api.twitter.com/1.1'
+        self.save = save
+        self.debug = debug
+
+    def gql(self, method: str, operation: tuple, variables: dict, features: dict = Operation.default_features) -> dict:
+        qid, op = operation
+        params = {
+            'queryId': qid,
+            'features': features,
+            'variables': variables | Operation.default_variables
+        }
+        if method == 'POST':
+            data = {'json': params}
+        else:
+            data = {'params': {k: orjson.dumps(v).decode() for k, v in params.items()}}
+        r = self.session.request(
+            method=method,
+            url=f'{self.gql_url}/{qid}/{op}',
+            headers=get_headers(self.session),
+            **data
+        )
+        if self.debug:
+            self.log(r)
+        if self.save:
+            save_data(r.json(), op, self.session.cookies.get('username', '_'))
+        return r.json()
 
-    def gql(self, operation: tuple, variables: dict) -> Response:
-        name, _ = operation
-        payload = deepcopy(operations[name])
-        qid = payload['queryId']
-        payload['variables'] |= variables
-        url = f"{self.GRAPHQL_URL}/{qid}/{name}"
-        r = self.session.post(url, headers=get_headers(self.session), json=payload)
-        self.check_response(r)
-        return r
-
-    def api(self, path: str, settings: dict) -> Response:
+    def v1(self, path: str, params: dict) -> dict:
         headers = get_headers(self.session)
         headers['content-type'] = 'application/x-www-form-urlencoded'
-        url = f'{self.V1_URL}/{path}'
-        r = self.session.post(url, headers=headers, data=urlencode(settings))
-        self.check_response(r)
-        return r
-
-    @log(info=['json'])
-    def dm(self, receivers: list[int], text: str, filename: str = '') -> Response:
-        name, _ = Operation.Account.useSendMessageMutation
-        params = deepcopy(operations[name])
-        qid = params['queryId']
-        params['variables']['target'] = {"participant_ids": receivers}
-        params['variables']['requestId'] = str(uuid1(getnode()))  # can be anything
-        url = f"{self.GRAPHQL_URL}/{qid}/{name}"
-        if filename:
-            media_id = self.upload_media(filename, is_dm=True)
-            params['variables']['message']['media'] = {'id': media_id, 'text': text}
-        else:
-            params['variables']['message']['text'] = {'text': text}
-        r = self.session.post(url, headers=get_headers(self.session), json=params)
-        return r
-
-    @log(info=['json'])
-    def tweet(self, text: str, media: list = None, **kwargs) -> Response:
-        name, _ = Operation.Account.CreateTweet
-        params = deepcopy(operations[name])
-        qid = params['queryId']
-        params['variables']['tweet_text'] = text
-        if media:
-            for m in media:
-                if isinstance(m, dict):
-                    media_id = self.upload_media(m['file'])
-                    params['variables']['media']['media_entities'].append({
-                        'media_id': media_id,
-                        'tagged_users': m.get('tagged_users', [])
-                    })
-                    if alt := m.get('alt'):
-                        self.add_alt_text(media_id, alt)
-                # for convenience, so we can just pass list of strings
-                elif isinstance(m, str):
-                    media_id = self.upload_media(m)
-                    params['variables']['media']['media_entities'].append({
-                        'media_id': media_id,
-                        'tagged_users': []
-                    })
-
-        if reply_params := kwargs.get('reply_params', {}):
-            params['variables'] |= reply_params
-        if quote_params := kwargs.get('quote_params', {}):
-            params['variables'] |= quote_params
-        if poll_params := kwargs.get('poll_params', {}):
-            params['variables'] |= poll_params
-
-        url = f"{self.GRAPHQL_URL}/{qid}/{name}"
-        r = self.session.post(url, headers=get_headers(self.session), json=params)
-        return r
-
-    @log(info=['json'])
-    def schedule_tweet(self, text: str, execute_at: any, *, reply_to: int = None,
-                       media: list = None) -> Response:
-        name, _ = Operation.Account.CreateScheduledTweet
-        params = deepcopy(operations[name])
-        qid = params['queryId']
-        params['variables']['post_tweet_request']['status'] = text
-        params['variables']['execute_at'] = (
-            datetime.strptime(execute_at, "%Y-%m-%d %H:%M").timestamp()
-            if isinstance(execute_at, str)
-            else execute_at
-        )
-        if reply_to:
-            params['variables']['post_tweet_request']['in_reply_to_status_id'] = reply_to
-        if media:
-            for m in media:
-                if isinstance(m, dict):
-                    media_id = self.upload_media(m['file'])
-                    params['variables']['post_tweet_request']['media_ids'].append(media_id)
-                    if alt := m.get('alt'):
-                        self.add_alt_text(self.session, media_id, alt)
-                # for convenience, so we can just pass list of strings
-                elif isinstance(m, str):
-                    media_id = self.upload_media(m)
-                    params['variables']['post_tweet_request']['media_ids'].append(media_id)
-        url = f"{self.GRAPHQL_URL}/{qid}/{name}"
-        r = self.session.post(url, headers=get_headers(self.session), json=params)
-        return r
+        r = self.session.post(f'{self.v1_url}/{path}', headers=headers, data=urlencode(params))
+        if self.debug:
+            self.log(r)
+        if self.save:
+            save_data(r.json(), '_', self.session.cookies.get('username', '_'))
+        return r.json()
 
-    @log(info=['json'])
-    def create_poll(self, text: str, choices: list[str], poll_duration: int) -> Response:
+    def create_poll(self, text: str, choices: list[str], poll_duration: int) -> dict:
         options = {
             "twitter:card": "poll4choice_text_only",
             "twitter:api:api:endpoint": "1",
             "twitter:long:duration_minutes": poll_duration  # max: 10080
         }
         for i, c in enumerate(choices):
             options[f"twitter:string:choice{i + 1}_label"] = c
@@ -222,429 +107,473 @@
         headers['content-type'] = 'application/x-www-form-urlencoded'
         url = 'https://caps.twitter.com/v2/cards/create.json'
         r = self.session.post(url, headers=headers, params={'card_data': orjson.dumps(options).decode()})
         card_uri = r.json()['card_uri']
         r = self.tweet(text, poll_params={'card_uri': card_uri})
         return r
 
-    def check_media(self, category: str, total_bytes: int) -> None:
-        def check(media):
-            name, size = media
-            fmt = lambda x: f'{(x / 1e6):.2f} MB'
-            if name in category and total_bytes > size:
-                raise Exception(f'cannot upload {fmt(total_bytes)} {name}: max {name} size is {fmt(size)}')
-
-        tuple(map(check, (Media.Type.image, Media.Type.gif, Media.Type.video)))
-
-    def upload_media(self, filename: str, is_dm: bool = False, is_profile=False) -> int:
-        if is_profile:
-            url = 'https://upload.twitter.com/i/media/upload.json'
+    def dm(self, text: str, receivers: list[int], media: str = '') -> dict:
+        variables = {
+            "message": {},
+            "requestId": str(uuid1(getnode())),
+            "target": {"participant_ids": receivers},
+        }
+        if media:
+            media_id = self._upload_media(media, is_dm=True)
+            variables['message']['media'] = {'id': media_id, 'text': text}
         else:
-            url = 'https://upload.twitter.com/1.1/media/upload.json'
+            variables['message']['text'] = {'text': text}
+        return self.gql('POST', Operation.useSendMessageMutation, variables)
 
-        file = Path(filename)
-        total_bytes = file.stat().st_size
-        headers = get_headers(self.session)
+    def tweet(self, text: str, *, media: any = None, **kwargs) -> dict:
+        variables = {
+            'tweet_text': text,
+            'dark_request': False,
+            'media': {
+                'media_entities': [],
+                'possibly_sensitive': False,
+            },
+            'semantic_annotation_ids': [],
+        }
+        if media:
+            for m in media:
+                media_id = self._upload_media(m['media'])
+                variables['media']['media_entities'].append({
+                    'media_id': media_id,
+                    'tagged_users': m.get('tagged_users', [])
+                })
+                if alt := m.get('alt'):
+                    self._add_alt_text(media_id, alt)
+        if reply_params := kwargs.get('reply_params', {}):
+            variables |= reply_params
+        if quote_params := kwargs.get('quote_params', {}):
+            variables |= quote_params
+        if poll_params := kwargs.get('poll_params', {}):
+            variables |= poll_params
+        return self.gql('POST', Operation.CreateTweet, variables)
 
-        upload_type = 'dm' if is_dm else 'tweet'
-        media_type = mimetypes.guess_type(file)[0]
-        media_category = f'{upload_type}_{media_type.split("/")[0]}'
+    def schedule_tweet(self, text: str, date: int | str, *, media: list = None) -> dict:
+        variables = {
+            'post_tweet_request': {
+                'auto_populate_reply_metadata': False,
+                'status': text,
+                'exclude_reply_user_ids': [],
+                'media_ids': [],
+            },
+            'execute_at': (
+                datetime.strptime(date, "%Y-%m-%d %H:%M").timestamp()
+                if isinstance(date, str)
+                else date
+            ),
+        }
+        if media:
+            for m in media:
+                media_id = self._upload_media(m['media'])
+                variables['post_tweet_request']['media_ids'].append(media_id)
+                if alt := m.get('alt'):
+                    self._add_alt_text(media_id, alt)
+        return self.gql('POST', Operation.CreateScheduledTweet, variables)
 
-        self.check_media(media_category, total_bytes)
+    def schedule_reply(self, text: str, date: int | str, tweet_id: int, *, media: list = None) -> dict:
+        variables = {
+            'post_tweet_request': {
+                'auto_populate_reply_metadata': True,
+                'in_reply_to_status_id': tweet_id,
+                'status': text,
+                'exclude_reply_user_ids': [],
+                'media_ids': [],
+            },
+            'execute_at': (
+                datetime.strptime(date, "%Y-%m-%d %H:%M").timestamp()
+                if isinstance(date, str)
+                else date
+            ),
+        }
+        if media:
+            for m in media:
+                media_id = self._upload_media(m['media'])
+                variables['post_tweet_request']['media_ids'].append(media_id)
+                if alt := m.get('alt'):
+                    self._add_alt_text(media_id, alt)
+        return self.gql('POST', Operation.CreateScheduledTweet, variables)
 
-        data = {'command': 'INIT', 'media_type': media_type, 'total_bytes': total_bytes,
-                'media_category': media_category}
-        r = self.session.post(url=url, headers=headers, data=data)
-        media_id = r.json()['media_id']
+    def unschedule_tweet(self, tweet_id: int) -> dict:
+        variables = {
+            'scheduled_tweet_id': tweet_id,
+        }
+        return self.gql('POST', Operation.DeleteScheduledTweet, variables)
 
-        desc = f"uploading: {file.name}"
-        with tqdm(total=total_bytes, desc=desc, unit='B', unit_scale=True, unit_divisor=1024) as pbar:
-            with open(file, 'rb') as f:
-                i = 0
-                while chunk := f.read(UPLOAD_CHUNK_SIZE):  # todo: arbitrary max size for now
-                    data = {'command': 'APPEND', 'media_id': media_id, 'segment_index': i}
-                    files = {'media': chunk}
-                    r = self.session.post(url=url, headers=headers, data=data, files=files)
-                    if r.status_code < 200 or r.status_code > 299:
-                        logger.debug(f'{r.status_code} {r.text}')
-                        raise Exception(f'[{ERROR}error{RESET}] upload failed')
-                    i += 1
-                    pbar.update(f.tell() - pbar.n)
+    def untweet(self, tweet_id: int) -> dict:
+        variables = {
+            'tweet_id': tweet_id,
+            'dark_request': False,
+        }
+        return self.gql('POST', Operation.DeleteTweet, variables)
 
-        data = {'command': 'FINALIZE', 'media_id': media_id, 'allow_async': 'true'}
-        if is_dm:
-            data |= {'original_md5': hashlib.md5(file.read_bytes()).hexdigest()}
-        r = self.session.post(url=url, headers=headers, data=data)
+    def reply(self, text: str, tweet_id: int) -> dict:
+        variables = {
+            'tweet_text': text,
+            'reply': {
+                'in_reply_to_tweet_id': tweet_id,
+                'exclude_reply_user_ids': [],
+            },
+            'batch_compose': 'BatchSubsequent',
+            'dark_request': False,
+            'media': {
+                'media_entities': [],
+                'possibly_sensitive': False,
+            },
+            'semantic_annotation_ids': [],
+        }
+        return self.gql('POST', Operation.CreateTweet, variables)
 
-        logger.debug(f'processing, please wait...')
-        processing_info = r.json().get('processing_info')
-        while processing_info:
-            state = processing_info['state']
-            logger.debug(f'{processing_info = }')
-            if state == MEDIA_UPLOAD_SUCCEED:
-                break
-            if state == MEDIA_UPLOAD_FAIL:
-                raise Exception(f'[{ERROR}error{RESET}] media processing failed')
-            check_after_secs = processing_info.get('check_after_secs', random.randint(1, 5))
-            time.sleep(check_after_secs)
-            params = {'command': 'STATUS', 'media_id': media_id}
-            r = self.session.get(url=url, headers=headers, params=params)
-            processing_info = r.json().get('processing_info')
-        logger.debug('processing complete')
+    def quote(self, text: str, tweet_id: int) -> dict:
+        variables = {
+            'tweet_text': text,
+            # can use `i` as it resolves to screen_name
+            'attachment_url': f'https://twitter.com/i/status/{tweet_id}',
+            'dark_request': False,
+            'media': {
+                'media_entities': [],
+                'possibly_sensitive': False,
+            },
+            'semantic_annotation_ids': [],
+        }
+        return self.gql('POST', Operation.CreateTweet, variables)
 
-        return media_id
+    def retweet(self, tweet_id: int) -> dict:
+        variables = {
+            "tweet_id": tweet_id,
+            "dark_request": False
+        }
+        return self.gql('POST', Operation.CreateRetweet, variables)
 
-    @log(info=['text'])
-    def add_alt_text(self, media_id: int, text: str) -> Response:
-        params = {"media_id": media_id, "alt_text": {"text": text}}
-        url = f'{self.V1_URL}/media/metadata/create.json'
-        r = self.session.post(url, headers=get_headers(self.session), json=params)
-        return r
+    def unretweet(self, tweet_id: int) -> dict:
+        variables = {
+            "source_tweet_id": tweet_id,
+            "dark_request": False
+        }
+        return self.gql('POST', Operation.DeleteRetweet, variables)
 
-    def reply(self, tweet_id: int, text: str, media: list = None) -> Response:
-        """ an un-reply operation is just DeleteTweet"""
-        params = {"reply": {"in_reply_to_tweet_id": tweet_id, "exclude_reply_user_ids": []}}
-        return self.tweet(text, media, reply_params=params)
-
-    def quote(self, tweet_id: int, screen_name: str, text: str, media: list = None) -> Response:
-        """ an un-quote operation is just DeleteTweet"""
-        params = {"attachment_url": f"https://twitter.com/{screen_name}/status/{tweet_id}"}
-        return self.tweet(text, media, quote_params=params)
-
-    @log(info=['json'])
-    def unschedule_tweet(self, tweet_id: int) -> Response:
-        return self.gql(Operation.Account.DeleteScheduledTweet, {'scheduled_tweet_id': tweet_id})
-
-    @log(info=['json'])
-    def untweet(self, tweet_id: int) -> Response:
-        return self.gql(Operation.Account.DeleteTweet, {'tweet_id': tweet_id})
-
-    @log(info=['json'])
-    def retweet(self, tweet_id: int) -> Response:
-        return self.gql(Operation.Account.CreateRetweet, {'tweet_id': tweet_id})
-
-    @log(info=['json'])
-    def unretweet(self, tweet_id: int) -> Response:
-        return self.gql(Operation.Account.DeleteRetweet, {'source_tweet_id': tweet_id})
-
-    @log(info=['json'])
-    def like(self, tweet_id: int) -> Response:
-        return self.gql(Operation.Account.FavoriteTweet, {'tweet_id': tweet_id})
-
-    @log(info=['json'])
-    def unlike(self, tweet_id: int) -> Response:
-        return self.gql(Operation.Account.UnfavoriteTweet, {'tweet_id': tweet_id})
-
-    @log(info=['json'])
-    def bookmark(self, tweet_id: int) -> Response:
-        return self.gql(Operation.Account.CreateBookmark, {'tweet_id': tweet_id})
-
-    @log(info=['json'])
-    def unbookmark(self, tweet_id: int) -> Response:
-        return self.gql(Operation.Account.DeleteBookmark, {'tweet_id': tweet_id})
-
-    @log(info=['json'])
-    def home_timeline(self):
-        return self.gql(Operation.Account.HomeTimeline, {})
-
-    def home_latest_timeline(self, limit: int = 100):
-        r = self.gql(Operation.Account.HomeLatestTimeline, {})
-        data = r.json() | {ID: self.session.cookies.get('username')}
-        return self.paginate(self.session, data, Operation.Account.HomeLatestTimeline, limit)
-
-    # todo: a lot of duplicated code here, will need to refactor
-    def paginate(self, session: Session, data: dict, operation: tuple, limit: int):
-
-        def get_cursor(data):
-            # inefficient, but need to deal with arbitrary schema
-            entries = find_key(data, 'entries')
-            if entries:
-                for entry in entries.pop():
-                    if entry.get('entryId', '').startswith('cursor-bottom'):
-                        content = entry['content']
-                        if itemContent := content.get('itemContent'):
-                            return itemContent['value']  # v2 cursor
-                        return content['value']  # v1 cursor
-
-        all_data = []
-        try:
-            name, key = operation
-            params = deepcopy(operations[name])
-            ids = set()
-            counts = []
-            # params['variables'][key] = data[ID]
-            cursor = get_cursor(data)
-            while 1:
-                params['variables']['cursor'] = cursor
+    def like(self, tweet_id: int) -> dict:
+        variables = {'tweet_id': tweet_id}
+        return self.gql('POST', Operation.FavoriteTweet, variables)
 
-                r = self.gql(operation, params['variables'])
-                _data = r.json()
+    def unlike(self, tweet_id: int) -> dict:
+        variables = {'tweet_id': tweet_id}
+        return self.gql('POST', Operation.UnfavoriteTweet, variables)
 
-                if csrf := r.cookies.get("ct0"):
-                    session.headers.update({"x-csrf-token": csrf.value})
-                session.cookies.update(r.cookies)
-
-                path = Path(f'data/raw/{data[ID]}')
-                path.mkdir(parents=True, exist_ok=True)
-                (path / f'{time.time_ns()}_{name}.json').write_text(
-                    orjson.dumps(_data, option=orjson.OPT_INDENT_2).decode(),
-                    encoding='utf-8'
-                )
-
-                all_data.append(_data)
-                cursor = get_cursor(_data)
-                logger.debug(f'{cursor = }')
-                ids |= set(find_key(_data, 'rest_id'))
-                logger.debug(f'({data[ID]})\t{len(ids)} unique results')
-                counts.append(len(ids))
-
-                success_message = f'[{SUCCESS}success{RESET}] done pagination'
-                # followers/following have "0|"
-                if not cursor or cursor.startswith('0|'):
-                    logger.debug(f'{success_message}\tlast cursor: {cursor}')
-                    break
-                if len(ids) >= limit:
-                    logger.debug(f'{success_message}\tsurpassed limit of {limit} results')
-                    break
-                # did last 5 requests return duplicate data?
-                if len(counts) > DUP_LIMIT and len(set(counts[-1:-DUP_LIMIT:-1])) == 1:
-                    logger.debug(f'{success_message}\tpast {DUP_LIMIT} requests returned duplicate data')
-                    break
-
-        except Exception as e:
-            logger.debug(f'[{ERROR}error{RESET}] paginate falied: {e}')
-        # save_data(all_data, name)
-        return all_data
+    def bookmark(self, tweet_id: int) -> dict:
+        variables = {'tweet_id': tweet_id}
+        return self.gql('POST', Operation.CreateBookmark, variables)
 
-    @log(info=['json'])
-    def create_list(self, name: str, description: str, private: bool) -> Response:
+    def unbookmark(self, tweet_id: int) -> dict:
+        variables = {'tweet_id': tweet_id}
+        return self.gql('POST', Operation.DeleteBookmark, variables)
+
+    def create_list(self, name: str, description: str, private: bool) -> dict:
         variables = {
             "isPrivate": private,
             "name": name,
             "description": description,
         }
-        return self.gql(Operation.Account.CreateList, variables)
+        return self.gql('POST', Operation.CreateList, variables)
 
-    @log(info=['json'])
-    def update_list(self, list_id: int, name: str, description: str, private: bool) -> Response:
+    def update_list(self, list_id: int, name: str, description: str, private: bool) -> dict:
         variables = {
             "listId": list_id,
             "isPrivate": private,
             "name": name,
             "description": description,
         }
-        return self.gql(Operation.Account.UpdateList, variables)
+        return self.gql('POST', Operation.UpdateList, variables)
 
-    @log(info=['json'])
-    def update_pinned_lists(self, list_ids: list[int]) -> Response:
+    def update_pinned_lists(self, list_ids: list[int]) -> dict:
         """
-        Update pinned lists
-
+        Update pinned lists.
         Reset all pinned lists and pin all specified lists in the order they are provided.
 
         @param list_ids: list of list ids to pin
         @return: response
         """
-        return self.gql(Operation.Account.ListsPinMany, {'listIds': list_ids})
+        return self.gql('POST', Operation.ListsPinMany, {'listIds': list_ids})
+
+    def pin_list(self, list_id: int) -> dict:
+        return self.gql('POST', Operation.ListPinOne, {'listId': list_id})
+
+    def unpin_list(self, list_id: int) -> dict:
+        return self.gql('POST', Operation.ListUnpinOne, {'listId': list_id})
+
+    def add_list_member(self, list_id: int, user_id: int) -> dict:
+        return self.gql('POST', Operation.ListAddMember, {'listId': list_id, "userId": user_id})
+
+    def remove_list_member(self, list_id: int, user_id: int) -> dict:
+        return self.gql('POST', Operation.ListRemoveMember, {'listId': list_id, "userId": user_id})
+
+    def delete_list(self, list_id: int) -> dict:
+        return self.gql('POST', Operation.DeleteList, {'listId': list_id})
 
-    @log(info=['json'])
-    def pin_list(self, list_id: int) -> Response:
-        return self.gql(Operation.Account.ListPinOne, {'listId': list_id})
-
-    @log(info=['json'])
-    def unpin_list(self, list_id: int) -> Response:
-        return self.gql(Operation.Account.ListUnpinOne, {'listId': list_id})
-
-    @log(info=['json'])
-    def add_list_member(self, list_id: int, user_id: int) -> Response:
-        return self.gql(Operation.Account.ListAddMember, {'listId': list_id, "userId": user_id})
-
-    @log(info=['json'])
-    def remove_list_member(self, list_id: int, user_id: int) -> Response:
-        return self.gql(Operation.Account.ListRemoveMember, {'listId': list_id, "userId": user_id})
-
-    @log(info=['json'])
-    def delete_list(self, list_id: int) -> Response:
-        return self.gql(Operation.Account.DeleteList, {'listId': list_id})
-
-    @log(info=['json'])
-    def update_list_banner(self, list_id: int, filename: str) -> Response:
-        media_id = self.upload_media(filename)
-        return self.gql(Operation.Account.EditListBanner, {'listId': list_id, 'mediaId': media_id})
-
-    @log(info=['json'])
-    def delete_list_banner(self, list_id: int) -> Response:
-        return self.gql(Operation.Account.DeleteListBanner, {'listId': list_id})
-
-    @log(info=['json'])
-    def unfollow_topic(self, topic_id: int) -> Response:
-        return self.gql(Operation.Account.TopicUnfollow, {'topicId': str(topic_id)})
-
-    @log(info=['json'])
-    def follow_topic(self, topic_id: int) -> Response:
-        return self.gql(Operation.Account.TopicFollow, {'topicId': str(topic_id)})
-
-    @log(info=['json'])
-    def follow(self, user_id: int) -> Response:
-        settings = follow_settings.copy()
+    def update_list_banner(self, list_id: int, media: str) -> dict:
+        media_id = self._upload_media(media)
+        variables = {'listId': list_id, 'mediaId': media_id}
+        return self.gql('POST', Operation.EditListBanner, variables)
+
+    def delete_list_banner(self, list_id: int) -> dict:
+        return self.gql('POST', Operation.DeleteListBanner, {'listId': list_id})
+
+    def follow_topic(self, topic_id: int) -> dict:
+        variables = {'topicId': str(topic_id)}
+        return self.gql('POST', Operation.TopicFollow, variables)
+
+    def unfollow_topic(self, topic_id: int) -> dict:
+        variables = {'topicId': str(topic_id)}
+        return self.gql('POST', Operation.TopicUnfollow, variables)
+
+    def pin(self, tweet_id: int) -> dict:
+        params = {'tweet_mode': 'extended', 'id': tweet_id}
+        return self.v1('account/pin_tweet.json', params)
+
+    def unpin(self, tweet_id: int) -> dict:
+        params = {'tweet_mode': 'extended', 'id': tweet_id}
+        return self.v1('account/unpin_tweet.json', params)
+
+    def follow(self, user_id: int) -> dict:
+        settings = deepcopy(follow_settings)
         settings |= {"user_id": user_id}
-        return self.api('friendships/create.json', settings)
+        return self.v1('friendships/create.json', settings)
 
-    @log(info=['json'])
-    def unfollow(self, user_id: int) -> Response:
-        settings = follow_settings.copy()
+    def unfollow(self, user_id: int) -> dict:
+        settings = deepcopy(follow_settings)
         settings |= {"user_id": user_id}
-        return self.api('friendships/destroy.json', settings)
+        return self.v1('friendships/destroy.json', settings)
 
-    @log(info=['json'])
-    def mute(self, user_id: int) -> Response:
-        settings = {'user_id': user_id}
-        return self.api('mutes/users/create.json', settings)
-
-    @log(info=['json'])
-    def unmute(self, user_id: int) -> Response:
-        settings = {'user_id': user_id}
-        return self.api('mutes/users/destroy.json', settings)
-
-    @log(info=['json'])
-    def enable_notifications(self, user_id: int) -> Response:
-        settings = notification_settings.copy()
+    def mute(self, user_id: int) -> dict:
+        params = {'user_id': user_id}
+        return self.v1('mutes/users/create.json', params)
+
+    def unmute(self, user_id: int) -> dict:
+        params = {'user_id': user_id}
+        return self.v1('mutes/users/destroy.json', params)
+
+    def enable_notifications(self, user_id: int) -> dict:
+        settings = deepcopy(notification_settings)
         settings |= {'id': user_id, 'device': 'true'}
-        return self.api('friendships/update.json', settings)
+        return self.v1('friendships/update.json', settings)
 
-    @log(info=['json'])
-    def disable_notifications(self, user_id: int) -> Response:
-        settings = notification_settings.copy()
+    def disable_notifications(self, user_id: int) -> dict:
+        settings = deepcopy(notification_settings)
         settings |= {'id': user_id, 'device': 'false'}
-        return self.api('friendships/update.json', settings)
+        return self.v1('friendships/update.json', settings)
 
-    @log(info=['json'])
-    def block(self, user_id: int) -> Response:
-        settings = {'user_id': user_id}
-        return self.api('blocks/create.json', settings)
-
-    @log(info=['json'])
-    def unblock(self, user_id: int) -> Response:
-        settings = {'user_id': user_id}
-        return self.api('blocks/destroy.json', settings)
-
-    @log(info=['json'])
-    def pin(self, tweet_id: int) -> Response:
-        settings = {'tweet_mode': 'extended', 'id': tweet_id}
-        return self.api('account/pin_tweet.json', settings)
-
-    @log(info=['json'])
-    def unpin(self, tweet_id: int) -> Response:
-        settings = {'tweet_mode': 'extended', 'id': tweet_id}
-        return self.api('account/unpin_tweet.json', settings)
-
-    @log(info=['json'])
-    def stats(self, rest_id: int) -> Response:
-        """private endpoint?"""
-        name, _ = Operation.Account.TweetStats
-        params = deepcopy(operations[name])
-        qid = params['queryId']
-        params['variables']['rest_id'] = rest_id
-        query = build_query(params)
-        url = f"{self.GRAPHQL_URL}/{qid}/{name}?{query}"
-        r = self.session.get(url, headers=get_headers(self.session))
-        return r
-
-    @log(info=['json'])
-    def remove_interests(self, *args):
-        url = f'{self.V1_URL}/account/personalization/twitter_interests.json'
-        r = self.session.get(url, headers=get_headers(self.session))
-        current_interests = r.json()['interested_in']
-        if args == 'all':
-            disabled_interests = [x['id'] for x in current_interests]
-        else:
-            disabled_interests = [x['id'] for x in current_interests if x['display_name'] in args]
-        payload = {
-            "preferences": {
-                "interest_preferences": {
-                    "disabled_interests": disabled_interests,
-                    "disabled_partner_interests": []
-                }
-            }
-        }
-        url = f'{self.V1_URL}/account/personalization/p13n_preferences.json'
-        r = self.session.post(url, headers=get_headers(self.session), json=payload)
-        return r
-
-    @log(info=['json'])
-    def update_profile_image(self, filename: str) -> Response:
-        media_id = self.upload_media(filename, is_profile=True)
-        url = f'{self.V1_URL}/account/update_profile_image.json'
+    def block(self, user_id: int) -> dict:
+        params = {'user_id': user_id}
+        return self.v1('blocks/create.json', params)
+
+    def unblock(self, user_id: int) -> dict:
+        params = {'user_id': user_id}
+        return self.v1('blocks/destroy.json', params)
+
+    def update_profile_image(self, media: str) -> Response:
+        media_id = self._upload_media(media, is_profile=True)
+        url = f'{self.v1_url}/account/update_profile_image.json'
         headers = get_headers(self.session)
         params = {'media_id': media_id}
         r = self.session.post(url, headers=headers, params=params)
         return r
 
-    @log
-    def update_profile_banner(self, filename: str) -> Response:
-        media_id = self.upload_media(filename, is_profile=True)
-        url = f'{self.V1_URL}/account/update_profile_banner.json'
+    def update_profile_banner(self, media: str) -> Response:
+        media_id = self._upload_media(media, is_profile=True)
+        url = f'{self.v1_url}/account/update_profile_banner.json'
         headers = get_headers(self.session)
         params = {'media_id': media_id}
         r = self.session.post(url, headers=headers, params=params)
         return r
 
-    @log
     def update_profile_info(self, **kwargs) -> Response:
-        url = f'{self.V1_URL}/account/update_profile.json'
+        url = f'{self.v1_url}/account/update_profile.json'
         headers = get_headers(self.session)
         r = self.session.post(url, headers=headers, params=kwargs)
         return r
 
-    @log(info=['text'])
     def update_search_settings(self, settings: dict) -> Response:
-        """
-        Update account search settings
-
-        @param settings: search filtering settings to enable/disable
-        @return: authenticated session
-        """
-        twid = int(self.session.cookies.get_dict()['twid'].split('=')[-1].strip('"'))
+        twid = int(self.session.cookies.get('twid').split('=')[-1].strip('"'))
         headers = get_headers(self.session)
         r = self.session.post(
-            url=f'{self.V1_URL}/strato/column/User/{twid}/search/searchSafety',
+            url=f'{self.v1_url}/strato/column/User/{twid}/search/searchSafety',
             headers=headers,
             json=settings,
         )
+        logger.debug(r)
         return r
 
-    @log(info=['json'])
-    def update_settings(self, settings: dict) -> Response:
-        """
-        Update account settings
-    
-        @param settings: settings to enable/disable
-        @return: authenticated session
-        """
-        return self.api('account/settings.json', settings)
+    def update_settings(self, settings: dict) -> dict:
+        return self.v1('account/settings.json', settings)
 
-    @log(info=['json'])
-    def change_password(self, old: str, new: str) -> Response:
-        settings = {
+    def change_password(self, old: str, new: str) -> dict:
+        params = {
             'current_password': old,
             'password': new,
             'password_confirmation': new
         }
         headers = get_headers(self.session)
         headers['content-type'] = 'application/x-www-form-urlencoded'
         url = 'https://twitter.com/i/api/i/account/change_password.json'
-        r = self.session.post(url, headers=headers, data=urlencode(settings))
+        r = self.session.post(url, headers=headers, data=urlencode(params))
+        return r.json()
+
+    def remove_interests(self, *args):
+        """
+        Pass 'all' to remove all interests
+        """
+        r = self.session.get(
+            f'{self.v1_url}/account/personalization/twitter_interests.json',
+            headers=get_headers(self.session)
+        )
+        current_interests = r.json()['interested_in']
+        if args == 'all':
+            disabled_interests = [x['id'] for x in current_interests]
+        else:
+            disabled_interests = [x['id'] for x in current_interests if x['display_name'] in args]
+        payload = {
+            "preferences": {
+                "interest_preferences": {
+                    "disabled_interests": disabled_interests,
+                    "disabled_partner_interests": []
+                }
+            }
+        }
+        r = self.session.post(
+            f'{self.v1_url}/account/personalization/p13n_preferences.json',
+            headers=get_headers(self.session),
+            json=payload
+        )
         return r
 
-    @log(info=['json'])
-    def logout_all_sessions(self) -> Response:
+    def home_timeline(self, limit=math.inf) -> list[dict]:
+        return self._paginate('POST', Operation.HomeTimeline, Operation.default_variables, limit)
+
+    def home_latest_timeline(self, limit=math.inf) -> list[dict]:
+        return self._paginate('POST', Operation.HomeLatestTimeline, Operation.default_variables, limit)
+
+    def bookmarks(self, limit=math.inf) -> list[dict]:
+        return self._paginate('GET', Operation.Bookmarks, {}, limit)
+
+    def _paginate(self, method: str, operation: tuple, variables: dict, limit: int) -> list[dict]:
+        initial_data = self.gql(method, operation, variables)
+        res = [initial_data]
+        ids = set(find_key(initial_data, 'rest_id'))
+        dups = 0
+        DUP_LIMIT = 3
+
+        cursor = get_cursor(initial_data)
+        while (dups < DUP_LIMIT) and cursor:
+            prev_len = len(ids)
+            if prev_len >= limit:
+                return res
+
+            variables['cursor'] = cursor
+            data = self.gql(method, operation, variables)
+
+            cursor = get_cursor(data)
+            ids |= set(find_key(data, 'rest_id'))
+
+            if self.debug:
+                logger.debug(f'cursor: {cursor}\tunique results: {len(ids)}')
+
+            if prev_len == len(ids):
+                dups += 1
+
+            res.append(data)
+        return res
+
+    def _upload_media(self, filename: str, is_dm: bool = False, is_profile=False) -> int | None:
+
+        def check_media(category: str, size: int) -> None:
+            fmt = lambda x: f'{(x / 1e6):.2f} MB'
+            msg = lambda x: f'cannot upload {fmt(size)} {category}, max size is {fmt(x)}'
+            if category == 'image' and size > MAX_IMAGE_SIZE:
+                raise Exception(msg(MAX_IMAGE_SIZE))
+            if category == 'gif' and size > MAX_GIF_SIZE:
+                raise Exception(msg(MAX_GIF_SIZE))
+            if category == 'video' and size > MAX_VIDEO_SIZE:
+                raise Exception(msg(MAX_VIDEO_SIZE))
+
+        if is_profile:
+            url = 'https://upload.twitter.com/i/media/upload.json'
+        else:
+            url = 'https://upload.twitter.com/1.1/media/upload.json'
+
+        file = Path(filename)
+        total_bytes = file.stat().st_size
         headers = get_headers(self.session)
-        url = 'https://twitter.com/i/api/account/self.sessions/revoke_all'
-        r = self.session.post(url, headers=headers)
+
+        upload_type = 'dm' if is_dm else 'tweet'
+        media_type = mimetypes.guess_type(file)[0]
+        media_category = f'{upload_type}_gif' if 'gif' in media_type else f'{upload_type}_{media_type.split("/")[0]}'
+
+        check_media(media_category, total_bytes)
+
+        data = {'command': 'INIT', 'media_type': media_type, 'total_bytes': total_bytes,
+                'media_category': media_category}
+        r = self.session.post(url=url, headers=headers, data=data)
+        media_id = r.json()['media_id']
+
+        desc = f"uploading: {file.name}"
+        with tqdm(total=total_bytes, desc=desc, unit='B', unit_scale=True, unit_divisor=1024) as pbar:
+            with open(file, 'rb') as f:
+                i = 0
+                while chunk := f.read(UPLOAD_CHUNK_SIZE):  # todo: arbitrary max size for now
+                    data = {'command': 'APPEND', 'media_id': media_id, 'segment_index': i}
+                    files = {'media': chunk}
+                    r = self.session.post(url=url, headers=headers, data=data, files=files)
+                    if r.status_code < 200 or r.status_code > 299:
+                        logger.debug(f'{r.status_code} {r.text}')
+                        raise Exception(f'[{RED}error{RESET}] upload failed')
+                    i += 1
+                    pbar.update(f.tell() - pbar.n)
+
+        data = {'command': 'FINALIZE', 'media_id': media_id, 'allow_async': 'true'}
+        if is_dm:
+            data |= {'original_md5': hashlib.md5(file.read_bytes()).hexdigest()}
+        r = self.session.post(url=url, headers=headers, data=data)
+
+        # logger.debug(f'processing, please wait...')
+        processing_info = r.json().get('processing_info')
+        while processing_info:
+            state = processing_info['state']
+            if error := processing_info.get("error"):
+                raise Exception(f'media upload failed: {error}')
+            if state == MEDIA_UPLOAD_SUCCEED:
+                break
+            if state == MEDIA_UPLOAD_FAIL:
+                raise Exception(f'[{RED}error{RESET}] media processing failed')
+            check_after_secs = processing_info.get('check_after_secs', random.randint(1, 5))
+            time.sleep(check_after_secs)
+            params = {'command': 'STATUS', 'media_id': media_id}
+            r = self.session.get(url=url, headers=headers, params=params)
+            processing_info = r.json().get('processing_info')
+        # logger.debug('processing complete')
+        return media_id
+
+    def _add_alt_text(self, media_id: int, text: str) -> Response:
+        params = {"media_id": media_id, "alt_text": {"text": text}}
+        url = f'{self.v1_url}/media/metadata/create.json'
+        r = self.session.post(url, headers=get_headers(self.session), json=params)
         return r
 
-    @staticmethod
-    def check_response(r):
-        if r.status_code == 429:
-            raise Exception(f'rate limit exceeded: {r.url}')
-        if find_key(data := r.json(), 'errors'):
-            logger.debug(f'[{ERROR}error{RESET}] {data}')
+    def log(self, response: Response):
+        status = fmt_status(response.status_code)
+        if 'json' in response.headers.get('content-type', ''):
+            if response.json().get('errors'):
+                logger.debug(f'[{RED}twitter error{RESET}]')
+                logger.debug(f'{response.url}')
+                logger.debug(f'{response.text}')
+                return
+        logger.debug(status)
+        if self.debug >= 1:
+            logger.debug(f'{response.url}')
+        if self.debug >= 2:
+            logger.debug(f'{response.text}')
+        if self.debug >= 3:
+            logger.debug(f'{response.headers}')
+        if self.debug >= 4:
+            logger.debug(f'{response.cookies}')
```

### Comparing `twitter-api-client-0.6.5/twitter/login.py` & `twitter-api-client-0.6.6/twitter/login.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,99 +1,104 @@
 import sys
 
 from requests import Session
 
-from .constants import SUCCESS, WARN, ERROR, BOLD, RESET
-from .utils import find_key
+from .constants import GREEN, YELLOW, RED, BOLD, RESET
+from .util import find_key
 
 
-def update_token(session: Session, key: str, url: str, payload: dict) -> Session:
+def update_token(session: Session, key: str, url: str, **kwargs) -> Session:
     caller_name = sys._getframe(1).f_code.co_name
     try:
         headers = {
             "authorization": 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs%3D1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
             "content-type": "application/json",
             "user-agent": 'Mozilla/5.0 (Linux; Android 11; Nokia G20) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.88 Mobile Safari/537.36',
             "x-guest-token": session.cookies.get('guest_token'),
             "x-csrf-token": session.cookies.get("ct0"),
             "x-twitter-auth-type": "OAuth2Session" if session.cookies.get("auth_token") else '',
             "x-twitter-active-user": "yes",
             "x-twitter-client-language": 'en',
         }
-        r = session.post(url, headers=headers, json=payload)
+        r = session.post(url, headers=headers, **kwargs)
         info = r.json()
 
         for s in info.get('subtasks', []):
             if s.get('enter_text', {}).get('keyboard_type') == 'email':
-                print(f"[{WARN}warning{RESET}] {' '.join(find_key(s, 'text'))}")
+                print(f"[{YELLOW}warning{RESET}] {' '.join(find_key(s, 'text'))}")
                 session.cookies.set('confirm_email', 'true')  # signal that email challenge must be solved
 
         session.cookies.set(key, info[key])
     except KeyError as e:
         session.cookies.set('flow_errors', 'true')  # signal that an error occurred somewhere in the flow
-        print(f'[{ERROR}error{RESET}] failed to update token at {BOLD}{caller_name}{RESET}\n{e}')
+        print(f'[{RED}error{RESET}] failed to update token at {BOLD}{caller_name}{RESET}\n{e}')
     return session
 
 
 def init_guest_token(session: Session) -> Session:
-    return update_token(session, 'guest_token', 'https://api.twitter.com/1.1/guest/activate.json', {})
+    return update_token(session, 'guest_token', 'https://api.twitter.com/1.1/guest/activate.json', json={})
 
 
 def flow_start(session: Session) -> Session:
-    return update_token(session, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json?flow_name=login', {
-        "input_flow_data": {
-            "flow_context": {"debug_overrides": {}, "start_location": {"location": "splash_screen"}}
-        }, "subtask_versions": {}
-    })
+    return update_token(session, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json',
+                        params={'flow_name': 'login'},
+                        json={
+                            "input_flow_data": {
+                                "flow_context": {
+                                    "debug_overrides": {},
+                                    "start_location": {"location": "splash_screen"}
+                                }
+                            }, "subtask_versions": {}
+                        })
 
 
 def flow_instrumentation(session: Session) -> Session:
-    return update_token(session, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', {
+    return update_token(session, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', json={
         "flow_token": session.cookies.get('flow_token'),
         "subtask_inputs": [{
             "subtask_id": "LoginJsInstrumentationSubtask",
             "js_instrumentation": {"response": "{}", "link": "next_link"}
         }],
     })
 
 
 def flow_username(session: Session) -> Session:
-    return update_token(session, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', {
+    return update_token(session, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', json={
         "flow_token": session.cookies.get('flow_token'),
         "subtask_inputs": [{
             "subtask_id": "LoginEnterUserIdentifierSSO",
             "settings_list": {
                 "setting_responses": [{
                     "key": "user_identifier",
                     "response_data": {"text_data": {"result": session.cookies.get('username')}}
                 }], "link": "next_link"}}],
     })
 
 
 def flow_password(session: Session) -> Session:
-    return update_token(session, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', {
+    return update_token(session, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', json={
         "flow_token": session.cookies.get('flow_token'),
         "subtask_inputs": [{
             "subtask_id": "LoginEnterPassword",
             "enter_password": {"password": session.cookies.get('password'), "link": "next_link"}}]
     })
 
 
 def flow_duplication_check(session: Session) -> Session:
-    return update_token(session, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', {
+    return update_token(session, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', json={
         "flow_token": session.cookies.get('flow_token'),
         "subtask_inputs": [{
             "subtask_id": "AccountDuplicationCheck",
             "check_logged_in_account": {"link": "AccountDuplicationCheck_false"},
         }],
     })
 
 
 def confirm_email(session: Session) -> Session:
-    return update_token(session, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', {
+    return update_token(session, 'flow_token', 'https://api.twitter.com/1.1/onboarding/task.json', json={
         "flow_token": session.cookies.get('flow_token'),
         "subtask_inputs": [
             {
                 "subtask_id": "LoginAcid",
                 "enter_text": {
                     "text": session.cookies.get('email'),
                     "link": "next_link"
@@ -121,11 +126,11 @@
         "username": username,
         "password": password,
         "guest_token": None,
         "flow_token": None,
     })
     session = execute_login_flow(session)
     if session.cookies.get('flow_errors') == 'true':
-        print(f'[{ERROR}error{RESET}] {BOLD}{username}{RESET} login failed')
+        print(f'[{RED}error{RESET}] {BOLD}{username}{RESET} login failed')
     else:
-        print(f'[{SUCCESS}success{RESET}] {BOLD}{username}{RESET} login success')
+        print(f'[{GREEN}success{RESET}] {BOLD}{username}{RESET} login success')
     return session
```

### Comparing `twitter-api-client-0.6.5/twitter/noauth/operation.py` & `twitter-api-client-0.6.6/twitter/noauth/operation.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     UserByRestId = 'GazOglcBvgLigl3ywt6b3Q', 'UserByRestId', 'userId'
     UsersByRestIds = 'OJBgJQIrij6e3cjqQ3Zu1Q', 'UsersByRestIds', 'userIds'
     UserTweets = 'HuTx74BxAnezK1gWvYY7zg', 'UserTweets', 'userId'
     UserMedia = 'YqiE3JL1KNgf9nSljYdxaA', 'UserMedia', 'userId'
     UserTweetsAndReplies = 'RIWc55YCNyUJ-U3HHGYkdg', 'UserTweetsAndReplies', 'userId'
     TweetResultByRestId = 'D_jNhjWZeRZT5NURzfJZSQ', 'TweetResultByRestId', 'tweetId'
     TweetDetail = 'zXaXQgfyR4GxE21uwYQSyA', 'TweetDetail', 'focalTweetId'
-    # auth required for: Followers,Following,Likes,Retweeters,Favoriters, etc.
 
     default_variables = {
         "count": 1000,
         "withSafetyModeUserFields": True,
         "includePromotedContent": True,
         "withQuickPromoteEligibilityTweetFields": True,
         "withVoice": True,
```

### Comparing `twitter-api-client-0.6.5/twitter/noauth/scraper.py` & `twitter-api-client-0.6.6/twitter/noauth/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,24 +89,24 @@
                     res.extend(future.result())
                     pbar.update(1)
         return res
 
     def profile_spotlight(self, screen_names: list[str], **kwargs) -> list:
         return self._threaded_query(Operation.ProfileSpotlightsQuery, screen_names, **kwargs)
 
-    def user(self, screen_names: list[str], **kwargs) -> list:
+    def users(self, screen_names: list[str], **kwargs) -> list:
         return self._threaded_query(Operation.UserByScreenName, screen_names, **kwargs)
 
-    def user_by_id(self, user_ids: list[int], **kwargs) -> list[dict]:
+    def users_by_id(self, user_ids: list[int], **kwargs) -> list[dict]:
         return self._threaded_query(Operation.UserByRestId, user_ids, **kwargs)
 
-    def tweet_by_id(self, tweet_ids: list[int], **kwargs) -> list[dict]:
+    def tweets_by_id(self, tweet_ids: list[int], **kwargs) -> list[dict]:
         return self._threaded_query(Operation.TweetResultByRestId, tweet_ids, **kwargs)
 
-    def tweet_details(self, tweet_ids: list[int], limit=math.inf, **kwargs) -> list[dict]:
+    def tweets_details(self, tweet_ids: list[int], limit=math.inf, **kwargs) -> list[dict]:
         return self._threaded_pagination(Operation.TweetDetail, tweet_ids, limit, **kwargs)
 
     def tweets(self, user_ids: list[int], limit=math.inf, **kwargs) -> list[dict]:
         return self._threaded_pagination(Operation.UserTweets, user_ids, limit, **kwargs)
 
     def tweets_and_replies(self, user_ids: list[int], limit=math.inf, **kwargs) -> list[dict]:
         return self._threaded_pagination(Operation.UserTweetsAndReplies, user_ids, limit, **kwargs)
```

### Comparing `twitter-api-client-0.6.5/twitter/noauth/util.py` & `twitter-api-client-0.6.6/twitter/noauth/util.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.6.5/twitter/scraper.py` & `twitter-api-client-0.6.6/twitter/scraper.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,310 +1,249 @@
 import asyncio
 import logging.config
 import math
-import platform
-import random
 import time
-from copy import deepcopy
+from concurrent.futures import ThreadPoolExecutor, as_completed
 from pathlib import Path
 from urllib.parse import urlsplit
 
 import orjson
-from aiohttp import ClientSession, TCPConnector
+from aiohttp import ClientSession, TCPConnector, ClientResponse
+from requests import Response
 from tqdm import tqdm
 
-from .config.log import log_config
-from .config.operations import operations
-from .config.settings import trending_params
 from .constants import *
 from .login import login
-from .utils import find_key, build_query, get_headers, set_qs
+from .util import find_key, save_data, get_cursor, get_headers, set_qs, fmt_status
 
-try:
-    if get_ipython().__class__.__name__ == 'ZMQInteractiveShell':
-        import nest_asyncio
-
-        nest_asyncio.apply()
-except:
-    ...
-
-if platform.system() != 'Windows':
-    import uvloop
-
-    asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
-else:
-    asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
-
-ID = 'ID'
-DUP_LIMIT = 5
 logging.config.dictConfig(log_config)
 logger = logging.getLogger(__name__)
 
 
 class Scraper:
-    GRAPHQL_URL = 'https://api.twitter.com/graphql'
-
-    def __init__(self, email: str, username: str, password: str):
+    def __init__(self, email: str, username: str, password: str, *, save=True, debug=False):
         self.session = login(email, username, password)
+        self.api = 'https://twitter.com/i/api/graphql'
+        self.save = save
+        self.debug = debug
 
-    def tweets(self, ids: list[int], limit=math.inf):
-        return self.run(ids, Operation.Data.UserTweets, limit)
+    def users(self, screen_names: list[str]) -> list:
+        return self._run(screen_names, Operation.UserByScreenName)
 
-    def tweets_and_replies(self, ids: list[int], limit=math.inf):
-        return self.run(ids, Operation.Data.UserTweetsAndReplies, limit)
+    def tweets_by_id(self, tweet_ids: list[int]) -> list[dict]:
+        return self._run(tweet_ids, Operation.TweetResultByRestId)
 
-    def likes(self, ids: list[int], limit=math.inf):
-        return self.run(ids, Operation.Data.Likes, limit)
+    def tweets_details(self, tweet_ids: list[int], limit=math.inf) -> list[dict]:
+        return self._run(tweet_ids, Operation.TweetDetail, limit)
 
-    def media(self, ids: list[int], limit=math.inf):
-        return self.run(ids, Operation.Data.UserMedia, limit)
+    def tweets(self, user_ids: list[int], limit=math.inf) -> list[dict]:
+        return self._run(user_ids, Operation.UserTweets, limit)
 
-    def followers(self, ids: list[int], limit=math.inf):
-        return self.run(ids, Operation.Data.Followers, limit)
+    def tweets_and_replies(self, user_ids: list[int], limit=math.inf) -> list[dict]:
+        return self._run(user_ids, Operation.UserTweetsAndReplies, limit)
 
-    def following(self, ids: list[int], limit=math.inf):
-        return self.run(ids, Operation.Data.Following, limit)
+    def media(self, user_ids: list[int], limit=math.inf) -> list[dict]:
+        return self._run(user_ids, Operation.UserMedia, limit)
 
-    def favoriters(self, ids: list[int], limit=math.inf):
-        return self.run(ids, Operation.Data.Favoriters, limit)
+    def likes(self, user_ids: list[int], limit=math.inf) -> list[dict]:
+        return self._run(user_ids, Operation.Likes, limit)
 
-    def retweeters(self, ids: list[int], limit=math.inf):
-        return self.run(ids, Operation.Data.Retweeters, limit)
+    def followers(self, user_ids: list[int], limit=math.inf) -> list[dict]:
+        return self._run(user_ids, Operation.Followers, limit)
 
-    def tweets_details(self, ids: list[int], limit=math.inf):
-        return self.run(ids, Operation.Data.TweetDetail, limit)
+    # auth required
+    def following(self, user_ids: list[int], limit=math.inf) -> list[dict]:
+        return self._run(user_ids, Operation.Following, limit)
 
-    # no pagination needed
-    def tweet_by_rest_id(self, ids: list[int]):
-        return self.run(ids, Operation.Data.TweetResultByRestId)
+    # auth required
+    def favoriters(self, tweet_ids: list[int], limit=math.inf) -> list[dict]:
+        return self._run(tweet_ids, Operation.Favoriters, limit)
 
-    # no pagination needed
-    def user_by_screen_name(self, ids: list[str]):
-        return self.run(ids, Operation.Data.UserByScreenName)
+    # auth required
+    def retweeters(self, tweet_ids: list[int], limit=math.inf) -> list[dict]:
+        return self._run(tweet_ids, Operation.Retweeters, limit)
 
-    # no pagination needed
-    def user_by_rest_id(self, ids: list[int]):
-        return self.run(ids, Operation.Data.UserByRestId)
+    def profile_spotlights(self, screen_names: list[str]) -> list:
+        """
+        This endpoint is included for completeness only. It returns very few data points.
+        Use the batched query `users_by_ids` instead if you wish to pull user profile data.
+        """
+        return self._run(screen_names, Operation.ProfileSpotlightsQuery)
 
-    # no pagination needed (special batch query)
-    def users_by_rest_ids(self, ids: list[int]):
-        name, key = Operation.Data.UsersByRestIds
-        params = deepcopy(operations[name])
-        qid = params['queryId']
-        params['variables']['userIds'] = ids
-        q = build_query(params)
-        url = f"{self.GRAPHQL_URL}/{qid}/{name}?{q}"
-        headers = get_headers(self.session)
-        headers['content-type'] = "application/json"
-        users = self.session.get(url, headers=headers).json()
-        return users
-
-    def run(self, ids: list, operation: tuple, limit=None):
-        res = self.query(ids, operation)
-        if limit is None:
-            return res
-        return asyncio.run(self.pagination(res, operation, limit)) + res
-
-    def query(self, ids: list[any], operation: tuple) -> list:
-        name, key = operation
-        params = deepcopy(operations[name])
-        qid = params['queryId']
-        urls = []
-        for _id in ids:
-            params['variables'][key] = _id
-            q = build_query(params)
-            urls.append((_id, f"{self.GRAPHQL_URL}/{qid}/{name}?{q}"))
-        headers = get_headers(self.session)
-        headers['content-type'] = "application/json"
-        res = asyncio.run(self.process(urls, headers))
-        self.save_data(res, name)
-        return res
+    def users_by_id(self, user_ids: list[int]) -> list[dict]:
+        """
+        This endpoint is included for completeness only.
+        Use the batched query `users_by_ids` instead if you wish to pull user profile data.
+        """
+        return self._run(user_ids, Operation.UserByRestId)
 
-    async def process(self, urls: list, headers: dict) -> list:
-        conn = TCPConnector(limit=100, ssl=False, ttl_dns_cache=69)
-        async with ClientSession(headers=headers, connector=conn) as s:
-            # add cookies from logged-in session
-            s.cookie_jar.update_cookies(self.session.cookies)
-            return await asyncio.gather(*(self.get(s, u) for u in urls))
+    def tweet_stats(self, user_ids: list[int]) -> list[dict]:
+        return self._run(user_ids, Operation.TweetStats)
 
-    async def get(self, session: ClientSession, url: tuple) -> dict:
-        identifier, api_url = url
-        logger.debug(f'processing: {url}')
-        try:
-            r = await session.get(api_url)
-            limits = {k: v for k, v in r.headers.items() if 'x-rate-limit' in k}
-            logger.debug(f'{limits = }')
-            if r.status == 429:
-                logger.debug(f'rate limit exceeded: {url}')
-                return {}
-            data = await r.json()
-            return {ID: identifier, **data}
-        except Exception as e:
-            logger.debug(f'[{ERROR}error{RESET}] failed to download {url}: {e}')
+    # special case, batch query
+    def users_by_ids(self, user_ids: list[int]) -> dict:
+        """
+        Get user data in batches
+
+        Batch-size limited to around 200-300 users
+        """
+        qid, op, k = Operation.UsersByRestIds
+        params = {k: orjson.dumps(v).decode() for k, v in {
+            'variables': {k: user_ids} | Operation.default_variables,
+            'features': Operation.default_features,
+        }.items()}
+        r = self.session.get(f'{self.api}/{qid}/{op}', headers=get_headers(self.session), params=params)
+        txt = r.text
+        data = r.json()
+        if self.debug:
+            self.log(r, txt, data)
+        if self.save:
+            save_data(data, op, user_ids[0])
+        return data
 
-    async def pagination(self, res: list, operation: tuple, limit: int) -> list:
+    def _run(self, ids: list[int | str], operation: tuple, limit=None):
+        return asyncio.run(self._process(ids, operation, limit))
+
+    async def _process(self, ids: list[int | str], op: tuple, limit: int | None) -> list:
         conn = TCPConnector(limit=100, ssl=False, ttl_dns_cache=69)
-        headers = get_headers(self.session)
-        headers['content-type'] = "application/json"
-        async with ClientSession(headers=headers, connector=conn) as s:
-            # add cookies from logged-in session
+        async with ClientSession(headers=get_headers(self.session), connector=conn) as s:
             s.cookie_jar.update_cookies(self.session.cookies)
-            return await asyncio.gather(*(self.paginate(s, data, operation, limit) for data in res))
+            return await asyncio.gather(*(self._paginate(s, _id, op, limit) for _id in ids))
 
-    async def paginate(self, session: ClientSession, data: dict, operation: tuple, limit: int):
-        def get_cursor(data):
-            # inefficient, but need to deal with arbitrary schema
-            entries = find_key(data, 'entries')
-            if entries:
-                for entry in entries.pop():
-                    entry_id = entry.get('entryId', '')
-                    if ('cursor-bottom' in entry_id) or ('cursor-showmorethreads' in entry_id):
-                        content = entry['content']
-                        if itemContent := content.get('itemContent'):
-                            return itemContent['value']  # v2 cursor
-                        return content['value']  # v1 cursor
-
-        all_data = []
-        try:
-            name, key = operation
-            params = deepcopy(operations[name])
-            qid = params['queryId']
+    async def _paginate(self, session: ClientSession, _id: int | str | list[int], operation: tuple,
+                        limit: int | None) -> list[dict]:
+        r = await self._query(session, _id, operation)
+        initial_data = await r.json()
+        res = [initial_data]
+        ids = set(find_key(initial_data, 'rest_id'))
+        dups = 0
+        DUP_LIMIT = 5
+
+        cursor = get_cursor(initial_data)
+        while (dups < DUP_LIMIT) and cursor:
+            prev_len = len(ids)
+            if prev_len >= limit:
+                return res
+
+            # csrf must match in headers and cookies
+            if csrf := r.cookies.get("ct0"):
+                session.headers.update({"x-csrf-token": csrf.value})
+            session.cookie_jar.update_cookies(r.cookies)
 
-            ids = set()
-            counts = []
+            r = await self._query(session, _id, operation, cursor=cursor)
+            data = await r.json()
 
-            params['variables'][key] = data[ID]
             cursor = get_cursor(data)
+            ids |= set(find_key(data, 'rest_id'))
 
-            while 1:
-                params['variables']['cursor'] = cursor
-                query = build_query(params)
-                url = f"{self.GRAPHQL_URL}/{qid}/{name}?{query}"
-
-                # code [353]: "This request requires a matching csrf cookie and header."
-                r, _data = await self.backoff(lambda: session.get(url))
-                if csrf := r.cookies.get("ct0"):
-                    session.headers.update({"x-csrf-token": csrf.value})
-                session.cookie_jar.update_cookies(r.cookies)
-
-                tagged_data = _data | {ID: data[ID]}
-                self.save_data([tagged_data], name)
-                all_data.append(tagged_data)
-                cursor = get_cursor(_data)
-                logger.debug(f'{cursor = }')
-                ids |= set(find_key(tagged_data, 'rest_id'))
-                logger.debug(f'({data[ID]})\t{len(ids)} unique results')
-                counts.append(len(ids))
-
-                success_message = f'[{SUCCESS}success{RESET}] done pagination'
-                # followers/following have "0|"
-                if not cursor or cursor.startswith('0|'):
-                    logger.debug(f'{success_message}\tlast cursor: {cursor}')
-                    break
-                if len(ids) >= limit:
-                    logger.debug(f'{success_message}\tsurpassed limit of {limit} results')
-                    break
-                # did last 5 requests return duplicate data?
-                if len(counts) > DUP_LIMIT and len(set(counts[-1:-DUP_LIMIT:-1])) == 1:
-                    logger.debug(f'{success_message}\tpast {DUP_LIMIT} requests returned duplicate data')
-                    break
-        except Exception as e:
-            logger.debug(f'[{ERROR}error{RESET}] paginate falied: {e}')
-        # save_data(all_data, name)
-        return all_data
-
-    async def backoff(self, fn, retries=12):
-        for i in range(retries + 1):
-            try:
-                r = await fn()
-                data = await r.json()
-                if r.status == 429:
-                    logger.debug(f'[{ERROR}error{RESET}] rate limit exceeded: {r.url}')
-                    return r, {}
-                if find_key(data, 'errors'):
-                    logger.debug(f'[{ERROR}error{RESET}] twitter errors: {data}')
-                return r, data
-            except Exception as e:
-                if i == retries:
-                    logger.debug(f'[{ERROR}error{RESET}] max retries exceeded{RESET}\n{e}')
-                    return
-                t = 2 ** i + random.random()
-                logger.debug(f'{WARN}retrying in {f"{t:.2f}"} seconds{RESET}\t\t{e}')
-                time.sleep(t)
+            if self.debug:
+                logger.debug(f'cursor: {cursor}\tunique results: {len(ids)}')
 
-    def save_data(self, data: list, name: str = ''):
-        try:
-            for d in data:
-                path = Path(f'data/raw/{d[ID]}')
-                path.mkdir(parents=True, exist_ok=True)
-                (path / f'{time.time_ns()}_{name}.json').write_text(
-                    orjson.dumps(d, option=orjson.OPT_INDENT_2).decode(),
-                    encoding='utf-8'
-                )
+            if prev_len == len(ids):
+                dups += 1
 
-        except KeyError as e:
-            logger.debug(f'[{ERROR}error{RESET}] failed to save data: {e}')
+            res.append(data)
+        return res
 
-    def download(self, post_url: str, cdn_url: str, path: str = 'media', chunk_size: int = 4096) -> None:
-        """
-        Download file
-    
-        @param post_url: the actual post url
-        @param cdn_url: the cdn url
-        @param path: path to save media
-        @param chunk_size: chunk size in bytes
-        @return: None
-        """
+    async def _query(self, session: ClientSession, _id: int | str | list, operation: tuple, **kwargs) -> ClientResponse:
+        qid, op, k = operation
+        params = {k: orjson.dumps(v).decode() for k, v in {
+            'variables': {k: _id} | kwargs | Operation.default_variables,
+            'features': Operation.default_features,
+        }.items()}
+        r = await session.get(f'{self.api}/{qid}/{op}', params=params)
+        txt = await r.text()
+        data = await r.json()
+        if self.debug:
+            self.log(r, txt, data)
+        if self.save:
+            save_data(data, op, _id[0] if isinstance(_id, list) else _id)
+        return r
+
+    def download_media(self, ids: list[int], photos: bool = True, videos: bool = True) -> None:
+        tweets = self.tweets_by_id(ids)
+        urls = []
+        for tweet in tweets:
+            tweet_id = find_key(tweet, 'id_str')[0]
+            url = f'https://twitter.com/i/status/{tweet_id}'  # `i` evaluates to screen_name
+            media = [y for x in find_key(tweet, 'media') for y in x]
+            if photos:
+                photo_urls = list({u for m in media if 'ext_tw_video_thumb' not in (u := m['media_url_https'])})
+                [urls.append([url, photo]) for photo in photo_urls]
+            if videos:
+                video_urls = [x['variants'] for m in media if (x := m.get('video_info'))]
+                hq_videos = {sorted(v, key=lambda d: d.get('bitrate', 0))[-1]['url'] for v in video_urls}
+                [urls.append([url, video]) for video in hq_videos]
+
+        with tqdm(total=len(urls), desc='downloading media') as pbar:
+            with ThreadPoolExecutor(max_workers=32) as e:
+                for future in as_completed(e.submit(self._download, x, y) for x, y in urls):
+                    future.result()
+                    pbar.update()
+
+    def _download(self, post_url: str, cdn_url: str, path: str = 'media', chunk_size: int = 4096) -> None:
         Path(path).mkdir(parents=True, exist_ok=True)
         name = urlsplit(post_url).path.replace('/', '_')[1:]
         ext = urlsplit(cdn_url).path.split('/')[-1]
         try:
             r = self.session.get(cdn_url, stream=True)
-            total_bytes = int(r.headers.get('Content-Length', 0))
-            desc = f'downloading: {name}'
-            with tqdm(total=total_bytes, desc=desc, unit='B', unit_scale=True, unit_divisor=1024) as pbar:
-                with open(f'{path}/{name}_{ext}', 'wb') as f:
-                    for chunk in r.iter_content(chunk_size=chunk_size):
-                        f.write(chunk)
-                        pbar.update(f.tell() - pbar.n)
+            with open(f'{path}/{name}_{ext}', 'wb') as f:
+                for chunk in r.iter_content(chunk_size=chunk_size):
+                    f.write(chunk)
         except Exception as e:
-            logger.debug(f'[{ERROR}error{RESET}] failed to download media: {post_url} {e}')
-
-    def download_media(self, ids: list[int], photos: bool = True, videos: bool = True) -> None:
-        res = self.tweet_by_rest_id(ids)
-        for r in res:
-            user_id = find_key(r, 'user_results')[0]['result']['rest_id']
-            url = f'https://twitter.com/{user_id}/status/{r[ID]}'  # evaluates to username in browser
-            media = [y for x in find_key(r, 'media') for y in x]  # in case of arbitrary schema
-            if photos:
-                photos = list({u for m in media if 'ext_tw_video_thumb' not in (u := m['media_url_https'])})
-                if photos:
-                    [self.download(url, photo) for photo in photos]
-            if videos:
-                videos = [x['variants'] for m in media if (x := m.get('video_info'))]
-                hq_videos = {sorted(v, key=lambda d: d.get('bitrate', 0))[-1]['url'] for v in videos}
-                if hq_videos:
-                    [self.download(url, video) for video in hq_videos]
+            logger.debug(f'[{RED}error{RESET}] failed to download media: {post_url} {e}')
 
     def trends(self) -> dict:
         """Get trends for all UTC offsets"""
-        url = set_qs('https://twitter.com/i/api/2/guide.json', trending_params)
-        headers = get_headers(self.session)
-        offsets = [f"{str(i).zfill(3)}00" if i < 0 else f"+{str(i).zfill(2)}00" for i in range(-12, 15)]
-        res = []
-        for offset in offsets:
+
+        def get_trends(offset: str, url: str, headers: dict):
             headers['x-twitter-utcoffset'] = offset
             r = self.session.get(url, headers=headers)
-            res.append(r.json())
-            logger.debug(f'getting trends for: {offset = }')
-        all_trends = {}
-        for data in res:
-            trends = find_key(data, 'item')
-            for t in trends:
-                all_trends |= {t['content']['trend']['name']: t}
+            trends = find_key(r.json(), 'item')
+            return {t['content']['trend']['name']: t for t in trends}
+
+        headers = get_headers(self.session)
+        url = set_qs('https://twitter.com/i/api/2/guide.json', trending_params)
+        offsets = [f"{str(i).zfill(3)}00" if i < 0 else f"+{str(i).zfill(2)}00" for i in range(-12, 15)]
+        trends = {}
+        with tqdm(total=len(offsets), desc='downloading trends') as pbar:
+            with ThreadPoolExecutor(max_workers=32) as e:
+                for future in as_completed(e.submit(get_trends, o, url, headers) for o in offsets):
+                    trends |= future.result()
+                    pbar.update()
+
         path = Path(f'data/raw/trends')
         path.mkdir(parents=True, exist_ok=True)
         (path / f'{time.time_ns()}.json').write_text(
-            orjson.dumps(all_trends, option=orjson.OPT_INDENT_2).decode(),
+            orjson.dumps(trends, option=orjson.OPT_INDENT_2).decode(),
             encoding='utf-8'
         )
-        return all_trends
+        return trends
+
+    def log(self, r: ClientResponse | Response, txt: str, data: dict):
+        status = r.status if isinstance(r, ClientResponse) else r.status_code
+
+        def stat(r):
+            if self.debug >= 1:
+                logger.debug(f'{r.url}')
+            if self.debug >= 2:
+                logger.debug(f'{txt}')
+
+            limits = {k: v for k, v in r.headers.items() if 'x-rate-limit' in k}
+            current_time = int(time.time())
+            wait = int(r.headers.get('x-rate-limit-reset', current_time)) - current_time
+            logger.debug(
+                f"remaining: {MAGENTA}{limits['x-rate-limit-remaining']}/{limits['x-rate-limit-limit']}{RESET} requests")
+            logger.debug(f'reset:     {MAGENTA}{(wait / 60):.2f}{RESET} minutes')
+
+        try:
+            if 'json' in r.headers.get('content-type', ''):
+                if data.get('errors'):
+                    logger.debug(f'[{RED}error{RESET}] {status} {data}')
+                else:
+                    logger.debug(fmt_status(status))
+                    stat(r)
+            else:
+                logger.debug(fmt_status(status))
+                stat(r)
+        except Exception as e:
+            logger.debug(f'failed to log: {e}')
```

### Comparing `twitter-api-client-0.6.5/twitter/search.py` & `twitter-api-client-0.6.6/twitter/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import asyncio
-import atexit
-import math
-
-import orjson
 import logging.config
+import math
 import platform
 import random
 import re
 import time
 from pathlib import Path
 
 import aiohttp
+import orjson
 import requests
 
-from .config.log import log_config
-from .config.settings import search_config
 from .constants import *
-from .utils import set_qs
+from .util import set_qs
 
 IN_PATH = Path('~/data/raw').expanduser()
 OUT_PATH = Path(f'~/data/processed/search_results_{time.time_ns()}.json').expanduser()
 
 reset = '\u001b[0m'
 colors = [f'\u001b[{i}m' for i in range(30, 38)]
 logging.config.dictConfig(log_config)
@@ -62,15 +58,15 @@
     data, next_cursor = await backoff(lambda: get(session, api, config), query)
     all_data = [data]
     c = colors.pop() if colors else ''
     ids = set()
     while next_cursor:
         ids |= set(data['globalObjects']['tweets'])
         if len(ids) >= kwargs.get('limit', math.inf):
-            logger.debug(f'[{SUCCESS}success{RESET}] returned {len(ids)} search results for {c}{query}{reset}')
+            logger.debug(f'[{GREEN}success{RESET}] returned {len(ids)} search results for {c}{query}{reset}')
             return all_data
         logger.debug(f'{c}{query}{reset}')
         config['cursor'] = next_cursor
         data, next_cursor = await backoff(lambda: get(session, api, config), query)
         data['query'] = query
         (out / f'raw/{time.time_ns()}.json').write_text(
             orjson.dumps(data, option=orjson.OPT_INDENT_2).decode(),
```

### Comparing `twitter-api-client-0.6.5/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.6.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,222 +1,242 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.6.5
+Version: 0.6.6
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
- Complete implementation of the undocumented Twitter API
+Complete implementation of the undocumented Twitter API
 
- Includes tools to **scrape**, **automate**, and **search** twitter
+Includes tools to **scrape**, **automate**, and **search** twitter
 
- ### Installation
+* [Installation](#installation)
+* [Automation](#automation)
+* [Scraping](#scraping)
+  * [Get all user/tweet data](#get-all-usertweet-data)
+  * [Get user/tweet data (no auth)](#get-usertweet-data-no-auth)
+  * [Search](#search)
+* [Notes](#notes)
+
+### Automation
 
 ```python
- from twitter.account import Account
+from twitter.account import Account
+
+email, username, password = ..., ..., ...
+account = Account(email, username, password, debug=2, save=True)
+
+account.tweet('test 123')
+account.untweet(123456)
+account.retweet(123456)
+account.unretweet(123456)
+account.reply('foo', tweet_id=123456)
+account.quote('bar', tweet_id=123456)
+account.schedule_tweet('schedule foo', 1681851240)
+account.unschedule_tweet(123456)
+
+account.tweet('hello world', media=[
+    {'media': 'test.jpg', 'alt': 'some alt text', 'tagged_users': [123]},
+    {'media': 'test.jpeg', 'alt': 'some alt text', 'tagged_users': [123]},
+    {'media': 'test.png', 'alt': 'some alt text', 'tagged_users': [123]},
+    {'media': 'test.jfif', 'alt': 'some alt text', 'tagged_users': [123]},
+])
+
+account.schedule_tweet('foo bar', '2023-04-18 15:42', media=[
+    {'media': 'test.gif', 'alt': 'some alt text'},
+])
+
+account.schedule_reply('hello world', '2023-04-19 15:42', tweet_id=123456, media=[
+    {'media': 'test.gif', 'alt': 'some alt text'},
+])
+
+account.dm('my message', [1234], media='test.jpg')
+
+account.create_poll('test poll 123', ['hello', 'world', 'foo', 'bar'], 10080)
+
+# tweets
+account.like(123456)
+account.unlike(123456)
+account.bookmark(123456)
+account.unbookmark(123456)
+account.pin(123456)
+account.unpin(123456)
+
+# users
+account.follow(1234)
+account.unfollow(1234)
+account.mute(1234)
+account.unmute(1234)
+account.enable_notifications(1234)
+account.disable_notifications(1234)
+account.block(1234)
+account.unblock(1234)
+
+# user profile
+account.update_profile_image('test.jpg')
+account.update_profile_banner('test.png')
+account.update_profile_info(name='Foo Bar', description='test 123', location='Victoria, BC')
+
+#  topics
+account.follow_topic(111)
+account.unfollow_topic(111)
+
+# lists
+account.create_list('My List', 'description of my list', private=False)
+account.update_list(222, 'My Updated List', 'some updated description', private=False)
+account.update_list_banner(222, 'test.png')
+account.delete_list_banner(222)
+account.add_list_member(222, 1234)
+account.remove_list_member(222, 1234)
+account.delete_list(222)
+account.pin_list(222)
+account.unpin_list(222)
+
+# refresh all pinned lists in this order
+account.update_pinned_lists([222, 111, 333])
+
+# unpin all lists
+account.update_pinned_lists([])
+
+# get timelines
+timeline = account.home_timeline()
+latest_timeline = account.home_latest_timeline(limit=500)
+
+# get bookmarks
+bookmarks = account.bookmarks()
+
+# example configuration
+account.update_settings({
+    "address_book_live_sync_enabled": False,
+    "allow_ads_personalization": False,
+    "allow_authenticated_periscope_requests": True,
+    "allow_dm_groups_from": "following",
+    "allow_dms_from": "following",
+    "allow_location_history_personalization": False,
+    "allow_logged_out_device_personalization": False,
+    "allow_media_tagging": "none",
+    "allow_sharing_data_for_third_party_personalization": False,
+    "alt_text_compose_enabled": None,
+    "always_use_https": True,
+    "autoplay_disabled": False,
+    "country_code": "us",
+    "discoverable_by_email": False,
+    "discoverable_by_mobile_phone": False,
+    "display_sensitive_media": False,
+    "dm_quality_filter": "enabled",
+    "dm_receipt_setting": "all_disabled",
+    "geo_enabled": False,
+    "include_alt_text_compose": True,
+    "include_mention_filter": True,
+    "include_nsfw_admin_flag": True,
+    "include_nsfw_user_flag": True,
+    "include_ranked_timeline": True,
+    "language": "en",
+    "mention_filter": "unfiltered",
+    "nsfw_admin": False,
+    "nsfw_user": False,
+    "personalized_trends": True,
+    "protected": False,
+    "ranked_timeline_eligible": None,
+    "ranked_timeline_setting": None,
+    "require_password_login": False,
+    "requires_login_verification": False,
+    "sleep_time": {
+        "enabled": False,
+        "end_time": None,
+        "start_time": None
+    },
+    "translator_type": "none",
+    "universal_quality_filtering_enabled": "enabled",
+    "use_cookie_personalization": False,
+})
+
+# example configuration
+account.update_search_settings({
+    "optInFiltering": True,  # filter nsfw content
+    "optInBlocking": True,  # filter blocked accounts
+})
+
+## change_password('old pwd','new pwd)
+
+```
+
+### Scraping
+
+#### Get all user/tweet data
 
- email, username, password = ..., ..., ...
- account = Account(email, username, password)
+```python
+from twitter.scraper import Scraper
+
+email, username, password = ..., ..., ...
+scraper = Scraper(email, username, password, debug=1, save=True)
+
+# user data
+users = scraper.users(['foo', 'bar', 'hello', 'world'])
+users = scraper.users_by_ids([123, 234, 345])  # batch-request
+tweets = scraper.tweets([123, 234, 345])
+likes = scraper.likes([123, 234, 345])
+tweets_and_replies = scraper.tweets_and_replies([123, 234, 345])
+media = scraper.media([123, 234, 345])
+following = scraper.following([123, 234, 345])
+followers = scraper.followers([123, 234, 345])
+scraper.tweet_stats([111111, 222222, 333333])
+
+
+# tweet data
+tweets_by_ids = scraper.tweets_by_id([987, 876, 754])
+tweets_details = scraper.tweets_details([987, 876, 754])
+retweeters = scraper.retweeters([987, 876, 754])
+favoriters = scraper.favoriters([987, 876, 754])
+
+scraper.download_media([
+    111111,
+    222222,
+    333333,
+    444444,
+])
+
+# trends
+scraper.trends()
+```
+
+#### Get user/tweet data (no auth)
+
+```python
+from twitter.noauth.scraper import Scraper
 
- account.create_poll('test poll 123', ['hello', 'world', 'foo', 'bar'], 10080)
+scraper = Scraper()
 
- # DM 1 user
- account.dm([123], 'hello world', filename='test.png')
-
- # DM group of users
- account.dm([123, 234, 345], 'foo bar', filename='test.mp4')
-
- # schedule a tweet (date str or timestamp)
- account.schedule_tweet('scheduled hello', 1679912795, media=['test.jpg'])
-
- # schedule a reply tweet (date str or timestamp)
- account.schedule_tweet('scheduled world', '2023-03-25 19:11', media=['test.jpg'], reply_to=645)
-
- account.unschedule_tweet(321)
-
- # tweets
- account.tweet('test 123')
- account.tweet('test 234', media=['test.mp4'])
- account.tweet('test 345', media=['test.jpg', 'test.png', 'test.jpeg', 'test.jfif'])
- account.tweet('test 456', media=[{'file': 'test.jpeg', 'tagged_users': [123234345456], 'alt': 'some image'}])
- account.untweet(123)
- account.retweet(1633609779745820675)
- account.unretweet(1633609779745820675)
- account.quote(1633609779745820675, 'elonmusk', 'test 123')
- account.reply(1633609779745820675, 'test 123')
- account.like(1633609779745820675)
- account.unlike(1633609779745820675)
- account.bookmark(1633609779745820675)
- account.unbookmark(1633609779745820675)
- account.pin(1635479755364651008)
- account.unpin(1635479755364651008)
-
- # users
- account.follow(50393960)
- account.unfollow(50393960)
- account.mute(50393960)
- account.unmute(50393960)
- account.enable_notifications(50393960)
- account.disable_notifications(50393960)
- account.block(50393960)
- account.unblock(50393960)
-
- # other
- account.stats(50393960)
-
- # user profile
- account.update_profile_image('test.jpg')
- account.update_profile_banner('test.png')
- account.update_profile_info(name='Foo Bar', description='test 123', location='Victoria, BC')
-
- # topics
- account.follow_topic(808713037230157824)
- account.unfollow_topic(808713037230157824)
-
- # lists
- account.create_list('My List', 'description of my list', private=False)
- account.update_list(543, 'My Updated List', 'some updated description', private=False)
- account.update_list_banner(543, 'test.png')
- account.delete_list_banner(543)
- account.add_list_member(543, 50393960)
- account.remove_list_member(543, 50393960)
- account.delete_list(543)
- account.pin_list(543)
- account.unpin_list(543)
-
- # refresh all pinned lists in this order
- account.update_pinned_lists([543, 432, 321])
-
- # unpin all lists
- account.update_pinned_lists([])
-
- # get timelines
- timeline = account.home_timeline()
- latest_timeline = account.home_latest_timeline(limit=100)
-
- # example configuration
- account.update_settings({
-     "address_book_live_sync_enabled": False,
-     "allow_ads_personalization": False,
-     "allow_authenticated_periscope_requests": True,
-     "allow_dm_groups_from": "following",
-     "allow_dms_from": "following",
-     "allow_location_history_personalization": False,
-     "allow_logged_out_device_personalization": False,
-     "allow_media_tagging": "none",
-     "allow_sharing_data_for_third_party_personalization": False,
-     "alt_text_compose_enabled": None,
-     "always_use_https": True,
-     "autoplay_disabled": False,
-     "country_code": "us",
-     "discoverable_by_email": False,
-     "discoverable_by_mobile_phone": False,
-     "display_sensitive_media": False,
-     "dm_quality_filter": "enabled",
-     "dm_receipt_setting": "all_disabled",
-     "geo_enabled": False,
-     "include_alt_text_compose": True,
-     "include_mention_filter": True,
-     "include_nsfw_admin_flag": True,
-     "include_nsfw_user_flag": True,
-     "include_ranked_timeline": True,
-     "language": "en",
-     "mention_filter": "unfiltered",
-     "nsfw_admin": False,
-     "nsfw_user": False,
-     "personalized_trends": True,
-     "protected": False,
-     "ranked_timeline_eligible": None,
-     "ranked_timeline_setting": None,
-     "require_password_login": False,
-     "requires_login_verification": False,
-     "sleep_time": {
-         "enabled": False,
-         "end_time": None,
-         "start_time": None
-     },
-     "translator_type": "none",
-     "universal_quality_filtering_enabled": "enabled",
-     "use_cookie_personalization": False,
- })
-
- # example configuration
- account.update_search_settings({
-     "optInFiltering": True,  # filter out nsfw content
-     "optInBlocking": True,  # filter out blocked accounts
- })
-
- ## account.change_password('old password', 'new password')
- ## account.logout_all_sessions()
-
- ```
-
-
- ### Scraping
-
- #### Get all user/tweet data
-
- ```python
- from twitter.scraper import Scraper
-
- email, username, password = ..., ..., ...
- scraper = Scraper(email, username, password)  # session
-
- ####### User Data ########
- users = scraper.user_by_screen_name(['foo', 'bar', 'baz'])
- tweets = scraper.tweets([123, 234, 345])
- likes = scraper.likes([123, 234, 345])
- tweets_and_replies = scraper.tweets_and_replies([123, 234, 345])
- media = scraper.media([123, 234, 345])
- following = scraper.following([123, 234, 345])
- followers = scraper.followers([123, 234, 345])
-
- ######## Tweet Data ########
- tweets_by_ids = scraper.tweet_by_rest_id([456, 567, 678])
- tweets_details = scraper.tweets_details([456, 567, 678])
- retweeters = scraper.retweeters([456, 567, 678])
- favoriters = scraper.favoriters([456, 567, 678])
-
- scraper.download_media([456, 567, 678])
- ```
-
- #### Get user/tweet data (no auth)
-
- ```python
- from twitter.noauth.scraper import Scraper
-
- scraper = Scraper()
-
- users = scraper.user(['foo', 'bar', 'baz'])
- users = scraper.user_by_id([123, 234, 345])
- users = scraper.users_by_ids([123, 234, 345])  # special batch query
-
- tweets = scraper.tweet_by_id([987, 876, 765])  # condensed
- tweets = scraper.tweet_details([987, 876, 765])
-
- user_tweets = scraper.tweets([123, 234, 345])
- user_tweets_replies = scraper.tweets_and_replies([123, 234, 345])
- user_media = scraper.media([123, 234, 345])
- ```
-
- #### Search
-
- ```python   
- from twitter.search import search
-
- search(
-     '(#dogs OR #cats) min_retweets:500',
-     'min_faves:10000 @elonmusk until:2023-02-16 since:2023-02-01',
-     'brasil portugal -argentina',
-     'paperswithcode -tensorflow -tf',
-     'skateboarding baseball guitar',
-     'cheese bread butter',
-     'ios android',
-     # limit=1000, # optional limit
- )
- ```
+users = scraper.users(['foo', 'bar', 'baz'])
+users = scraper.users_by_id([123, 234, 345])
+users = scraper.users_by_ids([123, 234, 345])  # special batch query
+
+tweets = scraper.tweets_by_id([987, 876, 765])  # condensed
+tweets = scraper.tweets_details([987, 876, 765])
+
+user_tweets = scraper.tweets([123, 234, 345])
+user_tweets_replies = scraper.tweets_and_replies([123, 234, 345])
+user_media = scraper.media([123, 234, 345])
+```
+
+#### Search
+
+```python   
+from twitter.search import search
+
+search(
+    '(#dogs OR #cats) min_retweets:500',
+    'min_faves:10000 @elonmusk until:2023-02-16 since:2023-02-01',
+    'brasil portugal -argentina',
+    'paperswithcode -tensorflow -tf',
+    'skateboarding baseball guitar',
+    'cheese bread butter',
+    'ios android',
+    # limit=1000, # optional limit
+)
+```
```

