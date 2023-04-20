# Comparing `tmp/amlopschat-1.0.7.tar.gz` & `tmp/amlopschat-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amlopschat-1.0.7.tar", last modified: Thu Apr 20 16:49:13 2023, max compression
+gzip compressed data, was "amlopschat-1.0.8.tar", last modified: Thu Apr 20 17:14:50 2023, max compression
```

## Comparing `amlopschat-1.0.7.tar` & `amlopschat-1.0.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:49:13.057206 amlopschat-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-20 16:48:34.000000 amlopschat-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 16:49:13.057206 amlopschat-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-20 16:48:34.000000 amlopschat-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:49:13.049206 amlopschat-1.0.7/amlopschat/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 16:49:02.000000 amlopschat-1.0.7/amlopschat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23620 2023-04-20 16:49:02.000000 amlopschat-1.0.7/amlopschat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:49:13.045206 amlopschat-1.0.7/amlopschat/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:49:13.057206 amlopschat-1.0.7/amlopschat/static/chat/
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-04-20 16:49:01.000000 amlopschat-1.0.7/amlopschat/static/chat/RoomHeader.vue
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-04-20 16:49:01.000000 amlopschat-1.0.7/amlopschat/static/chat/RoomMessageWrapper.vue
--rw-r--r--   0 runner    (1001) docker     (123)    23620 2023-04-20 16:49:01.000000 amlopschat-1.0.7/amlopschat/static/chat/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-20 16:49:01.000000 amlopschat-1.0.7/amlopschat/static/chat/arrow.svg
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-20 16:49:01.000000 amlopschat-1.0.7/amlopschat/static/chat/create-room.svg
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-20 16:49:01.000000 amlopschat-1.0.7/amlopschat/static/chat/emoji.svg
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-20 16:49:01.000000 amlopschat-1.0.7/amlopschat/static/chat/file.svg
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-20 16:49:01.000000 amlopschat-1.0.7/amlopschat/static/chat/header-chat-menu.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45378 2023-04-20 16:49:01.000000 amlopschat-1.0.7/amlopschat/static/chat/index.css
--rw-r--r--   0 runner    (1001) docker     (123)   425281 2023-04-20 16:49:01.000000 amlopschat-1.0.7/amlopschat/static/chat/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-20 16:49:01.000000 amlopschat-1.0.7/amlopschat/static/chat/link.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-20 16:49:01.000000 amlopschat-1.0.7/amlopschat/static/chat/microphone.svg
--rw-r--r--   0 runner    (1001) docker     (123)   450457 2023-04-20 16:49:01.000000 amlopschat-1.0.7/amlopschat/static/chat/no-messages.gif
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-20 16:49:01.000000 amlopschat-1.0.7/amlopschat/static/chat/read-message.svg
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-20 16:49:01.000000 amlopschat-1.0.7/amlopschat/static/chat/search.svg
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-20 16:49:01.000000 amlopschat-1.0.7/amlopschat/static/chat/send.svg
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-20 16:49:01.000000 amlopschat-1.0.7/amlopschat/static/chat/toggle.svg
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-20 16:49:01.000000 amlopschat-1.0.7/amlopschat/static/chat/unread-message.svg
--rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-04-20 16:49:01.000000 amlopschat-1.0.7/amlopschat/static/chat/user.png
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-20 16:49:01.000000 amlopschat-1.0.7/amlopschat/static/chat/vue.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:49:13.049206 amlopschat-1.0.7/amlopschat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 16:49:13.000000 amlopschat-1.0.7/amlopschat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-20 16:49:13.000000 amlopschat-1.0.7/amlopschat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 16:49:13.000000 amlopschat-1.0.7/amlopschat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 16:49:13.000000 amlopschat-1.0.7/amlopschat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-20 16:49:13.057206 amlopschat-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-20 16:48:34.000000 amlopschat-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:49:13.057206 amlopschat-1.0.7/src/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-20 16:49:13.057206 amlopschat-1.0.7/src/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-20 16:48:34.000000 amlopschat-1.0.7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:14:50.871281 amlopschat-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-20 17:14:10.000000 amlopschat-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 17:14:50.871281 amlopschat-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-20 17:14:10.000000 amlopschat-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:14:50.867281 amlopschat-1.0.8/amlopschat/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-20 17:14:39.000000 amlopschat-1.0.8/amlopschat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23620 2023-04-20 17:14:39.000000 amlopschat-1.0.8/amlopschat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:14:50.867281 amlopschat-1.0.8/amlopschat/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:14:50.871281 amlopschat-1.0.8/amlopschat/static/chat/
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-04-20 17:14:39.000000 amlopschat-1.0.8/amlopschat/static/chat/RoomHeader.vue
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-04-20 17:14:39.000000 amlopschat-1.0.8/amlopschat/static/chat/RoomMessageWrapper.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    23620 2023-04-20 17:14:39.000000 amlopschat-1.0.8/amlopschat/static/chat/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-20 17:14:39.000000 amlopschat-1.0.8/amlopschat/static/chat/arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-20 17:14:39.000000 amlopschat-1.0.8/amlopschat/static/chat/create-room.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-20 17:14:39.000000 amlopschat-1.0.8/amlopschat/static/chat/emoji.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-20 17:14:39.000000 amlopschat-1.0.8/amlopschat/static/chat/file.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-20 17:14:39.000000 amlopschat-1.0.8/amlopschat/static/chat/header-chat-menu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45378 2023-04-20 17:14:39.000000 amlopschat-1.0.8/amlopschat/static/chat/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)   425341 2023-04-20 17:14:39.000000 amlopschat-1.0.8/amlopschat/static/chat/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-20 17:14:39.000000 amlopschat-1.0.8/amlopschat/static/chat/link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-20 17:14:39.000000 amlopschat-1.0.8/amlopschat/static/chat/microphone.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   450457 2023-04-20 17:14:39.000000 amlopschat-1.0.8/amlopschat/static/chat/no-messages.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-20 17:14:39.000000 amlopschat-1.0.8/amlopschat/static/chat/read-message.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-20 17:14:39.000000 amlopschat-1.0.8/amlopschat/static/chat/search.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-20 17:14:39.000000 amlopschat-1.0.8/amlopschat/static/chat/send.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-20 17:14:39.000000 amlopschat-1.0.8/amlopschat/static/chat/toggle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-20 17:14:39.000000 amlopschat-1.0.8/amlopschat/static/chat/unread-message.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    19398 2023-04-20 17:14:39.000000 amlopschat-1.0.8/amlopschat/static/chat/user.png
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-20 17:14:39.000000 amlopschat-1.0.8/amlopschat/static/chat/vue.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:14:50.867281 amlopschat-1.0.8/amlopschat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-20 17:14:50.000000 amlopschat-1.0.8/amlopschat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-04-20 17:14:50.000000 amlopschat-1.0.8/amlopschat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 17:14:50.000000 amlopschat-1.0.8/amlopschat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-20 17:14:50.000000 amlopschat-1.0.8/amlopschat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-20 17:14:50.871281 amlopschat-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-20 17:14:10.000000 amlopschat-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:14:50.871281 amlopschat-1.0.8/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-20 17:14:50.871281 amlopschat-1.0.8/src/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-20 17:14:10.000000 amlopschat-1.0.8/versioneer.py
```

### Comparing `amlopschat-1.0.7/README.md` & `amlopschat-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.7/amlopschat/_version.py` & `amlopschat-1.0.8/amlopschat/_version.py`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.7/amlopschat/static/chat/RoomHeader.vue` & `amlopschat-1.0.8/amlopschat/static/chat/RoomHeader.vue`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.7/amlopschat/static/chat/RoomMessageWrapper.vue` & `amlopschat-1.0.8/amlopschat/static/chat/RoomMessageWrapper.vue`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.7/amlopschat/static/chat/_version.py` & `amlopschat-1.0.8/amlopschat/static/chat/_version.py`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.7/amlopschat/static/chat/emoji.svg` & `amlopschat-1.0.8/amlopschat/static/chat/emoji.svg`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.7/amlopschat/static/chat/index.css` & `amlopschat-1.0.8/amlopschat/static/chat/index.css`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.7/amlopschat/static/chat/index.js` & `amlopschat-1.0.8/amlopschat/static/chat/index.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -84,21 +84,21 @@
     if (!e) return null;
     let {
         class: t,
         style: n
     } = e;
     return t && !Ze(t) && (e.class = L(t)), n && (e.style = Ot(n)), e
 }
-const Pc = "itemscope,allowfullscreen,formnovalidate,ismap,nomodule,novalidate,readonly",
-    Fc = Ei(Pc);
+const Fc = "itemscope,allowfullscreen,formnovalidate,ismap,nomodule,novalidate,readonly",
+    Pc = Ei(Fc);
 
 function ba(e) {
     return !!e || e === ""
 }
-const Te = e => Ze(e) ? e : e == null ? "" : te(e) || ve(e) && (e.toString === va || !ne(e.toString)) ? JSON.stringify(e, Ca, 2) : String(e),
+const Ge = e => Ze(e) ? e : e == null ? "" : te(e) || ve(e) && (e.toString === va || !ne(e.toString)) ? JSON.stringify(e, Ca, 2) : String(e),
     Ca = (e, t) => t && t.__v_isRef ? Ca(e, t.value) : Zn(t) ? {
         [`Map(${t.size})`]: [...t.entries()].reduce((n, [o, s]) => (n[`${o} =>`] = s, n), {})
     } : ya(t) ? {
         [`Set(${t.size})`]: [...t.values()]
     } : ve(t) && !te(t) && !wa(t) ? String(t) : t,
     Ae = {},
     Mn = [],
@@ -214,38 +214,38 @@
 function fu(e) {
     $e && $e.cleanups.push(e)
 }
 const Ji = e => {
         const t = new Set(e);
         return t.w = 0, t.n = 0, t
     },
-    Za = e => (e.w & Pt) > 0,
-    Wa = e => (e.n & Pt) > 0,
+    Za = e => (e.w & Ft) > 0,
+    Wa = e => (e.n & Ft) > 0,
     ru = ({
         deps: e
     }) => {
         if (e.length)
-            for (let t = 0; t < e.length; t++) e[t].w |= Pt
+            for (let t = 0; t < e.length; t++) e[t].w |= Ft
     },
     au = e => {
         const {
             deps: t
         } = e;
         if (t.length) {
             let n = 0;
             for (let o = 0; o < t.length; o++) {
                 const s = t[o];
-                Za(s) && !Wa(s) ? s.delete(e) : t[n++] = s, s.w &= ~Pt, s.n &= ~Pt
+                Za(s) && !Wa(s) ? s.delete(e) : t[n++] = s, s.w &= ~Ft, s.n &= ~Ft
             }
             t.length = n
         }
     },
     es = new WeakMap;
 let Qn = 0,
-    Pt = 1;
+    Ft = 1;
 const ai = 30;
 let at;
 const gn = Symbol(""),
     li = Symbol("");
 class Ki {
     constructor(t, n = null, o) {
         this.fn = t, this.scheduler = n, this.active = !0, this.deps = [], this.parent = void 0, iu(this, o)
@@ -255,17 +255,17 @@
         let t = at,
             n = Lt;
         for (; t;) {
             if (t === this) return;
             t = t.parent
         }
         try {
-            return this.parent = at, at = this, Lt = !0, Pt = 1 << ++Qn, Qn <= ai ? ru(this) : Yf(this), this.fn()
+            return this.parent = at, at = this, Lt = !0, Ft = 1 << ++Qn, Qn <= ai ? ru(this) : Yf(this), this.fn()
         } finally {
-            Qn <= ai && au(this), Pt = 1 << --Qn, at = this.parent, Lt = n, this.parent = void 0, this.deferStop && this.stop()
+            Qn <= ai && au(this), Ft = 1 << --Qn, at = this.parent, Lt = n, this.parent = void 0, this.deferStop && this.stop()
         }
     }
     stop() {
         at === this ? this.deferStop = !0 : this.active && (Yf(this), this.onStop && this.onStop(), this.active = !1)
     }
 }
 
@@ -286,26 +286,26 @@
 }
 
 function En() {
     const e = Sa.pop();
     Lt = e === void 0 ? !0 : e
 }
 
-function Pe(e, t, n) {
+function Fe(e, t, n) {
     if (Lt && at) {
         let o = es.get(e);
         o || es.set(e, o = new Map);
         let s = o.get(n);
         s || o.set(n, s = Ji()), Ba(s)
     }
 }
 
 function Ba(e, t) {
     let n = !1;
-    Qn <= ai ? Wa(e) || (e.n |= Pt, n = !Za(e)) : n = !e.has(at), n && (e.add(at), at.deps.push(e))
+    Qn <= ai ? Wa(e) || (e.n |= Ft, n = !Za(e)) : n = !e.has(at), n && (e.add(at), at.deps.push(e))
 }
 
 function St(e, t, n, o, s, i) {
     const f = es.get(e);
     if (!f) return;
     let r = [];
     if (t === "clear") r = [...f.values()];
@@ -345,55 +345,55 @@
 
 function lu(e, t) {
     var n;
     return (n = es.get(e)) === null || n === void 0 ? void 0 : n.get(t)
 }
 const cu = Ei("__proto__,__v_isRef,__isVue"),
     za = new Set(Object.getOwnPropertyNames(Symbol).filter(e => e !== "arguments" && e !== "caller").map(e => Symbol[e]).filter(Li)),
-    uu = Pi(),
-    du = Pi(!1, !0),
-    gu = Pi(!0),
+    uu = Fi(),
+    du = Fi(!1, !0),
+    gu = Fi(!0),
     Hf = pu();
 
 function pu() {
     const e = {};
     return ["includes", "indexOf", "lastIndexOf"].forEach(t => {
         e[t] = function(...n) {
             const o = ce(this);
-            for (let i = 0, f = this.length; i < f; i++) Pe(o, "get", i + "");
+            for (let i = 0, f = this.length; i < f; i++) Fe(o, "get", i + "");
             const s = o[t](...n);
             return s === -1 || s === !1 ? o[t](...n.map(ce)) : s
         }
     }), ["push", "pop", "shift", "unshift", "splice"].forEach(t => {
         e[t] = function(...n) {
             Yn();
             const o = ce(this)[t].apply(this, n);
             return En(), o
         }
     }), e
 }
 
 function mu(e) {
     const t = ce(this);
-    return Pe(t, "has", e), t.hasOwnProperty(e)
+    return Fe(t, "has", e), t.hasOwnProperty(e)
 }
 
-function Pi(e = !1, t = !1) {
+function Fi(e = !1, t = !1) {
     return function(o, s, i) {
         if (s === "__v_isReactive") return !e;
         if (s === "__v_isReadonly") return e;
         if (s === "__v_isShallow") return t;
-        if (s === "__v_raw" && i === (e ? t ? zu : ka : t ? ja : Ga).get(o)) return o;
+        if (s === "__v_raw" && i === (e ? t ? zu : ka : t ? ja : Ta).get(o)) return o;
         const f = te(o);
         if (!e) {
             if (f && ge(Hf, s)) return Reflect.get(Hf, s, i);
             if (s === "hasOwnProperty") return mu
         }
         const r = Reflect.get(o, s, i);
-        return (Li(s) ? za.has(s) : cu(s)) || (e || Pe(o, "get", s), t) ? r : Be(r) ? f && Ui(s) ? r : r.value : ve(r) ? e ? Qi(r) : yo(r) : r
+        return (Li(s) ? za.has(s) : cu(s)) || (e || Fe(o, "get", s), t) ? r : Be(r) ? f && Ui(s) ? r : r.value : ve(r) ? e ? Qi(r) : yo(r) : r
     }
 }
 const Iu = Va(),
     hu = Va(!0);
 
 function Va(e = !1) {
     return function(n, o, s, i) {
@@ -411,21 +411,21 @@
     e[t];
     const o = Reflect.deleteProperty(e, t);
     return o && n && St(e, "delete", t, void 0), o
 }
 
 function Cu(e, t) {
     const n = Reflect.has(e, t);
-    return (!Li(t) || !za.has(t)) && Pe(e, "has", t), n
+    return (!Li(t) || !za.has(t)) && Fe(e, "has", t), n
 }
 
 function yu(e) {
-    return Pe(e, "iterate", te(e) ? "length" : gn), Reflect.ownKeys(e)
+    return Fe(e, "iterate", te(e) ? "length" : gn), Reflect.ownKeys(e)
 }
-const Ta = {
+const Ga = {
         get: uu,
         set: Iu,
         deleteProperty: bu,
         has: Cu,
         ownKeys: yu
     },
     Au = {
@@ -433,43 +433,43 @@
         set(e, t) {
             return !0
         },
         deleteProperty(e, t) {
             return !0
         }
     },
-    vu = Re({}, Ta, {
+    vu = Re({}, Ga, {
         get: du,
         set: hu
     }),
-    Fi = e => e,
+    Pi = e => e,
     Is = e => Reflect.getPrototypeOf(e);
 
 function zo(e, t, n = !1, o = !1) {
     e = e.__v_raw;
     const s = ce(e),
         i = ce(t);
-    n || (t !== i && Pe(s, "get", t), Pe(s, "get", i));
+    n || (t !== i && Fe(s, "get", t), Fe(s, "get", i));
     const {
         has: f
-    } = Is(s), r = o ? Fi : n ? ef : lo;
+    } = Is(s), r = o ? Pi : n ? ef : lo;
     if (f.call(s, t)) return r(e.get(t));
     if (f.call(s, i)) return r(e.get(i));
     e !== s && e.get(t)
 }
 
 function Vo(e, t = !1) {
     const n = this.__v_raw,
         o = ce(n),
         s = ce(e);
-    return t || (e !== s && Pe(o, "has", e), Pe(o, "has", s)), e === s ? n.has(e) : n.has(e) || n.has(s)
+    return t || (e !== s && Fe(o, "has", e), Fe(o, "has", s)), e === s ? n.has(e) : n.has(e) || n.has(s)
 }
 
-function To(e, t = !1) {
-    return e = e.__v_raw, !t && Pe(ce(e), "iterate", gn), Reflect.get(e, "size", e)
+function Go(e, t = !1) {
+    return e = e.__v_raw, !t && Fe(ce(e), "iterate", gn), Reflect.get(e, "size", e)
 }
 
 function Of(e) {
     e = ce(e);
     const t = ce(this);
     return Is(t).has.call(t, e) || (t.add(e), St(t, "add", e, e)), this
 }
@@ -502,34 +502,34 @@
 function Jf() {
     const e = ce(this),
         t = e.size !== 0,
         n = e.clear();
     return t && St(e, "clear", void 0, void 0), n
 }
 
-function Go(e, t) {
+function To(e, t) {
     return function(o, s) {
         const i = this,
             f = i.__v_raw,
             r = ce(f),
-            a = t ? Fi : e ? ef : lo;
-        return !e && Pe(r, "iterate", gn), f.forEach((l, c) => o.call(s, a(l), a(c), i))
+            a = t ? Pi : e ? ef : lo;
+        return !e && Fe(r, "iterate", gn), f.forEach((l, c) => o.call(s, a(l), a(c), i))
     }
 }
 
 function jo(e, t, n) {
     return function(...o) {
         const s = this.__v_raw,
             i = ce(s),
             f = Zn(i),
             r = e === "entries" || e === Symbol.iterator && f,
             a = e === "keys" && f,
             l = s[e](...o),
-            c = n ? Fi : t ? ef : lo;
-        return !t && Pe(i, "iterate", a ? li : gn), {
+            c = n ? Pi : t ? ef : lo;
+        return !t && Fe(i, "iterate", a ? li : gn), {
             next() {
                 const {
                     value: u,
                     done: d
                 } = l.next();
                 return d ? {
                     value: u,
@@ -554,68 +554,68 @@
 
 function wu() {
     const e = {
             get(i) {
                 return zo(this, i)
             },
             get size() {
-                return To(this)
+                return Go(this)
             },
             has: Vo,
             add: Of,
             set: Lf,
             delete: Uf,
             clear: Jf,
-            forEach: Go(!1, !1)
+            forEach: To(!1, !1)
         },
         t = {
             get(i) {
                 return zo(this, i, !1, !0)
             },
             get size() {
-                return To(this)
+                return Go(this)
             },
             has: Vo,
             add: Of,
             set: Lf,
             delete: Uf,
             clear: Jf,
-            forEach: Go(!1, !0)
+            forEach: To(!1, !0)
         },
         n = {
             get(i) {
                 return zo(this, i, !0)
             },
             get size() {
-                return To(this, !0)
+                return Go(this, !0)
             },
             has(i) {
                 return Vo.call(this, i, !0)
             },
             add: kt("add"),
             set: kt("set"),
             delete: kt("delete"),
             clear: kt("clear"),
-            forEach: Go(!0, !1)
+            forEach: To(!0, !1)
         },
         o = {
             get(i) {
                 return zo(this, i, !0, !0)
             },
             get size() {
-                return To(this, !0)
+                return Go(this, !0)
             },
             has(i) {
                 return Vo.call(this, i, !0)
             },
             add: kt("add"),
             set: kt("set"),
             delete: kt("delete"),
             clear: kt("clear"),
-            forEach: Go(!0, !0)
+            forEach: To(!0, !0)
         };
     return ["keys", "values", "entries", Symbol.iterator].forEach(i => {
         e[i] = jo(i, !1, !1), n[i] = jo(i, !0, !1), t[i] = jo(i, !1, !0), o[i] = jo(i, !0, !0)
     }), [e, n, t, o]
 }
 const [_u, Nu, Mu, Zu] = wu();
 
@@ -628,15 +628,15 @@
     },
     Su = {
         get: $i(!1, !0)
     },
     Bu = {
         get: $i(!0, !1)
     },
-    Ga = new WeakMap,
+    Ta = new WeakMap,
     ja = new WeakMap,
     ka = new WeakMap,
     zu = new WeakMap;
 
 function Vu(e) {
     switch (e) {
         case "Object":
@@ -648,35 +648,35 @@
         case "WeakSet":
             return 2;
         default:
             return 0
     }
 }
 
-function Tu(e) {
+function Gu(e) {
     return e.__v_skip || !Object.isExtensible(e) ? 0 : Vu(eu(e))
 }
 
 function yo(e) {
-    return Bn(e) ? e : qi(e, !1, Ta, Wu, Ga)
+    return Bn(e) ? e : qi(e, !1, Ga, Wu, Ta)
 }
 
 function Da(e) {
     return qi(e, !1, vu, Su, ja)
 }
 
 function Qi(e) {
     return qi(e, !0, Au, Bu, ka)
 }
 
 function qi(e, t, n, o, s) {
     if (!ve(e) || e.__v_raw && !(t && e.__v_isReactive)) return e;
     const i = s.get(e);
     if (i) return i;
-    const f = Tu(e);
+    const f = Gu(e);
     if (f === 0) return e;
     const r = new Proxy(e, f === 2 ? o : n);
     return s.set(e, r), r
 }
 
 function Ut(e) {
     return Bn(e) ? Ut(e.__v_raw) : !!(e && e.__v_isReactive)
@@ -716,18 +716,18 @@
 }
 
 function Be(e) {
     return !!(e && e.__v_isRef === !0)
 }
 
 function oe(e) {
-    return Gu(e, !1)
+    return Tu(e, !1)
 }
 
-function Gu(e, t) {
+function Tu(e, t) {
     return Be(e) ? e : new ju(e, t)
 }
 class ju {
     constructor(t, n) {
         this.__v_isShallow = n, this.dep = void 0, this.__v_isRef = !0, this._rawValue = n ? t : ce(t), this._value = n ? t : lo(t)
     }
     get value() {
@@ -985,18 +985,18 @@
     return De = e, Cs = e && e.type.__scopeId || null, t
 }
 
 function Ka(e) {
     Cs = e
 }
 
-function Pa() {
+function Fa() {
     Cs = null
 }
-const Fa = e => Ne;
+const Pa = e => Ne;
 
 function Ne(e, t = De, n) {
     if (!t || e._n) return e;
     const o = (...s) => {
         o._d && ir(-1);
         const i = ns(t);
         let f;
@@ -1025,15 +1025,15 @@
         renderCache: u,
         data: d,
         setupState: m,
         ctx: p,
         inheritAttrs: h
     } = e;
     let b, y;
-    const G = ns(e);
+    const T = ns(e);
     try {
         if (n.shapeFlag & 4) {
             const v = s || o;
             b = It(c.call(v, v, u, i, m, d, p)), y = a
         } else {
             const v = t;
             b = It(v.length > 1 ? v(i, {
@@ -1047,55 +1047,55 @@
     }
     let N = b;
     if (y && h !== !1) {
         const v = Object.keys(y),
             {
                 shapeFlag: E
             } = N;
-        v.length && E & 7 && (f && v.some(Hi) && (y = Pu(y, f)), N = Ft(N, y))
+        v.length && E & 7 && (f && v.some(Hi) && (y = Fu(y, f)), N = Pt(N, y))
     }
-    return n.dirs && (N = Ft(N), N.dirs = N.dirs ? N.dirs.concat(n.dirs) : n.dirs), n.transition && (N.transition = n.transition), b = N, ns(G), b
+    return n.dirs && (N = Pt(N), N.dirs = N.dirs ? N.dirs.concat(n.dirs) : n.dirs), n.transition && (N.transition = n.transition), b = N, ns(T), b
 }
 const Ku = e => {
         let t;
         for (const n in e)(n === "class" || n === "style" || ds(n)) && ((t || (t = {}))[n] = e[n]);
         return t
     },
-    Pu = (e, t) => {
+    Fu = (e, t) => {
         const n = {};
         for (const o in e)(!Hi(o) || !(o.slice(9) in t)) && (n[o] = e[o]);
         return n
     };
 
-function Fu(e, t, n) {
+function Pu(e, t, n) {
     const {
         props: o,
         children: s,
         component: i
     } = e, {
         props: f,
         children: r,
         patchFlag: a
     } = t, l = i.emitsOptions;
     if (t.dirs || t.transition) return !0;
     if (n && a >= 0) {
         if (a & 1024) return !0;
-        if (a & 16) return o ? Pf(o, f, l) : !!f;
+        if (a & 16) return o ? Ff(o, f, l) : !!f;
         if (a & 8) {
             const c = t.dynamicProps;
             for (let u = 0; u < c.length; u++) {
                 const d = c[u];
                 if (f[d] !== o[d] && !bs(l, d)) return !0
             }
         }
-    } else return (s || r) && (!r || !r.$stable) ? !0 : o === f ? !1 : o ? f ? Pf(o, f, l) : !0 : !!f;
+    } else return (s || r) && (!r || !r.$stable) ? !0 : o === f ? !1 : o ? f ? Ff(o, f, l) : !0 : !!f;
     return !1
 }
 
-function Pf(e, t, n) {
+function Ff(e, t, n) {
     const o = Object.keys(t);
     if (o.length !== Object.keys(e).length) return !0;
     for (let s = 0; s < o.length; s++) {
         const i = o[s];
         if (t[i] !== e[i] && !bs(n, i)) return !0
     }
     return !1
@@ -1175,18 +1175,18 @@
             } else y.run()
     };
     h.allowRecurse = !!t;
     let b;
     s === "sync" ? b = h : s === "post" ? b = () => Ue(h, r && r.suspense) : (h.pre = !0, r && (h.id = r.uid), b = () => nf(h));
     const y = new Ki(a, b);
     t ? n ? h() : p = y.run() : s === "post" ? Ue(y.run.bind(y), r && r.suspense) : y.run();
-    const G = () => {
+    const T = () => {
         y.stop(), r && r.scope && Oi(r.scope.effects, y)
     };
-    return m && m.push(G), G
+    return m && m.push(T), T
 }
 
 function ed(e, t, n) {
     const o = this.proxy,
         s = Ze(e) ? e.includes(".") ? qa(o, e) : () => o[e] : e.bind(o, o);
     let i;
     ne(t) ? i = t : (i = t.handler, n = t);
@@ -1269,38 +1269,38 @@
                         }
                 }
                 const r = ce(e),
                     {
                         mode: a
                     } = r;
                 if (o.isLeaving) return Os(f);
-                const l = Ff(f);
+                const l = Pf(f);
                 if (!l) return Os(f);
                 const c = di(l, r, o, n);
                 gi(l, c);
                 const u = n.subTree,
-                    d = u && Ff(u);
+                    d = u && Pf(u);
                 let m = !1;
                 const {
                     getTransitionKey: p
                 } = l.type;
                 if (p) {
                     const h = p();
                     s === void 0 ? s = h : h !== s && (s = h, m = !0)
                 }
                 if (d && d.type !== nt && (!cn(l, d) || m)) {
                     const h = di(d, r, o, n);
                     if (gi(d, h), a === "out-in") return o.isLeaving = !0, h.afterLeave = () => {
                         o.isLeaving = !1, n.update.active !== !1 && n.update()
                     }, Os(f);
-                    a === "in-out" && l.type !== nt && (h.delayLeave = (b, y, G) => {
+                    a === "in-out" && l.type !== nt && (h.delayLeave = (b, y, T) => {
                         const N = tl(o, d);
                         N[String(d.key)] = d, b._leaveCb = () => {
                             y(), b._leaveCb = void 0, delete c.delayedLeave
-                        }, c.delayedLeave = G
+                        }, c.delayedLeave = T
                     })
                 }
                 return f
             }
         }
     },
     el = nd;
@@ -1325,15 +1325,15 @@
         onBeforeLeave: u,
         onLeave: d,
         onAfterLeave: m,
         onLeaveCancelled: p,
         onBeforeAppear: h,
         onAppear: b,
         onAfterAppear: y,
-        onAppearCancelled: G
+        onAppearCancelled: T
     } = t, N = String(e.key), v = tl(n, e), E = (_, R) => {
         _ && et(_, o, 9, R)
     }, J = (_, R) => {
         const A = R[1];
         E(_, R), te(_) ? _.every(K => K.length <= 1) && A() : _.length <= 1 && A()
     }, Y = {
         mode: i,
@@ -1348,58 +1348,58 @@
             A && cn(e, A) && A.el._leaveCb && A.el._leaveCb(), E(R, [_])
         },
         enter(_) {
             let R = a,
                 A = l,
                 K = c;
             if (!n.isMounted)
-                if (s) R = b || a, A = y || l, K = G || c;
+                if (s) R = b || a, A = y || l, K = T || c;
                 else return;
-            let T = !1;
+            let G = !1;
             const z = _._enterCb = M => {
-                T || (T = !0, M ? E(K, [_]) : E(A, [_]), Y.delayedLeave && Y.delayedLeave(), _._enterCb = void 0)
+                G || (G = !0, M ? E(K, [_]) : E(A, [_]), Y.delayedLeave && Y.delayedLeave(), _._enterCb = void 0)
             };
             R ? J(R, [_, z]) : z()
         },
         leave(_, R) {
             const A = String(e.key);
             if (_._enterCb && _._enterCb(!0), n.isUnmounting) return R();
             E(u, [_]);
             let K = !1;
-            const T = _._leaveCb = z => {
+            const G = _._leaveCb = z => {
                 K || (K = !0, R(), z ? E(p, [_]) : E(m, [_]), _._leaveCb = void 0, v[A] === e && delete v[A])
             };
-            v[A] = e, d ? J(d, [_, T]) : T()
+            v[A] = e, d ? J(d, [_, G]) : G()
         },
         clone(_) {
             return di(_, t, n, o)
         }
     };
     return Y
 }
 
 function Os(e) {
-    if (ys(e)) return e = Ft(e), e.children = null, e
+    if (ys(e)) return e = Pt(e), e.children = null, e
 }
 
-function Ff(e) {
+function Pf(e) {
     return ys(e) ? e.children ? e.children[0] : void 0 : e
 }
 
 function gi(e, t) {
     e.shapeFlag & 6 && e.component ? gi(e.component.subTree, t) : e.shapeFlag & 128 ? (e.ssContent.transition = t.clone(e.ssContent), e.ssFallback.transition = t.clone(e.ssFallback)) : e.transition = t
 }
 
 function nl(e, t = !1, n) {
     let o = [],
         s = 0;
     for (let i = 0; i < e.length; i++) {
         let f = e[i];
         const r = n == null ? f.key : String(n) + String(f.key != null ? f.key : i);
-        f.type === _e ? (f.patchFlag & 128 && s++, o = o.concat(nl(f.children, t, r))) : (t || f.type !== nt) && o.push(r != null ? Ft(f, {
+        f.type === _e ? (f.patchFlag & 128 && s++, o = o.concat(nl(f.children, t, r))) : (t || f.type !== nt) && o.push(r != null ? Pt(f, {
             key: r
         }) : f)
     }
     if (s > 1)
         for (let i = 0; i < o.length; i++) o[i].patchFlag = -2;
     return o
 }
@@ -1451,24 +1451,24 @@
                 Yn(), zn(n);
                 const r = et(t, n, e, f);
                 return mn(), En(), r
             });
         return o ? s.unshift(i) : s.push(i), i
     }
 }
-const Tt = e => (t, n = Se) => (!po || e === "sp") && As(e, (...o) => t(...o), n),
-    fd = Tt("bm"),
-    $t = Tt("m"),
-    rd = Tt("bu"),
-    ad = Tt("u"),
-    of = Tt("bum"),
-    sl = Tt("um"),
-    ld = Tt("sp"),
-    cd = Tt("rtg"),
-    ud = Tt("rtc");
+const Gt = e => (t, n = Se) => (!po || e === "sp") && As(e, (...o) => t(...o), n),
+    fd = Gt("bm"),
+    $t = Gt("m"),
+    rd = Gt("bu"),
+    ad = Gt("u"),
+    of = Gt("bum"),
+    sl = Gt("um"),
+    ld = Gt("sp"),
+    cd = Gt("rtg"),
+    ud = Gt("rtc");
 
 function dd(e, t = Se) {
     As("ec", e, t)
 }
 
 function bn(e, t) {
     const n = De;
@@ -1627,15 +1627,15 @@
                     if ((l = e.propsOptions[0]) && ge(l, t)) return f[t] = 3, i[t];
                     if (n !== Ae && ge(n, t)) return f[t] = 4, n[t];
                     mi && (f[t] = 0)
                 }
             }
             const c = eo[t];
             let u, d;
-            if (c) return t === "$attrs" && Pe(e, "get", t), c(e);
+            if (c) return t === "$attrs" && Fe(e, "get", t), c(e);
             if ((u = r.__cssModules) && (u = u[t])) return u;
             if (n !== Ae && ge(n, t)) return f[t] = 4, n[t];
             if (d = a.config.globalProperties, ge(d, t)) return d[t]
         },
         set({
             _: e
         }, t, n) {
@@ -1681,25 +1681,25 @@
         beforeMount: u,
         mounted: d,
         beforeUpdate: m,
         updated: p,
         activated: h,
         deactivated: b,
         beforeDestroy: y,
-        beforeUnmount: G,
+        beforeUnmount: T,
         destroyed: N,
         unmounted: v,
         render: E,
         renderTracked: J,
         renderTriggered: Y,
         errorCaptured: _,
         serverPrefetch: R,
         expose: A,
         inheritAttrs: K,
-        components: T,
+        components: G,
         directives: z,
         filters: M
     } = t;
     if (l && hd(l, o, null, e.appContext.config.unwrapInjectedRef), f)
         for (const Z in f) {
             const H = f[Z];
             ne(H) && (o[Z] = H.bind(n))
@@ -1733,25 +1733,25 @@
         })
     }
     c && qf(c, e, "c");
 
     function k(Z, H) {
         te(H) ? H.forEach($ => Z($.bind(n))) : H && Z(H.bind(n))
     }
-    if (k(fd, u), k($t, d), k(rd, m), k(ad, p), k(od, h), k(sd, b), k(dd, _), k(ud, J), k(cd, Y), k(of, G), k(sl, v), k(ld, R), te(A))
+    if (k(fd, u), k($t, d), k(rd, m), k(ad, p), k(od, h), k(sd, b), k(dd, _), k(ud, J), k(cd, Y), k(of, T), k(sl, v), k(ld, R), te(A))
         if (A.length) {
             const Z = e.exposed || (e.exposed = {});
             A.forEach(H => {
                 Object.defineProperty(Z, H, {
                     get: () => n[H],
                     set: $ => n[H] = $
                 })
             })
         } else e.exposed || (e.exposed = {});
-    E && e.render === dt && (e.render = E), K != null && (e.inheritAttrs = K), T && (e.components = T), z && (e.directives = z)
+    E && e.render === dt && (e.render = E), K != null && (e.inheritAttrs = K), G && (e.components = G), z && (e.directives = z)
 }
 
 function hd(e, t, n = dt, o = !1) {
     te(e) && (e = Ii(e));
     for (const s in e) {
         const i = e[s];
         let f;
@@ -2184,42 +2184,42 @@
         insertStaticContent: p
     } = e, h = (g, I, C, B = null, W = null, x = null, O = !1, D = null, X = !!I.dynamicChildren) => {
         if (g === I) return;
         g && !cn(g, I) && (B = Ee(g), fe(g, W, x, !0), g = null), I.patchFlag === -2 && (X = !1, I.dynamicChildren = null);
         const {
             type: V,
             ref: q,
-            shapeFlag: P
+            shapeFlag: F
         } = I;
         switch (V) {
             case ws:
                 b(g, I, C, B);
                 break;
             case nt:
                 y(g, I, C, B);
                 break;
             case Us:
-                g == null && G(I, C, B, O);
+                g == null && T(I, C, B, O);
                 break;
             case _e:
-                T(g, I, C, B, W, x, O, D, X);
+                G(g, I, C, B, W, x, O, D, X);
                 break;
             default:
-                P & 1 ? E(g, I, C, B, W, x, O, D, X) : P & 6 ? z(g, I, C, B, W, x, O, D, X) : (P & 64 || P & 128) && V.process(g, I, C, B, W, x, O, D, X, ye)
+                F & 1 ? E(g, I, C, B, W, x, O, D, X) : F & 6 ? z(g, I, C, B, W, x, O, D, X) : (F & 64 || F & 128) && V.process(g, I, C, B, W, x, O, D, X, ye)
         }
         q != null && W && bi(q, g && g.ref, x, I || g, !I)
     }, b = (g, I, C, B) => {
         if (g == null) o(I.el = r(I.children), C, B);
         else {
             const W = I.el = g.el;
             I.children !== g.children && l(W, I.children)
         }
     }, y = (g, I, C, B) => {
         g == null ? o(I.el = a(I.children || ""), C, B) : I.el = g.el
-    }, G = (g, I, C, B) => {
+    }, T = (g, I, C, B) => {
         [g.el, g.anchor] = p(g.children, I, C, B, g.el, g.anchor)
     }, N = ({
         el: g,
         anchor: I
     }, C, B) => {
         let W;
         for (; g && g !== I;) W = d(g), o(g, C, B), g = W;
@@ -2233,26 +2233,26 @@
         s(I)
     }, E = (g, I, C, B, W, x, O, D, X) => {
         O = O || I.type === "svg", g == null ? J(I, C, B, W, x, O, D, X) : R(g, I, W, x, O, D, X)
     }, J = (g, I, C, B, W, x, O, D) => {
         let X, V;
         const {
             type: q,
-            props: P,
+            props: F,
             shapeFlag: Q,
             transition: ee,
             dirs: re
         } = g;
-        if (X = g.el = f(g.type, x, P && P.is, P), Q & 8 ? c(X, g.children) : Q & 16 && _(g.children, X, null, B, W, x && q !== "foreignObject", O, D), re && tn(g, null, B, "created"), Y(X, g, g.scopeId, O, B), P) {
-            for (const he in P) he !== "value" && !Xo(he) && i(X, he, null, P[he], x, g.children, B, W, We);
-            "value" in P && i(X, "value", null, P.value), (V = P.onVnodeBeforeMount) && mt(V, B, g)
+        if (X = g.el = f(g.type, x, F && F.is, F), Q & 8 ? c(X, g.children) : Q & 16 && _(g.children, X, null, B, W, x && q !== "foreignObject", O, D), re && tn(g, null, B, "created"), Y(X, g, g.scopeId, O, B), F) {
+            for (const he in F) he !== "value" && !Xo(he) && i(X, he, null, F[he], x, g.children, B, W, We);
+            "value" in F && i(X, "value", null, F.value), (V = F.onVnodeBeforeMount) && mt(V, B, g)
         }
         re && tn(g, null, B, "beforeMount");
         const be = (!W || W && !W.pendingBranch) && ee && !ee.persisted;
-        be && ee.beforeEnter(X), o(X, I, C), ((V = P && P.onVnodeMounted) || be || re) && Ue(() => {
+        be && ee.beforeEnter(X), o(X, I, C), ((V = F && F.onVnodeMounted) || be || re) && Ue(() => {
             V && mt(V, B, g), be && ee.enter(X), re && tn(g, null, B, "mounted")
         }, W)
     }, Y = (g, I, C, B, W) => {
         if (C && m(g, C), B)
             for (let x = 0; x < B.length; x++) m(g, B[x]);
         if (W) {
             let x = W.subTree;
@@ -2270,32 +2270,32 @@
         const D = I.el = g.el;
         let {
             patchFlag: X,
             dynamicChildren: V,
             dirs: q
         } = I;
         X |= g.patchFlag & 16;
-        const P = g.props || Ae,
+        const F = g.props || Ae,
             Q = I.props || Ae;
         let ee;
         C && nn(C, !1), (ee = Q.onVnodeBeforeUpdate) && mt(ee, C, I, g), q && tn(I, g, C, "beforeUpdate"), C && nn(C, !0);
         const re = W && I.type !== "foreignObject";
         if (V ? A(g.dynamicChildren, V, D, C, B, re, x) : O || H(g, I, D, null, C, B, re, x, !1), X > 0) {
-            if (X & 16) K(D, I, P, Q, C, B, W);
-            else if (X & 2 && P.class !== Q.class && i(D, "class", null, Q.class, W), X & 4 && i(D, "style", P.style, Q.style, W), X & 8) {
+            if (X & 16) K(D, I, F, Q, C, B, W);
+            else if (X & 2 && F.class !== Q.class && i(D, "class", null, Q.class, W), X & 4 && i(D, "style", F.style, Q.style, W), X & 8) {
                 const be = I.dynamicProps;
                 for (let he = 0; he < be.length; he++) {
                     const Ve = be[he],
-                        rt = P[Ve],
+                        rt = F[Ve],
                         vn = Q[Ve];
                     (vn !== rt || Ve === "value") && i(D, Ve, rt, vn, W, g.children, C, B, We)
                 }
             }
             X & 1 && g.children !== I.children && c(D, I.children)
-        } else !O && V == null && K(D, I, P, Q, C, B, W);
+        } else !O && V == null && K(D, I, F, Q, C, B, W);
         ((ee = Q.onVnodeUpdated) || q) && Ue(() => {
             ee && mt(ee, C, I, g), q && tn(I, g, C, "updated")
         }, B)
     }, A = (g, I, C, B, W, x, O) => {
         for (let D = 0; D < I.length; D++) {
             const X = g[D],
                 V = I[D],
@@ -2310,70 +2310,70 @@
                 if (Xo(D)) continue;
                 const X = B[D],
                     V = C[D];
                 X !== V && D !== "value" && i(g, D, V, X, O, I.children, W, x, We)
             }
             "value" in B && i(g, "value", C.value, B.value)
         }
-    }, T = (g, I, C, B, W, x, O, D, X) => {
+    }, G = (g, I, C, B, W, x, O, D, X) => {
         const V = I.el = g ? g.el : r(""),
             q = I.anchor = g ? g.anchor : r("");
         let {
-            patchFlag: P,
+            patchFlag: F,
             dynamicChildren: Q,
             slotScopeIds: ee
         } = I;
-        ee && (D = D ? D.concat(ee) : ee), g == null ? (o(V, C, B), o(q, C, B), _(I.children, C, q, W, x, O, D, X)) : P > 0 && P & 64 && Q && g.dynamicChildren ? (A(g.dynamicChildren, Q, C, W, x, O, D), (I.key != null || W && I === W.subTree) && pl(g, I, !0)) : H(g, I, C, q, W, x, O, D, X)
+        ee && (D = D ? D.concat(ee) : ee), g == null ? (o(V, C, B), o(q, C, B), _(I.children, C, q, W, x, O, D, X)) : F > 0 && F & 64 && Q && g.dynamicChildren ? (A(g.dynamicChildren, Q, C, W, x, O, D), (I.key != null || W && I === W.subTree) && pl(g, I, !0)) : H(g, I, C, q, W, x, O, D, X)
     }, z = (g, I, C, B, W, x, O, D, X) => {
         I.slotScopeIds = D, g == null ? I.shapeFlag & 512 ? W.ctx.activate(I, C, B, O, X) : M(I, C, B, W, x, O, X) : S(g, I, X)
     }, M = (g, I, C, B, W, x, O) => {
         const D = g.component = Dd(g, B, W);
         if (ys(g) && (D.ctx.renderer = ye), Rd(D), D.asyncDep) {
             if (W && W.registerDep(D, k), !g.el) {
                 const X = D.subTree = se(nt);
                 y(null, X, I, C)
             }
             return
         }
         k(D, g, I, C, W, x, O)
     }, S = (g, I, C) => {
         const B = I.component = g.component;
-        if (Fu(g, I, C))
+        if (Pu(g, I, C))
             if (B.asyncDep && !B.asyncResolved) {
                 Z(B, I, C);
                 return
             } else B.next = I, Ou(B.update), B.update();
         else I.el = g.el, B.vnode = I
     }, k = (g, I, C, B, W, x, O) => {
         const D = () => {
                 if (g.isMounted) {
                     let {
                         next: q,
-                        bu: P,
+                        bu: F,
                         u: Q,
                         parent: ee,
                         vnode: re
                     } = g, be = q, he;
-                    nn(g, !1), q ? (q.el = re.el, Z(g, q, O)) : q = re, P && Eo(P), (he = q.props && q.props.onVnodeBeforeUpdate) && mt(he, ee, q, re), nn(g, !0);
+                    nn(g, !1), q ? (q.el = re.el, Z(g, q, O)) : q = re, F && Eo(F), (he = q.props && q.props.onVnodeBeforeUpdate) && mt(he, ee, q, re), nn(g, !0);
                     const Ve = Hs(g),
                         rt = g.subTree;
                     g.subTree = Ve, h(rt, Ve, u(rt.el), Ee(rt), g, W, x), q.el = Ve.el, be === null && $u(g, Ve.el), Q && Ue(Q, W), (he = q.props && q.props.onVnodeUpdated) && Ue(() => mt(he, ee, q, re), W)
                 } else {
                     let q;
                     const {
-                        el: P,
+                        el: F,
                         props: Q
                     } = I, {
                         bm: ee,
                         m: re,
                         parent: be
                     } = g, he = qn(I);
-                    if (nn(g, !1), ee && Eo(ee), !he && (q = Q && Q.onVnodeBeforeMount) && mt(q, be, I), nn(g, !0), P && ft) {
+                    if (nn(g, !1), ee && Eo(ee), !he && (q = Q && Q.onVnodeBeforeMount) && mt(q, be, I), nn(g, !0), F && ft) {
                         const Ve = () => {
-                            g.subTree = Hs(g), ft(P, g.subTree, g, W, null)
+                            g.subTree = Hs(g), ft(F, g.subTree, g, W, null)
                         };
                         he ? I.type.__asyncLoader().then(() => !g.isUnmounted && Ve()) : Ve()
                     } else {
                         const Ve = g.subTree = Hs(g);
                         h(null, Ve, C, B, g, W, x), I.el = Ve.el
                     }
                     if (re && Ue(re, W), !he && (q = Q && Q.onVnodeMounted)) {
@@ -2388,101 +2388,101 @@
     }, Z = (g, I, C) => {
         I.component = g;
         const B = g.vnode.props;
         g.vnode = I, g.next = null, vd(g, I.props, B, C), Nd(g, I.children, C), Yn(), Kf(), En()
     }, H = (g, I, C, B, W, x, O, D, X = !1) => {
         const V = g && g.children,
             q = g ? g.shapeFlag : 0,
-            P = I.children,
+            F = I.children,
             {
                 patchFlag: Q,
                 shapeFlag: ee
             } = I;
         if (Q > 0) {
             if (Q & 128) {
-                le(V, P, C, B, W, x, O, D, X);
+                le(V, F, C, B, W, x, O, D, X);
                 return
             } else if (Q & 256) {
-                $(V, P, C, B, W, x, O, D, X);
+                $(V, F, C, B, W, x, O, D, X);
                 return
             }
         }
-        ee & 8 ? (q & 16 && We(V, W, x), P !== V && c(C, P)) : q & 16 ? ee & 16 ? le(V, P, C, B, W, x, O, D, X) : We(V, W, x, !0) : (q & 8 && c(C, ""), ee & 16 && _(P, C, B, W, x, O, D, X))
+        ee & 8 ? (q & 16 && We(V, W, x), F !== V && c(C, F)) : q & 16 ? ee & 16 ? le(V, F, C, B, W, x, O, D, X) : We(V, W, x, !0) : (q & 8 && c(C, ""), ee & 16 && _(F, C, B, W, x, O, D, X))
     }, $ = (g, I, C, B, W, x, O, D, X) => {
         g = g || Mn, I = I || Mn;
         const V = g.length,
             q = I.length,
-            P = Math.min(V, q);
+            F = Math.min(V, q);
         let Q;
-        for (Q = 0; Q < P; Q++) {
+        for (Q = 0; Q < F; Q++) {
             const ee = I[Q] = X ? Ht(I[Q]) : It(I[Q]);
             h(g[Q], ee, C, null, W, x, O, D, X)
         }
-        V > q ? We(g, W, x, !0, !1, P) : _(I, C, B, W, x, O, D, X, P)
+        V > q ? We(g, W, x, !0, !1, F) : _(I, C, B, W, x, O, D, X, F)
     }, le = (g, I, C, B, W, x, O, D, X) => {
         let V = 0;
         const q = I.length;
-        let P = g.length - 1,
+        let F = g.length - 1,
             Q = q - 1;
-        for (; V <= P && V <= Q;) {
+        for (; V <= F && V <= Q;) {
             const ee = g[V],
                 re = I[V] = X ? Ht(I[V]) : It(I[V]);
             if (cn(ee, re)) h(ee, re, C, null, W, x, O, D, X);
             else break;
             V++
         }
-        for (; V <= P && V <= Q;) {
-            const ee = g[P],
+        for (; V <= F && V <= Q;) {
+            const ee = g[F],
                 re = I[Q] = X ? Ht(I[Q]) : It(I[Q]);
             if (cn(ee, re)) h(ee, re, C, null, W, x, O, D, X);
             else break;
-            P--, Q--
+            F--, Q--
         }
-        if (V > P) {
+        if (V > F) {
             if (V <= Q) {
                 const ee = Q + 1,
                     re = ee < q ? I[ee].el : B;
                 for (; V <= Q;) h(null, I[V] = X ? Ht(I[V]) : It(I[V]), C, re, W, x, O, D, X), V++
             }
         } else if (V > Q)
-            for (; V <= P;) fe(g[V], W, x, !0), V++;
+            for (; V <= F;) fe(g[V], W, x, !0), V++;
         else {
             const ee = V,
                 re = V,
                 be = new Map;
             for (V = re; V <= Q; V++) {
-                const Fe = I[V] = X ? Ht(I[V]) : It(I[V]);
-                Fe.key != null && be.set(Fe.key, V)
+                const Pe = I[V] = X ? Ht(I[V]) : It(I[V]);
+                Pe.key != null && be.set(Pe.key, V)
             }
             let he, Ve = 0;
             const rt = Q - re + 1;
             let vn = !1,
                 Df = 0;
             const Jn = new Array(rt);
             for (V = 0; V < rt; V++) Jn[V] = 0;
-            for (V = ee; V <= P; V++) {
-                const Fe = g[V];
+            for (V = ee; V <= F; V++) {
+                const Pe = g[V];
                 if (Ve >= rt) {
-                    fe(Fe, W, x, !0);
+                    fe(Pe, W, x, !0);
                     continue
                 }
                 let pt;
-                if (Fe.key != null) pt = be.get(Fe.key);
+                if (Pe.key != null) pt = be.get(Pe.key);
                 else
                     for (he = re; he <= Q; he++)
-                        if (Jn[he - re] === 0 && cn(Fe, I[he])) {
+                        if (Jn[he - re] === 0 && cn(Pe, I[he])) {
                             pt = he;
                             break
-                        } pt === void 0 ? fe(Fe, W, x, !0) : (Jn[pt - re] = V + 1, pt >= Df ? Df = pt : vn = !0, h(Fe, I[pt], C, null, W, x, O, D, X), Ve++)
+                        } pt === void 0 ? fe(Pe, W, x, !0) : (Jn[pt - re] = V + 1, pt >= Df ? Df = pt : vn = !0, h(Pe, I[pt], C, null, W, x, O, D, X), Ve++)
             }
             const Rf = vn ? Bd(Jn) : Mn;
             for (he = Rf.length - 1, V = rt - 1; V >= 0; V--) {
-                const Fe = re + V,
-                    pt = I[Fe],
-                    xf = Fe + 1 < q ? I[Fe + 1].el : B;
+                const Pe = re + V,
+                    pt = I[Pe],
+                    xf = Pe + 1 < q ? I[Pe + 1].el : B;
                 Jn[V] === 0 ? h(null, pt, C, xf, W, x, O, D, X) : vn && (he < 0 || V !== Rf[he] ? Ie(pt, C, xf, 2) : he--)
             }
         }
     }, Ie = (g, I, C, B, W = null) => {
         const {
             el: x,
             type: O,
@@ -2500,46 +2500,46 @@
         }
         if (V & 64) {
             O.move(g, I, C, ye);
             return
         }
         if (O === _e) {
             o(x, I, C);
-            for (let P = 0; P < X.length; P++) Ie(X[P], I, C, B);
+            for (let F = 0; F < X.length; F++) Ie(X[F], I, C, B);
             o(g.anchor, I, C);
             return
         }
         if (O === Us) {
             N(g, I, C);
             return
         }
         if (B !== 2 && V & 1 && D)
             if (B === 0) D.beforeEnter(x), o(x, I, C), Ue(() => D.enter(x), W);
             else {
                 const {
-                    leave: P,
+                    leave: F,
                     delayLeave: Q,
                     afterLeave: ee
                 } = D, re = () => o(x, I, C), be = () => {
-                    P(x, () => {
+                    F(x, () => {
                         re(), ee && ee()
                     })
                 };
                 Q ? Q(x, re, be) : be()
             }
         else o(x, I, C)
     }, fe = (g, I, C, B = !1, W = !1) => {
         const {
             type: x,
             props: O,
             ref: D,
             children: X,
             dynamicChildren: V,
             shapeFlag: q,
-            patchFlag: P,
+            patchFlag: F,
             dirs: Q
         } = g;
         if (D != null && bi(D, null, C, g, !0), q & 256) {
             I.ctx.deactivate(g);
             return
         }
         const ee = q & 1 && Q,
@@ -2547,15 +2547,15 @@
         let be;
         if (re && (be = O && O.onVnodeBeforeUnmount) && mt(be, I, g), q & 6) ze(g.component, C, B);
         else {
             if (q & 128) {
                 g.suspense.unmount(C, B);
                 return
             }
-            ee && tn(g, null, I, "beforeUnmount"), q & 64 ? g.type.remove(g, I, C, W, ye, B) : V && (x !== _e || P > 0 && P & 64) ? We(V, I, C, !1, !0) : (x === _e && P & 384 || !W && q & 16) && We(X, I, C), B && we(g)
+            ee && tn(g, null, I, "beforeUnmount"), q & 64 ? g.type.remove(g, I, C, W, ye, B) : V && (x !== _e || F > 0 && F & 64) ? We(V, I, C, !1, !0) : (x === _e && F & 384 || !W && q & 16) && We(X, I, C), B && we(g)
         }(re && (be = O && O.onVnodeUnmounted) || ee) && Ue(() => {
             be && mt(be, I, g), ee && tn(g, null, I, "unmounted")
         }, C)
     }, we = g => {
         const {
             type: I,
             el: C,
@@ -2678,15 +2678,15 @@
 }
 
 function ml(e) {
     return e.dynamicChildren = go > 0 ? ct || Mn : null, Vd(), go > 0 && ct && ct.push(e), e
 }
 
 function U(e, t, n, o, s, i) {
-    return ml(F(e, t, n, o, s, i, !0))
+    return ml(P(e, t, n, o, s, i, !0))
 }
 
 function Me(e, t, n, o, s) {
     return ml(se(e, t, n, o, s, !0))
 }
 
 function ss(e) {
@@ -2707,15 +2707,15 @@
     }) => e != null ? Ze(e) || Be(e) || ne(e) ? {
         i: De,
         r: e,
         k: t,
         f: !!n
     } : e : null;
 
-function F(e, t = null, n = null, o = 0, s = null, i = e === _e ? 0 : 1, f = !1, r = !1) {
+function P(e, t = null, n = null, o = 0, s = null, i = e === _e ? 0 : 1, f = !1, r = !1) {
     const a = {
         __v_isVNode: !0,
         __v_skip: !0,
         type: e,
         props: t,
         key: t && Il(t),
         ref: t && Ho(t),
@@ -2738,38 +2738,38 @@
         dynamicProps: s,
         dynamicChildren: null,
         appContext: null,
         ctx: De
     };
     return r ? (cf(a, n), i & 128 && e.normalize(a)) : n && (a.shapeFlag |= Ze(n) ? 8 : 16), go > 0 && !f && ct && (a.patchFlag > 0 || i & 6) && a.patchFlag !== 32 && ct.push(a), a
 }
-const se = Td;
+const se = Gd;
 
-function Td(e, t = null, n = null, o = 0, s = null, i = !1) {
+function Gd(e, t = null, n = null, o = 0, s = null, i = !1) {
     if ((!e || e === il) && (e = nt), ss(e)) {
-        const r = Ft(e, t, !0);
+        const r = Pt(e, t, !0);
         return n && cf(r, n), go > 0 && !i && ct && (r.shapeFlag & 6 ? ct[ct.indexOf(e)] = r : ct.push(r)), r.patchFlag |= -2, r
     }
     if (Hd(e) && (e = e.__vccOpts), t) {
         t = lf(t);
         let {
             class: r,
             style: a
         } = t;
         r && !Ze(r) && (t.class = L(r)), ve(a) && (Ra(a) && !te(a) && (a = Re({}, a)), t.style = Ot(a))
     }
     const f = Ze(e) ? 1 : Qu(e) ? 128 : zd(e) ? 64 : ve(e) ? 4 : ne(e) ? 2 : 0;
-    return F(e, t, n, o, s, f, i, !0)
+    return P(e, t, n, o, s, f, i, !0)
 }
 
 function lf(e) {
     return e ? Ra(e) || _s in e ? Re({}, e) : e : null
 }
 
-function Ft(e, t, n = !1) {
+function Pt(e, t, n = !1) {
     const {
         props: o,
         ref: s,
         patchFlag: i,
         children: f
     } = e, r = t ? On(o || {}, t) : o;
     return {
@@ -2790,37 +2790,37 @@
         dynamicProps: e.dynamicProps,
         dynamicChildren: e.dynamicChildren,
         appContext: e.appContext,
         dirs: e.dirs,
         transition: e.transition,
         component: e.component,
         suspense: e.suspense,
-        ssContent: e.ssContent && Ft(e.ssContent),
-        ssFallback: e.ssFallback && Ft(e.ssFallback),
+        ssContent: e.ssContent && Pt(e.ssContent),
+        ssFallback: e.ssFallback && Pt(e.ssFallback),
         el: e.el,
         anchor: e.anchor,
         ctx: e.ctx,
         ce: e.ce
     }
 }
 
-function Gd(e = " ", t = 0) {
+function Td(e = " ", t = 0) {
     return se(ws, null, e, t)
 }
 
 function me(e = "", t = !1) {
     return t ? (j(), Me(nt, null, e)) : se(nt, null, e)
 }
 
 function It(e) {
     return e == null || typeof e == "boolean" ? se(nt) : te(e) ? se(_e, null, e.slice()) : typeof e == "object" ? Ht(e) : se(ws, null, String(e))
 }
 
 function Ht(e) {
-    return e.el === null && e.patchFlag !== -1 || e.memo ? e : Ft(e)
+    return e.el === null && e.patchFlag !== -1 || e.memo ? e : Pt(e)
 }
 
 function cf(e, t) {
     let n = 0;
     const {
         shapeFlag: o
     } = e;
@@ -2835,15 +2835,15 @@
             n = 32;
             const s = t._;
             !s && !(_s in t) ? t._ctx = De : s === 3 && De && (De.slots._ === 1 ? t._ = 1 : (t._ = 2, e.patchFlag |= 1024))
         }
     else ne(t) ? (t = {
         default: t,
         _ctx: De
-    }, n = 32) : (t = String(t), o & 64 ? (n = 16, t = [Gd(t)]) : n = 8);
+    }, n = 32) : (t = String(t), o & 64 ? (n = 16, t = [Td(t)]) : n = 8);
     e.children = t, e.shapeFlag |= n
 }
 
 function On(...e) {
     const t = {};
     for (let n = 0; n < e.length; n++) {
         const o = e[n];
@@ -3004,15 +3004,15 @@
     }
     zn(e), Yn(), Id(e), En(), mn()
 }
 
 function Xd(e) {
     return new Proxy(e.attrs, {
         get(t, n) {
-            return Pe(e, "get", "$attrs"), t[n]
+            return Fe(e, "get", "$attrs"), t[n]
         }
     })
 }
 
 function Yd(e) {
     const t = o => {
         e.exposed = o || {}
@@ -3101,20 +3101,20 @@
                 }
                 t.insertBefore(r, n)
             }
             return [f ? f.nextSibling : t.firstChild, n ? n.previousSibling : t.lastChild]
         }
     };
 
-function Pd(e, t, n) {
+function Fd(e, t, n) {
     const o = e._vtc;
     o && (t = (t ? [t, ...o] : [...o]).join(" ")), t == null ? e.removeAttribute("class") : n ? e.setAttribute("class", t) : e.className = t
 }
 
-function Fd(e, t, n) {
+function Pd(e, t, n) {
     const o = e.style,
         s = Ze(n);
     if (n && !s) {
         if (t && !Ze(t))
             for (const i in t) n[i] == null && Ci(o, i, "");
         for (const i in n) Ci(o, i, n[i])
     } else {
@@ -3148,15 +3148,15 @@
     return t
 }
 const ur = "http://www.w3.org/1999/xlink";
 
 function Qd(e, t, n, o, s) {
     if (o && t.startsWith("xlink:")) n == null ? e.removeAttributeNS(ur, t.slice(6, t.length)) : e.setAttributeNS(ur, t, n);
     else {
-        const i = Fc(t);
+        const i = Pc(t);
         n == null || i && !ba(n) ? e.removeAttribute(t) : e.setAttribute(t, i ? "" : n)
     }
 }
 
 function qd(e, t, n, o, s, i, f) {
     if (t === "innerHTML" || t === "textContent") {
         o && f(o, s, i), e[t] = n ?? "";
@@ -3229,15 +3229,15 @@
         return e.stopImmediatePropagation = () => {
             n.call(e), e._stopped = !0
         }, t.map(o => s => !s._stopped && o && o(s))
     } else return t
 }
 const gr = /^on[a-z]/,
     rg = (e, t, n, o, s = !1, i, f, r, a) => {
-        t === "class" ? Pd(e, o, s) : t === "style" ? Fd(e, n, o) : ds(t) ? Hi(t) || tg(e, t, n, o, f) : (t[0] === "." ? (t = t.slice(1), !0) : t[0] === "^" ? (t = t.slice(1), !1) : ag(e, t, o, s)) ? qd(e, t, o, i, f, r, a) : (t === "true-value" ? e._trueValue = o : t === "false-value" && (e._falseValue = o), Qd(e, t, o, s))
+        t === "class" ? Fd(e, o, s) : t === "style" ? Pd(e, n, o) : ds(t) ? Hi(t) || tg(e, t, n, o, f) : (t[0] === "." ? (t = t.slice(1), !0) : t[0] === "^" ? (t = t.slice(1), !1) : ag(e, t, o, s)) ? qd(e, t, o, i, f, r, a) : (t === "true-value" ? e._trueValue = o : t === "false-value" && (e._falseValue = o), Qd(e, t, o, s))
     };
 
 function ag(e, t, n, o) {
     return o ? !!(t === "innerHTML" || t === "textContent" || t in e && gr.test(t) && ne(n)) : t === "spellcheck" || t === "draggable" || t === "translate" || t === "form" || t === "list" && e.tagName === "INPUT" || t === "type" && e.tagName === "TEXTAREA" || gr.test(t) && Ze(n) ? !1 : t in e
 }
 const Dt = "transition",
     Kn = "animation",
@@ -3267,15 +3267,15 @@
 const on = (e, t = []) => {
         te(e) ? e.forEach(n => n(...t)) : e && e(...t)
     },
     pr = e => e ? te(e) ? e.some(t => t.length > 1) : e.length > 1 : !1;
 
 function lg(e) {
     const t = {};
-    for (const T in e) T in Cl || (t[T] = e[T]);
+    for (const G in e) G in Cl || (t[G] = e[G]);
     if (e.css === !1) return t;
     const {
         name: n = "v",
         type: o,
         duration: s,
         enterFromClass: i = `${n}-enter-from`,
         enterActiveClass: f = `${n}-enter-active`,
@@ -3284,69 +3284,69 @@
         appearActiveClass: l = f,
         appearToClass: c = r,
         leaveFromClass: u = `${n}-leave-from`,
         leaveActiveClass: d = `${n}-leave-active`,
         leaveToClass: m = `${n}-leave-to`
     } = e, p = cg(s), h = p && p[0], b = p && p[1], {
         onBeforeEnter: y,
-        onEnter: G,
+        onEnter: T,
         onEnterCancelled: N,
         onLeave: v,
         onLeaveCancelled: E,
         onBeforeAppear: J = y,
-        onAppear: Y = G,
+        onAppear: Y = T,
         onAppearCancelled: _ = N
-    } = t, R = (T, z, M) => {
-        sn(T, z ? c : r), sn(T, z ? l : f), M && M()
-    }, A = (T, z) => {
-        T._isLeaving = !1, sn(T, u), sn(T, m), sn(T, d), z && z()
-    }, K = T => (z, M) => {
-        const S = T ? Y : G,
-            k = () => R(z, T, M);
+    } = t, R = (G, z, M) => {
+        sn(G, z ? c : r), sn(G, z ? l : f), M && M()
+    }, A = (G, z) => {
+        G._isLeaving = !1, sn(G, u), sn(G, m), sn(G, d), z && z()
+    }, K = G => (z, M) => {
+        const S = G ? Y : T,
+            k = () => R(z, G, M);
         on(S, [z, k]), mr(() => {
-            sn(z, T ? a : i), Rt(z, T ? c : r), pr(S) || Ir(z, o, h, k)
+            sn(z, G ? a : i), Rt(z, G ? c : r), pr(S) || Ir(z, o, h, k)
         })
     };
     return Re(t, {
-        onBeforeEnter(T) {
-            on(y, [T]), Rt(T, i), Rt(T, f)
+        onBeforeEnter(G) {
+            on(y, [G]), Rt(G, i), Rt(G, f)
         },
-        onBeforeAppear(T) {
-            on(J, [T]), Rt(T, a), Rt(T, l)
+        onBeforeAppear(G) {
+            on(J, [G]), Rt(G, a), Rt(G, l)
         },
         onEnter: K(!1),
         onAppear: K(!0),
-        onLeave(T, z) {
-            T._isLeaving = !0;
-            const M = () => A(T, z);
-            Rt(T, u), gg(), Rt(T, d), mr(() => {
-                T._isLeaving && (sn(T, u), Rt(T, m), pr(v) || Ir(T, o, b, M))
-            }), on(v, [T, M])
+        onLeave(G, z) {
+            G._isLeaving = !0;
+            const M = () => A(G, z);
+            Rt(G, u), gg(), Rt(G, d), mr(() => {
+                G._isLeaving && (sn(G, u), Rt(G, m), pr(v) || Ir(G, o, b, M))
+            }), on(v, [G, M])
         },
-        onEnterCancelled(T) {
-            R(T, !1), on(N, [T])
+        onEnterCancelled(G) {
+            R(G, !1), on(N, [G])
         },
-        onAppearCancelled(T) {
-            R(T, !0), on(_, [T])
+        onAppearCancelled(G) {
+            R(G, !0), on(_, [G])
         },
-        onLeaveCancelled(T) {
-            A(T), on(E, [T])
+        onLeaveCancelled(G) {
+            A(G), on(E, [G])
         }
     })
 }
 
 function cg(e) {
     if (e == null) return null;
-    if (ve(e)) return [Ps(e.enter), Ps(e.leave)]; {
-        const t = Ps(e);
+    if (ve(e)) return [Fs(e.enter), Fs(e.leave)]; {
+        const t = Fs(e);
         return [t, t]
     }
 }
 
-function Ps(e) {
+function Fs(e) {
     return ou(e)
 }
 
 function Rt(e, t) {
     t.split(/\s+/).forEach(n => n && e.classList.add(n)), (e._vtc || (e._vtc = new Set)).add(t)
 }
 
@@ -3489,41 +3489,41 @@
     },
     Ar = {
         beforeMount(e, {
             value: t
         }, {
             transition: n
         }) {
-            e._vod = e.style.display === "none" ? "" : e.style.display, n && t ? n.beforeEnter(e) : Pn(e, t)
+            e._vod = e.style.display === "none" ? "" : e.style.display, n && t ? n.beforeEnter(e) : Fn(e, t)
         },
         mounted(e, {
             value: t
         }, {
             transition: n
         }) {
             n && t && n.enter(e)
         },
         updated(e, {
             value: t,
             oldValue: n
         }, {
             transition: o
         }) {
-            !t != !n && (o ? t ? (o.beforeEnter(e), Pn(e, !0), o.enter(e)) : o.leave(e, () => {
-                Pn(e, !1)
-            }) : Pn(e, t))
+            !t != !n && (o ? t ? (o.beforeEnter(e), Fn(e, !0), o.enter(e)) : o.leave(e, () => {
+                Fn(e, !1)
+            }) : Fn(e, t))
         },
         beforeUnmount(e, {
             value: t
         }) {
-            Pn(e, t)
+            Fn(e, t)
         }
     };
 
-function Pn(e, t) {
+function Fn(e, t) {
     e.style.display = t ? e._vod : "none"
 }
 const hg = Re({
     patchProp: rg
 }, Kd);
 let vr;
 
@@ -3580,15 +3580,15 @@
                 };
             return t({
                 inputRef: ue(() => o.value)
             }), (r, a) => (j(), U("div", {
                 class: L([r.$style["ops-rooms-search"], {
                     [r.$style["ops-rooms-search__focus"]]: s.value
                 }])
-            }, [Xe(r.$slots, "prefix"), F("input", {
+            }, [Xe(r.$slots, "prefix"), P("input", {
                 ref_key: "inputRef",
                 ref: o,
                 class: L(r.$style["ops-rooms-search__input"]),
                 placeholder: e.placeholder || "Type...",
                 value: e.modelValue,
                 type: "text",
                 onFocus: a[0] || (a[0] = l => s.value = !0),
@@ -3648,15 +3648,15 @@
             u = "month",
             d = "quarter",
             m = "year",
             p = "date",
             h = "Invalid Date",
             b = /^(\d{4})[-/]?(\d{1,2})?[-/]?(\d{0,2})[Tt\s]*(\d{1,2})?:?(\d{1,2})?:?(\d{1,2})?[.:]?(\d+)?$/,
             y = /\[([^\]]+)]|Y{1,4}|M{1,4}|D{1,2}|d{1,4}|H{1,2}|h{1,2}|a|A|m{1,2}|s{1,2}|Z{1,2}|SSS/g,
-            G = {
+            T = {
                 name: "en",
                 weekdays: "Sunday_Monday_Tuesday_Wednesday_Thursday_Friday_Saturday".split("_"),
                 months: "January_February_March_April_May_June_July_August_September_October_November_December".split("_"),
                 ordinal: function(z) {
                     var M = ["th", "st", "nd", "rd"],
                         S = z % 100;
                     return "[" + z + (M[(S - 20) % 10] || M[S] || M[0]) + "]"
@@ -3702,15 +3702,15 @@
                 },
                 u: function(z) {
                     return z === void 0
                 }
             },
             E = "en",
             J = {};
-        J[E] = G;
+        J[E] = T;
         var Y = function(z) {
                 return z instanceof K
             },
             _ = function z(M, S, k) {
                 var Z;
                 if (!M) return E;
                 if (typeof M == "string") {
@@ -3925,26 +3925,26 @@
                     return this.isValid() ? this.toISOString() : null
                 }, M.toISOString = function() {
                     return this.$d.toISOString()
                 }, M.toString = function() {
                     return this.$d.toUTCString()
                 }, z
             }(),
-            T = K.prototype;
-        return R.prototype = T, [
+            G = K.prototype;
+        return R.prototype = G, [
             ["$ms", i],
             ["$s", f],
             ["$m", r],
             ["$H", a],
             ["$W", l],
             ["$M", u],
             ["$y", m],
             ["$D", p]
         ].forEach(function(z) {
-            T[z[1]] = function(M) {
+            G[z[1]] = function(M) {
                 return this.$g(M, z[0], z[1])
             }
         }), R.extend = function(z, M) {
             return z.$i || (z(M, K, R), z.$i = !0), R
         }, R.locale = _, R.isDayjs = Y, R.unix = function(z) {
             return R(1e3 * z)
         }, R.en = J[E], R.Ls = J, R.p = {}, R
@@ -3983,15 +3983,15 @@
                     yy: "%d years"
                 };
 
             function r(l, c, u, d) {
                 return i.fromToBase(l, c, u, d)
             }
             s.en.relativeTime = f, i.fromToBase = function(l, c, u, d, m) {
-                for (var p, h, b, y = u.$locale().relativeTime || f, G = n.thresholds || [{
+                for (var p, h, b, y = u.$locale().relativeTime || f, T = n.thresholds || [{
                         l: "s",
                         r: 44,
                         d: "second"
                     }, {
                         l: "m",
                         r: 89
                     }, {
@@ -4021,20 +4021,20 @@
                         d: "month"
                     }, {
                         l: "y",
                         r: 17
                     }, {
                         l: "yy",
                         d: "year"
-                    }], N = G.length, v = 0; v < N; v += 1) {
-                    var E = G[v];
+                    }], N = T.length, v = 0; v < N; v += 1) {
+                    var E = T[v];
                     E.d && (p = d ? s(l).diff(u, E.d, !0) : u.diff(l, E.d, !0));
                     var J = (n.rounding || Math.round)(Math.abs(p));
                     if (b = p > 0, J <= E.r || !E.r) {
-                        J <= 1 && v > 0 && (E = G[v - 1]);
+                        J <= 1 && v > 0 && (E = T[v - 1]);
                         var Y = y[E.l];
                         m && (J = m("" + J)), h = typeof Y == "string" ? Y.replace("%d", J) : Y(J, c, E.l, b);
                         break
                     }
                 }
                 if (c) return h;
                 var _ = b ? y.future : y.past;
@@ -4075,15 +4075,15 @@
                     f = s();
                 return this.format(i) === f.format(i)
             }
         }
     })
 })(zg);
 const Vg = vi,
-    Tg = Ce({
+    Gg = Ce({
         __name: "RoomsItem",
         props: {
             roomData: {
                 type: Object,
                 default: () => ({})
             },
             isSelectedRoom: {
@@ -4105,75 +4105,75 @@
                 const f = tt("VDropdown");
                 return (r = e.roomData) != null && r.id ? (j(), U("div", {
                     key: 0,
                     class: L([s.$style["ops-rooms-item"], {
                         [s.$style["ops-rooms-item__selected"]]: e.isSelectedRoom
                     }]),
                     onClick: i[0] || (i[0] = c => s.$emit("select-room", e.roomData))
-                }, [F("div", {
+                }, [P("div", {
                     class: L([s.$style["ops-rooms-item__content"], s.$style.content])
-                }, [F("div", {
+                }, [P("div", {
                     class: L(s.$style.content__info)
                 }, [se(f, {
                     theme: "ops-room-item__name",
                     triggers: ["hover"],
                     placement: "bottom-start",
                     distance: 6
                 }, {
                     popper: Ne(() => {
                         var c;
-                        return [F("h2", {
+                        return [P("h2", {
                             class: L(s.$style.title)
-                        }, Te((c = e.roomData) == null ? void 0 : c.name), 3)]
+                        }, Ge((c = e.roomData) == null ? void 0 : c.name), 3)]
                     }),
                     default: Ne(() => {
                         var c;
-                        return [F("h2", {
+                        return [P("h2", {
                             class: L(s.$style.title)
-                        }, Te((c = e.roomData) == null ? void 0 : c.name), 3)]
+                        }, Ge((c = e.roomData) == null ? void 0 : c.name), 3)]
                     }),
                     _: 1
                 }), e.roomData.last_message ? (j(), U("p", {
                     key: 0,
                     class: L(s.$style["content__last-message"])
-                }, Te(e.roomData.last_message.content), 3)) : me("", !0)], 2), F("div", {
+                }, Ge(e.roomData.last_message.content), 3)) : me("", !0)], 2), P("div", {
                     class: L([s.$style["ops-rooms-item__action"], s.$style.action])
                 }, [(l = (a = e.roomData) == null ? void 0 : a.last_message) != null && l.timestamp ? (j(), U("p", {
                     key: 0,
                     class: L(s.$style.action__time)
-                }, Te(ae(n)), 3)) : me("", !0), se(Ao, {
+                }, Ge(ae(n)), 3)) : me("", !0), se(Ao, {
                     name: "ops-slide-left"
                 }, {
                     default: Ne(() => {
                         var c;
                         return [(c = e.roomData) != null && c.unread_messages ? (j(), U("div", {
                             key: 0,
                             class: L(s.$style["ops-rooms-item__unread-message"])
-                        }, [F("span", null, Te(ae(o)), 1)], 2)) : me("", !0)]
+                        }, [P("span", null, Ge(ae(o)), 1)], 2)) : me("", !0)]
                     }),
                     _: 1
                 })], 2)], 2)], 2)) : me("", !0)
             }
         }
     }),
-    Gg = "_ops-rooms-item_qrhoy_1",
+    Tg = "_ops-rooms-item_qrhoy_1",
     jg = "_ops-rooms-item__selected_qrhoy_4",
     kg = "_content_qrhoy_7",
     Dg = "_content__info_qrhoy_10",
     Rg = "_content__info_qrhoy_10",
     xg = "_title_qrhoy_13",
     Xg = "_content__last-message_qrhoy_16",
     Yg = "_action_qrhoy_19",
     Eg = "_action__time_qrhoy_22",
     Hg = "_action__time_qrhoy_22",
     Og = "_ops-rooms-item__unread-message_qrhoy_25",
     Lg = "_scaleDown_qrhoy_1",
     Ug = {
         "ops-rooms-item": "_ops-rooms-item_qrhoy_1",
-        opsRoomsItem: Gg,
+        opsRoomsItem: Tg,
         "ops-rooms-item__selected": "_ops-rooms-item__selected_qrhoy_4",
         opsRoomsItemSelected: jg,
         content: kg,
         content__info: Dg,
         contentInfo: Rg,
         title: xg,
         "content__last-message": "_content__last-message_qrhoy_16",
@@ -4184,26 +4184,26 @@
         "ops-rooms-item__unread-message": "_ops-rooms-item__unread-message_qrhoy_25",
         opsRoomsItemUnreadMessage: Og,
         scaleDown: Lg
     };
 const Jg = {
         $style: Ug
     },
-    Kg = Ye(Tg, [
+    Kg = Ye(Gg, [
         ["__cssModules", Jg]
     ]),
-    Pg = "_rooms-empty_1pd70_1",
-    Fg = "_emptyRooms_1pd70_1",
+    Fg = "_rooms-empty_1pd70_1",
+    Pg = "_emptyRooms_1pd70_1",
     $g = {
         "rooms-empty": "_rooms-empty_1pd70_1",
-        roomsEmpty: Pg,
-        emptyRooms: Fg
+        roomsEmpty: Fg,
+        emptyRooms: Pg
     },
     Qg = {},
-    qg = F("p", null, "There aren`t any rooms", -1),
+    qg = P("p", null, "There aren`t any rooms", -1),
     e1 = [qg];
 
 function t1(e, t) {
     return j(), U("div", {
         class: L(e.$style["rooms-empty"])
     }, e1, 2)
 }
@@ -4350,37 +4350,37 @@
             state: _
         } = n, R = _ ? _() : {};
         this.$patch(A => {
             Xt(A, R)
         })
     } : Nl;
 
-    function G() {
+    function T() {
         f.stop(), u = [], d = [], o._s.delete(e)
     }
 
     function N(Y, _) {
         return function() {
             Ms(o);
             const R = Array.from(arguments),
                 A = [],
                 K = [];
 
-            function T(S) {
+            function G(S) {
                 A.push(S)
             }
 
             function z(S) {
                 K.push(S)
             }
             wn(d, {
                 args: R,
                 name: Y,
                 store: E,
-                after: T,
+                after: G,
                 onError: z
             });
             let M;
             try {
                 M = _.apply(this && this.$id === e ? this : E, R)
             } catch (S) {
                 throw wn(K, S), S
@@ -4401,15 +4401,15 @@
                             storeId: e,
                             type: no.direct,
                             events: m
                         }, K)
                     }, Xt({}, a, _)));
                 return R
             },
-            $dispose: G
+            $dispose: T
         },
         E = yo(v);
     o._s.set(e, E);
     const J = o._e.run(() => (f = Na(), f.run(() => t())));
     for (const Y in J) {
         const _ = J[Y];
         if (Be(_) && !a1(_) || Ut(_)) i || (p && r1(_) && (Be(_) ? _.value = p[Y] : _i(_, p[Y])), o.state.value[e][Y] = _);
@@ -4455,22 +4455,24 @@
             setUser: o => {
                 e.value = o
             }
         }
     }),
     c1 = e => {
         const t = document.querySelector(e);
-        t.scrollTop = t.scrollHeight
+        t.scrollTop = t == null ? void 0 : t.scrollHeight
     },
     u1 = e => {
-        const t = document.querySelector(e),
-            n = t.scrollHeight;
-        new ResizeObserver(() => {
-            t.scrollTop = t.scrollHeight - n
-        }).observe(t)
+        const t = document.querySelector(e);
+        if (t) {
+            const n = t.scrollHeight;
+            new ResizeObserver(() => {
+                t.scrollTop = t.scrollHeight - n
+            }).observe(t)
+        }
     },
     d1 = e => {
         const t = document.querySelector(e),
             n = document.querySelectorAll(".vue-recycle-scroller__item-view:last-child");
         return t ? Math.abs(t.scrollHeight - t.scrollTop - t.clientHeight) <= n[0].clientHeight : !1
     };
 
@@ -4482,22 +4484,22 @@
 const {
     toString: g1
 } = Object.prototype, {
     getPrototypeOf: pf
 } = Object, Zs = (e => t => {
     const n = g1.call(t);
     return e[n] || (e[n] = n.slice(8, -1).toLowerCase())
-})(Object.create(null)), Gt = e => (e = e.toLowerCase(), t => Zs(t) === e), Ws = e => t => typeof t === e, {
+})(Object.create(null)), Tt = e => (e = e.toLowerCase(), t => Zs(t) === e), Ws = e => t => typeof t === e, {
     isArray: Un
 } = Array, mo = Ws("undefined");
 
 function p1(e) {
     return e !== null && !mo(e) && e.constructor !== null && !mo(e.constructor) && Bt(e.constructor.isBuffer) && e.constructor.isBuffer(e)
 }
-const Sl = Gt("ArrayBuffer");
+const Sl = Tt("ArrayBuffer");
 
 function m1(e) {
     let t;
     return typeof ArrayBuffer < "u" && ArrayBuffer.isView ? t = ArrayBuffer.isView(e) : t = e && e.buffer && Sl(e.buffer), t
 }
 const I1 = Ws("string"),
     Bt = Ws("function"),
@@ -4505,24 +4507,24 @@
     mf = e => e !== null && typeof e == "object",
     h1 = e => e === !0 || e === !1,
     Oo = e => {
         if (Zs(e) !== "object") return !1;
         const t = pf(e);
         return (t === null || t === Object.prototype || Object.getPrototypeOf(t) === null) && !(Symbol.toStringTag in e) && !(Symbol.iterator in e)
     },
-    b1 = Gt("Date"),
-    C1 = Gt("File"),
-    y1 = Gt("Blob"),
-    A1 = Gt("FileList"),
+    b1 = Tt("Date"),
+    C1 = Tt("File"),
+    y1 = Tt("Blob"),
+    A1 = Tt("FileList"),
     v1 = e => mf(e) && Bt(e.pipe),
     w1 = e => {
         let t;
         return e && (typeof FormData == "function" && e instanceof FormData || Bt(e.append) && ((t = Zs(e)) === "formdata" || t === "object" && Bt(e.toString) && e.toString() === "[object FormData]"))
     },
-    _1 = Gt("URLSearchParams"),
+    _1 = Tt("URLSearchParams"),
     N1 = e => e.trim ? e.trim() : e.replace(/^[\s\uFEFF\xA0]+|[\s\uFEFF\xA0]+$/g, "");
 
 function vo(e, t, {
     allOwnKeys: n = !1
 } = {}) {
     if (e === null || typeof e > "u") return;
     let o, s;
@@ -4542,20 +4544,20 @@
     let o = n.length,
         s;
     for (; o-- > 0;)
         if (s = n[o], t === s.toLowerCase()) return s;
     return null
 }
 const Vl = (() => typeof globalThis < "u" ? globalThis : typeof self < "u" ? self : typeof window < "u" ? window : global)(),
-    Tl = e => !mo(e) && e !== Vl;
+    Gl = e => !mo(e) && e !== Vl;
 
 function Ni() {
     const {
         caseless: e
-    } = Tl(this) && this || {}, t = {}, n = (o, s) => {
+    } = Gl(this) && this || {}, t = {}, n = (o, s) => {
         const i = e && zl(t, s) || s;
         Oo(t[i]) && Oo(o) ? t[i] = Ni(t[i], o) : Oo(o) ? t[i] = Ni({}, o) : Un(o) ? t[i] = o.slice() : t[i] = o
     };
     for (let o = 0, s = arguments.length; o < s; o++) arguments[o] && vo(arguments[o], n);
     return t
 }
 const M1 = (e, t, n, {
@@ -4592,47 +4594,47 @@
         let t = e.length;
         if (!Bl(t)) return null;
         const n = new Array(t);
         for (; t-- > 0;) n[t] = e[t];
         return n
     },
     V1 = (e => t => e && t instanceof e)(typeof Uint8Array < "u" && pf(Uint8Array)),
-    T1 = (e, t) => {
+    G1 = (e, t) => {
         const o = (e && e[Symbol.iterator]).call(e);
         let s;
         for (;
             (s = o.next()) && !s.done;) {
             const i = s.value;
             t.call(e, i[0], i[1])
         }
     },
-    G1 = (e, t) => {
+    T1 = (e, t) => {
         let n;
         const o = [];
         for (;
             (n = e.exec(t)) !== null;) o.push(n);
         return o
     },
-    j1 = Gt("HTMLFormElement"),
+    j1 = Tt("HTMLFormElement"),
     k1 = e => e.toLowerCase().replace(/[-_\s]([a-z\d])(\w*)/g, function(n, o, s) {
         return o.toUpperCase() + s
     }),
     _r = (({
         hasOwnProperty: e
     }) => (t, n) => e.call(t, n))(Object.prototype),
-    D1 = Gt("RegExp"),
-    Gl = (e, t) => {
+    D1 = Tt("RegExp"),
+    Tl = (e, t) => {
         const n = Object.getOwnPropertyDescriptors(e),
             o = {};
         vo(n, (s, i) => {
             t(s, i, e) !== !1 && (o[i] = s)
         }), Object.defineProperties(e, o)
     },
     R1 = e => {
-        Gl(e, (t, n) => {
+        Tl(e, (t, n) => {
             if (Bt(e) && ["arguments", "caller", "callee"].indexOf(n) !== -1) return !1;
             const o = e[n];
             if (Bt(o)) {
                 if (t.enumerable = !1, "writable" in t) {
                     t.writable = !1;
                     return
                 }
@@ -4649,20 +4651,20 @@
                     n[i] = !0
                 })
             };
         return Un(e) ? o(e) : o(String(e).split(t)), n
     },
     X1 = () => {},
     Y1 = (e, t) => (e = +e, Number.isFinite(e) ? e : t),
-    Fs = "abcdefghijklmnopqrstuvwxyz",
+    Ps = "abcdefghijklmnopqrstuvwxyz",
     Nr = "0123456789",
     jl = {
         DIGIT: Nr,
-        ALPHA: Fs,
-        ALPHA_DIGIT: Fs + Fs.toUpperCase() + Nr
+        ALPHA: Ps,
+        ALPHA_DIGIT: Ps + Ps.toUpperCase() + Nr
     },
     E1 = (e = 16, t = jl.ALPHA_DIGIT) => {
         let n = "";
         const {
             length: o
         } = t;
         for (; e--;) n += t[Math.random() * o | 0];
@@ -4715,31 +4717,31 @@
         merge: Ni,
         extend: M1,
         trim: N1,
         stripBOM: Z1,
         inherits: W1,
         toFlatObject: S1,
         kindOf: Zs,
-        kindOfTest: Gt,
+        kindOfTest: Tt,
         endsWith: B1,
         toArray: z1,
-        forEachEntry: T1,
-        matchAll: G1,
+        forEachEntry: G1,
+        matchAll: T1,
         isHTMLForm: j1,
         hasOwnProperty: _r,
         hasOwnProp: _r,
-        reduceDescriptors: Gl,
+        reduceDescriptors: Tl,
         freezeMethods: R1,
         toObjectSet: x1,
         toCamelCase: k1,
         noop: X1,
         toFiniteNumber: Y1,
         findKey: zl,
         global: Vl,
-        isContextDefined: Tl,
+        isContextDefined: Gl,
         ALPHABET: jl,
         generateString: E1,
         isSpecCompliantForm: H1,
         toJSONObject: O1
     };
 
 function pe(e, t, n, o, s) {
@@ -4841,16 +4843,16 @@
             convertValue: l,
             isVisitable: Mi
         });
 
     function m(p, h) {
         if (!w.isUndefined(p)) {
             if (u.indexOf(p) !== -1) throw Error("Circular reference detected in " + h.join("."));
-            u.push(p), w.forEach(p, function(y, G) {
-                (!(w.isUndefined(y) || y === null) && s.call(t, y, w.isString(G) ? G.trim() : G, h, d)) === !0 && m(y, h ? h.concat(G) : [G])
+            u.push(p), w.forEach(p, function(y, T) {
+                (!(w.isUndefined(y) || y === null) && s.call(t, y, w.isString(T) ? T.trim() : T, h, d)) === !0 && m(y, h ? h.concat(T) : [T])
             }), u.pop()
         }
     }
     if (!w.isObject(e)) throw new TypeError("data must be an object");
     return m(e), t
 }
 
@@ -4896,15 +4898,15 @@
     let i;
     if (s ? i = s(t, n) : i = w.isURLSearchParams(t) ? t.toString() : new If(t, n).toString(o), i) {
         const f = e.indexOf("#");
         f !== -1 && (e = e.slice(0, f)), e += (e.indexOf("?") === -1 ? "?" : "&") + i
     }
     return e
 }
-class P1 {
+class F1 {
     constructor() {
         this.handlers = []
     }
     use(t, n, o) {
         return this.handlers.push({
             fulfilled: t,
             rejected: n,
@@ -4920,32 +4922,32 @@
     }
     forEach(t) {
         w.forEach(this.handlers, function(o) {
             o !== null && t(o)
         })
     }
 }
-const Wr = P1,
+const Wr = F1,
     Yl = {
         silentJSONParsing: !0,
         forcedJSONParsing: !0,
         clarifyTimeoutError: !1
     },
-    F1 = typeof URLSearchParams < "u" ? URLSearchParams : If,
+    P1 = typeof URLSearchParams < "u" ? URLSearchParams : If,
     $1 = typeof FormData < "u" ? FormData : null,
     Q1 = typeof Blob < "u" ? Blob : null,
     q1 = (() => {
         let e;
         return typeof navigator < "u" && ((e = navigator.product) === "ReactNative" || e === "NativeScript" || e === "NS") ? !1 : typeof window < "u" && typeof document < "u"
     })(),
     ep = (() => typeof WorkerGlobalScope < "u" && self instanceof WorkerGlobalScope && typeof self.importScripts == "function")(),
     bt = {
         isBrowser: !0,
         classes: {
-            URLSearchParams: F1,
+            URLSearchParams: P1,
             FormData: $1,
             Blob: Q1
         },
         isStandardBrowserEnv: q1,
         isStandardBrowserWebWorkerEnv: ep,
         protocols: ["http", "https", "file", "blob", "url", "data"]
     };
@@ -5068,15 +5070,15 @@
         return e && e.split(`
 `).forEach(function(f) {
             s = f.indexOf(":"), n = f.substring(0, s).trim().toLowerCase(), o = f.substring(s + 1).trim(), !(!n || t[n] && fp[n]) && (n === "set-cookie" ? t[n] ? t[n].push(o) : t[n] = [o] : t[n] = t[n] ? t[n] + ", " + o : o)
         }), t
     },
     Sr = Symbol("internals");
 
-function Fn(e) {
+function Pn(e) {
     return e && String(e).trim().toLowerCase()
 }
 
 function Lo(e) {
     return e === !1 || e == null ? e : w.isArray(e) ? e.map(Lo) : String(e)
 }
 
@@ -5116,48 +5118,48 @@
     constructor(t) {
         t && this.set(t)
     }
     set(t, n, o) {
         const s = this;
 
         function i(r, a, l) {
-            const c = Fn(a);
+            const c = Pn(a);
             if (!c) throw new Error("header name must be a non-empty string");
             const u = w.findKey(s, c);
             (!u || s[u] === void 0 || l === !0 || l === void 0 && s[u] !== !1) && (s[u || a] = Lo(r))
         }
         const f = (r, a) => w.forEach(r, (l, c) => i(l, c, a));
         return w.isPlainObject(t) || t instanceof this.constructor ? f(t, n) : w.isString(t) && (t = t.trim()) && !lp(t) ? f(rp(t), n) : t != null && i(n, t, o), this
     }
     get(t, n) {
-        if (t = Fn(t), t) {
+        if (t = Pn(t), t) {
             const o = w.findKey(this, t);
             if (o) {
                 const s = this[o];
                 if (!n) return s;
                 if (n === !0) return ap(s);
                 if (w.isFunction(n)) return n.call(this, s, o);
                 if (w.isRegExp(n)) return n.exec(s);
                 throw new TypeError("parser must be boolean|regexp|function")
             }
         }
     }
     has(t, n) {
-        if (t = Fn(t), t) {
+        if (t = Pn(t), t) {
             const o = w.findKey(this, t);
             return !!(o && this[o] !== void 0 && (!n || $s(this, this[o], o, n)))
         }
         return !1
     }
     delete(t, n) {
         const o = this;
         let s = !1;
 
         function i(f) {
-            if (f = Fn(f), f) {
+            if (f = Pn(f), f) {
                 const r = w.findKey(o, f);
                 r && (!n || $s(o, o[r], r, n)) && (delete o[r], s = !0)
             }
         }
         return w.isArray(t) ? t.forEach(i) : i(t), s
     }
     clear(t) {
@@ -5211,15 +5213,15 @@
     static accessor(t) {
         const o = (this[Sr] = this[Sr] = {
                 accessors: {}
             }).accessors,
             s = this.prototype;
 
         function i(f) {
-            const r = Fn(f);
+            const r = Pn(f);
             o[r] || (up(s, f), o[r] = !0)
         }
         return w.isArray(t) ? t.forEach(i) : i(t), this
     }
 }
 zs.accessor(["Content-Type", "Content-Length", "Accept", "Accept-Encoding", "User-Agent", "Authorization"]);
 w.freezeMethods(zs.prototype);
@@ -5541,22 +5543,22 @@
 const Ll = "1.3.6",
     bf = {};
 ["object", "boolean", "number", "function", "string", "symbol"].forEach((e, t) => {
     bf[e] = function(o) {
         return typeof o === e || "a" + (t < 1 ? "n " : " ") + e
     }
 });
-const Tr = {};
+const Gr = {};
 bf.transitional = function(t, n, o) {
     function s(i, f) {
         return "[Axios v" + Ll + "] Transitional option '" + i + "'" + f + (o ? ". " + o : "")
     }
     return (i, f, r) => {
         if (t === !1) throw new pe(s(f, " has been removed" + (n ? " in " + n : "")), pe.ERR_DEPRECATED);
-        return n && !Tr[f] && (Tr[f] = !0, console.warn(s(f, " has been deprecated since v" + n + " and will be removed in the near future"))), t ? t(i, f, r) : !0
+        return n && !Gr[f] && (Gr[f] = !0, console.warn(s(f, " has been deprecated since v" + n + " and will be removed in the near future"))), t ? t(i, f, r) : !0
     }
 };
 
 function vp(e, t, n) {
     if (typeof e != "object") throw new pe("options must be an object", pe.ERR_BAD_OPTION_VALUE);
     const o = Object.keys(e);
     let s = o.length;
@@ -5810,36 +5812,36 @@
         allOwnKeys: !0
     }), w.extend(n, t, null, {
         allOwnKeys: !0
     }), n.create = function(s) {
         return Ul(Vn(e, s))
     }, n
 }
-const Ge = Ul(hf);
-Ge.Axios = Jo;
-Ge.CanceledError = wo;
-Ge.CancelToken = wp;
-Ge.isCancel = Hl;
-Ge.VERSION = Ll;
-Ge.toFormData = Ss;
-Ge.AxiosError = pe;
-Ge.Cancel = Ge.CanceledError;
-Ge.all = function(t) {
+const Te = Ul(hf);
+Te.Axios = Jo;
+Te.CanceledError = wo;
+Te.CancelToken = wp;
+Te.isCancel = Hl;
+Te.VERSION = Ll;
+Te.toFormData = Ss;
+Te.AxiosError = pe;
+Te.Cancel = Te.CanceledError;
+Te.all = function(t) {
     return Promise.all(t)
 };
-Ge.spread = _p;
-Ge.isAxiosError = Np;
-Ge.mergeConfig = Vn;
-Ge.AxiosHeaders = Mt;
-Ge.formToJSON = e => El(w.isHTMLForm(e) ? new FormData(e) : e);
-Ge.HttpStatusCode = Mp;
-Ge.default = Ge;
-const Zp = Ge,
+Te.spread = _p;
+Te.isAxiosError = Np;
+Te.mergeConfig = Vn;
+Te.AxiosHeaders = Mt;
+Te.formToJSON = e => El(w.isHTMLForm(e) ? new FormData(e) : e);
+Te.HttpStatusCode = Mp;
+Te.default = Te;
+const Zp = Te,
     Jl = () => window.api_token,
-    Kl = () => window.location.hostname,
+    Kl = () => window.location.host,
     Wp = e => {
         var t, n;
         if (Array.isArray(e)) {
             const s = (n = (t = Ln().getUser) == null ? void 0 : t.person) == null ? void 0 : n.id;
             return e.filter(f => f !== s).length
         }
         return 0
@@ -5926,46 +5928,46 @@
             return t
         } catch (t) {
             throw new Error(t)
         }
     }
 }
 const _o = new Vp,
-    Gr = {
+    Tr = {
         timer: 0
     },
-    Tp = e => {
+    Gp = e => {
         ie.peopleOnline.value = e.length - 1
     },
-    Gp = async e => {
+    Tp = async e => {
         var o;
         const t = Ln();
         !((e == null ? void 0 : e.author.id) === t.getUser.person.id) && !e.is_read && ie.unreadMessages.value.push(e.id), e.conversation === ((o = ie.selectedRoom.value) == null ? void 0 : o.id) && ie.messages.value.push(e), setTimeout(() => {
             d1(".vue-recycle-scroller") && c1(".vue-recycle-scroller")
         }, 500)
     }, jp = async e => {
         const t = ie.rooms.value.findIndex(n => n.id === e.id);
         t.toString() ? ie.rooms.value[t] = e : ie.rooms.value = await _o.fetchConversations()
     }, kp = e => {
         const t = ie.messages.value.findIndex(n => n.id === e.id);
-        ie.messages.value[t] = e, clearTimeout(Gr.timer), Gr.timer = setTimeout(() => {
+        ie.messages.value[t] = e, clearTimeout(Tr.timer), Tr.timer = setTimeout(() => {
             ie.unreadMessages.value = []
         }, 3e3)
     }, Dp = e => {
         ie.messages.value = e.messages, ie.hasMoreMessages.value = e.has_more, ie.loadingOptions.value.loading = !1, ie.loadingOptions.value.isLoaded = !0
     }, Rp = e => {
         switch (!0) {
             case qe.PEOPLE_ONLINE === e.type:
-                Tp(e.message);
+                Gp(e.message);
                 break;
             case qe.RECENT_MESSAGES === e.type:
                 Dp(e);
                 break;
             case qe.CHAT_MESSAGES === e.type:
-                Gp(e.message);
+                Tp(e.message);
                 break;
             case (qe.TYPING === e.type && e.typing):
                 ie.userTyping.value = e;
                 break;
             case (qe.TYPING === e.type && !e.typing):
                 ie.userTyping.value = {};
                 break;
@@ -6080,30 +6082,30 @@
     },
     Lp = Ye(Xp, [
         ["__cssModules", Op]
     ]),
     Up = "_loader_1lxm6_1",
     Jp = "_rotate_1lxm6_1",
     Kp = "_prixClipFix_1lxm6_1",
-    Pp = {
+    Fp = {
         loader: Up,
         rotate: Jp,
         prixClipFix: Kp
     },
-    Fp = {};
+    Pp = {};
 
 function $p(e, t) {
     return j(), U("div", {
         class: L(e.$style.loader)
     }, null, 2)
 }
 const Qp = {
-        $style: Pp
+        $style: Fp
     },
-    Pl = Ye(Fp, [
+    Fl = Ye(Pp, [
         ["render", $p],
         ["__cssModules", Qp]
     ]),
     qp = "data:application/octet-stream;base64,PHRlbXBsYXRlPgogIDxkaXYgdi1pZj0iZ2V0VXNlck1ldGEiIDpjbGFzcz0iJHN0eWxlWydjaGF0LWFwcCddIj4KICAgIDxSb29tc0NvbnRhaW5lciAvPgogIDwvZGl2Pgo8L3RlbXBsYXRlPgoKPHNjcmlwdCBsYW5nPSJ0cyIgc2V0dXA+CmltcG9ydCBSb29tc0NvbnRhaW5lciBmcm9tICJAL2NvbXBvbmVudHMvcm9vbXMvUm9vbXNDb250YWluZXIudnVlIjsKaW1wb3J0IHsgY29tcHV0ZWQsIG9uTW91bnRlZCB9IGZyb20gInZ1ZSI7CmltcG9ydCBjaGF0U2VydmljZSBmcm9tICJAL3NlcnZpY2VzL2NoYXQvY2hhdCI7CmltcG9ydCB7IHVzZVVzZXJTdG9yZSB9IGZyb20gIkAvc3RvcmUvdXNlVXNlclN0b3JlIjsKCmNvbnN0IHVzZXJTdG9yZSA9IHVzZVVzZXJTdG9yZSgpOwpjb25zdCBnZXRVc2VyTWV0YSA9IGNvbXB1dGVkKCgpID0+IHVzZXJTdG9yZS5nZXRVc2VyKTsKCm9uTW91bnRlZChhc3luYyAoKSA9PiB7CiAgY29uc3QgZGF0YSA9IGF3YWl0IGNoYXRTZXJ2aWNlLmZldGNoQ2hhdE1ldGEoKTsKICB1c2VyU3RvcmUuc2V0VXNlcihkYXRhKTsKfSk7Cjwvc2NyaXB0Pgo8c3R5bGUgbGFuZz0ic2NzcyIgbW9kdWxlPgouY2hhdC1hcHAgewogIEBhcHBseSBzaGFkb3ctWzBfMnB4XzhweF8wcHhfcmdiYSg5OSw5OSw5OSwwLjIpXSByb3VuZGVkLW1kIGJveC1ib3JkZXIgbXktNDsKfQo8L3N0eWxlPgo=",
     e0 = "data:application/octet-stream;base64,CmZyb20gLiBpbXBvcnQgX3ZlcnNpb24KX192ZXJzaW9uX18gPSBfdmVyc2lvbi5nZXRfdmVyc2lvbnMoKVsndmVyc2lvbiddCg==",
     t0 = "/static/chat/_version.py",
     n0 = "data:video/mp2t;base64,aW1wb3J0IGF4aW9zIGZyb20gImF4aW9zIjsKaW1wb3J0IHsKICBnZXRDaGF0QXBpVG9rZW4sCiAgZ2V0RG9tYWluTmFtZSwKICBnZXRUcmFuc2ZlclByb3RvY29sLAp9IGZyb20gIkAvaGVscGVycy9nZW5lcmFsIjsKCmV4cG9ydCBjb25zdCBheGlvc0Jhc2VDb25maWcgPSBheGlvcy5jcmVhdGUoewogIGJhc2VVUkw6IGAke2dldFRyYW5zZmVyUHJvdG9jb2woKX0ke2dldERvbWFpbk5hbWUoKX1gLAogIGhlYWRlcnM6IHsKICAgICJDb250ZW50LVR5cGUiOiAiYXBwbGljYXRpb24vanNvbiIsCiAgICBBdXRob3JpemF0aW9uOiBgQmVhcmVyICR7Z2V0Q2hhdEFwaVRva2VuKCl9YCwKICB9LAp9KTsKCmF4aW9zQmFzZUNvbmZpZy5pbnRlcmNlcHRvcnMucmVxdWVzdC51c2UoCiAgZnVuY3Rpb24gKGNvbmZpZykgewogICAgLy8gRG8gc29tZXRoaW5nIGJlZm9yZSByZXF1ZXN0IGlzIHNlbnQKICAgIHJldHVybiBjb25maWc7CiAgfSwKICBmdW5jdGlvbiAoZXJyb3IpIHsKICAgIC8vIERvIHNvbWV0aGluZyB3aXRoIHJlcXVlc3QgZXJyb3IKICAgIHJldHVybiBQcm9taXNlLnJlamVjdChlcnJvcik7CiAgfQopOwoKLy8gQWRkIGEgcmVzcG9uc2UgaW50ZXJjZXB0b3IKYXhpb3NCYXNlQ29uZmlnLmludGVyY2VwdG9ycy5yZXNwb25zZS51c2UoCiAgZnVuY3Rpb24gKHJlc3BvbnNlKSB7CiAgICAvLyBBbnkgc3RhdHVzIGNvZGUgdGhhdCBsaWUgd2l0aGluIHRoZSByYW5nZSBvZiAyeHggY2F1c2UgdGhpcyBmdW5jdGlvbiB0byB0cmlnZ2VyCiAgICAvLyBEbyBzb21ldGhpbmcgd2l0aCByZXNwb25zZSBkYXRhCiAgICByZXR1cm4gcmVzcG9uc2U7CiAgfSwKICBmdW5jdGlvbiAoZXJyb3IpIHsKICAgIC8vIEFueSBzdGF0dXMgY29kZXMgdGhhdCBmYWxscyBvdXRzaWRlIHRoZSByYW5nZSBvZiAyeHggY2F1c2UgdGhpcyBmdW5jdGlvbiB0byB0cmlnZ2VyCiAgICAvLyBEbyBzb21ldGhpbmcgd2l0aCByZXNwb25zZSBlcnJvcgogICAgcmV0dXJuIFByb21pc2UucmVqZWN0KGVycm9yKTsKICB9Cik7Cg==",
@@ -6133,32 +6135,32 @@
     M0 = "/static/chat/RoomMessageWrapper.vue",
     Z0 = "data:application/octet-stream;base64,PHRlbXBsYXRlPgogIDxkaXYgOmNsYXNzPSIkc3R5bGVbJ3Jvb21zLWVtcHR5J10iPgogICAgPHAgOmNsYXNzPSIkc3R5bGVbJ3Jvb21zLWVtcHR5X190ZXh0J10iPnt7IHRleHQgfX08L3A+CiAgPC9kaXY+CjwvdGVtcGxhdGU+Cgo8c2NyaXB0IGxhbmc9InRzIiBzZXR1cD4KaW1wb3J0IHsgUHJvcFR5cGUgfSBmcm9tICJ2dWUiOwoKZGVmaW5lUHJvcHMoewogIHRleHQ6IHsKICAgIHR5cGU6IFN0cmluZyBhcyBQcm9wVHlwZTxzdHJpbmc+LAogICAgZGVmYXVsdDogIiIsCiAgfSwKfSk7Cjwvc2NyaXB0PgoKPHN0eWxlIGxhbmc9InNjc3MiIG1vZHVsZT4KLnJvb21zLWVtcHR5IHsKICBAYXBwbHkgYmctY29uZmV0dGkgcm91bmRlZC1tZCBweS0yIHB4LTQgdy1maXQgYWJzb2x1dGUgbGVmdC1bNDAlXSB0b3AtMS8yOwogIGFuaW1hdGlvbjogZW1wdHlSb29tcyAwLjRzOwoKICAmX190ZXh0IHsKICAgIEBhcHBseSB0ZXh0LWNlbnRlciB0ZXh0LWdyZXkta2FzaG1pcjsKICB9Cn0KCkBrZXlmcmFtZXMgZW1wdHlSb29tcyB7CiAgMCUgewogICAgdHJhbnNmb3JtOiBzY2FsZSgwLjk1KTsKICB9CiAgNTAlIHsKICAgIHRyYW5zZm9ybTogc2NhbGUoMS4xKTsKICB9CiAgNzUlIHsKICAgIHRyYW5zZm9ybTogc2NhbGUoMS4wNSk7CiAgfQogIDkwJSB7CiAgICB0cmFuc2Zvcm06IHNjYWxlKDEuMDcpOwogIH0KICAxMDAlIHsKICAgIHRyYW5zZm9ybTogc2NhbGUoMSk7CiAgfQp9Cjwvc3R5bGU+Cg==",
     W0 = "data:application/octet-stream;base64,PHRlbXBsYXRlPgogIDwhLS0gICAgVE9ETzogd2lsbCBjaGFuZ2Ugd2hlbiBJIGNhbiBnZXQgYW4gYXBpIGRhdGEtLT4KICA8ZGl2IGNsYXNzPSJvcHMtcm9vbS1yZWFjdGlvbnMtd3JhcHBlciI+CiAgICA8ZGl2CiAgICAgIHYtaWY9Im1lc3NhZ2VEYXRhPy5tZXNzYWdlUmVhY3Rpb25zIgogICAgICBjbGFzcz0ib3BzLXJvb20tcmVhY3Rpb25zLXdyYXBwZXJfX3JlYWN0aW9ucyIKICAgID4KICAgICAgPGRpdgogICAgICAgIHYtZm9yPSIocmVhY3Rpb24sIGluZGV4KSBpbiBtZXNzYWdlRGF0YT8ubWVzc2FnZVJlYWN0aW9ucyIKICAgICAgICA6a2V5PSJpbmRleCIKICAgICAgICBjbGFzcz0ib3BzLXJvb20tcmVhY3Rpb25zLXdyYXBwZXJfX3JlYWN0aW9uIgogICAgICAgIEBjbGljaz0idm90ZVJlYWN0aW9uKHJlYWN0aW9uKSIKICAgICAgPgogICAgICAgIDxzcGFuPnt7IHJlYWN0aW9uLnJlYWN0aW9uIH19PC9zcGFuPgogICAgICAgIDxzcGFuPnt7IHJlYWN0aW9uLmNvdW50IH19PC9zcGFuPgogICAgICA8L2Rpdj4KICAgIDwvZGl2PgogICAgPHRyYW5zaXRpb24gbmFtZT0ib3BzLXNsaWRlLWxlZnQiPgogICAgICA8RW1vamlQaWNrZXIKICAgICAgICB2LXNob3c9ImlzRW1vamlWaXNpYmxlIgogICAgICAgIGlkPSJlbW9qaS1waWNrZXIiCiAgICAgICAgbmF0aXZlCiAgICAgICAgY2xhc3M9ImFic29sdXRlIHotMTAgbGVmdC1bNTAlXSB0b3AtWzUwJV0gdHJhbnNsYXRlLXgtWy01MCVdIHRyYW5zbGF0ZS15LVstNTAlXSIKICAgICAgICA6Y2xhc3M9InsKICAgICAgICAgICdsZWZ0LVsxMHJlbV0nOiAhbWVzc2FnZURhdGE/LmlzT3duLAogICAgICAgICAgJ3JpZ2h0LVsxMHJlbV0nOiBtZXNzYWdlRGF0YT8uaXNPd24sCiAgICAgICAgfSIKICAgICAgICBAc2VsZWN0PSJvblNlbGVjdEVtb2ppIgogICAgICAvPgogICAgPC90cmFuc2l0aW9uPgogIDwvZGl2Pgo8L3RlbXBsYXRlPgoKPHNjcmlwdCBsYW5nPSJ0cyIgc2V0dXA+CmltcG9ydCB7IElNZXNzYWdlLCBJTWVzc2FnZVJlYWN0aW9uIH0gZnJvbSAiQC90eXBlcy9yb29tL3Jvb20udHlwZXMiOwppbXBvcnQgeyBvbk1vdW50ZWQsIFByb3BUeXBlIH0gZnJvbSAidnVlIjsKaW1wb3J0IHsgdXNlVXNlclN0b3JlIH0gZnJvbSAiQC9zdG9yZS91c2VVc2VyU3RvcmUiOwppbXBvcnQgRW1vamlQaWNrZXIgZnJvbSAidnVlMy1lbW9qaS1waWNrZXIiOwppbXBvcnQgInZ1ZTMtZW1vamktcGlja2VyL2NzcyI7CmltcG9ydCB7IGdlbmVyYXRlSUQgfSBmcm9tICJAL2hlbHBlcnMvZ2VuZXJhbCI7Cgpjb25zdCB1c2VyU3RvcmUgPSB1c2VVc2VyU3RvcmUoKTsKCmNvbnN0IGVtaXQgPSBkZWZpbmVFbWl0czx7CiAgKGU6ICJjbG9zZS1lbW9qaSIpOiB2b2lkOwp9PigpOwoKY29uc3QgcHJvcHMgPSBkZWZpbmVQcm9wcyh7CiAgbWVzc2FnZURhdGE6IHsKICAgIHR5cGU6IE9iamVjdCBhcyBQcm9wVHlwZTxJTWVzc2FnZT4sCiAgICBkZWZhdWx0OiAoKSA9PiAoe30pLAogIH0sCiAgaXNFbW9qaVZpc2libGU6IHsKICAgIHR5cGU6IEJvb2xlYW4gYXMgUHJvcFR5cGU8Ym9vbGVhbj4sCiAgICBkZWZhdWx0OiBmYWxzZSwKICB9LAp9KTsKCmNvbnN0IG9uU2VsZWN0RW1vamkgPSAoZXZlbnQ6IGFueSkgPT4gewogIGNvbnN0IGZpbmRBZGRPbiA9IHByb3BzLm1lc3NhZ2VEYXRhPy5tZXNzYWdlUmVhY3Rpb25zLmZpbmQoCiAgICAoZWw6IElNZXNzYWdlUmVhY3Rpb24pID0+IGVsLnJlYWN0aW9uID09PSBldmVudC5pCiAgKTsKICAhZmluZEFkZE9uICYmCiAgICBwcm9wcy5tZXNzYWdlRGF0YT8ubWVzc2FnZVJlYWN0aW9ucy5wdXNoKHsKICAgICAgcmVhY3Rpb246IGV2ZW50LmksCiAgICAgIGNvdW50OiAxLAogICAgICB1c2VyX2lkOiB1c2VyU3RvcmUuZ2V0VXNlcj8udXNlcl9pZCwKICAgICAgcmVhY3Rpb25faWQ6IGdlbmVyYXRlSUQoKSwKICAgIH0pOwogIGVtaXQoImNsb3NlLWVtb2ppIik7Cn07Cgpjb25zdCB2b3RlUmVhY3Rpb24gPSAocmVhY3Rpb246IElNZXNzYWdlUmVhY3Rpb24pID0+IHsKICByZWFjdGlvbi51c2VyX2lkID09PSB1c2VyU3RvcmUuZ2V0VXNlcj8udXNlcl9pZAogICAgPyByZWFjdGlvbi5jb3VudC0tCiAgICA6IHJlYWN0aW9uLmNvdW50Kys7CgogIGlmICghcmVhY3Rpb24uY291bnQpIHsKICAgIGNvbnN0IGZpbmREZWxJbmRleCA9IHByb3BzLm1lc3NhZ2VEYXRhPy5tZXNzYWdlUmVhY3Rpb25zLmZpbmRJbmRleCgKICAgICAgKGVsOiBJTWVzc2FnZVJlYWN0aW9uKSA9PiBlbC5yZWFjdGlvbl9pZCA9PT0gcmVhY3Rpb24ucmVhY3Rpb25faWQKICAgICk7CiAgICBwcm9wcy5tZXNzYWdlRGF0YT8ubWVzc2FnZVJlYWN0aW9ucy5zcGxpY2UoZmluZERlbEluZGV4LCAxKTsKICB9Cn07Cgpvbk1vdW50ZWQoKCkgPT4gewogIGNvbnN0IGVtb2ppUGlja2VyID0gZG9jdW1lbnQuZ2V0RWxlbWVudEJ5SWQoImVtb2ppLXBpY2tlciIpIGFzIEhUTUxFbGVtZW50OwogIGNvbnN0IHJvb21Db250ZW50ID0gZG9jdW1lbnQuZ2V0RWxlbWVudEJ5SWQoInJvb20tbWVzc2FnZXMiKSBhcyBIVE1MRWxlbWVudDsKICByb29tQ29udGVudC5hcHBlbmRDaGlsZChlbW9qaVBpY2tlcik7Cn0pOwo8L3NjcmlwdD4KCjxzdHlsZSBsYW5nPSJzY3NzIj4KLm93bi1tZXNzYWdlIHsKICAub3BzLXJvb20tcmVhY3Rpb25zLXdyYXBwZXIgewogICAgQGFwcGx5IGZsZXgganVzdGlmeS1lbmQgI3shaW1wb3J0YW50fTsKICB9Cn0KCi5vcHMtcm9vbS1yZWFjdGlvbnMtd3JhcHBlciB7CiAgJl9fcmVhY3Rpb25zIHsKICAgIEBhcHBseSBpbmxpbmUtZmxleCBmbGV4LXdyYXAgaXRlbXMtY2VudGVyIGdhcC0xIG10LTEgcmVsYXRpdmU7CiAgfQoKICAmX19yZWFjdGlvbiB7CiAgICBAYXBwbHkgY3Vyc29yLXBvaW50ZXIgZmxleCBpdGVtcy1jZW50ZXIgZmxleC1ub3dyYXAgYmctY29uZmV0dGktMTAwIGJvcmRlciBib3JkZXItY29uZmV0dGkgcm91bmRlZC1tZCBweC0xOwoKICAgIHNwYW46bGFzdC1jaGlsZCB7CiAgICAgIEBhcHBseSB0ZXh0LWdyZXkta2FzaG1pciB0ZXh0LXhzIG1sLTE7CiAgICB9CiAgfQp9Cjwvc3R5bGU+Cg==",
     S0 = "data:application/octet-stream;base64,PHRlbXBsYXRlPgogIDxkaXY+QXVkaW88L2Rpdj4KPC90ZW1wbGF0ZT4KCjxzY3JpcHQgbGFuZz0idHMiIHNldHVwPjwvc2NyaXB0PgoKPHN0eWxlIHNjb3BlZD48L3N0eWxlPgo=",
     B0 = "data:application/octet-stream;base64,PHRlbXBsYXRlPgogIDxkaXY+RmlsZTwvZGl2Pgo8L3RlbXBsYXRlPgoKPHNjcmlwdCBsYW5nPSJ0cyIgc2V0dXA+PC9zY3JpcHQ+Cgo8c3R5bGUgc2NvcGVkPjwvc3R5bGU+Cg==",
     z0 = "data:application/octet-stream;base64,PHRlbXBsYXRlPgogIDxkaXY+UmVwbHk8L2Rpdj4KPC90ZW1wbGF0ZT4KCjxzY3JpcHQgbGFuZz0idHMiIHNldHVwPjwvc2NyaXB0PgoKPHN0eWxlIHNjb3BlZD48L3N0eWxlPgo=",
     V0 = "data:application/octet-stream;base64,PHRlbXBsYXRlPgogIDxkaXYgOmNsYXNzPSIkc3R5bGVbJ29wcy10ZXh0LW1lc3NhZ2UnXSI+CiAgICB7eyBtZXNzYWdlRGF0YT8uY29udGVudCB9fQogIDwvZGl2Pgo8L3RlbXBsYXRlPgoKPHNjcmlwdCBsYW5nPSJ0cyIgc2V0dXA+CmltcG9ydCB7IFByb3BUeXBlIH0gZnJvbSAidnVlIjsKaW1wb3J0IHsgSU1lc3NhZ2UgfSBmcm9tICJAL3R5cGVzL3Jvb20vcm9vbS50eXBlcyI7CgpkZWZpbmVQcm9wcyh7CiAgbWVzc2FnZURhdGE6IHsKICAgIHR5cGU6IE9iamVjdCBhcyBQcm9wVHlwZTxJTWVzc2FnZT4sCiAgICBkZWZhdWx0OiAoKSA9PiAoe30pLAogIH0sCn0pOwo8L3NjcmlwdD4KCjxzdHlsZSBsYW5nPSJzY3NzIiBtb2R1bGU+Ci5vcHMtdGV4dC1tZXNzYWdlIHsKICBAYXBwbHkgdGV4dC1zbSB3LWZ1bGwgaW5saW5lLWJsb2NrIHRleHQtZWxsaXBzaXMgb3ZlcmZsb3ctaGlkZGVuOwp9Cjwvc3R5bGU+Cg==",
-    T0 = "data:application/octet-stream;base64,PHRlbXBsYXRlPgogIDxkaXY+VmlkZW88L2Rpdj4KPC90ZW1wbGF0ZT4KCjxzY3JpcHQgbGFuZz0idHMiIHNldHVwPjwvc2NyaXB0PgoKPHN0eWxlIHNjb3BlZD48L3N0eWxlPgo=",
-    G0 = "data:application/octet-stream;base64,PHRlbXBsYXRlPgogIDxkaXYgdi1jbGljay1vdXRzaWRlPSJjbG9zZUVtb2ppIiA6Y2xhc3M9IiRzdHlsZVsnb3BzLWVtb2ppLXBpY2tlciddIj4KICAgIDxPQnV0dG9uCiAgICAgIHByZWZpeC1pY29uPSJlbW9qaSIKICAgICAgY2xhc3M9Im1sLTIiCiAgICAgIDpjbGFzcz0iJHN0eWxlWydvcHMtcm9vbS1mb290ZXJfX2FjdGlvbiddIgogICAgICBAY2xpY2s9InRvZ2dsZVBvcHVwIgogICAgLz4KICAgIDx0cmFuc2l0aW9uIG5hbWU9Im9wcy1zbGlkZS1sZWZ0Ij4KICAgICAgPEVtb2ppUGlja2VyCiAgICAgICAgdi1pZj0iaXNWaXNpYmxlIgogICAgICAgIG5hdGl2ZQogICAgICAgIDpjbGFzcz0iJHN0eWxlWydvcHMtZW1vamktcGlja2VyX19jb21wb25lbnQnXSIKICAgICAgICBAc2VsZWN0PSJvblNlbGVjdEVtb2ppIgogICAgICAvPgogICAgPC90cmFuc2l0aW9uPgogIDwvZGl2Pgo8L3RlbXBsYXRlPgoKPHNjcmlwdCBsYW5nPSJ0cyIgc2V0dXA+CmltcG9ydCB7IHJlZiB9IGZyb20gInZ1ZSI7CmltcG9ydCBPQnV0dG9uIGZyb20gIkAvY29tcG9uZW50cy91aS9PQnV0dG9uLnZ1ZSI7CmltcG9ydCBFbW9qaVBpY2tlciBmcm9tICJ2dWUzLWVtb2ppLXBpY2tlciI7CmltcG9ydCB7IElFbW9qaSB9IGZyb20gIkAvdHlwZXMvcm9vbS9yb29tLnR5cGVzIjsKaW1wb3J0ICJ2dWUzLWVtb2ppLXBpY2tlci9jc3MiOwoKY29uc3QgZW1pdCA9IGRlZmluZUVtaXRzPHsKICAoZTogInNlbGVjdC1lbW9qaSIsIHY6IElFbW9qaSk6IHZvaWQ7Cn0+KCk7Cgpjb25zdCBpc1Zpc2libGUgPSByZWYoZmFsc2UpOwoKY29uc3QgdG9nZ2xlUG9wdXAgPSAoKSA9PiB7CiAgaXNWaXNpYmxlLnZhbHVlID0gIWlzVmlzaWJsZS52YWx1ZTsKfTsKY29uc3QgY2xvc2VFbW9qaSA9ICgpID0+IHsKICBpc1Zpc2libGUudmFsdWUgPSBmYWxzZTsKfTsKY29uc3Qgb25TZWxlY3RFbW9qaSA9IChldmVudDogYW55KSA9PiB7CiAgY29uc3QgZW1vamlEYXRhOiBJRW1vamkgPSB7IGVtb2ppOiBldmVudC5pLCB1bmljb2RlOiBldmVudC51IH07CiAgZW1pdCgic2VsZWN0LWVtb2ppIiwgZW1vamlEYXRhKTsKfTsKCmRlZmluZUV4cG9zZSh7CiAgY2xvc2VFbW9qaSwKfSk7Cjwvc2NyaXB0PgoKPHN0eWxlIGxhbmc9InNjc3MiIG1vZHVsZT4KLm9wcy1lbW9qaS1waWNrZXIgewogIEBhcHBseSB3LWZpdCBoLWZpdCByZWxhdGl2ZSBmbGV4IGl0ZW1zLWNlbnRlciBqdXN0aWZ5LWNlbnRlcjsKICAmX19jb21wb25lbnQgewogICAgQGFwcGx5IGFic29sdXRlIGxlZnQtWy0xNXJlbV0gYm90dG9tLTEyOwogIH0KfQoKLm9wcy1yb29tLWZvb3Rlcl9fYWN0aW9uIHsKICBAYXBwbHkgcHgtMCB0cmFuc2l0aW9uLWFsbCBkdXJhdGlvbi0yMDAgcm91bmRlZC1mdWxsIHNocmluay0wOwogIGltZyB7CiAgICBAYXBwbHkgdy02IGgtNiBibG9jayB0cmFuc2l0aW9uLWFsbCBkdXJhdGlvbi0yMDA7CiAgICBmaWx0ZXI6IGludmVydCgzMyUpIHNlcGlhKDYlKSBzYXR1cmF0ZSgzODY3JSkgaHVlLXJvdGF0ZSgxOTBkZWcpCiAgICAgIGJyaWdodG5lc3MoOTYlKSBjb250cmFzdCg3NSUpICFpbXBvcnRhbnQ7CiAgfQp9Cjwvc3R5bGU+Cg==",
+    G0 = "data:application/octet-stream;base64,PHRlbXBsYXRlPgogIDxkaXY+VmlkZW88L2Rpdj4KPC90ZW1wbGF0ZT4KCjxzY3JpcHQgbGFuZz0idHMiIHNldHVwPjwvc2NyaXB0PgoKPHN0eWxlIHNjb3BlZD48L3N0eWxlPgo=",
+    T0 = "data:application/octet-stream;base64,PHRlbXBsYXRlPgogIDxkaXYgdi1jbGljay1vdXRzaWRlPSJjbG9zZUVtb2ppIiA6Y2xhc3M9IiRzdHlsZVsnb3BzLWVtb2ppLXBpY2tlciddIj4KICAgIDxPQnV0dG9uCiAgICAgIHByZWZpeC1pY29uPSJlbW9qaSIKICAgICAgY2xhc3M9Im1sLTIiCiAgICAgIDpjbGFzcz0iJHN0eWxlWydvcHMtcm9vbS1mb290ZXJfX2FjdGlvbiddIgogICAgICBAY2xpY2s9InRvZ2dsZVBvcHVwIgogICAgLz4KICAgIDx0cmFuc2l0aW9uIG5hbWU9Im9wcy1zbGlkZS1sZWZ0Ij4KICAgICAgPEVtb2ppUGlja2VyCiAgICAgICAgdi1pZj0iaXNWaXNpYmxlIgogICAgICAgIG5hdGl2ZQogICAgICAgIDpjbGFzcz0iJHN0eWxlWydvcHMtZW1vamktcGlja2VyX19jb21wb25lbnQnXSIKICAgICAgICBAc2VsZWN0PSJvblNlbGVjdEVtb2ppIgogICAgICAvPgogICAgPC90cmFuc2l0aW9uPgogIDwvZGl2Pgo8L3RlbXBsYXRlPgoKPHNjcmlwdCBsYW5nPSJ0cyIgc2V0dXA+CmltcG9ydCB7IHJlZiB9IGZyb20gInZ1ZSI7CmltcG9ydCBPQnV0dG9uIGZyb20gIkAvY29tcG9uZW50cy91aS9PQnV0dG9uLnZ1ZSI7CmltcG9ydCBFbW9qaVBpY2tlciBmcm9tICJ2dWUzLWVtb2ppLXBpY2tlciI7CmltcG9ydCB7IElFbW9qaSB9IGZyb20gIkAvdHlwZXMvcm9vbS9yb29tLnR5cGVzIjsKaW1wb3J0ICJ2dWUzLWVtb2ppLXBpY2tlci9jc3MiOwoKY29uc3QgZW1pdCA9IGRlZmluZUVtaXRzPHsKICAoZTogInNlbGVjdC1lbW9qaSIsIHY6IElFbW9qaSk6IHZvaWQ7Cn0+KCk7Cgpjb25zdCBpc1Zpc2libGUgPSByZWYoZmFsc2UpOwoKY29uc3QgdG9nZ2xlUG9wdXAgPSAoKSA9PiB7CiAgaXNWaXNpYmxlLnZhbHVlID0gIWlzVmlzaWJsZS52YWx1ZTsKfTsKY29uc3QgY2xvc2VFbW9qaSA9ICgpID0+IHsKICBpc1Zpc2libGUudmFsdWUgPSBmYWxzZTsKfTsKY29uc3Qgb25TZWxlY3RFbW9qaSA9IChldmVudDogYW55KSA9PiB7CiAgY29uc3QgZW1vamlEYXRhOiBJRW1vamkgPSB7IGVtb2ppOiBldmVudC5pLCB1bmljb2RlOiBldmVudC51IH07CiAgZW1pdCgic2VsZWN0LWVtb2ppIiwgZW1vamlEYXRhKTsKfTsKCmRlZmluZUV4cG9zZSh7CiAgY2xvc2VFbW9qaSwKfSk7Cjwvc2NyaXB0PgoKPHN0eWxlIGxhbmc9InNjc3MiIG1vZHVsZT4KLm9wcy1lbW9qaS1waWNrZXIgewogIEBhcHBseSB3LWZpdCBoLWZpdCByZWxhdGl2ZSBmbGV4IGl0ZW1zLWNlbnRlciBqdXN0aWZ5LWNlbnRlcjsKICAmX19jb21wb25lbnQgewogICAgQGFwcGx5IGFic29sdXRlIGxlZnQtWy0xNXJlbV0gYm90dG9tLTEyOwogIH0KfQoKLm9wcy1yb29tLWZvb3Rlcl9fYWN0aW9uIHsKICBAYXBwbHkgcHgtMCB0cmFuc2l0aW9uLWFsbCBkdXJhdGlvbi0yMDAgcm91bmRlZC1mdWxsIHNocmluay0wOwogIGltZyB7CiAgICBAYXBwbHkgdy02IGgtNiBibG9jayB0cmFuc2l0aW9uLWFsbCBkdXJhdGlvbi0yMDA7CiAgICBmaWx0ZXI6IGludmVydCgzMyUpIHNlcGlhKDYlKSBzYXR1cmF0ZSgzODY3JSkgaHVlLXJvdGF0ZSgxOTBkZWcpCiAgICAgIGJyaWdodG5lc3MoOTYlKSBjb250cmFzdCg3NSUpICFpbXBvcnRhbnQ7CiAgfQp9Cjwvc3R5bGU+Cg==",
     j0 = "data:application/octet-stream;base64,PHRlbXBsYXRlPgogIDxkaXYgOmNsYXNzPSIkc3R5bGVbJ29wcy1yb29tLWZvb3RlciddIj4KICAgIDxPQnV0dG9uCiAgICAgIHYtaWY9IjAiCiAgICAgIDpjbGFzcz0iJHN0eWxlWydvcHMtcm9vbS1mb290ZXJfX2FjdGlvbiddIgogICAgICBjbGFzcz0ibXItMiIKICAgICAgcHJlZml4LWljb249Im1pY3JvcGhvbmUiCiAgICAvPgogICAgPE9JbnB1dAogICAgICByZWY9ImlucHV0U2VhcmNoIgogICAgICB2LW1vZGVsPSJtZXNzYWdlUXVlcnkiCiAgICAgIGNsYXNzPSIhcHktMiIKICAgICAgcGxhY2Vob2xkZXI9IlR5cGUuLi4iCiAgICAgIEBrZXlkb3duLmVudGVyPSJvblNlbmQiCiAgICAgIEBpbnB1dD0ib25UeXBpbmciCiAgICAgIEBibHVyPSJvbkVuZFR5cGluZyIKICAgIC8+CiAgICA8ZGl2IDpjbGFzcz0iJHN0eWxlWydvcHMtcm9vbS1mb290ZXJfX2FjdGlvbi1lbmQnXSI+CiAgICAgIDxSb29tRW1vamlQaWNrZXIgcmVmPSJlbW9qaVBpY2tlciIgQHNlbGVjdC1lbW9qaT0ib25FbW9qaSIgLz4KICAgICAgPE9CdXR0b24KICAgICAgICB2LWlmPSIwIgogICAgICAgIHByZWZpeC1pY29uPSJmaWxlIgogICAgICAgIGNsYXNzPSJtbC0yIgogICAgICAgIDpjbGFzcz0iJHN0eWxlWydvcHMtcm9vbS1mb290ZXJfX2FjdGlvbiddIgogICAgICAvPgogICAgICA8T0J1dHRvbgogICAgICAgIHByZWZpeC1pY29uPSJzZW5kIgogICAgICAgIGNsYXNzPSJtbC0yIgogICAgICAgIDpjbGFzcz0iJHN0eWxlWydvcHMtcm9vbS1mb290ZXJfX2FjdGlvbiddIgogICAgICAgIEBjbGljaz0ib25TZW5kIgogICAgICAvPgogICAgPC9kaXY+CiAgPC9kaXY+CjwvdGVtcGxhdGU+Cgo8c2NyaXB0IHNldHVwIGxhbmc9InRzIj4KaW1wb3J0IHsgUHJvcFR5cGUsIHJlZiB9IGZyb20gInZ1ZSI7CmltcG9ydCBPSW5wdXQgZnJvbSAiQC9jb21wb25lbnRzL3VpL09JbnB1dC52dWUiOwppbXBvcnQgT0J1dHRvbiBmcm9tICJAL2NvbXBvbmVudHMvdWkvT0J1dHRvbi52dWUiOwppbXBvcnQgUm9vbUVtb2ppUGlja2VyIGZyb20gIkAvY29tcG9uZW50cy9yb29tL2Zvb3Rlci9Sb29tRW1vamlQaWNrZXIudnVlIjsKaW1wb3J0IHsgSUVtb2ppIH0gZnJvbSAiQC90eXBlcy9yb29tL3Jvb20udHlwZXMiOwppbXBvcnQgeyBJUm9vbSB9IGZyb20gIkAvdHlwZXMvcm9vbXMudHlwZXMiOwppbXBvcnQgeyBXU19UWVBFUyB9IGZyb20gIkAvdHlwZXMvZ2VuZXJhbC50eXBlcyI7CmltcG9ydCB3ZWJzb2NrZXRTZXJ2aWNlIGZyb20gIkAvc2VydmljZXMvY2hhdC93ZWJzb2NrZXQtY2hhdCI7Cgpjb25zdCBwcm9wcyA9IGRlZmluZVByb3BzKHsKICByb29tOiB7CiAgICB0eXBlOiBPYmplY3QgYXMgUHJvcFR5cGU8SVJvb20+LAogICAgZGVmYXVsdDogKCkgPT4gKHt9KSwKICB9LAp9KTsKY29uc3QgaW5wdXRTZWFyY2ggPSByZWY8SW5zdGFuY2VUeXBlPHR5cGVvZiBPSW5wdXQ+PigpOwpjb25zdCBlbW9qaVBpY2tlciA9IHJlZjxJbnN0YW5jZVR5cGU8dHlwZW9mIFJvb21FbW9qaVBpY2tlcj4+KCk7CmNvbnN0IG1lc3NhZ2VRdWVyeSA9IHJlZigiIik7CmNvbnN0IHR5cGluZ09wdGlvbnMgPSByZWYoewogIGlzQnVzeTogZmFsc2UsCiAgdGltZXI6IDAsCn0pOwoKY29uc3Qgb25FbW9qaSA9IChlbW9qaTogSUVtb2ppKSA9PiB7CiAgbWVzc2FnZVF1ZXJ5LnZhbHVlICs9IGVtb2ppLmVtb2ppOwogIGlucHV0U2VhcmNoLnZhbHVlPy5pbnB1dFJlZi5mb2N1cygpOwp9OwoKY29uc3Qgb25TZW5kID0gYXN5bmMgKCkgPT4gewogIGlmIChtZXNzYWdlUXVlcnkudmFsdWUpIHsKICAgIGNvbnN0IG1lc3NhZ2UgPSB7CiAgICAgIHR5cGU6IFdTX1RZUEVTLkNIQVRfTUVTU0FHRVMsCiAgICAgIG1lc3NhZ2U6IG1lc3NhZ2VRdWVyeS52YWx1ZSwKICAgIH07CgogICAgYXdhaXQgd2Vic29ja2V0U2VydmljZS5zZW5kTWVzc2FnZShtZXNzYWdlKTsKCiAgICByZXNldEZvb3RlcigpOwogICAgb25FbmRUeXBpbmcoKTsKICB9Cn07Cgpjb25zdCByZXNldEZvb3RlciA9ICgpID0+IHsKICBtZXNzYWdlUXVlcnkudmFsdWUgPSAiIjsKICBlbW9qaVBpY2tlci52YWx1ZT8uY2xvc2VFbW9qaSgpOwp9Owpjb25zdCBvblR5cGluZyA9ICgpID0+IHsKICBpZiAoIXR5cGluZ09wdGlvbnMudmFsdWUuaXNCdXN5KSB7CiAgICB3ZWJzb2NrZXRTZXJ2aWNlLnNlbmRNZXNzYWdlKHsKICAgICAgdHlwZTogV1NfVFlQRVMuVFlQSU5HLAogICAgICB0eXBpbmc6IHRydWUsCiAgICB9KTsKICAgIHR5cGluZ09wdGlvbnMudmFsdWUuaXNCdXN5ID0gdHJ1ZTsKICB9CiAgY2xlYXJUaW1lb3V0KHR5cGluZ09wdGlvbnMudmFsdWUudGltZXIpOwogIHR5cGluZ09wdGlvbnMudmFsdWUudGltZXIgPSBzZXRUaW1lb3V0KCgpID0+IHsKICAgIG9uRW5kVHlwaW5nKCk7CiAgICB0eXBpbmdPcHRpb25zLnZhbHVlLmlzQnVzeSA9IGZhbHNlOwogIH0sIDMwMDApOwp9Owpjb25zdCBvbkVuZFR5cGluZyA9ICgpID0+IHsKICB3ZWJzb2NrZXRTZXJ2aWNlLnNlbmRNZXNzYWdlKHsKICAgIHR5cGU6IFdTX1RZUEVTLlRZUElORywKICAgIHR5cGluZzogZmFsc2UsCiAgfSk7CiAgd2Vic29ja2V0U2VydmljZS51c2VyVHlwaW5nLnZhbHVlID0ge307Cn07Cjwvc2NyaXB0Pgo8c3R5bGUgbGFuZz0ic2NzcyIgbW9kdWxlPgoub3BzLXJvb20tZm9vdGVyIHsKICBAYXBwbHkgYmctZ3JleS1hdGhlbnMgdy1mdWxsIHotMTAgcHktNCBweC0yIGZsZXggaXRlbXMtY2VudGVyICBzaGFkb3ctWzBfMnB4XzhweF8wcHhfcmdiYSg5OSw5OSw5OSwwLjIpXTsKCiAgJl9fYWN0aW9uIHsKICAgIEBhcHBseSBweC0wIHRyYW5zaXRpb24tYWxsIGR1cmF0aW9uLTIwMCByb3VuZGVkLWZ1bGwgc2hyaW5rLTA7CgogICAgJjpob3ZlciB7CiAgICAgIGltZyB7CiAgICAgICAgQGFwcGx5IHNjYWxlLVsxLjJdOwogICAgICB9CiAgICB9CiAgfQoKICAmX19hY3Rpb24tZW5kIHsKICAgIEBhcHBseSBmbGV4IGl0ZW1zLWNlbnRlciBzaHJpbmstMDsKICB9Cn0KPC9zdHlsZT4K",
     k0 = "/static/chat/RoomHeader.vue",
     D0 = "data:application/octet-stream;base64,PHRlbXBsYXRlPgogIDxkaXYgOmNsYXNzPSIkc3R5bGVbJ29wcy1jaGF0LWNvbnRhaW5lciddIj4KICAgIDxkaXYKICAgICAgOmNsYXNzPSJbCiAgICAgICAgJHN0eWxlWydvcHMtcm9vbXMtd3JhcHBlciddLAogICAgICAgIHsgWyRzdHlsZVsnb3BzLXJvb21zLXdyYXBwZXJfX3Nob3ctcm9vbXMnXV06ICFzaG93Um9vbXNMaXN0IH0sCiAgICAgICAgeyBbJHN0eWxlWydzaG93LWJsb2NrJ11dOiBnZXRNb2JpbGVWaXNpYmxlIH0sCiAgICAgIF0iCiAgICA+CiAgICAgIDwhLS0gUm9vbSBzZWFyY2ggYm94IC0tPgogICAgICA8ZGl2IDpjbGFzcz0iJHN0eWxlWydvcHMtcm9vbXMtd3JhcHBlcl9fc2VhcmNoLWJveCddIj4KICAgICAgICA8T0lucHV0IHYtbW9kZWw9InNlYXJjaFF1ZXJ5IiBwbGFjZWhvbGRlcj0iU2VhcmNoLi4uIj4KICAgICAgICAgIDx0ZW1wbGF0ZSAjcHJlZml4PgogICAgICAgICAgICA8aW1nCiAgICAgICAgICAgICAgOmNsYXNzPSIkc3R5bGVbJ29wcy1yb29tcy13cmFwcGVyX19zZWFyY2gtaWNvbiddIgogICAgICAgICAgICAgIDpzcmM9ImdldEltYWdlVXJsKCdhc3NldHMvaWNvbnMvc2VhcmNoLnN2ZycpIgogICAgICAgICAgICAgIGFsdD0ic2VhcmNoLWljb24iCiAgICAgICAgICAgIC8+CiAgICAgICAgICA8L3RlbXBsYXRlPgogICAgICAgIDwvT0lucHV0PgogICAgICAgIDxidXR0b24gdi1pZj0iMCIgOmNsYXNzPSIkc3R5bGVbJ29wcy1yb29tcy13cmFwcGVyX19hZGQtcm9vbSddIj4KICAgICAgICAgIDxpbWcKICAgICAgICAgICAgd2lkdGg9IjMwIgogICAgICAgICAgICA6c3JjPSJnZXRJbWFnZVVybCgnYXNzZXRzL2ljb25zL2NyZWF0ZS1yb29tLnN2ZycpIgogICAgICAgICAgICBhbHQ9ImFkZCIKICAgICAgICAgIC8+CiAgICAgICAgPC9idXR0b24+CiAgICAgIDwvZGl2PgoKICAgICAgPCEtLSBMaXN0IG9mIGZpbHRlcmVkIHJvb21zIC0tPgogICAgICA8Um9vbXNMaXN0CiAgICAgICAgdi1pZj0id2Vic29ja2V0U2VydmljZS5yb29tcy52YWx1ZS5sZW5ndGgiCiAgICAgICAgOnJvb21zPSJmaWx0ZXJlZFJvb21zIgogICAgICAgIDpzZWxlY3RlZC1yb29tPSJzZWxlY3RlZFJvb20iCiAgICAgIC8+CiAgICA8L2Rpdj4KCiAgICA8IS0tICAgIEN1cnJlbnQgcm9vbS0tPgogICAgPGRpdiA6Y2xhc3M9IiRzdHlsZVsnb3BzLWNoYXQtcm9vbSddIj4KICAgICAgPFJvb20KICAgICAgICB2LWlmPSJzZWxlY3RlZFJvb20/LmlkIgogICAgICAgIDpjbGFzcz0ieyBbJHN0eWxlWydzaG93LWJsb2NrJ11dOiAhZ2V0TW9iaWxlVmlzaWJsZSB9IgogICAgICAgIDpzaG93LXJvb21zLWxpc3Q9InNob3dSb29tc0xpc3QiCiAgICAgICAgOnJvb20taWQ9InNlbGVjdGVkUm9vbS5pZCIKICAgICAgICBAdG9nZ2xlLXJvb21zLWxpc3Q9InRvZ2dsZVJvb21zTGlzdCIKICAgICAgLz4KICAgICAgPFJvb21Ob01lc3NhZ2VzIHYtZWxzZSB0ZXh0PSJQbGVhc2Ugc2VsZWN0IHJvb20iIC8+CiAgICA8L2Rpdj4KICA8L2Rpdj4KPC90ZW1wbGF0ZT4KCjxzY3JpcHQgbGFuZz0idHMiIHNldHVwPgppbXBvcnQgeyBjb21wdXRlZCwgb25Nb3VudGVkLCByZWYgfSBmcm9tICJ2dWUiOwppbXBvcnQgT0lucHV0IGZyb20gIkAvY29tcG9uZW50cy91aS9PSW5wdXQudnVlIjsKaW1wb3J0IFJvb21zTGlzdCBmcm9tICJAL2NvbXBvbmVudHMvcm9vbXMvUm9vbXNMaXN0LnZ1ZSI7CmltcG9ydCBSb29tIGZyb20gIkAvY29tcG9uZW50cy9yb29tL1Jvb20udnVlIjsKaW1wb3J0IHsgSVJvb20gfSBmcm9tICJAL3R5cGVzL3Jvb21zLnR5cGVzIjsKaW1wb3J0IHsgZ2V0SW1hZ2VVcmwgfSBmcm9tICJAL2hlbHBlcnMvaW1wb3J0LWltYWdlIjsKaW1wb3J0IHsgdXNlTWFpblN0b3JlIH0gZnJvbSAiQC9zdG9yZS91c2VNYWluU3RvcmUiOwppbXBvcnQgY2hhdFNlcnZpY2UgZnJvbSAiQC9zZXJ2aWNlcy9jaGF0L2NoYXQiOwppbXBvcnQgd2Vic29ja2V0U2VydmljZSBmcm9tICJAL3NlcnZpY2VzL2NoYXQvd2Vic29ja2V0LWNoYXQiOwppbXBvcnQgUm9vbU5vTWVzc2FnZXMgZnJvbSAiQC9jb21wb25lbnRzL3Jvb20vY29udGVudC9Sb29tTm9NZXNzYWdlcy52dWUiOwoKY29uc3QgbWFpblN0b3JlID0gdXNlTWFpblN0b3JlKCk7Cgpjb25zdCBzZWFyY2hRdWVyeSA9IHJlZigiIik7CmNvbnN0IHNob3dSb29tc0xpc3QgPSByZWYodHJ1ZSk7CmNvbnN0IGdldE1vYmlsZVZpc2libGUgPSBjb21wdXRlZCgoKSA9PiBtYWluU3RvcmUuaXNNb2JpbGVWaXNpYmxlKTsKY29uc3Qgc2VsZWN0ZWRSb29tID0gY29tcHV0ZWQoKCkgPT4gd2Vic29ja2V0U2VydmljZS5zZWxlY3RlZFJvb20udmFsdWUpOwoKY29uc3QgZmlsdGVyZWRSb29tcyA9IGNvbXB1dGVkKCgpID0+IHsKICBjb25zdCBxdWVyeSA9IHNlYXJjaFF1ZXJ5LnZhbHVlLnRvTG93ZXJDYXNlKCk7CiAgaWYgKCFxdWVyeSkgewogICAgcmV0dXJuIHdlYnNvY2tldFNlcnZpY2Uucm9vbXMudmFsdWU7CiAgfQogIHJldHVybiB3ZWJzb2NrZXRTZXJ2aWNlLnJvb21zLnZhbHVlPy5maWx0ZXIoKGNoYXQ6IElSb29tKSA9PiB7CiAgICByZXR1cm4gY2hhdC5uYW1lLnRvTG93ZXJDYXNlKCkuaW5jbHVkZXMocXVlcnkpOwogIH0pOwp9KTsKCmNvbnN0IHRvZ2dsZVJvb21zTGlzdCA9ICgpID0+IChzaG93Um9vbXNMaXN0LnZhbHVlID0gIXNob3dSb29tc0xpc3QudmFsdWUpOwoKY29uc3QgbG9hZFJvb21zID0gYXN5bmMgKCkgPT4gewogIHdlYnNvY2tldFNlcnZpY2Uucm9vbXMudmFsdWUgPSBhd2FpdCBjaGF0U2VydmljZS5mZXRjaENvbnZlcnNhdGlvbnMoKTsKfTsKCm9uTW91bnRlZCgoKSA9PiB7CiAgbG9hZFJvb21zKCk7Cn0pOwo8L3NjcmlwdD4KCjxzdHlsZSBsYW5nPSJzY3NzIiBtb2R1bGU+Ci5vcHMtY2hhdC1jb250YWluZXIgewogIEBhcHBseSBmbGV4IGgtW2NhbGMoMTAwdmgtNnJlbSldOwoKICAub3BzLXJvb21zLXdyYXBwZXIgewogICAgQGFwcGx5IGJnLXdoaXRlIGZsZXggZmxleC1jb2wgdHJhbnNpdGlvbi1hbGwgZHVyYXRpb24tMTAwMCBvdmVyZmxvdy1oaWRkZW4gcmVsYXRpdmUgZ3Jvdy0wIHNocmluay0wIG1kOmJhc2lzLTMvMTIgbWluLXctWzE2LjI1cmVtXSB3LWZ1bGwgbWQ6bWF4LXctWzMxLjI1cmVtXSBwLTQgaC1mdWxsIG1kOmJvcmRlci1ncmV5LW1pc2Noa2EgbWQ6Ym9yZGVyLXItWzFweF07CgogICAgJl9fc2VhcmNoLWJveCB7CiAgICAgIEBhcHBseSBmbGV4IGl0ZW1zLWNlbnRlciB3LWZ1bGw7CiAgICB9CgogICAgJl9fc2VhcmNoLWljb24gewogICAgICBAYXBwbHkgbXItMTsKICAgICAgZmlsdGVyOiBpbnZlcnQoNDUlKSBzZXBpYSg4JSkgc2F0dXJhdGUoNzc4JSkgaHVlLXJvdGF0ZSgxODJkZWcpCiAgICAgICAgYnJpZ2h0bmVzcyg5NCUpIGNvbnRyYXN0KDgwJSk7CiAgICB9CgogICAgJl9fYWRkLXJvb20gewogICAgICBAYXBwbHkgbWwtMyByb3VuZGVkLWZ1bGw7CgogICAgICBpbWcgewogICAgICAgIEBhcHBseSB0cmFuc2l0aW9uLWFsbCBkdXJhdGlvbi01MDA7CgogICAgICAgICY6aG92ZXIgewogICAgICAgICAgQGFwcGx5IHNjYWxlLTExMCBvcGFjaXR5LTcwOwogICAgICAgIH0KICAgICAgfQogICAgfQoKICAgICZfX3Nob3ctcm9vbXMgewogICAgICBAYXBwbHkgdy0wIG1pbi13LTAgYmFzaXMtMCBweC0wICN7IWltcG9ydGFudH07CiAgICB9CiAgfQoKICAub3BzLWNoYXQtcm9vbSB7CiAgICBAYXBwbHkgaC1mdWxsIHctZnVsbCByZWxhdGl2ZSBiZy1ncmV5LWF0aGVuczsKICB9Cn0KCi5zaG93LWJsb2NrIHsKICBAYXBwbHkgaGlkZGVuIG1kOmZsZXggI3shaW1wb3J0YW50fTsKfQo8L3N0eWxlPgo=",
     R0 = "data:application/octet-stream;base64,PHRlbXBsYXRlPgogIDxkaXYgOmNsYXNzPSIkc3R5bGVbJ3Jvb21zLWVtcHR5J10iPgogICAgPHA+VGhlcmUgYXJlbmB0IGFueSByb29tczwvcD4KICA8L2Rpdj4KPC90ZW1wbGF0ZT4KCjxzdHlsZSBsYW5nPSJzY3NzIiBtb2R1bGU+Ci5yb29tcy1lbXB0eSB7CiAgYW5pbWF0aW9uOiBlbXB0eVJvb21zIDAuNHM7CiAgQGFwcGx5IG10LTEwIGJnLWNvbmZldHRpIHJvdW5kZWQtbWQgcHktMjsKICBwIHsKICAgIEBhcHBseSB0ZXh0LWNlbnRlciB0ZXh0LWdyZXkta2FzaG1pcjsKICB9Cn0KCkBrZXlmcmFtZXMgZW1wdHlSb29tcyB7CiAgMCUgewogICAgdHJhbnNmb3JtOiBzY2FsZSgwLjk1KTsKICB9CiAgNTAlIHsKICAgIHRyYW5zZm9ybTogc2NhbGUoMS4xKTsKICB9CiAgNzUlIHsKICAgIHRyYW5zZm9ybTogc2NhbGUoMS4wNSk7CiAgfQogIDkwJSB7CiAgICB0cmFuc2Zvcm06IHNjYWxlKDEuMDcpOwogIH0KICAxMDAlIHsKICAgIHRyYW5zZm9ybTogc2NhbGUoMSk7CiAgfQp9Cjwvc3R5bGU+Cg==",
     x0 = "data:application/octet-stream;base64,PHRlbXBsYXRlPgogIDxkaXYKICAgIHYtaWY9InJvb21EYXRhPy5pZCIKICAgIDpjbGFzcz0iWwogICAgICAkc3R5bGVbJ29wcy1yb29tcy1pdGVtJ10sCiAgICAgIHsgWyRzdHlsZVsnb3BzLXJvb21zLWl0ZW1fX3NlbGVjdGVkJ11dOiBpc1NlbGVjdGVkUm9vbSB9LAogICAgXSIKICAgIEBjbGljaz0iJGVtaXQoJ3NlbGVjdC1yb29tJywgcm9vbURhdGEpIgogID4KICAgIDxkaXYgOmNsYXNzPSJbJHN0eWxlWydvcHMtcm9vbXMtaXRlbV9fY29udGVudCddLCAkc3R5bGVbJ2NvbnRlbnQnXV0iPgogICAgICA8ZGl2IDpjbGFzcz0iJHN0eWxlWydjb250ZW50X19pbmZvJ10iPgogICAgICAgIDxWRHJvcGRvd24KICAgICAgICAgIHRoZW1lPSJvcHMtcm9vbS1pdGVtX19uYW1lIgogICAgICAgICAgOnRyaWdnZXJzPSJbJ2hvdmVyJ10iCiAgICAgICAgICA6cGxhY2VtZW50PSInYm90dG9tLXN0YXJ0JyIKICAgICAgICAgIDpkaXN0YW5jZT0iNiIKICAgICAgICA+CiAgICAgICAgICA8aDIgOmNsYXNzPSIkc3R5bGVbJ3RpdGxlJ10iPnt7IHJvb21EYXRhPy5uYW1lIH19PC9oMj4KICAgICAgICAgIDx0ZW1wbGF0ZSAjcG9wcGVyPgogICAgICAgICAgICA8aDIgOmNsYXNzPSIkc3R5bGVbJ3RpdGxlJ10iPnt7IHJvb21EYXRhPy5uYW1lIH19PC9oMj4KICAgICAgICAgIDwvdGVtcGxhdGU+CiAgICAgICAgPC9WRHJvcGRvd24+CiAgICAgICAgPHAKICAgICAgICAgIHYtaWY9InJvb21EYXRhLmxhc3RfbWVzc2FnZSIKICAgICAgICAgIDpjbGFzcz0iJHN0eWxlWydjb250ZW50X19sYXN0LW1lc3NhZ2UnXSIKICAgICAgICA+CiAgICAgICAgICB7eyByb29tRGF0YS5sYXN0X21lc3NhZ2UuY29udGVudCB9fQogICAgICAgIDwvcD4KICAgICAgPC9kaXY+CiAgICAgIDxkaXYgOmNsYXNzPSJbJHN0eWxlWydvcHMtcm9vbXMtaXRlbV9fYWN0aW9uJ10sICRzdHlsZVsnYWN0aW9uJ11dIj4KICAgICAgICA8cAogICAgICAgICAgdi1pZj0icm9vbURhdGE/Lmxhc3RfbWVzc2FnZT8udGltZXN0YW1wIgogICAgICAgICAgOmNsYXNzPSIkc3R5bGVbJ2FjdGlvbl9fdGltZSddIgogICAgICAgID4KICAgICAgICAgIHt7IGZvcm1hdERhdGUgfX0KICAgICAgICA8L3A+CiAgICAgICAgPHRyYW5zaXRpb24gbmFtZT0ib3BzLXNsaWRlLWxlZnQiPgogICAgICAgICAgPGRpdgogICAgICAgICAgICB2LWlmPSJyb29tRGF0YT8udW5yZWFkX21lc3NhZ2VzIgogICAgICAgICAgICA6Y2xhc3M9IiRzdHlsZVsnb3BzLXJvb21zLWl0ZW1fX3VucmVhZC1tZXNzYWdlJ10iCiAgICAgICAgICA+CiAgICAgICAgICAgIDxzcGFuPnt7IGZvcm1hdFVucmVhZE1lc3NhZ2VzIH19PC9zcGFuPgogICAgICAgICAgPC9kaXY+CiAgICAgICAgPC90cmFuc2l0aW9uPgogICAgICA8L2Rpdj4KICAgIDwvZGl2PgogIDwvZGl2Pgo8L3RlbXBsYXRlPgoKPHNjcmlwdCBsYW5nPSJ0cyIgc2V0dXA+CmltcG9ydCB7IGNvbXB1dGVkLCBkZWZpbmVFbWl0cywgUHJvcFR5cGUgfSBmcm9tICJ2dWUiOwppbXBvcnQgeyBJUm9vbSB9IGZyb20gIkAvdHlwZXMvcm9vbXMudHlwZXMiOwppbXBvcnQgZGF5anMgZnJvbSAiZGF5anMiOwppbXBvcnQgcmVsYXRpdmVUaW1lIGZyb20gImRheWpzL3BsdWdpbi9yZWxhdGl2ZVRpbWUiOwppbXBvcnQgaXNUb2RheSBmcm9tICJkYXlqcy9wbHVnaW4vaXNUb2RheSI7CgpkYXlqcy5leHRlbmQocmVsYXRpdmVUaW1lKTsKZGF5anMuZXh0ZW5kKGlzVG9kYXkpOwoKY29uc3QgcHJvcHMgPSBkZWZpbmVQcm9wcyh7CiAgcm9vbURhdGE6IHsKICAgIHR5cGU6IE9iamVjdCBhcyBQcm9wVHlwZTxJUm9vbT4sCiAgICBkZWZhdWx0OiAoKSA9PiAoe30pLAogIH0sCiAgaXNTZWxlY3RlZFJvb206IHsKICAgIHR5cGU6IEJvb2xlYW4sCiAgICBkZWZhdWx0OiBmYWxzZSwKICB9LAp9KTsKCmRlZmluZUVtaXRzKFsic2VsZWN0LXJvb20iXSk7Cgpjb25zdCBmb3JtYXREYXRlID0gY29tcHV0ZWQoKCkgPT4KICBkYXlqcyhwcm9wcy5yb29tRGF0YT8ubGFzdF9tZXNzYWdlLnRpbWVzdGFtcCkuaXNUb2RheSgpCiAgICA/IGRheWpzKCkudG8ocHJvcHMucm9vbURhdGE/Lmxhc3RfbWVzc2FnZS50aW1lc3RhbXApCiAgICA6IGRheWpzKHByb3BzLnJvb21EYXRhPy5sYXN0X21lc3NhZ2UudGltZXN0YW1wKS5mb3JtYXQoIkRELU1NLVlZWVkiKQopOwpjb25zdCBmb3JtYXRVbnJlYWRNZXNzYWdlcyA9IGNvbXB1dGVkKCgpID0+CiAgcHJvcHMucm9vbURhdGEudW5yZWFkX21lc3NhZ2VzID49IDEwMCA/ICI5OSsiIDogcHJvcHMucm9vbURhdGEudW5yZWFkX21lc3NhZ2VzCik7Cjwvc2NyaXB0PgoKPHN0eWxlIGxhbmc9InNjc3MiIG1vZHVsZT4KLm9wcy1yb29tcy1pdGVtIHsKICBAYXBwbHkgbWluLWgtWzUuNXJlbV0gcmVsYXRpdmUgbXgtMC41IGN1cnNvci1wb2ludGVyIGZsZXggcC00IHJvdW5kZWQtbGcgbWItMiB0ZXh0LWdyZXkta2FzaG1pciBob3ZlcjpvdXRsaW5lIGhvdmVyOm91dGxpbmUtMSBob3ZlcjpvdXRsaW5lLWNvbmZldHRpOwoKICAmX19zZWxlY3RlZCB7CiAgICBAYXBwbHkgYmctY29uZmV0dGk7CiAgfQoKICAuY29udGVudCB7CiAgICBAYXBwbHkgdy1mdWxsICBvdmVyZmxvdy1oaWRkZW47CgogICAgJl9faW5mbyB7CiAgICAgIEBhcHBseSB3LWZ1bGwgb3ZlcmZsb3ctaGlkZGVuIG1yLTIgZmxleCBmbGV4LWNvbCBqdXN0aWZ5LWJldHdlZW47CiAgICAgIC50aXRsZSB7CiAgICAgICAgQGFwcGx5IHRleHQtc20gdGV4dC1ncmV5LWthc2htaXIgZm9udC1tZWRpdW0gdHJ1bmNhdGUgaW5saW5lLWJsb2NrIHctZnVsbDsKICAgICAgfQogICAgfQoKICAgICZfX2xhc3QtbWVzc2FnZSB7CiAgICAgIEBhcHBseSB0ZXh0LVswLjc1cmVtXSBsZWFkaW5nLTUgdHJ1bmNhdGUgdGV4dC1ncmV5LWhpdC1ncmV5OwogICAgfQoKICAgIC5hY3Rpb24gewogICAgICBAYXBwbHkgZmxleCBqdXN0aWZ5LWJldHdlZW47CgogICAgICAmX190aW1lIHsKICAgICAgICBAYXBwbHkgdGV4dC1bMC42OHJlbV0gbGVhZGluZy1bMS4ycmVtXSB0cnVuY2F0ZSB0ZXh0LWdyZXktaGl0LWdyZXk7CiAgICAgIH0KICAgIH0KICB9CgogICZfX3VucmVhZC1tZXNzYWdlIHsKICAgIEBhcHBseSBweC0xIGJnLWdyZXkta2FzaG1pciBmbGV4IGl0ZW1zLWNlbnRlciBqdXN0aWZ5LWNlbnRlciB0ZXh0LXdoaXRlIHRleHQtWzAuN3JlbV0gdGV4dC1jZW50ZXIgcm91bmRlZC1mdWxsIG1pbi13LVsxLjI1cmVtXTsKICB9Cn0KCkBrZXlmcmFtZXMgc2NhbGVEb3duIHsKICAwJSB7CiAgICB0cmFuc2Zvcm06IHNjYWxlKDEpOwogIH0KICAyNSUgewogICAgdHJhbnNmb3JtOiBzY2FsZSgwLjk1KTsKICB9CiAgNTAlIHsKICAgIHRyYW5zZm9ybTogc2NhbGUoMSk7CiAgfQogIDc1JSB7CiAgICB0cmFuc2Zvcm06IHNjYWxlKDAuOTgpOwogIH0KICAxMDAlIHsKICAgIHRyYW5zZm9ybTogc2NhbGUoMSk7CiAgfQp9Cjwvc3R5bGU+CjwhLS0gc3R5bGVzIGZvciBwYWNrYWdlcyAtLT4KPHN0eWxlIGxhbmc9InNjc3MiPgoudi1wb3BwZXItLXRoZW1lLW9wcy1yb29tLWl0ZW1fX25hbWUgewogIC52LXBvcHBlcl9faW5uZXIgewogICAgQGFwcGx5IGJnLXdoaXRlIHJvdW5kZWQtbWQgcHgtMiBweS0xIGJvcmRlciBib3JkZXItZ3JleS1rYXNobWlyIHRleHQtZ3JleS1rYXNobWlyIHRleHQtc207CiAgfQoKICAudi1wb3BwZXJfX2Fycm93LWNvbnRhaW5lciB7CiAgICAudi1wb3BwZXJfX2Fycm93LW91dGVyIHsKICAgICAgQGFwcGx5IGJvcmRlci1ncmV5LWthc2htaXI7CiAgICB9CiAgfQp9Cjwvc3R5bGU+Cg==",
     X0 = "data:application/octet-stream;base64,PHRlbXBsYXRlPgogIDxkaXYgOmNsYXNzPSIkc3R5bGVbJ29wcy1yb29tcy1saXN0J10iPgogICAgPGRpdiB2LWlmPSJyb29tcz8ubGVuZ3RoIiA6Y2xhc3M9IiRzdHlsZVsnb3BzLXJvb21zLWxpc3RfX2l0ZW1zJ10iPgogICAgICA8Um9vbXNJdGVtCiAgICAgICAgdi1mb3I9InJvb20gaW4gcm9vbXMiCiAgICAgICAgOmtleT0icm9vbS5pZCIKICAgICAgICA6cm9vbS1kYXRhPSJyb29tIgogICAgICAgIDppcy1zZWxlY3RlZC1yb29tPSJzZWxlY3RlZFJvb20/LmlkID09PSByb29tLmlkIgogICAgICAgIEBzZWxlY3Qtcm9vbT0iaGFuZGxlU2VsZWN0Um9vbSIKICAgICAgLz4KICAgIDwvZGl2PgogICAgPFJvb21zRW1wdHkgdi1lbHNlIC8+CiAgPC9kaXY+CjwvdGVtcGxhdGU+Cgo8c2NyaXB0IGxhbmc9InRzIiBzZXR1cD4KaW1wb3J0IHsgUHJvcFR5cGUgfSBmcm9tICJ2dWUiOwppbXBvcnQgUm9vbXNJdGVtIGZyb20gIkAvY29tcG9uZW50cy9yb29tcy9Sb29tc0l0ZW0udnVlIjsKaW1wb3J0IHsgSVJvb20gfSBmcm9tICJAL3R5cGVzL3Jvb21zLnR5cGVzIjsKaW1wb3J0IFJvb21zRW1wdHkgZnJvbSAiQC9jb21wb25lbnRzL3Jvb21zL1Jvb21zRW1wdHkudnVlIjsKaW1wb3J0IHdlYnNvY2tldFNlcnZpY2UgZnJvbSAiQC9zZXJ2aWNlcy9jaGF0L3dlYnNvY2tldC1jaGF0IjsKaW1wb3J0IHsgdXNlTWFpblN0b3JlIH0gZnJvbSAiQC9zdG9yZS91c2VNYWluU3RvcmUiOwoKY29uc3QgbWFpblN0b3JlID0gdXNlTWFpblN0b3JlKCk7CmRlZmluZVByb3BzKHsKICByb29tczogewogICAgdHlwZTogQXJyYXkgYXMgUHJvcFR5cGU8SVJvb21bXT4sCiAgICBkZWZhdWx0OiAoKSA9PiBbXSwKICB9LAogIHNlbGVjdGVkUm9vbTogewogICAgdHlwZTogT2JqZWN0IGFzIFByb3BUeXBlPElSb29tPiwKICAgIGRlZmF1bHQ6IG51bGwsCiAgfSwKfSk7Cgpjb25zdCBoYW5kbGVTZWxlY3RSb29tID0gKHJvb206IElSb29tKSA9PiB7CiAgd2Vic29ja2V0U2VydmljZS5zZWxlY3RlZFJvb20udmFsdWUgPSByb29tOwogIG1haW5TdG9yZS50b2dnbGVNb2JpbGVWaXNpYmxlKCk7Cn07Cjwvc2NyaXB0Pgo8c3R5bGUgbGFuZz0ic2NzcyIgbW9kdWxlPgoub3BzLXJvb21zLWxpc3QgewogIEBhcHBseSBoLWZ1bGw7CiAgJl9faXRlbXMgewogICAgQGFwcGx5IG10LTQgcHQtMiBoLVtjYWxjKDEwMHZoLTEycmVtKV0gb3ZlcmZsb3ctYXV0bzsKICB9Cn0KPC9zdHlsZT4K",
     Y0 = "data:application/octet-stream;base64,PHRlbXBsYXRlPgogIDxidXR0b24gOmNsYXNzPSIkc3R5bGVbJ29wcy1idXR0b24nXSIgdi1iaW5kPSIkYXR0cnMiPgogICAgPGltZwogICAgICB2LWlmPSJwcmVmaXhJY29uIgogICAgICA6Y2xhc3M9IiRzdHlsZVsnb3BzLWJ1dHRvbl9faW1nJ10iCiAgICAgIDpzcmM9ImdldEltYWdlVXJsKGBhc3NldHMvaWNvbnMvJHtwcmVmaXhJY29ufS5zdmdgKSIKICAgICAgYWx0PSJpY29uIgogICAgLz4KICAgIDxzbG90IC8+CiAgICA8aW1nCiAgICAgIHYtaWY9InN1ZmZpeEljb24iCiAgICAgIDpjbGFzcz0iJHN0eWxlWydvcHMtYnV0dG9uX19pbWcnXSIKICAgICAgOnNyYz0iZ2V0SW1hZ2VVcmwoYGFzc2V0cy9pY29ucy8ke3N1ZmZpeEljb259LnN2Z2ApIgogICAgICBhbHQ9Imljb24iCiAgICAvPgogIDwvYnV0dG9uPgo8L3RlbXBsYXRlPgoKPHNjcmlwdCBsYW5nPSJ0cyIgc2V0dXA+CmltcG9ydCB7IFByb3BUeXBlIH0gZnJvbSAidnVlIjsKaW1wb3J0IHsgZ2V0SW1hZ2VVcmwgfSBmcm9tICJAL2hlbHBlcnMvaW1wb3J0LWltYWdlIjsKCmRlZmluZVByb3BzKHsKICBwcmVmaXhJY29uOiB7CiAgICB0eXBlOiBTdHJpbmcgYXMgUHJvcFR5cGU8c3RyaW5nPiwKICAgIGRlZmF1bHQ6ICIiLAogIH0sCiAgc3VmZml4SWNvbjogewogICAgdHlwZTogU3RyaW5nIGFzIFByb3BUeXBlPHN0cmluZz4sCiAgICBkZWZhdWx0OiAiIiwKICB9LAp9KTsKPC9zY3JpcHQ+CjxzdHlsZSBsYW5nPSJzY3NzIiBtb2R1bGU+Ci5vcHMtYnV0dG9uIHsKICAmX19pbWcgewogICAgQGFwcGx5IHctNiBoLTYgYmxvY2sgdHJhbnNpdGlvbi1hbGwgZHVyYXRpb24tMjAwOwogICAgZmlsdGVyOiBpbnZlcnQoMzMlKSBzZXBpYSg2JSkgc2F0dXJhdGUoMzg2NyUpIGh1ZS1yb3RhdGUoMTkwZGVnKQogICAgICBicmlnaHRuZXNzKDk2JSkgY29udHJhc3QoNzUlKSAhaW1wb3J0YW50OwogIH0KfQo8L3N0eWxlPgo=",
     E0 = "data:application/octet-stream;base64,PHRlbXBsYXRlPgogIDxkaXYKICAgIDpjbGFzcz0iWwogICAgICAkc3R5bGVbJ29wcy1yb29tcy1zZWFyY2gnXSwKICAgICAgeyBbJHN0eWxlWydvcHMtcm9vbXMtc2VhcmNoX19mb2N1cyddXTogaXNGb2N1c2VkIH0sCiAgICBdIgogID4KICAgIDxzbG90IG5hbWU9InByZWZpeCIgLz4KICAgIDxpbnB1dAogICAgICByZWY9ImlucHV0UmVmIgogICAgICA6Y2xhc3M9IiRzdHlsZVsnb3BzLXJvb21zLXNlYXJjaF9faW5wdXQnXSIKICAgICAgOnBsYWNlaG9sZGVyPSJwbGFjZWhvbGRlciB8fCAnVHlwZS4uLiciCiAgICAgIDp2YWx1ZT0ibW9kZWxWYWx1ZSIKICAgICAgdHlwZT0idGV4dCIKICAgICAgQGZvY3VzPSJpc0ZvY3VzZWQgPSB0cnVlIgogICAgICBAYmx1cj0ib25CbHVyIgogICAgICBAaW5wdXQ9ImhhbmRsZUlucHV0IgogICAgLz4KICAgIDxzbG90IG5hbWU9InN1ZmZpeCIgLz4KICA8L2Rpdj4KPC90ZW1wbGF0ZT4KCjxzY3JpcHQgbGFuZz0idHMiIHNldHVwPgppbXBvcnQgeyBjb21wdXRlZCwgUHJvcFR5cGUsIHJlZiB9IGZyb20gInZ1ZSI7CgpkZWZpbmVQcm9wcyh7CiAgbW9kZWxWYWx1ZTogewogICAgdHlwZTogU3RyaW5nIGFzIFByb3BUeXBlPHN0cmluZz4sCiAgICBkZWZhdWx0OiAiIiwKICB9LAogIHBsYWNlaG9sZGVyOiB7CiAgICB0eXBlOiBTdHJpbmcgYXMgUHJvcFR5cGU8c3RyaW5nPiwKICAgIGRlZmF1bHQ6ICIiLAogIH0sCn0pOwpjb25zdCBpbnB1dFJlZiA9IHJlZihudWxsKTsKY29uc3QgZW1pdCA9IGRlZmluZUVtaXRzPHsKICAoZTogInVwZGF0ZTptb2RlbFZhbHVlIiwgdjogc3RyaW5nKTogdm9pZDsKICAoZTogImJsdXIiKTogdm9pZDsKfT4oKTsKCmNvbnN0IGlzRm9jdXNlZCA9IHJlZihmYWxzZSk7Cgpjb25zdCBoYW5kbGVJbnB1dCA9IChldmVudDogRXZlbnQpID0+IHsKICBjb25zdCBpbnB1dEVsZW1lbnQgPSBldmVudD8udGFyZ2V0IGFzIEhUTUxJbnB1dEVsZW1lbnQgfCBudWxsOwoKICBpZiAoaW5wdXRFbGVtZW50KSB7CiAgICBjb25zdCBpbnB1dFZhbHVlID0gaW5wdXRFbGVtZW50LnZhbHVlOwogICAgZW1pdCgidXBkYXRlOm1vZGVsVmFsdWUiLCBpbnB1dFZhbHVlKTsKICB9Cn07Cgpjb25zdCBvbkJsdXIgPSAoKSA9PiB7CiAgaXNGb2N1c2VkLnZhbHVlID0gZmFsc2U7CiAgZW1pdCgiYmx1ciIpOwp9OwoKZGVmaW5lRXhwb3NlKHsgaW5wdXRSZWY6IGNvbXB1dGVkKCgpID0+IGlucHV0UmVmLnZhbHVlKSB9KTsKPC9zY3JpcHQ+Cgo8c3R5bGUgbGFuZz0ic2NzcyIgbW9kdWxlPgoub3BzLXJvb21zLXNlYXJjaCB7CiAgQGFwcGx5IGZsZXggaXRlbXMtY2VudGVyIGZvY3VzOm91dGxpbmUtbm9uZSB0ZXh0LWdyZXktcGFsZSB3LWZ1bGwgIGJvcmRlci1ncmV5LW1pc2Noa2EgYm9yZGVyLVswLjA2MjVyZW1dIHJvdW5kZWQtWzIuNXJlbV0gcHktMiBweC0zOwogIGJveC1zaGFkb3c6IDAgMXB4IDJweCAwIHJnYmEoMCwgMCwgMCwgMC4wNyk7CiAgdHJhbnNpdGlvbjogYm9yZGVyLWNvbG9yIDAuMTVzIGVhc2UtaW4tb3V0LCBib3gtc2hhZG93IDAuMTVzIGVhc2UtaW4tb3V0OwoKICAmX19pY29uIHsKICAgIEBhcHBseSBoLTQgdy00IG9wYWNpdHktNTAgbXItMjsKICB9CgogICZfX2lucHV0IHsKICAgIEBhcHBseSB3LWZ1bGwgcHktMCBweC0wIGJnLXRyYW5zcGFyZW50IGJvcmRlci0wIG91dGxpbmUtbm9uZTsKICB9CgogICZfX2ZvY3VzIHsKICAgIEBhcHBseSBiZy13aGl0ZSBib3JkZXItZ3JleS1uZXBhbCBvdXRsaW5lLTA7CiAgfQp9Cjwvc3R5bGU+Cg==",
     H0 = "data:application/octet-stream;base64,PHRlbXBsYXRlPgogIDxkaXYgOmNsYXNzPSIkc3R5bGVbJ2xvYWRlciddIiAvPgo8L3RlbXBsYXRlPgoKPHN0eWxlIGxhbmc9InNjc3MiIG1vZHVsZT4KLmxvYWRlciB7CiAgYW5pbWF0aW9uOiByb3RhdGUgMXMgbGluZWFyIGluZmluaXRlOwogIEBhcHBseSB3LVsyNHB4XSBoLVsyNHB4XSBteC1hdXRvIHJvdW5kZWQtZnVsbCBibG9jayByZWxhdGl2ZTsKCiAgJjo6YmVmb3JlIHsKICAgIGNvbnRlbnQ6ICIiOwogICAgYW5pbWF0aW9uOiBwcml4Q2xpcEZpeCAycyBsaW5lYXIgaW5maW5pdGU7CiAgICBAYXBwbHkgYWJzb2x1dGUgcm91bmRlZC1mdWxsIGJvcmRlci1bM3B4XSBib3JkZXItZ3JleS1rYXNobWlyIGJveC1ib3JkZXIgaW5zZXQtMDsKICB9Cn0KCkBrZXlmcmFtZXMgcm90YXRlIHsKICAxMDAlIHsKICAgIHRyYW5zZm9ybTogcm90YXRlKDM2MGRlZyk7CiAgfQp9CgpAa2V5ZnJhbWVzIHByaXhDbGlwRml4IHsKICAwJSB7CiAgICBjbGlwLXBhdGg6IHBvbHlnb24oNTAlIDUwJSwgMCAwLCAwIDAsIDAgMCwgMCAwLCAwIDApOwogIH0KICAyNSUgewogICAgY2xpcC1wYXRoOiBwb2x5Z29uKDUwJSA1MCUsIDAgMCwgMTAwJSAwLCAxMDAlIDAsIDEwMCUgMCwgMTAwJSAwKTsKICB9CiAgNTAlIHsKICAgIGNsaXAtcGF0aDogcG9seWdvbig1MCUgNTAlLCAwIDAsIDEwMCUgMCwgMTAwJSAxMDAlLCAxMDAlIDEwMCUsIDEwMCUgMTAwJSk7CiAgfQogIDc1JSB7CiAgICBjbGlwLXBhdGg6IHBvbHlnb24oNTAlIDUwJSwgMCAwLCAxMDAlIDAsIDEwMCUgMTAwJSwgMCAxMDAlLCAwIDEwMCUpOwogIH0KICAxMDAlIHsKICAgIGNsaXAtcGF0aDogcG9seWdvbig1MCUgNTAlLCAwIDAsIDEwMCUgMCwgMTAwJSAxMDAlLCAwIDEwMCUsIDAgMCk7CiAgfQp9Cjwvc3R5bGU+Cg==",
     O0 = "data:application/octet-stream;base64,PHRlbXBsYXRlPgogIDxkaXYKICAgIHYtY2xpY2stb3V0c2lkZT0iY2xvc2VIZWFkZXJNZW51IgogICAgdi1iaW5kPSIkYXR0cnMiCiAgICA6Y2xhc3M9IiRzdHlsZVsnb3BzLXJvb20taGVhZGVyX19idXR0b24nXSIKICAgIEBjbGljaz0ibWVudU9wZW5lZCA9ICFtZW51T3BlbmVkIgogID4KICAgIDxpbWcKICAgICAgOnNyYz0iZ2V0SW1hZ2VVcmwoYGFzc2V0cy9pY29ucy8ke2ljb24gfHwgJ2hlYWRlci1jaGF0LW1lbnUnfS5zdmdgKSIKICAgICAgYWx0PSJtZW51IgogICAgLz4KICA8L2Rpdj4KICA8dHJhbnNpdGlvbiBuYW1lPSJvcHMtc2xpZGUtbGVmdCI+CiAgICA8ZGl2IHYtaWY9Im1lbnVPcGVuZWQiIDpjbGFzcz0iJHN0eWxlWydvcHMtaGVhZGVyLW1lbnUtb3B0aW9ucyddIj4KICAgICAgPGRpdiB2LWlmPSJvcHRpb25zIiA6Y2xhc3M9IiRzdHlsZVsnb3BzLWhlYWRlci1tZW51LW9wdGlvbnNfX2xpc3QnXSI+CiAgICAgICAgPGRpdgogICAgICAgICAgdi1mb3I9ImFjdGlvbiBpbiBvcHRpb25zIgogICAgICAgICAgOmtleT0iYWN0aW9uLmlkIgogICAgICAgICAgOmNsYXNzPSIkc3R5bGVbJ29wcy1oZWFkZXItbWVudS1vcHRpb25zX19saXN0LWl0ZW0nXSIKICAgICAgICAgIEBjbGljaz0ib25TZWxlY3RPcHRpb24oYWN0aW9uKSIKICAgICAgICA+CiAgICAgICAgICB7eyBhY3Rpb24udGl0bGUgfX0KICAgICAgICA8L2Rpdj4KICAgICAgPC9kaXY+CiAgICA8L2Rpdj4KICA8L3RyYW5zaXRpb24+CjwvdGVtcGxhdGU+Cgo8c2NyaXB0IHNldHVwIGxhbmc9InRzIj4KaW1wb3J0IHsgZ2V0SW1hZ2VVcmwgfSBmcm9tICJAL2hlbHBlcnMvaW1wb3J0LWltYWdlIjsKaW1wb3J0IHsgUHJvcFR5cGUsIHJlZiB9IGZyb20gInZ1ZSI7CmltcG9ydCB7IElNZW51QWN0aW9ucyB9IGZyb20gIkAvdHlwZXMvcm9vbS9yb29tLnR5cGVzIjsKCmRlZmluZVByb3BzKHsKICBvcHRpb25zOiB7CiAgICB0eXBlOiBBcnJheSBhcyBQcm9wVHlwZTxJTWVudUFjdGlvbnNbXT4sCiAgICBkZWZhdWx0OiAoKSA9PiB7CiAgICAgIHJldHVybiBbCiAgICAgICAgeyBpZDogImludml0ZVVzZXIiLCB0aXRsZTogIkludml0ZSBVc2VyIiwgZW1pdEFjdGlvbjogImludml0ZS11c2VyIiB9LAogICAgICAgIHsgaWQ6ICJyZW1vdmVVc2VyIiwgdGl0bGU6ICJSZW1vdmUgVXNlciIsIGVtaXRBY3Rpb246ICJyZW1vdmUtdXNlciIgfSwKICAgICAgICB7IGlkOiAiZGVsZXRlUm9vbSIsIHRpdGxlOiAiRGVsZXRlIFJvb20iLCBlbWl0QWN0aW9uOiAiZGVsZXRlLXVzZXIiIH0sCiAgICAgIF07CiAgICB9LAogIH0sCiAgaWNvbjogewogICAgdHlwZTogU3RyaW5nLAogICAgZGVmYXVsdDogIiIsCiAgfSwKfSk7CmNvbnN0IGVtaXQgPSBkZWZpbmVFbWl0czx7CiAgKGU6ICJibHVyIik6IHZvaWQ7CiAgKGU6ICJyZXBseSIpOiB2b2lkOwogIChlOiAiZWRpdC1tZXNzYWdlIik6IHZvaWQ7CiAgKGU6ICJkZWxldGUtbWVzc2FnZSIpOiB2b2lkOwogIChlOiAiaW52aXRlLXVzZXIiKTogdm9pZDsKICAoZTogInJlbW92ZS11c2VyIik6IHZvaWQ7CiAgKGU6ICJkZWxldGUtdXNlciIpOiB2b2lkOwp9PigpOwoKY29uc3QgbWVudU9wZW5lZCA9IHJlZihmYWxzZSk7Cgpjb25zdCBvblNlbGVjdE9wdGlvbiA9IChhY3Rpb246IElNZW51QWN0aW9ucykgPT4gewogIGVtaXQoYWN0aW9uLmVtaXRBY3Rpb24gYXMgYW55KTsKICBjbG9zZUhlYWRlck1lbnUoKTsKfTsKY29uc3QgY2xvc2VIZWFkZXJNZW51ID0gKCkgPT4gewogIG1lbnVPcGVuZWQudmFsdWUgPSBmYWxzZTsKICBlbWl0KCJibHVyIik7Cn07Cjwvc2NyaXB0PgoKPHN0eWxlIGxhbmc9InNjc3MiIG1vZHVsZT4KLm9wcy1oZWFkZXItbWVudS1vcHRpb25zIHsKICBAYXBwbHkgaW5saW5lLWJsb2NrIHRleHQtWzAuODc1cmVtXSB0b3AtWzNyZW1dIHRleHQtZ3JleS1rYXNobWlyIHJpZ2h0LVsxcmVtXSBtaW4tdy1bOC4zNzVyZW1dIHJvdW5kZWQgYWJzb2x1dGUgb3ZlcmZsb3cteS1hdXRvIG92ZXJmbG93LXgtaGlkZGVuIHotWzk5OTldOwogIGNvbnRhaW46IGNvbnRlbnQ7CiAgYm94LXNoYWRvdzogMCAycHggMnB4IC00cHggcmdiYSgwLCAwLCAwLCAwLjEpLAogICAgMCAycHggMnB4IDFweCByZ2JhKDAsIDAsIDAsIDAuMTIpLCAwIDFweCA4cHggMXB4IHJnYmEoMCwgMCwgMCwgMC4xMik7CgogICZfX2xpc3QgewogICAgQGFwcGx5IGJsb2NrIHJvdW5kZWQgY3Vyc29yLXBvaW50ZXIgcHgtMCBweS0wIGJnLXdoaXRlOwoKICAgIDpob3ZlciB7CiAgICAgIEBhcHBseSBiZy1jb25mZXR0aS0xMDA7CiAgICAgIHRyYW5zaXRpb246IGJhY2tncm91bmQtY29sb3IgMC4zcyBjdWJpYy1iZXppZXIoMC4yNSwgMC44LCAwLjUsIDEpOwogICAgfQoKICAgIDpub3QoOmhvdmVyKSB7CiAgICAgIHRyYW5zaXRpb246IGJhY2tncm91bmQtY29sb3IgMC4zcyBjdWJpYy1iZXppZXIoMC4yNSwgMC44LCAwLjUsIDEpOwogICAgfQogIH0KCiAgJl9fbGlzdC1pdGVtIHsKICAgIEBhcHBseSBmbGV4IGl0ZW1zLWNlbnRlciByZWxhdGl2ZSBsZWFkaW5nLTggd2hpdGVzcGFjZS1ub3dyYXAgcHktWzAuMnJlbV0gcHgtNDsKICB9Cn0KPC9zdHlsZT4K",
     L0 = "data:video/mp2t;base64,aW1wb3J0IGNoYXRTZXJ2aWNlIGZyb20gIkAvc2VydmljZXMvY2hhdC9jaGF0IjsKaW1wb3J0IHsgcmVmIH0gZnJvbSAidnVlIjsKaW1wb3J0IHdlYnNvY2tldFNlcnZpY2UgZnJvbSAiQC9zZXJ2aWNlcy9jaGF0L3dlYnNvY2tldC1jaGF0IjsKaW1wb3J0IHsgcHJldmVudEJvdHRvbVNjcm9sbGluZyB9IGZyb20gIkAvaGVscGVycy9zY3JvbGwiOwoKZXhwb3J0IGNvbnN0IHVzZUludGVyc2VjdGlvbiA9IChyb29tSWQ6IHN0cmluZywgZWxlbWVudFNlbGVjdG9yOiBzdHJpbmcpID0+IHsKICBjb25zdCBsb2FkaW5nID0gcmVmKGZhbHNlKTsKICBjb25zdCBwYWdlID0gcmVmKDIpOwoKICBjb25zdCBpbnRlcnNlY3Rpb25CbG9jayA9ICgpID0+IHsKICAgIGNvbnN0IGludGVyc2VjdGlvbkVsZW1lbnQgPSBkb2N1bWVudC5xdWVyeVNlbGVjdG9yKAogICAgICBlbGVtZW50U2VsZWN0b3IKICAgICkgYXMgSFRNTEVsZW1lbnQ7CiAgICBpZiAoIWludGVyc2VjdGlvbkVsZW1lbnQpIHJldHVybiBudWxsOwoKICAgIGNvbnN0IGxhc3RNZXNzYWdlVGltZSA9IHdlYnNvY2tldFNlcnZpY2UubWVzc2FnZXMudmFsdWUuYXQoLTEpPy50aW1lc3RhbXA7CgogICAgY29uc3Qgb25JbnRlcnNlY3Rpb24gPSBhc3luYyAoZW50cnk6IGFueSkgPT4gewogICAgICBpZiAoZW50cnkuYXQoMCkuaXNJbnRlcnNlY3RpbmcpIHsKICAgICAgICB0cnkgewogICAgICAgICAgbG9hZGluZy52YWx1ZSA9IHRydWU7CgogICAgICAgICAgY29uc3QgZGF0YSA9IGF3YWl0IGNoYXRTZXJ2aWNlLmZldGNoUmVjZW50TWVzc2FnZXMoCiAgICAgICAgICAgIHJvb21JZCwKICAgICAgICAgICAgcGFnZS52YWx1ZSwKICAgICAgICAgICAgeyBwYXJhbXM6IHsgb2xkZXJfdGhhbjogbGFzdE1lc3NhZ2VUaW1lIH0gfQogICAgICAgICAgKTsKCiAgICAgICAgICB3ZWJzb2NrZXRTZXJ2aWNlLm1lc3NhZ2VzLnZhbHVlID0gWwogICAgICAgICAgICAuLi5kYXRhLnJlc3VsdHMucmV2ZXJzZSgpLAogICAgICAgICAgICAuLi53ZWJzb2NrZXRTZXJ2aWNlLm1lc3NhZ2VzLnZhbHVlLAogICAgICAgICAgXTsKICAgICAgICAgIGxvYWRpbmcudmFsdWUgPSBmYWxzZTsKICAgICAgICAgIGNoZWNrSWZOZXh0RXhpc3RzKGRhdGEubmV4dCk7CiAgICAgICAgICBwcmV2ZW50Qm90dG9tU2Nyb2xsaW5nKCIudnVlLXJlY3ljbGUtc2Nyb2xsZXIiKTsKICAgICAgICB9IGNhdGNoIChlOiBhbnkpIHsKICAgICAgICAgIGNvbnNvbGUubG9nKGUsICJ1c2UtaW50ZXJzZWN0aW9uIik7CiAgICAgICAgICB0aHJvdyBuZXcgRXJyb3IoIlNvbWV0aGluZyB3ZW50IHdyb25nIik7CiAgICAgICAgfQogICAgICB9CiAgICB9OwogICAgY29uc3Qgb2JzZXJ2ZXI6IEludGVyc2VjdGlvbk9ic2VydmVyID0gbmV3IEludGVyc2VjdGlvbk9ic2VydmVyKAogICAgICBvbkludGVyc2VjdGlvbiwKICAgICAgewogICAgICAgIHJvb3Q6IG51bGwsCiAgICAgICAgdGhyZXNob2xkOiAwLjUsCiAgICAgIH0KICAgICk7CiAgICBvYnNlcnZlci5vYnNlcnZlKGludGVyc2VjdGlvbkVsZW1lbnQpOwoKICAgIGNvbnN0IGNoZWNrSWZOZXh0RXhpc3RzID0gKG5leHQ6IHN0cmluZyB8IG51bGwpID0+IHsKICAgICAgaWYgKG5leHQpIHsKICAgICAgICBwYWdlLnZhbHVlICs9IDE7CiAgICAgIH0gZWxzZSB7CiAgICAgICAgb2JzZXJ2ZXIudW5vYnNlcnZlKGludGVyc2VjdGlvbkVsZW1lbnQpOwogICAgICB9CiAgICB9OwogIH07CiAgcmV0dXJuIHsKICAgIGxvYWRpbmcsCiAgICBwYWdlLAogICAgaW50ZXJzZWN0aW9uQmxvY2ssCiAgfTsKfTsK",
     U0 = "data:video/mp2t;base64,aW1wb3J0IHsgaXNJblZpZXdwb3J0IH0gZnJvbSAiQC9oZWxwZXJzL3Njcm9sbCI7CmltcG9ydCB3ZWJzb2NrZXRTZXJ2aWNlIGZyb20gIkAvc2VydmljZXMvY2hhdC93ZWJzb2NrZXQtY2hhdCI7CmltcG9ydCB7IFdTX1RZUEVTIH0gZnJvbSAiQC90eXBlcy9nZW5lcmFsLnR5cGVzIjsKaW1wb3J0IHsgSU1lc3NhZ2UgfSBmcm9tICJAL3R5cGVzL3Jvb20vcm9vbS50eXBlcyI7CmltcG9ydCB7IENvbXB1dGVkUmVmLCBvbkJlZm9yZVVubW91bnQsIG9uTW91bnRlZCB9IGZyb20gInZ1ZSI7CgpleHBvcnQgY29uc3QgdXNlSXNSZWFkTWVzc2FnZSA9ICgKICBtZXNzYWdlRGF0YTogQ29tcHV0ZWRSZWY8SU1lc3NhZ2U+LAogIHRhcmdldElkOiBzdHJpbmcsCiAgdXNlcklkOiBudW1iZXIKKSA9PiB7CiAgY29uc3QgY2hlY2tJbnRvVmlldyA9ICgpID0+IHsKICAgIGlmICgKICAgICAgaXNJblZpZXdwb3J0KGBtZXNzYWdlLSR7bWVzc2FnZURhdGEudmFsdWUuaWR9YCkgJiYKICAgICAgIW1lc3NhZ2VEYXRhLnZhbHVlLmlzX3JlYWQgJiYKICAgICAgbWVzc2FnZURhdGEudmFsdWUuYXV0aG9yLmlkICE9PSB1c2VySWQKICAgICkgewogICAgICB3ZWJzb2NrZXRTZXJ2aWNlLnNlbmRNZXNzYWdlKHsKICAgICAgICB0eXBlOiBXU19UWVBFUy5SRUFEX01FU1NBR0VTLAogICAgICB9KTsKICAgIH0KICB9OwoKICBvbk1vdW50ZWQoKCkgPT4gewogICAgY29uc3QgY29udGVudE1lc3NhZ2VzID0gZG9jdW1lbnQuZ2V0RWxlbWVudEJ5SWQodGFyZ2V0SWQpIGFzIEhUTUxFbGVtZW50OwogICAgY29udGVudE1lc3NhZ2VzLmFkZEV2ZW50TGlzdGVuZXIoInNjcm9sbCIsIGNoZWNrSW50b1ZpZXcpOwogIH0pOwogIG9uQmVmb3JlVW5tb3VudCgoKSA9PiB7CiAgICBjb25zdCBjb250ZW50TWVzc2FnZXMgPSBkb2N1bWVudC5nZXRFbGVtZW50QnlJZCh0YXJnZXRJZCkgYXMgSFRNTEVsZW1lbnQ7CiAgICBjb250ZW50TWVzc2FnZXMucmVtb3ZlRXZlbnRMaXN0ZW5lcigic2Nyb2xsIiwgY2hlY2tJbnRvVmlldyk7CiAgfSk7Cn07Cg==",
     J0 = "data:video/mp2t;base64,aW1wb3J0IHsgRGlyZWN0aXZlQmluZGluZywgT2JqZWN0RGlyZWN0aXZlIH0gZnJvbSAidnVlIjsKCmludGVyZmFjZSBIVE1MRWxlbWVudFdpdGhDbGlja091dHNpZGVFdmVudCBleHRlbmRzIEhUTUxFbGVtZW50IHsKICBjbGlja091dHNpZGVFdmVudD86IChldmVudDogTW91c2VFdmVudCkgPT4gdm9pZDsKfQoKY29uc3QgY2xpY2tPdXRTaWRlOiBPYmplY3REaXJlY3RpdmU8SFRNTEVsZW1lbnRXaXRoQ2xpY2tPdXRzaWRlRXZlbnQ+ID0gewogIG1vdW50ZWQoCiAgICBlbDogSFRNTEVsZW1lbnRXaXRoQ2xpY2tPdXRzaWRlRXZlbnQsCiAgICBiaW5kaW5nOiBEaXJlY3RpdmVCaW5kaW5nPChldmVudDogTW91c2VFdmVudCkgPT4gdm9pZD4KICApIHsKICAgIGNvbnN0IGhhbmRsZUNsaWNrT3V0c2lkZSA9IChldmVudDogTW91c2VFdmVudCkgPT4gewogICAgICBpZiAoIShlbCA9PT0gZXZlbnQudGFyZ2V0IHx8IGVsLmNvbnRhaW5zKGV2ZW50LnRhcmdldCBhcyBOb2RlKSkpIHsKICAgICAgICBiaW5kaW5nLnZhbHVlKGV2ZW50KTsKICAgICAgfQogICAgfTsKICAgIGVsLmNsaWNrT3V0c2lkZUV2ZW50ID0gaGFuZGxlQ2xpY2tPdXRzaWRlOwogICAgZG9jdW1lbnQuYWRkRXZlbnRMaXN0ZW5lcigiY2xpY2siLCBoYW5kbGVDbGlja091dHNpZGUpOwogIH0sCiAgdW5tb3VudGVkKGVsOiBIVE1MRWxlbWVudFdpdGhDbGlja091dHNpZGVFdmVudCkgewogICAgZG9jdW1lbnQucmVtb3ZlRXZlbnRMaXN0ZW5lcigKICAgICAgImNsaWNrIiwKICAgICAgZWwuY2xpY2tPdXRzaWRlRXZlbnQgYXMgKGV2ZW50OiBNb3VzZUV2ZW50KSA9PiB2b2lkCiAgICApOwogICAgZWwuY2xpY2tPdXRzaWRlRXZlbnQgPSB1bmRlZmluZWQ7CiAgfSwKfTsKCmV4cG9ydCBkZWZhdWx0IGNsaWNrT3V0U2lkZTsK",
     K0 = "data:video/mp2t;base64,ZXhwb3J0IHt9OwoKZGVjbGFyZSBnbG9iYWwgewogIGludGVyZmFjZSBXaW5kb3cgewogICAgYXBpX3Rva2VuOiBzdHJpbmc7CiAgfQp9Cg==",
-    P0 = "data:video/mp2t;base64,aW1wb3J0IHsgdXNlVXNlclN0b3JlIH0gZnJvbSAiQC9zdG9yZS91c2VVc2VyU3RvcmUiOwoKZXhwb3J0IGNvbnN0IGdlbmVyYXRlSUQgPSAoKSA9PgogIERhdGUubm93KCkudG9TdHJpbmcoMzYpICsgTWF0aC5yYW5kb20oKS50b1N0cmluZygzNikuc3Vic3RyKDIpOwoKLyoqCiAqIFJldHVybnMgdG9rZW4gYmFzZWQgb24gYnVpbGQgbW9kZQogKiovCmV4cG9ydCBjb25zdCBnZXRDaGF0QXBpVG9rZW4gPSAoKSA9PiB7CiAgaWYgKGltcG9ydC5tZXRhLmVudi5ERVYpIHsKICAgIHJldHVybiBpbXBvcnQubWV0YS5lbnYuVklURV9BUElfVE9LRU47CiAgfQogIHJldHVybiB3aW5kb3cuYXBpX3Rva2VuOwp9OwovKioKICogUmV0dXJucyBob3N0bmFtZQogKiovCmV4cG9ydCBjb25zdCBnZXREb21haW5OYW1lID0gKCkgPT4gewogIGlmIChpbXBvcnQubWV0YS5lbnYuREVWKSB7CiAgICByZXR1cm4gaW1wb3J0Lm1ldGEuZW52LlZJVEVfQkFTRV9VUkw7CiAgfQogIHJldHVybiB3aW5kb3cubG9jYXRpb24uaG9zdG5hbWU7Cn07CgpleHBvcnQgY29uc3QgcmVtb3ZlT3duSWRPbmxpbmUgPSAodXNlcnM6IG51bWJlcltdKSA9PiB7CiAgaWYgKEFycmF5LmlzQXJyYXkodXNlcnMpKSB7CiAgICBjb25zdCB1c2VyU3RvcmUgPSB1c2VVc2VyU3RvcmUoKTsKICAgIGNvbnN0IHBlcnNvbklkID0gdXNlclN0b3JlLmdldFVzZXI/LnBlcnNvbj8uaWQ7CiAgICBjb25zdCByZW1vdmVPd25JZCA9IHVzZXJzLmZpbHRlcigoZWwpID0+IGVsICE9PSBwZXJzb25JZCk7CiAgICByZXR1cm4gcmVtb3ZlT3duSWQubGVuZ3RoOwogIH0KICByZXR1cm4gMDsKfTsKCmV4cG9ydCBjb25zdCBnZXRXc1Byb3RvY29sID0gKCkgPT4gewogIGlmICh3aW5kb3cubG9jYXRpb24ucHJvdG9jb2wgPT09ICJodHRwczoiKSB7CiAgICByZXR1cm4gIndzczovLyI7CiAgfSBlbHNlIGlmIChpbXBvcnQubWV0YS5lbnYuREVWKSB7CiAgICByZXR1cm4gIndzczovLyI7CiAgfSBlbHNlIHsKICAgIHJldHVybiAid3M6Ly8iOwogIH0KfTsKCmV4cG9ydCBjb25zdCBnZXRUcmFuc2ZlclByb3RvY29sID0gKCkgPT4gewogIGlmICh3aW5kb3cubG9jYXRpb24ucHJvdG9jb2wgPT09ICJodHRwczoiKSB7CiAgICByZXR1cm4gImh0dHBzOi8vIjsKICB9IGVsc2UgaWYgKGltcG9ydC5tZXRhLmVudi5ERVYpIHsKICAgIHJldHVybiAiaHR0cHM6Ly8iOwogIH0gZWxzZSB7CiAgICByZXR1cm4gImh0dHA6IjsKICB9Cn07Cg==",
-    F0 = "data:video/mp2t;base64,LyoqCiAqIENoYW5nZSBzY3JvbGwgcG9zaXRpb24gYXQgYm90dG9tIG9mIHRoZSBlbGVtZW50CiAqCiAqIEBwYXJhbSBzZWxlY3RvciAtIGNsYXNzIHNlbGVjdG9yIG9mIGVsZW1lbnQKICovCmV4cG9ydCBjb25zdCBzY3JvbGxUb0JvdHRvbSA9IChzZWxlY3Rvcjogc3RyaW5nKTogdm9pZCA9PiB7CiAgY29uc3QgZWxlbWVudCA9IGRvY3VtZW50LnF1ZXJ5U2VsZWN0b3Ioc2VsZWN0b3IpIGFzIEhUTUxFbGVtZW50OwogIGVsZW1lbnQuc2Nyb2xsVG9wID0gZWxlbWVudC5zY3JvbGxIZWlnaHQ7Cn07Ci8qKgogKiBQcmV2ZW50aW5nIHNjcm9sbGluZyB0byBib3R0b20KICogQHNlbGVjdG9yIC0gY2xhc3Mgc2VsZWN0b3Igb2YgbWVzc2FnZSBlbGVtZW50CiAqKi8KZXhwb3J0IGNvbnN0IHByZXZlbnRCb3R0b21TY3JvbGxpbmcgPSAoc2VsZWN0b3I6IHN0cmluZykgPT4gewogIGNvbnN0IGVsZW1lbnQgPSBkb2N1bWVudC5xdWVyeVNlbGVjdG9yKHNlbGVjdG9yKSBhcyBIVE1MRWxlbWVudDsKCiAgY29uc3QgY3VycmVudFNjcm9sbEhlaWdodCA9IGVsZW1lbnQuc2Nyb2xsSGVpZ2h0OwogIGNvbnN0IG9ic2VydmVyID0gbmV3IFJlc2l6ZU9ic2VydmVyKCgpID0+IHsKICAgIGVsZW1lbnQuc2Nyb2xsVG9wID0gZWxlbWVudC5zY3JvbGxIZWlnaHQgLSBjdXJyZW50U2Nyb2xsSGVpZ2h0OwogIH0pOwogIG9ic2VydmVyLm9ic2VydmUoZWxlbWVudCk7Cn07Ci8qKgogKiBNZXRob2QgY2hlY2tlZCBpZiBlbGVtZW50IG1lc3NhZ2UgcG9zaXRpb24gaW4gYm90dG9tIG9mIGVsZW1lbnQKICogQHNlbGVjdG9yIC0gY2xhc3Mgc2VsZWN0b3Igb2YgbWVzc2FnZSBlbGVtZW50CiAqKi8KZXhwb3J0IGNvbnN0IGNoZWNrSWZCb3R0b21TY3JvbGwgPSAoc2VsZWN0b3I6IHN0cmluZykgPT4gewogIGNvbnN0IGVsZW1lbnQgPSBkb2N1bWVudC5xdWVyeVNlbGVjdG9yKHNlbGVjdG9yKSBhcyBIVE1MRWxlbWVudDsKICBjb25zdCBlbGVtZW50Qm94ID0gZG9jdW1lbnQucXVlcnlTZWxlY3RvckFsbCgKICAgICIudnVlLXJlY3ljbGUtc2Nyb2xsZXJfX2l0ZW0tdmlldzpsYXN0LWNoaWxkIgogICkgYXMgTm9kZUxpc3RPZjxIVE1MRWxlbWVudD47CiAgaWYgKGVsZW1lbnQpIHsKICAgIHJldHVybiAoCiAgICAgIE1hdGguYWJzKAogICAgICAgIGVsZW1lbnQuc2Nyb2xsSGVpZ2h0IC0gZWxlbWVudC5zY3JvbGxUb3AgLSBlbGVtZW50LmNsaWVudEhlaWdodAogICAgICApIDw9IGVsZW1lbnRCb3hbMF0uY2xpZW50SGVpZ2h0CiAgICApOwogIH0KICByZXR1cm4gZmFsc2U7Cn07Ci8qKgogKiBNZXRob2QgY2hlY2tlZCBpZiBtZXNzYWdlIGlzIGluIHZpZXdwb3J0CiAqIEBpZCAtIGlkZW50aWZpY2F0aW9uIG9mIG1lc3NhZ2UgZWxlbWVudAogKiovCmV4cG9ydCBjb25zdCBpc0luVmlld3BvcnQgPSAoaWQ6IHN0cmluZykgPT4gewogIGNvbnN0IG1lc3NhZ2VzQm94ID0gZG9jdW1lbnQuZ2V0RWxlbWVudEJ5SWQoYHJvb20tbWVzc2FnZXNgKSBhcyBIVE1MRWxlbWVudDsKICBjb25zdCBlbGVtZW50ID0gZG9jdW1lbnQuZ2V0RWxlbWVudEJ5SWQoaWQpIGFzIEhUTUxFbGVtZW50OwogIGlmIChlbGVtZW50KSB7CiAgICBjb25zdCByZWN0ID0gZWxlbWVudD8uZ2V0Qm91bmRpbmdDbGllbnRSZWN0KCk7CiAgICByZXR1cm4gKAogICAgICByZWN0Py50b3AgPj0gMCAmJgogICAgICByZWN0Py5sZWZ0ID49IDAgJiYKICAgICAgcmVjdD8uYm90dG9tIDw9IG1lc3NhZ2VzQm94LmdldEJvdW5kaW5nQ2xpZW50UmVjdCgpLmJvdHRvbSAmJgogICAgICByZWN0Py5yaWdodCA8PSBtZXNzYWdlc0JveC5nZXRCb3VuZGluZ0NsaWVudFJlY3QoKS5yaWdodAogICAgKTsKICB9CiAgcmV0dXJuIGZhbHNlOwp9OwoKLyoqCiAqIE1ldGhvZCBjaGVjayBpZiBlbGVtZW50IGhhcyBzY3JvbGxiYXIKICogQGlkIC0gaWQgb2YgZWxlbWVudAogKiAqKi8KZXhwb3J0IGNvbnN0IGhhc1Njcm9sbEJhciA9IChpZDogc3RyaW5nKSA9PiB7CiAgY29uc3QgZWxlbWVudCA9IGRvY3VtZW50LmdldEVsZW1lbnRCeUlkKGlkKTsKICBpZiAoZWxlbWVudCkgewogICAgcmV0dXJuIGVsZW1lbnQuc2Nyb2xsSGVpZ2h0ID4gZWxlbWVudC5jbGllbnRIZWlnaHQ7CiAgfQogIHJldHVybiBmYWxzZTsKfTsK",
+    F0 = "data:video/mp2t;base64,aW1wb3J0IHsgdXNlVXNlclN0b3JlIH0gZnJvbSAiQC9zdG9yZS91c2VVc2VyU3RvcmUiOwoKZXhwb3J0IGNvbnN0IGdlbmVyYXRlSUQgPSAoKSA9PgogIERhdGUubm93KCkudG9TdHJpbmcoMzYpICsgTWF0aC5yYW5kb20oKS50b1N0cmluZygzNikuc3Vic3RyKDIpOwoKLyoqCiAqIFJldHVybnMgdG9rZW4gYmFzZWQgb24gYnVpbGQgbW9kZQogKiovCmV4cG9ydCBjb25zdCBnZXRDaGF0QXBpVG9rZW4gPSAoKSA9PiB7CiAgaWYgKGltcG9ydC5tZXRhLmVudi5ERVYpIHsKICAgIHJldHVybiBpbXBvcnQubWV0YS5lbnYuVklURV9BUElfVE9LRU47CiAgfQogIHJldHVybiB3aW5kb3cuYXBpX3Rva2VuOwp9OwovKioKICogUmV0dXJucyBob3N0bmFtZQogKiovCmV4cG9ydCBjb25zdCBnZXREb21haW5OYW1lID0gKCkgPT4gewogIGlmIChpbXBvcnQubWV0YS5lbnYuREVWKSB7CiAgICByZXR1cm4gaW1wb3J0Lm1ldGEuZW52LlZJVEVfQkFTRV9VUkw7CiAgfQogIHJldHVybiB3aW5kb3cubG9jYXRpb24uaG9zdDsKfTsKCmV4cG9ydCBjb25zdCByZW1vdmVPd25JZE9ubGluZSA9ICh1c2VyczogbnVtYmVyW10pID0+IHsKICBpZiAoQXJyYXkuaXNBcnJheSh1c2VycykpIHsKICAgIGNvbnN0IHVzZXJTdG9yZSA9IHVzZVVzZXJTdG9yZSgpOwogICAgY29uc3QgcGVyc29uSWQgPSB1c2VyU3RvcmUuZ2V0VXNlcj8ucGVyc29uPy5pZDsKICAgIGNvbnN0IHJlbW92ZU93bklkID0gdXNlcnMuZmlsdGVyKChlbCkgPT4gZWwgIT09IHBlcnNvbklkKTsKICAgIHJldHVybiByZW1vdmVPd25JZC5sZW5ndGg7CiAgfQogIHJldHVybiAwOwp9OwoKZXhwb3J0IGNvbnN0IGdldFdzUHJvdG9jb2wgPSAoKSA9PiB7CiAgaWYgKHdpbmRvdy5sb2NhdGlvbi5wcm90b2NvbCA9PT0gImh0dHBzOiIpIHsKICAgIHJldHVybiAid3NzOi8vIjsKICB9IGVsc2UgaWYgKGltcG9ydC5tZXRhLmVudi5ERVYpIHsKICAgIHJldHVybiAid3NzOi8vIjsKICB9IGVsc2UgewogICAgcmV0dXJuICJ3czovLyI7CiAgfQp9OwoKZXhwb3J0IGNvbnN0IGdldFRyYW5zZmVyUHJvdG9jb2wgPSAoKSA9PiB7CiAgaWYgKHdpbmRvdy5sb2NhdGlvbi5wcm90b2NvbCA9PT0gImh0dHBzOiIpIHsKICAgIHJldHVybiAiaHR0cHM6Ly8iOwogIH0gZWxzZSBpZiAoaW1wb3J0Lm1ldGEuZW52LkRFVikgewogICAgcmV0dXJuICJodHRwczovLyI7CiAgfSBlbHNlIHsKICAgIHJldHVybiAiaHR0cDoiOwogIH0KfTsK",
+    P0 = "data:video/mp2t;base64,LyoqCiAqIENoYW5nZSBzY3JvbGwgcG9zaXRpb24gYXQgYm90dG9tIG9mIHRoZSBlbGVtZW50CiAqCiAqIEBwYXJhbSBzZWxlY3RvciAtIGNsYXNzIHNlbGVjdG9yIG9mIGVsZW1lbnQKICovCmV4cG9ydCBjb25zdCBzY3JvbGxUb0JvdHRvbSA9IChzZWxlY3Rvcjogc3RyaW5nKTogdm9pZCA9PiB7CiAgY29uc3QgZWxlbWVudCA9IGRvY3VtZW50LnF1ZXJ5U2VsZWN0b3Ioc2VsZWN0b3IpIGFzIEhUTUxFbGVtZW50OwogIGVsZW1lbnQuc2Nyb2xsVG9wID0gZWxlbWVudD8uc2Nyb2xsSGVpZ2h0Owp9OwovKioKICogUHJldmVudGluZyBzY3JvbGxpbmcgdG8gYm90dG9tCiAqIEBzZWxlY3RvciAtIGNsYXNzIHNlbGVjdG9yIG9mIG1lc3NhZ2UgZWxlbWVudAogKiovCmV4cG9ydCBjb25zdCBwcmV2ZW50Qm90dG9tU2Nyb2xsaW5nID0gKHNlbGVjdG9yOiBzdHJpbmcpID0+IHsKICBjb25zdCBlbGVtZW50ID0gZG9jdW1lbnQucXVlcnlTZWxlY3RvcihzZWxlY3RvcikgYXMgSFRNTEVsZW1lbnQ7CiAgaWYgKGVsZW1lbnQpIHsKICAgIGNvbnN0IGN1cnJlbnRTY3JvbGxIZWlnaHQgPSBlbGVtZW50LnNjcm9sbEhlaWdodDsKICAgIGNvbnN0IG9ic2VydmVyID0gbmV3IFJlc2l6ZU9ic2VydmVyKCgpID0+IHsKICAgICAgZWxlbWVudC5zY3JvbGxUb3AgPSBlbGVtZW50LnNjcm9sbEhlaWdodCAtIGN1cnJlbnRTY3JvbGxIZWlnaHQ7CiAgICB9KTsKICAgIG9ic2VydmVyLm9ic2VydmUoZWxlbWVudCk7CiAgfQp9OwovKioKICogTWV0aG9kIGNoZWNrZWQgaWYgZWxlbWVudCBtZXNzYWdlIHBvc2l0aW9uIGluIGJvdHRvbSBvZiBlbGVtZW50CiAqIEBzZWxlY3RvciAtIGNsYXNzIHNlbGVjdG9yIG9mIG1lc3NhZ2UgZWxlbWVudAogKiovCmV4cG9ydCBjb25zdCBjaGVja0lmQm90dG9tU2Nyb2xsID0gKHNlbGVjdG9yOiBzdHJpbmcpID0+IHsKICBjb25zdCBlbGVtZW50ID0gZG9jdW1lbnQucXVlcnlTZWxlY3RvcihzZWxlY3RvcikgYXMgSFRNTEVsZW1lbnQ7CiAgY29uc3QgZWxlbWVudEJveCA9IGRvY3VtZW50LnF1ZXJ5U2VsZWN0b3JBbGwoCiAgICAiLnZ1ZS1yZWN5Y2xlLXNjcm9sbGVyX19pdGVtLXZpZXc6bGFzdC1jaGlsZCIKICApIGFzIE5vZGVMaXN0T2Y8SFRNTEVsZW1lbnQ+OwogIGlmIChlbGVtZW50KSB7CiAgICByZXR1cm4gKAogICAgICBNYXRoLmFicygKICAgICAgICBlbGVtZW50LnNjcm9sbEhlaWdodCAtIGVsZW1lbnQuc2Nyb2xsVG9wIC0gZWxlbWVudC5jbGllbnRIZWlnaHQKICAgICAgKSA8PSBlbGVtZW50Qm94WzBdLmNsaWVudEhlaWdodAogICAgKTsKICB9CiAgcmV0dXJuIGZhbHNlOwp9OwovKioKICogTWV0aG9kIGNoZWNrZWQgaWYgbWVzc2FnZSBpcyBpbiB2aWV3cG9ydAogKiBAaWQgLSBpZGVudGlmaWNhdGlvbiBvZiBtZXNzYWdlIGVsZW1lbnQKICoqLwpleHBvcnQgY29uc3QgaXNJblZpZXdwb3J0ID0gKGlkOiBzdHJpbmcpID0+IHsKICBjb25zdCBtZXNzYWdlc0JveCA9IGRvY3VtZW50LmdldEVsZW1lbnRCeUlkKGByb29tLW1lc3NhZ2VzYCkgYXMgSFRNTEVsZW1lbnQ7CiAgY29uc3QgZWxlbWVudCA9IGRvY3VtZW50LmdldEVsZW1lbnRCeUlkKGlkKSBhcyBIVE1MRWxlbWVudDsKICBpZiAoZWxlbWVudCkgewogICAgY29uc3QgcmVjdCA9IGVsZW1lbnQ/LmdldEJvdW5kaW5nQ2xpZW50UmVjdCgpOwogICAgcmV0dXJuICgKICAgICAgcmVjdD8udG9wID49IDAgJiYKICAgICAgcmVjdD8ubGVmdCA+PSAwICYmCiAgICAgIHJlY3Q/LmJvdHRvbSA8PSBtZXNzYWdlc0JveC5nZXRCb3VuZGluZ0NsaWVudFJlY3QoKS5ib3R0b20gJiYKICAgICAgcmVjdD8ucmlnaHQgPD0gbWVzc2FnZXNCb3guZ2V0Qm91bmRpbmdDbGllbnRSZWN0KCkucmlnaHQKICAgICk7CiAgfQogIHJldHVybiBmYWxzZTsKfTsKCi8qKgogKiBNZXRob2QgY2hlY2sgaWYgZWxlbWVudCBoYXMgc2Nyb2xsYmFyCiAqIEBpZCAtIGlkIG9mIGVsZW1lbnQKICogKiovCmV4cG9ydCBjb25zdCBoYXNTY3JvbGxCYXIgPSAoaWQ6IHN0cmluZykgPT4gewogIGNvbnN0IGVsZW1lbnQgPSBkb2N1bWVudC5nZXRFbGVtZW50QnlJZChpZCk7CiAgaWYgKGVsZW1lbnQpIHsKICAgIHJldHVybiBlbGVtZW50LnNjcm9sbEhlaWdodCA+IGVsZW1lbnQuY2xpZW50SGVpZ2h0OwogIH0KICByZXR1cm4gZmFsc2U7Cn07Cg==",
     $0 = "data:video/mp2t;base64,aW1wb3J0IHdlYnNvY2tldFNlcnZpY2UgZnJvbSAiQC9zZXJ2aWNlcy9jaGF0L3dlYnNvY2tldC1jaGF0IjsKaW1wb3J0IHsgV1NfVFlQRVMgfSBmcm9tICJAL3R5cGVzL2dlbmVyYWwudHlwZXMiOwppbXBvcnQgeyB1c2VVc2VyU3RvcmUgfSBmcm9tICJAL3N0b3JlL3VzZVVzZXJTdG9yZSI7CmltcG9ydCB7IGNoZWNrSWZCb3R0b21TY3JvbGwsIHNjcm9sbFRvQm90dG9tIH0gZnJvbSAiQC9oZWxwZXJzL3Njcm9sbCI7CmltcG9ydCBjaGF0U2VydmljZSBmcm9tICJAL3NlcnZpY2VzL2NoYXQvY2hhdCI7CgovKioKICogZ2xvYmFsIHZhcnMgZm9yIGN1cnJlbnQgZmlsZQogKiovCmNvbnN0IGdsb2JhbFZhciA9IHsKICB0aW1lcjogMCwKfTsKCi8qKgogKiBNZXRob2RzIHJlbW92ZSBjdXJyZW50IHVzZXIgaWQgZnJvbSB1c2VycyAtIGZvciBkaXNwbGF5aW5nIHRvdGFsIG9ubGluZSB1c2VycwogKiBAdXNlcnMgLSBsaXN0IG9mIG9ubGluZSB1c2VycwogKiovCgpjb25zdCBwZW9wbGVPbmxpbmUgPSAodXNlcnM6IG51bWJlcltdKSA9PiB7CiAgd2Vic29ja2V0U2VydmljZS5wZW9wbGVPbmxpbmUudmFsdWUgPSB1c2Vycy5sZW5ndGggLSAxOwp9OwoKLyoqCiAqIE1ldGhvZHMgd2hpY2ggY2FsbGVkIHdoZW4gImNoYXRfbWVzc2FnZXMiIHNpZ25hbCB3YXMgY2FsbGVkCiAqIEBtZXNzYWdlIC0gY3VycmVudCBtZXNzYWdlCiAqKi8KY29uc3Qgc2VuZE1lc3NhZ2UgPSBhc3luYyAobWVzc2FnZTogYW55KSA9PiB7CiAgY29uc3QgdXNlclN0b3JlID0gdXNlVXNlclN0b3JlKCk7CiAgY29uc3Qgb3duTWVzc2FnZSA9IG1lc3NhZ2U/LmF1dGhvci5pZCA9PT0gdXNlclN0b3JlLmdldFVzZXIucGVyc29uLmlkOwogIGlmICghb3duTWVzc2FnZSAmJiAhbWVzc2FnZS5pc19yZWFkKSB7CiAgICB3ZWJzb2NrZXRTZXJ2aWNlLnVucmVhZE1lc3NhZ2VzLnZhbHVlLnB1c2gobWVzc2FnZS5pZCk7CiAgfQogIGlmIChtZXNzYWdlLmNvbnZlcnNhdGlvbiA9PT0gd2Vic29ja2V0U2VydmljZS5zZWxlY3RlZFJvb20udmFsdWU/LmlkKSB7CiAgICB3ZWJzb2NrZXRTZXJ2aWNlLm1lc3NhZ2VzLnZhbHVlLnB1c2gobWVzc2FnZSk7CiAgfQogIHNldFRpbWVvdXQoKCkgPT4gewogICAgaWYgKGNoZWNrSWZCb3R0b21TY3JvbGwoIi52dWUtcmVjeWNsZS1zY3JvbGxlciIpKSB7CiAgICAgIHNjcm9sbFRvQm90dG9tKCIudnVlLXJlY3ljbGUtc2Nyb2xsZXIiKTsKICAgIH0KICB9LCA1MDApOwp9OwoKLyoqCiAqIE1ldGhvZHMgd2hpY2ggY2FsbGVkIHdoZW4gImNvbnZlcnNhdGlvbl9kZXRhaWxzIiBzaWduYWwgd2FzIGNhbGxlZAogKiBAY29udmVyc2F0aW9uIC0gaW5mbyBhYm91dCBjdXJyZW50IGNvbnZlcnNhdGlvbgogKiovCmNvbnN0IG9uQ29udmVyc2F0aW9uRGV0YWlscyA9IGFzeW5jIChjb252ZXJzYXRpb246IGFueSkgPT4gewogIGNvbnN0IGdldEN1cnJlbnRSb29tSW5kZXggPSB3ZWJzb2NrZXRTZXJ2aWNlLnJvb21zLnZhbHVlLmZpbmRJbmRleCgKICAgIChlbCkgPT4gZWwuaWQgPT09IGNvbnZlcnNhdGlvbi5pZAogICk7CiAgaWYgKGdldEN1cnJlbnRSb29tSW5kZXgudG9TdHJpbmcoKSkgewogICAgd2Vic29ja2V0U2VydmljZS5yb29tcy52YWx1ZVtnZXRDdXJyZW50Um9vbUluZGV4XSA9IGNvbnZlcnNhdGlvbjsKICB9IGVsc2UgewogICAgd2Vic29ja2V0U2VydmljZS5yb29tcy52YWx1ZSA9IGF3YWl0IGNoYXRTZXJ2aWNlLmZldGNoQ29udmVyc2F0aW9ucygpOwogIH0KfTsKCi8qKgogKiBNZXRob2RzIHdoaWNoIGNhbGxlZCB3aGVuICJjaGF0X21lc3NhZ2VfdXBkYXRlIiBzaWduYWwgd2FzIGNhbGxlZAogKiBAbWVzc2FnZSAtIHVwZGF0ZWQgbWVzc2FnZQogKiovCmNvbnN0IGNoYXRNZXNzYWdlVXBkYXRlID0gKG1lc3NhZ2U6IGFueSkgPT4gewogIGNvbnN0IGZpbmRDdXJyZW50TWVzc2FnZUluZGV4ID0gd2Vic29ja2V0U2VydmljZS5tZXNzYWdlcy52YWx1ZS5maW5kSW5kZXgoCiAgICAoZWwpID0+IGVsLmlkID09PSBtZXNzYWdlLmlkCiAgKTsKICB3ZWJzb2NrZXRTZXJ2aWNlLm1lc3NhZ2VzLnZhbHVlW2ZpbmRDdXJyZW50TWVzc2FnZUluZGV4XSA9IG1lc3NhZ2U7CiAgY2xlYXJUaW1lb3V0KGdsb2JhbFZhci50aW1lcik7CiAgZ2xvYmFsVmFyLnRpbWVyID0gc2V0VGltZW91dCgoKSA9PiB7CiAgICB3ZWJzb2NrZXRTZXJ2aWNlLnVucmVhZE1lc3NhZ2VzLnZhbHVlID0gW107CiAgfSwgMzAwMCk7Cn07CmNvbnN0IHJlY2VudE1lc3NhZ2VzID0gKHRpY2s6IGFueSkgPT4gewogIHdlYnNvY2tldFNlcnZpY2UubWVzc2FnZXMudmFsdWUgPSB0aWNrLm1lc3NhZ2VzOwogIHdlYnNvY2tldFNlcnZpY2UuaGFzTW9yZU1lc3NhZ2VzLnZhbHVlID0gdGljay5oYXNfbW9yZTsKICB3ZWJzb2NrZXRTZXJ2aWNlLmxvYWRpbmdPcHRpb25zLnZhbHVlLmxvYWRpbmcgPSBmYWxzZTsKICB3ZWJzb2NrZXRTZXJ2aWNlLmxvYWRpbmdPcHRpb25zLnZhbHVlLmlzTG9hZGVkID0gdHJ1ZTsKfTsKCi8qKgogKiBNZXRob2RzIGNhbGwgd2hlbiBzb21lIG9mIHdlYnNvY2tldCBzaWduYWwgd2FzIGNhbGxlZAogKiBAdGljayAtIGN1cnJlbnQgc2lnbmFsIGRhdGEKICoqLwpleHBvcnQgY29uc3Qgd2Vic29ja2V0TWVzc2FnZXMgPSAodGljazogYW55KSA9PiB7CiAgc3dpdGNoICh0cnVlKSB7CiAgICBjYXNlIFdTX1RZUEVTLlBFT1BMRV9PTkxJTkUgPT09IHRpY2sudHlwZToKICAgICAgcGVvcGxlT25saW5lKHRpY2subWVzc2FnZSk7CiAgICAgIGJyZWFrOwogICAgY2FzZSBXU19UWVBFUy5SRUNFTlRfTUVTU0FHRVMgPT09IHRpY2sudHlwZToKICAgICAgcmVjZW50TWVzc2FnZXModGljayk7CiAgICAgIGJyZWFrOwogICAgY2FzZSBXU19UWVBFUy5DSEFUX01FU1NBR0VTID09PSB0aWNrLnR5cGU6CiAgICAgIHNlbmRNZXNzYWdlKHRpY2subWVzc2FnZSk7CiAgICAgIGJyZWFrOwogICAgY2FzZSBXU19UWVBFUy5UWVBJTkcgPT09IHRpY2sudHlwZSAmJiB0aWNrLnR5cGluZzoKICAgICAgd2Vic29ja2V0U2VydmljZS51c2VyVHlwaW5nLnZhbHVlID0gdGljazsKICAgICAgYnJlYWs7CiAgICBjYXNlIFdTX1RZUEVTLlRZUElORyA9PT0gdGljay50eXBlICYmICF0aWNrLnR5cGluZzoKICAgICAgd2Vic29ja2V0U2VydmljZS51c2VyVHlwaW5nLnZhbHVlID0ge307CiAgICAgIGJyZWFrOwogICAgY2FzZSBXU19UWVBFUy5DSEFUX01FU1NBR0VfVVBEQVRFID09PSB0aWNrLnR5cGU6CiAgICAgIGNoYXRNZXNzYWdlVXBkYXRlKHRpY2subWVzc2FnZSk7CiAgICAgIGJyZWFrOwogICAgY2FzZSBXU19UWVBFUy5DT05WRVJTQVRJT05fREVUQUlMUyA9PT0gdGljay50eXBlOgogICAgICBvbkNvbnZlcnNhdGlvbkRldGFpbHModGljay5jb252ZXJzYXRpb24pOwogICAgICBicmVhazsKICB9Cn07Cg==",
     Q0 = "data:video/mp2t;base64,aW1wb3J0IHsgY3JlYXRlQXBwIH0gZnJvbSAidnVlIjsKaW1wb3J0ICIuL2Fzc2V0cy9tYWluLnNjc3MiOwppbXBvcnQgQXBwIGZyb20gIi4vQXBwLnZ1ZSI7CmltcG9ydCBjbGlja091dFNpZGUgZnJvbSAiQC9kaXJlY3RpdmVzL2NsaWNrT3V0U2lkZSI7CmltcG9ydCB7IGNyZWF0ZVBpbmlhIH0gZnJvbSAicGluaWEiOwppbXBvcnQgRmxvYXRpbmdWdWUgZnJvbSAiZmxvYXRpbmctdnVlIjsKCmNvbnN0IHBpbmlhID0gY3JlYXRlUGluaWEoKTsKCmNvbnN0IGFwcCA9IGNyZWF0ZUFwcChBcHApOwoKYXBwLnVzZShwaW5pYSk7CmFwcC51c2UoRmxvYXRpbmdWdWUpOwoKYXBwLmRpcmVjdGl2ZSgiY2xpY2stb3V0c2lkZSIsIGNsaWNrT3V0U2lkZSk7CgphcHAubW91bnQoIiNjaGF0LWFwcCIpOwo=",
     q0 = "data:video/mp2t;base64,aW1wb3J0IHsgcmVmIH0gZnJvbSAidnVlIjsKCmV4cG9ydCBkZWZhdWx0IHJlZjxhbnk+KFsKICB7CiAgICByb29tSWQ6IDEsCiAgICB0aXRsZTogIlRlc3Qgcm9vbSIsCiAgICByb29tTWVzc2FnZXM6IFsKICAgICAgewogICAgICAgIHR5cGU6ICJ0ZXh0IiwKICAgICAgICBkYXRhOiB7CiAgICAgICAgICB0ZXh0OiAiSGVsbG8gV29ybGQiLAogICAgICAgIH0sCiAgICAgICAgdGltZTogbmV3IERhdGUoIjA0LzAzLzIwMjMiKSwKICAgICAgICBpc093bjogdHJ1ZSwKICAgICAgICBtZXNzYWdlUmVhY3Rpb25zOiBbXSwKICAgICAgICBzaG93VGltZUxhYmVsOiB0cnVlLAogICAgICB9LAogICAgICB7CiAgICAgICAgdHlwZTogInRleHQiLAogICAgICAgIGRhdGE6IHsKICAgICAgICAgIHRleHQ6ICJIZWxsbyBXb3JsZCIsCiAgICAgICAgfSwKICAgICAgICB0aW1lOiBuZXcgRGF0ZSgiMDQvMDcvMjAyMyIpLAogICAgICAgIGlzT3duOiBmYWxzZSwKICAgICAgICBtZXNzYWdlUmVhY3Rpb25zOiBbXSwKICAgICAgICBzaG93VGltZUxhYmVsOiB0cnVlLAogICAgICB9LAogICAgXSwKICAgIHN0YXJ0Q29udmVyc2F0aW9uOiAiMDQvMDMvMjAyMyIsCiAgICBtZXNzYWdlc0xvYWRlZDogIjA0LzA3LzIwMjMiLAogICAgbmV3TWVzc2FnZVRpbWU6ICIwNC8wNy8yMDIzIiwKICB9LAogIHsKICAgIHJvb21JZDogMiwKICAgIHRpdGxlOiAiUm9vbSAyIiwKICAgIHJvb21NZXNzYWdlczogW10sCiAgICBzdGFydENvbnZlcnNhdGlvbjogIiIsCiAgICBtZXNzYWdlc0xvYWRlZDogIjA0LzA0LzIwMjMiLAogICAgbmV3TWVzc2FnZVRpbWU6ICIwNC8wNy8yMDIzIiwKICB9LAogIHsKICAgIHJvb21JZDogMywKICAgIHN0YXJ0Q29udmVyc2F0aW9uOiAiIiwKICAgIHRpdGxlOiAiUm9vbSAzIiwKICAgIHJvb21NZXNzYWdlczogW10sCiAgICBtZXNzYWdlc0xvYWRlZDogIjA0LzA0LzIwMjMiLAogICAgbmV3TWVzc2FnZVRpbWU6ICIwNC8wNy8yMDIzIiwKICB9LApdKTsK",
     em = "data:video/mp2t;base64,ZGVjbGFyZSBtb2R1bGUgInZ1ZTMtZW1vamktcGlja2VyIiB7fQo=",
     tm = "data:video/mp2t;base64,aW1wb3J0IEFwaSBmcm9tICJAL3NlcnZpY2VzIjsKaW1wb3J0IHsgSVJvb20gfSBmcm9tICJAL3R5cGVzL3Jvb21zLnR5cGVzIjsKCmNsYXNzIGNoYXRTZXJ2aWNlIGV4dGVuZHMgQXBpIHsKICBhc3luYyBmZXRjaENvbnZlcnNhdGlvbnMoKSB7CiAgICB0cnkgewogICAgICBjb25zdCB7IGRhdGEgfTogeyBkYXRhOiBJUm9vbVtdIH0gPSBhd2FpdCB0aGlzLmdldCgiY2hhdC9jb252ZXJzYXRpb25zLyIpOwogICAgICByZXR1cm4gZGF0YTsKICAgIH0gY2F0Y2ggKGU6IGFueSkgewogICAgICB0aHJvdyBuZXcgRXJyb3IoZSk7CiAgICB9CiAgfQoKICBhc3luYyBmZXRjaENvbnZlcnNhdGlvbkRldGFpbChpZDogc3RyaW5nKSB7CiAgICB0cnkgewogICAgICBjb25zdCB7IGRhdGEgfTogeyBkYXRhOiBJUm9vbSB9ID0gYXdhaXQgdGhpcy5nZXQoCiAgICAgICAgYGNoYXQvY29udmVyc2F0aW9ucy8ke2lkfS9gCiAgICAgICk7CiAgICAgIHJldHVybiBkYXRhOwogICAgfSBjYXRjaCAoZTogYW55KSB7CiAgICAgIHRocm93IG5ldyBFcnJvcihlKTsKICAgIH0KICB9CgogIGFzeW5jIGZldGNoUmVjZW50TWVzc2FnZXMoaWQ6IHN0cmluZywgcGFnZTogbnVtYmVyLCBwYXJhbXM/OiBhbnkpIHsKICAgIHRyeSB7CiAgICAgIGNvbnN0IHsgZGF0YSB9OiBhbnkgPSBhd2FpdCB0aGlzLmdldCgKICAgICAgICBgY2hhdC9tZXNzYWdlcy8/Y29udmVyc2F0aW9uPSR7aWR9JnBhZ2U9JHtwYWdlfWAsCiAgICAgICAgcGFyYW1zCiAgICAgICk7CiAgICAgIHJldHVybiBkYXRhOwogICAgfSBjYXRjaCAoZTogYW55KSB7CiAgICAgIHRocm93IG5ldyBFcnJvcihlKTsKICAgIH0KICB9CgogIGFzeW5jIGZldGNoQ2hhdE1ldGEoKSB7CiAgICB0cnkgewogICAgICBjb25zdCB7IGRhdGEgfTogYW55ID0gYXdhaXQgdGhpcy5nZXQoImNoYXQvbWV0YS8iKTsKICAgICAgcmV0dXJuIGRhdGE7CiAgICB9IGNhdGNoIChlOiBhbnkpIHsKICAgICAgdGhyb3cgbmV3IEVycm9yKGUpOwogICAgfQogIH0KfQoKZXhwb3J0IGRlZmF1bHQgbmV3IGNoYXRTZXJ2aWNlKCk7Cg==",
     nm = "data:video/mp2t;base64,aW1wb3J0IHsgcmVmIH0gZnJvbSAidnVlIjsKaW1wb3J0IHsgSU1lc3NhZ2UgfSBmcm9tICJAL3R5cGVzL3Jvb20vcm9vbS50eXBlcyI7CmltcG9ydCB7IHdlYnNvY2tldE1lc3NhZ2VzIH0gZnJvbSAiQC9oZWxwZXJzL3dlYnNvY2tldC1tZXNzYWdlcyI7CmltcG9ydCB7CiAgZ2V0Q2hhdEFwaVRva2VuLAogIGdldERvbWFpbk5hbWUsCiAgZ2V0V3NQcm90b2NvbCwKfSBmcm9tICJAL2hlbHBlcnMvZ2VuZXJhbCI7CmltcG9ydCB7IElSb29tIH0gZnJvbSAiQC90eXBlcy9yb29tcy50eXBlcyI7CmltcG9ydCBjaGF0U2VydmljZSBmcm9tICJAL3NlcnZpY2VzL2NoYXQvY2hhdCI7CgpjbGFzcyB3ZWJzb2NrZXRTZXJ2aWNlIHsKICBwdWJsaWMgc29ja2V0OiBhbnk7CiAgcHVibGljIHJvb21zID0gcmVmPElSb29tW10+KFtdKTsKICBwdWJsaWMgbWVzc2FnZXMgPSByZWY8SU1lc3NhZ2VbXT4oW10pOwogIHB1YmxpYyBwZW9wbGVPbmxpbmUgPSByZWY8bnVtYmVyPigwKTsKICBwdWJsaWMgdXNlclR5cGluZyA9IHJlZjxhbnk+KHt9KTsKICBwdWJsaWMgdW5yZWFkTWVzc2FnZXMgPSByZWY8c3RyaW5nW10+KFtdKTsKICBwdWJsaWMgc2VsZWN0ZWRSb29tID0gcmVmPElSb29tIHwgdW5kZWZpbmVkPigpOwogIHB1YmxpYyBoYXNNb3JlTWVzc2FnZXMgPSByZWYoZmFsc2UpOwogIHB1YmxpYyBsb2FkaW5nT3B0aW9ucyA9IHJlZih7CiAgICBsb2FkaW5nOiBmYWxzZSwKICAgIGlzTG9hZGVkOiBmYWxzZSwKICB9KTsKICBvcGVuU29ja2V0ID0gYXN5bmMgKGlkOiBzdHJpbmcpID0+IHsKICAgIHRoaXMubG9hZGluZ09wdGlvbnMudmFsdWUubG9hZGluZyA9IHRydWU7CiAgICAvLyBAdHMtaWdub3JlCiAgICB0aGlzLnNvY2tldCA9IG5ldyBXZWJTb2NrZXQoCiAgICAgIGAke2dldFdzUHJvdG9jb2woKX0ke2dldERvbWFpbk5hbWUoKX0vY2hhdC93cy8ke2lkfS8/dG9rZW49JHtnZXRDaGF0QXBpVG9rZW4oKX1gCiAgICApOwogICAgdGhpcy5zb2NrZXQub25vcGVuID0gKGV2ZW50OiBhbnkpOiB2b2lkID0+IHsKICAgICAgY29uc29sZS5sb2coIlNPQ0tFVCBJUyBPUEVOIFdJVEggTUVTU0FHRSIsIGV2ZW50KTsKICAgIH07CgogICAgdGhpcy5zb2NrZXQub25tZXNzYWdlID0gKGV2ZW50OiBNZXNzYWdlRXZlbnQpID0+IHsKICAgICAgY29uc29sZS5sb2coIlNPQ0tFVCBNRVNTQUdFIiwgSlNPTi5wYXJzZShldmVudC5kYXRhKSk7CiAgICAgIGNvbnN0IGN1cnJlbnRUaWNrID0gSlNPTi5wYXJzZShldmVudC5kYXRhKTsKICAgICAgd2Vic29ja2V0TWVzc2FnZXMoY3VycmVudFRpY2spOwogICAgfTsKCiAgICB0aGlzLnNvY2tldC5vbmVycm9yID0gKCkgPT4gewogICAgICB0aGlzLmxvYWRpbmdPcHRpb25zLnZhbHVlLmxvYWRpbmcgPSBmYWxzZTsKICAgIH07CgogICAgdGhpcy5zb2NrZXQub25jbG9zZSA9IChldmVudDogTWVzc2FnZUV2ZW50KSA9PiB7CiAgICAgIGNvbnNvbGUubG9nKCJTT0NLRVQgTUVTU0FHRSIsIGV2ZW50KTsKICAgIH07CiAgfTsKCiAgY2xvc2VTb2NrZXQgPSAoKSA9PiB7CiAgICB0aGlzLnNvY2tldD8uY2xvc2UoKTsKICAgIHRoaXMubWVzc2FnZXMudmFsdWUgPSBbXTsKICB9OwogIHNlbmRNZXNzYWdlID0gKG1lc3NhZ2U6IGFueSkgPT4gewogICAgdGhpcy5zb2NrZXQ/LnNlbmQoSlNPTi5zdHJpbmdpZnkobWVzc2FnZSkpOwogIH07CgogIGZldGNoUm9vbSA9IGFzeW5jIChpZDogc3RyaW5nKSA9PiB7CiAgICB0aGlzLnNlbGVjdGVkUm9vbS52YWx1ZSA9IGF3YWl0IGNoYXRTZXJ2aWNlLmZldGNoQ29udmVyc2F0aW9uRGV0YWlsKGlkKTsKICAgIGF3YWl0IHRoaXMub3BlblNvY2tldChpZCk7CiAgfTsKfQoKZXhwb3J0IGRlZmF1bHQgbmV3IHdlYnNvY2tldFNlcnZpY2UoKTsK",
     om = "data:video/mp2t;base64,aW1wb3J0IHsgQXhpb3NJbnN0YW5jZSB9IGZyb20gImF4aW9zIjsKaW1wb3J0IHsgYXhpb3NCYXNlQ29uZmlnIH0gZnJvbSAiQC9hcGkiOwoKZXhwb3J0IGRlZmF1bHQgYWJzdHJhY3QgY2xhc3MgQXBpIHsKICBwcml2YXRlIGluc3RhbmNlOiBBeGlvc0luc3RhbmNlID0gYXhpb3NCYXNlQ29uZmlnOwoKICBwcm90ZWN0ZWQgZ2V0VXJsKHVybD86IHN0cmluZykgewogICAgcmV0dXJuIGAke3RoaXMuaW5zdGFuY2UuZGVmYXVsdHM/LmJhc2VVUkx9LyR7dXJsIHx8ICIifWA7CiAgfQoKICBwcm90ZWN0ZWQgcG9zdDxUPih1cmw6IHN0cmluZywgZGF0YT86IHVua25vd24sIGNvbmZpZz86IGFueSkgewogICAgcmV0dXJuIHRoaXMuaW5zdGFuY2UucG9zdDxUPih0aGlzLmdldFVybCh1cmwpLCBkYXRhLCBjb25maWcpOwogIH0KCiAgcHJvdGVjdGVkIHB1dDxUPih1cmw6IHN0cmluZywgZGF0YT86IHVua25vd24sIGNvbmZpZz86IGFueSkgewogICAgcmV0dXJuIHRoaXMuaW5zdGFuY2UucHV0PFQ+KHRoaXMuZ2V0VXJsKHVybCksIGRhdGEsIGNvbmZpZyk7CiAgfQoKICBwcm90ZWN0ZWQgcGF0Y2g8VD4odXJsOiBzdHJpbmcsIGRhdGE/OiB1bmtub3duLCBjb25maWc/OiBhbnkpIHsKICAgIHJldHVybiB0aGlzLmluc3RhbmNlLnBhdGNoPFQ+KHRoaXMuZ2V0VXJsKHVybCksIGRhdGEsIGNvbmZpZyk7CiAgfQoKICBwcm90ZWN0ZWQgZ2V0PFQ+KHVybDogc3RyaW5nLCBjb25maWc/OiBhbnkpIHsKICAgIHJldHVybiB0aGlzLmluc3RhbmNlLmdldDxUPih0aGlzLmdldFVybCh1cmwpLCBjb25maWcpOwogIH0KCiAgcHJvdGVjdGVkIGRlbGV0ZTxUPih1cmw6IHN0cmluZywgY29uZmlnPzogYW55KSB7CiAgICByZXR1cm4gdGhpcy5pbnN0YW5jZS5kZWxldGU8VD4odGhpcy5nZXRVcmwodXJsKSwgY29uZmlnKTsKICB9Cn0K",
@@ -6200,32 +6202,32 @@
         "/src/components/room/content/RoomMessageWrapper.vue": M0,
         "/src/components/room/content/RoomNoMessages.vue": Z0,
         "/src/components/room/content/RoomReactions.vue": W0,
         "/src/components/room/content/audio-message/AudioMessage.vue": S0,
         "/src/components/room/content/files-message/FileMessage.vue": B0,
         "/src/components/room/content/reply-message/ReplyMessage.vue": z0,
         "/src/components/room/content/text-message/TextMessage.vue": V0,
-        "/src/components/room/content/video-message/VideoMessage.vue": T0,
-        "/src/components/room/footer/RoomEmojiPicker.vue": G0,
+        "/src/components/room/content/video-message/VideoMessage.vue": G0,
+        "/src/components/room/footer/RoomEmojiPicker.vue": T0,
         "/src/components/room/footer/RoomFooter.vue": j0,
         "/src/components/room/header/RoomHeader.vue": k0,
         "/src/components/rooms/RoomsContainer.vue": D0,
         "/src/components/rooms/RoomsEmpty.vue": R0,
         "/src/components/rooms/RoomsItem.vue": x0,
         "/src/components/rooms/RoomsList.vue": X0,
         "/src/components/ui/OButton.vue": Y0,
         "/src/components/ui/OInput.vue": E0,
         "/src/components/ui/OLoading.vue": H0,
         "/src/components/ui/OMenuHeader.vue": O0,
         "/src/composables/useIntersection.ts": L0,
         "/src/composables/useIsReadMessage.ts": U0,
         "/src/directives/clickOutSide.ts": J0,
         "/src/global.d.ts": K0,
-        "/src/helpers/general.ts": P0,
-        "/src/helpers/scroll.ts": F0,
+        "/src/helpers/general.ts": F0,
+        "/src/helpers/scroll.ts": P0,
         "/src/helpers/websocket-messages.ts": $0,
         "/src/main.ts": Q0,
         "/src/mock-data/room-structure.ts": q0,
         "/src/plugins.d.ts": em,
         "/src/services/chat/chat.ts": tm,
         "/src/services/chat/websocket-chat.ts": nm,
         "/src/services/index.ts": om,
@@ -6275,15 +6277,15 @@
                     n.value = !1, t("blur")
                 };
             return (i, f) => {
                 const r = vs("click-outside");
                 return j(), U(_e, null, [bn((j(), U("div", On(i.$attrs, {
                     class: i.$style["ops-room-header__button"],
                     onClick: f[0] || (f[0] = a => n.value = !n.value)
-                }), [F("img", {
+                }), [P("img", {
                     src: ae(Zt)(`assets/icons/${e.icon||"header-chat-menu"}.svg`),
                     alt: "menu"
                 }, null, 8, um)], 16)), [
                     [r, s]
                 ]), se(Ao, {
                     name: "ops-slide-left"
                 }, {
@@ -6293,15 +6295,15 @@
                     }, [e.options ? (j(), U("div", {
                         key: 0,
                         class: L(i.$style["ops-header-menu-options__list"])
                     }, [(j(!0), U(_e, null, Cn(e.options, a => (j(), U("div", {
                         key: a.id,
                         class: L(i.$style["ops-header-menu-options__list-item"]),
                         onClick: l => o(a)
-                    }, Te(a.title), 11, dm))), 128))], 2)) : me("", !0)], 2)) : me("", !0)]),
+                    }, Ge(a.title), 11, dm))), 128))], 2)) : me("", !0)], 2)) : me("", !0)]),
                     _: 1
                 })], 64)
             }
         }
     }),
     pm = "_ops-header-menu-options_358as_1",
     mm = "_ops-header-menu-options__list_358as_6",
@@ -6367,62 +6369,62 @@
                 c = () => {
                     n.toggleMobileVisible()
                 };
             return (u, d) => {
                 var m, p;
                 return j(), U("div", {
                     class: L(u.$style["ops-room-header"])
-                }, [F("div", {
+                }, [P("div", {
                     class: L(u.$style["ops-room-header__wrapper"])
-                }, [F("button", {
+                }, [P("button", {
                     class: L([u.$style["ops-room-header__button"], u.$style["ops-room-header__button--desktop"], {
                         [u.$style["ops-room-header__button--rotate"]]: !e.showRoomsList
                     }]),
                     onClick: d[0] || (d[0] = h => u.$emit("toggleRoomsList"))
-                }, [F("img", {
+                }, [P("img", {
                     src: ae(Zt)("assets/icons/toggle.svg"),
                     alt: "toggle icon"
-                }, null, 8, ym)], 2), F("button", {
+                }, null, 8, ym)], 2), P("button", {
                     class: L([u.$style["ops-room-header__button"], u.$style["ops-room-header__button--mobile"]]),
                     onClick: c
-                }, [F("img", {
+                }, [P("img", {
                     src: ae(Zt)("assets/icons/toggle.svg"),
                     alt: "toggle icon"
-                }, null, 8, Am)], 2), F("div", {
+                }, null, 8, Am)], 2), P("div", {
                     class: L(u.$style["ops-info-wrapper"])
-                }, [F("div", {
+                }, [P("div", {
                     class: L(u.$style["ops-text-ellipsis"])
                 }, [(m = e.room) != null && m.handling_request_url ? (j(), U("a", {
                     key: 0,
                     class: L([u.$style["ops-info-wrapper__name"], u.$style["ops-text-ellipsis"]]),
                     href: (p = e.room) == null ? void 0 : p.handling_request_url,
                     target: "_blank"
-                }, [F("span", null, Te(e.room.name), 1), F("img", {
+                }, [P("span", null, Ge(e.room.name), 1), P("img", {
                     class: L(u.$style["ops-info-wrapper__link"]),
                     src: ae(Zt)("assets/icons/link.svg"),
                     alt: "link"
                 }, null, 10, wm)], 10, vm)) : (j(), U("p", {
                     key: 1,
                     class: L([u.$style["ops-info-wrapper__name"], u.$style["ops-text-ellipsis"]])
-                }, Te(e.room.name), 3)), F("div", {
+                }, Ge(e.room.name), 3)), P("div", {
                     class: L([u.$style["ops-info-wrapper__info"], u.$style["ops-text-ellipsis"]])
-                }, Te(ae(l)), 3)], 2)], 2)], 2), se(Cm)], 2)
+                }, Ge(ae(l)), 3)], 2)], 2)], 2), se(Cm)], 2)
             }
         }
     }),
     Nm = "_ops-room-header_1tgxi_1",
     Mm = "_ops-room-header__button_1tgxi_4",
     Zm = "_ops-room-header__button--desktop_1tgxi_7",
     Wm = "_ops-room-header__button--mobile_1tgxi_10",
     Sm = "_ops-room-header__button--rotate_1tgxi_13",
     Bm = "_ops-room-header__wrapper_1tgxi_16",
     zm = "_ops-info-wrapper_1tgxi_19",
     Vm = "_ops-info-wrapper__name_1tgxi_22",
-    Tm = "_ops-info-wrapper__link_1tgxi_25",
-    Gm = "_ops-info-wrapper__info_1tgxi_29",
+    Gm = "_ops-info-wrapper__link_1tgxi_25",
+    Tm = "_ops-info-wrapper__info_1tgxi_29",
     jm = {
         "ops-room-header": "_ops-room-header_1tgxi_1",
         opsRoomHeader: Nm,
         "ops-room-header__button": "_ops-room-header__button_1tgxi_4",
         opsRoomHeaderButton: Mm,
         "ops-room-header__button--desktop": "_ops-room-header__button--desktop_1tgxi_7",
         opsRoomHeaderButtonDesktop: Zm,
@@ -6433,17 +6435,17 @@
         "ops-room-header__wrapper": "_ops-room-header__wrapper_1tgxi_16",
         opsRoomHeaderWrapper: Bm,
         "ops-info-wrapper": "_ops-info-wrapper_1tgxi_19",
         opsInfoWrapper: zm,
         "ops-info-wrapper__name": "_ops-info-wrapper__name_1tgxi_22",
         opsInfoWrapperName: Vm,
         "ops-info-wrapper__link": "_ops-info-wrapper__link_1tgxi_25",
-        opsInfoWrapperLink: Tm,
+        opsInfoWrapperLink: Gm,
         "ops-info-wrapper__info": "_ops-info-wrapper__info_1tgxi_29",
-        opsInfoWrapperInfo: Gm
+        opsInfoWrapperInfo: Tm
     },
     km = {
         $style: jm
     },
     Dm = Ye(_m, [
         ["__cssModules", km]
     ]),
@@ -6481,15 +6483,15 @@
     Em = {
         "ops-button__img": "_ops-button__img_19bb5_1",
         opsButtonImg: Ym
     },
     Hm = {
         $style: Em
     },
-    Fl = Ye(Xm, [
+    Pl = Ye(Xm, [
         ["__cssModules", Hm]
     ]);
 var Om = Object.defineProperty,
     Lm = Object.defineProperties,
     Um = Object.getOwnPropertyDescriptors,
     jr = Object.getOwnPropertySymbols,
     Jm = Object.prototype.hasOwnProperty,
@@ -6519,26 +6521,26 @@
         symbols: "Symbols",
         flags: "Flags"
     },
     ql = "u",
     Vs = "n",
     Do = "v",
     Io = "r",
-    Pm = {
+    Fm = {
         [Vs]: ["grinning face", "grinning"],
         [ql]: "1f600",
         [Io]: "1f600"
     },
     fs = "neutral",
-    Fm = "1f3fb",
+    Pm = "1f3fb",
     $m = "1f3fc",
     Qm = "1f3fd",
     qm = "1f3fe",
     eI = "1f3ff",
-    tI = [fs, Fm, $m, Qm, qm, eI],
+    tI = [fs, Pm, $m, Qm, qm, eI],
     nI = {
         placeholder: "Search emoji",
         skinTone: "Skin tone"
     },
     oI = ["light", "dark", "auto"],
     sI = [{
         n: ["grinning face", "grinning"],
@@ -11623,20 +11625,20 @@
     return ni.set(t, i), i
 }
 bI(e => No(ut({}, e), {
     get: (t, n, o) => Xr(t, n) || e.get(t, n, o),
     has: (t, n) => !!Xr(t, n) || e.has(t, n)
 }));
 const _f = "EMJ",
-    Tn = "emojis",
+    Gn = "emojis",
     Nf = 3;
 async function wI() {
     (await wf(_f, Nf, {
         upgrade(t, n) {
-            t.objectStoreNames.contains(Tn) || t.createObjectStore(Tn, {
+            t.objectStoreNames.contains(Gn) || t.createObjectStore(Gn, {
                 keyPath: "id",
                 autoIncrement: !0
             }).createIndex("id", "id", {
                 unique: !0
             })
         }
     })).close()
@@ -11652,21 +11654,21 @@
     groupNames: {},
     displayRecent: !1,
     additionalGroups: {},
     groupOrder: [],
     groupIcons: {}
 };
 async function NI() {
-    return await (await wf(_f, Nf)).transaction(Tn, "readonly").objectStore(Tn).getAll()
+    return await (await wf(_f, Nf)).transaction(Gn, "readonly").objectStore(Gn).getAll()
 }
 
 function MI() {
     const e = yo({
         search: "",
-        emoji: Pm,
+        emoji: Fm,
         activeGroup: "",
         skinTone: fs,
         options: _I,
         additionalGroups: {},
         recent: [],
         get emojis() {
             return ut(ut({
@@ -11712,15 +11714,15 @@
         r = (u = fs) => {
             e.skinTone = u
         },
         a = u => {
             e.options = Object.assign({}, e.options, u), t()
         };
     async function l() {
-        (await wf(_f, Nf)).transaction(Tn, "readwrite").objectStore(Tn).put({
+        (await wf(_f, Nf)).transaction(Gn, "readwrite").objectStore(Gn).put({
             id: 0,
             value: JSON.stringify(e.recent)
         })
     }
     const c = u => {
         if (e.options.displayRecent !== !0) return;
         const d = e.recent.findIndex(p => p.u === u.u);
@@ -11743,36 +11745,36 @@
 }
 var Je = "top",
     st = "bottom",
     it = "right",
     Ke = "left",
     Mf = "auto",
     Mo = [Je, st, it, Ke],
-    Gn = "start",
+    Tn = "start",
     ho = "end",
     ZI = "clippingParents",
     nc = "viewport",
     $n = "popper",
     WI = "reference",
     Yr = Mo.reduce(function(e, t) {
-        return e.concat([t + "-" + Gn, t + "-" + ho])
+        return e.concat([t + "-" + Tn, t + "-" + ho])
     }, []),
     oc = [].concat(Mo, [Mf]).reduce(function(e, t) {
-        return e.concat([t, t + "-" + Gn, t + "-" + ho])
+        return e.concat([t, t + "-" + Tn, t + "-" + ho])
     }, []),
     SI = "beforeRead",
     BI = "read",
     zI = "afterRead",
     VI = "beforeMain",
-    TI = "main",
-    GI = "afterMain",
+    GI = "main",
+    TI = "afterMain",
     jI = "beforeWrite",
     kI = "write",
     DI = "afterWrite",
-    RI = [SI, BI, zI, VI, TI, GI, jI, kI, DI];
+    RI = [SI, BI, zI, VI, GI, TI, jI, kI, DI];
 
 function At(e) {
     return e ? (e.nodeName || "").toLowerCase() : null
 }
 
 function gt(e) {
     if (e == null) return window;
@@ -11912,30 +11914,30 @@
     return ["table", "td", "th"].indexOf(At(e)) >= 0
 }
 
 function Qt(e) {
     return ((jn(e) ? e.ownerDocument : e.document) || window.document).documentElement
 }
 
-function Ts(e) {
+function Gs(e) {
     return At(e) === "html" ? e : e.assignedSlot || e.parentNode || (sc(e) ? e.host : null) || Qt(e)
 }
 
 function Er(e) {
     return !ot(e) || vt(e).position === "fixed" ? null : e.offsetParent
 }
 
 function HI(e) {
     var t = navigator.userAgent.toLowerCase().indexOf("firefox") !== -1,
         n = navigator.userAgent.indexOf("Trident") !== -1;
     if (n && ot(e)) {
         var o = vt(e);
         if (o.position === "fixed") return null
     }
-    for (var s = Ts(e); ot(s) && ["html", "body"].indexOf(At(s)) < 0;) {
+    for (var s = Gs(e); ot(s) && ["html", "body"].indexOf(At(s)) < 0;) {
         var i = vt(s);
         if (i.transform !== "none" || i.perspective !== "none" || i.contain === "paint" || ["transform", "perspective"].indexOf(i.willChange) !== -1 || t && i.willChange === "filter" || t && i.filter && i.filter !== "none") return s;
         s = s.parentNode
     }
     return null
 }
 
@@ -11995,19 +11997,19 @@
         var u = LI(s.padding, n),
             d = Zf(i),
             m = a === "y" ? Je : Ke,
             p = a === "y" ? st : it,
             h = n.rects.reference[c] + n.rects.reference[a] - f[a] - n.rects.popper[c],
             b = f[a] - n.rects.reference[a],
             y = Zo(i),
-            G = y ? a === "y" ? y.clientHeight || 0 : y.clientWidth || 0 : 0,
+            T = y ? a === "y" ? y.clientHeight || 0 : y.clientWidth || 0 : 0,
             N = h / 2 - b / 2,
             v = u[m],
-            E = G - d[c] - u[p],
-            J = G / 2 - d[c] / 2 + N,
+            E = T - d[c] - u[p],
+            J = T / 2 - d[c] / 2 + N,
             Y = oo(v, J, E),
             _ = a;
         n.modifiersData[o] = (t = {}, t[_] = Y, t.centerOffset = Y - J, t)
     }
 }
 
 function JI(e) {
@@ -12026,22 +12028,22 @@
     requires: ["popperOffsets"],
     requiresIfExists: ["preventOverflow"]
 };
 
 function Rn(e) {
     return e.split("-")[1]
 }
-var PI = {
+var FI = {
     top: "auto",
     right: "auto",
     bottom: "auto",
     left: "auto"
 };
 
-function FI(e) {
+function PI(e) {
     var t = e.x,
         n = e.y,
         o = window,
         s = o.devicePixelRatio || 1;
     return {
         x: kn(t * s) / s || 0,
         y: kn(n * s) / s || 0
@@ -12055,21 +12057,21 @@
         i = e.variation,
         f = e.offsets,
         r = e.position,
         a = e.gpuAcceleration,
         l = e.adaptive,
         c = e.roundOffsets,
         u = e.isFixed,
-        d = c === !0 ? FI(f) : typeof c == "function" ? c(f) : f,
+        d = c === !0 ? PI(f) : typeof c == "function" ? c(f) : f,
         m = d.x,
         p = m === void 0 ? 0 : m,
         h = d.y,
         b = h === void 0 ? 0 : h,
         y = f.hasOwnProperty("x"),
-        G = f.hasOwnProperty("y"),
+        T = f.hasOwnProperty("y"),
         N = Ke,
         v = Je,
         E = window;
     if (l) {
         var J = Zo(n),
             Y = "clientHeight",
             _ = "clientWidth";
@@ -12082,20 +12084,20 @@
             N = it;
             var A = u && E.visualViewport ? E.visualViewport.width : J[_];
             p -= A - o.width, p *= a ? 1 : -1
         }
     }
     var K = Object.assign({
         position: r
-    }, l && PI);
+    }, l && FI);
     if (a) {
-        var T;
-        return Object.assign({}, K, (T = {}, T[v] = G ? "0" : "", T[N] = y ? "0" : "", T.transform = (E.devicePixelRatio || 1) <= 1 ? "translate(" + p + "px, " + b + "px)" : "translate3d(" + p + "px, " + b + "px, 0)", T))
+        var G;
+        return Object.assign({}, K, (G = {}, G[v] = T ? "0" : "", G[N] = y ? "0" : "", G.transform = (E.devicePixelRatio || 1) <= 1 ? "translate(" + p + "px, " + b + "px)" : "translate3d(" + p + "px, " + b + "px, 0)", G))
     }
-    return Object.assign({}, K, (t = {}, t[v] = G ? b + "px" : "", t[N] = y ? p + "px" : "", t.transform = "", t))
+    return Object.assign({}, K, (t = {}, t[v] = T ? b + "px" : "", t[N] = y ? p + "px" : "", t.transform = "", t))
 }
 
 function $I(e) {
     var t = e.state,
         n = e.options,
         o = n.gpuAcceleration,
         s = o === void 0 ? !0 : o,
@@ -12237,26 +12239,26 @@
         n = t.overflow,
         o = t.overflowX,
         s = t.overflowY;
     return /auto|scroll|overlay|hidden/.test(n + s + o)
 }
 
 function lc(e) {
-    return ["html", "body", "#document"].indexOf(At(e)) >= 0 ? e.ownerDocument.body : ot(e) && zf(e) ? e : lc(Ts(e))
+    return ["html", "body", "#document"].indexOf(At(e)) >= 0 ? e.ownerDocument.body : ot(e) && zf(e) ? e : lc(Gs(e))
 }
 
 function so(e, t) {
     var n;
     t === void 0 && (t = []);
     var o = lc(e),
         s = o === ((n = e.ownerDocument) == null ? void 0 : n.body),
         i = gt(o),
         f = s ? [i].concat(i.visualViewport || [], zf(o) ? o : []) : o,
         r = t.concat(f);
-    return s ? r : r.concat(so(Ts(f)))
+    return s ? r : r.concat(so(Gs(f)))
 }
 
 function zi(e) {
     return Object.assign({}, e, {
         left: e.x,
         top: e.y,
         right: e.x + e.width,
@@ -12270,15 +12272,15 @@
 }
 
 function Lr(e, t) {
     return t === nc ? zi(oh(e)) : jn(t) ? ih(t) : zi(sh(Qt(e)))
 }
 
 function fh(e) {
-    var t = so(Ts(e)),
+    var t = so(Gs(e)),
         n = ["absolute", "fixed"].indexOf(vt(e).position) >= 0,
         o = n && ot(e) ? Zo(e) : e;
     return jn(o) ? t.filter(function(s) {
         return jn(s) && ic(s, o) && At(s) !== "body" && (n ? vt(s).position !== "static" : !0)
     }) : []
 }
 
@@ -12333,15 +12335,15 @@
                 y: t.y
             }
     }
     var l = s ? Wf(s) : null;
     if (l != null) {
         var c = l === "y" ? "height" : "width";
         switch (i) {
-            case Gn:
+            case Tn:
                 a[l] = a[l] - (t[c] / 2 - n[c] / 2);
                 break;
             case ho:
                 a[l] = a[l] + (t[c] / 2 - n[c] / 2);
                 break
         }
     }
@@ -12362,16 +12364,16 @@
         u = n.altBoundary,
         d = u === void 0 ? !1 : u,
         m = n.padding,
         p = m === void 0 ? 0 : m,
         h = rc(typeof p != "number" ? p : ac(p, Mo)),
         b = c === $n ? WI : $n,
         y = e.rects.popper,
-        G = e.elements[d ? b : c],
-        N = rh(jn(G) ? G : G.contextElement || Qt(e.elements.popper), f, a),
+        T = e.elements[d ? b : c],
+        N = rh(jn(T) ? T : T.contextElement || Qt(e.elements.popper), f, a),
         v = Dn(e.elements.reference),
         E = cc({
             reference: v,
             element: y,
             strategy: "absolute",
             placement: s
         }),
@@ -12383,17 +12385,17 @@
             left: N.left - Y.left + h.left,
             right: Y.right - N.right + h.right
         },
         R = e.modifiersData.offset;
     if (c === $n && R) {
         var A = R[s];
         Object.keys(_).forEach(function(K) {
-            var T = [it, st].indexOf(K) >= 0 ? 1 : -1,
+            var G = [it, st].indexOf(K) >= 0 ? 1 : -1,
                 z = [Je, st].indexOf(K) >= 0 ? "y" : "x";
-            _[K] += A[z] * T
+            _[K] += A[z] * G
         })
     }
     return _
 }
 
 function ah(e, t) {
     t === void 0 && (t = {});
@@ -12433,41 +12435,41 @@
 }
 
 function ch(e) {
     var t = e.state,
         n = e.options,
         o = e.name;
     if (!t.modifiersData[o]._skip) {
-        for (var s = n.mainAxis, i = s === void 0 ? !0 : s, f = n.altAxis, r = f === void 0 ? !0 : f, a = n.fallbackPlacements, l = n.padding, c = n.boundary, u = n.rootBoundary, d = n.altBoundary, m = n.flipVariations, p = m === void 0 ? !0 : m, h = n.allowedAutoPlacements, b = t.options.placement, y = Ct(b), G = y === b, N = a || (G || !p ? [Ko(b)] : lh(b)), v = [b].concat(N).reduce(function(je, ze) {
+        for (var s = n.mainAxis, i = s === void 0 ? !0 : s, f = n.altAxis, r = f === void 0 ? !0 : f, a = n.fallbackPlacements, l = n.padding, c = n.boundary, u = n.rootBoundary, d = n.altBoundary, m = n.flipVariations, p = m === void 0 ? !0 : m, h = n.allowedAutoPlacements, b = t.options.placement, y = Ct(b), T = y === b, N = a || (T || !p ? [Ko(b)] : lh(b)), v = [b].concat(N).reduce(function(je, ze) {
                 return je.concat(Ct(ze) === Mf ? ah(t, {
                     placement: ze,
                     boundary: c,
                     rootBoundary: u,
                     padding: l,
                     flipVariations: p,
                     allowedAutoPlacements: h
                 }) : ze)
             }, []), E = t.rects.reference, J = t.rects.popper, Y = new Map, _ = !0, R = v[0], A = 0; A < v.length; A++) {
             var K = v[A],
-                T = Ct(K),
-                z = Rn(K) === Gn,
-                M = [Je, st].indexOf(T) >= 0,
+                G = Ct(K),
+                z = Rn(K) === Tn,
+                M = [Je, st].indexOf(G) >= 0,
                 S = M ? "width" : "height",
                 k = bo(t, {
                     placement: K,
                     boundary: c,
                     rootBoundary: u,
                     altBoundary: d,
                     padding: l
                 }),
                 Z = M ? z ? it : Ke : z ? st : Je;
             E[S] > J[S] && (Z = Ko(Z));
             var H = Ko(Z),
                 $ = [];
-            if (i && $.push(k[T] <= 0), r && $.push(k[Z] <= 0, k[H] <= 0), $.every(function(je) {
+            if (i && $.push(k[G] <= 0), r && $.push(k[Z] <= 0, k[H] <= 0), $.every(function(je) {
                     return je
                 })) {
                 R = K, _ = !1;
                 break
             }
             Y.set(K, $)
         }
@@ -12630,16 +12632,16 @@
         b = bo(t, {
             boundary: a,
             rootBoundary: l,
             padding: u,
             altBoundary: c
         }),
         y = Ct(t.placement),
-        G = Rn(t.placement),
-        N = !G,
+        T = Rn(t.placement),
+        N = !T,
         v = Wf(y),
         E = Ch(v),
         J = t.modifiersData.popperOffsets,
         Y = t.rects.reference,
         _ = t.rects.popper,
         R = typeof h == "function" ? h(Object.assign({}, t.rects, {
             placement: t.placement
@@ -12648,29 +12650,29 @@
             mainAxis: R,
             altAxis: R
         } : Object.assign({
             mainAxis: 0,
             altAxis: 0
         }, R),
         K = t.modifiersData.offset ? t.modifiersData.offset[t.placement] : null,
-        T = {
+        G = {
             x: 0,
             y: 0
         };
     if (J) {
         if (i) {
             var z, M = v === "y" ? Je : Ke,
                 S = v === "y" ? st : it,
                 k = v === "y" ? "height" : "width",
                 Z = J[v],
                 H = Z + b[M],
                 $ = Z - b[S],
                 le = m ? -_[k] / 2 : 0,
-                Ie = G === Gn ? Y[k] : _[k],
-                fe = G === Gn ? -_[k] : -Y[k],
+                Ie = T === Tn ? Y[k] : _[k],
+                fe = T === Tn ? -_[k] : -Y[k],
                 we = t.elements.arrow,
                 je = m && we ? Zf(we) : {
                     width: 0,
                     height: 0
                 },
                 ze = t.modifiersData["arrow#persistent"] ? t.modifiersData["arrow#persistent"].padding : fc(),
                 We = ze[M],
@@ -12680,31 +12682,31 @@
                 Le = N ? -Y[k] / 2 + le + ke + Ee + A.mainAxis : fe + ke + Ee + A.mainAxis,
                 ft = t.elements.arrow && Zo(t.elements.arrow),
                 g = ft ? v === "y" ? ft.clientTop || 0 : ft.clientLeft || 0 : 0,
                 I = (z = K == null ? void 0 : K[v]) != null ? z : 0,
                 C = Z + ye - I - g,
                 B = Z + Le - I,
                 W = oo(m ? rs(H, C) : H, Z, m ? In($, B) : $);
-            J[v] = W, T[v] = W - Z
+            J[v] = W, G[v] = W - Z
         }
         if (r) {
             var x, O = v === "x" ? Je : Ke,
                 D = v === "x" ? st : it,
                 X = J[E],
                 V = E === "y" ? "height" : "width",
                 q = X + b[O],
-                P = X - b[D],
+                F = X - b[D],
                 Q = [Je, Ke].indexOf(y) !== -1,
                 ee = (x = K == null ? void 0 : K[E]) != null ? x : 0,
                 re = Q ? q : X - Y[V] - _[V] - ee + A.altAxis,
-                be = Q ? X + Y[V] + _[V] - ee - A.altAxis : P,
-                he = m && Q ? OI(re, X, be) : oo(m ? re : q, X, m ? be : P);
-            J[E] = he, T[E] = he - X
+                be = Q ? X + Y[V] + _[V] - ee - A.altAxis : F,
+                he = m && Q ? OI(re, X, be) : oo(m ? re : q, X, m ? be : F);
+            J[E] = he, G[E] = he - X
         }
-        t.modifiersData[o] = T
+        t.modifiersData[o] = G
     }
 }
 var Ah = {
     name: "preventOverflow",
     enabled: !0,
     phase: "main",
     fn: yh,
@@ -12808,15 +12810,15 @@
 }
 var Kr = {
     placement: "bottom",
     modifiers: [],
     strategy: "absolute"
 };
 
-function Pr() {
+function Fr() {
     for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
     return !t.some(function(o) {
         return !(o && typeof o.getBoundingClientRect == "function")
     })
 }
 
 function Bh(e) {
@@ -12841,32 +12843,32 @@
                 styles: {}
             },
             u = [],
             d = !1,
             m = {
                 state: c,
                 setOptions: function(y) {
-                    var G = typeof y == "function" ? y(c.options) : y;
-                    h(), c.options = Object.assign({}, i, c.options, G), c.scrollParents = {
+                    var T = typeof y == "function" ? y(c.options) : y;
+                    h(), c.options = Object.assign({}, i, c.options, T), c.scrollParents = {
                         reference: jn(r) ? so(r) : r.contextElement ? so(r.contextElement) : [],
                         popper: so(a)
                     };
                     var N = Zh(Sh([].concat(o, c.options.modifiers)));
                     return c.orderedModifiers = N.filter(function(v) {
                         return v.enabled
                     }), p(), m.update()
                 },
                 forceUpdate: function() {
                     if (!d) {
                         var y = c.elements,
-                            G = y.reference,
+                            T = y.reference,
                             N = y.popper;
-                        if (Pr(G, N)) {
+                        if (Fr(T, N)) {
                             c.rects = {
-                                reference: Nh(G, Zo(N), c.options.strategy === "fixed"),
+                                reference: Nh(T, Zo(N), c.options.strategy === "fixed"),
                                 popper: Zf(N)
                             }, c.reset = !1, c.placement = c.options.placement, c.orderedModifiers.forEach(function(A) {
                                 return c.modifiersData[A.name] = Object.assign({}, A.data)
                             });
                             for (var v = 0; v < c.orderedModifiers.length; v++) {
                                 if (c.reset === !0) {
                                     c.reset = !1, v = -1;
@@ -12892,24 +12894,24 @@
                         m.forceUpdate(), b(c)
                     })
                 }),
                 destroy: function() {
                     h(), d = !0
                 }
             };
-        if (!Pr(r, a)) return m;
+        if (!Fr(r, a)) return m;
         m.setOptions(l).then(function(b) {
             !d && l.onFirstUpdate && l.onFirstUpdate(b)
         });
 
         function p() {
             c.orderedModifiers.forEach(function(b) {
                 var y = b.name,
-                    G = b.options,
-                    N = G === void 0 ? {} : G,
+                    T = b.options,
+                    N = T === void 0 ? {} : T,
                     v = b.effect;
                 if (typeof v == "function") {
                     var E = v({
                             state: c,
                             name: y,
                             instance: m,
                             options: N
@@ -12930,19 +12932,19 @@
 }
 var zh = [eh, bh, QI, YI, Ih, uh, Ah, KI, gh],
     Vh = Bh({
         defaultModifiers: zh
     }),
     uc = "data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAzMiAzMiI+PHBhdGggZD0iTSAxNiA0IEMgOS4zODI4MTMgNCA0IDkuMzgyODEzIDQgMTYgQyA0IDIyLjYxNzE4OCA5LjM4MjgxMyAyOCAxNiAyOCBDIDIyLjYxNzE4OCAyOCAyOCAyMi42MTcxODggMjggMTYgQyAyOCA5LjM4MjgxMyAyMi42MTcxODggNCAxNiA0IFogTSAxNiA2IEMgMjEuNTM1MTU2IDYgMjYgMTAuNDY0ODQ0IDI2IDE2IEMgMjYgMjEuNTM1MTU2IDIxLjUzNTE1NiAyNiAxNiAyNiBDIDEwLjQ2NDg0NCAyNiA2IDIxLjUzNTE1NiA2IDE2IEMgNiAxMC40NjQ4NDQgMTAuNDY0ODQ0IDYgMTYgNiBaIE0gMTEuNSAxMiBDIDEwLjY3MTg3NSAxMiAxMCAxMi42NzE4NzUgMTAgMTMuNSBDIDEwIDE0LjMyODEyNSAxMC42NzE4NzUgMTUgMTEuNSAxNSBDIDEyLjMyODEyNSAxNSAxMyAxNC4zMjgxMjUgMTMgMTMuNSBDIDEzIDEyLjY3MTg3NSAxMi4zMjgxMjUgMTIgMTEuNSAxMiBaIE0gMjAuNSAxMiBDIDE5LjY3MTg3NSAxMiAxOSAxMi42NzE4NzUgMTkgMTMuNSBDIDE5IDE0LjMyODEyNSAxOS42NzE4NzUgMTUgMjAuNSAxNSBDIDIxLjMyODEyNSAxNSAyMiAxNC4zMjgxMjUgMjIgMTMuNSBDIDIyIDEyLjY3MTg3NSAyMS4zMjgxMjUgMTIgMjAuNSAxMiBaIE0gMTAuODEyNSAxOSBMIDkuMDkzNzUgMjAgQyAxMC40NzY1NjMgMjIuMzg2NzE5IDEzLjA0Njg3NSAyNCAxNiAyNCBDIDE4Ljk1MzEyNSAyNCAyMS41MjM0MzggMjIuMzg2NzE5IDIyLjkwNjI1IDIwIEwgMjEuMTg3NSAxOSBDIDIwLjE0ODQzOCAyMC43OTI5NjkgMTguMjI2NTYzIDIyIDE2IDIyIEMgMTMuNzczNDM4IDIyIDExLjg1MTU2MyAyMC43OTI5NjkgMTAuODEyNSAxOSBaIi8+PC9zdmc+";
 
-function Po(e) {
+function Fo(e) {
     return e.split("-").map(t => parseInt(t, 16)).map(t => String.fromCodePoint(t)).join("")
 }
 
-function Th(e, t, n, o = []) {
+function Gh(e, t, n, o = []) {
     const s = {};
     return Object.keys(e).forEach(i => {
         if (o.includes(i)) return;
         const f = [];
         e[i].forEach(r => {
             var a;
             if (r[Vs][0].includes(t.toLocaleLowerCase())) {
@@ -12967,57 +12969,57 @@
 function gc(e) {
     return e.replace(/^_*(.)|_+(.)/g, (t, n, o) => n ? n.toUpperCase() : " " + o.toUpperCase())
 }
 var Wo = (e, t) => {
     for (const [n, o] of t) e[n] = o;
     return e
 };
-const Gh = Ce({
+const Th = Ce({
         name: "Body",
         setup() {
             const {
                 state: e,
                 updateEmoji: t,
                 updateSelect: n
-            } = Nt("store"), o = oe(null), s = ue(() => Th(e.emojis, e.search, e.skinTone, e.options.disabledGroups)), i = uf(), f = ue(() => !e.options.hideGroupNames), r = ue(() => !e.options.disableStickyGroupNames), a = ce(e.options.groupNames), l = e.orderedGroupKeys;
+            } = Nt("store"), o = oe(null), s = ue(() => Gh(e.emojis, e.search, e.skinTone, e.options.disabledGroups)), i = uf(), f = ue(() => !e.options.hideGroupNames), r = ue(() => !e.options.disableStickyGroupNames), a = ce(e.options.groupNames), l = e.orderedGroupKeys;
             e.options.additionalGroups && Object.keys(e.options.additionalGroups).map(p => {
                 e.options.groupNames[p] ? a[p] = e.options.groupNames[p] : a[p] = gc(p)
             });
             const c = dc() ? "is-mac" : "";
 
             function u(p) {
                 t(p)
             }
 
             function d(p) {
                 n(p), i == null || i.emit("select", No(ut({}, p), {
                     t: e.skinTone,
-                    i: Po(p.r)
+                    i: Fo(p.r)
                 }))
             }
 
             function m(p, h) {
                 var b;
                 const y = (b = p == null ? void 0 : p.target) == null ? void 0 : b.closest("button");
-                y && (y.innerHTML = `<span>${Po(h)}</span>`)
+                y && (y.innerHTML = `<span>${Fo(h)}</span>`)
             }
             return pn(() => e.activeGroup, () => {
                 var p;
                 const h = (p = o.value) == null ? void 0 : p.querySelector("#" + e.activeGroup);
                 h && (h.parentNode.scrollTop = h.offsetTop - h.parentNode.offsetTop)
             }), {
                 emojis: s,
                 bodyInner: o,
                 EMOJI_REMOTE_SRC: $l,
                 GROUP_NAMES: Ql,
                 handleClick: d,
                 handleError: m,
                 handleMouseEnter: u,
                 native: e.options.native,
-                unicodeToEmoji: Po,
+                unicodeToEmoji: Fo,
                 EMOJI_RESULT_KEY: Io,
                 EMOJI_NAME_KEY: Vs,
                 hasGroupNames: f,
                 isSticky: r,
                 platform: c,
                 groupNames: a,
                 orderedKeys: l
@@ -13038,52 +13040,52 @@
     Xh = ["src", "alt", "onError"],
     Yh = {
         key: 1,
         class: "v3-no-result"
     };
 
 function Eh(e, t, n, o, s, i) {
-    return j(), U("div", jh, [F("div", {
+    return j(), U("div", jh, [P("div", {
         ref: "bodyInner",
         class: L([e.platform, "v3-body-inner"])
     }, [e.orderedKeys.length ? (j(!0), U(_e, {
         key: 0
     }, Cn(e.orderedKeys, f => (j(), U("div", {
         id: f,
         key: f,
         class: "v3-group"
     }, [e.hasGroupNames ? bn((j(), U("h5", {
         key: 0,
         class: L(e.isSticky ? "v3-sticky" : "")
-    }, Te(e.groupNames[f]), 3)), [
+    }, Ge(e.groupNames[f]), 3)), [
         [Ar, e.emojis[f]]
-    ]) : me("", !0), bn(F("div", Dh, [(j(!0), U(_e, null, Cn(e.emojis[f], r => (j(), U("button", {
+    ]) : me("", !0), bn(P("div", Dh, [(j(!0), U(_e, null, Cn(e.emojis[f], r => (j(), U("button", {
         key: r.r,
         type: "button",
         onMouseenter: a => e.handleMouseEnter(r),
         onClick: a => e.handleClick(r)
-    }, [e.native ? (j(), U("span", xh, Te(e.unicodeToEmoji(r.r)), 1)) : (j(), U("img", {
+    }, [e.native ? (j(), U("span", xh, Ge(e.unicodeToEmoji(r.r)), 1)) : (j(), U("img", {
         key: 1,
         src: e.EMOJI_REMOTE_SRC + `/${r.r}.png`,
         alt: r.n[0],
         onError: a => e.handleError(a, r.r)
     }, null, 40, Xh))], 40, Rh))), 128))], 512), [
         [Ar, e.emojis[f]]
     ])], 8, kh))), 128)) : (j(), U("span", Yh, " No emoji has been found! "))], 2)])
 }
-var Hh = Wo(Gh, [
+var Hh = Wo(Th, [
         ["render", Eh]
     ]),
     Oh = "data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAzMiAzMiI+PHBhdGggZD0iTSAxMi41IDUgQyAxMS40Mjk2ODggNSAxMC41IDUuNjA5Mzc1IDkuOTA2MjUgNi40Mzc1IEMgOS4zMTI1IDcuMjY1NjI1IDkgOC4zMzk4NDQgOSA5LjUgQyA5IDEwLjY2MDE1NiA5LjMxMjUgMTEuNzM0Mzc1IDkuOTA2MjUgMTIuNTYyNSBDIDEwLjUgMTMuMzkwNjI1IDExLjQyOTY4OCAxNCAxMi41IDE0IEMgMTMuNTcwMzEzIDE0IDE0LjUgMTMuMzkwNjI1IDE1LjA5Mzc1IDEyLjU2MjUgQyAxNS42ODc1IDExLjczNDM3NSAxNiAxMC42NjAxNTYgMTYgOS41IEMgMTYgOC4zMzk4NDQgMTUuNjg3NSA3LjI2NTYyNSAxNS4wOTM3NSA2LjQzNzUgQyAxNC41IDUuNjA5Mzc1IDEzLjU3MDMxMyA1IDEyLjUgNSBaIE0gMTYgOS41IEMgMTYgMTAuNjYwMTU2IDE2LjMxMjUgMTEuNzM0Mzc1IDE2LjkwNjI1IDEyLjU2MjUgQyAxNy41IDEzLjM5MDYyNSAxOC40Mjk2ODggMTQgMTkuNSAxNCBDIDIwLjU3MDMxMyAxNCAyMS41IDEzLjM5MDYyNSAyMi4wOTM3NSAxMi41NjI1IEMgMjIuNjg3NSAxMS43MzQzNzUgMjMgMTAuNjYwMTU2IDIzIDkuNSBDIDIzIDguMzM5ODQ0IDIyLjY4NzUgNy4yNjU2MjUgMjIuMDkzNzUgNi40Mzc1IEMgMjEuNSA1LjYwOTM3NSAyMC41NzAzMTMgNSAxOS41IDUgQyAxOC40Mjk2ODggNSAxNy41IDUuNjA5Mzc1IDE2LjkwNjI1IDYuNDM3NSBDIDE2LjMxMjUgNy4yNjU2MjUgMTYgOC4zMzk4NDQgMTYgOS41IFogTSAxMi41IDcgQyAxMi44MTI1IDcgMTMuMTU2MjUgNy4xNTYyNSAxMy40Njg3NSA3LjU5Mzc1IEMgMTMuNzgxMjUgOC4wMzEyNSAxNCA4LjcyNjU2MyAxNCA5LjUgQyAxNCAxMC4yNzM0MzggMTMuNzgxMjUgMTAuOTY4NzUgMTMuNDY4NzUgMTEuNDA2MjUgQyAxMy4xNTYyNSAxMS44NDM3NSAxMi44MTI1IDEyIDEyLjUgMTIgQyAxMi4xODc1IDEyIDExLjg0Mzc1IDExLjg0Mzc1IDExLjUzMTI1IDExLjQwNjI1IEMgMTEuMjE4NzUgMTAuOTY4NzUgMTEgMTAuMjczNDM4IDExIDkuNSBDIDExIDguNzI2NTYzIDExLjIxODc1IDguMDMxMjUgMTEuNTMxMjUgNy41OTM3NSBDIDExLjg0Mzc1IDcuMTU2MjUgMTIuMTg3NSA3IDEyLjUgNyBaIE0gMTkuNSA3IEMgMTkuODEyNSA3IDIwLjE1NjI1IDcuMTU2MjUgMjAuNDY4NzUgNy41OTM3NSBDIDIwLjc4MTI1IDguMDMxMjUgMjEgOC43MjY1NjMgMjEgOS41IEMgMjEgMTAuMjczNDM4IDIwLjc4MTI1IDEwLjk2ODc1IDIwLjQ2ODc1IDExLjQwNjI1IEMgMjAuMTU2MjUgMTEuODQzNzUgMTkuODEyNSAxMiAxOS41IDEyIEMgMTkuMTg3NSAxMiAxOC44NDM3NSAxMS44NDM3NSAxOC41MzEyNSAxMS40MDYyNSBDIDE4LjIxODc1IDEwLjk2ODc1IDE4IDEwLjI3MzQzOCAxOCA5LjUgQyAxOCA4LjcyNjU2MyAxOC4yMTg3NSA4LjAzMTI1IDE4LjUzMTI1IDcuNTkzNzUgQyAxOC44NDM3NSA3LjE1NjI1IDE5LjE4NzUgNyAxOS41IDcgWiBNIDcuNSAxMiBDIDYuNDI5Njg4IDEyIDUuNSAxMi42MDkzNzUgNC45MDYyNSAxMy40Mzc1IEMgNC4zMTI1IDE0LjI2NTYyNSA0IDE1LjMzOTg0NCA0IDE2LjUgQyA0IDE3LjY2MDE1NiA0LjMxMjUgMTguNzM0Mzc1IDQuOTA2MjUgMTkuNTYyNSBDIDUuNSAyMC4zOTA2MjUgNi40Mjk2ODggMjEgNy41IDIxIEMgOC41NzAzMTMgMjEgOS41IDIwLjM5MDYyNSAxMC4wOTM3NSAxOS41NjI1IEMgMTAuNjg3NSAxOC43MzQzNzUgMTEgMTcuNjYwMTU2IDExIDE2LjUgQyAxMSAxNS4zMzk4NDQgMTAuNjg3NSAxNC4yNjU2MjUgMTAuMDkzNzUgMTMuNDM3NSBDIDkuNSAxMi42MDkzNzUgOC41NzAzMTMgMTIgNy41IDEyIFogTSAyNC41IDEyIEMgMjMuNDI5Njg4IDEyIDIyLjUgMTIuNjA5Mzc1IDIxLjkwNjI1IDEzLjQzNzUgQyAyMS4zMTI1IDE0LjI2NTYyNSAyMSAxNS4zMzk4NDQgMjEgMTYuNSBDIDIxIDE3LjY2MDE1NiAyMS4zMTI1IDE4LjczNDM3NSAyMS45MDYyNSAxOS41NjI1IEMgMjIuNSAyMC4zOTA2MjUgMjMuNDI5Njg4IDIxIDI0LjUgMjEgQyAyNS41NzAzMTMgMjEgMjYuNSAyMC4zOTA2MjUgMjcuMDkzNzUgMTkuNTYyNSBDIDI3LjY4NzUgMTguNzM0Mzc1IDI4IDE3LjY2MDE1NiAyOCAxNi41IEMgMjggMTUuMzM5ODQ0IDI3LjY4NzUgMTQuMjY1NjI1IDI3LjA5Mzc1IDEzLjQzNzUgQyAyNi41IDEyLjYwOTM3NSAyNS41NzAzMTMgMTIgMjQuNSAxMiBaIE0gNy41IDE0IEMgNy44MTI1IDE0IDguMTU2MjUgMTQuMTU2MjUgOC40Njg3NSAxNC41OTM3NSBDIDguNzgxMjUgMTUuMDMxMjUgOSAxNS43MjY1NjMgOSAxNi41IEMgOSAxNy4yNzM0MzggOC43ODEyNSAxNy45Njg3NSA4LjQ2ODc1IDE4LjQwNjI1IEMgOC4xNTYyNSAxOC44NDM3NSA3LjgxMjUgMTkgNy41IDE5IEMgNy4xODc1IDE5IDYuODQzNzUgMTguODQzNzUgNi41MzEyNSAxOC40MDYyNSBDIDYuMjE4NzUgMTcuOTY4NzUgNiAxNy4yNzM0MzggNiAxNi41IEMgNiAxNS43MjY1NjMgNi4yMTg3NSAxNS4wMzEyNSA2LjUzMTI1IDE0LjU5Mzc1IEMgNi44NDM3NSAxNC4xNTYyNSA3LjE4NzUgMTQgNy41IDE0IFogTSAyNC41IDE0IEMgMjQuODEyNSAxNCAyNS4xNTYyNSAxNC4xNTYyNSAyNS40Njg3NSAxNC41OTM3NSBDIDI1Ljc4MTI1IDE1LjAzMTI1IDI2IDE1LjcyNjU2MyAyNiAxNi41IEMgMjYgMTcuMjczNDM4IDI1Ljc4MTI1IDE3Ljk2ODc1IDI1LjQ2ODc1IDE4LjQwNjI1IEMgMjUuMTU2MjUgMTguODQzNzUgMjQuODEyNSAxOSAyNC41IDE5IEMgMjQuMTg3NSAxOSAyMy44NDM3NSAxOC44NDM3NSAyMy41MzEyNSAxOC40MDYyNSBDIDIzLjIxODc1IDE3Ljk2ODc1IDIzIDE3LjI3MzQzOCAyMyAxNi41IEMgMjMgMTUuNzI2NTYzIDIzLjIxODc1IDE1LjAzMTI1IDIzLjUzMTI1IDE0LjU5Mzc1IEMgMjMuODQzNzUgMTQuMTU2MjUgMjQuMTg3NSAxNCAyNC41IDE0IFogTSAxNiAxNiBDIDE0LjY2Nzk2OSAxNiAxMy43MzgyODEgMTYuODY3MTg4IDEzLjI4MTI1IDE3LjYyNSBDIDEyLjgyNDIxOSAxOC4zODI4MTMgMTIuNTQ2ODc1IDE5LjAxNTYyNSAxMi4yODEyNSAxOS4yODEyNSBDIDEyLjEyNSAxOS40Mzc1IDExLjE2MDE1NiAxOS44MDA3ODEgMTAuMTU2MjUgMjAuMzEyNSBDIDkuNjUyMzQ0IDIwLjU3MDMxMyA5LjE0NDUzMSAyMC45MTQwNjMgOC43MTg3NSAyMS40Mzc1IEMgOC4yOTI5NjkgMjEuOTYwOTM4IDggMjIuNjg3NSA4IDIzLjUgQyA4IDI1LjQyMTg3NSA5LjU3ODEyNSAyNyAxMS41IDI3IEMgMTIuMzY3MTg4IDI3IDEzLjI2OTUzMSAyNi43MjI2NTYgMTQuMTU2MjUgMjYuNDY4NzUgQyAxNS4wNDI5NjkgMjYuMjE0ODQ0IDE2IDI2IDE2IDI2IEMgMTYgMjYgMTYuOTU3MDMxIDI2LjIxNDg0NCAxNy44NDM3NSAyNi40Njg3NSBDIDE4LjczMDQ2OSAyNi43MjI2NTYgMTkuNjMyODEzIDI3IDIwLjUgMjcgQyAyMi40MjE4NzUgMjcgMjQgMjUuNDIxODc1IDI0IDIzLjUgQyAyNCAyMi43MDcwMzEgMjMuNzA3MDMxIDIxLjk4MDQ2OSAyMy4yODEyNSAyMS40Njg3NSBDIDIyLjg1NTQ2OSAyMC45NTcwMzEgMjIuMzQzNzUgMjAuNjQwNjI1IDIxLjg0Mzc1IDIwLjM3NSBDIDIwLjg0Mzc1IDE5Ljg0Mzc1IDE5Ljg1OTM3NSAxOS40MjE4NzUgMTkuNzE4NzUgMTkuMjgxMjUgQyAxOS40ODA0NjkgMTkuMDQyOTY5IDE5LjIxMDkzOCAxOC4zOTA2MjUgMTguNzUgMTcuNjI1IEMgMTguMjg5MDYzIDE2Ljg1OTM3NSAxNy4zMzk4NDQgMTYgMTYgMTYgWiBNIDE2IDE4IEMgMTYuNjYwMTU2IDE4IDE2LjczNDM3NSAxOC4xNjAxNTYgMTcuMDMxMjUgMTguNjU2MjUgQyAxNy4zMjgxMjUgMTkuMTUyMzQ0IDE3LjU1NDY4OCAxOS45OTIxODggMTguMjgxMjUgMjAuNzE4NzUgQyAxOS4xMDU0NjkgMjEuNTQyOTY5IDIwLjE0ODQzOCAyMS43MjI2NTYgMjAuOTA2MjUgMjIuMTI1IEMgMjEuMjg1MTU2IDIyLjMyODEyNSAyMS41NzgxMjUgMjIuNTQyOTY5IDIxLjc1IDIyLjc1IEMgMjEuOTIxODc1IDIyLjk1NzAzMSAyMiAyMy4xNDg0MzggMjIgMjMuNSBDIDIyIDI0LjMzOTg0NCAyMS4zMzk4NDQgMjUgMjAuNSAyNSBDIDIwLjIxMDkzOCAyNSAxOS4yNzczNDQgMjQuNzc3MzQ0IDE4LjQwNjI1IDI0LjUzMTI1IEMgMTcuNTM1MTU2IDI0LjI4NTE1NiAxNi44MTY0MDYgMjQgMTYgMjQgQyAxNS4xODM1OTQgMjQgMTQuNDY0ODQ0IDI0LjI4NTE1NiAxMy41OTM3NSAyNC41MzEyNSBDIDEyLjcyMjY1NiAyNC43NzczNDQgMTEuNzg5MDYzIDI1IDExLjUgMjUgQyAxMC42NjAxNTYgMjUgMTAgMjQuMzM5ODQ0IDEwIDIzLjUgQyAxMCAyMy4wOTc2NTYgMTAuMDgyMDMxIDIyLjg5MDYyNSAxMC4yNSAyMi42ODc1IEMgMTAuNDE3OTY5IDIyLjQ4NDM3NSAxMC43MjI2NTYgMjIuMjg1MTU2IDExLjA5Mzc1IDIyLjA5Mzc1IEMgMTEuODM5ODQ0IDIxLjcxNDg0NCAxMi44NzUgMjEuNTYyNSAxMy43MTg3NSAyMC43MTg3NSBDIDE0LjQ1MzEyNSAxOS45ODQzNzUgMTQuNjc1NzgxIDE5LjExNzE4OCAxNC45Njg3NSAxOC42MjUgQyAxNS4yNjE3MTkgMTguMTMyODEzIDE1LjMzMjAzMSAxOCAxNiAxOCBaIi8+PC9zdmc+",
     Lh = "data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAzMiAzMiI+PHBhdGggZD0iTSAxMSAzIEwgMTEgNyBMIDEzIDcgTCAxMyAzIFogTSAxNSA0IEwgMTUgNyBMIDE3IDcgTCAxNyA0IFogTSA0Ljg3NSA4IEwgNSA5LjA5Mzc1IEwgNi44MTI1IDI2LjMxMjUgQyA2Ljk3MjY1NiAyNy44MzIwMzEgOC4yODUxNTYgMjkgOS44MTI1IDI5IEwgMTkuMTg3NSAyOSBDIDIwLjcxNDg0NCAyOSAyMi4wMjczNDQgMjcuODMyMDMxIDIyLjE4NzUgMjYuMzEyNSBMIDIyLjY1NjI1IDIyIEwgMjUgMjIgQyAyNi42NDQ1MzEgMjIgMjggMjAuNjQ0NTMxIDI4IDE5IEwgMjggMTYgQyAyOCAxNC4zNTU0NjkgMjYuNjQ0NTMxIDEzIDI1IDEzIEwgMjMuNTkzNzUgMTMgTCAyNCA5LjA5Mzc1IEwgMjQuMTI1IDggWiBNIDcuMTI1IDEwIEwgMjEuODc1IDEwIEwgMjAuMTg3NSAyNi4wOTM3NSBDIDIwLjEzMjgxMyAyNi42MTMyODEgMTkuNzA3MDMxIDI3IDE5LjE4NzUgMjcgTCA5LjgxMjUgMjcgQyA5LjI5Mjk2OSAyNyA4Ljg2NzE4OCAyNi42MTMyODEgOC44MTI1IDI2LjA5Mzc1IFogTSAyMy4zNzUgMTUgTCAyNSAxNSBDIDI1LjU2NjQwNiAxNSAyNiAxNS40MzM1OTQgMjYgMTYgTCAyNiAxOSBDIDI2IDE5LjU2NjQwNiAyNS41NjY0MDYgMjAgMjUgMjAgTCAyMi44NDM3NSAyMCBaIi8+PC9zdmc+",
     Uh = "data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAzMiAzMiI+PHBhdGggZD0iTSAxNiAzIEMgOC44MzIwMzEgMyAzIDguODMyMDMxIDMgMTYgQyAzIDIzLjE2Nzk2OSA4LjgzMjAzMSAyOSAxNiAyOSBDIDIzLjE2Nzk2OSAyOSAyOSAyMy4xNjc5NjkgMjkgMTYgQyAyOSA4LjgzMjAzMSAyMy4xNjc5NjkgMyAxNiAzIFogTSAxNiA1IEMgMTYuNjAxNTYzIDUgMTcuMTc1NzgxIDUuMDYyNSAxNy43NSA1LjE1NjI1IEwgMTYgNi40MDYyNSBMIDE0LjI1IDUuMTU2MjUgQyAxNC44MjAzMTMgNS4wNjY0MDYgMTUuNDAyMzQ0IDUgMTYgNSBaIE0gMTEuODEyNSA1Ljg0Mzc1IEwgMTUuNDA2MjUgOC40Njg3NSBMIDE2IDguOTA2MjUgTCAxNi41OTM3NSA4LjQ2ODc1IEwgMjAuMTg3NSA1Ljg0Mzc1IEMgMjEuNzg1MTU2IDYuNTA3ODEzIDIzLjE5NTMxMyA3LjUyMzQzOCAyNC4zMTI1IDguODEyNSBMIDIyLjkzNzUgMTMuMDkzNzUgTCAyMi43MTg3NSAxMy43ODEyNSBMIDIzLjMxMjUgMTQuMTg3NSBMIDI2LjkzNzUgMTYuODQzNzUgQyAyNi44MDQ2ODggMTguNjA1NDY5IDI2LjI2NTYyNSAyMC4yNTc4MTMgMjUuNDA2MjUgMjEuNjg3NSBMIDIwLjEyNSAyMS42ODc1IEwgMTkuOTA2MjUgMjIuMzc1IEwgMTguNSAyNi43MTg3NSBDIDE3LjY5OTIxOSAyNi45MDYyNSAxNi44NTkzNzUgMjcgMTYgMjcgQyAxNS4xMDU0NjkgMjcgMTQuMjM4MjgxIDI2Ljg4NjcxOSAxMy40MDYyNSAyNi42ODc1IEwgMTIuMDMxMjUgMjIuNDA2MjUgTCAxMS44MTI1IDIxLjcxODc1IEwgNi41OTM3NSAyMS43MTg3NSBDIDUuNzE4NzUgMjAuMjgxMjUgNS4xOTkyMTkgMTguNjIxMDk0IDUuMDYyNSAxNi44NDM3NSBMIDguNjU2MjUgMTQuMjE4NzUgTCA5LjI1IDEzLjgxMjUgTCA5LjAzMTI1IDEzLjEyNSBMIDcuNjI1IDguODc1IEMgOC43NSA3LjU1NDY4OCAxMC4xODM1OTQgNi41MTU2MjUgMTEuODEyNSA1Ljg0Mzc1IFogTSAxNiAxMC4wOTM3NSBMIDE1LjQwNjI1IDEwLjUzMTI1IEwgMTAuODQzNzUgMTMuODQzNzUgTCAxMC4yODEyNSAxNC4yODEyNSBMIDEwLjUgMTQuOTY4NzUgTCAxMi4yNSAyMC4zMTI1IEwgMTIuNDY4NzUgMjEgTCAxOS41MzEyNSAyMSBMIDE5Ljc1IDIwLjMxMjUgTCAyMS41IDE0Ljk2ODc1IEwgMjEuNzE4NzUgMTQuMjgxMjUgTCAyMS4xNTYyNSAxMy44NDM3NSBMIDE2LjU5Mzc1IDEwLjUzMTI1IFogTSAyNS43NSAxMC45MDYyNSBDIDI2LjI5Njg3NSAxMS45NTMxMjUgMjYuNjU2MjUgMTMuMTAxNTYzIDI2Ljg0Mzc1IDE0LjMxMjUgTCAyNS4wNjI1IDEzLjAzMTI1IFogTSA2LjIxODc1IDEwLjk2ODc1IEwgNi45MDYyNSAxMy4wMzEyNSBMIDUuMTU2MjUgMTQuMzEyNSBDIDUuMzM5ODQ0IDEzLjEyNSA1LjY4NzUgMTIgNi4yMTg3NSAxMC45Njg3NSBaIE0gMTYgMTIuNTkzNzUgTCAxOS4zNzUgMTUuMDMxMjUgTCAxOC4wOTM3NSAxOSBMIDEzLjkwNjI1IDE5IEwgMTIuNjI1IDE1LjAzMTI1IFogTSAyMS41OTM3NSAyMy42ODc1IEwgMjMuODQzNzUgMjMuNjg3NSBDIDIyLjk5MjE4OCAyNC41NjY0MDYgMjIuMDExNzE5IDI1LjI5Mjk2OSAyMC45MDYyNSAyNS44NDM3NSBaIE0gOC4xNTYyNSAyMy43MTg3NSBMIDEwLjM0Mzc1IDIzLjcxODc1IEwgMTEuMDMxMjUgMjUuODEyNSBDIDkuOTYwOTM4IDI1LjI2OTUzMSA4Ljk4ODI4MSAyNC41NjI1IDguMTU2MjUgMjMuNzE4NzUgWiIvPjwvc3ZnPg==",
     Jh = "data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAzMiAzMiI+PHBhdGggZD0iTSA5LjUgNiBDIDguMTc5Njg4IDYgNy4wMDM5MDYgNi44NTkzNzUgNi42MjUgOC4xMjUgTCA1LjI1IDEyLjcxODc1IEwgMy4zMTI1IDEyLjA2MjUgTCAyLjY4NzUgMTMuOTM3NSBMIDQuNjU2MjUgMTQuNTkzNzUgTCA0LjAzMTI1IDE2LjcxODc1IEMgNC4wMDc4MTMgMTYuODA4NTk0IDMuOTk2MDk0IDE2LjkwNjI1IDQgMTcgTCA0IDI0IEMgNCAyNC4wMzEyNSA0IDI0LjA2MjUgNCAyNC4wOTM3NSBMIDQgMjUgQyA0IDI1LjU1MDc4MSA0LjQ0OTIxOSAyNiA1IDI2IEwgOCAyNiBMIDguMzQzNzUgMjUgTCAyMy42NTYyNSAyNSBMIDI0IDI2IEwgMjcgMjYgQyAyNy41NTA3ODEgMjYgMjggMjUuNTUwNzgxIDI4IDI1IEwgMjggMjQuMTU2MjUgQyAyOC4wMDM5MDYgMjQuMTA1NDY5IDI4LjAwMzkwNiAyNC4wNTA3ODEgMjggMjQgTCAyOCAxNyBDIDI4LjAwMzkwNiAxNi45MDYyNSAyNy45OTIxODggMTYuODA4NTk0IDI3Ljk2ODc1IDE2LjcxODc1IEwgMjcuMzQzNzUgMTQuNTkzNzUgTCAyOS4zMTI1IDEzLjkzNzUgTCAyOC42ODc1IDEyLjA2MjUgTCAyNi43NSAxMi43MTg3NSBMIDI1LjM3NSA4LjEyNSBDIDI0Ljk5NjA5NCA2Ljg1OTM3NSAyMy44MjAzMTMgNiAyMi41IDYgWiBNIDkuNSA4IEwgMjIuNSA4IEMgMjIuOTQ1MzEzIDggMjMuMzM5ODQ0IDguMjkyOTY5IDIzLjQ2ODc1IDguNzE4NzUgTCAyNC43NSAxMyBMIDcuMjUgMTMgTCA4LjUzMTI1IDguNzE4NzUgQyA4LjY2MDE1NiA4LjI4OTA2MyA5LjA1NDY4OCA4IDkuNSA4IFogTSA2LjY1NjI1IDE1IEwgMjUuMzQzNzUgMTUgTCAyNiAxNy4xODc1IEwgMjYgMjMgTCA2IDIzIEwgNiAxNy4xODc1IFogTSA4LjUgMTYgQyA3LjY3MTg3NSAxNiA3IDE2LjY3MTg3NSA3IDE3LjUgQyA3IDE4LjMyODEyNSA3LjY3MTg3NSAxOSA4LjUgMTkgQyA5LjMyODEyNSAxOSAxMCAxOC4zMjgxMjUgMTAgMTcuNSBDIDEwIDE2LjY3MTg3NSA5LjMyODEyNSAxNiA4LjUgMTYgWiBNIDIzLjUgMTYgQyAyMi42NzE4NzUgMTYgMjIgMTYuNjcxODc1IDIyIDE3LjUgQyAyMiAxOC4zMjgxMjUgMjIuNjcxODc1IDE5IDIzLjUgMTkgQyAyNC4zMjgxMjUgMTkgMjUgMTguMzI4MTI1IDI1IDE3LjUgQyAyNSAxNi42NzE4NzUgMjQuMzI4MTI1IDE2IDIzLjUgMTYgWiBNIDEyIDE5IEwgMTAuNzUgMjIgTCAxMi45MDYyNSAyMiBMIDEzLjM0Mzc1IDIxIEwgMTguNjU2MjUgMjEgTCAxOS4wOTM3NSAyMiBMIDIxLjI1IDIyIEwgMjAgMTkgWiIvPjwvc3ZnPg==",
     Kh = "data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAzMiAzMiI+PHBhdGggZD0iTSAxNiA0IEMgMTEuMDQyOTY5IDQgNyA4LjA0Mjk2OSA3IDEzIEMgNyAxNC45MTc5NjkgNy44NDM3NSAxNi45MDYyNSA5IDE4LjY4NzUgQyA5Ljg1OTM3NSAyMC4wMTE3MTkgMTAuODg2NzE5IDIxLjIzMDQ2OSAxMiAyMi4xNTYyNSBMIDEyIDI1IEMgMTIgMjYuMDkzNzUgMTIuOTA2MjUgMjcgMTQgMjcgTCAxNSAyOCBMIDE3IDI4IEwgMTggMjcgQyAxOS4wOTM3NSAyNyAyMCAyNi4wOTM3NSAyMCAyNSBMIDIwIDIyLjE1NjI1IEMgMjEuMTEzMjgxIDIxLjIzMDQ2OSAyMi4xNDA2MjUgMjAuMDExNzE5IDIzIDE4LjY4NzUgQyAyNC4xNTYyNSAxNi45MDYyNSAyNSAxNC45MTc5NjkgMjUgMTMgQyAyNSA4LjA0Mjk2OSAyMC45NTcwMzEgNCAxNiA0IFogTSAxNiA2IEMgMTkuODc4OTA2IDYgMjMgOS4xMjEwOTQgMjMgMTMgQyAyMyAxNC4zMDg1OTQgMjIuMzU1NDY5IDE2LjAzNTE1NiAyMS4zNDM3NSAxNy41OTM3NSBDIDIwLjQ0MTQwNiAxOC45ODQzNzUgMTkuMjUzOTA2IDIwLjIyMjY1NiAxOC4xNTYyNSAyMSBMIDEzLjg0Mzc1IDIxIEMgMTIuNzQ2MDk0IDIwLjIyMjY1NiAxMS41NTg1OTQgMTguOTg0Mzc1IDEwLjY1NjI1IDE3LjU5Mzc1IEMgOS42NDQ1MzEgMTYuMDM1MTU2IDkgMTQuMzA4NTk0IDkgMTMgQyA5IDkuMTIxMDk0IDEyLjEyMTA5NCA2IDE2IDYgWiBNIDE0LjI1IDIzIEwgMTcuNzUgMjMgQyAxNy44MjgxMjUgMjMuMDU0Njg4IDE3LjkxMDE1NiAyMy4wOTM3NSAxOCAyMy4xMjUgTCAxOCAyNSBMIDE0IDI1IEwgMTQgMjMuMTI1IEMgMTQuMDg5ODQ0IDIzLjA5Mzc1IDE0LjE3MTg3NSAyMy4wNTQ2ODggMTQuMjUgMjMgWiIvPjwvc3ZnPg==",
-    Ph = "data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAzMiAzMiI+PHBhdGggZD0iTSAxMSA1IEwgMTEgMTEgTCA1IDExIEwgNSAxMyBMIDExIDEzIEwgMTEgMTkgTCA1IDE5IEwgNSAyMSBMIDExIDIxIEwgMTEgMjcgTCAxMyAyNyBMIDEzIDIxIEwgMTkgMjEgTCAxOSAyNyBMIDIxIDI3IEwgMjEgMjEgTCAyNyAyMSBMIDI3IDE5IEwgMjEgMTkgTCAyMSAxMyBMIDI3IDEzIEwgMjcgMTEgTCAyMSAxMSBMIDIxIDUgTCAxOSA1IEwgMTkgMTEgTCAxMyAxMSBMIDEzIDUgWiBNIDEzIDEzIEwgMTkgMTMgTCAxOSAxOSBMIDEzIDE5IFoiLz48L3N2Zz4=",
-    Fh = "data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAzMiAzMiI+PHBhdGggZD0iTSA5IDQgQyA3LjM0NiA0IDYgNS4zNDYgNiA3IEMgNiA4LjMwMTYwOTQgNi44Mzg3NDg2IDkuNDAyMTM5MSA4IDkuODE2NDA2MiBMIDggMTEuMzA0Njg4IEwgOCAyMy4yMDcwMzEgTCA4IDI3LjAyMzQzOCBDIDggMjcuNTYzNDM4IDguNDM2NTYyNSAyOCA4Ljk3NjU2MjUgMjggTCA5LjAyMzQzNzUgMjggQyA5LjU2MzQzNzUgMjggMTAgMjcuNTYzNDM3IDEwIDI3LjAyMzQzOCBMIDEwIDIyLjIyODUxNiBDIDEwLjMzNDcwNyAyMS44Mzk3NTYgMTEuMTM4NDIzIDIxLjA0Njg3NSAxMy40NDUzMTIgMjEuMDQ2ODc1IEMgMTQuNjY5MzEzIDIxLjA0Njg3NSAxNS42NzA0MjIgMjEuNDczNzgxIDE2LjczMjQyMiAyMS45MjU3ODEgQyAxNy43Njk0MjIgMjIuMzY3NzgxIDE4Ljg0MTg5MSAyMi44MjQyMTkgMjAuMDg3ODkxIDIyLjgyNDIxOSBDIDIyLjQ0Njg5MSAyMi44MjQyMTkgMjQuMDQ5Mzc1IDIxLjU4NDY4OCAyNC43MzQzNzUgMjEuMDU0Njg4IEwgMjQuODg2NzE5IDIwLjkzOTQ1MyBDIDI1LjQzNzcxOSAyMC41NDA0NTMgMjYgMTkuOTk2IDI2IDE5IEwgMjYgMTAuNjc1NzgxIEMgMjYgOS43Njc3ODEyIDI1LjIyMTgyOCA5IDI0LjI5ODgyOCA5IEMgMjMuODAzODI4IDkgMjMuNDQwNDA2IDkuMjg2NTkzNyAyMi45NDE0MDYgOS42ODM1OTM4IEMgMjIuMjc5NDA2IDEwLjIwNzU5NCAyMS4yODA4OTEgMTEgMjAuMDg3ODkxIDExIEMgMTkuMjcyODkxIDExIDE4LjQ3NzY4OCAxMC42MTk3MzQgMTcuNTU0Njg4IDEwLjE3NzczNCBDIDE2LjQwMzY4NyA5LjYyNTczNDQgMTUuMDk4MzU5IDkgMTMuNDQzMzU5IDkgQyAxMi4zMDgyNTcgOSAxMS40MjE2ODcgOS4xODgzMzkzIDEwLjcxMjg5MSA5LjQ1NzAzMTIgQyAxMS40ODkwNzEgOC45MTQxODI0IDEyIDguMDE2NzgwMiAxMiA3IEMgMTIgNS4zNDYgMTAuNjU0IDQgOSA0IHogTSA5IDYgQyA5LjU1MiA2IDEwIDYuNDQ5IDEwIDcgQyAxMCA3LjU1MSA5LjU1MiA4IDkgOCBDIDguNDQ4IDggOCA3LjU1MSA4IDcgQyA4IDYuNDQ5IDguNDQ4IDYgOSA2IHogTSAxMy40NDMzNTkgMTEgQyAxNC42NDUzNTkgMTEgMTUuNjM4NDA2IDExLjQ3NjQ2OSAxNi42OTE0MDYgMTEuOTgwNDY5IEMgMTcuNzM2NDA2IDEyLjQ4MjQ2OSAxOC44MTc4OTEgMTMgMjAuMDg3ODkxIDEzIEMgMjEuODQyODkxIDEzIDIzLjE1ODA0NyAxMi4wNTQ0ODQgMjMuOTk4MDQ3IDExLjM5NjQ4NCBMIDIzLjk5ODA0NyAxOS4wNjY0MDYgQyAyMy45OTcwNDcgMTkuMDcwNDA2IDIzLjk1Mjk4NCAxOS4xNDUyNjYgMjMuNzA4OTg0IDE5LjMyMjI2NiBMIDIzLjUwOTc2NiAxOS40NzQ2MDkgQyAyMi45NDI3NjYgMTkuOTEyNjA5IDIxLjc2Mjg5MSAyMC44MjQyMTkgMjAuMDg3ODkxIDIwLjgyNDIxOSBDIDE5LjI0OTg5MSAyMC44MjQyMTkgMTguNDQ2NjI1IDIwLjQ4MjkzNyAxNy41MTU2MjUgMjAuMDg1OTM4IEMgMTYuMzcyNjI1IDE5LjU5NzkzOCAxNS4wNzYzNTkgMTkuMDQ0OTIyIDEzLjQ0MzM1OSAxOS4wNDQ5MjIgQyAxMS44OTEzNTkgMTkuMDQ0OTIyIDEwLjc4NiAxOS4zNTggMTAgMTkuNzUgTCAxMCAxMi4zNjEzMjggQyAxMC4zNDUgMTEuOTA1MzI4IDExLjEzMjM1OSAxMSAxMy40NDMzNTkgMTEgeiIvPjwvc3ZnPg==",
+    Fh = "data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAzMiAzMiI+PHBhdGggZD0iTSAxMSA1IEwgMTEgMTEgTCA1IDExIEwgNSAxMyBMIDExIDEzIEwgMTEgMTkgTCA1IDE5IEwgNSAyMSBMIDExIDIxIEwgMTEgMjcgTCAxMyAyNyBMIDEzIDIxIEwgMTkgMjEgTCAxOSAyNyBMIDIxIDI3IEwgMjEgMjEgTCAyNyAyMSBMIDI3IDE5IEwgMjEgMTkgTCAyMSAxMyBMIDI3IDEzIEwgMjcgMTEgTCAyMSAxMSBMIDIxIDUgTCAxOSA1IEwgMTkgMTEgTCAxMyAxMSBMIDEzIDUgWiBNIDEzIDEzIEwgMTkgMTMgTCAxOSAxOSBMIDEzIDE5IFoiLz48L3N2Zz4=",
+    Ph = "data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAzMiAzMiI+PHBhdGggZD0iTSA5IDQgQyA3LjM0NiA0IDYgNS4zNDYgNiA3IEMgNiA4LjMwMTYwOTQgNi44Mzg3NDg2IDkuNDAyMTM5MSA4IDkuODE2NDA2MiBMIDggMTEuMzA0Njg4IEwgOCAyMy4yMDcwMzEgTCA4IDI3LjAyMzQzOCBDIDggMjcuNTYzNDM4IDguNDM2NTYyNSAyOCA4Ljk3NjU2MjUgMjggTCA5LjAyMzQzNzUgMjggQyA5LjU2MzQzNzUgMjggMTAgMjcuNTYzNDM3IDEwIDI3LjAyMzQzOCBMIDEwIDIyLjIyODUxNiBDIDEwLjMzNDcwNyAyMS44Mzk3NTYgMTEuMTM4NDIzIDIxLjA0Njg3NSAxMy40NDUzMTIgMjEuMDQ2ODc1IEMgMTQuNjY5MzEzIDIxLjA0Njg3NSAxNS42NzA0MjIgMjEuNDczNzgxIDE2LjczMjQyMiAyMS45MjU3ODEgQyAxNy43Njk0MjIgMjIuMzY3NzgxIDE4Ljg0MTg5MSAyMi44MjQyMTkgMjAuMDg3ODkxIDIyLjgyNDIxOSBDIDIyLjQ0Njg5MSAyMi44MjQyMTkgMjQuMDQ5Mzc1IDIxLjU4NDY4OCAyNC43MzQzNzUgMjEuMDU0Njg4IEwgMjQuODg2NzE5IDIwLjkzOTQ1MyBDIDI1LjQzNzcxOSAyMC41NDA0NTMgMjYgMTkuOTk2IDI2IDE5IEwgMjYgMTAuNjc1NzgxIEMgMjYgOS43Njc3ODEyIDI1LjIyMTgyOCA5IDI0LjI5ODgyOCA5IEMgMjMuODAzODI4IDkgMjMuNDQwNDA2IDkuMjg2NTkzNyAyMi45NDE0MDYgOS42ODM1OTM4IEMgMjIuMjc5NDA2IDEwLjIwNzU5NCAyMS4yODA4OTEgMTEgMjAuMDg3ODkxIDExIEMgMTkuMjcyODkxIDExIDE4LjQ3NzY4OCAxMC42MTk3MzQgMTcuNTU0Njg4IDEwLjE3NzczNCBDIDE2LjQwMzY4NyA5LjYyNTczNDQgMTUuMDk4MzU5IDkgMTMuNDQzMzU5IDkgQyAxMi4zMDgyNTcgOSAxMS40MjE2ODcgOS4xODgzMzkzIDEwLjcxMjg5MSA5LjQ1NzAzMTIgQyAxMS40ODkwNzEgOC45MTQxODI0IDEyIDguMDE2NzgwMiAxMiA3IEMgMTIgNS4zNDYgMTAuNjU0IDQgOSA0IHogTSA5IDYgQyA5LjU1MiA2IDEwIDYuNDQ5IDEwIDcgQyAxMCA3LjU1MSA5LjU1MiA4IDkgOCBDIDguNDQ4IDggOCA3LjU1MSA4IDcgQyA4IDYuNDQ5IDguNDQ4IDYgOSA2IHogTSAxMy40NDMzNTkgMTEgQyAxNC42NDUzNTkgMTEgMTUuNjM4NDA2IDExLjQ3NjQ2OSAxNi42OTE0MDYgMTEuOTgwNDY5IEMgMTcuNzM2NDA2IDEyLjQ4MjQ2OSAxOC44MTc4OTEgMTMgMjAuMDg3ODkxIDEzIEMgMjEuODQyODkxIDEzIDIzLjE1ODA0NyAxMi4wNTQ0ODQgMjMuOTk4MDQ3IDExLjM5NjQ4NCBMIDIzLjk5ODA0NyAxOS4wNjY0MDYgQyAyMy45OTcwNDcgMTkuMDcwNDA2IDIzLjk1Mjk4NCAxOS4xNDUyNjYgMjMuNzA4OTg0IDE5LjMyMjI2NiBMIDIzLjUwOTc2NiAxOS40NzQ2MDkgQyAyMi45NDI3NjYgMTkuOTEyNjA5IDIxLjc2Mjg5MSAyMC44MjQyMTkgMjAuMDg3ODkxIDIwLjgyNDIxOSBDIDE5LjI0OTg5MSAyMC44MjQyMTkgMTguNDQ2NjI1IDIwLjQ4MjkzNyAxNy41MTU2MjUgMjAuMDg1OTM4IEMgMTYuMzcyNjI1IDE5LjU5NzkzOCAxNS4wNzYzNTkgMTkuMDQ0OTIyIDEzLjQ0MzM1OSAxOS4wNDQ5MjIgQyAxMS44OTEzNTkgMTkuMDQ0OTIyIDEwLjc4NiAxOS4zNTggMTAgMTkuNzUgTCAxMCAxMi4zNjEzMjggQyAxMC4zNDUgMTEuOTA1MzI4IDExLjEzMjM1OSAxMSAxMy40NDMzNTkgMTEgeiIvPjwvc3ZnPg==",
     $h = "data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAzMiAzMiI+PHBhdGggZD0iTSAxNiA0IEMgMTEuODMyMDMxIDQgOC4xNTIzNDQgNi4xMTMyODEgNiA5LjM0Mzc1IEwgNiA2IEwgNCA2IEwgNCAxMyBMIDExIDEzIEwgMTEgMTEgTCA3LjM3NSAxMSBDIDkuMTAxNTYzIDguMDE5NTMxIDEyLjI5Njg3NSA2IDE2IDYgQyAyMS41MzUxNTYgNiAyNiAxMC40NjQ4NDQgMjYgMTYgQyAyNiAyMS41MzUxNTYgMjEuNTM1MTU2IDI2IDE2IDI2IEMgMTAuNDY0ODQ0IDI2IDYgMjEuNTM1MTU2IDYgMTYgTCA0IDE2IEMgNCAyMi42MTcxODggOS4zODI4MTMgMjggMTYgMjggQyAyMi42MTcxODggMjggMjggMjIuNjE3MTg4IDI4IDE2IEMgMjggOS4zODI4MTMgMjIuNjE3MTg4IDQgMTYgNCBaIE0gMTUgOCBMIDE1IDE3IEwgMjIgMTcgTCAyMiAxNSBMIDE3IDE1IEwgMTcgOCBaIi8+PC9zdmc+Cg==";
 const Qh = Ce({
         name: "Header",
         setup(e) {
             const {
                 state: t,
                 updateSearch: n,
@@ -13109,16 +13111,16 @@
                 icons: No(ut({
                     smileys_people: uc,
                     animals_nature: Oh,
                     food_drink: Lh,
                     activities: Uh,
                     travel_places: Jh,
                     objects: Kh,
-                    symbols: Ph,
-                    flags: Fh
+                    symbols: Fh,
+                    flags: Ph
                 }, t.options.groupIcons), {
                     recent: $h
                 })
             }
         }
     }),
     qh = {
@@ -13146,21 +13148,21 @@
     return e.hasGroupIcons || e.hasSearch ? (j(), U("div", qh, [e.hasGroupIcons ? (j(), U("div", eb, [(j(!0), U(_e, null, Cn(e.orderedGroups, f => (j(), U("button", {
         key: f.key,
         type: "button",
         class: L(["v3-group", {
             "v3-is-hidden": !e.icons[f.key]
         }]),
         onClick: r => e.updateActiveGroup(f.key)
-    }, [F("span", {
+    }, [P("span", {
         title: f.title,
         class: "v3-icon"
-    }, [F("img", {
+    }, [P("img", {
         src: e.icons[f.key],
         alt: ""
-    }, null, 8, ob)], 8, nb)], 10, tb))), 128))])) : me("", !0), e.hasGroupIcons && e.hasSearch ? (j(), U("div", sb)) : me("", !0), e.hasSearch ? (j(), U("div", ib, [bn(F("input", {
+    }, null, 8, ob)], 8, nb)], 10, tb))), 128))])) : me("", !0), e.hasGroupIcons && e.hasSearch ? (j(), U("div", sb)) : me("", !0), e.hasSearch ? (j(), U("div", ib, [bn(P("input", {
         "onUpdate:modelValue": t[0] || (t[0] = f => e.searchValue = f),
         type: "text",
         placeholder: e.placeholder
     }, null, 8, fb), [
         [mg, e.searchValue]
     ])])) : me("", !0)])) : me("", !0)
 }
@@ -13199,15 +13201,15 @@
                 selectSkinTone: u,
                 toggleSkinToneState: c,
                 EMOJI_RESULT_KEY: Io,
                 EMOJI_NAME_KEY: Vs,
                 skinToneText: i,
                 hasSkinTones: f,
                 native: e.options.native,
-                unicodeToEmoji: Po,
+                unicodeToEmoji: Fo,
                 platform: r,
                 hasError: o
             }
         }
     }),
     cb = {
         class: "v3-foot-left"
@@ -13224,30 +13226,30 @@
     },
     mb = ["onClick"];
 
 function Ib(e, t, n, o, s, i) {
     return j(), U("div", {
         class: "v3-footer",
         onMouseleave: t[2] || (t[2] = f => e.updateSkinToneState(!1))
-    }, [F("div", cb, [F("span", {
+    }, [P("div", cb, [P("span", {
         class: L([e.platform, "v3-icon"])
-    }, [e.native || e.hasError ? (j(), U("span", ub, Te(e.unicodeToEmoji(e.emoji.r)), 1)) : (j(), U("img", {
+    }, [e.native || e.hasError ? (j(), U("span", ub, Ge(e.unicodeToEmoji(e.emoji.r)), 1)) : (j(), U("img", {
         key: 1,
         alt: e.unicodeToEmoji(e.emoji.r),
         src: e.emoji.src,
         onError: t[0] || (t[0] = f => e.hasError = !0)
-    }, null, 40, db))], 2), F("span", gb, " :" + Te(e.emoji[e.EMOJI_NAME_KEY][1] || e.emoji[e.EMOJI_NAME_KEY][0]) + ": ", 1)]), e.hasSkinTones ? (j(), U(_e, {
+    }, null, 40, db))], 2), P("span", gb, " :" + Ge(e.emoji[e.EMOJI_NAME_KEY][1] || e.emoji[e.EMOJI_NAME_KEY][0]) + ": ", 1)]), e.hasSkinTones ? (j(), U(_e, {
         key: 0
-    }, [F("button", {
+    }, [P("button", {
         type: "button",
         class: "v3-tone",
         onClick: t[1] || (t[1] = (...f) => e.toggleSkinToneState && e.toggleSkinToneState(...f))
-    }, [F("span", pb, Te(e.skinToneText), 1), F("span", {
+    }, [P("span", pb, Ge(e.skinToneText), 1), P("span", {
         class: L(`v3-icon v3-tone-${e.stateSkinTone}`)
-    }, null, 2)]), F("div", {
+    }, null, 2)]), P("div", {
         class: L([e.skinTone ? "v3-is-open" : "", "v3-skin-tones"])
     }, [(j(!0), U(_e, null, Cn(e.SKIN_TONES, f => (j(), U("button", {
         key: f,
         type: "button",
         class: L(["v3-skin-tone-" + f, "v3-skin-tone"]),
         onClick: r => e.selectSkinTone(f)
     }, null, 10, mb))), 128))], 2)], 64)) : me("", !0)], 32)
@@ -13369,40 +13371,40 @@
     vb = ["value"],
     wb = ["src"];
 
 function _b(e, t, n, o, s, i) {
     const f = tt("Header"),
         r = tt("Body"),
         a = tt("Footer");
-    return e.isInputType ? (j(), U("div", Cb, [F("div", yb, [e.type === "input" ? (j(), U("input", {
+    return e.isInputType ? (j(), U("div", Cb, [P("div", yb, [e.type === "input" ? (j(), U("input", {
         key: 0,
         ref: "elem",
         value: e.input,
         type: "text",
         class: "v3-emoji-picker-input",
         onInput: t[0] || (t[0] = (...l) => e.onChangeText && e.onChangeText(...l)),
         onBlur: t[1] || (t[1] = (...l) => e.updateCursor && e.updateCursor(...l))
     }, null, 40, Ab)) : (j(), U("textarea", {
         key: 1,
         ref: "elem",
         value: e.input,
         class: "v3-emoji-picker-textarea",
         onInput: t[2] || (t[2] = (...l) => e.onChangeText && e.onChangeText(...l)),
         onBlur: t[3] || (t[3] = (...l) => e.updateCursor && e.updateCursor(...l))
-    }, null, 40, vb)), F("div", {
+    }, null, 40, vb)), P("div", {
         class: L(["v3-input-picker-wrap", e.open ? "v3-picker-is-open" : ""])
-    }, [F("button", {
+    }, [P("button", {
         ref: "button",
         type: "button",
         class: "v3-input-picker-icon",
         onClick: t[4] || (t[4] = l => e.open = !e.open)
-    }, [F("img", {
+    }, [P("img", {
         src: e.face,
         alt: ""
-    }, null, 8, wb)], 512), F("div", {
+    }, null, 8, wb)], 512), P("div", {
         ref: "picker",
         class: L(["v3-emoji-picker", "v3-color-theme-" + e.colorTheme])
     }, [se(f), se(r, {
         onSelect: e.onSelect
     }, null, 8, ["onSelect"]), se(a)], 2)], 2)])])) : (j(), U("div", {
         key: 1,
         class: L(["v3-emoji-picker", "v3-color-theme-" + e.colorTheme])
@@ -13562,15 +13564,15 @@
                 };
             return t({
                 closeEmoji: i
             }), (r, a) => {
                 const l = vs("click-outside");
                 return bn((j(), U("div", {
                     class: L(r.$style["ops-emoji-picker"])
-                }, [se(Fl, {
+                }, [se(Pl, {
                     "prefix-icon": "emoji",
                     class: L(["ml-2", r.$style["ops-room-footer__action"]]),
                     onClick: s
                 }, null, 8, ["class"]), se(Ao, {
                     name: "ops-slide-left"
                 }, {
                     default: Ne(() => [o.value ? (j(), Me(ae(Wb), {
@@ -13585,27 +13587,27 @@
                 ])
             }
         }
     }),
     Bb = "_ops-emoji-picker_ezhbu_1",
     zb = "_ops-emoji-picker__component_ezhbu_4",
     Vb = "_ops-room-footer__action_ezhbu_8",
-    Tb = {
+    Gb = {
         "ops-emoji-picker": "_ops-emoji-picker_ezhbu_1",
         opsEmojiPicker: Bb,
         "ops-emoji-picker__component": "_ops-emoji-picker__component_ezhbu_4",
         opsEmojiPickerComponent: zb,
         "ops-room-footer__action": "_ops-room-footer__action_ezhbu_8",
         opsRoomFooterAction: Vb
     },
-    Gb = {
-        $style: Tb
+    Tb = {
+        $style: Gb
     },
     jb = Ye(Sb, [
-        ["__cssModules", Gb]
+        ["__cssModules", Tb]
     ]),
     kb = Ce({
         __name: "RoomFooter",
         props: {
             room: {
                 type: Object,
                 default: () => ({})
@@ -13655,21 +13657,21 @@
                 modelValue: o.value,
                 "onUpdate:modelValue": u[0] || (u[0] = d => o.value = d),
                 class: "!py-2",
                 placeholder: "Type...",
                 onKeydown: yl(f, ["enter"]),
                 onInput: a,
                 onBlur: l
-            }, null, 8, ["modelValue", "onKeydown"]), F("div", {
+            }, null, 8, ["modelValue", "onKeydown"]), P("div", {
                 class: L(c.$style["ops-room-footer__action-end"])
             }, [se(jb, {
                 ref_key: "emojiPicker",
                 ref: n,
                 onSelectEmoji: i
-            }, null, 512), me("", !0), se(Fl, {
+            }, null, 512), me("", !0), se(Pl, {
                 "prefix-icon": "send",
                 class: L(["ml-2", c.$style["ops-room-footer__action"]]),
                 onClick: f
             }, null, 8, ["class"])], 2)], 2))
         }
     }),
     Db = "_ops-room-footer_1iulz_1",
@@ -13698,20 +13700,20 @@
     if (n > 0) {
         var o = e.indexOf("rv:");
         return parseInt(e.substring(o + 3, e.indexOf(".", o)), 10)
     }
     var s = e.indexOf("Edge/");
     return s > 0 ? parseInt(e.substring(s + 5, e.indexOf(".", s)), 10) : -1
 }
-let Fo;
+let Po;
 
 function Vi() {
-    Vi.init || (Vi.init = !0, Fo = Hb() !== -1)
+    Vi.init || (Vi.init = !0, Po = Hb() !== -1)
 }
-var Gs = {
+var Ts = {
     name: "ResizeObserver",
     props: {
         emitOnMount: {
             type: Boolean,
             default: !1
         },
         ignoreWidth: {
@@ -13725,15 +13727,15 @@
     },
     emits: ["notify"],
     mounted() {
         Vi(), Hn(() => {
             this._w = this.$el.offsetWidth, this._h = this.$el.offsetHeight, this.emitOnMount && this.emitSize()
         });
         const e = document.createElement("object");
-        this._resizeObject = e, e.setAttribute("aria-hidden", "true"), e.setAttribute("tabindex", -1), e.onload = this.addResizeHandlers, e.type = "text/html", Fo && this.$el.appendChild(e), e.data = "about:blank", Fo || this.$el.appendChild(e)
+        this._resizeObject = e, e.setAttribute("aria-hidden", "true"), e.setAttribute("tabindex", -1), e.onload = this.addResizeHandlers, e.type = "text/html", Po && this.$el.appendChild(e), e.data = "about:blank", Po || this.$el.appendChild(e)
     },
     beforeUnmount() {
         this.removeResizeHandlers()
     },
     methods: {
         compareAndNotify() {
             (!this.ignoreWidth && this._w !== this.$el.offsetWidth || !this.ignoreHeight && this._h !== this.$el.offsetHeight) && (this._w = this.$el.offsetWidth, this._h = this.$el.offsetHeight, this.emitSize())
@@ -13744,75 +13746,75 @@
                 height: this._h
             })
         },
         addResizeHandlers() {
             this._resizeObject.contentDocument.defaultView.addEventListener("resize", this.compareAndNotify), this.compareAndNotify()
         },
         removeResizeHandlers() {
-            this._resizeObject && this._resizeObject.onload && (!Fo && this._resizeObject.contentDocument && this._resizeObject.contentDocument.defaultView.removeEventListener("resize", this.compareAndNotify), this.$el.removeChild(this._resizeObject), this._resizeObject.onload = null, this._resizeObject = null)
+            this._resizeObject && this._resizeObject.onload && (!Po && this._resizeObject.contentDocument && this._resizeObject.contentDocument.defaultView.removeEventListener("resize", this.compareAndNotify), this.$el.removeChild(this._resizeObject), this._resizeObject.onload = null, this._resizeObject = null)
         }
     }
 };
-const Ob = Fa();
+const Ob = Pa();
 Ka("data-v-b329ee4c");
 const Lb = {
     class: "resize-observer",
     tabindex: "-1"
 };
-Pa();
+Fa();
 const Ub = Ob((e, t, n, o, s, i) => (j(), Me("div", Lb)));
-Gs.render = Ub;
-Gs.__scopeId = "data-v-b329ee4c";
-Gs.__file = "src/components/ResizeObserver.vue";
+Ts.render = Ub;
+Ts.__scopeId = "data-v-b329ee4c";
+Ts.__file = "src/components/ResizeObserver.vue";
 
 function $o(e) {
     return typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? $o = function(t) {
         return typeof t
     } : $o = function(t) {
         return t && typeof Symbol == "function" && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
     }, $o(e)
 }
 
 function Jb(e, t) {
     if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
 }
 
-function Fr(e, t) {
+function Pr(e, t) {
     for (var n = 0; n < t.length; n++) {
         var o = t[n];
         o.enumerable = o.enumerable || !1, o.configurable = !0, "value" in o && (o.writable = !0), Object.defineProperty(e, o.key, o)
     }
 }
 
 function Kb(e, t, n) {
-    return t && Fr(e.prototype, t), n && Fr(e, n), e
+    return t && Pr(e.prototype, t), n && Pr(e, n), e
 }
 
 function $r(e) {
-    return Pb(e) || Fb(e) || $b(e) || Qb()
+    return Fb(e) || Pb(e) || $b(e) || Qb()
 }
 
-function Pb(e) {
-    if (Array.isArray(e)) return Ti(e)
+function Fb(e) {
+    if (Array.isArray(e)) return Gi(e)
 }
 
-function Fb(e) {
+function Pb(e) {
     if (typeof Symbol < "u" && Symbol.iterator in Object(e)) return Array.from(e)
 }
 
 function $b(e, t) {
     if (e) {
-        if (typeof e == "string") return Ti(e, t);
+        if (typeof e == "string") return Gi(e, t);
         var n = Object.prototype.toString.call(e).slice(8, -1);
         if (n === "Object" && e.constructor && (n = e.constructor.name), n === "Map" || n === "Set") return Array.from(e);
-        if (n === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return Ti(e, t)
+        if (n === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n)) return Gi(e, t)
     }
 }
 
-function Ti(e, t) {
+function Gi(e, t) {
     (t == null || t > e.length) && (t = e.length);
     for (var n = 0, o = new Array(t); n < t; n++) o[n] = e[n];
     return o
 }
 
 function Qb() {
     throw new TypeError(`Invalid attempt to spread non-iterable instance.
@@ -13979,20 +13981,20 @@
     if (e instanceof HTMLElement || e instanceof SVGElement) {
         for (var t = hc(e.parentNode, []), n = 0; n < t.length; n += 1)
             if (a2(t[n])) return t[n];
         return document.scrollingElement || document.documentElement
     }
 }
 
-function Gi(e) {
-    return Gi = typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? function(t) {
+function Ti(e) {
+    return Ti = typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? function(t) {
         return typeof t
     } : function(t) {
         return t && typeof Symbol == "function" && t.constructor === Symbol && t !== Symbol.prototype ? "symbol" : typeof t
-    }, Gi(e)
+    }, Ti(e)
 }
 var bc = {
     items: {
         type: Array,
         required: !0
     },
     keyField: {
@@ -14013,15 +14015,15 @@
     itemTag: {
         type: String,
         default: "div"
     }
 };
 
 function Cc() {
-    return this.items.length && Gi(this.items[0]) !== "object"
+    return this.items.length && Ti(this.items[0]) !== "object"
 }
 var ji = !1;
 if (typeof window < "u") {
     ji = !1;
     try {
         var l2 = Object.defineProperty({}, "passive", {
             get: function() {
@@ -14031,15 +14033,15 @@
         window.addEventListener("test", null, l2)
     } catch {}
 }
 let c2 = 0;
 var Vf = {
     name: "RecycleScroller",
     components: {
-        ResizeObserver: Gs
+        ResizeObserver: Ts
     },
     directives: {
         ObserveVisibility: o2
     },
     props: {
         ...bc,
         itemSize: {
@@ -14240,46 +14242,46 @@
                 a = this.items,
                 l = a.length,
                 c = this.sizes,
                 u = this.$_views,
                 d = this.$_unusedViews,
                 m = this.pool,
                 p = this.itemIndexByKey;
-            let h, b, y, G, N;
-            if (!l) h = b = G = N = y = 0;
-            else if (this.$_prerender) h = G = 0, b = N = Math.min(this.prerender, a.length), y = null;
+            let h, b, y, T, N;
+            if (!l) h = b = T = N = y = 0;
+            else if (this.$_prerender) h = T = 0, b = N = Math.min(this.prerender, a.length), y = null;
             else {
                 const A = this.getScroll();
                 if (t) {
                     let z = A.start - this.$_lastUpdateScrollPosition;
                     if (z < 0 && (z = -z), n === null && z < i || z < n) return {
                         continuous: !0
                     }
                 }
                 this.$_lastUpdateScrollPosition = A.start;
                 const K = this.buffer;
                 A.start -= K, A.end += K;
-                let T = 0;
-                if (this.$refs.before && (T = this.$refs.before.scrollHeight, A.start -= T), this.$refs.after) {
+                let G = 0;
+                if (this.$refs.before && (G = this.$refs.before.scrollHeight, A.start -= G), this.$refs.after) {
                     const z = this.$refs.after.scrollHeight;
                     A.end += z
                 }
                 if (n === null) {
                     let z, M = 0,
                         S = l - 1,
                         k = ~~(l / 2),
                         Z;
                     do Z = k, z = c[k].accumulator, z < A.start ? M = k : k < l - 1 && c[k + 1].accumulator > A.start && (S = k), k = ~~((M + S) / 2); while (k !== Z);
                     for (k < 0 && (k = 0), h = k, y = c[l - 1].accumulator, b = k; b < l && c[b].accumulator < A.end; b++);
-                    for (b === -1 ? b = a.length - 1 : (b++, b > l && (b = l)), G = h; G < l && T + c[G].accumulator < A.start; G++);
-                    for (N = G; N < l && T + c[N].accumulator < A.end; N++);
+                    for (b === -1 ? b = a.length - 1 : (b++, b > l && (b = l)), T = h; T < l && G + c[T].accumulator < A.start; T++);
+                    for (N = T; N < l && G + c[N].accumulator < A.end; N++);
                 } else {
                     h = ~~(A.start / n * o);
                     const z = h % o;
-                    h -= z, b = Math.ceil(A.end / n * o), G = Math.max(0, Math.floor((A.start - T) / n * o)), N = Math.floor((A.end - T) / n * o), h < 0 && (h = 0), b > l && (b = l), G < 0 && (G = 0), N > l && (N = l), y = Math.ceil(l / o) * n
+                    h -= z, b = Math.ceil(A.end / n * o), T = Math.max(0, Math.floor((A.start - G) / n * o)), N = Math.floor((A.end - G) / n * o), h < 0 && (h = 0), b > l && (b = l), T < 0 && (T = 0), N > l && (N = l), y = Math.ceil(l / o) * n
                 }
             }
             b - h > i2.itemsLimit && this.itemsLimitError(), this.totalSize = y;
             let v;
             const E = h <= this.$_endIndex && b >= this.$_startIndex;
             if (E)
                 for (let A = 0, K = m.length; A < K; A++) v = m[A], v.nr.used && (e && (v.nr.index = p[v.item[r]]), (v.nr.index == null || v.nr.index < h || v.nr.index >= b) && this.unuseView(v));
@@ -14290,24 +14292,24 @@
                 const K = r ? Y[r] : Y;
                 if (K == null) throw new Error(`Key is ${K} on item (keyField is '${r}')`);
                 if (v = u.get(K), !n && !c[A].size) {
                     v && this.unuseView(v);
                     continue
                 }
                 _ = Y[f];
-                let T = d.get(_),
+                let G = d.get(_),
                     z = !1;
-                if (!v) E ? T && T.length ? v = T.pop() : v = this.addView(m, A, Y, K, _) : (R = J.get(_) || 0, (!T || R >= T.length) && (v = this.addView(m, A, Y, K, _), this.unuseView(v, !0), T = d.get(_)), v = T[R], J.set(_, R + 1)), u.delete(v.nr.key), v.nr.used = !0, v.nr.index = A, v.nr.key = K, v.nr.type = _, u.set(K, v), z = !0;
-                else if (!v.nr.used && (v.nr.used = !0, z = !0, T)) {
-                    const M = T.indexOf(v);
-                    M !== -1 && T.splice(M, 1)
+                if (!v) E ? G && G.length ? v = G.pop() : v = this.addView(m, A, Y, K, _) : (R = J.get(_) || 0, (!G || R >= G.length) && (v = this.addView(m, A, Y, K, _), this.unuseView(v, !0), G = d.get(_)), v = G[R], J.set(_, R + 1)), u.delete(v.nr.key), v.nr.used = !0, v.nr.index = A, v.nr.key = K, v.nr.type = _, u.set(K, v), z = !0;
+                else if (!v.nr.used && (v.nr.used = !0, z = !0, G)) {
+                    const M = G.indexOf(v);
+                    M !== -1 && G.splice(M, 1)
                 }
                 v.item = Y, z && (A === a.length - 1 && this.$emit("scroll-end"), A === 0 && this.$emit("scroll-start")), n === null ? (v.position = c[A - 1].accumulator, v.offset = 0) : (v.position = Math.floor(A / o) * n, v.offset = A % o * s)
             }
-            return this.$_startIndex = h, this.$_endIndex = b, this.emitUpdate && this.$emit("update", h, b, G, N), clearTimeout(this.$_sortTimer), this.$_sortTimer = setTimeout(this.sortViews, this.updateInterval + 300), {
+            return this.$_startIndex = h, this.$_endIndex = b, this.emitUpdate && this.$emit("update", h, b, T, N), clearTimeout(this.$_sortTimer), this.$_sortTimer = setTimeout(this.sortViews, this.updateInterval + 300), {
                 continuous: E
             }
         },
         getListenerTarget() {
             let e = Qr(this.$el);
             return window.document && (e === window.document.documentElement || e === window.document.body) && (e = window), e
         },
@@ -14437,15 +14439,15 @@
         onNotify: i.handleResize
     }, null, 8, ["onNotify"])], 34)), [
         [r, i.handleVisibilityChange]
     ])
 }
 Vf.render = g2;
 Vf.__file = "src/components/RecycleScroller.vue";
-var Tf = {
+var Gf = {
     name: "DynamicScroller",
     components: {
         RecycleScroller: Vf
     },
     provide() {
         return typeof ResizeObserver < "u" && (this.$_resizeObserver = new ResizeObserver(e => {
             requestAnimationFrame(() => {
@@ -14610,16 +14612,16 @@
         })))]),
         before: Ne(() => [Xe(e.$slots, "before")]),
         after: Ne(() => [Xe(e.$slots, "after")]),
         empty: Ne(() => [Xe(e.$slots, "empty")]),
         _: 3
     }, 16, ["items", "min-item-size", "direction", "list-tag", "item-tag", "onResize", "onVisible"])
 }
-Tf.render = p2;
-Tf.__file = "src/components/DynamicScroller.vue";
+Gf.render = p2;
+Gf.__file = "src/components/DynamicScroller.vue";
 var yc = {
     name: "DynamicScrollerItem",
     inject: ["vscrollData", "vscrollParent", "vscrollResizeObserver"],
     props: {
         item: {
             required: !0
         },
@@ -14747,15 +14749,15 @@
             }
         },
         setup(e) {
             return (t, n) => {
                 var o;
                 return j(), U("div", {
                     class: L(t.$style["ops-text-message"])
-                }, Te((o = e.messageData) == null ? void 0 : o.content), 3)
+                }, Ge((o = e.messageData) == null ? void 0 : o.content), 3)
             }
         }
     }),
     I2 = "_ops-text-message_4sur5_1",
     h2 = {
         "ops-text-message": "_ops-text-message_4sur5_1",
         opsTextMessage: I2
@@ -14786,15 +14788,15 @@
             const t = e,
                 n = ue(() => {
                     var o;
                     return Nn((o = t.messageData) == null ? void 0 : o.timestamp).format("HH:mm")
                 });
             return (o, s) => {
                 var i;
-                return j(), U("div", y2, [F("span", A2, Te(ae(n)), 1), (i = e.messageData) != null && i.is_read ? (j(), U("img", {
+                return j(), U("div", y2, [P("span", A2, Ge(ae(n)), 1), (i = e.messageData) != null && i.is_read ? (j(), U("img", {
                     key: 0,
                     class: "ops-message-time__read",
                     src: ae(Zt)("assets/icons/read-message.svg"),
                     alt: "read-message"
                 }, null, 8, v2)) : (j(), U("img", {
                     key: 1,
                     class: "ops-message-time__read",
@@ -14805,29 +14807,29 @@
         }
     });
 const N2 = ["id"],
     M2 = {
         key: 1,
         class: "ops-message-wrapper__new-message"
     },
-    Z2 = F("span", null, "New messages", -1),
+    Z2 = P("span", null, "New messages", -1),
     W2 = [Z2],
     S2 = {
         class: "ops-message-wrapper__box"
     },
     B2 = {
         class: "ops-message-wrapper__author"
     },
     z2 = {
         class: "group/message ops-message-wrapper__content"
     },
     V2 = {
         class: "ops-message-wrapper__message ops-message"
     },
-    T2 = Ce({
+    G2 = Ce({
         __name: "RoomMessageWrapper",
         props: {
             messages: {
                 type: Array,
                 default: () => []
             },
             messageData: {
@@ -14879,23 +14881,23 @@
                 var c, u;
                 const l = vs("click-outside");
                 return bn((j(), U("div", {
                     id: `message-${(c=e.messageData)==null?void 0:c.id}`,
                     class: L(["ops-message-wrapper", {
                         "own-message": ae(i)
                     }])
-                }, [me("", !0), e.isNewMessages && ((u = e.messageData) == null ? void 0 : u.author.id) !== ae(o).getUser.person.id ? (j(), U("div", M2, W2)) : me("", !0), F("div", S2, [F("div", B2, [F("span", null, Te(e.messageData.author.initials), 1)]), F("div", z2, [me("", !0), me("", !0), F("div", V2, [Xe(r.$slots, "default"), se(_2, {
+                }, [me("", !0), e.isNewMessages && ((u = e.messageData) == null ? void 0 : u.author.id) !== ae(o).getUser.person.id ? (j(), U("div", M2, W2)) : me("", !0), P("div", S2, [P("div", B2, [P("span", null, Ge(e.messageData.author.initials), 1)]), P("div", z2, [me("", !0), me("", !0), P("div", V2, [Xe(r.$slots, "default"), se(_2, {
                     "message-data": e.messageData
                 }, null, 8, ["message-data"])]), me("", !0)])])], 10, N2)), [
                     [l, f]
                 ])
             }
         }
     });
-const G2 = (e, t) => {
+const T2 = (e, t) => {
         const n = oe(!1),
             o = oe(2);
         return {
             loading: n,
             page: o,
             intersectionBlock: () => {
                 var c;
@@ -14932,17 +14934,17 @@
                 type: String,
                 default: ""
             }
         },
         setup(e) {
             return (t, n) => (j(), U("div", {
                 class: L(t.$style["rooms-empty"])
-            }, [F("p", {
+            }, [P("p", {
                 class: L(t.$style["rooms-empty__text"])
-            }, Te(e.text), 3)], 2))
+            }, Ge(e.text), 3)], 2))
         }
     }),
     k2 = "_rooms-empty_c4i6w_1",
     D2 = "_emptyRooms_c4i6w_1",
     R2 = "_rooms-empty__text_c4i6w_5",
     x2 = {
         "rooms-empty": "_rooms-empty_c4i6w_1",
@@ -14959,15 +14961,15 @@
     ]),
     Y2 = {
         id: "room-messages"
     },
     E2 = {
         key: 0
     },
-    H2 = F("div", {
+    H2 = P("div", {
         class: "intersection-block w-full h-2"
     }, null, -1),
     O2 = Ce({
         __name: "RoomContentScroller",
         props: {
             room: {
                 type: Object,
@@ -14982,30 +14984,30 @@
             var a;
             const t = e,
                 n = Ln(),
                 o = oe(),
                 {
                     loading: s,
                     intersectionBlock: i
-                } = G2((a = t.room) == null ? void 0 : a.id, ".intersection-block"),
+                } = T2((a = t.room) == null ? void 0 : a.id, ".intersection-block"),
                 f = ue(() => ie.unreadMessages.value[0]),
                 r = async (l, c, u, d) => {
                     var m, p, h;
                     !((m = t.messages[d - 1]) != null && m.is_read) && ((h = (p = t.messages[d - 1]) == null ? void 0 : p.author) == null ? void 0 : h.id) !== n.getUser.person.id && ie.sendMessage({
                         type: qe.READ_MESSAGES
                     })
                 };
             return $t(async () => {
                 var l;
                 await Hn(), (l = o.value) == null || l.scrollToBottom(), ie.hasMoreMessages.value && i()
             }), (l, c) => {
                 var u, d;
-                return j(), U("div", Y2, [(u = e.messages) != null && u.length ? (j(), U("div", E2, [ae(s) ? (j(), Me(Pl, {
+                return j(), U("div", Y2, [(u = e.messages) != null && u.length ? (j(), U("div", E2, [ae(s) ? (j(), Me(Fl, {
                     key: 0
-                })) : me("", !0), se(ae(Tf), {
+                })) : me("", !0), se(ae(Gf), {
                     ref_key: "scroller",
                     ref: o,
                     items: e.messages,
                     "min-item-size": 54,
                     class: L(l.$style.scroller),
                     "emit-update": !0,
                     buffer: 54,
@@ -15018,15 +15020,15 @@
                         active: h
                     }) => [se(ae(yc), {
                         item: m,
                         active: h,
                         "data-index": p,
                         "data-active": h
                     }, {
-                        default: Ne(() => [(j(), Me(T2, {
+                        default: Ne(() => [(j(), Me(G2, {
                             key: p,
                             "message-index": p,
                             "message-data": m,
                             messages: e.messages,
                             "is-new-messages": ae(f) === m.id,
                             room: e.room,
                             class: L(l.$style["room-message-wrapper"])
@@ -15053,15 +15055,15 @@
     };
 const J2 = {
         $style: U2
     },
     K2 = Ye(O2, [
         ["__cssModules", J2]
     ]),
-    P2 = Ce({
+    F2 = Ce({
         __name: "Room",
         props: {
             showRoomsList: {
                 type: Boolean,
                 default: !0
             },
             roomId: {
@@ -15083,44 +15085,44 @@
                 return ae(o) ? (j(), U("div", {
                     key: (f = ae(o)) == null ? void 0 : f.id,
                     class: L(s.$style["ops-room-chat"])
                 }, [se(Dm, {
                     "show-rooms-list": e.showRoomsList,
                     room: ae(o),
                     onToggleRoomsList: i[0] || (i[0] = r => s.$emit("toggleRoomsList"))
-                }, null, 8, ["show-rooms-list", "room"]), F("div", {
+                }, null, 8, ["show-rooms-list", "room"]), P("div", {
                     class: L(s.$style["ops-room-chat__box"])
                 }, [ae(o).id && !ae(n) ? (j(), Me(K2, {
                     key: 0,
                     messages: ae(ie).messages.value,
                     room: ae(o)
-                }, null, 8, ["messages", "room"])) : ae(n) ? (j(), Me(Pl, {
+                }, null, 8, ["messages", "room"])) : ae(n) ? (j(), Me(Fl, {
                     key: 1,
                     class: L(s.$style["ops-room-chat__loading"])
                 }, null, 8, ["class"])) : me("", !0)], 2), se(Eb, {
                     room: ae(o)
                 }, null, 8, ["room"])], 2)) : me("", !0)
             }
         }
     }),
-    F2 = "_ops-room-chat_1vais_1",
+    P2 = "_ops-room-chat_1vais_1",
     $2 = "_ops-room-chat__box_1vais_4",
     Q2 = "_ops-room-chat__loading_1vais_7",
     q2 = {
         "ops-room-chat": "_ops-room-chat_1vais_1",
-        opsRoomChat: F2,
+        opsRoomChat: P2,
         "ops-room-chat__box": "_ops-room-chat__box_1vais_4",
         opsRoomChatBox: $2,
         "ops-room-chat__loading": "_ops-room-chat__loading_1vais_7",
         opsRoomChatLoading: Q2
     },
     eC = {
         $style: q2
     },
-    tC = Ye(P2, [
+    tC = Ye(F2, [
         ["__cssModules", eC]
     ]),
     nC = ["src"],
     oC = Ce({
         __name: "RoomsContainer",
         setup(e) {
             const t = Af(),
@@ -15139,38 +15141,38 @@
                 };
             return $t(() => {
                 a()
             }), (l, c) => {
                 var u;
                 return j(), U("div", {
                     class: L(l.$style["ops-chat-container"])
-                }, [F("div", {
+                }, [P("div", {
                     class: L([l.$style["ops-rooms-wrapper"], {
                         [l.$style["ops-rooms-wrapper__show-rooms"]]: !o.value
                     }, {
                         [l.$style["show-block"]]: ae(s)
                     }])
-                }, [F("div", {
+                }, [P("div", {
                     class: L(l.$style["ops-rooms-wrapper__search-box"])
                 }, [se(vl, {
                     modelValue: n.value,
                     "onUpdate:modelValue": c[0] || (c[0] = d => n.value = d),
                     placeholder: "Search..."
                 }, {
-                    prefix: Ne(() => [F("img", {
+                    prefix: Ne(() => [P("img", {
                         class: L(l.$style["ops-rooms-wrapper__search-icon"]),
                         src: ae(Zt)("assets/icons/search.svg"),
                         alt: "search-icon"
                     }, null, 10, nC)]),
                     _: 1
                 }, 8, ["modelValue"]), me("", !0)], 2), ae(ie).rooms.value.length ? (j(), Me(Lp, {
                     key: 0,
                     rooms: ae(f),
                     "selected-room": ae(i)
-                }, null, 8, ["rooms", "selected-room"])) : me("", !0)], 2), F("div", {
+                }, null, 8, ["rooms", "selected-room"])) : me("", !0)], 2), P("div", {
                     class: L(l.$style["ops-chat-room"])
                 }, [(u = ae(i)) != null && u.id ? (j(), Me(tC, {
                     key: 0,
                     class: L({
                         [l.$style["show-block"]]: !ae(s)
                     }),
                     "show-rooms-list": o.value,
@@ -15260,15 +15262,15 @@
     return e.split("-")[1]
 }
 
 function So(e) {
     return ["top", "bottom"].includes(jt(e)) ? "x" : "y"
 }
 
-function Gf(e) {
+function Tf(e) {
     return e === "y" ? "height" : "width"
 }
 
 function qr(e) {
     let {
         reference: t,
         floating: n,
@@ -15305,15 +15307,15 @@
         default:
             f = {
                 x: t.x,
                 y: t.y
             }
     }
     const r = So(o),
-        a = Gf(r);
+        a = Tf(r);
     switch (Sn(o)) {
         case "start":
             f[r] = f[r] - (t[a] / 2 - n[a] / 2);
             break;
         case "end":
             f[r] = f[r] + (t[a] / 2 - n[a] / 2);
             break
@@ -15345,15 +15347,15 @@
         const {
             name: m,
             fn: p
         } = i[d], {
             x: h,
             y: b,
             data: y,
-            reset: G
+            reset: T
         } = await p({
             x: a,
             y: l,
             initialPlacement: o,
             placement: c,
             strategy: s,
             middlewareData: u,
@@ -15363,20 +15365,20 @@
                 reference: e,
                 floating: t
             }
         });
         if (a = h ?? a, l = b ?? l, u = {
                 ...u,
                 [m]: y ?? {}
-            }, G) {
-            typeof G == "object" && (G.placement && (c = G.placement), G.rects && (r = G.rects === !0 ? await f.getElementRects({
+            }, T) {
+            typeof T == "object" && (T.placement && (c = T.placement), T.rects && (r = T.rects === !0 ? await f.getElementRects({
                 reference: e,
                 floating: t,
                 strategy: s
-            }) : G.rects), {
+            }) : T.rects), {
                 x: a,
                 y: l
             } = qr({
                 ...r,
                 placement: c
             })), d = -1;
             continue
@@ -15482,27 +15484,27 @@
             const l = vc(o),
                 c = {
                     x: s,
                     y: i
                 },
                 u = jt(f),
                 d = So(u),
-                m = Gf(d),
+                m = Tf(d),
                 p = await a.getDimensions({
                     element: n
                 }),
                 h = d === "y" ? "top" : "left",
                 b = d === "y" ? "bottom" : "right",
                 y = r.reference[m] + r.reference[d] - c[d] - r.floating[m],
-                G = c[d] - r.reference[d],
+                T = c[d] - r.reference[d],
                 N = await a.getOffsetParent({
                     element: n
                 }),
                 v = N ? d === "y" ? N.clientHeight || 0 : N.clientWidth || 0 : 0,
-                E = y / 2 - G / 2,
+                E = y / 2 - T / 2,
                 J = l[h],
                 Y = v - p[m] - l[b],
                 _ = v / 2 - p[m] / 2 + E,
                 R = Di(J, _, Y);
             return {
                 data: {
                     [d]: R,
@@ -15521,15 +15523,15 @@
 function as(e) {
     return e.replace(/left|right|bottom|top/g, t => NC[t])
 }
 
 function wc(e, t) {
     const n = Sn(e) === "start",
         o = So(e),
-        s = Gf(o);
+        s = Tf(o);
     let i = o === "x" ? n ? "right" : "left" : n ? "bottom" : "top";
     return t.reference[s] > t.floating[s] && (i = as(i)), {
         main: i,
         cross: as(i)
     }
 }
 const MC = {
@@ -15562,48 +15564,48 @@
                 alignment: m = null,
                 allowedPlacements: p = WC,
                 autoAlignment: h = !0,
                 ...b
             } = e;
             if ((n = u.autoPlacement) != null && n.skip) return {};
             const y = SC(m, h, p),
-                G = await js(t, b),
+                T = await js(t, b),
                 N = (o = (s = u.autoPlacement) == null ? void 0 : s.index) != null ? o : 0,
                 v = y[N],
                 {
                     main: E,
                     cross: J
                 } = wc(v, c);
             if (d !== v) return {
                 x: a,
                 y: l,
                 reset: {
                     placement: y[0]
                 }
             };
-            const Y = [G[jt(v)], G[E], G[J]],
+            const Y = [T[jt(v)], T[E], T[J]],
                 _ = [...(i = (f = u.autoPlacement) == null ? void 0 : f.overflows) != null ? i : [], {
                     placement: v,
                     overflows: Y
                 }],
                 R = y[N + 1];
             if (R) return {
                 data: {
                     index: N + 1,
                     overflows: _
                 },
                 reset: {
                     placement: R
                 }
             };
-            const A = _.slice().sort((T, z) => T.overflows[0] - z.overflows[0]),
-                K = (r = A.find(T => {
+            const A = _.slice().sort((G, z) => G.overflows[0] - z.overflows[0]),
+                K = (r = A.find(G => {
                     let {
                         overflows: z
-                    } = T;
+                    } = G;
                     return z.every(M => M <= 0)
                 })) == null ? void 0 : r.placement;
             return {
                 data: {
                     skip: !0
                 },
                 reset: {
@@ -15634,22 +15636,22 @@
             const {
                 mainAxis: a = !0,
                 crossAxis: l = !0,
                 fallbackPlacements: c,
                 fallbackStrategy: u = "bestFit",
                 flipAlignment: d = !0,
                 ...m
-            } = e, p = jt(s), b = c || (p === r || !d ? [as(r)] : zC(r)), y = [r, ...b], G = await js(t, m), N = [];
+            } = e, p = jt(s), b = c || (p === r || !d ? [as(r)] : zC(r)), y = [r, ...b], T = await js(t, m), N = [];
             let v = ((o = i.flip) == null ? void 0 : o.overflows) || [];
-            if (a && N.push(G[p]), l) {
+            if (a && N.push(T[p]), l) {
                 const {
                     main: _,
                     cross: R
                 } = wc(s, f);
-                N.push(G[_], G[R])
+                N.push(T[_], T[R])
             }
             if (v = [...v, {
                     placement: s,
                     overflows: N
                 }], !N.every(_ => _ <= 0)) {
                 var E, J;
                 const _ = ((E = (J = i.flip) == null ? void 0 : J.index) != null ? E : 0) + 1,
@@ -15663,15 +15665,15 @@
                         placement: R
                     }
                 };
                 let A = "bottom";
                 switch (u) {
                     case "bestFit": {
                         var Y;
-                        const K = (Y = v.slice().sort((T, z) => T.overflows.filter(M => M > 0).reduce((M, S) => M + S, 0) - z.overflows.filter(M => M > 0).reduce((M, S) => M + S, 0))[0]) == null ? void 0 : Y.placement;
+                        const K = (Y = v.slice().sort((G, z) => G.overflows.filter(M => M > 0).reduce((M, S) => M + S, 0) - z.overflows.filter(M => M > 0).reduce((M, S) => M + S, 0))[0]) == null ? void 0 : Y.placement;
                         K && (A = K);
                         break
                     }
                     case "initialPlacement":
                         A = r;
                         break
                 }
@@ -15685,15 +15687,15 @@
                 }
             }
             return {}
         }
     }
 };
 
-function TC(e) {
+function GC(e) {
     let {
         placement: t,
         rects: n,
         value: o
     } = e;
     const s = jt(t),
         i = ["left", "top"].includes(s) ? -1 : 1,
@@ -15716,25 +15718,25 @@
         x: a,
         y: r * i
     } : {
         x: r * i,
         y: a
     }
 }
-const GC = function(e) {
+const TC = function(e) {
     return e === void 0 && (e = 0), {
         name: "offset",
         options: e,
         fn(t) {
             const {
                 x: n,
                 y: o,
                 placement: s,
                 rects: i
-            } = t, f = TC({
+            } = t, f = GC({
                 placement: s,
                 rects: i,
                 value: e
             });
             return {
                 x: n + f.x,
                 y: o + f.y,
@@ -15759,42 +15761,42 @@
                 } = t, {
                     mainAxis: i = !0,
                     crossAxis: f = !1,
                     limiter: r = {
                         fn: b => {
                             let {
                                 x: y,
-                                y: G
+                                y: T
                             } = b;
                             return {
                                 x: y,
-                                y: G
+                                y: T
                             }
                         }
                     },
                     ...a
                 } = e, l = {
                     x: n,
                     y: o
                 }, c = await js(t, a), u = So(jt(s)), d = jC(u);
                 let m = l[u],
                     p = l[d];
                 if (i) {
                     const b = u === "y" ? "top" : "left",
                         y = u === "y" ? "bottom" : "right",
-                        G = m + c[b],
+                        T = m + c[b],
                         N = m - c[y];
-                    m = Di(G, m, N)
+                    m = Di(T, m, N)
                 }
                 if (f) {
                     const b = d === "y" ? "top" : "left",
                         y = d === "y" ? "bottom" : "right",
-                        G = p + c[b],
+                        T = p + c[b],
                         N = p - c[y];
-                    p = Di(G, p, N)
+                    p = Di(T, p, N)
                 }
                 const h = r.fn({
                     ...t,
                     [u]: m,
                     [d]: p
                 });
                 return {
@@ -16117,29 +16119,29 @@
 
 function KC(e) {
     const t = us(xs(e)),
         o = ["absolute", "fixed"].includes(ks(e).position) && Vt(e) ? xi(e) : e;
     return ls(o) ? t.filter(s => ls(s) && UC(s, o) && zt(s) !== "body") : []
 }
 
-function PC(e) {
+function FC(e) {
     let {
         element: t,
         boundary: n,
         rootBoundary: o
     } = e;
     const i = [...n === "clippingParents" ? KC(t) : [].concat(n), o],
         f = i[0],
         r = i.reduce((a, l) => {
             const c = oa(t, l);
             return a.top = io(c.top, a.top), a.right = ea(c.right, a.right), a.bottom = ea(c.bottom, a.bottom), a.left = io(c.left, a.left), a
         }, oa(t, f));
     return r.width = r.right - r.left, r.height = r.bottom - r.top, r.x = r.left, r.y = r.top, r
 }
-const FC = {
+const PC = {
         getElementRects: e => {
             let {
                 reference: t,
                 floating: n,
                 strategy: o
             } = e;
             return {
@@ -16161,30 +16163,30 @@
         isElement: e => ls(e),
         getDocumentElement: e => {
             let {
                 element: t
             } = e;
             return en(t)
         },
-        getClippingClientRect: e => PC(e),
+        getClippingClientRect: e => FC(e),
         getDimensions: e => {
             let {
                 element: t
             } = e;
             return na(t)
         },
         getClientRects: e => {
             let {
                 element: t
             } = e;
             return t.getClientRects()
         }
     },
     $C = (e, t, n) => AC(e, t, {
-        platform: FC,
+        platform: PC,
         ...n
     });
 var QC = Object.defineProperty,
     qC = Object.defineProperties,
     ey = Object.getOwnPropertyDescriptors,
     sa = Object.getOwnPropertySymbols,
     ty = Object.prototype.hasOwnProperty,
@@ -16638,15 +16640,15 @@
         async $_computePosition() {
             var e;
             if (this.$_isDisposed || this.positioningDisabled) return;
             const t = {
                 strategy: this.strategy,
                 middleware: []
             };
-            (this.distance || this.skidding) && t.middleware.push(GC({
+            (this.distance || this.skidding) && t.middleware.push(TC({
                 mainAxis: this.distance,
                 crossAxis: this.skidding
             }));
             const n = this.placement.startsWith("auto");
             if (n ? t.middleware.push(BC({
                     alignment: (e = this.placement.split("-")[1]) != null ? e : ""
                 })) : t.placement = this.placement, this.preventOverflow && (this.shift && t.middleware.push(kC({
@@ -17045,38 +17047,38 @@
             this._resizeObject.contentDocument.defaultView.addEventListener("resize", this.compareAndNotify), this.compareAndNotify()
         },
         removeResizeHandlers() {
             this._resizeObject && this._resizeObject.onload && (!Qo && this._resizeObject.contentDocument && this._resizeObject.contentDocument.defaultView.removeEventListener("resize", this.compareAndNotify), this.$el.removeChild(this._resizeObject), this._resizeObject.onload = null, this._resizeObject = null)
         }
     }
 };
-const gy = Fa();
+const gy = Pa();
 Ka("data-v-b329ee4c");
 const py = {
     class: "resize-observer",
     tabindex: "-1"
 };
-Pa();
+Fa();
 const my = gy((e, t, n, o, s, i) => (j(), Me("div", py)));
 Ys.render = my;
 Ys.__scopeId = "data-v-b329ee4c";
 Ys.__file = "src/components/ResizeObserver.vue";
-var Tc = (e = "theme") => ({
+var Gc = (e = "theme") => ({
     computed: {
         themeClass() {
             return oy(this[e])
         }
     }
 });
 const Iy = Ce({
         name: "VPopperContent",
         components: {
             ResizeObserver: Ys
         },
-        mixins: [Tc()],
+        mixins: [Gc()],
         props: {
             popperId: String,
             theme: String,
             shown: Boolean,
             mounted: Boolean,
             skipTransition: Boolean,
             autoHide: Boolean,
@@ -17092,18 +17094,18 @@
         }
     }),
     hy = ["id", "aria-hidden", "tabindex", "data-popper-placement"],
     by = {
         ref: "inner",
         class: "v-popper__inner"
     },
-    Cy = F("div", {
+    Cy = P("div", {
         class: "v-popper__arrow-outer"
     }, null, -1),
-    yy = F("div", {
+    yy = P("div", {
         class: "v-popper__arrow-inner"
     }, null, -1),
     Ay = [Cy, yy];
 
 function vy(e, t, n, o, s, i) {
     const f = tt("ResizeObserver");
     return j(), U("div", {
@@ -17124,37 +17126,37 @@
             position: e.result.strategy,
             transform: `translate3d(${Math.round(e.result.x)}px,${Math.round(e.result.y)}px,0)`
         } : void 0),
         "aria-hidden": e.shown ? "false" : "true",
         tabindex: e.autoHide ? 0 : void 0,
         "data-popper-placement": e.result ? e.result.placement : void 0,
         onKeyup: t[2] || (t[2] = yl(r => e.autoHide && e.$emit("hide"), ["esc"]))
-    }, [F("div", {
+    }, [P("div", {
         class: "v-popper__backdrop",
         onClick: t[0] || (t[0] = r => e.autoHide && e.$emit("hide"))
-    }), F("div", {
+    }), P("div", {
         class: "v-popper__wrapper",
         style: Ot(e.result ? {
             transformOrigin: e.result.transformOrigin
         } : void 0)
-    }, [F("div", by, [e.mounted ? (j(), U(_e, {
+    }, [P("div", by, [e.mounted ? (j(), U(_e, {
         key: 0
-    }, [F("div", null, [Xe(e.$slots, "default")]), e.handleResize ? (j(), Me(f, {
+    }, [P("div", null, [Xe(e.$slots, "default")]), e.handleResize ? (j(), Me(f, {
         key: 0,
         onNotify: t[1] || (t[1] = r => e.$emit("resize", r))
-    })) : me("", !0)], 64)) : me("", !0)], 512), F("div", {
+    })) : me("", !0)], 64)) : me("", !0)], 512), P("div", {
         ref: "arrow",
         class: "v-popper__arrow-container",
         style: Ot(e.result ? {
             left: e.toPx(e.result.arrow.x),
             top: e.toPx(e.result.arrow.y)
         } : void 0)
     }, Ay, 4)], 4)], 46, hy)
 }
-var Gc = Xs(Iy, [
+var Tc = Xs(Iy, [
         ["render", vy]
     ]),
     jc = {
         methods: {
             show(...e) {
                 return this.$refs.popper.show(...e)
             },
@@ -17169,17 +17171,17 @@
             }
         }
     };
 const wy = Ce({
     name: "VPopperWrapper",
     components: {
         Popper: uy,
-        PopperContent: Gc
+        PopperContent: Tc
     },
-    mixins: [jc, Tc("finalTheme")],
+    mixins: [jc, Gc("finalTheme")],
     props: {
         theme: {
             type: String,
             default: null
         }
     },
     computed: {
@@ -17212,30 +17214,30 @@
             skipTransition: u,
             autoHide: d,
             show: m,
             hide: p,
             handleResize: h,
             onResize: b,
             classes: y,
-            result: G
+            result: T
         }) => [Xe(e.$slots, "default", {
             shown: l,
             show: m,
             hide: p
         }), se(f, {
             ref: "popperContent",
             "popper-id": a,
             theme: e.finalTheme,
             shown: l,
             mounted: c,
             "skip-transition": u,
             "auto-hide": d,
             "handle-resize": h,
             classes: y,
-            result: G,
+            result: T,
             onHide: p,
             onResize: b
         }, {
             default: Ne(() => [Xe(e.$slots, "popper", {
                 shown: l,
                 hide: p
             })]),
@@ -17259,15 +17261,15 @@
         name: "VTooltip",
         vPopperTheme: "tooltip"
     })),
     Wy = Ce({
         name: "VTooltipDirective",
         components: {
             Popper: zc(),
-            PopperContent: Gc
+            PopperContent: Tc
         },
         mixins: [jc],
         inheritAttrs: !1,
         props: {
             theme: {
                 type: String,
                 default: "tooltip"
@@ -17378,43 +17380,43 @@
             onResize: h
         }, {
             default: Ne(() => [e.html ? (j(), U("div", {
                 key: 0,
                 innerHTML: e.finalContent
             }, null, 8, Sy)) : (j(), U("div", {
                 key: 1,
-                textContent: Te(e.finalContent)
+                textContent: Ge(e.finalContent)
             }, null, 8, By))]),
             _: 2
         }, 1032, ["class", "popper-id", "theme", "shown", "mounted", "skip-transition", "auto-hide", "handle-resize", "classes", "result", "onHide", "onResize"])]),
         _: 1
     }, 16, ["theme", "popper-node", "onApplyShow", "onApplyHide"])
 }
 var Vy = Xs(Wy, [
     ["render", zy]
 ]);
 const kc = "v-popper--has-tooltip";
 
-function Ty(e, t) {
+function Gy(e, t) {
     let n = e.placement;
     if (!n && t)
         for (const o of Bc) t[o] && (n = o);
     return n || (n = Xn(e.theme || "tooltip", "placement")), n
 }
 
 function Dc(e, t, n) {
     let o;
     const s = typeof t;
     return s === "string" ? o = {
         content: t
     } : t && s === "object" ? o = t : o = {
         content: !1
-    }, o.placement = Ty(o, n), o.targetNodes = () => [e], o.referenceNode = () => e, o
+    }, o.placement = Gy(o, n), o.targetNodes = () => [e], o.referenceNode = () => e, o
 }
-let fi, Co, Gy = 0;
+let fi, Co, Ty = 0;
 
 function jy() {
     if (fi) return;
     Co = oe([]), fi = Al({
         name: "VTooltipDirectiveApp",
         setup() {
             return {
@@ -17436,15 +17438,15 @@
 }
 
 function ky(e, t, n) {
     jy();
     const o = oe(Dc(e, t, n)),
         s = oe(!1),
         i = {
-            id: Gy++,
+            id: Ty++,
             options: o,
             shown: s
         };
     return Co.value.push(i), e.classList && e.classList.add(kc), e.$_popper = {
         options: o,
         item: i,
         show() {
```

### Comparing `amlopschat-1.0.7/amlopschat/static/chat/link.svg` & `amlopschat-1.0.8/amlopschat/static/chat/link.svg`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.7/amlopschat/static/chat/microphone.svg` & `amlopschat-1.0.8/amlopschat/static/chat/microphone.svg`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.7/amlopschat/static/chat/no-messages.gif` & `amlopschat-1.0.8/amlopschat/static/chat/no-messages.gif`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.7/amlopschat/static/chat/user.png` & `amlopschat-1.0.8/amlopschat/static/chat/user.png`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.7/amlopschat.egg-info/SOURCES.txt` & `amlopschat-1.0.8/amlopschat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amlopschat-1.0.7/versioneer.py` & `amlopschat-1.0.8/versioneer.py`

 * *Files identical despite different names*

