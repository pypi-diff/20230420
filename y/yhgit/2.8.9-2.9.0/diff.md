# Comparing `tmp/yhgit-2.8.9.tar.gz` & `tmp/yhgit-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yhgit-2.8.9.tar", last modified: Thu Mar 23 06:19:27 2023, max compression
+gzip compressed data, was "yhgit-2.9.0.tar", last modified: Thu Apr 20 11:31:08 2023, max compression
```

## Comparing `yhgit-2.8.9.tar` & `yhgit-2.9.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 fanguohuijack   (501) staff       (20)        0 2023-03-23 06:19:27.387082 yhgit-2.8.9/
--rw-r--r--   0 fanguohuijack   (501) staff       (20)     1062 2022-11-04 01:44:48.000000 yhgit-2.8.9/LICENSE.txt
--rw-r--r--   0 fanguohuijack   (501) staff       (20)      851 2023-03-23 06:19:27.387199 yhgit-2.8.9/PKG-INFO
--rw-r--r--   0 fanguohuijack   (501) staff       (20)     3709 2023-03-22 10:57:10.000000 yhgit-2.8.9/README.md
--rw-r--r--   0 fanguohuijack   (501) staff       (20)       79 2023-03-23 06:19:27.387581 yhgit-2.8.9/setup.cfg
--rw-r--r--   0 fanguohuijack   (501) staff       (20)     2086 2023-03-23 06:18:49.000000 yhgit-2.8.9/setup.py
-drwxr-xr-x   0 fanguohuijack   (501) staff       (20)        0 2023-03-23 06:19:27.383940 yhgit-2.8.9/yhgit/
--rw-r--r--   0 fanguohuijack   (501) staff       (20)       13 2023-01-11 03:34:32.000000 yhgit-2.8.9/yhgit/__init__.py
--rw-r--r--   0 fanguohuijack   (501) staff       (20)    60363 2023-03-23 06:05:47.000000 yhgit-2.8.9/yhgit/yhgit.py
-drwxr-xr-x   0 fanguohuijack   (501) staff       (20)        0 2023-03-23 06:19:27.386874 yhgit-2.8.9/yhgit.egg-info/
--rw-r--r--   0 fanguohuijack   (501) staff       (20)      851 2023-03-23 06:19:27.000000 yhgit-2.8.9/yhgit.egg-info/PKG-INFO
--rw-r--r--   0 fanguohuijack   (501) staff       (20)      249 2023-03-23 06:19:27.000000 yhgit-2.8.9/yhgit.egg-info/SOURCES.txt
--rw-r--r--   0 fanguohuijack   (501) staff       (20)        1 2023-03-23 06:19:27.000000 yhgit-2.8.9/yhgit.egg-info/dependency_links.txt
--rw-r--r--   0 fanguohuijack   (501) staff       (20)       44 2023-03-23 06:19:27.000000 yhgit-2.8.9/yhgit.egg-info/entry_points.txt
--rw-r--r--   0 fanguohuijack   (501) staff       (20)      116 2023-03-23 06:19:27.000000 yhgit-2.8.9/yhgit.egg-info/requires.txt
--rw-r--r--   0 fanguohuijack   (501) staff       (20)        6 2023-03-23 06:19:27.000000 yhgit-2.8.9/yhgit.egg-info/top_level.txt
+drwxr-xr-x   0 fanguohuijack   (501) staff       (20)        0 2023-04-20 11:31:08.264033 yhgit-2.9.0/
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)     1062 2022-11-04 01:44:48.000000 yhgit-2.9.0/LICENSE.txt
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)      851 2023-04-20 11:31:08.264222 yhgit-2.9.0/PKG-INFO
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)     3709 2023-03-22 10:57:10.000000 yhgit-2.9.0/README.md
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)       79 2023-04-20 11:31:08.264809 yhgit-2.9.0/setup.cfg
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)     2113 2023-04-20 11:30:58.000000 yhgit-2.9.0/setup.py
+drwxr-xr-x   0 fanguohuijack   (501) staff       (20)        0 2023-04-20 11:31:08.260862 yhgit-2.9.0/yhgit/
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)       13 2023-01-11 03:34:32.000000 yhgit-2.9.0/yhgit/__init__.py
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)    62547 2023-04-20 11:29:46.000000 yhgit-2.9.0/yhgit/yhgit.py
+drwxr-xr-x   0 fanguohuijack   (501) staff       (20)        0 2023-04-20 11:31:08.263524 yhgit-2.9.0/yhgit.egg-info/
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)      851 2023-04-20 11:31:08.000000 yhgit-2.9.0/yhgit.egg-info/PKG-INFO
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)      249 2023-04-20 11:31:08.000000 yhgit-2.9.0/yhgit.egg-info/SOURCES.txt
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)        1 2023-04-20 11:31:08.000000 yhgit-2.9.0/yhgit.egg-info/dependency_links.txt
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)       44 2023-04-20 11:31:08.000000 yhgit-2.9.0/yhgit.egg-info/entry_points.txt
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)      116 2023-04-20 11:31:08.000000 yhgit-2.9.0/yhgit.egg-info/requires.txt
+-rw-r--r--   0 fanguohuijack   (501) staff       (20)        6 2023-04-20 11:31:08.000000 yhgit-2.9.0/yhgit.egg-info/top_level.txt
```

### Comparing `yhgit-2.8.9/LICENSE.txt` & `yhgit-2.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yhgit-2.8.9/PKG-INFO` & `yhgit-2.9.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yhgit
-Version: 2.8.9
+Version: 2.9.0
 Summary: yh branch git manager util
 Home-page: http://gitlab.yonghui.cn/operation-xm-qdjg/yhgit.git
 Author: yonghuifan21
 Author-email: jackfan1@yonghui.com
 License: MIT
 Download-URL: https://files.pythonhosted.org/packages/08/7d/95aa3aa88c4c195889993de691b7fe816ac8d0767ea22fce56ccd240169a/yhmgit-0.3.tar.gz
 Keywords: yhgit,git,yh
```

### Comparing `yhgit-2.8.9/README.md` & `yhgit-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `yhgit-2.8.9/setup.py` & `yhgit-2.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,21 +10,23 @@
     packages=find_packages(),
     entry_points={
           'console_scripts': [
               'yhgit = yhgit.yhgit:main'
           ]
     },
     python_requires='>=3.7',
-    version='2.8.9',  # Start with a small number and increase it with every change you make
+    version='2.9.0',  # Start with a small number and increase it with every change you make
     license='MIT',  # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     description='yh branch git manager util',  # Give a short description about your library
     author='yonghuifan21',  # Type in your name
     author_email='jackfan1@yonghui.com',  # Type in your E-Mail
     url='http://gitlab.yonghui.cn/operation-xm-qdjg/yhgit.git',
-    download_url='https://files.pythonhosted.org/packages/08/7d/95aa3aa88c4c195889993de691b7fe816ac8d0767ea22fce56ccd240169a/yhmgit-0.3.tar.gz',  # I explain this later on
+    download_url='https://files.pythonhosted.org/packages/08/7d'
+                 '/95aa3aa88c4c195889993de691b7fe816ac8d0767ea22fce56ccd240169a/yhmgit-0.3.tar.gz',  # I explain this
+    # later on 
     keywords=['yhgit', 'git', 'yh'],  # Keywords that define your package best
     install_requires=[  # I get to this in a second
         'ruamel.yaml==0.17.21',
         'datetime==4.7',
         'GitPython==3.1.30',
         'runcmd==2020.12.3',
         'prettytable==3.6.0',
```

### Comparing `yhgit-2.8.9/yhgit/yhgit.py` & `yhgit-2.9.0/yhgit/yhgit.py`

 * *Files 2% similar despite different names*

```diff
@@ -439,15 +439,15 @@
         for mo_re in branch_result:
             if a.module and mo_re.module and a.module == mo_re.module and mo_re.result == 1:
                 module_dict = {"module": mo_re.module, "pod": a.pod, "git": a.git, "branch": n_branch,
                                "configurations": a.configurations,
                                "inhibit_warnings": a.inhibit_warnings}
                 dependenceList[index] = module_dict
         index += 1
-    print("convert=======" + str(dependenceList))
+    # print("convert=======" + str(dependenceList))
     except_list = [
         module for module in branch_result if ((module.result == 1) and (module.module not in [
             pod.module for pod in conver_deplist]))]
     if len(except_list) > 0:
         for mo_re in except_list:
             module_dict = {
                 "module": mo_re.module,
@@ -557,21 +557,21 @@
     git_pull_command = "git pull origin " + branch
 
     # git push
     git_push_command = "git push origin master"
     # 用newTag来修改podspec中version
     os.system(git_clone_command)
     # print("执行 " + git_clone_command)
+    # master分支下的版本号
 
     # 获取开发分支最后一次提交的信息
     repogit = RepoGit(proj_path=filepath)
     commit_message, commit = repogit.most_recent_commit_message(branch)
     repogit.switch_branch('master')
     git_commit_command = "git commit -m \'自动提交，修改tag\'"
-    # master分支下的版本号
     os.chdir(filepath)
     cur_tag = get_version_for(pod + ".podspec")
     os.system("pwd")
     os.system("ls")
     os.system(git_add_command)
     # print("执行 " + git_add_command)
     os.system(git_commit_command)
@@ -732,33 +732,51 @@
     :param msg: 提交信息
     :return: 返回操作的分支
     """
     commit_result = []
     invert_list = module_list
     if len(include_list) > 0:
         invert_list = [i for i in module_list if i.module in include_list]
+    for i, module in enumerate(invert_list):
+        path = module.path
+        if not (path is not None and os.path.exists(path)):
+            path = module_f_path + module.module + "/"
+        module.path = path
     bar = Bar('commit...', fill="*", max=len(invert_list))
     for module in invert_list:
         bar.next()
-        filename = module.module
-        module_path = module_f_path + filename + "/"
-        git = RepoGit(module_path)
-        branch = git.getCurrentBranch()
+        module_path = module.path
+        result = 1
+        branch = ''
         error_msg = ''
-        result = 0
-        if not git.is_dirty():
-            error_msg = "很干净，没有可提交的"
+        if not os.path.exists(module_path):
+            result = 0
+            error_msg = "本地开发路径为空"
         else:
-            # 判断是否有没有追踪的文件
-            untracks = git.untracked()
-            git.add(untracks)
-            git.commit(msg)
-            result = not git.is_dirty()
-            if result == 0:
-                error_msg = "提交失败"
+            git = None
+            try:
+                git = RepoGit(module_path)
+            except Exception as e:
+                result = 0
+                error_msg = str(e)
+            finally:
+                if result != 0:
+                    branch = git.getCurrentBranch()
+                    error_msg = ''
+                    result = 0
+                    if not git.is_dirty():
+                        error_msg = "很干净，没有可提交的"
+                    else:
+                        # 判断是否有没有追踪的文件
+                        untracks = git.untracked()
+                        git.add(untracks)
+                        git.commit(msg)
+                        result = not git.is_dirty()
+                        if result == 0:
+                            error_msg = "提交失败"
         modul_branch_model = ModuleStatusModel(module.module, module.pod, result, branch, error_msg)
         commit_result.append(modul_branch_model)
     bar.finish()
     return commit_result
 
 
 # 基于podfileModule，提交模块开发分支代码
@@ -768,34 +786,45 @@
     :param module_list: 模块列表
     :param module_f_path: 路径
     :return: 返回操作的分支
     """
     invert_list = module_list;
     if len(include_list) > 0:
         invert_list = [i for i in module_list if i.module in include_list]
+
+    for i, module in enumerate(invert_list):
+        path = module.path
+        if not (path is not None and os.path.exists(path)):
+            path = module_f_path + module.module + "/"
+        module.path = path
+
     pull_result = []
     bar = Bar('pull...', fill="*", max=len(invert_list))
     for module in invert_list:
         bar.next()
-        filename = module.module
-        module_path = module_f_path + filename + "/"
-        git = RepoGit(module_path)
-        branch = git.getCurrentBranch()
         msg = ''
         result = 1
-        if git.is_dirty():
-            result = -1
-            msg = "本地有变动未提交，请确认"
+        module_path = module.path
+        branch = ''
+        if not os.path.exists(module_path):
+            result = 0
+            msg = "本地开发路径为空"
         else:
-            # ori = git.repo.remotes.origin
-            try:
-                git.repo.git.pull('--progress', '--no-rebase', 'origin', branch)
-            except Exception as e:
-                result = 0
-                msg = str(e)
+            git = RepoGit(module_path)
+            branch = git.getCurrentBranch()
+            if git.is_dirty():
+                result = -1
+                msg = "本地有变动未提交，请确认"
+            else:
+                # ori = git.repo.remotes.origin
+                try:
+                    git.repo.git.pull('--progress', '--no-rebase', 'origin', branch)
+                except Exception as e:
+                    result = 0
+                    msg = str(e)
 
         modul_branch_model = ModuleStatusModel(module.module, module.pod, result, branch, msg)
         pull_result.append(modul_branch_model)
     bar.finish()
     return pull_result
 
 
@@ -809,33 +838,45 @@
     """
 
     index = 0
     pull_result = []
     invert_list = module_list;
     if len(include_list) > 0:
         invert_list = [i for i in module_list if i.module in include_list]
+
+    for i, module in enumerate(invert_list):
+        path = module.path
+        if not (path is not None and os.path.exists(path)):
+            path = module_f_path + module.module + "/"
+        module.path = path
+
     bar = Bar('push...', fill="*", max=len(invert_list))
     for module in invert_list:
         bar.next()
-        filename = module.module
-        module_path = module_f_path + filename + "/"
-        git = RepoGit(module_path)
-        branch = git.getCurrentBranch()
+        module_path = module.path
         msg = ''
         result = 1
-        if git.is_dirty():
-            result = -1
-            msg = "本地有变动未提交，请确认"
+        branch = ''
+        if not os.path.exists(module_path):
+            result = 0
+            msg = "本地开发路径为空"
         else:
-            try:
-                git.repo.git.pull('--progress', '--no-rebase', 'origin', branch)
-                git.repo.git.push('--progress', 'origin', branch)
-            except Exception as e:
-                result = 0
-                msg = str(e)
+            git = RepoGit(module_path)
+            branch = git.getCurrentBranch()
+
+            if git.is_dirty():
+                result = -1
+                msg = "本地有变动未提交，请确认"
+            else:
+                try:
+                    git.repo.git.pull('--progress', '--no-rebase', 'origin', branch)
+                    git.repo.git.push('--progress', 'origin', branch)
+                except Exception as e:
+                    result = 0
+                    msg = str(e)
 
         modul_branch_model = ModuleStatusModel(module.module, module.pod, result, branch, msg)
         pull_result.append(modul_branch_model)
     bar.finish()
     return pull_result
 
 
@@ -850,42 +891,53 @@
     :return: 返回操作的分支
     """
     index = 0
     pull_result = []
     invert_list = convert_list
     if len(module_list) > 0:
         invert_list = [i for i in convert_list if i.module in module_list]
+
+    for i, module in enumerate(invert_list):
+        path = module.path
+        if not (path is not None and os.path.exists(path)):
+            path = module_f_path + module.module + "/"
+        module.path = path
+
     bar = Bar('merge...', fill="*", max=len(invert_list))
     for module in invert_list:
         if module.module in module_list:
             bar.next()
-            filename = module.module
-            module_path = module_f_path + filename + "/"
-            git = RepoGit(module_path)
-            branch = git.getCurrentBranch()
+            module_path = module.path
             msg = ''
             result = 1
-            if git.is_dirty():
-                result = -1
-                msg = "本地有变动未提交，请确认"
+            branch = ''
+            if not os.path.exists(module_path):
+                result = 0
+                msg = "本地开发路径为空"
             else:
-                branchs = git.get_branches()
-                if from_branch not in branchs:
+                git = RepoGit(module_path)
+                branch = git.getCurrentBranch()
+                if git.is_dirty():
                     result = -1
-                    msg = "分支： {0} 不存在".format(from_branch)
+                    msg = "本地有变动未提交，请确认"
                 else:
-                    try:
-                        if 'origin/' not in from_branch:
-                            from_branch = "origin/" + from_branch
-                        git.repo.git.pull('--progress', '--no-rebase', 'origin', branch)
-                        git.repo.git.merge(from_branch)
-                        git.repo.git.push('--progress', 'origin', branch)
-                    except Exception as e:
-                        result = 0
-                        msg = str(e)
+                    branchs = git.get_branches()
+                    if from_branch not in branchs:
+                        result = -1
+                        msg = "分支： {0} 不存在".format(from_branch)
+                    else:
+                        try:
+                            if 'origin/' not in from_branch:
+                                from_branch = "origin/" + from_branch
+                            git.repo.git.pull('--progress', '--no-rebase', 'origin', branch)
+                            git.repo.git.merge(from_branch)
+                            git.repo.git.push('--progress', 'origin', branch)
+                        except Exception as e:
+                            result = 0
+                            msg = str(e)
             modul_branch_model = ModuleStatusModel(module.module, module.pod, result, branch, msg)
             pull_result.append(modul_branch_model)
         index += 1
     bar.finish()
     return pull_result
 
 
@@ -897,39 +949,53 @@
     :param convert_list: 模块列表
     :param module_f_path: 路径
     :param from_branch: 要合并的分支
     :return: 返回操作的分支
     """
     index = 0
     pull_result = []
-    bar = Bar('rebase...', fill="*", max=len(module_list))
-    for module in convert_list:
+    if len(module_list) > 0:
+        invert_list = [i for i in convert_list if i.module in module_list]
+
+    for i, module in enumerate(invert_list):
+        path = module.path
+        if not (path is not None and os.path.exists(path)):
+            path = module_f_path + module.module + "/"
+        module.path = path
+
+    bar = Bar('rebase...', fill="*", max=len(invert_list))
+    for module in invert_list:
         if module.module in module_list:
             bar.next()
-            filename = module.module
-            module_path = module_f_path + filename + "/"
-            git = RepoGit(module_path)
-            branch = git.getCurrentBranch()
+            module_path = module.path
             msg = ''
             result = 1
-            if git.is_dirty():
-                result = -1
-                msg = "本地有变动未提交，请确认"
+            if not os.path.exists(module_path):
+                result = 0
+                msg = "本地开发路径为空"
             else:
-                branchs = git.get_branches()
-                if from_branch not in branchs:
+                git = RepoGit(module_path)
+                branch = git.getCurrentBranch()
+                msg = ''
+                result = 1
+                if git.is_dirty():
                     result = -1
-                    msg = "分支： {0} 不存在".format(from_branch)
+                    msg = "本地有变动未提交，请确认"
                 else:
-                    try:
-                        git.repo.git.merge(from_branch)
-                        git.repo.git.push('--progress', 'origin', branch)
-                    except Exception as e:
-                        result = 0
-                        msg = str(e)
+                    branchs = git.get_branches()
+                    if from_branch not in branchs:
+                        result = -1
+                        msg = "分支： {0} 不存在".format(from_branch)
+                    else:
+                        try:
+                            git.repo.git.merge(from_branch)
+                            git.repo.git.push('--progress', 'origin', branch)
+                        except Exception as e:
+                            result = 0
+                            msg = str(e)
             modul_branch_model = ModuleStatusModel(module.module, module.pod, result, branch, msg)
             pull_result.append(modul_branch_model)
         index += 1
     bar.finish()
     return pull_result
 
 
@@ -944,15 +1010,15 @@
     :return: 返回操作成功的分支
     """
 
     index = 0
     merge_result = []
     invert_list = module_list
     if len(include_list) > 0:
-        invert_list = [i for i in invert_list if i.module in include_list]
+        invert_list = [i for i in invert_list if (i.module in include_list) and (i.branch and len(i.branch) > 0)]
 
     bar = Bar('release...', fill="*", max=len(invert_list))
     for a in invert_list:
         bar.next()
         if not (a.branch and len(a.branch) > 0) and not (a.tag and len(a.tag) > 0):
             a.branch = f_branch
         if a.branch and len(a.branch) > 0:
@@ -1000,44 +1066,36 @@
         file.write(yaml.dump(dict_value, sort_keys=False))
 
 
 # 创建分支的对象
 # branch 组件新分支名字
 class yhgit:
 
-    # # 初始化
-    # def __init__(self):
-    #     """
-    #     基于项目git地址拉取代码，并通过读取PodfileModule中的组件依赖，来新建开发分支n_branch，或者更新本地仓库
-    #     :param git: 工程git地址
-    #     :param branch: 基于哪个分支新建开发分支， 默认master
-    #     :param tag: 基于哪个tag来新建开发分支， 默认不指定
-    #     :param path: 项目的路径，默认~/Desktop/Project/ + 项目名
-    #     :param n_branch: 新分支名， 默认当前年月日
-    #     """
-    #     _project_path = path
-    #     if not (_project_path and len(_project_path) > 0):
-    #         (file, ext) = os.path.splitext(git)
-    #         (path, filename) = os.path.split(git)
-    #         project_name = filename.replace(ext, "")
-    #         _project_path = "~/Desktop/Project/" + project_name + "/"
-    #     self.path = _project_path
-    #
-    #     _n_branch = n_branch
-    #     if not (_n_branch and len(_n_branch) > 0):
-    #         today = datetime.date.today()
-    #         for_today = today.strftime("%y%m%d")
-    #         _n_branch = for_today
-    #     self.n_branch = _n_branch
-    #
-    #     self.git = git
-    #     self.branch = branch
-    #     self.tag = tag
+    # 拉取壳工程代码
+    def clone(self, git, o_branch, n_branch):
+        f_path = os.getcwd()
+        os.chdir(f_path)
+        result = new_branch(f_path, git, o_branch, '', n_branch)
+        res = 0
+        if result and len(result):
+            res = 1
+        error = '分支创建失败'
+        if result and len(result):
+            error = ''
+        resultModule = [ModuleStatusModel("壳工程拉取成功", "壳工程拉取成功", res, n_branch, error, git=git)]
+        succ_list = []
+        fail_list = []
+        for merg_Model in resultModule:
+            if merg_Model.result == 1:
+                succ_list.append(merg_Model)
+            else:
+                fail_list.append(merg_Model)
+        printTable(succ_list, "分支创建成功的模块")
+        printTable(fail_list, "分支创建失败的模块")
 
-    # def __init__(self):
     def init(self, n_branch, git):
         """
         如果本地没有PodfileModule，该命令会自动生成PodfileModule文件，然后可以使用后续指令进行状态检测，推拉代码，提交及打tag的操作，如果有就会只执行后续的新增分支及拉取代码的操作
         :return:
         """
         c_path = ""
         f_path = os.getcwd()
@@ -1062,30 +1120,38 @@
             # 更新模块的名字{file_name}为{podspec}名字
             debugInfo(module_path)
             files = [filename for filename in os.listdir(f_path + "/" + module_path) if filename.endswith(".podspec")]
             # debugInfo(files)
             if len(files) > 0:
                 newfile_name = files[0]
                 newfile_name, file_ext = os.path.splitext(newfile_name)
+
+            isSame = newfile_name == file_name
+
             # debugInfo("执行结果" + newfile_name)
             newfile_path = modules_path + newfile_name
             # 判断是否有newfile_name对应的文件夹
             find = False
             for name in os.listdir(f_path + "/" + modules_path):
                 # 检查文件夹名称是否以指定字符串开头
                 if name.startswith(newfile_name) and os.path.isdir(os.path.join(f_path + "/" + modules_path, name)):
                     find = True
             if not find and newfile_name and len(newfile_name) > 0:
                 os.rename(f_path + "/" + module_path, f_path + "/" + newfile_path)
             else:
                 # 删除旧的文件夹
                 if os.path.exists(f_path + "/" + module_path):
-                    del_dir(f_path + "/" + module_path)
-                res = 1
-                error = "存在同名文件夹，新建分支失败，请手动切换"
+                    if not isSame:
+                        del_dir(f_path + "/" + module_path)
+                        res = 1
+                        error = "存在同名文件夹，新建分支失败，请手动切换"
+                    else:
+                        res = 1
+                        error = "新建分支成功，请手动切换"
+
         # 判断是否有PodfileModule文件夹
         pre_path = f_path + "/"
         # debugInfo(pre_path)
         localyamlPath_ = pre_path + 'PodfileLocal.yaml'
         yamlPath_ = pre_path + 'PodfileModule.yaml'
         localyamlPath = c_path + 'PodfileLocal.yaml'
         yamlPath = c_path + 'PodfileModule.yaml'
@@ -1183,14 +1249,15 @@
         local_dependenceList = podfile_module_data["dependencies"]
         # 转换成模型数组
         module_list = load_yaml(local_dependenceList)
         status_result = []
         invert_list = module_list
         if len(include_modules) > 0:
             invert_list = [i for i in module_list if i.module in include_modules]
+
         bar = Bar('status...', fill="*", max=len(invert_list))
         for module in invert_list:
             bar.next()
             result = 0
             branchname = ''
             msg = ''
             if not (module.path and len(module.path) > 0):
```

### Comparing `yhgit-2.8.9/yhgit.egg-info/PKG-INFO` & `yhgit-2.9.0/yhgit.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yhgit
-Version: 2.8.9
+Version: 2.9.0
 Summary: yh branch git manager util
 Home-page: http://gitlab.yonghui.cn/operation-xm-qdjg/yhgit.git
 Author: yonghuifan21
 Author-email: jackfan1@yonghui.com
 License: MIT
 Download-URL: https://files.pythonhosted.org/packages/08/7d/95aa3aa88c4c195889993de691b7fe816ac8d0767ea22fce56ccd240169a/yhmgit-0.3.tar.gz
 Keywords: yhgit,git,yh
```

