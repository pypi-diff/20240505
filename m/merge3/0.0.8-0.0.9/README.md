# Comparing `tmp/merge3-0.0.8.tar.gz` & `tmp/merge3-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merge3-0.0.8.tar", last modified: Sat Mar 13 13:36:08 2021, max compression
+gzip compressed data, was "merge3-0.0.9.tar", last modified: Sun Sep 25 01:10:04 2022, max compression
```

## Comparing `merge3-0.0.8.tar` & `merge3-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2021-03-13 13:36:08.884898 merge3-0.0.8/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2021-03-13 13:36:08.880898 merge3-0.0.8/.github/
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2021-03-13 13:36:08.880898 merge3-0.0.8/.github/workflows/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      918 2021-03-13 13:36:02.000000 merge3-0.0.8/.github/workflows/pythonpackage.yml
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       21 2021-03-13 13:36:02.000000 merge3-0.0.8/.gitignore
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      190 2021-03-13 13:36:02.000000 merge3-0.0.8/AUTHORS
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    18092 2021-03-13 13:36:02.000000 merge3-0.0.8/COPYING
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       51 2021-03-13 13:36:02.000000 merge3-0.0.8/MANIFEST.in
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1784 2021-03-13 13:36:08.884898 merge3-0.0.8/PKG-INFO
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      716 2021-03-13 13:36:02.000000 merge3-0.0.8/README.rst
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2021-03-13 13:36:08.884898 merge3-0.0.8/merge3/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    19128 2021-03-13 13:36:03.000000 merge3-0.0.8/merge3/__init__.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1807 2021-03-13 13:36:02.000000 merge3-0.0.8/merge3/__main__.py
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)    18395 2021-03-13 13:36:02.000000 merge3-0.0.8/merge3/test_merge3.py
-drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2021-03-13 13:36:08.884898 merge3-0.0.8/merge3.egg-info/
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1784 2021-03-13 13:36:08.000000 merge3-0.0.8/merge3.egg-info/PKG-INFO
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      288 2021-03-13 13:36:08.000000 merge3-0.0.8/merge3.egg-info/SOURCES.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)        1 2021-03-13 13:36:08.000000 merge3-0.0.8/merge3.egg-info/dependency_links.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)        7 2021-03-13 13:36:08.000000 merge3-0.0.8/merge3.egg-info/top_level.txt
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)      337 2021-03-13 13:36:02.000000 merge3-0.0.8/releaser.conf
--rw-r--r--   0 jelmer    (1000) jelmer    (1000)       38 2021-03-13 13:36:08.884898 merge3-0.0.8/setup.cfg
--rwxr-xr-x   0 jelmer    (1000) jelmer    (1000)     1167 2021-03-13 13:36:03.000000 merge3-0.0.8/setup.py
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2022-09-25 01:10:04.991914 merge3-0.0.9/
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2022-09-25 01:10:04.991914 merge3-0.0.9/.github/
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2022-09-25 01:10:04.991914 merge3-0.0.9/.github/workflows/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      839 2022-09-25 01:10:00.000000 merge3-0.0.9/.github/workflows/pythonpackage.yml
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       21 2022-09-25 01:10:00.000000 merge3-0.0.9/.gitignore
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      190 2022-09-25 01:10:00.000000 merge3-0.0.9/AUTHORS
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    18092 2022-09-25 01:10:00.000000 merge3-0.0.9/COPYING
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       51 2022-09-25 01:10:00.000000 merge3-0.0.9/MANIFEST.in
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1539 2022-09-25 01:10:04.991914 merge3-0.0.9/PKG-INFO
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      716 2022-09-25 01:10:00.000000 merge3-0.0.9/README.rst
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2022-09-25 01:10:04.991914 merge3-0.0.9/merge3/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    18336 2022-09-25 01:10:04.000000 merge3-0.0.9/merge3/__init__.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1767 2022-09-25 01:10:00.000000 merge3-0.0.9/merge3/__main__.py
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)        0 2022-09-25 01:10:00.000000 merge3-0.0.9/merge3/py.typed
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)    18418 2022-09-25 01:10:00.000000 merge3-0.0.9/merge3/test_merge3.py
+drwxr-xr-x   0 jelmer    (1000) jelmer    (1000)        0 2022-09-25 01:10:04.991914 merge3-0.0.9/merge3.egg-info/
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)     1539 2022-09-25 01:10:04.000000 merge3-0.0.9/merge3.egg-info/PKG-INFO
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      304 2022-09-25 01:10:04.000000 merge3-0.0.9/merge3.egg-info/SOURCES.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)        1 2022-09-25 01:10:04.000000 merge3-0.0.9/merge3.egg-info/dependency_links.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)        7 2022-09-25 01:10:04.000000 merge3-0.0.9/merge3.egg-info/top_level.txt
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)      389 2022-09-25 01:10:00.000000 merge3-0.0.9/releaser.conf
+-rw-r--r--   0 jelmer    (1000) jelmer    (1000)       38 2022-09-25 01:10:04.991914 merge3-0.0.9/setup.cfg
+-rwxr-xr-x   0 jelmer    (1000) jelmer    (1000)     1116 2022-09-25 01:10:04.000000 merge3-0.0.9/setup.py
```

### Comparing `merge3-0.0.8/.github/workflows/pythonpackage.yml` & `merge3-0.0.9/.github/workflows/pythonpackage.yml`

 * *Files 13% similar despite different names*

```diff
@@ -6,18 +6,15 @@
 jobs:
   build:
 
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: [2.7, 3.6, 3.7, 3.8, pypy3]
-        exclude:
-          - os: windows-latest
-            python-version: 2.7
+        python-version: [3.6, 3.7, 3.8, 3.9, '3.10']
       fail-fast: false
 
     steps:
       - uses: actions/checkout@v2
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
```

### Comparing `merge3-0.0.8/COPYING` & `merge3-0.0.9/COPYING`

 * *Files identical despite different names*

### Comparing `merge3-0.0.8/PKG-INFO` & `merge3-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 Metadata-Version: 2.1
 Name: merge3
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python implementation of 3-way merge.
 Home-page: https://www.breezy-vcs.org/
 Maintainer: Breezy Developers
 Maintainer-email: team@breezy-vcs.org
 License: GNU GPLv2 or later
-Description: A Python implementation of 3-way merge of texts.
-        
-        Given BASE, OTHER, THIS, tries to produce a combined text
-        incorporating the changes from both BASE->OTHER and BASE->THIS.
-        All three will typically be sequences of lines.
-        
-        Usage
-        =====
-        
-        From the command-line::
-        
-            $ echo foo > mine
-            $ echo bar > base
-            $ echo blah > other
-            $ python -m merge3 mine base other > merged
-            $ cat merged
-        
-        Or from Python::
-        
-            >>> import merge3
-            >>> m3 = merge3.Merge3(
-            ...                    ['common\n', 'base\n'],
-            ...                    ['common\n', 'a\n'],
-            ...                    ['common\n', 'b\n'])
-            >>> list(m3.merge_annotated())
-            ['u | common\n', '<<<<\n', 'A | a\n', '----\n', 'B | b\n', '>>>>\n']
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX
 Description-Content-Type: text/x-rst
+License-File: COPYING
+License-File: AUTHORS
+
+A Python implementation of 3-way merge of texts.
+
+Given BASE, OTHER, THIS, tries to produce a combined text
+incorporating the changes from both BASE->OTHER and BASE->THIS.
+All three will typically be sequences of lines.
+
+Usage
+=====
+
+From the command-line::
+
+    $ echo foo > mine
+    $ echo bar > base
+    $ echo blah > other
+    $ python -m merge3 mine base other > merged
+    $ cat merged
+
+Or from Python::
+
+    >>> import merge3
+    >>> m3 = merge3.Merge3(
+    ...                    ['common\n', 'base\n'],
+    ...                    ['common\n', 'a\n'],
+    ...                    ['common\n', 'b\n'])
+    >>> list(m3.merge_annotated())
+    ['u | common\n', '<<<<\n', 'A | a\n', '----\n', 'B | b\n', '>>>>\n']
```

### Comparing `merge3-0.0.8/README.rst` & `merge3-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `merge3-0.0.8/merge3/__init__.py` & `merge3-0.0.9/merge3/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,21 +10,20 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
 
-from __future__ import absolute_import
 
 # mbp: "you know that thing where cvs gives you conflict markers?"
 # s: "i hate that."
 
 
-__version__ = (0, 0, 8)
+__version__ = (0, 0, 9)
 
 
 class CantReprocessAndShowBase(Exception):
     """Can't reprocess and show base."""
 
 
 def intersect(ra, rb):
@@ -48,15 +47,15 @@
     else:
         return None
 
 
 def compare_range(a, astart, aend, b, bstart, bend):
     """Compare a[astart:aend] == b[bstart:bend], without slicing.
     """
-    if (aend-astart) != (bend-bstart):
+    if (aend - astart) != (bend - bstart):
         return False
     for ia, ib in zip(range(astart, aend), range(bstart, bend)):
         if a[ia] != b[ib]:
             return False
     else:
         return True
 
@@ -98,17 +97,17 @@
         else:
             return False
 
     def merge_lines(self,
                     name_a=None,
                     name_b=None,
                     name_base=None,
-                    start_marker='<<<<<<<',
-                    mid_marker='=======',
-                    end_marker='>>>>>>>',
+                    start_marker=None,
+                    mid_marker=None,
+                    end_marker=None,
                     base_marker=None,
                     reprocess=False):
         """Return merge in cvs-like form.
         """
         if base_marker and reprocess:
             raise CantReprocessAndShowBase()
         if self._uses_bytes():
@@ -117,50 +116,44 @@
                     newline = b'\r\n'
                 elif self.a[0].endswith(b'\r'):
                     newline = b'\r'
                 else:
                     newline = b'\n'
             else:
                 newline = b'\n'
-            if isinstance(start_marker, str):
-                start_marker = start_marker.encode()
-            if isinstance(end_marker, str):
-                end_marker = end_marker.encode()
-            if isinstance(mid_marker, str):
-                mid_marker = mid_marker.encode()
-            if base_marker is not None and isinstance(base_marker, str):
-                base_marker = base_marker.encode()
-            if name_a:
-                if isinstance(name_a, str):
-                    name_a = name_a.encode()
-                start_marker = start_marker + b' ' + name_a
-            if name_b:
-                if isinstance(name_b, str):
-                    name_b = name_b.encode()
-                end_marker = end_marker + b' ' + name_b
-            if name_base and base_marker:
-                if isinstance(name_base, str):
-                    name_base = name_base.encode()
-                base_marker = base_marker + b' ' + name_base
+            if start_marker is None:
+                start_marker = b'<<<<<<<'
+            if mid_marker is None:
+                mid_marker = b'======='
+            if end_marker is None:
+                end_marker = b'>>>>>>>'
+            space = b' '
         else:
+            if start_marker is None:
+                start_marker = '<<<<<<<'
+            if mid_marker is None:
+                mid_marker = '======='
+            if end_marker is None:
+                end_marker = '>>>>>>>'
             if len(self.a) > 0:
                 if self.a[0].endswith('\r\n'):
                     newline = '\r\n'
                 elif self.a[0].endswith('\r'):
                     newline = '\r'
                 else:
                     newline = '\n'
             else:
                 newline = '\n'
-            if name_a:
-                start_marker = start_marker + ' ' + name_a
-            if name_b:
-                end_marker = end_marker + ' ' + name_b
-            if name_base and base_marker:
-                base_marker = base_marker + ' ' + name_base
+            space = ' '
+        if name_a:
+            start_marker = start_marker + space + name_a
+        if name_b:
+            end_marker = end_marker + space + name_b
+        if name_base and base_marker:
+            base_marker = base_marker + space + name_base
         merge_regions = self.merge_regions()
         if reprocess is True:
             merge_regions = self.reprocess_merge_regions(merge_regions)
         for t in merge_regions:
             what = t[0]
             if what == 'unchanged':
                 for i in range(t[1], t[2]):
@@ -187,29 +180,30 @@
                 raise ValueError(what)
 
     def merge_annotated(self):
         """Return merge with conflicts, showing origin of lines.
 
         Most useful for debugging merge.
         """
-        UNCHANGED = 'u'
-        SEP = ' | '
-        CONFLICT_START = '<<<<\n'
-        CONFLICT_MID = '----\n'
-        CONFLICT_END = '>>>>\n'
-        WIN_A = 'a'
-        WIN_B = 'b'
         if self._uses_bytes():
-            UNCHANGED = UNCHANGED.encode()
-            SEP = SEP.encode()
-            CONFLICT_START = CONFLICT_START.encode()
-            CONFLICT_MID = CONFLICT_MID.encode()
-            CONFLICT_END = CONFLICT_END.encode()
-            WIN_A = WIN_A.encode()
-            WIN_B = WIN_B.encode()
+            UNCHANGED = b'u'
+            SEP = b' | '
+            CONFLICT_START = b'<<<<\n'
+            CONFLICT_MID = b'----\n'
+            CONFLICT_END = b'>>>>\n'
+            WIN_A = b'a'
+            WIN_B = b'b'
+        else:
+            UNCHANGED = 'u'
+            SEP = ' | '
+            CONFLICT_START = '<<<<\n'
+            CONFLICT_MID = '----\n'
+            CONFLICT_END = '>>>>\n'
+            WIN_A = 'a'
+            WIN_B = 'b'
 
         for t in self.merge_regions():
             what = t[0]
             if what == 'unchanged':
                 for i in range(t[1], t[2]):
                     yield UNCHANGED + SEP + self.base[i]
             elif what == 'a' or what == 'same':
@@ -298,19 +292,17 @@
             matchlen = zend - zmatch
             # invariants:
             #   matchlen >= 0
             #   matchlen == (aend - amatch)
             #   matchlen == (bend - bmatch)
             len_a = amatch - ia
             len_b = bmatch - ib
-            # len_base = zmatch - iz
             # invariants:
             # assert len_a >= 0
             # assert len_b >= 0
-            # assert len_base >= 0
 
             # print 'unmatched a=%d, b=%d' % (len_a, len_b)
 
             if len_a or len_b:
                 # try to avoid actually slicing the lists
                 same = compare_range(self.a, ia, amatch,
                                      self.b, ib, bmatch)
@@ -325,16 +317,16 @@
                     if equal_a and not equal_b:
                         yield 'b', ib, bmatch
                     elif equal_b and not equal_a:
                         yield 'a', ia, amatch
                     elif not equal_a and not equal_b:
                         if self.is_cherrypick:
                             for node in self._refine_cherrypick_conflict(
-                                                    iz, zmatch, ia, amatch,
-                                                    ib, bmatch):
+                                    iz, zmatch, ia, amatch,
+                                    ib, bmatch):
                                 yield node
                         else:
                             yield (
                                 'conflict', iz, zmatch, ia, amatch, ib, bmatch)
                     else:
                         raise AssertionError(
                             "can't handle a=b=base but unmatched")
@@ -365,17 +357,15 @@
             None, self.base[zstart:zend], self.b[bstart:bend])
         matches = matcher.get_matching_blocks()
         last_base_idx = 0
         last_b_idx = 0
         last_b_idx = 0
         yielded_a = False
         for base_idx, b_idx, match_len in matches:
-            # conflict_z_len = base_idx - last_base_idx
             conflict_b_len = b_idx - last_b_idx
-            # There are no lines in b which conflict, so skip it
             if conflict_b_len == 0:
                 pass
             else:
                 if yielded_a:
                     yield ('conflict',
                            zstart + last_base_idx, zstart + base_idx,
                            aend, aend, bstart + last_b_idx, bstart + b_idx)
@@ -409,60 +399,60 @@
             if region[0] != "conflict":
                 yield region
                 continue
             type, iz, zmatch, ia, amatch, ib, bmatch = region
             a_region = self.a[ia:amatch]
             b_region = self.b[ib:bmatch]
             matches = self.sequence_matcher(
-                    None, a_region, b_region).get_matching_blocks()
+                None, a_region, b_region).get_matching_blocks()
             next_a = ia
             next_b = ib
             for region_ia, region_ib, region_len in matches[:-1]:
                 region_ia += ia
                 region_ib += ib
                 reg = self.mismatch_region(next_a, region_ia, next_b,
                                            region_ib)
                 if reg is not None:
                     yield reg
-                yield 'same', region_ia, region_len+region_ia
+                yield 'same', region_ia, region_len + region_ia
                 next_a = region_ia + region_len
                 next_b = region_ib + region_len
             reg = self.mismatch_region(next_a, amatch, next_b, bmatch)
             if reg is not None:
                 yield reg
 
     @staticmethod
-    def mismatch_region(next_a, region_ia,  next_b, region_ib):
+    def mismatch_region(next_a, region_ia, next_b, region_ib):
         if next_a < region_ia or next_b < region_ib:
             return 'conflict', None, None, next_a, region_ia, next_b, region_ib
 
     def find_sync_regions(self):
-        """Return a list of sync regions, where both descendents match the base.
+        """Return list of sync regions, where both descendents match the base.
 
         Generates a list of (base1, base2, a1, a2, b1, b2).  There is
         always a zero-length sync region at the end of all the files.
         """
 
         ia = ib = 0
         amatches = self.sequence_matcher(
-                None, self.base, self.a).get_matching_blocks()
+            None, self.base, self.a).get_matching_blocks()
         bmatches = self.sequence_matcher(
-                None, self.base, self.b).get_matching_blocks()
+            None, self.base, self.b).get_matching_blocks()
         len_a = len(amatches)
         len_b = len(bmatches)
 
         sl = []
 
         while ia < len_a and ib < len_b:
             abase, amatch, alen = amatches[ia]
             bbase, bmatch, blen = bmatches[ib]
 
             # there is an unconflicted block at i; how long does it
             # extend?  until whichever one ends earlier.
-            i = intersect((abase, abase+alen), (bbase, bbase+blen))
+            i = intersect((abase, abase + alen), (bbase, bbase + blen))
             if i:
                 intbase = i[0]
                 intend = i[1]
                 intlen = intend - intbase
 
                 # found a match of base[i[0], i[1]]; this may be less than
                 # the region that matches in either one
@@ -495,17 +485,17 @@
         sl.append((intbase, intbase, abase, abase, bbase, bbase))
 
         return sl
 
     def find_unconflicted(self):
         """Return a list of ranges in base that are not conflicted."""
         am = self.sequence_matcher(
-                None, self.base, self.a).get_matching_blocks()
+            None, self.base, self.a).get_matching_blocks()
         bm = self.sequence_matcher(
-                None, self.base, self.b).get_matching_blocks()
+            None, self.base, self.b).get_matching_blocks()
 
         unc = []
 
         while am and bm:
             # there is an unconflicted block at i; how long does it
             # extend?  until whichever one ends earlier.
             a1 = am[0][0]
```

### Comparing `merge3-0.0.8/merge3/__main__.py` & `merge3-0.0.9/merge3/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
 
-from __future__ import absolute_import
-
 from . import Merge3
 
 
 def main(argv):
     import argparse
 
     parser = argparse.ArgumentParser()
```

### Comparing `merge3-0.0.8/merge3/test_merge3.py` & `merge3-0.0.9/merge3/test_merge3.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,16 @@
      But after they are produced,
        they have different names.
 
        -- The Way of Lao-Tzu, tr. Wing-tsit Chan
 
 """)
 
-MERGED_RESULT = split_lines("""     The Way that can be told of is not the eternal Way;
+MERGED_RESULT = split_lines(
+    """     The Way that can be told of is not the eternal Way;
      The name that can be named is not the eternal name.
      The Nameless is the origin of Heaven and Earth;
      The Named is the mother of all things.
      Therefore let there always be non-being,
        so we may see their subtlety,
      And let there always be being,
        so we may see their result.
@@ -305,15 +306,15 @@
 
     def test_merge_poem_bytes(self):
         """Test case from diff3 manual"""
         m3 = merge3.Merge3(
             [line.encode() for line in TZU],
             [line.encode() for line in LAO],
             [line.encode() for line in TAO])
-        ml = list(m3.merge_lines('LAO', 'TAO'))
+        ml = list(m3.merge_lines('LAO'.encode(), 'TAO'.encode()))
         self.assertEqual(
             ml, [line.encode() for line in MERGED_RESULT])
 
     def test_minimal_conflicts_common(self):
         """Reprocessing"""
         base_text = ("a\n" * 20).splitlines(True)
         this_text = ("a\n"*10 + "b\n" * 10).splitlines(True)
```

### Comparing `merge3-0.0.8/merge3.egg-info/PKG-INFO` & `merge3-0.0.9/merge3.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 Metadata-Version: 2.1
 Name: merge3
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python implementation of 3-way merge.
 Home-page: https://www.breezy-vcs.org/
 Maintainer: Breezy Developers
 Maintainer-email: team@breezy-vcs.org
 License: GNU GPLv2 or later
-Description: A Python implementation of 3-way merge of texts.
-        
-        Given BASE, OTHER, THIS, tries to produce a combined text
-        incorporating the changes from both BASE->OTHER and BASE->THIS.
-        All three will typically be sequences of lines.
-        
-        Usage
-        =====
-        
-        From the command-line::
-        
-            $ echo foo > mine
-            $ echo bar > base
-            $ echo blah > other
-            $ python -m merge3 mine base other > merged
-            $ cat merged
-        
-        Or from Python::
-        
-            >>> import merge3
-            >>> m3 = merge3.Merge3(
-            ...                    ['common\n', 'base\n'],
-            ...                    ['common\n', 'a\n'],
-            ...                    ['common\n', 'b\n'])
-            >>> list(m3.merge_annotated())
-            ['u | common\n', '<<<<\n', 'A | a\n', '----\n', 'B | b\n', '>>>>\n']
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX
 Description-Content-Type: text/x-rst
+License-File: COPYING
+License-File: AUTHORS
+
+A Python implementation of 3-way merge of texts.
+
+Given BASE, OTHER, THIS, tries to produce a combined text
+incorporating the changes from both BASE->OTHER and BASE->THIS.
+All three will typically be sequences of lines.
+
+Usage
+=====
+
+From the command-line::
+
+    $ echo foo > mine
+    $ echo bar > base
+    $ echo blah > other
+    $ python -m merge3 mine base other > merged
+    $ cat merged
+
+Or from Python::
+
+    >>> import merge3
+    >>> m3 = merge3.Merge3(
+    ...                    ['common\n', 'base\n'],
+    ...                    ['common\n', 'a\n'],
+    ...                    ['common\n', 'b\n'])
+    >>> list(m3.merge_annotated())
+    ['u | common\n', '<<<<\n', 'A | a\n', '----\n', 'B | b\n', '>>>>\n']
```

### Comparing `merge3-0.0.8/setup.py` & `merge3-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,25 +6,24 @@
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
 setup(name="merge3",
       description="Python implementation of 3-way merge.",
       long_description=long_description,
       long_description_content_type='text/x-rst',
-      version="0.0.8",
+      version="0.0.9",
       maintainer="Breezy Developers",
       maintainer_email="team@breezy-vcs.org",
       license="GNU GPLv2 or later",
       url="https://www.breezy-vcs.org/",
       packages=['merge3'],
       test_suite='merge3.test_merge3',
       classifiers=[
           'Development Status :: 4 - Beta',
           'License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)',  # noqa
-          'Programming Language :: Python :: 2.7',
           'Programming Language :: Python :: 3.3',
           'Programming Language :: Python :: 3.4',
           'Programming Language :: Python :: 3.5',
           'Programming Language :: Python :: 3.6',
           'Programming Language :: Python :: Implementation :: CPython',
           'Programming Language :: Python :: Implementation :: PyPy',
           'Operating System :: POSIX',
```

