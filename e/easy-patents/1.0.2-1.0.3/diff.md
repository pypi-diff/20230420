# Comparing `tmp/easy_patents-1.0.2.tar.gz` & `tmp/easy_patents-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easy_patents-1.0.2.tar", last modified: Fri Jan 28 10:03:10 2022, max compression
+gzip compressed data, was "dist/easy_patents-1.0.3.tar", last modified: Thu Apr 20 12:20:11 2023, max compression
```

## Comparing `easy_patents-1.0.2.tar` & `easy_patents-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-28 10:03:10.000000 easy_patents-1.0.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-28 10:03:10.000000 easy_patents-1.0.2/easy_patents/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-28 10:03:10.000000 easy_patents-1.0.2/easy_patents/config/
--rw-r--r--   0 root         (0) root         (0)      172 2022-01-28 10:03:09.000000 easy_patents-1.0.2/easy_patents/config/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-28 10:03:10.000000 easy_patents-1.0.2/easy_patents/sample/
--rw-r--r--   0 root         (0) root         (0)     2166 2022-01-23 13:19:58.000000 easy_patents-1.0.2/easy_patents/sample/sample.py
--rw-r--r--   0 root         (0) root         (0)     5306 2022-01-25 04:26:25.000000 easy_patents-1.0.2/easy_patents/sample/sample_check_due_date.py
--rw-r--r--   0 root         (0) root         (0)     3451 2022-01-20 10:22:47.000000 easy_patents-1.0.2/easy_patents/sample/sample_update_monitor_excel.py
--rw-r--r--   0 root         (0) root         (0)     2808 2022-01-28 09:59:46.000000 easy_patents-1.0.2/easy_patents/auth_info.py
--rw-r--r--   0 root         (0) root         (0)     1113 2022-01-23 12:53:38.000000 easy_patents-1.0.2/easy_patents/delete_caches.py
--rw-r--r--   0 root         (0) root         (0)     1574 2022-01-19 10:13:25.000000 easy_patents-1.0.2/easy_patents/errors.py
--rw-r--r--   0 root         (0) root         (0)      934 2022-01-28 09:52:02.000000 easy_patents-1.0.2/easy_patents/get_apitoken.py
--rw-r--r--   0 root         (0) root         (0)    37525 2022-01-22 05:01:39.000000 easy_patents-1.0.2/easy_patents/get_info.py
--rw-r--r--   0 root         (0) root         (0)     1321 2022-01-28 09:53:33.000000 easy_patents-1.0.2/easy_patents/update_authinfo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-28 10:03:10.000000 easy_patents-1.0.2/easy_patents.egg-info/
--rw-r--r--   0 root         (0) root         (0)      243 2022-01-28 10:03:10.000000 easy_patents-1.0.2/easy_patents.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      531 2022-01-28 10:03:10.000000 easy_patents-1.0.2/easy_patents.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-28 10:03:10.000000 easy_patents-1.0.2/easy_patents.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       34 2022-01-28 10:03:10.000000 easy_patents-1.0.2/easy_patents.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-01-28 10:03:10.000000 easy_patents-1.0.2/easy_patents.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       85 2022-01-21 06:03:13.000000 easy_patents-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)       69 2022-01-19 22:48:34.000000 easy_patents-1.0.2/README.md
--rw-r--r--   0 root         (0) root         (0)      448 2022-01-28 10:00:12.000000 easy_patents-1.0.2/setup.py
--rw-r--r--   0 root         (0) root         (0)      243 2022-01-28 10:03:10.000000 easy_patents-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2022-01-28 10:03:10.000000 easy_patents-1.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 12:20:11.000000 easy_patents-1.0.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 12:20:11.000000 easy_patents-1.0.3/easy_patents/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 12:20:11.000000 easy_patents-1.0.3/easy_patents/config/
+-rw-r--r--   0 root         (0) root         (0)      172 2023-04-20 12:20:11.000000 easy_patents-1.0.3/easy_patents/config/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 12:20:11.000000 easy_patents-1.0.3/easy_patents/sample/
+-rw-r--r--   0 root         (0) root         (0)     1165 2022-04-30 07:02:34.000000 easy_patents-1.0.3/easy_patents/sample/mail_notify.py
+-rw-r--r--   0 root         (0) root         (0)     2166 2022-04-30 07:02:34.000000 easy_patents-1.0.3/easy_patents/sample/sample.py
+-rw-r--r--   0 root         (0) root         (0)     7932 2022-04-30 07:02:34.000000 easy_patents-1.0.3/easy_patents/sample/sample_check_due_date.py
+-rw-r--r--   0 root         (0) root         (0)     3451 2022-04-30 07:02:34.000000 easy_patents-1.0.3/easy_patents/sample/sample_update_monitor_excel.py
+-rw-r--r--   0 root         (0) root         (0)     2808 2022-04-30 07:02:34.000000 easy_patents-1.0.3/easy_patents/auth_info.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2022-04-30 07:02:34.000000 easy_patents-1.0.3/easy_patents/delete_caches.py
+-rw-r--r--   0 root         (0) root         (0)     1574 2022-04-30 07:02:34.000000 easy_patents-1.0.3/easy_patents/errors.py
+-rw-r--r--   0 root         (0) root         (0)      934 2022-04-30 07:02:34.000000 easy_patents-1.0.3/easy_patents/get_apitoken.py
+-rw-r--r--   0 root         (0) root         (0)    34816 2023-04-20 12:14:28.000000 easy_patents-1.0.3/easy_patents/get_info.py
+-rw-r--r--   0 root         (0) root         (0)     1321 2022-04-30 07:02:34.000000 easy_patents-1.0.3/easy_patents/update_authinfo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 12:20:11.000000 easy_patents-1.0.3/easy_patents.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      243 2023-04-20 12:20:11.000000 easy_patents-1.0.3/easy_patents.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      566 2023-04-20 12:20:11.000000 easy_patents-1.0.3/easy_patents.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 12:20:11.000000 easy_patents-1.0.3/easy_patents.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-20 12:20:11.000000 easy_patents-1.0.3/easy_patents.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-20 12:20:11.000000 easy_patents-1.0.3/easy_patents.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2022-04-30 07:02:34.000000 easy_patents-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)       69 2022-04-30 07:02:34.000000 easy_patents-1.0.3/README.md
+-rw-r--r--   0 root         (0) root         (0)      448 2023-04-20 12:17:12.000000 easy_patents-1.0.3/setup.py
+-rw-r--r--   0 root         (0) root         (0)      243 2023-04-20 12:20:11.000000 easy_patents-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-20 12:20:11.000000 easy_patents-1.0.3/setup.cfg
```

### Comparing `easy_patents-1.0.2/easy_patents/sample/sample.py` & `easy_patents-1.0.3/easy_patents/sample/sample.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.2/easy_patents/sample/sample_update_monitor_excel.py` & `easy_patents-1.0.3/easy_patents/sample/sample_update_monitor_excel.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.2/easy_patents/auth_info.py` & `easy_patents-1.0.3/easy_patents/auth_info.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.2/easy_patents/delete_caches.py` & `easy_patents-1.0.3/easy_patents/delete_caches.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.2/easy_patents/errors.py` & `easy_patents-1.0.3/easy_patents/errors.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.2/easy_patents/get_apitoken.py` & `easy_patents-1.0.3/easy_patents/get_apitoken.py`

 * *Files identical despite different names*

### Comparing `easy_patents-1.0.2/easy_patents/get_info.py` & `easy_patents-1.0.3/easy_patents/get_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 import requests
 import mojimoji
 import time
 import datetime
 import configparser
 import zipfile
 import json
@@ -61,178 +62,15 @@
     # ステータスコードを確認してエラーの場合にはエラーを投げる
     # 対象とするのはjsonのみ
     if not isinstance(response, requests.Response):
         is_error(response)
     return response
 
 
-def get_app_progress(case_number):
-    '''
-    特許経過情報の取得
-    https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-app_progress
-
-    Parameters
-    ----------
-    case_number : str
-        出願番号
-        全角は半角に変換される。また-と/は無視される。
-    accesstoken : str
-        アクセストークン
-
-    Returns
-    -------
-    json
-        特許経過情報のJsonデータ
-
-    Examples
-    --------
-    >>> info = get_app_progress("２０２０－００８４２３")
-    >>> info["result"]["data"]["inventionTitle"]
-    '管理システム及び管理方法'
-    '''
-    url = make_url("app_progress", case_number)
-    return get_api_info(url)
-
-
-def get_app_progress_simple(case_number):
-    '''
-    指定された特許出願番号に紐づく経過情報（優先権基礎情報、原出願情報、分割出願群情報を含まない）を取得する。
-    https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-app_progress_simple
-
-    Parameters
-    ----------
-    case_number : str
-        出願番号
-        全角は半角に変換される。また-と/は無視される。
-    accesstoken : str
-        アクセストークン
-
-    Returns
-    -------
-    json
-        特許経過情報のJsonデータ
-
-    Examples
-    --------
-    >>> info = get_app_progress_simple("２０２０－００８４２３")
-    >>> info["result"]["data"]["inventionTitle"]
-    '管理システム及び管理方法'
-    '''
-    url = make_url("app_progress_simple", case_number)
-    return get_api_info(url)
-
-
-def get_divisional_app_info(case_number):
-    '''
-    指定された特許出願番号に紐づく分割出願情報を取得する。
-    https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-divisional_app_info
-
-    Parameters
-    ----------
-    case_number : str
-        出願番号
-        全角は半角に変換される。また-と/は無視される。
-    accesstoken : str
-        アクセストークン
-
-    Returns
-    -------
-    json
-        分割出願情報のJsonデータ
-
-    Examples
-    --------
-    >>> info = get_divisional_app_info("２００７－０３５９３７")
-    >>> info["result"]["data"]['parentApplicationInformation'] ['parentApplicationNumber']
-    '2000009310'
-    '''
-    url = make_url("divisional_app_info", case_number)
-    return get_api_info(url)
-
-
-def get_priority_right_app_info(case_number):
-    '''
-    指定された特許出願番号に紐づく優先基礎出願情報を取得する。
-    https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-priority_right_app_info
-
-    Parameters
-    ----------
-    case_number : str
-        出願番号
-        全角は半角に変換される。また-と/は無視される。
-    accesstoken : str
-        アクセストークン
-
-    Returns
-    -------
-    json
-        優先基礎情報のJsonデータ
-
-    Examples
-    --------
-    >>> info = get_priority_right_app_info("2020008423")
-    >>> info["result"]["data"]["priorityRightInformation"][0]['nationalPriorityDate']
-    '20190730'
-    '''
-    url = make_url("priority_right_app_info", case_number)
-    return get_api_info(url)
-
-
-def get_applicant_attorney_cd(code):
-    '''
-    指定された申請人コードで申請人(出願人・代理人)氏名・名称を取得する。
-    https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-applicant_attorney-cd
-
-    Parameters
-    ----------
-    code : str
-        申請人コード
-        全角は半角に変換される。また-と/は無視される。
-
-    Returns
-    -------
-    json
-        申請人情報のJsonデータ
-
-    Examples
-    --------
-    >>> info = get_applicant_attorney_cd("718000266")
-    >>> info["result"]["data"]["applicantAttorneyName"]
-    '特許庁長官'
-    '''
-    url = make_url("applicant_attorney_cd", code)
-    return get_api_info(url)
-
-
-def get_applicant_attorney(name):
-    '''
-    指定された申請人氏名・名称を完全一致検索で、申請人(出願人・代理人)コードを取得する。
-    https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-applicant_attorney
-
-    Parameters
-    ----------
-    name : str
-        氏名
-
-    Returns
-    -------
-    json
-        申請人情報のJsonデータ
-
-    Examples
-    --------
-    >>> info = get_applicant_attorney("特許庁長官")
-    >>> info["result"]["data"]["applicantAttorney"][0]['applicantAttorneyCd']
-    '718000266'
-    '''
-    url = make_url("applicant_attorney", name, convert=False)
-    return get_api_info(url)
-
-
-def get_case_number_reference(seed, case_number):
+def get_case_number_reference(seed, case_number, law="patent"):
     '''
     指定された種別と案件番号に紐づく案件番号を取得する。
     https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-case_number_reference
 
     Parameters
     ----------
     seed : str
@@ -242,219 +80,15 @@
         全角は半角に変換される。また-と/は無視される。
 
     Returns
     -------
     json
         案件情報のJsonデータ
     '''
-    url = make_url("case_number_reference", case_number, seed=seed)
-    return get_api_info(url)
-
-
-def get_application_reference(case_number):
-    '''
-    出願について出願番号に紐づく案件番号を取得する。
-
-    Parameters
-    ----------
-    case_number : str
-        出願番号
-        全角は半角に変換される。また-と/は無視される。
-    accesstoken : str
-        アクセストークン
-
-    Returns
-    -------
-    json
-        案件情報のJsonデータ
-
-    Examples
-    --------
-    >>> info = get_application_reference("2020008423")
-    >>> info['result']["data"]["publicationNumber"]
-    '2021022359'
-    '''
-    return get_case_number_reference('application', case_number)
-
-
-def get_publication_reference(case_number):
-    '''
-    公開について公開・公表番号に紐づく案件番号を取得する。
-
-    Parameters
-    ----------
-    case_number : str
-        公開・公表番号
-        全角は半角に変換される。また-と/は無視される。
-
-    Returns
-    -------
-    json
-        案件情報のJsonデータ
-
-    Examples
-    --------
-    >>> info = get_publication_reference("2021022359")
-    >>> info['result']["data"]["registrationNumber"]
-    '6691280'
-    '''
-    return get_case_number_reference('publication', case_number)
-
-
-def get_registration_reference(case_number):
-    '''
-    登録について登録番号に紐づく案件番号を取得する。
-
-    Parameters
-    ----------
-    case_number : str
-        登録番号
-        全角は半角に変換される。また-と/は無視される。
-
-    Returns
-    -------
-    json
-        案件情報のJsonデータ
-
-    Examples
-    --------
-    >>> info = get_registration_reference("6691280")
-    >>> info['result']["data"]["applicationNumber"]
-    '2020008423'
-    '''
-    return get_case_number_reference('registration', case_number)
-
-
-def get_app_doc_cont_opinion_amendment(case_number):
-    '''
-    指定された特許出願番号に対応する実体審査における特許申請書類の実体ファイル（意見書・手続補正書）のZIPファイルをダウンロードする。
-    https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-app_doc_cont_opinion_amendment
-
-    Parameters
-    ----------
-    case_number : str
-        出願番号
-        全角は半角に変換される。また-と/は無視される。
-
-    Returns
-    -------
-    zipを含むレスポンス
-        意見書・手続き補正書のzip
-
-    Examples
-    --------
-    >>> info = get_app_doc_cont_opinion_amendment("2020008423")
-    >>> info.headers['content-type']
-    'application/zip'
-    '''
-    url = make_url("app_doc_cont_opinion_amendment", case_number)
-    return get_api_info(url)
-
-
-def get_app_doc_cont_refusal_reason_decision(case_number):
-    '''
-    指定された特許出願番号に対応する実体審査における発送書類の実体ファイル（拒絶理由通知書、特許査定、拒絶査定、補正の却下の決定）のZIPファイルをダウンロードする。
-    https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-app_doc_cont_opinion_amendment
-
-    Parameters
-    ----------
-    case_number : str
-        出願番号
-        全角は半角に変換される。また-と/は無視される。
-
-    Returns
-    -------
-    zipを含むレスポンス
-        拒絶理由通知等
-
-    Examples
-    --------
-    >>> info = get_app_doc_cont_refusal_reason_decision("2020008423")
-    >>> info.headers['content-type']
-    'application/zip'
-    '''
-    url = make_url("app_doc_cont_refusal_reason_decision", case_number)
-    return get_api_info(url)
-
-
-def get_app_doc_cont_refusal_reason(case_number):
-    '''
-    指定された特許出願番号に対応する拒絶理由通知書のZIPファイルをダウンロードする。
-    https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-app_doc_cont_refusal_reason
-
-    Parameters
-    ----------
-    case_number : str
-        出願番号
-        全角は半角に変換される。また-と/は無視される。
-
-    Returns
-    -------
-    zipを含むレスポンス
-        拒絶理由通知等
-
-    Examples
-    --------
-    >>> info = get_app_doc_cont_refusal_reason("2007035937")
-    >>> info.headers['content-type']
-    'application/zip'
-    '''
-    url = make_url("app_doc_cont_refusal_reason", case_number)
-    return get_api_info(url)
-
-
-def get_cite_doc_info(case_number):
-    '''
-    指定された特許出願番号に紐づく引用文献情報を取得する。
-    https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-cite-doc-info
-
-    Parameters
-    ----------
-    case_number : str
-        出願番号
-        全角は半角に変換される。また-と/は無視される。
-
-    Returns
-    -------
-    json
-        引用文献情報のjsonデータ
-
-    Examples
-    --------
-    >>> info = get_cite_doc_info("2020008423")
-    >>> info["result"]["data"]["patentDoc"][0]["documentNumber"]
-    'JPA 421211144'
-    '''
-    url = make_url("cite_doc_info", case_number)
-    return get_api_info(url)
-
-
-def get_registration_info(case_number):
-    '''
-    指定された特許出願番号に紐づく登録情報を取得する。
-    https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-registration-info
-
-    Parameters
-    ----------
-    case_number : str
-        出願番号
-        全角は半角に変換される。また-と/は無視される。
-
-    Returns
-    -------
-    json
-        登録情報のjsonデータ
-
-    Examples
-    --------
-    >>> info = get_registration_info("2020008423")
-    >>> info["result"]["data"]["expireDate"]
-    '20400122'
-    '''
-    url = make_url("registration_info", case_number)
+    url = make_url("case_number_reference", case_number, seed=seed, law=law)
     return get_api_info(url)
 
 
 def save_to_file(response, dirname, filename=None):
     '''
     responseのcontentをファイルに保存する関数
 
@@ -471,15 +105,16 @@
     Returns
     -------
     str
         保存先ファイルのフルパス
 
     Examples
     --------
-    >>> info = get_app_doc_cont_refusal_reason("2007035937")
+    >>> url = make_url("app_doc_cont_refusal_reason", "2007035937", law="patent")
+    >>> info = get_api_info(url)
     >>> base_dir = os.path.dirname(__file__)
     >>> save_dir = os.path.join(base_dir, "tmp")
     >>> os.makedirs(save_dir, exist_ok=True)
 
     # ファイル名を指定しない場合、Content-Dispositionが使用される
     >>> save_path = save_to_file(info, save_dir)
     >>> save_path
@@ -536,22 +171,24 @@
     '20208423'
     '''
     if delimiter in key:
         first, second = key.split(delimiter)
         key = first + second.zfill(digit)
     return key
 
-def convert_key(key):
+def convert_key(key, law="patent"):
     '''
     半角変換と、出願番号などの形式に沿うように変換する関数
 
     Paramters
     ---------
     key : str
         変換対象文字列
+    law : str
+        patent, design, trademarkのいずれか
 
     Returns
     -------
     str
         変換後の文字列
 
     Examples
@@ -562,27 +199,30 @@
     '2020008423'
     >>> convert_key("2020008423")
     '2020008423'
     >>> convert_key("特許第1234567号")
     '1234567'
     '''
     key = mojimoji.zen_to_han(key)
-    key = key.replace("特願", "")
-    key = key.replace("特開", "")
-    key = key.replace("特表", "")
-    key = key.replace("特許", "")
+    if law == "patent":
+        key = key.replace("特願", "")
+        key = key.replace("特開", "")
+        key = key.replace("特表", "")
+        key = key.replace("特許", "")
+    if law == "design":
+        pass
     key = key.replace("第", "")
     key = key.replace("号", "")
     key = key.replace("公報", "")
     key = zfill_key(key, "-")
     key = zfill_key(key, "/")
     return key
 
 
-def make_url(api_name, key, seed=None, convert=True):
+def make_url(api_name, key, seed=None, convert=True, law='patent'):
     '''
     APIでのアクセス先URLを作成する関数
 
     Parameters
     ----------
     api_name : str
         取得先APIの名前(app_progressなど)
@@ -602,26 +242,28 @@
     --------
     >>> make_url("app_progress", "特願２０２０－８５２４")
     'https://ip-data.jpo.go.jp/api/patent/v1/app_progress/2020008524'
     >>> make_url("app_progress", "特願２０２０－８５２４", convert=False)
     'https://ip-data.jpo.go.jp/api/patent/v1/app_progress/特願２０２０－８５２４'
     >>> make_url("app_progress", "特願２０２０－８５２４", seed="test")
     'https://ip-data.jpo.go.jp/api/patent/v1/app_progress/test/2020008524'
+    >>> make_url("app_progress", "特願２０２０－８５２４", seed="test", law="design")
+    'https://ip-data.jpo.go.jp/api/design/v1/app_progress/test/2020008524'
     '''
-    base_url = "https://ip-data.jpo.go.jp/api/patent/v1"
+    base_url = "https://ip-data.jpo.go.jp/api"
     if convert:
         key = convert_key(key)
     if seed:
-        url = "%s/%s/%s/%s" % (base_url, api_name, seed, key)
+        url = "%s/%s/v1/%s/%s/%s" % (base_url, law, api_name, seed, key)
     else:
-        url = "%s/%s/%s" % (base_url, api_name, key)
+        url = "%s/%s/v1/%s/%s" % (base_url, law, api_name, key)
     return url
 
 
-def make_dir_path(api_type, key, file_type="json"):
+def make_dir_path(api_type, key, law="patent", file_type="json"):
     '''
     ディレクトリパス文字列を作成するとともに、そのディレクトリを作成する関数
 
     Parameters
     ----------
     api_type: str
         app_progressのようなAPIの種別を特定する文字列
@@ -637,69 +279,73 @@
     '''
     if file_type == "zip":
         dir_name = CONFIG['DirPath']['zip_dir']
     else:
         dir_name = CONFIG['DirPath']['data_dir']
     p = pathlib.Path(dir_name)
     if p.is_absolute():
-        dir_path = os.path.join(dir_name, key, api_type)
+        dir_path = os.path.join(dir_name, law, key, api_type)
     else:
         base_dir = os.path.dirname(__file__)
-        dir_path = os.path.join(base_dir, dir_name, key, api_type)
+        dir_path = os.path.join(base_dir, dir_name,law, key, api_type)
     os.makedirs(dir_path, exist_ok=True)
     return dir_path
 
-def unzip_and_save(response, api_type, key, zip_file_name=None):
+def unzip_and_save(response, api_type, key, law, zip_file_name=None):
     '''
     zipを含むレスポンスを、zipの解凍まで行う
 
     Parameters
     ----------
     response: Response
         レスポンスオブジェクト
     api_type: str
         APIの種別
     key: str
         出願番号などのキー
+    law: str
+        patent, design, trademarkのいずれか
     zip_file_name: str
         中間ファイルのzipファイル名を指定したい場合に使用
 
     Returns
     -------
     str
         解凍後のファイルが格納されたディレクトリパス
 
     Examples
     --------
-    >>> info = get_app_doc_cont_refusal_reason("2007035937")
-    >>> unzip_and_save(info, "app_doc_cont_refusal_reason", "2007035937")
-    'data/2007035937/app_doc_cont_refusal_reason'
+    >>> url = make_url("app_doc_cont_refusal_reason", "2007035937", law="patent")
+    >>> info = get_api_info(url)
+    >>> unzip_and_save(info, "app_doc_cont_refusal_reason", "2007035937", law="patent")
+    'data/patent/2007035937/app_doc_cont_refusal_reason'
     '''
     # zipファイルの保存
-    zip_dir = make_dir_path(api_type, key, file_type="zip")
+    zip_dir = make_dir_path(api_type, key, law, file_type="zip")
     zip_path = save_to_file(response, zip_dir, zip_file_name)
 
     # zipファイルの解凍
-    file_dir = make_dir_path(api_type, key, file_type="xml")
+    file_dir = make_dir_path(api_type, key, law, file_type="xml")
 
     with zipfile.ZipFile(zip_path) as z:
         z.extractall(file_dir)
     os.remove(zip_path)
     return file_dir
 
+
 def get_latest_file(file_dir):
     search_path = os.path.join(file_dir, "*")
     files = glob.glob(search_path) 
     if files:
         return max(files, key=os.path.getctime)
     else:
         return ""
 
 
-def get_unzip_data(func, key, reget_date=30):
+def get_unzip_data(api_type, key, law="patent", reget_date=1):
     '''
     unzipしたデータのディレクトリ名を取得する
 
     Parameters
     ----------
     func: func
         API情報取得関数
@@ -712,33 +358,34 @@
     -------
     str
         ディレクトリ名
 
     Examples
     --------
     >>> key = "2020008423"
-    >>> get_unzip_data(get_app_doc_cont_refusal_reason_decision, key)
-    'data/2020008423/app_doc_cont_refusal_reason_decision'
+    >>> get_unzip_data("app_doc_cont_refusal_reason_decision", key)
+    'data/patent/2020008423/app_doc_cont_refusal_reason_decision'
     '''
-    api_type = get_api_type(func)
     key = convert_key(key)
-    file_dir = make_dir_path(api_type, key, file_type="xml")
+    file_dir = make_dir_path(api_type, key, law, file_type="xml")
     now = datetime.datetime.now()
     expire_date = now - datetime.timedelta(days=reget_date)
     latest_file = get_latest_file(file_dir)
     if latest_file:
         file_timestamp = os.path.getctime(latest_file)
         create_date = datetime.datetime.fromtimestamp(file_timestamp)
         if expire_date < create_date:
             return file_dir
-    response = func(key)
-    return unzip_and_save(response, api_type, key)
+
+    url = make_url(api_type, key, law=law)
+    response = get_api_info(url)
+    return unzip_and_save(response, api_type, key, law)
 
 
-def get_json_path(dir_name, non_exist_ok=True):
+def get_json_path(dir_name, law="patent", non_exist_ok=True):
     '''
     指定されたディレクトリにあるjsonパスを返す
     
     Parameters
     ----------
     dir_name: str
         ディレクトリ名
@@ -772,16 +419,16 @@
     Returns
     -------
     str
         保存後のファイル名
 
     Examples
     --------
-    >>> info = get_app_progress("2020-8423")
-    >>> file_dir = make_dir_path("app_progress", "2020008423", file_type="json")
+    >>> info = app_progress("2020-8423")
+    >>> file_dir = make_dir_path("app_progress", "2020008423", "patent", file_type="json")
     >>> file_path = save_json(info, file_dir)
     >>> os.path.exists(file_path)
     True
     '''
     json_path = get_json_path(file_dir)
     now = datetime.datetime.now()
     json_data['ep_data'] = {
@@ -807,132 +454,152 @@
     str
         API情報取得関数を特定する文字列
     '''
     # 関数名のget_以降を取得
     return func.__name__[4:]
 
 
-'''
-def json_serial(obj):
-    if isinstance(obj, datetime):
-        return obj.isoformat()
-    raise TypeError ("Type %s not serializable" % type(obj))
-'''
-
-
-def get_json(func, key, reget_date=30, convert=True):
+def get_json(api_type, key, law="patent", reget_date=1, convert=True):
     '''
     jsonデータを取得する
 
     Parameters
     ----------
     func: func
         API情報を取得するための関数
     key: str
         どの情報化を特定するキー(出願番号など)
+    law : str
+        patent, design, trademarkのいずれか
     reget_date: int
         ファイルの存否に関係なくjsonデータを取得するか
 
     Returns
     -------
     json
         対象のJsonデータ
 
     Examples
     --------
-    >>> info = get_json(get_app_progress, "2020-8422")
+    >>> info = get_json("app_progress", "2020-8422")
     >>> info['result']['data']['inventionTitle']
     '窓装置及び窓の施工方法'
 
-    >>> json_dir = make_dir_path('app_progress', '2020008422', file_type="json")
+    >>> json_dir = make_dir_path('app_progress', '2020008422', "patent", file_type="json")
     >>> search_path = os.path.join(json_dir, "*")
     >>> before_get_json = len(glob.glob(search_path))
 
     # reget_date=0の場合、ファイルの即取得がなされる
-    >>> info = get_json(get_app_progress, "2020-8422", reget_date=0)
+    >>> info = get_json("app_progress", "2020-8422", reget_date=0)
 
     # reget_dateが0でない場合、ファイルの取得日からreget_date経ったときのみ再取得がなされる
-    >>> info = get_json(get_app_progress, "2020-8422", reget_date=30)
+    >>> info = get_json("app_progress", "2020-8422", reget_date=1)
     '''
-    api_type = get_api_type(func)
+    if law not in ["patent", "design", "trademark"]:
+        raise ValueError("Parameter law should be 'patent', 'design' or 'trademark'. Current parameter is %s" % law)
     if convert:
-        key = convert_key(key)
-    json_dir = make_dir_path(api_type, key, file_type="json")
+        key = convert_key(key, law)
+    json_dir = make_dir_path(api_type, key, law, file_type="json")
     json_file = get_json_path(json_dir, non_exist_ok=False)
     if json_file != "":
         now = datetime.datetime.now()
         expire_date = now - datetime.timedelta(days=reget_date)
         with open(json_file) as f:
             json_data = json.load(f)
         create_date = datetime.datetime.strptime(json_data['ep_data']['create_date'], DATETIME_FORMAT)
         if expire_date < create_date:
              return json_data
     # 既存ファイルがないか、再取得日数を過ぎている場合には、
     # API情報を取得する
-    json_data = func(key)
+    #json_data = func(key)
+    if api_type in ["application_reference", "publication_reference","registration_reference"]:
+        seed, _ = api_type.split("_")
+        url = make_url("case_number_reference", key, seed=seed, law=law)
+    elif api_type in ["international_application", "international_publication"]:
+        url = make_url("pct_national_phase_application_number", key, seed=api_type, law=law)
+    else:
+        url = make_url(api_type, key, law=law)
+    json_data = get_api_info(url)
+    
     # 次回以降の処理のために保存
     save_json(json_data, json_dir)
     return json_data
 
 
-def app_progress(case_number, reget_date=30):
+def app_progress(case_number, law="patent", reget_date=1):
     '''
     指定された特許出願番号に紐づく経過情報（優先権基礎情報、原出願情報、分割出願群情報を含まない）を取得する。
     https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-app_progress<
     既存のファイルがある場合には、既存のファイルを読み込む
 
     Parameters
     ----------
     case_number: str
         出願番号
+    law: str
+        patent, design, trademarkのいずれか
     reget_date: int
         データ再取得までの日数
     
     Returns
     -------
     json
         特許経過情報のjsonデータ
 
     Examples
     --------
     >>> info = app_progress("２０２０－００８４２３")
     >>> info["result"]["data"]["inventionTitle"]
     '管理システム及び管理方法'
+    >>> info = app_progress("2022012584", law="design")
+    >>> info["result"]["data"]["designArticle"]
+    '乗用自動車'
+    >>> info = app_progress("2018009480", law="trademark")
+    >>> info["result"]["data"]["trademarkForDisplay"][-3:]
+    '特許庁'
     '''
-    return get_json(get_app_progress, case_number, reget_date)
+    return get_json(sys._getframe().f_code.co_name, case_number, law, reget_date)
 
 
-def app_progress_simple(case_number, reget_date=30):
+def app_progress_simple(case_number, law="patent", reget_date=1):
     '''
     指定された特許出願番号に紐づく経過情報（優先権基礎情報、原出願情報、分割出願群情報を含まない）を取得する。
     https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-app_progress_simple
     既存のファイルがある場合には、既存のファイルを読み込む
 
     Parameters
     ----------
     case_number: str
         出願番号
+    law: str
+        patent, design, trademarkのいずれか
     reget_date: int
         データ再取得までの日数
     
     Returns
     -------
     json
         特許経過情報のjsonデータ
 
     Examples
     --------
     >>> info = app_progress_simple("２０２０－００８４２３")
     >>> info["result"]["data"]["inventionTitle"]
     '管理システム及び管理方法'
+    >>> info = app_progress_simple("2022012584", law="design")
+    >>> info["result"]["data"]["designArticle"]
+    '乗用自動車'
+    >>> info = app_progress_simple("2018009480", law="trademark")
+    >>> info["result"]["data"]["trademarkForDisplay"][-3:]
+    '特許庁'
     '''
-    return get_json(get_app_progress_simple, case_number, reget_date)
+    return get_json(sys._getframe().f_code.co_name, case_number, law, reget_date)
 
 
-def divisional_app_info(case_number, reget_date=30):
+def divisional_app_info(case_number, reget_date=1):
     '''
     指定された特許出願番号に紐づく分割出願情報を取得する。
     https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-divisional_app_info
     既存のファイルがある場合には、既存のファイルを読み込む
 
     Parameters
     ----------
@@ -948,126 +615,158 @@
 
     Examples
     --------
     >>> info = divisional_app_info("２００７－０３５９３７")
     >>> info["result"]["data"]['parentApplicationInformation'] ['parentApplicationNumber']
     '2000009310'
     '''
-    return get_json(get_divisional_app_info, case_number, reget_date)
+    return get_json(sys._getframe().f_code.co_name, case_number, 'patent', reget_date)
 
 
-def priority_right_app_info(case_number, reget_date=30):
+def priority_right_app_info(case_number, law="patent", reget_date=1):
     '''
     指定された特許出願番号に紐づく優先基礎出願情報を取得する。
     https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-priority_right_app_info
     既存のファイルがある場合には、既存のファイルを読み込む
 
     Parameters
     ----------
     case_number: str
         出願番号
+    law: str
+        patent, design, trademarkのいずれか
     reget_date: int
         データ再取得までの日数
     
     Returns
     -------
     json
         優先出願情報のjsonデータ
 
     Examples
     --------
     >>> info = priority_right_app_info("2020008423")
     >>> info["result"]["data"]["priorityRightInformation"][0]['nationalPriorityDate']
     '20190730'
+    >>> info = priority_right_app_info("2022012584", law="design")
+    >>> info["result"]["data"]["priorityRightInformation"][0]['parisPriorityApplicationNumber']
+    '402021101137.4'
+    >>> info = priority_right_app_info("2020089151", law="trademark")
+    >>> info["result"]["data"]["priorityRightInformation"][0]['parisPriorityApplicationNumber']
+    '00003477499'
     '''
-    return get_json(get_priority_right_app_info, case_number, reget_date)
+    return get_json(sys._getframe().f_code.co_name, case_number, law, reget_date)
 
 
-def applicant_attorney_cd(code, reget_date=30):
+def applicant_attorney_cd(code, law="patent", reget_date=1):
     '''
     指定された申請人コードで申請人(出願人・代理人)氏名・名称を取得する。
     https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-applicant_attorney-cd
     既存のファイルがある場合には、既存のファイルを読み込む
 
     Parameters
     ----------
     code: str
         申請人コード
+    law: str
+        patent, design, trademarkのいずれか
     reget_date: int
         データ再取得までの日数
     
     Returns
     -------
     json
         申請人情報のjsonデータ
 
     Examples
     --------
     >>> info = applicant_attorney_cd("718000266")
     >>> info["result"]["data"]["applicantAttorneyName"]
     '特許庁長官'
+    >>> info = applicant_attorney_cd("591037096", law="design")
+    >>> info["result"]["data"]["applicantAttorneyName"]
+    'フオルクスワーゲン・アクチエンゲゼルシヤフト'
+    >>> info = applicant_attorney_cd("718000266", law="trademark")
+    >>> info["result"]["data"]["applicantAttorneyName"]
+    '特許庁長官'
     '''
-    return get_json(get_applicant_attorney_cd, code, reget_date)
+    return get_json(sys._getframe().f_code.co_name, code, law, reget_date)
 
 
-def applicant_attorney(name, reget_date=30):
+def applicant_attorney(name, law="patent", reget_date=1):
     '''
     指定された申請人氏名・名称を完全一致検索で、申請人(出願人・代理人)コードを取得する。
     https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-applicant_attorney
     既存のファイルがある場合には、既存のファイルを読み込む
 
     Parameters
     ----------
     name: str
         申請人名称
+    law: str
+        patent, design, trademarkのいずれか
     reget_date: int
         データ再取得までの日数
     
     Returns
     -------
     json
         申請人情報のjsonデータ
 
     Examples
     --------
     >>> info = applicant_attorney("特許庁長官")
     >>> info["result"]["data"]["applicantAttorney"][0]['applicantAttorneyCd']
     '718000266'
+    >>> info = applicant_attorney("アッコ　ブランズ　コーポレイション", law="design")
+    >>> info["result"]["data"]["applicantAttorney"][0]['applicantAttorneyCd']
+    '516092430'
+    >>> info = applicant_attorney("特許庁長官", law="trademark")
+    >>> info["result"]["data"]["applicantAttorney"][0]['applicantAttorneyCd']
+    '718000266'
     '''
-    return get_json(get_applicant_attorney, name, reget_date, convert=False)
+    return get_json(sys._getframe().f_code.co_name, name, law, reget_date, convert=False)
 
 
-def application_reference(case_number, reget_date=30):
+def application_reference(case_number, law="patent", reget_date=1):
     '''
     出願番号に紐づく案件番号を取得する。
     https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-case_number_reference
     既存のファイルがある場合には、既存のファイルを読み込む
 
     Parameters
     ----------
     case_number: str
         出願番号
+    law: str
+        patent, design, trademarkのいずれか
     reget_date: int
         データ再取得までの日数
     
     Returns
     -------
     json
         案件情報のjsonデータ
 
     Examples
     --------
     >>> info = application_reference("2020008423")
     >>> info['result']["data"]["publicationNumber"]
     '2021022359'
+    >>> info = application_reference("2016500748", law="design")
+    >>> info['result']["data"]["registrationNumber"]
+    '1581216'
+    >>> info = application_reference("2018009480", law="trademark")
+    >>> info['result']["data"]["registrationNumber"]
+    '6036291'
     '''
-    return get_json(get_application_reference, case_number, reget_date)
+    return get_json(sys._getframe().f_code.co_name, case_number, law, reget_date)
 
 
-def publication_reference(case_number, reget_date=30):
+def publication_reference(case_number, reget_date=1):
     '''
     公開について公開・公表番号に紐づく案件番号を取得する。
     https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-case_number_reference
     既存のファイルがある場合には、既存のファイルを読み込む
 
     Parameters
     ----------
@@ -1083,123 +782,149 @@
 
     Examples
     --------
     >>> info = publication_reference("2021022359")
     >>> info['result']["data"]["registrationNumber"]
     '6691280'
     '''
-    return get_json(get_publication_reference, case_number, reget_date)
+    return get_json(sys._getframe().f_code.co_name, case_number, "patent", reget_date)
 
 
-def registration_reference(case_number, reget_date=30):
+def registration_reference(case_number, law="patent", reget_date=1):
     '''
     登録について登録番号に紐づく案件番号を取得する。
     https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-case_number_reference
     既存のファイルがある場合には、既存のファイルを読み込む
 
     Parameters
     ----------
     case_number: str
         登録番号
+    law: str
+        patent, design, trademarkのいずれか
     reget_date: int
         データ再取得までの日数
     
     Returns
     -------
     json
         案件情報のjsonデータ
 
     Examples
     --------
     >>> info = registration_reference("6691280")
     >>> info['result']["data"]["applicationNumber"]
     '2020008423'
+    >>> info = registration_reference("1581216", law="design")
+    >>> info['result']["data"]["applicationNumber"]
+    '2016500748'
+    >>> info = registration_reference("6036291", law="trademark")
+    >>> info['result']["data"]["applicationNumber"]
+    '2018009480'
     '''
-    return get_json(get_registration_reference, case_number, reget_date)
+    return get_json(sys._getframe().f_code.co_name, case_number, law, reget_date)
 
 
-def app_doc_cont_opinion_amendment(case_number, reget_date=30):
+def app_doc_cont_opinion_amendment(case_number, law="patent", reget_date=1):
     '''
     指定された特許出願番号に対応する実体審査における特許申請書類の実体ファイル（意見書・手続補正書）のxmlが格納されたディレクトリパスを返す。
     https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-app_doc_cont_opinion_amendment
     既存のファイルがある場合には、既存のファイルを読み込む
 
     Parameters
     ----------
     case_number: str
         出願番号
+    law: str
+        patent, design, trademarkのいずれか
     reget_date: int
         データ再取得までの日数
     
     Returns
     -------
     str
         ディレクトリパス
 
     Examples
     --------
     >>> app_doc_cont_opinion_amendment("2020008423")
-    'data/2020008423/app_doc_cont_opinion_amendment'
+    'data/patent/2020008423/app_doc_cont_opinion_amendment'
+    >>> app_doc_cont_opinion_amendment("2020021161", law="design")
+    'data/design/2020021161/app_doc_cont_opinion_amendment'
+    >>> app_doc_cont_opinion_amendment("2018039075", law="trademark")
+    'data/trademark/2018039075/app_doc_cont_opinion_amendment'
     '''
-    return get_unzip_data(get_app_doc_cont_opinion_amendment, case_number, reget_date)
+    return get_unzip_data(sys._getframe().f_code.co_name, case_number, law, reget_date)
 
 
-def app_doc_cont_refusal_reason_decision(case_number, reget_date=30):
+def app_doc_cont_refusal_reason_decision(case_number, law="patent", reget_date=1):
     '''
     指定された特許出願番号に対応する実体審査における発送書類の実体ファイル（拒絶理由通知書、特許査定、拒絶査定、補正の却下の決定）のxmlファイルの格納ディレクトリを返す
     https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-app_doc_cont_opinion_amendment
     既存のファイルがある場合には、既存のファイルを読み込む
 
     Parameters
     ----------
     case_number: str
         出願番号
+    law: str
+        patent, design, trademarkのいずれか
     reget_date: int
         データ再取得までの日数
     
     Returns
     -------
     str
         ディレクトリパス
 
     Examples
     --------
     >>> app_doc_cont_refusal_reason_decision("2020008423")
-    'data/2020008423/app_doc_cont_refusal_reason_decision'
+    'data/patent/2020008423/app_doc_cont_refusal_reason_decision'
+    >>> app_doc_cont_refusal_reason_decision("2020009549", law="design")
+    'data/design/2020009549/app_doc_cont_refusal_reason_decision'
+    >>> app_doc_cont_refusal_reason_decision("2021010720", law="trademark")
+    'data/trademark/2021010720/app_doc_cont_refusal_reason_decision'
     '''
-    return get_unzip_data(get_app_doc_cont_refusal_reason_decision, case_number, reget_date)
+    return get_unzip_data(sys._getframe().f_code.co_name, case_number, law, reget_date)
 
 
-def app_doc_cont_refusal_reason(case_number, reget_date=30):
+def app_doc_cont_refusal_reason(case_number, law="patent", reget_date=1):
     '''
     指定された特許出願番号に対応する拒絶理由通知書のZIPファイルをダウンロードする。
     https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-app_doc_cont_refusal_reason
     既存のファイルがある場合には、既存のファイルを読み込む
 
     Parameters
     ----------
     case_number: str
         出願番号
+    law: str
+        patent, design, trademarkのいずれか
     reget_date: int
         データ再取得までの日数
     
     Returns
     -------
     str
         ディレクトリパス
 
     Examples
     --------
     >>> app_doc_cont_refusal_reason("2007035937")
-    'data/2007035937/app_doc_cont_refusal_reason'
+    'data/patent/2007035937/app_doc_cont_refusal_reason'
+    >>> app_doc_cont_refusal_reason("2020009549", law="design")
+    'data/design/2020009549/app_doc_cont_refusal_reason'
+    >>> app_doc_cont_refusal_reason("2021010720", law="trademark")
+    'data/trademark/2021010720/app_doc_cont_refusal_reason'
     '''
-    return get_unzip_data(get_app_doc_cont_refusal_reason, case_number, reget_date)
+    return get_unzip_data(sys._getframe().f_code.co_name, case_number, law, reget_date)
 
 
-def cite_doc_info(case_number, reget_date=30):
+def cite_doc_info(case_number, reget_date=1):
     '''
     指定された特許出願番号に紐づく引用文献情報を取得する。
     https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-cite-doc-info
     既存のファイルがある場合には、既存のファイルを読み込む
 
     Parameters
     ----------
@@ -1213,42 +938,134 @@
     json 
         引用文献情報のjsonデータ
 
     Examples
     --------
     >>> info = cite_doc_info("2020008423")
     >>> info["result"]["data"]["patentDoc"][0]["documentNumber"]
-    'JPA 421211144'
+    'JPA 426119839'
     '''
-    return get_json(get_cite_doc_info, case_number, reget_date)
+    return get_json(sys._getframe().f_code.co_name, case_number, "patent", reget_date)
 
 
-def registration_info(case_number, reget_date=30):
+def registration_info(case_number, law="patent", reget_date=1):
     '''
     指定された特許出願番号に紐づく登録情報を取得する。
     https://ip-data.jpo.go.jp/api_guide/api_reference.html#/%E7%89%B9%E8%A8%B1%E6%83%85%E5%A0%B1%E5%8F%96%E5%BE%97API/get-registration-info
     既存のファイルがある場合には、既存のファイルを読み込む
 
     Parameters
     ----------
     case_number: str
         出願番号
+    law: str
+        patent, design, trademarkのいずれか
     reget_date: int
         データ再取得までの日数
     
     Returns
     -------
     json 
         登録情報のjsonデータ
 
     Examples
     --------
     >>> info = registration_info("2020008423")
     >>> info["result"]["data"]["expireDate"]
     '20400122'
+    >>> info = registration_info("2022012584", law="design")
+    >>> info["result"]["data"]["expireDate"]
+    '20470512'
+    >>> info = registration_info("2018009480", law="trademark")
+    >>> info["result"]["data"]["expireDate"]
+    '20280420'
+    '''
+    return get_json(sys._getframe().f_code.co_name, case_number, law, reget_date)
+
+def jpp_fixed_address(case_number, law="patent", reget_date=1):
+    '''
+    指定された出願番号に紐づくJ-PlatPatの固定アドレスを取得する。
+    既存のファイルがある場合には、既存のファイルを読み込む
+
+    Parameters
+    ----------
+    case_number: str
+        出願番号
+    law: str
+        patent, design, trademarkのいずれか
+    reget_date: int
+        データ再取得までの日数
+    
+    Returns
+    -------
+    json 
+        登録情報のjsonデータ
+
+    Examples
+    --------
+    >>> info = jpp_fixed_address("2020008423")
+    >>> info["result"]["data"]["URL"]
+    'https://www.j-platpat.inpit.go.jp/c1800/PU/JP-2020-008423/A9121C47B81363B5C6B5BE66C53D6572A2DB04417E66CF7B8D79A166F5ADB8C9/10/ja'
+    >>> info = jpp_fixed_address("2022012584", law="design")
+    >>> info["result"]["data"]["URL"]
+    'https://www.j-platpat.inpit.go.jp/c1800/DE/JP-2022-012584/27DBA8496517D2F4B482AEB97A0FC03B7FCD90E236B6B4847FDC349CB22E6034/30/ja'
+    >>> info = jpp_fixed_address("2018009480", law="trademark")
+    >>> info["result"]["data"]["URL"]
+    'https://www.j-platpat.inpit.go.jp/c1800/TR/JP-2018-009480/25AD3EA6D2E6DB18D4FF56AC680FB8A7D35923B6C546C571462BD72ABAFBACE0/40/ja'
+    '''
+    return get_json(sys._getframe().f_code.co_name, case_number, law, reget_date)
+
+def international_application(case_number, reget_date=1):
+    '''
+    国際出願番号に紐づくPCT出願の日本国内移行後の出願番号を取得する。
+    既存のファイルがある場合には、既存のファイルを読み込む
+
+    Parameters
+    ----------
+    case_number: str
+        国際出願番号
+    reget_date: int
+        データ再取得までの日数
+    
+    Returns
+    -------
+    json 
+        登録情報のjsonデータ
+
+    Examples
+    --------
+    >>> info = international_application("JP2019011858")
+    >>> info["result"]["data"]["applicationNumber"]
+    '2019563629'
+    '''
+    return get_json(sys._getframe().f_code.co_name, case_number, "patent", reget_date)
+
+
+def international_publication(case_number, reget_date=1):
+    '''
+    国際公開番号に紐づくPCT出願の日本国内移行後の出願番号を取得する。
+    既存のファイルがある場合には、既存のファイルを読み込む
+
+    Parameters
+    ----------
+    case_number: str
+        国際公開番号
+    reget_date: int
+        データ再取得までの日数
+    
+    Returns
+    -------
+    json 
+        登録情報のjsonデータ
+
+    Examples
+    --------
+    >>> info = international_publication("WO2019011858")
+    >>> info["result"]["data"]["applicationNumber"]
+    '2020501130'
     '''
-    return get_json(get_registration_info, case_number, reget_date)
+    return get_json(sys._getframe().f_code.co_name, case_number, "patent", reget_date)
 
 
 if __name__ == "__main__":
      import doctest
      doctest.testmod()
```

### Comparing `easy_patents-1.0.2/easy_patents/update_authinfo.py` & `easy_patents-1.0.3/easy_patents/update_authinfo.py`

 * *Files identical despite different names*

