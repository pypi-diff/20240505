# Comparing `tmp/seqlogic-0.0.8.tar.gz` & `tmp/seqlogic-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqlogic-0.0.8.tar", last modified: Mon Apr 29 04:37:57 2024, max compression
+gzip compressed data, was "seqlogic-0.0.9.tar", last modified: Sun May  5 19:09:58 2024, max compression
```

## Comparing `seqlogic-0.0.8.tar` & `seqlogic-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 04:37:57.900610 seqlogic-0.0.8/
--rw-rw-rw-   0        0        0      956 2024-04-29 04:37:57.900610 seqlogic-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      740 2024-03-11 04:13:25.000000 seqlogic-0.0.8/README.md
--rw-rw-rw-   0        0        0      263 2024-04-29 04:35:17.000000 seqlogic-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-29 04:37:57.900610 seqlogic-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-29 04:37:57.820661 seqlogic-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 04:37:57.850142 seqlogic-0.0.8/src/seqlogic/
--rw-rw-rw-   0        0        0      399 2024-04-29 04:32:29.000000 seqlogic-0.0.8/src/seqlogic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 04:37:57.874767 seqlogic-0.0.8/src/seqlogic/algorithms/
--rw-rw-rw-   0        0        0       27 2023-11-27 07:28:50.000000 seqlogic-0.0.8/src/seqlogic/algorithms/__init__.py
--rw-rw-rw-   0        0        0    12685 2024-03-10 17:38:01.000000 seqlogic-0.0.8/src/seqlogic/algorithms/aes.py
--rw-rw-rw-   0        0        0      285 2024-04-29 04:32:28.000000 seqlogic-0.0.8/src/seqlogic/algorithms/gray.py
--rw-rw-rw-   0        0        0    21726 2024-04-29 04:32:29.000000 seqlogic-0.0.8/src/seqlogic/bits.py
--rw-rw-rw-   0        0        0     7331 2024-04-29 04:32:29.000000 seqlogic-0.0.8/src/seqlogic/design.py
--rw-rw-rw-   0        0        0     2981 2024-04-01 05:33:29.000000 seqlogic-0.0.8/src/seqlogic/hier.py
--rw-rw-rw-   0        0        0    75435 2024-04-29 04:32:29.000000 seqlogic-0.0.8/src/seqlogic/lbool.py
--rw-rw-rw-   0        0        0    14107 2024-04-29 04:32:29.000000 seqlogic-0.0.8/src/seqlogic/sim.py
--rw-rw-rw-   0        0        0     1215 2023-11-27 07:28:50.000000 seqlogic-0.0.8/src/seqlogic/util.py
-drwxrwxrwx   0        0        0        0 2024-04-29 04:37:57.900610 seqlogic-0.0.8/src/seqlogic.egg-info/
--rw-rw-rw-   0        0        0      956 2024-04-29 04:37:57.000000 seqlogic-0.0.8/src/seqlogic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      630 2024-04-29 04:37:57.000000 seqlogic-0.0.8/src/seqlogic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 04:37:57.000000 seqlogic-0.0.8/src/seqlogic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-29 04:37:57.000000 seqlogic-0.0.8/src/seqlogic.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-29 04:37:57.900610 seqlogic-0.0.8/tests/
--rw-rw-rw-   0        0        0     4281 2024-03-09 21:03:27.000000 seqlogic-0.0.8/tests/test_aes.py
--rw-rw-rw-   0        0        0    24106 2024-04-28 01:11:05.000000 seqlogic-0.0.8/tests/test_bits.py
--rw-rw-rw-   0        0        0     1991 2024-04-29 04:32:29.000000 seqlogic-0.0.8/tests/test_enum.py
--rw-rw-rw-   0        0        0     4713 2024-04-29 04:32:29.000000 seqlogic-0.0.8/tests/test_fsm.py
--rw-rw-rw-   0        0        0      684 2024-04-21 07:30:53.000000 seqlogic-0.0.8/tests/test_gray.py
--rw-rw-rw-   0        0        0      705 2024-03-11 02:48:00.000000 seqlogic-0.0.8/tests/test_hier.py
--rw-rw-rw-   0        0        0    22816 2024-04-29 04:32:29.000000 seqlogic-0.0.8/tests/test_lbool.py
--rw-rw-rw-   0        0        0     3514 2024-04-29 04:32:29.000000 seqlogic-0.0.8/tests/test_lfsr.py
--rw-rw-rw-   0        0        0    29052 2024-04-29 04:32:29.000000 seqlogic-0.0.8/tests/test_riscv.py
--rw-rw-rw-   0        0        0     4299 2024-04-29 04:32:29.000000 seqlogic-0.0.8/tests/test_sim.py
--rw-rw-rw-   0        0        0     1865 2024-04-29 04:32:29.000000 seqlogic-0.0.8/tests/test_struct.py
+drwxrwxrwx   0        0        0        0 2024-05-05 19:09:58.483721 seqlogic-0.0.9/
+-rw-rw-rw-   0        0        0      956 2024-05-05 19:09:58.482539 seqlogic-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      740 2024-03-11 04:13:25.000000 seqlogic-0.0.9/README.md
+-rw-rw-rw-   0        0        0      263 2024-05-05 19:09:14.000000 seqlogic-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-05 19:09:58.484723 seqlogic-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-05 19:09:58.418208 seqlogic-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-05-05 19:09:58.434033 seqlogic-0.0.9/src/seqlogic/
+-rw-rw-rw-   0        0        0      357 2024-05-05 19:08:40.000000 seqlogic-0.0.9/src/seqlogic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 19:09:58.461745 seqlogic-0.0.9/src/seqlogic/algorithms/
+-rw-rw-rw-   0        0        0       27 2023-11-27 07:28:50.000000 seqlogic-0.0.9/src/seqlogic/algorithms/__init__.py
+-rw-rw-rw-   0        0        0    12685 2024-03-10 17:38:01.000000 seqlogic-0.0.9/src/seqlogic/algorithms/aes.py
+-rw-rw-rw-   0        0        0      285 2024-04-30 03:11:09.000000 seqlogic-0.0.9/src/seqlogic/algorithms/gray.py
+-rw-rw-rw-   0        0        0    21662 2024-05-05 19:08:40.000000 seqlogic-0.0.9/src/seqlogic/bits.py
+-rw-rw-rw-   0        0        0     7609 2024-05-05 19:08:40.000000 seqlogic-0.0.9/src/seqlogic/design.py
+-rw-rw-rw-   0        0        0     2981 2024-04-01 05:33:29.000000 seqlogic-0.0.9/src/seqlogic/hier.py
+-rw-rw-rw-   0        0        0    80210 2024-05-05 19:08:40.000000 seqlogic-0.0.9/src/seqlogic/lbool.py
+-rw-rw-rw-   0        0        0    13702 2024-05-05 19:08:40.000000 seqlogic-0.0.9/src/seqlogic/sim.py
+-rw-rw-rw-   0        0        0     1368 2024-05-05 19:08:40.000000 seqlogic-0.0.9/src/seqlogic/util.py
+drwxrwxrwx   0        0        0        0 2024-05-05 19:09:58.479748 seqlogic-0.0.9/src/seqlogic.egg-info/
+-rw-rw-rw-   0        0        0      956 2024-05-05 19:09:58.000000 seqlogic-0.0.9/src/seqlogic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      630 2024-05-05 19:09:58.000000 seqlogic-0.0.9/src/seqlogic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 19:09:58.000000 seqlogic-0.0.9/src/seqlogic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-05 19:09:58.000000 seqlogic-0.0.9/src/seqlogic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-05 19:09:58.478746 seqlogic-0.0.9/tests/
+-rw-rw-rw-   0        0        0     4281 2024-05-05 07:44:15.000000 seqlogic-0.0.9/tests/test_aes.py
+-rw-rw-rw-   0        0        0    24103 2024-05-05 19:08:40.000000 seqlogic-0.0.9/tests/test_bits.py
+-rw-rw-rw-   0        0        0     2583 2024-05-05 19:08:40.000000 seqlogic-0.0.9/tests/test_enum.py
+-rw-rw-rw-   0        0        0     4731 2024-05-05 19:08:40.000000 seqlogic-0.0.9/tests/test_fsm.py
+-rw-rw-rw-   0        0        0      684 2024-04-21 07:30:53.000000 seqlogic-0.0.9/tests/test_gray.py
+-rw-rw-rw-   0        0        0      705 2024-03-11 02:48:00.000000 seqlogic-0.0.9/tests/test_hier.py
+-rw-rw-rw-   0        0        0    27044 2024-05-05 19:08:40.000000 seqlogic-0.0.9/tests/test_lbool.py
+-rw-rw-rw-   0        0        0     3533 2024-05-05 19:08:40.000000 seqlogic-0.0.9/tests/test_lfsr.py
+-rw-rw-rw-   0        0        0    29052 2024-04-30 03:11:09.000000 seqlogic-0.0.9/tests/test_riscv.py
+-rw-rw-rw-   0        0        0     4327 2024-05-05 19:08:40.000000 seqlogic-0.0.9/tests/test_sim.py
+-rw-rw-rw-   0        0        0     2456 2024-05-05 19:08:40.000000 seqlogic-0.0.9/tests/test_struct.py
```

### Comparing `seqlogic-0.0.8/PKG-INFO` & `seqlogic-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqlogic
-Version: 0.0.8
+Version: 0.0.9
 Summary: Sequential Logic
 Project-URL: Repository, https://github.com/cjdrake/seqlogic.git
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Sequential Logic
```

### Comparing `seqlogic-0.0.8/README.md` & `seqlogic-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.8/src/seqlogic/algorithms/aes.py` & `seqlogic-0.0.9/src/seqlogic/algorithms/aes.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.8/src/seqlogic/bits.py` & `seqlogic-0.0.9/src/seqlogic/bits.py`

 * *Files 2% similar despite different names*

```diff
@@ -322,29 +322,29 @@
 
         Returns:
             Boolean result of unsigned(self) < unsigned(other)
 
         Raises:
             ValueError: bit array sizes do not match.
         """
-        return self._v.ult(other._v)
+        return bool(self._v.ltu(other._v))
 
     def slt(self, other: Bits) -> bool:
         """Signed less than.
 
         Args:
             other: bit array of equal size.
 
         Returns:
             Boolean result of signed(self) < signed(other)
 
         Raises:
             ValueError: bit array sizes do not match.
         """
-        return self._v.slt(other._v)
+        return bool(self._v.lt(other._v))
 
     def zext(self, n: int) -> Bits:
         """Return bit array zero extended by n bits.
 
         Zero extension is defined for 1-D vectors.
         Vectors of higher dimensions will be flattened, then zero extended.
         """
@@ -426,51 +426,51 @@
                 else:
                     n = n.to_uint()
             case _:
                 raise TypeError("Expected n to be int or Bits")
         y, co = self._v.arsh(n)
         return _v2b(y), _v2b(co)
 
-    def add(self, other: Bits, ci: Bits[1]) -> tuple[Bits, Bits[1], Bits[1]]:
+    def add(self, other: Bits, ci: Bits[1]) -> tuple[Bits, Bits[1]]:
         """Twos complement additions.
 
         Args:
             other: bit array of equal size.
 
         Returns:
             3-tuple of (sum, carry-out, overflow).
 
         Raises:
             ValueError: bit array lengths are invalid/inconsistent.
         """
-        s, co, ovf = self._v.add(other._v, ci._v)
-        return _v2b(s), _v2b(co), _v2b(ovf)
+        s, co = self._v.add(other._v, ci._v)
+        return _v2b(s), _v2b(co)
 
-    def sub(self, other: Bits) -> tuple[Bits, Bits[1], Bits[1]]:
+    def sub(self, other: Bits) -> tuple[Bits, Bits[1]]:
         """Twos complement subtraction.
 
         Args:
             other: bit array of equal size.
 
         Raises:
             ValueError: bit array lengths are invalid/inconsistent.
         """
-        s, co, ovf = self._v.sub(other._v)
-        return _v2b(s), _v2b(co), _v2b(ovf)
+        s, co = self._v.sub(other._v)
+        return _v2b(s), _v2b(co)
 
-    def neg(self) -> tuple[Bits, Bits[1], Bits[1]]:
+    def neg(self) -> tuple[Bits, Bits[1]]:
         """Twos complement negation.
 
         Computed using 0 - self.
 
         Returns:
             3-tuple of (sum, carry-out, overflow).
         """
-        s, co, ovf = self._v.neg()
-        return _v2b(s), _v2b(co), _v2b(ovf)
+        s, co = self._v.neg()
+        return _v2b(s), _v2b(co)
 
     def _check_shape(self, other: Bits):
         if self._shape != other.shape:
             s = f"Expected shape {self._shape}, got {other.shape}"
             raise ValueError(s)
 
     def _to_lit(self) -> str:
```

### Comparing `seqlogic-0.0.8/src/seqlogic/hier.py` & `seqlogic-0.0.9/src/seqlogic/hier.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.8/src/seqlogic/lbool.py` & `seqlogic-0.0.9/src/seqlogic/lbool.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 from __future__ import annotations
 
 import re
 from collections.abc import Generator, Iterable
 from functools import cached_property, partial
 
-from .util import clog2
+from .util import classproperty, clog2
 
 _ITEM_BITS = 2
 _ITEM_MASK = 0b11
 
 # Scalars
 _X = 0b00
 _0 = 0b01
@@ -317,14 +317,27 @@
         if n < 0:
             raise ValueError(f"Expected n ≥ 0, got {n}")
 
         if (vec_n := _VecN.get(n)) is None:
             _VecN[n] = vec_n = type(f"Vec[{n}]", (Vec,), {"_n": n})
         return vec_n
 
+    @classproperty
+    def nbits(cls):  # pylint: disable=no-self-argument
+        """Number of bits of data."""
+        return _ITEM_BITS * cls._n
+
+    @classmethod
+    def xes(cls):
+        return cls(0)
+
+    @classmethod
+    def dcs(cls):
+        return cls((1 << cls.nbits) - 1)
+
     def __init__(self, data: int):
         """Initialize.
 
         Args:
             data: lbool items packed into an int.
 
         Raises:
@@ -418,19 +431,14 @@
         return self.neg()[0]
 
     @property
     def data(self) -> int:
         """Packed items."""
         return self._data
 
-    @cached_property
-    def nbits(self) -> int:
-        """Number of bits of data."""
-        return _ITEM_BITS * self._n
-
     def not_(self) -> Vec:
         """Bitwise lifted NOT.
 
         Returns:
             vec of equal length and inverted data.
         """
         x_0 = self._bit_mask[0]
@@ -709,43 +717,187 @@
         if self._n == 0:
             return 0
         sign = self._get_item(self._n - 1)
         if sign == _1:
             return -(self.not_().to_uint() + 1)
         return self.to_uint()
 
-    def ult(self, other: Vec) -> bool:
-        """Unsigned less than.
+    def eq(self, other: Vec) -> Vec[1]:
+        """Equal operator.
 
         Args:
             other: vec of equal length.
 
         Returns:
-            Boolean result of unsigned(self) < unsigned(other)
+            Vec[1] result of self == other
+        """
+        self._check_len(other)
+        try:
+            return (_Vec0, _Vec1)[self.to_uint() == other.to_uint()]
+        except ValueError:
+            return _VecX
 
-        Raises:
-            ValueError: vec lengths do not match.
+    def neq(self, other: Vec) -> Vec[1]:
+        """Not Equal operator.
+
+        Args:
+            other: vec of equal length.
+
+        Returns:
+            Vec[1] result of self != other
         """
         self._check_len(other)
-        return self.to_uint() < other.to_uint()
+        try:
+            return (_Vec0, _Vec1)[self.to_uint() != other.to_uint()]
+        except ValueError:
+            return _VecX
 
-    def slt(self, other: Vec) -> bool:
-        """Signed less than.
+    def ltu(self, other: Vec) -> Vec[1]:
+        """Less than operator (unsigned).
 
         Args:
             other: vec of equal length.
 
         Returns:
-            Boolean result of signed(self) < signed(other)
+            Vec[1] result of unsigned(self) < unsigned(other)
+        """
+        self._check_len(other)
+        try:
+            return (_Vec0, _Vec1)[self.to_uint() < other.to_uint()]
+        except ValueError:
+            return _VecX
 
-        Raises:
-            ValueError: vec lengths do not match.
+    def lteu(self, other: Vec) -> Vec[1]:
+        """Less than or equal operator (unsigned).
+
+        Args:
+            other: vec of equal length.
+
+        Returns:
+            Vec[1] result of unsigned(self) ≤ unsigned(other)
+        """
+        self._check_len(other)
+        try:
+            return (_Vec0, _Vec1)[self.to_uint() <= other.to_uint()]
+        except ValueError:
+            return _VecX
+
+    def lt(self, other: Vec) -> Vec[1]:
+        """Less than operator (signed).
+
+        Args:
+            other: vec of equal length.
+
+        Returns:
+            Vec[1] result of signed(self) < signed(other)
+        """
+        self._check_len(other)
+        try:
+            return (_Vec0, _Vec1)[self.to_int() < other.to_int()]
+        except ValueError:
+            return _VecX
+
+    def lte(self, other: Vec) -> Vec[1]:
+        """Less than or equal operator (signed).
+
+        Args:
+            other: vec of equal length.
+
+        Returns:
+            Vec[1] result of signed(self) ≤ signed(other)
+        """
+        self._check_len(other)
+        try:
+            return (_Vec0, _Vec1)[self.to_int() <= other.to_int()]
+        except ValueError:
+            return _VecX
+
+    def gtu(self, other: Vec) -> Vec[1]:
+        """Greater than operator (unsigned).
+
+        Args:
+            other: vec of equal length.
+
+        Returns:
+            Vec[1] result of unsigned(self) > unsigned(other)
+        """
+        self._check_len(other)
+        try:
+            return (_Vec0, _Vec1)[self.to_uint() > other.to_uint()]
+        except ValueError:
+            return _VecX
+
+    def gteu(self, other: Vec) -> Vec[1]:
+        """Greater than or equal operator (unsigned).
+
+        Args:
+            other: vec of equal length.
+
+        Returns:
+            Vec[1] result of unsigned(self) ≥ unsigned(other)
+        """
+        self._check_len(other)
+        try:
+            return (_Vec0, _Vec1)[self.to_uint() >= other.to_uint()]
+        except ValueError:
+            return _VecX
+
+    def gt(self, other: Vec) -> Vec[1]:
+        """Greater than operator (signed).
+
+        Args:
+            other: vec of equal length.
+
+        Returns:
+            Vec[1] result of signed(self) > signed(other)
+        """
+        self._check_len(other)
+        try:
+            return (_Vec0, _Vec1)[self.to_int() > other.to_int()]
+        except ValueError:
+            return _VecX
+
+    def gte(self, other: Vec) -> Vec[1]:
+        """Greater than or equal operator (signed).
+
+        Args:
+            other: vec of equal length.
+
+        Returns:
+            Vec[1] result of signed(self) ≥ signed(other)
         """
         self._check_len(other)
-        return self.to_int() < other.to_int()
+        try:
+            return (_Vec0, _Vec1)[self.to_int() >= other.to_int()]
+        except ValueError:
+            return _VecX
+
+    def match(self, pattern: str | Vec) -> Vec[1]:
+        """Pattern match operator."""
+        match pattern:
+            case str() as lit:
+                pattern = lit2vec(lit)
+            case Vec():
+                pass
+            case _:
+                raise TypeError("Expected pattern to be str or Vec")
+
+        self._check_len(pattern)
+
+        # Propagate X
+        if self.has_x() or pattern.has_x():
+            return _VecX
+
+        for i in range(self._n):
+            a = self._get_item(i)
+            b = pattern._get_item(i)
+            # Mismatch on (0b01, 0b10) or (0b10, 0b01)
+            if a ^ b == 0b11:
+                return _Vec0
+        return _Vec1
 
     def zext(self, n: int) -> Vec:
         """Zero extend by n bits.
 
         Args:
             n: Non-negative number of bits.
 
@@ -755,16 +907,15 @@
         Raises:
             ValueError: If n is negative.
         """
         if n < 0:
             raise ValueError(f"Expected n ≥ 0, got {n}")
         if n == 0:
             return self
-        prefix = _fill(_0, n)
-        return Vec[self._n + n](self._data | (prefix << self.nbits))
+        return Vec[self._n + n](self._data | (_fill(_0, n) << self.nbits))
 
     def sext(self, n: int) -> Vec:
         """Sign extend by n bits.
 
         Args:
             n: Non-negative number of bits.
 
@@ -775,16 +926,15 @@
             ValueError: If n is negative.
         """
         if n < 0:
             raise ValueError(f"Expected n ≥ 0, got {n}")
         if n == 0:
             return self
         sign = self._get_item(self._n - 1)
-        prefix = _fill(sign, n)
-        return Vec[self._n + n](self._data | (prefix << self.nbits))
+        return Vec[self._n + n](self._data | (_fill(sign, n) << self.nbits))
 
     def lsh(self, n: int | Vec, ci: Vec[1] | None = None) -> tuple[Vec, Vec]:
         """Left shift by n bits.
 
         Args:
             n: Non-negative number of bits.
             ci: Optional "carry in"
@@ -797,17 +947,17 @@
             ValueError: If n or ci are invalid/inconsistent.
         """
         match n:
             case int():
                 pass
             case Vec():
                 if n.has_x():
-                    return xes(self._n), _VecE
+                    return self.xes(), _VecE
                 elif n.has_dc():
-                    return dcs(self._n), _VecE
+                    return self.dcs(), _VecE
                 else:
                     n = n.to_uint()
             case _:
                 raise TypeError("Expected n to be int or Vec")
         if not 0 <= n <= self._n:
             raise ValueError(f"Expected 0 ≤ n ≤ {self._n}, got {n}")
         if n == 0:
@@ -835,17 +985,17 @@
             ValueError: If n or ci are invalid/inconsistent.
         """
         match n:
             case int():
                 pass
             case Vec():
                 if n.has_x():
-                    return xes(self._n), _VecE
+                    return self.xes(), _VecE
                 elif n.has_dc():
-                    return dcs(self._n), _VecE
+                    return self.dcs(), _VecE
                 else:
                     n = n.to_uint()
             case _:
                 raise TypeError("Expected n to be int or Vec")
         if not 0 <= n <= self._n:
             raise ValueError(f"Expected 0 ≤ n ≤ {self._n}, got {n}")
         if n == 0:
@@ -871,32 +1021,31 @@
             ValueError: If n is invalid.
         """
         match n:
             case int():
                 pass
             case Vec():
                 if n.has_x():
-                    return xes(self._n), _VecE
+                    return self.xes(), _VecE
                 elif n.has_dc():
-                    return dcs(self._n), _VecE
+                    return self.dcs(), _VecE
                 else:
                     n = n.to_uint()
             case _:
                 raise TypeError("Expected n to be int or Vec")
         if not 0 <= n <= self._n:
             raise ValueError(f"Expected 0 ≤ n ≤ {self._n}, got {n}")
         if n == 0:
             return self, _VecE
         sign = self._get_item(self._n - 1)
-        ci_data = _fill(sign, n)
         co, sh = self[:n], self[n:]
-        y = Vec[self._n](sh._data | (ci_data << sh.nbits))
+        y = Vec[self._n](sh._data | (_fill(sign, n) << sh.nbits))
         return y, co
 
-    def add(self, other: Vec, ci: Vec[1]) -> tuple[Vec, Vec[1], Vec[1]]:
+    def add(self, other: Vec, ci: Vec[1]) -> tuple[Vec, Vec[1]]:
         """Twos complement addition.
 
         Args:
             other: vec of equal length.
 
         Returns:
             3-tuple of (sum, carry-out, overflow).
@@ -906,67 +1055,69 @@
         """
         self._check_len(other)
 
         # Rename for readability
         n, a, b = self._n, self, other
 
         if a.has_x() or b.has_x() or ci.has_x():
-            return Vec[n](_fill(_X, n)), _VecX, _VecX
+            return Vec[n](_fill(_X, n)), _VecX
         if a.has_dc() or b.has_dc() or ci.has_dc():
-            return Vec[n](_fill(_W, n)), _VecW, _VecW
+            return Vec[n](_fill(_W, n)), _VecW
 
         s = a.to_uint() + b.to_uint() + ci.to_uint()
 
         data = 0
         for i in range(n):
             data |= _from_bit[s & 1] << (_ITEM_BITS * i)
             s >>= 1
 
         # Carry out is True if there is leftover sum data
         co = (_Vec0, _Vec1)[s != 0]
 
-        s = Vec[n](data)
-
-        # Overflow is true if sign A matches sign B, and mismatches sign S
-        aa = a[-1]
-        bb = b[-1]
-        ss = s[-1]
-        ovf = ~aa & ~bb & ss | aa & bb & ~ss
-
-        return s, co, ovf
+        return Vec[n](data), co
 
-    def sub(self, other: Vec) -> tuple[Vec, Vec[1], Vec[1]]:
+    def sub(self, other: Vec) -> tuple[Vec, Vec[1]]:
         """Twos complement subtraction.
 
         Args:
             other: vec of equal length.
 
         Returns:
             3-tuple of (sum, carry-out, overflow).
 
         Raises:
             ValueError: vec lengths are invalid/inconsistent.
         """
         return self.add(other.not_(), ci=_Vec1)
 
-    def neg(self) -> tuple[Vec, Vec[1], Vec[1]]:
+    def neg(self) -> tuple[Vec, Vec[1]]:
         """Twos complement negation.
 
         Computed using 0 - self.
 
         Returns:
             3-tuple of (sum, carry-out, overflow).
         """
         zero = Vec[self._n](_fill(_0, self._n))
         return zero.sub(self)
 
+    def ite(self, v1: Vec, v0: Vec | None = None) -> Vec:
+        """If then else operator."""
+        if self.has_unknown():
+            return xes(v1._n)
+        if v0 is None:
+            v0 = dcs(v1._n)
+        else:
+            if v1._n != v0._n:
+                raise ValueError("Expected matching operand lengths")
+        return v1 if self else v0
+
     def _check_len(self, other: Vec):
         if self._n != other._n:
-            s = f"Expected n = {self._n}, got {other._n}"
-            raise ValueError(s)
+            raise ValueError(f"Expected n = {self._n}, got {other._n}")
 
     def _count(self, byte_cnt: dict[int, int], item: int) -> int:
         y = 0
         n, data = self._n, self._data
 
         stride = 4
         while n >= stride:
@@ -1154,19 +1305,19 @@
 def bools2vec(xs: Iterable[int]) -> Vec:
     """Convert an iterable of bools to a vec.
 
     This is a convenience function.
     For data in the form of [0, 1, 0, 1, ...],
     or [False, True, False, True, ...].
     """
-    i, data = 0, 0
+    n, data = 0, 0
     for x in xs:
-        data |= _from_bit[x] << (_ITEM_BITS * i)
-        i += 1
-    return Vec[i](data)
+        data |= _from_bit[x] << (_ITEM_BITS * n)
+        n += 1
+    return Vec[n](data)
 
 
 _NUM_RE = re.compile(
     r"((?P<BinSize>[0-9]+)b(?P<BinDigits>[X01\-_]+))|"
     r"((?P<HexSize>[0-9]+)h(?P<HexDigits>[0-9a-fA-F_]+))"
 )
 
@@ -1177,32 +1328,32 @@
         if m.group("BinSize"):
             size = int(m.group("BinSize"))
             digits = m.group("BinDigits").replace("_", "")
             ndigits = len(digits)
             if ndigits != size:
                 s = f"Expected {size} digits, got {ndigits}"
                 raise ValueError(s)
-            i, data = 0, 0
+            n, data = 0, 0
             for c in reversed(digits):
-                data |= _from_char[c] << (i * _ITEM_BITS)
-                i += 1
-            return i, data
+                data |= _from_char[c] << (n * _ITEM_BITS)
+                n += 1
+            return n, data
         # Hexadecimal
         elif m.group("HexSize"):
             size = int(m.group("HexSize"))
             digits = m.group("HexDigits").replace("_", "")
             ndigits = len(digits)
             if 4 * ndigits != size:
                 s = f"Expected size to match # digits, got {size} ≠ {4 * ndigits}"
                 raise ValueError(s)
-            i, data = 0, 0
+            n, data = 0, 0
             for c in reversed(digits):
-                data |= _from_hexchar[c] << (i * _ITEM_BITS)
-                i += 4
-            return i, data
+                data |= _from_hexchar[c] << (n * _ITEM_BITS)
+                n += 4
+            return n, data
         else:  # pragma: no cover
             assert False
     else:
         raise ValueError(f"Expected str literal, got {lit}")
 
 
 def lit2vec(lit: str) -> Vec:
@@ -1254,19 +1405,19 @@
             return bools2vec([x, *rst])
         case str() as lit:
             return lit2vec(lit)
         case _:
             raise TypeError(f"Invalid input: {obj}")
 
 
-def cat(*objs: int | Vec) -> Vec:
+def cat(*objs: int | str | Vec) -> Vec:
     """Concatenate a sequence of vectors.
 
     Args:
-        objs: a sequence of bools.
+        objs: a sequence of bool/lit/vec objects.
 
     Returns:
         A Vec instance.
 
     Raises:
         TypeError: If input obj is invalid.
     """
@@ -1275,44 +1426,45 @@
 
     # Convert inputs
     vs = []
     for obj in objs:
         match obj:
             case 0 | 1 as x:
                 vs.append((_Vec0, _Vec1)[x])
+            case str() as lit:
+                v = lit2vec(lit)
+                vs.append(v)
             case Vec() as v:
                 vs.append(v)
             case _:
                 raise TypeError(f"Invalid input: {obj}")
 
     if len(vs) == 1:
         return vs[0]
 
-    i, data = 0, 0
+    n, data = 0, 0
     for v in vs:
-        data |= v.data << (_ITEM_BITS * i)
-        i += len(v)
-    return Vec[i](data)
+        data |= v.data << (_ITEM_BITS * n)
+        n += len(v)
+    return Vec[n](data)
 
 
-def rep(obj: int | Vec, n: int) -> Vec:
+def rep(obj: int | str | Vec, n: int) -> Vec:
     """Repeat a vector n times."""
     objs = [obj] * n
     return cat(*objs)
 
 
 def _consts(x: int, n: int) -> Vec:
-    if n < 0:
-        raise ValueError(f"Expected n ≥, got {n}")
     return Vec[n](_fill(x, n))
 
 
 def xes(n: int) -> Vec:
     """Return a vec packed with n X items."""
-    return _consts(_X, n)
+    return Vec[n](0)
 
 
 def zeros(n: int) -> Vec:
     """Return a vec packed with n 0 items."""
     return _consts(_0, n)
 
 
@@ -1345,37 +1497,38 @@
             return super().__new__(mcs, name, bases, attrs)
 
         base_attrs = {}
         # ident = literal
         lit2name: dict[str, str] = {}
         data2name: dict[int, str] = {}
         n = None
+        dc_data = None
         for key, val in attrs.items():
             if key.startswith("__"):
                 base_attrs[key] = val
             else:
                 if n is None:
                     n, data = _lit2vec(val)
+                    dc_data = (1 << _ITEM_BITS * n) - 1
                 else:
                     n_i, data = _lit2vec(val)
                     if n_i != n:
                         raise ValueError(f"Expected lit len {n}, got {n_i}")
-                if key == "X":
-                    raise ValueError("Cannot use reserved name = 'X'")
-                if data == 0:
-                    raise ValueError("Cannot use reserved data = 0")
+                if key in ("X", "DC"):
+                    raise ValueError(f"Cannot use reserved name = '{key}'")
+                if data in (0, dc_data):
+                    raise ValueError(f"Cannot use reserved data = {data}")
                 lit2name[val] = key
                 data2name[data] = key
 
         # Empty Enum
         if n is None:
             # Create class
             super_cls = Vec[0]
             cls = super().__new__(mcs, name, bases + (super_cls,), base_attrs)
-            cls._data2name = data2name
             # Instantiate member
             obj = object.__new__(cls)  # pyright: ignore[reportArgumentType]
             super_cls.__init__(obj, 0)
             # Define methods
             cls.__new__ = lambda c: obj
             cls.__init__ = lambda s: None
             cls.name = property(fget=lambda self: "")
@@ -1383,14 +1536,20 @@
             return cls
 
         # Add X member
         x_lit = f"{n}b" + "X" * n
         lit2name[x_lit] = "X"
         data2name[0] = "X"
 
+        # Add DC member
+        dc_lit = f"{n}b" + "-" * n
+        lit2name[dc_lit] = "DC"
+        assert dc_data is not None
+        data2name[dc_data] = "DC"
+
         def _new(cls, arg: str | int):
             match arg:
                 case str() as lit:
                     try:
                         name = lit2name[lit]
                     except KeyError as e:
                         raise ValueError(f"Invalid lit: {lit}") from e
@@ -1402,15 +1561,14 @@
                 case _:
                     raise TypeError("Expected arg to be str or int")
             return getattr(cls, name)
 
         # Create class
         super_cls = Vec[n]
         cls = super().__new__(mcs, name, bases + (super_cls,), base_attrs)
-        cls._data2name = data2name
 
         # Instantiate members
         for data, name in data2name.items():
             obj = object.__new__(cls)  # pyright: ignore[reportArgumentType]
             super_cls.__init__(obj, data)
             obj._name = name
             setattr(cls, name, obj)
@@ -1465,43 +1623,55 @@
                 for field_name, field_type in val.items():
                     fields.append((field_name, field_type))
             else:
                 base_attrs[key] = val
 
         # Create Struct class
         n = sum(field_type._n for _, field_type in fields)
-        cls = super().__new__(mcs, name, bases + (Vec[n],), base_attrs)
+        super_cls = Vec[n]
+        cls = super().__new__(mcs, name, bases + (super_cls,), base_attrs)
 
         # Create Struct.__init__
         code = _vec_struct_init(fields)
         d = {}
         exec(code, None, d)  # pylint: disable=exec-used
         cls.__init__ = d["init"]
 
+        # Override Struct.xes and Struct.dcs methods
+        def _xes():
+            return cls()
+
+        def _dcs():
+            kwargs = {fn: ft.dcs() for fn, ft in fields}
+            return cls(**kwargs)  # pyright: ignore[reportCallIssue]
+
+        cls.xes = _xes
+        cls.dcs = _dcs
+
         # Create Struct.__str__
         def _str(self):
             args = []
             for fn, ft in fields:
                 v = getattr(self, fn)
                 if issubclass(ft, VecEnum):
-                    arg = f"{fn}={ft.__name__}.{ft._data2name[v.data]}"
+                    arg = f"{fn}={ft.__name__}.{v.name}"
                 else:
                     arg = f"{fn}={v!s}"
                 args.append(arg)
             return f'{name}({", ".join(args)})'
 
         cls.__str__ = _str
 
         # Create Struct.__repr__
         def _repr(self):
             args = []
             for fn, ft in fields:
                 v = getattr(self, fn)
                 if issubclass(ft, VecEnum):
-                    arg = f"{fn}={ft.__name__}.{ft._data2name[v.data]}"
+                    arg = f"{fn}={ft.__name__}.{v.name}"
                 else:
                     arg = f"{fn}={v!r}"
                 args.append(arg)
             return f'{name}({", ".join(args)})'
 
         cls.__repr__ = _repr
```

### Comparing `seqlogic-0.0.8/src/seqlogic/sim.py` & `seqlogic-0.0.9/src/seqlogic/sim.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,136 +8,135 @@
 """
 
 import heapq
 import inspect
 from abc import ABC
 from collections import defaultdict
 from collections.abc import Awaitable, Callable, Coroutine, Generator
+from enum import IntEnum, auto
 from functools import partial
-from typing import NewType, TypeAlias
-
-Region = NewType("Region", int)
-
+from typing import TypeAlias
 
 _INIT_TIME = -1
 _START_TIME = 0
 
 
-class State(ABC):
-    """TODO(cjdrake): Write docstring."""
+class Region(IntEnum):
+    REACTIVE = auto()
+    ACTIVE = auto()
 
-    def __init__(self, value):
-        """TODO(cjdrake): Write docstring."""
-        self._init_value = value
 
+class State(ABC):
+    """Model component."""
+
+    def __init__(self):
         # Reference to the event loop
         self._sim = _sim
 
     def changed(self) -> bool:
-        """TODO(cjdrake): Write docstring."""
         raise NotImplementedError
 
     def update(self):
-        """TODO(cjdrake): Write docstring."""
         raise NotImplementedError()
 
 
 class Singular(State):
-    """TODO(cjdrake): Write docstring."""
+    """Model state organized as a single unit."""
 
     def __init__(self, value):
-        super().__init__(value)
-        self._value = self._init_value
-        self._next_value = self._init_value
+        super().__init__()
+        self._value = value
+        self._next_value = value
         self._changed = False
 
     def get_value(self):
-        """TODO(cjdrake): Write docstring."""
-        return self._value
+        if self._sim.region is None:
+            return self._value
+        if self._sim.region == Region.REACTIVE:
+            return self._next_value
+        if self._sim.region == Region.ACTIVE:
+            return self._value
+        assert False
 
     value = property(fget=get_value)
 
-    def get_next(self):
-        """TODO(cjdrake): Write docstring."""
-        return self._next_value
-
     def set_next(self, value):
-        """TODO(cjdrake): Write docstring."""
         self._changed = value != self._next_value
         self._next_value = value
 
         # Notify the event loop
         _sim.touch(self)
 
-    next = property(fget=get_next, fset=set_next)
+    next = property(fset=set_next)
 
     def changed(self) -> bool:
         return self._changed
 
     def update(self):
         self._value = self._next_value
         self._changed = False
 
     def dirty(self) -> bool:
-        """TODO(cjdrake): Write docstring."""
         return self._next_value != self._value
 
 
 class Aggregate(State):
-    """TODO(cjdrake): Write docstring."""
+    """Model state organized as multiple units."""
 
     def __init__(self, value):
-        super().__init__(value)
-        self._values = defaultdict(lambda: self._init_value)
-        self._next_values = defaultdict(lambda: self._init_value)
+        super().__init__()
+        self._values = defaultdict(lambda: value)
+        self._next_values = defaultdict(lambda: value)
         self._changed = set()
 
-    def get_value(self, index: int):
-        """TODO(cjdrake): Write docstring."""
-        return self._values[index]
+    def __getitem__(self, key: int):
+        return _AggrItem(self, key)
 
-    def get_next(self, index: int):
-        """TODO(cjdrake): Write docstring."""
-        return self._next_values[index]
+    def get_value(self, index: int):
+        if self._sim.region is None:
+            return self._values[index]
+        if self._sim.region == Region.REACTIVE:
+            return self._next_values[index]
+        if self._sim.region == Region.ACTIVE:
+            return self._values[index]
+        assert False
 
     def set_next(self, index: int, value):
-        """TODO(cjdrake): Write docstring."""
         if value != self._next_values[index]:
             self._changed.add(index)
         self._next_values[index] = value
 
         # Notify the event loop
         _sim.touch(self)
 
-    def __getitem__(self, key: int):
-        return _ItemWrap(self, key)
-
     def changed(self) -> bool:
         return bool(self._changed)
 
     def update(self):
         for index in self._changed:
             self._values[index] = self._next_values[index]
         self._changed.clear()
 
 
-class _ItemWrap:
-    """Wrap Aggregate item getter/setter"""
+class _AggrItem:
+    """Wrap Aggregate item getter/setter."""
 
     def __init__(self, obj: Aggregate, index: int):
         self._obj = obj
         self._index = index
 
-    def _get_next(self):
-        return self._obj.get_next(self._index)
+    def get_value(self):
+        return self._obj.get_value(self._index)
+
+    value = property(fget=get_value)
 
-    def _set_next(self, value):
+    def set_next(self, value):
         self._obj.set_next(self._index, value)
 
-    next = property(fget=_get_next, fset=_set_next)
+    next = property(fset=set_next)
 
 
 _SimQueueItem: TypeAlias = tuple[int, Region, Coroutine, State | None]
 
 
 class _SimQueue:
     """Priority queue for ordering task execution."""
@@ -187,15 +186,15 @@
         return state
 
 
 class Sim:
     """Simulation event loop."""
 
     def __init__(self):
-        """TODO(cjdrake): Write docstring."""
+        """Initialize simulation."""
         self._started: bool = False
         # Simulation time
         self._time: int = _INIT_TIME
         self._region: Region | None = None
         # Task queue
         self._queue = _SimQueue()
         # Currently executing task
@@ -207,61 +206,57 @@
         # Postponed actions
         self._touched: set[State] = set()
         # Processes
         self._procs = []
 
     @property
     def started(self) -> bool:
-        """TODO(cjdrake): Write docstring."""
         return self._started
 
     def restart(self):
-        """Restart the simulation."""
+        """Restart simulation."""
         self._started = False
         self._time = _INIT_TIME
         self._region = None
         self._queue.clear()
         self._task = None
         self._waiting.clear()
         self._triggers.clear()
         self._touched.clear()
 
     def reset(self):
-        """Reset the simulation state."""
+        """Reset simulation state."""
         self.restart()
         self._procs.clear()
         self._task_region.clear()
 
     @property
     def time(self) -> int:
-        """TODO(cjdrake): Write docstring."""
         return self._time
 
     @property
     def region(self) -> Region | None:
-        """TODO(cjdrake): Write docstring."""
         return self._region
 
     @property
     def task(self) -> Coroutine | None:
-        """TODO(cjdrake): Write docstring."""
         return self._task
 
     def call_soon(self, task: Coroutine, state: State | None = None):
-        """Schedule the task in the current timeslot."""
+        """Schedule task in the current timeslot."""
         region = self._task_region[task]
         self._queue.push(self._time, region, task, state)
 
     def call_later(self, delay: int, task: Coroutine):
-        """Schedule the task after a relative delay."""
+        """Schedule task after a relative delay."""
         region = self._task_region[task]
         self._queue.push(self._time + delay, region, task)
 
     def call_at(self, when: int, task: Coroutine):
-        """Schedule the task for an absolute timeslot."""
+        """Schedule task for an absolute timeslot."""
         region = self._task_region[task]
         self._queue.push(when, region, task)
 
     def add_proc(self, region: Region, func, *args, **kwargs):
         """Add a process to run at start of simulation."""
         self._procs.append((region, func, args, kwargs))
 
@@ -406,61 +401,58 @@
     """Suspend the task, and wake up after a delay."""
     assert _sim.task is not None
     _sim.call_later(delay, _sim.task)
     await SimAwaitable()
 
 
 async def changed(*states: State) -> State:
-    """TODO(cjdrake): Write docstring."""
+    """Resume execution upon state change."""
     for state in states:
         _sim.add_event(state, state.changed)
     state = await SimAwaitable()
     return state
 
 
 async def resume(*events: tuple[State, Callable[[], bool]]) -> State:
-    """TODO(cjdrake): Write docstring."""
+    """Resume execution upon event."""
     for state, cond in events:
         _sim.add_event(state, cond)
     state = await SimAwaitable()
     return state
 
 
 def get_loop() -> Sim:
     """Return the event loop."""
     return _sim
 
 
 class _Schedule:
-    """TODO(cjdrake): Write docstring."""
+    """Add scheduling semantics to coroutine functions."""
 
     def __init__(self, region: Region, func):
         self._region = region
         assert inspect.iscoroutinefunction(func)
         self._func = func
 
     def __get__(self, obj, cls=None):
         return self._region, partial(self._func, obj)
 
 
 class initial(_Schedule):
-    """TODO(cjdrake): Write docstring."""
+    """Decorate a coroutine to run during initial scheduling region."""
 
     def __init__(self, func):
-        """TODO(cjdrake): Write docstring."""
-        super().__init__(Region(2), func)
+        super().__init__(Region.ACTIVE, func)
 
 
 class always_ff(_Schedule):
-    """TODO(cjdrake): Write docstring."""
+    """Decorate a coroutine to run during flop scheduling region."""
 
     def __init__(self, func):
-        """TODO(cjdrake): Write docstring."""
-        super().__init__(Region(1), func)
+        super().__init__(Region.ACTIVE, func)
 
 
 class always_comb(_Schedule):
-    """TODO(cjdrake): Write docstring."""
+    """Decorate a coroutine to run during combi scheduling region."""
 
     def __init__(self, func):
-        """TODO(cjdrake): Write docstring."""
-        super().__init__(Region(0), func)
+        super().__init__(Region.REACTIVE, func)
```

### Comparing `seqlogic-0.0.8/src/seqlogic/util.py` & `seqlogic-0.0.9/src/seqlogic/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,7 +49,15 @@
 
     y = 0
     shifter = 1
     while x > shifter:
         shifter <<= 1
         y += 1
     return y
+
+
+class classproperty:
+    def __init__(self, func):
+        self._f = func
+
+    def __get__(self, unused_obj, cls):
+        return self._f(cls)
```

### Comparing `seqlogic-0.0.8/src/seqlogic.egg-info/PKG-INFO` & `seqlogic-0.0.9/src/seqlogic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqlogic
-Version: 0.0.8
+Version: 0.0.9
 Summary: Sequential Logic
 Project-URL: Repository, https://github.com/cjdrake/seqlogic.git
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Sequential Logic
```

### Comparing `seqlogic-0.0.8/src/seqlogic.egg-info/SOURCES.txt` & `seqlogic-0.0.9/src/seqlogic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.8/tests/test_aes.py` & `seqlogic-0.0.9/tests/test_aes.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.8/tests/test_bits.py` & `seqlogic-0.0.9/tests/test_bits.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,17 +243,17 @@
     ("2b11", "2b10", T, "2b10", T, F),
     ("2b11", "2b11", T, "2b11", T, F),
 ]
 
 
 def test_add():
     """Test bits add method."""
-    for a, b, ci, s, co, v in ADD_VALS:
+    for a, b, ci, s, co, _ in ADD_VALS:
         a, b, s = bits(a), bits(b), bits(s)
-        assert a.add(b, ci) == (s, co, v)
+        assert a.add(b, ci) == (s, co)
 
 
 def test_addsubops():
     """Test bits add/substract operators."""
     assert bits("2b00") + bits("2b00") == bits("2b00")
     assert bits("2b00") + bits("2b01") == bits("2b01")
     assert bits("2b01") + bits("2b00") == bits("2b01")
```

### Comparing `seqlogic-0.0.8/tests/test_enum.py` & `seqlogic-0.0.9/tests/test_enum.py`

 * *Files 19% similar despite different names*

```diff
@@ -43,23 +43,39 @@
     assert Color("2b01") is Color.GREEN
 
     assert len(Color.BLUE) == 2
     assert Color.BLUE.name == "BLUE"
     assert Color.BLUE.data == 0b1001
     assert str(Color.BLUE) == "2b10"
     assert Color("2b10") is Color.BLUE
+    assert Color(0b1001) is Color.BLUE
 
     assert len(Color.X) == 2
     assert Color.X.name == "X"
     assert Color.X.data == 0
     assert str(Color.X) == "2bXX"
     assert Color("2bXX") is Color.X
 
+    assert Color.xes() is Color.X
+
+    assert len(Color.DC) == 2
+    assert Color.DC.name == "DC"
+    assert Color.DC.data == 0b1111
+    assert str(Color.DC) == "2b--"
+    assert Color("2b--") is Color.DC
+    assert Color(0b1111) is Color.DC
+
+    assert Color.dcs() is Color.DC
+
     with pytest.raises(ValueError):
         _ = Color("2b11")
+    with pytest.raises(ValueError):
+        _ = Color(0b1010)
+    with pytest.raises(TypeError):
+        _ = Color(1.23e4)
 
 
 def test_slicing():
     assert Color.GREEN[0] == ones(1)
     assert Color.GREEN[1] == zeros(1)
 
 
@@ -68,14 +84,21 @@
     with pytest.raises(ValueError):
 
         class InvalidName(VecEnum):
             X = "4bXXXX"
 
         _ = InvalidName()
 
+    with pytest.raises(ValueError):
+
+        class InvalidData(VecEnum):
+            FOO = "4bXXXX"
+
+        _ = InvalidData()
+
     # The literal must be a str
     with pytest.raises(TypeError):
 
         class InvalidType(VecEnum):
             FOO = 42
 
         _ = InvalidType()
```

### Comparing `seqlogic-0.0.8/tests/test_fsm.py` & `seqlogic-0.0.9/tests/test_fsm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Example FSM implementation.
 
 Demonstrate usage of an enum.
 """
 
 from collections import defaultdict
 
-from seqlogic import Bit, Enum, Module, get_loop
+from seqlogic import Bit, Bits, Module, get_loop
 from seqlogic.lbool import VecEnum, ones, xes, zeros
 from seqlogic.sim import Region
 
 from .common import p_clk, p_dff, p_rst
 
 # pyright: reportAttributeAccessIssue=false
 # pyright: reportReturnType=false
@@ -56,15 +56,15 @@
 def test_fsm():
     """Test a 3-bit LFSR."""
     loop.reset()
 
     top = Module(name="top")
     clock = Bit(name="clock", parent=top)
     reset_n = Bit(name="reset_n", parent=top)
-    ps = Enum(name="ps", parent=top, cls=SeqDetect)
+    ps = Bits(name="ps", parent=top, dtype=SeqDetect)
     x = Bit(name="x", parent=top)
 
     waves = defaultdict(dict)
     top.dump_waves(waves, r".*")
 
     def ns() -> SeqDetect:
         match ps.value:
@@ -88,23 +88,23 @@
                     return SeqDetect.D
                 else:
                     return SeqDetect.A
             case _:
                 return SeqDetect.X
 
     # Schedule input
-    loop.add_proc(Region(1), p_input, x, reset_n, clock)
+    loop.add_proc(Region.ACTIVE, p_input, x, reset_n, clock)
 
     # Schedule LFSR
-    loop.add_proc(Region(1), p_dff, ps, ns, reset_n, SeqDetect.A, clock)
+    loop.add_proc(Region.ACTIVE, p_dff, ps, ns, reset_n, SeqDetect.A, clock)
 
     # Schedule reset and clock
     # Note: Avoiding simultaneous reset/clock negedge/posedge on purpose
-    loop.add_proc(Region(2), p_rst, reset_n, init=ones(1), phase1=6, phase2=10)
-    loop.add_proc(Region(2), p_clk, clock, init=zeros(1), shift=5, phase1=5, phase2=5)
+    loop.add_proc(Region.ACTIVE, p_rst, reset_n, init=ones(1), phase1=6, phase2=10)
+    loop.add_proc(Region.ACTIVE, p_clk, clock, init=zeros(1), shift=5, phase1=5, phase2=5)
 
     loop.run(until=100)
 
     exp = {
         # Initialize everything to X'es
         -1: {
             reset_n: xes(1),
```

### Comparing `seqlogic-0.0.8/tests/test_gray.py` & `seqlogic-0.0.9/tests/test_gray.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.8/tests/test_hier.py` & `seqlogic-0.0.9/tests/test_hier.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.8/tests/test_lbool.py` & `seqlogic-0.0.9/tests/test_lbool.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     xnor,
     xor,
 )
 
 E = Vec[0](0)
 F = vec(False)
 T = vec(True)
+X = vec("1bX")
 
 
 LNOT = {
     "X": "X",
     "0": "1",
     "1": "0",
     "-": "-",
@@ -450,49 +451,226 @@
     0b00_11: 0b00,
     0b01_11: 0b11,
     0b10_11: 0b11,
     0b11_11: 0b11,
 }
 
 
-def test_vec_ult():
+def test_vec_ltu():
     zero = uint2vec(0, 8)
     one = uint2vec(1, 8)
     two = uint2vec(2, 8)
-    assert not zero.ult(zero)
-    assert zero.ult(one)
-    assert zero.ult(two)
-    assert not one.ult(zero)
-    assert not one.ult(one)
-    assert one.ult(two)
-    assert not two.ult(zero)
-    assert not two.ult(one)
-    assert not two.ult(two)
+    assert not zero.ltu(zero)
+    assert zero.ltu(one)
+    assert zero.ltu(two)
+    assert not one.ltu(zero)
+    assert not one.ltu(one)
+    assert one.ltu(two)
+    assert not two.ltu(zero)
+    assert not two.ltu(one)
+    assert not two.ltu(two)
 
 
-def test_vec_slt():
+def test_vec_lt():
     n_one = int2vec(-1, 8)
     zero = int2vec(0, 8)
     one = int2vec(1, 8)
-    assert not n_one.slt(n_one)
-    assert n_one.slt(zero)
-    assert n_one.slt(one)
-    assert not zero.slt(n_one)
-    assert not zero.slt(zero)
-    assert zero.slt(one)
-    assert not one.slt(n_one)
-    assert not one.slt(zero)
-    assert not one.slt(one)
+    assert not n_one.lt(n_one)
+    assert n_one.lt(zero)
+    assert n_one.lt(one)
+    assert not zero.lt(n_one)
+    assert not zero.lt(zero)
+    assert zero.lt(one)
+    assert not one.lt(n_one)
+    assert not one.lt(zero)
+    assert not one.lt(one)
 
 
 def test_vec_uxor():
     for k, v in UXOR.items():
         assert Vec[2](k).uxor() == Vec[1](v)
 
 
+def test_eq():
+    a = vec("4b0000")
+    b = vec("4b1111")
+    c = vec("4b0000")
+    x = vec("4bXXXX")
+
+    assert a.eq(c) == T
+    assert a.eq(b) == F
+
+    assert a.neq(b) == T
+    assert a.neq(c) == F
+
+    assert a.eq(x) == X
+    assert x.eq(a) == X
+    assert a.neq(x) == X
+    assert x.neq(a) == X
+
+
+def test_lt():
+    a = int2vec(-1, 4)
+    b = int2vec(0, 4)
+    c = int2vec(1, 4)
+    x = vec("4bXXXX")
+
+    assert a.lt(b) == T
+    assert b.lt(a) == F
+
+    assert a.lt(c) == T
+    assert c.lt(a) == F
+
+    assert b.lt(c) == T
+    assert c.lt(b) == F
+
+    assert a.lt(x) == X
+    assert x.lt(a) == X
+
+
+def test_lte():
+    a = int2vec(-1, 4)
+    b = int2vec(0, 4)
+    c = int2vec(1, 4)
+    x = vec("4bXXXX")
+
+    assert a.lte(b) == T
+    assert b.lte(a) == F
+
+    assert a.lte(c) == T
+    assert c.lte(a) == F
+
+    assert b.lte(c) == T
+    assert c.lte(b) == F
+
+    assert a.lte(x) == X
+    assert x.lte(a) == X
+
+
+def test_ltu():
+    a = uint2vec(0, 4)
+    b = uint2vec(1, 4)
+    x = vec("4bXXXX")
+
+    assert a.ltu(b) == T
+    assert b.ltu(a) == F
+
+    assert a.ltu(x) == X
+    assert x.ltu(a) == X
+
+
+def test_lteu():
+    a = uint2vec(0, 4)
+    b = uint2vec(1, 4)
+    x = vec("4bXXXX")
+
+    assert a.lteu(b) == T
+    assert b.lteu(a) == F
+
+    assert a.lteu(x) == X
+    assert x.lteu(a) == X
+
+
+def test_gt():
+    a = int2vec(-1, 4)
+    b = int2vec(0, 4)
+    c = int2vec(1, 4)
+    x = vec("4bXXXX")
+
+    assert a.gt(b) == F
+    assert b.gt(a) == T
+
+    assert a.gt(c) == F
+    assert c.gt(a) == T
+
+    assert b.gt(c) == F
+    assert c.gt(b) == T
+
+    assert a.gt(x) == X
+    assert x.gt(a) == X
+
+
+def test_gte():
+    a = int2vec(-1, 4)
+    b = int2vec(0, 4)
+    c = int2vec(1, 4)
+    x = vec("4bXXXX")
+
+    assert a.gte(b) == F
+    assert b.gte(a) == T
+
+    assert a.gte(c) == F
+    assert c.gte(a) == T
+
+    assert b.gte(c) == F
+    assert c.gte(b) == T
+
+    assert a.gte(x) == X
+    assert x.gte(a) == X
+
+
+def test_gtu():
+    a = uint2vec(0, 4)
+    b = uint2vec(1, 4)
+    x = vec("4bXXXX")
+
+    assert a.gtu(b) == F
+    assert b.gtu(a) == T
+
+    assert a.gtu(x) == X
+    assert x.gtu(a) == X
+
+
+def test_gteu():
+    a = uint2vec(0, 4)
+    b = uint2vec(1, 4)
+    x = vec("4bXXXX")
+
+    assert a.gteu(b) == F
+    assert b.gteu(a) == T
+
+    assert a.gteu(x) == X
+    assert x.gteu(a) == X
+
+
+def test_vec_match():
+    a = vec("2b01")
+    b = vec("1b-")
+    c = vec("1bX")
+
+    assert a.match("2b01") == T
+    assert a.match("2b00") == F
+    assert a.match("2b10") == F
+    assert a.match("2b11") == F
+
+    assert a.match("2b0-") == T
+    assert a.match("2b-1") == T
+    assert a.match("2b--") == T
+    assert a.match("2b-0") == F
+    assert a.match("2b1-") == F
+    assert a.match("2bX1") == X
+    assert a.match("2b0X") == X
+
+    assert a.match(vec("2b01")) == T
+    assert a.match(vec("2b00")) == F
+
+    assert b.match("1bX") == X
+    assert b.match("1b0") == T
+    assert b.match("1b1") == T
+    assert b.match("1b-") == T
+
+    assert c.match("1b0") == X
+    assert c.match("1b1") == X
+    assert c.match("1b-") == X
+    assert c.match("1bX") == X
+
+    with pytest.raises(TypeError):
+        _ = a.match(42)  # pyright: ignore[reportArgumentType]
+
+
 def test_vec_zext():
     v = Vec[4](0b10_01_10_01)
     with pytest.raises(ValueError):
         v.zext(-1)
     assert v.zext(0) is v
     assert v.zext(4) == Vec[8](0b01_01_01_01_10_01_10_01)
 
@@ -523,14 +701,21 @@
     with pytest.raises(ValueError):
         v.lsh(5)
 
     assert v.lsh(2, Vec[2](0b01_10)) == (Vec[4](0b10_10_01_10), Vec[2](0b10_10))
     with pytest.raises(ValueError):
         v.lsh(2, Vec[3](0b01_01_01))
 
+    assert vec("2b01").lsh(vec("1bX")) == (vec("2bXX"), E)
+    assert vec("2b01").lsh(vec("1b-")) == (vec("2b--"), E)
+    assert vec("2b01").lsh(vec("1b1")) == (vec("2b10"), F)
+
+    with pytest.raises(TypeError):
+        v.lsh("foo")  # pyright: ignore[reportArgumentType]
+
 
 def test_vec_rsh():
     v = Vec[4](0b10_10_10_10)
     y, co = v.rsh(0)
     assert y is v and co == E
     assert v.rsh(1) == (Vec[4](0b01_10_10_10), Vec[1](0b10))
     assert v.rsh(2) == (Vec[4](0b01_01_10_10), Vec[2](0b10_10))
@@ -543,14 +728,21 @@
     with pytest.raises(ValueError):
         v.rsh(5)
 
     assert v.rsh(2, Vec[2](0b01_10)) == (Vec[4](0b01_10_10_10), Vec[2](0b10_10))
     with pytest.raises(ValueError):
         v.rsh(2, Vec[3](0b01_01_01))
 
+    assert vec("2b01").rsh(vec("1bX")) == (vec("2bXX"), E)
+    assert vec("2b01").rsh(vec("1b-")) == (vec("2b--"), E)
+    assert vec("2b01").rsh(vec("1b1")) == (vec("2b00"), T)
+
+    with pytest.raises(TypeError):
+        v.rsh("foo")  # pyright: ignore[reportArgumentType]
+
 
 def test_vec_arsh():
     v = Vec[4](0b10_10_10_10)
     assert v.arsh(0) == (Vec[4](0b10_10_10_10), E)
     assert v.arsh(1) == (Vec[4](0b10_10_10_10), Vec[1](0b10))
     assert v.arsh(2) == (Vec[4](0b10_10_10_10), Vec[2](0b10_10))
     assert v.arsh(3) == (Vec[4](0b10_10_10_10), Vec[3](0b10_10_10))
@@ -564,14 +756,21 @@
     assert v.arsh(4) == (Vec[4](0b01_01_01_01), Vec[4](0b01_10_10_10))
 
     with pytest.raises(ValueError):
         v.arsh(-1)
     with pytest.raises(ValueError):
         v.arsh(5)
 
+    assert vec("2b01").arsh(vec("1bX")) == (vec("2bXX"), E)
+    assert vec("2b01").arsh(vec("1b-")) == (vec("2b--"), E)
+    assert vec("2b01").arsh(vec("1b1")) == (vec("2b00"), T)
+
+    with pytest.raises(TypeError):
+        v.arsh("foo")  # pyright: ignore[reportArgumentType]
+
 
 ADD_VALS = [
     ("2b00", "2b00", F, "2b00", F, F),
     ("2b00", "2b01", F, "2b01", F, F),
     ("2b00", "2b10", F, "2b10", F, F),
     ("2b00", "2b11", F, "2b11", F, F),
     ("2b01", "2b00", F, "2b01", F, F),
@@ -603,17 +802,17 @@
     ("2b11", "2b10", T, "2b10", T, F),
     ("2b11", "2b11", T, "2b11", T, F),
 ]
 
 
 def test_vec_add():
     """Test bits add method."""
-    for a, b, ci, s, co, v in ADD_VALS:
+    for a, b, ci, s, co, _ in ADD_VALS:
         a, b, s = vec(a), vec(b), vec(s)
-        assert a.add(b, ci) == (s, co, v)
+        assert a.add(b, ci) == (s, co)
 
 
 def test_vec_addsubnegops():
     """Test bits add/substract operators."""
     assert vec("2b00") + vec("2b00") == vec("2b00")
     assert vec("2b00") + vec("2b01") == vec("2b01")
     assert vec("2b01") + vec("2b00") == vec("2b01")
@@ -889,14 +1088,15 @@
     assert list(v) == [Vec[1](0b00), Vec[1](0b01), Vec[1](0b10), Vec[1](0b11)]
 
 
 def test_cat():
     v = vec("4b-10X")
     assert cat() == vec()
     assert cat(v) == v
+    assert cat("2b0X", "2b-1") == vec("4b-10X")
     assert cat(vec("2b0X"), vec("2b-1")) == vec("4b-10X")
     assert cat(0, 1) == vec("2b10")
 
     with pytest.raises(TypeError):
         _ = cat(v, 42)
```

### Comparing `seqlogic-0.0.8/tests/test_lfsr.py` & `seqlogic-0.0.9/tests/test_lfsr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Example LFSR implementation."""
 
 from collections import defaultdict
 
 from seqlogic import Bit, Bits, Module, get_loop
-from seqlogic.lbool import cat, ones, vec, xes, zeros
+from seqlogic.lbool import Vec, cat, ones, vec, xes, zeros
 from seqlogic.sim import Region
 
 from .common import p_clk, p_dff, p_rst
 
 loop = get_loop()
 
 
@@ -16,15 +16,15 @@
 
     def __init__(self):
         super().__init__(name="top", parent=None)
         # Control
         self.reset_n = Bit(name="reset_n", parent=self)
         self.clock = Bit(name="clock", parent=self)
         # State
-        self.q = Bits(name="q", parent=self, shape=(3,))
+        self.q = Bits(name="q", parent=self, dtype=Vec[3])
 
 
 def test_lfsr():
     """Test a 3-bit LFSR."""
     loop.reset()
 
     top = Top()
@@ -37,20 +37,20 @@
     def d():
         v = top.q.value
         return cat(v[0] ^ v[2], v[:2])
 
     reset_value = vec("3b100")
 
     # Schedule LFSR
-    loop.add_proc(Region(1), p_dff, top.q, d, top.reset_n, reset_value, top.clock)
+    loop.add_proc(Region.ACTIVE, p_dff, top.q, d, top.reset_n, reset_value, top.clock)
 
     # Schedule reset and clock
     # Note: Avoiding simultaneous reset/clock negedge/posedge on purpose
-    loop.add_proc(Region(2), p_rst, top.reset_n, init=ones(1), phase1=6, phase2=10)
-    loop.add_proc(Region(2), p_clk, top.clock, init=zeros(1), shift=5, phase1=5, phase2=5)
+    loop.add_proc(Region.ACTIVE, p_rst, top.reset_n, init=ones(1), phase1=6, phase2=10)
+    loop.add_proc(Region.ACTIVE, p_clk, top.clock, init=zeros(1), shift=5, phase1=5, phase2=5)
 
     loop.run(until=100)
 
     exp = {
         # Initialize everything to X'es
         -1: {
             top.reset_n: xes(1),
```

### Comparing `seqlogic-0.0.8/tests/test_riscv.py` & `seqlogic-0.0.9/tests/test_riscv.py`

 * *Files identical despite different names*

### Comparing `seqlogic-0.0.8/tests/test_sim.py` & `seqlogic-0.0.9/tests/test_sim.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     async def hello():
         await sleep(2)
         print(f"[{loop.time}] Hello")
         await sleep(2)
         print(f"[{loop.time}] World")
 
-    loop.add_proc(Region(2), hello)
+    loop.add_proc(Region.ACTIVE, hello)
 
     # Invalid run limit
     with pytest.raises(TypeError):
         loop.run("Invalid argument type")  # pyright: ignore[reportArgumentType]
 
     # Run until no events left
     loop.run()
@@ -95,17 +95,17 @@
         i = 0
         while True:
             await clk.edge()
             if i % 3 == 0:
                 b.next = not b.value
             i += 1
 
-    loop.add_proc(Region(2), p_clk)
-    loop.add_proc(Region(1), p_a)
-    loop.add_proc(Region(1), p_b)
+    loop.add_proc(Region.ACTIVE, p_clk)
+    loop.add_proc(Region.ACTIVE, p_a)
+    loop.add_proc(Region.ACTIVE, p_b)
 
     # Expected sim output
     exp = {
         -1: {clk: False, a: False, b: False},
         5: {clk: True, a: True, b: True},
         10: {clk: False},
         15: {clk: True, a: False},
@@ -158,17 +158,17 @@
         i = 0
         while True:
             await clk.edge()
             if i % 3 == 0:
                 b.next = not b.value
             i += 1
 
-    loop.add_proc(Region(2), p_clk)
-    loop.add_proc(Region(1), p_a)
-    loop.add_proc(Region(1), p_b)
+    loop.add_proc(Region.ACTIVE, p_clk)
+    loop.add_proc(Region.ACTIVE, p_a)
+    loop.add_proc(Region.ACTIVE, p_b)
 
     # Expected sim output
     exp = {
         -1: {clk: False, a: False, b: False},
         5: {clk: True, a: True, b: True},
         10: {clk: False},
         15: {clk: True, a: False},
```

### Comparing `seqlogic-0.0.8/tests/test_struct.py` & `seqlogic-0.0.9/tests/test_struct.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 """Test seqlogic.lbool.VecStruct."""
 
 # PyRight is confused by MetaClass behavior
 # pyright: reportArgumentType=false
 # pyright: reportAttributeAccessIssue=false
 # pyright: reportCallIssue=false
 
-from seqlogic.lbool import Vec, VecStruct, vec
+from seqlogic.lbool import Vec, VecEnum, VecStruct, vec
 
 
 class Pixel(VecStruct):
     r: Vec[8]
     g: Vec[8]
     b: Vec[8]
 
 
+class MyEnum(VecEnum):
+    A = "2b01"
+    B = "2b10"
+
+
+class Mixed(VecStruct):
+    a: Vec[4]
+    b: MyEnum
+
+
 def test_empty():
     class EmptyStruct(VecStruct):
         pass
 
     s = EmptyStruct()
     assert len(s) == 0
     assert s.data == 0
@@ -52,7 +62,20 @@
     assert str(p) == "Pixel(r=8bXXXX_XXXX, g=8bXXXX_XXXX, b=8b0100_0100)"
     p = Pixel(r=vec("8b0001_0001"), g=vec("8b0010_0010"))
     assert str(p) == "Pixel(r=8b0001_0001, g=8b0010_0010, b=8bXXXX_XXXX)"
     p = Pixel(r=vec("8b0001_0001"), b=vec("8b0100_0100"))
     assert str(p) == "Pixel(r=8b0001_0001, g=8bXXXX_XXXX, b=8b0100_0100)"
     p = Pixel(g=vec("8b0010_0010"), b=vec("8b0100_0100"))
     assert str(p) == "Pixel(r=8bXXXX_XXXX, g=8b0010_0010, b=8b0100_0100)"
+
+    assert str(Pixel.xes()) == "Pixel(r=8bXXXX_XXXX, g=8bXXXX_XXXX, b=8bXXXX_XXXX)"
+    assert str(Pixel.dcs()) == "Pixel(r=8b----_----, g=8b----_----, b=8b----_----)"
+
+
+def test_mixed():
+    mx = Mixed()
+    assert str(mx) == "Mixed(a=4bXXXX, b=MyEnum.X)"
+    assert repr(mx) == "Mixed(a=Vec[4](0b00000000), b=MyEnum.X)"
+
+    m1 = Mixed(a=vec("4b1010"), b=MyEnum.A)
+    assert str(m1) == "Mixed(a=4b1010, b=MyEnum.A)"
+    assert m1.b.B.name == "B"
```

