# Comparing `tmp/streamlit-navigation-bar-3.1.2.tar.gz` & `tmp/streamlit-navigation-bar-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-navigation-bar-3.1.2.tar", last modified: Fri Apr 19 17:36:36 2024, max compression
+gzip compressed data, was "streamlit-navigation-bar-3.2.0.tar", last modified: Sun May  5 12:57:30 2024, max compression
```

## Comparing `streamlit-navigation-bar-3.1.2.tar` & `streamlit-navigation-bar-3.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-19 17:36:36.672514 streamlit-navigation-bar-3.1.2/
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     1073 2024-01-27 21:14:24.000000 streamlit-navigation-bar-3.1.2/LICENSE
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       59 2024-03-03 21:06:11.000000 streamlit-navigation-bar-3.1.2/MANIFEST.in
--rw-r--r--   0 gabrieltempass   (501) staff       (20)    15103 2024-04-19 17:36:36.672321 streamlit-navigation-bar-3.1.2/PKG-INFO
--rw-r--r--   0 gabrieltempass   (501) staff       (20)    13316 2024-04-09 19:20:43.000000 streamlit-navigation-bar-3.1.2/README.md
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       38 2024-04-19 17:36:36.672563 streamlit-navigation-bar-3.1.2/setup.cfg
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     2474 2024-04-19 17:33:41.000000 streamlit-navigation-bar-3.1.2/setup.py
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-19 17:36:36.669415 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/
--rw-r--r--   0 gabrieltempass   (501) staff       (20)    17362 2024-04-09 19:02:56.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/__init__.py
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       77 2024-04-19 17:15:50.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/__main__.py
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     8452 2024-04-06 13:59:37.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/errors.py
--rw-r--r--   0 gabrieltempass   (501) staff       (20)      680 2024-04-19 17:10:51.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/example.py
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-19 17:36:36.667314 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/frontend/
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-19 17:36:36.670659 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/frontend/dist/
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-19 17:36:36.672064 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/frontend/dist/assets/
--rw-r--r--   0 gabrieltempass   (501) staff       (20)   241380 2024-04-06 12:47:00.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/frontend/dist/assets/index-QGLefmoh.js
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     1150 2024-04-06 12:47:00.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/frontend/dist/assets/index-nKPQXLAl.css
--rw-r--r--   0 gabrieltempass   (501) staff       (20)      683 2024-04-06 12:47:00.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/frontend/dist/index.html
--rw-r--r--   0 gabrieltempass   (501) staff       (20)     8267 2024-03-27 17:37:32.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/match_navbar.py
-drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-04-19 17:36:36.670538 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar.egg-info/
--rw-r--r--   0 gabrieltempass   (501) staff       (20)    15103 2024-04-19 17:36:36.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar.egg-info/PKG-INFO
--rw-r--r--   0 gabrieltempass   (501) staff       (20)      693 2024-04-19 17:36:36.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar.egg-info/SOURCES.txt
--rw-r--r--   0 gabrieltempass   (501) staff       (20)        1 2024-04-19 17:36:36.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar.egg-info/dependency_links.txt
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       85 2024-04-19 17:36:36.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar.egg-info/entry_points.txt
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       43 2024-04-19 17:36:36.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar.egg-info/requires.txt
--rw-r--r--   0 gabrieltempass   (501) staff       (20)       25 2024-04-19 17:36:36.000000 streamlit-navigation-bar-3.1.2/streamlit_navigation_bar.egg-info/top_level.txt
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-05-05 12:57:30.974625 streamlit-navigation-bar-3.2.0/
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     1073 2024-01-27 21:14:24.000000 streamlit-navigation-bar-3.2.0/LICENSE
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       59 2024-03-03 21:06:11.000000 streamlit-navigation-bar-3.2.0/MANIFEST.in
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     6561 2024-05-05 12:57:30.974488 streamlit-navigation-bar-3.2.0/PKG-INFO
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     4760 2024-05-05 12:20:56.000000 streamlit-navigation-bar-3.2.0/README.md
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       38 2024-05-05 12:57:30.974670 streamlit-navigation-bar-3.2.0/setup.cfg
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     2442 2024-05-05 01:28:38.000000 streamlit-navigation-bar-3.2.0/setup.py
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-05-05 12:57:30.971517 streamlit-navigation-bar-3.2.0/streamlit_navigation_bar/
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)    14212 2024-05-05 12:54:53.000000 streamlit-navigation-bar-3.2.0/streamlit_navigation_bar/__init__.py
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       77 2024-04-19 17:15:50.000000 streamlit-navigation-bar-3.2.0/streamlit_navigation_bar/__main__.py
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     8547 2024-05-04 15:32:59.000000 streamlit-navigation-bar-3.2.0/streamlit_navigation_bar/errors.py
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)      680 2024-05-03 20:55:49.000000 streamlit-navigation-bar-3.2.0/streamlit_navigation_bar/example.py
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-05-05 12:57:30.968048 streamlit-navigation-bar-3.2.0/streamlit_navigation_bar/frontend/
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-05-05 12:57:30.972613 streamlit-navigation-bar-3.2.0/streamlit_navigation_bar/frontend/dist/
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-05-05 12:57:30.973102 streamlit-navigation-bar-3.2.0/streamlit_navigation_bar/frontend/dist/assets/
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     1150 2024-05-03 20:58:53.000000 streamlit-navigation-bar-3.2.0/streamlit_navigation_bar/frontend/dist/assets/index-8KihYu-x.css
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)   241380 2024-05-03 20:58:53.000000 streamlit-navigation-bar-3.2.0/streamlit_navigation_bar/frontend/dist/assets/index-oWBpKCwX.js
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)      683 2024-05-03 20:58:53.000000 streamlit-navigation-bar-3.2.0/streamlit_navigation_bar/frontend/dist/index.html
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     8355 2024-05-04 21:48:10.000000 streamlit-navigation-bar-3.2.0/streamlit_navigation_bar/match_navbar.py
+drwxr-xr-x   0 gabrieltempass   (501) staff       (20)        0 2024-05-05 12:57:30.972502 streamlit-navigation-bar-3.2.0/streamlit_navigation_bar.egg-info/
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)     6561 2024-05-05 12:57:30.000000 streamlit-navigation-bar-3.2.0/streamlit_navigation_bar.egg-info/PKG-INFO
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)      693 2024-05-05 12:57:30.000000 streamlit-navigation-bar-3.2.0/streamlit_navigation_bar.egg-info/SOURCES.txt
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)        1 2024-05-05 12:57:30.000000 streamlit-navigation-bar-3.2.0/streamlit_navigation_bar.egg-info/dependency_links.txt
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       85 2024-05-05 12:57:30.000000 streamlit-navigation-bar-3.2.0/streamlit_navigation_bar.egg-info/entry_points.txt
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       34 2024-05-05 12:57:30.000000 streamlit-navigation-bar-3.2.0/streamlit_navigation_bar.egg-info/requires.txt
+-rw-r--r--   0 gabrieltempass   (501) staff       (20)       25 2024-05-05 12:57:30.000000 streamlit-navigation-bar-3.2.0/streamlit_navigation_bar.egg-info/top_level.txt
```

### Comparing `streamlit-navigation-bar-3.1.2/LICENSE` & `streamlit-navigation-bar-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.1.2/setup.py` & `streamlit-navigation-bar-3.2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="streamlit-navigation-bar",
-    version="3.1.2",
+    version="3.2.0",
     description="A component that allows you to place a navigation bar in your Streamlit app.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gabrieltempass/streamlit-navigation-bar",
     project_urls={
         "Source Code": "https://github.com/gabrieltempass/streamlit-navigation-bar",
         "Bug Tracker": "https://github.com/gabrieltempass/streamlit-navigation-bar/issues",
         "Release notes": "https://github.com/gabrieltempass/streamlit-navigation-bar/releases",
-        "Documentation": "https://github.com/gabrieltempass/streamlit-navigation-bar/wiki",
+        "Documentation": "https://github.com/gabrieltempass/streamlit-navigation-bar/wiki/API-reference",
         "Community": "https://discuss.streamlit.io/t/new-component-streamlit-navigation-bar/66032",
     },
     author="Gabriel Tem Pass",
     author_email="redo_hint_0x@icloud.com",
     license="MIT License",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
@@ -52,11 +52,11 @@
     entry_points={
         "console_scripts": [
             "streamlit-navigation-bar = streamlit_navigation_bar:print_version",
         ]
     },
     python_requires=">=3.8",
     install_requires=[
-        "streamlit >= 1.29.0, != 1.32.2",  # Navbar doesn't work with 1.32.2
-        "st-theme >= 1.2.2",
+        "streamlit >= 1.33.0",
+        "st-theme >= 1.2.3",
     ],
 )
```

### Comparing `streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/__init__.py` & `streamlit-navigation-bar-3.2.0/streamlit_navigation_bar/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,45 +45,46 @@
 def _encode_svg(path):
     """Encode an SVG to base64, from an absolute path."""
     svg = open(path).read()
     return base64.b64encode(svg.encode("utf-8")).decode("utf-8")
 
 
 def _prepare_urls(urls, pages):
-    """Build dict with targets, given hrefs and defaults where omitted."""
+    """Build dict with given hrefs, targets and defaults where omitted."""
     if urls is None:
         urls = {}
     for page in pages:
+        # Add {page: [href, target]} to the `urls` dict.
         if page in urls:
             urls[page] = [urls[page], "_blank"]
         else:
             urls[page] = ["#", "_self"]
     return urls
 
 
 def _prepare_options(options):
     """Build dict with given options, state and defaults where omitted."""
     available = {
         "show_menu": True,
         "show_sidebar": True,
+        "hide_nav": True,
         "fix_shadow": True,
         "use_padding": True,
     }
     for option in available:
         if isinstance(options, dict) and option in options:
             available[option] = options[option]
         elif isinstance(options, bool) and not options:
             available[option] = options
     return available
 
 
 def _adjust(css):
     """Apply a CSS adjustment."""
-    wrapped = "<style>" + css + "</style>"
-    st.markdown(wrapped, unsafe_allow_html=True)
+    st.html("<style>" + css + "</style>")
 
 
 def get_path(directory):
     """Get the abs path for a directory in the same location as this file."""
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     return os.path.join(parent_dir, directory)
 
@@ -94,17 +95,16 @@
     return Environment(loader=loader, trim_blocks=True, lstrip_blocks=True)
 
 
 def position_body(key, use_padding):
     """
     Add a stylized container to the app that adjusts the position of the body.
 
-    Insert a container into the app, to add an ``st.markdown``, using either
-    the "with" notation or by calling the method directly on the returned
-    object.
+    Insert a container into the app, to add an ``st.html``, using either the
+    "with" notation or by calling the method directly on the returned object.
 
     This container serves to position the body of the app in the y axis of the
     window. Which can be the same as the default in Streamlit (6rem from the
     top), or right below the navbar.
 
     It does so by having a unique CSS selector, and being inserted in a <div>
     palced immediately before the <div> of the body of the app. Then, it styles
@@ -115,44 +115,42 @@
     key : str, int or None
         A key associated with this container. This needs to be unique since all
         styles will be applied to the container with this key.
 
     Returns
     -------
     container : DeltaGenerator
-        A container object. ``st.markdown`` can be added to this container
-        using either the ``"with"`` notation or by calling methods directly on
-        the returned object.
+        A container object. ``st.html`` can be added to this container using
+        either the ``"with"`` notation or by calling methods directly on the
+        returned object.
     """
     if use_padding:
         # The position of the body will be 6rem from the top.
-        margin_bottom = "-5.875rem"
+        margin_bottom = "-4.875rem"
     else:
         # The position of the body will be right below the navbar.
-        margin_bottom = "-9rem"
+        margin_bottom = "-8rem"
 
     html = (
         f"""
         <style>
             div[data-testid="stVerticalBlockBorderWrapper"]:has(
                 div[data-testid="stVerticalBlock"]
                 > div.element-container
-                > div.stMarkdown
-                > div[data-testid='stMarkdownContainer']
-                > p
+                > div.stHtml
                 > span.{key}
             ) {{
                 margin-bottom: {margin_bottom};
             }}
         </style>
         <span class='{key}'></span>
         """
     )
     container = st.container()
-    container.markdown(html, unsafe_allow_html=True)
+    container.html(html)
     return container
 
 
 def adjust_css(styles, options, key, path):
     """
     Apply CSS adjustments to display the navbar correctly.
 
@@ -162,34 +160,35 @@
     top of the window, among other options that can be toggled on or off.
 
     It also matches the style, theme and configuration between the navbar and 
     Streamlit's User Interface (UI) elements, to make them look seamless.
 
     Parameters
     ----------
-    styles : dict of {str : {dict of {str : str}}
+    styles : dict of {str : dict of {str : str}}
         Apply CSS styles to desired targets, through a dictionary with the HTML
         tag or pseudo-class name as the key and another dictionary to style it
         as the value. In the second dictionary, the key-value pair is the name
-        of a CSS property and the value it takes. The keys and values must be
-        strings.
+        of a CSS property and the value it takes, both in string format. It
+        accepts CSS variables to be passed as values.
 
         The available HTML tags are: ``"nav"``, ``"div"``, ``"ul"``, ``"li"``,
         ``"a"``, ``"img"`` and ``"span"``.
 
         The available pseudo-classes are: ``"active"`` and ``"hover"``, which
         direct the styling to the ``"span"`` tag. The menu and sidebar buttons
         are only styled by ``"hover"`` (if they are set to ``True`` in
         `options`). Currently, ``"hover"`` only accepts two CSS properties,
         they are: ``"color"`` and ``"background-color"``.
     options : bool or dict of {str : bool}
         Customize the navbar with options that can be toggled on or off. It
         accepts a dictionary with the option name as the key and a boolean as
         the value. The available options are: ``"show_menu"``,
-        ``"show_sidebar"``, ``"fix_shadow"`` and ``"use_padding"``.
+        ``"show_sidebar"``, ``"hide_nav"``, ``"fix_shadow"`` and
+        ``"use_padding"``.
 
         It is also possible to toggle all options to the same state. Simply
         pass ``True`` or ``False`` to `options`.
     key : str, int or None
         A key associated with the container that adjusts the CSS. This needs to
         be unique since all styles will be applied to the container with this
         key.
@@ -240,15 +239,15 @@
         margin=margin,
         key=key,
     )
     with position_body(key, options["use_padding"]):
         _adjust(css)
 
 
-# A placeholder object to implement the default rules for selected
+# A placeholder object to implement the default rules for `selected`.
 sentinel = object()
 
 
 def st_navbar(
     pages,
     selected=sentinel,
     logo_path=None,
@@ -288,178 +287,87 @@
         there is one. Defaults to ``"Home"``. For a non-clickable logo, set
         this to ``None``.
     urls : dict of {str : str}, optional
         A dictionary with the page name as the key and an external URL as the
         value, both as strings. The page name must be contained in the `pages`
         list. The URL will open in a new window or tab. The default is
         ``None``.
-    styles : dict of {str : {dict of {str : str}}, optional
+    styles : dict of {str : dict of {str : str}}, optional
         Apply CSS styles to desired targets, through a dictionary with the HTML
         tag or pseudo-class name as the key and another dictionary to style it
         as the value. In the second dictionary, the key-value pair is the name
-        of a CSS property and the value it takes. The keys and values must be
-        strings. Defaults to ``None``, where no custom style is applied.
+        of a CSS property and the value it takes, both in string format. It
+        accepts CSS variables to be passed as values. Defaults to ``None``,
+        where just the default style is applied.
 
         The available HTML tags are: ``"nav"``, ``"div"``, ``"ul"``, ``"li"``,
-        ``"a"``, ``"img"`` and ``"span"``. To better understand the Document
-        Object Model, check the notes section.
+        ``"a"``, ``"img"`` and ``"span"``.
 
         The available pseudo-classes are: ``"active"`` and ``"hover"``, which
         direct the styling to the ``"span"`` tag. The menu and sidebar buttons
         are only styled by ``"hover"`` (if they are set to ``True`` in
         `options`). Currently, ``"hover"`` only accepts two CSS properties,
         they are: ``"color"`` and ``"background-color"``.
+
+        To understand the Document Object Model from the navbar, the CSS
+        variables and the default style, go to the API reference in the Notes
+        section.
     options : bool or dict of {str : bool}, default=True
         Customize the navbar with options that can be toggled on or off. It
         accepts a dictionary with the option name as the key and a boolean as
         the value. The available options are: ``"show_menu"``,
-        ``"show_sidebar"``, ``"fix_shadow"`` and ``"use_padding"``. Check the
-        notes section for a description of each one.
+        ``"show_sidebar"``, ``"hide_nav"``, ``"fix_shadow"`` and
+        ``"use_padding"``. Check the API reference in the Notes section for a
+        description of each one.
 
         It is also possible to toggle all options to the same state. Simply
         pass ``True`` to `options`, which is the parameter default value, or
         ``False``.
     adjust : bool, default=True
         When set to ``True`` (default), it overrides some Streamlit behaviors
         and makes a series of CSS adjustments to display the navbar correctly.
 
         In most cases, the CSS adjustments do not interfere with the rest of
         the web app, however there could be some situations where this occurs.
         If this happens, or it is desired to disable all of them, pass
         ``False`` to `adjust` and, when necessary, make your own CSS
-        adjustments with ``st.markdown``.
+        adjustments with ``st.html``.
 
         If set to ``False``, it will also disable all adjustments made by
         `options`, regardless of whether they are on or off.
     key : str or int, optional
-        A string or integer to use as a unique key for the component. Multiple
-        navbars may not share the same key. Defaults to ``None``.
+        A string or integer to use as a unique key for the component. If this
+        is omitted, a key will be generated for the widget based on its
+        content. Multiple navbars of the same type may not share the same key.
 
     Returns
     -------
     page : str or None
         The page selected by the user. If there has been no interaction yet,
         returns the preselected page or ``None``.
 
     Notes
     -----
-    **CSS variables**
-
-    The component accepts theme configuration options to be passed as CSS
-    variables in the `styles` dictionary, for example::
-    
-        styles = {
-            "nav": {
-                "background-color": "var(--primary-color)"
-            }
-        }
-    
-    The CSS variables that can be used are::
-    
-        --primary-color
-        --background-color
-        --secondary-background-color
-        --text-color
-        --font
+    To learn more about how to use the navbar, check the API reference
+    available at:
 
-    By default, the navbar uses in the following targets these CSS variables::
-    
-        styles = {
-            "nav": {
-                "font-family": "var(--font)",
-                "background-color": "var(--secondary-background-color)"
-            },
-            "span": {
-                "color": "var(--text-color)"
-            },
-            "active": {
-                "color": "var(--text-color)"
-            }
-        }
+    https://github.com/gabrieltempass/streamlit-navigation-bar/wiki/API-reference
     
-    They can be overridden by simply passing another value to the respective
-    target and CSS property in `styles`.
-
-    **Document Object Model**
-    
-    To style the navigation bar, it is important to understand its Document
-    Object Model (DOM). For example, if a navbar is created with
-    ``pages=["Hello, World!"]`` and an SVG logo. On the frontend side, the
-    component builds this DOM (simplified for readability)::
-
-        <nav>
-          <div>
-            <ul>
-              <li>
-                <a>
-                  <img src="svg_logo" img/>
-                </a>
-              </li>
-              <li>
-                <a>
-                  <span>
-                    Hello, World!
-                  </span>
-                </a>
-              </li>
-            </ul>
-          </div>
-        </nav>
-
-    Notice that the ``"a"`` tag will style both the logo and the page name.
-    However, the ``"img"`` tag is unique to the logo, just as ``"span"`` is to
-    the page names.
-
-    **Maximum width**
-
-    A fundamental CSS property to adjust is the ``"max-width"`` for the
-    ``"div"`` tag. Because it controls how much space the page names have
-    between them. The default value is ``"43.75rem"``, which works well
-    in most cases. But if the navbar has a large number of pages, or longer
-    names, it might be necessary to increase the maximum width. Conversely,
-    whenever the navbar has few pages or short names, this value may need to
-    be reduced.
-
-    **Options**
-
-    The available options and their descriptions are:
-
-    "show_menu"
-        Show Streamlit's menu button in the navbar.
-    "show_sidebar"
-        Show Streamlit's sidebar button in the navbar. However, it is still
-        needed to use ``st.sidebar`` in the app, in order for the sidebar
-        button to properly appear. Just like Streamlit's default behavior.
-    "fix_shadow"
-        Fix the shadow of the expanded sidebar, showing it no matter the window
-        width. It is useful when the navbar and the sidebar have the same
-        background color, which they do by default, because the shadow makes it
-        possible to differentiate between the two elements.
-
-        When set to ``False``, it assumes Streamlit's default behavior, where
-        it applies the shadow only when the window width is below a certain
-        threshold.
-    "use_padding"
-        Position the body of the app, in the y axis of the window, 6rem from
-        the top (if the navbar has a default height). This is the default style
-        used by Streamlit. When set to ``False``, it removes this padding and
-        positions the body right below the navbar.
-
     Examples
     --------
     >>> import streamlit as st
     >>> from streamlit_navigation_bar import st_navbar
     >>> page = st_navbar(
     ...     ["Home", "Documentation", "Examples", "Community", "About"]
     ... )
     >>> st.write(page)
 
     .. output::
-           https://st-navbar-1.streamlit.app/
-           height: 300px
+       https://st-navbar-1.streamlit.app/
+       height: 300px
     """
     check_pages(pages)
     check_selected(selected, logo_page, logo_path, pages)
     check_logo_path(logo_path)
     check_logo_page(logo_page)
     check_urls(urls, pages)
     check_styles(styles)
```

### Comparing `streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/errors.py` & `streamlit-navigation-bar-3.2.0/streamlit_navigation_bar/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,22 +203,28 @@
 
     for option, toggle in options.items():
         if not isinstance(option, str):
             raise StreamlitAPIException(
                 _dict_error(option, "options", "key", "bool")
             )
 
-        available = ["show_menu", "show_sidebar", "fix_shadow", "use_padding"]
+        available = [
+            "show_menu",
+            "show_sidebar",
+            "hide_nav",
+            "fix_shadow",
+            "use_padding",
+        ]
         if option not in available:
             raise StreamlitAPIException(
-                "The adjust parameter from st_navbar() received a "
-                "dictionary that has an invalid key. The key must be the name "
-                "of one of the available options.\n"
-                f"\nExpected: 'show_menu', 'show_sidebar', 'fix_shadow', "
-                "'use_padding'  "
+                "The option parameter from st_navbar() received a dictionary "
+                "that has an invalid key. The key must be the name of one of "
+                "the available options.\n"
+                f"\nExpected: 'show_menu', 'show_sidebar', 'hide_nav', "
+                "'fix_shadow', 'use_padding'  "
                 f"\nGot: '{option}'"
             )
 
         if not isinstance(toggle, bool):
             raise StreamlitAPIException(
                 _dict_error(toggle, "options", "value", "bool")
             )
```

### Comparing `streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/example.py` & `streamlit-navigation-bar-3.2.0/streamlit_navigation_bar/example.py`

 * *Files identical despite different names*

### Comparing `streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/frontend/dist/assets/index-QGLefmoh.js` & `streamlit-navigation-bar-3.2.0/streamlit_navigation_bar/frontend/dist/assets/index-oWBpKCwX.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -11800,16 +11800,16 @@
                 hoverColor: a,
                 hoverBgColor: c
             }
         }
     },
     il = () => {
         mp(e => ({
-            "0f327572": e.color,
-            "70c7d726": e.bgColor
+            "2d6f435a": e.color,
+            "49dd0855": e.bgColor
         }))
     },
     rl = Ja.setup;
 Ja.setup = rl ? (e, t) => (il(), rl(e, t)) : il;
 const tb = ["src"],
     eb = ["src"],
     nb = ["href", "target", "onClick"],
@@ -11853,15 +11853,15 @@
             active: o === i.activePage
         }, i.hoverColor, i.hoverBgColor]),
         style: Rt(i.parseStyles(i.styles.span) + i.parseStyles(i.styles.active, o === i.activePage))
     }, ul(o), 15, ib)], 12, nb)], 4))), 128))], 4)], 4)], 4)
 }
 const sb = Ka(Ja, [
         ["render", rb],
-        ["__scopeId", "data-v-30156451"]
+        ["__scopeId", "data-v-f2c846e5"]
     ]),
     ob = Rl({
         name: "WithStreamlitConnection",
         setup() {
             const e = ei(void 0),
                 t = ei(""),
                 n = i => {
```

### Comparing `streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/frontend/dist/index.html` & `streamlit-navigation-bar-3.2.0/streamlit_navigation_bar/frontend/dist/index.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!DOCTYPE html>
 <html lang="en">
   <head>
     <meta charset="UTF-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>Streamlit Navbar Component</title>
-    <script type="module" crossorigin src="./assets/index-QGLefmoh.js"></script>
-    <link rel="stylesheet" crossorigin href="./assets/index-nKPQXLAl.css">
+    <script type="module" crossorigin src="./assets/index-oWBpKCwX.js"></script>
+    <link rel="stylesheet" crossorigin href="./assets/index-8KihYu-x.css">
   </head>
   <body>
     <noscript>
       <strong>We're sorry but the website doesn't work properly without JavaScript enabled.
         Please enable it to continue.</strong>
     </noscript>
     <div id="app"></div>
```

### Comparing `streamlit-navigation-bar-3.1.2/streamlit_navigation_bar/match_navbar.py` & `streamlit-navigation-bar-3.2.0/streamlit_navigation_bar/match_navbar.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,19 +7,20 @@
     Represent a user interface object with a style that matches the navbar.
 
     Attributes
     ----------
     configs : dict of {str : str}
         A dictionary that maps CSS variables to theme variables names, which
         are also config options.
-    styles : dict of {str : {dict of {str : str}}
+    styles : dict of {str : dict of {str : str}}
         A dictionary with the HTML tag or pseudo-class name as the key and
         another dictionary to style it as the value. In the second dictionary,
         the key-value pair is the name of a CSS property and the value it
-        takes. The keys and values must be strings.
+        takes, both in string format. It accepts CSS variables to be passed as
+        values.
     key : str, int or None
         A key associated with the container that gets the theme. This needs to
         be unique since all styles will be applied to the container with this
         key.
 
     Methods
     -------
@@ -37,19 +38,20 @@
 
     def __init__(self, styles, key):
         """
         Instantiate a user interface object to get CSS that matches the navbar.
 
         Parameters
         ----------
-        styles : dict of {str : {dict of {str : str}}
+        styles : dict of {str : dict of {str : str}}
             A dictionary with the HTML tag or pseudo-class name as the key and
             another dictionary to style it as the value. In the second
             dictionary, the key-value pair is the name of a CSS property and
-            the value it takes. The keys and values must be strings.
+            the value it takes, both in string format. It accepts CSS variables
+            to be passed as values.
         key : str, int or None
             A key associated with the container that gets the theme. This needs
             to be unique since all styles will be applied to the container with
             this key.
         """
         self.styles = styles
         self.theme = st_theme(key=f"key_{key}")
```

### Comparing `streamlit-navigation-bar-3.1.2/streamlit_navigation_bar.egg-info/SOURCES.txt` & `streamlit-navigation-bar-3.2.0/streamlit_navigation_bar.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -10,9 +10,9 @@
 streamlit_navigation_bar.egg-info/PKG-INFO
 streamlit_navigation_bar.egg-info/SOURCES.txt
 streamlit_navigation_bar.egg-info/dependency_links.txt
 streamlit_navigation_bar.egg-info/entry_points.txt
 streamlit_navigation_bar.egg-info/requires.txt
 streamlit_navigation_bar.egg-info/top_level.txt
 streamlit_navigation_bar/frontend/dist/index.html
-streamlit_navigation_bar/frontend/dist/assets/index-QGLefmoh.js
-streamlit_navigation_bar/frontend/dist/assets/index-nKPQXLAl.css
+streamlit_navigation_bar/frontend/dist/assets/index-8KihYu-x.css
+streamlit_navigation_bar/frontend/dist/assets/index-oWBpKCwX.js
```

