# Comparing `tmp/pakettic-1.3.1.tar.gz` & `tmp/pakettic-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pakettic-1.3.1.tar", max compression
+gzip compressed data, was "pakettic-1.4.0.tar", max compression
```

## Comparing `pakettic-1.3.1.tar` & `pakettic-1.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1092 2023-02-13 17:06:22.498880 pakettic-1.3.1/LICENSE
--rw-r--r--   0        0        0        0 2023-02-13 17:06:22.519816 pakettic-1.3.1/pakettic/__init__.py
--rw-r--r--   0        0        0       42 2023-02-13 17:06:22.520811 pakettic-1.3.1/pakettic/__main__.py
--rw-r--r--   0        0        0     7096 2023-08-20 12:48:35.551820 pakettic-1.3.1/pakettic/ast.py
--rw-r--r--   0        0        0    13264 2023-09-27 05:25:47.524227 pakettic-1.3.1/pakettic/main.py
--rw-r--r--   0        0        0    25002 2023-08-21 17:25:49.523688 pakettic-1.3.1/pakettic/optimize.py
--rw-r--r--   0        0        0    13231 2023-09-27 05:32:32.126607 pakettic-1.3.1/pakettic/parser.py
--rw-r--r--   0        0        0    14125 2024-01-08 12:55:32.508220 pakettic-1.3.1/pakettic/printer.py
--rw-r--r--   0        0        0    11248 2023-09-27 05:25:47.527218 pakettic-1.3.1/pakettic/ticfile.py
--rw-r--r--   0        0        0      858 2024-01-09 08:20:58.918028 pakettic-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     9526 2023-09-29 07:11:58.242476 pakettic-1.3.1/README.md
--rw-r--r--   0        0        0    10403 1970-01-01 00:00:00.000000 pakettic-1.3.1/setup.py
--rw-r--r--   0        0        0    10170 1970-01-01 00:00:00.000000 pakettic-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-02-13 17:06:22.498880 pakettic-1.4.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-02-13 17:06:22.519816 pakettic-1.4.0/pakettic/__init__.py
+-rw-r--r--   0        0        0       42 2023-02-13 17:06:22.520811 pakettic-1.4.0/pakettic/__main__.py
+-rw-r--r--   0        0        0     7096 2023-08-20 12:48:35.551820 pakettic-1.4.0/pakettic/ast.py
+-rw-r--r--   0        0        0    15907 2024-05-03 09:34:27.137039 pakettic-1.4.0/pakettic/main.py
+-rw-r--r--   0        0        0    28781 2024-05-05 13:17:01.949757 pakettic-1.4.0/pakettic/optimize.py
+-rw-r--r--   0        0        0    13244 2024-04-19 20:47:47.298029 pakettic-1.4.0/pakettic/parser.py
+-rw-r--r--   0        0        0    14125 2024-04-03 16:56:30.536178 pakettic-1.4.0/pakettic/printer.py
+-rw-r--r--   0        0        0    16566 2024-05-03 08:46:21.932870 pakettic-1.4.0/pakettic/ticfile.py
+-rw-r--r--   0        0        0      858 2024-05-05 13:51:44.932438 pakettic-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    10105 2024-05-05 13:48:41.488926 pakettic-1.4.0/README.md
+-rw-r--r--   0        0        0    10982 1970-01-01 00:00:00.000000 pakettic-1.4.0/setup.py
+-rw-r--r--   0        0        0    10744 1970-01-01 00:00:00.000000 pakettic-1.4.0/PKG-INFO
```

### Comparing `pakettic-1.3.1/LICENSE` & `pakettic-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pakettic-1.3.1/pakettic/ast.py` & `pakettic-1.4.0/pakettic/ast.py`

 * *Files identical despite different names*

### Comparing `pakettic-1.3.1/pakettic/main.py` & `pakettic-1.4.0/pakettic/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 from cmath import inf
 import argparse
+import io
+import pickle
+import struct
+from typing import Callable
 from pakettic import ast
 from glob import glob
 import os
 import sys
 import zlib
 import pkg_resources
 import zopfli
@@ -50,35 +54,43 @@
         if level < 0 or level > 5:
             raise argparse.ArgumentTypeError()
         return _ZOPFLI_LEVELS[level]
     except:
         raise argparse.ArgumentTypeError("Compression level should be an integer 0-5")
 
 
-def _compress(bytes, split, split_max, iterations):
-    """Compress a byte string using Zopfli, dropping the check sum"""
-    c = zopfli.ZopfliCompressor(zopfli.ZOPFLI_FORMAT_ZLIB, block_splitting=split,
-                                block_splitting_max=split_max, iterations=iterations)
-    return (c.compress(bytes) + c.flush())[: -4]
+def _check_positive(value):
+    ivalue = int(value)
+    if ivalue <= 0:
+        raise argparse.ArgumentTypeError("%s is an invalid positive int value" % value)
+    return ivalue
 
 
 def main():
+    global args
     """Main entrypoint for the command line program"""
     sys.setrecursionlimit(100000)  # TODO: find out why the parser recurses so heavily and reduce that
 
     version = pkg_resources.get_distribution('pakettic').version
     argparser = argparse.ArgumentParser(
         prog='pakettic', description=f'Minify and compress TIC-80 fantasy console carts. v{version}',
         formatter_class=lambda prog: argparse.HelpFormatter(prog, max_help_position=33))
     argparser.add_argument('input', nargs='+', help='input file(s). ?, * and ** wildcards work')
     argparser.add_argument('-o', '--output', default=os.getcwd(), metavar='str', help='output file or directory')
     argparser.add_argument('-l', '--lua', action='store_const', const=True,
-                           help='output .lua carts instead of .tic carts')
+                           help='DEPRECATED: same as -f lua')
     argparser.add_argument('-u', '--uncompressed', action='store_const', const=True,
-                           help='leave code chunks uncompressed, even when outputting a .tic file')
+                           help='DEPRECATED: same as -f unc')
+    argparser.add_argument('-f', '--output-format',
+                           action='store',
+                           type=str.lower,
+                           metavar='str',
+                           help="output-format, tic (.tic cart with code compressed as CODE_ZIP), unc (.tic cart with uncompressed code), png (.tic cart that looks like PNG, can compress data sections too), lua (.lua text cart). Default: based on output file name or tic.",
+                           required=False,
+                           choices=["tic", "unc", "lua", "png"])
     argparser.add_argument('-p', '--print-best', action='store_const', const=True,
                            help='pretty-print the best solution when found')
     argparser.add_argument('-c', '--chunks',
                            default='code,default', metavar='str', help='chunk types to include and their order. valid: ALL, ALL_EXCEPT_DEFAULT, or comma-separated list without spaces: BINARY,CODE,COVER_DEP,DEFAULT,FLAGS,MAP,MUSIC,PALETTE,PATTERNS_DEP,PATTERNS,SAMPLES,SCREEN,SPRITES,TILES,WAVEFORM. default: %(default)s',
                            type=_parse_chunks_arg)
     argparser.add_argument('-d', '--data-to-code', action='store_const', const=True, default=False, help='convert data chunks into code, so they can be compressed')
     argparser.add_argument('--pedantic', action='store_const', const=True, default=False,
@@ -91,15 +103,19 @@
                           type=str.lower,
                           metavar='str',
                           help="optimization algorithm, LAHC (late acceptance hill climbing), DLAS (diversified late acceptance search) or ANNEAL (simulated annealing). Default: %(default)s",
                           required=False,
                           choices=["lahc", "dlas", "anneal"],
                           default="dlas")
     optgroup.add_argument('-s', '--steps', type=int, default=10000, metavar='int',
-                          help='number of steps in the optimization algorithm. default: %(default)d')
+                          help='number of steps in the optimization algorithm. 0 = iterate forever (intermediate results saved). default: %(default)d')
+    optgroup.add_argument('-q', '--queue-length', type=_check_positive, default=12, metavar='int',
+                          help='number of parallel jobs in queue. to use all CPUs, this should be >= number of logical processors. too long queue slows down convergence. default: %(default)d')
+    optgroup.add_argument('-P', '--processes', type=_check_positive, default=None, metavar='int',
+                          help='number of parallel processes. 1 = no parallel processing. defaults to number of available logical processors.')
     optgroup.add_argument('-H', '--lahc-history', type=int, default=500, metavar='int',
                           help='history length in late acceptance hill climbing. default: %(default)d')
     optgroup.add_argument('-D', '--dlas-history', type=int, default=5, metavar='int',
                           help='history length in diversified late acceptance search. default: %(default)d')
     optgroup.add_argument('-m', '--margin', type=float, default=0, metavar='float',
                           help='initialize the lahc/dlas history with initial_cost + margin (in bytes). Default: %(default).0f')
     optgroup.add_argument('-t', '--start-temp', type=float, default=1, metavar='float',
@@ -119,23 +135,38 @@
                              help='number of iterations in zopfli. default: based on compression level')
     zopfligroup.add_argument('--split', action=argparse.BooleanOptionalAction,
                              help='enable or disable block splitting in zopfli. default: based on compression level')
     zopfligroup.add_argument('--split-max', type=int, metavar='int',
                              help='maximum number of block splittings in zopfli (0: infinite). default: based on compression level')
     args = argparser.parse_args()
 
-    if args.lua:
-        args.uncompressed = True  # Outputting LUA and compressing are mutually exclusive
     if args.split is None:
         args.split = args.zopfli_level["split"]
     if args.split_max is None:
         args.split_max = args.zopfli_level["split_max"]
     if args.iterations is None:
         args.iterations = args.zopfli_level["iterations"]
 
+    # these are deprecated, can be removed when we bump the version
+    if args.lua:
+        args.output_format = "lua"
+    if args.uncompressed:
+        args.output_format = "unc"
+
+    # if we still don't have output_format, try to guess it based on the output file extension
+    if args.output_format is None:
+        if not os.path.isdir(args.output):
+            ext = os.path.splitext(args.output)[1].lower()
+            if ext == '.lua':
+                args.output_format = "lua"
+            else:
+                args.output_format = "tic"
+        else:
+            args.output_format = "tic"
+
     input = []
     # use glob to find files matching wildcards
     # if a string does not contain a wildcard, glob will return it as is.
     for arg in args.input:
         input += glob(arg, recursive=True)
     if len(input) > 1 and not os.path.isdir(args.output):
         sys.exit('When multiple input files are defined, the output must be a directory.')
@@ -145,81 +176,133 @@
     filepbar = tqdm.tqdm(input, leave=False, smoothing=0.02)
     error = False
     total_original_size = 0
     total_minified_size = 0
     total_optimized_size = 0
     total_start_time = time.time()
     maxpathlen = max(len(p) for p in input)
-    for filepath in filepbar:
+    for input_filepath in filepbar:
         cart_start_time = time.time()
-        _, filename = os.path.split(os.path.splitext(filepath)[0])
-        ext = '.lua' if args.lua else '.tic'
-        outfile = os.path.join(args.output, filename + '.packed' + ext) if os.path.isdir(args.output) else args.output
-        original_size = os.path.getsize(filepath)
-        filepath_sliced = filepath[-30:] if len(filepath) > 30 else filepath
-        filepbar.set_description(f"Reading       {filepath_sliced}")
+        _, filename = os.path.split(os.path.splitext(input_filepath)[0])
+        if os.path.isdir(args.output):
+            if args.output_format == 'lua':
+                ext = '.lua'
+            else:
+                ext = '.tic'
+            output_filepath = os.path.join(
+                args.output, filename + '.packed' + ext)
+        else:
+            output_filepath = args.output
+        original_size = os.path.getsize(input_filepath)
         try:
-            cart = ticfile.join_code(ticfile.read(filepath))
-        except Exception as e:
-            filepbar.write(f"Error reading {filepath}: {e}, skipping...")
+            minified_size, optimized_size = _process_file(input_filepath, output_filepath, filepbar)
+        except KeyboardInterrupt:
             error = True
-            continue
-        filepbar.set_description(f"Decompressing {filepath_sliced}")
-        cart.update([((k[0], ticfile.ChunkID.CODE), zlib.decompress(v[2:], -15))
-                    for k, v in cart.items() if k[1] == ticfile.ChunkID.CODE_ZIP])  # decompress zipped chunks
-        cart[(0, ticfile.ChunkID.DEFAULT)] = b''  # add default chunk if it's missing
-        cart = dict(c for i in args.chunks for c in cart.items() if c[0][1] == i)  # only include the chunks listed in args
-        if args.data_to_code:
-            ticfile.data_to_code(cart)
-        filepbar.set_description(f"Compressing   {filepath_sliced}")
-        outcart = cart.copy() if args.uncompressed else dict((k, v) if k[1] != ticfile.ChunkID.CODE else (
-            (k[0], ticfile.ChunkID.CODE_ZIP), _compress(v, args.split, args.split_max, args.iterations)) for k, v in cart.items())
-        final_size = ticfile.write(ticfile.split_code(outcart), outfile)
-        code_chunks = [c for c in cart if c[1] == ticfile.ChunkID.CODE]
-        for c in code_chunks:
-            code = cart[c].decode("ascii")
-            root = parser.parse_string(code)
-            root = optimize.loads_to_funcs(root)
-            root = optimize.minify(root)
-            root = ast.Hint(root)
-
-            def _cost_func(root, best_cost):
-                nonlocal final_size
-                bytes = printer.format(root, no_load=args.no_load).encode("ascii")
-                key = c
-                if not args.uncompressed:
-                    key = (c[0], ticfile.ChunkID.CODE_ZIP)
-                    bytes = _compress(bytes, args.split, args.split_max, args.iterations)
-                diff = len(bytes) - len(outcart[key])
-                ret = final_size + diff - args.target_size
-                if args.exact:
-                    ret = abs(ret)
-                if ret < best_cost:
-                    outcart[key] = bytes
-                    final_size = ticfile.write(ticfile.split_code(outcart), outfile, pedantic=args.pedantic)
-                    if args.print_best:
-                        filepbar.write(f"-- {ret} bytes:\n{'-'*40}\n{printer.format(root, pretty=True).strip()}\n{'-'*40}")
-                return ret
-            _cost_func(root, inf)
-            minified_size = final_size  # current final_size is the size after minification
-            if args.algorithm == 'lahc':
-                root = optimize.lahc(root, steps=args.steps, cost_func=_cost_func,
-                                     list_length=args.lahc_history, init_margin=args.margin, seed=args.seed)
-            elif args.algorithm == 'dlas':
-                root = optimize.dlas(root, steps=args.steps, cost_func=_cost_func,
-                                     list_length=args.dlas_history, init_margin=args.margin, seed=args.seed)
-            else:
-                root = optimize.anneal(root, steps=args.steps, cost_func=_cost_func,
-                                       start_temp=args.start_temp, end_temp=args.end_temp, seed=args.seed)
+            filepbar.write(f"Interrupt processing {input_filepath}")
+            break
         total_original_size += original_size
-        total_optimized_size += final_size
+        total_optimized_size += optimized_size
         total_minified_size += minified_size
         cart_time_str = '.'.join(str(datetime.timedelta(seconds=int(time.time() - cart_start_time))).split(':'))
-        filepbar.write(f"{filepath.ljust(maxpathlen)} Time:{cart_time_str} Orig:{original_size:<5} Min:{minified_size:<5} Pack:{final_size:<5}")
+        filepbar.write(f"{input_filepath.ljust(maxpathlen)} Time:{cart_time_str} Orig:{original_size:<5} Min:{minified_size:<5} Pack:{optimized_size:<5}")
     if len(input) > 1:
         total_time_str = str(datetime.timedelta(seconds=int(time.time() - total_start_time)))
         print("-" * 80 + f"\n{'Totals'.ljust(maxpathlen)} Time:{total_time_str} Orig:{total_original_size:<5} Min:{total_minified_size:<5} Pack:{total_optimized_size:<5}")
     sys.exit(1 if error else 0)
 
 
+def _process_file(input_path, output_filepath, pbar) -> tuple[int, int]:
+    # These are global for performance reasons. When multiprocessing, globals
+    # are not copied to child processes, so we pass them as arguments to the
+    # process initialize (_initializer) function, which set the globals for that
+    # process
+    global args, writer
+
+    input_sliced = input_path[-30:] if len(input_path) > 30 else input_path
+    pbar.set_description(f"Processing    {input_sliced}")
+    cart = ticfile.read(input_path)
+    def_chunk = (0, ticfile.ChunkID.DEFAULT, b'')
+    if def_chunk not in cart.data:  # add default chunk if it's missing
+        cart.data.append(def_chunk)
+    cart.data = [(bank, id, bytes)
+                 for bank, id, bytes in cart.data if id in args.chunks]
+    if args.data_to_code:
+        cart = ticfile.data_to_code(cart)
+
+    pbar.set_description(f"Compressing   {input_sliced}")
+    root = parser.parse_string(cart.code.decode('latin-1'))
+    root = optimize.loads_to_funcs(root)
+    root = optimize.minify(root)
+    root = ast.Hint(root)
+    # writer caches as much as possible of the data writing so that we don't have to recompute data parts for each optimization step
+    writer = _make_writer(cart.data)
+    minified_size, finisher = writer(_format(root))
+    with open(output_filepath, 'wb') as output_file:
+        final_size = finisher(output_file)
+    assert final_size == minified_size
+
+    def _best_func(state, cf):
+        nonlocal final_size
+        cand_size, finisher = cf
+        with open(output_filepath, 'wb') as output_file:
+            final_size = finisher(output_file)
+        assert final_size == cand_size
+        if args.print_best:
+            pbar.write(f"-- {final_size} bytes:\n{'-'*40}\n{printer.format(pickle.loads(state)[0], pretty=True).strip()}\n{'-'*40}")
+
+    # only PNG carts cab benefit from data chunk order shuffling
+    data = cart.data if args.output_format == 'png' else None
+
+    with optimize.Solutions((root, data), args.seed, args.queue_length, args.processes, _cost_func, _best_func, _initializer, (args, writer)) as solutions:
+        if args.algorithm == 'lahc':
+            optimize.lahc(solutions, steps=args.steps, list_length=args.lahc_history, init_margin=args.margin)
+        elif args.algorithm == 'dlas':
+            optimize.dlas(solutions, steps=args.steps, list_length=args.dlas_history, init_margin=args.margin)
+        else:
+            optimize.anneal(solutions, steps=args.steps, start_temp=args.start_temp, end_temp=args.end_temp, seed=args.seed)
+    return minified_size, final_size
+
+
+def _compress(bytes=None):
+    global args
+    c = zopfli.ZopfliCompressor(zopfli.ZOPFLI_FORMAT_ZLIB, block_splitting=args.split,
+                                block_splitting_max=args.split_max, iterations=args.iterations)
+    return (c.compress(bytes) + c.flush())
+
+
+def _format(root: ast.Node) -> bytes:
+    global args
+    return printer.format(root, no_load=args.no_load).encode('latin-1')
+
+
+def _make_writer(data) -> ticfile.Writer:
+    global args
+    if args.output_format == 'lua':
+        return ticfile.write_lua(data)
+    elif args.output_format == 'png':
+        return ticfile.write_png(data, args.pedantic, _compress)
+    elif args.output_format == 'unc':
+        return ticfile.write_tic(data, args.pedantic, None)
+    else:
+        return ticfile.write_tic(data, args.pedantic, _compress)
+
+
+def _initializer(a):
+    global args, writer
+    args, writer = a
+
+
+def _cost_func(root_data):
+    global args, writer
+    root, data = root_data
+    if data is not None:  # PNG carts shuffle the data chunks so we cannot cache the data parts & have to regenerate writer for each step
+        cand_size, finisher = _make_writer(data)(_format(root))
+    else:
+        cand_size, finisher = writer(_format(root))
+    cand_cost = cand_size - args.target_size
+    if args.exact:
+        cand_cost = abs(cand_cost)
+    return cand_cost, (cand_size, finisher)
+
+
 if __name__ == '__main__':
     main()
```

### Comparing `pakettic-1.3.1/pakettic/optimize.py` & `pakettic-1.4.0/pakettic/optimize.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-from cmath import inf
-from functools import singledispatch
+from collections import deque
+from functools import singledispatch, wraps
 import inspect
 import itertools
 import math
 import pickle
+import signal
 import random
-from typing import Any, Callable, Optional, Union, get_args, get_origin, get_type_hints
+from typing import Any, Callable, Optional, Tuple, get_args, get_origin, get_type_hints
 import tqdm
 from pakettic import ast, parser
-from dataclasses import replace
+from dataclasses import dataclass, replace
+from multiprocessing import Pool
 
 
 def _toBase26(num):
     s = ""
     while (num > 0):
         s += (chr(ord('z') - (num - 1) % 26))
         num -= 1
         num //= 26
     return s
 
 
-_MINIFIED_NAMES = (name for i in itertools.count(start=1, step=1) if (name := _toBase26(i)) not in _RESERVED and name not in parser.keywords)
 _FLIPPABLE_OPS = [">", "<", ">=", "<=", "~=", "=="]
 _FLIPPED_OPS = ["<", ">", "<=", ">=", "~=", "=="]
 _REORDERABLE_OPS = ["+", "-", "*", "/", "&", "|", "~"]
 _REORDERABLE_RIGHT = [["+", "-"], ["+", "-"], ["*", "/"], ["*", "/"], ["&"], ["|"], ["~"]]
 _REORDERABLE_LEFT = [True, False, True, False, True, True, True]
 _EVALUABLE_OPS = {
     "+": lambda l, r: l + r,
@@ -72,23 +73,23 @@
     return apply_trans(root, _trans)
 
 
 def minify(root: ast.Node) -> ast.Node:
     """
     Perform initial minification of the variable names
         Parameters:
-            root (ast.Node): Root of the abstract syntax tree            
+            root (ast.Node): Root of the abstract syntax tree
         Returns:
             new_root (ast.Node): Root of the new, mutated abstract syntax tree
     """
     new_root = pickle.loads(pickle.dumps(root))  # pickling/unpickling is faster than deepcopy
     changed_names = dict()
     changed_labels = dict()
-    name_iter = iter(_MINIFIED_NAMES)
-    label_iter = iter(_MINIFIED_NAMES)
+    name_iter = iter((name for i in itertools.count(start=1, step=1) if (name := _toBase26(i)) not in _RESERVED and name not in parser.keywords))
+    label_iter = iter((name for i in itertools.count(start=1, step=1) if (name := _toBase26(i)) not in _RESERVED and name not in parser.keywords))
 
     def _tryget(d: dict, key: str, it):
         if key in _RESERVED:
             return key
         new = d.get(key, None)
         if new is None:
             new = next(it)
@@ -103,27 +104,27 @@
         elif type(node) == ast.Goto:
             node.target = _tryget(changed_labels, node.target, label_iter)
 
     visit(new_root, _minify)
     return new_root
 
 
-def mutate(root: ast.Node, rand: random.Random) -> ast.Node:
+def mutate(root_order: tuple[ast.Node, list], rand: random.Random):
     """
-    Mutates an abstract syntax tree by making small modification to it,
-    e.g. flipping binary operators or changing variable names
+    Mutates an abstract syntax tree by making small modification to it, e.g.
+    flipping binary operators or changing variable names
         Parameters:
-            root (ast.Node): Root of the abstract syntax tree
+            root_order (tuple[ast.Node,list]): First item is the root of the
+                abstract syntax tree, second item the chunk order in cart (can be
+                nil if chunk shuffling not wanted). These will get modified, so deep
+                copy them before calling this function if needed.
             rand (random.Random): Random number generator to use
-        Returns:
-            new_root (ast.Node): Root of the new, mutated abstract syntax tree
     """
-    new_root = pickle.loads(pickle.dumps(root))  # pickling/unpickling is faster than deepcopy
+    root, order = root_order
     mutations = []
-
     used_names = set()
     used_labels = set()
 
     def _check_mutations(node: ast.Node, parent: ast.Node, attr: str):
         if type(node) == ast.BinOp:
             try:
                 i = _FLIPPABLE_OPS.index(node.op)
@@ -202,26 +203,26 @@
                 node.no_hex = not node.no_hex
             mutations.append(_mutation2)
 
         if node.original != None and parent != None:
             def _mutation():
                 replace_node(parent, attr, node.original, None)
 
-    visit(new_root, _check_mutations)
+    visit(root, _check_mutations)
     used_names = sorted(used_names.difference(_RESERVED))
 
     def var_repl(id_a, id_b):
         def _mut():
             def _repl(node, parent, attr):
                 if type(node) == ast.Name:
                     if node.id == id_a:
                         node.id = id_b
                     elif node.id == id_b:
                         node.id = id_a
-            visit(new_root, _repl)
+            visit(root, _repl)
         return _mut
     # if both a and b are in used_names, we have both copies of a,b and b,a in the list
     # but that's probably ok: swapping variables head to head is usually better idea
     # that swapping variables with new ones
     mutations.extend((var_repl(a, b) for a in used_names for b in _LOWERS if a != b))
 
     def label_repl(name_a, name_b):
@@ -233,22 +234,31 @@
                     elif node.name == name_b:
                         node.name = name_a
                 if type(node) == ast.Goto:
                     if node.target == name_a:
                         node.target = name_b
                     elif node.target == name_b:
                         node.target = name_a
-            visit(new_root, _repl)
+            visit(root, _repl)
         return _mut
     used_labels = sorted(used_labels)
-    mutations.extend((label_repl(a, b) for a in used_labels for b in _LOWERS if a != b))
+    mutations.extend((label_repl(a, b)
+                     for a in used_labels for b in _LOWERS if a != b))
+
+    if order is not None and len(order) > 0:
+        def chunk_swap(i, j: int):
+            def _mut():
+                order[i], order[j] = order[j], order[i]
+            return _mut
+        mutations.extend(chunk_swap(i, j) for i, _ in enumerate(
+            order) for j, _ in enumerate(order) if j > i)
+
     if len(mutations) > 0:
         mutation = rand.choice(mutations)
         mutation()
-    return new_root
 
 
 def replace_node(parent: ast.Node, attr: str, node: ast.Node, old: ast.Node):
     """
     Replaces one node in the abstract syntax tree with another.
     Adds a reference to the old node from the new node's 'original' attribute.
         Parameters:
@@ -261,114 +271,170 @@
     if "." in attr:
         a, i = attr.split(".")
         getattr(parent, a)[int(i)] = node
     else:
         setattr(parent, attr, node)
 
 
-def anneal(state: Any, cost_func: Callable[[Any, int], int], steps: int, start_temp: float, end_temp: float, seed: int, mutate_func: Callable[[Any], Any] = mutate) -> Any:
+class Solutions:
+    processes: int
+    queue: deque
+    mutate_func: Callable[[Any], Any]
+    cost_func: Callable[[Any, int], Tuple[int, Any]]
+    init_state: Any
+    queue_length: int
+
+    def __init__(self, state, seed: int, queue_length: int, processes: int, cost_func: Callable[[Any, int], Tuple[int, Any]],  best_func, init=None, initargs=()):
+        self.processes = processes
+        if processes != 1:
+            self.pool = Pool(processes=processes, initializer=_PoolInitializer(init), initargs=(initargs,))
+        else:
+            self.pool = None
+        self.queue = deque()
+        self.cost_func = cost_func
+        self.cost_func_pickled = pickle.dumps(self.cost_func)
+        self.queue_length = queue_length
+        self.init_state = pickle.dumps(state)
+        self.seed = seed
+        self.best_func = best_func
+
+    def __enter__(self):
+        if self.pool is not None:
+            self.pool.__enter__()
+
+        rng = random.Random(self.seed)
+        for i in range(self.queue_length):
+            if self.pool is not None:
+                self.put(self.init_state, pickle.dumps(rng), first=i == 0)
+            else:
+                self.put(self.init_state, pickle.loads(pickle.dumps(rng)), first=i == 0)
+            rng = random.Random(rng.getrandbits(32))  # shuffle the rng so that the different rngs are used
+        return self
+
+    def __exit__(self, *args):
+        if self.pool is not None:
+            self.pool.close()
+            self.pool.join()
+            self.pool.__exit__(*args)
+
+    def get(self):
+        if self.pool is not None:
+            return self.queue.popleft().get(timeout=9999)
+        else:
+            state, rng, first = self.queue.popleft()
+            return _mutate_cost(state, rng, self.cost_func, first)
+
+    def put(self, state: Any, rng: random.Random, first=False):
+        if self.pool is not None:
+            self.queue.append(self.pool.apply_async(_mutate_cost_pickled, (state, rng, self.cost_func_pickled, first)))
+        else:
+            self.queue.append((state, rng, first))
+
+    def best(self, state, finisher):
+        self.best_func(state, finisher)
+
+
+def anneal(solutions: Solutions, steps: int, start_temp: float, end_temp: float, seed: int = 0) -> Any:
     """
     Perform simulated annealing optimization, using exponential temperature schedule.
     See https://en.wikipedia.org/wiki/Simulated_annealing
         Parameters:
-            state: Starting state for the optimization
-            cost_func (Callable[[Any, int], int]): Callback function, with the first parameter the state and second parameter the cost of best solution so far
+            solutions (Solutions): the Solutions object with a pool of solutions, cost function and best function
             steps (int): how many steps the optimization algorithms takes
             start_temp (float): starting temperature for the optimization
             end_temp (float): end temperature for the optimization
-            mutate_func (Callable[[Any], Any]): Callback function state -> state that performs a small mutation in the code
+            seed (int): seed for the random number generator
         Returns:
             best (Any): The best solution found
     """
-    current_cost = cost_func(state, inf)
+    state, current_cost, rng, finalize = solutions.get()
+    solutions.best(state, finalize)
     best_cost = current_cost
     best = state
     r = random.Random(seed)  # deterministic seed, to have deterministic results
-    bar = tqdm.tqdm(range(steps), position=1, leave=False)
+    bar = tqdm.tqdm(_stepsGenerator(steps), position=1, leave=False)
     for i in bar:
+        solutions.put(state, rng)
         alpha = i / (steps - 1)
         temp = math.exp((1 - alpha) * math.log(start_temp) + alpha * math.log(end_temp))
-        candidate = mutate_func(state, r)
-        cand_cost = cost_func(candidate, best_cost)
+        candidate, cand_cost, rng, finalize = solutions.get()
         if cand_cost < current_cost or math.exp(-(cand_cost - current_cost) / temp) >= r.random():
             current_cost = cand_cost
             state = candidate
         if cand_cost < best_cost:
             best_cost = cand_cost
             best = candidate
+            solutions.best(best, finalize)
         bar.set_description(f"B:{best_cost} C:{current_cost} A:{cand_cost} T: {temp:.1f}")
         if best_cost <= 0:
             break
     return best
 
 
-def lahc(state: Any, cost_func: Callable[[Any, int], int], steps: int, list_length: int, init_margin: int, seed: int, mutate_func: Callable[[Any], Any] = mutate) -> Any:
+def lahc(solutions: Solutions, steps: int, list_length: int, init_margin: int) -> Any:
     """
     Optimize a function using Late Acceptance Hill Climbing
     See https://arxiv.org/pdf/1806.09328.pdf
         Parameters:
-            state: Starting state for the optimization
-            cost_func (Callable[[Any, int], int]): Callback function, with the first parameter the state and second parameter the cost of best solution so far
+            solutions (Solutions): the Solutions object with a pool of solutions, cost function and best function
             steps (int): how many steps the optimization algorithms takes
             list_length (int): length of the history in the algorithm
             init_margin (int): how much margin, in bytes, to add to the initial best cost
-            mutate_func (Callable[[Any], Any]): Callback function state -> state that performs a small mutation in the code
         Returns:
             best (Any): The best solution found
     """
-    current_cost = cost_func(state, inf)
+    state, current_cost, rng, finalize = solutions.get()
+    solutions.best(state, finalize)
     best_cost = current_cost
     history = [best_cost + init_margin] * list_length
     best = state
-    r = random.Random(seed)  # deterministic seed, to have deterministic results
-    bar = tqdm.tqdm(range(steps), position=1, leave=False)
+    bar = tqdm.tqdm(_stepsGenerator(steps), position=1, leave=False)
     for i in bar:
-        candidate = mutate_func(state, r)
-        cand_cost = cost_func(candidate, best_cost)
+        solutions.put(state, rng)
+        candidate, cand_cost, rng, finalize = solutions.get()
         v = i % list_length
         if cand_cost < history[v] or cand_cost <= current_cost:
             current_cost = cand_cost
             state = candidate
         if current_cost < history[v]:
             history[v] = current_cost
         if cand_cost < best_cost:
             best_cost = cand_cost
             best = candidate
+            solutions.best(best, finalize)
         bar.set_description(f"B:{best_cost} C:{current_cost} A:{cand_cost}")
         if best_cost <= 0:
             break
     return best
 
 
-def dlas(state: Any, cost_func: Callable[[Any, int], int], steps: int, list_length: int, init_margin: int, seed: int, mutate_func: Callable[[Any], Any] = mutate) -> Any:
+def dlas(solutions: Solutions, steps: int, list_length: int, init_margin: int) -> Any:
     """
     Optimize a function using Diversified Late Acceptance Search
     See https://arxiv.org/pdf/1806.09328.pdf
         Parameters:
-            state: Starting state for the optimization
-            cost_func (Callable[[Any, int], int]): Callback function, with the first parameter the state and second parameter the cost of best solution so far
+            solutions (Solutions): the Solutions object with a pool of solutions, cost function and best function
             steps (int): how many steps the optimization algorithms takes
             list_length (int): length of the history in the algorithm
             init_margin (int): how much margin, in bytes, to add to the initial best cost
-            mutate_func (Callable[[Any], Any]): Callback function state -> state that performs a small mutation in the code
         Returns:
             best (Any): The best solution found
     """
-    current_cost = cost_func(state, inf)
+    state, current_cost, rng, finalize = solutions.get()
+    solutions.best(state, finalize)
     best_cost = current_cost
     cost_max = best_cost + init_margin
     history = [cost_max] * list_length
     N = list_length
     best = state
-    r = random.Random(seed)  # deterministic seed, to have deterministic results
-    bar = tqdm.tqdm(range(steps), position=1, leave=False)
+    bar = tqdm.tqdm(_stepsGenerator(steps), position=1, leave=False)
     for i in bar:
+        solutions.put(state, rng)
         prev_cost = current_cost
-        candidate = mutate_func(state, r)
-        cand_cost = cost_func(candidate, best_cost)
+        candidate, cand_cost, rng, finalize = solutions.get()
         v = i % list_length
         if cand_cost == current_cost or cand_cost < cost_max:
             current_cost = cand_cost
             state = candidate
         if current_cost > history[v]:
             history[v] = current_cost
         elif current_cost < history[v] and current_cost < prev_cost:
@@ -377,20 +443,72 @@
             history[v] = current_cost
             if N <= 0:
                 cost_max = max(history)
                 N = history.count(cost_max)
         if cand_cost < best_cost:
             best_cost = cand_cost
             best = candidate
+            solutions.best(best, finalize)
         bar.set_description(f"B:{best_cost} C:{current_cost} M:{cost_max} A:{cand_cost}")
         if best_cost <= 0:
             break
     return best
 
 
+@dataclass
+class _PoolInitializer:
+    """
+    This class was just a simple lambda function, but it is not possible to pickle lambda functions with default pickling
+    """
+    init: Callable[[Any], None]
+
+    def __call__(self, a):
+        # ignore SIGINT in the pool processes; rather, let the main process handle it and close the pool when it happens
+        signal.signal(signal.SIGINT, signal.SIG_IGN)
+        if self.init is not None:
+            self.init(a)
+
+
+def _mutate_cost(state, rng: random.Random, cost_func, first):
+    """
+    Helper function that mutates a state and calculates the cost. Used when not
+    doing multiprocessing. Avoids unnecessary pickling/unpickling of the rng and
+    the cost_func.
+    """
+    state = pickle.loads(state)
+    if not first:
+        mutate(state, rng)
+    new_cost, finisher = cost_func(state)
+    return pickle.dumps(state), new_cost, rng, finisher
+
+
+def _mutate_cost_pickled(state, rng, cost_func, first):
+    """
+    Helper function that mutates a state and calculates the cost. Used when
+    multiprocessing. Pickles/unpickles also the rng and cost_func as these need
+    to go back and forth between the main process and the pool processes.
+    """
+    rng = pickle.loads(rng)
+    state = pickle.loads(state)
+    if not first:
+        mutate(state, rng)
+    new_cost, finisher = pickle.loads(cost_func)(state)
+    return pickle.dumps(state), new_cost, pickle.dumps(rng), finisher
+
+
+def _stepsGenerator(steps: int):
+    """
+    Generator for the steps of the optimization algorithms, taking into account that 0 means infinite steps
+    """
+    if steps == 0:
+        return itertools.count()
+    else:
+        return range(steps)
+
+
 def apply_trans(node: ast.Node, trans: Callable[[ast.Node], ast.Node]) -> ast.Node:
     """
     Applies a transformation to an abstract syntax tree recursively
         Parameters:
             node (ast.Node): Root of the syntax tree to transform
             trans (Callable[[ast.Node], ast.Node]): Callback function that takes a node and returns a transformed node
         Returns:
```

### Comparing `pakettic-1.3.1/pakettic/parser.py` & `pakettic-1.4.0/pakettic/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 # The power operator is weird: it binds more strongly than unary to the
 # thing on its left, but less strongly than unary to its right. So, we
 # need to treat it separately
 expliteral = nil | false | true | Numeral | LiteralString | ellipsis | functiondef | prefixexp | tableconstructor | LPAR + exp + RPAR
 altexp = expliteral + (pp.Literal('--|').suppress() - expliteral)[0, ...]
 altexp.set_parse_action(alt)
 powerexp = pp.Forward()
-unaryexp = pp.Regex(r"not|#|-(?!-)|~")[0, ...] + powerexp
+unaryexp = pp.Regex(r"not(?![a-zA-Z_])|#|-(?!-)|~")[0, ...] + powerexp
 unaryexp.set_parse_action(unaryAction)
 powerexp <<= altexp + (pp.Literal('^').suppress() - unaryexp)[0, 1]
 powerexp.set_parse_action(lambda t: ast.BinOp(left=t[0], op="^", right=t[1]) if len(t) > 1 else t[0])
 exp <<= pp.infixNotation(
     unaryexp,
     [
         (pp.oneOf('* / // %'), 2, pp.OpAssoc.LEFT, left_assoc),
```

### Comparing `pakettic-1.3.1/pakettic/printer.py` & `pakettic-1.4.0/pakettic/printer.py`

 * *Files identical despite different names*

### Comparing `pakettic-1.3.1/pyproject.toml` & `pakettic-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pakettic"
-version = "1.3.1"
+version = "1.4.0"
 description = "A tool for minifying and compressing TIC-80 fantasy console carts"
 authors = ["Veikko Sariola <5684185+vsariola@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/vsariola/pakettic"
 keywords = ["TIC-80", "Fantasy Console", "Compression", "LUA"]
 classifiers = [
```

### Comparing `pakettic-1.3.1/README.md` & `pakettic-1.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -177,53 +177,58 @@
 
 Pakettic treats `--![` and `--!]` as multiline comment tags, while LUA
 treats these as single line comments. Useful for including debug code in
 the unpacked intro: the code will not be included in the packed cart.
 
 ## Tips for command line arguments
 
-- If pakettic complains about CODE_ZIP chunk size, the code is just too
-  big after compression. In TIC-80, CODE_ZIP chunks do not support
-  multiple banks (and likely never will, as the feature is already
-  deprecated), and thus are unfortunately limited to 65535 bytes.
-  `--uncompressed` is a temporary fix, but code will be uncompressed and
-  thus the size much larger.
+- If you have a CPU with many logical processors and want to max out your CPU
+  usage, you can increase the processing queue length with `-q`. You should
+  usually use `-q N` where N is the number of logical processors. Too high queue
+  length hurts the convergence rate. Defaults to 12.
 - The Zopfli compression level can be set with `-z<level>`, with level
   ranging from 0 to 5. When developing, start with `-z0` for fast
   optimization, and only increase when necessary e.g. when you are just
   a few bytes over the limit. The default Zopfli-level is 0.
 - The algorithm uses a pseudorandom generator. Sometimes using a
   different seed finds a few byte better or worse solution. Use command
   line argument `--seed` to try different seeds.
 - Similarly, different optimization heuristics produce slightly
   different results. Try different heuristics e.g. with `-alahc`,
   `-adlas` or `-aanneal`.
-- To avoid re-optimizing all the expressions every time, do a long
-  optimization run, study the results and change your expressions to the
-  forms that pack well. Set the number of steps with `-s`. Use
-  command-line argument `-p` to always print a reasonably readable
-  version of the best solution when one is found.
+- To avoid re-optimizing all the expressions every time, do a long optimization
+  run, study the results and change your expressions to the forms that pack
+  well. Set the number of steps with `-s`; `-s0` iterates forever. Intermediate
+  results are saved. Use command-line argument `-p` to always print a reasonably
+  readable version of the best solution when one is found.
 - By default, pakettic only includes CODE and DEFAULT chunks. DEFAULT
   indicates that before loading the cart, TIC-80 loads the default cart,
   setting default palette, waveforms etc. If you don't need the default
   values (e.g. you set the palette yourself), save one byte by only
   including CODE chunk in the cart: `-ccode`
-- Working on a tweet-cart? Use `-l` to output LUA carts, which are
-  uncompressed. The optimization algorithm then just optimizes the
-  uncompressed size of the code.
+- Working on a tweet-cart? Use `-flua` to output LUA carts, which are
+  uncompressed. The optimization algorithm then just optimizes the uncompressed
+  size of the code.
 - If the packed cart is missing sprites, music, map etc., try adding
   `-call` (or something more specific) to include necessary chunks.
-- Do you want to use the TIC-80 sprites or the tracker, but don't like
-  the fact that the data chunks are uncompressed? Use `-d` to have
-  pakettic automatically convert all data chunks into hexadecimal
-  strings in the code, along with a small stub placed at the beginning
-  of the code that interprets the string and loads the data at correct
-  address. For example,
-  `-d -cCODE,MUSIC,PATTERNS,WAVEFORM,SAMPLES,DEFAULT` would include the
-  necessary chunks for the music.
+- Do you want to use the TIC-80 sprites or the tracker, but don't like the fact
+  that the data chunks are uncompressed? Is your code longer than 65536
+  characters? Use `-fpng` to output "fake" PNG-like carts, which TIC-80 detects
+  as PNGs based on their headers and loads the cart from a `caRt` chunk, which
+  contains a TIC-80 cart, but this time the entire cart is compressed. ~ 20
+  bytes of additional headers are needed to fool TIC-80, so this is not
+  recommended for very tiny intros. You need to specify which data chunks should
+  be kept. For example, `-fpng -cCODE,MUSIC,PATTERNS,WAVEFORM,SAMPLES,DEFAULT`
+  would include the necessary chunks for the music. PNG-like carts require
+  TIC-80 v1.1.2729 or newer.
+- Alternative way to use data chunks is to use `-d` to have pakettic
+  automatically convert data chunks in bank 0 into hexadecimal strings in the
+  code, along with a small stub placed at the beginning of the code that
+  interprets the string and loads the data at correct address. This breaks
+  `sync` from bank 0, so use with care in multibank carts.
 
 ## Known issues
 
 - At the moment, all the branches of swappable operators are assumed to
   be without side effects. If they have side-effects, the swapping might
   inadvertedly swap the execution order of the two branches.
 - The parser can crash with large carts. Carts in the size coding range
```

### Comparing `pakettic-1.3.1/setup.py` & `pakettic-1.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['pyparsing>=3.0.8,<4.0.0', 'tqdm>=4.64.0,<5.0.0', 'zopflipy>=1.7,<2.0']
 
 entry_points = \
 {'console_scripts': ['pakettic = pakettic.main:main']}
 
 setup_kwargs = {
     'name': 'pakettic',
-    'version': '1.3.1',
+    'version': '1.4.0',
     'description': 'A tool for minifying and compressing TIC-80 fantasy console carts',
-    'long_description': '# Pakettic\n\nPakettic is a command-line tool for minifying and compressing\n[TIC-80](http://tic80.com/) fantasy console carts. The tool is written\nin Python (3.9+) and used especially for\n[sizecoding](http://www.sizecoding.org/wiki/TIC-80). It compresses\nexisting carts approximately ~1.2% better than best alternatives, and by\nusing its [magic comments](#magic-comments), pakettic might find code\nthat compresses even better.\n\n## Installation\n\nInstalling with pip:\n\n```bash\n$ pip install pakettic\n```\n\nInstalling the latest main branch from GitHub:\n\n```bash\n$ pip install git+https://github.com/vsariola/pakettic.git@main\n```\n\nInstalling a checked out version of the repository:\n\n```bash\n$ pip install -e path/to/pakettic\n```\n\nInstalling a checked out version of the repository using\n[poetry](https://python-poetry.org/) for a nice virtual environment with\nlocked dependencies (run inside the pakettic folder):\n\n```bash\n$ poetry install\n```\n\n## Usage\n\nTo compress a cart, run:\n\n```bash\n$ pakettic path/to/cart.tic\n```\n\nIf your PATH is not configured to include pip installed executables, you\ncan use\n\n```bash\n$ python -m pakettic path/to/cart.tic\n```\n\nIf you installed using poetry into a virtual environment, you need to\nprepend `poetry run` before every command e.g.\n\n```bash\n$ poetry run pakettic path/to/cart.tic\n```\n\nPakettic supports both .tic and .lua carts. Multiple input files may be\ndefined. Input files are globbed, so `?`, `*`, and `**` work as\nwildcards for a single character, multiple characters and a directory,\nrespectively.\n\nFor a full list of command line options, see:\n\n```bash\n$ pakettic --help\n```\n\nSee also [tips for command line arguments](#tips-for-command-line-arguments)\n\nRunning all tests:\n\n```bash\n$ poetry run python -m unittest discover -s tests\n```\n\n## Features\n\nPakettic first parses the LUA-script to an abstract syntax tree, and\nthen uses a local optimization algorithm\n([simulated annealing](https://en.wikipedia.org/wiki/Simulated_annealing),\n[late acceptance hill climbing](https://arxiv.org/pdf/1806.09328.pdf) or\nits variant diversified late acceptance search) to randomly mutate the\nsyntax tree & see if it compresses better. Implemented mutations\ninclude:\n  - shortening variable names\n  - flipping comparisons `>`, `<`, `>=`, `<=`, `~=`, and `==`\n  - reordering arithmetic operators `+`, `-`, `*` and `/` and bit logic\n    operators `&`, `~` and `|`\n  - converting `a^2` into `a*a` and vice versa\n  - using either single or double quotes for all strings\n  - converting whole hexadecimals into decimals\n  - convert `for a,b,1 do` into `for a,b do` and vice versa\n  - reordering statements: statements that can be reordered are marked\n    with [magic comments](#magic-comments)\n  - alternative expressions: alternatives are marked with\n    [magic comments](#magic-comments)\n  - folding constant expressions\n\nInternally, pakettic uses [zopfli](https://github.com/google/zopfli) for\nthe compression.\n\n`load\'<code>\'` is parsed as `function(...)<code>end` so you can easily\nrecompress already compressed carts. Conversely, `function()<code>end`\nor `function(...)<code>end` is replaced with `load\'<code>\'` during\ncompression.\n\nNote that `function(...)<code>end` and `load\'<code>\'` are not 100%\nsemantically identical: the load version cannot access locals in the outer\nscope. For example: `local x="hello" function f()print(x)end` works but\n`local x="hello" f=load\'print(x)\'` does not. Since locals are rarely\nused in size-coding, we default to using the load-trick, but you can\ndisable it with the command-line parameter `--no-load`.\n\nHowever, pakettic does not convert functions with parameters. In\nparticular, pakettic does not automatically convert\n`function SCN(x)<code>end` into `SCN=load\'x=...<code>\'`, because they\nare not semantically identical: in the load version, `x` is now global\nand thus could trash a global variable, unintentionally breaking the\ncart. To make `SCN` compress nicely, you have to write it as\n`function SCN(...)x=...<code>end`, taking responsibility for `x` not\noverwriting anything important.\n\nUnnecessary parentheses are removed from expressions so you do not have\nto worry about those.\n\n## Magic comments\n\n### Reorderable statements\n\nThe algorithm will try to reorder statements between `--{` and `--}`.\nFor example:\n\n```lua\n --{\n a="hello"\n b="world"\n --}\n```\n\nwill try both `a="hello"b="world"` and `b="world"a="hello"` to see which\ncompresses better.\n\nNotice that only complete statements can be reordered. Thus, this will\nNOT work:\n\n```lua\n --{\n for x=0,239 do\n  for y=0,135 do\n --}\n  end\n end\n```\n\nA good rule of thumb is that you should be able to replace `--{` and\n`--}` with `do` and `end`, respectively, and still have valid code.\n\nStatements between `--{!` and `--}` are not ordered, so you can make\nblocks of statements that are kept in order within a pair of `--{` and\n`--}` tags.\n\n### Alternative expressions\n\nThere is a special `--|` operator that allows alternative expressions to\nbe tested, to see if they compress better. For example: `5--|4--|6`\nmeans that the algorithm will try 4 and 6 in place of the 5. This will\nnaturally show up as a comment in LUA so you will have to continue the\nexpression on next line if this is in the middle of an expression. `--|`\nhas the lowest precedence, even lower than `^`, so put parentheses if\nyou want to try more complicated expressions e.g. `(x//256)--|(x>>8)`\n\n### Debug code\n\nPakettic treats `--![` and `--!]` as multiline comment tags, while LUA\ntreats these as single line comments. Useful for including debug code in\nthe unpacked intro: the code will not be included in the packed cart.\n\n## Tips for command line arguments\n\n- If pakettic complains about CODE_ZIP chunk size, the code is just too\n  big after compression. In TIC-80, CODE_ZIP chunks do not support\n  multiple banks (and likely never will, as the feature is already\n  deprecated), and thus are unfortunately limited to 65535 bytes.\n  `--uncompressed` is a temporary fix, but code will be uncompressed and\n  thus the size much larger.\n- The Zopfli compression level can be set with `-z<level>`, with level\n  ranging from 0 to 5. When developing, start with `-z0` for fast\n  optimization, and only increase when necessary e.g. when you are just\n  a few bytes over the limit. The default Zopfli-level is 0.\n- The algorithm uses a pseudorandom generator. Sometimes using a\n  different seed finds a few byte better or worse solution. Use command\n  line argument `--seed` to try different seeds.\n- Similarly, different optimization heuristics produce slightly\n  different results. Try different heuristics e.g. with `-alahc`,\n  `-adlas` or `-aanneal`.\n- To avoid re-optimizing all the expressions every time, do a long\n  optimization run, study the results and change your expressions to the\n  forms that pack well. Set the number of steps with `-s`. Use\n  command-line argument `-p` to always print a reasonably readable\n  version of the best solution when one is found.\n- By default, pakettic only includes CODE and DEFAULT chunks. DEFAULT\n  indicates that before loading the cart, TIC-80 loads the default cart,\n  setting default palette, waveforms etc. If you don\'t need the default\n  values (e.g. you set the palette yourself), save one byte by only\n  including CODE chunk in the cart: `-ccode`\n- Working on a tweet-cart? Use `-l` to output LUA carts, which are\n  uncompressed. The optimization algorithm then just optimizes the\n  uncompressed size of the code.\n- If the packed cart is missing sprites, music, map etc., try adding\n  `-call` (or something more specific) to include necessary chunks.\n- Do you want to use the TIC-80 sprites or the tracker, but don\'t like\n  the fact that the data chunks are uncompressed? Use `-d` to have\n  pakettic automatically convert all data chunks into hexadecimal\n  strings in the code, along with a small stub placed at the beginning\n  of the code that interprets the string and loads the data at correct\n  address. For example,\n  `-d -cCODE,MUSIC,PATTERNS,WAVEFORM,SAMPLES,DEFAULT` would include the\n  necessary chunks for the music.\n\n## Known issues\n\n- At the moment, all the branches of swappable operators are assumed to\n  be without side effects. If they have side-effects, the swapping might\n  inadvertedly swap the execution order of the two branches.\n- The parser can crash with large carts. Carts in the size coding range\n  (few thousand characters) do not seem to cause problems, but crashes\n  have been observed parsing carts with tens of thousands of code\n  characters. This may be related to how the pyparsing grammar is\n  defined, which could result in highly recursive parsing and eventually\n  stack overflows.\n\n## Credits\n\nCode contributors: [Veikko Sariola/pestis](https://github.com/vsariola), [wojciech-graj](https://github.com/wojciech-graj),\n[koorogi](https://github.com/koorogi), [dezgeg](https://github.com/dezgeg)\n\nTest corpus contributors: [psenough](corpus/psenough/), [ilmenit](corpus/ilmenit/),\n[gigabates](corpus/gigabates/), [gasman](corpus/gasman/), [pellicus](corpus/pellicus/),\n[luchak](corpus/psenough/fabracid.lua).\n\n## License\n\n[MIT](https://choosealicense.com/licenses/mit/)\n\nThe test corpus carts have their own licenses, see the license files in\nthe subdirectories of the [corpus](corpus/) directory.\n',
+    'long_description': '# Pakettic\n\nPakettic is a command-line tool for minifying and compressing\n[TIC-80](http://tic80.com/) fantasy console carts. The tool is written\nin Python (3.9+) and used especially for\n[sizecoding](http://www.sizecoding.org/wiki/TIC-80). It compresses\nexisting carts approximately ~1.2% better than best alternatives, and by\nusing its [magic comments](#magic-comments), pakettic might find code\nthat compresses even better.\n\n## Installation\n\nInstalling with pip:\n\n```bash\n$ pip install pakettic\n```\n\nInstalling the latest main branch from GitHub:\n\n```bash\n$ pip install git+https://github.com/vsariola/pakettic.git@main\n```\n\nInstalling a checked out version of the repository:\n\n```bash\n$ pip install -e path/to/pakettic\n```\n\nInstalling a checked out version of the repository using\n[poetry](https://python-poetry.org/) for a nice virtual environment with\nlocked dependencies (run inside the pakettic folder):\n\n```bash\n$ poetry install\n```\n\n## Usage\n\nTo compress a cart, run:\n\n```bash\n$ pakettic path/to/cart.tic\n```\n\nIf your PATH is not configured to include pip installed executables, you\ncan use\n\n```bash\n$ python -m pakettic path/to/cart.tic\n```\n\nIf you installed using poetry into a virtual environment, you need to\nprepend `poetry run` before every command e.g.\n\n```bash\n$ poetry run pakettic path/to/cart.tic\n```\n\nPakettic supports both .tic and .lua carts. Multiple input files may be\ndefined. Input files are globbed, so `?`, `*`, and `**` work as\nwildcards for a single character, multiple characters and a directory,\nrespectively.\n\nFor a full list of command line options, see:\n\n```bash\n$ pakettic --help\n```\n\nSee also [tips for command line arguments](#tips-for-command-line-arguments)\n\nRunning all tests:\n\n```bash\n$ poetry run python -m unittest discover -s tests\n```\n\n## Features\n\nPakettic first parses the LUA-script to an abstract syntax tree, and\nthen uses a local optimization algorithm\n([simulated annealing](https://en.wikipedia.org/wiki/Simulated_annealing),\n[late acceptance hill climbing](https://arxiv.org/pdf/1806.09328.pdf) or\nits variant diversified late acceptance search) to randomly mutate the\nsyntax tree & see if it compresses better. Implemented mutations\ninclude:\n  - shortening variable names\n  - flipping comparisons `>`, `<`, `>=`, `<=`, `~=`, and `==`\n  - reordering arithmetic operators `+`, `-`, `*` and `/` and bit logic\n    operators `&`, `~` and `|`\n  - converting `a^2` into `a*a` and vice versa\n  - using either single or double quotes for all strings\n  - converting whole hexadecimals into decimals\n  - convert `for a,b,1 do` into `for a,b do` and vice versa\n  - reordering statements: statements that can be reordered are marked\n    with [magic comments](#magic-comments)\n  - alternative expressions: alternatives are marked with\n    [magic comments](#magic-comments)\n  - folding constant expressions\n\nInternally, pakettic uses [zopfli](https://github.com/google/zopfli) for\nthe compression.\n\n`load\'<code>\'` is parsed as `function(...)<code>end` so you can easily\nrecompress already compressed carts. Conversely, `function()<code>end`\nor `function(...)<code>end` is replaced with `load\'<code>\'` during\ncompression.\n\nNote that `function(...)<code>end` and `load\'<code>\'` are not 100%\nsemantically identical: the load version cannot access locals in the outer\nscope. For example: `local x="hello" function f()print(x)end` works but\n`local x="hello" f=load\'print(x)\'` does not. Since locals are rarely\nused in size-coding, we default to using the load-trick, but you can\ndisable it with the command-line parameter `--no-load`.\n\nHowever, pakettic does not convert functions with parameters. In\nparticular, pakettic does not automatically convert\n`function SCN(x)<code>end` into `SCN=load\'x=...<code>\'`, because they\nare not semantically identical: in the load version, `x` is now global\nand thus could trash a global variable, unintentionally breaking the\ncart. To make `SCN` compress nicely, you have to write it as\n`function SCN(...)x=...<code>end`, taking responsibility for `x` not\noverwriting anything important.\n\nUnnecessary parentheses are removed from expressions so you do not have\nto worry about those.\n\n## Magic comments\n\n### Reorderable statements\n\nThe algorithm will try to reorder statements between `--{` and `--}`.\nFor example:\n\n```lua\n --{\n a="hello"\n b="world"\n --}\n```\n\nwill try both `a="hello"b="world"` and `b="world"a="hello"` to see which\ncompresses better.\n\nNotice that only complete statements can be reordered. Thus, this will\nNOT work:\n\n```lua\n --{\n for x=0,239 do\n  for y=0,135 do\n --}\n  end\n end\n```\n\nA good rule of thumb is that you should be able to replace `--{` and\n`--}` with `do` and `end`, respectively, and still have valid code.\n\nStatements between `--{!` and `--}` are not ordered, so you can make\nblocks of statements that are kept in order within a pair of `--{` and\n`--}` tags.\n\n### Alternative expressions\n\nThere is a special `--|` operator that allows alternative expressions to\nbe tested, to see if they compress better. For example: `5--|4--|6`\nmeans that the algorithm will try 4 and 6 in place of the 5. This will\nnaturally show up as a comment in LUA so you will have to continue the\nexpression on next line if this is in the middle of an expression. `--|`\nhas the lowest precedence, even lower than `^`, so put parentheses if\nyou want to try more complicated expressions e.g. `(x//256)--|(x>>8)`\n\n### Debug code\n\nPakettic treats `--![` and `--!]` as multiline comment tags, while LUA\ntreats these as single line comments. Useful for including debug code in\nthe unpacked intro: the code will not be included in the packed cart.\n\n## Tips for command line arguments\n\n- If you have a CPU with many logical processors and want to max out your CPU\n  usage, you can increase the processing queue length with `-q`. You should\n  usually use `-q N` where N is the number of logical processors. Too high queue\n  length hurts the convergence rate. Defaults to 12.\n- The Zopfli compression level can be set with `-z<level>`, with level\n  ranging from 0 to 5. When developing, start with `-z0` for fast\n  optimization, and only increase when necessary e.g. when you are just\n  a few bytes over the limit. The default Zopfli-level is 0.\n- The algorithm uses a pseudorandom generator. Sometimes using a\n  different seed finds a few byte better or worse solution. Use command\n  line argument `--seed` to try different seeds.\n- Similarly, different optimization heuristics produce slightly\n  different results. Try different heuristics e.g. with `-alahc`,\n  `-adlas` or `-aanneal`.\n- To avoid re-optimizing all the expressions every time, do a long optimization\n  run, study the results and change your expressions to the forms that pack\n  well. Set the number of steps with `-s`; `-s0` iterates forever. Intermediate\n  results are saved. Use command-line argument `-p` to always print a reasonably\n  readable version of the best solution when one is found.\n- By default, pakettic only includes CODE and DEFAULT chunks. DEFAULT\n  indicates that before loading the cart, TIC-80 loads the default cart,\n  setting default palette, waveforms etc. If you don\'t need the default\n  values (e.g. you set the palette yourself), save one byte by only\n  including CODE chunk in the cart: `-ccode`\n- Working on a tweet-cart? Use `-flua` to output LUA carts, which are\n  uncompressed. The optimization algorithm then just optimizes the uncompressed\n  size of the code.\n- If the packed cart is missing sprites, music, map etc., try adding\n  `-call` (or something more specific) to include necessary chunks.\n- Do you want to use the TIC-80 sprites or the tracker, but don\'t like the fact\n  that the data chunks are uncompressed? Is your code longer than 65536\n  characters? Use `-fpng` to output "fake" PNG-like carts, which TIC-80 detects\n  as PNGs based on their headers and loads the cart from a `caRt` chunk, which\n  contains a TIC-80 cart, but this time the entire cart is compressed. ~ 20\n  bytes of additional headers are needed to fool TIC-80, so this is not\n  recommended for very tiny intros. You need to specify which data chunks should\n  be kept. For example, `-fpng -cCODE,MUSIC,PATTERNS,WAVEFORM,SAMPLES,DEFAULT`\n  would include the necessary chunks for the music. PNG-like carts require\n  TIC-80 v1.1.2729 or newer.\n- Alternative way to use data chunks is to use `-d` to have pakettic\n  automatically convert data chunks in bank 0 into hexadecimal strings in the\n  code, along with a small stub placed at the beginning of the code that\n  interprets the string and loads the data at correct address. This breaks\n  `sync` from bank 0, so use with care in multibank carts.\n\n## Known issues\n\n- At the moment, all the branches of swappable operators are assumed to\n  be without side effects. If they have side-effects, the swapping might\n  inadvertedly swap the execution order of the two branches.\n- The parser can crash with large carts. Carts in the size coding range\n  (few thousand characters) do not seem to cause problems, but crashes\n  have been observed parsing carts with tens of thousands of code\n  characters. This may be related to how the pyparsing grammar is\n  defined, which could result in highly recursive parsing and eventually\n  stack overflows.\n\n## Credits\n\nCode contributors: [Veikko Sariola/pestis](https://github.com/vsariola), [wojciech-graj](https://github.com/wojciech-graj),\n[koorogi](https://github.com/koorogi), [dezgeg](https://github.com/dezgeg)\n\nTest corpus contributors: [psenough](corpus/psenough/), [ilmenit](corpus/ilmenit/),\n[gigabates](corpus/gigabates/), [gasman](corpus/gasman/), [pellicus](corpus/pellicus/),\n[luchak](corpus/psenough/fabracid.lua).\n\n## License\n\n[MIT](https://choosealicense.com/licenses/mit/)\n\nThe test corpus carts have their own licenses, see the license files in\nthe subdirectories of the [corpus](corpus/) directory.\n',
     'author': 'Veikko Sariola',
     'author_email': '5684185+vsariola@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/vsariola/pakettic',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pakettic-1.3.1/PKG-INFO` & `pakettic-1.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pakettic
-Version: 1.3.1
+Version: 1.4.0
 Summary: A tool for minifying and compressing TIC-80 fantasy console carts
 Home-page: https://github.com/vsariola/pakettic
 License: MIT
 Keywords: TIC-80,Fantasy Console,Compression,LUA
 Author: Veikko Sariola
 Author-email: 5684185+vsariola@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
@@ -200,53 +200,58 @@
 
 Pakettic treats `--![` and `--!]` as multiline comment tags, while LUA
 treats these as single line comments. Useful for including debug code in
 the unpacked intro: the code will not be included in the packed cart.
 
 ## Tips for command line arguments
 
-- If pakettic complains about CODE_ZIP chunk size, the code is just too
-  big after compression. In TIC-80, CODE_ZIP chunks do not support
-  multiple banks (and likely never will, as the feature is already
-  deprecated), and thus are unfortunately limited to 65535 bytes.
-  `--uncompressed` is a temporary fix, but code will be uncompressed and
-  thus the size much larger.
+- If you have a CPU with many logical processors and want to max out your CPU
+  usage, you can increase the processing queue length with `-q`. You should
+  usually use `-q N` where N is the number of logical processors. Too high queue
+  length hurts the convergence rate. Defaults to 12.
 - The Zopfli compression level can be set with `-z<level>`, with level
   ranging from 0 to 5. When developing, start with `-z0` for fast
   optimization, and only increase when necessary e.g. when you are just
   a few bytes over the limit. The default Zopfli-level is 0.
 - The algorithm uses a pseudorandom generator. Sometimes using a
   different seed finds a few byte better or worse solution. Use command
   line argument `--seed` to try different seeds.
 - Similarly, different optimization heuristics produce slightly
   different results. Try different heuristics e.g. with `-alahc`,
   `-adlas` or `-aanneal`.
-- To avoid re-optimizing all the expressions every time, do a long
-  optimization run, study the results and change your expressions to the
-  forms that pack well. Set the number of steps with `-s`. Use
-  command-line argument `-p` to always print a reasonably readable
-  version of the best solution when one is found.
+- To avoid re-optimizing all the expressions every time, do a long optimization
+  run, study the results and change your expressions to the forms that pack
+  well. Set the number of steps with `-s`; `-s0` iterates forever. Intermediate
+  results are saved. Use command-line argument `-p` to always print a reasonably
+  readable version of the best solution when one is found.
 - By default, pakettic only includes CODE and DEFAULT chunks. DEFAULT
   indicates that before loading the cart, TIC-80 loads the default cart,
   setting default palette, waveforms etc. If you don't need the default
   values (e.g. you set the palette yourself), save one byte by only
   including CODE chunk in the cart: `-ccode`
-- Working on a tweet-cart? Use `-l` to output LUA carts, which are
-  uncompressed. The optimization algorithm then just optimizes the
-  uncompressed size of the code.
+- Working on a tweet-cart? Use `-flua` to output LUA carts, which are
+  uncompressed. The optimization algorithm then just optimizes the uncompressed
+  size of the code.
 - If the packed cart is missing sprites, music, map etc., try adding
   `-call` (or something more specific) to include necessary chunks.
-- Do you want to use the TIC-80 sprites or the tracker, but don't like
-  the fact that the data chunks are uncompressed? Use `-d` to have
-  pakettic automatically convert all data chunks into hexadecimal
-  strings in the code, along with a small stub placed at the beginning
-  of the code that interprets the string and loads the data at correct
-  address. For example,
-  `-d -cCODE,MUSIC,PATTERNS,WAVEFORM,SAMPLES,DEFAULT` would include the
-  necessary chunks for the music.
+- Do you want to use the TIC-80 sprites or the tracker, but don't like the fact
+  that the data chunks are uncompressed? Is your code longer than 65536
+  characters? Use `-fpng` to output "fake" PNG-like carts, which TIC-80 detects
+  as PNGs based on their headers and loads the cart from a `caRt` chunk, which
+  contains a TIC-80 cart, but this time the entire cart is compressed. ~ 20
+  bytes of additional headers are needed to fool TIC-80, so this is not
+  recommended for very tiny intros. You need to specify which data chunks should
+  be kept. For example, `-fpng -cCODE,MUSIC,PATTERNS,WAVEFORM,SAMPLES,DEFAULT`
+  would include the necessary chunks for the music. PNG-like carts require
+  TIC-80 v1.1.2729 or newer.
+- Alternative way to use data chunks is to use `-d` to have pakettic
+  automatically convert data chunks in bank 0 into hexadecimal strings in the
+  code, along with a small stub placed at the beginning of the code that
+  interprets the string and loads the data at correct address. This breaks
+  `sync` from bank 0, so use with care in multibank carts.
 
 ## Known issues
 
 - At the moment, all the branches of swappable operators are assumed to
   be without side effects. If they have side-effects, the swapping might
   inadvertedly swap the execution order of the two branches.
 - The parser can crash with large carts. Carts in the size coding range
```

