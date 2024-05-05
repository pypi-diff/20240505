# Comparing `tmp/feincms3_cookiecontrol-1.4.6.tar.gz` & `tmp/feincms3_cookiecontrol-1.5.0.tar.gz`

## Comparing `feincms3_cookiecontrol-1.4.6.tar` & `feincms3_cookiecontrol-1.5.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/__init__.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/admin.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/apps.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/embedding.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/models.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/views.py
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/migrations/0001_rework.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/migrations/__init__.py
--rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/static/f3cc.js
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/templates/feincms3_cookiecontrol/banner.html
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/templates/feincms3_cookiecontrol/embed.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/templatetags/__init__.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/templatetags/feincms3_cookiecontrol.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/.gitignore
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/LICENSE
--rw-r--r--   0        0        0     9790 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/README.rst
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/pyproject.toml
--rw-r--r--   0        0        0    11082 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.4.6/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/__init__.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/admin.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/apps.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/embedding.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/models.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/views.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/migrations/0001_rework.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/migrations/__init__.py
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/static/f3cc.js
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/static/f3cc/gcm.js
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/templates/feincms3_cookiecontrol/banner.html
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/templates/feincms3_cookiecontrol/embed.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/templatetags/__init__.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/templatetags/feincms3_cookiecontrol.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/.gitignore
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/LICENSE
+-rw-r--r--   0        0        0     9790 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/README.rst
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0    11160 2020-02-02 00:00:00.000000 feincms3_cookiecontrol-1.5.0/PKG-INFO
```

### Comparing `feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/embedding.py` & `feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/embedding.py`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/models.py` & `feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/models.py`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/views.py` & `feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/views.py`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.mo` & `feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/locale/es/LC_MESSAGES/django.mo` & `feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/locale/es/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.mo` & `feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.mo` & `feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.mo` & `feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.po` & `feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/locale/rm/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/migrations/0001_rework.py` & `feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/migrations/0001_rework.py`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/static/f3cc.js` & `feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/static/f3cc.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,169 +1,160 @@
 (() => {
     (function() {
         var e = document.createElement("style");
         e.textContent = ".f3cc{font-size:16px;line-height:1.3;--_b:var(--f3cc-background,#e9e9e9);--_f:var(--f3cc-foreground,#000000);--_B:var(--f3cc-button-background,#cbcbcb);--_A:var(--f3cc-accept-background,#90f690);--_F:var(--f3cc-button-foreground,var(--_f));--_E:var(--f3cc-accept-foreground,var(--_F))}.f3cc .f3cc-banner{position:fixed;bottom:0;width:100%;background:var(--_b);color:var(--_f);z-index:2000;padding:1rem 1rem 1.25rem}.f3cc .f3cc-embed{background:var(--_b);color:var(--_f);padding:4rem}.f3cc .f3cc-container{display:flex;gap:2rem;max-width:70em;margin:0 auto;width:80%}@media (max-width:60rem){.f3cc .f3cc-container{width:100%;flex-direction:column}}.f3cc .f3cc-title{font-size:1.5em;font-weight:700;margin-bottom:.25em}.f3cc .f3cc-description a{color:inherit;text-decoration:underline}.f3cc .f3cc-description a:hover{opacity:.7}.f3cc .f3cc-buttons{display:flex;flex-direction:column;gap:1rem;justify-content:center;align-items:stretch}.f3cc .f3cc-button{display:inline-block;background:var(--_B);color:var(--_F);padding:.8rem 1.2rem;white-space:nowrap;text-decoration:none;text-align:center;cursor:pointer;border:none}.f3cc .f3cc-button:hover{opacity:.7}.f3cc .f3cc-button.accept{background:var(--_A);color:var(--_E)}.f3cc .f3cc-button.modify{position:fixed;z-index:2000;bottom:1rem;right:1rem}.f3cc-embed .f3cc-description{margin-bottom:1em}", document.head.appendChild(e)
     })();
     var b = (e, t = document) => t.querySelector(e),
-        w = document.body,
+        k = (e, t = document) => t.querySelectorAll(e),
+        x = document.body,
         r = "className",
-        f = "textContent",
+        l = "textContent",
         j = "innerHTML",
-        x = "f3cc",
-        i = window.f3ccData || JSON.parse(b("#f3cc-data")[f]),
-        y = {},
+        _ = "f3cc",
+        i = window.f3ccData || JSON.parse(b("#f3cc-data")[l]),
+        w = {},
         m = "f3cc-embed-providers",
-        p, d, s, o = (e, t = null, c = []) => {
-            let n = document.createElement(e);
+        p, f, d, o = (e, t = null, n = []) => {
+            let c = document.createElement(e);
             if (t)
-                for (let [a, l] of Object.entries(t)) a.startsWith("data-") ? n.setAttribute(a, l) : n[a] = l;
-            return n.append(...c), n
+                for (let [a, s] of Object.entries(t)) a.startsWith("data-") ? c.setAttribute(a, s) : c[a] = s;
+            return c.append(...n), c
         },
         u = () => {
-            if (d) {
-                N(d);
+            if (f) {
+                N(f);
                 return
             }
             let e = [o("div", {
                     [r]: "f3cc-title",
-                    [f]: i.heading
+                    [l]: i.heading
                 }), o("div", {
                     [r]: "f3cc-description",
                     [j]: i.description
                 })],
                 t = [o("a", {
                     [r]: "f3cc-button accept",
-                    [f]: i.buttonAccept,
-                    onclick: k(!0)
+                    [l]: i.buttonAccept,
+                    onclick: y(!0)
                 }), o("a", {
                     [r]: "f3cc-button reject",
-                    [f]: i.buttonReject,
-                    onclick: k(!1)
+                    [l]: i.buttonReject,
+                    onclick: y(!1)
                 })];
-            d = o("div", {
+            f = o("div", {
                 [r]: "f3cc f3cc-banner"
             }, [o("div", {
                 [r]: "f3cc-container"
             }, [o("div", {
                 [r]: "f3cc-content"
             }, e), o("div", {
                 [r]: "f3cc-buttons"
-            }, t)])]), g().append(d)
+            }, t)])]), g().append(f)
         },
-        _ = () => {
-            if (s) {
-                N(s);
+        E = () => {
+            if (d) {
+                N(d);
                 return
             }
             let e;
             if (e = b(".f3cc-modify")) {
-                e.addEventListener("click", n => {
-                    n.preventDefault(), u()
+                e.addEventListener("click", c => {
+                    c.preventDefault(), u()
                 });
                 return
             }
             let t = i.ppu,
-                c = window.location;
-            i.buttonModify && (!t || t == `${c.protocol}//${c.host}${c.pathname}`) && (s = o("a", {
+                n = window.location;
+            i.buttonModify && (!t || t == `${n.protocol}//${n.host}${n.pathname}`) && (d = o("a", {
                 [r]: "f3cc-button modify",
-                [f]: i.buttonModify,
-                onclick: n => {
-                    n.preventDefault(), A(s), u()
+                [l]: i.buttonModify,
+                onclick: c => {
+                    c.preventDefault(), T(d), u()
                 }
-            }), g().append(s))
+            }), g().append(d))
         },
-        I = e => {
-            let t = `${x}=${e};max-age=31536000;path=/;sameSite=Strict`;
+        D = e => {
+            let t = `${_}=${e};max-age=31536000;path=/;sameSite=Strict`;
             i.domain && (t += `;domain=${i.domain}`), document.cookie = t
         },
         S = () => {
-            let e = `${x}=`;
+            let e = `${_}=`;
             for (let t of document.cookie.split("; "))
                 if (t.startsWith(e)) return decodeURIComponent(t.substring(e.length))
         },
         v = "all",
         C = "essential",
-        R = () => {
+        H = () => {
             let e = S();
             return v == e || C == e
         },
-        E = () => S() === v,
+        A = () => S() === v,
         N = e => {
             e.style.display = ""
         },
-        A = e => {
+        T = e => {
             e && (e.style.display = "none")
         },
-        k = e => t => {
-            t.preventDefault(), I(e ? v : C), A(d), _(), h(), L()
+        y = e => t => {
+            t.preventDefault(), D(e ? v : C), T(f), E(), h(), L(), window.dispatchEvent(new Event(`f3cc_consent_${e?"granted":"denied"}`))
         },
         L = () => {
-            if (E())
+            if (A())
                 for (let e of i.cookies) {
-                    let t = y[e.name];
-                    t || (y[e.name] = t = o("div"), t.dataset.name = e.name, g().append(t)), t.innerHTML = e.script, $(t)
+                    let t = w[e.name];
+                    t || (w[e.name] = t = o("div"), t.dataset.name = e.name, g().append(t)), z(t, e.script)
                 }
         },
         g = () => (p || (p = o("div", {
             [r]: "f3cc"
-        }), w.append(p)), p),
+        }), x.append(p)), p),
         M = {},
-        D = (e, t) => {
+        I = (e, t) => {
             try {
                 window.localStorage.setItem(e, JSON.stringify(t))
             } catch {
                 M[e] = t
             }
         },
-        T = e => {
+        $ = e => {
             try {
                 return JSON.parse(window.localStorage.getItem(e))
             } catch {
                 return M[e]
             }
         },
         h = window.f3ccRenderEmbeds = () => {
-            let e = T(m) || [];
-            document.querySelectorAll(".f3cc-embed").forEach(c => {
-                let n = b("template", c),
-                    a = c.dataset.provider;
-                if (n && a && (E() || e.includes(a))) {
-                    let l = n.content.cloneNode(!0);
-                    c.closest(".f3cc").replaceWith(l)
+            let e = $(m) || [];
+            k(".f3cc-embed").forEach(n => {
+                let c = b("template", n),
+                    a = n.dataset.provider;
+                if (c && a && (A() || e.includes(a))) {
+                    let s = c.content.cloneNode(!0);
+                    n.closest(".f3cc").replaceWith(s)
                 }
             })
         },
-        z = () => {
-            w.addEventListener("click", e => {
+        q = () => {
+            x.addEventListener("click", e => {
                 let t = e.target.closest(".f3cc-button"),
-                    c = t && t.closest(".f3cc-embed");
-                if (t && c) {
+                    n = t && t.closest(".f3cc-embed");
+                if (t && n) {
                     e.preventDefault();
-                    let n = T(m) || [];
-                    n.push(c.dataset.provider), D(m, n), h()
+                    let c = $(m) || [];
+                    c.push(n.dataset.provider), I(m, c), h()
                 }
             })
         },
-        $ = e => {
-            if (H(e) === !0) e.parentNode.replaceChild(F(e), e);
-            else {
-                let t = -1,
-                    c = e.childNodes;
-                for (; ++t < c.length;) $(c[t])
-            }
-            return e
-        },
-        F = e => {
-            let t = o("script");
-            t.text = e.innerHTML;
-            let c = -1,
-                n = e.attributes,
-                a;
-            for (; ++c < n.length;) t.setAttribute((a = n[c]).name, a.value);
-            return t
-        },
-        H = e => e.tagName === "SCRIPT";
+        z = (e, t) => {
+            e.innerHTML = t;
+            for (let n of k("script", e)) {
+                let c = document.createElement("script");
+                for (let s of n.attributes) c.setAttribute(s.name, s.value);
+                let a = document.createTextNode(n.innerHTML);
+                c.appendChild(a), n.replaceWith(c)
+            }
+        };
     L();
     h();
-    z();
-    R() ? _() : u();
+    q();
+    H() ? E() : u();
 })();
```

### Comparing `feincms3_cookiecontrol-1.4.6/feincms3_cookiecontrol/templatetags/feincms3_cookiecontrol.py` & `feincms3_cookiecontrol-1.5.0/feincms3_cookiecontrol/templatetags/feincms3_cookiecontrol.py`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.4.6/LICENSE` & `feincms3_cookiecontrol-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.4.6/README.rst` & `feincms3_cookiecontrol-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `feincms3_cookiecontrol-1.4.6/pyproject.toml` & `feincms3_cookiecontrol-1.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 ]
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: Django",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
+    "Framework :: Django :: 5.0",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `feincms3_cookiecontrol-1.4.6/PKG-INFO` & `feincms3_cookiecontrol-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: feincms3-cookiecontrol
-Version: 1.4.6
+Version: 1.5.0
 Summary: Cookie Control Panel for GDPR compliant feincms3 websites
 Project-URL: Homepage, https://github.com/feinheit/feincms3-cookiecontrol/
 Author-email: York Schickl <ys@feinheit.ch>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

