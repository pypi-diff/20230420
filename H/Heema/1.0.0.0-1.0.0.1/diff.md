# Comparing `tmp/Heema-1.0.0.0.tar.gz` & `tmp/Heema-1.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Heema-1.0.0.0.tar", last modified: Fri Mar 24 17:05:14 2023, max compression
+gzip compressed data, was "dist\Heema-1.0.0.1.tar", last modified: Thu Apr 20 20:37:50 2023, max compression
```

## Comparing `Heema-1.0.0.0.tar` & `Heema-1.0.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-03-24 17:05:14.270949 Heema-1.0.0.0/
-drwxrwxrwx   0        0        0        0 2023-03-24 17:05:14.246949 Heema-1.0.0.0/Heema/
--rw-rw-rw-   0        0        0    40201 2023-03-24 16:47:54.000000 Heema-1.0.0.0/Heema/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-24 17:05:14.268951 Heema-1.0.0.0/Heema.egg-info/
--rw-rw-rw-   0        0        0     5400 2023-03-24 17:05:14.000000 Heema-1.0.0.0/Heema.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-03-24 17:05:14.000000 Heema-1.0.0.0/Heema.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-24 17:05:14.000000 Heema-1.0.0.0/Heema.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-03-24 17:05:14.000000 Heema-1.0.0.0/Heema.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-24 17:05:14.000000 Heema-1.0.0.0/Heema.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5400 2023-03-24 17:05:14.269949 Heema-1.0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3468 2023-02-26 07:49:56.000000 Heema-1.0.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-03-24 17:05:14.270949 Heema-1.0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1170 2023-03-24 17:05:09.000000 Heema-1.0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:37:50.309145 Heema-1.0.0.1/
+drwxrwxrwx   0        0        0        0 2023-04-20 20:37:50.288144 Heema-1.0.0.1/Heema/
+-rw-rw-rw-   0        0        0    41788 2023-04-20 20:32:54.000000 Heema-1.0.0.1/Heema/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 20:37:50.307145 Heema-1.0.0.1/Heema.egg-info/
+-rw-rw-rw-   0        0        0     5400 2023-04-20 20:37:50.000000 Heema-1.0.0.1/Heema.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-04-20 20:37:50.000000 Heema-1.0.0.1/Heema.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 20:37:50.000000 Heema-1.0.0.1/Heema.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-04-20 20:37:50.000000 Heema-1.0.0.1/Heema.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-20 20:37:50.000000 Heema-1.0.0.1/Heema.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5400 2023-04-20 20:37:50.308145 Heema-1.0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3468 2023-02-26 07:49:56.000000 Heema-1.0.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-20 20:37:50.309145 Heema-1.0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1170 2023-04-20 20:37:45.000000 Heema-1.0.0.1/setup.py
```

### Comparing `Heema-1.0.0.0/Heema/__init__.py` & `Heema-1.0.0.1/Heema/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 bg="#202020"
 root_bg="#202020"
 label_bd=0
 label_bg="#202020"
 label_fg="#018574"
 symbols=""
+
 #############################           Theme Names (themenames)
 
 """def page():
     root=Tk()
     
     root.overrideredirect(True)
     #title_bar(root,text="Page 1")
@@ -323,16 +324,18 @@
 reddish_purple='#30121244' #for reddish purple
 more_reddish_purple='#30121277' #for more redish purple
 purple='#99004444' #for purple
 reddish='#99000044' #for reddish
 full_reddish='#99000099' #for full reddish
 
 
-def label(frame_name,text,bg=label_bg):
-    a=Label(frame_name,bd=label_bd,text=text,bg=bg,fg="#ffffff")
+def label(frame_name,text,bg="",fg="white",font=("Segoe UI",20)):
+    if(bg==""):
+        bg=frame_name["bg"]
+    a=Label(frame_name,bd=label_bd,text=text,bg=bg,fg=fg,font=font)
     return a
 
 
 back_buttons=['','','','']
 back_buttons_all=""
 keyboard_buttons="⌨⌫"
 
@@ -362,25 +365,25 @@
     def leave(e):
         #print("left")
         l.config(text="",bg="#202020",fg="#ffffff")
     l.bind("<Leave>",leave)
     l.bind("<Enter>",enter)
     return l
 
-def label_button(frame_name,text,command=do_nothing):
-    l=Button(frame_name,font=('calibri',"11"),text=text,border=label_bd,bg=label_bg,fg=label_fg,bd=0,command=command)
+def label_button(frame_name,text,command=do_nothing,fg="#009999",fg_on_hover="#ffffff",font=("Segoe UI",20),bd=0,bd_on_hover=0):
+    l=Button(frame_name,font=('calibri',"11"),text=text,border=label_bd,bg=frame_name["bg"],fg=fg,bd=0,command=command)
     def enter(e):
         #print("hovered")
-        l.config(activebackground="#202020",bg="#202020",fg="#ffffff",)#018574
+        l.config(fg=fg_on_hover,activebackground=frame_name["bg"])#018574
         #7BD5F5
         #205565
         
     def leave(e):
         #print("left")
-        l.config(bg="#202020",fg="#009999")
+        l.config(fg=fg)
     l.bind("<Leave>",leave)
     l.bind("<Enter>",enter)
     return l
 def white_label_button(frame_name,text,command=do_nothing):
     l=Button(frame_name,font=('calibri',"11"),text=text,border=label_bd,bg=label_bg,fg="#999999",command=command)
     def enter(e):
         #print("hovered")
@@ -407,110 +410,124 @@
         #print("left")
         l.config(bg="#000000",fg="#CC4329")
     l.bind("<Leave>",leave)
     l.bind("<Enter>",enter)
     return l
 
 
-def button(frame_name, text,command):
-
-    a=Button(frame_name,text=text, command=command,border=0,activebackground="#444444",bg="#202020",fg="#999999", font=('calibri',"20"),bd=0)
+def frame(frame_name,bd=0,bg=""):
+    if(bg==""):
+        bg=frame_name["bg"]
+    return Frame(frame_name,bg=bg,bd=bd)
+
+
+def label_frame(frame_name,bd=0,bg=""):
+    if(bg==""):
+        bg=frame_name["bg"]
+    return LabelFrame(frame_name,bg=bg,bd=bd)
+
+
+def button(frame_name, text,command,bg="",fg="#999999",activebackground="#444444",bg_on_hover="#444444",fg_on_hover="#ffffff",activebackground_on_hover="#7e7e7e",font=("Segoe UI",20),bd=0,bd_on_hover=0):
+    if(bg==""):
+        bg=frame_name["bg"]
+    a=Button(frame_name,text=text, command=command,border=0,activebackground=activebackground,bg=bg,fg=fg, font=font,bd=0)
     def enter(e):
         #print("hovered")
-        a.config(bd=0,activebackground="#7e7e7e",bg="#444444",fg="#ffffff",)#018574
+        a.config(bd=bd_on_hover,activebackground=activebackground_on_hover,fg=fg_on_hover)#018574
         #7BD5F5
         #205565
         
     def leave(e):
         #print("left")
-        a.config(bd=0,activebackground="#444444",bg="#202020",fg="#999999")
+        a.config(bd=bd,activebackground=activebackground,bg=bg,fg=fg)
     a.bind("<Leave>",leave)
     a.bind("<Enter>",enter)
     return a
 
-def button1(frame_name, text,command):
-
-    a=Button(frame_name,text=text, command=command,border=0,activebackground="#444444",bg="#202020",fg="#999999", font=('calibri',"20"),bd=0)
+def button1(frame_name, text,command,bg="",fg="#999999",activebackground="#444444",bg_on_hover="#444444",fg_on_hover="#ffffff",activebackground_on_hover="#7e7e7e",font=("Segoe UI",20),bd=0,bd_on_hover=0):
+    if(bg==""):
+        bg=frame_name["bg"]
+    a=Button(frame_name,text=text, command=command,border=0,activebackground=activebackground,bg=bg,fg=fg, font=font,bd=bd)
     def enter(e):
         #print("hovered")
-        a.config(bd=0,activebackground="#7e7e7e",bg="#444444",fg="#ffffff",)#018574
+        a.config(bd=bd_on_hover,activebackground=activebackground_on_hover,bg=bg_on_hover,fg=fg_on_hover,)#018574
         #7BD5F5
         #205565
         
     def leave(e):
         #print("left")
-        a.config(bd=0,activebackground="#444444",bg="#202020",fg="#999999")
+        a.config(bd=bd,activebackground=activebackground,bg=bg,fg=fg)
     a.bind("<Leave>",leave)
     a.bind("<Enter>",enter)
     return a
 
-def button2(frame_name, text,command):
+def button2(frame_name, text,command,bg="#2f2f2f",fg="#ffffff",activebackground="#444444",bg_on_hover="#EBEBEB",fg_on_hover="#000000",activebackground_on_hover="#7e7e7e",font=("Segoe UI",20),bd=0,bd_on_hover=0):
 
-    a=Button(frame_name,text=text, command=command,border=0,activebackground="#444444",bg="#2f2f2f",fg="#ffffff", font=('calibri',"20"),bd=0)
+    a=Button(frame_name,text=text, command=command,border=0,activebackground=activebackground,bg=bg,fg=fg, font=font,bd=0)
     def enter(e):
         #print("hovered")
-        a.config(bd=0,activebackground="#7e7e7e",bg="#EBEBEB",fg="#000000",)#018574
+        a.config(bd=bd_on_hover,activebackground=activebackground_on_hover,bg=bg_on_hover,fg=fg_on_hover,)#018574
         #7BD5F5
         #205565
         
     def leave(e):
         #print("left")
-        a.config(bd=0,activebackground="#444444",bg="#2f2f2f",fg="#ffffff")
+        a.config(bd=bd,activebackground=activebackground,bg=bg,fg=fg)
     a.bind("<Leave>",leave)
     a.bind("<Enter>",enter)
     return a
 
 
 
 
-def button3(frame_name, text,command):
+def button3(frame_name, text,command,bg="",fg="",activebackground="",bg_on_hover="",fg_on_hover="",activebackground_on_hover="",font=("Segoe UI",20),bd=0,bd_on_hover=0):
 
-    a=Button(frame_name,text=text, command=command,border=0,activebackground="#444444",bg="#2f2f2f",fg="#ffffff", font=('calibri',"20"),bd=0)
+    a=Button(frame_name,text=text, command=command,border=0,activebackground="#444444",bg="#2f2f2f",fg="#ffffff", font=font,bd=0)
     def enter(e):
         #print("hovered")
         a.config(bd=0,activebackground="#CC4329",bg="#EBEBEB",fg="#000000",)#018574
         #7BD5F5
         #205565
         
     def leave(e):
         #print("left")
         a.config(bd=0,activebackground="#444444",bg="#2f2f2f",fg="#ffffff")
     a.bind("<Leave>",leave)
     a.bind("<Enter>",enter)
     return a
+#bg="",fg="",activebackground="",bg_on_hover="",fg_on_hover="",activebackground_on_hover="",font=("Segoe UI",20),bd=0,bd_on_hover=0
 
+def button4(frame_name, text,command,bg="#2f2f2f",fg="#ffffff",activebackground="#444444",bg_on_hover="#3f3f3f",fg_on_hover="#ffffff",activebackground_on_hover="#7e7e7e",font=("Segoe UI",20),bd=0,bd_on_hover=0):
 
-def button4(frame_name, text,command):
-
-    a=Button(frame_name,text=text, command=command,border=0,activebackground="#444444",bg="#2f2f2f",fg="#ffffff", font=('calibri',"20"),bd=0)
+    a=Button(frame_name,text=text, command=command,border=0,activebackground=activebackground,bg=bg,fg=fg, font=font,bd=bd)
     def enter(e):
         #print("hovered")
-        a.config(bd=0,activebackground="#7e7e7e",bg="#3f3f3f",fg="#ffffff",)#018574
+        a.config(bd=bd_on_hover,activebackground=activebackground_on_hover,bg=bg_on_hover,fg=fg_on_hover,)#018574
         #7BD5F5
         #205565
         
     def leave(e):
         #print("left")
-        a.config(bd=0,activebackground="#444444",bg="#2f2f2f",fg="#ffffff")
+        a.config(bd=bd,activebackground=activebackground,bg=bg,fg=fg)
     a.bind("<Leave>",leave)
     a.bind("<Enter>",enter)
     return a
 
-def button5(frame_name, text,command):
+def button5(frame_name, text,command,bg="#2f2f2f",fg="#ffffff",activebackground="#444444",bg_on_hover="#CC4329",fg_on_hover="#ffffff",activebackground_on_hover="#EBEBEB",font=("Segoe UI",20),bd=0,bd_on_hover=0):
 
-    a=Button(frame_name,text=text, command=command,border=0,activebackground="#444444",bg="#2f2f2f",fg="#ffffff", font=('calibri',"20"),bd=0)
+    a=Button(frame_name,text=text, command=command,border=0,activebackground=activebackground,bg=bg,fg=fg, font=font,bd=0)
     def enter(e):
         #print("hovered")
-        a.config(bd=0,activebackground="#EBEBEB",bg="#CC4329",fg="#ffffff",)#018574
+        a.config(bd=bd_on_hover,activebackground=activebackground_on_hover,bg=bg_on_hover,fg=fg_on_hover,)#018574
         #7BD5F5
         #2055651
         
     def leave(e):
         #print("left")
-        a.config(bd=0,activebackground="#444444",bg="#2f2f2f",fg="#ffffff")
+        a.config(bd=bd,activebackground=activebackground,bg=bg,fg=fg)
     a.bind("<Leave>",leave)
     a.bind("<Enter>",enter)
     return a
 
 button_activebackground="#444444" 
 button_bg="#202020" 
 button_fg="#999999" 
@@ -948,15 +965,14 @@
     resizey_widget.bind("<B1-Motion>",resizey)
 
     # some settings
     root.bind("<FocusIn>",deminimize) # to view the window by clicking on the window icon on the taskbar
     root.bind("<FocusOut>",deminimize)
     root.after(1, lambda: set_appwindow(root)) # to see the icon on the task bar
 
-
     #YOUR CODE GOES between the lines :)
     # ===================================================================================================
 
 
 
 
 
@@ -1203,16 +1219,16 @@
 
     label1 = Label(frame_name,image=test,bg=label_bg,bd=label_bd)
     label1.image = test
 
     return label1
 def create_image(frame_name,path,size,bg=label_bg):
     image1 = Image.open(path)
-    
-    resize_image = image1.resize((size,size))
+    x,y=size
+    resize_image = image1.resize((x,y))
     test = ImageTk.PhotoImage(resize_image,master = frame_name)
     label1 = Label(frame_name,image=test,bd=0,bg=label_bg)
 
     label1.image = test
 
     return label1
 
@@ -1250,14 +1266,8 @@
 
 
 
 
 
 def navigate_to(main_frame ,welcome_page):
     main_frame.forget()
-    welcome_page.pack(fill=BOTH,expand=True)
-
-
-
-
-
-
+    welcome_page.pack(fill=BOTH,expand=True)
```

### Comparing `Heema-1.0.0.0/Heema.egg-info/PKG-INFO` & `Heema-1.0.0.1/Heema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Heema
-Version: 1.0.0.0
+Version: 1.0.0.1
 Summary: A GUI framework built on top of tkinter, with new features.
 Home-page: UNKNOWN
 Author: Федор Глеб | Abhay Gaur
 Author-email: <abhay.12104531@gmail.com>
 License: UNKNOWN
 Description: 
         # Heema
```

### Comparing `Heema-1.0.0.0/PKG-INFO` & `Heema-1.0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Heema
-Version: 1.0.0.0
+Version: 1.0.0.1
 Summary: A GUI framework built on top of tkinter, with new features.
 Home-page: UNKNOWN
 Author: Федор Глеб | Abhay Gaur
 Author-email: <abhay.12104531@gmail.com>
 License: UNKNOWN
 Description: 
         # Heema
```

### Comparing `Heema-1.0.0.0/README.md` & `Heema-1.0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `Heema-1.0.0.0/setup.py` & `Heema-1.0.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.0.0'
+VERSION = "1.0.0.1"
 DESCRIPTION = 'A GUI framework built on top of tkinter, with new features.'
 LONG_DESCRIPTION = ''
 
 # Setting up
 setup(
     name="Heema",
     version=VERSION,
```

