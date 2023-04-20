# Comparing `tmp/general_calculator_zsd-1.1.4.tar.gz` & `tmp/general_calculator_zsd-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "general_calculator_zsd-1.1.4.tar", last modified: Thu Mar 30 02:13:31 2023, max compression
+gzip compressed data, was "general_calculator_zsd-1.1.5.tar", last modified: Thu Apr 20 05:22:07 2023, max compression
```

## Comparing `general_calculator_zsd-1.1.4.tar` & `general_calculator_zsd-1.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 02:13:31.001432 general_calculator_zsd-1.1.4/
--rw-rw-rw-   0        0        0     1089 2022-11-17 02:56:12.000000 general_calculator_zsd-1.1.4/LICENSE
--rw-rw-rw-   0        0        0      418 2023-03-30 02:13:31.001432 general_calculator_zsd-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-02-13 09:53:05.000000 general_calculator_zsd-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-30 02:13:30.901192 general_calculator_zsd-1.1.4/general_calculator_zsd/
--rw-rw-rw-   0        0        0        0 2022-11-16 09:26:23.000000 general_calculator_zsd-1.1.4/general_calculator_zsd/__init__.py
--rw-rw-rw-   0        0        0    43299 2023-02-08 05:29:36.000000 general_calculator_zsd-1.1.4/general_calculator_zsd/general_calculator.py
--rw-rw-rw-   0        0        0    58954 2023-03-30 02:12:00.000000 general_calculator_zsd-1.1.4/general_calculator_zsd/mysql_transmit_data4all.py
-drwxrwxrwx   0        0        0        0 2023-03-30 02:13:31.001432 general_calculator_zsd-1.1.4/general_calculator_zsd.egg-info/
--rw-rw-rw-   0        0        0      418 2023-03-30 02:13:29.000000 general_calculator_zsd-1.1.4/general_calculator_zsd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-03-30 02:13:30.000000 general_calculator_zsd-1.1.4/general_calculator_zsd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 02:13:29.000000 general_calculator_zsd-1.1.4/general_calculator_zsd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-03-30 02:13:29.000000 general_calculator_zsd-1.1.4/general_calculator_zsd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-30 02:13:31.001432 general_calculator_zsd-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      531 2023-03-30 02:13:10.000000 general_calculator_zsd-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 05:22:07.797138 general_calculator_zsd-1.1.5/
+-rw-rw-rw-   0        0        0     1089 2022-11-17 02:56:12.000000 general_calculator_zsd-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0      418 2023-04-20 05:22:07.797138 general_calculator_zsd-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-03-30 02:25:01.000000 general_calculator_zsd-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 05:22:07.787098 general_calculator_zsd-1.1.5/general_calculator_zsd/
+-rw-rw-rw-   0        0        0        0 2022-11-16 09:26:23.000000 general_calculator_zsd-1.1.5/general_calculator_zsd/__init__.py
+-rw-rw-rw-   0        0        0    47345 2023-04-20 05:20:08.000000 general_calculator_zsd-1.1.5/general_calculator_zsd/general_calculator.py
+-rw-rw-rw-   0        0        0    60050 2023-04-19 03:08:55.000000 general_calculator_zsd-1.1.5/general_calculator_zsd/mysql_transmit_data4all.py
+drwxrwxrwx   0        0        0        0 2023-04-20 05:22:07.795121 general_calculator_zsd-1.1.5/general_calculator_zsd.egg-info/
+-rw-rw-rw-   0        0        0      418 2023-04-20 05:22:06.000000 general_calculator_zsd-1.1.5/general_calculator_zsd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-04-20 05:22:07.000000 general_calculator_zsd-1.1.5/general_calculator_zsd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 05:22:06.000000 general_calculator_zsd-1.1.5/general_calculator_zsd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-04-20 05:22:06.000000 general_calculator_zsd-1.1.5/general_calculator_zsd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 05:22:07.797138 general_calculator_zsd-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      531 2023-04-20 05:21:14.000000 general_calculator_zsd-1.1.5/setup.py
```

### Comparing `general_calculator_zsd-1.1.4/LICENSE` & `general_calculator_zsd-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `general_calculator_zsd-1.1.4/general_calculator_zsd/general_calculator.py` & `general_calculator_zsd-1.1.5/general_calculator_zsd/general_calculator.py`

 * *Files 4% similar despite different names*

```diff
@@ -183,14 +183,20 @@
         weekday = '周五'
     elif day_of_week == 6:
         weekday = '周六'
     else:
         weekday = '周日'
     return weekday
 
+#根据输入的date格式，得到n_day前的date
+def get_date_before(date_now, n_day):
+    days = datetime.timedelta(days=n_day)
+    date_before = date_now - days
+    return date_before
+
 # --------------------------------------------------------------------------
 # 2.字体处理的模块
 
 # 比较两个列表的坐标信息是否相同，位置是否接近
 def cor_compare(l1, l2):
     if len(l1) != len(l2):
         return False
@@ -1202,8 +1208,111 @@
         dict_out[str(account_id)]["car_list"] = {}
         for idx, row in df_account.iterrows():
             brand_id = row["brand_id"]
             series_id = row["series_id"]
             series_keyword = row[col_word].split('、')
             dict_out[str(account_id)]["car_list"][str(series_id)] = {"series_keyword": series_keyword}
         dict_out[str(account_id)]["brand_id"] = brand_id
-    return dict_out
+    return dict_out
+
+sp_list = {'车险销售': ['车险', '汽车保险'], '车品销售': ['车品', '内饰', '汽车用品', '车辆用品'], '车膜销售': ['车膜', '贴膜', '车衣'], '轮毂销售': ['轮毂'], '二手车车商': ['二手车']}
+def speacial_identify_summmary(text):
+    if (type(text) is not str) or text == '':
+        return None, None
+    for i in list(sp_list.keys()):
+        for keyword in sp_list[i]:
+            if keyword in text:
+                return keyword, i
+            else:
+                continue
+    return None, None
+
+emo_neg = 0.3
+emo_pos = 0.7
+def find_emotion_by_api(TEXT):
+    # 接口地址
+    url = "http://ltpapi.xfyun.cn/v2/sa"
+    # 开放平台应用ID
+    x_appid = "d98c93ce"
+    # 开放平台应用接口秘钥
+    api_key = "9ed34088080000bf82286f25f6702a36"
+    body = urllib.parse.urlencode({'text': TEXT}).encode('utf-8')
+    param = {"type": "dependent"}
+    x_param = base64.b64encode(json.dumps(param).replace(' ', '').encode('utf-8'))
+    x_time = str(int(time.time()))
+    x_checksum = hashlib.md5(api_key.encode('utf-8') + str(x_time).encode('utf-8') + x_param).hexdigest()
+    x_header = {'X-Appid': x_appid,
+                'X-CurTime': x_time,
+                'X-Param': x_param,
+                'X-CheckSum': x_checksum}
+    req = urllib.request.Request(url, body, x_header)
+    result = urllib.request.urlopen(req)
+    result = result.read()
+    # print(result.decode('utf-8'))
+    return result.decode('utf-8')
+
+def cut_sentences(content):
+    # 结束符号，包含中文和英文的
+    end_flag = ['?', '!', '.', '？', '！', '。', '…']
+    try:
+        content_len = len(content)
+    except:
+        return []
+    sentences = []
+    tmp_char = ''
+    for idx, char in enumerate(content):
+        # 拼接字符
+        tmp_char += char
+        # 判断是否已经到了最后一位
+        if (idx + 1) == content_len:
+            sentences.append(tmp_char)
+            break
+        # 判断此字符是否为结束符号
+        if char in end_flag:
+            # 再判断下一个字符是否为结束符号，如果不是结束符号，则切分句子
+            next_idx = idx + 1
+            if not content[next_idx] in end_flag:
+                sentences.append(tmp_char)
+                tmp_char = ''
+    return sentences
+
+def calculate_emotion_score(text):
+    if text == '' or (text.__contains__('互赞|回赞|已赞|求赞') and len(text) <= 15):
+        final_sen = 0.50
+    else:
+        try:
+            res = find_emotion_by_api(text)
+            res = json.loads(res)
+            if res['code'] != "0":
+                text_list = cut_sentences(text)
+                text_num = len(text_list)
+                sentiments = 0
+                for text in text_list:
+                    time.sleep(0.5)
+                    res = find_emotion_by_api(text)
+                    res = json.loads(res)
+                    if res['code'] == '10106':
+                        text_num = text_num - 1
+                        continue
+                    try:
+                        sentiment = res['data']['score']
+                    except:
+                        text_num = text_num - 1
+                        sentiment = 0
+                        continue
+                    sentiments = sentiments + sentiment
+                try:
+                    final_sen = sentiments / text_num
+                except Exception as e:
+                    final_sen = 0.5
+            else:
+                final_sen = res['data']['score']
+        except Exception as e:
+            print(e)
+            final_sen = 0.5
+    if final_sen < emo_neg:
+        emo_pn = -1
+    elif final_sen > emo_pos:
+        emo_pn = 1
+    else:
+        emo_pn = 0
+    return final_sen, emo_pn
```

### Comparing `general_calculator_zsd-1.1.4/general_calculator_zsd/mysql_transmit_data4all.py` & `general_calculator_zsd-1.1.5/general_calculator_zsd/mysql_transmit_data4all.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,45 +48,55 @@
     'moment': 'etl_post',
     'momentcomment': 'etl_comment',
     'user_base': 'etl_user',
     'smart_tucaoba_comment': 'etl_comment'
 }
 
 insert_map_detail = {
+    'weibo_auth_post': ['etl_post', 'id', 100, 'BA_USING'],
+    'weibo_search_post': ['etl_post', 'id', 100, 'BA_USING'],
+    'weibo_user_info': ['etl_user', 'user_id', 100, 'BA_USING'],
+    'weibo_comment': ['etl_comment', 'comment_id', 100, 'BA_USING'],
     'autohome_wenzhang_post': ['etl_post', 'wenzhang_id', 200, 'BA_USING'],
     'autohome_luntan_post': ['etl_post', 'tiezi_id', 200, 'BA_USING'],
     'autohome_koubei_post': ['etl_post', 'post_id', 200, 'BA_USING'],
     'autohome_wenzhang_comment': ['etl_comment', 'comment_id', 200, 'BA_USING'],
     'autohome_luntan_comment': ['etl_comment', 'comment_id', 200, 'BA_USING'],
     'autohome_koubei_comment': ['etl_comment', 'comment_id', 200, 'BA_USING'],
     'autohome_user_info': ['etl_user', 'user_id', 200, 'BA_USING'],
-    'dongchedi_wenzhang_post': ['etl_post', 'wenzhang_id', 200, 'BA_USING'],
-    'dongchedi_cheyouquan_post': ['etl_post', 'post_id', 200, 'BA_USING'],
-    'dongchedi_koubei_post': ['etl_post', 'post_id', 200, 'BA_USING'],
-    'dongchedi_wenzhang_comment': ['etl_comment', 'comment_id', 200, 'BA_USING'],
-    'dongchedi_cheyouquan_comment': ['etl_comment', 'comment_id', 200, 'BA_USING'],
-    'dongchedi_koubei_comment': ['etl_comment', 'comment_id', 200, 'BA_USING'],
-    'dongchedi_user_info': ['etl_user', 'user_id', 200, 'BA_USING'],
     'bilibili_video_post': ['etl_post', 'video_id', 300, 'BA_USING'],
     'bilibili_video_comment': ['etl_comment', 'rpid',300, 'BA_USING'],
     'bilibili_video_danmu': ['etl_comment','danmu_comment_id', 300, 'BA_USING'],
     'bilibili_user_info': ['etl_user', 'user_id', 300, 'BA_USING'],
-    'weibo_auth_post': ['etl_post', 'id', 100, 'BA_USING'],
-    'weibo_search_post': ['etl_post', 'id', 100, 'BA_USING'],
-    'weibo_user_info': ['etl_user', 'user_id', 100, 'BA_USING'],
-    'weibo_comment': ['etl_comment', 'comment_id', 100, 'BA_USING'],
     'xiaohongshu_search_post': ['etl_post', 'note_id', 400, 'BA_USING'],
     'xiaohongshu_comment': ['etl_comment', 'comment_id', 400, 'BA_USING'],
     'xiaohongshu_user_info': ['etl_user', 'user_id', 400, 'BA_USING'],
     'moment': ['etl_post', 'id', 500, 'BA_USING'],
     'momentcomment': ['etl_comment', 'id', 500, 'BA_USING'],
     'user_base': ['etl_user', 'user_id', 500, 'BI_READ'],
     'smart_tucaoba_comment': ['etl_comment', 'comment_id', 500, 'BA_USING']
+    'dongchedi_wenzhang_post': ['etl_post', 'wenzhang_id', 600, 'BA_USING'],
+    'dongchedi_cheyouquan_post': ['etl_post', 'post_id', 600, 'BA_USING'],
+    'dongchedi_koubei_post': ['etl_post', 'post_id', 600, 'BA_USING'],
+    'dongchedi_wenzhang_comment': ['etl_comment', 'comment_id', 600, 'BA_USING'],
+    'dongchedi_cheyouquan_comment': ['etl_comment', 'comment_id', 600, 'BA_USING'],
+    'dongchedi_koubei_comment': ['etl_comment', 'comment_id', 600, 'BA_USING'],
+    'dongchedi_user_info': ['etl_user', 'user_id', 600, 'BA_USING'],
 }
 
+# insert_table与select_table对应关系
+post_list = ['autohome_wenzhang_post', 'autohome_luntan_post', 'autohome_koubei_post','dongchedi_wenzhang_post',
+             'dongchedi_cheyouquan_post', 'dongchedi_koubei_post', 'bilibili_video_post',
+             'weibo_auth_post', 'weibo_search_post', 'xiaohongshu_search_post', 'moment']
+cmt_list = ['autohome_wenzhang_comment', 'autohome_luntan_comment', 'autohome_koubei_comment',
+            'dongchedi_wenzhang_comment', 'dongchedi_cheyouquan_comment', 'dongchedi_koubei_comment',
+            'bilibili_video_comment','bilibili_video_danmu', 'weibo_comment', 'xiaohongshu_comment',
+            'momentcomment', 'smart_tucaoba_comment']
+user_list = ['autohome_user_info', 'dongchedi_user_info', 'weibo_user_info', 'xiaohongshu_user_info', 'bilibili_user_info', 'user_base']
+
 def get_datetime_now():
     return datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
 
 def combine_text(df):
     data_list = df.tolist()
     return '\n'.join(i for i in data_list if i is not None)
 
@@ -219,25 +229,14 @@
         for row in df1:  # 循环每一行数据，组装成一个字典，然后得到字典的列表
             lst.append(dict(zip(column_list, list(row))))
         conn.close() # 关闭数据库连接
     except Exception as ex:
         print(ex)
     return lst
 
-# insert_table与select_table对应关系
-post_list = ['autohome_wenzhang_post', 'autohome_luntan_post', 'autohome_koubei_post','dongchedi_wenzhang_post',
-             'dongchedi_cheyouquan_post', 'dongchedi_koubei_post', 'bilibili_video_post',
-             'weibo_auth_post', 'weibo_search_post', 'xiaohongshu_search_post', 'moment']
-cmt_list = ['autohome_wenzhang_comment', 'autohome_luntan_comment', 'autohome_koubei_comment', 'dongchedi_wenzhang_comment',
-            'bilibili_video_comment', 'dongchedi_cheyouquan_comment', 'dongchedi_koubei_comment',
-            'bilibili_video_danmu', 'weibo_comment', 'xiaohongshu_comment', 'momentcomment', 'smart_tucaoba_comment']
-user_list = ['autohome_user_info', 'dongchedi_user_info', 'weibo_user_info', 'xiaohongshu_user_info']
-
-
-
 def select_sql_json4loss(select_ip, select_table):  # sql 执行数据库语句
     goal_table = insert_map_detail[select_table][0]
     select_key = insert_map_detail[select_table][1]
     plat_low = insert_map_detail[select_table][2]
     plat_high = plat_low+100
     if select_table in post_list:
         goal_key = 'post_id'
@@ -245,15 +244,15 @@
         goal_key = 'comment_id'
     else:
         goal_key = 'user_id'
 
     if select_table == 'momentcomment':
         select_sql = f"""
                 select mc.id id , mc.momentid momentid, mc.createtime createtime, mc.content content, mc.root root, 
-                mc.rootid rootid, mc.createdby createdby, m.source from {select_table} mc
+                mc.rootid rootid, mc.createdby createdby, mc.commentscount commentscount, m.source from {select_table} mc
                 left join moment m on m.id=mc.momentid where mc.{select_key} not in 
                 (select {goal_key} from {goal_table} where platform_id >={plat_low} and platform_id < {plat_high});
                 """
     elif select_table == 'bilibili_video_comment':
         select_sql = f"""
                 select c.*, p.video_id from {select_table} c
                 left join bilibili_video_post p on c.vid=p.video_bvid where {select_key} not in 
@@ -485,15 +484,15 @@
         insert_data["user_gender"] = json_data["user_gender"]
         insert_data["user_country"] = json_data["user_country"]
         insert_data["user_province"] = json_data["user_province"]
         insert_data["user_city"] = json_data["user_city"]
         insert_data["user_birth_date"] = json_data["user_birth_date"]
         # insert_data["user_education"] = json_data[""]
         # insert_data["user_work"] = json_data[""]
-        # insert_data["user_summary"] = json_data[""]
+        insert_data["user_summary"] = None
         insert_data["verified_flag"] = json_data["certified_flag"]
         # insert_data["verified_type"] = json_data["brand_id"]
         # insert_data["verified_reason"] = json_data["series_id"]
         # insert_data["user_label"] = json_data["tiezi_datetime"]
         insert_data["user_post_count"] = json_data["tiezi_count"]
         insert_data["following_count"] = json_data["following_count"]
         insert_data["follower_count"] = json_data["follower_count"]
@@ -554,21 +553,25 @@
         insert_data["spider_datetime"] = json_data["spider_datetime"]
         insert_data["hot_degree"] = 0
     elif select_table == 'bilibili_user_info':
         insert_data["media_id"] = 300
         insert_data["user_id"] = json_data["user_id"]
         insert_data["user_nickname"] = json_data["user_nickname"]
         insert_data["spider_datetime"] = json_data["spider_datetime"]
+        insert_data["user_summary"] = None
     elif select_table == 'moment':
         insert_data["platform_id"] = get_platform_id(json_data["source"])
         insert_data["post_id"] = json_data["id"]
         insert_data["user_id"] = int(json_data["createdby"].replace("CMS", "9999999999").replace("smarter_unknown", "1111111111"))
         insert_data["post_datetime"] = json_data["createtime"]
         insert_data["post_content"] = json_data["content"]
-        insert_data["post_subject"] = json_data["subject"]
+        if json_data["subject"] == '无命名':
+            insert_data["post_subject"] = ''
+        else:
+            insert_data["post_subject"] = json_data["subject"]
         insert_data["post_hashtag"] = get_hashtag(json_data["topics"])
         # insert_data["publish_province"] = ""
         # insert_data["publish_city"] = ""
         # insert_data["post_type"] = ""
         # insert_data["publish_device"] = ""
         insert_data["like_count"] = int(json_data["likescount"])
         insert_data["read_count"] = int(json_data["viewcount"])
@@ -578,27 +581,27 @@
         # insert_data["keyword"] = ""
         insert_data["account_name"] = json_data["source"]
         insert_data["brand_id"] = 45
         if any(word if word in (json_data["subject"]+json_data["content"]) else False for word in ['#3', '三号', '3号', '精灵3', '精灵三']):
             insert_data["series_id"] = 7044
         elif any(word if word in (json_data["subject"]+json_data["content"]) else False for word in ['#1', '一号', '1号', '精灵1', '精灵一']):
             insert_data["series_id"] = 6369
-        insert_data["hot_degree"] = 50*json_data["favoritescount"] + 8*json_data["commentscount"] + 5*json_data["likescount"] + 20*json_data["sharecount"]
+        insert_data["hot_degree"] = 50*int(json_data["favoritescount"]) + 8*int(json_data["commentscount"]) + 5*int(json_data["likescount"]) + 20*int(json_data["sharecount"])
     elif select_table == 'momentcomment':
         insert_data["platform_id"] = get_platform_id(json_data["source"])
         insert_data["comment_id"] = json_data["id"]
         insert_data["user_id"] = json_data["createdby"]
         insert_data["comment_datetime"] = json_data["createtime"]
         # insert_data["comment_province"] = ""
         insert_data["comment_content"] = json_data["content"]
         # insert_data["comment_like_count"] = None
         # insert_data["comment_reply_count"] = None
         insert_data["comment_main_flag"] = get_flag(json_data["root"])
         insert_data["comment_main_id"] = json_data["rootid"]
-        insert_data["post_id"] = json_data["momentid"]
+        insert_data["post_id"] = int(json_data["momentid"])
         insert_data["spider_datetime"] = time.strftime('%Y-%m-%d %H:%M:%S', time.localtime(time.time()))
         insert_data["hot_degree"] = int(json_data["commentscount"])
     elif select_table == 'weibo_auth_post' or select_table == 'weibo_search_post':
         insert_data["platform_id"] = 100
         insert_data["post_id"] = json_data["id"]
         insert_data["user_id"] = json_data["user_id"]
         insert_data["account_name"] = json_data['screen_name']
@@ -876,27 +879,41 @@
         insert_data["user_gender"] = json_data["user_gender"]
         insert_data["user_country"] = json_data["user_country"]
         insert_data["user_province"] = json_data["user_province"]
         insert_data["user_city"] = json_data["user_city"]
         insert_data["user_birth_date"] = json_data["user_birth_date"]
         # insert_data["user_education"] = json_data[""]
         # insert_data["user_work"] = json_data[""]
-        # insert_data["user_summary"] = json_data[""]
+        insert_data["user_summary"] = None
         insert_data["verified_flag"] = json_data["certified_flag"]
         # insert_data["verified_type"] = json_data["brand_id"]
         # insert_data["verified_reason"] = json_data["series_id"]
         # insert_data["user_label"] = json_data["tiezi_datetime"]
         insert_data["user_post_count"] = json_data["post_count"]
         insert_data["following_count"] = json_data["following_count"]
         insert_data["follower_count"] = json_data["follower_count"]
         insert_data["user_level"] = json_data["vip_level"]
         insert_data["register_date"] = json_data["register_date"]
         insert_data["spider_datetime"] = json_data["spider_datetime"]
     else:
         sys.exit()
+    # 判断用户类型
+    # if select_table in user_list:
+    #     # 检查方式1：检查昵称中是否包含某个异常类型关键词
+    #     keyword, user_type1 = gc.speacial_identify_summmary(insert_data['user_nickname'])
+    #     if user_type1:
+    #         feature_list.append('昵称中包含"{}"'.format(keyword))
+    #         type_list.append(user_type1)
+    #     # 检查方式2：检查简介中是否包含某个异常类型关键词
+    #     keyword, user_type2 = gc.speacial_identify_summmary(insert_data['user_summary'])
+    #     if user_type2 and user_type1 != user_type2:
+    #         feature_list.append('简介中包含"{}"'.format(keyword))
+    #         type_list.append(user_type2)
+    #     insert_data['user_feature'] = '|'.join(feature_list)
+    #     insert_data['user_type'] = '|'.join(type_list)
     # 写入数据库
     keys = ", ".join(insert_data.keys())
     values = ", ".join(['%s'] * len(insert_data.keys()))
     if update_flag:
         insert_sql = '''INSERT INTO {table}({keys}) VALUES ({values}) ON DUPLICATE KEY UPDATE'''.format(table=insert_table,
                                                                                                         keys=keys,
                                                                                                         values=values)
@@ -908,46 +925,46 @@
                     INSERT ignore INTO {table}({keys}) VALUES ({values})
                     """.format(table=insert_table, keys=keys, values=values)
         # print(insert_sql)
         insert_cursor.executemany(insert_sql, [tuple(insert_data.values())])
     insert_conn.commit()
 
 def start_sql_insert_process(select_tbl, start_dt, end_dt):
-    insert_table = insert_map_detail[select_tbl][0]
-    print(f'\n-----当前将{select_tbl}导入{insert_table}中-----')
+    insert_tbl = insert_map_detail[select_tbl][0]
+    print(f'\n-----当前将{select_tbl}导入{insert_tbl}中-----')
     if select_tbl == 'user_base':
         select_ip = 'BI_READ'
         insert_ip = 'BA_USING'
     else:
         select_ip = 'BA_USING'
         insert_ip = 'BA_USING'
     res = select_sql_json(select_ip, select_tbl, start_dt, end_dt)
-    for data in tqdm(res, desc=f'当前将{select_tbl}导入{insert_table}中'):
+    for data in tqdm(res, desc=f'当前将{select_tbl}导入{insert_tbl}中' ,ncols=100):
         for (k, v) in data.items():
             try:
                 if np.isnan(data[k]):
                     data[k] = None
             except:
                 continue
         try:
-            insert_json_sql(data, insert_ip, insert_table, select_tbl, update_flag=True)
+            insert_json_sql(data, insert_ip, insert_tbl, select_tbl, update_flag=True)
         except:
             print('数据插入失败：', data)
 
-def mysql_transmit_data(select_ip, insert_ip, select_table, start_datetime, end_datetime, update_flag):
-    insert_table = insert_map[select_table]
-    print(f'\n-----当前将{select_table}导入{insert_table}中-----')
-    res = select_sql_json(select_ip, select_table, start_datetime, end_datetime)
+def mysql_transmit_data(select_ip, insert_ip, select_tbl, start_datetime, end_datetime, update_flag):
+    insert_tbl = insert_map_detail[select_tbl][0]
+    print(f'\n-----当前将{select_tbl}导入{insert_tbl}中-----')
+    res = select_sql_json(select_ip, select_tbl, start_datetime, end_datetime)
     if len(res) == 0:
         print('此次数据库查询无数据...')
     else:
-        for data in tqdm(res, desc=f'当前将{select_tbl}导入{insert_table}中'):
+        for data in tqdm(res, desc=f'当前将{select_tbl}导入{insert_tbl}中',ncols=100):
             for (k, v) in data.items():
                 try:
                     if np.isnan(data[k]):
                         data[k] = None
                 except:
                     continue
             try:
-                insert_json_sql(data, insert_ip, insert_table, select_table, update_flag)
+                insert_json_sql(data, insert_ip, insert_tbl, select_tbl, update_flag)
             except:
                 print('数据插入失败：', data)
```

### Comparing `general_calculator_zsd-1.1.4/setup.py` & `general_calculator_zsd-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='general_calculator_zsd',
-    version='1.1.4',
+    version='1.1.5',
     author='colin zhang',
     author_email='zsd0830@163.com',
     description='通用脚本及数据导入脚本，不定期按需更新。',
     long_description_content_type="""text/markdown""",
     url='',
     packages=find_packages(),
     classifiers=[
```

