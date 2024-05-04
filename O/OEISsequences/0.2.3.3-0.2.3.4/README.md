# Comparing `tmp/OEISsequences-0.2.3.3.tar.gz` & `tmp/OEISsequences-0.2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OEISsequences-0.2.3.3.tar", last modified: Mon Mar  4 23:55:25 2024, max compression
+gzip compressed data, was "OEISsequences-0.2.3.4.tar", last modified: Sat May  4 22:08:46 2024, max compression
```

## Comparing `OEISsequences-0.2.3.3.tar` & `OEISsequences-0.2.3.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-04 23:55:25.397398 OEISsequences-0.2.3.3/
--rw-rw-rw-   0        0        0    11527 2024-01-15 19:29:10.000000 OEISsequences-0.2.3.3/LICENSE
-drwxrwxrwx   0        0        0        0 2024-03-04 23:55:25.388391 OEISsequences-0.2.3.3/OEISsequences.egg-info/
--rw-rw-rw-   0        0        0     4615 2024-03-04 23:55:25.000000 OEISsequences-0.2.3.3/OEISsequences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2024-03-04 23:55:25.000000 OEISsequences-0.2.3.3/OEISsequences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-04 23:55:25.000000 OEISsequences-0.2.3.3/OEISsequences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-03-04 23:55:25.000000 OEISsequences-0.2.3.3/OEISsequences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-03-04 23:55:25.000000 OEISsequences-0.2.3.3/OEISsequences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4615 2024-03-04 23:55:25.397398 OEISsequences-0.2.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     4014 2023-12-31 04:55:34.000000 OEISsequences-0.2.3.3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-04 23:55:25.396406 OEISsequences-0.2.3.3/oeis_sequences/
--rw-rw-rw-   0        0        0  1287482 2024-03-04 21:22:12.000000 OEISsequences-0.2.3.3/oeis_sequences/OEISsequences.py
--rw-rw-rw-   0        0        0       46 2022-12-04 15:54:39.000000 OEISsequences-0.2.3.3/oeis_sequences/__init__.py
--rw-rw-rw-   0        0        0       86 2024-03-04 23:55:25.398398 OEISsequences-0.2.3.3/setup.cfg
--rw-rw-rw-   0        0        0      972 2024-03-04 21:28:52.000000 OEISsequences-0.2.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-04 22:08:46.195011 OEISsequences-0.2.3.4/
+-rw-rw-rw-   0        0        0    11527 2024-01-15 19:29:10.000000 OEISsequences-0.2.3.4/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-04 22:08:46.183010 OEISsequences-0.2.3.4/OEISsequences.egg-info/
+-rw-rw-rw-   0        0        0     4615 2024-05-04 22:08:45.000000 OEISsequences-0.2.3.4/OEISsequences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2024-05-04 22:08:46.000000 OEISsequences-0.2.3.4/OEISsequences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-04 22:08:45.000000 OEISsequences-0.2.3.4/OEISsequences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-04 22:08:45.000000 OEISsequences-0.2.3.4/OEISsequences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-04 22:08:45.000000 OEISsequences-0.2.3.4/OEISsequences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4615 2024-05-04 22:08:46.195011 OEISsequences-0.2.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4014 2023-12-31 04:55:34.000000 OEISsequences-0.2.3.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-04 22:08:46.194010 OEISsequences-0.2.3.4/oeis_sequences/
+-rw-rw-rw-   0        0        0  1347487 2024-05-04 22:01:14.000000 OEISsequences-0.2.3.4/oeis_sequences/OEISsequences.py
+-rw-rw-rw-   0        0        0       46 2022-12-04 15:54:39.000000 OEISsequences-0.2.3.4/oeis_sequences/__init__.py
+-rw-rw-rw-   0        0        0       86 2024-05-04 22:08:46.197011 OEISsequences-0.2.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      972 2024-05-04 22:07:40.000000 OEISsequences-0.2.3.4/setup.py
```

### Comparing `OEISsequences-0.2.3.3/LICENSE` & `OEISsequences-0.2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `OEISsequences-0.2.3.3/OEISsequences.egg-info/PKG-INFO` & `OEISsequences-0.2.3.4/OEISsequences.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OEISsequences
-Version: 0.2.3.3
+Version: 0.2.3.4
 Summary: Python functions to generate OEIS sequences
 Home-page: https://github.com/postvakje/oeis-sequences
 Author: Chai Wah Wu
 Author-email: cwwuieee@gmail.com
 License: LICENSE
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `OEISsequences-0.2.3.3/PKG-INFO` & `OEISsequences-0.2.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OEISsequences
-Version: 0.2.3.3
+Version: 0.2.3.4
 Summary: Python functions to generate OEIS sequences
 Home-page: https://github.com/postvakje/oeis-sequences
 Author: Chai Wah Wu
 Author-email: cwwuieee@gmail.com
 License: LICENSE
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `OEISsequences-0.2.3.3/README.md` & `OEISsequences-0.2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `OEISsequences-0.2.3.3/oeis_sequences/OEISsequences.py` & `OEISsequences-0.2.3.4/oeis_sequences/OEISsequences.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,14 @@
     composite,
     compositepi,
     factorial2,
     prevprime,
     primefactors,
     harmonic,
     multiplicity,
-    n_order,
     primorial,
     sqrt,
     ff,
     rf,
     sin,
     cos,
     tan,
@@ -145,14 +144,16 @@
     Rational,
     sturm,
     oo,
     LT,
     nan,
     sign,
     proper_divisors,
+    exp,
+    is_nthpow_residue,
 )
 from sympy.functions import hyper, partition, euler
 from sympy.ntheory import (
     mobius,
     jacobi_symbol,
     legendre_symbol,
     sqrt_mod,
@@ -219,14 +220,15 @@
     path_graph,
     cycle_graph,
     mycielski_graph,
     hypercube_graph,
     contracted_nodes,
     simple_cycles,
 )
+from heapq import heappop, heappushpop
 
 if sys.version_info < (3, 9):
     from sympy import lcm as sympylcm, gcd as sympygcd
 
     def gcd(*x):
         r = x[0]
         for y in x[1:]:
@@ -467,15 +469,15 @@
 def RLT(n, f):
     """run length transform of a function f"""
     return prod(f(len(d)) for d in split("0+", bin(n)[2:]) if d != "") if n > 0 else 1
 
 
 def n_order(a, b):
     """returns 1 if b = 1 following older version of n_order in sympy"""
-    return n_order(a, b) if b > 1 else 1
+    return sympy.n_order(a, b) if b > 1 else 1
 
 
 def repeating_decimals_expr(f, digits_only=False):
     """returns repeating decimals of Fraction f as the string aaa.bbb[ccc].
     returns only digits if digits_only=True.
     """
     a, b = f.as_integer_ratio()
@@ -11840,27 +11842,33 @@
                 l.append((d2, d))
     l.sort()
     yield from (b for a, b in l)
 
 
 def A258103(n):
     """requires 2 <= n <= 62"""
-    c, sm, sq = (
-        0,
-        mpz("".join([gmpy2digits(i, n) for i in range(n - 1, -1, -1)]), n),
-        mpz("".join(["1", "0"] + [gmpy2digits(i, n) for i in range(2, n)]), n),
-    )
-    m = isqrt(sq)
-    sq = m * m
-    m = 2 * m + 1
-    while sq <= sm:
-        if len(set(gmpy2digits(sq, n))) == n:
-            c += 1
-        sq += m
-        m += 2
+    if n & 1 and (~(m := n - 1 >> 1) & m - 1).bit_length() & 1:
+        return 0
+    t = "".join(gmpy2digits(d, n) for d in range(n))
+    k = mpz("".join(gmpy2digits(d, n) for d in range(n - 1, -1, -1)), n)
+    k2 = mpz(t, n)
+    c = 0
+    start = isqrt(k2)
+    end = isqrt(k)
+    d = (n * (n - 1) >> 1) % (n - 1)
+    for r in sqrt_mod_iter(d, n - 1):
+        e = start % (n - 1)
+        start2 = start
+        if e != r:
+            start2 += (r - e) % (n - 1)
+        for i in range(start2, end + 1, n - 1):
+            j = i**2
+            s = "".join(sorted(gmpy2digits(j, n)))
+            if s == t:
+                c += 1
     return c
 
 
 def A258774(n):
     return (lambda x: x * (x + 1) + 1)(divisor_sigma(n))
 
 
@@ -20126,15 +20134,15 @@
 
 
 def A000040(n):
     return prime(n)
 
 
 def A000079(n):
-    return 2**n
+    return 1 << n
 
 
 def A000142(n):
     return factorial(n)
 
 
 def A001222(n):
@@ -20178,27 +20186,27 @@
 
 
 def A002275(n):
     return (10**n - 1) // 9
 
 
 def A005408(n):
-    return 2 * n + 1
+    return (n << 1) + 1
 
 
 def A006530(n):
     return 1 if n == 1 else max(primefactors(n))
 
 
 def A020639(n):
     return 1 if n == 1 else min(primefactors(n))
 
 
 def A000984(n):
-    return comb(2 * n, n)
+    return comb(n << 1, n)
 
 
 def A000292(n):
     return comb(n + 2, 3)
 
 
 def A000290(n):
@@ -20210,15 +20218,15 @@
 
 
 def A002378(n):
     return n * (n + 1)
 
 
 def A005843(n):
-    return 2 * n
+    return n << 1
 
 
 def A000129_gen():  # generator of terms
     a, b = 0, 1
     yield from [a, b]
     while True:
         a, b = b, a + 2 * b
@@ -44561,14 +44569,29 @@
                 a := bisect.bisect(
                     qlist, plist[i], lo=1, hi=c + 1, key=lambda x: plist[x]
                 )
             ] = i
             c = max(c, a)
         return 64 + primepi(n) - c
 
+    def A371156(n):
+        def f(n):
+            r = primefactors(n)
+            return n * prod(p + 1 for p in r) // prod(r)
+
+        plist, qlist, c = tuple(f(i) for i in range(1, n + 1)), [0] * (n + 1), 0
+        for i in range(n):
+            qlist[
+                a := bisect.bisect(
+                    qlist, plist[i], lo=1, hi=c + 1, key=lambda x: plist[x]
+                )
+            ] = i
+            c = max(c, a)
+        return c
+
 else:
 
     def A365339(n):
         plist, qlist, rlist, c = (
             tuple(totient(i) for i in range(1, n + 1)),
             [0] * (n + 1),
             [1] * (n + 1),
@@ -44634,14 +44657,31 @@
         )
         for i in range(n):
             qlist[a := bisect.bisect(rlist, p := plist[i], lo=1, hi=c + 1)] = i
             rlist[a] = p
             c = max(c, a)
         return 64 + primepi(n) - c
 
+    def A371156(n):
+        def f(n):
+            r = primefactors(n)
+            return n * prod(p + 1 for p in r) // prod(r)
+
+        plist, qlist, rlist, c = (
+            tuple(f(i) for i in range(1, n + 1)),
+            [0] * (n + 1),
+            [1] * (n + 1),
+            0,
+        )
+        for i in range(n):
+            qlist[a := bisect.bisect(rlist, p := plist[i], lo=1, hi=c + 1)] = i
+            rlist[a] = p
+            c = max(c, a)
+        return c
+
 
 def A365373(n):
     return n * (n * (n * (n * (3 * n + 15) + 25) - 15) - 28) // 60
 
 
 def A364633(n):
     return (n + 1) * (prime(n) // (n + 1) + 1) - prime(n) if n > 2 else 0
@@ -54214,7 +54254,2415 @@
         elif (b := a + p) not in aset:
             a = b
         else:
             a = 0
             yield c
         aset.add(a)
         p = nextprime(p)
+
+
+def A117129_gen():  # generator of terms
+    a, aset, p = 1, {1}, 2
+    for c in count(2):
+        if (b := a - p) > 0 and b not in aset:
+            a = b
+        elif (b := a + p) not in aset:
+            a = b
+        else:
+            a = 0
+            yield p
+        aset.add(a)
+        p = nextprime(p)
+
+
+def A368956(n):
+    return 3**n - (1 << n + 1) - 1
+
+
+def A206369(n):
+    return prod(
+        (lambda x: x[0] + int((x[1] << 1) >= p + 1))(divmod(p ** (e + 1), p + 1))
+        for p, e in factorint(n).items()
+    )
+
+
+def A370906(n):
+    return sum(
+        (1 if k & 1 else -1)
+        * prod(
+            (lambda x: x[0] + int((x[1] << 1) >= p + 1))(divmod(p ** (e + 1), p + 1))
+            for p, e in factorint(k).items()
+        )
+        for k in range(1, n + 1)
+    )
+
+
+def A370905(n):
+    return sum(
+        prod(
+            (lambda x: x[0] + int((x[1] << 1) >= p + 1))(divmod(p ** (e + 1), p + 1))
+            for p, e in factorint(k).items()
+        )
+        for k in range(1, n + 1)
+    )
+
+
+def A242491_gen():  # generator of terms
+    return (
+        int("".join(str(d) if d < 4 else str(d + 1) for d in sympydigits(n, 8)[1:]))
+        for n in count(1)
+    )
+
+
+def A039145_gen(startvalue=0):  # generator of terms >= startvalue
+    return filter(
+        lambda k: (s := str(k)).count("4") == s.count("9"), count(max(startvalue, 0))
+    )
+
+
+def A001651(n):
+    return (n << 1) - (n >> 1) - 1
+
+
+def A369304(n):
+    return ((n + 1 << 1) - (n >> 1)) ** 2 // 3 - 2
+
+
+def A022998(n):
+    return n if n & 1 else n << 1
+
+
+def A190577(n):
+    return n * (n * (n * (n + 12) + 44) + 48)
+
+
+def A370950(n):
+    """requires 2 <= n <= 62"""
+    if n & 1 and (~(m := n - 1 >> 1) & m - 1).bit_length() & 1:
+        return 0
+    t = "".join(gmpy2digits(d, n) for d in range(1, n))
+    k = mpz("".join(gmpy2digits(d, n) for d in range(n - 1, 0, -1)), n)
+    k2 = mpz(t, n)
+    c = 0
+    start = isqrt(k2)
+    end = isqrt(k)
+    d = (n * (n - 1) >> 1) % (n - 1)
+    for r in sqrt_mod_iter(d, n - 1):
+        e = start % (n - 1)
+        start2 = start
+        if e != r:
+            start2 += (r - e) % (n - 1)
+        for i in range(start2, end + 1, n - 1):
+            if i % n:
+                j = i**2
+                s = "".join(sorted(gmpy2digits(j, n)))
+                if s == t:
+                    c += 1
+    return c
+
+
+def A092118_gen():  # generator of terms
+    for j in count(0):
+        b = 10**j
+        a = b * 10 + 1
+        ab, aa = a * b, a * a
+        for k in sorted(sqrt_mod(0, a, all_roots=True)):
+            if ab <= (m := k**2) < aa:
+                yield m
+
+
+def A370951_gen():  # generator of terms
+    a, aset, p, q = 1, {1}, 2, 0
+    for c in count(2):
+        if (b := a - p) > 0 and b not in aset:
+            a = b
+        elif (b := a + p) not in aset:
+            a = b
+        else:
+            a = 0
+            if q:
+                yield c - q
+            q = c
+        aset.add(a)
+        p = nextprime(p)
+
+
+def A370823(n):
+    return (a := 3**n - 1 << n - 1) // gcd(a, 3**n - (1 << n))
+
+
+def A370824(n):
+    return (a := 3**n - (1 << n)) // gcd(a, 3**n - 1 << n - 1)
+
+
+def A105951(n):
+    return (
+        (1 << n + 1) + 1 + (1 << m + 2 if (m := n >> 1) & 1 else -(1 << m + 2))
+        if n & 1
+        else -(1 << n + 1) - 1
+    )
+
+
+def A103145(n):
+    return (n * (n * (n + 21) + 74) + 18) // 6
+
+
+def A370932(n):
+    t = accumulate(
+        ((-j if i & 1 else j) for i, j in enumerate(sympydigits(n, 3)[1:])),
+        func=lambda x, y: (x + y) % 3,
+    )
+    return int("".join(str(-d % 3 if i & 1 else d) for i, d in enumerate(t)), 3)
+
+
+def A370849(n):
+    return min(
+        (max(primefactors(a := int("".join(s)))), a)
+        for i in range(1, 10)
+        for j in range(i + 1, 10)
+        for s in product(str(i) + str(j), repeat=n)
+    )[1]
+
+
+def A370361(n):
+    return min(
+        (max(primefactors(a := int("".join(s)))), a)
+        for i in range(10)
+        for j in range(i + 1, 10)
+        for k in range(1, n)
+        for s in multiset_permutations(str(i) * k + str(j) * (n - k))
+        if s[0] != "0" and s[-1] != "0"
+    )[0]
+
+
+def A370825(n):
+    return (a := 3 ** (n + 1) - 3 >> 1) // gcd(a, (1 << n + 1) - 2)
+
+
+def A370826(n):
+    return (a := (1 << n + 1) - 2) // gcd(a, 3 ** (n + 1) - 3 >> 1)
+
+
+def A005730(n):
+    return 1 if isprime(n) else prod(primefactors(n)) << (not n % 6)
+
+
+def A005729(n):
+    c, p = 1, 2
+    while p < n:
+        if n % p:
+            for m in count(2):
+                if (p**m - 1) // (p - 1) > n:
+                    break
+                for r in count(1):
+                    q = (p ** (m * r) - 1) // (p**r - 1)
+                    if q > n:
+                        break
+                    if not n % q:
+                        c *= p
+                        break
+                else:
+                    continue
+                if q <= n:
+                    break
+        else:
+            c *= p if p & 1 or n % 6 else p**2
+        p = nextprime(p)
+    return c
+
+
+def A005731(n):
+    c, p = 1, 2
+    while p < n:
+        if n % p:
+            for m in count(2):
+                if (p**m - 1) // (p - 1) > n:
+                    break
+                for r in count(1):
+                    q = (p ** (m * r) - 1) // (p**r - 1)
+                    if q > n:
+                        break
+                    if not n % q:
+                        c *= p
+                        break
+                else:
+                    continue
+                if q <= n:
+                    break
+        p = nextprime(p)
+    return c
+
+
+def A370252(n):
+    c, p = n, 2
+    while p < n:
+        if n % p:
+            for m in count(2):
+                if (p**m - 1) // (p - 1) > n:
+                    break
+                for r in count(1):
+                    q = (p ** (m * r) - 1) // (p**r - 1)
+                    if q > n:
+                        break
+                    if not n % q:
+                        c *= p
+                        break
+                else:
+                    continue
+                if q <= n:
+                    break
+        else:
+            c *= p if p & 1 or n % 6 else p**2
+        p = nextprime(p)
+    return c
+
+
+def A370349(n):
+    return ((n << 2) + 10) * (n + 1) ** 2 // 9
+
+
+def A141530(n):
+    return (m := (n << 1) - 1) * (n * (m - 1) - 1)
+
+
+def A370532(n):
+    return 10 * (n - 2) if n > 2 else 4 * n - 3
+
+
+def A318780(n):
+    return next(
+        k
+        for k in count(
+            integer_nthroot(
+                (n**n - n) // (n - 1) ** 2 + n ** (n - 2) * (n - 1) - 1, n
+            )[0]
+        )
+        if len(set(sympydigits(k**n, n)[1:])) == n
+    )
+
+
+def A185122(n):
+    m = n
+    j = 0
+    if n > 3:
+        for j in range(1, n):
+            if gcd((n * (n - 1) >> 1) + j, n - 1) == 1:
+                break
+    if j == 0:
+        for i in range(2, n):
+            m = n * m + i
+    elif j == 1:
+        for i in range(1, n):
+            m = n * m + i
+    else:
+        for i in range(2, 1 + j):
+            m = n * m + i
+        for i in range(j, n):
+            m = n * m + i
+    m -= 1
+    while True:
+        if len(set(sympydigits(m := nextprime(m), n)[1:])) == n:
+            return m
+
+
+def A370828(n):
+    return (a := 5**n - 3**n << n - 1) // gcd(a, 3 ** (n - 1) * (5**n - (1 << n)))
+
+
+def A370827(n):
+    return (a := 3 ** (n - 1) * (5**n - (1 << n))) // gcd(a, 5**n - 3**n << n - 1)
+
+
+def A066328(n):
+    return sum(map(primepi, primefactors(n)))
+
+
+def A049363(n):
+    return (n**n - n) // (n - 1) ** 2 + n ** (n - 2) * (n - 1) - 1 if n > 1 else 1
+
+
+def A318779(n):
+    return next(
+        k
+        for k in (
+            k**n
+            for k in count(
+                integer_nthroot(
+                    (n**n - n) // (n - 1) ** 2 + n ** (n - 2) * (n - 1) - 1, n
+                )[0]
+            )
+        )
+        if len(set(sympydigits(k, n)[1:])) == n
+    )
+
+
+def A370259(n):
+    return (chebyshevt(n, n + 1) - 1) // n**3
+
+
+def A370261(n):
+    return isqrt((chebyshevt((m := n << 1), m + 1) - 1) // ((n + 1) * m**3))
+
+
+def A318725(n):
+    c, flag = 1, False
+    for k in count(1):
+        m = k
+        if flag:
+            a, b = divmod(m, n)
+            while not b:
+                m = a
+                a, b = divmod(m, n)
+        c *= m
+        if len(set(sympydigits(c, n)[1:])) == n:
+            return k
+        if not (flag or c % n):
+            flag = True
+
+
+def A245340(n):
+    a, aset = 0, set()
+    for m in count(1):
+        if a == n:
+            return m - 1
+        aset.add(a)
+        a = next(a for a in count(a % m, m) if a not in aset)
+
+
+def A371566_gen():  # generator of terms
+    from sympy.abc import x
+
+    p = 2
+    while True:
+        if Poly(
+            x * (x * (x * (x * (x - 1) - 1) - 1) - 1) - 1, x, modulus=p
+        ).is_irreducible:
+            yield p
+        p = nextprime(p)
+
+
+def A370830_gen():  # generator of terms
+    from sympy.abc import x
+
+    p = 2
+    while True:
+        if Poly(x * (x * (x * (x - 1) - 1) - 1) - 1, x, modulus=p).is_irreducible:
+            yield p
+        p = nextprime(p)
+
+
+def A106284_gen():  # generator of terms
+    from sympy.abc import x
+
+    p = 2
+    while True:
+        if (
+            len(
+                Poly(
+                    x * (x * (x * (x * (x - 1) - 1) - 1) - 1) - 1, x, modulus=p
+                ).ground_roots()
+            )
+            == 0
+        ):
+            yield p
+        p = nextprime(p)
+
+
+def A106283_gen():  # generator of terms
+    from sympy.abc import x
+
+    p = 2
+    while True:
+        if (
+            len(Poly(x * (x * (x * (x - 1) - 1) - 1) - 1, x, modulus=p).ground_roots())
+            == 0
+        ):
+            yield p
+        p = nextprime(p)
+
+
+def A106278(n):
+    from sympy.abc import x
+
+    return len(
+        Poly(
+            x * (x * (x * (x * (x - 1) - 1) - 1) - 1) - 1, x, modulus=prime(n)
+        ).ground_roots()
+    )
+
+
+def A106281_gen():  # generator of terms
+    from sympy.abc import x
+
+    p = 2
+    while True:
+        if (
+            len(
+                Poly(
+                    x * (x * (x * (x * (x - 1) - 1) - 1) - 1) - 1, x, modulus=p
+                ).ground_roots()
+            )
+            == 5
+        ):
+            yield p
+        p = nextprime(p)
+
+
+def A370956_gen():  # generator of terms
+    a, aset, b, c = 0, set(), 0, -1
+    for n in count(1):
+        aset.add(a)
+        if a == b:
+            if n - 1 > c:
+                c = n - 1
+                yield c
+            while b in aset:
+                b += 1
+        a = next(a for a in count(a % n, n) if a not in aset)
+
+
+def A370959_gen():  # generator of terms
+    a, aset, b, c = 0, set(), 0, -1
+    for n in count(1):
+        aset.add(a)
+        if a == b:
+            if n - 1 > c:
+                c = n - 1
+                yield a
+            while b in aset:
+                b += 1
+        a = next(a for a in count(a % n, n) if a not in aset)
+
+
+def A371194(n):
+    m, j = 1, 0
+    if n > 3:
+        for j in range(1, n):
+            if gcd((n * (n - 1) >> 1) + j, n - 1) == 1:
+                break
+    if j == 0:
+        for i in range(2, n):
+            m = n * m + i
+    elif j == 1:
+        for i in range(1, n):
+            m = n * m + i
+    else:
+        for i in range(2, 1 + j):
+            m = n * m + i
+        for i in range(j, n):
+            m = n * m + i
+    m -= 1
+    while True:
+        s = sympydigits(m := nextprime(m), n)[1:]
+        if 0 not in s and len(set(s)) == n - 1:
+            return m
+
+
+def A371193(n):
+    return (1 << n) - 1 << (n - 1 << 2) if n else 0
+
+
+def A163839(n):
+    return (1 << n) - 1 << (n << 2) - 2 if n else 0
+
+
+def A060073(n):
+    return (n ** (n - 1) - 1) // (n - 1) ** 2
+
+
+def A371210(n):
+    return (m := n + 1 >> 1) * factorial(m) if n & 1 else factorial(n >> 1)
+
+
+def A048679_gen():  # generator of terms
+    return map(
+        lambda n: int(bin(n)[2:].replace("01", "1"), 2),
+        filter(lambda n: not (n << 1) & n, count(0)),
+    )
+
+
+def A371163_gen():  # generator of terms
+    c = 0
+    for n in count(0):
+        if not (n << 1) & n:
+            if int(bin(n)[2:].replace("01", "1"), 2) == c:
+                yield c
+            c += 1
+
+
+def A048678(n):
+    return int(bin(n)[2:].replace("1", "01"), 2)
+
+
+def A371033(n):
+    c = 0
+    for i in range(n):
+        c <<= n - i
+        if i & 1 ^ 1:
+            c += (1 << n - i) - 1
+    return c
+
+
+def A371032(n):
+    c = 0
+    for i in range(n):
+        c = (m := 10 ** (n - i)) * c
+        if i & 1 ^ 1:
+            c += (m - 1) // 9
+    return c
+
+
+def A371281(n):
+    return reduce(lambda a, b: a * b % 10, map(int, str(n)), 1)
+
+
+def A068792(n):
+    return ((n ** (n - 1) - 1) // (n - 1)) ** 2
+
+
+def A123668(n):
+    return (
+        n * ((n ** (n - 1) - 1) // (n - 1)) ** 2 + (n - 1) * (n ** (2 * n - 3) - 1)
+        if n > 2
+        else 4 * n - 3
+    )
+
+
+def A062813(n):
+    return (m := n**n) - (m - n) // (n - 1) ** 2 if n > 1 else 0
+
+
+def A068793(n):
+    return ((m := n**n) * (m * (n - 2) + 2) - n**2 + n - 1) // (n - 1) ** 2
+
+
+def A126646(n):
+    return (1 << n + 1) - 1
+
+
+def A007018_gen():  # generator of terms
+    a = 1
+    while True:
+        yield a
+        a *= a + 1
+
+
+def A100016_gen():  # generator of terms
+    yield (a := 1)
+    while a := a * nextprime(a):
+        yield a
+
+
+@lru_cache(maxsize=None)
+def A139145(n):
+    return (m := A139145(n >> 1)) * (m + (n & 1)) if n > 1 else 1
+
+
+def A074839_gen():  # generator of terms
+    yield (a := 1)
+    while a := a + nextprime(a):
+        yield a
+
+
+def A006279_gen():  # generator of terms
+    a, b = 1, 1
+    yield a
+    while True:
+        yield b
+        a, b = b, a * (a * b + 1)
+
+
+def A129868(n):
+    return ((m := 1 << n) - 1) * ((m << 1) + 1)
+
+
+def A280049_gen():  # generator of terms
+    return map(
+        lambda n: int(bin(n)[2:]), filter(lambda n: (n & -n).bit_length() & 1, count(1))
+    )
+
+
+def A371222(n):
+    return reduce(lambda a, b: a * b % 3, sympydigits(n, 3)[1:], 1)
+
+
+def A371054_gen():  # generator of terms
+    return (
+        3 ** (l - a) * (3**a - 1 >> 1) + 3**b - 1
+        for l in count(3)
+        for a in range(1, l - 1)
+        for b in range(1, l - a)
+    )
+
+
+def A371056_gen():  # generator of terms
+    return (
+        3 ** (l - a) * (3**a - 1) + (3**b - 1 >> 1)
+        for l in count(3)
+        for a in range(1, l - 1)
+        for b in range(1, l - a)
+    )
+
+
+def A371050_gen():  # generator of terms
+    return (
+        (3**b * (3 ** (l - a) - 1 >> 1) + 3**b - 1) * 3 ** (a - b)
+        for l in count(3)
+        for a in range(2, l)
+        for b in range(1, a)
+    )
+
+
+def A371051_gen():  # generator of terms
+    return (
+        (10**b * (10 ** (l - a) - 1) + (10**b - 1 << 1)) // 9 * 10 ** (a - b)
+        for l in count(3)
+        for a in range(2, l)
+        for b in range(1, a)
+    )
+
+
+def A371372(n):
+    return (
+        sum(
+            comb((d << 1) - 1, d) * totient((n << 1) // d)
+            for d in divisors(n << 1, generator=True)
+        )
+        // n
+        >> 2
+        if n
+        else 0
+    )
+
+
+def A371382(n):
+    return n**2 + (q := n + isqrt(5 * n**2) >> 1) * (q + 1)
+
+
+def A371388(n):
+    return n * ((n + isqrt(5 * n**2) & -2) - n)
+
+
+def A371381(n):
+    return (n << 1) * (n - 1) + 1 + (q := n + isqrt(5 * n**2) >> 1) * (q - (n - 1 << 1))
+
+
+def A370998(n):
+    ptuple = tuple(prime(k) for k in range(1, n + 1))
+    return (
+        next(filter(lambda m: not any(isprime(p + m) for p in ptuple), count(2, 2)))
+        >> 1
+    )
+
+
+def A371052_gen():  # generator of terms
+    return (
+        (3**b * (3**a - 1) + (3**b - 1 >> 1)) * 3 ** (l - a - b)
+        for l in count(3)
+        for a in range(1, l - 1)
+        for b in range(1, l - a)
+    )
+
+
+def A371053_gen():  # generator of terms
+    return (
+        (10**b * (10**a - 1 << 1) + 10**b - 1) // 9 * 10 ** (l - a - b)
+        for l in count(3)
+        for a in range(1, l - 1)
+        for b in range(1, l - a)
+    )
+
+
+def A371399(n):
+    return sum(
+        comb(k + n, k) * comb((n << 1) - k, n) * (-1 if k & 1 else 1) << n - k
+        for k in range(n + 1)
+    )
+
+
+def A371384(n):
+    return (l := len(s := str(n))) // gcd(l, sum(map(int, s)))
+
+
+def A371383(n):
+    return (l := sum(map(int, (s := str(n))))) // gcd(l, len(s))
+
+
+def A371070(n):
+    CM = (
+        lambda x, y, z, t, u, v: (x * y * z << 2)
+        + (a := x + y - t) * (b := x + z - u) * (c := y + z - v)
+        - x * c**2
+        - y * b**2
+        - z * a**2
+    )
+    TR1 = lambda x, y, z: not (x + y < z or x + z < y or y + z < x)
+    TR = (
+        lambda x, y, z, t, u, v: TR1(t, u, v)
+        and TR1(x, y, t)
+        and TR1(x, z, u)
+        and TR1(y, z, v)
+    )
+    c, d, sq = 0, set(), tuple(x**2 for x in range(n + 1))
+    for s, w in partitions(n, m=6, k=n - 5, size=True):
+        if s == 6:
+            for v in multiset_permutations(Counter(w).elements()):
+                if (
+                    TR(*v)
+                    and (
+                        M := CM(
+                            sq[v[0]], sq[v[1]], sq[v[2]], sq[v[3]], sq[v[4]], sq[v[5]]
+                        )
+                    )
+                    > 0
+                    and M not in d
+                ):
+                    d.add(M)
+                    c += 1
+    return c
+
+
+def A181790_gen():  # generator of terms
+    for j in count(9):
+        b = 10**j
+        a = b * 10 + 1
+        for k in sorted(sqrt_mod(0, a, all_roots=True)):
+            if a * b <= k**2 < a * (a - 1) and len(set(str(m := k**2 // a))) == 10:
+                yield m
+
+
+def A181789_gen():  # generator of terms
+    for j in count(9):
+        b = 10**j
+        a = b * 10 + 1
+        for k in sorted(sqrt_mod(0, a, all_roots=True)):
+            if a * b <= (m := k**2) < a * (a - 1) and len(set(str(m // a))) == 10:
+                yield m
+
+
+def A370980(n):
+    return n * (n - 1 >> 1) + 1
+
+
+def A186995(n):
+    p = 2
+    while True:
+        s = sympydigits(p, n)[1:]
+        for i, j in enumerate(s[::-1]):
+            m = n**i
+            for k in range(n):
+                if k != j and isprime(p + (k - j) * m):
+                    break
+            else:
+                continue
+            break
+        else:
+            return p
+        p = nextprime(p)
+
+
+def A371475(n):
+    if n == 1:
+        return 2
+    p, r = 5, (n << 1) + 1
+    while True:
+        s = sympydigits(p, r)[1:]
+        for i, j in enumerate(s[::-1]):
+            m = r**i
+            for k in range(j & 1, r, 2):
+                if k != j and isprime(p + (k - j) * m):
+                    break
+            else:
+                continue
+            break
+        else:
+            return p
+        p = nextprime(p)
+
+
+def A369793(n):
+    return sum(
+        1
+        for m in range(1, (n**2 >> 2) + 1)
+        if (d := divisors(m))[((l := len(d)) - 1) >> 1] + d[l >> 1] == n
+    )
+
+
+def A323745(n):
+    p = 2
+    while True:
+        m = 1
+        for j in sympydigits(p, n)[:0:-1]:
+            for k in range(1, n):
+                if k != j and isprime(p + (k - j) * m):
+                    break
+            else:
+                m *= n
+                continue
+            break
+        else:
+            return p
+        p = nextprime(p)
+
+
+def A371509(n):
+    if n == 1:
+        return 2
+    p, r = 5, (n << 1) + 1
+    while True:
+        m = 1
+        for j in sympydigits(p, r)[:0:-1]:
+            for k in range(2 - (j & 1), r, 2):
+                if k != j and isprime(p + (k - j) * m):
+                    break
+            else:
+                m *= r
+                continue
+            break
+        else:
+            return p
+        p = nextprime(p)
+
+
+def A371474_gen():  # generator of terms
+    return filter(lambda k: not comb(k**2, k) % (k**3), count(1))
+
+
+def A006003(n):
+    return n * (n**2 + 1) >> 1
+
+
+def A002623(n):
+    return ((n + 2) * (n + 4) * ((n << 1) + 3) >> 3) // 3
+
+
+def A004613_gen(startvalue=1):  # generator of terms >= startvalue
+    return filter(
+        lambda n: all(p & 3 == 1 for p in primefactors(n)), count(max(startvalue, 1))
+    )
+
+
+def A371055_gen():  # generator of terms
+    return (
+        10 ** (l - a) * ((10**a - 1) // 9) + ((10**b - 1) // 9 << 1)
+        for l in count(3)
+        for a in range(1, l - 1)
+        for b in range(1, l - a)
+    )
+
+
+def A371057_gen():  # generator of terms
+    return (
+        10 ** (l - a) * ((10**a - 1) // 9 << 1) + ((10**b - 1) // 9)
+        for l in count(3)
+        for a in range(1, l - 1)
+        for b in range(1, l - a)
+    )
+
+
+def A370848_gen():  # generator of terms
+    for l in count(1):
+        k = (10**l - 1) // 9
+        for m in range(l):
+            a = 10**m
+            for j in (1, 2, 4, 6):
+                p = k + a * j
+                if isprime(p) and not isprime(sum(map(int, str(nextprime(p))))):
+                    yield p
+
+
+def A370851_gen():  # generator of terms
+    for l in count(1):
+        k = (10**l - 1) // 9
+        for m in range(l):
+            a = 10**m
+            for j in (1, 2, 4, 6):
+                p = k + a * j
+                if isprime(p) and not (
+                    isprime(s := prod(map(int, str(nextprime(p))))) or s == 1
+                ):
+                    yield p
+
+
+def A264828_gen(startvalue=1):  # generator of terms >= startvalue
+    return filter(
+        lambda n: not (isprime(n) or (n & 1 ^ 1 and isprime(n >> 1))),
+        count(max(startvalue, 1)),
+    )
+
+
+def A370759_gen(startvalue=4):  # generator of terms >= startvalue
+    return filter(
+        lambda n: not (isprime(n + 5) or (n & 1 and isprime((n >> 1) + 3))),
+        count(max(startvalue, 4)),
+    )
+
+
+def A371402(n):
+    return (
+        (
+            (~n & n - 1).bit_length() + 2 << (n << 1)
+            if n & 1
+            else ((m := (~n & n - 1).bit_length()) + 1 << (n << 1) + 1) - m
+        )
+        if n
+        else 0
+    )
+
+
+def A371459(n):
+    return int(bin(n)[3::2], 2) if n > 1 else 0
+
+
+def A371347(n):
+    return nextprime((m := prime(n)) ** m)
+
+
+def A371346(n):
+    return prevprime((m := prime(n)) ** m)
+
+
+def A370071_gen():  # generator of terms
+    a, b = 1, 2
+    yield from (0, 1)
+    while True:
+        s = sorted(str(b))
+        l = len(s)
+        m = int("".join(s[::-1]))
+        u = int("".join(s))
+        for i in count(2):
+            if i**2 > m:
+                break
+            startcount = max(2, integer_log(u, i)[0])
+            k = i**startcount
+            for j in count(startcount):
+                if k > m:
+                    break
+                t = sorted(str(k))
+                if ["0"] * (l - len(t)) + t == s:
+                    yield b
+                    break
+                k *= i
+            else:
+                continue
+            if k <= m:
+                break
+        a, b = b, a + b
+
+
+def A370796(n):
+    return (
+        -primepi(((p := prime(n)) + 1) ** 2) + primepi((nextprime(p) - 1) ** 2)
+        if n > 1
+        else 2
+    )
+
+
+def A371462_gen(startvalue=0):  # generator of terms >= startvalue
+    return filter(
+        lambda n: sum(map(int, (s := str(n)))) ** 2 << 1
+        == len(s) * sum(int(d) ** 2 for d in s),
+        count(max(startvalue, 0)),
+    )
+
+
+def A371588(n):
+    a, b = 1, 2
+    while True:
+        s = sorted(str(b))
+        l = len(s)
+        m = int("".join(s[::-1]))
+        u = int("".join(s))
+        for i in count(max(2, integer_nthroot(u, n)[0])):
+            if (k := i**n) > m:
+                break
+            t = sorted(str(k))
+            if ["0"] * (l - len(t)) + t == s:
+                return b
+                break
+        a, b = b, a + b
+
+
+def A371589(n):
+    a, b = 1, 2
+    while True:
+        s = sorted(str(b))
+        m = int("".join(s[::-1]))
+        u = int("".join(s))
+        for i in count(max(2, integer_nthroot(u, n)[0])):
+            if (k := i**n) > m:
+                break
+            t = sorted(str(k))
+            if t == s:
+                return i
+                break
+        a, b = b, a + b
+
+
+def A115419(n):
+    return ((n - 1 << 1) & -7 | 8) + (n - 1 & 7)
+
+
+def A115420(n):
+    return ((n - 1 << 1) & -15 | 16) + (n - 1 & 15)
+
+
+def A115421(n):
+    return ((n - 1 << 1) & -31 | 32) + (n - 1 & 31)
+
+
+def A007429(n):
+    return prod(
+        (p * (p ** (e + 1) - 1) - (p - 1) * (e + 1)) // (p - 1) ** 2
+        for p, e in factorint(n).items()
+    )
+
+
+def A371003(n):
+    return comb((n << 1) - 1, n) - n - ((m := (n - 1) ** 2) * (m + 3) >> 2)
+
+
+def A106277(n):
+    from sympy.abc import x
+
+    return len(
+        Poly(x * (x * (x * (x - 1) - 1) - 1) - 1, x, modulus=prime(n)).ground_roots()
+    )
+
+
+def A047461(n):
+    return (n - 1 << 2) | (n & 1)
+
+
+def A369801(n):
+    return (n - 2 << 2) - (n & 1) if n >= 7 else (1, 3, 6, 10, 15)[n - 2]
+
+
+def A047452(n):
+    return (n << 2) - 2 - (n & 1)
+
+
+def A047470(n):
+    return (n - 1 << 2) - (n & 1 ^ 1)
+
+
+def A075123(n):
+    return (n - 2 << 2) - 2 - (n & 1) if n > 3 else n
+
+
+def A047617(n):
+    return (n - 1 << 2) + 1 + (n & 1)
+
+
+def A047524(n):
+    return (n << 2) - 1 - (n & 1)
+
+
+def A047535(n):
+    return (n << 2) - (n & 1 ^ 1)
+
+
+def A047398(n):
+    return ((n << 2) | (n & 1)) - 2
+
+
+def A047615(n):
+    return (n << 2) - 3 - (n & 1)
+
+
+def A371463_gen(startvalue=0):  # generator of terms >= startvalue
+    return filter(
+        lambda n: 5 * sum(s := tuple(map(int, str(n)))) ** 2
+        == len(s) * sum(d**2 for d in s) << 2,
+        count(max(startvalue, 0)),
+    )
+
+
+def A371464_gen(startvalue=0):  # generator of terms >= startvalue
+    return filter(
+        lambda n: 10 * sum(s := tuple(map(int, str(n)))) ** 2
+        == 9 * len(s) * sum(d**2 for d in s),
+        count(max(startvalue, 0)),
+    )
+
+
+def A371532(n):
+    return n * (n * (5 * n + 6 << 2) + 10) // 3 + 1
+
+
+def A371515(n):
+    return n * (n * (32 * n + 18) + 6) + 1
+
+
+def A039269_gen(startvalue=0):  # generator of terms >= startvalue
+    return filter(
+        lambda n: (s := sympydigits(n, 12)[1:]).count(8) == s.count(9),
+        count(max(startvalue, 0)),
+    )
+
+
+def A371651(n):
+    p = 3
+    while True:
+        if n == primeomega(p - 2) == primeomega(p + 2):
+            return p
+        p = nextprime(p)
+
+
+def A371573(n):
+    return n if (p := min(factorint(n).items(), default=(1, 1)))[1] == 1 else n // p[0]
+
+
+def A371670(n):
+    p = n**4
+    while p := prevprime(p):
+        pset = set(q := tuple(pow(x, n, p) for x in range(p)))
+        if not all(
+            any(
+                (k - a[0] - a[1]) % p in pset
+                for a in combinations_with_replacement(q, 2)
+            )
+            for k in range(p)
+        ):
+            return p
+
+
+def A368055(n):
+    p = 1
+    while p := nextprime(p):
+        pset = set(q := tuple(pow(x, n, p) for x in range(p)))
+        if not all(
+            any(
+                (k - a[0] - a[1]) % p in pset
+                for a in combinations_with_replacement(q, 2)
+            )
+            for k in range(p)
+        ):
+            return p
+
+
+def A309805(n):
+    return n**2 - (m := n >> 1) * (m + 1)
+
+
+def A133090(n):
+    return (n << 1) - 1 if n & 1 else n - 1
+
+
+def A371706(n):
+    m = n
+    for k in count(1):
+        if "1" in str(m):
+            return k
+        m *= n
+
+
+def A275533(n):
+    return next(
+        m for m in count(1) if not any("1" in str(m**k) for k in range(1, n + 1))
+    )
+
+
+def A178316_gen():  # generator of terms
+    yield from (2, 5)
+    r = "".maketrans("69", "96")
+    for l in count(1):
+        for a in "125689":
+            for d in product("0125689", repeat=l):
+                s = a + "".join(d)
+                m = int(s)
+                if isprime(m) and isprime(int(s[::-1].translate(r))):
+                    yield m
+
+
+def A366494(n):
+    return sum(
+        totient(d) // n_order(10, d)
+        for d in divisors(10 * n - 1, generator=True)
+        if d > 1
+    )
+
+
+def A006694(n):
+    return sum(
+        totient(d) // n_order(2, d)
+        for d in divisors((n + 1 << 1) - 1, generator=True)
+        if d > 1
+    )
+
+
+def A081844(n):
+    return (
+        sum(
+            totient(d) // n_order(2, d)
+            for d in divisors((n + 1 << 1) - 1, generator=True)
+            if d > 1
+        )
+        + 1
+    )
+
+
+def A023142(n):
+    m = n >> (~n & n - 1).bit_length()
+    a, b = divmod(m, 5)
+    while not b:
+        m = a
+        a, b = divmod(m, 5)
+    return (
+        sum(totient(d) // n_order(10, d) for d in divisors(m, generator=True) if d > 1)
+        + 1
+    )
+
+
+def A128858(n):
+    return n_order(10, 10 * n - 1)
+
+
+def A128857(n):
+    return n * (10 ** n_order(10, (m := 10 * n - 1)) - 1) // m
+
+
+def A275028_gen():  # generator of terms
+    r, t = "".maketrans("69", "96"), set("0125689")
+    for l in count(1):
+        if l % 10:
+            m = l**2
+            if set(s := str(m)) <= t and is_square(int(s[::-1].translate(r))):
+                yield m
+
+
+def A371845_gen():  # generator of terms
+    for l in count(1):
+        m = 10**l
+        for a in range(1, 10):
+            b = (a * 10**4 + 2345) * m
+            yield from primerange(b, b + m)
+
+
+def A371833_gen():  # generator of terms
+    for l in count(1):
+        m = 10**l
+        for a in range(1, 10):
+            b = (a * 10**3 + 234) * m
+            yield from primerange(b, b + m)
+
+
+def A018847_gen():  # generator of terms
+    r, t, u = "".maketrans("69", "96"), set("0125689"), {0, 1, 2, 5, 8}
+    for x in count(1):
+        for y in range(10 ** (x - 1), 10**x):
+            if y % 10 in u:
+                s = str(y)
+                if set(s) <= t and isprime(m := int(s + s[-2::-1].translate(r))):
+                    yield m
+        for y in range(10 ** (x - 1), 10**x):
+            s = str(y)
+            if set(s) <= t and isprime(m := int(s + s[::-1].translate(r))):
+                yield m
+
+
+def A371865_gen():  # generator of terms
+    for l in count(1):
+        m = 10**l
+        for a in range(1, 10):
+            b = (a * 10**8 + 23456789) * m
+            yield from primerange(b, b + m)
+
+
+def A000374(n):
+    return (
+        sum(
+            totient(d) // n_order(2, d)
+            for d in divisors(n >> (~n & n - 1).bit_length(), generator=True)
+            if d > 1
+        )
+        + 1
+    )
+
+
+def A023138(n):
+    m = n >> (~n & n - 1).bit_length()
+    a, b = divmod(m, 3)
+    while not b:
+        m = a
+        a, b = divmod(m, 3)
+    return (
+        sum(totient(d) // n_order(6, d) for d in divisors(m, generator=True) if d > 1)
+        + 1
+    )
+
+
+def A023141(n):
+    a, b = divmod(n, 3)
+    while not b:
+        n = a
+        a, b = divmod(n, 3)
+    return (
+        sum(totient(d) // n_order(9, d) for d in divisors(n, generator=True) if d > 1)
+        + 1
+    )
+
+
+def A023139(n):
+    a, b = divmod(n, 7)
+    while not b:
+        n = a
+        a, b = divmod(n, 7)
+    return (
+        sum(totient(d) // n_order(7, d) for d in divisors(n, generator=True) if d > 1)
+        + 1
+    )
+
+
+def A023136(n):
+    return (
+        sum(
+            totient(d) // n_order(4, d)
+            for d in divisors(n >> (~n & n - 1).bit_length(), generator=True)
+            if d > 1
+        )
+        + 1
+    )
+
+
+def A023137(n):
+    a, b = divmod(n, 5)
+    while not b:
+        n = a
+        a, b = divmod(n, 5)
+    return (
+        sum(totient(d) // n_order(5, d) for d in divisors(n, generator=True) if d > 1)
+        + 1
+    )
+
+
+def A371511(n):
+    m, j = n, 0
+    if n > 3:
+        for j in range(1, n - 1):
+            if gcd((n * (n - 1) >> 1) + j, n - 1) == 1:
+                break
+    if j == 0:
+        for i in range(2, n - 1):
+            m = n * m + i
+    elif j == 1:
+        for i in range(1, n - 1):
+            m = n * m + i
+    else:
+        for i in range(2, 1 + j):
+            m = n * m + i
+        for i in range(j, n - 1):
+            m = n * m + i
+    m -= 1
+    while True:
+        s = sympydigits(m := nextprime(m), n)[1:]
+        if n - 1 not in s and len(set(s)) == n - 1:
+            return m
+
+
+def A371512(n):
+    m, j = 1, 0
+    if n > 3:
+        for j in range(1, n - 1):
+            if gcd((n * (n - 1) >> 1) + j, n - 1) == 1:
+                break
+    if j == 0:
+        for i in range(2, n - 1):
+            m = n * m + i
+    elif j == 1:
+        for i in range(1, n - 1):
+            m = n * m + i
+    else:
+        for i in range(2, 1 + j):
+            m = n * m + i
+        for i in range(j, n - 1):
+            m = n * m + i
+    m -= 1
+    while True:
+        s = sympydigits(m := nextprime(m), n)[1:]
+        if (not (0 in s or n - 1 in s)) and len(set(s)) == n - 2:
+            return m
+
+
+def A371653_gen():  # generator of terms
+    for l in count(1):
+        xlist = []
+        for p in combinations_with_replacement("987654321", l):
+            if isprime(int("".join(p))):
+                xlist.extend(int("".join(d)) for d in multiset_permutations(p))
+        yield from sorted(xlist)
+
+
+def A371654_gen():  # generator of terms
+    for l in count(1):
+        xlist = []
+        for p in combinations_with_replacement("0123456789", l):
+            if isprime(int("".join(p))):
+                xlist.extend(
+                    int("".join(d))
+                    for d in multiset_permutations(p)
+                    if d[0] != "0" and d[-1] != "0"
+                )
+        yield from sorted(xlist)
+
+
+def A371811_gen(startvalue=1):  # generator of terms >= startvalue
+    for n in count(max(startvalue, 1)):
+        f = factorint(n)
+        if len(f) == 2 and max(f.values()) == 1:
+            q, p = sorted(f.keys())
+            try:
+                discrete_log(p, q, 2)
+            except:
+                continue
+            yield n
+
+
+def A371821_gen(startvalue=1):  # generator of terms >= startvalue
+    for n in count(max(startvalue, 1)):
+        f = sorted(factorint(n, multiple=True))
+        if len(f) > 1:
+            c = 0
+            for p in f:
+                c = ((c << p.bit_length()) + p) % n
+            if not c:
+                yield n
+
+
+def A371641(n):
+    for m in count(4):
+        f = factorint(m)
+        if sum(f.values()) > 1:
+            c = 0
+            for p in sorted(f):
+                a = pow(n, integer_log(p, n)[0] + 1, m)
+                for _ in range(f[p]):
+                    c = (c * a + p) % m
+            if not c:
+                return m
+
+
+def A337486_gen():  # generator of terms
+    c = 1
+    for n in count(1):
+        a, b = divmod(c, n)
+        if not b:
+            c = a
+            yield n
+        else:
+            c *= n
+
+
+def A370969_gen():  # generator of terms
+    c, m = 1, 1
+    for n in count(2):
+        a, b = divmod(c, n)
+        if not b:
+            yield n - m
+            c, m = a, n
+        else:
+            c *= n
+
+
+@lru_cache(maxsize=None)
+def A008336(n):
+    if n == 1:
+        return 1
+    a, b = divmod(c := A008336(n - 1), n - 1)
+    return c * (n - 1) if b else a
+
+
+def A008336_gen():  # generator of terms
+    m = 1
+    for n in count(1):
+        yield m
+        a, b = divmod(m, n)
+        m = m * n if b else a
+
+
+def A371900_gen(startvalue=2):  # generator of terms >= startvalue
+    for n in count(max(startvalue, 2)):
+        if not isprime(n + 1):
+            q = min(primefactors(n + 1))
+            for m in range(4, q**2):
+                f = factorint(m)
+                if sum(f.values()) > 1:
+                    c = 0
+                    for p in sorted(f):
+                        a = pow(n, integer_log(p, n)[0] + 1, m)
+                        for _ in range(f[p]):
+                            c = (c * a + p) % m
+                    if not c:
+                        yield n
+                        break
+
+
+def A033880(n):
+    return divisor_sigma(n) - (n << 1)
+
+
+def A033879(n):
+    return (n << 1) - divisor_sigma(n)
+
+
+def A152016(n):
+    return n * (n * (n * (n - 1) - 1) - 1)
+
+
+def A371696_gen(startvalue=4):  # generator of terms >= startvalue
+    for n in count(max(startvalue, 4)):
+        f = factorint(n)
+        if sum(f.values()) > 1:
+            c = 0
+            for p in sorted(f, reverse=True):
+                a = pow(10, len(s := str(p)), n)
+                q = int(s[::-1])
+                for _ in range(f[p]):
+                    c = (c * a + q) % n
+            if not c:
+                yield n
+
+
+def A371666_gen(startvalue=4):  # generator of terms >= startvalue
+    for n in count(max(startvalue, 4)):
+        f = factorint(n)
+        if sum(f.values()) > 1:
+            c = 0
+            for p in sorted(f, reverse=True):
+                a, q = p.bit_length(), int(bin(p)[:1:-1], 2)
+                for _ in range(f[p]):
+                    c = (c << a) + q
+            if c == n:
+                yield n
+
+
+def A055773(n):
+    return prod(primerange((n >> 1) + 1, n + 1))
+
+
+def A371948_gen(startvalue=2):  # generator of terms >= startvalue
+    for n in count(max(startvalue, 2)):
+        if not isprime(n + 1):
+            q = min(primefactors(n + 1))
+            for m in range(4, q**2):
+                f = factorint(m)
+                if sum(f.values()) > 1:
+                    c = 0
+                    for p in sorted(f, reverse=True):
+                        a = pow(n, integer_log(p, n)[0] + 1, m)
+                        for _ in range(f[p]):
+                            c = (c * a + p) % m
+                    if not c:
+                        yield n
+                        break
+
+
+def A116667(n):
+    s = set(str(n))
+    for i in range(9, -1, -1):
+        if str(i) not in s:
+            return i
+    return 10
+
+
+def A067898(n):
+    s = set(str(n))
+    for i in range(10):
+        if str(i) not in s:
+            return i
+    return 10
+
+
+def A371390_gen():  # generator of terms
+    xlist, p = [2, 3, 5, 7, 1], 11
+    for k in count(1):
+        if len(set(xlist)) == 1:
+            yield k
+        p = nextprime(p)
+        xlist = xlist[1:] + [p % 10]
+
+
+def A322843_gen(startvalue=4):  # generator of terms >= startvalue
+    for m in count(max(startvalue, 4)):
+        f = factorint(m, multiple=True)
+        if len(f) > 1:
+            c = 0
+            a = {p: pow(10, len(str(p)), m) for p in f}
+            for g in multiset_permutations(f):
+                c = 0
+                for p in g:
+                    c = (c * a[p] + p) % m
+                if not c:
+                    yield m
+                    break
+
+
+@lru_cache(maxsize=None)
+def A358552(n):
+    if n == 1:
+        return 1
+    if isprime(n):
+        return 1 + A358552(primepi(n))
+    return max(A358552(p) for p in primefactors(n))
+
+
+def A371908_gen():  # generator of terms
+    m = 1
+    for n in count(1, 2):
+        a, b = divmod(m, n)
+        m = m * n if b else a
+        yield (~m & m - 1).bit_length()
+        a, b = divmod(m, n + 1)
+        m = m * (n + 1) if b else a
+
+
+def A371965(n):
+    return sum(comb((n - i << 1) - 3, n - i - 3) for i in range(n - 2))
+
+
+def A371964(n):
+    return sum(comb((n - i << 1) - 4, n - i - 4) for i in range(n - 3))
+
+
+def A371963(n):
+    return sum(comb((n - i << 1) - 3, n - i - 4) for i in range(n - 3))
+
+
+def A086330(n):
+    a, c = 0, 1
+    for m in range(2, n):
+        c = c * m % n
+        if c == 0:
+            break
+        a += c
+    return a
+
+
+def A371035(n):
+    a, c, p = 0, 1, prime(n)
+    for m in range(2, p):
+        c = c * m % p
+        a += c
+    return a
+
+
+def A226570(n):
+    a, c = 0, 1
+    for m in range(2, n):
+        c = c * m % n
+        if c == 0:
+            break
+        a = (a + c) % n
+    return a
+
+
+def A100083_gen(startvalue=1):  # generator of terms >= startvalue
+    for n in count(max(startvalue, 1)):
+        a, c = 0, 1
+        for m in range(2, n):
+            c = c * m % n
+            if c == 0:
+                break
+            a = (a + c) % n
+        if not a:
+            yield n
+
+
+def A372010(n):
+    return 10 ** (a := n >> 1) * (10 ** (a - (n & 1 ^ 1)) + 1) - 1
+
+
+def A014682(n):
+    return (3 * n + 1 if n & 1 else n) >> 1
+
+
+def A370952_gen():  # generator of terms
+    a, aset = 1, {0, 1}
+    for p in count(3, 2):
+        yield a
+        for b in count(a % p, p):
+            if b not in aset:
+                aset.add(b)
+                a = b
+                break
+
+
+def A370975_gen():  # generator of terms
+    a, aset = 1, {0, 1}
+    for p in count(3, 2):
+        for b in count(a % p, p):
+            if b not in aset:
+                aset.add(b)
+                yield (b - a) // p
+                a = b
+                break
+
+
+def A372052(n):
+    a, aset = 1, {0, 1}
+    for p in count(3, 2):
+        if a == n:
+            return p >> 1
+        for b in count(a % p, p):
+            if b not in aset:
+                aset.add(b)
+                a = b
+                break
+
+
+def A371561_gen():  # generator of terms
+    for l in count(1):
+        for a in range(l, -1, -1):
+            a3 = 3**a
+            for b in range(l - a, -1, -1):
+                b3 = a3 * 5**b
+                for c in range(l - a - b, -1, -1):
+                    d = l - a - b - c
+                    d3 = b3 * 7**c * 9**d
+                    while d3 > 9:
+                        d3 = prod(int(x) for x in str(d3))
+                    if d3 == 5:
+                        yield (10 ** (a + b + c + d) - 1) // 3 + (
+                            10**d * (10**c * (10**b + 1) + 1) - 3 << 1
+                        ) // 9
+
+
+def A028356(n):
+    return (1, 2, 3, 4, 3, 2)[n % 6]
+
+
+def A212801_T(m, n):
+    return simplify(
+        prod(
+            2 - exp(2 * I * h * pi / m) - exp(2 * I * k * pi / n)
+            for k in range(1, n)
+            for h in range(1, m)
+        )
+    )
+
+
+def A371093(n):
+    return ((m := 3 * n) & ~(m + 1)).bit_length()
+
+
+def A371560(n):
+    return factorial(n) ** 4 * (n + 1) ** 3
+
+
+def A224900(n):
+    return factorial(n) ** 3 * (n + 1) ** 2
+
+
+def A172492(n):
+    return factorial(n) ** 3 * (n + 1)
+
+
+def A090443(n):
+    return factorial(n) ** 3 * (n + 2) * (n + 1) ** 2 >> 1
+
+
+def A090444(n):
+    return factorial(n) ** 4 * (n + 3) * (n + 2) ** 2 * (n + 1) ** 3 // 12
+
+
+def A010790(n):
+    return factorial(n) ** 2 * (n + 1)
+
+
+def A126120(n):
+    return 0 if n & 1 else comb(n, m := n >> 1) // (m + 1)
+
+
+def A371623_gen(startvalue=1):  # generator of terms >= startvalue
+    p = max(startvalue - 1, 0)
+    while p := nextprime(p):
+        if isprime(q := p << 1 | 1) and sorted(str(p)) == sorted(str(q)):
+            yield p
+
+
+def A372029_gen():  # generator of terms
+    c = {
+        "1": "12357",
+        "2": "2357",
+        "3": "357",
+        "4": "57",
+        "5": "57",
+        "6": "7",
+        "7": "7",
+    }
+    for l in count(1):
+        for d in combinations_with_replacement("1234567", l):
+            for e in c[d[-1]]:
+                n = int("".join(d) + (a := e))
+                if not isprime(n):
+                    for p in factorint(n, multiple=True):
+                        s = str(p)
+                        if s[0] < a or sorted(s) != list(s):
+                            break
+                        a = s[-1]
+                    else:
+                        yield n
+
+
+def A372046_gen(startvalue=4):  # generator of terms >= startvalue
+    for n in count(max(startvalue, 4)):
+        f = factorint(n)
+        if sum(f.values()) > 1:
+            c = 0
+            for p in sorted(f):
+                a = pow(10, len(s := str(p)), n)
+                q = int(s[::-1])
+                for _ in range(f[p]):
+                    c = (c * a + q) % n
+            if not c:
+                yield n
+
+
+def A272799_gen(startvalue=1):  # generator of terms >= startvalue
+    return filter(
+        lambda k: max(factorint((k << 1) - 1).values(), default=1) == 1
+        and max(factorint((k << 1) + 1).values()) == 1,
+        count(max(startvalue, 1)),
+    )
+
+
+def A067874_gen(startvalue=2):  # generator of terms >= startvalue
+    return filter(
+        lambda k: max(factorint(k - 1).values(), default=1) == 1
+        and max(factorint(k + 1).values()) == 1,
+        count(max(startvalue + (startvalue & 1), 2), 2),
+    )
+
+
+def A372277_gen(startvalue=4):  # generator of terms >= startvalue
+    for n in count(max(startvalue, 4)):
+        f = factorint(n)
+        if sum(f.values()) > 1:
+            c = 0
+            for p in sorted(f):
+                a = pow(2, len(s := bin(p)[2:]), n)
+                q = int(s[::-1], 2)
+                for _ in range(f[p]):
+                    c = (c * a + q) % n
+            if not c:
+                yield n
+
+
+def A371597(n):
+    return sum(
+        filter(
+            lambda m: (d := divisors(m))[((l := len(d)) - 1) >> 1] + d[l >> 1] == n,
+            range(1, (n**2 >> 2) + 1),
+        )
+    )
+
+
+def A369110(n):
+    c = {n}
+    while n < 4 or n > 5:
+        c.add(n := (d := divisors(n))[((l := len(d)) - 1) >> 1] + d[l >> 1])
+    if n == 5:
+        c.add(6)
+    return len(c)
+
+
+def A371924(n):
+    m = prime(n) - 1
+    b, k = 1, 1 % m
+    while k:
+        b += 1
+        k = k * b % m
+    return b
+
+
+def A370482(n):
+    return isprime(n) + (n & 1 ^ 1)
+
+
+def A370469_T(n, k):
+    return comb(k - 1, n - 1) << n
+
+
+def A306284(n):
+    y, a = 0, set()
+    for x in count(0):
+        if y in a:
+            return x
+        a.add(y)
+        y = (y + (x << 1) + 1) % n
+
+
+def A138191(n):
+    return (1, 1, 2, 1)[n & 3]
+
+
+def A371124(n):
+    y, a = 0, {}
+    for x in count(0):
+        if y in a:
+            return a[y]
+        a[y] = x
+        y = (y + (x << 1) + 1) % n
+
+
+def A371252_gen():  # generator of terms
+    a, b, c = 1, 9, 297
+    yield from (a, b)
+    for k in count(3):
+        yield c
+        a, b, c = (
+            b,
+            c,
+            (
+                3888 * a
+                - 4338 * b
+                + 738 * c
+                + k
+                * (
+                    -42120 * a
+                    + 43839 * b
+                    - 7263 * c
+                    + k
+                    * (
+                        154548 * a
+                        - 162865 * b
+                        + 29297 * c
+                        + k
+                        * (
+                            -238302 * a
+                            + 274917 * b
+                            - 60393 * c
+                            + k
+                            * (
+                                174636 * a
+                                - 233053 * b
+                                + 66698 * c
+                                + k
+                                * (
+                                    -60750 * a
+                                    + 97800 * b
+                                    - 37350 * c
+                                    + k * (8100 * a - 16300 * b + 8300 * c)
+                                )
+                            )
+                        )
+                    )
+                )
+            )
+            // (k**3 * (k * (k * (100 * k - 300) + 281) - 78)),
+        )
+
+
+def A059074_gen():  # generator of terms
+    a, b, c, d = 1, 0, 1, 346
+    yield from (a, b, c)
+    for k in count(4):
+        yield d
+        a, b, c, d = (
+            b,
+            c,
+            d,
+            (
+                k
+                * (
+                    -222912 * a
+                    - 151968 * b
+                    + 185062 * c
+                    + 4179 * d
+                    + k
+                    * (
+                        588384 * a
+                        + 462000 * b
+                        - 474198 * c
+                        - 38670 * d
+                        + k
+                        * (
+                            -856512 * a
+                            - 725040 * b
+                            + 672688 * c
+                            + 75248 * d
+                            + k
+                            * (
+                                995616 * a
+                                + 849696 * b
+                                - 777792 * c
+                                - 92992 * d
+                                + k
+                                * (
+                                    -739584 * a
+                                    - 651264 * b
+                                    + 592384 * c
+                                    + 62720 * d
+                                    + k
+                                    * (
+                                        271872 * a
+                                        + 253440 * b
+                                        - 235008 * c
+                                        - 24064 * d
+                                        + k * (36864 * (c - b - a) + 4096 * d)
+                                        + 8192
+                                    )
+                                    - 28672
+                                )
+                                + 23680
+                            )
+                            - 7904
+                        )
+                        + 1416
+                    )
+                    + 14382
+                )
+                - 1611
+            )
+            // (k * (k * (384 * k - 1680) + 2520) - 1611),
+        )
+
+
+def A372289(n):
+    return (n << (e := (~n & n - 1).bit_length())) + ((1 << (e << 1)) - 1) // 3
+
+
+def A372228(n):
+    return max(max(primefactors(n), default=1), max(primefactors(n ** (n - 1) + 1)))
+
+
+def A372229(n):
+    return max(
+        max(primefactors(n), default=1), max(primefactors(n ** (n - 1) - 1), default=1)
+    )
+
+
+def A370397(n):
+    return prod(range(5, (n << 2) + 2, 4)) >> (n << 1)
+
+
+def A372204(n):
+    return len(num2words(n, ordinal=True, lang="it"))
+
+
+def A026858(n):
+    return len(num2words(n, lang="it"))
+
+
+def A371094(n):
+    return ((m := 3 * n + 1) << (e := (~m & m - 1).bit_length())) + (
+        (1 << (e << 1)) - 1
+    ) // 3
+
+
+def A372351(n):
+    return ((m := 6 * n - 2) << (e := (~m & m - 1).bit_length())) + (
+        (1 << (e << 1)) - 1
+    ) // 3
+
+
+def A372385(n):
+    return Matrix(
+        n - 1,
+        n - 1,
+        [
+            jacobi_symbol(i - j, (n << 1) | 1)
+            for i in range(n - 1)
+            for j in range(n - 1)
+        ],
+    ).det()
+
+
+def A086893(n):
+    return (1 << n + 1 if n & 1 else 5 << n - 1) // 3
+
+
+def A372381(n):
+    return prod(1 << (e + 1).bit_length() - 1 for e in factorint(n).values())
+
+
+def A372380(n):
+    return prod((e + 1).bit_length() for e in factorint(n).values())
+
+
+def A372379(n):
+    return prod(
+        p ** ((1 << (e + 1).bit_length() - 1) - 1) for p, e in factorint(n).items()
+    )
+
+
+def A370612(n):
+    return next(
+        k
+        for k in count(max(factorial(n - 1), 2))
+        if 0
+        not in (s := set.union(*(set(sympydigits(p, n)[1:]) for p in primefactors(k))))
+        and len(s) == n - 1
+    )
+
+
+def A372394(n):
+    return Matrix(
+        n - 1 << 1,
+        n - 1 << 1,
+        [
+            jacobi_symbol(i * (i + 5 * j + 14) + j * (5 * j + 30) + 44, (n << 1) | 1)
+            for i in range(n - 1 << 1)
+            for j in range(n - 1 << 1)
+        ],
+    ).det()
+
+
+def A372409(n):
+    return Matrix(
+        n - 1,
+        n - 1,
+        [
+            jacobi_symbol(i - j, (n << 1) | 1) if i else 1
+            for i in range(n - 1)
+            for j in range(n - 1)
+        ],
+    ).det()
+
+
+def A120286(n):
+    return sum(Fraction(n - i + 1, i**2) for i in range(1, n + 1)).numerator
+
+
+def A370774(n):
+    return sum(Fraction(n - i + 1, i**2) for i in range(1, n + 1)).denominator
+
+
+def A370048(n):
+    return (
+        0
+        if n < 2
+        else 1
+        + sum(
+            (x := comb((k := m << 1), m + 1) * comb(n - 1 - k, m))
+            + x * (k + 1) * (n - 1 - 3 * m) // (m * (n - 1 - k))
+            for m in range(1, (n + 2) // 3)
+        )
+    )
+
+
+def A163493(n):
+    return (
+        2
+        + sum(
+            (x := comb((k := m << 1) - 1, m) * comb(n - k, m))
+            + (x * (n - 3 * m) << 1) // (n - k)
+            for m in range(1, n // 3 + 1)
+        )
+        if n
+        else 1
+    )
+
+
+def A372457(n):
+    if n == 1:
+        return 1
+    p, m, r = 7, None, None
+    while m is None or p**n <= m:
+        if (
+            k := min((r >> 1 for r in sqrt_mod_iter(-3, p**n) if r & 1), default=None)
+        ) is not None:
+            m = (r := k if r is None else min(r, k)) * (r + 1) + 1
+        while (p := nextprime(p)) % 6 != 1:
+            pass
+    return r
+
+
+def A372060(n):
+    if n < 3:
+        return n
+    l1, l2, s, b, k = 2, 1, 3, set(), 3
+    while True:
+        for i in count(s):
+            if not (i in b or i & l1) and i & l2:
+                if i == n:
+                    return k
+                k += 1
+                l2, l1 = l1, i
+                b.add(i)
+                while s in b:
+                    b.remove(s)
+                    s += 1
+                break
+
+
+def A364722_gen(startvalue=1):  # generator of terms >= startvalue
+    if startvalue <= 1:
+        yield 1
+    if startvalue <= 3:
+        yield 3
+    for k in count(max(startvalue, 4)):
+        for d in (r >> 1 for r in sqrt_mod_iter(-3, k) if r & 1):
+            try:
+                discrete_log(k, d, 2)
+            except:
+                continue
+            yield k
+            break
+
+
+def A364724_gen():  # generator of terms
+    yield 0
+    for k in count(2):
+        m = None
+        for d in sqrt_mod_iter(-3, k):
+            r = d >> 1 if d & 1 else d + k >> 1
+            try:
+                m = (
+                    discrete_log(k, r, 2)
+                    if m is None
+                    else min(m, discrete_log(k, r, 2))
+                )
+            except:
+                continue
+        if m is not None:
+            yield m
+
+
+def A125611(n):
+    m = 7**n
+    r = sorted(nthroot_mod(1, 6, m, all_roots=True))
+    for i in count(0, m):
+        for p in r:
+            if isprime(i + p):
+                return i + p
+
+
+def A125612(n):
+    m = 11**n
+    r = sorted(nthroot_mod(1, 10, m, all_roots=True))
+    for i in count(0, m):
+        for p in r:
+            if isprime(i + p):
+                return i + p
+
+
+def A125646(n):
+    m = (p := prime(n)) ** 5
+    r = sorted(nthroot_mod(1, p - 1, m, all_roots=True))
+    for i in count(0, m):
+        for a in r:
+            if isprime(i + a):
+                return i + a
+
+
+def A070183_gen(startvalue=2):  # generator of terms >= startvalue
+    p = max(nextprime(startvalue - 1), 2)
+    while True:
+        if is_nthpow_residue(2, 6, p) and not is_nthpow_residue(2, 36, p):
+            yield p
+        p = nextprime(p)
+
+
+def A014755_gen(startvalue=2):  # generator of terms >= startvalue
+    p = max(nextprime(startvalue - 1), 2)
+    while True:
+        if p & 7 == 1 and is_nthpow_residue(3, 4, p) and is_nthpow_residue(-3, 4, p):
+            yield p
+        p = nextprime(p)
+
+
+def A372304(n):
+    return sum(comb(n, k) * (k ^ k >> 1) for k in range(n + 1))
+
+
+def A372264(n):
+    return factorial(n) - (n - 1) ** 2
+
+
+def A371217(n):
+    return n + (
+        (n - 1)
+        * sum(
+            factorial(n - 1) // ((i + 1) * factorial(n - i - 2)) for i in range(n - 1)
+        )
+        << 1
+    )
+
+
+def A372494(n):
+    k = (1 << n) - 1
+    k2 = k >> 1
+    return min(
+        (d >> 1 if d & 1 else (d >> 1) + k2 for d in sqrt_mod_iter(-3, k)), default=-1
+    )
+
+
+def A145296_gen():  # generator of terms
+    p = 1
+    while p := nextprime(p):
+        if p & 3 == 1:
+            yield min(sqrt_mod_iter(-1, p**3))
+
+
+def A145299_gen():  # generator of terms
+    p = 1
+    while p := nextprime(p):
+        if p & 3 == 1:
+            yield min(sqrt_mod_iter(-1, p**6))
+
+
+def A145298_gen():  # generator of terms
+    p = 1
+    while p := nextprime(p):
+        if p & 3 == 1:
+            yield min(sqrt_mod_iter(-1, p**5))
+
+
+def A145297_gen():  # generator of terms
+    p = 1
+    while p := nextprime(p):
+        if p & 3 == 1:
+            yield min(sqrt_mod_iter(-1, p**4))
+
+
+def A059321_gen():  # generator of terms
+    p = 1
+    while p := nextprime(p):
+        if p & 3 == 1:
+            yield min(sqrt_mod_iter(-1, p**2))
+
+
+def A227220(n):
+    k, a = 10**n << 1, (10**n - 1) // 3 << 2
+    m = (a << 2) + 1
+    return (
+        min(
+            b
+            for b in ((d >> 1) * ((d >> 1) + 1) for d in sqrt_mod_iter(m, k) if d & 1)
+            if b % k == a
+        )
+        >> 1
+    )
+
+
+def A227219(n):
+    k, a = 10**n << 1, 10 * (10**n - 1) // 9
+    m = (a << 2) + 1
+    return (
+        min(
+            b
+            for b in ((d >> 1) * ((d >> 1) + 1) for d in sqrt_mod_iter(m, k) if d & 1)
+            if b % k == a
+        )
+        >> 1
+    )
+
+
+def A229262(n):
+    if n == 2:
+        return 153
+    c = n * (n + 1) >> 1
+    k, a = 10 ** len(str(c)) << 1, c << 1
+    m = (a << 2) + 1
+    return (
+        min(
+            (
+                b
+                for b in (
+                    (d >> 1) * ((d >> 1) + 1) for d in sqrt_mod_iter(m, k) if d & 1
+                )
+                if b > a and b % k == a
+            )
+        )
+        >> 1
+    )
```

### Comparing `OEISsequences-0.2.3.3/setup.py` & `OEISsequences-0.2.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 with open("requirements.txt", "r") as fh:
     requirements = [line.strip() for line in fh]
 
 setup(
    name='OEISsequences',
    python_requires='>= 3.8',
-   version='0.2.3.3',
+   version='0.2.3.4',
    author='Chai Wah Wu',
    author_email='cwwuieee@gmail.com',
    packages=find_packages(),
    url='https://github.com/postvakje/oeis-sequences',
    license='LICENSE',
    description='Python functions to generate OEIS sequences',
    long_description=long_description,
```

