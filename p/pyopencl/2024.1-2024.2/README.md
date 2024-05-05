# Comparing `tmp/pyopencl-2024.1.tar.gz` & `tmp/pyopencl-2024.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopencl-2024.1.tar", last modified: Tue Jan 23 22:07:59 2024, max compression
+gzip compressed data, was "pyopencl-2024.2.tar", last modified: Sun May  5 15:53:41 2024, max compression
```

## Comparing `pyopencl-2024.1.tar` & `pyopencl-2024.2.tar`

### file list

```diff
@@ -1,142 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:07:59.732832 pyopencl-2024.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-01-23 22:07:40.000000 pyopencl-2024.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-01-23 22:07:40.000000 pyopencl-2024.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-01-23 22:07:40.000000 pyopencl-2024.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-01-23 22:07:40.000000 pyopencl-2024.1/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-01-23 22:07:59.732832 pyopencl-2024.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3198 2024-01-23 22:07:40.000000 pyopencl-2024.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-01-23 22:07:40.000000 pyopencl-2024.1/README_SETUP.txt
--rw-r--r--   0 runner    (1001) docker     (127)    32046 2024-01-23 22:07:40.000000 pyopencl-2024.1/aksetup_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-01-23 22:07:40.000000 pyopencl-2024.1/configure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:07:59.712832 pyopencl-2024.1/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-01-23 22:07:40.000000 pyopencl-2024.1/contrib/cldis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:07:59.712832 pyopencl-2024.1/contrib/fortran-to-opencl/
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-01-23 22:07:40.000000 pyopencl-2024.1/contrib/fortran-to-opencl/README
--rw-r--r--   0 runner    (1001) docker     (127)    43661 2024-01-23 22:07:40.000000 pyopencl-2024.1/contrib/fortran-to-opencl/translate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-01-23 22:07:40.000000 pyopencl-2024.1/contrib/pyopencl.vim
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:07:59.716832 pyopencl-2024.1/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-01-23 22:07:40.000000 pyopencl-2024.1/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-01-23 22:07:40.000000 pyopencl-2024.1/doc/algorithm.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-01-23 22:07:40.000000 pyopencl-2024.1/doc/array.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-01-23 22:07:40.000000 pyopencl-2024.1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-01-23 22:07:40.000000 pyopencl-2024.1/doc/howto.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-01-23 22:07:40.000000 pyopencl-2024.1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    17802 2024-01-23 22:07:40.000000 pyopencl-2024.1/doc/make_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    29441 2024-01-23 22:07:40.000000 pyopencl-2024.1/doc/misc.rst
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-01-23 22:07:40.000000 pyopencl-2024.1/doc/runtime.rst
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-01-23 22:07:40.000000 pyopencl-2024.1/doc/runtime_const.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-01-23 22:07:40.000000 pyopencl-2024.1/doc/runtime_gl.rst
--rw-r--r--   0 runner    (1001) docker     (127)    17090 2024-01-23 22:07:40.000000 pyopencl-2024.1/doc/runtime_memory.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-01-23 22:07:40.000000 pyopencl-2024.1/doc/runtime_platform.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12385 2024-01-23 22:07:40.000000 pyopencl-2024.1/doc/runtime_program.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-01-23 22:07:40.000000 pyopencl-2024.1/doc/runtime_queue.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-01-23 22:07:40.000000 pyopencl-2024.1/doc/subst.rst
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-23 22:07:40.000000 pyopencl-2024.1/doc/tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-01-23 22:07:40.000000 pyopencl-2024.1/doc/types.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:07:59.716832 pyopencl-2024.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    54748 2024-01-23 22:07:40.000000 pyopencl-2024.1/examples/black-hole-accretion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-01-23 22:07:40.000000 pyopencl-2024.1/examples/demo-struct-reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-01-23 22:07:40.000000 pyopencl-2024.1/examples/demo.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-01-23 22:07:40.000000 pyopencl-2024.1/examples/demo_array.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-01-23 22:07:40.000000 pyopencl-2024.1/examples/demo_array_svm.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-23 22:07:40.000000 pyopencl-2024.1/examples/demo_elementwise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-01-23 22:07:40.000000 pyopencl-2024.1/examples/demo_elementwise_complex.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-01-23 22:07:40.000000 pyopencl-2024.1/examples/demo_mandelbrot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-01-23 22:07:40.000000 pyopencl-2024.1/examples/demo_meta_codepy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-01-23 22:07:40.000000 pyopencl-2024.1/examples/demo_meta_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-01-23 22:07:40.000000 pyopencl-2024.1/examples/dump-performance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-01-23 22:07:40.000000 pyopencl-2024.1/examples/dump-properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-01-23 22:07:40.000000 pyopencl-2024.1/examples/gl_interop_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-01-23 22:07:40.000000 pyopencl-2024.1/examples/gl_particle_animation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-01-23 22:07:40.000000 pyopencl-2024.1/examples/ipython-demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-01-23 22:07:40.000000 pyopencl-2024.1/examples/median-filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    32112 2024-01-23 22:07:40.000000 pyopencl-2024.1/examples/n-body.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-01-23 22:07:40.000000 pyopencl-2024.1/examples/narray.py
--rw-r--r--   0 runner    (1001) docker     (127)    66806 2024-01-23 22:07:40.000000 pyopencl-2024.1/examples/noisyImage.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    35441 2024-01-23 22:07:40.000000 pyopencl-2024.1/examples/pi-monte-carlo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-01-23 22:07:40.000000 pyopencl-2024.1/examples/svm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-01-23 22:07:40.000000 pyopencl-2024.1/examples/transpose.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:07:59.720832 pyopencl-2024.1/pyopencl/
--rw-r--r--   0 runner    (1001) docker     (127)    80151 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/_cluda.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/_mymako.py
--rw-r--r--   0 runner    (1001) docker     (127)    51198 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)   111639 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/bitonic_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)    16172 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/bitonic_sort_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    15720 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/capture_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:07:59.724832 pyopencl-2024.1/pyopencl/characterize/
--rw-r--r--   0 runner    (1001) docker     (127)    13827 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/characterize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6865 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/characterize/performance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:07:59.724832 pyopencl-2024.1/pyopencl/cl/
--rw-r--r--   0 runner    (1001) docker     (127)     8122 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/cl/pyopencl-airy.cl
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/cl/pyopencl-bessel-j-complex.cl
--rw-r--r--   0 runner    (1001) docker     (127)    23274 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/cl/pyopencl-bessel-j.cl
--rw-r--r--   0 runner    (1001) docker     (127)    12297 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/cl/pyopencl-bessel-y.cl
--rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/cl/pyopencl-complex.h
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/cl/pyopencl-eval-tbl.cl
--rw-r--r--   0 runner    (1001) docker     (127)    31561 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/cl/pyopencl-hankel-complex.cl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:07:59.724832 pyopencl-2024.1/pyopencl/cl/pyopencl-random123/
--rw-r--r--   0 runner    (1001) docker     (127)    17088 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/cl/pyopencl-random123/array.h
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/cl/pyopencl-random123/openclfeatures.h
--rw-r--r--   0 runner    (1001) docker     (127)    21740 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/cl/pyopencl-random123/philox.cl
--rw-r--r--   0 runner    (1001) docker     (127)    54699 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/cl/pyopencl-random123/threefry.cl
--rw-r--r--   0 runner    (1001) docker     (127)    38528 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/cl/pyopencl-ranluxcl.cl
--rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/clmath.py
--rw-r--r--   0 runner    (1001) docker     (127)    25553 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/clrandom.py
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/cltypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:07:59.724832 pyopencl-2024.1/pyopencl/compyte/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 22:07:59.000000 pyopencl-2024.1/pyopencl/compyte/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-01-23 22:07:59.000000 pyopencl-2024.1/pyopencl/compyte/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-01-23 22:07:59.000000 pyopencl-2024.1/pyopencl/compyte/dtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:07:59.724832 pyopencl-2024.1/pyopencl/compyte/ndarray/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 22:07:59.000000 pyopencl-2024.1/pyopencl/compyte/ndarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    76836 2024-01-23 22:07:59.000000 pyopencl-2024.1/pyopencl/compyte/ndarray/gen_elemwise.py
--rw-r--r--   0 runner    (1001) docker     (127)    56332 2024-01-23 22:07:59.000000 pyopencl-2024.1/pyopencl/compyte/ndarray/gen_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-01-23 22:07:59.000000 pyopencl-2024.1/pyopencl/compyte/ndarray/setup_opencl.py
--rw-r--r--   0 runner    (1001) docker     (127)    18436 2024-01-23 22:07:59.000000 pyopencl-2024.1/pyopencl/compyte/ndarray/test_gpu_elemwise.py
--rw-r--r--   0 runner    (1001) docker     (127)    17782 2024-01-23 22:07:59.000000 pyopencl-2024.1/pyopencl/compyte/ndarray/test_gpu_ndarray.py
--rw-r--r--   0 runner    (1001) docker     (127)    38637 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/elementwise.py
--rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/invoker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/ipython_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)    25547 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)    65308 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)    45549 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyopencl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:07:59.732832 pyopencl-2024.1/pyopencl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-01-23 22:07:59.000000 pyopencl-2024.1/pyopencl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-01-23 22:07:59.000000 pyopencl-2024.1/pyopencl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 22:07:59.000000 pyopencl-2024.1/pyopencl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 22:07:59.000000 pyopencl-2024.1/pyopencl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-01-23 22:07:59.000000 pyopencl-2024.1/pyopencl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-23 22:07:59.000000 pyopencl-2024.1/pyopencl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-01-23 22:07:40.000000 pyopencl-2024.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-23 22:07:40.000000 pyopencl-2024.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-01-23 22:07:59.732832 pyopencl-2024.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     9507 2024-01-23 22:07:40.000000 pyopencl-2024.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:07:59.728832 pyopencl-2024.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-01-23 22:07:40.000000 pyopencl-2024.1/src/bitlog.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-01-23 22:07:40.000000 pyopencl-2024.1/src/bitlog.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-01-23 22:07:40.000000 pyopencl-2024.1/src/clinfo_ext.h
--rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-01-23 22:07:40.000000 pyopencl-2024.1/src/mempool.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-23 22:07:40.000000 pyopencl-2024.1/src/pyopencl_ext.h
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-01-23 22:07:40.000000 pyopencl-2024.1/src/tools.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-01-23 22:07:40.000000 pyopencl-2024.1/src/wrap_cl.cpp
--rw-r--r--   0 runner    (1001) docker     (127)   163384 2024-01-23 22:07:40.000000 pyopencl-2024.1/src/wrap_cl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-01-23 22:07:40.000000 pyopencl-2024.1/src/wrap_cl_part_1.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    20925 2024-01-23 22:07:40.000000 pyopencl-2024.1/src/wrap_cl_part_2.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    38145 2024-01-23 22:07:40.000000 pyopencl-2024.1/src/wrap_constants.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-01-23 22:07:40.000000 pyopencl-2024.1/src/wrap_helpers.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    18767 2024-01-23 22:07:40.000000 pyopencl-2024.1/src/wrap_mempool.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:07:59.728832 pyopencl-2024.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-01-23 22:07:40.000000 pyopencl-2024.1/test/add-vectors-32.spv
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-23 22:07:40.000000 pyopencl-2024.1/test/add-vectors-64.spv
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-23 22:07:40.000000 pyopencl-2024.1/test/empty-header.h
--rw-r--r--   0 runner    (1001) docker     (127)    35358 2024-01-23 22:07:40.000000 pyopencl-2024.1/test/test_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)    63301 2024-01-23 22:07:40.000000 pyopencl-2024.1/test/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-01-23 22:07:40.000000 pyopencl-2024.1/test/test_arrays_in_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16187 2024-01-23 22:07:40.000000 pyopencl-2024.1/test/test_clmath.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-01-23 22:07:40.000000 pyopencl-2024.1/test/test_clrandom.py
--rw-r--r--   0 runner    (1001) docker     (127)     9781 2024-01-23 22:07:40.000000 pyopencl-2024.1/test/test_enqueue_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)    43780 2024-01-23 22:07:40.000000 pyopencl-2024.1/test/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.178653 pyopencl-2024.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-05 15:53:24.000000 pyopencl-2024.2/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-05 15:53:24.000000 pyopencl-2024.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-05 15:53:24.000000 pyopencl-2024.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-05 15:53:24.000000 pyopencl-2024.2/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-05 15:53:41.178653 pyopencl-2024.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-05 15:53:24.000000 pyopencl-2024.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-05 15:53:24.000000 pyopencl-2024.2/README_SETUP.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    32285 2024-05-05 15:53:24.000000 pyopencl-2024.2/aksetup_helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       94 2024-05-05 15:53:24.000000 pyopencl-2024.2/configure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.162653 pyopencl-2024.2/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-05 15:53:24.000000 pyopencl-2024.2/contrib/cldis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.162653 pyopencl-2024.2/contrib/fortran-to-opencl/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-05 15:53:24.000000 pyopencl-2024.2/contrib/fortran-to-opencl/README
+-rw-r--r--   0 runner    (1001) docker     (127)    43618 2024-05-05 15:53:24.000000 pyopencl-2024.2/contrib/fortran-to-opencl/translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-05 15:53:24.000000 pyopencl-2024.2/contrib/pyopencl.vim
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.162653 pyopencl-2024.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/algorithm.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/array.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/howto.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17804 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/make_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29441 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/runtime.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/runtime_const.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/runtime_gl.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17090 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/runtime_memory.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/runtime_platform.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12672 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/runtime_program.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/runtime_queue.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/subst.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-05 15:53:24.000000 pyopencl-2024.2/doc/types.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.166653 pyopencl-2024.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    54750 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/black-hole-accretion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/demo-struct-reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/demo_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/demo_array_svm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/demo_elementwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/demo_elementwise_complex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/demo_mandelbrot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/demo_meta_codepy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/demo_meta_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/dump-performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/dump-properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/gl_interop_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/gl_particle_animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/ipython-demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/median-filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32124 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/n-body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/narray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66806 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/noisyImage.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    35442 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/pi-monte-carlo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/svm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-05-05 15:53:24.000000 pyopencl-2024.2/examples/transpose.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.170653 pyopencl-2024.2/pyopencl/
+-rw-r--r--   0 runner    (1001) docker     (127)    80676 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/_cluda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/_mymako.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51196 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   111717 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7876 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/bitonic_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16172 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/bitonic_sort_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15959 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/capture_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.170653 pyopencl-2024.2/pyopencl/characterize/
+-rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/characterize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/characterize/performance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.174653 pyopencl-2024.2/pyopencl/cl/
+-rw-r--r--   0 runner    (1001) docker     (127)     8122 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cl/pyopencl-airy.cl
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cl/pyopencl-bessel-j-complex.cl
+-rw-r--r--   0 runner    (1001) docker     (127)    23274 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cl/pyopencl-bessel-j.cl
+-rw-r--r--   0 runner    (1001) docker     (127)    12297 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cl/pyopencl-bessel-y.cl
+-rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cl/pyopencl-complex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cl/pyopencl-eval-tbl.cl
+-rw-r--r--   0 runner    (1001) docker     (127)    31561 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cl/pyopencl-hankel-complex.cl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.174653 pyopencl-2024.2/pyopencl/cl/pyopencl-random123/
+-rw-r--r--   0 runner    (1001) docker     (127)    17088 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cl/pyopencl-random123/array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cl/pyopencl-random123/openclfeatures.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21740 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cl/pyopencl-random123/philox.cl
+-rw-r--r--   0 runner    (1001) docker     (127)    54699 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cl/pyopencl-random123/threefry.cl
+-rw-r--r--   0 runner    (1001) docker     (127)     8222 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/clmath.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13043 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/clrandom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/cltypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.174653 pyopencl-2024.2/pyopencl/compyte/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:40.000000 pyopencl-2024.2/pyopencl/compyte/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-05-05 15:53:40.000000 pyopencl-2024.2/pyopencl/compyte/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-05-05 15:53:40.000000 pyopencl-2024.2/pyopencl/compyte/dtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.174653 pyopencl-2024.2/pyopencl/compyte/ndarray/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:40.000000 pyopencl-2024.2/pyopencl/compyte/ndarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76820 2024-05-05 15:53:40.000000 pyopencl-2024.2/pyopencl/compyte/ndarray/gen_elemwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56315 2024-05-05 15:53:40.000000 pyopencl-2024.2/pyopencl/compyte/ndarray/gen_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-05-05 15:53:40.000000 pyopencl-2024.2/pyopencl/compyte/ndarray/setup_opencl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18438 2024-05-05 15:53:40.000000 pyopencl-2024.2/pyopencl/compyte/ndarray/test_gpu_elemwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17781 2024-05-05 15:53:40.000000 pyopencl-2024.2/pyopencl/compyte/ndarray/test_gpu_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38602 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/elementwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13994 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/invoker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/ipython_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25524 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65500 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45510 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyopencl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.178653 pyopencl-2024.2/pyopencl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-05 15:53:41.000000 pyopencl-2024.2/pyopencl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-05 15:53:41.000000 pyopencl-2024.2/pyopencl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 15:53:41.000000 pyopencl-2024.2/pyopencl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 15:53:40.000000 pyopencl-2024.2/pyopencl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-05 15:53:41.000000 pyopencl-2024.2/pyopencl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-05 15:53:41.000000 pyopencl-2024.2/pyopencl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-05 15:53:24.000000 pyopencl-2024.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-05 15:53:24.000000 pyopencl-2024.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-05 15:53:41.178653 pyopencl-2024.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8648 2024-05-05 15:53:24.000000 pyopencl-2024.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.178653 pyopencl-2024.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/bitlog.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/bitlog.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/clinfo_ext.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/mempool.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/pyopencl_ext.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/tools.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/wrap_cl.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)   165179 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/wrap_cl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/wrap_cl_part_1.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19945 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/wrap_cl_part_2.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    38496 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/wrap_constants.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/wrap_helpers.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18776 2024-05-05 15:53:24.000000 pyopencl-2024.2/src/wrap_mempool.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 15:53:41.178653 pyopencl-2024.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-05 15:53:24.000000 pyopencl-2024.2/test/add-vectors-32.spv
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-05 15:53:24.000000 pyopencl-2024.2/test/add-vectors-64.spv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-05 15:53:24.000000 pyopencl-2024.2/test/empty-header.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35331 2024-05-05 15:53:24.000000 pyopencl-2024.2/test/test_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63792 2024-05-05 15:53:24.000000 pyopencl-2024.2/test/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-05-05 15:53:24.000000 pyopencl-2024.2/test/test_arrays_in_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16184 2024-05-05 15:53:24.000000 pyopencl-2024.2/test/test_clmath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-05 15:53:24.000000 pyopencl-2024.2/test/test_clrandom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-05-05 15:53:24.000000 pyopencl-2024.2/test/test_enqueue_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44638 2024-05-05 15:53:24.000000 pyopencl-2024.2/test/test_wrapper.py
```

### Comparing `pyopencl-2024.1/CITATION.cff` & `pyopencl-2024.2/CITATION.cff`

 * *Files 0% similar despite different names*

```diff
@@ -67,7 +67,8 @@
   orcid: 'https://orcid.org/0000-0002-5470-1676'
 
 title: "PyOpenCL"
 version: 2022.1.3
 doi: 10.5281/zenodo.6533956
 date-released: 2022-03-10
 url: "https://github.com/inducer/pyopencl"
+license: MIT
```

### Comparing `pyopencl-2024.1/LICENSE` & `pyopencl-2024.2/LICENSE`

 * *Files 15% similar despite different names*

```diff
@@ -74,30 +74,7 @@
     OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
     SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
     LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
     DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
     THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
     (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
     OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-PyOpenCL includes the RANLUXCL random number generator:
-
-    Copyright (c) 2011 Ivar Ursin Nikolaisen
-
-    Permission is hereby granted, free of charge, to any person obtaining a copy of this
-    software and associated documentation files (the "Software"), to deal in the Software
-    without restriction, including without limitation the rights to use, copy, modify,
-    merge, publish, distribute, sublicense, and/or sell copies of the Software, and to
-    permit persons to whom the Software is furnished to do so, subject to the following
-    conditions:
-
-    The above copyright notice and this permission notice shall be included in all copies
-    or substantial portions of the Software.
-
-    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
-    INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-    PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
-    HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
-    CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE
-    OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-
```

### Comparing `pyopencl-2024.1/MANIFEST.in` & `pyopencl-2024.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/PKG-INFO` & `pyopencl-2024.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopencl
-Version: 2024.1
+Version: 2024.2
 Summary: Python wrapper for OpenCL
 Home-page: http://mathema.tician.de/software/pyopencl
 Author: Andreas Kloeckner
 Author-email: inform@tiker.net
 License: MIT
 Classifier: Environment :: Console
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,40 +18,43 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: ~=3.8
 License-File: LICENSE
 Requires-Dist: numpy
-Requires-Dist: pytools>=2021.2.7
+Requires-Dist: pytools>=2022.1.13
 Requires-Dist: platformdirs>=2.2.0
+Requires-Dist: importlib-resources; python_version < "3.9"
 Provides-Extra: pocl
 Requires-Dist: pocl_binary_distribution>=1.2; extra == "pocl"
 Provides-Extra: oclgrind
 Requires-Dist: oclgrind_binary_distribution>=18.3; extra == "oclgrind"
 Provides-Extra: test
 Requires-Dist: pytest>=7.0.0; extra == "test"
 Requires-Dist: Mako; extra == "test"
 
 PyOpenCL: Pythonic Access to OpenCL, with Arrays and Algorithms
 ===============================================================
 
-.. image:: https://gitlab.tiker.net/inducer/pyopencl/badges/main/pipeline.svg
+.. |badge-gitlab-ci| image:: https://gitlab.tiker.net/inducer/pyopencl/badges/main/pipeline.svg
     :alt: Gitlab Build Status
     :target: https://gitlab.tiker.net/inducer/pyopencl/commits/main
-.. image:: https://github.com/inducer/pyopencl/workflows/CI/badge.svg?branch=main&event=push
+.. |badge-github-ci| image:: https://github.com/inducer/pyopencl/workflows/CI/badge.svg?branch=main&event=push
     :alt: Github Build Status
     :target: https://github.com/inducer/pyopencl/actions?query=branch%3Amain+workflow%3ACI+event%3Apush
-.. image:: https://badge.fury.io/py/pyopencl.svg
+.. |badge-pypi| image:: https://badge.fury.io/py/pyopencl.svg
     :alt: Python Package Index Release Page
     :target: https://pypi.org/project/pyopencl/
-.. image:: https://zenodo.org/badge/1575307.svg
+.. |badge-zenodo| image:: https://zenodo.org/badge/1575307.svg
     :alt: Zenodo DOI for latest release
     :target: https://zenodo.org/badge/latestdoi/1575307
 
+|badge-gitlab-ci| |badge-github-ci| |badge-pypi| |badge-zenodo|
+
 PyOpenCL lets you access GPUs and other massively parallel compute
 devices from Python. It tries to offer computing goodness in the
 spirit of its sister project `PyCUDA <https://mathema.tician.de/software/pycuda>`__:
 
 * Object cleanup tied to lifetime of objects. This idiom, often
   called `RAII <https://en.wikipedia.org/wiki/Resource_Acquisition_Is_Initialization>`__
   in C++, makes it much easier to write correct, leak- and
@@ -80,26 +83,23 @@
 Simple 4-step `install instructions <https://documen.tician.de/pyopencl/misc.html#installation>`__
 using Conda on Linux and macOS (that also install a working OpenCL implementation!)
 can be found in the `documentation <https://documen.tician.de/pyopencl/>`__.
 
 What you'll need if you do *not* want to use the convenient instructions above and
 instead build from source:
 
-* gcc/g++ new enough to be compatible with pybind11
-  (see their `FAQ <https://pybind11.readthedocs.io/en/stable/faq.html>`__)
+* g++/clang new enough to be compatible with nanobind (specifically, full support of C++17 is needed)
 * `numpy <https://numpy.org>`__, and
 * an OpenCL implementation. (See this `howto <https://wiki.tiker.net/OpenCLHowTo>`__
   for how to get one.)
 
 Links
 -----
 
 * `Documentation <https://documen.tician.de/pyopencl>`__
   (read how things work)
+* `Python package index <https://pypi.python.org/pypi/pyopencl>`__
+  (download releases, including binary wheels for Linux, macOS, Windows)
 * `Conda Forge <https://anaconda.org/conda-forge/pyopencl>`__
   (download binary packages for Linux, macOS, Windows)
-* `Python package index <https://pypi.python.org/pypi/pyopencl>`__
-  (download releases)
-* `C. Gohlke's Windows binaries <https://www.lfd.uci.edu/~gohlke/pythonlibs/#pyopencl>`__
-  (download Windows binaries)
 * `Github <https://github.com/inducer/pyopencl>`__
   (get latest source code, file bugs)
```

### Comparing `pyopencl-2024.1/README.rst` & `pyopencl-2024.2/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 PyOpenCL: Pythonic Access to OpenCL, with Arrays and Algorithms
 ===============================================================
 
-.. image:: https://gitlab.tiker.net/inducer/pyopencl/badges/main/pipeline.svg
+.. |badge-gitlab-ci| image:: https://gitlab.tiker.net/inducer/pyopencl/badges/main/pipeline.svg
     :alt: Gitlab Build Status
     :target: https://gitlab.tiker.net/inducer/pyopencl/commits/main
-.. image:: https://github.com/inducer/pyopencl/workflows/CI/badge.svg?branch=main&event=push
+.. |badge-github-ci| image:: https://github.com/inducer/pyopencl/workflows/CI/badge.svg?branch=main&event=push
     :alt: Github Build Status
     :target: https://github.com/inducer/pyopencl/actions?query=branch%3Amain+workflow%3ACI+event%3Apush
-.. image:: https://badge.fury.io/py/pyopencl.svg
+.. |badge-pypi| image:: https://badge.fury.io/py/pyopencl.svg
     :alt: Python Package Index Release Page
     :target: https://pypi.org/project/pyopencl/
-.. image:: https://zenodo.org/badge/1575307.svg
+.. |badge-zenodo| image:: https://zenodo.org/badge/1575307.svg
     :alt: Zenodo DOI for latest release
     :target: https://zenodo.org/badge/latestdoi/1575307
 
+|badge-gitlab-ci| |badge-github-ci| |badge-pypi| |badge-zenodo|
+
 PyOpenCL lets you access GPUs and other massively parallel compute
 devices from Python. It tries to offer computing goodness in the
 spirit of its sister project `PyCUDA <https://mathema.tician.de/software/pycuda>`__:
 
 * Object cleanup tied to lifetime of objects. This idiom, often
   called `RAII <https://en.wikipedia.org/wiki/Resource_Acquisition_Is_Initialization>`__
   in C++, makes it much easier to write correct, leak- and
@@ -46,26 +48,23 @@
 Simple 4-step `install instructions <https://documen.tician.de/pyopencl/misc.html#installation>`__
 using Conda on Linux and macOS (that also install a working OpenCL implementation!)
 can be found in the `documentation <https://documen.tician.de/pyopencl/>`__.
 
 What you'll need if you do *not* want to use the convenient instructions above and
 instead build from source:
 
-* gcc/g++ new enough to be compatible with pybind11
-  (see their `FAQ <https://pybind11.readthedocs.io/en/stable/faq.html>`__)
+* g++/clang new enough to be compatible with nanobind (specifically, full support of C++17 is needed)
 * `numpy <https://numpy.org>`__, and
 * an OpenCL implementation. (See this `howto <https://wiki.tiker.net/OpenCLHowTo>`__
   for how to get one.)
 
 Links
 -----
 
 * `Documentation <https://documen.tician.de/pyopencl>`__
   (read how things work)
+* `Python package index <https://pypi.python.org/pypi/pyopencl>`__
+  (download releases, including binary wheels for Linux, macOS, Windows)
 * `Conda Forge <https://anaconda.org/conda-forge/pyopencl>`__
   (download binary packages for Linux, macOS, Windows)
-* `Python package index <https://pypi.python.org/pypi/pyopencl>`__
-  (download releases)
-* `C. Gohlke's Windows binaries <https://www.lfd.uci.edu/~gohlke/pythonlibs/#pyopencl>`__
-  (download Windows binaries)
 * `Github <https://github.com/inducer/pyopencl>`__
   (get latest source code, file bugs)
```

### Comparing `pyopencl-2024.1/README_SETUP.txt` & `pyopencl-2024.2/README_SETUP.txt`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/aksetup_helper.py` & `pyopencl-2024.2/aksetup_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import sys
+
+
 try:
     from setuptools import Extension
-    from setuptools.command.build_ext import (  # noqa: N812
-            build_ext as BaseBuildExtCommand)
+    from setuptools.command.build_ext import \
+        build_ext as BaseBuildExtCommand  # noqa: N812
 
 except ImportError:
     class Extension:
         pass
 
     class BaseBuildExtCommand:
         pass
@@ -39,22 +41,29 @@
         print("Sorry, your build failed. Try rerunning configure.py with "
                 "different options.")
         print(DASH_SEPARATOR)
         raise
 
 
 def get_numpy_incpath():
-    from os.path import join, dirname
     from importlib.util import find_spec
+    from os.path import dirname, exists, join
     origin = find_spec("numpy").origin
     if origin is None:
         raise RuntimeError("origin of numpy package not found")
 
     pathname = dirname(origin)
-    return join(pathname, "core", "include")
+    for p in [
+        join(pathname, "_core", "include"),  # numpy 2 onward
+        join(pathname, "core", "include"),  # numpy prior to 2
+    ]:
+        if exists(join(p, "numpy", "arrayobject.h")):
+            return p
+
+    raise RuntimeError("no valid path for numpy found")
 
 
 class NumpyExtension(Extension):
     # nicked from
     # http://mail.python.org/pipermail/distutils-sig/2007-September/008253.html
     # solution by Michael Hoffmann
     def __init__(self, *args, **kwargs):
@@ -758,24 +767,24 @@
         new_lines.append(line)
     new_lines.insert(1, "# DO NOT EDIT THIS FILE -- "
             "it was generated by configure.py\n")
     new_lines.insert(2, "# %s\n" % (" ".join(sys.argv)))
     with open(fname, "w") as outf:
         outf.write("".join(new_lines))
 
-    from os import stat, chmod
+    from os import chmod, stat
     infile_stat_res = stat(fname_in)
     chmod(fname, infile_stat_res.st_mode)
 
 
 # {{{ git bits
 
 def _run_git_command(cmd):
     git_error = None
-    from subprocess import Popen, PIPE
+    from subprocess import PIPE, Popen
     stdout = None
     try:
         popen = Popen(["git"] + cmd, stdout=PIPE)
         stdout, stderr = popen.communicate()
         if popen.returncode != 0:
             git_error = "git returned error code %d: %s" % (popen.returncode, stderr)
     except OSError:
```

### Comparing `pyopencl-2024.1/contrib/cldis.py` & `pyopencl-2024.2/contrib/cldis.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,31 +24,31 @@
 cldis.py
 
 A script to compile and print the native code for a OpenCL kernel.
 
 Usage: python cldis.py prog.cl <ptx/sass/asm> <build options>
 """
 
+import glob
 import os
-import tempfile
-import subprocess
 import re
+import subprocess
 import sys
-import glob
+import tempfile
 
 
 def main(ctx, tmp_dir, cl_str, output=None, build_options=[]):
     device = ctx.devices[0]
     platform = device.platform
     if platform.name == "NVIDIA CUDA":
         supported_outputs = ["ptx", "sass"]
     elif platform.name == "Portable Computing Language":
         if device.name.startswith("NVIDIA"):
             supported_outputs = ["ptx", "sass"]
-        elif device.name.startswith("pthread"):
+        elif device.name.startswith("pthread") or device.name.startswith("cpu")
             supported_outputs = ["asm"]
         else:
             raise NotImplementedError(f"Unknown pocl device '{device.name}'")
     else:
         raise NotImplementedError(f"Unknown opencl device '{device}'")
     if output is None:
         output = supported_outputs[0]
```

### Comparing `pyopencl-2024.1/contrib/fortran-to-opencl/README` & `pyopencl-2024.2/contrib/fortran-to-opencl/README`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/contrib/fortran-to-opencl/translate.py` & `pyopencl-2024.2/contrib/fortran-to-opencl/translate.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,26 +16,25 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
-import cgen
-import numpy as np
 import re
-from pymbolic.parser import Parser as ExpressionParserBase
-from pymbolic.mapper import CombineMapper
-import pymbolic.primitives as p
-from pymbolic.mapper.c_code import CCodeMapper as CCodeMapperBase
 from sys import intern
-
 from warnings import warn
 
+import cgen
+import numpy as np
+import pymbolic.primitives as p
 import pytools.lex
+from pymbolic.mapper import CombineMapper
+from pymbolic.mapper.c_code import CCodeMapper as CCodeMapperBase
+from pymbolic.parser import Parser as ExpressionParserBase
 
 
 class TranslatorWarning(UserWarning):
     pass
 
 
 class TranslationError(RuntimeError):
@@ -150,16 +149,15 @@
         self.tree_walker = tree_walker
 
     _PREC_FUNC_ARGS = 1
 
     def parse_terminal(self, pstate):
         scope = self.tree_walker.scope_stack[-1]
 
-        from pymbolic.parser import (
-            _identifier, _openpar, _closepar, _float)
+        from pymbolic.parser import _closepar, _float, _identifier, _openpar
 
         next_tag = pstate.next_tag()
         if next_tag is _float:
             value = pstate.next_str_and_advance().lower()
             if "d" in value:
                 dtype = np.float64
             else:
@@ -217,32 +215,31 @@
             _greater_than: ">",
             _greater_equal: ">=",
             _equal: "==",
             _not_equal: "!=",
             }
 
     def parse_prefix(self, pstate, min_precedence=0):
-        from pymbolic.parser import _PREC_UNARY
         import pymbolic.primitives as primitives
+        from pymbolic.parser import _PREC_UNARY
 
         pstate.expect_not_end()
 
         if pstate.is_next(_not):
             pstate.advance()
             return primitives.LogicalNot(
                     self.parse_expression(pstate, _PREC_UNARY))
         else:
             return ExpressionParserBase.parse_prefix(self, pstate)
 
     def parse_postfix(self, pstate, min_precedence, left_exp):
         from pymbolic.parser import (
-                _PREC_CALL, _PREC_COMPARISON, _openpar,
-                _PREC_LOGICAL_OR, _PREC_LOGICAL_AND)
-        from pymbolic.primitives import (
-                Comparison, LogicalAnd, LogicalOr)
+            _PREC_CALL, _PREC_COMPARISON, _PREC_LOGICAL_AND, _PREC_LOGICAL_OR,
+            _openpar)
+        from pymbolic.primitives import Comparison, LogicalAnd, LogicalOr
 
         next_tag = pstate.next_tag()
         if next_tag is _openpar and _PREC_CALL > min_precedence:
             raise TranslationError("parenthesis operator only works on names")
         elif next_tag in self.COMP_MAP and _PREC_COMPARISON > min_precedence:
             pstate.advance()
             left_exp = Comparison(
@@ -347,15 +344,15 @@
             tgt_name = complex_type_name(tgt_dtype)
 
             reals = [child for child in expr.children
                     if "c" != self.infer_type(child).kind]
             complexes = [child for child in expr.children
                     if "c" == self.infer_type(child).kind]
 
-            from pymbolic.mapper.stringifier import PREC_SUM, PREC_NONE
+            from pymbolic.mapper.stringifier import PREC_NONE, PREC_SUM
             real_sum = self.join_rec(" + ", reals, PREC_SUM)
 
             if len(complexes) == 1:
                 myprec = PREC_SUM
             else:
                 myprec = PREC_NONE
 
@@ -383,15 +380,15 @@
             tgt_name = complex_type_name(tgt_dtype)
 
             reals = [child for child in expr.children
                     if "c" != self.infer_type(child).kind]
             complexes = [child for child in expr.children
                     if "c" == self.infer_type(child).kind]
 
-            from pymbolic.mapper.stringifier import PREC_PRODUCT, PREC_NONE
+            from pymbolic.mapper.stringifier import PREC_NONE, PREC_PRODUCT
             real_prd = self.join_rec("*", reals, PREC_PRODUCT)
 
             if len(complexes) == 1:
                 myprec = PREC_PRODUCT
             else:
                 myprec = PREC_NONE
 
@@ -485,15 +482,15 @@
         else:
             ind_prefix = ""
 
         idx = expr.index
         if isinstance(idx, tuple) and len(idx) == 1:
             idx, = idx
 
-        from pymbolic.mapper.stringifier import PREC_NONE, PREC_CALL
+        from pymbolic.mapper.stringifier import PREC_CALL, PREC_NONE
         return self.parenthesize_if_needed(
                 self.format("%s[%s%s]",
                     self.scope.translate_var_name(expr.aggregate.name),
                     ind_prefix,
                     self.rec(idx, PREC_NONE)),
                 enclosing_prec, PREC_CALL)
```

### Comparing `pyopencl-2024.1/contrib/pyopencl.vim` & `pyopencl-2024.2/contrib/pyopencl.vim`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/doc/Makefile` & `pyopencl-2024.2/doc/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Minimal makefile for Sphinx documentation
 #
 
 # You can set these variables from the command line, and also
 # from the environment for the first two.
-SPHINXOPTS    ?=
+SPHINXOPTS    ?= -W -n
 SPHINXBUILD   ?= python $(shell which sphinx-build)
 SOURCEDIR     = .
 BUILDDIR      = _build
 
 # Put it first so that "make" without argument is like "make help".
 help:
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `pyopencl-2024.1/doc/algorithm.rst` & `pyopencl-2024.2/doc/algorithm.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/doc/array.rst` & `pyopencl-2024.2/doc/array.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/doc/conf.py` & `pyopencl-2024.2/doc/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from urllib.request import urlopen
 
+
 _conf_url = \
         "https://raw.githubusercontent.com/inducer/sphinxconfig/main/sphinxconfig.py"
 with urlopen(_conf_url) as _inf:
     exec(compile(_inf.read(), _conf_url, "exec"), globals())
 
 exclude_patterns = ["subst.rst"]
 
@@ -17,8 +18,9 @@
 # The full version, including alpha/beta/rc tags.
 release = ver_dic["VERSION_TEXT"]
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
     "numpy": ("https://numpy.org/doc/stable/", None),
     "mako": ("https://docs.makotemplates.org/en/latest", None),
+    "pytools": ("https://documen.tician.de/pytools", None),
 }
```

### Comparing `pyopencl-2024.1/doc/howto.rst` & `pyopencl-2024.2/doc/howto.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/doc/index.rst` & `pyopencl-2024.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/doc/make_constants.py` & `pyopencl-2024.2/doc/make_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
 import pyopencl as cl
 
+
 fission = ("cl_ext_device_fission", "2011.1")
 nv_devattr = ("cl_nv_device_attribute_query", "0.92")
 gl_sharing = ("cl_khr_gl_sharing", "0.92")
 cl_spir_devattr = ("cl_khr_spir", "2016.2")
 cl_11 = ("CL_1.1", "0.92")
 cl_12 = ("CL_1.2", "2011.2")
 cl_12_2015 = ("CL_1.2", "2015.2")
@@ -544,14 +545,15 @@
     print()
     print("    This set of PyOpenCL documentation is incomplete because it")
     print("    was generated on a PyOpenCL build that did not support OpenGL.")
     print()
 
 import inspect
 
+
 CONSTANT_CLASSES = [
         getattr(cl, name) for name in dir(cl)
         if inspect.isclass(getattr(cl, name))
         and name[0].islower() and name not in ["zip", "map", "range"]]
 
 print(".. This is an automatically generated file. DO NOT EDIT")
 print()
```

### Comparing `pyopencl-2024.1/doc/misc.rst` & `pyopencl-2024.2/doc/misc.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/doc/runtime.rst` & `pyopencl-2024.2/doc/runtime.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/doc/runtime_const.rst` & `pyopencl-2024.2/doc/runtime_const.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/doc/runtime_gl.rst` & `pyopencl-2024.2/doc/runtime_gl.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/doc/runtime_memory.rst` & `pyopencl-2024.2/doc/runtime_memory.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/doc/runtime_platform.rst` & `pyopencl-2024.2/doc/runtime_platform.rst`

 * *Files 4% similar despite different names*

```diff
@@ -100,14 +100,16 @@
 
     .. method:: host_timer
 
         Only available with CL 2.0.
 
         .. versionadded:: 2020.3
 
+.. autofunction:: choose_devices
+
 Context
 -------
 
 .. class:: Context(devices=None, properties=None, dev_type=None, cache_dir=None)
 
     Create a new context. *properties* is a list of key-value
     tuples, where each key must be one of :class:`context_properties`.
@@ -118,17 +120,17 @@
     :attr:`device_type.DEFAULT` is created.
 
     If *cache_dir* is not *None* - it will be used as default *cache_dir*
     for all its' :class:`Program` instances builds (see also :meth:`Program.build`).
 
     .. note::
 
-        Calling the constructor with no arguments will fail for recent
-        CL drivers that support the OpenCL ICD. If you want similar,
-        just-give-me-a-context-already behavior, we recommend
+        Calling the constructor with no arguments will fail for
+        CL drivers that support the OpenCL ICD (which applies to most modern systems).
+        If you want similar, just-give-me-a-context-already behavior, we recommend
         :func:`create_some_context`. See, e.g. this
         `explanation by AMD
         <https://web.archive.org/web/20101114195033/https://developer.amd.com/support/KnowledgeBase/Lists/KnowledgeBase/DispForm.aspx?ID=71>`__.
 
     .. note::
 
         Because of how OpenCL changed in order to support Installable Client
@@ -175,17 +177,8 @@
     .. automethod:: from_int_ptr
     .. autoattribute:: int_ptr
 
     .. method:: set_default_device_command_queue(dev, queue)
 
     |comparable|
 
-.. function:: create_some_context(interactive=True, answers=None, cache_dir=None)
-
-    Create a :class:`Context` 'somehow'.
-
-    If multiple choices for platform and/or device exist, *interactive*
-    is True, and *sys.stdin.isatty()* is also True,
-    then the user is queried about which device should be chosen.
-    Otherwise, a device is chosen in an implementation-defined manner.
-
-
+.. autofunction:: create_some_context
```

### Comparing `pyopencl-2024.1/doc/runtime_program.rst` & `pyopencl-2024.2/doc/runtime_program.rst`

 * *Files 6% similar despite different names*

```diff
@@ -11,25 +11,31 @@
 .. envvar:: PYOPENCL_NO_CACHE
 
     By default, PyOpenCL will use cached (on disk) "binaries" returned by the
     OpenCL runtime when calling :meth:`Program.build` on a program
     constructed with source. (It will depend on the ICD in use how much
     compilation work is saved by this.)
     By setting the environment variable :envvar:`PYOPENCL_NO_CACHE` to any
-    non-empty value, this caching is suppressed. No additional in-memory
-    caching is performed. To retain the compiled version of a kernel
-    in memory, simply retain the :class:`Program` and/or :class:`Kernel`
-    objects.
+    string that :func:`pytools.strtobool` evaluates as ``True``, this caching
+    is suppressed. No additional in-memory caching is performed. To retain the
+    compiled version of a kernel in memory, simply retain the :class:`Program`
+    and/or :class:`Kernel` objects.
 
     PyOpenCL will also cache "invokers", which are short snippets of Python
     that are generated to accelerate passing arguments to and enqueuing
     a kernel.
 
     .. versionadded:: 2013.1
 
+.. envvar:: PYOPENCL_COMPILER_OUTPUT
+
+    When setting the environment variable :envvar:`PYOPENCL_COMPILER_OUTPUT`
+    to any string that :func:`pytools.strtobool` evaluates as ``True``,
+    PyOpenCL will show compiler messages emitted during program build.
+
 .. envvar:: PYOPENCL_BUILD_OPTIONS
 
     Any options found in the environment variable
     :envvar:`PYOPENCL_BUILD_OPTIONS` will be appended to *options*
     in :meth:`Program.build`.
 
     .. versionadded:: 2013.1
@@ -97,16 +103,16 @@
 
             prg.sum.set_args(a_g, b_g, res_g)
             ev = cl.enqueue_nd_range_kernel(queue, prg.sum, a_np.shape, None)
 
         Instead, either use the (recommended, stateless) calling interface::
 
             sum_knl = prg.sum
-            sum_knl(queue, a_np.shape, None, a_g, b_g, res_g)    
-            
+            sum_knl(queue, a_np.shape, None, a_g, b_g, res_g)
+
         or the long, stateful way around, if you prefer::
 
             sum_knl.set_args(a_g, b_g, res_g)
             ev = cl.enqueue_nd_range_kernel(queue, sum_knl, a_np.shape, None)
 
         The following will also work, however note that a number of caches that
         are important for efficient kernel enqueue are attached to the :class:`Kernel`
```

### Comparing `pyopencl-2024.1/doc/runtime_queue.rst` & `pyopencl-2024.2/doc/runtime_queue.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/doc/subst.rst` & `pyopencl-2024.2/doc/subst.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/doc/types.rst` & `pyopencl-2024.2/doc/types.rst`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/examples/black-hole-accretion.py` & `pyopencl-2024.2/examples/black-hole-accretion.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,21 +28,23 @@
 # - Pierre Lena for his passion about science and vulgarisation
 
 # If crash on OpenCL Intel implementation, add following options and force
 # export PYOPENCL_COMPILER_OUTPUT=1
 # export CL_CONFIG_USE_VECTORIZER=True
 # export CL_CONFIG_CPU_VECTORIZER_MODE=16
 
-import pyopencl as cl
-import numpy
-import time
-import sys
 import getopt
+import sys
+import time
 from socket import gethostname
 
+import numpy
+
+import pyopencl as cl
+
 
 def DictionariesAPI():
     PhysicsList = {"Einstein": 0, "Newton": 1}
     return PhysicsList
 
 
 #
```

### Comparing `pyopencl-2024.1/examples/demo-struct-reduce.py` & `pyopencl-2024.2/examples/demo-struct-reduce.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+
 import pyopencl as cl
 
 
 def make_collector_dtype(device):
     dtype = np.dtype([
         ("cur_min", np.int32),
         ("cur_max", np.int32),
@@ -51,18 +52,22 @@
             result.cur_max = b.cur_max;
         return result;
     }
 
     """
 
 from pyopencl.clrandom import rand as clrand
+
+
 a_gpu = clrand(queue, (20000,), dtype=np.int32, a=0, b=10**6)
 a = a_gpu.get()
 
 from pyopencl.reduction import ReductionKernel
+
+
 red = ReductionKernel(ctx, mmc_dtype,
         neutral="mmc_neutral()",
         reduce_expr="agg_mmc(a, b)", map_expr="mmc_from_scalar(x[i])",
         arguments="__global int *x", preamble=preamble)
 
 minmax = red(a_gpu).get()
```

### Comparing `pyopencl-2024.1/examples/demo_array.py` & `pyopencl-2024.2/examples/demo_array.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import numpy as np
+import numpy.linalg as la
+
 import pyopencl as cl
 import pyopencl.array as cl_array
-import numpy
-import numpy.linalg as la
 
-a = numpy.random.rand(50000).astype(numpy.float32)
-b = numpy.random.rand(50000).astype(numpy.float32)
+
+rng = np.random.default_rng()
+a = rng.random(50000, dtype=np.float32)
+b = rng.random(50000, dtype=np.float32)
 
 ctx = cl.create_some_context()
 queue = cl.CommandQueue(ctx)
 
 a_dev = cl_array.to_device(queue, a)
 b_dev = cl_array.to_device(queue, b)
 dest_dev = cl_array.empty_like(a_dev)
@@ -22,7 +25,8 @@
     }
     """).build()
 
 knl = prg.sum  # Use this Kernel object for repeated calls
 knl(queue, a.shape, None, a_dev.data, b_dev.data, dest_dev.data)
 
 print(la.norm((dest_dev - (a_dev+b_dev)).get()))
+assert np.allclose(dest_dev.get(), (a_dev + b_dev).get())
```

### Comparing `pyopencl-2024.1/examples/demo_array_svm.py` & `pyopencl-2024.2/examples/demo_array_svm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+import numpy as np
+
 import pyopencl as cl
 import pyopencl.array as cl_array
 from pyopencl.tools import SVMAllocator, SVMPool
-import numpy as np
+
 
 n = 50000
-a = np.random.rand(n).astype(np.float32)
-b = np.random.rand(n).astype(np.float32)
 
+rng = np.random.default_rng()
+a = rng.random(n, dtype=np.float32)
+b = rng.random(n, dtype=np.float32)
 
 ctx = cl.create_some_context()
 queue = cl.CommandQueue(ctx)
 
 alloc = SVMAllocator(ctx, alignment=0, queue=queue)
 alloc = SVMPool(alloc)
 
@@ -26,8 +29,9 @@
       c[gid] = a[gid] + b[gid];
     }
     """).build()
 
 knl = prg.sum
 knl(queue, a.shape, None, a_dev.data, b_dev.data, dest_dev.data)
 
-np.testing.assert_allclose(dest_dev.get(), (a_dev+b_dev).get())
+print(np.linalg.norm((dest_dev - (a_dev + b_dev)).get()))
+assert np.allclose(dest_dev.get(), (a_dev + b_dev).get())
```

### Comparing `pyopencl-2024.1/examples/demo_elementwise.py` & `pyopencl-2024.2/examples/demo_elementwise.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-#!/usr/bin/env python
-
 import numpy as np
+
 import pyopencl as cl
 import pyopencl.array
 from pyopencl.elementwise import ElementwiseKernel
 
+
 n = 10
-a_np = np.random.randn(n).astype(np.float32)
-b_np = np.random.randn(n).astype(np.float32)
+
+rng = np.random.default_rng()
+a_np = rng.random(n, dtype=np.float32)
+b_np = rng.random(n, dtype=np.float32)
 
 ctx = cl.create_some_context()
 queue = cl.CommandQueue(ctx)
 
 a_g = cl.array.to_device(queue, a_np)
 b_g = cl.array.to_device(queue, b_np)
```

### Comparing `pyopencl-2024.1/examples/demo_elementwise_complex.py` & `pyopencl-2024.2/examples/demo_elementwise_complex.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,28 @@
+import numpy as np
+import numpy.linalg as la
+
 import pyopencl as cl
 import pyopencl.array as cl_array
-import numpy
-import numpy.linalg as la
+from pyopencl.elementwise import ElementwiseKernel
+
 
 ctx = cl.create_some_context()
 queue = cl.CommandQueue(ctx)
 
 n = 10
+
+rng = np.random.default_rng()
 a_gpu = cl_array.to_device(queue,
-        (numpy.random.randn(n) + 1j*numpy.random.randn(n)).astype(numpy.complex64))
+        rng.standard_normal(n, dtype=np.float32)
+        + 1j*rng.standard_normal(n, dtype=np.float32))
 b_gpu = cl_array.to_device(queue,
-        (numpy.random.randn(n) + 1j*numpy.random.randn(n)).astype(numpy.complex64))
+        rng.standard_normal(n, dtype=np.float32)
+        + 1j*rng.standard_normal(n, dtype=np.float32))
 
-from pyopencl.elementwise import ElementwiseKernel
 complex_prod = ElementwiseKernel(ctx,
         "float a, "
         "cfloat_t *x, "
         "cfloat_t *y, "
         "cfloat_t *z",
         "z[i] = cfloat_rmul(a, cfloat_mul(x[i], y[i]))",
         "complex_prod",
@@ -35,13 +41,13 @@
         "z[i] = cfloat_real(x[i])",
         "real_part",
         preamble="#include <pyopencl-complex.h>")
 
 c_gpu = cl_array.empty_like(a_gpu)
 complex_prod(5, a_gpu, b_gpu, c_gpu)
 
-c_gpu_real = cl_array.empty(queue, len(a_gpu), dtype=numpy.float32)
+c_gpu_real = cl_array.empty(queue, len(a_gpu), dtype=np.float32)
 real_part(c_gpu, c_gpu_real)
 print(c_gpu.get().real - c_gpu_real.get())
 
 print(la.norm(c_gpu.get() - (5*a_gpu.get()*b_gpu.get())))
 assert la.norm(c_gpu.get() - (5*a_gpu.get()*b_gpu.get())) < 1e-5
```

### Comparing `pyopencl-2024.1/examples/demo_mandelbrot.py` & `pyopencl-2024.2/examples/demo_mandelbrot.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # Based on vegaseat's TKinter/numpy example code from 2006
 # http://www.daniweb.com/code/snippet216851.html#
 # with minor changes to move to numpy from the obsolete Numeric
 
 import time
 
 import numpy as np
+from PIL import Image
 
 import pyopencl as cl
 
-from PIL import Image
 
 # You can choose a calculation routine below (calc_fractal), uncomment
 # one of the three lines to test the three variations
 # Speed notes are listed in the same place
 
 # set width and height of window, more pixels take longer to calculate
 w = 2048
```

### Comparing `pyopencl-2024.1/examples/demo_meta_codepy.py` & `pyopencl-2024.2/examples/demo_meta_codepy.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-import pyopencl as cl
-import numpy
+import numpy as np
 import numpy.linalg as la
+from cgen import (
+    POD, Assign, Block, Const, FunctionBody, FunctionDeclaration, Initializer,
+    Module, Pointer, Value)
+from cgen.opencl import CLGlobal, CLKernel, CLRequiredWorkGroupSize
+
+import pyopencl as cl
+
 
 local_size = 256
 thread_strides = 32
 macroblock_count = 33
-dtype = numpy.float32
+dtype = np.float32
 total_size = local_size*thread_strides*macroblock_count
 
 ctx = cl.create_some_context()
 queue = cl.CommandQueue(ctx)
 
-a = numpy.random.randn(total_size).astype(dtype)
-b = numpy.random.randn(total_size).astype(dtype)
+rng = np.random.default_rng()
+a = rng.standard_normal(total_size, dtype=dtype)
+b = rng.standard_normal(total_size, dtype=dtype)
 
 mf = cl.mem_flags
 a_buf = cl.Buffer(ctx, mf.READ_ONLY | mf.COPY_HOST_PTR, hostbuf=a)
 b_buf = cl.Buffer(ctx, mf.READ_ONLY | mf.COPY_HOST_PTR, hostbuf=b)
 c_buf = cl.Buffer(ctx, mf.WRITE_ONLY, b.nbytes)
 
-from cgen import FunctionBody, \
-        FunctionDeclaration, POD, Value, \
-        Pointer, Module, Block, Initializer, Assign, Const
-from cgen.opencl import CLKernel, CLGlobal, \
-        CLRequiredWorkGroupSize
-
 mod = Module([
     FunctionBody(
         CLKernel(CLRequiredWorkGroupSize((local_size,),
             FunctionDeclaration(
             Value("void", "add"),
             arg_decls=[CLGlobal(Pointer(Const(POD(dtype, name))))
                 for name in ["tgt", "op1", "op2"]]))),
         Block([
-            Initializer(POD(numpy.int32, "idx"),
+            Initializer(POD(np.int32, "idx"),
                 "get_local_id(0) + %d * get_group_id(0)"
                 % (local_size*thread_strides))
             ]+[
             Assign(
                 "tgt[idx+%d]" % (o*local_size),
                 "op1[idx+%d] + op2[idx+%d]" % (
                     o*local_size,
@@ -45,11 +46,11 @@
             for o in range(thread_strides)]))])
 
 knl = cl.Program(ctx, str(mod)).build().add
 
 knl(queue, (local_size*macroblock_count,), (local_size,),
         c_buf, a_buf, b_buf)
 
-c = numpy.empty_like(a)
+c = np.empty_like(a)
 cl.enqueue_copy(queue, c, c_buf).wait()
 
 assert la.norm(c-(a+b)) == 0
```

### Comparing `pyopencl-2024.1/examples/demo_meta_template.py` & `pyopencl-2024.2/examples/demo_meta_template.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-import pyopencl as cl
-import numpy
+import numpy as np
 import numpy.linalg as la
+from mako.template import Template
+
+import pyopencl as cl
+
 
 local_size = 256
 thread_strides = 32
 macroblock_count = 33
-dtype = numpy.float32
+dtype = np.float32
 total_size = local_size*thread_strides*macroblock_count
 
 ctx = cl.create_some_context()
 queue = cl.CommandQueue(ctx)
 
-a = numpy.random.randn(total_size).astype(dtype)
-b = numpy.random.randn(total_size).astype(dtype)
+rng = np.random.default_rng()
+a = rng.standard_normal(total_size, dtype=dtype)
+b = rng.standard_normal(total_size, dtype=dtype)
 
 mf = cl.mem_flags
 a_buf = cl.Buffer(ctx, mf.READ_ONLY | mf.COPY_HOST_PTR, hostbuf=a)
 b_buf = cl.Buffer(ctx, mf.READ_ONLY | mf.COPY_HOST_PTR, hostbuf=b)
 c_buf = cl.Buffer(ctx, mf.WRITE_ONLY, b.nbytes)
 
-from mako.template import Template
-
 tpl = Template("""
     __kernel void add(
             __global ${ type_name } *tgt,
             __global const ${ type_name } *op1,
             __global const ${ type_name } *op2)
     {
       int idx = get_local_id(0)
@@ -43,11 +45,11 @@
     local_size=local_size, thread_strides=thread_strides)
 
 knl = cl.Program(ctx, str(rendered_tpl)).build().add
 
 knl(queue, (local_size*macroblock_count,), (local_size,),
         c_buf, a_buf, b_buf)
 
-c = numpy.empty_like(a)
+c = np.empty_like(a)
 cl.enqueue_copy(queue, c, c_buf).wait()
 
 assert la.norm(c-(a+b)) == 0
```

### Comparing `pyopencl-2024.1/examples/dump-performance.py` & `pyopencl-2024.2/examples/dump-performance.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/examples/dump-properties.py` & `pyopencl-2024.2/examples/dump-properties.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-import pyopencl as cl
 from optparse import OptionParser
 
+import pyopencl as cl
+
+
 parser = OptionParser()
 parser.add_option("-s", "--short", action="store_true",
                   help="don't print all device properties")
 
 (options, args) = parser.parse_args()
```

### Comparing `pyopencl-2024.1/examples/gl_interop_demo.py` & `pyopencl-2024.2/examples/gl_interop_demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from OpenGL.GL import *
 from OpenGL.GLUT import *
 from OpenGL.raw.GL.VERSION.GL_1_5 import glBufferData as rawGlBufferData
+
 import pyopencl as cl
 
 
 n_vertices = 10000
 
 src = """
 
@@ -19,16 +20,17 @@
 }
 
 """
 
 def initialize():
     platform = cl.get_platforms()[0]
 
-    from pyopencl.tools import get_gl_sharing_context_properties
     import sys
+
+    from pyopencl.tools import get_gl_sharing_context_properties
     if sys.platform == "darwin":
         ctx = cl.Context(properties=get_gl_sharing_context_properties(),
                 devices=[])
     else:
         # Some OSs prefer clCreateContextFromType, some prefer
         # clCreateContext. Try both.
         try:
```

### Comparing `pyopencl-2024.1/examples/gl_particle_animation.py` & `pyopencl-2024.2/examples/gl_particle_animation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,89 +1,98 @@
 # Visualization of particles with gravity
 # Source: http://enja.org/2010/08/27/adventures-in-opencl-part-2-particles-with-opengl/
 
-import pyopencl as cl  # OpenCL - GPU computing interface
+import sys
 
-mf = cl.mem_flags
-from pyopencl.tools import get_gl_sharing_context_properties
-from OpenGL.GL import *  # OpenGL - GPU rendering interface
-from OpenGL.GLU import *  # OpenGL tools (mipmaps, NURBS, perspective projection, shapes)
-from OpenGL.GLUT import *  # OpenGL tool to make a visualization window
+import numpy as np
+from OpenGL import GL, GLU, GLUT
 from OpenGL.arrays import vbo
-import numpy  # Number tools
-import sys  # System tools (path, modules, maxint)
+from OpenGL.GL import (
+    GL_ARRAY_BUFFER, GL_BLEND, GL_COLOR_ARRAY, GL_COLOR_BUFFER_BIT,
+    GL_DEPTH_BUFFER_BIT, GL_DYNAMIC_DRAW, GL_FLOAT, GL_MODELVIEW,
+    GL_ONE_MINUS_SRC_ALPHA, GL_POINT_SMOOTH, GL_POINTS, GL_PROJECTION, GL_SRC_ALPHA,
+    GL_VERTEX_ARRAY)
+from OpenGL.GLUT import GLUT_DEPTH, GLUT_DOUBLE, GLUT_RGBA
+
+import pyopencl as cl
+from pyopencl.tools import get_gl_sharing_context_properties
+
+
+mf = cl.mem_flags
 
 width = 800
 height = 600
 num_particles = 100000
 time_step = 0.005
 mouse_down = False
 mouse_old = {"x": 0.0, "y": 0.0}
 rotate = {"x": 0.0, "y": 0.0, "z": 0.0}
 translate = {"x": 0.0, "y": 0.0, "z": 0.0}
 initial_translate = {"x": 0.0, "y": 0.0, "z": -2.5}
 
 
 def glut_window():
-    glutInit(sys.argv)
-    glutInitDisplayMode(GLUT_RGBA | GLUT_DOUBLE | GLUT_DEPTH)
-    glutInitWindowSize(width, height)
-    glutInitWindowPosition(0, 0)
-    window = glutCreateWindow("Particle Simulation")
-
-    glutDisplayFunc(on_display)  # Called by GLUT every frame
-    glutKeyboardFunc(on_key)
-    glutMouseFunc(on_click)
-    glutMotionFunc(on_mouse_move)
-    glutTimerFunc(10, on_timer, 10)  # Call draw every 30 ms
-
-    glViewport(0, 0, width, height)
-    glMatrixMode(GL_PROJECTION)
-    glLoadIdentity()
-    gluPerspective(60.0, width / float(height), 0.1, 1000.0)
+    GLUT.glutInit(sys.argv)
+    GLUT.glutInitDisplayMode(GLUT_RGBA | GLUT_DOUBLE | GLUT_DEPTH)
+    GLUT.glutInitWindowSize(width, height)
+    GLUT.glutInitWindowPosition(0, 0)
+    window = GLUT.glutCreateWindow("Particle Simulation")
+
+    GLUT.glutDisplayFunc(on_display)  # Called by GLUT every frame
+    GLUT.glutKeyboardFunc(on_key)
+    GLUT.glutMouseFunc(on_click)
+    GLUT.glutMotionFunc(on_mouse_move)
+    GLUT.glutTimerFunc(10, on_timer, 10)  # Call draw every 30 ms
+
+    GL.glViewport(0, 0, width, height)
+    GL.glMatrixMode(GL_PROJECTION)
+    GL.glLoadIdentity()
+    GLU.gluPerspective(60.0, width / float(height), 0.1, 1000.0)
 
     return window
 
 
 def initial_buffers(num_particles):
-    np_position = numpy.ndarray((num_particles, 4), dtype=numpy.float32)
-    np_color = numpy.ndarray((num_particles, 4), dtype=numpy.float32)
-    np_velocity = numpy.ndarray((num_particles, 4), dtype=numpy.float32)
+    rng = np.random.default_rng()
+
+    np_position = np.empty((num_particles, 4), dtype=np.float32)
+    np_color = np.empty((num_particles, 4), dtype=np.float32)
+    np_velocity = np.empty((num_particles, 4), dtype=np.float32)
 
-    np_position[:, 0] = numpy.sin(
-        numpy.arange(0.0, num_particles) * 2.001 * numpy.pi / num_particles
+    np_position[:, 0] = np.sin(
+        np.arange(0.0, num_particles) * 2.001 * np.pi / num_particles
     )
-    np_position[:, 0] *= numpy.random.random_sample((num_particles,)) / 3.0 + 0.2
-    np_position[:, 1] = numpy.cos(
-        numpy.arange(0.0, num_particles) * 2.001 * numpy.pi / num_particles
+    np_position[:, 0] *= rng.integers(num_particles) / 3.0 + 0.2
+    np_position[:, 1] = np.cos(
+        np.arange(0.0, num_particles) * 2.001 * np.pi / num_particles
     )
-    np_position[:, 1] *= numpy.random.random_sample((num_particles,)) / 3.0 + 0.2
+    np_position[:, 1] *= rng.integers(num_particles) / 3.0 + 0.2
     np_position[:, 2] = 0.0
     np_position[:, 3] = 1.0
 
     np_color[:, :] = [1.0, 1.0, 1.0, 1.0]  # White particles
 
     np_velocity[:, 0] = np_position[:, 0] * 2.0
     np_velocity[:, 1] = np_position[:, 1] * 2.0
     np_velocity[:, 2] = 3.0
-    np_velocity[:, 3] = numpy.random.random_sample((num_particles,))
+    np_velocity[:, 3] = rng.integers(num_particles)
 
     gl_position = vbo.VBO(
         data=np_position, usage=GL_DYNAMIC_DRAW, target=GL_ARRAY_BUFFER
     )
     gl_position.bind()
     gl_color = vbo.VBO(data=np_color, usage=GL_DYNAMIC_DRAW, target=GL_ARRAY_BUFFER)
     gl_color.bind()
 
     return (np_position, np_velocity, gl_position, gl_color)
 
 
 def on_timer(t):
-    glutTimerFunc(t, on_timer, t)
-    glutPostRedisplay()
+    GLUT.glutTimerFunc(t, on_timer, t)
+    GLUT.glutPostRedisplay()
 
 
 def on_key(*args):
     if args[0] == "\033" or args[0] == "q":
         sys.exit()
 
 
@@ -106,54 +115,54 @@
     cl.enqueue_acquire_gl_objects(queue, [cl_gl_position, cl_gl_color])
     kernelargs = (
         cl_gl_position,
         cl_gl_color,
         cl_velocity,
         cl_start_position,
         cl_start_velocity,
-        numpy.float32(time_step),
+        np.float32(time_step),
     )
     program.particle_fountain(queue, (num_particles,), None, *(kernelargs))
     cl.enqueue_release_gl_objects(queue, [cl_gl_position, cl_gl_color])
     queue.finish()
-    glFlush()
+    GL.glFlush()
 
-    glClear(GL_COLOR_BUFFER_BIT | GL_DEPTH_BUFFER_BIT)
-    glMatrixMode(GL_MODELVIEW)
-    glLoadIdentity()
+    GL.glClear(GL_COLOR_BUFFER_BIT | GL_DEPTH_BUFFER_BIT)
+    GL.glMatrixMode(GL_MODELVIEW)
+    GL.glLoadIdentity()
 
     # Handle mouse transformations
-    glTranslatef(initial_translate["x"], initial_translate["y"], initial_translate["z"])
-    glRotatef(rotate["x"], 1, 0, 0)
-    glRotatef(rotate["y"], 0, 1, 0)  # we switched around the axis so make this rotate_z
-    glTranslatef(translate["x"], translate["y"], translate["z"])
+    GL.glTranslatef(initial_translate["x"], initial_translate["y"], initial_translate["z"])
+    GL.glRotatef(rotate["x"], 1, 0, 0)
+    GL.glRotatef(rotate["y"], 0, 1, 0)  # we switched around the axis so make this rotate_z
+    GL.glTranslatef(translate["x"], translate["y"], translate["z"])
 
     # Render the particles
-    glEnable(GL_POINT_SMOOTH)
-    glPointSize(2)
-    glEnable(GL_BLEND)
-    glBlendFunc(GL_SRC_ALPHA, GL_ONE_MINUS_SRC_ALPHA)
+    GL.glEnable(GL_POINT_SMOOTH)
+    GL.glPointSize(2)
+    GL.glEnable(GL_BLEND)
+    GL.glBlendFunc(GL_SRC_ALPHA, GL_ONE_MINUS_SRC_ALPHA)
 
     # Set up the VBOs
     gl_color.bind()
-    glColorPointer(4, GL_FLOAT, 0, gl_color)
+    GL.glColorPointer(4, GL_FLOAT, 0, gl_color)
     gl_position.bind()
-    glVertexPointer(4, GL_FLOAT, 0, gl_position)
-    glEnableClientState(GL_VERTEX_ARRAY)
-    glEnableClientState(GL_COLOR_ARRAY)
+    GL.glVertexPointer(4, GL_FLOAT, 0, gl_position)
+    GL.glEnableClientState(GL_VERTEX_ARRAY)
+    GL.glEnableClientState(GL_COLOR_ARRAY)
 
     # Draw the VBOs
-    glDrawArrays(GL_POINTS, 0, num_particles)
+    GL.glDrawArrays(GL_POINTS, 0, num_particles)
 
-    glDisableClientState(GL_COLOR_ARRAY)
-    glDisableClientState(GL_VERTEX_ARRAY)
+    GL.glDisableClientState(GL_COLOR_ARRAY)
+    GL.glDisableClientState(GL_VERTEX_ARRAY)
 
-    glDisable(GL_BLEND)
+    GL.glDisable(GL_BLEND)
 
-    glutSwapBuffers()
+    GLUT.glutSwapBuffers()
 
 
 window = glut_window()
 
 (np_position, np_velocity, gl_position, gl_color) = initial_buffers(num_particles)
 
 platform = cl.get_platforms()[0]
@@ -202,8 +211,8 @@
     position[i] = p;
     velocity[i] = v;
 
     color[i].w = life; /* Fade points as life decreases */
 }"""
 program = cl.Program(context, kernel).build()
 
-glutMainLoop()
+GLUT.glutMainLoop()
```

### Comparing `pyopencl-2024.1/examples/ipython-demo.ipynb` & `pyopencl-2024.2/examples/ipython-demo.ipynb`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/examples/median-filter.py` & `pyopencl-2024.2/examples/median-filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 from imageio import imread, imsave
 
 import pyopencl as cl
 
+
 # Read in image
 img = imread("noisyImage.jpg").astype(np.float32)
 print(img.shape)
 
 img = np.mean(img, axis=2)
 print(img.shape)
```

### Comparing `pyopencl-2024.1/examples/n-body.py` & `pyopencl-2024.2/examples/n-body.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 Thanks to Andreas Klockner for PyOpenCL:
 http://mathema.tician.de/software/pyopencl
 
 """
 import getopt
 import sys
 import time
+
 import numpy as np
+
 import pyopencl as cl
 import pyopencl.array
-from numpy.random import randint as nprnd
 
 
 def DictionariesAPI():
     Marsaglia = {"CONG": 0, "SHR3": 1, "MWC": 2, "KISS": 3}
     Computing = {"FP32": 0, "FP64": 1}
     Interaction = {"Force": 0, "Potential": 1}
     Artevasion = {"None": 0, "NegExp": 1, "CorRad": 2}
@@ -867,16 +868,17 @@
     # clKinetic = cl.Buffer(ctx, mf.WRITE_ONLY|mf.COPY_HOST_PTR,hostbuf=MyKinetic)
     # clCoM = cl.Buffer(ctx, mf.WRITE_ONLY|mf.COPY_HOST_PTR,hostbuf=MyCoM)
 
     print("All particles superimposed.")
 
     # Set particles to RNG points
     if InitialRandom:
-        seed_w = np.uint32(nprnd(2 ** 32))
-        seed_z = np.uint32(nprnd(2 ** 32))
+        rng = np.random.default_rng()
+        seed_w = np.uint32(rng.integers(2 ** 32))
+        seed_z = np.uint32(rng.integers(2 ** 32))
     else:
         seed_w = np.uint32(19710211)
         seed_z = np.uint32(20081010)
 
     if Shape == "Ball":
         MyRoutines.InBallSplutterPoints(
             queue, (Number, 1), None, clDataX, SizeOfShape, seed_w, seed_z
```

### Comparing `pyopencl-2024.1/examples/narray.py` & `pyopencl-2024.2/examples/narray.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # example by Roger Pau Monn'e
-import pyopencl as cl
 import numpy as np
 
+import pyopencl as cl
+
+
 demo_r = np.empty((500, 5), dtype=np.uint32)
 ctx = cl.create_some_context()
 queue = cl.CommandQueue(ctx)
 
 mf = cl.mem_flags
 demo_buf = cl.Buffer(ctx, mf.WRITE_ONLY, demo_r.nbytes)
```

### Comparing `pyopencl-2024.1/examples/noisyImage.jpg` & `pyopencl-2024.2/examples/noisyImage.jpg`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/examples/pi-monte-carlo.py` & `pyopencl-2024.2/examples/pi-monte-carlo.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,22 +19,23 @@
 # http://mathema.tician.de/software/pyopencl
 #
 
 # 2013-01-01 : problems with launch timeout
 # http://stackoverflow.com/questions/497685/how-do-you-get-around-the-maximum-cuda-run-time
 # Option "Interactive" "0" in /etc/X11/xorg.conf
 
-# Common tools
-import numpy
-import sys
 import getopt
-import time
 import itertools
+import sys
+import time
 from socket import gethostname
 
+# Common tools
+import numpy
+
 
 class PenStacle:
     """Pentacle of Statistics from data"""
 
     Avg = 0
     Med = 0
     Std = 0
@@ -649,16 +650,16 @@
     }
     # print(OutputCL)
     return OutputCL
 
 
 def FitAndPrint(N, D, Curves):
 
-    from scipy.optimize import curve_fit
     import matplotlib.pyplot as plt
+    from scipy.optimize import curve_fit
 
     try:
         coeffs_Amdahl, matcov_Amdahl = curve_fit(Amdahl, N, D)
 
         D_Amdahl = Amdahl(N, coeffs_Amdahl[0], coeffs_Amdahl[1], coeffs_Amdahl[2])
         coeffs_Amdahl[1] = coeffs_Amdahl[1] * coeffs_Amdahl[0] / D[0]
         coeffs_Amdahl[2] = coeffs_Amdahl[2] * coeffs_Amdahl[0] / D[0]
```

### Comparing `pyopencl-2024.1/examples/svm.py` & `pyopencl-2024.2/examples/svm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python
 
-from pyopencl.characterize import (has_coarse_grain_buffer_svm,
-                                   has_fine_grain_buffer_svm,
-                                   has_fine_grain_system_svm)
 import numpy as np
+
 import pyopencl as cl
+from pyopencl.characterize import (
+    has_coarse_grain_buffer_svm, has_fine_grain_buffer_svm,
+    has_fine_grain_system_svm)
+
 
 ctx = cl.create_some_context()
 queue = cl.CommandQueue(ctx)
 
 dev = queue.device
 
 print(
```

### Comparing `pyopencl-2024.1/examples/transpose.py` & `pyopencl-2024.2/examples/transpose.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Transposition of a matrix
 # originally for PyCUDA by Hendrik Riedmann <riedmann@dam.brown.edu>
 
-import pyopencl as cl
-import numpy
+import numpy as np
 import numpy.linalg as la
 
+import pyopencl as cl
+
 
 block_size = 16
 
 
 class NaiveTranspose:
     def __init__(self, ctx):
         self.kernel = (
@@ -36,27 +37,27 @@
 
         return self.kernel(
             queue,
             (w, h),
             (block_size, block_size),
             tgt,
             src,
-            numpy.uint32(w),
-            numpy.uint32(h),
+            np.uint32(w),
+            np.uint32(h),
         )
 
 
 class SillyTranspose(NaiveTranspose):
     def __call__(self, queue, tgt, src, shape):
         w, h = shape
         assert w % block_size == 0
         assert h % block_size == 0
 
         return self.kernel(
-            queue, (w, h), None, tgt, src, numpy.uint32(w), numpy.uint32(h)
+            queue, (w, h), None, tgt, src, np.uint32(w), np.uint32(h)
         )
 
 
 class TransposeWithLocal:
     def __init__(self, ctx):
         self.kernel = (
             cl.Program(
@@ -104,28 +105,28 @@
 
         return self.kernel(
             queue,
             (w, h),
             (block_size, block_size),
             tgt,
             src,
-            numpy.uint32(w),
-            numpy.uint32(h),
+            np.uint32(w),
+            np.uint32(h),
             cl.LocalMemory(4 * block_size * (block_size + 1)),
         )
 
 
 def transpose_using_cl(ctx, queue, cpu_src, cls):
     mf = cl.mem_flags
     a_buf = cl.Buffer(ctx, mf.READ_ONLY | mf.COPY_HOST_PTR, hostbuf=cpu_src)
     a_t_buf = cl.Buffer(ctx, mf.WRITE_ONLY, size=cpu_src.nbytes)
     cls(ctx)(queue, a_t_buf, a_buf, cpu_src.shape)
 
     w, h = cpu_src.shape
-    result = numpy.empty((h, w), dtype=cpu_src.dtype)
+    result = np.empty((h, w), dtype=cpu_src.dtype)
     cl.enqueue_copy(queue, result, a_t_buf).wait()
 
     a_buf.release()
     a_t_buf.release()
 
     return result
 
@@ -136,19 +137,20 @@
         ctx = cl.create_some_context()
 
         for dev in ctx.devices:
             assert dev.local_mem_size > 0
 
         queue = cl.CommandQueue(ctx)
 
-        for i in numpy.arange(10, 13, 0.125):
+        for i in np.arange(10, 13, 0.125):
             size = int(((2 ** i) // 32) * 32)
             print(size)
 
-            source = numpy.random.rand(size, size).astype(numpy.float32)
+            rng = np.random.default_rng()
+            source = rng.random((size, size), dtype=np.float32)
             result = transpose_using_cl(ctx, queue, source, NaiveTranspose)
 
             err = source.T - result
             err_norm = la.norm(err)
 
             assert err_norm == 0, (size, err_norm)
 
@@ -159,28 +161,28 @@
     for dev in ctx.devices:
         assert dev.local_mem_size > 0
 
     queue = cl.CommandQueue(
         ctx, properties=cl.command_queue_properties.PROFILING_ENABLE
     )
 
-    sizes = [int(((2 ** i) // 32) * 32) for i in numpy.arange(10, 13, 0.125)]
-    # for i in numpy.arange(10, 10.5, 0.125)]
+    sizes = [int(((2 ** i) // 32) * 32) for i in np.arange(10, 13, 0.125)]
+    # for i in np.arange(10, 10.5, 0.125)]
 
     mem_bandwidths = {}
 
     methods = [SillyTranspose, NaiveTranspose, TransposeWithLocal]
     for cls in methods:
         name = cls.__name__.replace("Transpose", "")
 
         mem_bandwidths[cls] = meth_mem_bws = []
 
         for size in sizes:
-
-            source = numpy.random.rand(size, size).astype(numpy.float32)
+            rng = np.random.default_rng()
+            source = rng.random((size, size), dtype=np.float32)
 
             mf = cl.mem_flags
             a_buf = cl.Buffer(ctx, mf.READ_ONLY | mf.COPY_HOST_PTR, hostbuf=source)
             a_t_buf = cl.Buffer(ctx, mf.WRITE_ONLY, size=source.nbytes)
             method = cls(ctx)
 
             for _i in range(4):
@@ -199,31 +201,24 @@
             meth_mem_bws.append(mem_bw)
 
             a_buf.release()
             a_t_buf.release()
 
     try:
         from matplotlib.pyplot import (
-            clf,
-            plot,
-            xlabel,
-            ylabel,
-            savefig,
-            legend,
-            grid,
-        )
+            clf, grid, legend, plot, savefig, xlabel, ylabel)
     except ModuleNotFoundError:
         pass
     else:
         for i in range(len(methods)):
             clf()
             for j in range(i + 1):
                 method = methods[j]
                 name = method.__name__.replace("Transpose", "")
-                plot(sizes, numpy.array(mem_bandwidths[method]) / 1e9, "o-",
+                plot(sizes, np.array(mem_bandwidths[method]) / 1e9, "o-",
                         label=name)
 
             xlabel("Matrix width/height $N$")
             ylabel("Memory Bandwidth [GB/s]")
             legend(loc="best")
             grid()
```

### Comparing `pyopencl-2024.1/pyopencl/__init__.py` & `pyopencl-2024.2/pyopencl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,45 +16,47 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
+import logging
 from sys import intern
-from warnings import warn
 from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
-
-from pyopencl.version import VERSION, VERSION_STATUS, VERSION_TEXT  # noqa: F401
+from warnings import warn
 
 # must import, otherwise dtype registry will not be fully populated
 import pyopencl.cltypes  # noqa: F401
+from pyopencl.version import VERSION, VERSION_STATUS, VERSION_TEXT  # noqa: F401
+
 
-import logging
 logger = logging.getLogger(__name__)
 
 # This supports ocl-icd find shipped OpenCL ICDs, cf.
 # https://github.com/isuruf/ocl-icd/commit/3862386b51930f95d9ad1089f7157a98165d5a6b
 # via
 # https://github.com/inducer/pyopencl/blob/0b3d0ef92497e6838eea300b974f385f94cb5100/scripts/build-wheels.sh#L43-L44
 import os
+
+
 os.environ["PYOPENCL_HOME"] = os.path.dirname(os.path.abspath(__file__))
 
 try:
     import pyopencl._cl as _cl
 except ImportError:
     from os.path import dirname, join, realpath
     if realpath(join(os.getcwd(), "pyopencl")) == realpath(dirname(__file__)):
         warn(
             "It looks like you are importing PyOpenCL from "
             "its source directory. This likely won't work.",
             stacklevel=2)
     raise
 
-import numpy as np
+import numpy as np  # noqa: I003
 
 import sys
 
 _PYPY = "__pypy__" in sys.builtin_module_names
 
 from pyopencl._cl import (  # noqa: F401
         get_cl_header_version,
@@ -164,78 +166,56 @@
         Sampler,
 
         # This class is available unconditionally, even though CL only
         # has it on CL2.0 and newer.
         Pipe,
         )
 
+
 try:
     from pyopencl._cl import DeviceTopologyAmd  # noqa: F401
     from pyopencl._cl import enqueue_copy_buffer_p2p_amd  # noqa: F401
 except ImportError:
     pass
 
 if not _PYPY:
     # FIXME: Add back to default set when pypy support catches up
-    from pyopencl._cl import (  # noqa: F401
-        enqueue_map_buffer,
-        enqueue_map_image,
-        )
+    from pyopencl._cl import enqueue_map_buffer  # noqa: F401
+    from pyopencl._cl import enqueue_map_image  # noqa: F401
 
 if get_cl_header_version() >= (1, 1):
-    from pyopencl._cl import (  # noqa: F401
-        UserEvent,
-        )
+    from pyopencl._cl import UserEvent  # noqa: F401
 if get_cl_header_version() >= (1, 2):
+    from pyopencl._cl import ImageDescriptor  # noqa: F401
     from pyopencl._cl import (  # noqa: F401
-        _enqueue_marker_with_wait_list,
-        _enqueue_barrier_with_wait_list,
-
-        unload_platform_compiler,
-
-
-        enqueue_migrate_mem_objects,
-        _enqueue_fill_buffer,
-        enqueue_fill_image,
-
-        ImageDescriptor,
-        )
+        _enqueue_barrier_with_wait_list, _enqueue_fill_buffer,
+        _enqueue_marker_with_wait_list, enqueue_fill_image,
+        enqueue_migrate_mem_objects, unload_platform_compiler)
 
 if get_cl_header_version() >= (2, 0):
-    from pyopencl._cl import (  # noqa: F401
-        SVMPointer,
-        SVM,
-        SVMAllocation,
-        )
+    from pyopencl._cl import SVM, SVMAllocation, SVMPointer  # noqa: F401
 
 if _cl.have_gl():
     from pyopencl._cl import (  # noqa: F401
-        gl_object_type,
-        gl_texture_info,
-
-        GLBuffer,
-        GLRenderBuffer,
-        GLTexture,
-        )
+        GLBuffer, GLRenderBuffer, GLTexture, gl_object_type, gl_texture_info)
 
     try:
         from pyopencl._cl import get_apple_cgl_share_group  # noqa: F401
     except ImportError:
         pass
 
     try:
-        from pyopencl._cl import (  # noqa: F401
-            enqueue_acquire_gl_objects,
-            enqueue_release_gl_objects,
-        )
+        from pyopencl._cl import enqueue_acquire_gl_objects  # noqa: F401
+        from pyopencl._cl import enqueue_release_gl_objects  # noqa: F401
     except ImportError:
         pass
 
 import inspect as _inspect
 
+
 CONSTANT_CLASSES = tuple(
         getattr(_cl, name) for name in dir(_cl)
         if _inspect.isclass(getattr(_cl, name))
         and name[0].islower() and name not in ["zip", "map", "range"])
 
 BITFIELD_CONSTANT_CLASSES = (
         _cl.device_type,
@@ -262,42 +242,43 @@
     pass
 
 
 class CommandQueueUsedAfterExit(UserWarning):
     pass
 
 
-def compiler_output(text):
-    if int(os.environ.get("PYOPENCL_COMPILER_OUTPUT", "0")):
+def compiler_output(text: str) -> None:
+    from pytools import strtobool
+    if strtobool(os.environ.get("PYOPENCL_COMPILER_OUTPUT", "False")):
         warn(text, CompilerWarning, stacklevel=3)
     else:
         warn("Non-empty compiler output encountered. Set the "
                 "environment variable PYOPENCL_COMPILER_OUTPUT=1 "
                 "to see more.", CompilerWarning, stacklevel=3)
 
 # }}}
 
 
 # {{{ find pyopencl shipped source code
 
-def _find_pyopencl_include_path():
-    from os.path import join, abspath, dirname, exists
-    try:
-        # Try to find the include path in the same directory as this file
-        include_path = join(abspath(dirname(__file__)), "cl")
-        if not exists(include_path):
-            raise OSError("unable to find pyopencl include path")
-    except Exception:
-        # Try to find the resource with pkg_resources (the recommended
-        # setuptools approach). This is very slow.
-        from pkg_resources import Requirement, resource_filename
-        include_path = resource_filename(
-                Requirement.parse("pyopencl"), "pyopencl/cl")
+def _find_pyopencl_include_path() -> str:
+    from os.path import abspath, dirname, exists, join
+
+    # Try to find the include path in the same directory as this file
+    include_path = join(abspath(dirname(__file__)), "cl")
+    if not exists(include_path):
+        try:
+            # NOTE: only available in Python >=3.9
+            from importlib.resources import files
+        except ImportError:
+            from importlib_resources import files
+
+        include_path = str(files("pyopencl") / "cl")
         if not exists(include_path):
-            raise OSError("unable to find pyopencl include path")
+            raise OSError("Unable to find PyOpenCL include path")
 
     # Quote the path if it contains a space and is not quoted already.
     # See https://github.com/inducer/pyopencl/issues/250 for discussion.
     if " " in include_path and not include_path.startswith('"'):
         return '"' + include_path + '"'
     else:
         return include_path
@@ -306,17 +287,14 @@
 
 
 # {{{ build option munging
 
 def _split_options_if_necessary(options):
     if isinstance(options, str):
         import shlex
-        # shlex.split takes unicode (py3 str) on py3
-        if isinstance(options, bytes):
-            options = options.decode("utf-8")
 
         options = shlex.split(options)
 
     return options
 
 
 def _find_include_path(options):
@@ -358,15 +336,18 @@
 
 
 # }}}
 
 
 # {{{ Program (wrapper around _Program, adds caching support)
 
-_PYOPENCL_NO_CACHE: bool = "PYOPENCL_NO_CACHE" in os.environ
+from pytools import strtobool
+
+
+_PYOPENCL_NO_CACHE = strtobool(os.environ.get("PYOPENCL_NO_CACHE", "false"))
 
 _DEFAULT_BUILD_OPTIONS: List[str] = []
 _DEFAULT_INCLUDE_OPTIONS: List[str] = ["-I", _find_pyopencl_include_path()]
 
 # map of platform.name to build options list
 _PLAT_BUILD_OPTIONS: Dict[str, List[str]] = {
         "Oclgrind": ["-D", "PYOPENCL_USING_OCLGRIND"],
@@ -550,15 +531,15 @@
         self._build_duration_info = (build_descr, was_cached, end_time-start_time)
 
         return self
 
     def _build_and_catch_errors(self, build_func, options_bytes, source=None):
         try:
             return build_func()
-        except _cl.RuntimeError as e:
+        except RuntimeError as e:
             msg = str(e)
             if options_bytes:
                 msg = msg + "\n(options: %s)" % options_bytes.decode("utf-8")
 
             if source is not None:
                 from tempfile import NamedTemporaryFile
                 srcfile = NamedTemporaryFile(mode="wt", delete=False, suffix=".cl")
@@ -568,15 +549,15 @@
                     srcfile.close()
 
                 msg = msg + "\n(source saved as %s)" % srcfile.name
 
             code = e.code
             routine = e.routine
 
-            err = _cl.RuntimeError(
+            err = RuntimeError(
                     _cl._ErrorRecord(
                         msg=msg,
                         code=code,
                         routine=routine))
 
         # Python 3.2 outputs the whole list of currently active exceptions
         # This serves to remove one (redundant) level from that nesting.
@@ -850,37 +831,23 @@
                 work_around_arg_count_bug = single_valued(count_bug_per_dev)
             else:
                 warn_about_arg_count_bug = True
 
         # }}}
 
         from pyopencl.invoker import generate_enqueue_and_set_args
-        enqueue, my_set_args = \
+        self._enqueue, self.set_args = \
                 generate_enqueue_and_set_args(
                         self.function_name,
                         len(arg_types), self.num_args,
                         arg_types,
                         warn_about_arg_count_bug=warn_about_arg_count_bug,
                         work_around_arg_count_bug=work_around_arg_count_bug,
                         devs=self.context.devices)
 
-        # Make ourselves a kernel-specific class, so that we're able to override
-        # __call__. Inspired by https://stackoverflow.com/a/38541437
-        class KernelWithCustomEnqueue(type(self)):
-            __call__ = enqueue
-            set_args = my_set_args
-
-        try:
-            self.__class__ = KernelWithCustomEnqueue
-        except TypeError:
-            # __class__ assignment may not work in all cases, due to differing
-            # object layouts. Fall back to bouncing through kernel_call below.
-            self._enqueue = enqueue
-            self.set_args = my_set_args
-
     def kernel_get_work_group_info(self, param, device):
         cache_key = (param, device.int_ptr)
         try:
             return self._wg_info_cache[cache_key]
         except KeyError:
             pass
 
@@ -1551,25 +1518,40 @@
             self.__array_interface__ = _interface
 
 # }}}
 
 
 # {{{ create_some_context
 
-def create_some_context(interactive=None, answers=None):
+def choose_devices(interactive: Optional[bool] = None,
+                   answers: Optional[List[str]] = None) -> List[Device]:
+    """
+    Choose :class:`Device` instances 'somehow'.
+
+    :arg interactive: If multiple choices for platform and/or device exist,
+        *interactive* is ``True`` (or ``None`` and ``sys.stdin.isatty()``
+        returns ``True``), then the user is queried about which device should be
+        chosen. Otherwise, a device is chosen in an implementation-defined
+        manner.
+    :arg answers: A sequence of strings that will be used to answer the
+        platform/device selection questions.
+
+    :returns: a list of :class:`Device` instances.
+    """
+
     if answers is None:
         if "PYOPENCL_CTX" in os.environ:
             ctx_spec = os.environ["PYOPENCL_CTX"]
             answers = ctx_spec.split(":")
 
         if "PYOPENCL_TEST" in os.environ:
             from pyopencl.tools import get_test_platforms_and_devices
             for _plat, devs in get_test_platforms_and_devices():
                 for dev in devs:
-                    return Context([dev])
+                    return [dev]
 
     if answers is not None:
         pre_provided_answers = answers
         answers = answers[:]
     else:
         pre_provided_answers = None
 
@@ -1673,15 +1655,35 @@
         if pre_provided_answers is not None:
             user_inputs = pre_provided_answers + user_inputs
         cc_print("Set the environment variable PYOPENCL_CTX='%s' to "
                 "avoid being asked again." % ":".join(user_inputs))
 
     if answers:
         raise RuntimeError("not all provided choices were used by "
-                "create_some_context. (left over: '%s')" % ":".join(answers))
+                "choose_device. (left over: '%s')" % ":".join(answers))
+
+    return devices
+
+
+def create_some_context(interactive: Optional[bool] = None,
+                        answers: Optional[List[str]] = None) -> Context:
+    """
+    Create a :class:`Context` 'somehow'.
+
+    :arg interactive: If multiple choices for platform and/or device exist,
+        *interactive* is ``True`` (or ``None`` and ``sys.stdin.isatty()``
+        returns ``True``), then the user is queried about which device should be
+        chosen. Otherwise, a device is chosen in an implementation-defined
+        manner.
+    :arg answers: A sequence of strings that will be used to answer the
+        platform/device selection questions.
+
+    :returns: an instance of :class:`Context`.
+    """
+    devices = choose_devices(interactive, answers)
 
     return Context(devices)
 
 
 _csc = create_some_context
 
 # }}}
```

### Comparing `pyopencl-2024.1/pyopencl/_cluda.py` & `pyopencl-2024.2/pyopencl/_cluda.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/pyopencl/_mymako.py` & `pyopencl-2024.2/pyopencl/_mymako.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/pyopencl/algorithm.py` & `pyopencl-2024.2/pyopencl/algorithm.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,32 +29,30 @@
 OTHER DEALINGS IN THE SOFTWARE.
 """
 
 from dataclasses import dataclass
 from typing import Optional
 
 import numpy as np
+from mako.template import Template
+from pytools import memoize, memoize_method
 
 import pyopencl as cl
 import pyopencl.array
-
 from pyopencl.elementwise import ElementwiseKernel
-from pyopencl.scan import ScanTemplate, GenericScanKernel
+from pyopencl.scan import GenericScanKernel, ScanTemplate
 from pyopencl.tools import dtype_to_ctype, get_arg_offset_adjuster_code
 
-from pytools import memoize, memoize_method
-from mako.template import Template
-
 
 # {{{ "extra args" handling utility
 
 def _extract_extra_args_types_values(extra_args):
     if extra_args is None:
         extra_args = []
-    from pyopencl.tools import VectorArg, ScalarArg
+    from pyopencl.tools import ScalarArg, VectorArg
 
     extra_args_types = []
     extra_args_values = []
     extra_wait_for = []
     for name, val in extra_args:
         if isinstance(val, cl.array.Array):
             extra_args_types.append(VectorArg(val.dtype, name, with_offset=False))
@@ -465,15 +463,15 @@
         # }}}
 
         # {{{ kernel creation
 
         scan_ctype, scan_dtype, scan_t_cdecl = \
                 _make_sort_scan_type(context.devices[0], self.bits, self.index_dtype)
 
-        from pyopencl.tools import VectorArg, ScalarArg
+        from pyopencl.tools import ScalarArg, VectorArg
         scan_arguments = (
                 list(self.arguments)
                 + [VectorArg(arg.dtype, "sorted_"+arg.name) for arg in self.arguments
                     if arg.name in sort_arg_names]
                 + [ScalarArg(np.int32, "base_bit")])
 
         def get_count_branch(known_bits):
@@ -923,15 +921,15 @@
         return (self.complex_kernel
                 and any(dev.type & cl.device_type.CPU
                     for dev in self.context.devices))
 
     @memoize_method
     def get_count_kernel(self, index_dtype):
         index_ctype = dtype_to_ctype(index_dtype)
-        from pyopencl.tools import VectorArg, OtherArg
+        from pyopencl.tools import OtherArg, VectorArg
         kernel_list_args = [
                 VectorArg(index_dtype, "plb_%s_count" % name)
                 for name, dtype in self.list_names_and_dtypes
                 if name not in self.count_sharing]
 
         user_list_args = []
         for name, _dtype in self.list_names_and_dtypes:
@@ -982,15 +980,15 @@
             kernel_list_args+self.arg_decls) + [index_dtype])
 
         return knl
 
     @memoize_method
     def get_write_kernel(self, index_dtype):
         index_ctype = dtype_to_ctype(index_dtype)
-        from pyopencl.tools import VectorArg, OtherArg
+        from pyopencl.tools import OtherArg, VectorArg
         kernel_list_args = []
         kernel_list_arg_values = ""
         user_list_args = []
 
         for name, dtype in self.list_names_and_dtypes:
             list_name = "plb_%s_list" % name
             list_arg = VectorArg(dtype, list_name)
@@ -1365,15 +1363,15 @@
     """
 
     def __init__(self, context):
         self.context = context
 
     @memoize_method
     def get_kernels(self, key_dtype, value_dtype, starts_dtype):
-        from pyopencl.tools import VectorArg, ScalarArg
+        from pyopencl.tools import ScalarArg, VectorArg
 
         by_target_sorter = RadixSort(
                 self.context, [
                     VectorArg(value_dtype, "values"),
                     VectorArg(key_dtype, "keys"),
                     ],
                 key_expr="keys[i]",
```

### Comparing `pyopencl-2024.1/pyopencl/array.py` & `pyopencl-2024.2/pyopencl/array.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,40 +26,42 @@
 WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 """
 
 import builtins
 from dataclasses import dataclass
-from warnings import warn
-from numbers import Number
 from functools import reduce
+from numbers import Number
 from typing import Any, Dict, Hashable, List, Optional, Tuple, Union
+from warnings import warn
 
 import numpy as np
-import pyopencl.elementwise as elementwise
 
 import pyopencl as cl
-from pyopencl.compyte.array import (
-        as_strided as _as_strided,
-        f_contiguous_strides as _f_contiguous_strides,
-        c_contiguous_strides as _c_contiguous_strides,
-        equal_strides as _equal_strides,
-        ArrayFlags as _ArrayFlags)
-from pyopencl.characterize import has_double_support
+import pyopencl.elementwise as elementwise
 from pyopencl import cltypes
+from pyopencl.characterize import has_double_support
+from pyopencl.compyte.array import (
+    ArrayFlags as _ArrayFlags, as_strided as _as_strided,
+    c_contiguous_strides as _c_contiguous_strides, equal_strides as _equal_strides,
+    f_contiguous_strides as _f_contiguous_strides)
+
 
 SCALAR_CLASSES = (Number, np.bool_, bool)
 
 if cl.get_cl_header_version() >= (2, 0):
     _SVMPointer_or_nothing = cl.SVMPointer
 else:
     _SVMPointer_or_nothing = ()
 
 
+_NUMPY_PRE_2 = np.__version__.startswith("1.")
+
+
 # {{{ _get_common_dtype
 
 _COMMON_DTYPE_CACHE: Dict[Tuple[Hashable, ...], np.dtype] = {}
 
 
 class DoubleDowncastWarning(UserWarning):
     pass
@@ -119,15 +121,17 @@
     # dtype('int32')
     # >>> (a + np.int32(1234)).dtype
     # dtype('int16')
     #
     # Note that np.find_common_type, while appealing, won't be able to tell
     # the full story.
 
-    if not (o1_is_array and o2_is_array) and o1_is_integral and o2_is_integral:
+    if (_NUMPY_PRE_2
+            and not (o1_is_array and o2_is_array)
+            and o1_is_integral and o2_is_integral):
         if o1_is_array:
             obj1 = np.zeros(1, dtype=o1_dtype)
         if o2_is_array:
             obj2 = np.zeros(1, dtype=o2_dtype)
 
         result = (obj1 + obj2).dtype
     else:
@@ -1409,15 +1413,15 @@
             return NotImplemented
 
     __rtruediv__ = __rdiv__
 
     def __itruediv__(self, other):
         # raise an error if the result cannot be cast to self
         common_dtype = _get_truedivide_dtype(self, other, self.queue)
-        if not np.can_cast(common_dtype, self.dtype.type):
+        if not np.can_cast(common_dtype, self.dtype.type, "same_kind"):
             raise TypeError(
                 "Cannot cast {!r} to {!r}".format(self.dtype, common_dtype))
 
         if isinstance(other, Array):
             if other.shape != self.shape and other.shape != ():
                 raise NotImplementedError("Broadcasting binary op with shapes:"
                                           f" {self.shape}, {other.shape}.")
```

### Comparing `pyopencl-2024.1/pyopencl/bitonic_sort.py` & `pyopencl-2024.2/pyopencl/bitonic_sort.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,22 +29,23 @@
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
 HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
 LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
 OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 
-import pyopencl as cl
-from pyopencl.tools import dtype_to_ctype
-from operator import mul
 from functools import reduce
-from pytools import memoize_method
+from operator import mul
+
 from mako.template import Template
+from pytools import memoize_method
 
+import pyopencl as cl
 import pyopencl.bitonic_sort_templates as _tmpl
+from pyopencl.tools import dtype_to_ctype
 
 
 def _is_power_of_2(n):
     from pyopencl.tools import bitlog2
     return n == 0 or 2**bitlog2(n) == n
```

### Comparing `pyopencl-2024.1/pyopencl/bitonic_sort_templates.py` & `pyopencl-2024.2/pyopencl/bitonic_sort_templates.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/pyopencl/cache.py` & `pyopencl-2024.2/pyopencl/cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,32 +19,35 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
-import re
+import logging
 import os
+import re
 import sys
 from dataclasses import dataclass
 from typing import List, Optional, Tuple
 
 import pyopencl._cl as _cl
 
-import logging
+
 logger = logging.getLogger(__name__)
 
 
 import hashlib
+
+
 new_hash = hashlib.md5
 
 
 def _erase_dir(dir):
-    from os import listdir, unlink, rmdir
+    from os import listdir, rmdir, unlink
     from os.path import join
     for name in listdir(dir):
         unlink(join(dir, name))
     rmdir(dir)
 
 
 def update_checksum(checksum, obj):
@@ -164,15 +167,15 @@
 C_INCLUDE_RE = re.compile(r'^\s*\#\s*include\s+[<"](.+)[">]\s*$',
         re.MULTILINE)
 
 
 def get_dependencies(src, include_path):
     result = {}
 
-    from os.path import realpath, join
+    from os.path import join, realpath
 
     def _inner(src):
         for match in C_INCLUDE_RE.finditer(src):
             included = match.group(1)
 
             found = False
             for ipath in include_path:
@@ -185,15 +188,15 @@
                         continue
 
                     try:
                         included_src = src_file.read()
                     finally:
                         src_file.close()
 
-                    # jrevent infinite recursion if some header file appears to
+                    # prevent infinite recursion if some header file appears to
                     # include itself
                     result[included_file_name] = None
 
                     checksum = new_hash()
                     update_checksum(checksum, included_src)
                     _inner(included_src)
 
@@ -262,15 +265,15 @@
 # }}}
 
 
 def retrieve_from_cache(cache_dir, cache_key):
     class _InvalidInfoFile(RuntimeError):
         pass
 
-    from os.path import join, isdir
+    from os.path import isdir, join
     module_cache_dir = join(cache_dir, cache_key)
     if not isdir(module_cache_dir):
         return None
 
     cleanup_m = CleanupManager()
     try:
         try:
@@ -339,33 +342,30 @@
 
 
 def _create_built_program_from_source_cached(ctx, src, options_bytes,
         devices, cache_dir, include_path):
     from os.path import join
 
     if cache_dir is None:
-        try:
-            import platformdirs as appdirs
-        except ImportError:
-            import appdirs
+        import platformdirs
 
-        cache_dir = join(appdirs.user_cache_dir("pyopencl", "pyopencl"),
+        # Determine the cache directory in the same way as pytools.PersistentDict,
+        # which PyOpenCL uses for invoker caches.
+        if sys.platform == "darwin" and os.getenv("XDG_CACHE_HOME") is not None:
+            # platformdirs does not handle XDG_CACHE_HOME on macOS
+            # https://github.com/platformdirs/platformdirs/issues/269
+            cache_dir = join(os.getenv("XDG_CACHE_HOME"), "pyopencl")
+        else:
+            cache_dir = platformdirs.user_cache_dir("pyopencl", "pyopencl")
+
+        cache_dir = join(cache_dir,
                 "pyopencl-compiler-cache-v2-py{}".format(
                     ".".join(str(i) for i in sys.version_info)))
 
-    # {{{ ensure cache directory exists
-
-    try:
-        os.makedirs(cache_dir)
-    except OSError as e:
-        from errno import EEXIST
-        if e.errno != EEXIST:
-            raise
-
-    # }}}
+    os.makedirs(cache_dir, exist_ok=True)
 
     if devices is None:
         devices = ctx.devices
 
     cache_keys = [get_cache_key(device, options_bytes, src) for device in devices]
 
     binaries = []
@@ -509,16 +509,16 @@
         # Mac error on intel CPU driver: can't build from cached version.
         # If we get a build_program_failure from the cached version then
         # build from source instead, otherwise report the failure.
         if build_program_failure and not was_cached:
             raise
 
         if not build_program_failure:
-            from warnings import warn
             from traceback import format_exc
+            from warnings import warn
             warn(
                 "PyOpenCL compiler caching failed with an exception:\n"
                 f"[begin exception]\n{format_exc()}[end exception]",
                 stacklevel=2)
 
         prg = _cl._Program(ctx, src)
         was_cached = False
```

### Comparing `pyopencl-2024.1/pyopencl/capture_call.py` & `pyopencl-2024.2/pyopencl/capture_call.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
 
-import pyopencl as cl
 import numpy as np
-from pytools.py_codegen import PythonCodeGenerator, Indentation
+from pytools.py_codegen import Indentation, PythonCodeGenerator
+
+import pyopencl as cl
 
 
 def capture_kernel_call(kernel, output_file, queue, g_size, l_size, *args, **kwargs):
     try:
         source = kernel._source
     except AttributeError:
         raise RuntimeError("cannot capture call, kernel source not available")
@@ -134,16 +135,16 @@
         cg("")
         cg("queue.finish()")
 
     # }}}
 
     # {{{ data
 
-    from zlib import compress
     from base64 import b64encode
+    from zlib import compress
     cg("")
     line_len = 70
 
     for name, val in arg_data:
         cg("%s = (" % name)
         with Indentation(cg):
             val = b64encode(compress(memoryview(val))).decode()
```

### Comparing `pyopencl-2024.1/pyopencl/characterize/__init__.py` & `pyopencl-2024.2/pyopencl/characterize/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,20 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
-import pyopencl as cl
-from pytools import memoize
 from typing import Dict, Optional, Tuple
 
+from pytools import memoize
+
+import pyopencl as cl
+
 
 class CLCharacterizationWarning(UserWarning):
     pass
 
 
 @memoize
 def has_double_support(dev):
```

### Comparing `pyopencl-2024.1/pyopencl/characterize/performance.py` & `pyopencl-2024.2/pyopencl/characterize/performance.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
-import pyopencl as cl
 import numpy as np
 
+import pyopencl as cl
+
 
 # {{{ timing helpers
 
 class Timer:
     def __init__(self, queue):
         self.queue = queue
```

### Comparing `pyopencl-2024.1/pyopencl/cl/pyopencl-airy.cl` & `pyopencl-2024.2/pyopencl/cl/pyopencl-airy.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/pyopencl/cl/pyopencl-bessel-j-complex.cl` & `pyopencl-2024.2/pyopencl/cl/pyopencl-bessel-j-complex.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/pyopencl/cl/pyopencl-bessel-j.cl` & `pyopencl-2024.2/pyopencl/cl/pyopencl-bessel-j.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/pyopencl/cl/pyopencl-bessel-y.cl` & `pyopencl-2024.2/pyopencl/cl/pyopencl-bessel-y.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/pyopencl/cl/pyopencl-complex.h` & `pyopencl-2024.2/pyopencl/cl/pyopencl-complex.h`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/pyopencl/cl/pyopencl-eval-tbl.cl` & `pyopencl-2024.2/pyopencl/cl/pyopencl-eval-tbl.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/pyopencl/cl/pyopencl-hankel-complex.cl` & `pyopencl-2024.2/pyopencl/cl/pyopencl-hankel-complex.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/pyopencl/cl/pyopencl-random123/array.h` & `pyopencl-2024.2/pyopencl/cl/pyopencl-random123/array.h`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/pyopencl/cl/pyopencl-random123/openclfeatures.h` & `pyopencl-2024.2/pyopencl/cl/pyopencl-random123/openclfeatures.h`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/pyopencl/cl/pyopencl-random123/philox.cl` & `pyopencl-2024.2/pyopencl/cl/pyopencl-random123/philox.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/pyopencl/cl/pyopencl-random123/threefry.cl` & `pyopencl-2024.2/pyopencl/cl/pyopencl-random123/threefry.cl`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/pyopencl/clmath.py` & `pyopencl-2024.2/pyopencl/clmath.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,19 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
+import numpy as np
+
 import pyopencl.array as cl_array
 import pyopencl.elementwise as elementwise
 from pyopencl.array import _get_common_dtype
-import numpy as np
 
 
 def _make_unary_array_func(name):
     @cl_array.elwise_kernel_runner
     def knl_runner(result, arg):
         if arg.dtype.kind == "c":
             from pyopencl.elementwise import complex_dtype_to_name
```

### Comparing `pyopencl-2024.1/pyopencl/cltypes.py` & `pyopencl-2024.2/pyopencl/cltypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,20 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
+import warnings
+
 import numpy as np
+
 from pyopencl.tools import get_or_register_dtype
-import warnings
+
 
 if __file__.endswith("array.py"):
     warnings.warn(
         "pyopencl.array.vec is deprecated. Please use pyopencl.cltypes.",
         stacklevel=2)
 
 """
```

### Comparing `pyopencl-2024.1/pyopencl/compyte/array.py` & `pyopencl-2024.2/pyopencl/compyte/array.py`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/pyopencl/compyte/dtypes.py` & `pyopencl-2024.2/pyopencl/compyte/dtypes.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -107,16 +107,16 @@
 
 # }}}
 
 
 # {{{ C types
 
 def fill_registry_with_c_types(reg, respect_windows, include_bool=True):
-    from sys import platform
     import struct
+    from sys import platform
 
     if include_bool:
         # bool is of unspecified size in the OpenCL spec and may in fact be
         # 4-byte.
         reg.get_or_register_dtype("bool", np.bool_)
 
     reg.get_or_register_dtype(["signed char", "char"], np.int8)
```

### Comparing `pyopencl-2024.1/pyopencl/compyte/ndarray/gen_elemwise.py` & `pyopencl-2024.2/pyopencl/compyte/ndarray/gen_elemwise.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 
 The elemwise fct are also used with scalar operation! So it can happen
 that ndim is 0 as with all scalar type.
 """
 
 
 import numpy
+import pygpu_ndarray as gpu_ndarray
 import StringIO
 
-import pygpu_ndarray as gpu_ndarray
 _CL_MODE = hasattr(gpu_ndarray, "set_opencl_context")
 
 
 if _CL_MODE:
     # THIS IS NOT FINISHED
     import pyopencl as cl
     import pyopencl.array as cl_array
     from pyopencl.tools import dtype_to_ctype
 #    import pyopencl._mymako as mako
     from pyopencl._cluda import CLUDA_PREAMBLE
+
     # TODO: use mako to get rid of the %if
     CLUDA_PREAMBLE = CLUDA_PREAMBLE[:455]
     CLUDA_PREAMBLE += """
 #define LDIM_0 get_local_size(0)
 #define LDIM_1 get_local_size(1)
 #define LDIM_2 get_local_size(2)
 
@@ -47,20 +48,20 @@
 #define LDIM_2 blockDim.z
 
 #define GDIM_0 gridDim.x
 #define GDIM_1 gridDim.y
 #define GDIM_2 gridDim.z
  """
 
-from theano import Apply
-from theano import scalar
-from theano.tensor import TensorType
+import logging
+
 import theano
+from theano import Apply, scalar
+from theano.tensor import TensorType
 
-import logging
 _logger_name = 'compyte.gen_elemwise'
 _logger = logging.getLogger(_logger_name)
 _logger.setLevel(logging.INFO)
 _logger.addHandler(logging.StreamHandler())  # TO REMOVE
 
 
 def warning(*msg):
```

### Comparing `pyopencl-2024.1/pyopencl/compyte/ndarray/gen_reduction.py` & `pyopencl-2024.2/pyopencl/compyte/ndarray/gen_reduction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import numpy
 import StringIO
 
-
 _CL_MODE = False  # "pyopencl" in __name__
 
 
 if _CL_MODE:
     # THIS IS NOT FINISHED
     import pyopencl as cl
     import pyopencl.array as cl_array
     from pyopencl.tools import dtype_to_ctype
 #    import pyopencl._mymako as mako
     from pyopencl._cluda import CLUDA_PREAMBLE
+
     # TODO: use mako to get rid of the %if
     CLUDA_PREAMBLE = CLUDA_PREAMBLE[:455]
     CLUDA_PREAMBLE += """
 #define LDIM_0 get_local_id(0)
 #define LDIM_1 get_local_id(1)
 #define LDIM_2 get_local_id(2)
 
@@ -39,21 +39,21 @@
 #define LDIM_2 blockDim.z
 
 #define GDIM_0 gridDim.x
 #define GDIM_1 gridDim.y
 #define GDIM_2 gridDim.z
  """
 
-from theano import Apply
-from theano import scalar
-from theano.tensor import TensorType
-from theano.sandbox.cuda import CudaNdarrayType
+import logging
+
 import theano
+from theano import Apply, scalar
+from theano.sandbox.cuda import CudaNdarrayType
+from theano.tensor import TensorType
 
-import logging
 _logger_name = 'compyte.gen_reduction'
 _logger = logging.getLogger(_logger_name)
 _logger.setLevel(logging.INFO)
 _logger.addHandler(logging.StreamHandler())  # TO REMOVE
 
 
 def warning(*msg):
```

### Comparing `pyopencl-2024.1/pyopencl/compyte/ndarray/setup_opencl.py` & `pyopencl-2024.2/pyopencl/compyte/ndarray/setup_opencl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
-
-from distutils.core import setup, Extension
 from distutils.command.build_ext import build_ext
+from distutils.core import Extension, setup
 from distutils.dep_util import newer
+
 import numpy as np
 
 
 class build_ext_nvcc(build_ext):
     user_options = build_ext.user_options
     user_options.extend([
             ('cuda-root=', None, "The cuda root directory")])
@@ -78,14 +78,15 @@
             self.cuda_extension(ext)
             # uncomment this + inherit from the cython version of build_ext
             # work with cuda and cython sources
             #ext.sources = self.cython_sources(ext.sources, ext)
             self.build_extension(ext)
 
 import sys
+
 if sys.platform == 'darwin':
     libcl_args = {'extra_link_args': ['-framework', 'OpenCL']}
 else:
     libcl_args = {'libraries': ['OpenCL']}
 
 
 setup(name='compyte',
```

### Comparing `pyopencl-2024.1/pyopencl/compyte/ndarray/test_gpu_elemwise.py` & `pyopencl-2024.2/pyopencl/compyte/ndarray/test_gpu_elemwise.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # TODO: test other dtype
+from functools import reduce
+
 import numpy
+import pygpu_ndarray as gpu_ndarray
 import theano
 
-import pygpu_ndarray as gpu_ndarray
 from .gen_elemwise import MyGpuNdArray, elemwise_collapses
-from .test_gpu_ndarray import (dtypes_all, enable_double,
-                              gen_gpu_nd_array, product)
-from functools import reduce
+from .test_gpu_ndarray import (dtypes_all, enable_double, gen_gpu_nd_array,
+                               product)
 
 
 def rand(shape, dtype):
     r = numpy.random.randn(*shape) * 10
     if dtype.startswith("u"):
         r = numpy.absolute(r)
     return r.astype(dtype)
```

### Comparing `pyopencl-2024.1/pyopencl/compyte/ndarray/test_gpu_ndarray.py` & `pyopencl-2024.2/pyopencl/compyte/ndarray/test_gpu_ndarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import copy
 
 import numpy
-
 import pygpu_ndarray as gpu_ndarray
 
 enable_double = True
 enable_double = False
 
 dtypes_all = ["float32",
               "int8", "int16", "int32", "int64",
```

### Comparing `pyopencl-2024.1/pyopencl/elementwise.py` & `pyopencl-2024.2/pyopencl/elementwise.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,22 +27,20 @@
 """
 
 
 import enum
 from typing import Any, List, Optional, Tuple, Union
 
 import numpy as np
+from pytools import memoize_method
 
 import pyopencl as cl
-from pyopencl.tools import context_dependent_memoize
 from pyopencl.tools import (
-        dtype_to_ctype, DtypedArgument, VectorArg, ScalarArg,
-        KernelTemplateBase, dtype_to_c_struct)
-
-from pytools import memoize_method
+    DtypedArgument, KernelTemplateBase, ScalarArg, VectorArg,
+    context_dependent_memoize, dtype_to_c_struct, dtype_to_ctype)
 
 
 # {{{ elementwise kernel code generator
 
 def get_elwise_program(
         context: cl.Context,
         arguments: List[DtypedArgument],
@@ -117,15 +115,15 @@
         operation: str, *,
         name: str = "elwise_kernel",
         options: Any = None,
         preamble: str = "",
         use_range: bool = False,
         **kwargs: Any) -> Tuple[cl.Kernel, List[DtypedArgument]]:
 
-    from pyopencl.tools import parse_arg_list, get_arg_offset_adjuster_code
+    from pyopencl.tools import get_arg_offset_adjuster_code, parse_arg_list
     parsed_args = parse_arg_list(arguments, with_offset=True)
 
     auto_preamble = kwargs.pop("auto_preamble", True)
 
     pragmas = []
     includes = []
     have_double_pragma = False
```

### Comparing `pyopencl-2024.1/pyopencl/invoker.py` & `pyopencl-2024.2/pyopencl/invoker.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,22 +18,24 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
-import numpy as np
-
+from typing import Any, Tuple
 from warnings import warn
-import pyopencl._cl as _cl
+
+import numpy as np
 from pytools.persistent_dict import WriteOncePersistentDict
 from pytools.py_codegen import Indentation, PythonCodeGenerator
-from pyopencl.tools import _NumpyTypesKeyBuilder, VectorArg
+
 import pyopencl as cl
+import pyopencl._cl as _cl
+from pyopencl.tools import VectorArg, _NumpyTypesKeyBuilder
 
 
 # {{{ arg packing helpers
 
 _size_t_char = ({
     8: "Q",
     4: "L",
@@ -369,18 +371,21 @@
                 f"the limit of {dev_limit} bytes on {dev}. This might "
                 "lead to compilation errors, especially on GPU devices.",
                 stacklevel=3)
 
 # }}}
 
 
-invoker_cache = WriteOncePersistentDict(
-        "pyopencl-invoker-cache-v41",
-        key_builder=_NumpyTypesKeyBuilder(),
-        in_mem_cache_size=0)
+if not cl._PYOPENCL_NO_CACHE:
+    from pytools.py_codegen import PicklableModule
+    invoker_cache: WriteOncePersistentDict[Any, Tuple[PicklableModule, str]] \
+        = WriteOncePersistentDict(
+            "pyopencl-invoker-cache-v42-nano",
+            key_builder=_NumpyTypesKeyBuilder(),
+            in_mem_cache_size=0)
 
 
 def generate_enqueue_and_set_args(function_name,
         num_passed_args, num_cl_args,
         arg_types,
         work_around_arg_count_bug, warn_about_arg_count_bug, devs):
 
@@ -396,15 +401,16 @@
             pmod, enqueue_name = invoker_cache[cache_key]
             from_cache = True
         except KeyError:
             pass
 
     if not from_cache:
         pmod, enqueue_name = _generate_enqueue_and_set_args_module(*cache_key)
-        invoker_cache.store_if_not_present(cache_key, (pmod, enqueue_name))
+        if not cl._PYOPENCL_NO_CACHE:
+            invoker_cache.store_if_not_present(cache_key, (pmod, enqueue_name))
 
     return (
             pmod.mod_globals[enqueue_name],
             pmod.mod_globals["set_args"])
 
 # }}}
```

### Comparing `pyopencl-2024.1/pyopencl/ipython_ext.py` & `pyopencl-2024.2/pyopencl/ipython_ext.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from IPython.core.magic import (magics_class, Magics, cell_magic, line_magic)
+from IPython.core.magic import Magics, cell_magic, line_magic, magics_class
 
 import pyopencl as cl
 
 
 @magics_class
 class PyOpenCLMagics(Magics):
     def _run_kernel(self, kernel, options):
```

### Comparing `pyopencl-2024.1/pyopencl/reduction.py` & `pyopencl-2024.2/pyopencl/reduction.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,17 +31,16 @@
 from dataclasses import dataclass
 from typing import Any, List, Optional, Tuple, Union
 
 import numpy as np
 
 import pyopencl as cl
 from pyopencl.tools import (
-        DtypedArgument, KernelTemplateBase,
-        context_dependent_memoize, dtype_to_ctype,
-        _process_code_for_macro)
+    DtypedArgument, KernelTemplateBase, _process_code_for_macro,
+    context_dependent_memoize, dtype_to_ctype)
 
 
 # {{{ kernel source
 
 KERNEL = r"""//CL//
     #define PCL_GROUP_SIZE ${group_size}
     #define PCL_READ_AND_MAP(i) (${map_expr})
@@ -173,14 +172,15 @@
 
     if max_group_size is not None:
         group_size = min(max_group_size, group_size)
 
     # }}}
 
     from mako.template import Template
+
     from pyopencl.characterize import has_double_support
 
     arguments = ", ".join(arg.declarator() for arg in parsed_args)
     if parsed_args:
         arguments += ", "
 
     src = str(Template(KERNEL).render(
@@ -215,16 +215,16 @@
     if stage not in (1, 2):
         raise ValueError(f"unknown stage index: '{stage}'")
 
     if map_expr is None:
         map_expr = "pyopencl_reduction_inp[i]" if stage == 2 else "in[i]"
 
     from pyopencl.tools import (
-            parse_arg_list, get_arg_list_scalar_arg_dtypes,
-            get_arg_offset_adjuster_code, VectorArg)
+        VectorArg, get_arg_list_scalar_arg_dtypes, get_arg_offset_adjuster_code,
+        parse_arg_list)
 
     if arguments is None:
         raise ValueError("arguments must not be None")
 
     arguments = parse_arg_list(arguments, with_offset=True)
     arg_prep = get_arg_offset_adjuster_code(arguments)
```

### Comparing `pyopencl-2024.1/pyopencl/scan.py` & `pyopencl-2024.2/pyopencl/scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,41 +18,32 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
 Derived from code within the Thrust project, https://github.com/NVIDIA/thrust
 """
 
+import logging
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional, Set, Tuple, Union
 
 import numpy as np
+from pytools.persistent_dict import WriteOncePersistentDict
 
 import pyopencl as cl
-import pyopencl.array
-from pyopencl.tools import (
-        KernelTemplateBase,
-        DtypedArgument,
-        bitlog2,
-        context_dependent_memoize,
-        dtype_to_ctype,
-        get_arg_list_scalar_arg_dtypes,
-        get_arg_offset_adjuster_code,
-        _process_code_for_macro,
-        _NumpyTypesKeyBuilder,
-        )
-
 import pyopencl._mymako as mako
+import pyopencl.array
 from pyopencl._cluda import CLUDA_PREAMBLE
-
-from pytools.persistent_dict import WriteOncePersistentDict
+from pyopencl.tools import (
+    DtypedArgument, KernelTemplateBase, _NumpyTypesKeyBuilder,
+    _process_code_for_macro, bitlog2, context_dependent_memoize, dtype_to_ctype,
+    get_arg_list_scalar_arg_dtypes, get_arg_offset_adjuster_code)
 
 
-import logging
 logger = logging.getLogger(__name__)
 
 
 # {{{ preamble
 
 SHARED_PREAMBLE = CLUDA_PREAMBLE + """//CL//
 #define WG_SIZE ${wg_size}
@@ -1137,18 +1128,22 @@
     # }}}
 
     @abstractmethod
     def finish_setup(self) -> None:
         pass
 
 
-generic_scan_kernel_cache = WriteOncePersistentDict(
-        "pyopencl-generated-scan-kernel-cache-v1",
-        key_builder=_NumpyTypesKeyBuilder(),
-        in_mem_cache_size=0)
+if not cl._PYOPENCL_NO_CACHE:
+    generic_scan_kernel_cache: WriteOncePersistentDict[Any,
+                    Tuple[_GeneratedScanKernelInfo, _GeneratedScanKernelInfo,
+                    _GeneratedFinalUpdateKernelInfo]] = \
+        WriteOncePersistentDict(
+            "pyopencl-generated-scan-kernel-cache-v1",
+            key_builder=_NumpyTypesKeyBuilder(),
+            in_mem_cache_size=0)
 
 
 class GenericScanKernel(GenericScanKernelBase):
     """Generates and executes code that performs prefix sums ("scans") on
     arbitrary types, with many possible tweaks.
 
     Usage example::
@@ -1195,15 +1190,16 @@
                     "cache miss for generated scan kernel '%s'" % self.name_prefix)
             self._finish_setup_impl()
 
             result = (self.first_level_scan_gen_info,
                       self.second_level_scan_gen_info,
                       self.final_update_gen_info)
 
-            generic_scan_kernel_cache.store_if_not_present(cache_key, result)
+            if not cl._PYOPENCL_NO_CACHE:
+                generic_scan_kernel_cache.store_if_not_present(cache_key, result)
 
         # Build the kernels.
         self.first_level_scan_info = self.first_level_scan_gen_info.build(
                 self.context, self.options)
         del self.first_level_scan_gen_info
 
         self.second_level_scan_info = self.second_level_scan_gen_info.build(
```

### Comparing `pyopencl-2024.1/pyopencl/tools.py` & `pyopencl-2024.2/pyopencl/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,59 +122,53 @@
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
 HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 """
 
+import re
 from abc import ABC, abstractmethod
 from sys import intern
 from typing import Any, List, Optional, Union
 
-# Do not add a pyopencl import here: This will add an import cycle.
-
 import numpy as np
 from pytools import memoize, memoize_method
-from pyopencl._cl import bitlog2, get_cl_header_version  # noqa: F401
 from pytools.persistent_dict import KeyBuilder as KeyBuilderBase
 
-import re
-
+from pyopencl._cl import bitlog2, get_cl_header_version  # noqa: F401
+from pyopencl.compyte.dtypes import TypeNameNotKnown  # noqa: F401
 from pyopencl.compyte.dtypes import (  # noqa: F401
-        get_or_register_dtype, TypeNameNotKnown,
-        register_dtype, dtype_to_ctype)
+    dtype_to_ctype, get_or_register_dtype, register_dtype)
+
+
+# Do not add a pyopencl import here: This will add an import cycle.
 
 
 def _register_types():
     from pyopencl.compyte.dtypes import (
-            TYPE_REGISTRY, fill_registry_with_opencl_c_types)
+        TYPE_REGISTRY, fill_registry_with_opencl_c_types)
 
     fill_registry_with_opencl_c_types(TYPE_REGISTRY)
 
     get_or_register_dtype("cfloat_t", np.complex64)
     get_or_register_dtype("cdouble_t", np.complex128)
 
 
 _register_types()
 
 
 # {{{ imported names
 
 from pyopencl._cl import (  # noqa: F401
-        PooledBuffer, AllocatorBase, DeferredAllocator,
-        ImmediateAllocator, MemoryPool,
-        )
+    AllocatorBase, DeferredAllocator, ImmediateAllocator, MemoryPool, PooledBuffer)
 
 
 if get_cl_header_version() >= (2, 0):
-    from pyopencl._cl import (  # noqa: F401
-            SVMPool,
-            PooledSVM,
-            SVMAllocator,
-            )
+    from pyopencl._cl import PooledSVM, SVMAllocator, SVMPool  # noqa: F401
 
 # }}}
 
 
 # {{{ monkeypatch docstrings into imported interfaces
 
 _MEMPOOL_IFACE_DOCS = """
@@ -514,14 +508,15 @@
 
     from functools import wraps
     cache_dict_name = intern("_memoize_inner_dic_%s_%s_%d"
             % (nested_func.__name__, nested_func.__code__.co_filename,
                 nested_func.__code__.co_firstlineno))
 
     from inspect import currentframe
+
     # prevent ref cycle
     try:
         caller_frame = currentframe().f_back
         cache_context = caller_frame.f_globals[
                 caller_frame.f_code.co_name]
     finally:
         #del caller_frame
@@ -556,14 +551,16 @@
     .. versionadded:: 2011.2
     """
     for cache in _first_arg_dependent_caches:
         cache.clear()
 
 
 import atexit
+
+
 atexit.register(clear_first_arg_caches)
 
 # }}}
 
 
 # {{{ pytest fixtures
```

### Comparing `pyopencl-2024.1/pyopencl.egg-info/PKG-INFO` & `pyopencl-2024.2/pyopencl.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyopencl
-Version: 2024.1
+Version: 2024.2
 Summary: Python wrapper for OpenCL
 Home-page: http://mathema.tician.de/software/pyopencl
 Author: Andreas Kloeckner
 Author-email: inform@tiker.net
 License: MIT
 Classifier: Environment :: Console
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,40 +18,43 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: ~=3.8
 License-File: LICENSE
 Requires-Dist: numpy
-Requires-Dist: pytools>=2021.2.7
+Requires-Dist: pytools>=2022.1.13
 Requires-Dist: platformdirs>=2.2.0
+Requires-Dist: importlib-resources; python_version < "3.9"
 Provides-Extra: pocl
 Requires-Dist: pocl_binary_distribution>=1.2; extra == "pocl"
 Provides-Extra: oclgrind
 Requires-Dist: oclgrind_binary_distribution>=18.3; extra == "oclgrind"
 Provides-Extra: test
 Requires-Dist: pytest>=7.0.0; extra == "test"
 Requires-Dist: Mako; extra == "test"
 
 PyOpenCL: Pythonic Access to OpenCL, with Arrays and Algorithms
 ===============================================================
 
-.. image:: https://gitlab.tiker.net/inducer/pyopencl/badges/main/pipeline.svg
+.. |badge-gitlab-ci| image:: https://gitlab.tiker.net/inducer/pyopencl/badges/main/pipeline.svg
     :alt: Gitlab Build Status
     :target: https://gitlab.tiker.net/inducer/pyopencl/commits/main
-.. image:: https://github.com/inducer/pyopencl/workflows/CI/badge.svg?branch=main&event=push
+.. |badge-github-ci| image:: https://github.com/inducer/pyopencl/workflows/CI/badge.svg?branch=main&event=push
     :alt: Github Build Status
     :target: https://github.com/inducer/pyopencl/actions?query=branch%3Amain+workflow%3ACI+event%3Apush
-.. image:: https://badge.fury.io/py/pyopencl.svg
+.. |badge-pypi| image:: https://badge.fury.io/py/pyopencl.svg
     :alt: Python Package Index Release Page
     :target: https://pypi.org/project/pyopencl/
-.. image:: https://zenodo.org/badge/1575307.svg
+.. |badge-zenodo| image:: https://zenodo.org/badge/1575307.svg
     :alt: Zenodo DOI for latest release
     :target: https://zenodo.org/badge/latestdoi/1575307
 
+|badge-gitlab-ci| |badge-github-ci| |badge-pypi| |badge-zenodo|
+
 PyOpenCL lets you access GPUs and other massively parallel compute
 devices from Python. It tries to offer computing goodness in the
 spirit of its sister project `PyCUDA <https://mathema.tician.de/software/pycuda>`__:
 
 * Object cleanup tied to lifetime of objects. This idiom, often
   called `RAII <https://en.wikipedia.org/wiki/Resource_Acquisition_Is_Initialization>`__
   in C++, makes it much easier to write correct, leak- and
@@ -80,26 +83,23 @@
 Simple 4-step `install instructions <https://documen.tician.de/pyopencl/misc.html#installation>`__
 using Conda on Linux and macOS (that also install a working OpenCL implementation!)
 can be found in the `documentation <https://documen.tician.de/pyopencl/>`__.
 
 What you'll need if you do *not* want to use the convenient instructions above and
 instead build from source:
 
-* gcc/g++ new enough to be compatible with pybind11
-  (see their `FAQ <https://pybind11.readthedocs.io/en/stable/faq.html>`__)
+* g++/clang new enough to be compatible with nanobind (specifically, full support of C++17 is needed)
 * `numpy <https://numpy.org>`__, and
 * an OpenCL implementation. (See this `howto <https://wiki.tiker.net/OpenCLHowTo>`__
   for how to get one.)
 
 Links
 -----
 
 * `Documentation <https://documen.tician.de/pyopencl>`__
   (read how things work)
+* `Python package index <https://pypi.python.org/pypi/pyopencl>`__
+  (download releases, including binary wheels for Linux, macOS, Windows)
 * `Conda Forge <https://anaconda.org/conda-forge/pyopencl>`__
   (download binary packages for Linux, macOS, Windows)
-* `Python package index <https://pypi.python.org/pypi/pyopencl>`__
-  (download releases)
-* `C. Gohlke's Windows binaries <https://www.lfd.uci.edu/~gohlke/pythonlibs/#pyopencl>`__
-  (download Windows binaries)
 * `Github <https://github.com/inducer/pyopencl>`__
   (get latest source code, file bugs)
```

### Comparing `pyopencl-2024.1/pyopencl.egg-info/SOURCES.txt` & `pyopencl-2024.2/pyopencl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,14 @@
 pyopencl/cl/pyopencl-airy.cl
 pyopencl/cl/pyopencl-bessel-j-complex.cl
 pyopencl/cl/pyopencl-bessel-j.cl
 pyopencl/cl/pyopencl-bessel-y.cl
 pyopencl/cl/pyopencl-complex.h
 pyopencl/cl/pyopencl-eval-tbl.cl
 pyopencl/cl/pyopencl-hankel-complex.cl
-pyopencl/cl/pyopencl-ranluxcl.cl
 pyopencl/cl/pyopencl-random123/array.h
 pyopencl/cl/pyopencl-random123/openclfeatures.h
 pyopencl/cl/pyopencl-random123/philox.cl
 pyopencl/cl/pyopencl-random123/threefry.cl
 pyopencl/compyte/__init__.py
 pyopencl/compyte/array.py
 pyopencl/compyte/dtypes.py
```

### Comparing `pyopencl-2024.1/pyproject.toml` & `pyopencl-2024.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [build-system]
 # Minimum requirements for the build system to execute.
 requires = [
         "setuptools>=42.0.0",
         "wheel>=0.34.2",
         "numpy;python_version >= '3.9' and platform_python_implementation == 'PyPy'",
         "oldest-supported-numpy;python_version < '3.9' or platform_python_implementation != 'PyPy'",
-        "pybind11>=2.5.0"
+        "scikit-build",
+        "cmake>=3.17",
+        "nanobind>=1.9.2",
+        "ninja; platform_system!='Windows'",
         ]
 build-backend = "setuptools.build_meta"
 
-
 [tool.cibuildwheel]
 test-command = "pytest {project}/test"
 test-extras = ["test"]
 
 [tool.cibuildwheel.linux]
-skip = ["pp37*", "cp36-*", "cp37-*", "*_i686"]
+skip = ["pp*", "cp36-*", "cp37-*", "*_i686"]
 test-command = ""
 before-all = [
     "yum install -y git openssl-devel ruby",
     "bash {package}/scripts/build-ocl.sh",
 ]
 before-build = [
     "pip install numpy -Csetup-args=-Dallow-noblas=true",
@@ -38,12 +40,16 @@
 skip = ["pp*", "cp36-*", "cp37-*"]
 before-all = "bash {package}/scripts/build-ocl-macos.sh"
 test-command = "pytest {project}/test/test_array.py" # same limitation as conda-forge
 archs = "x86_64 arm64"
 
 # https://github.com/conda-forge/pyopencl-feedstock/blob/6f3c5de59b18c9518abba3cb94f6ae92964553f8/recipe/meta.yaml#L62-L63
 
+[tool.cibuildwheel.macos.environment]
+# Needed for full C++17 support
+MACOSX_DEPLOYMENT_TARGET = "10.14"
+
 [tool.cibuildwheel.windows]
 skip = ["*-win32", "pp*", "cp36-*", "cp37-*"]
 test-command = ""
 before-all = "bash {package}/scripts/build-ocl-windows.sh"
 before-build = "python configure.py --cl-inc-dir=D:/a/pyopencl/pyopencl/OpenCL-Headers/install/include --cl-lib-dir=\"C:/Program Files/OpenCL-ICD-Loader/lib\""
```

### Comparing `pyopencl-2024.1/setup.cfg` & `pyopencl-2024.2/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -2,27 +2,31 @@
 ignore = E126,E127,E128,E123,E226,E241,E242,E265,W503,E402
 max-line-length = 85
 exclude = pyopencl/compyte/ndarray,pyopencl/compyte/array.py,gl_particle_animation.py,gl_interop_demo.py
 per-file-ignores = 
 	examples/pi-monte-carlo.py:N,B
 	examples/black-hole-accretion.py:N
 	examples/n-body.py:N
+	pyopencl/__init__.py:I001,I004,I005
 inline-quotes = "
 docstring-quotes = """
 multiline-quotes = """
 
+[isort]
+line_length = 85
+lines_after_imports = 2
+combine_as_imports = True
+multi_line_output = 4
+
 [mypy]
 warn_unused_ignores = True
 exclude = (?x)(
 	pyopencl/compyte
 	)
 
-[mypy-appdirs.*]
-ignore_missing_imports = True
-
 [mypy-IPython.*]
 ignore_missing_imports = True
 
 [mypy-OpenGL.*]
 ignore_missing_imports = True
 
 [mypy-mako.*]
```

### Comparing `pyopencl-2024.1/src/bitlog.cpp` & `pyopencl-2024.2/src/bitlog.cpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/src/bitlog.hpp` & `pyopencl-2024.2/src/bitlog.hpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/src/clinfo_ext.h` & `pyopencl-2024.2/src/clinfo_ext.h`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/src/mempool.hpp` & `pyopencl-2024.2/src/mempool.hpp`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/src/pyopencl_ext.h` & `pyopencl-2024.2/src/pyopencl_ext.h`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/src/tools.hpp` & `pyopencl-2024.2/src/tools.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 // OTHER DEALINGS IN THE SOFTWARE.
 
 
 #ifndef _ASDFDAFVVAFF_PYCUDA_HEADER_SEEN_TOOLS_HPP
 #define _ASDFDAFVVAFF_PYCUDA_HEADER_SEEN_TOOLS_HPP
 
 
-#include <pybind11/pybind11.h>
+#include <nanobind/nanobind.h>
 
 #include <numeric>
 #include <numpy/arrayobject.h>
 
 
 
 namespace pyopencl
@@ -47,17 +47,17 @@
   }
 
 
 
 
   inline void run_python_gc()
   {
-    namespace py = pybind11;
+    namespace py = nanobind;
 
-    py::module_::import("gc").attr("collect")();
+    py::module_::import_("gc").attr("collect")();
   }
 
 
   // https://stackoverflow.com/a/28139075
   template <typename T>
   struct reversion_wrapper { T& iterable; };
```

### Comparing `pyopencl-2024.1/src/wrap_cl.cpp` & `pyopencl-2024.2/src/wrap_cl.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -43,18 +43,18 @@
 
 static bool import_numpy_helper()
 {
   import_array1(false);
   return true;
 }
 
-PYBIND11_MODULE(_cl, m)
+NB_MODULE(_cl, m)
 {
   if (!import_numpy_helper())
-    throw py::error_already_set();
+    throw py::python_error();
 
   pyopencl_expose_constants(m);
   pyopencl_expose_part_1(m);
   pyopencl_expose_part_2(m);
   pyopencl_expose_mempool(m);
 }
```

### Comparing `pyopencl-2024.1/src/wrap_cl.hpp` & `pyopencl-2024.2/src/wrap_cl.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,15 @@
 #include <condition_variable>
 
 #include <cstdio>
 #include <stdexcept>
 #include <iostream>
 #include <vector>
 #include <utility>
+#include <array>
 #include <numeric>
 #include "wrap_helpers.hpp"
 #include <numpy/arrayobject.h>
 #include "tools.hpp"
 
 #ifdef PYOPENCL_PRETEND_CL_VERSION
 #define PYOPENCL_CL_VERSION PYOPENCL_PRETEND_CL_VERSION
@@ -135,14 +136,18 @@
 #endif
 
 // }}}
 
 
 // {{{ macros and typedefs for wrappers
 
+#if NPY_ABI_VERSION < 0x02000000
+  #define PyDataType_ELSIZE(descr) ((descr)->elsize)
+#endif
+
 #if PY_VERSION_HEX >= 0x02050000
   typedef Py_ssize_t PYOPENCL_BUFFER_SIZE_T;
 #else
   typedef int PYOPENCL_BUFFER_SIZE_T;
 #endif
 
 #define PYOPENCL_CAST_BOOL(B) ((B) ? CL_TRUE : CL_FALSE)
@@ -464,15 +469,15 @@
       // This is here because clLinkProgram returns a program
       // object *just* so that there is somewhere for it to
       // stuff the linker logs. :/
       bool m_program_initialized;
       cl_program m_program;
 
     public:
-      error(const char *routine, cl_int c, const char *msg="")
+      error(std::string const &routine, cl_int c, std::string const &msg="")
         : std::runtime_error(msg), m_routine(routine), m_code(c),
         m_program_initialized(false), m_program(nullptr)
       { }
 
       error(const char *routine, cl_program prg, cl_int c,
           const char *msg="")
         : std::runtime_error(msg), m_routine(routine), m_code(c),
@@ -500,14 +505,35 @@
         return (code() == CL_MEM_OBJECT_ALLOCATION_FAILURE
             || code() == CL_OUT_OF_RESOURCES
             || code() == CL_OUT_OF_HOST_MEMORY);
       }
 
       program *get_program() const;
 
+      // FIXME: Inheritance from builtin_exception confuses nanobind
+      const char *err_what()
+      {
+        return what();
+      }
+
+      void set_error() const
+      {
+        py::object err_obj = py::cast(*this);
+        py::object errors_mod = py::module_::import_("pyopencl._errors");
+
+        if (code() == CL_MEM_OBJECT_ALLOCATION_FAILURE)
+          PyErr_SetObject(errors_mod.attr("MemoryError").ptr(), err_obj.ptr());
+        else if (code() <= CL_INVALID_VALUE)
+          PyErr_SetObject(errors_mod.attr("LogicError").ptr(), err_obj.ptr());
+        else if (code() > CL_INVALID_VALUE && code() < CL_SUCCESS)
+          PyErr_SetObject(errors_mod.attr("RuntimeError").ptr(), err_obj.ptr());
+        else
+          PyErr_SetObject(errors_mod.attr("Error").ptr(), err_obj.ptr());
+      }
+
   };
 
   // }}}
 
 
   // {{{ utility functions
 
@@ -520,22 +546,21 @@
   }
 
   // }}}
 
 
   // {{{ buffer interface helper
 
-
   class py_buffer_wrapper : public noncopyable
   {
     private:
       bool m_initialized;
 
-    public:
-      Py_buffer m_buf;
+      public:
+        Py_buffer m_buf;
 
     py_buffer_wrapper()
       : m_initialized(false)
     {}
 
     void get(PyObject *obj, int flags)
     {
@@ -544,21 +569,21 @@
       if (flags & PyBUF_ANY_CONTIGUOUS)
       {
         int flags_wo_cont = flags & ~PyBUF_ANY_CONTIGUOUS;
         if (PyObject_GetBuffer(obj, &m_buf, flags_wo_cont | PyBUF_C_CONTIGUOUS))
         {
           PyErr_Clear();
           if (PyObject_GetBuffer(obj, &m_buf, flags_wo_cont | PyBUF_F_CONTIGUOUS))
-            throw py::error_already_set();
+            throw py::python_error();
         }
       }
       else
 #endif
       if (PyObject_GetBuffer(obj, &m_buf, flags))
-        throw py::error_already_set();
+        throw py::python_error();
 
       m_initialized = true;
     }
 
     virtual ~py_buffer_wrapper()
     {
       if (m_initialized)
@@ -1308,15 +1333,15 @@
             prop == CL_GL_CONTEXT_KHR
             || prop == CL_EGL_DISPLAY_KHR
             || prop == CL_GLX_DISPLAY_KHR
             || prop == CL_CGL_SHAREGROUP_KHR
 #endif
            )
        {
-          py::object ctypes = py::module_::import("ctypes");
+          py::object ctypes = py::module_::import_("ctypes");
           py::object prop = prop_tuple[1], c_void_p = ctypes.attr("c_void_p");
           py::object ptr = ctypes.attr("cast")(prop, c_void_p);
           props.push_back(py::cast<cl_context_properties>(ptr.attr("value")));
        }
 #endif
         else
           throw error("Context", CL_INVALID_VALUE, "invalid context property");
@@ -1325,15 +1350,15 @@
     }
 
     return props;
   }
 
 
   inline
-  context *create_context_inner(py::object py_devices, py::object py_properties,
+  void create_context_inner(context *self, py::object py_devices, py::object py_properties,
       py::object py_dev_type)
   {
     std::vector<cl_context_properties> props
       = parse_context_properties(py_properties);
 
     cl_context_properties *props_ptr
       = props.empty( ) ? nullptr : &props.front();
@@ -1372,33 +1397,23 @@
     }
 
     if (status_code != CL_SUCCESS)
       throw pyopencl::error("Context", status_code);
 
     try
     {
-      return new context(ctx, false);
+      new (self) context(ctx, false);
     }
     catch (...)
     {
       PYOPENCL_CALL_GUARDED(clReleaseContext, (ctx));
       throw;
     }
   }
 
-
-  inline
-  context *create_context(py::object py_devices, py::object py_properties,
-      py::object py_dev_type)
-  {
-    PYOPENCL_RETRY_RETURN_IF_MEM_ERROR(
-      return create_context_inner(py_devices, py_properties, py_dev_type);
-    )
-  }
-
   // }}}
 
 
   // {{{ command_queue
 
   class command_queue
   {
@@ -1548,16 +1563,16 @@
             (m_queue));
       }
 
       const cl_command_queue data() const
       {
         if (m_finalized)
         {
-          auto mod_warnings(py::module_::import("warnings"));
-          auto mod_cl(py::module_::import("pyopencl"));
+          auto mod_warnings(py::module_::import_("warnings"));
+          auto mod_cl(py::module_::import_("pyopencl"));
           mod_warnings.attr("warn")(
               "Command queue used after exit of context manager. "
               "This is deprecated and will stop working in 2023.",
               mod_cl.attr("CommandQueueUsedAfterExit")
               );
         }
         return m_queue;
@@ -1869,14 +1884,15 @@
 
     private:
       struct event_callback_info_t
       {
         std::mutex m_mutex;
         std::condition_variable m_condvar;
 
+        // FIXME: Should implement GC traversal so that these can be collected.
         py::object m_py_event;
         py::object m_py_callback;
 
         bool m_set_callback_suceeded;
 
         bool m_notify_thread_wakeup_is_genuine;
 
@@ -1997,15 +2013,15 @@
         wait_during_cleanup_without_releasing_the_gil();
       }
 
       py::object get_ward() const
       {
         if (m_ward.get())
         {
-          return py::reinterpret_borrow<py::object>(m_ward->m_buf.obj);
+          return py::borrow<py::object>(m_ward->m_buf.obj);
         }
         else
           return py::none();
       }
 
       virtual void wait()
       {
@@ -2117,26 +2133,26 @@
       }
   };
 
 
 
 
   inline
-  user_event *create_user_event(context &ctx)
+  void create_user_event(user_event *self, context &ctx)
   {
     cl_int status_code;
     PYOPENCL_PRINT_CALL_TRACE("clCreateUserEvent");
     cl_event evt = clCreateUserEvent(ctx.data(), &status_code);
 
     if (status_code != CL_SUCCESS)
       throw pyopencl::error("UserEvent", status_code);
 
     try
     {
-      return new user_event(evt, false);
+      new (self) user_event(evt, false);
     }
     catch (...)
     {
       clReleaseEvent(evt);
       throw;
     }
   }
@@ -2224,15 +2240,15 @@
         if (m_valid)
           release();
       }
 
       py::object hostbuf()
       {
         if (m_hostbuf.get())
-          return py::reinterpret_borrow<py::object>(m_hostbuf->m_buf.obj);
+          return py::borrow<py::object>(m_hostbuf->m_buf.obj);
         else
           return py::none();
       }
 
       const cl_mem data() const
       { return m_mem; }
 
@@ -2356,31 +2372,29 @@
         catch (...)
         {
           PYOPENCL_CALL_GUARDED(clReleaseMemObject, (mem));
           throw;
         }
       }
 
-      buffer *getitem(py::slice slc) const
+      buffer *getitem(py::object slc) const
       {
         PYOPENCL_BUFFER_SIZE_T start, end, stride, length;
 
+        if (!PySlice_Check(slc.ptr()))
+          throw pyopencl::error("Buffer.__getitem__", CL_INVALID_VALUE,
+              "Buffer slice must be a slice object");
+
         size_t my_length;
         PYOPENCL_CALL_GUARDED(clGetMemObjectInfo,
             (data(), CL_MEM_SIZE, sizeof(my_length), &my_length, 0));
 
-#if PY_VERSION_HEX >= 0x03020000
         if (PySlice_GetIndicesEx(slc.ptr(),
               my_length, &start, &end, &stride, &length) != 0)
-          throw py::error_already_set();
-#else
-        if (PySlice_GetIndicesEx(reinterpret_cast<PySliceObject *>(slc.ptr()),
-              my_length, &start, &end, &stride, &length) != 0)
-          throw py::error_already_set();
-#endif
+          throw py::python_error();
 
         if (stride != 1)
           throw pyopencl::error("Buffer.__getitem__", CL_INVALID_VALUE,
               "Buffer slice must have stride 1");
 
         cl_mem_flags my_flags;
         PYOPENCL_CALL_GUARDED(clGetMemObjectInfo,
@@ -2395,16 +2409,16 @@
         return get_sub_region(start, end-start, my_flags);
       }
 #endif
   };
 
   // {{{ buffer creation
 
-  inline
-  buffer *create_buffer_py(
+  inline void create_buffer_py(
+      buffer *self,
       context &ctx,
       cl_mem_flags flags,
       size_t size,
       py::object py_hostbuf
       )
   {
     if (py_hostbuf.ptr() != Py_None &&
@@ -2439,15 +2453,15 @@
     cl_mem mem = create_buffer_gc(ctx.data(), flags, size, buf);
 
     if (!(flags & CL_MEM_USE_HOST_PTR))
       retained_buf_obj.reset();
 
     try
     {
-      return new buffer(mem, false, std::move(retained_buf_obj));
+      new (self) buffer(mem, false, std::move(retained_buf_obj));
     }
     catch (...)
     {
       PYOPENCL_CALL_GUARDED(clReleaseMemObject, (mem));
       throw;
     }
   }
@@ -2862,20 +2876,18 @@
 
 
 
 
   // {{{ image formats
 
   inline
-  cl_image_format *make_image_format(cl_channel_order ord, cl_channel_type tp)
+  void set_image_format(cl_image_format *self, cl_channel_order ord, cl_channel_type tp)
   {
-    std::unique_ptr<cl_image_format> result(new cl_image_format);
-    result->image_channel_order = ord;
-    result->image_channel_data_type = tp;
-    return result.release();
+    self->image_channel_order = ord;
+    self->image_channel_data_type = tp;
   }
 
   inline
   py::list get_supported_image_formats(
       context const &ctx,
       cl_mem_flags flags,
       cl_mem_object_type image_type)
@@ -2949,15 +2961,16 @@
   }
 
   // }}}
 
   // {{{ image creation
 
   inline
-  image *create_image(
+  void create_image(
+      image *self,
       context const &ctx,
       cl_mem_flags flags,
       cl_image_format const &fmt,
       py::sequence shape,
       py::sequence pitches,
       py::object buffer)
   {
@@ -3059,27 +3072,28 @@
           "invalid dimension");
 
     if (!(flags & CL_MEM_USE_HOST_PTR))
       retained_buf_obj.reset();
 
     try
     {
-      return new image(mem, false, std::move(retained_buf_obj));
+      new (self) image(mem, false, std::move(retained_buf_obj));
     }
     catch (...)
     {
       PYOPENCL_CALL_GUARDED(clReleaseMemObject, (mem));
       throw;
     }
   }
 
 #if PYOPENCL_CL_VERSION >= 0x1020
 
   inline
-  image *create_image_from_desc(
+  void create_image_from_desc(
+      image *self,
       context const &ctx,
       cl_mem_flags flags,
       cl_image_format const &fmt,
       cl_image_desc &desc,
       py::object buffer)
   {
     if (buffer.ptr() != Py_None &&
@@ -3112,15 +3126,15 @@
       throw pyopencl::error("clCreateImage", status_code);
 
     if (!(flags & CL_MEM_USE_HOST_PTR))
       retained_buf_obj.reset();
 
     try
     {
-      return new image(mem, false, std::move(retained_buf_obj));
+      new (self) image(mem, false, std::move(retained_buf_obj));
     }
     catch (...)
     {
       PYOPENCL_CALL_GUARDED(clReleaseMemObject, (mem));
       throw;
     }
   }
@@ -3364,15 +3378,16 @@
             CL_INVALID_VALUE);
 #endif
       }
   };
 
 #if PYOPENCL_CL_VERSION >= 0x2000
   inline
-  pipe *create_pipe(
+  void create_pipe(
+      pipe *self,
       context const &ctx,
       cl_mem_flags flags,
       cl_uint pipe_packet_size,
       cl_uint pipe_max_packets,
       py::sequence py_props)
   {
 #if 0
@@ -3400,15 +3415,15 @@
         &status_code);
 
     if (status_code != CL_SUCCESS)
       throw pyopencl::error("Pipe", status_code);
 
     try
     {
-      return new pipe(mem, false);
+      new (self) pipe(mem, false);
     }
     catch (...)
     {
       PYOPENCL_CALL_GUARDED(clReleaseMemObject, (mem));
       throw;
     }
 }
@@ -3473,19 +3488,20 @@
       py::object py_wait_for,
       bool is_blocking
       )
   {
     PYOPENCL_PARSE_WAIT_FOR;
     PYOPENCL_PARSE_NUMPY_ARRAY_SPEC;
 
-    npy_uintp size_in_bytes = tp_descr->elsize;
+    npy_uintp size_in_bytes = PyDataType_ELSIZE(tp_descr);
     for (npy_intp sdim: shape)
       size_in_bytes *= sdim;
 
     py::object result;
+    PyArrayObject *result_arr;
 
     cl_event evt;
     cl_int status_code;
     PYOPENCL_PRINT_CALL_TRACE("clEnqueueMapBuffer");
     void *mapped;
 
     PYOPENCL_RETRY_IF_MEM_ERROR(
@@ -3502,38 +3518,40 @@
           if (status_code != CL_SUCCESS)
             throw pyopencl::error("clEnqueueMapBuffer", status_code);
         } );
 
     event evt_handle(evt, false);
 
     std::unique_ptr<memory_map> map;
+
     try
     {
-      result = py::object(py::reinterpret_steal<py::object>(PyArray_NewFromDescr(
+      result = py::object(py::steal<py::object>(PyArray_NewFromDescr(
           &PyArray_Type, tp_descr,
           shape.size(),
           shape.empty() ? nullptr : &shape.front(),
           strides.empty() ? nullptr : &strides.front(),
           mapped, ary_flags, /*obj*/nullptr)));
 
-      if (size_in_bytes != (npy_uintp) PyArray_NBYTES(result.ptr()))
+      result_arr = (PyArrayObject *) result.ptr();
+      if (size_in_bytes != (npy_uintp) PyArray_NBYTES(result_arr))
         throw pyopencl::error("enqueue_map_buffer", CL_INVALID_VALUE,
             "miscalculated numpy array size (not contiguous?)");
 
        map = std::unique_ptr<memory_map>(new memory_map(cq, buf, mapped));
     }
     catch (...)
     {
       PYOPENCL_CALL_GUARDED_CLEANUP(clEnqueueUnmapMemObject, (
             cq->data(), buf.data(), mapped, 0, 0, 0));
       throw;
     }
 
     py::object map_py(handle_from_new_ptr(map.release()));
-    PyArray_BASE(result.ptr()) = map_py.ptr();
+    PyArray_SetBaseObject(result_arr, map_py.ptr());
     Py_INCREF(map_py.ptr());
 
     return py::make_tuple(
         result,
         handle_from_new_ptr(new event(evt_handle)));
   }
 #endif
@@ -3591,23 +3609,24 @@
     catch (...)
     {
       PYOPENCL_CALL_GUARDED_CLEANUP(clEnqueueUnmapMemObject, (
             cq->data(), img.data(), mapped, 0, 0, 0));
       throw;
     }
 
-    py::object result = py::reinterpret_steal<py::object>(PyArray_NewFromDescr(
+    py::object result = py::steal<py::object>(PyArray_NewFromDescr(
         &PyArray_Type, tp_descr,
         shape.size(),
         shape.empty() ? nullptr : &shape.front(),
         strides.empty() ? nullptr : &strides.front(),
         mapped, ary_flags, /*obj*/nullptr));
+    PyArrayObject *result_arr = (PyArrayObject *) result.ptr();
 
     py::object map_py(handle_from_new_ptr(map.release()));
-    PyArray_BASE(result.ptr()) = map_py.ptr();
+    PyArray_SetBaseObject(result_arr, map_py.ptr());
     Py_INCREF(map_py.ptr());
 
     return py::make_tuple(
         result,
         handle_from_new_ptr(new event(evt_handle)),
         row_pitch, slice_pitch);
   }
@@ -3694,30 +3713,33 @@
         {
           m_queue.set(queue->data());
           if (is_queue_out_of_order(m_queue.data()))
             throw error("SVMAllocation.__init__", CL_INVALID_VALUE,
                 "supplying an out-of-order queue to SVMAllocation is invalid");
         }
 
-        int try_count = 0;
-        while (try_count < 2)
+        if (size)
         {
-          PYOPENCL_PRINT_CALL_TRACE("clSVMalloc");
-          m_allocation = clSVMAlloc(
-              ctx->data(),
-              flags, size, alignment);
-          if (m_allocation)
-            return;
+          int try_count = 0;
+          while (try_count < 2)
+          {
+            PYOPENCL_PRINT_CALL_TRACE("clSVMalloc");
+            m_allocation = clSVMAlloc(
+                ctx->data(),
+                flags, size, alignment);
+            if (m_allocation)
+              return;
 
-          ++try_count;
-          run_python_gc();
-        }
+            ++try_count;
+            run_python_gc();
+          }
 
-        if (!m_allocation)
-          throw pyopencl::error("clSVMAlloc", CL_OUT_OF_RESOURCES);
+          if (!m_allocation)
+            throw pyopencl::error("clSVMAlloc", CL_OUT_OF_RESOURCES);
+        }
       }
 
       svm_allocation(std::shared_ptr<context> const &ctx, void *allocation, size_t size,
            const cl_command_queue queue)
         : m_context(ctx), m_allocation(allocation), m_size(size)
       {
         if (queue)
@@ -3739,14 +3761,17 @@
       {
         if (m_allocation)
           release();
       }
 
       void release()
       {
+        if (m_size == 0)
+          return;
+
         if (!m_allocation)
           throw error("SVMAllocation.release", CL_INVALID_VALUE,
               "trying to double-unref svm allocation");
 
         if (m_queue.is_valid())
         {
           PYOPENCL_CALL_GUARDED_CLEANUP(clEnqueueSVMFree, (
@@ -3763,15 +3788,15 @@
         m_allocation = nullptr;
       }
 
       event *enqueue_release(command_queue *queue, py::object py_wait_for)
       {
         PYOPENCL_PARSE_WAIT_FOR;
 
-        if (!m_allocation)
+        if (m_size && !m_allocation)
           throw error("SVMAllocation.enqueue_release", CL_INVALID_VALUE,
               "trying to enqueue_release on an already-freed allocation");
 
         cl_command_queue use_queue;
         if (queue)
           use_queue = queue->data();
         else
@@ -3781,18 +3806,28 @@
           else
             throw error("SVMAllocation.enqueue_release", CL_INVALID_VALUE,
                 "no implicit queue available, must be provided explicitly");
         }
 
         cl_event evt;
 
-        PYOPENCL_CALL_GUARDED_CLEANUP(clEnqueueSVMFree, (
-              use_queue, 1, &m_allocation,
-              nullptr, nullptr,
-              PYOPENCL_WAITLIST_ARGS, &evt));
+        if (m_size == 0)
+        {
+          // We need to get an event from somewhere...
+          // We're using SVM, we must have 2.0 > 1.2.
+          PYOPENCL_CALL_GUARDED_CLEANUP(clEnqueueMarkerWithWaitList,
+                      (use_queue, PYOPENCL_WAITLIST_ARGS, &evt));
+        }
+        else
+        {
+          PYOPENCL_CALL_GUARDED_CLEANUP(clEnqueueSVMFree, (
+                use_queue, 1, &m_allocation,
+                nullptr, nullptr,
+                PYOPENCL_WAITLIST_ARGS, &evt));
+        }
 
         m_allocation = nullptr;
 
         PYOPENCL_RETURN_NEW_EVENT(evt);
       }
 
       void *svm_ptr() const
@@ -3872,15 +3907,15 @@
     PYOPENCL_PARSE_WAIT_FOR;
 
     // {{{ process size
 
     PYOPENCL_GET_SVM_SIZE(src);
     PYOPENCL_GET_SVM_SIZE(dst);
 
-    size_t size;
+    size_t size = 0;
     bool have_size = false;
 
     if (src_has_size)
     {
       size = src_size;
       have_size = true;
     }
@@ -3953,15 +3988,15 @@
     pattern_ptr = pattern_ward->m_buf.buf;
     pattern_len = pattern_ward->m_buf.len;
 
     // {{{ process size
 
     PYOPENCL_GET_SVM_SIZE(dst);
 
-    size_t size;
+    size_t size = 0;
     bool have_size = false;
     if (dst_has_size)
     {
       size = dst_size;
       have_size = true;
     }
     if (!byte_count.is_none())
@@ -4008,15 +4043,15 @@
   {
     PYOPENCL_PARSE_WAIT_FOR;
 
     // {{{ process size
 
     PYOPENCL_GET_SVM_SIZE(svm);
 
-    size_t size;
+    size_t size = 0;
     bool have_size = false;
     if (svm_has_size)
     {
       size = svm_size;
       have_size = true;
     }
     if (!user_size_py.is_none())
@@ -4365,15 +4400,15 @@
                    result_ptrs.empty( ) ? nullptr : &result_ptrs.front(), 0)); \
 
               py::list py_result;
               ptr = result.get();
               for (unsigned i = 0; i < sizes.size(); ++i)
               {
                 py::object binary_pyobj(
-                    py::reinterpret_steal<py::object>(
+                    py::steal<py::object>(
 #if PY_VERSION_HEX >= 0x03000000
                     PyBytes_FromStringAndSize(
                       reinterpret_cast<char *>(ptr), sizes[i])
 #else
                     PyString_FromStringAndSize(
                       reinterpret_cast<char *>(ptr), sizes[i])
 #endif
@@ -4436,37 +4471,37 @@
 #undef PYOPENCL_FIRST_ARG
 
           default:
             throw error("Program.get_build_info", CL_INVALID_VALUE);
         }
       }
 
-      void build(std::string options, py::object py_devices)
+      void build(py::bytes options, py::object py_devices)
       {
         PYOPENCL_PARSE_PY_DEVICES;
 
         PYOPENCL_CALL_GUARDED_THREADED(clBuildProgram,
             (m_program, num_devices, devices,
              options.c_str(), 0 ,0));
       }
 
 #if PYOPENCL_CL_VERSION >= 0x1020
-      void compile(std::string options, py::object py_devices,
+      void compile(py::bytes options, py::object py_devices,
           py::object py_headers)
       {
         PYOPENCL_PARSE_PY_DEVICES;
 
         // {{{ pick apart py_headers
         // py_headers is a list of tuples *(name, program)*
 
         std::vector<std::string> header_names;
         std::vector<cl_program> programs;
         for (py::handle name_hdr_tup_py: py_headers)
         {
-          py::tuple name_hdr_tup = py::reinterpret_borrow<py::tuple>(name_hdr_tup_py);
+          py::tuple name_hdr_tup = py::borrow<py::tuple>(name_hdr_tup_py);
           if (py::len(name_hdr_tup) != 2)
             throw error("Program.compile", CL_INVALID_VALUE,
                 "epxected (name, header) tuple in headers list");
           std::string name = py::cast<std::string>(name_hdr_tup[0]);
           program &prg = py::cast<program &>(name_hdr_tup[1]);
 
           header_names.push_back(name);
@@ -4499,15 +4534,16 @@
 #endif
   };
 
 
 
 
   inline
-  program *create_program_with_source(
+  void create_program_with_source(
+      program *self,
       context &ctx,
       std::string const &src)
   {
     const char *string = src.c_str();
     size_t length = src.size();
 
     cl_int status_code;
@@ -4515,29 +4551,30 @@
     cl_program result = clCreateProgramWithSource(
         ctx.data(), 1, &string, &length, &status_code);
     if (status_code != CL_SUCCESS)
       throw pyopencl::error("clCreateProgramWithSource", status_code);
 
     try
     {
-      return new program(result, false, program::KND_SOURCE);
+      new (self) program(result, false, program::KND_SOURCE);
     }
     catch (...)
     {
       clReleaseProgram(result);
       throw;
     }
   }
 
 
 
 
 
   inline
-  program *create_program_with_binary(
+  void create_program_with_binary(
+      program *self,
       context &ctx,
       py::sequence py_devices,
       py::sequence py_binaries)
   {
     std::vector<cl_device_id> devices;
     std::vector<const unsigned char *> binaries;
     std::vector<size_t> sizes;
@@ -4581,15 +4618,15 @@
     /*
     for (int i = 0; i < num_devices; ++i)
       printf("%d:%d\n", i, binary_statuses[i]);
       */
 
     try
     {
-      return new program(result, false, program::KND_BINARY);
+      new (self) program(result, false, program::KND_BINARY);
     }
     catch (...)
     {
       clReleaseProgram(result);
       throw;
     }
   }
@@ -4628,15 +4665,15 @@
 
 
 
 #if (PYOPENCL_CL_VERSION >= 0x2010)
   inline
   program *create_program_with_il(
       context &ctx,
-      std::string const &src)
+      py::bytes const &src)
   {
     cl_int status_code;
     PYOPENCL_PRINT_CALL_TRACE("clCreateProgramWithIL");
     cl_program result = clCreateProgramWithIL(
         ctx.data(), src.c_str(), src.size(), &status_code);
     if (status_code != CL_SUCCESS)
       throw pyopencl::error("clCreateProgramWithIL", status_code);
@@ -4658,15 +4695,15 @@
 
 
 #if PYOPENCL_CL_VERSION >= 0x1020
   inline
   program *link_program(
       context &ctx,
       py::object py_programs,
-      std::string const &options,
+      py::bytes options,
       py::object py_devices
       )
   {
     PYOPENCL_PARSE_PY_DEVICES;
 
     std::vector<cl_program> programs;
     for (py::handle py_prg: py_programs)
@@ -4823,41 +4860,44 @@
         cl_command_queue q = queue.data();
         PYOPENCL_CALL_GUARDED(clSetKernelArg,
             (m_kernel, arg_index, sizeof(cl_command_queue), &q));
       }
 
       void set_arg_buf_pack(cl_uint arg_index, py::handle py_typechar, py::handle obj)
       {
-        std::string typechar_str(py::cast<std::string>(py_typechar));
+        py::bytes typechar_str(py::cast<py::bytes>(py_typechar));
         if (typechar_str.size() != 1)
           throw error("Kernel.set_arg_buf_pack", CL_INVALID_VALUE,
               "type char argument must have exactly one character");
 
-        char typechar = typechar_str[0];
+        char typechar = *typechar_str.c_str();
 
-#define PYOPENCL_KERNEL_PACK_AND_SET_ARG(TYPECH_VAL, TYPE) \
+#define PYOPENCL_KERNEL_PACK_AND_SET_ARG(TYPECH_VAL, TYPE, CAST_TYPE) \
         case TYPECH_VAL: \
           { \
-            TYPE val = py::cast<TYPE>(obj); \
+            TYPE val = (TYPE) py::cast<CAST_TYPE>(obj); \
             PYOPENCL_CALL_GUARDED(clSetKernelArg, (m_kernel, arg_index, sizeof(val), &val)); \
             break; \
           }
         switch (typechar)
         {
-          PYOPENCL_KERNEL_PACK_AND_SET_ARG('c', char)
-          PYOPENCL_KERNEL_PACK_AND_SET_ARG('b', signed char)
-          PYOPENCL_KERNEL_PACK_AND_SET_ARG('B', unsigned char)
-          PYOPENCL_KERNEL_PACK_AND_SET_ARG('h', short)
-          PYOPENCL_KERNEL_PACK_AND_SET_ARG('H', unsigned short)
-          PYOPENCL_KERNEL_PACK_AND_SET_ARG('i', int)
-          PYOPENCL_KERNEL_PACK_AND_SET_ARG('I', unsigned int)
-          PYOPENCL_KERNEL_PACK_AND_SET_ARG('l', long)
-          PYOPENCL_KERNEL_PACK_AND_SET_ARG('L', unsigned long)
-          PYOPENCL_KERNEL_PACK_AND_SET_ARG('f', float)
-          PYOPENCL_KERNEL_PACK_AND_SET_ARG('d', double)
+          // FIXME: nanobind thinks of char as "short string", not number
+          // The detour via 'int' may lose data.
+          PYOPENCL_KERNEL_PACK_AND_SET_ARG('c', char, int)
+          PYOPENCL_KERNEL_PACK_AND_SET_ARG('b', signed char, int)
+          PYOPENCL_KERNEL_PACK_AND_SET_ARG('B', unsigned char, int)
+
+          PYOPENCL_KERNEL_PACK_AND_SET_ARG('h', short, short)
+          PYOPENCL_KERNEL_PACK_AND_SET_ARG('H', unsigned short, unsigned short)
+          PYOPENCL_KERNEL_PACK_AND_SET_ARG('i', int, int)
+          PYOPENCL_KERNEL_PACK_AND_SET_ARG('I', unsigned int, unsigned int)
+          PYOPENCL_KERNEL_PACK_AND_SET_ARG('l', long, long)
+          PYOPENCL_KERNEL_PACK_AND_SET_ARG('L', unsigned long, unsigned long)
+          PYOPENCL_KERNEL_PACK_AND_SET_ARG('f', float, float)
+          PYOPENCL_KERNEL_PACK_AND_SET_ARG('d', double, double)
           default:
             throw error("Kernel.set_arg_buf_pack", CL_INVALID_VALUE,
                 "invalid type char");
         }
 #undef PYOPENCL_KERNEL_PACK_AND_SET_ARG
       }
 
@@ -4868,15 +4908,15 @@
 
         py_buffer_wrapper buf_wrapper;
 
         try
         {
           buf_wrapper.get(py_buffer.ptr(), PyBUF_ANY_CONTIGUOUS);
         }
-        catch (py::error_already_set &)
+        catch (py::python_error &)
         {
           PyErr_Clear();
           throw error("Kernel.set_arg", CL_INVALID_VALUE,
               "invalid kernel argument");
         }
 
         buf = buf_wrapper.m_buf.buf;
@@ -5135,17 +5175,21 @@
 #define PYOPENCL_KERNEL_SET_ARG_MULTI_ERROR_HANDLER \
     catch (error &err) \
     { \
       std::string msg( \
           std::string("when processing arg#") + std::to_string(arg_index+1) \
           + std::string(" (1-based): ") + std::string(err.what())); \
       \
-      auto mod_cl_ary(py::module_::import("pyopencl.array")); \
+      auto mod_cl_ary(py::module_::import_("pyopencl.array")); \
       auto cls_array(mod_cl_ary.attr("Array")); \
-      if (arg_value.ptr() && py::isinstance(arg_value, cls_array)) \
+      int isinstance_result = PyObject_IsInstance(arg_value.ptr(), cls_array.ptr()); \
+      if (isinstance_result == -1) \
+        throw py::python_error(); \
+      \
+      if (arg_value.ptr() && isinstance_result) \
         msg.append( \
             " (perhaps you meant to pass 'array.data' instead of the array itself?)"); \
       throw error(err.routine().c_str(), err.code(), msg.c_str()); \
     } \
     catch (std::exception &err) \
     { \
       std::string msg( \
@@ -5421,66 +5465,67 @@
   };
 
 
 
 
 #define PYOPENCL_WRAP_BUFFER_CREATOR(TYPE, NAME, CL_NAME, ARGS, CL_ARGS) \
   inline \
-  TYPE *NAME ARGS \
+  void NAME ARGS \
   { \
     cl_int status_code; \
     PYOPENCL_PRINT_CALL_TRACE(#CL_NAME); \
     cl_mem mem = CL_NAME CL_ARGS; \
     \
     if (status_code != CL_SUCCESS) \
       throw pyopencl::error(#CL_NAME, status_code); \
     \
     try \
     { \
-      return new TYPE(mem, false); \
+      new (self) TYPE(mem, false); \
     } \
     catch (...) \
     { \
       PYOPENCL_CALL_GUARDED(clReleaseMemObject, (mem)); \
       throw; \
     } \
   }
 
 
 
 
   PYOPENCL_WRAP_BUFFER_CREATOR(gl_buffer,
       create_from_gl_buffer, clCreateFromGLBuffer,
-      (context &ctx, cl_mem_flags flags, GLuint bufobj),
+      (gl_buffer *self, context &ctx, cl_mem_flags flags, GLuint bufobj),
       (ctx.data(), flags, bufobj, &status_code));
   PYOPENCL_WRAP_BUFFER_CREATOR(gl_texture,
       create_from_gl_texture_2d, clCreateFromGLTexture2D,
-      (context &ctx, cl_mem_flags flags,
+      (gl_texture *self, context &ctx, cl_mem_flags flags,
          GLenum texture_target, GLint miplevel, GLuint texture),
       (ctx.data(), flags, texture_target, miplevel, texture, &status_code));
   PYOPENCL_WRAP_BUFFER_CREATOR(gl_texture,
       create_from_gl_texture_3d, clCreateFromGLTexture3D,
-      (context &ctx, cl_mem_flags flags,
+      (gl_texture *self, context &ctx, cl_mem_flags flags,
          GLenum texture_target, GLint miplevel, GLuint texture),
       (ctx.data(), flags, texture_target, miplevel, texture, &status_code));
   PYOPENCL_WRAP_BUFFER_CREATOR(gl_renderbuffer,
       create_from_gl_renderbuffer, clCreateFromGLRenderbuffer,
-      (context &ctx, cl_mem_flags flags, GLuint renderbuffer),
+      (gl_renderbuffer *self, context &ctx, cl_mem_flags flags, GLuint renderbuffer),
       (ctx.data(), flags, renderbuffer, &status_code));
 
   inline
-  gl_texture *create_from_gl_texture(
+  void create_from_gl_texture(
+      gl_texture *self,
       context &ctx, cl_mem_flags flags,
       GLenum texture_target, GLint miplevel,
       GLuint texture, unsigned dims)
   {
     if (dims == 2)
-      return create_from_gl_texture_2d(ctx, flags, texture_target, miplevel, texture);
+      return create_from_gl_texture_2d(self, ctx, flags, texture_target, miplevel, texture);
     else if (dims == 3)
-      return create_from_gl_texture_3d(ctx, flags, texture_target, miplevel, texture);
+      return create_from_gl_texture_3d(self, ctx, flags, texture_target, miplevel, texture);
     else
       throw pyopencl::error("Image", CL_INVALID_VALUE,
           "invalid dimension");
   }
 
 
 
@@ -5738,15 +5783,15 @@
       py::object shape, py::object dtype,
       py::object order_py)
   {
     memory_object_holder const &mem_obj =
       py::cast<memory_object_holder const &>(mem_obj_py);
     PyArray_Descr *tp_descr;
     if (PyArray_DescrConverter(dtype.ptr(), &tp_descr) != NPY_SUCCEED)
-      throw py::error_already_set();
+      throw py::python_error();
     cl_mem_flags mem_flags;
     PYOPENCL_CALL_GUARDED(clGetMemObjectInfo,
             (mem_obj.data(), CL_MEM_FLAGS, sizeof(mem_flags), &mem_flags, 0));
     if (!(mem_flags & CL_MEM_USE_HOST_PTR))
       throw pyopencl::error("MemoryObject.get_host_array", CL_INVALID_VALUE,
                             "Only MemoryObject with USE_HOST_PTR "
                             "is supported.");
@@ -5758,45 +5803,46 @@
     }
     catch (py::cast_error &)
     {
       for (auto it: shape)
         dims.push_back(py::cast<npy_intp>(it));
     }
 
-    NPY_ORDER order = PyArray_CORDER;
+    NPY_ORDER order = NPY_CORDER;
     PyArray_OrderConverter(order_py.ptr(), &order);
 
     int ary_flags = 0;
-    if (order == PyArray_FORTRANORDER)
+    if (order == NPY_FORTRANORDER)
       ary_flags |= NPY_FARRAY;
-    else if (order == PyArray_CORDER)
+    else if (order == NPY_CORDER)
       ary_flags |= NPY_CARRAY;
     else
       throw std::runtime_error("unrecognized order specifier");
 
     void *host_ptr;
     size_t mem_obj_size;
     PYOPENCL_CALL_GUARDED(clGetMemObjectInfo,
         (mem_obj.data(), CL_MEM_HOST_PTR, sizeof(host_ptr),
          &host_ptr, 0));
     PYOPENCL_CALL_GUARDED(clGetMemObjectInfo,
         (mem_obj.data(), CL_MEM_SIZE, sizeof(mem_obj_size),
          &mem_obj_size, 0));
 
-    py::object result = py::reinterpret_steal<py::object>(PyArray_NewFromDescr(
+    py::object result = py::steal<py::object>(PyArray_NewFromDescr(
         &PyArray_Type, tp_descr,
         dims.size(), &dims.front(), /*strides*/ nullptr,
         host_ptr, ary_flags, /*obj*/nullptr));
+    PyArrayObject *result_arr = (PyArrayObject *) result.ptr();
 
-    if ((size_t) PyArray_NBYTES(result.ptr()) > mem_obj_size)
+    if ((size_t) PyArray_NBYTES(result_arr) > mem_obj_size)
       throw pyopencl::error("MemoryObject.get_host_array",
           CL_INVALID_VALUE,
           "Resulting array is larger than memory object.");
 
-    PyArray_BASE(result.ptr()) = mem_obj_py.ptr();
+    PyArray_SetBaseObject(result_arr, mem_obj_py.ptr());
     Py_INCREF(mem_obj_py.ptr());
 
     return result;
   }
 #endif
 
   // }}}
```

### Comparing `pyopencl-2024.1/src/wrap_cl_part_1.cpp` & `pyopencl-2024.2/src/wrap_cl_part_1.cpp`

 * *Files 12% similar despite different names*

```diff
@@ -43,30 +43,28 @@
 
   {
     typedef platform cls;
     py::class_<cls>(m, "Platform", py::dynamic_attr())
       .DEF_SIMPLE_METHOD(get_info)
       .def("get_devices", &cls::get_devices,
           py::arg("device_type")=CL_DEVICE_TYPE_ALL)
-      .def(py::self == py::self)
-      .def(py::self != py::self)
       .def("__hash__", &cls::hash)
+      PYOPENCL_EXPOSE_EQUALITY_TESTS
       PYOPENCL_EXPOSE_TO_FROM_INT_PTR(cl_platform_id)
       ;
   }
 
   // }}}
 
   // {{{ device
   {
     typedef device cls;
     py::class_<cls>(m, "Device", py::dynamic_attr())
       .DEF_SIMPLE_METHOD(get_info)
-      .def(py::self == py::self)
-      .def(py::self != py::self)
+      PYOPENCL_EXPOSE_EQUALITY_TESTS
       .def("__hash__", &cls::hash)
 #if PYOPENCL_CL_VERSION >= 0x1020
       .DEF_SIMPLE_METHOD(create_sub_devices)
 #endif
       PYOPENCL_EXPOSE_TO_FROM_INT_PTR(cl_device_id)
 #if PYOPENCL_CL_VERSION >= 0x2010
       .DEF_SIMPLE_METHOD(device_and_host_timer)
@@ -77,78 +75,76 @@
 
   // }}}
 
   // {{{ context
 
   {
     typedef context cls;
-    py::class_<cls, std::shared_ptr<cls>>(m, "Context", py::dynamic_attr())
+    py::class_<cls>(m, "Context", py::dynamic_attr(), py::is_weak_referenceable())
       .def(
-          py::init(
-            [](py::object py_devices, py::object py_properties,
-              py::object py_dev_type)
-            {
-              PYOPENCL_RETRY_RETURN_IF_MEM_ERROR(
-                  return create_context_inner(
-                    py_devices,
-                    py_properties,
-                    py_dev_type);
-              )
-            }),
+          "__init__",
+          [](cls *self, py::object py_devices, py::object py_properties,
+            py::object py_dev_type)
+          {
+            PYOPENCL_RETRY_IF_MEM_ERROR(
+                create_context_inner(
+                  self,
+                  py_devices,
+                  py_properties,
+                  py_dev_type);
+            )
+          },
           py::arg("devices").none(true)=py::none(),
           py::arg("properties").none(true)=py::none(),
           py::arg("dev_type").none(true)=py::none()
           )
       .DEF_SIMPLE_METHOD(get_info)
-      .def(py::self == py::self)
-      .def(py::self != py::self)
+      PYOPENCL_EXPOSE_EQUALITY_TESTS
       .def("__hash__", &cls::hash)
       PYOPENCL_EXPOSE_TO_FROM_INT_PTR(cl_context)
 #if PYOPENCL_CL_VERSION >= 0x2010
       .DEF_SIMPLE_METHOD(set_default_device_command_queue)
 #endif
       ;
   }
 
   // }}}
 
   // {{{ command queue
   {
     typedef command_queue cls;
-    py::class_<cls, std::shared_ptr<cls>>(m, "CommandQueue", py::dynamic_attr())
+    py::class_<cls>(m, "CommandQueue", py::dynamic_attr())
       .def(
         py::init<const context &, const device *, py::object>(),
         py::arg("context"),
         py::arg("device").none(true)=py::none(),
         py::arg("properties")=py::cast(0))
       .def("_finalize", &cls::finalize)
       .DEF_SIMPLE_METHOD(get_info)
 #if PYOPENCL_CL_VERSION < 0x1010
       .DEF_SIMPLE_METHOD(set_property)
 #endif
       .DEF_SIMPLE_METHOD(flush)
       .DEF_SIMPLE_METHOD(finish)
-      .def(py::self == py::self)
-      .def(py::self != py::self)
+      PYOPENCL_EXPOSE_EQUALITY_TESTS
       .def("__hash__", &cls::hash)
       PYOPENCL_EXPOSE_TO_FROM_INT_PTR(cl_command_queue)
       ;
   }
 
   // }}}
 
   // {{{ events/synchronization
   {
     typedef event cls;
-    py::class_<cls>(m, "Event", py::dynamic_attr())
+    py::class_<cls>(m, "Event")
       .DEF_SIMPLE_METHOD(get_info)
       .DEF_SIMPLE_METHOD(get_profiling_info)
       .DEF_SIMPLE_METHOD(wait)
-      .def(py::self == py::self)
-      .def(py::self != py::self)
+      PYOPENCL_EXPOSE_EQUALITY_TESTS
       .def("__hash__", &cls::hash)
       PYOPENCL_EXPOSE_TO_FROM_INT_PTR(cl_event)
 #if PYOPENCL_CL_VERSION >= 0x1010
       .DEF_SIMPLE_METHOD(set_callback)
 #endif
       ;
   }
@@ -179,19 +175,17 @@
 #endif
   m.def("_enqueue_barrier", enqueue_barrier, py::arg("queue"));
 
 #if PYOPENCL_CL_VERSION >= 0x1010
   {
     typedef user_event cls;
     py::class_<cls, event>(m, "UserEvent", py::dynamic_attr())
-      .def(py::init(
-            [](context &ctx)
-            {
-              return create_user_event(ctx);
-            }),
+      .def("__init__",
+          [](cls *self, context &ctx)
+          { create_user_event(self, ctx); },
           py::arg("context"))
       .DEF_SIMPLE_METHOD(set_status)
       ;
   }
 #endif
 
   // }}}
@@ -205,30 +199,29 @@
   // FIXME: Reenable in pypy
 #ifndef PYPY_VERSION
       .def("get_host_array", get_mem_obj_host_array,
           py::arg("shape"),
           py::arg("dtype"),
           py::arg("order")="C")
 #endif
-      .def("__eq__", [](const cls &self, const cls &other){ return self == other; })
-      .def("__ne__", [](const cls &self, const cls &other){ return self != other; })
+      PYOPENCL_EXPOSE_EQUALITY_TESTS
       .def("__hash__", &cls::hash)
 
-      .def_property_readonly("int_ptr", to_int_ptr<cls>,
+      .def_prop_ro("int_ptr", to_int_ptr<cls>,
           "Return an integer corresponding to the pointer value "
           "of the underlying :c:type:`cl_mem`. "
           "Use :meth:`from_int_ptr` to turn back into a Python object."
           "\n\n.. versionadded:: 2013.2\n")
       ;
   }
   {
     typedef memory_object cls;
     py::class_<cls, memory_object_holder>(m, "MemoryObject", py::dynamic_attr())
       .DEF_SIMPLE_METHOD(release)
-      .def_property_readonly("hostbuf", &cls::hostbuf)
+      .def_prop_ro("hostbuf", &cls::hostbuf)
 
       .def_static("from_int_ptr", memory_object_from_int,
         "(static method) Return a new Python object referencing the C-level "
         ":c:type:`cl_mem` object at the location pointed to "
         "by *int_ptr_value*. The relevant ``clRetain*`` function "
         "will be called if *retain* is True."
         "If the previous owner of the object will *not* release the reference, "
@@ -253,18 +246,17 @@
   // }}}
 
   // {{{ buffer
   {
     typedef buffer cls;
     py::class_<cls, memory_object>(m, "Buffer", py::dynamic_attr())
       .def(
-          py::init(
-            [](context &ctx, cl_mem_flags flags, size_t size, py::object py_hostbuf)
-            { return create_buffer_py(ctx, flags, size, py_hostbuf); }
-            ),
+          "__init__",
+          [](cls *self, context &ctx, cl_mem_flags flags, size_t size, py::object py_hostbuf)
+          { create_buffer_py(self, ctx, flags, size, py_hostbuf); },
           py::arg("context"),
           py::arg("flags"),
           py::arg("size")=0,
           py::arg("hostbuf").none(true)=py::none()
           )
 #if PYOPENCL_CL_VERSION >= 0x1010
       .def("get_sub_region", &cls::get_sub_region,
```

### Comparing `pyopencl-2024.1/src/wrap_cl_part_2.cpp` & `pyopencl-2024.2/src/wrap_cl_part_2.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -61,30 +61,14 @@
     if (mobj)
       desc.buffer = mobj->data();
     else
       desc.buffer = 0;
   }
 
 #endif
-
-#if PYOPENCL_CL_VERSION >= 0x2000
-  class svm_pointer_as_buffer
-  {
-    private:
-      svm_pointer &m_ptr;
-
-    public:
-      svm_pointer_as_buffer(svm_pointer &ptr)
-        : m_ptr(ptr)
-      { }
-
-      svm_pointer &ptr() const
-      { return m_ptr; }
-  };
-#endif
 }
 
 
 
 
 using namespace pyopencl;
 
@@ -96,59 +80,63 @@
   // {{{ image
 
 #if PYOPENCL_CL_VERSION >= 0x1020
   {
     typedef cl_image_desc cls;
     py::class_<cls>(m, "ImageDescriptor")
       .def(py::init<>())
-      .def_readwrite("image_type", &cls::image_type)
-      .def_property("shape", &image_desc_dummy_getter, image_desc_set_shape)
-      .def_readwrite("array_size", &cls::image_array_size)
-      .def_property("pitches", &image_desc_dummy_getter, image_desc_set_pitches)
-      .def_readwrite("num_mip_levels", &cls::num_mip_levels)
-      .def_readwrite("num_samples", &cls::num_samples)
-      .def_property("buffer", &image_desc_dummy_getter, image_desc_set_buffer)
+      .def_rw("image_type", &cls::image_type)
+      .def_prop_rw("shape", &image_desc_dummy_getter, image_desc_set_shape)
+      .def_rw("array_size", &cls::image_array_size)
+      .def_prop_rw("pitches", &image_desc_dummy_getter, image_desc_set_pitches)
+      .def_rw("num_mip_levels", &cls::num_mip_levels)
+      .def_rw("num_samples", &cls::num_samples)
+      .def_prop_rw("buffer", &image_desc_dummy_getter, image_desc_set_buffer,
+                   py::arg("buffer").none()
+                 )
       ;
   }
 #endif
 
   {
     typedef image cls;
     py::class_<cls, memory_object>(m, "Image", py::dynamic_attr())
       .def(
-          py::init(
-            [](
-              context const &ctx,
-              cl_mem_flags flags,
-              cl_image_format const &fmt,
-              py::sequence shape,
-              py::sequence pitches,
-              py::object buffer)
-            {
-              return create_image(ctx, flags, fmt, shape, pitches, buffer);
-            }),
+          "__init__",
+          [](
+            cls *self,
+            context const &ctx,
+            cl_mem_flags flags,
+            cl_image_format const &fmt,
+            py::sequence shape,
+            py::sequence pitches,
+            py::object buffer)
+          {
+            return create_image(self, ctx, flags, fmt, shape, pitches, buffer);
+          },
           py::arg("context"),
           py::arg("flags"),
           py::arg("format"),
           py::arg("shape")=py::none(),
           py::arg("pitches")=py::none(),
           py::arg("hostbuf")=py::none()
           )
 #if PYOPENCL_CL_VERSION >= 0x1020
       .def(
-          py::init(
-            [](
-              context const &ctx,
-              cl_mem_flags flags,
-              cl_image_format const &fmt,
-              cl_image_desc &desc,
-              py::object buffer)
-            {
-              return create_image_from_desc(ctx, flags, fmt, desc, buffer);
-            }),
+          "__init__",
+          [](
+            cls *self,
+            context const &ctx,
+            cl_mem_flags flags,
+            cl_image_format const &fmt,
+            cl_image_desc &desc,
+            py::object buffer)
+          {
+            create_image_from_desc(self, ctx, flags, fmt, desc, buffer);
+          },
           py::arg("context"),
           py::arg("flags"),
           py::arg("format"),
           py::arg("desc"),
           py::arg("hostbuf")=py::none()
           )
 #endif
@@ -156,24 +144,24 @@
       ;
   }
 
   {
     typedef cl_image_format cls;
     py::class_<cls>(m, "ImageFormat")
       .def(
-          py::init(
-            [](cl_channel_order ord, cl_channel_type tp)
-            {
-              return make_image_format(ord, tp);
-            }))
-      .def_readwrite("channel_order", &cls::image_channel_order)
-      .def_readwrite("channel_data_type", &cls::image_channel_data_type)
-      .def_property_readonly("channel_count", &get_image_format_channel_count)
-      .def_property_readonly("dtype_size", &get_image_format_channel_dtype_size)
-      .def_property_readonly("itemsize", &get_image_format_item_size)
+          "__init__",
+          [](cls *self, cl_channel_order ord, cl_channel_type tp)
+          {
+            set_image_format(self, ord, tp);
+          })
+      .def_rw("channel_order", &cls::image_channel_order)
+      .def_rw("channel_data_type", &cls::image_channel_data_type)
+      .def_prop_ro("channel_count", &get_image_format_channel_count)
+      .def_prop_ro("dtype_size", &get_image_format_channel_dtype_size)
+      .def_prop_ro("itemsize", &get_image_format_item_size)
       ;
   }
 
   DEF_SIMPLE_FUNCTION(get_supported_image_formats);
 
   m.def("_enqueue_read_image", enqueue_read_image,
       py::arg("queue"),
@@ -242,24 +230,25 @@
   // {{{ pipe
 
   {
     typedef pyopencl::pipe cls;
     py::class_<cls, memory_object>(m, "Pipe", py::dynamic_attr())
 #if PYOPENCL_CL_VERSION >= 0x2000
       .def(
-          py::init(
-            [](
-              context const &ctx,
-              cl_mem_flags flags,
-              cl_uint pipe_packet_size,
-              cl_uint pipe_max_packets,
-              py::sequence py_props)
-            {
-              return create_pipe(ctx, flags, pipe_packet_size, pipe_max_packets, py_props);
-            }),
+          "__init__",
+          [](
+            cls *self,
+            context const &ctx,
+            cl_mem_flags flags,
+            cl_uint pipe_packet_size,
+            cl_uint pipe_max_packets,
+            py::sequence py_props)
+          {
+            create_pipe(self, ctx, flags, pipe_packet_size, pipe_max_packets, py_props);
+          },
           py::arg("context"),
           py::arg("flags"),
           py::arg("packet_size"),
           py::arg("max_packets"),
           py::arg("properties")=py::make_tuple()
           )
 #endif
@@ -314,64 +303,46 @@
 #if PYOPENCL_CL_VERSION >= 0x2000
   {
     typedef svm_pointer cls;
     py::class_<cls>(m, "SVMPointer", py::dynamic_attr())
       // For consistency, it may seem appropriate to use int_ptr here, but
       // that would work on both buffers and SVM, and passing a buffer pointer to
       // a kernel is going to lead to a bad time.
-      .def_property_readonly("svm_ptr",
+      .def_prop_ro("svm_ptr",
           [](cls &self) { return (intptr_t) self.svm_ptr(); })
-      .def_property_readonly("size", [](cls &self) -> py::object
+      .def_prop_ro("size", [](cls &self) -> py::object
           {
             try
             {
               return py::cast(self.size());
             }
             catch (size_not_available)
             {
               return py::none();
             }
           })
-      .def_property_readonly("buf", [](cls &self) -> svm_pointer_as_buffer * {
-            return new svm_pointer_as_buffer(self);
-          }, py::return_value_policy::reference_internal)
-      ;
-  }
-
-  {
-    typedef svm_pointer_as_buffer cls;
-    py::class_<cls>(m, "_SVMPointerAsBuffer", pybind11::buffer_protocol())
-      .def_buffer([](cls &self) -> pybind11::buffer_info
-          {
+      .def_prop_ro("buf", [](cls &self) -> py::ndarray<py::numpy, unsigned char, py::ndim<1>> {
             size_t size;
             try
             {
-              size = self.ptr().size();
+              size = self.size();
             }
             catch (size_not_available)
             {
               throw pyopencl::error("SVMPointer buffer protocol", CL_INVALID_VALUE,
                   "size of SVM is not known");
             }
-            return pybind11::buffer_info(
-                // Pointer to buffer
-                self.ptr().svm_ptr(),
-                // Size of one scalar
-                sizeof(unsigned char),
-                // Python struct-style format descriptor
-                pybind11::format_descriptor<unsigned char>::format(),
-                // Number of dimensions
-                1,
-                // Buffer dimensions
-                { size },
-                // Strides (in bytes) for each index
-                { sizeof(unsigned char) }
-                );
-          })
-    ;
+
+            return py::ndarray<py::numpy, unsigned char, py::ndim<1>>(
+              /* data = */ self.svm_ptr(),
+              /* ndim = */ 1,
+              /* shape pointer = */ &size,
+              /* owner = */ py::handle());
+          }, py::rv_policy::reference_internal)
+      ;
   }
 
   // }}}
 
   // {{{ svm_arg_wrapper
 
   {
@@ -398,23 +369,22 @@
       .DEF_SIMPLE_METHOD(release)
       .def("enqueue_release", &cls::enqueue_release,
           ":returns: a :class:`pyopencl.Event`\n\n"
           "|std-enqueue-blurb|",
           py::arg("queue").none(true)=py::none(),
           py::arg("wait_for").none(true)=py::none()
           )
-      .def(py::self == py::self)
-      .def(py::self != py::self)
+      PYOPENCL_EXPOSE_EQUALITY_TESTS
       .def("__hash__", [](cls &self) { return (intptr_t) self.svm_ptr(); })
       .def("bind_to_queue", &cls::bind_to_queue,
           py::arg("queue"))
       .DEF_SIMPLE_METHOD(unbind_from_queue)
 
       // only for diagnostic/debugging/testing purposes!
-      .def_property_readonly("_queue",
+      .def_prop_ro("_queue",
           [](cls const &self) -> py::object
           {
             cl_command_queue queue = self.queue();
             if (queue)
               return py::cast(new command_queue(queue, true));
             else
               return py::none();
@@ -475,16 +445,15 @@
     typedef sampler cls;
     py::class_<cls>(m, "Sampler", py::dynamic_attr())
 #if PYOPENCL_CL_VERSION >= 0x2000
       .def(py::init<context const &, py::sequence>())
 #endif
       .def(py::init<context const &, bool, cl_addressing_mode, cl_filter_mode>())
       .DEF_SIMPLE_METHOD(get_info)
-      .def(py::self == py::self)
-      .def(py::self != py::self)
+      PYOPENCL_EXPOSE_EQUALITY_TESTS
       .def("__hash__", &cls::hash)
       PYOPENCL_EXPOSE_TO_FROM_INT_PTR(cl_sampler)
       ;
   }
 
   // }}}
 
@@ -496,27 +465,27 @@
       .value("SOURCE", cls::KND_SOURCE)
       .value("BINARY", cls::KND_BINARY)
       .value("IL", cls::KND_IL)
       ;
 
     py::class_<cls>(m, "_Program", py::dynamic_attr())
       .def(
-          py::init(
-            [](context &ctx, std::string const &src)
-            {
-              return create_program_with_source(ctx, src);
-            }),
+          "__init__",
+          [](cls *self, context &ctx, std::string const &src)
+          {
+            create_program_with_source(self, ctx, src);
+          },
           py::arg("context"),
           py::arg("src"))
       .def(
-          py::init(
-            [](context &ctx, py::sequence devices, py::sequence binaries)
-            {
-              return create_program_with_binary(ctx, devices, binaries);
-            }),
+          "__init__",
+          [](cls *self, context &ctx, py::sequence devices, py::sequence binaries)
+          {
+            return create_program_with_binary(self, ctx, devices, binaries);
+          },
           py::arg("context"),
           py::arg("devices"),
           py::arg("binaries"))
 #if (PYOPENCL_CL_VERSION >= 0x1020) || \
       ((PYOPENCL_CL_VERSION >= 0x1030) && defined(__APPLE__))
       .def_static("create_with_built_in_kernels",
           create_program_with_built_in_kernels,
@@ -543,16 +512,15 @@
           )
 #endif
 #if PYOPENCL_CL_VERSION >= 0x2020
       .def("set_specialization_constant", &cls::set_specialization_constant,
           py::arg("spec_id"),
           py::arg("buffer"))
 #endif
-      .def(py::self == py::self)
-      .def(py::self != py::self)
+      PYOPENCL_EXPOSE_EQUALITY_TESTS
       .def("__hash__", &cls::hash)
       .def("all_kernels", create_kernels_in_program)
       PYOPENCL_EXPOSE_TO_FROM_INT_PTR(cl_program)
       ;
   }
 
 #if (PYOPENCL_CL_VERSION >= 0x2010)
@@ -603,16 +571,15 @@
                 { knl.set_arg_buf_pack(i, typechar, arg); },
                 indices_chars_and_args);
           })
       .DEF_SIMPLE_METHOD(set_arg)
 #if PYOPENCL_CL_VERSION >= 0x1020
       .DEF_SIMPLE_METHOD(get_arg_info)
 #endif
-      .def(py::self == py::self)
-      .def(py::self != py::self)
+      PYOPENCL_EXPOSE_EQUALITY_TESTS
       .def("__hash__", &cls::hash)
       PYOPENCL_EXPOSE_TO_FROM_INT_PTR(cl_kernel)
 #if PYOPENCL_CL_VERSION >= 0x2010
       .def("get_sub_group_info", &cls::get_sub_group_info,
           py::arg("device"),
           py::arg("param"),
           py::arg("input_value").none(true)=py::none()
@@ -623,15 +590,15 @@
 
   {
     typedef local_memory cls;
     py::class_<cls>(m, "LocalMemory", py::dynamic_attr())
       .def(
           py::init<size_t>(),
           py::arg("size"))
-      .def_property_readonly("size", &cls::size)
+      .def_prop_ro("size", &cls::size)
       ;
   }
 
   m.def("enqueue_nd_range_kernel", enqueue_nd_range_kernel,
       py::arg("queue"),
       py::arg("kernel"),
       py::arg("global_work_size"),
@@ -654,52 +621,52 @@
   DEF_SIMPLE_FUNCTION(get_apple_cgl_share_group);
 #endif /* __APPLE__ */
 
   {
     typedef gl_buffer cls;
     py::class_<cls, memory_object>(m, "GLBuffer", py::dynamic_attr())
       .def(
-          py::init(
-            [](context &ctx, cl_mem_flags flags, GLuint bufobj)
-            {
-              return create_from_gl_buffer(ctx, flags, bufobj);
-            }),
+          "__init__",
+          [](cls *self, context &ctx, cl_mem_flags flags, GLuint bufobj)
+          {
+            create_from_gl_buffer(self, ctx, flags, bufobj);
+          },
           py::arg("context"),
           py::arg("flags"),
           py::arg("bufobj"))
       .def("get_gl_object_info", get_gl_object_info)
       ;
   }
 
   {
     typedef gl_renderbuffer cls;
     py::class_<cls, memory_object>(m, "GLRenderBuffer", py::dynamic_attr())
       .def(
-          py::init(
-            [](context &ctx, cl_mem_flags flags, GLuint bufobj)
-            {
-              return create_from_gl_renderbuffer(ctx, flags, bufobj);
-            }),
+          "__init__",
+          [](cls *self, context &ctx, cl_mem_flags flags, GLuint bufobj)
+          {
+            create_from_gl_renderbuffer(self, ctx, flags, bufobj);
+          },
           py::arg("context"),
           py::arg("flags"),
           py::arg("bufobj"))
       .def("get_gl_object_info", get_gl_object_info)
       ;
   }
 
   {
     typedef gl_texture cls;
     py::class_<cls, image>(m, "GLTexture", py::dynamic_attr())
       .def(
-          py::init(
-            [](context &ctx, cl_mem_flags flags, GLenum texture_target,
-              GLint miplevel, GLuint texture, unsigned dims)
-            {
-              return create_from_gl_texture(ctx, flags, texture_target, miplevel, texture, dims);
-            }),
+          "__init__",
+          [](cls *self, context &ctx, cl_mem_flags flags, GLenum texture_target,
+            GLint miplevel, GLuint texture, unsigned dims)
+          {
+            create_from_gl_texture(self, ctx, flags, texture_target, miplevel, texture, dims);
+          },
           py::arg("context"),
           py::arg("flags"),
           py::arg("texture_target"),
           py::arg("miplevel"),
           py::arg("texture"),
           py::arg("dims"))
       .def("get_gl_object_info", get_gl_object_info)
```

### Comparing `pyopencl-2024.1/src/wrap_constants.cpp` & `pyopencl-2024.2/src/wrap_constants.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
     DECLARE_EXC(Error, PyExc_Exception);
     DECLARE_EXC(MemoryError, CLError.ptr());
     DECLARE_EXC(LogicError, CLError.ptr());
     DECLARE_EXC(RuntimeError, CLError.ptr());
 
     py::register_exception_translator(
-        [](std::exception_ptr p)
+        [](const std::exception_ptr &p, void * /* unused */)
         {
           try
           {
             if (p) std::rethrow_exception(p);
           }
           catch (pyopencl::error &err)
           {
@@ -135,21 +135,21 @@
   // }}}
 
   // {{{ error record
 
   {
     typedef error cls;
     py::class_<error> (m, "_ErrorRecord")
-      .def(py::init<const char *, cl_int, const char *>(),
+      .def(py::init<const std::string &, cl_int, const std::string &>(),
           py::arg("routine"),
           py::arg("code"),
           py::arg("msg"))
       .DEF_SIMPLE_METHOD(routine)
       .DEF_SIMPLE_METHOD(code)
-      .DEF_SIMPLE_METHOD(what)
+      .def("what", &cls::err_what)
       .DEF_SIMPLE_METHOD(is_out_of_memory)
       .def("_program", &cls::get_program)
       ;
   }
 
   // }}}
 
@@ -1190,76 +1190,80 @@
   // }}}
 
   // {{{ cl_name_version
 #if PYOPENCL_CL_VERSION >= 0x3000
   {
     typedef cl_name_version cls;
     py::class_<cls>(m, "NameVersion")
-      .def(py::init(
-            [](cl_version version, const char* name)
-            {
-              cl_name_version result;
-              result.version = version;
-              result.name[0] = '\0';
-              // https://stackoverflow.com/a/1258577
-              strncat(result.name, name, CL_NAME_VERSION_MAX_NAME_SIZE-1);
-              return result;
-            }),
+      .def("__init__",
+          [](cls *self, cl_version version, const std::string &name)
+          {
+            self->version = version;
+            self->name[0] = '\0';
+            // https://stackoverflow.com/a/1258577
+            strncat(self->name, name.c_str(), CL_NAME_VERSION_MAX_NAME_SIZE-1);
+          },
           py::arg("version")=0,
-          py::arg("name")=0)
+          py::arg("name")=0
+          )
 
-      .def_property("version",
+      .def_prop_rw("version",
           [](cls &t) { return t.version; },
           [](cls &t, cl_version val) { t.version = val; })
-      .def_property("name",
+      .def_prop_rw("name",
           [](cls &t) { return t.name; },
-          [](cls &t, const char *name)
+          [](cls &t, const std::string &name)
           {
               t.name[0] = '\0';
               // https://stackoverflow.com/a/1258577
-              strncat(t.name, name, CL_NAME_VERSION_MAX_NAME_SIZE-1);
+              strncat(t.name, name.c_str(), CL_NAME_VERSION_MAX_NAME_SIZE-1);
           })
       ;
   }
 #endif
   // }}}
 
   // {{{ CL_DEVICE_TOPOLOGY_AMD
 
 #ifdef CL_DEVICE_TOPOLOGY_AMD
   {
     typedef cl_device_topology_amd cls;
     py::class_<cls>(m, "DeviceTopologyAmd")
-      .def(py::init(
-            [](cl_char bus, cl_char device, cl_char function)
-            {
-              cl_device_topology_amd result;
-              result.pcie.type = CL_DEVICE_TOPOLOGY_TYPE_PCIE_AMD;
-              result.pcie.bus = bus;
-              result.pcie.device = device;
-              result.pcie.function = function;
-              return result;
-            }),
+      .def("__init__",
+
+          // FIXME: Nanobind thinks of 'char' as "short string", not small integer.
+          // The detour via cl_int may lose data on assignment.
+          // [](cl_char bus, cl_char device, cl_char function)
+          [](cls *self, cl_int bus, cl_int device, cl_int function)
+          {
+            self->pcie.type = CL_DEVICE_TOPOLOGY_TYPE_PCIE_AMD;
+            self->pcie.bus = (cl_char) bus;
+            self->pcie.device = (cl_char) device;
+            self->pcie.function = (cl_char) function;
+          },
           py::arg("bus")=0,
           py::arg("device")=0,
           py::arg("function")=0)
 
-      .def_property("type",
+      .def_prop_rw("type",
           [](cls &t) { return t.pcie.type; },
           [](cls &t, cl_uint val) { t.pcie.type = val; })
 
-      .def_property("bus",
+      .def_prop_rw("bus",
           [](cls &t) { return t.pcie.bus; },
-          [](cls &t, cl_char val) { t.pcie.bus = val; })
-      .def_property("device",
+          // FIXME: Revert to cl_char when possible
+          [](cls &t, cl_int val) { t.pcie.bus = (cl_char) val; })
+      .def_prop_rw("device",
           [](cls &t) { return t.pcie.device; },
-          [](cls &t, cl_char val) { t.pcie.device = val; })
-      .def_property("function",
+          // FIXME: Revert to cl_char when possible
+          [](cls &t, cl_int val) { t.pcie.device = (cl_char) val; })
+      .def_prop_rw("function",
           [](cls &t) { return t.pcie.function; },
-          [](cls &t, cl_char val) { t.pcie.function = val; })
+          // FIXME: Revert to cl_char when possible
+          [](cls &t, cl_int val) { t.pcie.function = (cl_char) val; })
       ;
   }
 #endif
 
   // }}}
 
 }
```

### Comparing `pyopencl-2024.1/src/wrap_helpers.hpp` & `pyopencl-2024.2/src/wrap_helpers.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -24,24 +24,28 @@
 // OTHER DEALINGS IN THE SOFTWARE.
 
 
 #ifndef PYCUDA_WRAP_HELPERS_HEADER_SEEN
 #define PYCUDA_WRAP_HELPERS_HEADER_SEEN
 
 
-#include <pybind11/pybind11.h>
-#include <pybind11/operators.h>
+#include <nanobind/nanobind.h>
+#include <nanobind/stl/string.h>
+#include <nanobind/stl/shared_ptr.h>
+#include <nanobind/ndarray.h>
 
 
-namespace py = pybind11;
+namespace py = nanobind;
 
 
 #define ENUM_VALUE(NAME) \
   value(#NAME, NAME)
 
+// {{{ DEF_SIMPLE_XXX
+
 #define DEF_SIMPLE_METHOD(NAME) \
   def(#NAME, &cls::NAME)
 
 #define DEF_SIMPLE_STATIC_METHOD(NAME) \
   def_static(#NAME, &cls::NAME)
 
 #define DEF_SIMPLE_METHOD_WITH_ARGS(NAME, ARGS) \
@@ -116,33 +120,33 @@
   }
 
 // }}}
 
 #define PYOPENCL_PARSE_NUMPY_ARRAY_SPEC \
     PyArray_Descr *tp_descr; \
     if (PyArray_DescrConverter(dtype.ptr(), &tp_descr) != NPY_SUCCEED) \
-      throw py::error_already_set(); \
+      throw py::python_error(); \
     \
     std::vector<npy_intp> shape; \
     try \
     { \
       shape.push_back(py::cast<npy_intp>(py_shape)); \
     } \
     catch (py::cast_error &) \
     { \
       COPY_PY_LIST(npy_intp, shape); \
     } \
     \
-    NPY_ORDER order = PyArray_CORDER; \
+    NPY_ORDER order = NPY_CORDER; \
     PyArray_OrderConverter(py_order.ptr(), &order); \
     \
     int ary_flags = 0; \
-    if (order == PyArray_FORTRANORDER) \
+    if (order == NPY_FORTRANORDER) \
       ary_flags |= NPY_FARRAY; \
-    else if (order == PyArray_CORDER) \
+    else if (order == NPY_CORDER) \
       ary_flags |= NPY_CARRAY; \
     else \
       throw std::runtime_error("unrecognized order specifier"); \
     \
     std::vector<npy_intp> strides; \
     if (py_strides.ptr() != Py_None) \
     { \
@@ -158,15 +162,15 @@
   }
 
 namespace
 {
   template <typename T>
   inline py::object handle_from_new_ptr(T *ptr)
   {
-    return py::cast(ptr, py::return_value_policy::take_ownership);
+    return py::cast(ptr, py::rv_policy::take_ownership);
   }
 
   template <typename T, typename ClType>
   inline T *from_int_ptr(intptr_t obj_ref, bool retain)
   {
     ClType clobj = (ClType) obj_ref;
     return new T(clobj, retain);
@@ -188,14 +192,22 @@
       "by *int_ptr_value*. The relevant ``clRetain*`` function " \
       "will be called if *retain* is True." \
       "If the previous owner of the object will *not* release the reference, " \
       "*retain* should be set to *False*, to effectively transfer ownership to " \
       ":mod:`pyopencl`." \
       "\n\n.. versionadded:: 2013.2\n" \
       "\n\n.. versionchanged:: 2016.1\n\n    *retain* added.") \
-  .def_property_readonly("int_ptr", to_int_ptr<cls>, \
+  .def_prop_ro("int_ptr", to_int_ptr<cls>, \
       "Return an integer corresponding to the pointer value " \
       "of the underlying :c:type:`" #CL_TYPENAME "`. " \
       "Use :meth:`from_int_ptr` to turn back into a Python object." \
       "\n\n.. versionadded:: 2013.2\n") \
 
+#define PYOPENCL_EXPOSE_EQUALITY_TESTS \
+    /* this relies on nanobind overload resolution going in order of registration */ \
+    .def("__eq__", [](cls const &self, cls const &other) { return self == other; }) \
+    .def("__eq__", [](cls const &self, py::object obj) { return false; }, py::arg("obj").none())
+
+
 #endif
+
+// vim: foldmethod=marker
```

### Comparing `pyopencl-2024.1/src/wrap_mempool.cpp` & `pyopencl-2024.2/src/wrap_mempool.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -493,14 +493,21 @@
       cl_command_queue queue() const
       {
         if (m_ptr.queue.is_valid())
           return m_ptr.queue.data();
         else
           return nullptr;
       }
+
+      // This shouldn't be necessary, but somehow nanobind gets unhappy if
+      // it's not there.
+      void free()
+      {
+        super::free();
+      }
   };
 
   // }}}
 
 
   // {{{ svm_allocator_call
 
@@ -550,20 +557,20 @@
 }
 
 
 namespace {
   template<class Wrapper>
   void expose_memory_pool(Wrapper &wrapper)
   {
-    typedef typename Wrapper::type cls;
+    typedef typename Wrapper::Type cls;
     wrapper
-      .def_property_readonly("held_blocks", &cls::held_blocks)
-      .def_property_readonly("active_blocks", &cls::active_blocks)
-      .def_property_readonly("managed_bytes", &cls::managed_bytes)
-      .def_property_readonly("active_bytes", &cls::active_bytes)
+      .def_prop_ro("held_blocks", &cls::held_blocks)
+      .def_prop_ro("active_blocks", &cls::active_blocks)
+      .def_prop_ro("managed_bytes", &cls::managed_bytes)
+      .def_prop_ro("active_bytes", &cls::active_bytes)
       .DEF_SIMPLE_METHOD(bin_number)
       .DEF_SIMPLE_METHOD(alloc_size)
       .DEF_SIMPLE_METHOD(free_held)
       .DEF_SIMPLE_METHOD(stop_holding)
 
       // undoc for now
       .def("_set_trace", &cls::set_trace)
@@ -576,60 +583,62 @@
 
 void pyopencl_expose_mempool(py::module_ &m)
 {
   m.def("bitlog2", pyopencl::bitlog2);
 
   {
     typedef pyopencl::buffer_allocator_base cls;
-    py::class_<cls, std::shared_ptr<cls>> wrapper(m, "AllocatorBase");
+    py::class_<cls> wrapper(m, "AllocatorBase");
     wrapper
       .def("__call__", pyopencl::allocate_from_buffer_allocator, py::arg("size"))
       ;
 
   }
 
   {
     typedef pyopencl::memory_pool<pyopencl::test_allocator> cls;
 
-    py::class_<cls, std::shared_ptr<cls>> wrapper( m, "_TestMemoryPool");
+    py::class_<cls> wrapper(m, "_TestMemoryPool");
     wrapper
-      .def(py::init([](unsigned leading_bits_in_bin_id)
-            { return new cls(
-                std::shared_ptr<pyopencl::test_allocator>(
-                  new pyopencl::test_allocator()),
-                leading_bits_in_bin_id); }),
+      .def("__init__",
+            [](cls *self, unsigned leading_bits_in_bin_id)
+            {
+              new (self) cls(
+                  std::shared_ptr<pyopencl::test_allocator>(
+                    new pyopencl::test_allocator()),
+                leading_bits_in_bin_id);
+            },
           py::arg("leading_bits_in_bin_id")=4
           )
       .def("allocate", [](std::shared_ptr<cls> pool, cls::size_type sz)
           {
             pool->allocate(sz);
             return py::none();
           })
       ;
 
     expose_memory_pool(wrapper);
   }
 
   {
     typedef pyopencl::deferred_buffer_allocator cls;
-    py::class_<cls, pyopencl::buffer_allocator_base, std::shared_ptr<cls>> wrapper(
+    py::class_<cls, pyopencl::buffer_allocator_base> wrapper(
         m, "DeferredAllocator");
     wrapper
-      .def(py::init<
-          std::shared_ptr<pyopencl::context> const &>())
+      .def(py::init<std::shared_ptr<pyopencl::context> const &>())
       .def(py::init<
           std::shared_ptr<pyopencl::context> const &,
           cl_mem_flags>(),
           py::arg("queue"), py::arg("mem_flags"))
       ;
   }
 
   {
     typedef pyopencl::immediate_buffer_allocator cls;
-    py::class_<cls, pyopencl::buffer_allocator_base, std::shared_ptr<cls>> wrapper(
+    py::class_<cls, pyopencl::buffer_allocator_base> wrapper(
         m, "ImmediateAllocator");
     wrapper
       .def(py::init<pyopencl::command_queue &>())
       .def(py::init<pyopencl::command_queue &, cl_mem_flags>(),
           py::arg("queue"), py::arg("mem_flags"))
       ;
   }
@@ -643,15 +652,15 @@
       .def("unbind_from_queue", [](cls &self) { /* no-op */ })
       ;
   }
 
   {
     typedef pyopencl::memory_pool<pyopencl::buffer_allocator_base> cls;
 
-    py::class_<cls, std::shared_ptr<cls>> wrapper( m, "MemoryPool");
+    py::class_<cls> wrapper( m, "MemoryPool");
     wrapper
       .def(py::init<std::shared_ptr<pyopencl::buffer_allocator_base>, unsigned>(),
           py::arg("allocator"),
           py::arg("leading_bits_in_bin_id")=4
           )
       .def("allocate", pyopencl::allocate_from_buffer_pool, py::arg("size"))
       .def("__call__", pyopencl::allocate_from_buffer_pool, py::arg("size"))
@@ -659,19 +668,19 @@
 
     expose_memory_pool(wrapper);
   }
 
 #if PYOPENCL_CL_VERSION >= 0x2000
   {
     typedef pyopencl::svm_allocator cls;
-    py::class_<cls, std::shared_ptr<cls>> wrapper(m, "SVMAllocator");
+    py::class_<cls> wrapper(m, "SVMAllocator");
     wrapper
       .def(py::init<std::shared_ptr<pyopencl::context>  const &, cl_uint, cl_uint, pyopencl::command_queue *>(),
           py::arg("context"),
-          py::kw_only(),
+          /* py::kw_only(), */
           py::arg("alignment")=0,
           py::arg("flags")=CL_MEM_READ_WRITE,
           py::arg("queue").none(true)=nullptr
           )
       .def("__call__", pyopencl::svm_allocator_call, py::arg("size"))
       ;
   }
@@ -684,34 +693,34 @@
       .def("__eq__", [](const cls &self, const cls &other)
           { return self.svm_ptr() == other.svm_ptr(); })
       .def("__hash__", [](cls &self) { return (intptr_t) self.svm_ptr(); })
       .DEF_SIMPLE_METHOD(bind_to_queue)
       .DEF_SIMPLE_METHOD(unbind_from_queue)
 
       // only for diagnostic/debugging/testing purposes!
-      .def_property_readonly("_queue",
+      .def_prop_ro("_queue",
           [](cls const &self) -> py::object
           {
             cl_command_queue queue = self.queue();
             if (queue)
               return py::cast(new pyopencl::command_queue(queue, true));
             else
               return py::none();
           })
       ;
   }
 
   {
     typedef pyopencl::memory_pool<pyopencl::svm_allocator> cls;
 
-    py::class_<cls, std::shared_ptr<cls>> wrapper( m, "SVMPool");
+    py::class_<cls> wrapper( m, "SVMPool");
     wrapper
       .def(py::init<std::shared_ptr<pyopencl::svm_allocator>, unsigned>(),
           py::arg("allocator"),
-          py::kw_only(),
+          /* py::kw_only(), */
           py::arg("leading_bits_in_bin_id")=4
           )
       .def("__call__", pyopencl::allocate_from_svm_pool, py::arg("size"))
       ;
 
     expose_memory_pool(wrapper);
   }
```

### Comparing `pyopencl-2024.1/test/add-vectors-32.spv` & `pyopencl-2024.2/test/add-vectors-32.spv`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/test/add-vectors-64.spv` & `pyopencl-2024.2/test/add-vectors-64.spv`

 * *Files identical despite different names*

### Comparing `pyopencl-2024.1/test/test_algorithm.py` & `pyopencl-2024.2/test/test_algorithm.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,30 +16,31 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
+import sys
+
 import numpy as np
 import numpy.linalg as la
-import sys
+import pytest
 from pytools import memoize
 from test_array import general_clrand
 
-import pytest
-
 import pyopencl as cl
 import pyopencl.array
-from pyopencl.tools import (  # noqa: F401
-        pytest_generate_tests_for_pyopencl as pytest_generate_tests)
-from pyopencl.characterize import has_double_support, has_struct_arg_count_bug
-from pyopencl.scan import (InclusiveScanKernel, ExclusiveScanKernel,
-        GenericScanKernel, GenericDebugScanKernel)
-from pyopencl.characterize import get_pocl_version
+from pyopencl.characterize import (
+    get_pocl_version, has_double_support, has_struct_arg_count_bug)
+from pyopencl.scan import (
+    ExclusiveScanKernel, GenericDebugScanKernel, GenericScanKernel,
+    InclusiveScanKernel)
+from pyopencl.tools import \
+    pytest_generate_tests_for_pyopencl as pytest_generate_tests  # noqa: F401
 
 
 # {{{ elementwise
 
 def test_elwise_kernel(ctx_factory):
     context = ctx_factory()
     queue = cl.CommandQueue(context)
@@ -761,14 +762,15 @@
                 scan_expr="across_seg_boundary ? b : (a+b)", neutral="0",
                 is_segment_start_expr="segflags[i]",
                 output_statement=output_statement,
                 options=[])
 
         np.set_printoptions(threshold=2000)
         from random import randrange
+
         from pyopencl.clrandom import rand as clrand
         for n in scan_test_counts:
             a_dev = clrand(queue, (n,), dtype=dtype, a=0, b=10)
             a = a_dev.get()
 
             if 10 <= n < 20:
                 seg_boundaries_values = [
@@ -843,16 +845,16 @@
 
     dtype = np.int32
 
     from pyopencl.algorithm import RadixSort
     sort = RadixSort(context, "int *ary", key_expr="ary[i]",
             sort_arg_names=["ary"], scan_kernel=scan_kernel)
 
-    from pyopencl.clrandom import RanluxGenerator
-    rng = RanluxGenerator(queue, seed=15)
+    from pyopencl.clrandom import PhiloxGenerator
+    rng = PhiloxGenerator(context, seed=15)
 
     from time import time
 
     # intermediate arrays for largest size cause out-of-memory on low-end GPUs
     for n in scan_test_counts[:-1]:
         if n >= 2000 and isinstance(scan_kernel, GenericDebugScanKernel):
             continue
```

### Comparing `pyopencl-2024.1/test/test_array.py` & `pyopencl-2024.2/test/test_array.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,32 +18,32 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
-import numpy as np
-import numpy.linalg as la
+import operator
+import platform
 import sys
 from itertools import product
 
+import numpy as np
+import numpy.linalg as la
 import pytest
 
 import pyopencl as cl
 import pyopencl.array as cl_array
 import pyopencl.cltypes as cltypes
 import pyopencl.tools as cl_tools
-from pyopencl.tools import (  # noqa: F401
-        pytest_generate_tests_for_pyopencl as pytest_generate_tests)
 from pyopencl.characterize import has_double_support, has_struct_arg_count_bug
+from pyopencl.clrandom import PhiloxGenerator, ThreefryGenerator
+from pyopencl.tools import \
+    pytest_generate_tests_for_pyopencl as pytest_generate_tests  # noqa: F401
 
-from pyopencl.clrandom import RanluxGenerator, PhiloxGenerator, ThreefryGenerator
-import operator
-import platform
 
 _PYPY = cl._PYPY
 
 
 # {{{ helpers
 
 TO_REAL = {
@@ -679,15 +679,14 @@
     from pyopencl.characterize import has_double_support
     if has_double_support(queue.device):
         dtypes = dtypes + (np.float64, np.complex128)
 
     from itertools import product
 
     for dtype_a, dtype_s in product(dtypes, repeat=2):
-
         a = np.array([10, 20, 30, 40, 50, 60, 70, 80, 90, 100]).astype(dtype_a)
         s = dtype_s(40)
         a_gpu = cl_array.to_device(queue, a)
 
         # ensure the same behavior as inplace numpy.ndarray division
         try:
             a /= s
@@ -781,41 +780,57 @@
 
         for op in [o.and_, o.or_, o.xor]:
             res_dev = op(a_dev, b_dev)
             res = op(a, b)
 
             assert (res_dev.get() == res).all()
 
-            res_dev = op(a_dev, s)
-            res = op(a, s)
-
-            assert (res_dev.get() == res).all()
-
-            res_dev = op(s, b_dev)
-            res = op(s, b)
+            try:
+                res = op(a, s)
+            except OverflowError:
+                pass
+            else:
+                res_dev = op(a_dev, s)
+
+                assert (res_dev.get() == res).all()
+
+            try:
+                res = op(s, b)
+            except OverflowError:
+                pass
+            else:
+                res_dev = op(s, b_dev)
 
-            assert (res_dev.get() == res).all()
+                assert (res_dev.get() == res).all()
 
         for op in [o.iand, o.ior, o.ixor]:
             res_dev = a_dev.copy()
             op_res = op(res_dev, b_dev)
             assert op_res is res_dev
 
             res = a.copy()
-            op(res, b)
+            try:
+                op(res, b)
+            except OverflowError:
+                pass
+            else:
 
-            assert (res_dev.get() == res).all()
+                assert (res_dev.get() == res).all()
 
-            res_dev = a_dev.copy()
-            op_res = op(res_dev, s)
-            assert op_res is res_dev
             res = a.copy()
-            op(res, s)
+            try:
+                op(res, s)
+            except OverflowError:
+                pass
+            else:
+                res_dev = a_dev.copy()
+                op_res = op(res_dev, s)
+                assert op_res is res_dev
 
-            assert (res_dev.get() == res).all()
+                assert (res_dev.get() == res).all()
 
         # Test unary ~
         res_dev = ~a_dev
         res = ~a  # pylint:disable=invalid-unary-operand-type
         assert (res_dev.get() == res).all()
 
 # }}}
@@ -824,58 +839,40 @@
 
 
 # {{{ RNG
 
 # {{{ test_random_float_in_range
 
 @pytest.mark.parametrize("rng_class",
-        [RanluxGenerator, PhiloxGenerator, ThreefryGenerator])
+        [PhiloxGenerator, ThreefryGenerator])
 @pytest.mark.parametrize("ary_size", [300, 301, 302, 303, 10007, 1000000])
 def test_random_float_in_range(ctx_factory, rng_class, ary_size, plot_hist=False):
     context = ctx_factory()
     queue = cl.CommandQueue(context)
 
-    device = queue.device
-    if device.platform.vendor == "The pocl project" \
-            and device.type & cl.device_type.GPU \
-            and rng_class is RanluxGenerator:
-        pytest.xfail("ranlux test fails on PoCL + Nvidia,"
-                "at least the Titan V, as of PoCL 1.6, 2021-01-20")
-
-    if device.platform.vendor == "Intel(R) Corporation" \
-            and rng_class is RanluxGenerator:
-        pytest.xfail("compiling ranlux kernel causes a segfault on "
-                "Intel CPU runtime as of 2022-02-13")
-
     if has_double_support(context.devices[0]):
         dtypes = [np.float32, np.float64]
     else:
         dtypes = [np.float32]
 
-    if rng_class is RanluxGenerator:
-        gen = rng_class(queue, 5120)
-    else:
-        gen = rng_class(context)
+    gen = rng_class(context)
 
     for dtype in dtypes:
         print(dtype)
         ran = cl_array.zeros(queue, ary_size, dtype)
         gen.fill_uniform(ran)
 
         if plot_hist:
             import matplotlib.pyplot as pt
             pt.hist(ran.get(), 30)
             pt.show()
 
         assert (0 <= ran.get()).all()
         assert (ran.get() <= 1).all()
 
-        if rng_class is RanluxGenerator:
-            gen.synchronize(queue)
-
         ran = cl_array.zeros(queue, ary_size, dtype)
         gen.fill_uniform(ran, a=4, b=7)
         ran_host = ran.get()
 
         for cond in [4 <= ran_host,  ran_host <= 7]:
             good = cond.all()
             if not good:
@@ -893,29 +890,20 @@
 # }}}
 
 
 # {{{ test_random_int_in_range
 
 @pytest.mark.parametrize("dtype", [np.int32, np.int64])
 @pytest.mark.parametrize("rng_class",
-        [RanluxGenerator, PhiloxGenerator, ThreefryGenerator])
+        [PhiloxGenerator, ThreefryGenerator])
 def test_random_int_in_range(ctx_factory, rng_class, dtype, plot_hist=False):
     context = ctx_factory()
     queue = cl.CommandQueue(context)
 
-    if queue.device.platform.vendor == "The pocl project" \
-            and queue.device.type & cl.device_type.GPU \
-            and rng_class is RanluxGenerator:
-        pytest.xfail("ranlux test fails on PoCL + Nvidia,"
-                "at least the Titan V, as of PoCL 1.6, 2021-01-20")
-
-    if rng_class is RanluxGenerator:
-        gen = rng_class(queue, 5120)
-    else:
-        gen = rng_class(context)
+    gen = rng_class(context)
 
     # if (dtype == np.int64
     #         and context.devices[0].platform.vendor.startswith("Advanced Micro")):
     #     pytest.xfail("AMD miscompiles 64-bit RNG math")
 
     ran = gen.uniform(queue, (10000007,), dtype, a=200, b=300).get()
     assert (200 <= ran).all()
@@ -2346,14 +2334,58 @@
         cl_array.logical_not(cl_array.zeros(cq, 10, np.float64)).get(),
         np.logical_not(np.zeros(10)))
     np.testing.assert_array_equal(
         cl_array.logical_not((cl_array.zeros(cq, 10, np.float64) + 1)).get(),
         np.logical_not(np.ones(10)))
 
 
+# {{{ test XDG_CACHE_HOME handling
+
+@pytest.mark.skipif(sys.platform == "win32",
+                    reason="XDG_CACHE_HOME is not used on Windows")
+def test_xdg_cache_home(ctx_factory):
+    import os
+    import shutil
+    from os.path import join
+
+    context = ctx_factory()
+    queue = cl.CommandQueue(context)
+
+    a = np.array([1, 2, 3, 4, 5]).astype(np.float32)
+    a_gpu = cl_array.to_device(queue, a)
+
+    xdg_dir = "tmpdir_pyopencl_xdg_test"
+
+    # PyOpenCL uses pytools.PersistentDict for invoker caches,
+    # which is why xdg_dir will always exist. Therefore, check
+    # whether xdg_pyopencl_dir exists.
+    xdg_pyopencl_dir = join(xdg_dir, "pyopencl")
+    assert not os.path.exists(xdg_dir)
+
+    old_xdg_cache_home = None
+
+    try:
+        old_xdg_cache_home = os.getenv("XDG_CACHE_HOME")
+        os.environ["XDG_CACHE_HOME"] = xdg_dir
+
+        result = pow(a_gpu, a_gpu).get()
+        assert (np.abs(a ** a - result) < 3e-3).all()
+
+        assert os.path.exists(xdg_pyopencl_dir)
+    finally:
+        if old_xdg_cache_home is not None:
+            os.environ["XDG_CACHE_HOME"] = old_xdg_cache_home
+        else:
+            del os.environ["XDG_CACHE_HOME"]
+
+        shutil.rmtree(xdg_dir)
+
+# }}}
+
+
 if __name__ == "__main__":
     if len(sys.argv) > 1:
         exec(sys.argv[1])
     else:
         from pytest import main
         main([__file__])
```

### Comparing `pyopencl-2024.1/test/test_arrays_in_structs.py` & `pyopencl-2024.2/test/test_arrays_in_structs.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 import numpy as np
 
 import pyopencl as cl
 import pyopencl.cltypes as cltypes
 import pyopencl.tools as cl_tools
 from pyopencl import mem_flags
-from pyopencl.tools import (  # noqa: F401
-        pytest_generate_tests_for_pyopencl as pytest_generate_tests)
+from pyopencl.tools import \
+    pytest_generate_tests_for_pyopencl as pytest_generate_tests  # noqa: F401
 
 
 def test_struct_with_array_fields(ctx_factory):
     #
     # typedef struct {
     #     uint x[2];
     #     float y;
```

### Comparing `pyopencl-2024.1/test/test_clmath.py` & `pyopencl-2024.2/test/test_clmath.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,24 +17,25 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
 import math
-import numpy as np
 
+import numpy as np
 import pytest
 
-import pyopencl.array as cl_array
 import pyopencl as cl
+import pyopencl.array as cl_array
 import pyopencl.clmath as clmath
-from pyopencl.tools import (  # noqa: F401
-        pytest_generate_tests_for_pyopencl as pytest_generate_tests)
 from pyopencl.characterize import has_double_support, has_struct_arg_count_bug
+from pyopencl.tools import \
+    pytest_generate_tests_for_pyopencl as pytest_generate_tests  # noqa: F401
+
 
 try:
     import faulthandler
 except ImportError:
     pass
 else:
     faulthandler.enable()
@@ -236,15 +237,15 @@
     if not has_double_support(ctx.devices[0]):
         from pytest import skip
         skip("no double precision support--cannot test bessel function")
 
     nterms = 30
 
     try:
-        from pyfmmlib import jfuns2d, hank103_vec
+        from pyfmmlib import hank103_vec, jfuns2d
     except ImportError:
         use_pyfmmlib = False
     else:
         use_pyfmmlib = True
 
     print("PYFMMLIB", use_pyfmmlib)
 
@@ -298,14 +299,15 @@
             else:
                 print(which_func, n, error_scipy)
 
             assert not np.isnan(cl_bessel).any()
 
             if 0 and n == 15:
                 import matplotlib.pyplot as pt
+
                 #pt.plot(scipy_bessel)
                 #pt.plot(cl_bessel)
 
                 pt.loglog(a, np.abs(cl_bessel-scipy_bessel), label="vs scipy")
                 if use_pyfmmlib:
                     pt.loglog(a, np.abs(cl_bessel-pyfmm_bessel), label="vs pyfmmlib")
                 pt.legend()
```

### Comparing `pyopencl-2024.1/test/test_clrandom.py` & `pyopencl-2024.2/test/test_clrandom.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,35 +20,30 @@
 THE SOFTWARE.
 """
 
 import numpy as np
 import pytest
 
 import pyopencl as cl
-import pyopencl.cltypes as cltypes
 import pyopencl.clrandom as clrandom
-from pyopencl.tools import (  # noqa: F401
-        pytest_generate_tests_for_pyopencl as pytest_generate_tests)
+import pyopencl.cltypes as cltypes
 from pyopencl.characterize import has_double_support
+from pyopencl.tools import \
+    pytest_generate_tests_for_pyopencl as pytest_generate_tests  # noqa: F401
+
 
 try:
     import faulthandler
 except ImportError:
     pass
 else:
     faulthandler.enable()
 
 
-def make_ranlux_generator(cl_ctx):
-    queue = cl.CommandQueue(cl_ctx)
-    return clrandom.RanluxGenerator(queue)
-
-
 @pytest.mark.parametrize("rng_class", [
-    make_ranlux_generator,
     clrandom.PhiloxGenerator,
     clrandom.ThreefryGenerator])
 @pytest.mark.parametrize("dtype", [
     np.int32,
     np.int64,
     np.float32,
     np.float64,
@@ -61,21 +56,14 @@
     if dtype == np.float64 and not has_double_support(cl_ctx.devices[0]):
         pytest.skip("double precision not supported on this device")
     rng = rng_class(cl_ctx)
 
     size = 10
 
     with cl.CommandQueue(cl_ctx) as queue:
-        device = queue.device
-        if device.platform.vendor == "The pocl project" \
-                and device.type & cl.device_type.GPU \
-                and rng_class is make_ranlux_generator:
-            pytest.xfail("ranlux test fails on PoCL + Nvidia,"
-                    "at least the K40, as of PoCL 1.6, 2021-01-20")
-
         rng.uniform(queue, size, dtype)
 
         if dtype not in (np.int32, np.int64):
             rng.normal(queue, size, dtype)
 
 
 if __name__ == "__main__":
```

### Comparing `pyopencl-2024.1/test/test_enqueue_copy.py` & `pyopencl-2024.2/test/test_enqueue_copy.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
 import numpy as np
-import pyopencl as cl
 import pytest
 
-from pyopencl.tools import (  # noqa: F401
-        pytest_generate_tests_for_pyopencl as pytest_generate_tests)
+import pyopencl as cl
 from pyopencl.characterize import get_pocl_version
+from pyopencl.tools import \
+    pytest_generate_tests_for_pyopencl as pytest_generate_tests  # noqa: F401
 
 
 def generate_slice(start, shape):
     return tuple([slice(start[i], start[i]+shape[i]) for i in range(len(start))])
 
 
 def test_enqueue_copy_rect_2d(ctx_factory, honor_skip=True):
```

### Comparing `pyopencl-2024.1/test/test_wrapper.py` & `pyopencl-2024.2/test/test_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 
 import numpy as np
 import numpy.linalg as la
 import pytest
 
 import pyopencl as cl
 import pyopencl.array as cl_array
-import pyopencl.cltypes as cltypes
 import pyopencl.clrandom
-from pyopencl.tools import (  # noqa: F401
-        pytest_generate_tests_for_pyopencl as pytest_generate_tests,
-        ImmediateAllocator, DeferredAllocator)
+import pyopencl.cltypes as cltypes
 from pyopencl.characterize import get_pocl_version
+from pyopencl.tools import \
+    pytest_generate_tests_for_pyopencl as pytest_generate_tests  # noqa: F401
+from pyopencl.tools import DeferredAllocator, ImmediateAllocator
 
 
 def _xfail_if_pocl(plat, up_to_version, msg="unsupported by PoCL"):
     if plat.vendor == "The pocl project":
         if up_to_version is None or get_pocl_version(plat) <= up_to_version:
             pytest.xfail(msg)
 
@@ -577,15 +577,15 @@
 
 # }}}
 
 
 # {{{ test_mempool_*
 
 def test_mempool(ctx_factory):
-    from pyopencl.tools import MemoryPool, ImmediateAllocator
+    from pyopencl.tools import ImmediateAllocator, MemoryPool
 
     context = ctx_factory()
     queue = cl.CommandQueue(context)
 
     pool = MemoryPool(ImmediateAllocator(queue))
     alloc_queue = []
 
@@ -597,17 +597,18 @@
             if len(alloc_queue) > 10:
                 alloc_queue.pop(0)
     del alloc_queue
     pool.stop_holding()
 
 
 def test_mempool_2(ctx_factory):
-    from pyopencl.tools import MemoryPool, ImmediateAllocator
     from random import randrange
 
+    from pyopencl.tools import ImmediateAllocator, MemoryPool
+
     context = ctx_factory()
     queue = cl.CommandQueue(context)
 
     pool = MemoryPool(ImmediateAllocator(queue))
 
     for s in [randrange(1 << 31) >> randrange(32) for _ in range(2000)] + [2**30]:
         bin_nr = pool.bin_number(s)
@@ -680,15 +681,15 @@
 # }}}
 
 
 # {{{ test_header_dep_handling
 def test_header_dep_handling(ctx_factory):
     context = ctx_factory()
 
-    from os.path import exists, dirname, join
+    from os.path import dirname, exists, join
     assert exists(join(dirname(__file__), "empty-header.h"))
 
     kernel_src = """
     #include <empty-header.h>
     kernel void zonk(global int *a)
     {
       *a = 5;
@@ -1120,16 +1121,17 @@
     is_pypy = "__pypy__" in sys.builtin_module_names
 
     ctx = ctx_factory()
     queue = cl.CommandQueue(ctx)
 
     dev = ctx.devices[0]
 
-    from pyopencl.characterize import has_coarse_grain_buffer_svm
     from pytest import skip
+
+    from pyopencl.characterize import has_coarse_grain_buffer_svm
     if not has_coarse_grain_buffer_svm(queue.device):
         skip("device does not support coarse-grain SVM")
 
     if ("AMD" in dev.platform.name
             and dev.type & cl.device_type.CPU):
         pytest.xfail("AMD CPU doesn't do coarse-grain SVM")
     if ("AMD" in dev.platform.name
@@ -1228,16 +1230,17 @@
     is_pypy = "__pypy__" in sys.builtin_module_names
 
     ctx = ctx_factory()
     queue = cl.CommandQueue(ctx)
 
     _xfail_if_pocl_gpu(queue.device, "GPU SVM")
 
-    from pyopencl.characterize import has_fine_grain_buffer_svm
     from pytest import skip
+
+    from pyopencl.characterize import has_fine_grain_buffer_svm
     if not has_fine_grain_buffer_svm(queue.device):
         skip("device does not support fine-grain SVM")
 
     n = 3000
     ary = cl.fsvm_empty(ctx, n, np.float32, alignment=64)
 
     if not is_pypy:
@@ -1424,16 +1427,17 @@
 
 # {{{ test_capture_call
 
 def test_capture_call(ctx_factory):
     ctx = ctx_factory()
     queue = cl.CommandQueue(ctx)
 
-    a_np = np.random.rand(500).astype(np.float32)
-    b_np = np.random.rand(500).astype(np.float32)
+    rng = np.random.default_rng()
+    a_np = rng.random(500, dtype=np.float32)
+    b_np = rng.random(500, dtype=np.float32)
 
     ctx = cl.create_some_context()
     queue = cl.CommandQueue(ctx)
 
     mf = cl.mem_flags
     a_g = cl.Buffer(ctx, mf.READ_ONLY | mf.COPY_HOST_PTR, hostbuf=a_np)
     b_g = cl.Buffer(ctx, mf.READ_ONLY | mf.COPY_HOST_PTR, hostbuf=b_np)
@@ -1510,14 +1514,39 @@
     cl._cl._enqueue_copy_image_to_buffer(
             queue, src=image_array_cl, dest=buffer_cl, offset=0, origin=(0, 0, 0),
             region=array_shape)
 
 # }}}
 
 
+def test_zero_size_svm_allocations(ctx_factory):
+    ctx = ctx_factory()
+
+    from pytest import skip
+
+    from pyopencl.characterize import has_coarse_grain_buffer_svm
+    if not has_coarse_grain_buffer_svm(ctx.devices[0]):
+        skip("device does not support coarse-grain SVM")
+
+    # Go back to svm_empty once
+    # https://github.com/numpy/numpy/issues/26366 is solved.
+    # zero_sized_svm = cl.svm_empty(ctx, cl.svm_mem_flags.READ_WRITE, 0, np.float64)
+    zero_sized_svm = cl.SVMAllocation(ctx, 0, 0, cl.svm_mem_flags.READ_WRITE)
+    zero_sized_svm.release()
+
+    from pyopencl.tools import SVMAllocator, SVMPool
+    svm_alloc = SVMAllocator(ctx)
+    zero_sized_svm = svm_alloc(0)
+    zero_sized_svm.release()
+
+    svm_pool = SVMPool(svm_alloc)
+    zero_sized_svm = svm_pool(0)
+    zero_sized_svm.release()
+
+
 if __name__ == "__main__":
     import sys
     if len(sys.argv) > 1:
         exec(sys.argv[1])
     else:
         from pytest import main
         main([__file__])
```

