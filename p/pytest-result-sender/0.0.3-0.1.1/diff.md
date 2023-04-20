# Comparing `tmp/pytest_result_sender-0.0.3-py3-none-any.whl.zip` & `tmp/pytest_result_sender-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2112 bytes, number of entries: 6
--rw-r--r--  2.0 unx      124 b- defN 16-Jan-01 00:00 pytest_result_sender/__init__.py
--rw-r--r--  2.0 unx      386 b- defN 16-Jan-01 00:00 pytest_result_sender/plugin.py
-?rw-------  2.0 unx       61 b- defN 16-Jan-01 00:00 pytest_result_sender-0.0.3.dist-info/entry_points.txt
-?rw-------  2.0 unx       87 b- defN 16-Jan-01 00:00 pytest_result_sender-0.0.3.dist-info/WHEEL
-?rw-------  2.0 unx      568 b- defN 16-Jan-01 00:00 pytest_result_sender-0.0.3.dist-info/METADATA
-?rw-------  2.0 unx      526 b- defN 16-Jan-01 00:00 pytest_result_sender-0.0.3.dist-info/RECORD
-6 files, 1752 bytes uncompressed, 1144 bytes compressed:  34.7%
+Zip file size: 2872 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      127 b- defN 16-Jan-01 00:00 pytest_result_sender/__init__.py
+-rw-r--r--  2.0 unx     2494 b- defN 16-Jan-01 00:00 pytest_result_sender/plugin.py
+?rw-------  2.0 unx       51 b- defN 16-Jan-01 00:00 pytest_result_sender-0.1.1.dist-info/entry_points.txt
+?rw-------  2.0 unx       87 b- defN 16-Jan-01 00:00 pytest_result_sender-0.1.1.dist-info/WHEEL
+?rw-------  2.0 unx      308 b- defN 16-Jan-01 00:00 pytest_result_sender-0.1.1.dist-info/METADATA
+?rw-------  2.0 unx      527 b- defN 16-Jan-01 00:00 pytest_result_sender-0.1.1.dist-info/RECORD
+6 files, 3594 bytes uncompressed, 1904 bytes compressed:  47.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pytest_result_sender/__init__.py
 Comment: 
 
 Filename: pytest_result_sender/plugin.py
 Comment: 
 
-Filename: pytest_result_sender-0.0.3.dist-info/entry_points.txt
+Filename: pytest_result_sender-0.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: pytest_result_sender-0.0.3.dist-info/WHEEL
+Filename: pytest_result_sender-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pytest_result_sender-0.0.3.dist-info/METADATA
+Filename: pytest_result_sender-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pytest_result_sender-0.0.3.dist-info/RECORD
+Filename: pytest_result_sender-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytest_result_sender/__init__.py

```diff
@@ -1,6 +1,6 @@
 """
-@Filename:   src/pytest_result_sender/__init__
+@Filename:   src/pytest_result_sender/__init__.py
 @Author:      北凡
-@Time:        2023/4/17 15:42
+@Time:        2023/4/18 21:18
 @Describe:    ...
 """
```

## pytest_result_sender/plugin.py

```diff
@@ -1,16 +1,88 @@
-from dataclasses import dataclass
-from datetime import datetime, timedelta
+"""
+@Filename:   src/pytest_result_sender/plugin.py
+@Author:      北凡
+@Time:        2023/4/18 21:20
+@Describe:    ...
+"""
+from datetime import datetime
 
 import pytest
+import requests
 
-def  pytest_collection_finish(session):
-    print('用例总数:', len(session.items))
+data = {
+    "passed": 0,
+    "failed": 0,
+}
 
 
-@pytest.hookimpl(tryfirst=True, hookwrapper=True)
-def pytest_runtest_makereport(item, call):
-    outcome = yield
-    result = outcome.get_result()
+def pytest_addoption(parser):
+    parser.addini("send_when", help="什么时候发送测试结果， every表示每次都发送 或者 on_fail表示只有失败时才发送")
+    parser.addini("send_api", help="结果发往何处")
 
-    if result.when == 'call':
-        print(result.passed)
+
+def pytest_runtest_logreport(report: pytest.TestReport):
+    if report.when == "call":
+        data[report.outcome] += 1
+
+
+def pytest_collection_finish(session: pytest.Session):
+    # 用例加载完成之后执行，包含了全部的用例
+    data["total"] = len(session.items)
+
+
+def pytest_configure(config: pytest.Config):
+    # 配置加载完毕之后执行，所有测试用例执行前执行
+    data["start_time"] = datetime.now()
+    data["send_when"] = config.getini("send_when")
+    data["send_api"] = config.getini("send_api")
+
+
+def pytest_unconfigure():
+    # 配置卸载完毕之后执行，所有测试用例执行后执行
+    data["end_time"] = datetime.now()
+    data["duration"] = data["end_time"] - data["start_time"]
+    data["pass_ratio"] = data["passed"] / data["total"] * 100
+    data["pass_ratio"] = f"{data['pass_ratio']:.2f}"
+
+    # assert timedelta(seconds=3) > data['duration'] >= timedelta(seconds=2.5)
+    # assert data['total'] == 3
+    # assert data['passed'] == 2
+    # assert data['failed'] == 1
+    # assert data['pass_ratio'] == '66.67%'
+
+    send_result()
+
+
+def send_result():
+    if data["send_when"] == "on_fail" and data["failed"] == 0:
+        # 如果配置失败才发送，但实际没有失败， 则不发送
+        return
+
+    if not data["send_api"]:
+        # 如果没有配置API地址，则不发送
+        return
+
+    url = data["send_api"]  # 动态指定结果发送位置
+
+    content = f"""
+    pytest自动化测试结果
+
+
+    测试时间：{data['end_time']}
+    用例数量：{data['total']}
+    执行时长：{data['duration']}
+    测试通过：<font color='green'>{data['passed']} </font>
+    测试失败：<font color='red'>{data['failed']} </font>
+    测试通过率：{data['pass_ratio']}% <br/>
+
+    测试报告地址: http://baidu.com
+    """
+
+    try:
+        requests.post(
+            url, json={"msgtype": "markdown", "markdown": {"content": content}}
+        )
+    except Exception:
+        pass
+
+    data["send_done"] = 1  # 发送成功
```

