# Comparing `tmp/dogpile.cache-1.3.2.tar.gz` & `tmp/dogpile.cache-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dogpile.cache-1.3.2.tar", last modified: Wed Feb 21 19:41:01 2024, max compression
+gzip compressed data, was "dogpile.cache-1.3.3.tar", last modified: Sun May  5 16:53:13 2024, max compression
```

## Comparing `dogpile.cache-1.3.2.tar` & `dogpile.cache-1.3.3.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-02-21 19:41:01.955502 dogpile.cache-1.3.2/
--rw-r--r--   0 classic   (1000) classic   (1000)      213 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/.gitignore
--rw-r--r--   0 classic   (1000) classic   (1000)       99 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/.gitreview
--rw-r--r--   0 classic   (1000) classic   (1000)      882 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/.pre-commit-config.yaml
--rw-r--r--   0 classic   (1000) classic   (1000)     1059 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/LICENSE
--rw-r--r--   0 classic   (1000) classic   (1000)      239 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/MANIFEST.in
--rw-r--r--   0 classic   (1000) classic   (1000)     5175 2024-02-21 19:41:01.955502 dogpile.cache-1.3.2/PKG-INFO
--rw-r--r--   0 classic   (1000) classic   (1000)     4176 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/README.rst
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-02-21 19:41:01.947502 dogpile.cache-1.3.2/docs/
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-02-21 19:41:01.948502 dogpile.cache-1.3.2/docs/_sources/
--rw-r--r--   0 classic   (1000) classic   (1000)     1587 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/_sources/api.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)    41854 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/_sources/changelog.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)    10222 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/_sources/core_usage.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)      769 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/_sources/front.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)     1215 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/_sources/index.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)     9296 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/_sources/recipes.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)    11625 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/_sources/usage.rst.txt
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-02-21 19:41:01.950502 dogpile.cache-1.3.2/docs/_static/
--rw-r--r--   0 classic   (1000) classic   (1000)    15094 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/_static/basic.css
--rw-r--r--   0 classic   (1000) classic   (1000)      107 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/_static/changelog.css
--rw-r--r--   0 classic   (1000) classic   (1000)     4472 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/_static/doctools.js
--rw-r--r--   0 classic   (1000) classic   (1000)      328 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/_static/documentation_options.js
--rw-r--r--   0 classic   (1000) classic   (1000)      286 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/_static/file.png
--rw-r--r--   0 classic   (1000) classic   (1000)     4758 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/_static/language_data.js
--rw-r--r--   0 classic   (1000) classic   (1000)       90 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/_static/minus.png
--rw-r--r--   0 classic   (1000) classic   (1000)     4243 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/_static/nature.css
--rw-r--r--   0 classic   (1000) classic   (1000)      507 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/_static/nature_override.css
--rw-r--r--   0 classic   (1000) classic   (1000)       90 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/_static/plus.png
--rw-r--r--   0 classic   (1000) classic   (1000)     4929 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/_static/pygments.css
--rw-r--r--   0 classic   (1000) classic   (1000)    18732 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/_static/searchtools.js
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/_static/site_custom_css.css
--rw-r--r--   0 classic   (1000) classic   (1000)     5123 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/_static/sphinx_highlight.js
--rw-r--r--   0 classic   (1000) classic   (1000)      204 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/_static/sphinx_paramlinks.css
--rw-r--r--   0 classic   (1000) classic   (1000)   503829 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/api.html
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-02-21 19:41:01.951502 dogpile.cache-1.3.2/docs/build/
--rw-r--r--   0 classic   (1000) classic   (1000)     3373 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/docs/build/Makefile
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-02-21 19:41:01.951502 dogpile.cache-1.3.2/docs/build/_static/
--rw-r--r--   0 classic   (1000) classic   (1000)      507 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/docs/build/_static/nature_override.css
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/docs/build/_static/site_custom_css.css
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-02-21 19:41:01.951502 dogpile.cache-1.3.2/docs/build/_templates/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/docs/build/_templates/site_custom_sidebars.html
--rw-r--r--   0 classic   (1000) classic   (1000)     1587 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/docs/build/api.rst
--rw-r--r--   0 classic   (1000) classic   (1000)      266 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/docs/build/builder.py
--rw-------   0 classic   (1000) classic   (1000)    41854 2024-02-21 19:40:59.000000 dogpile.cache-1.3.2/docs/build/changelog.rst
--rw-r--r--   0 classic   (1000) classic   (1000)     7408 2024-02-21 19:40:59.000000 dogpile.cache-1.3.2/docs/build/conf.py
--rw-r--r--   0 classic   (1000) classic   (1000)    10222 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/docs/build/core_usage.rst
--rw-r--r--   0 classic   (1000) classic   (1000)      769 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/docs/build/front.rst
--rw-r--r--   0 classic   (1000) classic   (1000)     1215 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/docs/build/index.rst
--rw-r--r--   0 classic   (1000) classic   (1000)     3077 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/docs/build/make.bat
--rw-r--r--   0 classic   (1000) classic   (1000)     9296 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/docs/build/recipes.rst
--rw-r--r--   0 classic   (1000) classic   (1000)      178 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/docs/build/requirements.txt
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-02-21 19:41:01.951502 dogpile.cache-1.3.2/docs/build/unreleased/
--rw-r--r--   0 classic   (1000) classic   (1000)      410 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/docs/build/unreleased/README.txt
--rw-r--r--   0 classic   (1000) classic   (1000)    11625 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/docs/build/usage.rst
--rw-r--r--   0 classic   (1000) classic   (1000)   141845 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/changelog.html
--rw-r--r--   0 classic   (1000) classic   (1000)    28463 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/core_usage.html
--rw-r--r--   0 classic   (1000) classic   (1000)     6486 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/front.html
--rw-r--r--   0 classic   (1000) classic   (1000)    71809 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/genindex.html
--rw-r--r--   0 classic   (1000) classic   (1000)    15419 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/index.html
--rw-r--r--   0 classic   (1000) classic   (1000)     5985 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/py-modindex.html
--rw-r--r--   0 classic   (1000) classic   (1000)    32457 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/recipes.html
--rw-r--r--   0 classic   (1000) classic   (1000)     3536 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/search.html
--rw-r--r--   0 classic   (1000) classic   (1000)    77323 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/searchindex.js
--rw-r--r--   0 classic   (1000) classic   (1000)   112814 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/docs/usage.html
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-02-21 19:41:01.940503 dogpile.cache-1.3.2/dogpile/
--rw-r--r--   0 classic   (1000) classic   (1000)      106 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/__init__.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-02-21 19:41:01.941502 dogpile.cache-1.3.2/dogpile/cache/
--rw-r--r--   0 classic   (1000) classic   (1000)      180 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/cache/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)    17864 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/cache/api.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-02-21 19:41:01.941502 dogpile.cache-1.3.2/dogpile/cache/backends/
--rw-r--r--   0 classic   (1000) classic   (1000)     1315 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/cache/backends/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)    13710 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/cache/backends/file.py
--rw-r--r--   0 classic   (1000) classic   (1000)    20887 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/cache/backends/memcached.py
--rw-r--r--   0 classic   (1000) classic   (1000)     3030 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/cache/backends/memory.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1167 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/cache/backends/null.py
--rw-r--r--   0 classic   (1000) classic   (1000)    19744 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/cache/backends/redis.py
--rw-r--r--   0 classic   (1000) classic   (1000)      601 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/cache/exception.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-02-21 19:41:01.942503 dogpile.cache-1.3.2/dogpile/cache/plugins/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/cache/plugins/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)     2964 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/cache/plugins/mako_cache.py
--rw-r--r--   0 classic   (1000) classic   (1000)     3667 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/cache/proxy.py
--rw-r--r--   0 classic   (1000) classic   (1000)    69882 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/cache/region.py
--rw-r--r--   0 classic   (1000) classic   (1000)     5416 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/cache/util.py
--rw-r--r--   0 classic   (1000) classic   (1000)      565 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/core.py
--rw-r--r--   0 classic   (1000) classic   (1000)     7077 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/lock.py
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/py.typed
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-02-21 19:41:01.942503 dogpile.cache-1.3.2/dogpile/testing/
--rw-r--r--   0 classic   (1000) classic   (1000)      221 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/testing/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)      870 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/testing/assertions.py
--rw-r--r--   0 classic   (1000) classic   (1000)    17368 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/testing/fixtures.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-02-21 19:41:01.942503 dogpile.cache-1.3.2/dogpile/util/
--rw-r--r--   0 classic   (1000) classic   (1000)      339 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/util/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1735 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/util/compat.py
--rw-r--r--   0 classic   (1000) classic   (1000)     4479 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/util/langhelpers.py
--rw-r--r--   0 classic   (1000) classic   (1000)     2801 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/util/nameregistry.py
--rw-r--r--   0 classic   (1000) classic   (1000)     4532 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/util/readwrite_lock.py
--rw-r--r--   0 classic   (1000) classic   (1000)      131 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/dogpile/util/typing.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-02-21 19:41:01.952502 dogpile.cache-1.3.2/dogpile.cache.egg-info/
--rw-r--r--   0 classic   (1000) classic   (1000)     5175 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/dogpile.cache.egg-info/PKG-INFO
--rw-r--r--   0 classic   (1000) classic   (1000)     4087 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/dogpile.cache.egg-info/SOURCES.txt
--rw-r--r--   0 classic   (1000) classic   (1000)        1 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/dogpile.cache.egg-info/dependency_links.txt
--rw-r--r--   0 classic   (1000) classic   (1000)       73 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/dogpile.cache.egg-info/entry_points.txt
--rw-r--r--   0 classic   (1000) classic   (1000)        1 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/dogpile.cache.egg-info/not-zip-safe
--rw-r--r--   0 classic   (1000) classic   (1000)      157 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/dogpile.cache.egg-info/requires.txt
--rw-r--r--   0 classic   (1000) classic   (1000)        8 2024-02-21 19:41:01.000000 dogpile.cache-1.3.2/dogpile.cache.egg-info/top_level.txt
--rw-r--r--   0 classic   (1000) classic   (1000)      838 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/hash_port.py
--rw-r--r--   0 classic   (1000) classic   (1000)      513 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/log_tests.ini
--rw-r--r--   0 classic   (1000) classic   (1000)      807 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/mypy.ini
--rw-r--r--   0 classic   (1000) classic   (1000)     1792 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/pyproject.toml
--rw-r--r--   0 classic   (1000) classic   (1000)      388 2024-02-21 19:41:01.956503 dogpile.cache-1.3.2/setup.cfg
--rw-r--r--   0 classic   (1000) classic   (1000)      558 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/setup.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-02-21 19:41:01.953503 dogpile.cache-1.3.2/tests/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/__init__.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-02-21 19:41:01.953503 dogpile.cache-1.3.2/tests/cache/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/cache/__init__.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-02-21 19:41:01.954502 dogpile.cache-1.3.2/tests/cache/plugins/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/cache/plugins/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1362 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/cache/plugins/test_mako_cache.py
--rw-r--r--   0 classic   (1000) classic   (1000)     3088 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/cache/test_dbm_backend.py
--rw-r--r--   0 classic   (1000) classic   (1000)    19037 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/cache/test_decorator.py
--rw-r--r--   0 classic   (1000) classic   (1000)    16122 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/cache/test_memcached_backend.py
--rw-r--r--   0 classic   (1000) classic   (1000)      420 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/cache/test_memory_backend.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1922 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/cache/test_null_backend.py
--rw-r--r--   0 classic   (1000) classic   (1000)     8661 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/cache/test_redis_backend.py
--rw-r--r--   0 classic   (1000) classic   (1000)     3528 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/cache/test_redis_sentinel_backend.py
--rw-r--r--   0 classic   (1000) classic   (1000)    33788 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/cache/test_region.py
--rw-r--r--   0 classic   (1000) classic   (1000)      517 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/test_backgrounding.py
--rw-r--r--   0 classic   (1000) classic   (1000)    10351 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/test_lock.py
--rw-r--r--   0 classic   (1000) classic   (1000)      819 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/test_utils.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-02-21 19:41:01.954502 dogpile.cache-1.3.2/tests/tls/
--rw-r--r--   0 classic   (1000) classic   (1000)      368 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/tls/README.rst
--rw-r--r--   0 classic   (1000) classic   (1000)     2354 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/tls/ca-root.crt
--rw-r--r--   0 classic   (1000) classic   (1000)     2354 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/tls/client-ca-root.crt
--rw-r--r--   0 classic   (1000) classic   (1000)     1692 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/tls/client.crt
--rw-r--r--   0 classic   (1000) classic   (1000)     1679 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/tls/client.key
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-02-21 19:41:01.954502 dogpile.cache-1.3.2/tests/tls/generate/
--rw-r--r--   0 classic   (1000) classic   (1000)     2892 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/tls/generate/Makefile
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-02-21 19:41:01.955502 dogpile.cache-1.3.2/tests/tls/generate/conf/
--rw-r--r--   0 classic   (1000) classic   (1000)      565 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/tls/generate/conf/ca-intermediate.conf
--rw-r--r--   0 classic   (1000) classic   (1000)      564 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/tls/generate/conf/ca-root.conf
--rw-r--r--   0 classic   (1000) classic   (1000)      564 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/tls/generate/conf/client-ca-root.conf
--rw-r--r--   0 classic   (1000) classic   (1000)      492 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/tls/generate/conf/client.conf
--rw-r--r--   0 classic   (1000) classic   (1000)      475 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/tls/generate/conf/server.conf
--rwxr-xr-x   0 classic   (1000) classic   (1000)     1567 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/tls/generate/tool
--rw-r--r--   0 classic   (1000) classic   (1000)     1675 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/tls/server.key
--rw-r--r--   0 classic   (1000) classic   (1000)     4021 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/tls/server_chain.pem
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-02-21 19:41:01.955502 dogpile.cache-1.3.2/tests/util/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/util/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1495 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tests/util/test_nameregistry.py
--rw-r--r--   0 classic   (1000) classic   (1000)     2733 2024-02-21 19:40:52.000000 dogpile.cache-1.3.2/tox.ini
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:13.733079 dogpile.cache-1.3.3/
+-rw-r--r--   0 classic   (1000) classic   (1000)      213 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/.gitignore
+-rw-r--r--   0 classic   (1000) classic   (1000)       99 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/.gitreview
+-rw-r--r--   0 classic   (1000) classic   (1000)      882 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 classic   (1000) classic   (1000)     1059 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/LICENSE
+-rw-r--r--   0 classic   (1000) classic   (1000)      239 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/MANIFEST.in
+-rw-r--r--   0 classic   (1000) classic   (1000)     5175 2024-05-05 16:53:13.733079 dogpile.cache-1.3.3/PKG-INFO
+-rw-r--r--   0 classic   (1000) classic   (1000)     4176 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/README.rst
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:13.723079 dogpile.cache-1.3.3/docs/
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:13.725078 dogpile.cache-1.3.3/docs/_sources/
+-rw-r--r--   0 classic   (1000) classic   (1000)     1587 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/_sources/api.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    42644 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/_sources/changelog.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    10222 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/_sources/core_usage.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)      769 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/_sources/front.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)     1215 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/_sources/index.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)     9296 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/_sources/recipes.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    11625 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/_sources/usage.rst.txt
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:13.728078 dogpile.cache-1.3.3/docs/_static/
+-rw-r--r--   0 classic   (1000) classic   (1000)    15094 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/_static/basic.css
+-rw-r--r--   0 classic   (1000) classic   (1000)      107 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/_static/changelog.css
+-rw-r--r--   0 classic   (1000) classic   (1000)     4472 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/_static/doctools.js
+-rw-r--r--   0 classic   (1000) classic   (1000)      328 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/_static/documentation_options.js
+-rw-r--r--   0 classic   (1000) classic   (1000)      286 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/_static/file.png
+-rw-r--r--   0 classic   (1000) classic   (1000)     4758 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/_static/language_data.js
+-rw-r--r--   0 classic   (1000) classic   (1000)       90 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/_static/minus.png
+-rw-r--r--   0 classic   (1000) classic   (1000)     4243 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/_static/nature.css
+-rw-r--r--   0 classic   (1000) classic   (1000)      507 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/_static/nature_override.css
+-rw-r--r--   0 classic   (1000) classic   (1000)       90 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/_static/plus.png
+-rw-r--r--   0 classic   (1000) classic   (1000)     4929 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/_static/pygments.css
+-rw-r--r--   0 classic   (1000) classic   (1000)    20731 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/_static/searchtools.js
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/_static/site_custom_css.css
+-rw-r--r--   0 classic   (1000) classic   (1000)     5123 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/_static/sphinx_highlight.js
+-rw-r--r--   0 classic   (1000) classic   (1000)      204 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/_static/sphinx_paramlinks.css
+-rw-r--r--   0 classic   (1000) classic   (1000)   504826 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/api.html
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:13.729079 dogpile.cache-1.3.3/docs/build/
+-rw-r--r--   0 classic   (1000) classic   (1000)     3373 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/docs/build/Makefile
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:13.729079 dogpile.cache-1.3.3/docs/build/_static/
+-rw-r--r--   0 classic   (1000) classic   (1000)      507 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/docs/build/_static/nature_override.css
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/docs/build/_static/site_custom_css.css
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:13.729079 dogpile.cache-1.3.3/docs/build/_templates/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/docs/build/_templates/site_custom_sidebars.html
+-rw-r--r--   0 classic   (1000) classic   (1000)     1587 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/docs/build/api.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)      266 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/docs/build/builder.py
+-rw-------   0 classic   (1000) classic   (1000)    42644 2024-05-05 16:53:11.000000 dogpile.cache-1.3.3/docs/build/changelog.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     7408 2024-05-05 16:53:11.000000 dogpile.cache-1.3.3/docs/build/conf.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    10222 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/docs/build/core_usage.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)      769 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/docs/build/front.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     1215 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/docs/build/index.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     3077 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/docs/build/make.bat
+-rw-r--r--   0 classic   (1000) classic   (1000)     9296 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/docs/build/recipes.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)      178 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/docs/build/requirements.txt
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:13.729079 dogpile.cache-1.3.3/docs/build/unreleased/
+-rw-r--r--   0 classic   (1000) classic   (1000)      410 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/docs/build/unreleased/README.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    11625 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/docs/build/usage.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)   144974 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/changelog.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    28469 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/core_usage.html
+-rw-r--r--   0 classic   (1000) classic   (1000)     6492 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/front.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    71803 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/genindex.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    15528 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/index.html
+-rw-r--r--   0 classic   (1000) classic   (1000)     5991 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/py-modindex.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    32463 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/recipes.html
+-rw-r--r--   0 classic   (1000) classic   (1000)     3584 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/search.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    78849 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/searchindex.js
+-rw-r--r--   0 classic   (1000) classic   (1000)   113287 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/docs/usage.html
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:13.717079 dogpile.cache-1.3.3/dogpile/
+-rw-r--r--   0 classic   (1000) classic   (1000)      106 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/__init__.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:13.718078 dogpile.cache-1.3.3/dogpile/cache/
+-rw-r--r--   0 classic   (1000) classic   (1000)      180 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/cache/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    18029 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/cache/api.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:13.718078 dogpile.cache-1.3.3/dogpile/cache/backends/
+-rw-r--r--   0 classic   (1000) classic   (1000)     1315 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/cache/backends/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    13710 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/cache/backends/file.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    21552 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/cache/backends/memcached.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     3030 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/cache/backends/memory.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1167 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/cache/backends/null.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    19744 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/cache/backends/redis.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      601 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/cache/exception.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:13.718078 dogpile.cache-1.3.3/dogpile/cache/plugins/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/cache/plugins/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     2964 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/cache/plugins/mako_cache.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     3667 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/cache/proxy.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    69988 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/cache/region.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     5416 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/cache/util.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      565 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/core.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     7077 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/lock.py
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/py.typed
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:13.719079 dogpile.cache-1.3.3/dogpile/testing/
+-rw-r--r--   0 classic   (1000) classic   (1000)      221 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/testing/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      870 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/testing/assertions.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    17368 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/testing/fixtures.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:13.719079 dogpile.cache-1.3.3/dogpile/util/
+-rw-r--r--   0 classic   (1000) classic   (1000)      339 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/util/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1735 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/util/compat.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     4479 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/util/langhelpers.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     2801 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/util/nameregistry.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     4532 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/util/readwrite_lock.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      131 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/dogpile/util/typing.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:13.729079 dogpile.cache-1.3.3/dogpile.cache.egg-info/
+-rw-r--r--   0 classic   (1000) classic   (1000)     5175 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/dogpile.cache.egg-info/PKG-INFO
+-rw-r--r--   0 classic   (1000) classic   (1000)     4087 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/dogpile.cache.egg-info/SOURCES.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)        1 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/dogpile.cache.egg-info/dependency_links.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)       73 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/dogpile.cache.egg-info/entry_points.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)        1 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/dogpile.cache.egg-info/not-zip-safe
+-rw-r--r--   0 classic   (1000) classic   (1000)      157 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/dogpile.cache.egg-info/requires.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)        8 2024-05-05 16:53:13.000000 dogpile.cache-1.3.3/dogpile.cache.egg-info/top_level.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)      838 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/hash_port.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      513 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/log_tests.ini
+-rw-r--r--   0 classic   (1000) classic   (1000)      807 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/mypy.ini
+-rw-r--r--   0 classic   (1000) classic   (1000)     1792 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/pyproject.toml
+-rw-r--r--   0 classic   (1000) classic   (1000)      392 2024-05-05 16:53:13.733079 dogpile.cache-1.3.3/setup.cfg
+-rw-r--r--   0 classic   (1000) classic   (1000)      558 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/setup.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:13.730079 dogpile.cache-1.3.3/tests/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/__init__.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:13.731078 dogpile.cache-1.3.3/tests/cache/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/cache/__init__.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:13.731078 dogpile.cache-1.3.3/tests/cache/plugins/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/cache/plugins/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1362 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/cache/plugins/test_mako_cache.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     3088 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/cache/test_dbm_backend.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    19037 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/cache/test_decorator.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    16532 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/cache/test_memcached_backend.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      420 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/cache/test_memory_backend.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1922 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/cache/test_null_backend.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     8661 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/cache/test_redis_backend.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     3528 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/cache/test_redis_sentinel_backend.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    33770 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/cache/test_region.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      517 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/test_backgrounding.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    10351 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/test_lock.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      819 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/test_utils.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:13.731078 dogpile.cache-1.3.3/tests/tls/
+-rw-r--r--   0 classic   (1000) classic   (1000)      368 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/tls/README.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     2354 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/tls/ca-root.crt
+-rw-r--r--   0 classic   (1000) classic   (1000)     2354 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/tls/client-ca-root.crt
+-rw-r--r--   0 classic   (1000) classic   (1000)     1692 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/tls/client.crt
+-rw-r--r--   0 classic   (1000) classic   (1000)     1679 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/tls/client.key
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:13.732078 dogpile.cache-1.3.3/tests/tls/generate/
+-rw-r--r--   0 classic   (1000) classic   (1000)     2892 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/tls/generate/Makefile
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:13.732078 dogpile.cache-1.3.3/tests/tls/generate/conf/
+-rw-r--r--   0 classic   (1000) classic   (1000)      565 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/tls/generate/conf/ca-intermediate.conf
+-rw-r--r--   0 classic   (1000) classic   (1000)      564 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/tls/generate/conf/ca-root.conf
+-rw-r--r--   0 classic   (1000) classic   (1000)      564 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/tls/generate/conf/client-ca-root.conf
+-rw-r--r--   0 classic   (1000) classic   (1000)      492 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/tls/generate/conf/client.conf
+-rw-r--r--   0 classic   (1000) classic   (1000)      475 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/tls/generate/conf/server.conf
+-rwxr-xr-x   0 classic   (1000) classic   (1000)     1567 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/tls/generate/tool
+-rw-r--r--   0 classic   (1000) classic   (1000)     1675 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/tls/server.key
+-rw-r--r--   0 classic   (1000) classic   (1000)     4021 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/tls/server_chain.pem
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:13.732078 dogpile.cache-1.3.3/tests/util/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/util/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1495 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tests/util/test_nameregistry.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     2733 2024-05-05 16:53:04.000000 dogpile.cache-1.3.3/tox.ini
```

### Comparing `dogpile.cache-1.3.2/.pre-commit-config.yaml` & `dogpile.cache-1.3.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/LICENSE` & `dogpile.cache-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/PKG-INFO` & `dogpile.cache-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dogpile.cache
-Version: 1.3.2
+Version: 1.3.3
 Summary: A caching front-end based on the Dogpile lock.
 Author-email: Mike Bayer <mike_mp@zzzcomputing.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sqlalchemy/dogpile.cache
 Project-URL: Documentation, https://dogpilecache.sqlalchemy.org
 Project-URL: Issue Tracker, https://github.com/sqlalchemy/dogpile.cache/
 Keywords: caching
```

### Comparing `dogpile.cache-1.3.2/README.rst` & `dogpile.cache-1.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/docs/_sources/api.rst.txt` & `dogpile.cache-1.3.3/docs/_sources/api.rst.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/docs/_sources/changelog.rst.txt` & `dogpile.cache-1.3.3/docs/_sources/changelog.rst.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,33 @@
 =========
 Changelog
 =========
 
 .. changelog::
+    :version: 1.3.3
+    :released: Sun May 5 2024
+
+    .. change::
+        :tags: bug, typing
+
+        Fixed the return type for :meth:`.CacheRegion.get`, which was inadvertently
+        hardcoded to use ``CacheReturnType`` that only resolved to ``CachedValue``
+        or ``NoValue``.   Fixed to return ``ValuePayload`` which resolves to
+        ``Any``, as well as a new literal indicating an enum constant for
+        :data:`.api.NO_VALUE`.  The :data:`.api.NO_VALUE` constant remains
+        available as the single element of this enum.
+
+    .. change::
+        :tags: usecase, memcached
+
+        Added support for an additional pymemcached client parameter
+        :paramref:`.PyMemcacheBackend.memcached_expire_time`.  Pull request
+        courtesy Takashi Kajinami.
+
+.. changelog::
     :version: 1.3.2
     :released: Wed Feb 21 2024
 
     .. change::
         :tags: usecase, redis
         :tickets: 250
```

### Comparing `dogpile.cache-1.3.2/docs/_sources/core_usage.rst.txt` & `dogpile.cache-1.3.3/docs/_sources/core_usage.rst.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/docs/_sources/front.rst.txt` & `dogpile.cache-1.3.3/docs/_sources/front.rst.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/docs/_sources/index.rst.txt` & `dogpile.cache-1.3.3/docs/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/docs/_sources/recipes.rst.txt` & `dogpile.cache-1.3.3/docs/_sources/recipes.rst.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/docs/_sources/usage.rst.txt` & `dogpile.cache-1.3.3/docs/_sources/usage.rst.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/docs/_static/basic.css` & `dogpile.cache-1.3.3/docs/_static/basic.css`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 /*
  * basic.css
  * ~~~~~~~~~
  *
  * Sphinx stylesheet -- basic theme.
  *
- * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2024 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 /* -- main layout ----------------------------------------------------------- */
 
 div.clearer {
```

### Comparing `dogpile.cache-1.3.2/docs/_static/doctools.js` & `dogpile.cache-1.3.3/docs/_static/doctools.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 /*
  * doctools.js
  * ~~~~~~~~~~~
  *
  * Base JavaScript utilities for all Sphinx HTML documentation.
  *
- * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2024 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 "use strict";
 
 const BLACKLISTED_KEY_CONTROL_ELEMENTS = new Set([
     "TEXTAREA",
```

### Comparing `dogpile.cache-1.3.2/docs/_static/language_data.js` & `dogpile.cache-1.3.3/docs/_static/language_data.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,23 +1,23 @@
 /*
  * language_data.js
  * ~~~~~~~~~~~~~~~~
  *
  * This script contains the language-specific data used by searchtools.js,
  * namely the list of stopwords, stemmer, scorer and splitter.
  *
- * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2024 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 var stopwords = ["a", "and", "are", "as", "at", "be", "but", "by", "for", "if", "in", "into", "is", "it", "near", "no", "not", "of", "on", "or", "such", "that", "the", "their", "then", "there", "these", "they", "this", "to", "was", "will", "with"];
 
 
-/* Non-minified version is copied as a separate JS file, is available */
+/* Non-minified version is copied as a separate JS file, if available */
 
 /**
  * Porter Stemmer
  */
 var Stemmer = function() {
 
     var step2list = {
```

### Comparing `dogpile.cache-1.3.2/docs/_static/nature.css` & `dogpile.cache-1.3.3/docs/_static/nature.css`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 /*
  * nature.css_t
  * ~~~~~~~~~~~~
  *
  * Sphinx stylesheet -- nature theme.
  *
- * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2024 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 
 @import url("basic.css");
 
 /* -- page layout ----------------------------------------------------------- */
```

### Comparing `dogpile.cache-1.3.2/docs/_static/pygments.css` & `dogpile.cache-1.3.3/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/docs/_static/searchtools.js` & `dogpile.cache-1.3.3/docs/_static/searchtools.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 /*
  * searchtools.js
  * ~~~~~~~~~~~~~~~~
  *
  * Sphinx JavaScript utilities for the full-text search.
  *
- * :copyright: Copyright 2007-2023 by the Sphinx team, see AUTHORS.
+ * :copyright: Copyright 2007-2024 by the Sphinx team, see AUTHORS.
  * :license: BSD, see LICENSE for details.
  *
  */
 "use strict";
 
 /**
  * Simple result scoring code.
@@ -94,15 +94,15 @@
             highlightTerms.forEach((term) => _highlightText(listItem, term, "highlighted"));
     } else if (showSearchSummary)
         fetch(requestUrl)
         .then((responseData) => responseData.text())
         .then((data) => {
             if (data)
                 listItem.appendChild(
-                    Search.makeSearchSummary(data, searchTerms)
+                    Search.makeSearchSummary(data, searchTerms, anchor)
                 );
             // highlight search terms in the summary
             if (SPHINX_HIGHLIGHT_ENABLED) // set in sphinx_highlight.js
                 highlightTerms.forEach((term) => _highlightText(listItem, term, "highlighted"));
         });
     Search.output.appendChild(listItem);
 };
@@ -111,16 +111,16 @@
     Search.title.innerText = _("Search Results");
     if (!resultCount)
         Search.status.innerText = Documentation.gettext(
             "Your search did not match any documents. Please make sure that all words are spelled correctly and that you've selected enough categories."
         );
     else
         Search.status.innerText = _(
-            `Search finished, found ${resultCount} page(s) matching the search query.`
-        );
+            "Search finished, found ${resultCount} page(s) matching the search query."
+        ).replace('${resultCount}', resultCount);
 };
 const _displayNextItem = (
     results,
     resultCount,
     searchTerms,
     highlightTerms,
 ) => {
@@ -132,14 +132,30 @@
             () => _displayNextItem(results, resultCount, searchTerms, highlightTerms),
             5
         );
     }
     // search finished, update title and status message
     else _finishSearch(resultCount);
 };
+// Helper function used by query() to order search results.
+// Each input is an array of [docname, title, anchor, descr, score, filename].
+// Order the results by score (in opposite order of appearance, since the
+// `_displayNextItem` function uses pop() to retrieve items) and then alphabetically.
+const _orderResultsByScoreThenName = (a, b) => {
+    const leftScore = a[4];
+    const rightScore = b[4];
+    if (leftScore === rightScore) {
+        // same score: sort alphabetically
+        const leftTitle = a[1].toLowerCase();
+        const rightTitle = b[1].toLowerCase();
+        if (leftTitle === rightTitle) return 0;
+        return leftTitle > rightTitle ? -1 : 1; // inverted is intentional
+    }
+    return leftScore > rightScore ? 1 : -1;
+};
 
 /**
  * Default splitQuery function. Can be overridden in ``sphinx.search`` with a
  * custom function per language.
  *
  * The regular expression works by splitting the string on consecutive characters
  * that are not Unicode letters, numbers, underscores, or emoji characters.
@@ -155,23 +171,36 @@
  * Search Module
  */
 const Search = {
     _index: null,
     _queued_query: null,
     _pulse_status: -1,
 
-    htmlToText: (htmlString) => {
+    htmlToText: (htmlString, anchor) => {
         const htmlElement = new DOMParser().parseFromString(htmlString, 'text/html');
-        htmlElement.querySelectorAll(".headerlink").forEach((el) => {
-            el.remove()
-        });
+        for (const removalQuery of [".headerlinks", "script", "style"]) {
+            htmlElement.querySelectorAll(removalQuery).forEach((el) => {
+                el.remove()
+            });
+        }
+        if (anchor) {
+            const anchorContent = htmlElement.querySelector(`[role="main"] ${anchor}`);
+            if (anchorContent) return anchorContent.textContent;
+
+            console.warn(
+                `Anchored content block not found. Sphinx search tries to obtain it via DOM query '[role=main] ${anchor}'. Check your theme or template.`
+            );
+        }
+
+        // if anchor not specified or not found, fall back to main content
         const docContent = htmlElement.querySelector('[role="main"]');
-        if (docContent !== undefined) return docContent.textContent;
+        if (docContent) return docContent.textContent;
+
         console.warn(
-            "Content block not found. Sphinx search tries to obtain it via '[role=main]'. Could you check your theme or template."
+            "Content block not found. Sphinx search tries to obtain it via DOM query '[role=main]'. Check your theme or template."
         );
         return "";
     },
 
     init: () => {
         const query = new URLSearchParams(window.location.search).get("q");
         document
@@ -236,24 +265,15 @@
         Search.startPulse();
 
         // index already loaded, the browser was quick!
         if (Search.hasIndex()) Search.query(query);
         else Search.deferQuery(query);
     },
 
-    /**
-     * execute search (requires search index to be loaded)
-     */
-    query: (query) => {
-        const filenames = Search._index.filenames;
-        const docNames = Search._index.docnames;
-        const titles = Search._index.titles;
-        const allTitles = Search._index.alltitles;
-        const indexEntries = Search._index.indexentries;
-
+    _parseQuery: (query) => {
         // stem the search terms and add them to the correct list
         const stemmer = new Stemmer();
         const searchTerms = new Set();
         const excludedTerms = new Set();
         const highlightTerms = new Set();
         const objectTerms = new Set(splitQuery(query.toLowerCase().trim()));
         splitQuery(query.trim()).forEach((queryTerm) => {
@@ -281,92 +301,114 @@
             localStorage.setItem("sphinx_highlight_terms", [...highlightTerms].join(" "))
         }
 
         // console.debug("SEARCH: searching for:");
         // console.info("required: ", [...searchTerms]);
         // console.info("excluded: ", [...excludedTerms]);
 
-        // array of [docname, title, anchor, descr, score, filename]
-        let results = [];
+        return [query, searchTerms, excludedTerms, highlightTerms, objectTerms];
+    },
+
+    /**
+     * execute search (requires search index to be loaded)
+     */
+    _performSearch: (query, searchTerms, excludedTerms, highlightTerms, objectTerms) => {
+        const filenames = Search._index.filenames;
+        const docNames = Search._index.docnames;
+        const titles = Search._index.titles;
+        const allTitles = Search._index.alltitles;
+        const indexEntries = Search._index.indexentries;
+
+        // Collect multiple result groups to be sorted separately and then ordered.
+        // Each is an array of [docname, title, anchor, descr, score, filename].
+        const normalResults = [];
+        const nonMainIndexResults = [];
+
         _removeChildren(document.getElementById("search-progress"));
 
-        const queryLower = query.toLowerCase();
+        const queryLower = query.toLowerCase().trim();
         for (const [title, foundTitles] of Object.entries(allTitles)) {
-            if (title.toLowerCase().includes(queryLower) && (queryLower.length >= title.length / 2)) {
+            if (title.toLowerCase().trim().includes(queryLower) && (queryLower.length >= title.length / 2)) {
                 for (const [file, id] of foundTitles) {
                     let score = Math.round(100 * queryLower.length / title.length)
-                    results.push([
+                    normalResults.push([
                         docNames[file],
                         titles[file] !== title ? `${titles[file]} > ${title}` : title,
                         id !== null ? "#" + id : "",
                         null,
                         score,
                         filenames[file],
                     ]);
                 }
             }
         }
 
         // search for explicit entries in index directives
         for (const [entry, foundEntries] of Object.entries(indexEntries)) {
             if (entry.includes(queryLower) && (queryLower.length >= entry.length / 2)) {
-                for (const [file, id] of foundEntries) {
-                    let score = Math.round(100 * queryLower.length / entry.length)
-                    results.push([
+                for (const [file, id, isMain] of foundEntries) {
+                    const score = Math.round(100 * queryLower.length / entry.length);
+                    const result = [
                         docNames[file],
                         titles[file],
                         id ? "#" + id : "",
                         null,
                         score,
                         filenames[file],
-                    ]);
+                    ];
+                    if (isMain) {
+                        normalResults.push(result);
+                    } else {
+                        nonMainIndexResults.push(result);
+                    }
                 }
             }
         }
 
         // lookup as object
         objectTerms.forEach((term) =>
-            results.push(...Search.performObjectSearch(term, objectTerms))
+            normalResults.push(...Search.performObjectSearch(term, objectTerms))
         );
 
         // lookup as search terms in fulltext
-        results.push(...Search.performTermsSearch(searchTerms, excludedTerms));
+        normalResults.push(...Search.performTermsSearch(searchTerms, excludedTerms));
 
         // let the scorer override scores with a custom scoring function
-        if (Scorer.score) results.forEach((item) => (item[4] = Scorer.score(item)));
+        if (Scorer.score) {
+            normalResults.forEach((item) => (item[4] = Scorer.score(item)));
+            nonMainIndexResults.forEach((item) => (item[4] = Scorer.score(item)));
+        }
 
-        // now sort the results by score (in opposite order of appearance, since the
-        // display function below uses pop() to retrieve items) and then
-        // alphabetically
-        results.sort((a, b) => {
-            const leftScore = a[4];
-            const rightScore = b[4];
-            if (leftScore === rightScore) {
-                // same score: sort alphabetically
-                const leftTitle = a[1].toLowerCase();
-                const rightTitle = b[1].toLowerCase();
-                if (leftTitle === rightTitle) return 0;
-                return leftTitle > rightTitle ? -1 : 1; // inverted is intentional
-            }
-            return leftScore > rightScore ? 1 : -1;
-        });
+        // Sort each group of results by score and then alphabetically by name.
+        normalResults.sort(_orderResultsByScoreThenName);
+        nonMainIndexResults.sort(_orderResultsByScoreThenName);
+
+        // Combine the result groups in (reverse) order.
+        // Non-main index entries are typically arbitrary cross-references,
+        // so display them after other results.
+        let results = [...nonMainIndexResults, ...normalResults];
 
         // remove duplicate search results
         // note the reversing of results, so that in the case of duplicates, the highest-scoring entry is kept
         let seen = new Set();
         results = results.reverse().reduce((acc, result) => {
             let resultStr = result.slice(0, 4).concat([result[5]]).map(v => String(v)).join(',');
             if (!seen.has(resultStr)) {
                 acc.push(result);
                 seen.add(resultStr);
             }
             return acc;
         }, []);
 
-        results = results.reverse();
+        return results.reverse();
+    },
+
+    query: (query) => {
+        const [searchQuery, searchTerms, excludedTerms, highlightTerms, objectTerms] = Search._parseQuery(query);
+        const results = Search._performSearch(searchQuery, searchTerms, excludedTerms, highlightTerms, objectTerms);
 
         // for debugging
         //Search.lastresults = results.slice();  // a copy
         // console.info("search results:", Search.lastresults);
 
         // print the results
         _displayNextItem(results, results.length, searchTerms, highlightTerms);
@@ -466,28 +508,32 @@
             }, {
                 files: titleTerms[word],
                 score: Scorer.title
             }, ];
             // add support for partial matches
             if (word.length > 2) {
                 const escapedWord = _escapeRegExp(word);
-                Object.keys(terms).forEach((term) => {
-                    if (term.match(escapedWord) && !terms[word])
-                        arr.push({
-                            files: terms[term],
-                            score: Scorer.partialTerm
-                        });
-                });
-                Object.keys(titleTerms).forEach((term) => {
-                    if (term.match(escapedWord) && !titleTerms[word])
-                        arr.push({
-                            files: titleTerms[word],
-                            score: Scorer.partialTitle
-                        });
-                });
+                if (!terms.hasOwnProperty(word)) {
+                    Object.keys(terms).forEach((term) => {
+                        if (term.match(escapedWord))
+                            arr.push({
+                                files: terms[term],
+                                score: Scorer.partialTerm
+                            });
+                    });
+                }
+                if (!titleTerms.hasOwnProperty(word)) {
+                    Object.keys(titleTerms).forEach((term) => {
+                        if (term.match(escapedWord))
+                            arr.push({
+                                files: titleTerms[term],
+                                score: Scorer.partialTitle
+                            });
+                    });
+                }
             }
 
             // no match but word was a required one
             if (arr.every((record) => record.files === undefined)) return;
 
             // found search word in contents
             arr.forEach((record) => {
@@ -502,17 +548,16 @@
                     if (!scoreMap.has(file)) scoreMap.set(file, {});
                     scoreMap.get(file)[word] = record.score;
                 });
             });
 
             // create the mapping
             files.forEach((file) => {
-                if (fileMap.has(file) && fileMap.get(file).indexOf(word) === -1)
-                    fileMap.get(file).push(word);
-                else fileMap.set(file, [word]);
+                if (!fileMap.has(file)) fileMap.set(file, [word]);
+                else if (fileMap.get(file).indexOf(word) === -1) fileMap.get(file).push(word);
             });
         });
 
         // now check if the files don't contain excluded terms
         const results = [];
         for (const [file, wordList] of fileMap) {
             // check if all requirements are matched
@@ -555,16 +600,16 @@
     },
 
     /**
      * helper function to return a node containing the
      * search summary for a given text. keywords is a list
      * of stemmed words.
      */
-    makeSearchSummary: (htmlText, keywords) => {
-        const text = Search.htmlToText(htmlText);
+    makeSearchSummary: (htmlText, keywords, anchor) => {
+        const text = Search.htmlToText(htmlText, anchor);
         if (text === "") return null;
 
         const textLower = text.toLowerCase();
         const actualStartPosition = [...keywords]
             .map((k) => textLower.indexOf(k.toLowerCase()))
             .filter((i) => i > -1)
             .slice(-1)[0];
```

### Comparing `dogpile.cache-1.3.2/docs/_static/sphinx_highlight.js` & `dogpile.cache-1.3.3/docs/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/docs/api.html` & `dogpile.cache-1.3.3/docs/api.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>API &#8212; dogpile.cache 1.3.2 documentation</title>
+    <title>API &#8212; dogpile.cache 1.3.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css?v=d00006d9" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
-    <script src="_static/documentation_options.js?v=8ca9e7a0"></script>
-    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/documentation_options.js?v=28d163b9"></script>
+    <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Changelog" href="changelog.html" />
     <link rel="prev" title="dogpile Core" href="core_usage.html" /> 
   </head><body>
     <div class="related" role="navigation" aria-label="related navigation">
@@ -29,15 +29,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog.html" title="Changelog"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="core_usage.html" title="dogpile Core"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">API</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -139,32 +139,32 @@
 needed when using a backend such as bsddb or dbm under Python 2.x
 in conjunction with Unicode keys.</p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.params.serializer"></span><strong>serializer</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.params.serializer">¶</a> – <p>function which will be applied to all values before
 passing to the backend.  Defaults to <code class="docutils literal notranslate"><span class="pre">None</span></code>, in which case the
 serializer recommended by the backend will be used.   Typical
 serializers include <code class="docutils literal notranslate"><span class="pre">pickle.dumps</span></code> and <code class="docutils literal notranslate"><span class="pre">json.dumps</span></code>.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.0.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.0.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.params.deserializer"></span><strong>deserializer</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.params.deserializer">¶</a> – <p>function which will be applied to all values returned
 by the backend.  Defaults to <code class="docutils literal notranslate"><span class="pre">None</span></code>, in which case the
 deserializer recommended by the backend will be used.   Typical
 deserializers include <code class="docutils literal notranslate"><span class="pre">pickle.dumps</span></code> and <code class="docutils literal notranslate"><span class="pre">json.dumps</span></code>.</p>
 <p>Deserializers can raise a <a class="reference internal" href="#dogpile.cache.api.CantDeserializeException" title="dogpile.cache.api.CantDeserializeException"><code class="xref py py-class docutils literal notranslate"><span class="pre">api.CantDeserializeException</span></code></a> if they
 are unable to deserialize the value from the backend, indicating
 deserialization failed and that caching should proceed to re-generate
 a value.  This allows an application that has been updated to gracefully
 re-cache old items which were persisted by a previous version of the
 application and can no longer be successfully deserialized.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.0: </span>added “deserializer” parameter</p>
+<p><span class="versionmodified added">Added in version 1.1.0: </span>added “deserializer” parameter</p>
 </div>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.2.0: </span>added support for
+<p><span class="versionmodified added">Added in version 1.2.0: </span>added support for
 <a class="reference internal" href="#dogpile.cache.api.CantDeserializeException" title="dogpile.cache.api.CantDeserializeException"><code class="xref py py-class docutils literal notranslate"><span class="pre">api.CantDeserializeException</span></code></a></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.params.async_creation_runner"></span><strong>async_creation_runner</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.params.async_creation_runner">¶</a> – <p>A callable that, when specified,
 will be passed to and called by dogpile.lock when
 there is a stale value present in the cache.  It will be passed the
 mutex and is responsible releasing that mutex when finished.
@@ -206,29 +206,29 @@
 However, subsequent requests for cached-but-expired values will
 still return promptly.  They will be refreshed by whatever
 asynchronous means the provided async_creation_runner callable
 implements.</p>
 <p>By default the async_creation_runner is disabled and is set
 to <code class="docutils literal notranslate"><span class="pre">None</span></code>.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.4.2: </span>added the async_creation_runner
+<p><span class="versionmodified added">Added in version 0.4.2: </span>added the async_creation_runner
 feature.</p>
 </div>
 </p></li>
 </ul>
 </dd>
 </dl>
 <dl class="py property">
 <dt class="sig sig-object py" id="dogpile.cache.region.CacheRegion.actual_backend">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">actual_backend</span></span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.actual_backend" title="Link to this definition">¶</a></dt>
 <dd><p>Return the ultimate backend underneath any proxies.</p>
 <p>The backend might be the result of one or more <code class="docutils literal notranslate"><span class="pre">proxy.wrap</span></code>
 applications. If so, derive the actual underlying backend.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.6.6.</span></p>
+<p><span class="versionmodified added">Added in version 0.6.6.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.CacheRegion.cache_multi_on_arguments">
 <span class="sig-name descname"><span class="pre">cache_multi_on_arguments</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="pre">namespace:</span> <span class="pre">str</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">expiration_time:</span> <span class="pre">float</span> <span class="pre">|</span> <span class="pre">~typing.Callable[[],</span> <span class="pre">float]</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">should_cache_fn:</span> <span class="pre">~typing.Callable[[~typing.Any],</span> <span class="pre">bool]</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None,</span> <span class="pre">asdict:</span> <span class="pre">bool</span> <span class="pre">=</span> <span class="pre">False,</span> <span class="pre">to_str:</span> <span class="pre">~typing.Callable[[~typing.Any],</span> <span class="pre">str]</span> <span class="pre">=</span> <span class="pre">&lt;class</span> <span class="pre">'str'&gt;,</span> <span class="pre">function_multi_key_generator:</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">~typing.Callable[[...],</span> <span class="pre">~typing.Sequence[str]]]</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None</span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.cache_multi_on_arguments" title="Link to this definition">¶</a></dt>
 <dd><p>A function decorator that will cache multiple return
@@ -288,15 +288,15 @@
 </div>
 <p>…and a <code class="docutils literal notranslate"><span class="pre">get()</span></code> method, which will return values
 based on the given arguments:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">values</span> <span class="o">=</span> <span class="n">generate_something</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;k1&quot;</span><span class="p">,</span> <span class="s2">&quot;k2&quot;</span><span class="p">,</span> <span class="s2">&quot;k3&quot;</span><span class="p">)</span>
 </pre></div>
 </div>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.3: </span>Added <code class="docutils literal notranslate"><span class="pre">get()</span></code> method to decorated
+<p><span class="versionmodified added">Added in version 0.5.3: </span>Added <code class="docutils literal notranslate"><span class="pre">get()</span></code> method to decorated
 function.</p>
 </div>
 <p>Parameters passed to <a class="reference internal" href="#dogpile.cache.region.CacheRegion.cache_multi_on_arguments" title="dogpile.cache.region.CacheRegion.cache_multi_on_arguments"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.cache_multi_on_arguments()</span></code></a>
 have the same meaning as those passed to
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.cache_on_arguments" title="dogpile.cache.region.CacheRegion.cache_on_arguments"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.cache_on_arguments()</span></code></a>.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
@@ -325,23 +325,23 @@
 <code class="docutils literal notranslate"><span class="pre">unicode()</span></code> builtin can be substituted, but note this will
 produce unicode cache keys which may require key mangling before
 reaching the cache.</p></li>
 </ul>
 </dd>
 </dl>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.0.</span></p>
 </div>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.region.CacheRegion.cache_multi_on_arguments.params.function_multi_key_generator"></span><strong>function_multi_key_generator</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.cache_multi_on_arguments.params.function_multi_key_generator">¶</a> – <p>a function that will produce a
 list of keys. This function will supersede the one configured on the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a> itself.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.5.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.5.</span></p>
 </div>
 </p>
 </dd>
 </dl>
 <div class="admonition seealso">
 <p class="admonition-title">See also</p>
 <p><a class="reference internal" href="#dogpile.cache.region.CacheRegion.cache_on_arguments" title="dogpile.cache.region.CacheRegion.cache_on_arguments"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.cache_on_arguments()</span></code></a></p>
@@ -388,43 +388,43 @@
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">generate_something</span><span class="o">.</span><span class="n">set</span><span class="p">(</span><span class="mi">3</span><span class="p">,</span> <span class="mi">5</span><span class="p">,</span> <span class="mi">6</span><span class="p">)</span>
 </pre></div>
 </div>
 <p>The above example is equivalent to calling
 <code class="docutils literal notranslate"><span class="pre">generate_something(5,</span> <span class="pre">6)</span></code>, if the function were to produce
 the value <code class="docutils literal notranslate"><span class="pre">3</span></code> as the value to be cached.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.4.1: </span>Added <code class="docutils literal notranslate"><span class="pre">set()</span></code> method to decorated function.</p>
+<p><span class="versionmodified added">Added in version 0.4.1: </span>Added <code class="docutils literal notranslate"><span class="pre">set()</span></code> method to decorated function.</p>
 </div>
 <p>Similar to <code class="docutils literal notranslate"><span class="pre">set()</span></code> is <code class="docutils literal notranslate"><span class="pre">refresh()</span></code>.   This attribute will
 invoke the decorated function and populate a new value into
 the cache with the new value, as well as returning that value:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">newvalue</span> <span class="o">=</span> <span class="n">generate_something</span><span class="o">.</span><span class="n">refresh</span><span class="p">(</span><span class="mi">5</span><span class="p">,</span> <span class="mi">6</span><span class="p">)</span>
 </pre></div>
 </div>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0: </span>Added <code class="docutils literal notranslate"><span class="pre">refresh()</span></code> method to decorated
+<p><span class="versionmodified added">Added in version 0.5.0: </span>Added <code class="docutils literal notranslate"><span class="pre">refresh()</span></code> method to decorated
 function.</p>
 </div>
 <p><code class="docutils literal notranslate"><span class="pre">original()</span></code> on other hand will invoke the decorated function
 without any caching:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">newvalue</span> <span class="o">=</span> <span class="n">generate_something</span><span class="o">.</span><span class="n">original</span><span class="p">(</span><span class="mi">5</span><span class="p">,</span> <span class="mi">6</span><span class="p">)</span>
 </pre></div>
 </div>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.6.0: </span>Added <code class="docutils literal notranslate"><span class="pre">original()</span></code> method to decorated
+<p><span class="versionmodified added">Added in version 0.6.0: </span>Added <code class="docutils literal notranslate"><span class="pre">original()</span></code> method to decorated
 function.</p>
 </div>
 <p>Lastly, the <code class="docutils literal notranslate"><span class="pre">get()</span></code> method returns either the value cached
 for the given key, or the token <code class="docutils literal notranslate"><span class="pre">NO_VALUE</span></code> if no such key
 exists:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">value</span> <span class="o">=</span> <span class="n">generate_something</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="mi">5</span><span class="p">,</span> <span class="mi">6</span><span class="p">)</span>
 </pre></div>
 </div>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.3: </span>Added <code class="docutils literal notranslate"><span class="pre">get()</span></code> method to decorated
+<p><span class="versionmodified added">Added in version 0.5.3: </span>Added <code class="docutils literal notranslate"><span class="pre">get()</span></code> method to decorated
 function.</p>
 </div>
 <p>The default key generation will use the name
 of the function, the module name for the function,
 the arguments passed, as well as an optional “namespace”
 parameter in order to generate a cache key.</p>
 <p>Given a function <code class="docutils literal notranslate"><span class="pre">one</span></code> inside the module
@@ -544,33 +544,33 @@
 directly to the constructor of the <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a>
 in use, though is typically a dictionary.</p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.configure.params.wrap"></span><strong>wrap</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.configure.params.wrap">¶</a> – <p>Optional.  A list of <a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a>
 classes and/or instances, each of which will be applied
 in a chain to ultimately wrap the original backend,
 so that custom functionality augmentation can be applied.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.0.</span></p>
 </div>
 <div class="admonition seealso">
 <p class="admonition-title">See also</p>
 <p><a class="reference internal" href="usage.html#changing-backend-behavior"><span class="std std-ref">Changing Backend Behavior</span></a></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.configure.params.replace_existing_backend"></span><strong>replace_existing_backend</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.configure.params.replace_existing_backend">¶</a> – <p>if True, the existing cache backend
 will be replaced.  Without this flag, an exception is raised if
 a backend is already configured.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.7.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.7.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.configure.params.region_invalidator"></span><strong>region_invalidator</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.configure.params.region_invalidator">¶</a> – <p>Optional. Override default invalidation
 strategy with custom implementation of
 <a class="reference internal" href="#dogpile.cache.region.RegionInvalidationStrategy" title="dogpile.cache.region.RegionInvalidationStrategy"><code class="xref py py-class docutils literal notranslate"><span class="pre">RegionInvalidationStrategy</span></code></a>.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.6.2.</span></p>
+<p><span class="versionmodified added">Added in version 0.6.2.</span></p>
 </div>
 </p></li>
 </ul>
 </dd>
 </dl>
 </dd></dl>
 
@@ -611,47 +611,48 @@
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.CacheRegion.delete_multi">
 <span class="sig-name descname"><span class="pre">delete_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.delete_multi" title="Link to this definition">¶</a></dt>
 <dd><p>Remove multiple values from the cache.</p>
 <p>This operation is idempotent (can be called multiple times, or on a
 non-existent key, safely)</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.CacheRegion.get">
-<span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">expiration_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ignore_expiration</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a></span></span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.get" title="Link to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">expiration_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ignore_expiration</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Any</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Literal</span><span class="p"><span class="pre">[</span></span><span class="pre">NoValue.NO_VALUE</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.get" title="Link to this definition">¶</a></dt>
 <dd><p>Return a value from the cache, based on the given key.</p>
 <p>If the value is not present, the method returns the token
-<code class="docutils literal notranslate"><span class="pre">NO_VALUE</span></code>. <code class="docutils literal notranslate"><span class="pre">NO_VALUE</span></code> evaluates to False, but is separate from
-<code class="docutils literal notranslate"><span class="pre">None</span></code> to distinguish between a cached value of <code class="docutils literal notranslate"><span class="pre">None</span></code>.</p>
+<a class="reference internal" href="#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">api.NO_VALUE</span></code></a>. <a class="reference internal" href="#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">api.NO_VALUE</span></code></a> evaluates to False, but is
+separate from <code class="docutils literal notranslate"><span class="pre">None</span></code> to distinguish between a cached value of
+<code class="docutils literal notranslate"><span class="pre">None</span></code>.</p>
 <p>By default, the configured expiration time of the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a>, or alternatively the expiration
 time supplied by the <code class="docutils literal notranslate"><span class="pre">expiration_time</span></code> argument,
 is tested against the creation time of the retrieved
 value versus the current time (as reported by <code class="docutils literal notranslate"><span class="pre">time.time()</span></code>).
-If stale, the cached value is ignored and the <code class="docutils literal notranslate"><span class="pre">NO_VALUE</span></code>
+If stale, the cached value is ignored and the <a class="reference internal" href="#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">api.NO_VALUE</span></code></a>
 token is returned.  Passing the flag <code class="docutils literal notranslate"><span class="pre">ignore_expiration=True</span></code>
 bypasses the expiration time check.</p>
 <div class="versionchanged">
 <p><span class="versionmodified changed">Changed in version 0.3.0: </span><a class="reference internal" href="#dogpile.cache.region.CacheRegion.get" title="dogpile.cache.region.CacheRegion.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get()</span></code></a> now checks the value’s creation time
 against the expiration time, rather than returning
 the value unconditionally.</p>
 </div>
 <p>The method also interprets the cached value in terms
 of the current “invalidation” time as set by
 the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.invalidate" title="dogpile.cache.region.CacheRegion.invalidate"><code class="xref py py-meth docutils literal notranslate"><span class="pre">invalidate()</span></code></a> method.   If a value is present,
 but its creation time is older than the current
-invalidation time, the <code class="docutils literal notranslate"><span class="pre">NO_VALUE</span></code> token is returned.
+invalidation time, the <a class="reference internal" href="#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">api.NO_VALUE</span></code></a> token is returned.
 Passing the flag <code class="docutils literal notranslate"><span class="pre">ignore_expiration=True</span></code> bypasses
 the invalidation time check.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.3.0: </span>Support for the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.invalidate" title="dogpile.cache.region.CacheRegion.invalidate"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.invalidate()</span></code></a>
+<p><span class="versionmodified added">Added in version 0.3.0: </span>Support for the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.invalidate" title="dogpile.cache.region.CacheRegion.invalidate"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.invalidate()</span></code></a>
 method.</p>
 </div>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.get.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.get.params.key">¶</a> – Key to be retrieved. While it’s typical for a key to be a
 string, it is ultimately passed directly down to the cache backend,
@@ -667,23 +668,23 @@
 argument is <strong>not persisted in the cache</strong> and is relevant
 only to <strong>this specific cache retrieval operation</strong>, relative to
 the creation time stored with the existing cached value.
 Subsequent calls to <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get" title="dogpile.cache.region.CacheRegion.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get()</span></code></a> are <strong>not</strong> affected
 by this value.</p>
 </div>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.3.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.3.0.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.get.params.ignore_expiration"></span><strong>ignore_expiration</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.get.params.ignore_expiration">¶</a> – <p>if <code class="docutils literal notranslate"><span class="pre">True</span></code>, the value is returned
 from the cache if present, regardless of configured
 expiration times or whether or not <a class="reference internal" href="#dogpile.cache.region.CacheRegion.invalidate" title="dogpile.cache.region.CacheRegion.invalidate"><code class="xref py py-meth docutils literal notranslate"><span class="pre">invalidate()</span></code></a>
 was called.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.3.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.3.0.</span></p>
 </div>
 </p></li>
 </ul>
 </dd>
 </dl>
 <div class="admonition seealso">
 <p class="admonition-title">See also</p>
@@ -718,15 +719,15 @@
 time supplied by the <code class="docutils literal notranslate"><span class="pre">expiration_time</span></code> argument,
 is tested against the creation time of the retrieved
 value versus the current time (as reported by <code class="docutils literal notranslate"><span class="pre">time.time()</span></code>).
 If stale, the cached value is ignored and the <code class="docutils literal notranslate"><span class="pre">NO_VALUE</span></code>
 token is returned.  Passing the flag <code class="docutils literal notranslate"><span class="pre">ignore_expiration=True</span></code>
 bypasses the expiration time check.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.CacheRegion.get_or_create">
 <span class="sig-name descname"><span class="pre">get_or_create</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">creator</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">expiration_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">should_cache_fn</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">creator_args</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">Any</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Any</span></span></span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.get_or_create" title="Link to this definition">¶</a></dt>
 <dd><p>Return a cached value based on the given key.</p>
@@ -760,15 +761,15 @@
 before being optionally processed by the key_mangler function, so can
 be of any type recognized by the backend or by the key_mangler
 function, if present.</p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.get_or_create.params.creator"></span><strong>creator</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.get_or_create.params.creator">¶</a> – function which creates a new value.</p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.get_or_create.params.creator_args"></span><strong>creator_args</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.get_or_create.params.creator_args">¶</a> – <p>optional tuple of (args, kwargs) that will be
 passed to the creator function if present.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.7.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.7.0.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.get_or_create.params.expiration_time"></span><strong>expiration_time</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.get_or_create.params.expiration_time">¶</a> – <p>optional expiration time which will override
 the expiration time already configured on this <a class="reference internal" href="#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a>
 if not None.   To set no expiration, use the value -1.</p>
 <div class="admonition note">
 <p class="admonition-title">Note</p>
@@ -793,15 +794,15 @@
                     <span class="n">should_cache_fn</span><span class="o">=</span><span class="n">dont_cache_none</span><span class="p">)</span>
 </pre></div>
 </div>
 <p>Above, the function returns the value of create_value() if
 the cache is invalid, however if the return value is None,
 it won’t be cached.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.4.3.</span></p>
+<p><span class="versionmodified added">Added in version 0.4.3.</span></p>
 </div>
 </p></li>
 </ul>
 </dd>
 </dl>
 <div class="admonition seealso">
 <p class="admonition-title">See also</p>
@@ -845,15 +846,15 @@
 each value returned by the “creator”, and will then return True or
 False, indicating if the value should actually be cached or not.  If
 it returns False, the value is still returned, but isn’t cached.</p></li>
 </ul>
 </dd>
 </dl>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.0.</span></p>
 </div>
 <div class="admonition seealso">
 <p class="admonition-title">See also</p>
 <p><a class="reference internal" href="#dogpile.cache.region.CacheRegion.cache_multi_on_arguments" title="dogpile.cache.region.CacheRegion.cache_multi_on_arguments"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.cache_multi_on_arguments()</span></code></a></p>
 <p><a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_or_create" title="dogpile.cache.region.CacheRegion.get_or_create"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_or_create()</span></code></a></p>
 </div>
 </dd></dl>
@@ -864,15 +865,15 @@
 <dd><p>Return the <a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><code class="xref py py-class docutils literal notranslate"><span class="pre">CachedValue</span></code></a> object directly from the cache.</p>
 <p>This is the enclosing datastructure that includes the value as well as
 the metadata, including the timestamp when the value was cached.
 Convenience accessors on <a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><code class="xref py py-class docutils literal notranslate"><span class="pre">CachedValue</span></code></a> also provide for common
 data such as <a class="reference internal" href="#dogpile.cache.api.CachedValue.cached_time" title="dogpile.cache.api.CachedValue.cached_time"><code class="xref py py-attr docutils literal notranslate"><span class="pre">CachedValue.cached_time</span></code></a> and
 <a class="reference internal" href="#dogpile.cache.api.CachedValue.age" title="dogpile.cache.api.CachedValue.age"><code class="xref py py-attr docutils literal notranslate"><span class="pre">CachedValue.age</span></code></a>.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.3.: </span>Added <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_value_metadata" title="dogpile.cache.region.CacheRegion.get_value_metadata"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_value_metadata()</span></code></a></p>
+<p><span class="versionmodified added">Added in version 1.3.: </span>Added <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_value_metadata" title="dogpile.cache.region.CacheRegion.get_value_metadata"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_value_metadata()</span></code></a></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.CacheRegion.invalidate">
 <span class="sig-name descname"><span class="pre">invalidate</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">hard</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.invalidate" title="Link to this definition">¶</a></dt>
 <dd><p>Invalidate this <a class="reference internal" href="#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a>.</p>
@@ -904,47 +905,47 @@
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_or_create" title="dogpile.cache.region.CacheRegion.get_or_create"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_or_create()</span></code></a> will force an immediate
 regeneration of the value which all getters will wait for.
 With “soft” invalidation, subsequent getters will return the
 “old” value until the new one is available.</p>
 <p>Usage of “soft” invalidation requires that the region or the method
 is given a non-None expiration time.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.3.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.3.0.</span></p>
 </div>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.region.CacheRegion.invalidate.params.hard"></span><strong>hard</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.invalidate.params.hard">¶</a> – <p>if True, cache values will all require immediate
 regeneration; dogpile logic won’t be used.  If False, the
 creation time of existing values will be pushed back before
 the expiration time so that a return+regen will be invoked.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.1.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.1.</span></p>
 </div>
 </p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py property">
 <dt class="sig sig-object py" id="dogpile.cache.region.CacheRegion.is_configured">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">is_configured</span></span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.is_configured" title="Link to this definition">¶</a></dt>
 <dd><p>Return True if the backend has been configured via the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.configure" title="dogpile.cache.region.CacheRegion.configure"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.configure()</span></code></a> method already.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.1.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.1.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.CacheRegion.key_is_locked">
 <span class="sig-name descname"><span class="pre">key_is_locked</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">bool</span></span></span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.key_is_locked" title="Link to this definition">¶</a></dt>
 <dd><p>Return True if a particular cache key is currently being generated
 within the dogpile lock.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.2.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.2.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.CacheRegion.set">
 <span class="sig-name descname"><span class="pre">set</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Any</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.region.CacheRegion.set" title="Link to this definition">¶</a></dt>
 <dd><p>Place a new value in the cache under the given key.</p>
@@ -1103,15 +1104,15 @@
     <span class="c1"># ...</span>
 
 <span class="n">region</span> <span class="o">=</span> <span class="n">CacheRegion</span><span class="p">()</span>
 <span class="n">region</span> <span class="o">=</span> <span class="n">region</span><span class="o">.</span><span class="n">configure</span><span class="p">(</span><span class="n">region_invalidator</span><span class="o">=</span><span class="n">MyInvalidator</span><span class="p">(</span><span class="n">region</span><span class="p">))</span>
 </pre></div>
 </div>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.6.2.</span></p>
+<p><span class="versionmodified added">Added in version 0.6.2.</span></p>
 </div>
 <div class="admonition seealso">
 <p class="admonition-title">See also</p>
 <p><a class="reference internal" href="#dogpile.cache.region.CacheRegion.configure.params.region_invalidator" title="dogpile.cache.region.CacheRegion.configure"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">CacheRegion.configure.region_invalidator</span></code></a></p>
 </div>
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.region.RegionInvalidationStrategy.invalidate">
@@ -1208,74 +1209,74 @@
 <p>See the section <a class="reference internal" href="usage.html#creating-backends"><span class="std std-ref">Creating Backends</span></a> for details on how to
 register new backends or <a class="reference internal" href="usage.html#changing-backend-behavior"><span class="std std-ref">Changing Backend Behavior</span></a> for details on
 how to alter the behavior of existing backends.</p>
 <dl class="py data" id="module-dogpile.cache.api">
 <dt class="sig sig-object py" id="dogpile.cache.api.BackendFormatted">
 <span class="sig-prename descclassname"><span class="pre">dogpile.cache.api.</span></span><span class="sig-name descname"><span class="pre">BackendFormatted</span></span><a class="headerlink" href="#dogpile.cache.api.BackendFormatted" title="Link to this definition">¶</a></dt>
 <dd><p>Describes the type returned from the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get" title="dogpile.cache.api.CacheBackend.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get()</span></code></a> method.</p>
-<p>alias of <code class="xref py py-obj docutils literal notranslate"><span class="pre">Union</span></code>[<a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><code class="xref py py-class docutils literal notranslate"><span class="pre">CachedValue</span></code></a>, <a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><code class="xref py py-class docutils literal notranslate"><span class="pre">NoValue</span></code></a>, <code class="xref py py-class docutils literal notranslate"><span class="pre">bytes</span></code>]</p>
+<p>alias of <a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><code class="xref py py-class docutils literal notranslate"><span class="pre">CachedValue</span></code></a> | <code class="xref py py-obj docutils literal notranslate"><span class="pre">Literal</span></code>[<code class="xref py py-attr docutils literal notranslate"><span class="pre">NO_VALUE</span></code>] | <code class="xref py py-class docutils literal notranslate"><span class="pre">bytes</span></code></p>
 </dd></dl>
 
 <dl class="py data">
 <dt class="sig sig-object py" id="dogpile.cache.api.BackendSetType">
 <span class="sig-prename descclassname"><span class="pre">dogpile.cache.api.</span></span><span class="sig-name descname"><span class="pre">BackendSetType</span></span><a class="headerlink" href="#dogpile.cache.api.BackendSetType" title="Link to this definition">¶</a></dt>
 <dd><p>Describes the value argument passed to the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.set" title="dogpile.cache.api.CacheBackend.set"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.set()</span></code></a>
 method.</p>
-<p>alias of <code class="xref py py-obj docutils literal notranslate"><span class="pre">Union</span></code>[<a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><code class="xref py py-class docutils literal notranslate"><span class="pre">CachedValue</span></code></a>, <code class="xref py py-class docutils literal notranslate"><span class="pre">bytes</span></code>]</p>
+<p>alias of <a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><code class="xref py py-class docutils literal notranslate"><span class="pre">CachedValue</span></code></a> | <code class="xref py py-class docutils literal notranslate"><span class="pre">bytes</span></code></p>
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="dogpile.cache.api.BytesBackend">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.api.</span></span><span class="sig-name descname"><span class="pre">BytesBackend</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">arguments</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.api.BytesBackend" title="Link to this definition">¶</a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">DefaultSerialization</span></code>, <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a></p>
 <p>A cache backend that receives and returns series of bytes.</p>
 <p>This backend only supports the “serialized” form of values; subclasses
 should implement <a class="reference internal" href="#dogpile.cache.api.BytesBackend.get_serialized" title="dogpile.cache.api.BytesBackend.get_serialized"><code class="xref py py-meth docutils literal notranslate"><span class="pre">BytesBackend.get_serialized()</span></code></a>,
 <a class="reference internal" href="#dogpile.cache.api.BytesBackend.get_serialized_multi" title="dogpile.cache.api.BytesBackend.get_serialized_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">BytesBackend.get_serialized_multi()</span></code></a>,
 <a class="reference internal" href="#dogpile.cache.api.BytesBackend.set_serialized" title="dogpile.cache.api.BytesBackend.set_serialized"><code class="xref py py-meth docutils literal notranslate"><span class="pre">BytesBackend.set_serialized()</span></code></a>,
 <a class="reference internal" href="#dogpile.cache.api.BytesBackend.set_serialized_multi" title="dogpile.cache.api.BytesBackend.set_serialized_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">BytesBackend.set_serialized_multi()</span></code></a>.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.BytesBackend.get_serialized">
-<span class="sig-name descname"><span class="pre">get_serialized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">bytes</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a></span></span><a class="headerlink" href="#dogpile.cache.api.BytesBackend.get_serialized" title="Link to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get_serialized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">bytes</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Literal</span><span class="p"><span class="pre">[</span></span><span class="pre">NoValue.NO_VALUE</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.api.BytesBackend.get_serialized" title="Link to this definition">¶</a></dt>
 <dd><p>Retrieve a serialized value from the cache.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.api.BytesBackend.get_serialized.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.BytesBackend.get_serialized.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get" title="dogpile.cache.region.CacheRegion.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>a bytes object, or <a class="reference internal" href="#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">NO_VALUE</span></code></a>
 constant if not present.</p>
 </dd>
 </dl>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.BytesBackend.get_serialized_multi">
-<span class="sig-name descname"><span class="pre">get_serialized_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">bytes</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.api.BytesBackend.get_serialized_multi" title="Link to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get_serialized_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">bytes</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Literal</span><span class="p"><span class="pre">[</span></span><span class="pre">NoValue.NO_VALUE</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.api.BytesBackend.get_serialized_multi" title="Link to this definition">¶</a></dt>
 <dd><p>Retrieve multiple serialized values from the cache.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.api.BytesBackend.get_serialized_multi.params.keys"></span><strong>keys</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.BytesBackend.get_serialized_multi.params.keys">¶</a> – sequence of string keys that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_multi" title="dogpile.cache.region.CacheRegion.get_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_multi()</span></code></a> method, which will also be processed
 by the “key mangling” function if one was present.</p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>list of bytes objects</p>
 </dd>
 </dl>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.BytesBackend.set_serialized">
 <span class="sig-name descname"><span class="pre">set_serialized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bytes</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.api.BytesBackend.set_serialized" title="Link to this definition">¶</a></dt>
 <dd><p>Set a serialized value in the cache.</p>
@@ -1286,15 +1287,15 @@
 method, which will also be processed by the “key mangling” function
 if one was present.</p></li>
 <li><p><span class="target" id="dogpile.cache.api.BytesBackend.set_serialized.params.value"></span><strong>value</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.BytesBackend.set_serialized.params.value">¶</a> – a bytes object to be stored.</p></li>
 </ul>
 </dd>
 </dl>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.BytesBackend.set_serialized_multi">
 <span class="sig-name descname"><span class="pre">set_serialized_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">mapping</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.api.BytesBackend.set_serialized_multi" title="Link to this definition">¶</a></dt>
 <dd><p>Set multiple serialized values in the cache.</p>
@@ -1309,15 +1310,15 @@
 <a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a>, be aware that when this method is invoked by
 <code class="xref py py-meth docutils literal notranslate"><span class="pre">Region.get_or_create_multi()</span></code>, the <code class="docutils literal notranslate"><span class="pre">mapping</span></code> values are the
 same ones returned to the upstream caller. If the subclass alters the
 values in any way, it must not do so ‘in-place’ on the <code class="docutils literal notranslate"><span class="pre">mapping</span></code> dict
 – that will have the undesirable effect of modifying the returned
 values as well.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheBackend">
@@ -1357,31 +1358,31 @@
 </dd>
 </dl>
 <p>The behavior here should be idempotent,
 that is, can be called any number of times
 regardless of whether or not the
 key exists.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheBackend.deserializer">
 <span class="sig-name descname"><span class="pre">deserializer</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">None</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#dogpile.cache.api.CacheBackend.deserializer" title="Link to this definition">¶</a></dt>
 <dd><p>deserializer function that will be used by default if not overridden
 by the region.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheBackend.get">
-<span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">bytes</span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.get" title="Link to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Literal</span><span class="p"><span class="pre">[</span></span><span class="pre">NoValue.NO_VALUE</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">bytes</span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.get" title="Link to this definition">¶</a></dt>
 <dd><p>Retrieve an optionally serialized value from the cache.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.api.CacheBackend.get.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.CacheBackend.get.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get" title="dogpile.cache.region.CacheRegion.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p>
 </dd>
@@ -1393,15 +1394,15 @@
 </dl>
 <p>If a serializer is in use, this method will only be called if the
 <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get_serialized" title="dogpile.cache.api.CacheBackend.get_serialized"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get_serialized()</span></code></a> method is not overridden.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheBackend.get_multi">
-<span class="sig-name descname"><span class="pre">get_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.get_multi" title="Link to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Literal</span><span class="p"><span class="pre">[</span></span><span class="pre">NoValue.NO_VALUE</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.get_multi" title="Link to this definition">¶</a></dt>
 <dd><p>Retrieve multiple optionally serialized values from the cache.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.api.CacheBackend.get_multi.params.keys"></span><strong>keys</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.CacheBackend.get_multi.params.keys">¶</a> – sequence of string keys that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_multi" title="dogpile.cache.region.CacheRegion.get_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_multi()</span></code></a> method, which will also be processed
 by the “key mangling” function if one was present.</p>
 </dd>
@@ -1410,15 +1411,15 @@
 <dt>:return a list of values as would be returned</dt><dd><p>individually via the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get" title="dogpile.cache.api.CacheBackend.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get()</span></code></a> method, corresponding
 to the list of keys given.</p>
 </dd>
 </dl>
 <p>If a serializer is in use, this method will only be called if the
 <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get_serialized_multi" title="dogpile.cache.api.CacheBackend.get_serialized_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get_serialized_multi()</span></code></a> method is not overridden.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheBackend.get_mutex">
 <span class="sig-name descname"><span class="pre">get_mutex</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#dogpile.cache.api.CacheMutex" title="dogpile.cache.api.CacheMutex"><span class="pre">CacheMutex</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.get_mutex" title="Link to this definition">¶</a></dt>
 <dd><p>Return an optional mutexing object for the given key.</p>
@@ -1445,15 +1446,15 @@
 can be used as a means of throttling the total
 number of value recreation operations that may
 proceed at one time.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheBackend.get_serialized">
-<span class="sig-name descname"><span class="pre">get_serialized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">bytes</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.get_serialized" title="Link to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get_serialized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">bytes</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Literal</span><span class="p"><span class="pre">[</span></span><span class="pre">NoValue.NO_VALUE</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.get_serialized" title="Link to this definition">¶</a></dt>
 <dd><p>Retrieve a serialized value from the cache.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.api.CacheBackend.get_serialized.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.CacheBackend.get_serialized.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get" title="dogpile.cache.region.CacheRegion.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p>
 </dd>
@@ -1461,40 +1462,40 @@
 <dd class="field-even"><p>a bytes object, or <a class="reference internal" href="#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">NO_VALUE</span></code></a>
 constant if not present.</p>
 </dd>
 </dl>
 <p>The default implementation of this method for <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a>
 returns the value of the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get" title="dogpile.cache.api.CacheBackend.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get()</span></code></a> method.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 <div class="admonition seealso">
 <p class="admonition-title">See also</p>
 <p><a class="reference internal" href="#dogpile.cache.api.BytesBackend" title="dogpile.cache.api.BytesBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">BytesBackend</span></code></a></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheBackend.get_serialized_multi">
-<span class="sig-name descname"><span class="pre">get_serialized_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">bytes</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.get_serialized_multi" title="Link to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get_serialized_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">bytes</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Literal</span><span class="p"><span class="pre">[</span></span><span class="pre">NoValue.NO_VALUE</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.get_serialized_multi" title="Link to this definition">¶</a></dt>
 <dd><p>Retrieve multiple serialized values from the cache.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.api.CacheBackend.get_serialized_multi.params.keys"></span><strong>keys</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.CacheBackend.get_serialized_multi.params.keys">¶</a> – sequence of string keys that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_multi" title="dogpile.cache.region.CacheRegion.get_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_multi()</span></code></a> method, which will also be processed
 by the “key mangling” function if one was present.</p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>list of bytes objects</p>
 </dd>
 </dl>
 <p>The default implementation of this method for <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a>
 returns the value of the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get_multi" title="dogpile.cache.api.CacheBackend.get_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get_multi()</span></code></a> method.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 <div class="admonition seealso">
 <p class="admonition-title">See also</p>
 <p><a class="reference internal" href="#dogpile.cache.api.BytesBackend" title="dogpile.cache.api.BytesBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">BytesBackend</span></code></a></p>
 </div>
 </dd></dl>
 
@@ -1508,15 +1509,15 @@
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheBackend.serializer">
 <span class="sig-name descname"><span class="pre">serializer</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">None</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Callable</span><span class="p"><span class="pre">[</span></span><span class="p"><span class="pre">[</span></span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#dogpile.cache.api.CacheBackend.serializer" title="Link to this definition">¶</a></dt>
 <dd><p>Serializer function that will be used by default if not overridden
 by the region.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheBackend.set">
 <span class="sig-name descname"><span class="pre">set</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">bytes</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.set" title="Link to this definition">¶</a></dt>
 <dd><p>Set an optionally serialized value in the cache.</p>
@@ -1556,15 +1557,15 @@
 same ones returned to the upstream caller. If the subclass alters the
 values in any way, it must not do so ‘in-place’ on the <code class="docutils literal notranslate"><span class="pre">mapping</span></code> dict
 – that will have the undesirable effect of modifying the returned
 values as well.</p>
 <p>If a serializer is in use, this method will only be called if the
 <a class="reference internal" href="#dogpile.cache.api.CacheBackend.set_serialized_multi" title="dogpile.cache.api.CacheBackend.set_serialized_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.set_serialized_multi()</span></code></a> method is not overridden.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheBackend.set_serialized">
 <span class="sig-name descname"><span class="pre">set_serialized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bytes</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheBackend.set_serialized" title="Link to this definition">¶</a></dt>
 <dd><p>Set a serialized value in the cache.</p>
@@ -1577,15 +1578,15 @@
 <li><p><span class="target" id="dogpile.cache.api.CacheBackend.set_serialized.params.value"></span><strong>value</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.api.CacheBackend.set_serialized.params.value">¶</a> – a bytes object to be stored.</p></li>
 </ul>
 </dd>
 </dl>
 <p>The default implementation of this method for <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a>
 calls upon the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.set" title="dogpile.cache.api.CacheBackend.set"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.set()</span></code></a> method.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 <div class="admonition seealso">
 <p class="admonition-title">See also</p>
 <p><a class="reference internal" href="#dogpile.cache.api.BytesBackend" title="dogpile.cache.api.BytesBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">BytesBackend</span></code></a></p>
 </div>
 </dd></dl>
 
@@ -1604,15 +1605,15 @@
 <a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a>, be aware that when this method is invoked by
 <code class="xref py py-meth docutils literal notranslate"><span class="pre">Region.get_or_create_multi()</span></code>, the <code class="docutils literal notranslate"><span class="pre">mapping</span></code> values are the
 same ones returned to the upstream caller. If the subclass alters the
 values in any way, it must not do so ‘in-place’ on the <code class="docutils literal notranslate"><span class="pre">mapping</span></code> dict
 – that will have the undesirable effect of modifying the returned
 values as well.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 <p>The default implementation of this method for <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a>
 calls upon the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.set_multi" title="dogpile.cache.api.CacheBackend.set_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.set_multi()</span></code></a> method.</p>
 <div class="admonition seealso">
 <p class="admonition-title">See also</p>
 <p><a class="reference internal" href="#dogpile.cache.api.BytesBackend" title="dogpile.cache.api.BytesBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">BytesBackend</span></code></a></p>
 </div>
@@ -1624,15 +1625,15 @@
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheMutex">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.api.</span></span><span class="sig-name descname"><span class="pre">CacheMutex</span></span><a class="headerlink" href="#dogpile.cache.api.CacheMutex" title="Link to this definition">¶</a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">ABC</span></code></p>
 <p>Describes a mutexing object with acquire and release methods.</p>
 <p>This is an abstract base class; any object that has acquire/release
 methods may be used.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 <div class="admonition seealso">
 <p class="admonition-title">See also</p>
 <p><a class="reference internal" href="#dogpile.cache.api.CacheBackend.get_mutex" title="dogpile.cache.api.CacheBackend.get_mutex"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get_mutex()</span></code></a> - the backend method that optionally
 returns this locking object.</p>
 </div>
 <dl class="py method">
@@ -1656,15 +1657,15 @@
 <dd><p>Check if the mutex was acquired.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Returns<span class="colon">:</span></dt>
 <dd class="field-odd"><p>true if the lock is acquired.</p>
 </dd>
 </dl>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.2.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.2.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheMutex.release">
 <em class="property"><span class="pre">abstract</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">release</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.api.CacheMutex.release" title="Link to this definition">¶</a></dt>
 <dd><p>Release the mutex.</p>
@@ -1673,15 +1674,15 @@
 </dd></dl>
 
 <dl class="py data">
 <dt class="sig sig-object py" id="dogpile.cache.api.CacheReturnType">
 <span class="sig-prename descclassname"><span class="pre">dogpile.cache.api.</span></span><span class="sig-name descname"><span class="pre">CacheReturnType</span></span><a class="headerlink" href="#dogpile.cache.api.CacheReturnType" title="Link to this definition">¶</a></dt>
 <dd><p>The non-serialized form of what may be returned from a backend
 get method.</p>
-<p>alias of <code class="xref py py-obj docutils literal notranslate"><span class="pre">Union</span></code>[<a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><code class="xref py py-class docutils literal notranslate"><span class="pre">CachedValue</span></code></a>, <a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><code class="xref py py-class docutils literal notranslate"><span class="pre">NoValue</span></code></a>]</p>
+<p>alias of <a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><code class="xref py py-class docutils literal notranslate"><span class="pre">CachedValue</span></code></a> | <code class="xref py py-obj docutils literal notranslate"><span class="pre">Literal</span></code>[<code class="xref py py-attr docutils literal notranslate"><span class="pre">NO_VALUE</span></code>]</p>
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="dogpile.cache.api.CachedValue">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.api.</span></span><span class="sig-name descname"><span class="pre">CachedValue</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">payload</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">ValuePayload</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">metadata</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">MetaDataType</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.api.CachedValue" title="Link to this definition">¶</a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">NamedTuple</span></code></p>
 <p>Represent a value stored in the cache.</p>
@@ -1693,25 +1694,25 @@
 <dt class="sig sig-object py" id="dogpile.cache.api.CachedValue.age">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">age</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">float</span></em><a class="headerlink" href="#dogpile.cache.api.CachedValue.age" title="Link to this definition">¶</a></dt>
 <dd><p>Returns the elapsed time in seconds as a <cite>float</cite> since the insertion
 of the value in the cache.</p>
 <p>This value is computed <strong>dynamically</strong> by subtracting the cached
 floating point epoch value from the value of <code class="docutils literal notranslate"><span class="pre">time.time()</span></code>.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.3.</span></p>
+<p><span class="versionmodified added">Added in version 1.3.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py property">
 <dt class="sig sig-object py" id="dogpile.cache.api.CachedValue.cached_time">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">cached_time</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">float</span></em><a class="headerlink" href="#dogpile.cache.api.CachedValue.cached_time" title="Link to this definition">¶</a></dt>
 <dd><p>The epoch (floating point time value) stored when this payload was
 cached.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.3.</span></p>
+<p><span class="versionmodified added">Added in version 1.3.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="dogpile.cache.api.CachedValue.metadata">
 <span class="sig-name descname"><span class="pre">metadata</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">Mapping</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">Any</span><span class="p"><span class="pre">]</span></span></em><a class="headerlink" href="#dogpile.cache.api.CachedValue.metadata" title="Link to this definition">¶</a></dt>
 <dd><p>Metadata dictionary for the cached value.</p>
@@ -1730,44 +1731,44 @@
 <dl class="py exception">
 <dt class="sig sig-object py" id="dogpile.cache.api.CantDeserializeException">
 <em class="property"><span class="pre">exception</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.api.</span></span><span class="sig-name descname"><span class="pre">CantDeserializeException</span></span><a class="headerlink" href="#dogpile.cache.api.CantDeserializeException" title="Link to this definition">¶</a></dt>
 <dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">Exception</span></code></p>
 <p>Exception indicating deserialization failed, and that caching
 should proceed to re-generate a value</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.2.0.</span></p>
+<p><span class="versionmodified added">Added in version 1.2.0.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="dogpile.cache.api.KeyType">
 <span class="sig-prename descclassname"><span class="pre">dogpile.cache.api.</span></span><span class="sig-name descname"><span class="pre">KeyType</span></span><a class="headerlink" href="#dogpile.cache.api.KeyType" title="Link to this definition">¶</a></dt>
 <dd><p>A cache key.</p>
 </dd></dl>
 
 <dl class="py data">
 <dt class="sig sig-object py" id="dogpile.cache.api.NO_VALUE">
 <span class="sig-prename descclassname"><span class="pre">dogpile.cache.api.</span></span><span class="sig-name descname"><span class="pre">NO_VALUE</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">&lt;dogpile.cache.api.NoValue</span> <span class="pre">object&gt;</span></em><a class="headerlink" href="#dogpile.cache.api.NO_VALUE" title="Link to this definition">¶</a></dt>
-<dd><p>Value returned from <code class="docutils literal notranslate"><span class="pre">get()</span></code> that describes
+<dd><p>Value returned from <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get" title="dogpile.cache.region.CacheRegion.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get()</span></code></a> that describes
 a  key not present.</p>
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="dogpile.cache.api.NoValue">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.api.</span></span><span class="sig-name descname"><span class="pre">NoValue</span></span><a class="headerlink" href="#dogpile.cache.api.NoValue" title="Link to this definition">¶</a></dt>
-<dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">object</span></code></p>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.api.</span></span><span class="sig-name descname"><span class="pre">NoValue</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">value</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.api.NoValue" title="Link to this definition">¶</a></dt>
+<dd><p>Bases: <code class="xref py py-class docutils literal notranslate"><span class="pre">Enum</span></code></p>
 <p>Describe a missing cache value.</p>
 <p>The <a class="reference internal" href="#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">NO_VALUE</span></code></a> constant should be used.</p>
 </dd></dl>
 
 <dl class="py data">
 <dt class="sig sig-object py" id="dogpile.cache.api.SerializedReturnType">
 <span class="sig-prename descclassname"><span class="pre">dogpile.cache.api.</span></span><span class="sig-name descname"><span class="pre">SerializedReturnType</span></span><a class="headerlink" href="#dogpile.cache.api.SerializedReturnType" title="Link to this definition">¶</a></dt>
 <dd><p>the serialized form of what may be returned from a backend get method.</p>
-<p>alias of <code class="xref py py-obj docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">bytes</span></code>, <a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><code class="xref py py-class docutils literal notranslate"><span class="pre">NoValue</span></code></a>]</p>
+<p>alias of <code class="xref py py-class docutils literal notranslate"><span class="pre">bytes</span></code> | <code class="xref py py-obj docutils literal notranslate"><span class="pre">Literal</span></code>[<code class="xref py py-attr docutils literal notranslate"><span class="pre">NO_VALUE</span></code>]</p>
 </dd></dl>
 
 <dl class="py data">
 <dt class="sig sig-object py" id="dogpile.cache.api.ValuePayload">
 <span class="sig-prename descclassname"><span class="pre">dogpile.cache.api.</span></span><span class="sig-name descname"><span class="pre">ValuePayload</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">typing.Any</span></em><a class="headerlink" href="#dogpile.cache.api.ValuePayload" title="Link to this definition">¶</a></dt>
 <dd><p>An object to be placed in the cache against a key.</p>
 </dd></dl>
@@ -1843,15 +1844,15 @@
 </dd>
 </dl>
 <p>The behavior here should be idempotent,
 that is, can be called any number of times
 regardless of whether or not the
 key exists.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memory.MemoryBackend.get">
 <span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.memory.MemoryBackend.get" title="Link to this definition">¶</a></dt>
 <dd><p>Retrieve an optionally serialized value from the cache.</p>
@@ -1886,15 +1887,15 @@
 <dt>:return a list of values as would be returned</dt><dd><p>individually via the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get" title="dogpile.cache.api.CacheBackend.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get()</span></code></a> method, corresponding
 to the list of keys given.</p>
 </dd>
 </dl>
 <p>If a serializer is in use, this method will only be called if the
 <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get_serialized_multi" title="dogpile.cache.api.CacheBackend.get_serialized_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get_serialized_multi()</span></code></a> method is not overridden.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memory.MemoryBackend.set">
 <span class="sig-name descname"><span class="pre">set</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.memory.MemoryBackend.set" title="Link to this definition">¶</a></dt>
 <dd><p>Set an optionally serialized value in the cache.</p>
@@ -1934,15 +1935,15 @@
 same ones returned to the upstream caller. If the subclass alters the
 values in any way, it must not do so ‘in-place’ on the <code class="docutils literal notranslate"><span class="pre">mapping</span></code> dict
 – that will have the undesirable effect of modifying the returned
 values as well.</p>
 <p>If a serializer is in use, this method will only be called if the
 <a class="reference internal" href="#dogpile.cache.api.CacheBackend.set_serialized_multi" title="dogpile.cache.api.CacheBackend.set_serialized_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.set_serialized_multi()</span></code></a> method is not overridden.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memory.MemoryPickleBackend">
@@ -1968,15 +1969,15 @@
 the <a class="reference internal" href="#dogpile.cache.backends.memory.MemoryPickleBackend" title="dogpile.cache.backends.memory.MemoryPickleBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">MemoryPickleBackend</span></code></a> performance is somewhere in between
 that of the pure <a class="reference internal" href="#dogpile.cache.backends.memory.MemoryBackend" title="dogpile.cache.backends.memory.MemoryBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">MemoryBackend</span></code></a> and the remote server oriented
 backends such as that of Memcached or Redis.</p>
 <p>Pickle behavior here is the same as that of the Redis backend, using
 either <code class="docutils literal notranslate"><span class="pre">cPickle</span></code> or <code class="docutils literal notranslate"><span class="pre">pickle</span></code> and specifying <code class="docutils literal notranslate"><span class="pre">HIGHEST_PROTOCOL</span></code>
 upon serialize.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.3.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.3.</span></p>
 </div>
 </dd></dl>
 
 <section id="memcached-backends">
 <span id="module-dogpile.cache.backends.memcached"></span><h3>Memcached Backends<a class="headerlink" href="#memcached-backends" title="Link to this heading">¶</a></h3>
 <p>Provides backends for talking to <a class="reference external" href="http://memcached.org">memcached</a>.</p>
 </section>
@@ -2031,15 +2032,15 @@
 <li><p><span class="target" id="dogpile.cache.backends.memcached.BMemcachedBackend.params.username"></span><strong>username</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.BMemcachedBackend.params.username">¶</a> – optional username, will be used for
 SASL authentication.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.memcached.BMemcachedBackend.params.password"></span><strong>password</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.BMemcachedBackend.params.password">¶</a> – optional password, will be used for
 SASL authentication.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.memcached.BMemcachedBackend.params.tls_context"></span><strong>tls_context</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.BMemcachedBackend.params.tls_context">¶</a> – <p>optional TLS context, will be used for
 TLS connections.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.0.2.</span></p>
+<p><span class="versionmodified added">Added in version 1.0.2.</span></p>
 </div>
 </p></li>
 </ul>
 </dd>
 </dl>
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memcached.BMemcachedBackend.delete_multi">
@@ -2068,35 +2069,15 @@
 processes will be talking to the same memcached instance.
 When left at False, dogpile will coordinate on a regular
 threading mutex.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.memcached.GenericMemcachedBackend.params.lock_timeout"></span><strong>lock_timeout</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.params.lock_timeout">¶</a> – <p>integer, number of seconds after acquiring a lock that
 memcached should expire it.  This argument is only valid when
 <code class="docutils literal notranslate"><span class="pre">distributed_lock</span></code> is <code class="docutils literal notranslate"><span class="pre">True</span></code>.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.7.</span></p>
-</div>
-</p></li>
-<li><p><span class="target" id="dogpile.cache.backends.memcached.GenericMemcachedBackend.params.memcached_expire_time"></span><strong>memcached_expire_time</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.params.memcached_expire_time">¶</a> – <p>integer, when present will
-be passed as the <code class="docutils literal notranslate"><span class="pre">time</span></code> parameter to <code class="docutils literal notranslate"><span class="pre">pylibmc.Client.set</span></code>.
-This is used to set the memcached expiry time for a value.</p>
-<div class="admonition note">
-<p class="admonition-title">Note</p>
-<p>This parameter is <strong>different</strong> from Dogpile’s own
-<code class="docutils literal notranslate"><span class="pre">expiration_time</span></code>, which is the number of seconds after
-which Dogpile will consider the value to be expired.
-When Dogpile considers a value to be expired,
-it <strong>continues to use the value</strong> until generation
-of a new value is complete, when using
-<a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_or_create" title="dogpile.cache.region.CacheRegion.get_or_create"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_or_create()</span></code></a>.
-Therefore, if you are setting <code class="docutils literal notranslate"><span class="pre">memcached_expire_time</span></code>, you’ll
-want to make sure it is greater than <code class="docutils literal notranslate"><span class="pre">expiration_time</span></code>
-by at least enough seconds for new values to be generated,
-else the value won’t be available during a regeneration,
-forcing all threads to wait for a regeneration each time
-a value expires.</p>
+<p><span class="versionmodified added">Added in version 0.5.7.</span></p>
 </div>
 </p></li>
 </ul>
 </dd>
 </dl>
 <p>The <code class="xref py py-class docutils literal notranslate"><span class="pre">GenericMemachedBackend</span></code> uses a <code class="docutils literal notranslate"><span class="pre">threading.local()</span></code>
 object to store individual client objects per thread,
@@ -2145,25 +2126,25 @@
 </dd>
 </dl>
 <p>The behavior here should be idempotent,
 that is, can be called any number of times
 regardless of whether or not the
 key exists.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memcached.GenericMemcachedBackend.deserializer">
 <span class="sig-name descname"><span class="pre">deserializer</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">None</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Deserializer</span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.deserializer" title="Link to this definition">¶</a></dt>
 <dd><p>deserializer function that will be used by default if not overridden
 by the region.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memcached.GenericMemcachedBackend.get">
 <span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.get" title="Link to this definition">¶</a></dt>
 <dd><p>Retrieve an optionally serialized value from the cache.</p>
@@ -2198,15 +2179,15 @@
 <dt>:return a list of values as would be returned</dt><dd><p>individually via the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get" title="dogpile.cache.api.CacheBackend.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get()</span></code></a> method, corresponding
 to the list of keys given.</p>
 </dd>
 </dl>
 <p>If a serializer is in use, this method will only be called if the
 <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get_serialized_multi" title="dogpile.cache.api.CacheBackend.get_serialized_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get_serialized_multi()</span></code></a> method is not overridden.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memcached.GenericMemcachedBackend.get_mutex">
 <span class="sig-name descname"><span class="pre">get_mutex</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.get_mutex" title="Link to this definition">¶</a></dt>
 <dd><p>Return an optional mutexing object for the given key.</p>
@@ -2237,15 +2218,15 @@
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memcached.GenericMemcachedBackend.serializer">
 <span class="sig-name descname"><span class="pre">serializer</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">None</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Serializer</span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.serializer" title="Link to this definition">¶</a></dt>
 <dd><p>Serializer function that will be used by default if not overridden
 by the region.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memcached.GenericMemcachedBackend.set">
 <span class="sig-name descname"><span class="pre">set</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend.set" title="Link to this definition">¶</a></dt>
 <dd><p>Set an optionally serialized value in the cache.</p>
@@ -2292,15 +2273,15 @@
 same ones returned to the upstream caller. If the subclass alters the
 values in any way, it must not do so ‘in-place’ on the <code class="docutils literal notranslate"><span class="pre">mapping</span></code> dict
 – that will have the undesirable effect of modifying the returned
 values as well.</p>
 <p>If a serializer is in use, this method will only be called if the
 <a class="reference internal" href="#dogpile.cache.api.CacheBackend.set_serialized_multi" title="dogpile.cache.api.CacheBackend.set_serialized_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.set_serialized_multi()</span></code></a> method is not overridden.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="dogpile.cache.backends.memcached.MemcachedBackend">
@@ -2359,15 +2340,15 @@
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.backends.memcached.</span></span><span class="sig-name descname"><span class="pre">PyMemcacheBackend</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">arguments</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.memcached.PyMemcacheBackend" title="Link to this definition">¶</a></dt>
 <dd><p>Bases: <a class="reference internal" href="#dogpile.cache.backends.memcached.GenericMemcachedBackend" title="dogpile.cache.backends.memcached.GenericMemcachedBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">GenericMemcachedBackend</span></code></a></p>
 <p>A backend for the
 <a class="reference external" href="https://github.com/pinterest/pymemcache">pymemcache</a>
 memcached client.</p>
 <p>A comprehensive, fast, pure Python memcached client</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.2.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.2.</span></p>
 </div>
 <p>pymemcache supports the following features:</p>
 <ul class="simple">
 <li><p>Complete implementation of the memcached text protocol.</p></li>
 <li><p>Configurable timeouts for socket connect and send/recv calls.</p></li>
 <li><p>Access to the “noreply” flag, which can significantly increase
 the speed of writes.</p></li>
@@ -2433,15 +2414,15 @@
         <span class="s1">&#39;url&#39;</span><span class="p">:[</span><span class="s2">&quot;127.0.0.1&quot;</span><span class="p">],</span>
         <span class="s1">&#39;socket_keepalive&#39;</span><span class="p">:</span> <span class="n">socket_keepalive</span>
     <span class="p">}</span>
 <span class="p">)</span>
 </pre></div>
 </div>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.4: </span>- added support for <code class="docutils literal notranslate"><span class="pre">socket_keepalive</span></code>.</p>
+<p><span class="versionmodified added">Added in version 1.1.4: </span>- added support for <code class="docutils literal notranslate"><span class="pre">socket_keepalive</span></code>.</p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.backends.memcached.PyMemcacheBackend.params.enable_retry_client"></span><strong>enable_retry_client</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.PyMemcacheBackend.params.enable_retry_client">¶</a> – <p>optional flag to enable retry client
 mechanisms to handle failure.  Defaults to False.  When set to <code class="docutils literal notranslate"><span class="pre">True</span></code>,
 the <a class="reference internal" href="#dogpile.cache.backends.memcached.PyMemcacheBackend.params.retry_attempts" title="dogpile.cache.backends.memcached.PyMemcacheBackend"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">PyMemcacheBackend.retry_attempts</span></code></a> parameter must also
 be set, along with optional parameters
 <a class="reference internal" href="#dogpile.cache.backends.memcached.PyMemcacheBackend.params.retry_delay" title="dogpile.cache.backends.memcached.PyMemcacheBackend"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">PyMemcacheBackend.retry_delay</span></code></a>.
@@ -2449,63 +2430,86 @@
 <a class="reference internal" href="#dogpile.cache.backends.memcached.PyMemcacheBackend.params.do_not_retry_for" title="dogpile.cache.backends.memcached.PyMemcacheBackend"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">PyMemcacheBackend.do_not_retry_for</span></code></a>.</p>
 <div class="admonition seealso">
 <p class="admonition-title">See also</p>
 <p><a class="reference external" href="https://pymemcache.readthedocs.io/en/latest/getting_started.html#using-the-built-in-retrying-mechanism">https://pymemcache.readthedocs.io/en/latest/getting_started.html#using-the-built-in-retrying-mechanism</a> -
 in the pymemcache documentation</p>
 </div>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.4.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.4.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.backends.memcached.PyMemcacheBackend.params.retry_attempts"></span><strong>retry_attempts</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.PyMemcacheBackend.params.retry_attempts">¶</a> – <p>how many times to attempt an action with
 pymemcache’s retrying wrapper before failing. Must be 1 or above.
 Defaults to None.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.4.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.4.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.backends.memcached.PyMemcacheBackend.params.retry_delay"></span><strong>retry_delay</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.PyMemcacheBackend.params.retry_delay">¶</a> – <p>optional int|float, how many seconds to sleep between
 each attempt. Used by the retry wrapper. Defaults to None.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.4.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.4.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.backends.memcached.PyMemcacheBackend.params.retry_for"></span><strong>retry_for</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.PyMemcacheBackend.params.retry_for">¶</a> – <p>optional None|tuple|set|list, what exceptions to
 allow retries for. Will allow retries for all exceptions if None.
 Example: <code class="docutils literal notranslate"><span class="pre">(MemcacheClientError,</span> <span class="pre">MemcacheUnexpectedCloseError)</span></code>
 Accepts any class that is a subclass of Exception.  Defaults to None.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.4.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.4.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.backends.memcached.PyMemcacheBackend.params.do_not_retry_for"></span><strong>do_not_retry_for</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.PyMemcacheBackend.params.do_not_retry_for">¶</a> – <p>optional None|tuple|set|list, what
 exceptions should be retried. Will not block retries for any Exception if
 None. Example: <code class="docutils literal notranslate"><span class="pre">(IOError,</span> <span class="pre">MemcacheIllegalInputError)</span></code>
 Accepts any class that is a subclass of Exception. Defaults to None.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.4.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.4.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.backends.memcached.PyMemcacheBackend.params.hashclient_retry_attempts"></span><strong>hashclient_retry_attempts</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.PyMemcacheBackend.params.hashclient_retry_attempts">¶</a> – <p>Amount of times a client should be tried
 before it is marked dead and removed from the pool in the HashClient’s
 internal mechanisms.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.5.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.5.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.backends.memcached.PyMemcacheBackend.params.hashclient_retry_timeout"></span><strong>hashclient_retry_timeout</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.PyMemcacheBackend.params.hashclient_retry_timeout">¶</a> – <p>Time in seconds that should pass between
 retry attempts in the HashClient’s internal mechanisms.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.5.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.5.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.backends.memcached.PyMemcacheBackend.params.dead_timeout"></span><strong>dead_timeout</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.PyMemcacheBackend.params.dead_timeout">¶</a> – <p>Time in seconds before attempting to add a node
 back in the pool in the HashClient’s internal mechanisms.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.5.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.5.</span></p>
+</div>
+</p></li>
+<li><p><span class="target" id="dogpile.cache.backends.memcached.PyMemcacheBackend.params.memcached_expire_time"></span><strong>memcached_expire_time</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.memcached.PyMemcacheBackend.params.memcached_expire_time">¶</a> – <p>integer, when present will
+be passed as the <code class="docutils literal notranslate"><span class="pre">time</span></code> parameter to the <code class="docutils literal notranslate"><span class="pre">set</span></code> method.
+This is used to set the memcached expiry time for a value.</p>
+<div class="admonition note">
+<p class="admonition-title">Note</p>
+<p>This parameter is <strong>different</strong> from Dogpile’s own
+<code class="docutils literal notranslate"><span class="pre">expiration_time</span></code>, which is the number of seconds after
+which Dogpile will consider the value to be expired.
+When Dogpile considers a value to be expired,
+it <strong>continues to use the value</strong> until generation
+of a new value is complete, when using
+<a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_or_create" title="dogpile.cache.region.CacheRegion.get_or_create"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_or_create()</span></code></a>.
+Therefore, if you are setting <code class="docutils literal notranslate"><span class="pre">memcached_expire_time</span></code>, you’ll
+want to make sure it is greater than <code class="docutils literal notranslate"><span class="pre">expiration_time</span></code>
+by at least enough seconds for new values to be generated,
+else the value won’t be available during a regeneration,
+forcing all threads to wait for a regeneration each time
+a value expires.</p>
+</div>
+<div class="versionadded">
+<p><span class="versionmodified added">Added in version 1.3.3.</span></p>
 </div>
 </p></li>
 </ul>
 </dd>
 </dl>
 </dd></dl>
 
@@ -2581,15 +2585,15 @@
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.params.url"></span><strong>url</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.params.url">¶</a> – string. If provided, will override separate
 host/username/password/port/db params.  The format is that accepted by
 <code class="docutils literal notranslate"><span class="pre">StrictRedis.from_url()</span></code>.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.params.host"></span><strong>host</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.params.host">¶</a> – string, default is <code class="docutils literal notranslate"><span class="pre">localhost</span></code>.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.params.username"></span><strong>username</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.params.username">¶</a> – <p>string, default is no username.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.3.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.3.1.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.params.password"></span><strong>password</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.params.password">¶</a> – string, default is no password.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.params.port"></span><strong>port</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.params.port">¶</a> – integer, default is <code class="docutils literal notranslate"><span class="pre">6379</span></code>.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.params.db"></span><strong>db</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.params.db">¶</a> – integer, default is <code class="docutils literal notranslate"><span class="pre">0</span></code>.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.params.redis_expiration_time"></span><strong>redis_expiration_time</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.params.redis_expiration_time">¶</a> – integer, number of seconds after setting
 a value that Redis should expire it.  This should be larger than dogpile’s
@@ -2602,27 +2606,27 @@
 Redis should expire it.  This argument is only valid when
 <code class="docutils literal notranslate"><span class="pre">distributed_lock</span></code> is <code class="docutils literal notranslate"><span class="pre">True</span></code>.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.params.socket_timeout"></span><strong>socket_timeout</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.params.socket_timeout">¶</a> – float, seconds for socket timeout.
 Default is None (no timeout).</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.params.socket_connect_timeout"></span><strong>socket_connect_timeout</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.params.socket_connect_timeout">¶</a> – <p>float, seconds for socket connection
 timeout. Default is None (no timeout).</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.3.2.</span></p>
+<p><span class="versionmodified added">Added in version 1.3.2.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.params.socket_keepalive"></span><strong>socket_keepalive</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.params.socket_keepalive">¶</a> – <p>boolean, when True, socket keepalive is enabled.
 Default is False.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.3.2.</span></p>
+<p><span class="versionmodified added">Added in version 1.3.2.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.params.socket_keepalive_options"></span><strong>socket_keepalive_options</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.params.socket_keepalive_options">¶</a> – <p>dict, socket keepalive options.
 Default is None (no options).</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.3.2.</span></p>
+<p><span class="versionmodified added">Added in version 1.3.2.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.params.lock_sleep"></span><strong>lock_sleep</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.params.lock_sleep">¶</a> – integer, number of seconds to sleep when failed to
 acquire a lock.  This argument is only valid when
 <code class="docutils literal notranslate"><span class="pre">distributed_lock</span></code> is <code class="docutils literal notranslate"><span class="pre">True</span></code>.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.params.connection_pool"></span><strong>connection_pool</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.params.connection_pool">¶</a> – <code class="docutils literal notranslate"><span class="pre">redis.ConnectionPool</span></code> object.  If provided,
 this object supersedes other connection arguments passed to the
@@ -2635,15 +2639,15 @@
 used to create the lock.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.params.connection_kwargs"></span><strong>connection_kwargs</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.params.connection_kwargs">¶</a> – <p>dict, additional keyword arguments are passed
 along to the
 <code class="docutils literal notranslate"><span class="pre">StrictRedis.from_url()</span></code> method or <code class="docutils literal notranslate"><span class="pre">StrictRedis()</span></code> constructor
 directly, including parameters like <code class="docutils literal notranslate"><span class="pre">ssl</span></code>, <code class="docutils literal notranslate"><span class="pre">ssl_certfile</span></code>,
 <code class="docutils literal notranslate"><span class="pre">charset</span></code>, etc.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.6.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.6.</span></p>
 </div>
 </p></li>
 </ul>
 </dd>
 </dl>
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.redis.RedisBackend.delete">
@@ -2675,15 +2679,15 @@
 </dd>
 </dl>
 <p>The behavior here should be idempotent,
 that is, can be called any number of times
 regardless of whether or not the
 key exists.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.redis.RedisBackend.get_mutex">
 <span class="sig-name descname"><span class="pre">get_mutex</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.redis.RedisBackend.get_mutex" title="Link to this definition">¶</a></dt>
 <dd><p>Return an optional mutexing object for the given key.</p>
@@ -2724,15 +2728,15 @@
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>a bytes object, or <a class="reference internal" href="#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">NO_VALUE</span></code></a>
 constant if not present.</p>
 </dd>
 </dl>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.redis.RedisBackend.get_serialized_multi">
 <span class="sig-name descname"><span class="pre">get_serialized_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.redis.RedisBackend.get_serialized_multi" title="Link to this definition">¶</a></dt>
 <dd><p>Retrieve multiple serialized values from the cache.</p>
@@ -2743,15 +2747,15 @@
 by the “key mangling” function if one was present.</p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>list of bytes objects</p>
 </dd>
 </dl>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.redis.RedisBackend.set_serialized">
 <span class="sig-name descname"><span class="pre">set_serialized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.redis.RedisBackend.set_serialized" title="Link to this definition">¶</a></dt>
 <dd><p>Set a serialized value in the cache.</p>
@@ -2762,15 +2766,15 @@
 method, which will also be processed by the “key mangling” function
 if one was present.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisBackend.set_serialized.params.value"></span><strong>value</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisBackend.set_serialized.params.value">¶</a> – a bytes object to be stored.</p></li>
 </ul>
 </dd>
 </dl>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.redis.RedisBackend.set_serialized_multi">
 <span class="sig-name descname"><span class="pre">set_serialized_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">mapping</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.redis.RedisBackend.set_serialized_multi" title="Link to this definition">¶</a></dt>
 <dd><p>Set multiple serialized values in the cache.</p>
@@ -2785,15 +2789,15 @@
 <a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a>, be aware that when this method is invoked by
 <code class="xref py py-meth docutils literal notranslate"><span class="pre">Region.get_or_create_multi()</span></code>, the <code class="docutils literal notranslate"><span class="pre">mapping</span></code> values are the
 same ones returned to the upstream caller. If the subclass alters the
 values in any way, it must not do so ‘in-place’ on the <code class="docutils literal notranslate"><span class="pre">mapping</span></code> dict
 – that will have the undesirable effect of modifying the returned
 values as well.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="dogpile.cache.backends.redis.RedisClusterBackend">
@@ -2808,15 +2812,15 @@
 <div class="admonition seealso">
 <p class="admonition-title">See also</p>
 <p><a class="reference external" href="https://redis.readthedocs.io/en/stable/clustering.html">Clustering</a>
 in the redis-py documentation.</p>
 </div>
 <p>Requires redis-py version &gt;=4.1.0.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.3.2.</span></p>
+<p><span class="versionmodified added">Added in version 1.3.2.</span></p>
 </div>
 <p>Connecting to the cluster requires one of:</p>
 <ul class="simple">
 <li><p>Passing a list of startup nodes</p></li>
 <li><p>Passing only one node of the cluster, Redis will use automatic discovery
 to find the other nodes.</p></li>
 </ul>
@@ -2926,15 +2930,15 @@
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.backends.redis.</span></span><span class="sig-name descname"><span class="pre">RedisSentinelBackend</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">arguments</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.redis.RedisSentinelBackend" title="Link to this definition">¶</a></dt>
 <dd><p>Bases: <a class="reference internal" href="#dogpile.cache.backends.redis.RedisBackend" title="dogpile.cache.backends.redis.RedisBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">RedisBackend</span></code></a></p>
 <p>A <a class="reference external" href="http://redis.io/">Redis</a> backend, using the
 <a class="reference external" href="http://pypi.python.org/pypi/redis/">redis-py</a> driver.
 This backend is to be used when using
 <a class="reference external" href="https://redis.io/docs/management/sentinel/">Redis Sentinel</a>.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.0.0.</span></p>
+<p><span class="versionmodified added">Added in version 1.0.0.</span></p>
 </div>
 <p>Example configuration:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="kn">from</span> <span class="nn">dogpile.cache</span> <span class="kn">import</span> <span class="n">make_region</span>
 
 <span class="n">region</span> <span class="o">=</span> <span class="n">make_region</span><span class="p">()</span><span class="o">.</span><span class="n">configure</span><span class="p">(</span>
     <span class="s1">&#39;dogpile.cache.redis_sentinel&#39;</span><span class="p">,</span>
     <span class="n">arguments</span> <span class="o">=</span> <span class="p">{</span>
@@ -2952,15 +2956,15 @@
 </div>
 <p>Arguments accepted in the arguments dictionary:</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisSentinelBackend.params.username"></span><strong>username</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisSentinelBackend.params.username">¶</a> – <p>string, default is no username.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.3.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.3.1.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisSentinelBackend.params.password"></span><strong>password</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisSentinelBackend.params.password">¶</a> – string, default is no password.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisSentinelBackend.params.db"></span><strong>db</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisSentinelBackend.params.db">¶</a> – integer, default is <code class="docutils literal notranslate"><span class="pre">0</span></code>.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisSentinelBackend.params.redis_expiration_time"></span><strong>redis_expiration_time</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisSentinelBackend.params.redis_expiration_time">¶</a> – integer, number of seconds after setting
 a value that Redis should expire it.  This should be larger than dogpile’s
 cache expiration.  By default no expiration is set.</p></li>
@@ -2970,27 +2974,27 @@
 coordinate on a regular threading mutex, Default is True.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisSentinelBackend.params.lock_timeout"></span><strong>lock_timeout</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisSentinelBackend.params.lock_timeout">¶</a> – integer, number of seconds after acquiring a lock that
 Redis should expire it.  This argument is only valid when
 <code class="docutils literal notranslate"><span class="pre">distributed_lock</span></code> is <code class="docutils literal notranslate"><span class="pre">True</span></code>.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisSentinelBackend.params.socket_timeout"></span><strong>socket_timeout</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisSentinelBackend.params.socket_timeout">¶</a> – <p>float, seconds for socket timeout.
 Default is None (no timeout).</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.3.2.</span></p>
+<p><span class="versionmodified added">Added in version 1.3.2.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisSentinelBackend.params.socket_connect_timeout"></span><strong>socket_connect_timeout</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisSentinelBackend.params.socket_connect_timeout">¶</a> – <p>float, seconds for socket connection
 timeout.  Default is None (no timeout).</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.3.2.</span></p>
+<p><span class="versionmodified added">Added in version 1.3.2.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisSentinelBackend.params.socket_keepalive"></span><strong>socket_keepalive</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisSentinelBackend.params.socket_keepalive">¶</a> – <p>boolean, when True, socket keepalive is enabled
 Default is False.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.3.2.</span></p>
+<p><span class="versionmodified added">Added in version 1.3.2.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisSentinelBackend.params.socket_keepalive_options"></span><strong>socket_keepalive_options</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisSentinelBackend.params.socket_keepalive_options">¶</a> – dict, socket keepalive options.
 Default is {} (no options).</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.redis.RedisSentinelBackend.params.sentinels"></span><strong>sentinels</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.redis.RedisSentinelBackend.params.sentinels">¶</a> – is a list of sentinel nodes. Each node is represented by
 a pair (hostname, port).
 Default is None (not in sentinel mode).</p></li>
@@ -3222,15 +3226,15 @@
 <span class="p">)</span>
 </pre></div>
 </div>
 <p>While the included <a class="reference internal" href="#dogpile.cache.backends.file.FileLock" title="dogpile.cache.backends.file.FileLock"><code class="xref py py-class docutils literal notranslate"><span class="pre">FileLock</span></code></a> uses <code class="docutils literal notranslate"><span class="pre">os.flock()</span></code>, a
 windows-compatible implementation can be built using a library
 such as <a class="reference external" href="https://pypi.python.org/pypi/portalocker">portalocker</a>.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.2.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.2.</span></p>
 </div>
 </p></li>
 </ul>
 </dd>
 </dl>
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.file.DBMBackend.delete">
@@ -3262,15 +3266,15 @@
 </dd>
 </dl>
 <p>The behavior here should be idempotent,
 that is, can be called any number of times
 regardless of whether or not the
 key exists.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.file.DBMBackend.get_mutex">
 <span class="sig-name descname"><span class="pre">get_mutex</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.file.DBMBackend.get_mutex" title="Link to this definition">¶</a></dt>
 <dd><p>Return an optional mutexing object for the given key.</p>
@@ -3311,15 +3315,15 @@
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>a bytes object, or <a class="reference internal" href="#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">NO_VALUE</span></code></a>
 constant if not present.</p>
 </dd>
 </dl>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.file.DBMBackend.get_serialized_multi">
 <span class="sig-name descname"><span class="pre">get_serialized_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.file.DBMBackend.get_serialized_multi" title="Link to this definition">¶</a></dt>
 <dd><p>Retrieve multiple serialized values from the cache.</p>
@@ -3330,15 +3334,15 @@
 by the “key mangling” function if one was present.</p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>list of bytes objects</p>
 </dd>
 </dl>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.file.DBMBackend.set_serialized">
 <span class="sig-name descname"><span class="pre">set_serialized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.file.DBMBackend.set_serialized" title="Link to this definition">¶</a></dt>
 <dd><p>Set a serialized value in the cache.</p>
@@ -3349,15 +3353,15 @@
 method, which will also be processed by the “key mangling” function
 if one was present.</p></li>
 <li><p><span class="target" id="dogpile.cache.backends.file.DBMBackend.set_serialized.params.value"></span><strong>value</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.backends.file.DBMBackend.set_serialized.params.value">¶</a> – a bytes object to be stored.</p></li>
 </ul>
 </dd>
 </dl>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.file.DBMBackend.set_serialized_multi">
 <span class="sig-name descname"><span class="pre">set_serialized_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">mapping</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.file.DBMBackend.set_serialized_multi" title="Link to this definition">¶</a></dt>
 <dd><p>Set multiple serialized values in the cache.</p>
@@ -3372,15 +3376,15 @@
 <a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a>, be aware that when this method is invoked by
 <code class="xref py py-meth docutils literal notranslate"><span class="pre">Region.get_or_create_multi()</span></code>, the <code class="docutils literal notranslate"><span class="pre">mapping</span></code> values are the
 same ones returned to the upstream caller. If the subclass alters the
 values in any way, it must not do so ‘in-place’ on the <code class="docutils literal notranslate"><span class="pre">mapping</span></code> dict
 – that will have the undesirable effect of modifying the returned
 values as well.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="dogpile.cache.backends.file.FileLock">
@@ -3431,15 +3435,15 @@
 
 <section id="proxy-backends">
 <span id="module-dogpile.cache.proxy"></span><h3>Proxy Backends<a class="headerlink" href="#proxy-backends" title="Link to this heading">¶</a></h3>
 <p>Provides a utility and a decorator class that allow for modifying the behavior
 of different backends without altering the class itself or having to extend the
 base backend.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0: </span>Added support for the <a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a> class.</p>
+<p><span class="versionmodified added">Added in version 0.5.0: </span>Added support for the <a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a> class.</p>
 </div>
 </section>
 <dl class="py class">
 <dt class="sig sig-object py" id="dogpile.cache.proxy.ProxyBackend">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.proxy.</span></span><span class="sig-name descname"><span class="pre">ProxyBackend</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="o"><span class="pre">*</span></span><span class="n"><span class="pre">arg</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kw</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend" title="Link to this definition">¶</a></dt>
 <dd><p>Bases: <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a></p>
 <p>A decorator class for altering the functionality of backends.</p>
@@ -3474,15 +3478,15 @@
 </div>
 <p>Classes that extend <a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a> can be stacked
 together.  The <code class="docutils literal notranslate"><span class="pre">.proxied</span></code> property will always
 point to either the concrete backend instance or
 the next proxy in the chain that a method can be
 delegated towards.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.0.</span></p>
 </div>
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.proxy.ProxyBackend.delete">
 <span class="sig-name descname"><span class="pre">delete</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.delete" title="Link to this definition">¶</a></dt>
 <dd><p>Delete a value from the cache.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
@@ -3510,21 +3514,21 @@
 </dd>
 </dl>
 <p>The behavior here should be idempotent,
 that is, can be called any number of times
 regardless of whether or not the
 key exists.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.proxy.ProxyBackend.get">
-<span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">bytes</span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.get" title="Link to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Literal</span><span class="p"><span class="pre">[</span></span><span class="pre">NoValue.NO_VALUE</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">bytes</span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.get" title="Link to this definition">¶</a></dt>
 <dd><p>Retrieve an optionally serialized value from the cache.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.proxy.ProxyBackend.get.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.proxy.ProxyBackend.get.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get" title="dogpile.cache.region.CacheRegion.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p>
 </dd>
@@ -3536,15 +3540,15 @@
 </dl>
 <p>If a serializer is in use, this method will only be called if the
 <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get_serialized" title="dogpile.cache.api.CacheBackend.get_serialized"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get_serialized()</span></code></a> method is not overridden.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.proxy.ProxyBackend.get_multi">
-<span class="sig-name descname"><span class="pre">get_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.get_multi" title="Link to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Literal</span><span class="p"><span class="pre">[</span></span><span class="pre">NoValue.NO_VALUE</span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">bytes</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.get_multi" title="Link to this definition">¶</a></dt>
 <dd><p>Retrieve multiple optionally serialized values from the cache.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.proxy.ProxyBackend.get_multi.params.keys"></span><strong>keys</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.proxy.ProxyBackend.get_multi.params.keys">¶</a> – sequence of string keys that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_multi" title="dogpile.cache.region.CacheRegion.get_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_multi()</span></code></a> method, which will also be processed
 by the “key mangling” function if one was present.</p>
 </dd>
@@ -3553,15 +3557,15 @@
 <dt>:return a list of values as would be returned</dt><dd><p>individually via the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get" title="dogpile.cache.api.CacheBackend.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get()</span></code></a> method, corresponding
 to the list of keys given.</p>
 </dd>
 </dl>
 <p>If a serializer is in use, this method will only be called if the
 <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get_serialized_multi" title="dogpile.cache.api.CacheBackend.get_serialized_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get_serialized_multi()</span></code></a> method is not overridden.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.proxy.ProxyBackend.get_mutex">
 <span class="sig-name descname"><span class="pre">get_mutex</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="#dogpile.cache.api.CacheMutex" title="dogpile.cache.api.CacheMutex"><span class="pre">CacheMutex</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.get_mutex" title="Link to this definition">¶</a></dt>
 <dd><p>Return an optional mutexing object for the given key.</p>
@@ -3588,15 +3592,15 @@
 can be used as a means of throttling the total
 number of value recreation operations that may
 proceed at one time.</p>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.proxy.ProxyBackend.get_serialized">
-<span class="sig-name descname"><span class="pre">get_serialized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">bytes</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.get_serialized" title="Link to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get_serialized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">bytes</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Literal</span><span class="p"><span class="pre">[</span></span><span class="pre">NoValue.NO_VALUE</span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.get_serialized" title="Link to this definition">¶</a></dt>
 <dd><p>Retrieve a serialized value from the cache.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.proxy.ProxyBackend.get_serialized.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.proxy.ProxyBackend.get_serialized.params.key">¶</a> – String key that was passed to the <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get" title="dogpile.cache.region.CacheRegion.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get()</span></code></a>
 method, which will also be processed by the “key mangling” function
 if one was present.</p>
 </dd>
@@ -3604,40 +3608,40 @@
 <dd class="field-even"><p>a bytes object, or <a class="reference internal" href="#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">NO_VALUE</span></code></a>
 constant if not present.</p>
 </dd>
 </dl>
 <p>The default implementation of this method for <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a>
 returns the value of the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get" title="dogpile.cache.api.CacheBackend.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get()</span></code></a> method.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 <div class="admonition seealso">
 <p class="admonition-title">See also</p>
 <p><a class="reference internal" href="#dogpile.cache.api.BytesBackend" title="dogpile.cache.api.BytesBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">BytesBackend</span></code></a></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.proxy.ProxyBackend.get_serialized_multi">
-<span class="sig-name descname"><span class="pre">get_serialized_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">bytes</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.get_serialized_multi" title="Link to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">get_serialized_multi</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">keys</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><span class="pre">bytes</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Literal</span><span class="p"><span class="pre">[</span></span><span class="pre">NoValue.NO_VALUE</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.get_serialized_multi" title="Link to this definition">¶</a></dt>
 <dd><p>Retrieve multiple serialized values from the cache.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><p><span class="target" id="dogpile.cache.proxy.ProxyBackend.get_serialized_multi.params.keys"></span><strong>keys</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.proxy.ProxyBackend.get_serialized_multi.params.keys">¶</a> – sequence of string keys that was passed to the
 <a class="reference internal" href="#dogpile.cache.region.CacheRegion.get_multi" title="dogpile.cache.region.CacheRegion.get_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get_multi()</span></code></a> method, which will also be processed
 by the “key mangling” function if one was present.</p>
 </dd>
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>list of bytes objects</p>
 </dd>
 </dl>
 <p>The default implementation of this method for <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a>
 returns the value of the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get_multi" title="dogpile.cache.api.CacheBackend.get_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get_multi()</span></code></a> method.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 <div class="admonition seealso">
 <p class="admonition-title">See also</p>
 <p><a class="reference internal" href="#dogpile.cache.api.BytesBackend" title="dogpile.cache.api.BytesBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">BytesBackend</span></code></a></p>
 </div>
 </dd></dl>
 
@@ -3681,15 +3685,15 @@
 same ones returned to the upstream caller. If the subclass alters the
 values in any way, it must not do so ‘in-place’ on the <code class="docutils literal notranslate"><span class="pre">mapping</span></code> dict
 – that will have the undesirable effect of modifying the returned
 values as well.</p>
 <p>If a serializer is in use, this method will only be called if the
 <a class="reference internal" href="#dogpile.cache.api.CacheBackend.set_serialized_multi" title="dogpile.cache.api.CacheBackend.set_serialized_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.set_serialized_multi()</span></code></a> method is not overridden.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.proxy.ProxyBackend.set_serialized">
 <span class="sig-name descname"><span class="pre">set_serialized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">value</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bytes</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">None</span></span></span><a class="headerlink" href="#dogpile.cache.proxy.ProxyBackend.set_serialized" title="Link to this definition">¶</a></dt>
 <dd><p>Set a serialized value in the cache.</p>
@@ -3702,15 +3706,15 @@
 <li><p><span class="target" id="dogpile.cache.proxy.ProxyBackend.set_serialized.params.value"></span><strong>value</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.proxy.ProxyBackend.set_serialized.params.value">¶</a> – a bytes object to be stored.</p></li>
 </ul>
 </dd>
 </dl>
 <p>The default implementation of this method for <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a>
 calls upon the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.set" title="dogpile.cache.api.CacheBackend.set"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.set()</span></code></a> method.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 <div class="admonition seealso">
 <p class="admonition-title">See also</p>
 <p><a class="reference internal" href="#dogpile.cache.api.BytesBackend" title="dogpile.cache.api.BytesBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">BytesBackend</span></code></a></p>
 </div>
 </dd></dl>
 
@@ -3729,15 +3733,15 @@
 <a class="reference internal" href="#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a>, be aware that when this method is invoked by
 <code class="xref py py-meth docutils literal notranslate"><span class="pre">Region.get_or_create_multi()</span></code>, the <code class="docutils literal notranslate"><span class="pre">mapping</span></code> values are the
 same ones returned to the upstream caller. If the subclass alters the
 values in any way, it must not do so ‘in-place’ on the <code class="docutils literal notranslate"><span class="pre">mapping</span></code> dict
 – that will have the undesirable effect of modifying the returned
 values as well.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.</span></p>
 </div>
 <p>The default implementation of this method for <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a>
 calls upon the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.set_multi" title="dogpile.cache.api.CacheBackend.set_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.set_multi()</span></code></a> method.</p>
 <div class="admonition seealso">
 <p class="admonition-title">See also</p>
 <p><a class="reference internal" href="#dogpile.cache.api.BytesBackend" title="dogpile.cache.api.BytesBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">BytesBackend</span></code></a></p>
 </div>
@@ -3755,15 +3759,15 @@
 
 <section id="null-backend">
 <span id="module-dogpile.cache.backends.null"></span><h3>Null Backend<a class="headerlink" href="#null-backend" title="Link to this heading">¶</a></h3>
 <p>The Null backend does not do any caching at all.  It can be
 used to test behavior without caching, or as a means of disabling
 caching for a region that is otherwise used normally.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.4.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.4.</span></p>
 </div>
 </section>
 <dl class="py class">
 <dt class="sig sig-object py" id="dogpile.cache.backends.null.NullBackend">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.backends.null.</span></span><span class="sig-name descname"><span class="pre">NullBackend</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">arguments</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.null.NullBackend" title="Link to this definition">¶</a></dt>
 <dd><p>Bases: <a class="reference internal" href="#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a></p>
 <p>A “null” backend that effectively disables all cache operations.</p>
@@ -3805,15 +3809,15 @@
 </dd>
 </dl>
 <p>The behavior here should be idempotent,
 that is, can be called any number of times
 regardless of whether or not the
 key exists.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.null.NullBackend.get">
 <span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.null.NullBackend.get" title="Link to this definition">¶</a></dt>
 <dd><p>Retrieve an optionally serialized value from the cache.</p>
@@ -3848,15 +3852,15 @@
 <dt>:return a list of values as would be returned</dt><dd><p>individually via the <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get" title="dogpile.cache.api.CacheBackend.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get()</span></code></a> method, corresponding
 to the list of keys given.</p>
 </dd>
 </dl>
 <p>If a serializer is in use, this method will only be called if the
 <a class="reference internal" href="#dogpile.cache.api.CacheBackend.get_serialized_multi" title="dogpile.cache.api.CacheBackend.get_serialized_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.get_serialized_multi()</span></code></a> method is not overridden.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py method">
 <dt class="sig sig-object py" id="dogpile.cache.backends.null.NullBackend.get_mutex">
 <span class="sig-name descname"><span class="pre">get_mutex</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#dogpile.cache.backends.null.NullBackend.get_mutex" title="Link to this definition">¶</a></dt>
 <dd><p>Return an optional mutexing object for the given key.</p>
@@ -3925,15 +3929,15 @@
 same ones returned to the upstream caller. If the subclass alters the
 values in any way, it must not do so ‘in-place’ on the <code class="docutils literal notranslate"><span class="pre">mapping</span></code> dict
 – that will have the undesirable effect of modifying the returned
 values as well.</p>
 <p>If a serializer is in use, this method will only be called if the
 <a class="reference internal" href="#dogpile.cache.api.CacheBackend.set_serialized_multi" title="dogpile.cache.api.CacheBackend.set_serialized_multi"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheBackend.set_serialized_multi()</span></code></a> method is not overridden.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.0.</span></p>
 </div>
 </dd></dl>
 
 </dd></dl>
 
 </section>
 <section id="module-dogpile.cache.exception">
@@ -3948,15 +3952,15 @@
 
 <dl class="py exception">
 <dt class="sig sig-object py" id="dogpile.cache.exception.PluginNotFound">
 <em class="property"><span class="pre">exception</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.exception.</span></span><span class="sig-name descname"><span class="pre">PluginNotFound</span></span><a class="headerlink" href="#dogpile.cache.exception.PluginNotFound" title="Link to this definition">¶</a></dt>
 <dd><p>Bases: <a class="reference internal" href="#dogpile.cache.exception.DogpileCacheException" title="dogpile.cache.exception.DogpileCacheException"><code class="xref py py-class docutils literal notranslate"><span class="pre">DogpileCacheException</span></code></a></p>
 <p>The specified plugin could not be found.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.6.4.</span></p>
+<p><span class="versionmodified added">Added in version 0.6.4.</span></p>
 </div>
 </dd></dl>
 
 <dl class="py exception">
 <dt class="sig sig-object py" id="dogpile.cache.exception.RegionAlreadyConfigured">
 <em class="property"><span class="pre">exception</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">dogpile.cache.exception.</span></span><span class="sig-name descname"><span class="pre">RegionAlreadyConfigured</span></span><a class="headerlink" href="#dogpile.cache.exception.RegionAlreadyConfigured" title="Link to this definition">¶</a></dt>
 <dd><p>Bases: <a class="reference internal" href="#dogpile.cache.exception.DogpileCacheException" title="dogpile.cache.exception.DogpileCacheException"><code class="xref py py-class docutils literal notranslate"><span class="pre">DogpileCacheException</span></code></a></p>
@@ -4107,15 +4111,15 @@
 arguments to the returned function itself.</p>
 <p>For kwargs passed in, we will build a dict of
 all argname (key) argvalue (values) including
 default args from the argspec and then
 alphabetize the list before generating the
 key.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.6.2.</span></p>
+<p><span class="versionmodified added">Added in version 0.6.2.</span></p>
 </div>
 <div class="admonition seealso">
 <p class="admonition-title">See also</p>
 <p><a class="reference internal" href="#dogpile.cache.util.function_key_generator" title="dogpile.cache.util.function_key_generator"><code class="xref py py-func docutils literal notranslate"><span class="pre">function_key_generator()</span></code></a> - default key generation function</p>
 </div>
 </dd></dl>
 
@@ -4534,23 +4538,23 @@
 </ul>
 </li>
 </ul>
 </li>
 </ul>
 
   </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
   <div>
     <h4>Previous topic</h4>
     <p class="topless"><a href="core_usage.html"
                           title="previous chapter">dogpile Core</a></p>
   </div>
   <div>
@@ -4573,17 +4577,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="changelog.html" title="Changelog"
              >next</a> |</li>
         <li class="right" >
           <a href="core_usage.html" title="dogpile Core"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">API</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
     &#169; Copyright 2011-2024 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.2.6.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.3.7.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 ******** NNaavviiggaattiioonn ********
     * _i_n_d_e_x
     * _m_o_d_u_l_e_s |
     * _n_e_x_t |
     * _p_r_e_v_i_o_u_s |
-    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._2_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
+    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._3_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
     * API
 ************ AAPPII_?¶ ************
 ********** RReeggiioonn_?¶ **********
   ccllaassss dogpile.cache.region.CacheRegion(nnaammee:: ssttrr || NNoonnee == NNoonnee,,
   ffuunnccttiioonn__kkeeyy__ggeenneerraattoorr:: ~~ttyyppiinngg..CCaallllaabbllee[[[[......]],, ~~ttyyppiinngg..CCaallllaabbllee[[[[......]],, ssttrr]]]]
   == <<ffuunnccttiioonn ffuunnccttiioonn__kkeeyy__ggeenneerraattoorr>>,, ffuunnccttiioonn__mmuullttii__kkeeyy__ggeenneerraattoorr::
   ~~ttyyppiinngg..CCaallllaabbllee[[[[......]],, ~~ttyyppiinngg..CCaallllaabbllee[[[[......]],, ~~ttyyppiinngg..SSeeqquueennccee[[ssttrr]]]]]] ==
@@ -19,15 +19,15 @@
   || NNoonnee == NNoonnee)_¶
       Bases: object
       A front end to a particular cache backend.
         pprrooppeerrttyy actual_backend_¶
             Return the ultimate backend underneath any proxies.
             The backend might be the result of one or more proxy.wrap
             applications. If so, derive the actual underlying backend.
-            New in version 0.6.6.
+            Added in version 0.6.6.
         cache_multi_on_arguments(nnaammeessppaaccee:: ssttrr || NNoonnee == NNoonnee,, eexxppiirraattiioonn__ttiimmee::
         ffllooaatt || ~~ttyyppiinngg..CCaallllaabbllee[[[[]],, ffllooaatt]] || NNoonnee == NNoonnee,, sshhoouulldd__ccaacchhee__ffnn::
         ~~ttyyppiinngg..CCaallllaabbllee[[[[~~ttyyppiinngg..AAnnyy]],, bbooooll]] || NNoonnee == NNoonnee,, aassddiicctt:: bbooooll ==
         FFaallssee,, ttoo__ssttrr:: ~~ttyyppiinngg..CCaallllaabbllee[[[[~~ttyyppiinngg..AAnnyy]],, ssttrr]] == <<ccllaassss ''ssttrr''>>,,
         ffuunnccttiioonn__mmuullttii__kkeeyy__ggeenneerraattoorr:: ~~ttyyppiinngg..CCaallllaabbllee[[[[......]],, ~~ttyyppiinngg..CCaallllaabbllee[[
         [[......]],, ~~ttyyppiinngg..SSeeqquueennccee[[ssttrr]]]]]] || NNoonnee == NNoonnee) → Callable[[Callable[
         [...], Sequence[Any]]], Callable[[...], Sequence[Any] | Mapping[str,
@@ -75,19 +75,19 @@
             generate_something.invalidate("k1", "k2", "k3")
             …a refresh() method, which will call the creation function, cache
             the new values, and return them:
             values = generate_something.refresh("k1", "k2", "k3")
             …and a get() method, which will return values based on the given
             arguments:
             values = generate_something.get("k1", "k2", "k3")
-            New in version 0.5.3: Added get() method to decorated function.
+            Added in version 0.5.3: Added get() method to decorated function.
             Parameters passed to _C_a_c_h_e_R_e_g_i_o_n_._c_a_c_h_e___m_u_l_t_i___o_n___a_r_g_u_m_e_n_t_s_(_) have
             the same meaning as those passed to _C_a_c_h_e_R_e_g_i_o_n_._c_a_c_h_e___o_n___a_r_g_u_m_e_n_t_s
             _(_).
-            New in version 0.5.0.
+            Added in version 0.5.0.
             See also
             _C_a_c_h_e_R_e_g_i_o_n_._c_a_c_h_e___o_n___a_r_g_u_m_e_n_t_s_(_)
             _C_a_c_h_e_R_e_g_i_o_n_._g_e_t___o_r___c_r_e_a_t_e___m_u_l_t_i_(_)
         cache_on_arguments(nnaammeessppaaccee:: ssttrr || NNoonnee == NNoonnee,, eexxppiirraattiioonn__ttiimmee:: ffllooaatt
         || ~~ttyyppiinngg..CCaallllaabbllee[[[[]],, ffllooaatt]] || NNoonnee == NNoonnee,, sshhoouulldd__ccaacchhee__ffnn::
         ~~ttyyppiinngg..CCaallllaabbllee[[[[~~ttyyppiinngg..AAnnyy]],, bbooooll]] || NNoonnee == NNoonnee,, ttoo__ssttrr::
         ~~ttyyppiinngg..CCaallllaabbllee[[[[~~ttyyppiinngg..AAnnyy]],, ssttrr]] == <<ccllaassss ''ssttrr''>>,,
@@ -118,29 +118,30 @@
             directly without calling the decorated function. The value to be
             cached is passed as the first argument, and the arguments which
             would normally be passed to the function should follow:
             generate_something.set(3, 5, 6)
             The above example is equivalent to calling generate_something(5,
             6), if the function were to produce the value 3 as the value to be
             cached.
-            New in version 0.4.1: Added set() method to decorated function.
+            Added in version 0.4.1: Added set() method to decorated function.
             Similar to set() is refresh(). This attribute will invoke the
             decorated function and populate a new value into the cache with the
             new value, as well as returning that value:
             newvalue = generate_something.refresh(5, 6)
-            New in version 0.5.0: Added refresh() method to decorated function.
+            Added in version 0.5.0: Added refresh() method to decorated
+            function.
             original() on other hand will invoke the decorated function without
             any caching:
             newvalue = generate_something.original(5, 6)
-            New in version 0.6.0: Added original() method to decorated
+            Added in version 0.6.0: Added original() method to decorated
             function.
             Lastly, the get() method returns either the value cached for the
             given key, or the token NO_VALUE if no such key exists:
             value = generate_something.get(5, 6)
-            New in version 0.5.3: Added get() method to decorated function.
+            Added in version 0.5.3: Added get() method to decorated function.
             The default key generation will use the name of the function, the
             module name for the function, the arguments passed, as well as an
             optional “namespace” parameter in order to generate a cache key.
             Given a function one inside the module myapp.tools:
             @region.cache_on_arguments(namespace="foo")
             def one(a, b):
                 return a + b
@@ -211,37 +212,37 @@
             Remove a value from the cache.
             This operation is idempotent (can be called multiple times, or on a
             non-existent key, safely)
         delete_multi(kkeeyyss:: SSeeqquueennccee[[ssttrr]]) → None_¶
             Remove multiple values from the cache.
             This operation is idempotent (can be called multiple times, or on a
             non-existent key, safely)
-            New in version 0.5.0.
+            Added in version 0.5.0.
         get(kkeeyy:: ssttrr, eexxppiirraattiioonn__ttiimmee:: ffllooaatt || NNoonnee == NNoonnee, iiggnnoorree__eexxppiirraattiioonn::
-        bbooooll == FFaallssee) → _C_a_c_h_e_d_V_a_l_u_e | _N_o_V_a_l_u_e_¶
+        bbooooll == FFaallssee) → Any | Literal[NoValue.NO_VALUE]_¶
             Return a value from the cache, based on the given key.
-            If the value is not present, the method returns the token NO_VALUE.
-            NO_VALUE evaluates to False, but is separate from None to
-            distinguish between a cached value of None.
+            If the value is not present, the method returns the token
+            _a_p_i_._N_O___V_A_L_U_E. _a_p_i_._N_O___V_A_L_U_E evaluates to False, but is separate from
+            None to distinguish between a cached value of None.
             By default, the configured expiration time of the _C_a_c_h_e_R_e_g_i_o_n, or
             alternatively the expiration time supplied by the expiration_time
             argument, is tested against the creation time of the retrieved
             value versus the current time (as reported by time.time()). If
-            stale, the cached value is ignored and the NO_VALUE token is
+            stale, the cached value is ignored and the _a_p_i_._N_O___V_A_L_U_E token is
             returned. Passing the flag ignore_expiration=True bypasses the
             expiration time check.
             Changed in version 0.3.0: _C_a_c_h_e_R_e_g_i_o_n_._g_e_t_(_) now checks the value’s
             creation time against the expiration time, rather than returning
             the value unconditionally.
             The method also interprets the cached value in terms of the current
             “invalidation” time as set by the _i_n_v_a_l_i_d_a_t_e_(_) method. If a value
             is present, but its creation time is older than the current
-            invalidation time, the NO_VALUE token is returned. Passing the flag
-            ignore_expiration=True bypasses the invalidation time check.
-            New in version 0.3.0: Support for the _C_a_c_h_e_R_e_g_i_o_n_._i_n_v_a_l_i_d_a_t_e_(_)
+            invalidation time, the _a_p_i_._N_O___V_A_L_U_E token is returned. Passing the
+            flag ignore_expiration=True bypasses the invalidation time check.
+            Added in version 0.3.0: Support for the _C_a_c_h_e_R_e_g_i_o_n_._i_n_v_a_l_i_d_a_t_e_(_)
             method.
             See also
             _C_a_c_h_e_R_e_g_i_o_n_._g_e_t___m_u_l_t_i_(_)
             _C_a_c_h_e_R_e_g_i_o_n_._g_e_t___o_r___c_r_e_a_t_e_(_)
             _C_a_c_h_e_R_e_g_i_o_n_._s_e_t_(_)
             _C_a_c_h_e_R_e_g_i_o_n_._d_e_l_e_t_e_(_)
         get_multi(kkeeyyss, eexxppiirraattiioonn__ttiimmee==NNoonnee, iiggnnoorree__eexxppiirraattiioonn==FFaallssee)_¶
@@ -259,15 +260,15 @@
             By default, the configured expiration time of the _C_a_c_h_e_R_e_g_i_o_n, or
             alternatively the expiration time supplied by the expiration_time
             argument, is tested against the creation time of the retrieved
             value versus the current time (as reported by time.time()). If
             stale, the cached value is ignored and the NO_VALUE token is
             returned. Passing the flag ignore_expiration=True bypasses the
             expiration time check.
-            New in version 0.5.0.
+            Added in version 0.5.0.
         get_or_create(kkeeyy:: ssttrr, ccrreeaattoorr:: CCaallllaabbllee[[[[......]],, AAnnyy]], eexxppiirraattiioonn__ttiimmee::
         ffllooaatt || NNoonnee == NNoonnee, sshhoouulldd__ccaacchhee__ffnn:: CCaallllaabbllee[[[[AAnnyy]],, bbooooll]] || NNoonnee ==
         NNoonnee, ccrreeaattoorr__aarrggss:: TTuuppllee[[AAnnyy,, MMaappppiinngg[[ssttrr,, AAnnyy]]]] || NNoonnee == NNoonnee) → Any_¶
             Return a cached value based on the given key.
             If the value does not exist or is considered to be expired based on
             its creation time, the given creation function may or may not be
             used to recreate the value and persist the newly generated value in
@@ -317,26 +318,26 @@
                         _C_a_c_h_e_R_e_g_i_o_n if not None. To set no expiration, use the
                         value -1.
                       * sshhoouulldd__ccaacchhee__ffnn_¶ – optional callable function which
                         will receive each value returned by the “creator”, and
                         will then return True or False, indicating if the value
                         should actually be cached or not. If it returns False,
                         the value is still returned, but isn’t cached.
-            New in version 0.5.0.
+            Added in version 0.5.0.
             See also
             _C_a_c_h_e_R_e_g_i_o_n_._c_a_c_h_e___m_u_l_t_i___o_n___a_r_g_u_m_e_n_t_s_(_)
             _C_a_c_h_e_R_e_g_i_o_n_._g_e_t___o_r___c_r_e_a_t_e_(_)
         get_value_metadata(kkeeyy:: ssttrr, eexxppiirraattiioonn__ttiimmee:: ffllooaatt || NNoonnee == NNoonnee,
         iiggnnoorree__eexxppiirraattiioonn:: bbooooll == FFaallssee) → _C_a_c_h_e_d_V_a_l_u_e | None_¶
             Return the _C_a_c_h_e_d_V_a_l_u_e object directly from the cache.
             This is the enclosing datastructure that includes the value as well
             as the metadata, including the timestamp when the value was cached.
             Convenience accessors on _C_a_c_h_e_d_V_a_l_u_e also provide for common data
             such as _C_a_c_h_e_d_V_a_l_u_e_._c_a_c_h_e_d___t_i_m_e and _C_a_c_h_e_d_V_a_l_u_e_._a_g_e.
-            New in version 1.3.: Added _C_a_c_h_e_R_e_g_i_o_n_._g_e_t___v_a_l_u_e___m_e_t_a_d_a_t_a_(_)
+            Added in version 1.3.: Added _C_a_c_h_e_R_e_g_i_o_n_._g_e_t___v_a_l_u_e___m_e_t_a_d_a_t_a_(_)
         invalidate(hhaarrdd==TTrruuee)_¶
             Invalidate this _C_a_c_h_e_R_e_g_i_o_n.
             The default invalidation system works by setting a current
             timestamp (using time.time()) representing the “minimum creation
             time” for a value. Any retrieved value whose creation time is prior
             to this timestamp is considered to be stale. It does not affect the
             data in the cache in any way, and is llooccaall ttoo tthhiiss iinnssttaannccee ooff ::
@@ -355,23 +356,23 @@
             The method supports both “hard” and “soft” invalidation options.
             With “hard” invalidation, _C_a_c_h_e_R_e_g_i_o_n_._g_e_t___o_r___c_r_e_a_t_e_(_) will force an
             immediate regeneration of the value which all getters will wait
             for. With “soft” invalidation, subsequent getters will return the
             “old” value until the new one is available.
             Usage of “soft” invalidation requires that the region or the method
             is given a non-None expiration time.
-            New in version 0.3.0.
+            Added in version 0.3.0.
         pprrooppeerrttyy is_configured_¶
             Return True if the backend has been configured via the
             _C_a_c_h_e_R_e_g_i_o_n_._c_o_n_f_i_g_u_r_e_(_) method already.
-            New in version 0.5.1.
+            Added in version 0.5.1.
         key_is_locked(kkeeyy:: ssttrr) → bool_¶
             Return True if a particular cache key is currently being generated
             within the dogpile lock.
-            New in version 1.1.2.
+            Added in version 1.1.2.
         set(kkeeyy:: ssttrr, vvaalluuee:: AAnnyy) → None_¶
             Place a new value in the cache under the given key.
         set_multi(mmaappppiinngg:: MMaappppiinngg[[ssttrr,, AAnnyy]]) → None_¶
             Place new values in the cache under the given keys.
         wrap(pprrooxxyy:: _PP_rr_oo_xx_yy_BB_aa_cc_kk_ee_nn_dd || TTyyppee[[_PP_rr_oo_xx_yy_BB_aa_cc_kk_ee_nn_dd]]) → None_¶
             Takes a ProxyBackend instance or class and wraps the attached
             backend.
@@ -457,15 +458,15 @@
               self.region = region
               # ...
 
           # ...
 
       region = CacheRegion()
       region = region.configure(region_invalidator=MyInvalidator(region))
-      New in version 0.6.2.
+      Added in version 0.6.2.
       See also
       _C_a_c_h_e_R_e_g_i_o_n_._c_o_n_f_i_g_u_r_e_._r_e_g_i_o_n___i_n_v_a_l_i_d_a_t_o_r
         invalidate(hhaarrdd:: bbooooll == TTrruuee) → None_¶
             Region invalidation.
             _C_a_c_h_e_R_e_g_i_o_n propagated call. The default invalidation system works
             by setting a current timestamp (using time.time()) to consider all
             older timestamps effectively invalidated.
@@ -502,66 +503,67 @@
       incompatible version.
 ********** BBaacckkeenndd AAPPII_?¶ **********
 See the section _C_r_e_a_t_i_n_g_ _B_a_c_k_e_n_d_s for details on how to register new backends
 or _C_h_a_n_g_i_n_g_ _B_a_c_k_e_n_d_ _B_e_h_a_v_i_o_r for details on how to alter the behavior of
 existing backends.
   dogpile.cache.api.BackendFormatted_¶
       Describes the type returned from the _C_a_c_h_e_B_a_c_k_e_n_d_._g_e_t_(_) method.
-      alias of Union[_C_a_c_h_e_d_V_a_l_u_e, _N_o_V_a_l_u_e, bytes]
+      alias of _C_a_c_h_e_d_V_a_l_u_e | Literal[NO_VALUE] | bytes
   dogpile.cache.api.BackendSetType_¶
       Describes the value argument passed to the _C_a_c_h_e_B_a_c_k_e_n_d_._s_e_t_(_) method.
-      alias of Union[_C_a_c_h_e_d_V_a_l_u_e, bytes]
+      alias of _C_a_c_h_e_d_V_a_l_u_e | bytes
   ccllaassss dogpile.cache.api.BytesBackend(aarrgguummeennttss:: MMaappppiinngg[[ssttrr,, AAnnyy]])_¶
       Bases: DefaultSerialization, _C_a_c_h_e_B_a_c_k_e_n_d
       A cache backend that receives and returns series of bytes.
       This backend only supports the “serialized” form of values; subclasses
       should implement _B_y_t_e_s_B_a_c_k_e_n_d_._g_e_t___s_e_r_i_a_l_i_z_e_d_(_),
       _B_y_t_e_s_B_a_c_k_e_n_d_._g_e_t___s_e_r_i_a_l_i_z_e_d___m_u_l_t_i_(_), _B_y_t_e_s_B_a_c_k_e_n_d_._s_e_t___s_e_r_i_a_l_i_z_e_d_(_),
       _B_y_t_e_s_B_a_c_k_e_n_d_._s_e_t___s_e_r_i_a_l_i_z_e_d___m_u_l_t_i_(_).
-      New in version 1.1.
-        get_serialized(kkeeyy:: ssttrr) → bytes | _N_o_V_a_l_u_e_¶
+      Added in version 1.1.
+        get_serialized(kkeeyy:: ssttrr) → bytes | Literal[NoValue.NO_VALUE]_¶
             Retrieve a serialized value from the cache.
               Parameters:
                   kkeeyy_¶ – String key that was passed to the _C_a_c_h_e_R_e_g_i_o_n_._g_e_t_(_)
                   method, which will also be processed by the “key mangling”
                   function if one was present.
               Returns:
                   a bytes object, or _N_O___V_A_L_U_E constant if not present.
-            New in version 1.1.
-        get_serialized_multi(kkeeyyss:: SSeeqquueennccee[[ssttrr]]) → Sequence[bytes | _N_o_V_a_l_u_e]_¶
+            Added in version 1.1.
+        get_serialized_multi(kkeeyyss:: SSeeqquueennccee[[ssttrr]]) → Sequence[bytes | Literal
+        [NoValue.NO_VALUE]]_¶
             Retrieve multiple serialized values from the cache.
               Parameters:
                   kkeeyyss_¶ – sequence of string keys that was passed to the
                   _C_a_c_h_e_R_e_g_i_o_n_._g_e_t___m_u_l_t_i_(_) method, which will also be processed
                   by the “key mangling” function if one was present.
               Returns:
                   list of bytes objects
-            New in version 1.1.
+            Added in version 1.1.
         set_serialized(kkeeyy:: ssttrr, vvaalluuee:: bbyytteess) → None_¶
             Set a serialized value in the cache.
               Parameters:
                       * kkeeyy_¶ – String key that was passed to the
                         _C_a_c_h_e_R_e_g_i_o_n_._s_e_t_(_) method, which will also be processed
                         by the “key mangling” function if one was present.
                       * vvaalluuee_¶ – a bytes object to be stored.
-            New in version 1.1.
+            Added in version 1.1.
         set_serialized_multi(mmaappppiinngg:: MMaappppiinngg[[ssttrr,, bbyytteess]]) → None_¶
             Set multiple serialized values in the cache.
               Parameters:
                   mmaappppiinngg_¶ – a dict in which the key will be whatever was
                   passed to the _C_a_c_h_e_R_e_g_i_o_n_._s_e_t___m_u_l_t_i_(_) method, processed by
                   the “key mangling” function, if any.
             When implementing a new _C_a_c_h_e_B_a_c_k_e_n_d or cutomizing via
             _P_r_o_x_y_B_a_c_k_e_n_d, be aware that when this method is invoked by
             Region.get_or_create_multi(), the mapping values are the same ones
             returned to the upstream caller. If the subclass alters the values
             in any way, it must not do so ‘in-place’ on the mapping dict – that
             will have the undesirable effect of modifying the returned values
             as well.
-            New in version 1.1.
+            Added in version 1.1.
   ccllaassss dogpile.cache.api.CacheBackend(aarrgguummeennttss:: MMaappppiinngg[[ssttrr,, AAnnyy]])_¶
       Bases: object
       Base class for backend implementations.
       Backends which set and get Python object values should subclass this
       backend. For backends in which the value that’s stored is ultimately a
       stream of bytes, the _B_y_t_e_s_B_a_c_k_e_n_d should be used.
         delete(kkeeyy:: ssttrr) → None_¶
@@ -576,44 +578,44 @@
             Delete multiple values from the cache.
               Parameters:
                   kkeeyyss_¶ – sequence of string keys that was passed to the
                   _C_a_c_h_e_R_e_g_i_o_n_._d_e_l_e_t_e___m_u_l_t_i_(_) method, which will also be
                   processed by the “key mangling” function if one was present.
             The behavior here should be idempotent, that is, can be called any
             number of times regardless of whether or not the key exists.
-            New in version 0.5.0.
+            Added in version 0.5.0.
         deserializer:: NNoonnee || CCaallllaabbllee[[[[bbyytteess]],, AAnnyy]] == NNoonnee_¶
             deserializer function that will be used by default if not
             overridden by the region.
-            New in version 1.1.
-        get(kkeeyy:: ssttrr) → _C_a_c_h_e_d_V_a_l_u_e | _N_o_V_a_l_u_e | bytes_¶
+            Added in version 1.1.
+        get(kkeeyy:: ssttrr) → _C_a_c_h_e_d_V_a_l_u_e | Literal[NoValue.NO_VALUE] | bytes_¶
             Retrieve an optionally serialized value from the cache.
               Parameters:
                   kkeeyy_¶ – String key that was passed to the _C_a_c_h_e_R_e_g_i_o_n_._g_e_t_(_)
                   method, which will also be processed by the “key mangling”
                   function if one was present.
               Returns:
                   the Python object that corresponds to what was established
                   via the _C_a_c_h_e_B_a_c_k_e_n_d_._s_e_t_(_) method, or the _N_O___V_A_L_U_E constant
                   if not present.
             If a serializer is in use, this method will only be called if the
             _C_a_c_h_e_B_a_c_k_e_n_d_._g_e_t___s_e_r_i_a_l_i_z_e_d_(_) method is not overridden.
-        get_multi(kkeeyyss:: SSeeqquueennccee[[ssttrr]]) → Sequence[_C_a_c_h_e_d_V_a_l_u_e | _N_o_V_a_l_u_e |
-        bytes]_¶
+        get_multi(kkeeyyss:: SSeeqquueennccee[[ssttrr]]) → Sequence[_C_a_c_h_e_d_V_a_l_u_e | Literal
+        [NoValue.NO_VALUE] | bytes]_¶
             Retrieve multiple optionally serialized values from the cache.
               Parameters:
                   kkeeyyss_¶ – sequence of string keys that was passed to the
                   _C_a_c_h_e_R_e_g_i_o_n_._g_e_t___m_u_l_t_i_(_) method, which will also be processed
                   by the “key mangling” function if one was present.
               :return a list of values as would be returned
                   individually via the _C_a_c_h_e_B_a_c_k_e_n_d_._g_e_t_(_) method, corresponding
                   to the list of keys given.
             If a serializer is in use, this method will only be called if the
             _C_a_c_h_e_B_a_c_k_e_n_d_._g_e_t___s_e_r_i_a_l_i_z_e_d___m_u_l_t_i_(_) method is not overridden.
-            New in version 0.5.0.
+            Added in version 0.5.0.
         get_mutex(kkeeyy:: ssttrr) → _C_a_c_h_e_M_u_t_e_x | None_¶
             Return an optional mutexing object for the given key.
             This object need only provide an acquire() and release() method.
             May return None, in which case the dogpile lock will use a regular
             threading.Lock object to mutex concurrent threads for value
             creation. The default implementation returns None.
             Different backends may want to provide various kinds of “mutex”
@@ -623,47 +625,48 @@
             A mutex that takes the key into account will allow multiple
             regenerate operations across keys to proceed simultaneously, while
             a mutex that does not will serialize regenerate operations to just
             one at a time across all keys in the region. The latter approach,
             or a variant that involves a modulus of the given key’s hash value,
             can be used as a means of throttling the total number of value
             recreation operations that may proceed at one time.
-        get_serialized(kkeeyy:: ssttrr) → bytes | _N_o_V_a_l_u_e_¶
+        get_serialized(kkeeyy:: ssttrr) → bytes | Literal[NoValue.NO_VALUE]_¶
             Retrieve a serialized value from the cache.
               Parameters:
                   kkeeyy_¶ – String key that was passed to the _C_a_c_h_e_R_e_g_i_o_n_._g_e_t_(_)
                   method, which will also be processed by the “key mangling”
                   function if one was present.
               Returns:
                   a bytes object, or _N_O___V_A_L_U_E constant if not present.
             The default implementation of this method for _C_a_c_h_e_B_a_c_k_e_n_d returns
             the value of the _C_a_c_h_e_B_a_c_k_e_n_d_._g_e_t_(_) method.
-            New in version 1.1.
+            Added in version 1.1.
             See also
             _B_y_t_e_s_B_a_c_k_e_n_d
-        get_serialized_multi(kkeeyyss:: SSeeqquueennccee[[ssttrr]]) → Sequence[bytes | _N_o_V_a_l_u_e]_¶
+        get_serialized_multi(kkeeyyss:: SSeeqquueennccee[[ssttrr]]) → Sequence[bytes | Literal
+        [NoValue.NO_VALUE]]_¶
             Retrieve multiple serialized values from the cache.
               Parameters:
                   kkeeyyss_¶ – sequence of string keys that was passed to the
                   _C_a_c_h_e_R_e_g_i_o_n_._g_e_t___m_u_l_t_i_(_) method, which will also be processed
                   by the “key mangling” function if one was present.
               Returns:
                   list of bytes objects
             The default implementation of this method for _C_a_c_h_e_B_a_c_k_e_n_d returns
             the value of the _C_a_c_h_e_B_a_c_k_e_n_d_._g_e_t___m_u_l_t_i_(_) method.
-            New in version 1.1.
+            Added in version 1.1.
             See also
             _B_y_t_e_s_B_a_c_k_e_n_d
         key_mangler:: CCaallllaabbllee[[[[ssttrr]],, ssttrr]] || NNoonnee == NNoonnee_¶
             Key mangling function.
             May be None, or otherwise declared as an ordinary instance method.
         serializer:: NNoonnee || CCaallllaabbllee[[[[AAnnyy]],, bbyytteess]] == NNoonnee_¶
             Serializer function that will be used by default if not overridden
             by the region.
-            New in version 1.1.
+            Added in version 1.1.
         set(kkeeyy:: ssttrr, vvaalluuee:: _CC_aa_cc_hh_ee_dd_VV_aa_ll_uu_ee || bbyytteess) → None_¶
             Set an optionally serialized value in the cache.
               Parameters:
                       * kkeeyy_¶ – String key that was passed to the
                         _C_a_c_h_e_R_e_g_i_o_n_._s_e_t_(_) method, which will also be processed
                         by the “key mangling” function if one was present.
                       * vvaalluuee_¶ – The optionally serialized _C_a_c_h_e_d_V_a_l_u_e object.
@@ -684,25 +687,25 @@
             Region.get_or_create_multi(), the mapping values are the same ones
             returned to the upstream caller. If the subclass alters the values
             in any way, it must not do so ‘in-place’ on the mapping dict – that
             will have the undesirable effect of modifying the returned values
             as well.
             If a serializer is in use, this method will only be called if the
             _C_a_c_h_e_B_a_c_k_e_n_d_._s_e_t___s_e_r_i_a_l_i_z_e_d___m_u_l_t_i_(_) method is not overridden.
-            New in version 0.5.0.
+            Added in version 0.5.0.
         set_serialized(kkeeyy:: ssttrr, vvaalluuee:: bbyytteess) → None_¶
             Set a serialized value in the cache.
               Parameters:
                       * kkeeyy_¶ – String key that was passed to the
                         _C_a_c_h_e_R_e_g_i_o_n_._s_e_t_(_) method, which will also be processed
                         by the “key mangling” function if one was present.
                       * vvaalluuee_¶ – a bytes object to be stored.
             The default implementation of this method for _C_a_c_h_e_B_a_c_k_e_n_d calls
             upon the _C_a_c_h_e_B_a_c_k_e_n_d_._s_e_t_(_) method.
-            New in version 1.1.
+            Added in version 1.1.
             See also
             _B_y_t_e_s_B_a_c_k_e_n_d
         set_serialized_multi(mmaappppiinngg:: MMaappppiinngg[[ssttrr,, bbyytteess]]) → None_¶
             Set multiple serialized values in the cache.
               Parameters:
                   mmaappppiinngg_¶ – a dict in which the key will be whatever was
                   passed to the _C_a_c_h_e_R_e_g_i_o_n_._s_e_t___m_u_l_t_i_(_) method, processed by
@@ -710,84 +713,84 @@
             When implementing a new _C_a_c_h_e_B_a_c_k_e_n_d or cutomizing via
             _P_r_o_x_y_B_a_c_k_e_n_d, be aware that when this method is invoked by
             Region.get_or_create_multi(), the mapping values are the same ones
             returned to the upstream caller. If the subclass alters the values
             in any way, it must not do so ‘in-place’ on the mapping dict – that
             will have the undesirable effect of modifying the returned values
             as well.
-            New in version 1.1.
+            Added in version 1.1.
             The default implementation of this method for _C_a_c_h_e_B_a_c_k_e_n_d calls
             upon the _C_a_c_h_e_B_a_c_k_e_n_d_._s_e_t___m_u_l_t_i_(_) method.
             See also
             _B_y_t_e_s_B_a_c_k_e_n_d
   ccllaassss dogpile.cache.api.CacheMutex_¶
       Bases: ABC
       Describes a mutexing object with acquire and release methods.
       This is an abstract base class; any object that has acquire/release
       methods may be used.
-      New in version 1.1.
+      Added in version 1.1.
       See also
       _C_a_c_h_e_B_a_c_k_e_n_d_._g_e_t___m_u_t_e_x_(_) - the backend method that optionally returns
       this locking object.
         aabbssttrraacctt acquire(wwaaiitt:: bbooooll == TTrruuee) → bool_¶
             Acquire the mutex.
               Parameters:
                   wwaaiitt_¶ – if True, block until available, else return True/
                   False immediately.
               Returns:
                   True if the lock succeeded.
         aabbssttrraacctt locked() → bool_¶
             Check if the mutex was acquired.
               Returns:
                   true if the lock is acquired.
-            New in version 1.1.2.
+            Added in version 1.1.2.
         aabbssttrraacctt release() → None_¶
             Release the mutex.
   dogpile.cache.api.CacheReturnType_¶
       The non-serialized form of what may be returned from a backend get
       method.
-      alias of Union[_C_a_c_h_e_d_V_a_l_u_e, _N_o_V_a_l_u_e]
+      alias of _C_a_c_h_e_d_V_a_l_u_e | Literal[NO_VALUE]
   ccllaassss dogpile.cache.api.CachedValue(ppaayyllooaadd:: VVaalluueePPaayyllooaadd, mmeettaaddaattaa::
   MMeettaaDDaattaaTTyyppee)_¶
       Bases: NamedTuple
       Represent a value stored in the cache.
       _C_a_c_h_e_d_V_a_l_u_e is a two-tuple of (payload, metadata), where metadata is
       dogpile.cache’s tracking information ( currently the creation time).
         pprrooppeerrttyy age:: ffllooaatt_¶
             Returns the elapsed time in seconds as afloatsince the insertion of
             the value in the cache.
             This value is computed ddyynnaammiiccaallllyy by subtracting the cached
             floating point epoch value from the value of time.time().
-            New in version 1.3.
+            Added in version 1.3.
         pprrooppeerrttyy cached_time:: ffllooaatt_¶
             The epoch (floating point time value) stored when this payload was
             cached.
-            New in version 1.3.
+            Added in version 1.3.
         metadata:: MMaappppiinngg[[ssttrr,, AAnnyy]]_¶
             Metadata dictionary for the cached value.
             Prefer using accessors such as _C_a_c_h_e_d_V_a_l_u_e_._c_a_c_h_e_d___t_i_m_e rather than
             accessing this mapping directly.
         payload:: AAnnyy_¶
             the actual cached value.
   eexxcceeppttiioonn dogpile.cache.api.CantDeserializeException_¶
       Bases: Exception
       Exception indicating deserialization failed, and that caching should
       proceed to re-generate a value
-      New in version 1.2.0.
+      Added in version 1.2.0.
   dogpile.cache.api.KeyType_¶
       A cache key.
   dogpile.cache.api.NO_VALUE == <<ddooggppiillee..ccaacchhee..aappii..NNooVVaalluuee oobbjjeecctt>>_¶
-      Value returned from get() that describes a key not present.
-  ccllaassss dogpile.cache.api.NoValue_¶
-      Bases: object
+      Value returned from _C_a_c_h_e_R_e_g_i_o_n_._g_e_t_(_) that describes a key not present.
+  ccllaassss dogpile.cache.api.NoValue(vvaalluuee)_¶
+      Bases: Enum
       Describe a missing cache value.
       The _N_O___V_A_L_U_E constant should be used.
   dogpile.cache.api.SerializedReturnType_¶
       the serialized form of what may be returned from a backend get method.
-      alias of Union[bytes, _N_o_V_a_l_u_e]
+      alias of bytes | Literal[NO_VALUE]
   dogpile.cache.api.ValuePayload == ttyyppiinngg..AAnnyy_¶
       An object to be placed in the cache against a key.
 ********** BBaacckkeennddss_?¶ **********
 ******** MMeemmoorryy BBaacckkeennddss_?¶ ********
 Provides simple dictionary-based backends.
 The two backends are _M_e_m_o_r_y_B_a_c_k_e_n_d and _M_e_m_o_r_y_P_i_c_k_l_e_B_a_c_k_e_n_d; the latter applies
 a serialization step to cached values while the former places the value as
@@ -826,15 +829,15 @@
             Delete multiple values from the cache.
               Parameters:
                   kkeeyyss_¶ – sequence of string keys that was passed to the
                   _C_a_c_h_e_R_e_g_i_o_n_._d_e_l_e_t_e___m_u_l_t_i_(_) method, which will also be
                   processed by the “key mangling” function if one was present.
             The behavior here should be idempotent, that is, can be called any
             number of times regardless of whether or not the key exists.
-            New in version 0.5.0.
+            Added in version 0.5.0.
         get(kkeeyy)_¶
             Retrieve an optionally serialized value from the cache.
               Parameters:
                   kkeeyy_¶ – String key that was passed to the _C_a_c_h_e_R_e_g_i_o_n_._g_e_t_(_)
                   method, which will also be processed by the “key mangling”
                   function if one was present.
               Returns:
@@ -850,15 +853,15 @@
                   _C_a_c_h_e_R_e_g_i_o_n_._g_e_t___m_u_l_t_i_(_) method, which will also be processed
                   by the “key mangling” function if one was present.
               :return a list of values as would be returned
                   individually via the _C_a_c_h_e_B_a_c_k_e_n_d_._g_e_t_(_) method, corresponding
                   to the list of keys given.
             If a serializer is in use, this method will only be called if the
             _C_a_c_h_e_B_a_c_k_e_n_d_._g_e_t___s_e_r_i_a_l_i_z_e_d___m_u_l_t_i_(_) method is not overridden.
-            New in version 0.5.0.
+            Added in version 0.5.0.
         set(kkeeyy, vvaalluuee)_¶
             Set an optionally serialized value in the cache.
               Parameters:
                       * kkeeyy_¶ – String key that was passed to the
                         _C_a_c_h_e_R_e_g_i_o_n_._s_e_t_(_) method, which will also be processed
                         by the “key mangling” function if one was present.
                       * vvaalluuee_¶ – The optionally serialized _C_a_c_h_e_d_V_a_l_u_e object.
@@ -879,15 +882,15 @@
             Region.get_or_create_multi(), the mapping values are the same ones
             returned to the upstream caller. If the subclass alters the values
             in any way, it must not do so ‘in-place’ on the mapping dict – that
             will have the undesirable effect of modifying the returned values
             as well.
             If a serializer is in use, this method will only be called if the
             _C_a_c_h_e_B_a_c_k_e_n_d_._s_e_t___s_e_r_i_a_l_i_z_e_d___m_u_l_t_i_(_) method is not overridden.
-            New in version 0.5.0.
+            Added in version 0.5.0.
   ccllaassss dogpile.cache.backends.memory.MemoryPickleBackend(aarrgguummeennttss)_¶
       Bases: DefaultSerialization, _M_e_m_o_r_y_B_a_c_k_e_n_d
       A backend that uses a plain dictionary, but serializes objects on
       _M_e_m_o_r_y_B_a_c_k_e_n_d_._s_e_t_(_) and deserializes _M_e_m_o_r_y_B_a_c_k_e_n_d_._g_e_t_(_).
       E.g.:
       from dogpile.cache import make_region
 
@@ -902,15 +905,15 @@
       The serialization is performed via pickle, and incurs the same
       performance hit in doing so as that of other backends; in this way the
       _M_e_m_o_r_y_P_i_c_k_l_e_B_a_c_k_e_n_d performance is somewhere in between that of the pure
       _M_e_m_o_r_y_B_a_c_k_e_n_d and the remote server oriented backends such as that of
       Memcached or Redis.
       Pickle behavior here is the same as that of the Redis backend, using
       either cPickle or pickle and specifying HIGHEST_PROTOCOL upon serialize.
-      New in version 0.5.3.
+      Added in version 0.5.3.
 ******** MMeemmccaacchheedd BBaacckkeennddss_?¶ ********
 Provides backends for talking to _m_e_m_c_a_c_h_e_d.
   ccllaassss dogpile.cache.backends.memcached.BMemcachedBackend(aarrgguummeennttss)_¶
       Bases: _G_e_n_e_r_i_c_M_e_m_c_a_c_h_e_d_B_a_c_k_e_n_d
       A backend for the _p_y_t_h_o_n_-_b_i_n_a_r_y_-_m_e_m_c_a_c_h_e_d memcached client.
       This is a pure Python memcached client which includes security features
       like SASL and SSL/TLS.
@@ -973,19 +976,19 @@
             Delete multiple values from the cache.
               Parameters:
                   kkeeyyss_¶ – sequence of string keys that was passed to the
                   _C_a_c_h_e_R_e_g_i_o_n_._d_e_l_e_t_e___m_u_l_t_i_(_) method, which will also be
                   processed by the “key mangling” function if one was present.
             The behavior here should be idempotent, that is, can be called any
             number of times regardless of whether or not the key exists.
-            New in version 0.5.0.
+            Added in version 0.5.0.
         deserializer:: NNoonnee || DDeesseerriiaalliizzeerr == NNoonnee_¶
             deserializer function that will be used by default if not
             overridden by the region.
-            New in version 1.1.
+            Added in version 1.1.
         get(kkeeyy)_¶
             Retrieve an optionally serialized value from the cache.
               Parameters:
                   kkeeyy_¶ – String key that was passed to the _C_a_c_h_e_R_e_g_i_o_n_._g_e_t_(_)
                   method, which will also be processed by the “key mangling”
                   function if one was present.
               Returns:
@@ -1001,15 +1004,15 @@
                   _C_a_c_h_e_R_e_g_i_o_n_._g_e_t___m_u_l_t_i_(_) method, which will also be processed
                   by the “key mangling” function if one was present.
               :return a list of values as would be returned
                   individually via the _C_a_c_h_e_B_a_c_k_e_n_d_._g_e_t_(_) method, corresponding
                   to the list of keys given.
             If a serializer is in use, this method will only be called if the
             _C_a_c_h_e_B_a_c_k_e_n_d_._g_e_t___s_e_r_i_a_l_i_z_e_d___m_u_l_t_i_(_) method is not overridden.
-            New in version 0.5.0.
+            Added in version 0.5.0.
         get_mutex(kkeeyy)_¶
             Return an optional mutexing object for the given key.
             This object need only provide an acquire() and release() method.
             May return None, in which case the dogpile lock will use a regular
             threading.Lock object to mutex concurrent threads for value
             creation. The default implementation returns None.
             Different backends may want to provide various kinds of “mutex”
@@ -1022,15 +1025,15 @@
             one at a time across all keys in the region. The latter approach,
             or a variant that involves a modulus of the given key’s hash value,
             can be used as a means of throttling the total number of value
             recreation operations that may proceed at one time.
         serializer:: NNoonnee || SSeerriiaalliizzeerr == NNoonnee_¶
             Serializer function that will be used by default if not overridden
             by the region.
-            New in version 1.1.
+            Added in version 1.1.
         set(kkeeyy, vvaalluuee)_¶
             Set an optionally serialized value in the cache.
               Parameters:
                       * kkeeyy_¶ – String key that was passed to the
                         _C_a_c_h_e_R_e_g_i_o_n_._s_e_t_(_) method, which will also be processed
                         by the “key mangling” function if one was present.
                       * vvaalluuee_¶ – The optionally serialized _C_a_c_h_e_d_V_a_l_u_e object.
@@ -1053,15 +1056,15 @@
             Region.get_or_create_multi(), the mapping values are the same ones
             returned to the upstream caller. If the subclass alters the values
             in any way, it must not do so ‘in-place’ on the mapping dict – that
             will have the undesirable effect of modifying the returned values
             as well.
             If a serializer is in use, this method will only be called if the
             _C_a_c_h_e_B_a_c_k_e_n_d_._s_e_t___s_e_r_i_a_l_i_z_e_d___m_u_l_t_i_(_) method is not overridden.
-            New in version 0.5.0.
+            Added in version 0.5.0.
   ccllaassss dogpile.cache.backends.memcached.MemcachedBackend(aarrgguummeennttss)_¶
       Bases: MemcacheArgs, _G_e_n_e_r_i_c_M_e_m_c_a_c_h_e_d_B_a_c_k_e_n_d
       A backend using the standard _P_y_t_h_o_n_-_m_e_m_c_a_c_h_e_d library.
       Example:
       from dogpile.cache import make_region
 
       region = make_region().configure(
@@ -1075,15 +1078,15 @@
   ttiimmeeoouutt==00)_¶
       Bases: object
       Simple distributed lock using memcached.
   ccllaassss dogpile.cache.backends.memcached.PyMemcacheBackend(aarrgguummeennttss)_¶
       Bases: _G_e_n_e_r_i_c_M_e_m_c_a_c_h_e_d_B_a_c_k_e_n_d
       A backend for the _p_y_m_e_m_c_a_c_h_e memcached client.
       A comprehensive, fast, pure Python memcached client
-      New in version 1.1.2.
+      Added in version 1.1.2.
       pymemcache supports the following features:
           * Complete implementation of the memcached text protocol.
           * Configurable timeouts for socket connect and send/recv calls.
           * Access to the “noreply” flag, which can significantly increase the
             speed of writes.
           * Flexible, simple approach to serialization and deserialization.
           * The (optional) ability to treat network and memcached errors as
@@ -1148,15 +1151,15 @@
             Delete multiple values from the cache.
               Parameters:
                   kkeeyyss_¶ – sequence of string keys that was passed to the
                   _C_a_c_h_e_R_e_g_i_o_n_._d_e_l_e_t_e___m_u_l_t_i_(_) method, which will also be
                   processed by the “key mangling” function if one was present.
             The behavior here should be idempotent, that is, can be called any
             number of times regardless of whether or not the key exists.
-            New in version 0.5.0.
+            Added in version 0.5.0.
         get_mutex(kkeeyy)_¶
             Return an optional mutexing object for the given key.
             This object need only provide an acquire() and release() method.
             May return None, in which case the dogpile lock will use a regular
             threading.Lock object to mutex concurrent threads for value
             creation. The default implementation returns None.
             Different backends may want to provide various kinds of “mutex”
@@ -1174,55 +1177,55 @@
             Retrieve a serialized value from the cache.
               Parameters:
                   kkeeyy_¶ – String key that was passed to the _C_a_c_h_e_R_e_g_i_o_n_._g_e_t_(_)
                   method, which will also be processed by the “key mangling”
                   function if one was present.
               Returns:
                   a bytes object, or _N_O___V_A_L_U_E constant if not present.
-            New in version 1.1.
+            Added in version 1.1.
         get_serialized_multi(kkeeyyss)_¶
             Retrieve multiple serialized values from the cache.
               Parameters:
                   kkeeyyss_¶ – sequence of string keys that was passed to the
                   _C_a_c_h_e_R_e_g_i_o_n_._g_e_t___m_u_l_t_i_(_) method, which will also be processed
                   by the “key mangling” function if one was present.
               Returns:
                   list of bytes objects
-            New in version 1.1.
+            Added in version 1.1.
         set_serialized(kkeeyy, vvaalluuee)_¶
             Set a serialized value in the cache.
               Parameters:
                       * kkeeyy_¶ – String key that was passed to the
                         _C_a_c_h_e_R_e_g_i_o_n_._s_e_t_(_) method, which will also be processed
                         by the “key mangling” function if one was present.
                       * vvaalluuee_¶ – a bytes object to be stored.
-            New in version 1.1.
+            Added in version 1.1.
         set_serialized_multi(mmaappppiinngg)_¶
             Set multiple serialized values in the cache.
               Parameters:
                   mmaappppiinngg_¶ – a dict in which the key will be whatever was
                   passed to the _C_a_c_h_e_R_e_g_i_o_n_._s_e_t___m_u_l_t_i_(_) method, processed by
                   the “key mangling” function, if any.
             When implementing a new _C_a_c_h_e_B_a_c_k_e_n_d or cutomizing via
             _P_r_o_x_y_B_a_c_k_e_n_d, be aware that when this method is invoked by
             Region.get_or_create_multi(), the mapping values are the same ones
             returned to the upstream caller. If the subclass alters the values
             in any way, it must not do so ‘in-place’ on the mapping dict – that
             will have the undesirable effect of modifying the returned values
             as well.
-            New in version 1.1.
+            Added in version 1.1.
   ccllaassss dogpile.cache.backends.redis.RedisClusterBackend(aarrgguummeennttss)_¶
       Bases: _R_e_d_i_s_B_a_c_k_e_n_d
       A _R_e_d_i_s backend, using the _r_e_d_i_s_-_p_y driver. This backend is to be used
       when connecting to a _R_e_d_i_s_ _C_l_u_s_t_e_r which will use the _R_e_d_i_s_C_l_u_s_t_e_r
       _C_l_i_e_n_t.
       See also
       _C_l_u_s_t_e_r_i_n_g in the redis-py documentation.
       Requires redis-py version >=4.1.0.
-      New in version 1.3.2.
+      Added in version 1.3.2.
       Connecting to the cluster requires one of:
           * Passing a list of startup nodes
           * Passing only one node of the cluster, Redis will use automatic
             discovery to find the other nodes.
       Example configuration, using startup nodes:
       from dogpile.cache import make_region
       from redis.cluster import ClusterNode
@@ -1311,15 +1314,15 @@
                   passed along to the RedisCluster.from_url() method or
                   RedisCluster() constructor directly, including parameters
                   like ssl, ssl_certfile, charset, etc.
   ccllaassss dogpile.cache.backends.redis.RedisSentinelBackend(aarrgguummeennttss)_¶
       Bases: _R_e_d_i_s_B_a_c_k_e_n_d
       A _R_e_d_i_s backend, using the _r_e_d_i_s_-_p_y driver. This backend is to be used
       when using _R_e_d_i_s_ _S_e_n_t_i_n_e_l.
-      New in version 1.0.0.
+      Added in version 1.0.0.
       Example configuration:
       from dogpile.cache import make_region
 
       region = make_region().configure(
           'dogpile.cache.redis_sentinel',
           arguments = {
               'sentinels': [
@@ -1435,15 +1438,15 @@
             Delete multiple values from the cache.
               Parameters:
                   kkeeyyss_¶ – sequence of string keys that was passed to the
                   _C_a_c_h_e_R_e_g_i_o_n_._d_e_l_e_t_e___m_u_l_t_i_(_) method, which will also be
                   processed by the “key mangling” function if one was present.
             The behavior here should be idempotent, that is, can be called any
             number of times regardless of whether or not the key exists.
-            New in version 0.5.0.
+            Added in version 0.5.0.
         get_mutex(kkeeyy)_¶
             Return an optional mutexing object for the given key.
             This object need only provide an acquire() and release() method.
             May return None, in which case the dogpile lock will use a regular
             threading.Lock object to mutex concurrent threads for value
             creation. The default implementation returns None.
             Different backends may want to provide various kinds of “mutex”
@@ -1461,46 +1464,46 @@
             Retrieve a serialized value from the cache.
               Parameters:
                   kkeeyy_¶ – String key that was passed to the _C_a_c_h_e_R_e_g_i_o_n_._g_e_t_(_)
                   method, which will also be processed by the “key mangling”
                   function if one was present.
               Returns:
                   a bytes object, or _N_O___V_A_L_U_E constant if not present.
-            New in version 1.1.
+            Added in version 1.1.
         get_serialized_multi(kkeeyyss)_¶
             Retrieve multiple serialized values from the cache.
               Parameters:
                   kkeeyyss_¶ – sequence of string keys that was passed to the
                   _C_a_c_h_e_R_e_g_i_o_n_._g_e_t___m_u_l_t_i_(_) method, which will also be processed
                   by the “key mangling” function if one was present.
               Returns:
                   list of bytes objects
-            New in version 1.1.
+            Added in version 1.1.
         set_serialized(kkeeyy, vvaalluuee)_¶
             Set a serialized value in the cache.
               Parameters:
                       * kkeeyy_¶ – String key that was passed to the
                         _C_a_c_h_e_R_e_g_i_o_n_._s_e_t_(_) method, which will also be processed
                         by the “key mangling” function if one was present.
                       * vvaalluuee_¶ – a bytes object to be stored.
-            New in version 1.1.
+            Added in version 1.1.
         set_serialized_multi(mmaappppiinngg)_¶
             Set multiple serialized values in the cache.
               Parameters:
                   mmaappppiinngg_¶ – a dict in which the key will be whatever was
                   passed to the _C_a_c_h_e_R_e_g_i_o_n_._s_e_t___m_u_l_t_i_(_) method, processed by
                   the “key mangling” function, if any.
             When implementing a new _C_a_c_h_e_B_a_c_k_e_n_d or cutomizing via
             _P_r_o_x_y_B_a_c_k_e_n_d, be aware that when this method is invoked by
             Region.get_or_create_multi(), the mapping values are the same ones
             returned to the upstream caller. If the subclass alters the values
             in any way, it must not do so ‘in-place’ on the mapping dict – that
             will have the undesirable effect of modifying the returned values
             as well.
-            New in version 1.1.
+            Added in version 1.1.
   ccllaassss dogpile.cache.backends.file.FileLock(ffiilleennaammee)_¶
       Bases: _A_b_s_t_r_a_c_t_F_i_l_e_L_o_c_k
       Use lockfiles to coordinate read/write access to a file.
       Only works on Unix systems, using _f_c_n_t_l_._f_l_o_c_k_(_).
         acquire_read_lock(wwaaiitt)_¶
             Acquire a ‘reader’ lock.
             Raises NotImplementedError by default, must be implemented by
@@ -1519,15 +1522,15 @@
             Release a ‘writer’ lock.
             Raises NotImplementedError by default, must be implemented by
             subclasses.
 ******** PPrrooxxyy BBaacckkeennddss_?¶ ********
 Provides a utility and a decorator class that allow for modifying the behavior
 of different backends without altering the class itself or having to extend the
 base backend.
-New in version 0.5.0: Added support for the _P_r_o_x_y_B_a_c_k_e_n_d class.
+Added in version 0.5.0: Added support for the _P_r_o_x_y_B_a_c_k_e_n_d class.
   ccllaassss dogpile.cache.proxy.ProxyBackend(**aarrgg, ****kkww)_¶
       Bases: _C_a_c_h_e_B_a_c_k_e_n_d
       A decorator class for altering the functionality of backends.
       Basic usage:
       from dogpile.cache import make_region
       from dogpile.cache.proxy import ProxyBackend
 
@@ -1553,15 +1556,15 @@
               "filename":"/path/to/cachefile.dbm"
           },
           wrap = [ MyFirstProxy, MySecondProxy ]
       )
       Classes that extend _P_r_o_x_y_B_a_c_k_e_n_d can be stacked together. The .proxied
       property will always point to either the concrete backend instance or the
       next proxy in the chain that a method can be delegated towards.
-      New in version 0.5.0.
+      Added in version 0.5.0.
         delete(kkeeyy:: ssttrr) → None_¶
             Delete a value from the cache.
               Parameters:
                   kkeeyy_¶ – String key that was passed to the _C_a_c_h_e_R_e_g_i_o_n_._d_e_l_e_t_e_(_)
                   method, which will also be processed by the “key mangling”
                   function if one was present.
             The behavior here should be idempotent, that is, can be called any
@@ -1570,40 +1573,40 @@
             Delete multiple values from the cache.
               Parameters:
                   kkeeyyss_¶ – sequence of string keys that was passed to the
                   _C_a_c_h_e_R_e_g_i_o_n_._d_e_l_e_t_e___m_u_l_t_i_(_) method, which will also be
                   processed by the “key mangling” function if one was present.
             The behavior here should be idempotent, that is, can be called any
             number of times regardless of whether or not the key exists.
-            New in version 0.5.0.
-        get(kkeeyy:: ssttrr) → _C_a_c_h_e_d_V_a_l_u_e | _N_o_V_a_l_u_e | bytes_¶
+            Added in version 0.5.0.
+        get(kkeeyy:: ssttrr) → _C_a_c_h_e_d_V_a_l_u_e | Literal[NoValue.NO_VALUE] | bytes_¶
             Retrieve an optionally serialized value from the cache.
               Parameters:
                   kkeeyy_¶ – String key that was passed to the _C_a_c_h_e_R_e_g_i_o_n_._g_e_t_(_)
                   method, which will also be processed by the “key mangling”
                   function if one was present.
               Returns:
                   the Python object that corresponds to what was established
                   via the _C_a_c_h_e_B_a_c_k_e_n_d_._s_e_t_(_) method, or the _N_O___V_A_L_U_E constant
                   if not present.
             If a serializer is in use, this method will only be called if the
             _C_a_c_h_e_B_a_c_k_e_n_d_._g_e_t___s_e_r_i_a_l_i_z_e_d_(_) method is not overridden.
-        get_multi(kkeeyyss:: SSeeqquueennccee[[ssttrr]]) → Sequence[_C_a_c_h_e_d_V_a_l_u_e | _N_o_V_a_l_u_e |
-        bytes]_¶
+        get_multi(kkeeyyss:: SSeeqquueennccee[[ssttrr]]) → Sequence[_C_a_c_h_e_d_V_a_l_u_e | Literal
+        [NoValue.NO_VALUE] | bytes]_¶
             Retrieve multiple optionally serialized values from the cache.
               Parameters:
                   kkeeyyss_¶ – sequence of string keys that was passed to the
                   _C_a_c_h_e_R_e_g_i_o_n_._g_e_t___m_u_l_t_i_(_) method, which will also be processed
                   by the “key mangling” function if one was present.
               :return a list of values as would be returned
                   individually via the _C_a_c_h_e_B_a_c_k_e_n_d_._g_e_t_(_) method, corresponding
                   to the list of keys given.
             If a serializer is in use, this method will only be called if the
             _C_a_c_h_e_B_a_c_k_e_n_d_._g_e_t___s_e_r_i_a_l_i_z_e_d___m_u_l_t_i_(_) method is not overridden.
-            New in version 0.5.0.
+            Added in version 0.5.0.
         get_mutex(kkeeyy:: ssttrr) → _C_a_c_h_e_M_u_t_e_x | None_¶
             Return an optional mutexing object for the given key.
             This object need only provide an acquire() and release() method.
             May return None, in which case the dogpile lock will use a regular
             threading.Lock object to mutex concurrent threads for value
             creation. The default implementation returns None.
             Different backends may want to provide various kinds of “mutex”
@@ -1613,38 +1616,39 @@
             A mutex that takes the key into account will allow multiple
             regenerate operations across keys to proceed simultaneously, while
             a mutex that does not will serialize regenerate operations to just
             one at a time across all keys in the region. The latter approach,
             or a variant that involves a modulus of the given key’s hash value,
             can be used as a means of throttling the total number of value
             recreation operations that may proceed at one time.
-        get_serialized(kkeeyy:: ssttrr) → bytes | _N_o_V_a_l_u_e_¶
+        get_serialized(kkeeyy:: ssttrr) → bytes | Literal[NoValue.NO_VALUE]_¶
             Retrieve a serialized value from the cache.
               Parameters:
                   kkeeyy_¶ – String key that was passed to the _C_a_c_h_e_R_e_g_i_o_n_._g_e_t_(_)
                   method, which will also be processed by the “key mangling”
                   function if one was present.
               Returns:
                   a bytes object, or _N_O___V_A_L_U_E constant if not present.
             The default implementation of this method for _C_a_c_h_e_B_a_c_k_e_n_d returns
             the value of the _C_a_c_h_e_B_a_c_k_e_n_d_._g_e_t_(_) method.
-            New in version 1.1.
+            Added in version 1.1.
             See also
             _B_y_t_e_s_B_a_c_k_e_n_d
-        get_serialized_multi(kkeeyyss:: SSeeqquueennccee[[ssttrr]]) → Sequence[bytes | _N_o_V_a_l_u_e]_¶
+        get_serialized_multi(kkeeyyss:: SSeeqquueennccee[[ssttrr]]) → Sequence[bytes | Literal
+        [NoValue.NO_VALUE]]_¶
             Retrieve multiple serialized values from the cache.
               Parameters:
                   kkeeyyss_¶ – sequence of string keys that was passed to the
                   _C_a_c_h_e_R_e_g_i_o_n_._g_e_t___m_u_l_t_i_(_) method, which will also be processed
                   by the “key mangling” function if one was present.
               Returns:
                   list of bytes objects
             The default implementation of this method for _C_a_c_h_e_B_a_c_k_e_n_d returns
             the value of the _C_a_c_h_e_B_a_c_k_e_n_d_._g_e_t___m_u_l_t_i_(_) method.
-            New in version 1.1.
+            Added in version 1.1.
             See also
             _B_y_t_e_s_B_a_c_k_e_n_d
         set(kkeeyy:: ssttrr, vvaalluuee:: _CC_aa_cc_hh_ee_dd_VV_aa_ll_uu_ee || bbyytteess) → None_¶
             Set an optionally serialized value in the cache.
               Parameters:
                       * kkeeyy_¶ – String key that was passed to the
                         _C_a_c_h_e_R_e_g_i_o_n_._s_e_t_(_) method, which will also be processed
@@ -1667,25 +1671,25 @@
             Region.get_or_create_multi(), the mapping values are the same ones
             returned to the upstream caller. If the subclass alters the values
             in any way, it must not do so ‘in-place’ on the mapping dict – that
             will have the undesirable effect of modifying the returned values
             as well.
             If a serializer is in use, this method will only be called if the
             _C_a_c_h_e_B_a_c_k_e_n_d_._s_e_t___s_e_r_i_a_l_i_z_e_d___m_u_l_t_i_(_) method is not overridden.
-            New in version 0.5.0.
+            Added in version 0.5.0.
         set_serialized(kkeeyy:: ssttrr, vvaalluuee:: bbyytteess) → None_¶
             Set a serialized value in the cache.
               Parameters:
                       * kkeeyy_¶ – String key that was passed to the
                         _C_a_c_h_e_R_e_g_i_o_n_._s_e_t_(_) method, which will also be processed
                         by the “key mangling” function if one was present.
                       * vvaalluuee_¶ – a bytes object to be stored.
             The default implementation of this method for _C_a_c_h_e_B_a_c_k_e_n_d calls
             upon the _C_a_c_h_e_B_a_c_k_e_n_d_._s_e_t_(_) method.
-            New in version 1.1.
+            Added in version 1.1.
             See also
             _B_y_t_e_s_B_a_c_k_e_n_d
         set_serialized_multi(mmaappppiinngg:: MMaappppiinngg[[ssttrr,, bbyytteess]]) → None_¶
             Set multiple serialized values in the cache.
               Parameters:
                   mmaappppiinngg_¶ – a dict in which the key will be whatever was
                   passed to the _C_a_c_h_e_R_e_g_i_o_n_._s_e_t___m_u_l_t_i_(_) method, processed by
@@ -1693,27 +1697,27 @@
             When implementing a new _C_a_c_h_e_B_a_c_k_e_n_d or cutomizing via
             _P_r_o_x_y_B_a_c_k_e_n_d, be aware that when this method is invoked by
             Region.get_or_create_multi(), the mapping values are the same ones
             returned to the upstream caller. If the subclass alters the values
             in any way, it must not do so ‘in-place’ on the mapping dict – that
             will have the undesirable effect of modifying the returned values
             as well.
-            New in version 1.1.
+            Added in version 1.1.
             The default implementation of this method for _C_a_c_h_e_B_a_c_k_e_n_d calls
             upon the _C_a_c_h_e_B_a_c_k_e_n_d_._s_e_t___m_u_l_t_i_(_) method.
             See also
             _B_y_t_e_s_B_a_c_k_e_n_d
         wrap(bbaacckkeenndd:: _CC_aa_cc_hh_ee_BB_aa_cc_kk_ee_nn_dd) → Self_¶
             Take a backend as an argument and setup the self.proxied property.
             Return an object that be used as a backend by a _C_a_c_h_e_R_e_g_i_o_n object.
 ******** NNuullll BBaacckkeenndd_?¶ ********
 The Null backend does not do any caching at all. It can be used to test
 behavior without caching, or as a means of disabling caching for a region that
 is otherwise used normally.
-New in version 0.5.4.
+Added in version 0.5.4.
   ccllaassss dogpile.cache.backends.null.NullBackend(aarrgguummeennttss)_¶
       Bases: _C_a_c_h_e_B_a_c_k_e_n_d
       A “null” backend that effectively disables all cache operations.
       Basic usage:
       from dogpile.cache import make_region
 
       region = make_region().configure(
@@ -1731,15 +1735,15 @@
             Delete multiple values from the cache.
               Parameters:
                   kkeeyyss_¶ – sequence of string keys that was passed to the
                   _C_a_c_h_e_R_e_g_i_o_n_._d_e_l_e_t_e___m_u_l_t_i_(_) method, which will also be
                   processed by the “key mangling” function if one was present.
             The behavior here should be idempotent, that is, can be called any
             number of times regardless of whether or not the key exists.
-            New in version 0.5.0.
+            Added in version 0.5.0.
         get(kkeeyy)_¶
             Retrieve an optionally serialized value from the cache.
               Parameters:
                   kkeeyy_¶ – String key that was passed to the _C_a_c_h_e_R_e_g_i_o_n_._g_e_t_(_)
                   method, which will also be processed by the “key mangling”
                   function if one was present.
               Returns:
@@ -1755,15 +1759,15 @@
                   _C_a_c_h_e_R_e_g_i_o_n_._g_e_t___m_u_l_t_i_(_) method, which will also be processed
                   by the “key mangling” function if one was present.
               :return a list of values as would be returned
                   individually via the _C_a_c_h_e_B_a_c_k_e_n_d_._g_e_t_(_) method, corresponding
                   to the list of keys given.
             If a serializer is in use, this method will only be called if the
             _C_a_c_h_e_B_a_c_k_e_n_d_._g_e_t___s_e_r_i_a_l_i_z_e_d___m_u_l_t_i_(_) method is not overridden.
-            New in version 0.5.0.
+            Added in version 0.5.0.
         get_mutex(kkeeyy)_¶
             Return an optional mutexing object for the given key.
             This object need only provide an acquire() and release() method.
             May return None, in which case the dogpile lock will use a regular
             threading.Lock object to mutex concurrent threads for value
             creation. The default implementation returns None.
             Different backends may want to provide various kinds of “mutex”
@@ -1801,24 +1805,24 @@
             Region.get_or_create_multi(), the mapping values are the same ones
             returned to the upstream caller. If the subclass alters the values
             in any way, it must not do so ‘in-place’ on the mapping dict – that
             will have the undesirable effect of modifying the returned values
             as well.
             If a serializer is in use, this method will only be called if the
             _C_a_c_h_e_B_a_c_k_e_n_d_._s_e_t___s_e_r_i_a_l_i_z_e_d___m_u_l_t_i_(_) method is not overridden.
-            New in version 0.5.0.
+            Added in version 0.5.0.
 ********** EExxcceeppttiioonnss_?¶ **********
 Exception classes for dogpile.cache.
   eexxcceeppttiioonn dogpile.cache.exception.DogpileCacheException_¶
       Bases: Exception
       Base Exception for dogpile.cache exceptions to inherit from.
   eexxcceeppttiioonn dogpile.cache.exception.PluginNotFound_¶
       Bases: _D_o_g_p_i_l_e_C_a_c_h_e_E_x_c_e_p_t_i_o_n
       The specified plugin could not be found.
-      New in version 0.6.4.
+      Added in version 0.6.4.
   eexxcceeppttiioonn dogpile.cache.exception.RegionAlreadyConfigured_¶
       Bases: _D_o_g_p_i_l_e_C_a_c_h_e_E_x_c_e_p_t_i_o_n
       CacheRegion instance is already configured.
   eexxcceeppttiioonn dogpile.cache.exception.RegionNotConfigured_¶
       Bases: _D_o_g_p_i_l_e_C_a_c_h_e_E_x_c_e_p_t_i_o_n
       CacheRegion instance has not been configured.
   eexxcceeppttiioonn dogpile.cache.exception.ValidationError_¶
@@ -1898,15 +1902,15 @@
   dogpile.cache.util.kwarg_function_key_generator(nnaammeessppaaccee, ffnn, ttoo__ssttrr==<<ccllaassss
   ''ssttrr''>>)_¶
       Return a function that generates a string key, based on a given function
       as well as arguments to the returned function itself.
       For kwargs passed in, we will build a dict of all argname (key) argvalue
       (values) including default args from the argspec and then alphabetize the
       list before generating the key.
-      New in version 0.6.2.
+      Added in version 0.6.2.
       See also
       _f_u_n_c_t_i_o_n___k_e_y___g_e_n_e_r_a_t_o_r_(_) - default key generation function
   dogpile.cache.util.sha1_mangle_key(kkeeyy)_¶
       a SHA1 key mangler.
   dogpile.cache.util.length_conditional_mangler(lleennggtthh, mmaanngglleerr)_¶
       a key mangler that mangles if the length of the key is past a certain
       threshold.
@@ -2194,10 +2198,10 @@
 ****** NNeexxtt ttooppiicc ******
 _C_h_a_n_g_e_l_o_g
 ******** NNaavviiggaattiioonn ********
     * _i_n_d_e_x
     * _m_o_d_u_l_e_s |
     * _n_e_x_t |
     * _p_r_e_v_i_o_u_s |
-    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._2_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
+    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._3_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
     * API
-© Copyright 2011-2024 Mike Bayer. Created using _S_p_h_i_n_x 7.2.6.
+© Copyright 2011-2024 Mike Bayer. Created using _S_p_h_i_n_x 7.3.7.
```

### Comparing `dogpile.cache-1.3.2/docs/build/Makefile` & `dogpile.cache-1.3.3/docs/build/Makefile`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/docs/build/api.rst` & `dogpile.cache-1.3.3/docs/build/api.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/docs/build/changelog.rst` & `dogpile.cache-1.3.3/docs/build/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,33 @@
 =========
 Changelog
 =========
 
 .. changelog::
+    :version: 1.3.3
+    :released: Sun May 5 2024
+
+    .. change::
+        :tags: bug, typing
+
+        Fixed the return type for :meth:`.CacheRegion.get`, which was inadvertently
+        hardcoded to use ``CacheReturnType`` that only resolved to ``CachedValue``
+        or ``NoValue``.   Fixed to return ``ValuePayload`` which resolves to
+        ``Any``, as well as a new literal indicating an enum constant for
+        :data:`.api.NO_VALUE`.  The :data:`.api.NO_VALUE` constant remains
+        available as the single element of this enum.
+
+    .. change::
+        :tags: usecase, memcached
+
+        Added support for an additional pymemcached client parameter
+        :paramref:`.PyMemcacheBackend.memcached_expire_time`.  Pull request
+        courtesy Takashi Kajinami.
+
+.. changelog::
     :version: 1.3.2
     :released: Wed Feb 21 2024
 
     .. change::
         :tags: usecase, redis
         :tickets: 250
```

### Comparing `dogpile.cache-1.3.2/docs/build/conf.py` & `dogpile.cache-1.3.3/docs/build/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = dogpile.__version__
 # The full version, including alpha/beta/rc tags.
-release = "1.3.2"
+release = "1.3.3"
 
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to some
```

### Comparing `dogpile.cache-1.3.2/docs/build/core_usage.rst` & `dogpile.cache-1.3.3/docs/build/core_usage.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/docs/build/front.rst` & `dogpile.cache-1.3.3/docs/build/front.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/docs/build/index.rst` & `dogpile.cache-1.3.3/docs/build/index.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/docs/build/make.bat` & `dogpile.cache-1.3.3/docs/build/make.bat`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/docs/build/recipes.rst` & `dogpile.cache-1.3.3/docs/build/recipes.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/docs/build/usage.rst` & `dogpile.cache-1.3.3/docs/build/usage.rst`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/docs/changelog.html` & `dogpile.cache-1.3.3/docs/changelog.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Changelog &#8212; dogpile.cache 1.3.2 documentation</title>
+    <title>Changelog &#8212; dogpile.cache 1.3.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css?v=d00006d9" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
-    <script src="_static/documentation_options.js?v=8ca9e7a0"></script>
-    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/documentation_options.js?v=28d163b9"></script>
+    <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="prev" title="API" href="api.html" /> 
   </head><body>
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
@@ -25,26 +25,54 @@
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="api.html" title="API"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Changelog</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
             
   <section id="changelog">
 <h1>Changelog<a class="headerlink" href="#changelog" title="Link to this heading">¶</a></h1>
+<section id="change-1.3.3">
+<h2 class="release-version">1.3.3<a class="headerlink" href="#change-1.3.3" title="Link to this heading">¶</a></h2>
+Released: Sun May 5 2024<section id="change-1.3.3-usecase">
+<h3>usecase<a class="headerlink" href="#change-1.3.3-usecase" title="Link to this heading">¶</a></h3>
+<ul class="simple">
+<li><p class="caption" id="change-1.3.3-0"><span class="target" id="change-63479d35c0d4f19314acebc6f5640ac9"><strong>[usecase] [memcached]</strong> <a class="changelog-reference headerlink reference internal" href="#change-63479d35c0d4f19314acebc6f5640ac9">¶</a></span><p>Added support for an additional pymemcached client parameter
+<a class="reference internal" href="api.html#dogpile.cache.backends.memcached.PyMemcacheBackend.params.memcached_expire_time" title="dogpile.cache.backends.memcached.PyMemcacheBackend"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">PyMemcacheBackend.memcached_expire_time</span></code></a>.  Pull request
+courtesy Takashi Kajinami.</p>
+<p></p>
+</p>
+</li>
+</ul>
+</section>
+<section id="change-1.3.3-bug">
+<h3>bug<a class="headerlink" href="#change-1.3.3-bug" title="Link to this heading">¶</a></h3>
+<ul class="simple">
+<li><p class="caption" id="change-1.3.3-1"><span class="target" id="change-207b4da738bb71dd9c0705eb03db1a78"><strong>[bug] [typing]</strong> <a class="changelog-reference headerlink reference internal" href="#change-207b4da738bb71dd9c0705eb03db1a78">¶</a></span><p>Fixed the return type for <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion.get" title="dogpile.cache.region.CacheRegion.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get()</span></code></a>, which was inadvertently
+hardcoded to use <code class="docutils literal notranslate"><span class="pre">CacheReturnType</span></code> that only resolved to <code class="docutils literal notranslate"><span class="pre">CachedValue</span></code>
+or <code class="docutils literal notranslate"><span class="pre">NoValue</span></code>.   Fixed to return <code class="docutils literal notranslate"><span class="pre">ValuePayload</span></code> which resolves to
+<code class="docutils literal notranslate"><span class="pre">Any</span></code>, as well as a new literal indicating an enum constant for
+<a class="reference internal" href="api.html#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">api.NO_VALUE</span></code></a>.  The <a class="reference internal" href="api.html#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">api.NO_VALUE</span></code></a> constant remains
+available as the single element of this enum.</p>
+<p></p>
+</p>
+</li>
+</ul>
+</section>
+</section>
 <section id="change-1.3.2">
 <h2 class="release-version">1.3.2<a class="headerlink" href="#change-1.3.2" title="Link to this heading">¶</a></h2>
 Released: Wed Feb 21 2024<section id="change-1.3.2-usecase">
 <h3>usecase<a class="headerlink" href="#change-1.3.2-usecase" title="Link to this heading">¶</a></h3>
 <ul class="simple">
 <li><p class="caption" id="change-1.3.2-0"><span class="target" id="change-9c71fe524fb508c874e5776c58baf763"><strong>[usecase] [redis]</strong> <a class="changelog-reference headerlink reference internal" href="#change-9c71fe524fb508c874e5776c58baf763">¶</a></span><p>Added a new backend <a class="reference internal" href="api.html#dogpile.cache.backends.redis.RedisClusterBackend" title="dogpile.cache.backends.redis.RedisClusterBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">RedisClusterBackend</span></code></a>, allowing support for
 Redis Cluster.  Pull request courtesy Maël Naccache Tüfekçi.</p>
@@ -1445,14 +1473,19 @@
       </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <div>
     <h3><a href="index.html">Table of Contents</a></h3>
     <ul>
 <li><a class="reference internal" href="#">Changelog</a><ul>
+<li><a class="reference internal" href="#change-1.3.3">1.3.3</a><ul>
+<li><a class="reference internal" href="#change-1.3.3-usecase">usecase</a></li>
+<li><a class="reference internal" href="#change-1.3.3-bug">bug</a></li>
+</ul>
+</li>
 <li><a class="reference internal" href="#change-1.3.2">1.3.2</a><ul>
 <li><a class="reference internal" href="#change-1.3.2-usecase">usecase</a></li>
 </ul>
 </li>
 <li><a class="reference internal" href="#change-1.3.1">1.3.1</a><ul>
 <li><a class="reference internal" href="#change-1.3.1-usecase">usecase</a></li>
 </ul>
@@ -1662,23 +1695,23 @@
 <li><a class="reference internal" href="#change-0.1.1">0.1.1</a></li>
 <li><a class="reference internal" href="#change-0.1.0">0.1.0</a></li>
 </ul>
 </li>
 </ul>
 
   </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
   <div>
     <h4>Previous topic</h4>
     <p class="topless"><a href="api.html"
                           title="previous chapter">API</a></p>
   </div>
         </div>
@@ -1693,17 +1726,17 @@
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="api.html" title="API"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Changelog</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
     &#169; Copyright 2011-2024 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.2.6.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.3.7.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,14 +1,29 @@
 ******** NNaavviiggaattiioonn ********
     * _i_n_d_e_x
     * _m_o_d_u_l_e_s |
     * _p_r_e_v_i_o_u_s |
-    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._2_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
+    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._3_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
     * Changelog
 ************ CChhaannggeelloogg_?¶ ************
+********** 11..33..33_?¶ **********
+Released: Sun May 5 2024
+******** uusseeccaassee_?¶ ********
+    * [[uusseeccaassee]] [[mmeemmccaacchheedd]] _¶
+      Added support for an additional pymemcached client parameter
+      _P_y_M_e_m_c_a_c_h_e_B_a_c_k_e_n_d_._m_e_m_c_a_c_h_e_d___e_x_p_i_r_e___t_i_m_e. Pull request courtesy Takashi
+      Kajinami.
+******** bbuugg_?¶ ********
+    * [[bbuugg]] [[ttyyppiinngg]] _¶
+      Fixed the return type for _C_a_c_h_e_R_e_g_i_o_n_._g_e_t_(_), which was inadvertently
+      hardcoded to use CacheReturnType that only resolved to CachedValue or
+      NoValue. Fixed to return ValuePayload which resolves to Any, as well as a
+      new literal indicating an enum constant for _a_p_i_._N_O___V_A_L_U_E. The
+      _a_p_i_._N_O___V_A_L_U_E constant remains available as the single element of this
+      enum.
 ********** 11..33..22_?¶ **********
 Released: Wed Feb 21 2024
 ******** uusseeccaassee_?¶ ********
     * [[uusseeccaassee]] [[rreeddiiss]] _¶
       Added a new backend _R_e_d_i_s_C_l_u_s_t_e_r_B_a_c_k_e_n_d, allowing support for Redis
       Cluster. Pull request courtesy Maël Naccache Tüfekçi.
       References: _#_2_5_0
@@ -809,14 +824,17 @@
 Released: Sun Apr 08 2012
     * [[nnoo__ttaaggss]] _¶
       Initial release.
 [[nnoo__ttaaggss]] _¶
 Includes a pylibmc backend and a plain dictionary backend.
 ******** _TT_aa_bb_ll_ee_ _oo_ff_ _CC_oo_nn_tt_ee_nn_tt_ss ********
     * _C_h_a_n_g_e_l_o_g
+          o _1_._3_._3
+                # _u_s_e_c_a_s_e
+                # _b_u_g
           o _1_._3_._2
                 # _u_s_e_c_a_s_e
           o _1_._3_._1
                 # _u_s_e_c_a_s_e
           o _1_._3_._0
                 # _f_e_a_t_u_r_e
                 # _m_i_s_c
@@ -937,10 +955,10 @@
 [q                   ][Go]
 ****** PPrreevviioouuss ttooppiicc ******
 _A_P_I
 ******** NNaavviiggaattiioonn ********
     * _i_n_d_e_x
     * _m_o_d_u_l_e_s |
     * _p_r_e_v_i_o_u_s |
-    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._2_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
+    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._3_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
     * Changelog
-© Copyright 2011-2024 Mike Bayer. Created using _S_p_h_i_n_x 7.2.6.
+© Copyright 2011-2024 Mike Bayer. Created using _S_p_h_i_n_x 7.3.7.
```

### Comparing `dogpile.cache-1.3.2/docs/core_usage.html` & `dogpile.cache-1.3.3/docs/core_usage.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>dogpile Core &#8212; dogpile.cache 1.3.2 documentation</title>
+    <title>dogpile Core &#8212; dogpile.cache 1.3.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css?v=d00006d9" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
-    <script src="_static/documentation_options.js?v=8ca9e7a0"></script>
-    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/documentation_options.js?v=28d163b9"></script>
+    <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="API" href="api.html" />
     <link rel="prev" title="Recipes" href="recipes.html" /> 
   </head><body>
     <div class="related" role="navigation" aria-label="related navigation">
@@ -29,15 +29,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="api.html" title="API"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="recipes.html" title="Recipes"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">dogpile Core</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -288,23 +288,23 @@
 <li><a class="reference internal" href="#example-using-dogpile-directly-for-caching">Example: Using dogpile directly for Caching</a></li>
 <li><a class="reference internal" href="#using-a-file-or-distributed-lock-with-dogpile">Using a File or Distributed Lock with Dogpile</a></li>
 </ul>
 </li>
 </ul>
 
   </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
   <div>
     <h4>Previous topic</h4>
     <p class="topless"><a href="recipes.html"
                           title="previous chapter">Recipes</a></p>
   </div>
   <div>
@@ -327,17 +327,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="api.html" title="API"
              >next</a> |</li>
         <li class="right" >
           <a href="recipes.html" title="Recipes"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">dogpile Core</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
     &#169; Copyright 2011-2024 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.2.6.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.3.7.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 ******** NNaavviiggaattiioonn ********
     * _i_n_d_e_x
     * _m_o_d_u_l_e_s |
     * _n_e_x_t |
     * _p_r_e_v_i_o_u_s |
-    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._2_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
+    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._3_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
     * dogpile Core
 ************ ddooggppiillee CCoorree_?¶ ************
 dogpile provides a locking interface around a “value creation” and “value
 retrieval” pair of functions.
 Changed in version 0.6.0: The dogpile package encapsulates the functionality
 that was previously provided by the separate dogpile.core package.
 The primary interface is the _L_o_c_k object, which provides for the invocation of
@@ -221,10 +221,10 @@
 ****** NNeexxtt ttooppiicc ******
 _A_P_I
 ******** NNaavviiggaattiioonn ********
     * _i_n_d_e_x
     * _m_o_d_u_l_e_s |
     * _n_e_x_t |
     * _p_r_e_v_i_o_u_s |
-    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._2_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
+    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._3_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
     * dogpile Core
-© Copyright 2011-2024 Mike Bayer. Created using _S_p_h_i_n_x 7.2.6.
+© Copyright 2011-2024 Mike Bayer. Created using _S_p_h_i_n_x 7.3.7.
```

### Comparing `dogpile.cache-1.3.2/docs/front.html` & `dogpile.cache-1.3.3/docs/front.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Front Matter &#8212; dogpile.cache 1.3.2 documentation</title>
+    <title>Front Matter &#8212; dogpile.cache 1.3.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css?v=d00006d9" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
-    <script src="_static/documentation_options.js?v=8ca9e7a0"></script>
-    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/documentation_options.js?v=28d163b9"></script>
+    <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Usage Guide" href="usage.html" />
     <link rel="prev" title="Welcome to dogpile.cache’s documentation!" href="index.html" /> 
   </head><body>
     <div class="related" role="navigation" aria-label="related navigation">
@@ -29,15 +29,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="usage.html" title="Usage Guide"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="index.html" title="Welcome to dogpile.cache’s documentation!"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Front Matter</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -81,23 +81,23 @@
 <li><a class="reference internal" href="#installation">Installation</a></li>
 <li><a class="reference internal" href="#bugs">Bugs</a></li>
 </ul>
 </li>
 </ul>
 
   </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
   <div>
     <h4>Previous topic</h4>
     <p class="topless"><a href="index.html"
                           title="previous chapter">Welcome to dogpile.cache’s documentation!</a></p>
   </div>
   <div>
@@ -120,17 +120,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="usage.html" title="Usage Guide"
              >next</a> |</li>
         <li class="right" >
           <a href="index.html" title="Welcome to dogpile.cache’s documentation!"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Front Matter</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
     &#169; Copyright 2011-2024 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.2.6.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.3.7.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 ******** NNaavviiggaattiioonn ********
     * _i_n_d_e_x
     * _m_o_d_u_l_e_s |
     * _n_e_x_t |
     * _p_r_e_v_i_o_u_s |
-    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._2_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
+    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._3_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
     * Front Matter
 ************ FFrroonntt MMaatttteerr_?¶ ************
 Information about the dogpile.cache project.
 ********** PPrroojjeecctt HHoommeeppaaggee_?¶ **********
 dogpile.cache is hosted on GitHub at _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_s_q_l_a_l_c_h_e_m_y_/
 _d_o_g_p_i_l_e_._c_a_c_h_e.
 Releases and project status are available on Pypi at _h_t_t_p_s_:_/_/_p_y_p_i_._p_y_t_h_o_n_._o_r_g_/
@@ -33,10 +33,10 @@
 ****** NNeexxtt ttooppiicc ******
 _U_s_a_g_e_ _G_u_i_d_e
 ******** NNaavviiggaattiioonn ********
     * _i_n_d_e_x
     * _m_o_d_u_l_e_s |
     * _n_e_x_t |
     * _p_r_e_v_i_o_u_s |
-    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._2_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
+    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._3_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
     * Front Matter
-© Copyright 2011-2024 Mike Bayer. Created using _S_p_h_i_n_x 7.2.6.
+© Copyright 2011-2024 Mike Bayer. Created using _S_p_h_i_n_x 7.3.7.
```

### Comparing `dogpile.cache-1.3.2/docs/genindex.html` & `dogpile.cache-1.3.3/docs/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Index &#8212; dogpile.cache 1.3.2 documentation</title>
+    <title>Index &#8212; dogpile.cache 1.3.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css?v=d00006d9" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
-    <script src="_static/documentation_options.js?v=8ca9e7a0"></script>
-    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/documentation_options.js?v=28d163b9"></script>
+    <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="#" />
     <link rel="search" title="Search" href="search.html" /> 
   </head><body>
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Index</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -746,15 +746,15 @@
         <li><a href="api.html#dogpile.cache.backends.redis.RedisBackend.set_serialized_multi.params.mapping">(dogpile.cache.backends.redis.RedisBackend.set_serialized_multi parameter)</a>
 </li>
         <li><a href="api.html#dogpile.cache.proxy.ProxyBackend.set_multi.params.mapping">(dogpile.cache.proxy.ProxyBackend.set_multi parameter)</a>
 </li>
         <li><a href="api.html#dogpile.cache.proxy.ProxyBackend.set_serialized_multi.params.mapping">(dogpile.cache.proxy.ProxyBackend.set_serialized_multi parameter)</a>
 </li>
       </ul></li>
-      <li><a href="api.html#dogpile.cache.backends.memcached.GenericMemcachedBackend.params.memcached_expire_time">memcached_expire_time (dogpile.cache.backends.memcached.GenericMemcachedBackend parameter)</a>
+      <li><a href="api.html#dogpile.cache.backends.memcached.PyMemcacheBackend.params.memcached_expire_time">memcached_expire_time (dogpile.cache.backends.memcached.PyMemcacheBackend parameter)</a>
 </li>
       <li><a href="api.html#dogpile.cache.backends.memcached.MemcachedBackend">MemcachedBackend (class in dogpile.cache.backends.memcached)</a>
 </li>
       <li><a href="api.html#dogpile.cache.backends.memcached.MemcachedLock">MemcachedLock (class in dogpile.cache.backends.memcached)</a>
 </li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
@@ -1170,40 +1170,40 @@
 
             <div class="clearer"></div>
           </div>
         </div>
       </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
         </div>
       </div>
       <div class="clearer"></div>
     </div>
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Index</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
     &#169; Copyright 2011-2024 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.2.6.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.3.7.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 ******** NNaavviiggaattiioonn ********
     * _i_n_d_e_x
     * _m_o_d_u_l_e_s |
-    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._2_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
+    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._3_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
     * Index
 ************ IInnddeexx ************
 _SS_yy_mm_bb_oo_ll_ss | _AA | _BB | _CC | _DD | _EE | _FF | _GG | _HH | _II | _KK | _LL | _MM | _NN | _PP | _RR | _SS | _TT | _UU
 | _VV | _WW
 ********** SSyymmbboollss **********
     * _*_*_k_w_ _(_d_o_g_p_i_l_e_._c_a_c_h_e_._p_l_u_g_i_n_s_._m_a_k_o___c_a_c_h_e_._M_a_k_o_P_l_u_g_i_n_._g_e_t_ _p_a_r_a_m_e_t_e_r_)
           o _(_d_o_g_p_i_l_e_._c_a_c_h_e_._p_l_u_g_i_n_s_._m_a_k_o___c_a_c_h_e_._M_a_k_o_P_l_u_g_i_n_._g_e_t___o_r___c_r_e_a_t_e
@@ -240,16 +240,16 @@
             _p_a_r_a_m_e_t_e_r_)                                                                _p_a_r_a_m_e_t_e_r_)
           o _(_d_o_g_p_i_l_e_._c_a_c_h_e_._b_a_c_k_e_n_d_s_._m_e_m_o_r_y_._M_e_m_o_r_y_B_a_c_k_e_n_d_._s_e_t___m_u_l_t_i_ _p_a_r_a_m_e_t_e_r_)       * module
           o _(_d_o_g_p_i_l_e_._c_a_c_h_e_._b_a_c_k_e_n_d_s_._n_u_l_l_._N_u_l_l_B_a_c_k_e_n_d_._s_e_t___m_u_l_t_i_ _p_a_r_a_m_e_t_e_r_)                 o _d_o_g_p_i_l_e_._c_a_c_h_e_._a_p_i
           o _(_d_o_g_p_i_l_e_._c_a_c_h_e_._b_a_c_k_e_n_d_s_._r_e_d_i_s_._R_e_d_i_s_B_a_c_k_e_n_d_._s_e_t___s_e_r_i_a_l_i_z_e_d___m_u_l_t_i               o _d_o_g_p_i_l_e_._c_a_c_h_e_._b_a_c_k_e_n_d_s_._f_i_l_e
             _p_a_r_a_m_e_t_e_r_)                                                                    o _d_o_g_p_i_l_e_._c_a_c_h_e_._b_a_c_k_e_n_d_s_._m_e_m_c_a_c_h_e_d
           o _(_d_o_g_p_i_l_e_._c_a_c_h_e_._p_r_o_x_y_._P_r_o_x_y_B_a_c_k_e_n_d_._s_e_t___m_u_l_t_i_ _p_a_r_a_m_e_t_e_r_)                        o _d_o_g_p_i_l_e_._c_a_c_h_e_._b_a_c_k_e_n_d_s_._m_e_m_o_r_y
           o _(_d_o_g_p_i_l_e_._c_a_c_h_e_._p_r_o_x_y_._P_r_o_x_y_B_a_c_k_e_n_d_._s_e_t___s_e_r_i_a_l_i_z_e_d___m_u_l_t_i_ _p_a_r_a_m_e_t_e_r_)             o _d_o_g_p_i_l_e_._c_a_c_h_e_._b_a_c_k_e_n_d_s_._n_u_l_l
-    * _m_e_m_c_a_c_h_e_d___e_x_p_i_r_e___t_i_m_e_                                                               o _d_o_g_p_i_l_e_._c_a_c_h_e_._b_a_c_k_e_n_d_s_._r_e_d_i_s
-      _(_d_o_g_p_i_l_e_._c_a_c_h_e_._b_a_c_k_e_n_d_s_._m_e_m_c_a_c_h_e_d_._G_e_n_e_r_i_c_M_e_m_c_a_c_h_e_d_B_a_c_k_e_n_d_ _p_a_r_a_m_e_t_e_r_)                o _d_o_g_p_i_l_e_._c_a_c_h_e_._e_x_c_e_p_t_i_o_n
+    * _m_e_m_c_a_c_h_e_d___e_x_p_i_r_e___t_i_m_e_ _(_d_o_g_p_i_l_e_._c_a_c_h_e_._b_a_c_k_e_n_d_s_._m_e_m_c_a_c_h_e_d_._P_y_M_e_m_c_a_c_h_e_B_a_c_k_e_n_d           o _d_o_g_p_i_l_e_._c_a_c_h_e_._b_a_c_k_e_n_d_s_._r_e_d_i_s
+      _p_a_r_a_m_e_t_e_r_)                                                                          o _d_o_g_p_i_l_e_._c_a_c_h_e_._e_x_c_e_p_t_i_o_n
     * _M_e_m_c_a_c_h_e_d_B_a_c_k_e_n_d_ _(_c_l_a_s_s_ _i_n_ _d_o_g_p_i_l_e_._c_a_c_h_e_._b_a_c_k_e_n_d_s_._m_e_m_c_a_c_h_e_d_)                        o _d_o_g_p_i_l_e_._c_a_c_h_e_._p_l_u_g_i_n_s_._m_a_k_o___c_a_c_h_e
     * _M_e_m_c_a_c_h_e_d_L_o_c_k_ _(_c_l_a_s_s_ _i_n_ _d_o_g_p_i_l_e_._c_a_c_h_e_._b_a_c_k_e_n_d_s_._m_e_m_c_a_c_h_e_d_)                           o _d_o_g_p_i_l_e_._c_a_c_h_e_._p_r_o_x_y
                                                                                           o _d_o_g_p_i_l_e_._c_a_c_h_e_._r_e_g_i_o_n
                                                                                     * _m_u_t_e_x_ _(_d_o_g_p_i_l_e_._L_o_c_k_ _p_a_r_a_m_e_t_e_r_)
 ********** NN **********
     * _n_a_m_e_ _(_d_o_g_p_i_l_e_._c_a_c_h_e_._r_e_g_i_o_n_._C_a_c_h_e_R_e_g_i_o_n_ _p_a_r_a_m_e_t_e_r_), _[_1_]         * _N_e_e_d_R_e_g_e_n_e_r_a_t_i_o_n_E_x_c_e_p_t_i_o_n_ 
     * _N_a_m_e_R_e_g_i_s_t_r_y_ _(_c_l_a_s_s_ _i_n_ _d_o_g_p_i_l_e_._u_t_i_l_)                             _(_c_l_a_s_s_ _i_n_ _d_o_g_p_i_l_e_)
@@ -391,10 +391,10 @@
           o _(_d_o_g_p_i_l_e_._c_a_c_h_e_._r_e_g_i_o_n_._R_e_g_i_o_n_I_n_v_a_l_i_d_a_t_i_o_n_S_t_r_a_t_e_g_y       _m_e_t_h_o_d_)
             _m_e_t_h_o_d_)
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
 ******** NNaavviiggaattiioonn ********
     * _i_n_d_e_x
     * _m_o_d_u_l_e_s |
-    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._2_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
+    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._3_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
     * Index
-© Copyright 2011-2024 Mike Bayer. Created using _S_p_h_i_n_x 7.2.6.
+© Copyright 2011-2024 Mike Bayer. Created using _S_p_h_i_n_x 7.3.7.
```

### Comparing `dogpile.cache-1.3.2/docs/index.html` & `dogpile.cache-1.3.3/docs/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Welcome to dogpile.cache’s documentation! &#8212; dogpile.cache 1.3.2 documentation</title>
+    <title>Welcome to dogpile.cache’s documentation! &#8212; dogpile.cache 1.3.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css?v=d00006d9" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
-    <script src="_static/documentation_options.js?v=8ca9e7a0"></script>
-    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/documentation_options.js?v=28d163b9"></script>
+    <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Front Matter" href="front.html" /> 
   </head><body>
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
@@ -25,15 +25,15 @@
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="front.html" title="Front Matter"
              accesskey="N">next</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">dogpile.cache 1.3.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="#">dogpile.cache 1.3.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Welcome to dogpile.cache’s documentation!</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -92,14 +92,15 @@
 <li class="toctree-l2"><a class="reference internal" href="api.html#module-dogpile.cache.exception">Exceptions</a></li>
 <li class="toctree-l2"><a class="reference internal" href="api.html#module-dogpile.cache.plugins.mako_cache">Plugins</a></li>
 <li class="toctree-l2"><a class="reference internal" href="api.html#utilities">Utilities</a></li>
 <li class="toctree-l2"><a class="reference internal" href="api.html#dogpile-core">dogpile Core</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="changelog.html">Changelog</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.3.3">1.3.3</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.3.2">1.3.2</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.3.1">1.3.1</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.3.0">1.3.0</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.2.2">1.2.2</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.2.1">1.2.1</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.2.0">1.2.0</a></li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.1.8">1.1.8</a></li>
@@ -177,23 +178,23 @@
 <li><a class="reference internal" href="#">Welcome to dogpile.cache’s documentation!</a><ul>
 <li><a class="reference internal" href="#indices-and-tables">Indices and tables</a></li>
 </ul>
 </li>
 </ul>
 
   </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
   <div>
     <h4>Next topic</h4>
     <p class="topless"><a href="front.html"
                           title="next chapter">Front Matter</a></p>
   </div>
         </div>
@@ -208,17 +209,17 @@
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="front.html" title="Front Matter"
              >next</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">dogpile.cache 1.3.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="#">dogpile.cache 1.3.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Welcome to dogpile.cache’s documentation!</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
     &#169; Copyright 2011-2024 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.2.6.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.3.7.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 ******** NNaavviiggaattiioonn ********
     * _i_n_d_e_x
     * _m_o_d_u_l_e_s |
     * _n_e_x_t |
-    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._2_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
+    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._3_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
     * Welcome to dogpile.cache’s documentation!
 ************ WWeellccoommee ttoo ddooggppiillee..ccaacchhee?’ss ddooccuummeennttaattiioonn!!_?¶ ************
 Dogpile consists of two subsystems, one building on top of the other.
 dogpile provides the concept of a “dogpile lock”, a control structure which
 allows a single thread of execution to be selected as the “creator” of some
 resource, while allowing other threads of execution to refer to the previous
 version of this resource as the creation proceeds; if there is no previous
@@ -44,14 +44,15 @@
           o _B_a_c_k_e_n_d_ _A_P_I
           o _B_a_c_k_e_n_d_s
           o _E_x_c_e_p_t_i_o_n_s
           o _P_l_u_g_i_n_s
           o _U_t_i_l_i_t_i_e_s
           o _d_o_g_p_i_l_e_ _C_o_r_e
     * _C_h_a_n_g_e_l_o_g
+          o _1_._3_._3
           o _1_._3_._2
           o _1_._3_._1
           o _1_._3_._0
           o _1_._2_._2
           o _1_._2_._1
           o _1_._2_._0
           o _1_._1_._8
@@ -113,10 +114,10 @@
 [q                   ][Go]
 ****** NNeexxtt ttooppiicc ******
 _F_r_o_n_t_ _M_a_t_t_e_r
 ******** NNaavviiggaattiioonn ********
     * _i_n_d_e_x
     * _m_o_d_u_l_e_s |
     * _n_e_x_t |
-    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._2_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
+    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._3_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
     * Welcome to dogpile.cache’s documentation!
-© Copyright 2011-2024 Mike Bayer. Created using _S_p_h_i_n_x 7.2.6.
+© Copyright 2011-2024 Mike Bayer. Created using _S_p_h_i_n_x 7.3.7.
```

### Comparing `dogpile.cache-1.3.2/docs/py-modindex.html` & `dogpile.cache-1.3.3/docs/py-modindex.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Python Module Index &#8212; dogpile.cache 1.3.2 documentation</title>
+    <title>Python Module Index &#8212; dogpile.cache 1.3.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css?v=d00006d9" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
-    <script src="_static/documentation_options.js?v=8ca9e7a0"></script>
-    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/documentation_options.js?v=28d163b9"></script>
+    <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
  
 
 
   </head><body>
@@ -23,15 +23,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Python Module Index</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -109,40 +109,40 @@
 
             <div class="clearer"></div>
           </div>
         </div>
       </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
         </div>
       </div>
       <div class="clearer"></div>
     </div>
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Python Module Index</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
     &#169; Copyright 2011-2024 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.2.6.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.3.7.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 ******** NNaavviiggaattiioonn ********
     * _i_n_d_e_x
     * _m_o_d_u_l_e_s |
-    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._2_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
+    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._3_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
     * Python Module Index
 ************ PPyytthhoonn MMoodduullee IInnddeexx ************
 _dd
      
     dd
 [-] dogpile
         _d_o_g_p_i_l_e_._c_a_c_h_e_._a_p_i
@@ -19,10 +19,10 @@
         _d_o_g_p_i_l_e_._c_a_c_h_e_._p_r_o_x_y
         _d_o_g_p_i_l_e_._c_a_c_h_e_._r_e_g_i_o_n
 ******** QQuuiicckk sseeaarrcchh ********
 [q                   ][Go]
 ******** NNaavviiggaattiioonn ********
     * _i_n_d_e_x
     * _m_o_d_u_l_e_s |
-    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._2_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
+    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._3_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
     * Python Module Index
-© Copyright 2011-2024 Mike Bayer. Created using _S_p_h_i_n_x 7.2.6.
+© Copyright 2011-2024 Mike Bayer. Created using _S_p_h_i_n_x 7.3.7.
```

### Comparing `dogpile.cache-1.3.2/docs/recipes.html` & `dogpile.cache-1.3.3/docs/recipes.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Recipes &#8212; dogpile.cache 1.3.2 documentation</title>
+    <title>Recipes &#8212; dogpile.cache 1.3.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css?v=d00006d9" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
-    <script src="_static/documentation_options.js?v=8ca9e7a0"></script>
-    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/documentation_options.js?v=28d163b9"></script>
+    <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="dogpile Core" href="core_usage.html" />
     <link rel="prev" title="Usage Guide" href="usage.html" /> 
   </head><body>
     <div class="related" role="navigation" aria-label="related navigation">
@@ -29,15 +29,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="core_usage.html" title="dogpile Core"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="usage.html" title="Usage Guide"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Recipes</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -302,23 +302,23 @@
 <li><a class="reference internal" href="#prefixing-all-keys-in-redis">Prefixing all keys in Redis</a></li>
 <li><a class="reference internal" href="#encoding-decoding-data-into-another-format">Encoding/Decoding data into another format</a></li>
 </ul>
 </li>
 </ul>
 
   </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
   <div>
     <h4>Previous topic</h4>
     <p class="topless"><a href="usage.html"
                           title="previous chapter">Usage Guide</a></p>
   </div>
   <div>
@@ -341,17 +341,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="core_usage.html" title="dogpile Core"
              >next</a> |</li>
         <li class="right" >
           <a href="usage.html" title="Usage Guide"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Recipes</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
     &#169; Copyright 2011-2024 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.2.6.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.3.7.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 ******** NNaavviiggaattiioonn ********
     * _i_n_d_e_x
     * _m_o_d_u_l_e_s |
     * _n_e_x_t |
     * _p_r_e_v_i_o_u_s |
-    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._2_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
+    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._3_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
     * Recipes
 ************ RReecciippeess_?¶ ************
 ********** IInnvvaalliiddaattiinngg aa ggrroouupp ooff rreellaatteedd kkeeyyss_?¶ **********
 This recipe presents a way to track the cache keys related to a particular
 region, for the purposes of invalidating a series of keys that relate to a
 particular id.
 Three cached functions, user_fn_one(), user_fn_two(), user_fn_three() each
@@ -235,10 +235,10 @@
 ****** NNeexxtt ttooppiicc ******
 _d_o_g_p_i_l_e_ _C_o_r_e
 ******** NNaavviiggaattiioonn ********
     * _i_n_d_e_x
     * _m_o_d_u_l_e_s |
     * _n_e_x_t |
     * _p_r_e_v_i_o_u_s |
-    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._2_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
+    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._3_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
     * Recipes
-© Copyright 2011-2024 Mike Bayer. Created using _S_p_h_i_n_x 7.2.6.
+© Copyright 2011-2024 Mike Bayer. Created using _S_p_h_i_n_x 7.3.7.
```

### Comparing `dogpile.cache-1.3.2/docs/search.html` & `dogpile.cache-1.3.3/docs/search.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; dogpile.cache 1.3.2 documentation</title>
+    <title>Search &#8212; dogpile.cache 1.3.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css?v=d00006d9" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     
-    <script src="_static/documentation_options.js?v=8ca9e7a0"></script>
-    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/documentation_options.js?v=28d163b9"></script>
+    <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <script src="_static/searchtools.js"></script>
     <script src="_static/language_data.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="#" />
-  <script src="searchindex.js" defer></script>
-   
+    <script src="searchindex.js" defer="defer"></script>
+    <meta name="robots" content="noindex" />
+     
 
   </head><body>
     <div class="related" role="navigation" aria-label="related navigation">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -61,18 +62,15 @@
   <form action="" method="get">
     <input type="text" name="q" aria-labelledby="search-documentation" value="" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
     <input type="submit" value="search" />
     <span id="search-progress" style="padding-left: 10px"></span>
   </form>
   
   
-  
-  <div id="search-results">
-  
-  </div>
+  <div id="search-results"></div>
   
 
             <div class="clearer"></div>
           </div>
         </div>
       </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
@@ -86,17 +84,17 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
     &#169; Copyright 2011-2024 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.2.6.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.3.7.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 ******** NNaavviiggaattiioonn ********
     * _i_n_d_e_x
     * _m_o_d_u_l_e_s |
-    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._2_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
+    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._3_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
     * Search
 ************ SSeeaarrcchh ************
 Please activate JavaScript to enable the search functionality.
 Searching for multiple words only shows matches that contain all words.
 [q                   ][search]
 ******** NNaavviiggaattiioonn ********
     * _i_n_d_e_x
     * _m_o_d_u_l_e_s |
-    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._2_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
+    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._3_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
     * Search
-© Copyright 2011-2024 Mike Bayer. Created using _S_p_h_i_n_x 7.2.6.
+© Copyright 2011-2024 Mike Bayer. Created using _S_p_h_i_n_x 7.3.7.
```

### Comparing `dogpile.cache-1.3.2/docs/searchindex.js` & `dogpile.cache-1.3.3/docs/searchindex.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,1723 +1,960 @@
 Search.setIndex({
+    "alltitles": {
+        "0.1.0": [
+            [1, "change-0.1.0"]
+        ],
+        "0.1.1": [
+            [1, "change-0.1.1"]
+        ],
+        "0.2.0": [
+            [1, "change-0.2.0"]
+        ],
+        "0.2.1": [
+            [1, "change-0.2.1"]
+        ],
+        "0.2.2": [
+            [1, "change-0.2.2"]
+        ],
+        "0.2.3": [
+            [1, "change-0.2.3"]
+        ],
+        "0.2.4": [
+            [1, "change-0.2.4"]
+        ],
+        "0.3.0": [
+            [1, "change-0.3.0"]
+        ],
+        "0.3.1": [
+            [1, "change-0.3.1"]
+        ],
+        "0.4.0": [
+            [1, "change-0.4.0"]
+        ],
+        "0.4.1": [
+            [1, "change-0.4.1"]
+        ],
+        "0.4.2": [
+            [1, "change-0.4.2"]
+        ],
+        "0.4.3": [
+            [1, "change-0.4.3"]
+        ],
+        "0.5.0": [
+            [1, "change-0.5.0"]
+        ],
+        "0.5.1": [
+            [1, "change-0.5.1"]
+        ],
+        "0.5.2": [
+            [1, "change-0.5.2"]
+        ],
+        "0.5.3": [
+            [1, "change-0.5.3"]
+        ],
+        "0.5.4": [
+            [1, "change-0.5.4"]
+        ],
+        "0.5.5": [
+            [1, "change-0.5.5"]
+        ],
+        "0.5.6": [
+            [1, "change-0.5.6"]
+        ],
+        "0.5.7": [
+            [1, "change-0.5.7"]
+        ],
+        "0.6.0": [
+            [1, "change-0.6.0"]
+        ],
+        "0.6.1": [
+            [1, "change-0.6.1"]
+        ],
+        "0.6.2": [
+            [1, "change-0.6.2"]
+        ],
+        "0.6.3": [
+            [1, "change-0.6.3"]
+        ],
+        "0.6.4": [
+            [1, "change-0.6.4"]
+        ],
+        "0.6.5": [
+            [1, "change-0.6.5"]
+        ],
+        "0.6.6": [
+            [1, "change-0.6.6"]
+        ],
+        "0.6.7": [
+            [1, "change-0.6.7"]
+        ],
+        "0.6.8": [
+            [1, "change-0.6.8"]
+        ],
+        "0.7.0": [
+            [1, "change-0.7.0"]
+        ],
+        "0.7.1": [
+            [1, "change-0.7.1"]
+        ],
+        "0.8.0": [
+            [1, "change-0.8.0"]
+        ],
+        "0.9.0": [
+            [1, "change-0.9.0"]
+        ],
+        "0.9.1": [
+            [1, "change-0.9.1"]
+        ],
+        "0.9.2": [
+            [1, "change-0.9.2"]
+        ],
+        "1.0.0": [
+            [1, "change-1.0.0"]
+        ],
+        "1.0.1": [
+            [1, "change-1.0.1"]
+        ],
+        "1.0.2": [
+            [1, "change-1.0.2"]
+        ],
+        "1.1.0": [
+            [1, "change-1.1.0"]
+        ],
+        "1.1.1": [
+            [1, "change-1.1.1"]
+        ],
+        "1.1.2": [
+            [1, "change-1.1.2"]
+        ],
+        "1.1.3": [
+            [1, "change-1.1.3"]
+        ],
+        "1.1.4": [
+            [1, "change-1.1.4"]
+        ],
+        "1.1.5": [
+            [1, "change-1.1.5"]
+        ],
+        "1.1.6": [
+            [1, "change-1.1.6"]
+        ],
+        "1.1.7": [
+            [1, "change-1.1.7"]
+        ],
+        "1.1.8": [
+            [1, "change-1.1.8"]
+        ],
+        "1.2.0": [
+            [1, "change-1.2.0"]
+        ],
+        "1.2.1": [
+            [1, "change-1.2.1"]
+        ],
+        "1.2.2": [
+            [1, "change-1.2.2"]
+        ],
+        "1.3.0": [
+            [1, "change-1.3.0"]
+        ],
+        "1.3.1": [
+            [1, "change-1.3.1"]
+        ],
+        "1.3.2": [
+            [1, "change-1.3.2"]
+        ],
+        "1.3.3": [
+            [1, "change-1.3.3"]
+        ],
+        "A Note on Data Encoding": [
+            [5, null]
+        ],
+        "API": [
+            [0, "api"]
+        ],
+        "Asynchronous Data Updates with ORM Events": [
+            [5, "asynchronous-data-updates-with-orm-events"]
+        ],
+        "Backend API": [
+            [0, "backend-api"]
+        ],
+        "Backends": [
+            [0, "module-dogpile.cache.backends.memory"]
+        ],
+        "Bugs": [
+            [3, "bugs"]
+        ],
+        "Changelog": [
+            [1, "changelog"]
+        ],
+        "Changing Backend Behavior": [
+            [6, "changing-backend-behavior"]
+        ],
+        "Configuring Logging": [
+            [6, "configuring-logging"]
+        ],
+        "Creating Backends": [
+            [6, "creating-backends"]
+        ],
+        "Do I Need to Learn the dogpile Core API Directly?": [
+            [2, "do-i-need-to-learn-the-dogpile-core-api-directly"]
+        ],
+        "Encoding/Decoding data into another format": [
+            [5, "encoding-decoding-data-into-another-format"]
+        ],
+        "Example: Using dogpile directly for Caching": [
+            [2, "example-using-dogpile-directly-for-caching"]
+        ],
+        "Exceptions": [
+            [0, "module-dogpile.cache.exception"]
+        ],
+        "File Backends": [
+            [0, "file-backends"]
+        ],
+        "Front Matter": [
+            [3, "front-matter"]
+        ],
+        "Indices and tables": [
+            [4, "indices-and-tables"]
+        ],
+        "Installation": [
+            [3, "installation"]
+        ],
+        "Invalidating a group of related keys": [
+            [5, "invalidating-a-group-of-related-keys"]
+        ],
+        "Mako Integration": [
+            [0, "mako-integration"]
+        ],
+        "Memcached Backends": [
+            [0, "memcached-backends"]
+        ],
+        "Memory Backends": [
+            [0, "memory-backends"]
+        ],
+        "Null Backend": [
+            [0, "null-backend"]
+        ],
+        "Overview": [
+            [6, "overview"]
+        ],
+        "Plugins": [
+            [0, "module-dogpile.cache.plugins.mako_cache"]
+        ],
+        "Prefixing all keys in Redis": [
+            [5, "prefixing-all-keys-in-redis"]
+        ],
+        "Project Homepage": [
+            [3, "project-homepage"]
+        ],
+        "Proxy Backends": [
+            [0, "proxy-backends"]
+        ],
+        "Recipes": [
+            [5, "recipes"]
+        ],
+        "Redis Backends": [
+            [0, "redis-backends"]
+        ],
+        "Region": [
+            [0, "module-dogpile.cache.region"]
+        ],
+        "Region Configuration": [
+            [6, "region-configuration"]
+        ],
+        "Rudimentary Usage": [
+            [2, "rudimentary-usage"],
+            [6, "rudimentary-usage"]
+        ],
+        "Usage Guide": [
+            [6, "usage-guide"]
+        ],
+        "Using a File or Distributed Lock with Dogpile": [
+            [2, "using-a-file-or-distributed-lock-with-dogpile"]
+        ],
+        "Using a Region": [
+            [6, "using-a-region"]
+        ],
+        "Utilities": [
+            [0, "utilities"]
+        ],
+        "Welcome to dogpile.cache\u2019s documentation!": [
+            [4, "welcome-to-dogpile-cache-s-documentation"]
+        ],
+        "bug": [
+            [1, "change-1.3.3-bug"],
+            [1, "change-1.2.2-bug"],
+            [1, "change-1.2.1-bug"],
+            [1, "change-1.1.8-bug"],
+            [1, "change-1.1.6-bug"],
+            [1, "change-1.1.4-bug"],
+            [1, "change-1.1.3-bug"],
+            [1, "change-1.1.1-bug"],
+            [1, "change-1.0.2-bug"],
+            [1, "change-1.0.1-bug"],
+            [1, "change-0.9.2-bug"],
+            [1, "change-0.9.1-bug"],
+            [1, "change-0.8.0-bug"],
+            [1, "change-0.7.1-bug"],
+            [1, "change-0.7.0-bug"],
+            [1, "change-0.6.7-bug"],
+            [1, "change-0.6.6-bug"],
+            [1, "change-0.6.5-bug"],
+            [1, "change-0.6.4-bug"],
+            [1, "change-0.6.2-bug"],
+            [1, "change-0.6.1-bug"],
+            [1, "change-0.6.0-bug"],
+            [1, "change-0.5.7-bug"],
+            [1, "change-0.5.5-bug"],
+            [1, "change-0.5.4-bug"],
+            [1, "change-0.5.3-bug"],
+            [1, "change-0.5.2-bug"],
+            [1, "change-0.5.1-bug"],
+            [1, "change-0.5.0-bug"],
+            [1, "change-0.4.3-bug"],
+            [1, "change-0.4.1-bug"],
+            [1, "change-0.4.0-bug"],
+            [1, "change-0.3.1-bug"],
+            [1, "change-0.3.0-bug"]
+        ],
+        "dogpile Core": [
+            [0, "dogpile-core"],
+            [2, "dogpile-core"]
+        ],
+        "feature": [
+            [1, "change-1.3.0-feature"],
+            [1, "change-1.2.0-feature"],
+            [1, "change-1.1.2-feature"],
+            [1, "change-1.1.0-feature"],
+            [1, "change-1.0.2-feature"],
+            [1, "change-1.0.0-feature"],
+            [1, "change-0.9.0-feature"],
+            [1, "change-0.6.6-feature"],
+            [1, "change-0.6.3-feature"],
+            [1, "change-0.6.2-feature"],
+            [1, "change-0.6.0-feature"],
+            [1, "change-0.5.7-feature"],
+            [1, "change-0.5.6-feature"],
+            [1, "change-0.5.5-feature"],
+            [1, "change-0.5.4-feature"],
+            [1, "change-0.5.3-feature"],
+            [1, "change-0.5.2-feature"],
+            [1, "change-0.5.1-feature"],
+            [1, "change-0.5.0-feature"],
+            [1, "change-0.4.3-feature"],
+            [1, "change-0.4.2-feature"],
+            [1, "change-0.4.1-feature"],
+            [1, "change-0.3.0-feature"]
+        ],
+        "misc": [
+            [1, "change-1.3.0-misc"],
+            [1, "change-1.1.0-misc"],
+            [1, "change-1.0.0-misc"],
+            [1, "change-0.5.0-misc"]
+        ],
+        "pylibmc": [
+            [6, null]
+        ],
+        "usecase": [
+            [1, "change-1.3.3-usecase"],
+            [1, "change-1.3.2-usecase"],
+            [1, "change-1.3.1-usecase"],
+            [1, "change-1.1.7-usecase"],
+            [1, "change-1.1.6-usecase"],
+            [1, "change-1.1.5-usecase"],
+            [1, "change-1.1.4-usecase"]
+        ]
+    },
     "docnames": ["api", "changelog", "core_usage", "front", "index", "recipes", "usage"],
+    "envversion": {
+        "sphinx": 61,
+        "sphinx.domains.c": 3,
+        "sphinx.domains.changeset": 1,
+        "sphinx.domains.citation": 1,
+        "sphinx.domains.cpp": 9,
+        "sphinx.domains.index": 1,
+        "sphinx.domains.javascript": 3,
+        "sphinx.domains.math": 2,
+        "sphinx.domains.python": 4,
+        "sphinx.domains.rst": 2,
+        "sphinx.domains.std": 2,
+        "sphinx.ext.intersphinx": 1
+    },
     "filenames": ["api.rst", "changelog.rst", "core_usage.rst", "front.rst", "index.rst", "recipes.rst", "usage.rst"],
-    "titles": ["API", "Changelog", "dogpile Core", "Front Matter", "Welcome to dogpile.cache\u2019s documentation!", "Recipes", "Usage Guide"],
-    "terms": {
-        "class": [0, 1, 2, 5, 6],
-        "cach": [0, 1, 3, 5, 6],
-        "cacheregion": [0, 1, 5, 6],
-        "name": [0, 1, 6],
-        "str": [0, 1, 5, 6],
-        "none": [0, 1, 2, 6],
-        "function_key_gener": [0, 1, 5, 6],
-        "type": [0, 1, 6],
-        "callabl": [0, 1, 5, 6],
-        "function": [0, 1, 2, 5, 6],
-        "function_multi_key_gener": [0, 1, 6],
-        "sequenc": [0, 5, 6],
-        "key_mangl": [0, 1, 5, 6],
-        "serial": [0, 1, 5, 6],
-        "ani": [0, 1, 2, 4, 6],
-        "byte": [0, 1, 6],
-        "deseri": [0, 1, 6],
-        "async_creation_runn": [0, 1, 5, 6],
-        "cachemutex": [0, 6],
-        "base": [0, 1, 2, 5, 6],
-        "object": [0, 1, 2, 4, 6],
-        "A": [0, 1, 2, 6],
-        "front": [0, 2, 4, 6],
-        "end": [0, 1, 2, 6],
-        "particular": [0, 1, 2, 5, 6],
-        "paramet": [0, 1, 6],
-        "option": [0, 1, 6],
-        "string": [0, 1, 6],
-        "thi": [0, 1, 2, 3, 4, 5, 6],
-        "isn": [0, 1, 6],
-        "t": [0, 1, 2, 5, 6],
-        "us": [0, 1, 4, 5],
-        "intern": [0, 1, 2, 6],
-        "can": [0, 1, 2, 5, 6],
-        "access": [0, 1, 2, 6],
-        "via": [0, 1, 2, 5, 6],
-        "help": [0, 5, 6],
-        "configur": [0, 1, 4, 5],
-        "from": [0, 1, 2, 3, 5, 6],
-        "config": [0, 1, 6],
-        "produc": [0, 1, 6],
-        "kei": [0, 1, 2, 4, 6],
-        "given": [0, 1, 2, 5, 6],
-        "data": [0, 4, 6],
-        "creation": [0, 1, 2, 4, 6],
-        "argument": [0, 1, 2, 5, 6],
-        "when": [0, 1, 2, 5, 6],
-        "cache_on_argu": [0, 1, 5, 6],
-        "method": [0, 1, 5, 6],
-        "The": [0, 1, 2, 3, 5, 6],
-        "structur": [0, 1, 4, 6],
-        "should": [0, 1, 3, 6],
-        "two": [0, 2, 4, 5, 6],
-        "level": [0, 1, 2, 6],
-        "return": [0, 1, 2, 5, 6],
-        "new": [0, 1, 2, 4, 5, 6],
-        "gener": [0, 1, 2, 4, 5, 6],
-        "Such": [0, 6],
-        "def": [0, 2, 5, 6],
-        "my_key_gener": [0, 5, 6],
-        "namespac": [0, 1, 5, 6],
-        "fn": [0, 2, 5, 6],
-        "kw": [0, 6],
-        "fname": [0, 5, 6],
-        "__name__": [0, 5, 6],
-        "generate_kei": [0, 5, 6],
-        "arg": [0, 5, 6],
-        "_": [0, 5, 6],
-        "join": [0, 2, 5, 6],
-        "": [0, 1, 2, 5, 6],
-        "make_region": [0, 5, 6],
-        "dbm": [0, 1, 6],
-        "expiration_tim": [0, 1, 2, 5, 6],
-        "300": [0, 6],
-        "filenam": [0, 2, 6],
-        "i": [0, 1, 3, 4, 5, 6],
-        "pass": [0, 1, 2, 5, 6],
-        "It": [0, 2, 6],
-        "consult": [0, 6],
-        "outsid": [0, 2, 6],
-        "so": [0, 1, 2, 5, 6],
-        "fact": [0, 6],
-        "form": [0, 1, 6],
-        "For": [0, 1, 2, 6],
-        "exampl": [0, 1, 4, 5, 6],
-        "tupl": [0, 2, 6],
-        "specifi": [0, 1, 5, 6],
-        "pluck": [0, 6],
-        "k": [0, 5, 6],
-        "x": [0, 1, 6],
-        "where": [0, 1, 2, 6],
-        "decor": [0, 1, 2, 5, 6],
-        "might": [0, 6],
-        "my_region": [0, 6],
-        "y": [0, 6],
-        "my_funct": [0, 6],
-        "b": [0, 6],
-        "my_data": [0, 6],
-        "default": [0, 1, 5, 6],
-        "kwarg_function_key_gener": [0, 1, 6],
-        "gen": [0, 6],
-        "also": [0, 1, 2, 5, 6],
-        "keyword": [0, 1, 6],
-        "similar": [0, 1, 3, 6],
-        "cache_multi_on_argu": [0, 1, 6],
-        "list": [0, 1, 6],
-        "my_multi_key_gener": [0, 6],
-        "which": [0, 1, 2, 4, 5, 6],
-        "all": [0, 1, 2, 4, 6],
-        "incom": [0, 1, 6],
-        "befor": [0, 1, 2, 6],
-        "case": [0, 1, 2, 5, 6],
-        "mangl": [0, 1, 5, 6],
-        "recommend": [0, 6],
-        "typic": [0, 5, 6],
-        "mangler": [0, 1, 5, 6],
-        "sha1": [0, 2, 6],
-        "found": [0, 6],
-        "sha1_mangle_kei": [0, 1, 6],
-        "coerc": [0, 1, 6],
-        "hash": [0, 6],
-        "length": [0, 1, 6],
-        "fix": [0, 1, 6],
-        "To": [0, 6],
-        "disabl": [0, 1, 6],
-        "set": [0, 1, 5, 6],
-        "fals": [0, 1, 5, 6],
-        "anoth": [0, 1, 2, 4, 6],
-        "built": [0, 6],
-        "python": [0, 1, 2, 3, 5, 6],
-        "convert": [0, 6],
-        "non": [0, 1, 2, 6],
-        "unicod": [0, 1, 6],
-        "bytestr": [0, 1, 6],
-        "need": [0, 1, 4, 5, 6],
-        "bsddb": [0, 6],
-        "under": [0, 1, 5, 6],
-        "2": [0, 4, 5, 6],
-        "conjunct": [0, 1, 6],
-        "appli": [0, 1, 5, 6],
-        "valu": [0, 1, 2, 5, 6],
-        "includ": [0, 1, 6],
-        "pickl": [0, 1, 5, 6],
-        "dump": [0, 1, 6],
-        "json": [0, 1, 5, 6],
-        "version": [0, 1, 2, 3, 4, 6],
-        "1": [0, 4, 5, 6],
-        "0": [0, 2, 4, 5, 6],
-        "rais": [0, 1, 2, 5, 6],
-        "cantdeserializeexcept": [0, 1, 6],
-        "thei": [0, 1, 2, 6],
-        "ar": [0, 1, 3, 4, 6],
-        "unabl": [0, 6],
-        "indic": [0, 1, 6],
-        "fail": [0, 1, 6],
-        "proce": [0, 1, 2, 4, 6],
-        "re": [0, 1, 2, 5, 6],
-        "allow": [0, 1, 2, 4, 6],
-        "an": [0, 1, 2, 4, 5, 6],
-        "applic": [0, 1, 2, 4, 6],
-        "ha": [0, 1, 2, 5, 6],
-        "been": [0, 1, 2, 5, 6],
-        "updat": [0, 1, 4, 6],
-        "gracefulli": [0, 1, 6],
-        "old": [0, 1, 5, 6],
-        "item": [0, 1, 6],
-        "were": [0, 1, 6],
-        "persist": [0, 1, 5, 6],
-        "previou": [0, 1, 2, 4, 6],
-        "longer": [0, 1, 6],
-        "successfulli": [0, 2, 6],
-        "ad": [0, 1, 2, 6],
-        "support": [0, 1, 6],
-        "call": [0, 1, 2, 5, 6],
-        "lock": [0, 1, 4, 6],
-        "stale": [0, 2, 6],
-        "present": [0, 1, 5, 6],
-        "mutex": [0, 2, 6],
-        "respons": [0, 6],
-        "releas": [0, 1, 3, 6],
-        "finish": [0, 2, 6],
-        "defer": [0, 2, 6],
-        "comput": [0, 6],
-        "expens": [0, 2, 6],
-        "creator": [0, 1, 4, 6],
-        "later": [0, 6],
-        "point": [0, 1, 5, 6],
-        "futur": [0, 1, 6],
-        "wai": [0, 1, 5, 6],
-        "background": [0, 5, 6],
-        "thread": [0, 1, 2, 4, 5, 6],
-        "long": [0, 1, 6],
-        "run": [0, 1, 6],
-        "queue": [0, 6],
-        "task": [0, 6],
-        "manag": [0, 2, 5, 6],
-        "system": [0, 1, 2, 5, 6],
-        "like": [0, 1, 2, 5, 6],
-        "celeri": [0, 6],
-        "specif": [0, 1, 4, 6],
-        "creat": [0, 1, 2, 4],
-        "import": [0, 1, 2, 5, 6],
-        "somekei": [0, 6],
-        "appropri": [0, 6],
-        "runner": [0, 1, 6],
-        "try": [0, 5, 6],
-        "final": [0, 6],
-        "target": [0, 5, 6],
-        "start": [0, 5, 6],
-        "5": [0, 4, 5, 6],
-        "url": [0, 1, 5, 6],
-        "127": [0, 5, 6],
-        "11211": [0, 6],
-        "distributed_lock": [0, 1, 6],
-        "true": [0, 1, 5, 6],
-        "rememb": [0, 6],
-        "first": [0, 1, 2, 6],
-        "request": [0, 1, 6],
-        "associ": [0, 5, 6],
-        "alwai": [0, 6],
-        "block": [0, 2, 4, 5, 6],
-        "async_cr": [0, 6],
-        "invok": [0, 2, 6],
-        "howev": [0, 1, 2, 5, 6],
-        "subsequ": [0, 1, 6],
-        "expir": [0, 1, 2, 6],
-        "still": [0, 1, 2, 5, 6],
-        "promptli": [0, 6],
-        "refresh": [0, 1, 5, 6],
-        "whatev": [0, 6],
-        "asynchron": [0, 1, 4, 6],
-        "mean": [0, 1, 5, 6],
-        "provid": [0, 1, 2, 4, 6],
-        "implement": [0, 1, 5, 6],
-        "By": [0, 6],
-        "4": [0, 4, 5, 6],
-        "featur": [0, 3, 6],
-        "properti": 0,
-        "actual_backend": [0, 1],
-        "ultim": [0, 1, 2, 6],
-        "underneath": [0, 6],
-        "result": [0, 1, 5, 6],
-        "one": [0, 1, 2, 4, 5, 6],
-        "more": [0, 1, 2, 6],
-        "wrap": [0, 1, 5, 6],
-        "If": [0, 2, 5, 6],
-        "deriv": [0, 6],
-        "actual": [0, 1, 2, 5, 6],
-        "underli": [0, 6],
-        "6": [0, 2, 4, 6],
-        "float": [0, 1, 6],
-        "should_cache_fn": [0, 1, 6],
-        "bool": [0, 6],
-        "asdict": [0, 1],
-        "to_str": [0, 1, 6],
-        "map": [0, 1, 5, 6],
-        "multipl": [0, 1, 2, 6],
-        "itself": [0, 1, 2, 6],
-        "analogu": 0,
-        "someregion": [0, 6],
-        "generate_someth": [0, 6],
-        "somedatabas": [0, 6],
-        "queri": [0, 5, 6],
-        "normal": [0, 2, 6],
-        "mechan": [0, 1, 4, 6],
-        "combin": [0, 6],
-        "each": [0, 1, 2, 5, 6],
-        "same": [0, 1, 2, 6],
-        "get_multi": [0, 1, 5, 6],
-        "retriev": [0, 1, 2, 6],
-        "current": [0, 1, 2, 6],
-        "origin": [0, 1, 6],
-        "correspond": 0,
-        "those": [0, 1, 4, 5, 6],
-        "aren": 0,
-        "regener": [0, 1, 2, 6],
-        "assembl": 0,
-        "subset": 0,
-        "key1": 0,
-        "key2": 0,
-        "key3": 0,
-        "make": [0, 1, 2, 6],
-        "get_or_create_multi": [0, 1, 5, 6],
-        "condition": [0, 6],
-        "see": [0, 1, 2, 6],
-        "addit": [0, 1, 2, 6],
-        "behavior": [0, 1, 4, 5],
-        "detail": [0, 6],
-        "unlik": [0, 2],
-        "work": [0, 1, 2, 5],
-        "onli": [0, 1, 2, 5, 6],
-        "singl": [0, 1, 2, 4, 6],
-        "signatur": [0, 1],
-        "take": [0, 1, 6],
-        "simpl": [0, 1, 2, 5, 6],
-        "here": [0, 2, 6],
-        "accept": [0, 1, 6],
-        "k1": 0,
-        "value1": 0,
-        "k2": 0,
-        "value2": 0,
-        "k3": 0,
-        "value3": 0,
-        "invalid": [0, 1, 4, 6],
-        "effect": [0, 1],
-        "delet": [0, 1, 5, 6],
-        "delete_multi": [0, 1],
-        "them": [0, 1, 5],
-        "get": [0, 1, 2, 5, 6],
-        "3": [0, 4, 6],
-        "have": [0, 1, 2, 5, 6],
-        "establish": [0, 1, 6],
-        "part": [0, 1, 6],
-        "overrid": [0, 5, 6],
-        "time": [0, 1, 2, 6],
-        "mai": [0, 1, 2, 5, 6],
-        "integ": [0, 1, 5, 6],
-        "place": [0, 1, 5, 6],
-        "its": [0, 1, 2, 4, 6],
-        "dictionari": [0, 1, 6],
-        "left": [0, 1],
-        "miss": [0, 1, 6],
-        "order": [0, 1, 2, 5, 6],
-        "ascii": [0, 6],
-        "builtin": [0, 6],
-        "substitut": [0, 6],
-        "note": [0, 2, 6],
-        "requir": [0, 1, 2, 4, 6],
-        "reach": [0, 2, 6],
-        "supersed": [0, 6],
-        "get_or_cr": [0, 1, 6],
-        "e": [0, 1, 5, 6],
-        "g": [0, 1, 6],
-        "pull": [0, 1, 5, 6],
-        "unless": [0, 2, 6],
-        "attribut": [0, 1, 6],
-        "you": [0, 2, 5, 6],
-        "d": [0, 2, 5, 6],
-        "repres": [0, 6],
-        "extra": [0, 6],
-        "possibl": [0, 5, 6],
-        "rel": [0, 6],
-        "conveni": [0, 6],
-        "store": [0, 1, 2, 5, 6],
-        "directli": [0, 1, 4, 6],
-        "without": [0, 1, 2, 6],
-        "would": [0, 1, 5, 6],
-        "follow": [0, 1, 2, 6],
-        "abov": [0, 1, 2, 5, 6],
-        "equival": [0, 1, 6],
-        "popul": [0, 6],
-        "well": [0, 1, 2, 5, 6],
-        "newvalu": [0, 6],
-        "other": [0, 1, 2, 4, 5, 6],
-        "hand": [0, 6],
-        "lastli": [0, 6],
-        "either": [0, 1, 5, 6],
-        "token": [0, 6],
-        "no_valu": [0, 1, 5, 6],
-        "exist": [0, 1, 2, 6],
-        "modul": [0, 1, 4, 6],
-        "insid": [0, 6],
-        "myapp": [0, 5, 6],
-        "tool": [0, 1, 3, 6],
-        "foo": [0, 6],
-        "ignor": [0, 1, 6],
-        "initi": [0, 1, 2, 6],
-        "self": [0, 1, 5, 6],
-        "cl": [0, 6],
-        "suitabl": [0, 6],
-        "caveat": [0, 6],
-        "instanc": [0, 1, 2, 5, 6],
-        "myclass": [0, 6],
-        "again": [0, 2, 6],
-        "skip": [0, 6],
-        "disambigu": [0, 6],
-        "within": [0, 1, 5, 6],
-        "occur": [0, 1, 6],
-        "below": [0, 5, 6],
-        "mc": [0, 2, 6],
-        "somemethod": [0, 6],
-        "myotherclass": [0, 6],
-        "moc": [0, 6],
-        "between": [0, 6],
-        "declar": [0, 6],
-        "otherwis": [0, 1, 5, 6],
-        "prevent": [0, 1, 6],
-        "awar": [0, 5, 6],
-        "receiv": [0, 1, 6],
-        "becom": [0, 6],
-        "entir": [0, 1, 6],
-        "replac": [0, 1, 5, 6],
-        "per": [0, 1, 2, 6],
-        "basi": [0, 1, 6],
-        "sourc": [0, 1, 2, 6],
-        "parent": [0, 6],
-        "being": [0, 1, 5, 6],
-        "whenev": [0, 6],
-        "thu": [0, 1, 2, 6],
-        "determin": [0, 1, 6],
-        "dynam": [0, 1, 6],
-        "until": [0, 1, 2, 4, 5, 6],
-        "dai": [0, 6],
-        "week": [0, 6],
-        "period": [0, 2, 6],
-        "certain": [0, 6],
-        "date": [0, 1, 6],
-        "timedelta": [0, 1, 6],
-        "_config_argument_dict": [0, 6],
-        "_config_prefix": [0, 6],
-        "proxybackend": [0, 1, 5, 6],
-        "replace_existing_backend": [0, 1, 6],
-        "region_invalid": [0, 6],
-        "regioninvalidationstrategi": [0, 1, 6],
-        "cachebackend": [0, 6],
-        "resolv": [0, 6],
-        "load": [0, 1, 6],
-        "entrypoint": [0, 1, 6],
-        "number": [0, 2, 6],
-        "second": [0, 1, 2, 6],
-        "datetim": [0, 1, 6],
-        "though": [0, 1, 6],
-        "upon": [0, 1, 2, 6],
-        "after": [0, 1, 5, 6],
-        "sinc": [0, 5, 6],
-        "last": [0, 6],
-        "constructor": [0, 6],
-        "chain": [0, 1, 6],
-        "custom": [0, 1, 5, 6],
-        "augment": [0, 1, 6],
-        "chang": [0, 1, 2, 4, 5],
-        "flag": [0, 1, 6],
-        "alreadi": [0, 1, 6],
-        "7": [0, 4, 5, 6],
-        "strategi": [0, 1, 2, 6],
-        "configure_from_config": [0, 1, 6],
-        "config_dict": [0, 6],
-        "prefix": [0, 4, 6],
-        "local_region": [0, 6],
-        "memcached_region": [0, 6],
-        "readi": [0, 6],
-        "yet": [0, 1, 6],
-        "avail": [0, 1, 3, 4, 5, 6],
-        "myconfig": [0, 6],
-        "local": [0, 1, 2, 5, 6],
-        "path": [0, 2, 6],
-        "dbmfile": [0, 6],
-        "pylibmc": [0, 1, 2, 5],
-        "10": [0, 1, 6],
-        "remov": [0, 1, 2, 6],
-        "oper": [0, 1, 2, 5, 6],
-        "idempot": [0, 6],
-        "safe": [0, 2, 6],
-        "ignore_expir": [0, 1, 6],
-        "cachedvalu": [0, 1, 5, 6],
-        "novalu": [0, 6],
-        "evalu": [0, 6],
-        "separ": [0, 1, 2, 6],
-        "distinguish": [0, 6],
-        "altern": [0, 6],
-        "suppli": [0, 6],
-        "test": [0, 1, 6],
-        "against": [0, 1, 2, 6],
-        "versu": [0, 6],
-        "report": [0, 3, 6],
-        "bypass": [0, 1, 6],
-        "check": [0, 1, 2, 6],
-        "now": [0, 1, 2, 5, 6],
-        "rather": [0, 2, 6],
-        "than": [0, 2, 5, 6],
-        "uncondition": [0, 6],
-        "interpret": [0, 1, 6],
-        "term": [0, 6],
-        "older": [0, 2, 6],
-        "while": [0, 1, 4, 5, 6],
-        "down": [0, 6],
-        "process": [0, 1, 2, 5, 6],
-        "recogn": [0, 1, 6],
-        "relev": [0, 6],
-        "affect": [0, 6],
-        "regardless": [0, 6],
-        "whether": [0, 1, 6],
-        "wa": [0, 1, 2, 5, 6],
-        "match": [0, 1],
-        "three": [0, 5],
-        "zip": 0,
-        "dict": [0, 5],
-        "creator_arg": [0, 1, 6],
-        "doe": [0, 1, 5, 6],
-        "consid": [0, 1, 6],
-        "recreat": [0, 6],
-        "newli": [0, 1, 2, 6],
-        "depend": [0, 1, 6],
-        "acquir": [0, 1, 6],
-        "differ": [0, 1, 2, 5, 6],
-        "cannot": [0, 1, 6],
-        "immedi": [0, 6],
-        "timestamp": [0, 1, 6],
-        "attempt": [0, 6],
-        "wait": [0, 1, 6],
-        "kwarg": [0, 5, 6],
-        "dont_cache_non": [0, 6],
-        "some": [0, 1, 2, 4, 5, 6],
-        "create_valu": [0, 6],
-        "won": [0, 2, 6],
-        "ask": 0,
-        "approach": [0, 1, 2, 5, 6],
-        "set_multi": [0, 1, 5],
-        "modifi": 0,
-        "correct": [0, 6],
-        "submit": 0,
-        "get_value_metadata": [0, 1],
-        "enclos": 0,
-        "datastructur": 0,
-        "metadata": [0, 1, 5, 6],
-        "accessor": [0, 1],
-        "common": [0, 1, 2, 6],
-        "cached_tim": 0,
-        "ag": [0, 1],
-        "hard": [0, 1, 5, 6],
-        "minimum": [0, 1],
-        "whose": 0,
-        "prior": [0, 1],
-        "mode": [0, 1, 6],
-        "impact": 0,
-        "onc": [0, 1, 2],
-        "honor": [0, 1],
-        "both": [0, 1],
-        "soft": [0, 1],
-        "With": [0, 6],
-        "forc": [0, 1],
-        "getter": [0, 1],
-        "usag": [0, 1, 4],
-        "logic": [0, 1],
-        "push": [0, 5],
-        "back": [0, 1],
-        "regen": 0,
-        "is_configur": [0, 1],
-        "key_is_lock": [0, 1],
-        "attach": 0,
-        "defaultinvalidationstrategi": 0,
-        "propag": [0, 1],
-        "is_hard_invalid": 0,
-        "boolean": [0, 1],
-        "is_invalid": 0,
-        "is_soft_invalid": 0,
-        "was_hard_invalid": 0,
-        "was_soft_invalid": 0,
-        "interfac": [0, 2, 4, 6],
-        "custominvalidationstrategi": 0,
-        "__init__": [0, 6],
-        "_soft_invalid": 0,
-        "_hard_invalid": 0,
-        "els": [0, 2],
-        "inject": 0,
-        "noqa": 0,
-        "wish": 0,
-        "construct": [0, 1, 6],
-        "myinvalid": 0,
-        "instanti": [0, 5, 6],
-        "passthrough": 0,
-        "value_vers": 0,
-        "detect": [0, 6],
-        "backward": [0, 1],
-        "incompat": [0, 1],
-        "section": [0, 2, 6],
-        "how": [0, 2, 6],
-        "regist": [0, 1, 6],
-        "alter": [0, 6],
-        "backendformat": 0,
-        "describ": [0, 2, 6],
-        "alia": 0,
-        "union": 0,
-        "backendsettyp": 0,
-        "bytesbackend": [0, 1],
-        "defaultseri": 0,
-        "seri": [0, 1, 5],
-        "subclass": [0, 1, 6],
-        "get_seri": 0,
-        "get_serialized_multi": 0,
-        "set_seri": 0,
-        "set_serialized_multi": 0,
-        "constant": [0, 1],
-        "cutom": 0,
-        "ones": [0, 5],
-        "upstream": 0,
-        "caller": 0,
-        "must": [0, 1],
-        "do": [0, 1, 4, 5],
-        "undesir": 0,
-        "stream": 0,
-        "overridden": [0, 6],
-        "what": [0, 1, 2],
-        "individu": 0,
-        "get_mutex": 0,
-        "regular": 0,
-        "concurr": [0, 2, 6],
-        "want": [0, 2, 5, 6],
-        "variou": [0, 2],
-        "kind": [0, 6],
-        "link": [0, 5],
-        "distribut": [0, 1, 4],
-        "semaphor": 0,
-        "etc": [0, 1],
-        "best": 0,
-        "suit": [0, 1],
-        "scope": [0, 1],
-        "account": [0, 1],
-        "across": [0, 1, 2],
-        "simultan": [0, 6],
-        "just": [0, 2, 5, 6],
-        "latter": 0,
-        "variant": [0, 1, 5],
-        "involv": [0, 1],
-        "modulu": 0,
-        "throttl": 0,
-        "total": 0,
-        "ordinari": 0,
-        "abc": 0,
-        "abstract": [0, 1],
-        "succeed": 0,
-        "cachereturntyp": 0,
-        "payload": [0, 1, 5, 6],
-        "valuepayload": 0,
-        "metadatatyp": 0,
-        "namedtupl": 0,
-        "track": [0, 2, 5],
-        "inform": [0, 3, 6],
-        "elaps": 0,
-        "insert": 0,
-        "subtract": 0,
-        "epoch": 0,
-        "prefer": 0,
-        "keytyp": 0,
-        "serializedreturntyp": 0,
-        "memorybackend": [0, 1],
-        "memorypicklebackend": [0, 1],
-        "step": [0, 1, 6],
-        "former": 0,
-        "plain": [0, 1],
-        "There": [0, 2],
-        "size": [0, 5],
-        "remain": [0, 1],
-        "explicitli": 0,
-        "your": [0, 2, 5],
-        "choos": 0,
-        "cache_dict": 0,
-        "my_dictionari": 0,
-        "memory_pickl": 0,
-        "copi": [0, 1],
-        "reflect": 0,
-        "behav": 0,
-        "perform": [0, 1, 2, 5, 6],
-        "incur": 0,
-        "hit": [0, 5],
-        "somewher": 0,
-        "pure": [0, 1],
-        "remot": 0,
-        "server": [0, 2, 6],
-        "orient": 0,
-        "cpickl": 0,
-        "highest_protocol": [0, 1],
-        "talk": [0, 6],
-        "bmemcachedbackend": 0,
-        "genericmemcachedbackend": [0, 1],
-        "binari": 0,
-        "client": [0, 1, 2, 5, 6],
-        "secur": 0,
-        "sasl": 0,
-        "ssl": 0,
-        "tl": [0, 1],
-        "standard": 0,
-        "authent": [0, 1],
-        "protocol": [0, 1],
-        "independ": 0,
-        "usernam": [0, 1],
-        "password": [0, 1],
-        "bmemcach": [0, 1],
-        "3600": [0, 2, 5, 6],
-        "scott": 0,
-        "tiger": 0,
-        "tls_context": 0,
-        "ctx": 0,
-        "create_default_context": 0,
-        "cafil": 0,
-        "my": 0,
-        "ca": 0,
-        "pem": 0,
-        "advanc": 0,
-        "complex": 0,
-        "visit": 0,
-        "http": [0, 1, 3, 5],
-        "doc": [0, 1],
-        "org": [0, 3, 5],
-        "librari": [0, 1, 6],
-        "html": 0,
-        "context": [0, 2],
-        "connect": [0, 1],
-        "paramt": 0,
-        "memcachedlock": 0,
-        "coordin": [0, 2, 6],
-        "lock_timeout": [0, 1],
-        "valid": 0,
-        "memcached_expire_tim": [0, 1],
-        "expiri": 0,
-        "own": [0, 2, 4, 5],
-        "continu": [0, 1, 2],
-        "complet": [0, 2],
-        "therefor": [0, 1, 6],
-        "ll": [0, 2],
-        "sure": [0, 6],
-        "greater": 0,
-        "least": [0, 2, 5],
-        "enough": 0,
-        "dure": [0, 1, 2],
-        "genericmemachedbackend": 0,
-        "most": [0, 1, 2, 3],
-        "modern": 0,
-        "appear": [0, 1],
-        "inher": 0,
-        "threadsaf": [0, 2],
-        "In": [0, 1, 2, 5, 6],
-        "advantag": 0,
-        "over": 0,
-        "pool": 0,
-        "automat": 0,
-        "discard": 0,
-        "lib": 0,
-        "set_argu": 0,
-        "memcachedbackend": [0, 1],
-        "memcachearg": [0, 1],
-        "dead_retri": [0, 1],
-        "dead": 0,
-        "tri": 0,
-        "Will": 0,
-        "8": [0, 4, 5],
-        "move": [0, 1],
-        "erron": [0, 1],
-        "set_paramet": [0, 1],
-        "socket_timeout": [0, 1],
-        "timeout": [0, 1],
-        "everi": [0, 1, 2],
-        "client_fn": 0,
-        "pymemcachebackend": [0, 1],
-        "pymemcach": [0, 1],
-        "comprehens": 0,
-        "fast": 0,
-        "text": 0,
-        "socket": [0, 1],
-        "send": [0, 1],
-        "recv": 0,
-        "norepli": 0,
-        "significantli": 0,
-        "increas": 0,
-        "speed": 0,
-        "write": [0, 1, 6],
-        "flexibl": 0,
-        "abil": 0,
-        "treat": 0,
-        "network": 0,
-        "error": [0, 1],
-        "hashclient": [0, 1],
-        "reduc": 0,
-        "compar": [0, 6],
-        "driver": 0,
-        "user": [0, 1, 2, 4, 5, 6],
-        "document": [0, 1, 3],
-        "serd": 0,
-        "pickle_serd": 0,
-        "default_norepli": 0,
-        "enabl": [0, 1],
-        "further": 0,
-        "socket_keepal": [0, 1],
-        "keepal": [0, 1],
-        "tcp": 0,
-        "keepaliveopt": 0,
-        "enable_retry_cli": [0, 1],
-        "retri": [0, 1, 6],
-        "handl": 0,
-        "failur": [0, 1],
-        "retry_attempt": [0, 1],
-        "along": [0, 1, 2, 5],
-        "retry_delai": 0,
-        "retry_for": 0,
-        "do_not_retry_for": 0,
-        "readthedoc": 0,
-        "io": 0,
-        "en": 0,
-        "latest": 0,
-        "getting_start": 0,
-        "mani": [0, 1, 6],
-        "action": 0,
-        "wrapper": 0,
-        "int": [0, 1],
-        "sleep": 0,
-        "memcacheclienterror": 0,
-        "memcacheunexpectedcloseerror": 0,
-        "ioerror": 0,
-        "memcacheillegalinputerror": 0,
-        "hashclient_retry_attempt": [0, 1],
-        "amount": 0,
-        "mark": [0, 1],
-        "hashclient_retry_timeout": [0, 1],
-        "dead_timeout": [0, 1],
-        "add": [0, 1, 5],
-        "node": 0,
-        "pylibmcbackend": 0,
-        "illustr": [0, 2, 6],
-        "sever": [0, 1],
-        "tcp_nodelai": 0,
-        "ketama": 0,
-        "understood": 0,
-        "min_compress_len": [0, 1],
-        "redisbackend": [0, 1],
-        "py": [0, 1, 6],
-        "host": [0, 1, 3],
-        "localhost": [0, 2],
-        "port": 0,
-        "6379": 0,
-        "db": 0,
-        "redis_expiration_tim": 0,
-        "60": 0,
-        "hour": 0,
-        "thread_local_lock": [0, 1],
-        "param": 0,
-        "format": [0, 1, 4],
-        "strictredi": [0, 1],
-        "from_url": [0, 1],
-        "larger": [0, 1],
-        "socket_connect_timeout": [0, 1],
-        "socket_keepalive_opt": [0, 1],
-        "lock_sleep": [0, 1],
-        "connection_pool": [0, 1],
-        "connectionpool": [0, 1],
-        "compat": [0, 1],
-        "connection_kwarg": [0, 1],
-        "ssl_certfil": 0,
-        "charset": 0,
-        "redisclusterbackend": [0, 1],
-        "cluster": [0, 1],
-        "redisclust": 0,
-        "startup": 0,
-        "discoveri": 0,
-        "find": 0,
-        "clusternod": 0,
-        "redis_clust": 0,
-        "startup_nod": 0,
-        "6378": 0,
-        "success": [0, 1],
-        "certif": 0,
-        "admin": 0,
-        "averystrongpassword": 0,
-        "ssl_ca_cert": 0,
-        "6380": 0,
-        "6381": 0,
-        "discov": 0,
-        "whole": [0, 1],
-        "redissentinelbackend": [0, 1],
-        "sentinel": [0, 1],
-        "redis_sentinel": 0,
-        "redis_sentinel_1": 0,
-        "26379": 0,
-        "redis_sentinel_2": 0,
-        "pair": [0, 2],
-        "hostnam": 0,
-        "service_nam": 0,
-        "servic": [0, 1, 2],
-        "mymast": 0,
-        "sentinel_kwarg": 0,
-        "deal": [0, 1],
-        "filesystem": [0, 2],
-        "abstractfilelock": [0, 1],
-        "read": 0,
-        "doesn": [0, 2],
-        "necessarili": [0, 1, 6],
-        "filelock": [0, 1, 2],
-        "acquire_read_lock": 0,
-        "acquire_write_lock": 0,
-        "release_read_lock": 0,
-        "release_write_lock": 0,
-        "multithread": [0, 6],
-        "environ": [0, 1, 4],
-        "descriptor": 0,
-        "uniqu": [0, 2, 5],
-        "held": 0,
-        "code": [0, 2, 5],
-        "direct": [0, 1, 5],
-        "reader": [0, 1],
-        "notimplementederror": [0, 5],
-        "is_open": 0,
-        "writer": [0, 5, 6],
-        "dbmbackend": [0, 1],
-        "basic": [0, 6],
-        "cachefil": 0,
-        "anydbm": 0,
-        "select": [0, 4],
-        "platform": [0, 1],
-        "made": [0, 1, 2],
-        "don": [0, 1],
-        "lockfil": [0, 2],
-        "even": [0, 1],
-        "unnecessari": [0, 1],
-        "One": [0, 6],
-        "protect": 0,
-        "flock": [0, 1, 2],
-        "unix": [0, 1, 2],
-        "third": [0, 5],
-        "parti": 0,
-        "portalock": 0,
-        "drop": [0, 1],
-        "lock_factori": [0, 1],
-        "job": 0,
-        "improv": [0, 1, 5],
-        "problemat": 0,
-        "impli": [0, 2],
-        "unlimit": 0,
-        "never": 0,
-        "suffix": 0,
-        "rw_lockfil": 0,
-        "omit": [0, 1],
-        "append": [0, 5],
-        "rw": [0, 1],
-        "dogpile_lockfil": 0,
-        "readwritemutex": [0, 1],
-        "readwrite_lock": [0, 1],
-        "mutexlock": 0,
-        "ret": 0,
-        "o": [0, 1, 2],
-        "window": [0, 1],
-        "fcntl": 0,
-        "extend": [0, 5, 6],
-        "myfirstproxi": 0,
-        "goe": [0, 2],
-        "mysecondproxi": 0,
-        "stack": 0,
-        "togeth": [0, 6],
-        "concret": 0,
-        "next": [0, 2, 5],
-        "deleg": 0,
-        "toward": [0, 1],
-        "setup": [0, 1, 2, 6],
-        "nullbackend": [0, 1],
-        "dogpilecacheexcept": 0,
-        "inherit": [0, 5],
-        "pluginnotfound": [0, 1],
-        "could": [0, 1, 5],
-        "regionalreadyconfigur": 0,
-        "regionnotconfigur": 0,
-        "validationerror": 0,
-        "beaker": [0, 2],
-        "templat": [0, 1, 5],
-        "lookup": [0, 2],
-        "templatelookup": 0,
-        "360": 0,
-        "mako_lookup": 0,
-        "directori": [0, 1],
-        "cache_impl": 0,
-        "cache_arg": 0,
-        "tag": 0,
-        "desir": 0,
-        "cache_region": 0,
-        "mysect": 0,
-        "content": 0,
-        "mako_cach": [0, 1],
-        "makoplugin": 0,
-        "cacheimpl": 0,
-        "creation_funct": 0,
-        "we": [0, 2, 5, 6],
-        "build": [0, 1, 2, 4, 5],
-        "argnam": 0,
-        "argvalu": 0,
-        "argspec": 0,
-        "alphabet": 0,
-        "length_conditional_mangl": 0,
-        "past": 0,
-        "threshold": 0,
-        "value_and_created_fn": 0,
-        "expiretim": 0,
-        "around": [0, 2],
-        "arbitrari": 0,
-        "elect": 0,
-        "new_valu": 0,
-        "creation_tim": 0,
-        "state": [0, 1],
-        "existing_valu": 0,
-        "assum": [0, 1],
-        "needregenerationexcept": [0, 2],
-        "thrown": [0, 1],
-        "intent": 0,
-        "invoc": [0, 2],
-        "has_valu": 0,
-        "condit": [0, 1],
-        "packag": [0, 1, 2, 3],
-        "contain": [0, 5, 6],
-        "concept": [0, 2, 4],
-        "synchron": [0, 2],
-        "nameregistri": [0, 1],
-        "keep": [0, 2],
-        "singleton": 0,
-        "identifi": [0, 1, 6],
-        "strongli": 0,
-        "referenc": 0,
-        "myfoo": 0,
-        "registri": [0, 5],
-        "my_foo": 0,
-        "foo1": 0,
-        "refer": [0, 1, 2, 4],
-        "garbag": 0,
-        "collect": 0,
-        "possibli": 0,
-        "wed": 1,
-        "feb": 1,
-        "21": 1,
-        "2024": 1,
-        "redi": [1, 4, 6],
-        "backend": [1, 2, 4, 5],
-        "courtesi": 1,
-        "ma\u00ebl": 1,
-        "naccach": 1,
-        "t\u00fcfek\u00e7i": 1,
-        "250": 1,
-        "takashi": 1,
-        "kajinami": 1,
-        "252": 1,
-        "These": [1, 6],
-        "rbac": 1,
-        "dec": 1,
-        "20": 1,
-        "2023": 1,
-        "region": [1, 4, 5],
-        "gr\u00e9goir": 1,
-        "deveaux": 1,
-        "37": 1,
-        "eol": 1,
-        "project": [1, 4],
-        "pep": 1,
-        "621": 1,
-        "pyproject": 1,
-        "toml": 1,
-        "sat": 1,
-        "jul": 1,
-        "673": 1,
-        "viico": 1,
-        "240": 1,
-        "file": [1, 4, 6],
-        "root": 1,
-        "mypi": 1,
-        "dogpil": [1, 3, 5, 6],
-        "daverbal": 1,
-        "238": 1,
-        "apr": 1,
-        "26": 1,
-        "api": [1, 4, 5, 6],
-        "defin": [1, 5, 6],
-        "simon": 1,
-        "hewitt": 1,
-        "236": 1,
-        "fri": 1,
-        "2022": 1,
-        "memcach": [1, 2, 6],
-        "223": 1,
-        "228": 1,
-        "tue": 1,
-        "jun": 1,
-        "221": 1,
-        "regress": 1,
-        "caus": 1,
-        "220": 1,
-        "jan": 1,
-        "19": 1,
-        "retry_timeout": 1,
-        "sep": 1,
-        "2021": 1,
-        "deprec": 1,
-        "warn": 1,
-        "karthikeyan": 1,
-        "singaravelan": 1,
-        "203": 1,
-        "repair": 1,
-        "__signature__": 1,
-        "202": 1,
-        "subject": 1,
-        "bastien": 1,
-        "gerard": 1,
-        "101": 1,
-        "mois\u00e9": 1,
-        "guimar\u00e3": 1,
-        "de": 1,
-        "medeiro": 1,
-        "134": 1,
-        "mon": 1,
-        "nov": 1,
-        "23": 1,
-        "2020": 1,
-        "inadvert": 1,
-        "turn": [1, 6],
-        "unexpect": 1,
-        "pypi": [1, 3],
-        "195": 1,
-        "sun": 1,
-        "15": 1,
-        "rework": 1,
-        "simplifi": 1,
-        "easier": [1, 6],
-        "maintain": 1,
-        "addition": [1, 4],
-        "portion": [1, 6],
-        "overal": 1,
-        "scheme": [1, 2, 5],
-        "hardwir": 1,
-        "themselv": 1,
-        "issu": [1, 2, 3, 6],
-        "forego": 1,
-        "come": 1,
-        "out": [1, 5],
-        "alessio": 1,
-        "bogon": 1,
-        "191": 1,
-        "484": 1,
-        "annot": 1,
-        "aug": 1,
-        "173": 1,
-        "instal": [1, 4, 6],
-        "cfg": 1,
-        "wheel": 1,
-        "micha\u0142": 1,
-        "g\u00f3rny": 1,
-        "due": 1,
-        "184": 1,
-        "univers": 1,
-        "py2": 1,
-        "py3": 1,
-        "185": 1,
-        "plugin": [1, 4, 6],
-        "scanner": 1,
-        "switch": 1,
-        "pkg_resourc": 1,
-        "stevedor": 1,
-        "st\u00e9phane": 1,
-        "brunner": 1,
-        "181": 1,
-        "py3k": 1,
-        "ensur": [1, 2],
-        "presenc": 1,
-        "pip": [1, 3],
-        "517": 1,
-        "As": 1,
-        "distro": 1,
-        "problem": 1,
-        "avoid": [1, 5],
-        "178": 1,
-        "29": 1,
-        "tox": 1,
-        "ini": 1,
-        "pre": [1, 5],
-        "known": 1,
-        "interfer": 1,
-        "async": 1,
-        "conserv": 1,
-        "emit": [1, 6],
-        "break": 1,
-        "171": 1,
-        "oct": 1,
-        "28": 1,
-        "2019": 1,
-        "log": [1, 4],
-        "facilil": 1,
-        "event": [1, 4, 6],
-        "veri": [1, 4],
-        "high": [1, 4, 6],
-        "volum": [1, 4],
-        "messag": [1, 6],
-        "debug": [1, 6],
-        "favor": 1,
-        "straight": 1,
-        "pypa": 1,
-        "pytest": 1,
-        "develop": 1,
-        "command": 1,
-        "head": 1,
-        "script": 1,
-        "github": [1, 3],
-        "com": [1, 3],
-        "setuptool": [1, 6],
-        "1684": 1,
-        "dev": 1,
-        "5534": 1,
-        "157": 1,
-        "compatbl": 1,
-        "routin": 1,
-        "getfullargspec": 1,
-        "fulli": 1,
-        "vendor": 1,
-        "alpha": 1,
-        "revert": 1,
-        "observ": 1,
-        "magnitud": 1,
-        "slower": 1,
-        "rewritten": 1,
-        "plan": 1,
-        "situat": 1,
-        "sqlalchemi": [1, 3, 5],
-        "154": 1,
-        "pin": 1,
-        "juli": 1,
-        "2015": 1,
-        "160": 1,
-        "159": 1,
-        "11": 1,
-        "2018": 1,
-        "136": 1,
-        "expand": 1,
-        "implicitli": 1,
-        "exact": 1,
-        "restor": 1,
-        "139": 1,
-        "preserv": [1, 5],
-        "ankitpatel96": 1,
-        "small": [1, 6],
-        "enhanc": [1, 3],
-        "137": 1,
-        "inspect": 1,
-        "getargspec": 1,
-        "129": 1,
-        "24": 1,
-        "organ": 1,
-        "field": 1,
-        "had": 1,
-        "ben": 1,
-        "usual": [1, 2, 6],
-        "typeerror": 1,
-        "less": 1,
-        "frequent": 1,
-        "lead": [1, 5],
-        "excess": 1,
-        "pluggabl": 1,
-        "38": 1,
-        "128": 1,
-        "27": 1,
-        "calcul": 1,
-        "123": 1,
-        "unnecessarili": 1,
-        "122": 1,
-        "mar": 1,
-        "variabl": 1,
-        "syntax": 1,
-        "brian": 1,
-        "sheldon": 1,
-        "119": 1,
-        "2017": 1,
-        "empti": 1,
-        "tobia": 1,
-        "sauerwein": 1,
-        "__repr__": 1,
-        "output": [1, 2],
-        "scenario": 1,
-        "up": 1,
-        "paul": 1,
-        "brown": 1,
-        "except": [1, 4, 5, 6],
-        "locat": [1, 6],
-        "previous": [1, 2],
-        "jami": 1,
-        "lennox": 1,
-        "18": 1,
-        "daniel": 1,
-        "krau": 1,
-        "16": 1,
-        "2016": 1,
-        "potenti": [1, 5, 6],
-        "special": 1,
-        "customiz": 1,
-        "contribut": 1,
-        "recip": [1, 2, 4],
-        "alexand": 1,
-        "makarov": 1,
-        "posit": 1,
-        "43": 1,
-        "util": [1, 4],
-        "symbol": [1, 2],
-        "reli": [1, 2],
-        "although": 1,
-        "intend": 1,
-        "face": 1,
-        "coerce_string_conf": 1,
-        "keyreentrantmutex": 1,
-        "memoized_properti": 1,
-        "pluginload": 1,
-        "to_list": 1,
-        "core": [1, 4, 6],
-        "99": 1,
-        "roll": 1,
-        "unaffect": 1,
-        "retir": 1,
-        "syncreaderdogpil": 1,
-        "91": 1,
-        "pop": [1, 6],
-        "lose": 1,
-        "null": 1,
-        "nulllock": 1,
-        "did": [1, 6],
-        "nor": 1,
-        "97": 1,
-        "commun": 1,
-        "frit": 1,
-        "stegmann": 1,
-        "morgan": 1,
-        "fainberg": 1,
-        "54": 1,
-        "hbccbh": 1,
-        "65": 1,
-        "35": 1,
-        "john": 1,
-        "anderson": 1,
-        "33": 1,
-        "zero": 1,
-        "74": 1,
-        "memorypickl": 1,
-        "anentrop": 1,
-        "30": 1,
-        "serv": 1,
-        "wide": 1,
-        "respect": 1,
-        "product": [1, 6],
-        "hongbin": 1,
-        "lu": 1,
-        "71": 1,
-        "25": 1,
-        "jonathan": 1,
-        "vanasco": 1,
-        "41": 1,
-        "is_unittest": 1,
-        "14": 1,
-        "2014": 1,
-        "purpos": [1, 2, 5],
-        "wichert": 1,
-        "akkerman": 1,
-        "masayuko": 1,
-        "17": 1,
-        "sauliu": 1,
-        "menkevi\u010diu": 1,
-        "mako": 1,
-        "58": 1,
-        "entri": 1,
-        "wrong": 1,
-        "v": [1, 5],
-        "beyond": 1,
-        "zoomorph": 1,
-        "pars": 1,
-        "conf": 1,
-        "deliv": 1,
-        "pullreq": 1,
-        "jeff": 1,
-        "dairiki": 1,
-        "57": 1,
-        "13": 1,
-        "complement": 1,
-        "eric": 1,
-        "hanchrow": 1,
-        "55": 1,
-        "emploi": 1,
-        "guard": 1,
-        "memori": [1, 5],
-        "51": 1,
-        "instead": [1, 2, 5],
-        "suppos": [1, 5],
-        "expos": 1,
-        "storag": [1, 5, 6],
-        "ryan": 1,
-        "kolak": 1,
-        "wasn": 1,
-        "correctli": 1,
-        "destruct": 1,
-        "2013": 1,
-        "44": 1,
-        "unit": 1,
-        "adjust": [1, 4],
-        "unsupport": 1,
-        "total_second": 1,
-        "unconfigur": 1,
-        "40": 1,
-        "\u0142ukasz": 1,
-        "fidosz": 1,
-        "errant": 1,
-        "u": [1, 2, 6],
-        "python3": 1,
-        "jimmei": 1,
-        "mabei": 1,
-        "39": 1,
-        "neg": 1,
-        "sign": 1,
-        "david": 1,
-        "beitei": 1,
-        "semant": 1,
-        "36": 1,
-        "jack": 1,
-        "lutz": 1,
-        "thank": 1,
-        "tim": 1,
-        "hanu": 1,
-        "great": 1,
-        "effort": 1,
-        "full": 1,
-        "multivalu": 1,
-        "marco": 1,
-        "araujo": 1,
-        "sobrinho": 1,
-        "lx": 1,
-        "yu": 1,
-        "patch": 1,
-        "repositori": 1,
-        "git": 1,
-        "plu": 1,
-        "cache_timeout": 1,
-        "subsitut": 1,
-        "ralph": 1,
-        "bean": 1,
-        "2012": 1,
-        "antoin": 1,
-        "bertin": 1,
-        "info": 1,
-        "jon": 1,
-        "rosebaugh": 1,
-        "fallback": 1,
-        "keyerror": 1,
-        "gdbm": 1,
-        "wherebi": 1,
-        "therebi": 1,
-        "deadlock": 1,
-        "app": 1,
-        "appar": 1,
-        "12": 1,
-        "critic": 1,
-        "pileup": 1,
-        "relianc": 1,
-        "share": [1, 2, 6],
-        "__future__": 1,
-        "with_stat": 1,
-        "cover": 1,
-        "hayden": 1,
-        "yank": 1,
-        "didn": 1,
-        "no_tag": 1,
-        "fedorov": 1,
-        "justin": 1,
-        "azoff": 1,
-        "coercion": 1,
-        "reentrant": 1,
-        "glitch": 1,
-        "ef206ed4473fec3b639": 1,
-        "olli": 1,
-        "rutherfurd": 1,
-        "2to3": 1,
-        "thing": [1, 6],
-        "christian": 1,
-        "klinger": 1,
-        "08": 1,
-        "encapsul": 2,
-        "primari": 2,
-        "anticip": 2,
-        "indirectli": 2,
-        "fall": 2,
-        "categori": 2,
-        "short": 2,
-        "answer": 2,
-        "resourc": [2, 4],
-        "the_resourc": 2,
-        "some_creation_funct": 2,
-        "create_some_resourc": 2,
-        "creationtim": 2,
-        "tup": 2,
-        "retrieve_resourc": 2,
-        "do_someth": 2,
-        "minu": 2,
-        "through": [2, 5],
-        "design": [2, 6],
-        "address": 2,
-        "disappear": 2,
-        "our": [2, 5, 6],
-        "alert": 2,
-        "ahead": 2,
-        "round": 2,
-        "trip": 2,
-        "expect": 2,
-        "effici": 2,
-        "approxim": 2,
-        "mc_pool": 2,
-        "threadmappedpool": 2,
-        "get_valu": 2,
-        "reserv": 2,
-        "value_plus_tim": 2,
-        "createdtim": 2,
-        "gen_cach": 2,
-        "put": [2, 6],
-        "generate_my_expensive_valu": 2,
-        "slow_databas": 2,
-        "stuff": 2,
-        "twice": 2,
-        "global": 2,
-        "cross": 2,
-        "accomplish": 2,
-        "far": 2,
-        "symlink": 2,
-        "off": 2,
-        "nf": 2,
-        "flufl": 2,
-        "act": 2,
-        "hashlib": 2,
-        "lock_path": 2,
-        "tmp": 2,
-        "hexdigest": 2,
-        "hoc": [2, 6],
-        "some_kei": 2,
-        "hex": 2,
-        "digest": 2,
-        "53def077a4264bd3183d4eb21b1f56f883e1b572": 2,
-        "baton": 2,
-        "often": 2,
-        "good": [2, 5],
-        "idea": [2, 5],
-        "about": 3,
-        "statu": 3,
-        "recent": 3,
-        "publish": 3,
-        "dogpilecach": 3,
-        "index": [3, 4],
-        "tracker": 3,
-        "consist": [4, 6],
-        "subsystem": 4,
-        "top": 4,
-        "control": 4,
-        "execut": 4,
-        "varieti": 4,
-        "hook": [4, 5],
-        "integr": 4,
-        "easi": 4,
-        "encourag": 4,
-        "adapt": 4,
-        "lot": 4,
-        "tweak": 4,
-        "matter": 4,
-        "homepag": 4,
-        "bug": 4,
-        "guid": 4,
-        "overview": 4,
-        "rudimentari": 4,
-        "group": 4,
-        "relat": 4,
-        "orm": 4,
-        "encod": 4,
-        "decod": 4,
-        "learn": 4,
-        "changelog": 4,
-        "9": [4, 6],
-        "search": 4,
-        "page": 4,
-        "id": 5,
-        "user_fn_on": 5,
-        "user_fn_two": 5,
-        "user_fn_thre": 5,
-        "user_id": [5, 6],
-        "user_fn_one_": 5,
-        "user_fn_two_": 5,
-        "user_fn_three_": 5,
-        "invalidate_user_id": 5,
-        "know": 5,
-        "everyth": 5,
-        "itertool": 5,
-        "count": 5,
-        "user_kei": 5,
-        "fname_": 5,
-        "d_arg1_arg2_arg3": 5,
-        "key_templ": 5,
-        "counter": 5,
-        "print": 5,
-        "techniqu": 5,
-        "optimist": 5,
-        "sent": 5,
-        "databas": 5,
-        "get_some_data": 5,
-        "session": 5,
-        "dbclass": 5,
-        "filter": 5,
-        "moment": 5,
-        "delai": 5,
-        "offload": 5,
-        "acheiv": 5,
-        "expedi": 5,
-        "smaller": 5,
-        "commit": 5,
-        "cache_refresh": 5,
-        "assert": 5,
-        "isinst": 5,
-        "sessionmak": 5,
-        "scoped_sess": 5,
-        "listens_for": 5,
-        "after_commit": 5,
-        "do_refresh": 5,
-        "daemon": 5,
-        "add_new_data": 5,
-        "something_new": 5,
-        "besid": 5,
-        "collis": 5,
-        "easili": [5, 6],
-        "done": 5,
-        "lambda": 5,
-        "hood": 5,
-        "bookkeep": 5,
-        "transform": 5,
-        "happen": 5,
-        "raw": 5,
-        "negat": 5,
-        "hope": 5,
-        "concern": 5,
-        "minim": 5,
-        "recod": 5,
-        "fly": 5,
-        "enter": 5,
-        "leav": 5,
-        "msgpack": 5,
-        "exception": 5,
-        "nest": 5,
-        "much": 5,
-        "_encodedproxi": 5,
-        "main": 5,
-        "msgpackproxi": 5,
-        "simpli": 5,
-        "necessari": 5,
-        "value_decod": 5,
-        "value_encod": 5,
-        "proxi": [5, 6],
-        "me": 5,
-        "unencod": 5,
-        "mapping_set": 5,
-        "iteritem": 5,
-        "translat": 5,
-        "record": 5,
-        "probabl": 5,
-        "object_hook": 5,
-        "unpackb": 5,
-        "utf": 5,
-        "packb": 5,
-        "use_bin_typ": 5,
-        "At": 6,
-        "popular": 6,
-        "focus": 6,
-        "model": 6,
-        "particularli": 6,
-        "foremost": 6,
-        "mind": 6,
-        "compon": 6,
-        "behind": 6,
-        "scene": 6,
-        "circumst": 6,
-        "offer": 6,
-        "instruct": 6,
-        "pattern": 6,
-        "among": 6,
-        "elimin": 6,
-        "redundantli": 6,
-        "worker": 6,
-        "look": 6,
-        "load_user_info": 6,
-        "some_databas": 6,
-        "lookup_user_by_id": 6,
-        "excel": 6,
-        "written": 6,
-        "nativ": 6,
-        "markedli": 6,
-        "faster": 6,
-        "rougher": 6,
-        "edg": 6,
-        "bit": 6,
-        "verbos": 6,
-        "runtim": 6,
-        "henc": 6,
-        "life": 6,
-        "helper": 6,
-        "sy": 6,
-        "dictionarybackend": 6,
-        "Then": 6,
-        "entry_point": 6,
-        "mypackag": 6,
-        "mybackend": 6,
-        "space": 6,
-        "bother": 6,
-        "anyth": 6,
-        "register_backend": 6,
-        "usabl": 6,
-        "myregion": 6,
-        "somevalu": 6,
-        "serializ": 6,
-        "adventag": 6,
-        "real": 6,
-        "getlogg": 6,
-        "loggingproxi": 6,
-        "properli": 6,
-        "super": 6,
-        "retrydeleteproxi": 6,
-        "retry_count": 6,
-        "uninstanti": 6,
-        "retry_proxi": 6,
-        "instant": 6,
-        "behalf": 6,
-        "facil": 6,
-        "basicconfig": 6,
-        "setlevel": 6,
-        "spent": 6,
-        "No": 6,
-        "__main__": 6,
-        "501": 6
+    "indexentries": {
+        "abstractfilelock (class in dogpile.cache.backends.file)": [
+            [0, "dogpile.cache.backends.file.AbstractFileLock", false]
+        ],
+        "acquire() (dogpile.cache.api.cachemutex method)": [
+            [0, "dogpile.cache.api.CacheMutex.acquire", false]
+        ],
+        "acquire() (dogpile.cache.backends.file.abstractfilelock method)": [
+            [0, "dogpile.cache.backends.file.AbstractFileLock.acquire", false]
+        ],
+        "acquire_read_lock() (dogpile.cache.backends.file.abstractfilelock method)": [
+            [0, "dogpile.cache.backends.file.AbstractFileLock.acquire_read_lock", false]
+        ],
+        "acquire_read_lock() (dogpile.cache.backends.file.filelock method)": [
+            [0, "dogpile.cache.backends.file.FileLock.acquire_read_lock", false]
+        ],
+        "acquire_read_lock() (dogpile.util.readwritemutex method)": [
+            [0, "dogpile.util.ReadWriteMutex.acquire_read_lock", false]
+        ],
+        "acquire_write_lock() (dogpile.cache.backends.file.abstractfilelock method)": [
+            [0, "dogpile.cache.backends.file.AbstractFileLock.acquire_write_lock", false]
+        ],
+        "acquire_write_lock() (dogpile.cache.backends.file.filelock method)": [
+            [0, "dogpile.cache.backends.file.FileLock.acquire_write_lock", false]
+        ],
+        "acquire_write_lock() (dogpile.util.readwritemutex method)": [
+            [0, "dogpile.util.ReadWriteMutex.acquire_write_lock", false]
+        ],
+        "actual_backend (dogpile.cache.region.cacheregion property)": [
+            [0, "dogpile.cache.region.CacheRegion.actual_backend", false]
+        ],
+        "age (dogpile.cache.api.cachedvalue property)": [
+            [0, "dogpile.cache.api.CachedValue.age", false]
+        ],
+        "backendformatted (in module dogpile.cache.api)": [
+            [0, "dogpile.cache.api.BackendFormatted", false]
+        ],
+        "backendsettype (in module dogpile.cache.api)": [
+            [0, "dogpile.cache.api.BackendSetType", false]
+        ],
+        "bmemcachedbackend (class in dogpile.cache.backends.memcached)": [
+            [0, "dogpile.cache.backends.memcached.BMemcachedBackend", false]
+        ],
+        "bytesbackend (class in dogpile.cache.api)": [
+            [0, "dogpile.cache.api.BytesBackend", false]
+        ],
+        "cache_multi_on_arguments() (dogpile.cache.region.cacheregion method)": [
+            [0, "dogpile.cache.region.CacheRegion.cache_multi_on_arguments", false]
+        ],
+        "cache_on_arguments() (dogpile.cache.region.cacheregion method)": [
+            [0, "dogpile.cache.region.CacheRegion.cache_on_arguments", false]
+        ],
+        "cachebackend (class in dogpile.cache.api)": [
+            [0, "dogpile.cache.api.CacheBackend", false]
+        ],
+        "cached_time (dogpile.cache.api.cachedvalue property)": [
+            [0, "dogpile.cache.api.CachedValue.cached_time", false]
+        ],
+        "cachedvalue (class in dogpile.cache.api)": [
+            [0, "dogpile.cache.api.CachedValue", false]
+        ],
+        "cachemutex (class in dogpile.cache.api)": [
+            [0, "dogpile.cache.api.CacheMutex", false]
+        ],
+        "cacheregion (class in dogpile.cache.region)": [
+            [0, "dogpile.cache.region.CacheRegion", false]
+        ],
+        "cachereturntype (in module dogpile.cache.api)": [
+            [0, "dogpile.cache.api.CacheReturnType", false]
+        ],
+        "cantdeserializeexception": [
+            [0, "dogpile.cache.api.CantDeserializeException", false]
+        ],
+        "client (dogpile.cache.backends.memcached.genericmemcachedbackend property)": [
+            [0, "dogpile.cache.backends.memcached.GenericMemcachedBackend.client", false]
+        ],
+        "configure() (dogpile.cache.region.cacheregion method)": [
+            [0, "dogpile.cache.region.CacheRegion.configure", false]
+        ],
+        "configure_from_config() (dogpile.cache.region.cacheregion method)": [
+            [0, "dogpile.cache.region.CacheRegion.configure_from_config", false]
+        ],
+        "dbmbackend (class in dogpile.cache.backends.file)": [
+            [0, "dogpile.cache.backends.file.DBMBackend", false]
+        ],
+        "defaultinvalidationstrategy (class in dogpile.cache.region)": [
+            [0, "dogpile.cache.region.DefaultInvalidationStrategy", false]
+        ],
+        "delete() (dogpile.cache.api.cachebackend method)": [
+            [0, "dogpile.cache.api.CacheBackend.delete", false]
+        ],
+        "delete() (dogpile.cache.backends.file.dbmbackend method)": [
+            [0, "dogpile.cache.backends.file.DBMBackend.delete", false]
+        ],
+        "delete() (dogpile.cache.backends.memcached.genericmemcachedbackend method)": [
+            [0, "dogpile.cache.backends.memcached.GenericMemcachedBackend.delete", false]
+        ],
+        "delete() (dogpile.cache.backends.memory.memorybackend method)": [
+            [0, "dogpile.cache.backends.memory.MemoryBackend.delete", false]
+        ],
+        "delete() (dogpile.cache.backends.null.nullbackend method)": [
+            [0, "dogpile.cache.backends.null.NullBackend.delete", false]
+        ],
+        "delete() (dogpile.cache.backends.redis.redisbackend method)": [
+            [0, "dogpile.cache.backends.redis.RedisBackend.delete", false]
+        ],
+        "delete() (dogpile.cache.proxy.proxybackend method)": [
+            [0, "dogpile.cache.proxy.ProxyBackend.delete", false]
+        ],
+        "delete() (dogpile.cache.region.cacheregion method)": [
+            [0, "dogpile.cache.region.CacheRegion.delete", false]
+        ],
+        "delete_multi() (dogpile.cache.api.cachebackend method)": [
+            [0, "dogpile.cache.api.CacheBackend.delete_multi", false]
+        ],
+        "delete_multi() (dogpile.cache.backends.file.dbmbackend method)": [
+            [0, "dogpile.cache.backends.file.DBMBackend.delete_multi", false]
+        ],
+        "delete_multi() (dogpile.cache.backends.memcached.bmemcachedbackend method)": [
+            [0, "dogpile.cache.backends.memcached.BMemcachedBackend.delete_multi", false]
+        ],
+        "delete_multi() (dogpile.cache.backends.memcached.genericmemcachedbackend method)": [
+            [0, "dogpile.cache.backends.memcached.GenericMemcachedBackend.delete_multi", false]
+        ],
+        "delete_multi() (dogpile.cache.backends.memory.memorybackend method)": [
+            [0, "dogpile.cache.backends.memory.MemoryBackend.delete_multi", false]
+        ],
+        "delete_multi() (dogpile.cache.backends.null.nullbackend method)": [
+            [0, "dogpile.cache.backends.null.NullBackend.delete_multi", false]
+        ],
+        "delete_multi() (dogpile.cache.backends.redis.redisbackend method)": [
+            [0, "dogpile.cache.backends.redis.RedisBackend.delete_multi", false]
+        ],
+        "delete_multi() (dogpile.cache.proxy.proxybackend method)": [
+            [0, "dogpile.cache.proxy.ProxyBackend.delete_multi", false]
+        ],
+        "delete_multi() (dogpile.cache.region.cacheregion method)": [
+            [0, "dogpile.cache.region.CacheRegion.delete_multi", false]
+        ],
+        "deserializer (dogpile.cache.api.cachebackend attribute)": [
+            [0, "dogpile.cache.api.CacheBackend.deserializer", false]
+        ],
+        "deserializer (dogpile.cache.backends.memcached.genericmemcachedbackend attribute)": [
+            [0, "dogpile.cache.backends.memcached.GenericMemcachedBackend.deserializer", false]
+        ],
+        "dogpile.cache.api": [
+            [0, "module-dogpile.cache.api", false]
+        ],
+        "dogpile.cache.backends.file": [
+            [0, "module-dogpile.cache.backends.file", false]
+        ],
+        "dogpile.cache.backends.memcached": [
+            [0, "module-dogpile.cache.backends.memcached", false]
+        ],
+        "dogpile.cache.backends.memory": [
+            [0, "module-dogpile.cache.backends.memory", false]
+        ],
+        "dogpile.cache.backends.null": [
+            [0, "module-dogpile.cache.backends.null", false]
+        ],
+        "dogpile.cache.backends.redis": [
+            [0, "module-dogpile.cache.backends.redis", false]
+        ],
+        "dogpile.cache.exception": [
+            [0, "module-dogpile.cache.exception", false]
+        ],
+        "dogpile.cache.plugins.mako_cache": [
+            [0, "module-dogpile.cache.plugins.mako_cache", false]
+        ],
+        "dogpile.cache.proxy": [
+            [0, "module-dogpile.cache.proxy", false]
+        ],
+        "dogpile.cache.region": [
+            [0, "module-dogpile.cache.region", false]
+        ],
+        "dogpilecacheexception": [
+            [0, "dogpile.cache.exception.DogpileCacheException", false]
+        ],
+        "filelock (class in dogpile.cache.backends.file)": [
+            [0, "dogpile.cache.backends.file.FileLock", false]
+        ],
+        "function_key_generator() (in module dogpile.cache.util)": [
+            [0, "dogpile.cache.util.function_key_generator", false]
+        ],
+        "genericmemcachedbackend (class in dogpile.cache.backends.memcached)": [
+            [0, "dogpile.cache.backends.memcached.GenericMemcachedBackend", false]
+        ],
+        "get() (dogpile.cache.api.cachebackend method)": [
+            [0, "dogpile.cache.api.CacheBackend.get", false]
+        ],
+        "get() (dogpile.cache.backends.memcached.genericmemcachedbackend method)": [
+            [0, "dogpile.cache.backends.memcached.GenericMemcachedBackend.get", false]
+        ],
+        "get() (dogpile.cache.backends.memory.memorybackend method)": [
+            [0, "dogpile.cache.backends.memory.MemoryBackend.get", false]
+        ],
+        "get() (dogpile.cache.backends.null.nullbackend method)": [
+            [0, "dogpile.cache.backends.null.NullBackend.get", false]
+        ],
+        "get() (dogpile.cache.plugins.mako_cache.makoplugin method)": [
+            [0, "dogpile.cache.plugins.mako_cache.MakoPlugin.get", false]
+        ],
+        "get() (dogpile.cache.proxy.proxybackend method)": [
+            [0, "dogpile.cache.proxy.ProxyBackend.get", false]
+        ],
+        "get() (dogpile.cache.region.cacheregion method)": [
+            [0, "dogpile.cache.region.CacheRegion.get", false]
+        ],
+        "get() (dogpile.util.nameregistry method)": [
+            [0, "dogpile.util.NameRegistry.get", false]
+        ],
+        "get_multi() (dogpile.cache.api.cachebackend method)": [
+            [0, "dogpile.cache.api.CacheBackend.get_multi", false]
+        ],
+        "get_multi() (dogpile.cache.backends.memcached.genericmemcachedbackend method)": [
+            [0, "dogpile.cache.backends.memcached.GenericMemcachedBackend.get_multi", false]
+        ],
+        "get_multi() (dogpile.cache.backends.memory.memorybackend method)": [
+            [0, "dogpile.cache.backends.memory.MemoryBackend.get_multi", false]
+        ],
+        "get_multi() (dogpile.cache.backends.null.nullbackend method)": [
+            [0, "dogpile.cache.backends.null.NullBackend.get_multi", false]
+        ],
+        "get_multi() (dogpile.cache.proxy.proxybackend method)": [
+            [0, "dogpile.cache.proxy.ProxyBackend.get_multi", false]
+        ],
+        "get_multi() (dogpile.cache.region.cacheregion method)": [
+            [0, "dogpile.cache.region.CacheRegion.get_multi", false]
+        ],
+        "get_mutex() (dogpile.cache.api.cachebackend method)": [
+            [0, "dogpile.cache.api.CacheBackend.get_mutex", false]
+        ],
+        "get_mutex() (dogpile.cache.backends.file.dbmbackend method)": [
+            [0, "dogpile.cache.backends.file.DBMBackend.get_mutex", false]
+        ],
+        "get_mutex() (dogpile.cache.backends.memcached.genericmemcachedbackend method)": [
+            [0, "dogpile.cache.backends.memcached.GenericMemcachedBackend.get_mutex", false]
+        ],
+        "get_mutex() (dogpile.cache.backends.null.nullbackend method)": [
+            [0, "dogpile.cache.backends.null.NullBackend.get_mutex", false]
+        ],
+        "get_mutex() (dogpile.cache.backends.redis.redisbackend method)": [
+            [0, "dogpile.cache.backends.redis.RedisBackend.get_mutex", false]
+        ],
+        "get_mutex() (dogpile.cache.proxy.proxybackend method)": [
+            [0, "dogpile.cache.proxy.ProxyBackend.get_mutex", false]
+        ],
+        "get_or_create() (dogpile.cache.plugins.mako_cache.makoplugin method)": [
+            [0, "dogpile.cache.plugins.mako_cache.MakoPlugin.get_or_create", false]
+        ],
+        "get_or_create() (dogpile.cache.region.cacheregion method)": [
+            [0, "dogpile.cache.region.CacheRegion.get_or_create", false]
+        ],
+        "get_or_create_multi() (dogpile.cache.region.cacheregion method)": [
+            [0, "dogpile.cache.region.CacheRegion.get_or_create_multi", false]
+        ],
+        "get_serialized() (dogpile.cache.api.bytesbackend method)": [
+            [0, "dogpile.cache.api.BytesBackend.get_serialized", false]
+        ],
+        "get_serialized() (dogpile.cache.api.cachebackend method)": [
+            [0, "dogpile.cache.api.CacheBackend.get_serialized", false]
+        ],
+        "get_serialized() (dogpile.cache.backends.file.dbmbackend method)": [
+            [0, "dogpile.cache.backends.file.DBMBackend.get_serialized", false]
+        ],
+        "get_serialized() (dogpile.cache.backends.redis.redisbackend method)": [
+            [0, "dogpile.cache.backends.redis.RedisBackend.get_serialized", false]
+        ],
+        "get_serialized() (dogpile.cache.proxy.proxybackend method)": [
+            [0, "dogpile.cache.proxy.ProxyBackend.get_serialized", false]
+        ],
+        "get_serialized_multi() (dogpile.cache.api.bytesbackend method)": [
+            [0, "dogpile.cache.api.BytesBackend.get_serialized_multi", false]
+        ],
+        "get_serialized_multi() (dogpile.cache.api.cachebackend method)": [
+            [0, "dogpile.cache.api.CacheBackend.get_serialized_multi", false]
+        ],
+        "get_serialized_multi() (dogpile.cache.backends.file.dbmbackend method)": [
+            [0, "dogpile.cache.backends.file.DBMBackend.get_serialized_multi", false]
+        ],
+        "get_serialized_multi() (dogpile.cache.backends.redis.redisbackend method)": [
+            [0, "dogpile.cache.backends.redis.RedisBackend.get_serialized_multi", false]
+        ],
+        "get_serialized_multi() (dogpile.cache.proxy.proxybackend method)": [
+            [0, "dogpile.cache.proxy.ProxyBackend.get_serialized_multi", false]
+        ],
+        "get_value_metadata() (dogpile.cache.region.cacheregion method)": [
+            [0, "dogpile.cache.region.CacheRegion.get_value_metadata", false]
+        ],
+        "invalidate() (dogpile.cache.plugins.mako_cache.makoplugin method)": [
+            [0, "dogpile.cache.plugins.mako_cache.MakoPlugin.invalidate", false]
+        ],
+        "invalidate() (dogpile.cache.region.cacheregion method)": [
+            [0, "dogpile.cache.region.CacheRegion.invalidate", false]
+        ],
+        "invalidate() (dogpile.cache.region.defaultinvalidationstrategy method)": [
+            [0, "dogpile.cache.region.DefaultInvalidationStrategy.invalidate", false]
+        ],
+        "invalidate() (dogpile.cache.region.regioninvalidationstrategy method)": [
+            [0, "dogpile.cache.region.RegionInvalidationStrategy.invalidate", false]
+        ],
+        "is_configured (dogpile.cache.region.cacheregion property)": [
+            [0, "dogpile.cache.region.CacheRegion.is_configured", false]
+        ],
+        "is_hard_invalidated() (dogpile.cache.region.defaultinvalidationstrategy method)": [
+            [0, "dogpile.cache.region.DefaultInvalidationStrategy.is_hard_invalidated", false]
+        ],
+        "is_hard_invalidated() (dogpile.cache.region.regioninvalidationstrategy method)": [
+            [0, "dogpile.cache.region.RegionInvalidationStrategy.is_hard_invalidated", false]
+        ],
+        "is_invalidated() (dogpile.cache.region.defaultinvalidationstrategy method)": [
+            [0, "dogpile.cache.region.DefaultInvalidationStrategy.is_invalidated", false]
+        ],
+        "is_invalidated() (dogpile.cache.region.regioninvalidationstrategy method)": [
+            [0, "dogpile.cache.region.RegionInvalidationStrategy.is_invalidated", false]
+        ],
+        "is_open (dogpile.cache.backends.file.abstractfilelock property)": [
+            [0, "dogpile.cache.backends.file.AbstractFileLock.is_open", false]
+        ],
+        "is_open (dogpile.cache.backends.file.filelock property)": [
+            [0, "dogpile.cache.backends.file.FileLock.is_open", false]
+        ],
+        "is_soft_invalidated() (dogpile.cache.region.defaultinvalidationstrategy method)": [
+            [0, "dogpile.cache.region.DefaultInvalidationStrategy.is_soft_invalidated", false]
+        ],
+        "is_soft_invalidated() (dogpile.cache.region.regioninvalidationstrategy method)": [
+            [0, "dogpile.cache.region.RegionInvalidationStrategy.is_soft_invalidated", false]
+        ],
+        "key_is_locked() (dogpile.cache.region.cacheregion method)": [
+            [0, "dogpile.cache.region.CacheRegion.key_is_locked", false]
+        ],
+        "key_mangler (dogpile.cache.api.cachebackend attribute)": [
+            [0, "dogpile.cache.api.CacheBackend.key_mangler", false]
+        ],
+        "keytype (in module dogpile.cache.api)": [
+            [0, "dogpile.cache.api.KeyType", false]
+        ],
+        "kwarg_function_key_generator() (in module dogpile.cache.util)": [
+            [0, "dogpile.cache.util.kwarg_function_key_generator", false]
+        ],
+        "length_conditional_mangler() (in module dogpile.cache.util)": [
+            [0, "dogpile.cache.util.length_conditional_mangler", false]
+        ],
+        "lock (class in dogpile)": [
+            [0, "dogpile.Lock", false]
+        ],
+        "locked() (dogpile.cache.api.cachemutex method)": [
+            [0, "dogpile.cache.api.CacheMutex.locked", false]
+        ],
+        "make_region() (in module dogpile.cache.region)": [
+            [0, "dogpile.cache.region.make_region", false]
+        ],
+        "makoplugin (class in dogpile.cache.plugins.mako_cache)": [
+            [0, "dogpile.cache.plugins.mako_cache.MakoPlugin", false]
+        ],
+        "memcachedbackend (class in dogpile.cache.backends.memcached)": [
+            [0, "dogpile.cache.backends.memcached.MemcachedBackend", false]
+        ],
+        "memcachedlock (class in dogpile.cache.backends.memcached)": [
+            [0, "dogpile.cache.backends.memcached.MemcachedLock", false]
+        ],
+        "memorybackend (class in dogpile.cache.backends.memory)": [
+            [0, "dogpile.cache.backends.memory.MemoryBackend", false]
+        ],
+        "memorypicklebackend (class in dogpile.cache.backends.memory)": [
+            [0, "dogpile.cache.backends.memory.MemoryPickleBackend", false]
+        ],
+        "metadata (dogpile.cache.api.cachedvalue attribute)": [
+            [0, "dogpile.cache.api.CachedValue.metadata", false]
+        ],
+        "module": [
+            [0, "module-dogpile.cache.api", false],
+            [0, "module-dogpile.cache.backends.file", false],
+            [0, "module-dogpile.cache.backends.memcached", false],
+            [0, "module-dogpile.cache.backends.memory", false],
+            [0, "module-dogpile.cache.backends.null", false],
+            [0, "module-dogpile.cache.backends.redis", false],
+            [0, "module-dogpile.cache.exception", false],
+            [0, "module-dogpile.cache.plugins.mako_cache", false],
+            [0, "module-dogpile.cache.proxy", false],
+            [0, "module-dogpile.cache.region", false]
+        ],
+        "nameregistry (class in dogpile.util)": [
+            [0, "dogpile.util.NameRegistry", false]
+        ],
+        "needregenerationexception (class in dogpile)": [
+            [0, "dogpile.NeedRegenerationException", false]
+        ],
+        "no_value (in module dogpile.cache.api)": [
+            [0, "dogpile.cache.api.NO_VALUE", false]
+        ],
+        "novalue (class in dogpile.cache.api)": [
+            [0, "dogpile.cache.api.NoValue", false]
+        ],
+        "nullbackend (class in dogpile.cache.backends.null)": [
+            [0, "dogpile.cache.backends.null.NullBackend", false]
+        ],
+        "payload (dogpile.cache.api.cachedvalue attribute)": [
+            [0, "dogpile.cache.api.CachedValue.payload", false]
+        ],
+        "pluginnotfound": [
+            [0, "dogpile.cache.exception.PluginNotFound", false]
+        ],
+        "proxybackend (class in dogpile.cache.proxy)": [
+            [0, "dogpile.cache.proxy.ProxyBackend", false]
+        ],
+        "pylibmcbackend (class in dogpile.cache.backends.memcached)": [
+            [0, "dogpile.cache.backends.memcached.PylibmcBackend", false]
+        ],
+        "pymemcachebackend (class in dogpile.cache.backends.memcached)": [
+            [0, "dogpile.cache.backends.memcached.PyMemcacheBackend", false]
+        ],
+        "read() (dogpile.cache.backends.file.abstractfilelock method)": [
+            [0, "dogpile.cache.backends.file.AbstractFileLock.read", false]
+        ],
+        "readwritemutex (class in dogpile.util)": [
+            [0, "dogpile.util.ReadWriteMutex", false]
+        ],
+        "redisbackend (class in dogpile.cache.backends.redis)": [
+            [0, "dogpile.cache.backends.redis.RedisBackend", false]
+        ],
+        "redisclusterbackend (class in dogpile.cache.backends.redis)": [
+            [0, "dogpile.cache.backends.redis.RedisClusterBackend", false]
+        ],
+        "redissentinelbackend (class in dogpile.cache.backends.redis)": [
+            [0, "dogpile.cache.backends.redis.RedisSentinelBackend", false]
+        ],
+        "regionalreadyconfigured": [
+            [0, "dogpile.cache.exception.RegionAlreadyConfigured", false]
+        ],
+        "regioninvalidationstrategy (class in dogpile.cache.region)": [
+            [0, "dogpile.cache.region.RegionInvalidationStrategy", false]
+        ],
+        "regionnotconfigured": [
+            [0, "dogpile.cache.exception.RegionNotConfigured", false]
+        ],
+        "release() (dogpile.cache.api.cachemutex method)": [
+            [0, "dogpile.cache.api.CacheMutex.release", false]
+        ],
+        "release() (dogpile.cache.backends.file.abstractfilelock method)": [
+            [0, "dogpile.cache.backends.file.AbstractFileLock.release", false]
+        ],
+        "release_read_lock() (dogpile.cache.backends.file.abstractfilelock method)": [
+            [0, "dogpile.cache.backends.file.AbstractFileLock.release_read_lock", false]
+        ],
+        "release_read_lock() (dogpile.cache.backends.file.filelock method)": [
+            [0, "dogpile.cache.backends.file.FileLock.release_read_lock", false]
+        ],
+        "release_read_lock() (dogpile.util.readwritemutex method)": [
+            [0, "dogpile.util.ReadWriteMutex.release_read_lock", false]
+        ],
+        "release_write_lock() (dogpile.cache.backends.file.abstractfilelock method)": [
+            [0, "dogpile.cache.backends.file.AbstractFileLock.release_write_lock", false]
+        ],
+        "release_write_lock() (dogpile.cache.backends.file.filelock method)": [
+            [0, "dogpile.cache.backends.file.FileLock.release_write_lock", false]
+        ],
+        "release_write_lock() (dogpile.util.readwritemutex method)": [
+            [0, "dogpile.util.ReadWriteMutex.release_write_lock", false]
+        ],
+        "serializedreturntype (in module dogpile.cache.api)": [
+            [0, "dogpile.cache.api.SerializedReturnType", false]
+        ],
+        "serializer (dogpile.cache.api.cachebackend attribute)": [
+            [0, "dogpile.cache.api.CacheBackend.serializer", false]
+        ],
+        "serializer (dogpile.cache.backends.memcached.genericmemcachedbackend attribute)": [
+            [0, "dogpile.cache.backends.memcached.GenericMemcachedBackend.serializer", false]
+        ],
+        "set() (dogpile.cache.api.cachebackend method)": [
+            [0, "dogpile.cache.api.CacheBackend.set", false]
+        ],
+        "set() (dogpile.cache.backends.memcached.genericmemcachedbackend method)": [
+            [0, "dogpile.cache.backends.memcached.GenericMemcachedBackend.set", false]
+        ],
+        "set() (dogpile.cache.backends.memory.memorybackend method)": [
+            [0, "dogpile.cache.backends.memory.MemoryBackend.set", false]
+        ],
+        "set() (dogpile.cache.backends.null.nullbackend method)": [
+            [0, "dogpile.cache.backends.null.NullBackend.set", false]
+        ],
+        "set() (dogpile.cache.proxy.proxybackend method)": [
+            [0, "dogpile.cache.proxy.ProxyBackend.set", false]
+        ],
+        "set() (dogpile.cache.region.cacheregion method)": [
+            [0, "dogpile.cache.region.CacheRegion.set", false]
+        ],
+        "set_arguments (dogpile.cache.backends.memcached.genericmemcachedbackend attribute)": [
+            [0, "dogpile.cache.backends.memcached.GenericMemcachedBackend.set_arguments", false]
+        ],
+        "set_multi() (dogpile.cache.api.cachebackend method)": [
+            [0, "dogpile.cache.api.CacheBackend.set_multi", false]
+        ],
+        "set_multi() (dogpile.cache.backends.memcached.genericmemcachedbackend method)": [
+            [0, "dogpile.cache.backends.memcached.GenericMemcachedBackend.set_multi", false]
+        ],
+        "set_multi() (dogpile.cache.backends.memory.memorybackend method)": [
+            [0, "dogpile.cache.backends.memory.MemoryBackend.set_multi", false]
+        ],
+        "set_multi() (dogpile.cache.backends.null.nullbackend method)": [
+            [0, "dogpile.cache.backends.null.NullBackend.set_multi", false]
+        ],
+        "set_multi() (dogpile.cache.proxy.proxybackend method)": [
+            [0, "dogpile.cache.proxy.ProxyBackend.set_multi", false]
+        ],
+        "set_multi() (dogpile.cache.region.cacheregion method)": [
+            [0, "dogpile.cache.region.CacheRegion.set_multi", false]
+        ],
+        "set_serialized() (dogpile.cache.api.bytesbackend method)": [
+            [0, "dogpile.cache.api.BytesBackend.set_serialized", false]
+        ],
+        "set_serialized() (dogpile.cache.api.cachebackend method)": [
+            [0, "dogpile.cache.api.CacheBackend.set_serialized", false]
+        ],
+        "set_serialized() (dogpile.cache.backends.file.dbmbackend method)": [
+            [0, "dogpile.cache.backends.file.DBMBackend.set_serialized", false]
+        ],
+        "set_serialized() (dogpile.cache.backends.redis.redisbackend method)": [
+            [0, "dogpile.cache.backends.redis.RedisBackend.set_serialized", false]
+        ],
+        "set_serialized() (dogpile.cache.proxy.proxybackend method)": [
+            [0, "dogpile.cache.proxy.ProxyBackend.set_serialized", false]
+        ],
+        "set_serialized_multi() (dogpile.cache.api.bytesbackend method)": [
+            [0, "dogpile.cache.api.BytesBackend.set_serialized_multi", false]
+        ],
+        "set_serialized_multi() (dogpile.cache.api.cachebackend method)": [
+            [0, "dogpile.cache.api.CacheBackend.set_serialized_multi", false]
+        ],
+        "set_serialized_multi() (dogpile.cache.backends.file.dbmbackend method)": [
+            [0, "dogpile.cache.backends.file.DBMBackend.set_serialized_multi", false]
+        ],
+        "set_serialized_multi() (dogpile.cache.backends.redis.redisbackend method)": [
+            [0, "dogpile.cache.backends.redis.RedisBackend.set_serialized_multi", false]
+        ],
+        "set_serialized_multi() (dogpile.cache.proxy.proxybackend method)": [
+            [0, "dogpile.cache.proxy.ProxyBackend.set_serialized_multi", false]
+        ],
+        "sha1_mangle_key() (in module dogpile.cache.util)": [
+            [0, "dogpile.cache.util.sha1_mangle_key", false]
+        ],
+        "validationerror": [
+            [0, "dogpile.cache.exception.ValidationError", false]
+        ],
+        "value_version (in module dogpile.cache.region)": [
+            [0, "dogpile.cache.region.value_version", false]
+        ],
+        "valuepayload (in module dogpile.cache.api)": [
+            [0, "dogpile.cache.api.ValuePayload", false]
+        ],
+        "was_hard_invalidated() (dogpile.cache.region.defaultinvalidationstrategy method)": [
+            [0, "dogpile.cache.region.DefaultInvalidationStrategy.was_hard_invalidated", false]
+        ],
+        "was_hard_invalidated() (dogpile.cache.region.regioninvalidationstrategy method)": [
+            [0, "dogpile.cache.region.RegionInvalidationStrategy.was_hard_invalidated", false]
+        ],
+        "was_soft_invalidated() (dogpile.cache.region.defaultinvalidationstrategy method)": [
+            [0, "dogpile.cache.region.DefaultInvalidationStrategy.was_soft_invalidated", false]
+        ],
+        "was_soft_invalidated() (dogpile.cache.region.regioninvalidationstrategy method)": [
+            [0, "dogpile.cache.region.RegionInvalidationStrategy.was_soft_invalidated", false]
+        ],
+        "wrap() (dogpile.cache.proxy.proxybackend method)": [
+            [0, "dogpile.cache.proxy.ProxyBackend.wrap", false]
+        ],
+        "wrap() (dogpile.cache.region.cacheregion method)": [
+            [0, "dogpile.cache.region.CacheRegion.wrap", false]
+        ],
+        "write() (dogpile.cache.backends.file.abstractfilelock method)": [
+            [0, "dogpile.cache.backends.file.AbstractFileLock.write", false]
+        ]
     },
     "objects": {
         "dogpile": [
             [0, 0, 1, "", "Lock"],
             [0, 0, 1, "", "NeedRegenerationException"]
         ],
         "dogpile.Lock.params": [
@@ -1933,15 +1170,14 @@
         ],
         "dogpile.cache.backends.memcached.GenericMemcachedBackend.get_multi.params": [
             [0, 1, 1, "", "keys"]
         ],
         "dogpile.cache.backends.memcached.GenericMemcachedBackend.params": [
             [0, 1, 1, "", "distributed_lock"],
             [0, 1, 1, "", "lock_timeout"],
-            [0, 1, 1, "", "memcached_expire_time"],
             [0, 1, 1, "", "url"]
         ],
         "dogpile.cache.backends.memcached.GenericMemcachedBackend.set.params": [
             [0, 1, 1, "", "key"],
             [0, 1, 1, "", "value"]
         ],
         "dogpile.cache.backends.memcached.GenericMemcachedBackend.set_multi.params": [
@@ -1954,14 +1190,15 @@
         "dogpile.cache.backends.memcached.PyMemcacheBackend.params": [
             [0, 1, 1, "", "dead_timeout"],
             [0, 1, 1, "", "default_noreply"],
             [0, 1, 1, "", "do_not_retry_for"],
             [0, 1, 1, "", "enable_retry_client"],
             [0, 1, 1, "", "hashclient_retry_attempts"],
             [0, 1, 1, "", "hashclient_retry_timeout"],
+            [0, 1, 1, "", "memcached_expire_time"],
             [0, 1, 1, "", "retry_attempts"],
             [0, 1, 1, "", "retry_delay"],
             [0, 1, 1, "", "retry_for"],
             [0, 1, 1, "", "serde"],
             [0, 1, 1, "", "socket_keepalive"],
             [0, 1, 1, "", "tls_context"]
         ],
@@ -2315,1057 +1552,1828 @@
         "dogpile.util.ReadWriteMutex": [
             [0, 4, 1, "", "acquire_read_lock"],
             [0, 4, 1, "", "acquire_write_lock"],
             [0, 4, 1, "", "release_read_lock"],
             [0, 4, 1, "", "release_write_lock"]
         ]
     },
+    "objnames": {
+        "0": ["py", "class", "Python class"],
+        "1": ["py", "parameter", "Python parameter"],
+        "2": ["py", "module", "Python module"],
+        "3": ["py", "data", "Python data"],
+        "4": ["py", "method", "Python method"],
+        "5": ["py", "attribute", "Python attribute"],
+        "6": ["py", "property", "Python property"],
+        "7": ["py", "exception", "Python exception"],
+        "8": ["py", "function", "Python function"]
+    },
     "objtypes": {
         "0": "py:class",
         "1": "py:parameter",
         "2": "py:module",
         "3": "py:data",
         "4": "py:method",
         "5": "py:attribute",
         "6": "py:property",
         "7": "py:exception",
         "8": "py:function"
     },
-    "objnames": {
-        "0": ["py", "class", "Python class"],
-        "1": ["py", "parameter", "Python parameter"],
-        "2": ["py", "module", "Python module"],
-        "3": ["py", "data", "Python data"],
-        "4": ["py", "method", "Python method"],
-        "5": ["py", "attribute", "Python attribute"],
-        "6": ["py", "property", "Python property"],
-        "7": ["py", "exception", "Python exception"],
-        "8": ["py", "function", "Python function"]
+    "terms": {
+        "": [0, 1, 2, 5, 6],
+        "0": [0, 2, 4, 5, 6],
+        "08": 1,
+        "1": [0, 4, 5, 6],
+        "10": [0, 1, 6],
+        "101": 1,
+        "11": 1,
+        "11211": [0, 6],
+        "119": 1,
+        "12": 1,
+        "122": 1,
+        "123": 1,
+        "127": [0, 5, 6],
+        "128": 1,
+        "129": 1,
+        "13": 1,
+        "134": 1,
+        "136": 1,
+        "137": 1,
+        "139": 1,
+        "14": 1,
+        "15": 1,
+        "154": 1,
+        "157": 1,
+        "159": 1,
+        "16": 1,
+        "160": 1,
+        "1684": 1,
+        "17": 1,
+        "171": 1,
+        "173": 1,
+        "178": 1,
+        "18": 1,
+        "181": 1,
+        "184": 1,
+        "185": 1,
+        "19": 1,
+        "191": 1,
+        "195": 1,
+        "2": [0, 4, 5, 6],
+        "20": 1,
+        "2012": 1,
+        "2013": 1,
+        "2014": 1,
+        "2015": 1,
+        "2016": 1,
+        "2017": 1,
+        "2018": 1,
+        "2019": 1,
+        "202": 1,
+        "2020": 1,
+        "2021": 1,
+        "2022": 1,
+        "2023": 1,
+        "2024": 1,
+        "203": 1,
+        "21": 1,
+        "220": 1,
+        "221": 1,
+        "223": 1,
+        "228": 1,
+        "23": 1,
+        "236": 1,
+        "238": 1,
+        "24": 1,
+        "240": 1,
+        "25": 1,
+        "250": 1,
+        "252": 1,
+        "26": 1,
+        "26379": 0,
+        "27": 1,
+        "28": 1,
+        "29": 1,
+        "2to3": 1,
+        "3": [0, 4, 6],
+        "30": 1,
+        "300": [0, 6],
+        "33": 1,
+        "35": 1,
+        "36": 1,
+        "360": 0,
+        "3600": [0, 2, 5, 6],
+        "37": 1,
+        "38": 1,
+        "39": 1,
+        "4": [0, 4, 5, 6],
+        "40": 1,
+        "41": 1,
+        "43": 1,
+        "44": 1,
+        "484": 1,
+        "5": [0, 4, 5, 6],
+        "501": 6,
+        "51": 1,
+        "517": 1,
+        "53def077a4264bd3183d4eb21b1f56f883e1b572": 2,
+        "54": 1,
+        "55": 1,
+        "5534": 1,
+        "57": 1,
+        "58": 1,
+        "6": [0, 2, 4, 6],
+        "60": 0,
+        "621": 1,
+        "6378": 0,
+        "6379": 0,
+        "6380": 0,
+        "6381": 0,
+        "65": 1,
+        "673": 1,
+        "7": [0, 4, 5, 6],
+        "71": 1,
+        "74": 1,
+        "8": [0, 4, 5],
+        "9": [4, 6],
+        "91": 1,
+        "97": 1,
+        "99": 1,
+        "A": [0, 1, 2, 6],
+        "As": 1,
+        "At": 6,
+        "By": [0, 6],
+        "For": [0, 1, 2, 6],
+        "If": [0, 2, 5, 6],
+        "In": [0, 1, 2, 5, 6],
+        "It": [0, 2, 6],
+        "No": 6,
+        "One": [0, 6],
+        "Such": [0, 6],
+        "The": [0, 1, 2, 3, 5, 6],
+        "Then": 6,
+        "There": [0, 2],
+        "These": [1, 6],
+        "To": [0, 6],
+        "Will": 0,
+        "With": [0, 6],
+        "_": [0, 5, 6],
+        "__future__": 1,
+        "__init__": [0, 6],
+        "__main__": 6,
+        "__name__": [0, 5, 6],
+        "__repr__": 1,
+        "__signature__": 1,
+        "_config_argument_dict": [0, 6],
+        "_config_prefix": [0, 6],
+        "_encodedproxi": 5,
+        "_hard_invalid": 0,
+        "_soft_invalid": 0,
+        "abc": 0,
+        "abil": 0,
+        "about": 3,
+        "abov": [0, 1, 2, 5, 6],
+        "abstract": [0, 1],
+        "abstractfilelock": [0, 1],
+        "accept": [0, 1, 6],
+        "access": [0, 1, 2, 6],
+        "accessor": [0, 1],
+        "accomplish": 2,
+        "account": [0, 1],
+        "acheiv": 5,
+        "acquir": [0, 1, 6],
+        "acquire_read_lock": 0,
+        "acquire_write_lock": 0,
+        "across": [0, 1, 2],
+        "act": 2,
+        "action": 0,
+        "actual": [0, 1, 2, 5, 6],
+        "actual_backend": [0, 1],
+        "ad": [0, 1, 2, 6],
+        "adapt": 4,
+        "add": [0, 1, 5],
+        "add_new_data": 5,
+        "addit": [0, 1, 2, 6],
+        "addition": [1, 4],
+        "address": 2,
+        "adjust": [1, 4],
+        "admin": 0,
+        "advanc": 0,
+        "advantag": 0,
+        "adventag": 6,
+        "affect": [0, 6],
+        "after": [0, 1, 5, 6],
+        "after_commit": 5,
+        "ag": [0, 1],
+        "again": [0, 2, 6],
+        "against": [0, 1, 2, 6],
+        "ahead": 2,
+        "akkerman": 1,
+        "alert": 2,
+        "alessio": 1,
+        "alexand": 1,
+        "alia": 0,
+        "all": [0, 1, 2, 4, 6],
+        "allow": [0, 1, 2, 4, 6],
+        "along": [0, 1, 2, 5],
+        "alpha": 1,
+        "alphabet": 0,
+        "alreadi": [0, 1, 6],
+        "also": [0, 1, 2, 5, 6],
+        "alter": [0, 6],
+        "altern": [0, 6],
+        "although": 1,
+        "alwai": [0, 6],
+        "among": 6,
+        "amount": 0,
+        "an": [0, 1, 2, 4, 5, 6],
+        "analogu": 0,
+        "anderson": 1,
+        "anentrop": 1,
+        "ani": [0, 1, 2, 4, 6],
+        "ankitpatel96": 1,
+        "annot": 1,
+        "anoth": [0, 1, 2, 4, 6],
+        "answer": 2,
+        "anticip": 2,
+        "antoin": 1,
+        "anydbm": 0,
+        "anyth": 6,
+        "api": [1, 4, 5, 6],
+        "app": 1,
+        "appar": 1,
+        "appear": [0, 1],
+        "append": [0, 5],
+        "appli": [0, 1, 5, 6],
+        "applic": [0, 1, 2, 4, 6],
+        "approach": [0, 1, 2, 5, 6],
+        "appropri": [0, 6],
+        "approxim": 2,
+        "apr": 1,
+        "ar": [0, 1, 3, 4, 6],
+        "araujo": 1,
+        "arbitrari": 0,
+        "aren": 0,
+        "arg": [0, 5, 6],
+        "argnam": 0,
+        "argspec": 0,
+        "argument": [0, 1, 2, 5, 6],
+        "argvalu": 0,
+        "around": [0, 2],
+        "ascii": [0, 6],
+        "asdict": [0, 1],
+        "ask": 0,
+        "assembl": 0,
+        "assert": 5,
+        "associ": [0, 5, 6],
+        "assum": [0, 1],
+        "async": 1,
+        "async_cr": [0, 6],
+        "async_creation_runn": [0, 1, 5, 6],
+        "asynchron": [0, 1, 4, 6],
+        "attach": 0,
+        "attempt": [0, 6],
+        "attribut": [0, 1, 6],
+        "aug": 1,
+        "augment": [0, 1, 6],
+        "authent": [0, 1],
+        "automat": 0,
+        "avail": [0, 1, 3, 4, 5, 6],
+        "averystrongpassword": 0,
+        "avoid": [1, 5],
+        "awar": [0, 5, 6],
+        "azoff": 1,
+        "b": [0, 6],
+        "back": [0, 1],
+        "backend": [1, 2, 4, 5],
+        "backendformat": 0,
+        "backendsettyp": 0,
+        "background": [0, 5, 6],
+        "backward": [0, 1],
+        "base": [0, 1, 2, 5, 6],
+        "basi": [0, 1, 6],
+        "basic": [0, 6],
+        "basicconfig": 6,
+        "bastien": 1,
+        "baton": 2,
+        "beaker": [0, 2],
+        "bean": 1,
+        "becom": [0, 6],
+        "been": [0, 1, 2, 5, 6],
+        "befor": [0, 1, 2, 6],
+        "behalf": 6,
+        "behav": 0,
+        "behavior": [0, 1, 4, 5],
+        "behind": 6,
+        "being": [0, 1, 5, 6],
+        "beitei": 1,
+        "below": [0, 5, 6],
+        "ben": 1,
+        "bertin": 1,
+        "besid": 5,
+        "best": 0,
+        "between": [0, 6],
+        "beyond": 1,
+        "binari": 0,
+        "bit": 6,
+        "block": [0, 2, 4, 5, 6],
+        "bmemcach": [0, 1],
+        "bmemcachedbackend": 0,
+        "bogon": 1,
+        "bookkeep": 5,
+        "bool": [0, 6],
+        "boolean": [0, 1],
+        "both": [0, 1],
+        "bother": 6,
+        "break": 1,
+        "brian": 1,
+        "brown": 1,
+        "brunner": 1,
+        "bsddb": [0, 6],
+        "bug": 4,
+        "build": [0, 1, 2, 4, 5],
+        "built": [0, 6],
+        "builtin": [0, 6],
+        "bypass": [0, 1, 6],
+        "byte": [0, 1, 6],
+        "bytesbackend": [0, 1],
+        "bytestr": [0, 1, 6],
+        "ca": 0,
+        "cach": [0, 1, 3, 5, 6],
+        "cache_arg": 0,
+        "cache_dict": 0,
+        "cache_impl": 0,
+        "cache_multi_on_argu": [0, 1, 6],
+        "cache_on_argu": [0, 1, 5, 6],
+        "cache_refresh": 5,
+        "cache_region": 0,
+        "cache_timeout": 1,
+        "cachebackend": [0, 6],
+        "cached_tim": 0,
+        "cachedvalu": [0, 1, 5, 6],
+        "cachefil": 0,
+        "cacheimpl": 0,
+        "cachemutex": [0, 6],
+        "cacheregion": [0, 1, 5, 6],
+        "cachereturntyp": [0, 1],
+        "cafil": 0,
+        "calcul": 1,
+        "call": [0, 1, 2, 5, 6],
+        "callabl": [0, 1, 5, 6],
+        "caller": 0,
+        "can": [0, 1, 2, 5, 6],
+        "cannot": [0, 1, 6],
+        "cantdeserializeexcept": [0, 1, 6],
+        "case": [0, 1, 2, 5, 6],
+        "categori": 2,
+        "caus": 1,
+        "caveat": [0, 6],
+        "celeri": [0, 6],
+        "certain": [0, 6],
+        "certif": 0,
+        "cfg": 1,
+        "chain": [0, 1, 6],
+        "chang": [0, 1, 2, 4, 5],
+        "changelog": 4,
+        "charset": 0,
+        "check": [0, 1, 2, 6],
+        "choos": 0,
+        "christian": 1,
+        "circumst": 6,
+        "cl": [0, 6],
+        "class": [0, 1, 2, 5, 6],
+        "client": [0, 1, 2, 5, 6],
+        "client_fn": 0,
+        "cluster": [0, 1],
+        "clusternod": 0,
+        "code": [0, 2, 5],
+        "coerc": [0, 1, 6],
+        "coerce_string_conf": 1,
+        "coercion": 1,
+        "collect": 0,
+        "collis": 5,
+        "com": [1, 3],
+        "combin": [0, 6],
+        "come": 1,
+        "command": 1,
+        "commit": 5,
+        "common": [0, 1, 2, 6],
+        "commun": 1,
+        "compar": [0, 6],
+        "compat": [0, 1],
+        "compatbl": 1,
+        "complement": 1,
+        "complet": [0, 2],
+        "complex": 0,
+        "compon": 6,
+        "comprehens": 0,
+        "comput": [0, 6],
+        "concept": [0, 2, 4],
+        "concern": 5,
+        "concret": 0,
+        "concurr": [0, 2, 6],
+        "condit": [0, 1],
+        "condition": [0, 6],
+        "conf": 1,
+        "config": [0, 1, 6],
+        "config_dict": [0, 6],
+        "configur": [0, 1, 4, 5],
+        "configure_from_config": [0, 1, 6],
+        "conjunct": [0, 1, 6],
+        "connect": [0, 1],
+        "connection_kwarg": [0, 1],
+        "connection_pool": [0, 1],
+        "connectionpool": [0, 1],
+        "conserv": 1,
+        "consid": [0, 1, 6],
+        "consist": [4, 6],
+        "constant": [0, 1],
+        "construct": [0, 1, 6],
+        "constructor": [0, 6],
+        "consult": [0, 6],
+        "contain": [0, 5, 6],
+        "content": 0,
+        "context": [0, 2],
+        "continu": [0, 1, 2],
+        "contribut": 1,
+        "control": 4,
+        "conveni": [0, 6],
+        "convert": [0, 6],
+        "coordin": [0, 2, 6],
+        "copi": [0, 1],
+        "core": [1, 4, 6],
+        "correct": [0, 6],
+        "correctli": 1,
+        "correspond": 0,
+        "could": [0, 1, 5],
+        "count": 5,
+        "counter": 5,
+        "courtesi": 1,
+        "cover": 1,
+        "cpickl": 0,
+        "creat": [0, 1, 2, 4],
+        "create_default_context": 0,
+        "create_some_resourc": 2,
+        "create_valu": [0, 6],
+        "createdtim": 2,
+        "creation": [0, 1, 2, 4, 6],
+        "creation_funct": 0,
+        "creation_tim": 0,
+        "creationtim": 2,
+        "creator": [0, 1, 4, 6],
+        "creator_arg": [0, 1, 6],
+        "critic": 1,
+        "cross": 2,
+        "ctx": 0,
+        "current": [0, 1, 2, 6],
+        "custom": [0, 1, 5, 6],
+        "custominvalidationstrategi": 0,
+        "customiz": 1,
+        "cutom": 0,
+        "d": [0, 2, 5, 6],
+        "d_arg1_arg2_arg3": 5,
+        "daemon": 5,
+        "dai": [0, 6],
+        "dairiki": 1,
+        "daniel": 1,
+        "data": [0, 4, 6],
+        "databas": 5,
+        "datastructur": 0,
+        "date": [0, 1, 6],
+        "datetim": [0, 1, 6],
+        "daverbal": 1,
+        "david": 1,
+        "db": 0,
+        "dbclass": 5,
+        "dbm": [0, 1, 6],
+        "dbmbackend": [0, 1],
+        "dbmfile": [0, 6],
+        "de": 1,
+        "dead": 0,
+        "dead_retri": [0, 1],
+        "dead_timeout": [0, 1],
+        "deadlock": 1,
+        "deal": [0, 1],
+        "debug": [1, 6],
+        "dec": 1,
+        "declar": [0, 6],
+        "decod": 4,
+        "decor": [0, 1, 2, 5, 6],
+        "def": [0, 2, 5, 6],
+        "default": [0, 1, 5, 6],
+        "default_norepli": 0,
+        "defaultinvalidationstrategi": 0,
+        "defaultseri": 0,
+        "defer": [0, 2, 6],
+        "defin": [1, 5, 6],
+        "delai": 5,
+        "deleg": 0,
+        "delet": [0, 1, 5, 6],
+        "delete_multi": [0, 1],
+        "deliv": 1,
+        "depend": [0, 1, 6],
+        "deprec": 1,
+        "deriv": [0, 6],
+        "describ": [0, 2, 6],
+        "descriptor": 0,
+        "deseri": [0, 1, 6],
+        "design": [2, 6],
+        "desir": 0,
+        "destruct": 1,
+        "detail": [0, 6],
+        "detect": [0, 6],
+        "determin": [0, 1, 6],
+        "dev": 1,
+        "deveaux": 1,
+        "develop": 1,
+        "dict": [0, 5],
+        "dictionari": [0, 1, 6],
+        "dictionarybackend": 6,
+        "did": [1, 6],
+        "didn": 1,
+        "differ": [0, 1, 2, 5, 6],
+        "digest": 2,
+        "direct": [0, 1, 5],
+        "directli": [0, 1, 4, 6],
+        "directori": [0, 1],
+        "disabl": [0, 1, 6],
+        "disambigu": [0, 6],
+        "disappear": 2,
+        "discard": 0,
+        "discov": 0,
+        "discoveri": 0,
+        "distinguish": [0, 6],
+        "distribut": [0, 1, 4],
+        "distributed_lock": [0, 1, 6],
+        "distro": 1,
+        "do": [0, 1, 4, 5],
+        "do_not_retry_for": 0,
+        "do_refresh": 5,
+        "do_someth": 2,
+        "doc": [0, 1],
+        "document": [0, 1, 3],
+        "doe": [0, 1, 5, 6],
+        "doesn": [0, 2],
+        "dogpil": [1, 3, 5, 6],
+        "dogpile_lockfil": 0,
+        "dogpilecach": 3,
+        "dogpilecacheexcept": 0,
+        "don": [0, 1],
+        "done": 5,
+        "dont_cache_non": [0, 6],
+        "down": [0, 6],
+        "driver": 0,
+        "drop": [0, 1],
+        "due": 1,
+        "dump": [0, 1, 6],
+        "dure": [0, 1, 2],
+        "dynam": [0, 1, 6],
+        "e": [0, 1, 5, 6],
+        "each": [0, 1, 2, 5, 6],
+        "easi": 4,
+        "easier": [1, 6],
+        "easili": [5, 6],
+        "edg": 6,
+        "ef206ed4473fec3b639": 1,
+        "effect": [0, 1],
+        "effici": 2,
+        "effort": 1,
+        "either": [0, 1, 5, 6],
+        "elaps": 0,
+        "elect": 0,
+        "element": 1,
+        "elimin": 6,
+        "els": [0, 2],
+        "emit": [1, 6],
+        "emploi": 1,
+        "empti": 1,
+        "en": 0,
+        "enabl": [0, 1],
+        "enable_retry_cli": [0, 1],
+        "encapsul": 2,
+        "enclos": 0,
+        "encod": 4,
+        "encourag": 4,
+        "end": [0, 1, 2, 6],
+        "enhanc": [1, 3],
+        "enough": 0,
+        "ensur": [1, 2],
+        "enter": 5,
+        "entir": [0, 1, 6],
+        "entri": 1,
+        "entry_point": 6,
+        "entrypoint": [0, 1, 6],
+        "enum": [0, 1],
+        "environ": [0, 1, 4],
+        "eol": 1,
+        "epoch": 0,
+        "equival": [0, 1, 6],
+        "eric": 1,
+        "errant": 1,
+        "erron": [0, 1],
+        "error": [0, 1],
+        "establish": [0, 1, 6],
+        "etc": [0, 1],
+        "evalu": [0, 6],
+        "even": [0, 1],
+        "event": [1, 4, 6],
+        "everi": [0, 1, 2],
+        "everyth": 5,
+        "exact": 1,
+        "exampl": [0, 1, 4, 5, 6],
+        "excel": 6,
+        "except": [1, 4, 5, 6],
+        "exception": 5,
+        "excess": 1,
+        "execut": 4,
+        "exist": [0, 1, 2, 6],
+        "existing_valu": 0,
+        "expand": 1,
+        "expect": 2,
+        "expedi": 5,
+        "expens": [0, 2, 6],
+        "expir": [0, 1, 2, 6],
+        "expiration_tim": [0, 1, 2, 5, 6],
+        "expiretim": 0,
+        "expiri": 0,
+        "explicitli": 0,
+        "expos": 1,
+        "extend": [0, 5, 6],
+        "extra": [0, 6],
+        "face": 1,
+        "facil": 6,
+        "facilil": 1,
+        "fact": [0, 6],
+        "fail": [0, 1, 6],
+        "failur": [0, 1],
+        "fainberg": 1,
+        "fall": 2,
+        "fallback": 1,
+        "fals": [0, 1, 5, 6],
+        "far": 2,
+        "fast": 0,
+        "faster": 6,
+        "favor": 1,
+        "fcntl": 0,
+        "featur": [0, 3, 6],
+        "feb": 1,
+        "fedorov": 1,
+        "fidosz": 1,
+        "field": 1,
+        "file": [1, 4, 6],
+        "filelock": [0, 1, 2],
+        "filenam": [0, 2, 6],
+        "filesystem": [0, 2],
+        "filter": 5,
+        "final": [0, 6],
+        "find": 0,
+        "finish": [0, 2, 6],
+        "first": [0, 1, 2, 6],
+        "fix": [0, 1, 6],
+        "flag": [0, 1, 6],
+        "flexibl": 0,
+        "float": [0, 1, 6],
+        "flock": [0, 1, 2],
+        "flufl": 2,
+        "fly": 5,
+        "fn": [0, 2, 5, 6],
+        "fname": [0, 5, 6],
+        "fname_": 5,
+        "focus": 6,
+        "follow": [0, 1, 2, 6],
+        "foo": [0, 6],
+        "foo1": 0,
+        "forc": [0, 1],
+        "forego": 1,
+        "foremost": 6,
+        "form": [0, 1, 6],
+        "format": [0, 1, 4],
+        "former": 0,
+        "found": [0, 6],
+        "frequent": 1,
+        "fri": 1,
+        "frit": 1,
+        "from": [0, 1, 2, 3, 5, 6],
+        "from_url": [0, 1],
+        "front": [0, 2, 4, 6],
+        "full": 1,
+        "fulli": 1,
+        "function": [0, 1, 2, 5, 6],
+        "function_key_gener": [0, 1, 5, 6],
+        "function_multi_key_gener": [0, 1, 6],
+        "further": 0,
+        "futur": [0, 1, 6],
+        "g": [0, 1, 6],
+        "garbag": 0,
+        "gdbm": 1,
+        "gen": [0, 6],
+        "gen_cach": 2,
+        "gener": [0, 1, 2, 4, 5, 6],
+        "generate_kei": [0, 5, 6],
+        "generate_my_expensive_valu": 2,
+        "generate_someth": [0, 6],
+        "genericmemachedbackend": 0,
+        "genericmemcachedbackend": [0, 1],
+        "gerard": 1,
+        "get": [0, 1, 2, 5, 6],
+        "get_multi": [0, 1, 5, 6],
+        "get_mutex": 0,
+        "get_or_cr": [0, 1, 6],
+        "get_or_create_multi": [0, 1, 5, 6],
+        "get_seri": 0,
+        "get_serialized_multi": 0,
+        "get_some_data": 5,
+        "get_valu": 2,
+        "get_value_metadata": [0, 1],
+        "getargspec": 1,
+        "getfullargspec": 1,
+        "getlogg": 6,
+        "getter": [0, 1],
+        "getting_start": 0,
+        "git": 1,
+        "github": [1, 3],
+        "given": [0, 1, 2, 5, 6],
+        "glitch": 1,
+        "global": 2,
+        "goe": [0, 2],
+        "good": [2, 5],
+        "gracefulli": [0, 1, 6],
+        "great": 1,
+        "greater": 0,
+        "group": 4,
+        "gr\u00e9goir": 1,
+        "guard": 1,
+        "guid": 4,
+        "guimar\u00e3": 1,
+        "g\u00f3rny": 1,
+        "ha": [0, 1, 2, 5, 6],
+        "had": 1,
+        "hanchrow": 1,
+        "hand": [0, 6],
+        "handl": 0,
+        "hanu": 1,
+        "happen": 5,
+        "hard": [0, 1, 5, 6],
+        "hardcod": 1,
+        "hardwir": 1,
+        "has_valu": 0,
+        "hash": [0, 6],
+        "hashclient": [0, 1],
+        "hashclient_retry_attempt": [0, 1],
+        "hashclient_retry_timeout": [0, 1],
+        "hashlib": 2,
+        "have": [0, 1, 2, 5, 6],
+        "hayden": 1,
+        "hbccbh": 1,
+        "head": 1,
+        "held": 0,
+        "help": [0, 5, 6],
+        "helper": 6,
+        "henc": 6,
+        "here": [0, 2, 6],
+        "hewitt": 1,
+        "hex": 2,
+        "hexdigest": 2,
+        "high": [1, 4, 6],
+        "highest_protocol": [0, 1],
+        "hit": [0, 5],
+        "hoc": [2, 6],
+        "homepag": 4,
+        "hongbin": 1,
+        "honor": [0, 1],
+        "hood": 5,
+        "hook": [4, 5],
+        "hope": 5,
+        "host": [0, 1, 3],
+        "hostnam": 0,
+        "hour": 0,
+        "how": [0, 2, 6],
+        "howev": [0, 1, 2, 5, 6],
+        "html": 0,
+        "http": [0, 1, 3, 5],
+        "i": [0, 1, 3, 4, 5, 6],
+        "id": 5,
+        "idea": [2, 5],
+        "idempot": [0, 6],
+        "identifi": [0, 1, 6],
+        "ignor": [0, 1, 6],
+        "ignore_expir": [0, 1, 6],
+        "illustr": [0, 2, 6],
+        "immedi": [0, 6],
+        "impact": 0,
+        "implement": [0, 1, 5, 6],
+        "impli": [0, 2],
+        "implicitli": 1,
+        "import": [0, 1, 2, 5, 6],
+        "improv": [0, 1, 5],
+        "inadvert": 1,
+        "includ": [0, 1, 6],
+        "incom": [0, 1, 6],
+        "incompat": [0, 1],
+        "increas": 0,
+        "incur": 0,
+        "independ": 0,
+        "index": [3, 4],
+        "indic": [0, 1, 6],
+        "indirectli": 2,
+        "individu": 0,
+        "info": 1,
+        "inform": [0, 3, 6],
+        "inher": 0,
+        "inherit": [0, 5],
+        "ini": 1,
+        "initi": [0, 1, 2, 6],
+        "inject": 0,
+        "insert": 0,
+        "insid": [0, 6],
+        "inspect": 1,
+        "instal": [1, 4, 6],
+        "instanc": [0, 1, 2, 5, 6],
+        "instant": 6,
+        "instanti": [0, 5, 6],
+        "instead": [1, 2, 5],
+        "instruct": 6,
+        "int": [0, 1],
+        "integ": [0, 1, 5, 6],
+        "integr": 4,
+        "intend": 1,
+        "intent": 0,
+        "interfac": [0, 2, 4, 6],
+        "interfer": 1,
+        "intern": [0, 1, 2, 6],
+        "interpret": [0, 1, 6],
+        "invalid": [0, 1, 4, 6],
+        "invalidate_user_id": 5,
+        "invoc": [0, 2],
+        "invok": [0, 2, 6],
+        "involv": [0, 1],
+        "io": 0,
+        "ioerror": 0,
+        "is_configur": [0, 1],
+        "is_hard_invalid": 0,
+        "is_invalid": 0,
+        "is_open": 0,
+        "is_soft_invalid": 0,
+        "is_unittest": 1,
+        "isinst": 5,
+        "isn": [0, 1, 6],
+        "issu": [1, 2, 3, 6],
+        "item": [0, 1, 6],
+        "iteritem": 5,
+        "itertool": 5,
+        "its": [0, 1, 2, 4, 6],
+        "itself": [0, 1, 2, 6],
+        "jack": 1,
+        "jami": 1,
+        "jan": 1,
+        "jeff": 1,
+        "jimmei": 1,
+        "job": 0,
+        "john": 1,
+        "join": [0, 2, 5, 6],
+        "jon": 1,
+        "jonathan": 1,
+        "json": [0, 1, 5, 6],
+        "jul": 1,
+        "juli": 1,
+        "jun": 1,
+        "just": [0, 2, 5, 6],
+        "justin": 1,
+        "k": [0, 5, 6],
+        "k1": 0,
+        "k2": 0,
+        "k3": 0,
+        "kajinami": 1,
+        "karthikeyan": 1,
+        "keep": [0, 2],
+        "keepal": [0, 1],
+        "keepaliveopt": 0,
+        "kei": [0, 1, 2, 4, 6],
+        "ketama": 0,
+        "key1": 0,
+        "key2": 0,
+        "key3": 0,
+        "key_is_lock": [0, 1],
+        "key_mangl": [0, 1, 5, 6],
+        "key_templ": 5,
+        "keyerror": 1,
+        "keyreentrantmutex": 1,
+        "keytyp": 0,
+        "keyword": [0, 1, 6],
+        "kind": [0, 6],
+        "klinger": 1,
+        "know": 5,
+        "known": 1,
+        "kolak": 1,
+        "krau": 1,
+        "kw": [0, 6],
+        "kwarg": [0, 5, 6],
+        "kwarg_function_key_gener": [0, 1, 6],
+        "lambda": 5,
+        "larger": [0, 1],
+        "last": [0, 6],
+        "lastli": [0, 6],
+        "later": [0, 6],
+        "latest": 0,
+        "latter": 0,
+        "lead": [1, 5],
+        "learn": 4,
+        "least": [0, 2, 5],
+        "leav": 5,
+        "left": [0, 1],
+        "length": [0, 1, 6],
+        "length_conditional_mangl": 0,
+        "lennox": 1,
+        "less": 1,
+        "level": [0, 1, 2, 6],
+        "lib": 0,
+        "librari": [0, 1, 6],
+        "life": 6,
+        "like": [0, 1, 2, 5, 6],
+        "link": [0, 5],
+        "list": [0, 1, 6],
+        "listens_for": 5,
+        "liter": [0, 1, 6],
+        "ll": [0, 2],
+        "load": [0, 1, 6],
+        "load_user_info": 6,
+        "local": [0, 1, 2, 5, 6],
+        "local_region": [0, 6],
+        "localhost": [0, 2],
+        "locat": [1, 6],
+        "lock": [0, 1, 4, 6],
+        "lock_factori": [0, 1],
+        "lock_path": 2,
+        "lock_sleep": [0, 1],
+        "lock_timeout": [0, 1],
+        "lockfil": [0, 2],
+        "log": [1, 4],
+        "loggingproxi": 6,
+        "logic": [0, 1],
+        "long": [0, 1, 6],
+        "longer": [0, 1, 6],
+        "look": 6,
+        "lookup": [0, 2],
+        "lookup_user_by_id": 6,
+        "lose": 1,
+        "lot": 4,
+        "lu": 1,
+        "lutz": 1,
+        "lx": 1,
+        "mabei": 1,
+        "made": [0, 1, 2],
+        "magnitud": 1,
+        "mai": [0, 1, 2, 5, 6],
+        "main": 5,
+        "maintain": 1,
+        "makarov": 1,
+        "make": [0, 1, 2, 6],
+        "make_region": [0, 5, 6],
+        "mako": 1,
+        "mako_cach": [0, 1],
+        "mako_lookup": 0,
+        "makoplugin": 0,
+        "manag": [0, 2, 5, 6],
+        "mangl": [0, 1, 5, 6],
+        "mangler": [0, 1, 5, 6],
+        "mani": [0, 1, 6],
+        "map": [0, 1, 5, 6],
+        "mapping_set": 5,
+        "mar": 1,
+        "marco": 1,
+        "mark": [0, 1],
+        "markedli": 6,
+        "masayuko": 1,
+        "match": [0, 1],
+        "matter": 4,
+        "ma\u00ebl": 1,
+        "mc": [0, 2, 6],
+        "mc_pool": 2,
+        "me": 5,
+        "mean": [0, 1, 5, 6],
+        "mechan": [0, 1, 4, 6],
+        "medeiro": 1,
+        "memcach": [1, 2, 6],
+        "memcachearg": [0, 1],
+        "memcacheclienterror": 0,
+        "memcached_expire_tim": [0, 1],
+        "memcached_region": [0, 6],
+        "memcachedbackend": [0, 1],
+        "memcachedlock": 0,
+        "memcacheillegalinputerror": 0,
+        "memcacheunexpectedcloseerror": 0,
+        "memoized_properti": 1,
+        "memori": [1, 5],
+        "memory_pickl": 0,
+        "memorybackend": [0, 1],
+        "memorypickl": 1,
+        "memorypicklebackend": [0, 1],
+        "menkevi\u010diu": 1,
+        "messag": [1, 6],
+        "metadata": [0, 1, 5, 6],
+        "metadatatyp": 0,
+        "method": [0, 1, 5, 6],
+        "micha\u0142": 1,
+        "might": [0, 6],
+        "min_compress_len": [0, 1],
+        "mind": 6,
+        "minim": 5,
+        "minimum": [0, 1],
+        "minu": 2,
+        "miss": [0, 1, 6],
+        "moc": [0, 6],
+        "mode": [0, 1, 6],
+        "model": 6,
+        "modern": 0,
+        "modifi": 0,
+        "modul": [0, 1, 4, 6],
+        "modulu": 0,
+        "mois\u00e9": 1,
+        "moment": 5,
+        "mon": 1,
+        "more": [0, 1, 2, 6],
+        "morgan": 1,
+        "most": [0, 1, 2, 3],
+        "move": [0, 1],
+        "msgpack": 5,
+        "msgpackproxi": 5,
+        "much": 5,
+        "multipl": [0, 1, 2, 6],
+        "multithread": [0, 6],
+        "multivalu": 1,
+        "must": [0, 1],
+        "mutex": [0, 2, 6],
+        "mutexlock": 0,
+        "my": 0,
+        "my_data": [0, 6],
+        "my_dictionari": 0,
+        "my_foo": 0,
+        "my_funct": [0, 6],
+        "my_key_gener": [0, 5, 6],
+        "my_multi_key_gener": [0, 6],
+        "my_region": [0, 6],
+        "myapp": [0, 5, 6],
+        "mybackend": 6,
+        "myclass": [0, 6],
+        "myconfig": [0, 6],
+        "myfirstproxi": 0,
+        "myfoo": 0,
+        "myinvalid": 0,
+        "mymast": 0,
+        "myotherclass": [0, 6],
+        "mypackag": 6,
+        "mypi": 1,
+        "myregion": 6,
+        "mysecondproxi": 0,
+        "mysect": 0,
+        "naccach": 1,
+        "name": [0, 1, 6],
+        "namedtupl": 0,
+        "nameregistri": [0, 1],
+        "namespac": [0, 1, 5, 6],
+        "nativ": 6,
+        "necessari": 5,
+        "necessarili": [0, 1, 6],
+        "need": [0, 1, 4, 5, 6],
+        "needregenerationexcept": [0, 2],
+        "neg": 1,
+        "negat": 5,
+        "nest": 5,
+        "network": 0,
+        "never": 0,
+        "new": [0, 1, 2, 4, 5, 6],
+        "new_valu": 0,
+        "newli": [0, 1, 2, 6],
+        "newvalu": [0, 6],
+        "next": [0, 2, 5],
+        "nf": 2,
+        "no_tag": 1,
+        "no_valu": [0, 1, 5, 6],
+        "node": 0,
+        "non": [0, 1, 2, 6],
+        "none": [0, 1, 2, 6],
+        "noqa": 0,
+        "nor": 1,
+        "norepli": 0,
+        "normal": [0, 2, 6],
+        "note": [0, 2, 6],
+        "notimplementederror": [0, 5],
+        "nov": 1,
+        "novalu": [0, 1, 6],
+        "now": [0, 1, 2, 5, 6],
+        "null": 1,
+        "nullbackend": [0, 1],
+        "nulllock": 1,
+        "number": [0, 2, 6],
+        "o": [0, 1, 2],
+        "object": [0, 1, 2, 4, 6],
+        "object_hook": 5,
+        "observ": 1,
+        "occur": [0, 1, 6],
+        "oct": 1,
+        "off": 2,
+        "offer": 6,
+        "offload": 5,
+        "often": 2,
+        "old": [0, 1, 5, 6],
+        "older": [0, 2, 6],
+        "olli": 1,
+        "omit": [0, 1],
+        "onc": [0, 1, 2],
+        "one": [0, 1, 2, 4, 5, 6],
+        "ones": [0, 5],
+        "onli": [0, 1, 2, 5, 6],
+        "oper": [0, 1, 2, 5, 6],
+        "optimist": 5,
+        "option": [0, 1, 6],
+        "order": [0, 1, 2, 5, 6],
+        "ordinari": 0,
+        "org": [0, 3, 5],
+        "organ": 1,
+        "orient": 0,
+        "origin": [0, 1, 6],
+        "orm": 4,
+        "other": [0, 1, 2, 4, 5, 6],
+        "otherwis": [0, 1, 5, 6],
+        "our": [2, 5, 6],
+        "out": [1, 5],
+        "output": [1, 2],
+        "outsid": [0, 2, 6],
+        "over": 0,
+        "overal": 1,
+        "overrid": [0, 5, 6],
+        "overridden": [0, 6],
+        "overview": 4,
+        "own": [0, 2, 4, 5],
+        "packag": [0, 1, 2, 3],
+        "packb": 5,
+        "page": 4,
+        "pair": [0, 2],
+        "param": 0,
+        "paramet": [0, 1, 6],
+        "paramt": 0,
+        "parent": [0, 6],
+        "pars": 1,
+        "part": [0, 1, 6],
+        "parti": 0,
+        "particular": [0, 1, 2, 5, 6],
+        "particularli": 6,
+        "pass": [0, 1, 2, 5, 6],
+        "passthrough": 0,
+        "password": [0, 1],
+        "past": 0,
+        "patch": 1,
+        "path": [0, 2, 6],
+        "pattern": 6,
+        "paul": 1,
+        "payload": [0, 1, 5, 6],
+        "pem": 0,
+        "pep": 1,
+        "per": [0, 1, 2, 6],
+        "perform": [0, 1, 2, 5, 6],
+        "period": [0, 2, 6],
+        "persist": [0, 1, 5, 6],
+        "pickl": [0, 1, 5, 6],
+        "pickle_serd": 0,
+        "pileup": 1,
+        "pin": 1,
+        "pip": [1, 3],
+        "pkg_resourc": 1,
+        "place": [0, 1, 5, 6],
+        "plain": [0, 1],
+        "plan": 1,
+        "platform": [0, 1],
+        "plu": 1,
+        "pluck": [0, 6],
+        "pluggabl": 1,
+        "plugin": [1, 4, 6],
+        "pluginload": 1,
+        "pluginnotfound": [0, 1],
+        "point": [0, 1, 5, 6],
+        "pool": 0,
+        "pop": [1, 6],
+        "popul": [0, 6],
+        "popular": 6,
+        "port": 0,
+        "portalock": 0,
+        "portion": [1, 6],
+        "posit": 1,
+        "possibl": [0, 5, 6],
+        "possibli": 0,
+        "potenti": [1, 5, 6],
+        "pre": [1, 5],
+        "prefer": 0,
+        "prefix": [0, 4, 6],
+        "presenc": 1,
+        "present": [0, 1, 5, 6],
+        "preserv": [1, 5],
+        "prevent": [0, 1, 6],
+        "previou": [0, 1, 2, 4, 6],
+        "previous": [1, 2],
+        "primari": 2,
+        "print": 5,
+        "prior": [0, 1],
+        "probabl": 5,
+        "problem": 1,
+        "problemat": 0,
+        "proce": [0, 1, 2, 4, 6],
+        "process": [0, 1, 2, 5, 6],
+        "produc": [0, 1, 6],
+        "product": [1, 6],
+        "project": [1, 4],
+        "promptli": [0, 6],
+        "propag": [0, 1],
+        "properli": 6,
+        "properti": 0,
+        "protect": 0,
+        "protocol": [0, 1],
+        "provid": [0, 1, 2, 4, 6],
+        "proxi": [5, 6],
+        "proxybackend": [0, 1, 5, 6],
+        "publish": 3,
+        "pull": [0, 1, 5, 6],
+        "pullreq": 1,
+        "pure": [0, 1],
+        "purpos": [1, 2, 5],
+        "push": [0, 5],
+        "put": [2, 6],
+        "py": [0, 1, 6],
+        "py2": 1,
+        "py3": 1,
+        "py3k": 1,
+        "pylibmc": [0, 1, 2, 5],
+        "pylibmcbackend": 0,
+        "pymemcach": [0, 1],
+        "pymemcachebackend": [0, 1],
+        "pypa": 1,
+        "pypi": [1, 3],
+        "pyproject": 1,
+        "pytest": 1,
+        "python": [0, 1, 2, 3, 5, 6],
+        "python3": 1,
+        "queri": [0, 5, 6],
+        "queue": [0, 6],
+        "rais": [0, 1, 2, 5, 6],
+        "ralph": 1,
+        "rather": [0, 2, 6],
+        "raw": 5,
+        "rbac": 1,
+        "re": [0, 1, 2, 5, 6],
+        "reach": [0, 2, 6],
+        "read": 0,
+        "reader": [0, 1],
+        "readi": [0, 6],
+        "readthedoc": 0,
+        "readwrite_lock": [0, 1],
+        "readwritemutex": [0, 1],
+        "real": 6,
+        "receiv": [0, 1, 6],
+        "recent": 3,
+        "recip": [1, 2, 4],
+        "recod": 5,
+        "recogn": [0, 1, 6],
+        "recommend": [0, 6],
+        "record": 5,
+        "recreat": [0, 6],
+        "recv": 0,
+        "redi": [1, 4, 6],
+        "redis_clust": 0,
+        "redis_expiration_tim": 0,
+        "redis_sentinel": 0,
+        "redis_sentinel_1": 0,
+        "redis_sentinel_2": 0,
+        "redisbackend": [0, 1],
+        "redisclust": 0,
+        "redisclusterbackend": [0, 1],
+        "redissentinelbackend": [0, 1],
+        "reduc": 0,
+        "redundantli": 6,
+        "reentrant": 1,
+        "refer": [0, 1, 2, 4],
+        "referenc": 0,
+        "reflect": 0,
+        "refresh": [0, 1, 5, 6],
+        "regardless": [0, 6],
+        "regen": 0,
+        "regener": [0, 1, 2, 6],
+        "region": [1, 4, 5],
+        "region_invalid": [0, 6],
+        "regionalreadyconfigur": 0,
+        "regioninvalidationstrategi": [0, 1, 6],
+        "regionnotconfigur": 0,
+        "regist": [0, 1, 6],
+        "register_backend": 6,
+        "registri": [0, 5],
+        "regress": 1,
+        "regular": 0,
+        "rel": [0, 6],
+        "relat": 4,
+        "releas": [0, 1, 3, 6],
+        "release_read_lock": 0,
+        "release_write_lock": 0,
+        "relev": [0, 6],
+        "reli": [1, 2],
+        "relianc": 1,
+        "remain": [0, 1],
+        "rememb": [0, 6],
+        "remot": 0,
+        "remov": [0, 1, 2, 6],
+        "repair": 1,
+        "replac": [0, 1, 5, 6],
+        "replace_existing_backend": [0, 1, 6],
+        "report": [0, 3, 6],
+        "repositori": 1,
+        "repres": [0, 6],
+        "request": [0, 1, 6],
+        "requir": [0, 1, 2, 4, 6],
+        "reserv": 2,
+        "resolv": [0, 1, 6],
+        "resourc": [2, 4],
+        "respect": 1,
+        "respons": [0, 6],
+        "restor": 1,
+        "result": [0, 1, 5, 6],
+        "ret": 0,
+        "retir": 1,
+        "retri": [0, 1, 6],
+        "retriev": [0, 1, 2, 6],
+        "retrieve_resourc": 2,
+        "retry_attempt": [0, 1],
+        "retry_count": 6,
+        "retry_delai": 0,
+        "retry_for": 0,
+        "retry_proxi": 6,
+        "retry_timeout": 1,
+        "retrydeleteproxi": 6,
+        "return": [0, 1, 2, 5, 6],
+        "revert": 1,
+        "rework": 1,
+        "rewritten": 1,
+        "roll": 1,
+        "root": 1,
+        "rosebaugh": 1,
+        "rougher": 6,
+        "round": 2,
+        "routin": 1,
+        "rudimentari": 4,
+        "run": [0, 1, 6],
+        "runner": [0, 1, 6],
+        "runtim": 6,
+        "rutherfurd": 1,
+        "rw": [0, 1],
+        "rw_lockfil": 0,
+        "ryan": 1,
+        "safe": [0, 2, 6],
+        "same": [0, 1, 2, 6],
+        "sasl": 0,
+        "sat": 1,
+        "sauerwein": 1,
+        "sauliu": 1,
+        "scanner": 1,
+        "scenario": 1,
+        "scene": 6,
+        "scheme": [1, 2, 5],
+        "scope": [0, 1],
+        "scoped_sess": 5,
+        "scott": 0,
+        "script": 1,
+        "search": 4,
+        "second": [0, 1, 2, 6],
+        "section": [0, 2, 6],
+        "secur": 0,
+        "see": [0, 1, 2, 6],
+        "select": [0, 4],
+        "self": [0, 1, 5, 6],
+        "semant": 1,
+        "semaphor": 0,
+        "send": [0, 1],
+        "sent": 5,
+        "sentinel": [0, 1],
+        "sentinel_kwarg": 0,
+        "sep": 1,
+        "separ": [0, 1, 2, 6],
+        "sequenc": [0, 5, 6],
+        "serd": 0,
+        "seri": [0, 1, 5],
+        "serial": [0, 1, 5, 6],
+        "serializ": 6,
+        "serializedreturntyp": 0,
+        "serv": 1,
+        "server": [0, 2, 6],
+        "servic": [0, 1, 2],
+        "service_nam": 0,
+        "session": 5,
+        "sessionmak": 5,
+        "set": [0, 1, 5, 6],
+        "set_argu": 0,
+        "set_multi": [0, 1, 5],
+        "set_paramet": [0, 1],
+        "set_seri": 0,
+        "set_serialized_multi": 0,
+        "setlevel": 6,
+        "setup": [0, 1, 2, 6],
+        "setuptool": [1, 6],
+        "sever": [0, 1],
+        "sha1": [0, 2, 6],
+        "sha1_mangle_kei": [0, 1, 6],
+        "share": [1, 2, 6],
+        "sheldon": 1,
+        "short": 2,
+        "should": [0, 1, 3, 6],
+        "should_cache_fn": [0, 1, 6],
+        "sign": 1,
+        "signatur": [0, 1],
+        "significantli": 0,
+        "similar": [0, 1, 3, 6],
+        "simon": 1,
+        "simpl": [0, 1, 2, 5, 6],
+        "simpli": 5,
+        "simplifi": 1,
+        "simultan": [0, 6],
+        "sinc": [0, 5, 6],
+        "singaravelan": 1,
+        "singl": [0, 1, 2, 4, 6],
+        "singleton": 0,
+        "situat": 1,
+        "size": [0, 5],
+        "skip": [0, 6],
+        "sleep": 0,
+        "slow_databas": 2,
+        "slower": 1,
+        "small": [1, 6],
+        "smaller": 5,
+        "so": [0, 1, 2, 5, 6],
+        "sobrinho": 1,
+        "socket": [0, 1],
+        "socket_connect_timeout": [0, 1],
+        "socket_keepal": [0, 1],
+        "socket_keepalive_opt": [0, 1],
+        "socket_timeout": [0, 1],
+        "soft": [0, 1],
+        "some": [0, 1, 2, 4, 5, 6],
+        "some_creation_funct": 2,
+        "some_databas": 6,
+        "some_kei": 2,
+        "somedatabas": [0, 6],
+        "somekei": [0, 6],
+        "somemethod": [0, 6],
+        "someregion": [0, 6],
+        "something_new": 5,
+        "somevalu": 6,
+        "somewher": 0,
+        "sourc": [0, 1, 2, 6],
+        "space": 6,
+        "special": 1,
+        "specif": [0, 1, 4, 6],
+        "specifi": [0, 1, 5, 6],
+        "speed": 0,
+        "spent": 6,
+        "sqlalchemi": [1, 3, 5],
+        "ssl": 0,
+        "ssl_ca_cert": 0,
+        "ssl_certfil": 0,
+        "stack": 0,
+        "stale": [0, 2, 6],
+        "standard": 0,
+        "start": [0, 5, 6],
+        "startup": 0,
+        "startup_nod": 0,
+        "state": [0, 1],
+        "statu": 3,
+        "stegmann": 1,
+        "step": [0, 1, 6],
+        "stevedor": 1,
+        "still": [0, 1, 2, 5, 6],
+        "storag": [1, 5, 6],
+        "store": [0, 1, 2, 5, 6],
+        "str": [0, 1, 5, 6],
+        "straight": 1,
+        "strategi": [0, 1, 2, 6],
+        "stream": 0,
+        "strictredi": [0, 1],
+        "string": [0, 1, 6],
+        "strongli": 0,
+        "structur": [0, 1, 4, 6],
+        "stuff": 2,
+        "st\u00e9phane": 1,
+        "subclass": [0, 1, 6],
+        "subject": 1,
+        "submit": 0,
+        "subsequ": [0, 1, 6],
+        "subset": 0,
+        "subsitut": 1,
+        "substitut": [0, 6],
+        "subsystem": 4,
+        "subtract": 0,
+        "succeed": 0,
+        "success": [0, 1],
+        "successfulli": [0, 2, 6],
+        "suffix": 0,
+        "suit": [0, 1],
+        "suitabl": [0, 6],
+        "sun": 1,
+        "super": 6,
+        "supersed": [0, 6],
+        "suppli": [0, 6],
+        "support": [0, 1, 6],
+        "suppos": [1, 5],
+        "sure": [0, 6],
+        "switch": 1,
+        "sy": 6,
+        "symbol": [1, 2],
+        "symlink": 2,
+        "synchron": [0, 2],
+        "syncreaderdogpil": 1,
+        "syntax": 1,
+        "system": [0, 1, 2, 5, 6],
+        "t": [0, 1, 2, 5, 6],
+        "tag": 0,
+        "takashi": 1,
+        "take": [0, 1, 6],
+        "talk": [0, 6],
+        "target": [0, 5, 6],
+        "task": [0, 6],
+        "tcp": 0,
+        "tcp_nodelai": 0,
+        "techniqu": 5,
+        "templat": [0, 1, 5],
+        "templatelookup": 0,
+        "term": [0, 6],
+        "test": [0, 1, 6],
+        "text": 0,
+        "than": [0, 2, 5, 6],
+        "thank": 1,
+        "the_resourc": 2,
+        "thei": [0, 1, 2, 6],
+        "them": [0, 1, 5],
+        "themselv": 1,
+        "therebi": 1,
+        "therefor": [0, 1, 6],
+        "thi": [0, 1, 2, 3, 4, 5, 6],
+        "thing": [1, 6],
+        "third": [0, 5],
+        "those": [0, 1, 4, 5, 6],
+        "though": [0, 1, 6],
+        "thread": [0, 1, 2, 4, 5, 6],
+        "thread_local_lock": [0, 1],
+        "threadmappedpool": 2,
+        "threadsaf": [0, 2],
+        "three": [0, 5],
+        "threshold": 0,
+        "throttl": 0,
+        "through": [2, 5],
+        "thrown": [0, 1],
+        "thu": [0, 1, 2, 6],
+        "tiger": 0,
+        "tim": 1,
+        "time": [0, 1, 2, 6],
+        "timedelta": [0, 1, 6],
+        "timeout": [0, 1],
+        "timestamp": [0, 1, 6],
+        "tl": [0, 1],
+        "tls_context": 0,
+        "tmp": 2,
+        "to_list": 1,
+        "to_str": [0, 1, 6],
+        "tobia": 1,
+        "togeth": [0, 6],
+        "token": [0, 6],
+        "toml": 1,
+        "tool": [0, 1, 3, 6],
+        "top": 4,
+        "total": 0,
+        "total_second": 1,
+        "toward": [0, 1],
+        "tox": 1,
+        "track": [0, 2, 5],
+        "tracker": 3,
+        "transform": 5,
+        "translat": 5,
+        "treat": 0,
+        "tri": 0,
+        "trip": 2,
+        "true": [0, 1, 5, 6],
+        "try": [0, 5, 6],
+        "tue": 1,
+        "tup": 2,
+        "tupl": [0, 2, 6],
+        "turn": [1, 6],
+        "tweak": 4,
+        "twice": 2,
+        "two": [0, 2, 4, 5, 6],
+        "type": [0, 1, 6],
+        "typeerror": 1,
+        "typic": [0, 5, 6],
+        "t\u00fcfek\u00e7i": 1,
+        "u": [1, 2, 6],
+        "ultim": [0, 1, 2, 6],
+        "unabl": [0, 6],
+        "unaffect": 1,
+        "uncondition": [0, 6],
+        "unconfigur": 1,
+        "under": [0, 1, 5, 6],
+        "underli": [0, 6],
+        "underneath": [0, 6],
+        "understood": 0,
+        "undesir": 0,
+        "unencod": 5,
+        "unexpect": 1,
+        "unicod": [0, 1, 6],
+        "uninstanti": 6,
+        "uniqu": [0, 2, 5],
+        "unit": 1,
+        "univers": 1,
+        "unix": [0, 1, 2],
+        "unless": [0, 2, 6],
+        "unlik": [0, 2],
+        "unlimit": 0,
+        "unnecessari": [0, 1],
+        "unnecessarili": 1,
+        "unpackb": 5,
+        "unsupport": 1,
+        "until": [0, 1, 2, 4, 5, 6],
+        "up": 1,
+        "updat": [0, 1, 4, 6],
+        "upon": [0, 1, 2, 6],
+        "upstream": 0,
+        "url": [0, 1, 5, 6],
+        "us": [0, 1, 4, 5],
+        "usabl": 6,
+        "usag": [0, 1, 4],
+        "use_bin_typ": 5,
+        "user": [0, 1, 2, 4, 5, 6],
+        "user_fn_on": 5,
+        "user_fn_one_": 5,
+        "user_fn_thre": 5,
+        "user_fn_three_": 5,
+        "user_fn_two": 5,
+        "user_fn_two_": 5,
+        "user_id": [5, 6],
+        "user_kei": 5,
+        "usernam": [0, 1],
+        "usual": [1, 2, 6],
+        "utf": 5,
+        "util": [1, 4],
+        "v": [1, 5],
+        "valid": 0,
+        "validationerror": 0,
+        "valu": [0, 1, 2, 5, 6],
+        "value1": 0,
+        "value2": 0,
+        "value3": 0,
+        "value_and_created_fn": 0,
+        "value_decod": 5,
+        "value_encod": 5,
+        "value_plus_tim": 2,
+        "value_vers": 0,
+        "valuepayload": [0, 1],
+        "vanasco": 1,
+        "variabl": 1,
+        "variant": [0, 1, 5],
+        "varieti": 4,
+        "variou": [0, 2],
+        "vendor": 1,
+        "verbos": 6,
+        "veri": [1, 4],
+        "version": [0, 1, 2, 3, 4, 6],
+        "versu": [0, 6],
+        "via": [0, 1, 2, 5, 6],
+        "viico": 1,
+        "visit": 0,
+        "volum": [1, 4],
+        "wa": [0, 1, 2, 5, 6],
+        "wai": [0, 1, 5, 6],
+        "wait": [0, 1, 6],
+        "want": [0, 2, 5, 6],
+        "warn": 1,
+        "was_hard_invalid": 0,
+        "was_soft_invalid": 0,
+        "wasn": 1,
+        "we": [0, 2, 5, 6],
+        "wed": 1,
+        "week": [0, 6],
+        "well": [0, 1, 2, 5, 6],
+        "were": [0, 1, 6],
+        "what": [0, 1, 2],
+        "whatev": [0, 6],
+        "wheel": 1,
+        "when": [0, 1, 2, 5, 6],
+        "whenev": [0, 6],
+        "where": [0, 1, 2, 6],
+        "wherebi": 1,
+        "whether": [0, 1, 6],
+        "which": [0, 1, 2, 4, 5, 6],
+        "while": [0, 1, 4, 5, 6],
+        "whole": [0, 1],
+        "whose": 0,
+        "wichert": 1,
+        "wide": 1,
+        "window": [0, 1],
+        "wish": 0,
+        "with_stat": 1,
+        "within": [0, 1, 5, 6],
+        "without": [0, 1, 2, 6],
+        "won": [0, 2, 6],
+        "work": [0, 1, 2, 5],
+        "worker": 6,
+        "would": [0, 1, 5, 6],
+        "wrap": [0, 1, 5, 6],
+        "wrapper": 0,
+        "write": [0, 1, 6],
+        "writer": [0, 5, 6],
+        "written": 6,
+        "wrong": 1,
+        "x": [0, 1, 6],
+        "y": [0, 6],
+        "yank": 1,
+        "yet": [0, 1, 6],
+        "you": [0, 2, 5, 6],
+        "your": [0, 2, 5],
+        "yu": 1,
+        "zero": 1,
+        "zip": 0,
+        "zoomorph": 1,
+        "\u0142ukasz": 1
     },
+    "titles": ["API", "Changelog", "dogpile Core", "Front Matter", "Welcome to dogpile.cache\u2019s documentation!", "Recipes", "Usage Guide"],
     "titleterms": {
-        "api": [0, 2],
-        "region": [0, 6],
-        "backend": [0, 6],
-        "memori": 0,
-        "memcach": 0,
-        "redi": [0, 5],
-        "file": [0, 2],
-        "proxi": 0,
-        "null": 0,
-        "except": 0,
-        "plugin": 0,
-        "mako": 0,
-        "integr": 0,
-        "util": 0,
-        "dogpil": [0, 2, 4],
-        "core": [0, 2],
-        "changelog": 1,
+        "": 4,
+        "0": 1,
         "1": 1,
-        "3": 1,
         "2": 1,
-        "usecas": 1,
-        "0": 1,
-        "featur": 1,
-        "misc": 1,
-        "bug": [1, 3],
-        "8": 1,
-        "7": 1,
-        "6": 1,
-        "5": 1,
+        "3": 1,
         "4": 1,
+        "5": 1,
+        "6": 1,
+        "7": 1,
+        "8": 1,
         "9": 1,
-        "do": 2,
-        "i": 2,
-        "need": 2,
-        "learn": 2,
-        "directli": 2,
-        "rudimentari": [2, 6],
-        "usag": [2, 6],
-        "exampl": 2,
-        "us": [2, 6],
+        "A": 5,
+        "all": 5,
+        "anoth": 5,
+        "api": [0, 2],
+        "asynchron": 5,
+        "backend": [0, 6],
+        "behavior": 6,
+        "bug": [1, 3],
         "cach": [2, 4],
+        "chang": 6,
+        "changelog": 1,
+        "configur": 6,
+        "core": [0, 2],
+        "creat": 6,
+        "data": 5,
+        "decod": 5,
+        "directli": 2,
         "distribut": 2,
-        "lock": 2,
+        "do": 2,
+        "document": 4,
+        "dogpil": [0, 2, 4],
+        "encod": 5,
+        "event": 5,
+        "exampl": 2,
+        "except": 0,
+        "featur": 1,
+        "file": [0, 2],
+        "format": 5,
         "front": 3,
-        "matter": 3,
-        "project": 3,
+        "group": 5,
+        "guid": 6,
         "homepag": 3,
-        "instal": 3,
-        "welcom": 4,
-        "": 4,
-        "document": 4,
+        "i": 2,
         "indic": 4,
-        "tabl": 4,
-        "recip": 5,
+        "instal": 3,
+        "integr": 0,
         "invalid": 5,
-        "group": 5,
-        "relat": 5,
         "kei": 5,
-        "asynchron": 5,
-        "data": 5,
-        "updat": 5,
-        "orm": 5,
-        "event": 5,
-        "prefix": 5,
-        "all": 5,
-        "encod": 5,
-        "decod": 5,
-        "anoth": 5,
-        "format": 5,
-        "A": 5,
+        "learn": 2,
+        "lock": 2,
+        "log": 6,
+        "mako": 0,
+        "matter": 3,
+        "memcach": 0,
+        "memori": 0,
+        "misc": 1,
+        "need": 2,
         "note": 5,
-        "guid": 6,
+        "null": 0,
+        "orm": 5,
         "overview": 6,
+        "plugin": 0,
+        "prefix": 5,
+        "project": 3,
+        "proxi": 0,
         "pylibmc": 6,
-        "configur": 6,
-        "creat": 6,
-        "chang": 6,
-        "behavior": 6,
-        "log": 6
-    },
-    "envversion": {
-        "sphinx.domains.c": 3,
-        "sphinx.domains.changeset": 1,
-        "sphinx.domains.citation": 1,
-        "sphinx.domains.cpp": 9,
-        "sphinx.domains.index": 1,
-        "sphinx.domains.javascript": 3,
-        "sphinx.domains.math": 2,
-        "sphinx.domains.python": 4,
-        "sphinx.domains.rst": 2,
-        "sphinx.domains.std": 2,
-        "sphinx.ext.intersphinx": 1,
-        "sphinx": 60
-    },
-    "alltitles": {
-        "API": [
-            [0, "api"]
-        ],
-        "Region": [
-            [0, "module-dogpile.cache.region"]
-        ],
-        "Backend API": [
-            [0, "backend-api"]
-        ],
-        "Backends": [
-            [0, "module-dogpile.cache.backends.memory"]
-        ],
-        "Memory Backends": [
-            [0, "memory-backends"]
-        ],
-        "Memcached Backends": [
-            [0, "memcached-backends"]
-        ],
-        "Redis Backends": [
-            [0, "redis-backends"]
-        ],
-        "File Backends": [
-            [0, "file-backends"]
-        ],
-        "Proxy Backends": [
-            [0, "proxy-backends"]
-        ],
-        "Null Backend": [
-            [0, "null-backend"]
-        ],
-        "Exceptions": [
-            [0, "module-dogpile.cache.exception"]
-        ],
-        "Plugins": [
-            [0, "module-dogpile.cache.plugins.mako_cache"]
-        ],
-        "Mako Integration": [
-            [0, "mako-integration"]
-        ],
-        "Utilities": [
-            [0, "utilities"]
-        ],
-        "dogpile Core": [
-            [0, "dogpile-core"],
-            [2, "dogpile-core"]
-        ],
-        "Changelog": [
-            [1, "changelog"]
-        ],
-        "1.3.2": [
-            [1, "change-1.3.2"]
-        ],
-        "usecase": [
-            [1, "change-1.3.2-usecase"],
-            [1, "change-1.3.1-usecase"],
-            [1, "change-1.1.7-usecase"],
-            [1, "change-1.1.6-usecase"],
-            [1, "change-1.1.5-usecase"],
-            [1, "change-1.1.4-usecase"]
-        ],
-        "1.3.1": [
-            [1, "change-1.3.1"]
-        ],
-        "1.3.0": [
-            [1, "change-1.3.0"]
-        ],
-        "feature": [
-            [1, "change-1.3.0-feature"],
-            [1, "change-1.2.0-feature"],
-            [1, "change-1.1.2-feature"],
-            [1, "change-1.1.0-feature"],
-            [1, "change-1.0.2-feature"],
-            [1, "change-1.0.0-feature"],
-            [1, "change-0.9.0-feature"],
-            [1, "change-0.6.6-feature"],
-            [1, "change-0.6.3-feature"],
-            [1, "change-0.6.2-feature"],
-            [1, "change-0.6.0-feature"],
-            [1, "change-0.5.7-feature"],
-            [1, "change-0.5.6-feature"],
-            [1, "change-0.5.5-feature"],
-            [1, "change-0.5.4-feature"],
-            [1, "change-0.5.3-feature"],
-            [1, "change-0.5.2-feature"],
-            [1, "change-0.5.1-feature"],
-            [1, "change-0.5.0-feature"],
-            [1, "change-0.4.3-feature"],
-            [1, "change-0.4.2-feature"],
-            [1, "change-0.4.1-feature"],
-            [1, "change-0.3.0-feature"]
-        ],
-        "misc": [
-            [1, "change-1.3.0-misc"],
-            [1, "change-1.1.0-misc"],
-            [1, "change-1.0.0-misc"],
-            [1, "change-0.5.0-misc"]
-        ],
-        "1.2.2": [
-            [1, "change-1.2.2"]
-        ],
-        "bug": [
-            [1, "change-1.2.2-bug"],
-            [1, "change-1.2.1-bug"],
-            [1, "change-1.1.8-bug"],
-            [1, "change-1.1.6-bug"],
-            [1, "change-1.1.4-bug"],
-            [1, "change-1.1.3-bug"],
-            [1, "change-1.1.1-bug"],
-            [1, "change-1.0.2-bug"],
-            [1, "change-1.0.1-bug"],
-            [1, "change-0.9.2-bug"],
-            [1, "change-0.9.1-bug"],
-            [1, "change-0.8.0-bug"],
-            [1, "change-0.7.1-bug"],
-            [1, "change-0.7.0-bug"],
-            [1, "change-0.6.7-bug"],
-            [1, "change-0.6.6-bug"],
-            [1, "change-0.6.5-bug"],
-            [1, "change-0.6.4-bug"],
-            [1, "change-0.6.2-bug"],
-            [1, "change-0.6.1-bug"],
-            [1, "change-0.6.0-bug"],
-            [1, "change-0.5.7-bug"],
-            [1, "change-0.5.5-bug"],
-            [1, "change-0.5.4-bug"],
-            [1, "change-0.5.3-bug"],
-            [1, "change-0.5.2-bug"],
-            [1, "change-0.5.1-bug"],
-            [1, "change-0.5.0-bug"],
-            [1, "change-0.4.3-bug"],
-            [1, "change-0.4.1-bug"],
-            [1, "change-0.4.0-bug"],
-            [1, "change-0.3.1-bug"],
-            [1, "change-0.3.0-bug"]
-        ],
-        "1.2.1": [
-            [1, "change-1.2.1"]
-        ],
-        "1.2.0": [
-            [1, "change-1.2.0"]
-        ],
-        "1.1.8": [
-            [1, "change-1.1.8"]
-        ],
-        "1.1.7": [
-            [1, "change-1.1.7"]
-        ],
-        "1.1.6": [
-            [1, "change-1.1.6"]
-        ],
-        "1.1.5": [
-            [1, "change-1.1.5"]
-        ],
-        "1.1.4": [
-            [1, "change-1.1.4"]
-        ],
-        "1.1.3": [
-            [1, "change-1.1.3"]
-        ],
-        "1.1.2": [
-            [1, "change-1.1.2"]
-        ],
-        "1.1.1": [
-            [1, "change-1.1.1"]
-        ],
-        "1.1.0": [
-            [1, "change-1.1.0"]
-        ],
-        "1.0.2": [
-            [1, "change-1.0.2"]
-        ],
-        "1.0.1": [
-            [1, "change-1.0.1"]
-        ],
-        "1.0.0": [
-            [1, "change-1.0.0"]
-        ],
-        "0.9.2": [
-            [1, "change-0.9.2"]
-        ],
-        "0.9.1": [
-            [1, "change-0.9.1"]
-        ],
-        "0.9.0": [
-            [1, "change-0.9.0"]
-        ],
-        "0.8.0": [
-            [1, "change-0.8.0"]
-        ],
-        "0.7.1": [
-            [1, "change-0.7.1"]
-        ],
-        "0.7.0": [
-            [1, "change-0.7.0"]
-        ],
-        "0.6.8": [
-            [1, "change-0.6.8"]
-        ],
-        "0.6.7": [
-            [1, "change-0.6.7"]
-        ],
-        "0.6.6": [
-            [1, "change-0.6.6"]
-        ],
-        "0.6.5": [
-            [1, "change-0.6.5"]
-        ],
-        "0.6.4": [
-            [1, "change-0.6.4"]
-        ],
-        "0.6.3": [
-            [1, "change-0.6.3"]
-        ],
-        "0.6.2": [
-            [1, "change-0.6.2"]
-        ],
-        "0.6.1": [
-            [1, "change-0.6.1"]
-        ],
-        "0.6.0": [
-            [1, "change-0.6.0"]
-        ],
-        "0.5.7": [
-            [1, "change-0.5.7"]
-        ],
-        "0.5.6": [
-            [1, "change-0.5.6"]
-        ],
-        "0.5.5": [
-            [1, "change-0.5.5"]
-        ],
-        "0.5.4": [
-            [1, "change-0.5.4"]
-        ],
-        "0.5.3": [
-            [1, "change-0.5.3"]
-        ],
-        "0.5.2": [
-            [1, "change-0.5.2"]
-        ],
-        "0.5.1": [
-            [1, "change-0.5.1"]
-        ],
-        "0.5.0": [
-            [1, "change-0.5.0"]
-        ],
-        "0.4.3": [
-            [1, "change-0.4.3"]
-        ],
-        "0.4.2": [
-            [1, "change-0.4.2"]
-        ],
-        "0.4.1": [
-            [1, "change-0.4.1"]
-        ],
-        "0.4.0": [
-            [1, "change-0.4.0"]
-        ],
-        "0.3.1": [
-            [1, "change-0.3.1"]
-        ],
-        "0.3.0": [
-            [1, "change-0.3.0"]
-        ],
-        "0.2.4": [
-            [1, "change-0.2.4"]
-        ],
-        "0.2.3": [
-            [1, "change-0.2.3"]
-        ],
-        "0.2.2": [
-            [1, "change-0.2.2"]
-        ],
-        "0.2.1": [
-            [1, "change-0.2.1"]
-        ],
-        "0.2.0": [
-            [1, "change-0.2.0"]
-        ],
-        "0.1.1": [
-            [1, "change-0.1.1"]
-        ],
-        "0.1.0": [
-            [1, "change-0.1.0"]
-        ],
-        "Do I Need to Learn the dogpile Core API Directly?": [
-            [2, "do-i-need-to-learn-the-dogpile-core-api-directly"]
-        ],
-        "Rudimentary Usage": [
-            [2, "rudimentary-usage"],
-            [6, "rudimentary-usage"]
-        ],
-        "Example: Using dogpile directly for Caching": [
-            [2, "example-using-dogpile-directly-for-caching"]
-        ],
-        "Using a File or Distributed Lock with Dogpile": [
-            [2, "using-a-file-or-distributed-lock-with-dogpile"]
-        ],
-        "Front Matter": [
-            [3, "front-matter"]
-        ],
-        "Project Homepage": [
-            [3, "project-homepage"]
-        ],
-        "Installation": [
-            [3, "installation"]
-        ],
-        "Bugs": [
-            [3, "bugs"]
-        ],
-        "Welcome to dogpile.cache\u2019s documentation!": [
-            [4, "welcome-to-dogpile-cache-s-documentation"]
-        ],
-        "Indices and tables": [
-            [4, "indices-and-tables"]
-        ],
-        "Recipes": [
-            [5, "recipes"]
-        ],
-        "Invalidating a group of related keys": [
-            [5, "invalidating-a-group-of-related-keys"]
-        ],
-        "Asynchronous Data Updates with ORM Events": [
-            [5, "asynchronous-data-updates-with-orm-events"]
-        ],
-        "Prefixing all keys in Redis": [
-            [5, "prefixing-all-keys-in-redis"]
-        ],
-        "Encoding/Decoding data into another format": [
-            [5, "encoding-decoding-data-into-another-format"]
-        ],
-        "A Note on Data Encoding": [
-            [5, null]
-        ],
-        "Usage Guide": [
-            [6, "usage-guide"]
-        ],
-        "Overview": [
-            [6, "overview"]
-        ],
-        "pylibmc": [
-            [6, null]
-        ],
-        "Region Configuration": [
-            [6, "region-configuration"]
-        ],
-        "Using a Region": [
-            [6, "using-a-region"]
-        ],
-        "Creating Backends": [
-            [6, "creating-backends"]
-        ],
-        "Changing Backend Behavior": [
-            [6, "changing-backend-behavior"]
-        ],
-        "Configuring Logging": [
-            [6, "configuring-logging"]
-        ]
-    },
-    "indexentries": {
-        "abstractfilelock (class in dogpile.cache.backends.file)": [
-            [0, "dogpile.cache.backends.file.AbstractFileLock"]
-        ],
-        "bmemcachedbackend (class in dogpile.cache.backends.memcached)": [
-            [0, "dogpile.cache.backends.memcached.BMemcachedBackend"]
-        ],
-        "backendformatted (in module dogpile.cache.api)": [
-            [0, "dogpile.cache.api.BackendFormatted"]
-        ],
-        "backendsettype (in module dogpile.cache.api)": [
-            [0, "dogpile.cache.api.BackendSetType"]
-        ],
-        "bytesbackend (class in dogpile.cache.api)": [
-            [0, "dogpile.cache.api.BytesBackend"]
-        ],
-        "cachebackend (class in dogpile.cache.api)": [
-            [0, "dogpile.cache.api.CacheBackend"]
-        ],
-        "cachemutex (class in dogpile.cache.api)": [
-            [0, "dogpile.cache.api.CacheMutex"]
-        ],
-        "cacheregion (class in dogpile.cache.region)": [
-            [0, "dogpile.cache.region.CacheRegion"]
-        ],
-        "cachereturntype (in module dogpile.cache.api)": [
-            [0, "dogpile.cache.api.CacheReturnType"]
-        ],
-        "cachedvalue (class in dogpile.cache.api)": [
-            [0, "dogpile.cache.api.CachedValue"]
-        ],
-        "cantdeserializeexception": [
-            [0, "dogpile.cache.api.CantDeserializeException"]
-        ],
-        "dbmbackend (class in dogpile.cache.backends.file)": [
-            [0, "dogpile.cache.backends.file.DBMBackend"]
-        ],
-        "defaultinvalidationstrategy (class in dogpile.cache.region)": [
-            [0, "dogpile.cache.region.DefaultInvalidationStrategy"]
-        ],
-        "dogpilecacheexception": [
-            [0, "dogpile.cache.exception.DogpileCacheException"]
-        ],
-        "filelock (class in dogpile.cache.backends.file)": [
-            [0, "dogpile.cache.backends.file.FileLock"]
-        ],
-        "genericmemcachedbackend (class in dogpile.cache.backends.memcached)": [
-            [0, "dogpile.cache.backends.memcached.GenericMemcachedBackend"]
-        ],
-        "keytype (in module dogpile.cache.api)": [
-            [0, "dogpile.cache.api.KeyType"]
-        ],
-        "lock (class in dogpile)": [
-            [0, "dogpile.Lock"]
-        ],
-        "makoplugin (class in dogpile.cache.plugins.mako_cache)": [
-            [0, "dogpile.cache.plugins.mako_cache.MakoPlugin"]
-        ],
-        "memcachedbackend (class in dogpile.cache.backends.memcached)": [
-            [0, "dogpile.cache.backends.memcached.MemcachedBackend"]
-        ],
-        "memcachedlock (class in dogpile.cache.backends.memcached)": [
-            [0, "dogpile.cache.backends.memcached.MemcachedLock"]
-        ],
-        "memorybackend (class in dogpile.cache.backends.memory)": [
-            [0, "dogpile.cache.backends.memory.MemoryBackend"]
-        ],
-        "memorypicklebackend (class in dogpile.cache.backends.memory)": [
-            [0, "dogpile.cache.backends.memory.MemoryPickleBackend"]
-        ],
-        "no_value (in module dogpile.cache.api)": [
-            [0, "dogpile.cache.api.NO_VALUE"]
-        ],
-        "nameregistry (class in dogpile.util)": [
-            [0, "dogpile.util.NameRegistry"]
-        ],
-        "needregenerationexception (class in dogpile)": [
-            [0, "dogpile.NeedRegenerationException"]
-        ],
-        "novalue (class in dogpile.cache.api)": [
-            [0, "dogpile.cache.api.NoValue"]
-        ],
-        "nullbackend (class in dogpile.cache.backends.null)": [
-            [0, "dogpile.cache.backends.null.NullBackend"]
-        ],
-        "pluginnotfound": [
-            [0, "dogpile.cache.exception.PluginNotFound"]
-        ],
-        "proxybackend (class in dogpile.cache.proxy)": [
-            [0, "dogpile.cache.proxy.ProxyBackend"]
-        ],
-        "pymemcachebackend (class in dogpile.cache.backends.memcached)": [
-            [0, "dogpile.cache.backends.memcached.PyMemcacheBackend"]
-        ],
-        "pylibmcbackend (class in dogpile.cache.backends.memcached)": [
-            [0, "dogpile.cache.backends.memcached.PylibmcBackend"]
-        ],
-        "readwritemutex (class in dogpile.util)": [
-            [0, "dogpile.util.ReadWriteMutex"]
-        ],
-        "redisbackend (class in dogpile.cache.backends.redis)": [
-            [0, "dogpile.cache.backends.redis.RedisBackend"]
-        ],
-        "redisclusterbackend (class in dogpile.cache.backends.redis)": [
-            [0, "dogpile.cache.backends.redis.RedisClusterBackend"]
-        ],
-        "redissentinelbackend (class in dogpile.cache.backends.redis)": [
-            [0, "dogpile.cache.backends.redis.RedisSentinelBackend"]
-        ],
-        "regionalreadyconfigured": [
-            [0, "dogpile.cache.exception.RegionAlreadyConfigured"]
-        ],
-        "regioninvalidationstrategy (class in dogpile.cache.region)": [
-            [0, "dogpile.cache.region.RegionInvalidationStrategy"]
-        ],
-        "regionnotconfigured": [
-            [0, "dogpile.cache.exception.RegionNotConfigured"]
-        ],
-        "serializedreturntype (in module dogpile.cache.api)": [
-            [0, "dogpile.cache.api.SerializedReturnType"]
-        ],
-        "validationerror": [
-            [0, "dogpile.cache.exception.ValidationError"]
-        ],
-        "valuepayload (in module dogpile.cache.api)": [
-            [0, "dogpile.cache.api.ValuePayload"]
-        ],
-        "acquire() (dogpile.cache.api.cachemutex method)": [
-            [0, "dogpile.cache.api.CacheMutex.acquire"]
-        ],
-        "acquire() (dogpile.cache.backends.file.abstractfilelock method)": [
-            [0, "dogpile.cache.backends.file.AbstractFileLock.acquire"]
-        ],
-        "acquire_read_lock() (dogpile.cache.backends.file.abstractfilelock method)": [
-            [0, "dogpile.cache.backends.file.AbstractFileLock.acquire_read_lock"]
-        ],
-        "acquire_read_lock() (dogpile.cache.backends.file.filelock method)": [
-            [0, "dogpile.cache.backends.file.FileLock.acquire_read_lock"]
-        ],
-        "acquire_read_lock() (dogpile.util.readwritemutex method)": [
-            [0, "dogpile.util.ReadWriteMutex.acquire_read_lock"]
-        ],
-        "acquire_write_lock() (dogpile.cache.backends.file.abstractfilelock method)": [
-            [0, "dogpile.cache.backends.file.AbstractFileLock.acquire_write_lock"]
-        ],
-        "acquire_write_lock() (dogpile.cache.backends.file.filelock method)": [
-            [0, "dogpile.cache.backends.file.FileLock.acquire_write_lock"]
-        ],
-        "acquire_write_lock() (dogpile.util.readwritemutex method)": [
-            [0, "dogpile.util.ReadWriteMutex.acquire_write_lock"]
-        ],
-        "actual_backend (dogpile.cache.region.cacheregion property)": [
-            [0, "dogpile.cache.region.CacheRegion.actual_backend"]
-        ],
-        "age (dogpile.cache.api.cachedvalue property)": [
-            [0, "dogpile.cache.api.CachedValue.age"]
-        ],
-        "cache_multi_on_arguments() (dogpile.cache.region.cacheregion method)": [
-            [0, "dogpile.cache.region.CacheRegion.cache_multi_on_arguments"]
-        ],
-        "cache_on_arguments() (dogpile.cache.region.cacheregion method)": [
-            [0, "dogpile.cache.region.CacheRegion.cache_on_arguments"]
-        ],
-        "cached_time (dogpile.cache.api.cachedvalue property)": [
-            [0, "dogpile.cache.api.CachedValue.cached_time"]
-        ],
-        "client (dogpile.cache.backends.memcached.genericmemcachedbackend property)": [
-            [0, "dogpile.cache.backends.memcached.GenericMemcachedBackend.client"]
-        ],
-        "configure() (dogpile.cache.region.cacheregion method)": [
-            [0, "dogpile.cache.region.CacheRegion.configure"]
-        ],
-        "configure_from_config() (dogpile.cache.region.cacheregion method)": [
-            [0, "dogpile.cache.region.CacheRegion.configure_from_config"]
-        ],
-        "delete() (dogpile.cache.api.cachebackend method)": [
-            [0, "dogpile.cache.api.CacheBackend.delete"]
-        ],
-        "delete() (dogpile.cache.backends.file.dbmbackend method)": [
-            [0, "dogpile.cache.backends.file.DBMBackend.delete"]
-        ],
-        "delete() (dogpile.cache.backends.memcached.genericmemcachedbackend method)": [
-            [0, "dogpile.cache.backends.memcached.GenericMemcachedBackend.delete"]
-        ],
-        "delete() (dogpile.cache.backends.memory.memorybackend method)": [
-            [0, "dogpile.cache.backends.memory.MemoryBackend.delete"]
-        ],
-        "delete() (dogpile.cache.backends.null.nullbackend method)": [
-            [0, "dogpile.cache.backends.null.NullBackend.delete"]
-        ],
-        "delete() (dogpile.cache.backends.redis.redisbackend method)": [
-            [0, "dogpile.cache.backends.redis.RedisBackend.delete"]
-        ],
-        "delete() (dogpile.cache.proxy.proxybackend method)": [
-            [0, "dogpile.cache.proxy.ProxyBackend.delete"]
-        ],
-        "delete() (dogpile.cache.region.cacheregion method)": [
-            [0, "dogpile.cache.region.CacheRegion.delete"]
-        ],
-        "delete_multi() (dogpile.cache.api.cachebackend method)": [
-            [0, "dogpile.cache.api.CacheBackend.delete_multi"]
-        ],
-        "delete_multi() (dogpile.cache.backends.file.dbmbackend method)": [
-            [0, "dogpile.cache.backends.file.DBMBackend.delete_multi"]
-        ],
-        "delete_multi() (dogpile.cache.backends.memcached.bmemcachedbackend method)": [
-            [0, "dogpile.cache.backends.memcached.BMemcachedBackend.delete_multi"]
-        ],
-        "delete_multi() (dogpile.cache.backends.memcached.genericmemcachedbackend method)": [
-            [0, "dogpile.cache.backends.memcached.GenericMemcachedBackend.delete_multi"]
-        ],
-        "delete_multi() (dogpile.cache.backends.memory.memorybackend method)": [
-            [0, "dogpile.cache.backends.memory.MemoryBackend.delete_multi"]
-        ],
-        "delete_multi() (dogpile.cache.backends.null.nullbackend method)": [
-            [0, "dogpile.cache.backends.null.NullBackend.delete_multi"]
-        ],
-        "delete_multi() (dogpile.cache.backends.redis.redisbackend method)": [
-            [0, "dogpile.cache.backends.redis.RedisBackend.delete_multi"]
-        ],
-        "delete_multi() (dogpile.cache.proxy.proxybackend method)": [
-            [0, "dogpile.cache.proxy.ProxyBackend.delete_multi"]
-        ],
-        "delete_multi() (dogpile.cache.region.cacheregion method)": [
-            [0, "dogpile.cache.region.CacheRegion.delete_multi"]
-        ],
-        "deserializer (dogpile.cache.api.cachebackend attribute)": [
-            [0, "dogpile.cache.api.CacheBackend.deserializer"]
-        ],
-        "deserializer (dogpile.cache.backends.memcached.genericmemcachedbackend attribute)": [
-            [0, "dogpile.cache.backends.memcached.GenericMemcachedBackend.deserializer"]
-        ],
-        "dogpile.cache.api": [
-            [0, "module-dogpile.cache.api"]
-        ],
-        "dogpile.cache.backends.file": [
-            [0, "module-dogpile.cache.backends.file"]
-        ],
-        "dogpile.cache.backends.memcached": [
-            [0, "module-dogpile.cache.backends.memcached"]
-        ],
-        "dogpile.cache.backends.memory": [
-            [0, "module-dogpile.cache.backends.memory"]
-        ],
-        "dogpile.cache.backends.null": [
-            [0, "module-dogpile.cache.backends.null"]
-        ],
-        "dogpile.cache.backends.redis": [
-            [0, "module-dogpile.cache.backends.redis"]
-        ],
-        "dogpile.cache.exception": [
-            [0, "module-dogpile.cache.exception"]
-        ],
-        "dogpile.cache.plugins.mako_cache": [
-            [0, "module-dogpile.cache.plugins.mako_cache"]
-        ],
-        "dogpile.cache.proxy": [
-            [0, "module-dogpile.cache.proxy"]
-        ],
-        "dogpile.cache.region": [
-            [0, "module-dogpile.cache.region"]
-        ],
-        "function_key_generator() (in module dogpile.cache.util)": [
-            [0, "dogpile.cache.util.function_key_generator"]
-        ],
-        "get() (dogpile.cache.api.cachebackend method)": [
-            [0, "dogpile.cache.api.CacheBackend.get"]
-        ],
-        "get() (dogpile.cache.backends.memcached.genericmemcachedbackend method)": [
-            [0, "dogpile.cache.backends.memcached.GenericMemcachedBackend.get"]
-        ],
-        "get() (dogpile.cache.backends.memory.memorybackend method)": [
-            [0, "dogpile.cache.backends.memory.MemoryBackend.get"]
-        ],
-        "get() (dogpile.cache.backends.null.nullbackend method)": [
-            [0, "dogpile.cache.backends.null.NullBackend.get"]
-        ],
-        "get() (dogpile.cache.plugins.mako_cache.makoplugin method)": [
-            [0, "dogpile.cache.plugins.mako_cache.MakoPlugin.get"]
-        ],
-        "get() (dogpile.cache.proxy.proxybackend method)": [
-            [0, "dogpile.cache.proxy.ProxyBackend.get"]
-        ],
-        "get() (dogpile.cache.region.cacheregion method)": [
-            [0, "dogpile.cache.region.CacheRegion.get"]
-        ],
-        "get() (dogpile.util.nameregistry method)": [
-            [0, "dogpile.util.NameRegistry.get"]
-        ],
-        "get_multi() (dogpile.cache.api.cachebackend method)": [
-            [0, "dogpile.cache.api.CacheBackend.get_multi"]
-        ],
-        "get_multi() (dogpile.cache.backends.memcached.genericmemcachedbackend method)": [
-            [0, "dogpile.cache.backends.memcached.GenericMemcachedBackend.get_multi"]
-        ],
-        "get_multi() (dogpile.cache.backends.memory.memorybackend method)": [
-            [0, "dogpile.cache.backends.memory.MemoryBackend.get_multi"]
-        ],
-        "get_multi() (dogpile.cache.backends.null.nullbackend method)": [
-            [0, "dogpile.cache.backends.null.NullBackend.get_multi"]
-        ],
-        "get_multi() (dogpile.cache.proxy.proxybackend method)": [
-            [0, "dogpile.cache.proxy.ProxyBackend.get_multi"]
-        ],
-        "get_multi() (dogpile.cache.region.cacheregion method)": [
-            [0, "dogpile.cache.region.CacheRegion.get_multi"]
-        ],
-        "get_mutex() (dogpile.cache.api.cachebackend method)": [
-            [0, "dogpile.cache.api.CacheBackend.get_mutex"]
-        ],
-        "get_mutex() (dogpile.cache.backends.file.dbmbackend method)": [
-            [0, "dogpile.cache.backends.file.DBMBackend.get_mutex"]
-        ],
-        "get_mutex() (dogpile.cache.backends.memcached.genericmemcachedbackend method)": [
-            [0, "dogpile.cache.backends.memcached.GenericMemcachedBackend.get_mutex"]
-        ],
-        "get_mutex() (dogpile.cache.backends.null.nullbackend method)": [
-            [0, "dogpile.cache.backends.null.NullBackend.get_mutex"]
-        ],
-        "get_mutex() (dogpile.cache.backends.redis.redisbackend method)": [
-            [0, "dogpile.cache.backends.redis.RedisBackend.get_mutex"]
-        ],
-        "get_mutex() (dogpile.cache.proxy.proxybackend method)": [
-            [0, "dogpile.cache.proxy.ProxyBackend.get_mutex"]
-        ],
-        "get_or_create() (dogpile.cache.plugins.mako_cache.makoplugin method)": [
-            [0, "dogpile.cache.plugins.mako_cache.MakoPlugin.get_or_create"]
-        ],
-        "get_or_create() (dogpile.cache.region.cacheregion method)": [
-            [0, "dogpile.cache.region.CacheRegion.get_or_create"]
-        ],
-        "get_or_create_multi() (dogpile.cache.region.cacheregion method)": [
-            [0, "dogpile.cache.region.CacheRegion.get_or_create_multi"]
-        ],
-        "get_serialized() (dogpile.cache.api.bytesbackend method)": [
-            [0, "dogpile.cache.api.BytesBackend.get_serialized"]
-        ],
-        "get_serialized() (dogpile.cache.api.cachebackend method)": [
-            [0, "dogpile.cache.api.CacheBackend.get_serialized"]
-        ],
-        "get_serialized() (dogpile.cache.backends.file.dbmbackend method)": [
-            [0, "dogpile.cache.backends.file.DBMBackend.get_serialized"]
-        ],
-        "get_serialized() (dogpile.cache.backends.redis.redisbackend method)": [
-            [0, "dogpile.cache.backends.redis.RedisBackend.get_serialized"]
-        ],
-        "get_serialized() (dogpile.cache.proxy.proxybackend method)": [
-            [0, "dogpile.cache.proxy.ProxyBackend.get_serialized"]
-        ],
-        "get_serialized_multi() (dogpile.cache.api.bytesbackend method)": [
-            [0, "dogpile.cache.api.BytesBackend.get_serialized_multi"]
-        ],
-        "get_serialized_multi() (dogpile.cache.api.cachebackend method)": [
-            [0, "dogpile.cache.api.CacheBackend.get_serialized_multi"]
-        ],
-        "get_serialized_multi() (dogpile.cache.backends.file.dbmbackend method)": [
-            [0, "dogpile.cache.backends.file.DBMBackend.get_serialized_multi"]
-        ],
-        "get_serialized_multi() (dogpile.cache.backends.redis.redisbackend method)": [
-            [0, "dogpile.cache.backends.redis.RedisBackend.get_serialized_multi"]
-        ],
-        "get_serialized_multi() (dogpile.cache.proxy.proxybackend method)": [
-            [0, "dogpile.cache.proxy.ProxyBackend.get_serialized_multi"]
-        ],
-        "get_value_metadata() (dogpile.cache.region.cacheregion method)": [
-            [0, "dogpile.cache.region.CacheRegion.get_value_metadata"]
-        ],
-        "invalidate() (dogpile.cache.plugins.mako_cache.makoplugin method)": [
-            [0, "dogpile.cache.plugins.mako_cache.MakoPlugin.invalidate"]
-        ],
-        "invalidate() (dogpile.cache.region.cacheregion method)": [
-            [0, "dogpile.cache.region.CacheRegion.invalidate"]
-        ],
-        "invalidate() (dogpile.cache.region.defaultinvalidationstrategy method)": [
-            [0, "dogpile.cache.region.DefaultInvalidationStrategy.invalidate"]
-        ],
-        "invalidate() (dogpile.cache.region.regioninvalidationstrategy method)": [
-            [0, "dogpile.cache.region.RegionInvalidationStrategy.invalidate"]
-        ],
-        "is_configured (dogpile.cache.region.cacheregion property)": [
-            [0, "dogpile.cache.region.CacheRegion.is_configured"]
-        ],
-        "is_hard_invalidated() (dogpile.cache.region.defaultinvalidationstrategy method)": [
-            [0, "dogpile.cache.region.DefaultInvalidationStrategy.is_hard_invalidated"]
-        ],
-        "is_hard_invalidated() (dogpile.cache.region.regioninvalidationstrategy method)": [
-            [0, "dogpile.cache.region.RegionInvalidationStrategy.is_hard_invalidated"]
-        ],
-        "is_invalidated() (dogpile.cache.region.defaultinvalidationstrategy method)": [
-            [0, "dogpile.cache.region.DefaultInvalidationStrategy.is_invalidated"]
-        ],
-        "is_invalidated() (dogpile.cache.region.regioninvalidationstrategy method)": [
-            [0, "dogpile.cache.region.RegionInvalidationStrategy.is_invalidated"]
-        ],
-        "is_open (dogpile.cache.backends.file.abstractfilelock property)": [
-            [0, "dogpile.cache.backends.file.AbstractFileLock.is_open"]
-        ],
-        "is_open (dogpile.cache.backends.file.filelock property)": [
-            [0, "dogpile.cache.backends.file.FileLock.is_open"]
-        ],
-        "is_soft_invalidated() (dogpile.cache.region.defaultinvalidationstrategy method)": [
-            [0, "dogpile.cache.region.DefaultInvalidationStrategy.is_soft_invalidated"]
-        ],
-        "is_soft_invalidated() (dogpile.cache.region.regioninvalidationstrategy method)": [
-            [0, "dogpile.cache.region.RegionInvalidationStrategy.is_soft_invalidated"]
-        ],
-        "key_is_locked() (dogpile.cache.region.cacheregion method)": [
-            [0, "dogpile.cache.region.CacheRegion.key_is_locked"]
-        ],
-        "key_mangler (dogpile.cache.api.cachebackend attribute)": [
-            [0, "dogpile.cache.api.CacheBackend.key_mangler"]
-        ],
-        "kwarg_function_key_generator() (in module dogpile.cache.util)": [
-            [0, "dogpile.cache.util.kwarg_function_key_generator"]
-        ],
-        "length_conditional_mangler() (in module dogpile.cache.util)": [
-            [0, "dogpile.cache.util.length_conditional_mangler"]
-        ],
-        "locked() (dogpile.cache.api.cachemutex method)": [
-            [0, "dogpile.cache.api.CacheMutex.locked"]
-        ],
-        "make_region() (in module dogpile.cache.region)": [
-            [0, "dogpile.cache.region.make_region"]
-        ],
-        "metadata (dogpile.cache.api.cachedvalue attribute)": [
-            [0, "dogpile.cache.api.CachedValue.metadata"]
-        ],
-        "module": [
-            [0, "module-dogpile.cache.api"],
-            [0, "module-dogpile.cache.backends.file"],
-            [0, "module-dogpile.cache.backends.memcached"],
-            [0, "module-dogpile.cache.backends.memory"],
-            [0, "module-dogpile.cache.backends.null"],
-            [0, "module-dogpile.cache.backends.redis"],
-            [0, "module-dogpile.cache.exception"],
-            [0, "module-dogpile.cache.plugins.mako_cache"],
-            [0, "module-dogpile.cache.proxy"],
-            [0, "module-dogpile.cache.region"]
-        ],
-        "payload (dogpile.cache.api.cachedvalue attribute)": [
-            [0, "dogpile.cache.api.CachedValue.payload"]
-        ],
-        "read() (dogpile.cache.backends.file.abstractfilelock method)": [
-            [0, "dogpile.cache.backends.file.AbstractFileLock.read"]
-        ],
-        "release() (dogpile.cache.api.cachemutex method)": [
-            [0, "dogpile.cache.api.CacheMutex.release"]
-        ],
-        "release() (dogpile.cache.backends.file.abstractfilelock method)": [
-            [0, "dogpile.cache.backends.file.AbstractFileLock.release"]
-        ],
-        "release_read_lock() (dogpile.cache.backends.file.abstractfilelock method)": [
-            [0, "dogpile.cache.backends.file.AbstractFileLock.release_read_lock"]
-        ],
-        "release_read_lock() (dogpile.cache.backends.file.filelock method)": [
-            [0, "dogpile.cache.backends.file.FileLock.release_read_lock"]
-        ],
-        "release_read_lock() (dogpile.util.readwritemutex method)": [
-            [0, "dogpile.util.ReadWriteMutex.release_read_lock"]
-        ],
-        "release_write_lock() (dogpile.cache.backends.file.abstractfilelock method)": [
-            [0, "dogpile.cache.backends.file.AbstractFileLock.release_write_lock"]
-        ],
-        "release_write_lock() (dogpile.cache.backends.file.filelock method)": [
-            [0, "dogpile.cache.backends.file.FileLock.release_write_lock"]
-        ],
-        "release_write_lock() (dogpile.util.readwritemutex method)": [
-            [0, "dogpile.util.ReadWriteMutex.release_write_lock"]
-        ],
-        "serializer (dogpile.cache.api.cachebackend attribute)": [
-            [0, "dogpile.cache.api.CacheBackend.serializer"]
-        ],
-        "serializer (dogpile.cache.backends.memcached.genericmemcachedbackend attribute)": [
-            [0, "dogpile.cache.backends.memcached.GenericMemcachedBackend.serializer"]
-        ],
-        "set() (dogpile.cache.api.cachebackend method)": [
-            [0, "dogpile.cache.api.CacheBackend.set"]
-        ],
-        "set() (dogpile.cache.backends.memcached.genericmemcachedbackend method)": [
-            [0, "dogpile.cache.backends.memcached.GenericMemcachedBackend.set"]
-        ],
-        "set() (dogpile.cache.backends.memory.memorybackend method)": [
-            [0, "dogpile.cache.backends.memory.MemoryBackend.set"]
-        ],
-        "set() (dogpile.cache.backends.null.nullbackend method)": [
-            [0, "dogpile.cache.backends.null.NullBackend.set"]
-        ],
-        "set() (dogpile.cache.proxy.proxybackend method)": [
-            [0, "dogpile.cache.proxy.ProxyBackend.set"]
-        ],
-        "set() (dogpile.cache.region.cacheregion method)": [
-            [0, "dogpile.cache.region.CacheRegion.set"]
-        ],
-        "set_arguments (dogpile.cache.backends.memcached.genericmemcachedbackend attribute)": [
-            [0, "dogpile.cache.backends.memcached.GenericMemcachedBackend.set_arguments"]
-        ],
-        "set_multi() (dogpile.cache.api.cachebackend method)": [
-            [0, "dogpile.cache.api.CacheBackend.set_multi"]
-        ],
-        "set_multi() (dogpile.cache.backends.memcached.genericmemcachedbackend method)": [
-            [0, "dogpile.cache.backends.memcached.GenericMemcachedBackend.set_multi"]
-        ],
-        "set_multi() (dogpile.cache.backends.memory.memorybackend method)": [
-            [0, "dogpile.cache.backends.memory.MemoryBackend.set_multi"]
-        ],
-        "set_multi() (dogpile.cache.backends.null.nullbackend method)": [
-            [0, "dogpile.cache.backends.null.NullBackend.set_multi"]
-        ],
-        "set_multi() (dogpile.cache.proxy.proxybackend method)": [
-            [0, "dogpile.cache.proxy.ProxyBackend.set_multi"]
-        ],
-        "set_multi() (dogpile.cache.region.cacheregion method)": [
-            [0, "dogpile.cache.region.CacheRegion.set_multi"]
-        ],
-        "set_serialized() (dogpile.cache.api.bytesbackend method)": [
-            [0, "dogpile.cache.api.BytesBackend.set_serialized"]
-        ],
-        "set_serialized() (dogpile.cache.api.cachebackend method)": [
-            [0, "dogpile.cache.api.CacheBackend.set_serialized"]
-        ],
-        "set_serialized() (dogpile.cache.backends.file.dbmbackend method)": [
-            [0, "dogpile.cache.backends.file.DBMBackend.set_serialized"]
-        ],
-        "set_serialized() (dogpile.cache.backends.redis.redisbackend method)": [
-            [0, "dogpile.cache.backends.redis.RedisBackend.set_serialized"]
-        ],
-        "set_serialized() (dogpile.cache.proxy.proxybackend method)": [
-            [0, "dogpile.cache.proxy.ProxyBackend.set_serialized"]
-        ],
-        "set_serialized_multi() (dogpile.cache.api.bytesbackend method)": [
-            [0, "dogpile.cache.api.BytesBackend.set_serialized_multi"]
-        ],
-        "set_serialized_multi() (dogpile.cache.api.cachebackend method)": [
-            [0, "dogpile.cache.api.CacheBackend.set_serialized_multi"]
-        ],
-        "set_serialized_multi() (dogpile.cache.backends.file.dbmbackend method)": [
-            [0, "dogpile.cache.backends.file.DBMBackend.set_serialized_multi"]
-        ],
-        "set_serialized_multi() (dogpile.cache.backends.redis.redisbackend method)": [
-            [0, "dogpile.cache.backends.redis.RedisBackend.set_serialized_multi"]
-        ],
-        "set_serialized_multi() (dogpile.cache.proxy.proxybackend method)": [
-            [0, "dogpile.cache.proxy.ProxyBackend.set_serialized_multi"]
-        ],
-        "sha1_mangle_key() (in module dogpile.cache.util)": [
-            [0, "dogpile.cache.util.sha1_mangle_key"]
-        ],
-        "value_version (in module dogpile.cache.region)": [
-            [0, "dogpile.cache.region.value_version"]
-        ],
-        "was_hard_invalidated() (dogpile.cache.region.defaultinvalidationstrategy method)": [
-            [0, "dogpile.cache.region.DefaultInvalidationStrategy.was_hard_invalidated"]
-        ],
-        "was_hard_invalidated() (dogpile.cache.region.regioninvalidationstrategy method)": [
-            [0, "dogpile.cache.region.RegionInvalidationStrategy.was_hard_invalidated"]
-        ],
-        "was_soft_invalidated() (dogpile.cache.region.defaultinvalidationstrategy method)": [
-            [0, "dogpile.cache.region.DefaultInvalidationStrategy.was_soft_invalidated"]
-        ],
-        "was_soft_invalidated() (dogpile.cache.region.regioninvalidationstrategy method)": [
-            [0, "dogpile.cache.region.RegionInvalidationStrategy.was_soft_invalidated"]
-        ],
-        "wrap() (dogpile.cache.proxy.proxybackend method)": [
-            [0, "dogpile.cache.proxy.ProxyBackend.wrap"]
-        ],
-        "wrap() (dogpile.cache.region.cacheregion method)": [
-            [0, "dogpile.cache.region.CacheRegion.wrap"]
-        ],
-        "write() (dogpile.cache.backends.file.abstractfilelock method)": [
-            [0, "dogpile.cache.backends.file.AbstractFileLock.write"]
-        ]
+        "recip": 5,
+        "redi": [0, 5],
+        "region": [0, 6],
+        "relat": 5,
+        "rudimentari": [2, 6],
+        "tabl": 4,
+        "updat": 5,
+        "us": [2, 6],
+        "usag": [2, 6],
+        "usecas": 1,
+        "util": 0,
+        "welcom": 4
     }
 })
```

### Comparing `dogpile.cache-1.3.2/docs/usage.html` & `dogpile.cache-1.3.3/docs/usage.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <!DOCTYPE html>
 
 <html lang="en" data-content_root="./">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="viewport" content="width=device-width, initial-scale=1" />
 
-    <title>Usage Guide &#8212; dogpile.cache 1.3.2 documentation</title>
+    <title>Usage Guide &#8212; dogpile.cache 1.3.3 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css?v=fa44fd50" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css?v=d00006d9" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
-    <script src="_static/documentation_options.js?v=8ca9e7a0"></script>
-    <script src="_static/doctools.js?v=888ff710"></script>
+    <script src="_static/documentation_options.js?v=28d163b9"></script>
+    <script src="_static/doctools.js?v=9a2dae69"></script>
     <script src="_static/sphinx_highlight.js?v=dc90522c"></script>
     <link rel="index" title="Index" href="genindex.html" />
     <link rel="search" title="Search" href="search.html" />
     <link rel="next" title="Recipes" href="recipes.html" />
     <link rel="prev" title="Front Matter" href="front.html" /> 
   </head><body>
     <div class="related" role="navigation" aria-label="related navigation">
@@ -29,15 +29,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="recipes.html" title="Recipes"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="front.html" title="Front Matter"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Usage Guide</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -213,32 +213,32 @@
 needed when using a backend such as bsddb or dbm under Python 2.x
 in conjunction with Unicode keys.</p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.params.serializer"></span><strong>serializer</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.params.serializer">¶</a> – <p>function which will be applied to all values before
 passing to the backend.  Defaults to <code class="docutils literal notranslate"><span class="pre">None</span></code>, in which case the
 serializer recommended by the backend will be used.   Typical
 serializers include <code class="docutils literal notranslate"><span class="pre">pickle.dumps</span></code> and <code class="docutils literal notranslate"><span class="pre">json.dumps</span></code>.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.0.</span></p>
+<p><span class="versionmodified added">Added in version 1.1.0.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.params.deserializer"></span><strong>deserializer</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.params.deserializer">¶</a> – <p>function which will be applied to all values returned
 by the backend.  Defaults to <code class="docutils literal notranslate"><span class="pre">None</span></code>, in which case the
 deserializer recommended by the backend will be used.   Typical
 deserializers include <code class="docutils literal notranslate"><span class="pre">pickle.dumps</span></code> and <code class="docutils literal notranslate"><span class="pre">json.dumps</span></code>.</p>
 <p>Deserializers can raise a <a class="reference internal" href="api.html#dogpile.cache.api.CantDeserializeException" title="dogpile.cache.api.CantDeserializeException"><code class="xref py py-class docutils literal notranslate"><span class="pre">api.CantDeserializeException</span></code></a> if they
 are unable to deserialize the value from the backend, indicating
 deserialization failed and that caching should proceed to re-generate
 a value.  This allows an application that has been updated to gracefully
 re-cache old items which were persisted by a previous version of the
 application and can no longer be successfully deserialized.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.1.0: </span>added “deserializer” parameter</p>
+<p><span class="versionmodified added">Added in version 1.1.0: </span>added “deserializer” parameter</p>
 </div>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 1.2.0: </span>added support for
+<p><span class="versionmodified added">Added in version 1.2.0: </span>added support for
 <a class="reference internal" href="api.html#dogpile.cache.api.CantDeserializeException" title="dogpile.cache.api.CantDeserializeException"><code class="xref py py-class docutils literal notranslate"><span class="pre">api.CantDeserializeException</span></code></a></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.params.async_creation_runner"></span><strong>async_creation_runner</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.params.async_creation_runner">¶</a> – <p>A callable that, when specified,
 will be passed to and called by dogpile.lock when
 there is a stale value present in the cache.  It will be passed the
 mutex and is responsible releasing that mutex when finished.
@@ -280,15 +280,15 @@
 However, subsequent requests for cached-but-expired values will
 still return promptly.  They will be refreshed by whatever
 asynchronous means the provided async_creation_runner callable
 implements.</p>
 <p>By default the async_creation_runner is disabled and is set
 to <code class="docutils literal notranslate"><span class="pre">None</span></code>.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.4.2: </span>added the async_creation_runner
+<p><span class="versionmodified added">Added in version 0.4.2: </span>added the async_creation_runner
 feature.</p>
 </div>
 </p></li>
 </ul>
 </dd>
 </dl>
 </dd></dl>
@@ -321,33 +321,33 @@
 directly to the constructor of the <a class="reference internal" href="api.html#dogpile.cache.api.CacheBackend" title="dogpile.cache.api.CacheBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheBackend</span></code></a>
 in use, though is typically a dictionary.</p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.configure.params.wrap"></span><strong>wrap</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.configure.params.wrap">¶</a> – <p>Optional.  A list of <a class="reference internal" href="api.html#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a>
 classes and/or instances, each of which will be applied
 in a chain to ultimately wrap the original backend,
 so that custom functionality augmentation can be applied.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.0.</span></p>
 </div>
 <div class="admonition seealso">
 <p class="admonition-title">See also</p>
 <p><a class="reference internal" href="#changing-backend-behavior"><span class="std std-ref">Changing Backend Behavior</span></a></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.configure.params.replace_existing_backend"></span><strong>replace_existing_backend</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.configure.params.replace_existing_backend">¶</a> – <p>if True, the existing cache backend
 will be replaced.  Without this flag, an exception is raised if
 a backend is already configured.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.7.</span></p>
+<p><span class="versionmodified added">Added in version 0.5.7.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.configure.params.region_invalidator"></span><strong>region_invalidator</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.configure.params.region_invalidator">¶</a> – <p>Optional. Override default invalidation
 strategy with custom implementation of
 <a class="reference internal" href="api.html#dogpile.cache.region.RegionInvalidationStrategy" title="dogpile.cache.region.RegionInvalidationStrategy"><code class="xref py py-class docutils literal notranslate"><span class="pre">RegionInvalidationStrategy</span></code></a>.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.6.2.</span></p>
+<p><span class="versionmodified added">Added in version 0.6.2.</span></p>
 </div>
 </p></li>
 </ul>
 </dd>
 </dl>
 </dd></dl>
 
@@ -382,41 +382,42 @@
 </section>
 <section id="using-a-region">
 <h2>Using a Region<a class="headerlink" href="#using-a-region" title="Link to this heading">¶</a></h2>
 <p>The <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a> object is our front-end interface to a cache.  It includes
 the following methods:</p>
 <dl class="py method">
 <dt class="sig sig-object py">
-<span class="sig-prename descclassname"><span class="pre">CacheRegion.</span></span><span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">expiration_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ignore_expiration</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference internal" href="api.html#dogpile.cache.api.CachedValue" title="dogpile.cache.api.CachedValue"><span class="pre">CachedValue</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference internal" href="api.html#dogpile.cache.api.NoValue" title="dogpile.cache.api.NoValue"><span class="pre">NoValue</span></a></span></span></dt>
+<span class="sig-prename descclassname"><span class="pre">CacheRegion.</span></span><span class="sig-name descname"><span class="pre">get</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">key</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">str</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">expiration_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">None</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ignore_expiration</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">bool</span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><span class="pre">Any</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Literal</span><span class="p"><span class="pre">[</span></span><span class="pre">NoValue.NO_VALUE</span><span class="p"><span class="pre">]</span></span></span></span></dt>
 <dd><p>Return a value from the cache, based on the given key.</p>
 <p>If the value is not present, the method returns the token
-<code class="docutils literal notranslate"><span class="pre">NO_VALUE</span></code>. <code class="docutils literal notranslate"><span class="pre">NO_VALUE</span></code> evaluates to False, but is separate from
-<code class="docutils literal notranslate"><span class="pre">None</span></code> to distinguish between a cached value of <code class="docutils literal notranslate"><span class="pre">None</span></code>.</p>
+<a class="reference internal" href="api.html#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">api.NO_VALUE</span></code></a>. <a class="reference internal" href="api.html#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">api.NO_VALUE</span></code></a> evaluates to False, but is
+separate from <code class="docutils literal notranslate"><span class="pre">None</span></code> to distinguish between a cached value of
+<code class="docutils literal notranslate"><span class="pre">None</span></code>.</p>
 <p>By default, the configured expiration time of the
 <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a>, or alternatively the expiration
 time supplied by the <code class="docutils literal notranslate"><span class="pre">expiration_time</span></code> argument,
 is tested against the creation time of the retrieved
 value versus the current time (as reported by <code class="docutils literal notranslate"><span class="pre">time.time()</span></code>).
-If stale, the cached value is ignored and the <code class="docutils literal notranslate"><span class="pre">NO_VALUE</span></code>
+If stale, the cached value is ignored and the <a class="reference internal" href="api.html#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">api.NO_VALUE</span></code></a>
 token is returned.  Passing the flag <code class="docutils literal notranslate"><span class="pre">ignore_expiration=True</span></code>
 bypasses the expiration time check.</p>
 <div class="versionchanged">
 <p><span class="versionmodified changed">Changed in version 0.3.0: </span><a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion.get" title="dogpile.cache.region.CacheRegion.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get()</span></code></a> now checks the value’s creation time
 against the expiration time, rather than returning
 the value unconditionally.</p>
 </div>
 <p>The method also interprets the cached value in terms
 of the current “invalidation” time as set by
 the <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion.invalidate" title="dogpile.cache.region.CacheRegion.invalidate"><code class="xref py py-meth docutils literal notranslate"><span class="pre">invalidate()</span></code></a> method.   If a value is present,
 but its creation time is older than the current
-invalidation time, the <code class="docutils literal notranslate"><span class="pre">NO_VALUE</span></code> token is returned.
+invalidation time, the <a class="reference internal" href="api.html#dogpile.cache.api.NO_VALUE" title="dogpile.cache.api.NO_VALUE"><code class="xref py py-data docutils literal notranslate"><span class="pre">api.NO_VALUE</span></code></a> token is returned.
 Passing the flag <code class="docutils literal notranslate"><span class="pre">ignore_expiration=True</span></code> bypasses
 the invalidation time check.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.3.0: </span>Support for the <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion.invalidate" title="dogpile.cache.region.CacheRegion.invalidate"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.invalidate()</span></code></a>
+<p><span class="versionmodified added">Added in version 0.3.0: </span>Support for the <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion.invalidate" title="dogpile.cache.region.CacheRegion.invalidate"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.invalidate()</span></code></a>
 method.</p>
 </div>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.get.params.key"></span><strong>key</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.get.params.key">¶</a> – Key to be retrieved. While it’s typical for a key to be a
 string, it is ultimately passed directly down to the cache backend,
@@ -432,23 +433,23 @@
 argument is <strong>not persisted in the cache</strong> and is relevant
 only to <strong>this specific cache retrieval operation</strong>, relative to
 the creation time stored with the existing cached value.
 Subsequent calls to <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion.get" title="dogpile.cache.region.CacheRegion.get"><code class="xref py py-meth docutils literal notranslate"><span class="pre">CacheRegion.get()</span></code></a> are <strong>not</strong> affected
 by this value.</p>
 </div>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.3.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.3.0.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.get.params.ignore_expiration"></span><strong>ignore_expiration</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.get.params.ignore_expiration">¶</a> – <p>if <code class="docutils literal notranslate"><span class="pre">True</span></code>, the value is returned
 from the cache if present, regardless of configured
 expiration times or whether or not <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion.invalidate" title="dogpile.cache.region.CacheRegion.invalidate"><code class="xref py py-meth docutils literal notranslate"><span class="pre">invalidate()</span></code></a>
 was called.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.3.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.3.0.</span></p>
 </div>
 </p></li>
 </ul>
 </dd>
 </dl>
 <div class="admonition seealso">
 <p class="admonition-title">See also</p>
@@ -493,15 +494,15 @@
 before being optionally processed by the key_mangler function, so can
 be of any type recognized by the backend or by the key_mangler
 function, if present.</p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.get_or_create.params.creator"></span><strong>creator</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.get_or_create.params.creator">¶</a> – function which creates a new value.</p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.get_or_create.params.creator_args"></span><strong>creator_args</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.get_or_create.params.creator_args">¶</a> – <p>optional tuple of (args, kwargs) that will be
 passed to the creator function if present.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.7.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.7.0.</span></p>
 </div>
 </p></li>
 <li><p><span class="target" id="dogpile.cache.region.CacheRegion.get_or_create.params.expiration_time"></span><strong>expiration_time</strong><a class="paramlink headerlink reference internal" href="#dogpile.cache.region.CacheRegion.get_or_create.params.expiration_time">¶</a> – <p>optional expiration time which will override
 the expiration time already configured on this <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a>
 if not None.   To set no expiration, use the value -1.</p>
 <div class="admonition note">
 <p class="admonition-title">Note</p>
@@ -526,15 +527,15 @@
                     <span class="n">should_cache_fn</span><span class="o">=</span><span class="n">dont_cache_none</span><span class="p">)</span>
 </pre></div>
 </div>
 <p>Above, the function returns the value of create_value() if
 the cache is invalid, however if the return value is None,
 it won’t be cached.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.4.3.</span></p>
+<p><span class="versionmodified added">Added in version 0.4.3.</span></p>
 </div>
 </p></li>
 </ul>
 </dd>
 </dl>
 <div class="admonition seealso">
 <p class="admonition-title">See also</p>
@@ -599,43 +600,43 @@
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">generate_something</span><span class="o">.</span><span class="n">set</span><span class="p">(</span><span class="mi">3</span><span class="p">,</span> <span class="mi">5</span><span class="p">,</span> <span class="mi">6</span><span class="p">)</span>
 </pre></div>
 </div>
 <p>The above example is equivalent to calling
 <code class="docutils literal notranslate"><span class="pre">generate_something(5,</span> <span class="pre">6)</span></code>, if the function were to produce
 the value <code class="docutils literal notranslate"><span class="pre">3</span></code> as the value to be cached.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.4.1: </span>Added <code class="docutils literal notranslate"><span class="pre">set()</span></code> method to decorated function.</p>
+<p><span class="versionmodified added">Added in version 0.4.1: </span>Added <code class="docutils literal notranslate"><span class="pre">set()</span></code> method to decorated function.</p>
 </div>
 <p>Similar to <code class="docutils literal notranslate"><span class="pre">set()</span></code> is <code class="docutils literal notranslate"><span class="pre">refresh()</span></code>.   This attribute will
 invoke the decorated function and populate a new value into
 the cache with the new value, as well as returning that value:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">newvalue</span> <span class="o">=</span> <span class="n">generate_something</span><span class="o">.</span><span class="n">refresh</span><span class="p">(</span><span class="mi">5</span><span class="p">,</span> <span class="mi">6</span><span class="p">)</span>
 </pre></div>
 </div>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.0: </span>Added <code class="docutils literal notranslate"><span class="pre">refresh()</span></code> method to decorated
+<p><span class="versionmodified added">Added in version 0.5.0: </span>Added <code class="docutils literal notranslate"><span class="pre">refresh()</span></code> method to decorated
 function.</p>
 </div>
 <p><code class="docutils literal notranslate"><span class="pre">original()</span></code> on other hand will invoke the decorated function
 without any caching:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">newvalue</span> <span class="o">=</span> <span class="n">generate_something</span><span class="o">.</span><span class="n">original</span><span class="p">(</span><span class="mi">5</span><span class="p">,</span> <span class="mi">6</span><span class="p">)</span>
 </pre></div>
 </div>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.6.0: </span>Added <code class="docutils literal notranslate"><span class="pre">original()</span></code> method to decorated
+<p><span class="versionmodified added">Added in version 0.6.0: </span>Added <code class="docutils literal notranslate"><span class="pre">original()</span></code> method to decorated
 function.</p>
 </div>
 <p>Lastly, the <code class="docutils literal notranslate"><span class="pre">get()</span></code> method returns either the value cached
 for the given key, or the token <code class="docutils literal notranslate"><span class="pre">NO_VALUE</span></code> if no such key
 exists:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">value</span> <span class="o">=</span> <span class="n">generate_something</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="mi">5</span><span class="p">,</span> <span class="mi">6</span><span class="p">)</span>
 </pre></div>
 </div>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.5.3: </span>Added <code class="docutils literal notranslate"><span class="pre">get()</span></code> method to decorated
+<p><span class="versionmodified added">Added in version 0.5.3: </span>Added <code class="docutils literal notranslate"><span class="pre">get()</span></code> method to decorated
 function.</p>
 </div>
 <p>The default key generation will use the name
 of the function, the module name for the function,
 the arguments passed, as well as an optional “namespace”
 parameter in order to generate a cache key.</p>
 <p>Given a function <code class="docutils literal notranslate"><span class="pre">one</span></code> inside the module
@@ -856,21 +857,21 @@
 </pre></div>
 </div>
 <p>In the above example, the <code class="docutils literal notranslate"><span class="pre">LoggingProxy</span></code> object would be instantated by the
 <a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a> and applied to wrap requests on behalf of
 the <code class="docutils literal notranslate"><span class="pre">retry_proxy</span></code> instance; that proxy in turn wraps
 requests on behalf of the original dogpile.cache.pylibmc backend.</p>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.4.4: </span>Added support for the <a class="reference internal" href="api.html#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a> class.</p>
+<p><span class="versionmodified added">Added in version 0.4.4: </span>Added support for the <a class="reference internal" href="api.html#dogpile.cache.proxy.ProxyBackend" title="dogpile.cache.proxy.ProxyBackend"><code class="xref py py-class docutils literal notranslate"><span class="pre">ProxyBackend</span></code></a> class.</p>
 </div>
 </section>
 <section id="configuring-logging">
 <h2>Configuring Logging<a class="headerlink" href="#configuring-logging" title="Link to this heading">¶</a></h2>
 <div class="versionadded">
-<p><span class="versionmodified added">New in version 0.9.0.</span></p>
+<p><span class="versionmodified added">Added in version 0.9.0.</span></p>
 </div>
 <p><a class="reference internal" href="api.html#dogpile.cache.region.CacheRegion" title="dogpile.cache.region.CacheRegion"><code class="xref py py-class docutils literal notranslate"><span class="pre">CacheRegion</span></code></a> includes logging facilities that will emit debug log
 messages when key cache events occur, including when keys are regenerated as
 well as when hard invalidations occur.   Using the <a class="reference external" href="https://docs.python.org/3/library/logging.html">Python logging</a> module, set the log level to
 <code class="docutils literal notranslate"><span class="pre">dogpile.cache</span></code> to <code class="docutils literal notranslate"><span class="pre">logging.DEBUG</span></code>:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="n">logging</span><span class="o">.</span><span class="n">basicConfig</span><span class="p">()</span>
 <span class="n">logging</span><span class="o">.</span><span class="n">getLogger</span><span class="p">(</span><span class="s2">&quot;dogpile.cache&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">setLevel</span><span class="p">(</span><span class="n">logging</span><span class="o">.</span><span class="n">DEBUG</span><span class="p">)</span>
@@ -907,23 +908,23 @@
 <li><a class="reference internal" href="#changing-backend-behavior">Changing Backend Behavior</a></li>
 <li><a class="reference internal" href="#configuring-logging">Configuring Logging</a></li>
 </ul>
 </li>
 </ul>
 
   </div>
-<div id="searchbox" style="display: none" role="search">
+<search id="searchbox" style="display: none" role="search">
   <h3 id="searchlabel">Quick search</h3>
     <div class="searchformwrapper">
     <form class="search" action="search.html" method="get">
       <input type="text" name="q" aria-labelledby="searchlabel" autocomplete="off" autocorrect="off" autocapitalize="off" spellcheck="false"/>
       <input type="submit" value="Go" />
     </form>
     </div>
-</div>
+</search>
 <script>document.getElementById('searchbox').style.display = "block"</script>
   <div>
     <h4>Previous topic</h4>
     <p class="topless"><a href="front.html"
                           title="previous chapter">Front Matter</a></p>
   </div>
   <div>
@@ -946,17 +947,17 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="recipes.html" title="Recipes"
              >next</a> |</li>
         <li class="right" >
           <a href="front.html" title="Front Matter"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.2 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">dogpile.cache 1.3.3 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Usage Guide</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
     &#169; Copyright 2011-2024 Mike Bayer.
-      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.2.6.
+      Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 7.3.7.
     </div>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 ******** NNaavviiggaattiioonn ********
     * _i_n_d_e_x
     * _m_o_d_u_l_e_s |
     * _n_e_x_t |
     * _p_r_e_v_i_o_u_s |
-    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._2_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
+    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._3_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
     * Usage Guide
 ************ UUssaaggee GGuuiiddee_?¶ ************
 ********** OOvveerrvviieeww_?¶ **********
 At the time of this writing, popular key/value servers include _M_e_m_c_a_c_h_e_d, _R_e_d_i_s
 and many others. While these tools all have different usage focuses, they all
 have in common that the storage model is based on the retrieval of a value
 based on a key; as such, they are all potentially suitable for caching,
@@ -119,34 +119,34 @@
       local_region.configure_from_config(myconfig, "cache.local.")
       memcached_region.configure_from_config(myconfig,
                                           "cache.memcached.")
 ********** UUssiinngg aa RReeggiioonn_?¶ **********
 The _C_a_c_h_e_R_e_g_i_o_n object is our front-end interface to a cache. It includes the
 following methods:
   CacheRegion.get(kkeeyy:: ssttrr, eexxppiirraattiioonn__ttiimmee:: ffllooaatt || NNoonnee == NNoonnee,
-  iiggnnoorree__eexxppiirraattiioonn:: bbooooll == FFaallssee) → _C_a_c_h_e_d_V_a_l_u_e | _N_o_V_a_l_u_e
+  iiggnnoorree__eexxppiirraattiioonn:: bbooooll == FFaallssee) → Any | Literal[NoValue.NO_VALUE]
       Return a value from the cache, based on the given key.
-      If the value is not present, the method returns the token NO_VALUE.
-      NO_VALUE evaluates to False, but is separate from None to distinguish
+      If the value is not present, the method returns the token _a_p_i_._N_O___V_A_L_U_E.
+      _a_p_i_._N_O___V_A_L_U_E evaluates to False, but is separate from None to distinguish
       between a cached value of None.
       By default, the configured expiration time of the _C_a_c_h_e_R_e_g_i_o_n, or
       alternatively the expiration time supplied by the expiration_time
       argument, is tested against the creation time of the retrieved value
       versus the current time (as reported by time.time()). If stale, the
-      cached value is ignored and the NO_VALUE token is returned. Passing the
-      flag ignore_expiration=True bypasses the expiration time check.
+      cached value is ignored and the _a_p_i_._N_O___V_A_L_U_E token is returned. Passing
+      the flag ignore_expiration=True bypasses the expiration time check.
       Changed in version 0.3.0: _C_a_c_h_e_R_e_g_i_o_n_._g_e_t_(_) now checks the value’s
       creation time against the expiration time, rather than returning the
       value unconditionally.
       The method also interprets the cached value in terms of the current
       “invalidation” time as set by the _i_n_v_a_l_i_d_a_t_e_(_) method. If a value is
       present, but its creation time is older than the current invalidation
-      time, the NO_VALUE token is returned. Passing the flag
+      time, the _a_p_i_._N_O___V_A_L_U_E token is returned. Passing the flag
       ignore_expiration=True bypasses the invalidation time check.
-      New in version 0.3.0: Support for the _C_a_c_h_e_R_e_g_i_o_n_._i_n_v_a_l_i_d_a_t_e_(_) method.
+      Added in version 0.3.0: Support for the _C_a_c_h_e_R_e_g_i_o_n_._i_n_v_a_l_i_d_a_t_e_(_) method.
       See also
       _C_a_c_h_e_R_e_g_i_o_n_._g_e_t___m_u_l_t_i_(_)
       _C_a_c_h_e_R_e_g_i_o_n_._g_e_t___o_r___c_r_e_a_t_e_(_)
       _C_a_c_h_e_R_e_g_i_o_n_._s_e_t_(_)
       _C_a_c_h_e_R_e_g_i_o_n_._d_e_l_e_t_e_(_)
   CacheRegion.get_or_create(kkeeyy:: ssttrr, ccrreeaattoorr:: CCaallllaabbllee[[[[......]],, AAnnyy]],
   eexxppiirraattiioonn__ttiimmee:: ffllooaatt || NNoonnee == NNoonnee, sshhoouulldd__ccaacchhee__ffnn:: CCaallllaabbllee[[[[AAnnyy]],, bbooooll]]
@@ -208,28 +208,28 @@
       _C_a_c_h_e_R_e_g_i_o_n_._s_e_t_(_) which will store a given value directly without calling
       the decorated function. The value to be cached is passed as the first
       argument, and the arguments which would normally be passed to the
       function should follow:
       generate_something.set(3, 5, 6)
       The above example is equivalent to calling generate_something(5, 6), if
       the function were to produce the value 3 as the value to be cached.
-      New in version 0.4.1: Added set() method to decorated function.
+      Added in version 0.4.1: Added set() method to decorated function.
       Similar to set() is refresh(). This attribute will invoke the decorated
       function and populate a new value into the cache with the new value, as
       well as returning that value:
       newvalue = generate_something.refresh(5, 6)
-      New in version 0.5.0: Added refresh() method to decorated function.
+      Added in version 0.5.0: Added refresh() method to decorated function.
       original() on other hand will invoke the decorated function without any
       caching:
       newvalue = generate_something.original(5, 6)
-      New in version 0.6.0: Added original() method to decorated function.
+      Added in version 0.6.0: Added original() method to decorated function.
       Lastly, the get() method returns either the value cached for the given
       key, or the token NO_VALUE if no such key exists:
       value = generate_something.get(5, 6)
-      New in version 0.5.3: Added get() method to decorated function.
+      Added in version 0.5.3: Added get() method to decorated function.
       The default key generation will use the name of the function, the module
       name for the function, the arguments passed, as well as an optional
       “namespace” parameter in order to generate a cache key.
       Given a function one inside the module myapp.tools:
       @region.cache_on_arguments(namespace="foo")
       def one(a, b):
           return a + b
@@ -370,17 +370,17 @@
     },
     wrap = [ LoggingProxy, retry_proxy ]
 )
 In the above example, the LoggingProxy object would be instantated by the
 _C_a_c_h_e_R_e_g_i_o_n and applied to wrap requests on behalf of the retry_proxy instance;
 that proxy in turn wraps requests on behalf of the original
 dogpile.cache.pylibmc backend.
-New in version 0.4.4: Added support for the _P_r_o_x_y_B_a_c_k_e_n_d class.
+Added in version 0.4.4: Added support for the _P_r_o_x_y_B_a_c_k_e_n_d class.
 ********** CCoonnffiigguurriinngg LLooggggiinngg_?¶ **********
-New in version 0.9.0.
+Added in version 0.9.0.
 _C_a_c_h_e_R_e_g_i_o_n includes logging facilities that will emit debug log messages when
 key cache events occur, including when keys are regenerated as well as when
 hard invalidations occur. Using the _P_y_t_h_o_n_ _l_o_g_g_i_n_g module, set the log level to
 dogpile.cache to logging.DEBUG:
 logging.basicConfig()
 logging.getLogger("dogpile.cache").setLevel(logging.DEBUG)
 Debug logging will indicate time spent regenerating keys as well as when keys
@@ -412,10 +412,10 @@
 ****** NNeexxtt ttooppiicc ******
 _R_e_c_i_p_e_s
 ******** NNaavviiggaattiioonn ********
     * _i_n_d_e_x
     * _m_o_d_u_l_e_s |
     * _n_e_x_t |
     * _p_r_e_v_i_o_u_s |
-    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._2_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
+    * _d_o_g_p_i_l_e_._c_a_c_h_e_ _1_._3_._3_ _d_o_c_u_m_e_n_t_a_t_i_o_n »
     * Usage Guide
-© Copyright 2011-2024 Mike Bayer. Created using _S_p_h_i_n_x 7.2.6.
+© Copyright 2011-2024 Mike Bayer. Created using _S_p_h_i_n_x 7.3.7.
```

### Comparing `dogpile.cache-1.3.2/dogpile/cache/api.py` & `dogpile.cache-1.3.3/dogpile/cache/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from __future__ import annotations
 
 import abc
+import enum
 import pickle
 import time
 from typing import Any
 from typing import Callable
 from typing import cast
+from typing import Literal
 from typing import Mapping
 from typing import NamedTuple
 from typing import Optional
 from typing import Sequence
 from typing import Union
 
 from ..util.typing import Self
 
 
-class NoValue:
+class NoValue(enum.Enum):
     """Describe a missing cache value.
 
     The :data:`.NO_VALUE` constant should be used.
 
     """
 
     @property
@@ -29,20 +31,24 @@
     def __repr__(self):
         """Ensure __repr__ is a consistent value in case NoValue is used to
         fill another cache key.
 
         """
         return "<dogpile.cache.api.NoValue object>"
 
-    def __bool__(self):  # pragma NO COVERAGE
+    def __bool__(self) -> Literal[False]:  # pragma NO COVERAGE
         return False
 
+    NO_VALUE = "NoValue"
 
-NO_VALUE = NoValue()
-"""Value returned from ``get()`` that describes
+
+NoValueType = Literal[NoValue.NO_VALUE]
+
+NO_VALUE = NoValue.NO_VALUE
+"""Value returned from :meth:`.CacheRegion.get` that describes
 a  key not present."""
 
 MetaDataType = Mapping[str, Any]
 
 
 KeyType = str
 """A cache key."""
@@ -156,21 +162,21 @@
 
         .. versionadded:: 1.3
 
         """
         return time.time() - self.cached_time
 
 
-CacheReturnType = Union[CachedValue, NoValue]
+CacheReturnType = Union[CachedValue, NoValueType]
 """The non-serialized form of what may be returned from a backend
 get method.
 
 """
 
-SerializedReturnType = Union[bytes, NoValue]
+SerializedReturnType = Union[bytes, NoValueType]
 """the serialized form of what may be returned from a backend get method."""
 
 BackendFormatted = Union[CacheReturnType, SerializedReturnType]
 """Describes the type returned from the :meth:`.CacheBackend.get` method."""
 
 BackendSetType = Union[CachedValue, bytes]
 """Describes the value argument passed to the :meth:`.CacheBackend.set`
```

### Comparing `dogpile.cache-1.3.2/dogpile/cache/backends/__init__.py` & `dogpile.cache-1.3.3/dogpile/cache/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/dogpile/cache/backends/file.py` & `dogpile.cache-1.3.3/dogpile/cache/backends/file.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/dogpile/cache/backends/memcached.py` & `dogpile.cache-1.3.3/dogpile/cache/backends/memcached.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,34 +91,14 @@
      threading mutex.
     :param lock_timeout: integer, number of seconds after acquiring a lock that
      memcached should expire it.  This argument is only valid when
      ``distributed_lock`` is ``True``.
 
      .. versionadded:: 0.5.7
 
-    :param memcached_expire_time: integer, when present will
-     be passed as the ``time`` parameter to ``pylibmc.Client.set``.
-     This is used to set the memcached expiry time for a value.
-
-     .. note::
-
-         This parameter is **different** from Dogpile's own
-         ``expiration_time``, which is the number of seconds after
-         which Dogpile will consider the value to be expired.
-         When Dogpile considers a value to be expired,
-         it **continues to use the value** until generation
-         of a new value is complete, when using
-         :meth:`.CacheRegion.get_or_create`.
-         Therefore, if you are setting ``memcached_expire_time``, you'll
-         want to make sure it is greater than ``expiration_time``
-         by at least enough seconds for new values to be generated,
-         else the value won't be available during a regeneration,
-         forcing all threads to wait for a regeneration each time
-         a value expires.
-
     The :class:`.GenericMemachedBackend` uses a ``threading.local()``
     object to store individual client objects per thread,
     as most modern memcached clients do not appear to be inherently
     threadsafe.
 
     In particular, ``threading.local()`` has the advantage over pylibmc's
     built-in thread pool in that it automatically discards objects
@@ -143,15 +123,14 @@
         # automatically deletes the __dict__ when a thread ends,
         # so the idea is that this is superior to pylibmc's
         # own ThreadMappedPool which doesn't handle this
         # automatically.
         self.url = util.to_list(arguments["url"])
         self.distributed_lock = arguments.get("distributed_lock", False)
         self.lock_timeout = arguments.get("lock_timeout", 0)
-        self.memcached_expire_time = arguments.get("memcached_expire_time", 0)
 
     def has_lock_timeout(self):
         return self.lock_timeout != 0
 
     def _imports(self):
         """client library imports go here."""
         raise NotImplementedError()
@@ -218,14 +197,37 @@
     def delete_multi(self, keys):
         self.client.delete_multi(keys)
 
 
 class MemcacheArgs(GenericMemcachedBackend):
     """Mixin which provides support for the 'time' argument to set(),
     'min_compress_len' to other methods.
+
+    :param memcached_expire_time: integer, when present will
+     be passed as the ``time`` parameter to the ``set`` method.
+     This is used to set the memcached expiry time for a value.
+
+     .. note::
+
+         This parameter is **different** from Dogpile's own
+         ``expiration_time``, which is the number of seconds after
+         which Dogpile will consider the value to be expired.
+         When Dogpile considers a value to be expired,
+         it **continues to use the value** until generation
+         of a new value is complete, when using
+         :meth:`.CacheRegion.get_or_create`.
+         Therefore, if you are setting ``memcached_expire_time``, you'll
+         want to make sure it is greater than ``expiration_time``
+         by at least enough seconds for new values to be generated,
+         else the value won't be available during a regeneration,
+         forcing all threads to wait for a regeneration each time
+         a value expires.
+
+    :param min_compress_len: Threshold length to kick in auto-compression
+     of the value using the compressor
     """
 
     def __init__(self, arguments):
         self.min_compress_len = arguments.get("min_compress_len", 0)
 
         self.set_arguments = {}
         if "memcached_expire_time" in arguments:
@@ -404,33 +406,16 @@
         self.tls_context = arguments.get("tls_context", None)
         super(BMemcachedBackend, self).__init__(arguments)
 
     def _imports(self):
         global bmemcached
         import bmemcached
 
-        class RepairBMemcachedAPI(bmemcached.Client):
-            """Repairs BMemcached's non-standard method
-            signatures, which was fixed in BMemcached
-            ef206ed4473fec3b639e.
-
-            """
-
-            def add(self, key, value, timeout=0):
-                try:
-                    return super(RepairBMemcachedAPI, self).add(
-                        key, value, timeout
-                    )
-                except ValueError:
-                    return False
-
-        self.Client = RepairBMemcachedAPI
-
     def _create_client(self):
-        return self.Client(
+        return bmemcached.Client(
             self.url,
             username=self.username,
             password=self.password,
             tls_context=self.tls_context,
         )
 
     def delete_multi(self, keys):
@@ -576,14 +561,36 @@
      .. versionadded:: 1.1.5
 
     :param dead_timeout: Time in seconds before attempting to add a node
      back in the pool in the HashClient's internal mechanisms.
 
      .. versionadded:: 1.1.5
 
+    :param memcached_expire_time: integer, when present will
+     be passed as the ``time`` parameter to the ``set`` method.
+     This is used to set the memcached expiry time for a value.
+
+     .. note::
+
+         This parameter is **different** from Dogpile's own
+         ``expiration_time``, which is the number of seconds after
+         which Dogpile will consider the value to be expired.
+         When Dogpile considers a value to be expired,
+         it **continues to use the value** until generation
+         of a new value is complete, when using
+         :meth:`.CacheRegion.get_or_create`.
+         Therefore, if you are setting ``memcached_expire_time``, you'll
+         want to make sure it is greater than ``expiration_time``
+         by at least enough seconds for new values to be generated,
+         else the value won't be available during a regeneration,
+         forcing all threads to wait for a regeneration each time
+         a value expires.
+
+     .. versionadded:: 1.3.3
+
     """  # noqa E501
 
     def __init__(self, arguments):
         super().__init__(arguments)
 
         self.serde = arguments.get("serde", pymemcache.serde.pickle_serde)
         self.default_noreply = arguments.get("default_noreply", False)
@@ -607,14 +614,17 @@
             or self.retry_for is not None
             or self.do_not_retry_for is not None
         ) and not self.enable_retry_client:
             warnings.warn(
                 "enable_retry_client is not set; retry options "
                 "will be ignored"
             )
+        self.set_arguments = {}
+        if "memcached_expire_time" in arguments:
+            self.set_arguments["expire"] = arguments["memcached_expire_time"]
 
     def _imports(self):
         global pymemcache
         import pymemcache
 
     def _create_client(self):
         _kwargs = {
```

### Comparing `dogpile.cache-1.3.2/dogpile/cache/backends/memory.py` & `dogpile.cache-1.3.3/dogpile/cache/backends/memory.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/dogpile/cache/backends/null.py` & `dogpile.cache-1.3.3/dogpile/cache/backends/null.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/dogpile/cache/backends/redis.py` & `dogpile.cache-1.3.3/dogpile/cache/backends/redis.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/dogpile/cache/exception.py` & `dogpile.cache-1.3.3/dogpile/cache/exception.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/dogpile/cache/plugins/mako_cache.py` & `dogpile.cache-1.3.3/dogpile/cache/plugins/mako_cache.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/dogpile/cache/proxy.py` & `dogpile.cache-1.3.3/dogpile/cache/proxy.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/dogpile/cache/region.py` & `dogpile.cache-1.3.3/dogpile/cache/region.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from .api import CachedValue
 from .api import CacheMutex
 from .api import CacheReturnType
 from .api import CantDeserializeException
 from .api import KeyType
 from .api import MetaDataType
 from .api import NO_VALUE
+from .api import NoValueType
 from .api import SerializedReturnType
 from .api import Serializer
 from .api import ValuePayload
 from .backends import _backend_loader
 from .backends import register_backend  # noqa
 from .proxy import ProxyBackend
 from .util import function_key_generator
@@ -702,40 +703,41 @@
         return "backend" in self.__dict__
 
     def get(
         self,
         key: KeyType,
         expiration_time: Optional[float] = None,
         ignore_expiration: bool = False,
-    ) -> CacheReturnType:
+    ) -> Union[ValuePayload, NoValueType]:
         """Return a value from the cache, based on the given key.
 
         If the value is not present, the method returns the token
-        ``NO_VALUE``. ``NO_VALUE`` evaluates to False, but is separate from
-        ``None`` to distinguish between a cached value of ``None``.
+        :data:`.api.NO_VALUE`. :data:`.api.NO_VALUE` evaluates to False, but is
+        separate from ``None`` to distinguish between a cached value of
+        ``None``.
 
         By default, the configured expiration time of the
         :class:`.CacheRegion`, or alternatively the expiration
         time supplied by the ``expiration_time`` argument,
         is tested against the creation time of the retrieved
         value versus the current time (as reported by ``time.time()``).
-        If stale, the cached value is ignored and the ``NO_VALUE``
+        If stale, the cached value is ignored and the :data:`.api.NO_VALUE`
         token is returned.  Passing the flag ``ignore_expiration=True``
         bypasses the expiration time check.
 
         .. versionchanged:: 0.3.0
            :meth:`.CacheRegion.get` now checks the value's creation time
            against the expiration time, rather than returning
            the value unconditionally.
 
         The method also interprets the cached value in terms
         of the current "invalidation" time as set by
         the :meth:`.invalidate` method.   If a value is present,
         but its creation time is older than the current
-        invalidation time, the ``NO_VALUE`` token is returned.
+        invalidation time, the :data:`.api.NO_VALUE` token is returned.
         Passing the flag ``ignore_expiration=True`` bypasses
         the invalidation time check.
 
         .. versionadded:: 0.3.0
            Support for the :meth:`.CacheRegion.invalidate`
            method.
 
@@ -1079,15 +1081,15 @@
                     ca = creator_args
 
                     @wraps(creator)
                     def go():
                         return creator(*ca[0], **ca[1])
 
                 else:
-                    go = creator
+                    go = creator  # type: ignore
                 return acr(self, orig_key, go, mutex)
 
         else:
             async_creator = None
 
         with Lock(
             self._mutex(key),
```

### Comparing `dogpile.cache-1.3.2/dogpile/cache/util.py` & `dogpile.cache-1.3.3/dogpile/cache/util.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/dogpile/core.py` & `dogpile.cache-1.3.3/dogpile/core.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/dogpile/lock.py` & `dogpile.cache-1.3.3/dogpile/lock.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/dogpile/testing/assertions.py` & `dogpile.cache-1.3.3/dogpile/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/dogpile/testing/fixtures.py` & `dogpile.cache-1.3.3/dogpile/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/dogpile/util/compat.py` & `dogpile.cache-1.3.3/dogpile/util/compat.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/dogpile/util/langhelpers.py` & `dogpile.cache-1.3.3/dogpile/util/langhelpers.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/dogpile/util/nameregistry.py` & `dogpile.cache-1.3.3/dogpile/util/nameregistry.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/dogpile/util/readwrite_lock.py` & `dogpile.cache-1.3.3/dogpile/util/readwrite_lock.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/dogpile.cache.egg-info/PKG-INFO` & `dogpile.cache-1.3.3/dogpile.cache.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dogpile.cache
-Version: 1.3.2
+Version: 1.3.3
 Summary: A caching front-end based on the Dogpile lock.
 Author-email: Mike Bayer <mike_mp@zzzcomputing.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sqlalchemy/dogpile.cache
 Project-URL: Documentation, https://dogpilecache.sqlalchemy.org
 Project-URL: Issue Tracker, https://github.com/sqlalchemy/dogpile.cache/
 Keywords: caching
```

### Comparing `dogpile.cache-1.3.2/dogpile.cache.egg-info/SOURCES.txt` & `dogpile.cache-1.3.3/dogpile.cache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/hash_port.py` & `dogpile.cache-1.3.3/hash_port.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/log_tests.ini` & `dogpile.cache-1.3.3/log_tests.ini`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/mypy.ini` & `dogpile.cache-1.3.3/mypy.ini`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/pyproject.toml` & `dogpile.cache-1.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/setup.py` & `dogpile.cache-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/tests/cache/plugins/test_mako_cache.py` & `dogpile.cache-1.3.3/tests/cache/plugins/test_mako_cache.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/tests/cache/test_dbm_backend.py` & `dogpile.cache-1.3.3/tests/cache/test_dbm_backend.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/tests/cache/test_decorator.py` & `dogpile.cache-1.3.3/tests/cache/test_decorator.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/tests/cache/test_memcached_backend.py` & `dogpile.cache-1.3.3/tests/cache/test_memcached_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -341,14 +341,24 @@
                     warn_mock.mock_calls[0],
                     mock.call(
                         "enable_retry_client is not set; retry options "
                         "will be ignored"
                     ),
                 )
 
+    def test_pymemcache_memacached_expire_time(self):
+        config_args = {"url": "127.0.0.1:11211", "memcached_expire_time": 20}
+        with self._mock_pymemcache_fixture():
+            backend = MockPyMemcacheBackend(config_args)
+            backend.set("foo", "bar")
+            eq_(
+                self.hash_client().set.mock_calls,
+                [mock.call("foo", "bar", expire=20)],
+            )
+
 
 class MemcachedTest(_NonDistributedMemcachedTestSuite):
     backend = "dogpile.cache.memcached"
 
 
 class MemcachedDistributedTest(_DistributedMemcachedTestSuite):
     backend = "dogpile.cache.memcached"
```

### Comparing `dogpile.cache-1.3.2/tests/cache/test_null_backend.py` & `dogpile.cache-1.3.3/tests/cache/test_null_backend.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/tests/cache/test_redis_backend.py` & `dogpile.cache-1.3.3/tests/cache/test_redis_backend.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/tests/cache/test_redis_sentinel_backend.py` & `dogpile.cache-1.3.3/tests/cache/test_redis_sentinel_backend.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/tests/cache/test_region.py` & `dogpile.cache-1.3.3/tests/cache/test_region.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 def key_mangler(key):
     return "HI!" + key
 
 
 class APITest:
     def test_no_value_str(self):
-        eq_(str(NO_VALUE), "<dogpile.cache.api.NoValue object>")
+        eq_(str(NO_VALUE), "NoValue.NO_VALUE")
 
 
 class RegionTest:
     def _region(self, init_args={}, config_args={}, backend="mock"):
         reg = CacheRegion(**init_args)
         reg.configure(backend, **config_args)
         return reg
```

### Comparing `dogpile.cache-1.3.2/tests/test_backgrounding.py` & `dogpile.cache-1.3.3/tests/test_backgrounding.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/tests/test_lock.py` & `dogpile.cache-1.3.3/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/tests/test_utils.py` & `dogpile.cache-1.3.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/tests/tls/ca-root.crt` & `dogpile.cache-1.3.3/tests/tls/ca-root.crt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/tests/tls/client-ca-root.crt` & `dogpile.cache-1.3.3/tests/tls/client-ca-root.crt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/tests/tls/client.crt` & `dogpile.cache-1.3.3/tests/tls/client.crt`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/tests/tls/client.key` & `dogpile.cache-1.3.3/tests/tls/client.key`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/tests/tls/generate/Makefile` & `dogpile.cache-1.3.3/tests/tls/generate/Makefile`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/tests/tls/generate/conf/ca-intermediate.conf` & `dogpile.cache-1.3.3/tests/tls/generate/conf/ca-intermediate.conf`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/tests/tls/generate/conf/ca-root.conf` & `dogpile.cache-1.3.3/tests/tls/generate/conf/ca-root.conf`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/tests/tls/generate/conf/client-ca-root.conf` & `dogpile.cache-1.3.3/tests/tls/generate/conf/client-ca-root.conf`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/tests/tls/generate/tool` & `dogpile.cache-1.3.3/tests/tls/generate/tool`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/tests/tls/server.key` & `dogpile.cache-1.3.3/tests/tls/server.key`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/tests/tls/server_chain.pem` & `dogpile.cache-1.3.3/tests/tls/server_chain.pem`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/tests/util/test_nameregistry.py` & `dogpile.cache-1.3.3/tests/util/test_nameregistry.py`

 * *Files identical despite different names*

### Comparing `dogpile.cache-1.3.2/tox.ini` & `dogpile.cache-1.3.3/tox.ini`

 * *Files identical despite different names*

