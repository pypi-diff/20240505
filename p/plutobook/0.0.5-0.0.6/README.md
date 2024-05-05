# Comparing `tmp/plutobook-0.0.5-pp310-pypy310_pp73-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/plutobook-0.0.6-cp310-cp310-manylinux_2_5_x86_64.manylinux1_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4843 bytes, number of entries: 7
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-05 13:15 plutobook-0.0.5.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-05 13:15 plutobook.libs/
--rwxr-xr-x  2.0 unx    16160 b- defN 24-May-05 13:15 plutobook.pypy310-pp73-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx     1073 b- defN 24-May-05 13:15 plutobook-0.0.5.dist-info/LICENSE
--rw-rw-r--  2.0 unx      408 b- defN 24-May-05 13:15 plutobook-0.0.5.dist-info/RECORD
--rw-rw-r--  2.0 unx      238 b- defN 24-May-05 13:15 plutobook-0.0.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx     1473 b- defN 24-May-05 13:15 plutobook-0.0.5.dist-info/METADATA
-7 files, 19352 bytes uncompressed, 3863 bytes compressed:  80.0%
+Zip file size: 4819 bytes, number of entries: 7
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-05 13:25 plutobook-0.0.6.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-05 13:25 plutobook.libs/
+-rwxr-xr-x  2.0 unx    16160 b- defN 24-May-05 13:25 plutobook.cpython-310-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx     1073 b- defN 24-May-05 13:25 plutobook-0.0.6.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      407 b- defN 24-May-05 13:25 plutobook-0.0.6.dist-info/RECORD
+-rw-rw-r--  2.0 unx      210 b- defN 24-May-05 13:25 plutobook-0.0.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     1473 b- defN 24-May-05 13:25 plutobook-0.0.6.dist-info/METADATA
+7 files, 19323 bytes uncompressed, 3841 bytes compressed:  80.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: plutobook-0.0.5.dist-info/
+Filename: plutobook-0.0.6.dist-info/
 Comment: 
 
 Filename: plutobook.libs/
 Comment: 
 
-Filename: plutobook.pypy310-pp73-x86_64-linux-gnu.so
+Filename: plutobook.cpython-310-x86_64-linux-gnu.so
 Comment: 
 
-Filename: plutobook-0.0.5.dist-info/LICENSE
+Filename: plutobook-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: plutobook-0.0.5.dist-info/RECORD
+Filename: plutobook-0.0.6.dist-info/RECORD
 Comment: 
 
-Filename: plutobook-0.0.5.dist-info/WHEEL
+Filename: plutobook-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: plutobook-0.0.5.dist-info/METADATA
+Filename: plutobook-0.0.6.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## Comparing `plutobook.pypy310-pp73-x86_64-linux-gnu.so` & `plutobook.cpython-310-x86_64-linux-gnu.so`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 10% similar despite different names*

### readelf --wide --program-header {}

```diff
@@ -1,15 +1,15 @@
 
 Elf file type is DYN (Shared object file)
 Entry point 0x1070
 There are 9 program headers, starting at offset 64
 
 Program Headers:
   Type           Offset   VirtAddr           PhysAddr           FileSiz  MemSiz   Flg Align
-  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x000588 0x000588 R   0x1000
+  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x000580 0x000580 R   0x1000
   LOAD           0x001000 0x0000000000001000 0x0000000000001000 0x00015d 0x00015d R E 0x1000
   LOAD           0x002000 0x0000000000002000 0x0000000000002000 0x0000a4 0x0000a4 R   0x1000
   LOAD           0x002e48 0x0000000000003e48 0x0000000000003e48 0x0002b8 0x0002c0 RW  0x1000
   DYNAMIC        0x002e60 0x0000000000003e60 0x0000000000003e60 0x000180 0x000180 RW  0x8
   NOTE           0x000238 0x0000000000000238 0x0000000000000238 0x000024 0x000024 R   0x4
   GNU_EH_FRAME   0x002014 0x0000000000002014 0x0000000000002014 0x000024 0x000024 R   0x4
   GNU_STACK      0x000000 0x0000000000000000 0x0000000000000000 0x000000 0x000000 RW  0x10
```

### readelf --wide --sections {}

```diff
@@ -2,17 +2,17 @@
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .note.gnu.build-id NOTE            0000000000000238 000238 000024 00   A  0   0  4
   [ 2] .gnu.hash         GNU_HASH        0000000000000260 000260 000030 00   A  3   0  8
   [ 3] .dynsym           DYNSYM          0000000000000290 000290 0000f0 18   A  4   1  8
-  [ 4] .dynstr           STRTAB          0000000000000380 000380 00009c 00   A  0   0  1
-  [ 5] .rela.dyn         RELA            0000000000000420 000420 000108 18   A  3   0  8
-  [ 6] .rela.plt         RELA            0000000000000528 000528 000060 18  AI  3  19  8
+  [ 4] .dynstr           STRTAB          0000000000000380 000380 000098 00   A  0   0  1
+  [ 5] .rela.dyn         RELA            0000000000000418 000418 000108 18   A  3   0  8
+  [ 6] .rela.plt         RELA            0000000000000520 000520 000060 18  AI  3  19  8
   [ 7] .init             PROGBITS        0000000000001000 001000 00001a 00  AX  0   0  4
   [ 8] .plt              PROGBITS        0000000000001020 001020 000050 10  AX  0   0 16
   [ 9] .text             PROGBITS        0000000000001070 001070 0000e1 00  AX  0   0 16
   [10] .fini             PROGBITS        0000000000001154 001154 000009 00  AX  0   0  4
   [11] .rodata           PROGBITS        0000000000002000 002000 000012 01 AMS  0   0  1
   [12] .eh_frame_hdr     PROGBITS        0000000000002014 002014 000024 00   A  0   0  4
   [13] .eh_frame         PROGBITS        0000000000002038 002038 00006c 00   A  0   0  8
@@ -22,14 +22,14 @@
   [17] .dynamic          DYNAMIC         0000000000003e60 002e60 000180 10  WA  4   0  8
   [18] .got              PROGBITS        0000000000003fe0 002fe0 000020 08  WA  0   0  8
   [19] .got.plt          PROGBITS        0000000000004000 003000 000038 08  WA  0   0  8
   [20] .data             PROGBITS        0000000000004040 003040 0000c0 00  WA  0   0 32
   [21] .bss              NOBITS          0000000000004100 003100 000008 00  WA  0   0  1
   [22] .comment          PROGBITS        0000000000000000 003100 00002f 01  MS  0   0  1
   [23] .symtab           SYMTAB          0000000000000000 003130 0004e0 18     24  43  8
-  [24] .strtab           STRTAB          0000000000000000 003610 0001af 00      0   0  1
-  [25] .shstrtab         STRTAB          0000000000000000 0037bf 0000de 00      0   0  1
+  [24] .strtab           STRTAB          0000000000000000 003610 0001ab 00      0   0  1
+  [25] .shstrtab         STRTAB          0000000000000000 0037bb 0000de 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

### readelf --wide --symbols {}

```diff
@@ -1,30 +1,30 @@
 
 Symbol table '.dynsym' contains 10 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __cxa_finalize
-     2: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
-     3: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
-     4: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyPyModule_Create2
-     5: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyPyUnicode_FromString
+     2: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_FromString
+     3: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
+     4: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
+     5: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyModule_Create2
      6: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
      7: 0000000000001140    17 FUNC    GLOBAL DEFAULT    9 PyInit_plutobook
      8: 0000000000001000     0 FUNC    GLOBAL DEFAULT    7 _init
      9: 0000000000001154     0 FUNC    GLOBAL DEFAULT   10 _fini
 
 Symbol table '.symtab' contains 52 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000238     0 SECTION LOCAL  DEFAULT    1 .note.gnu.build-id
      2: 0000000000000260     0 SECTION LOCAL  DEFAULT    2 .gnu.hash
      3: 0000000000000290     0 SECTION LOCAL  DEFAULT    3 .dynsym
      4: 0000000000000380     0 SECTION LOCAL  DEFAULT    4 .dynstr
-     5: 0000000000000420     0 SECTION LOCAL  DEFAULT    5 .rela.dyn
-     6: 0000000000000528     0 SECTION LOCAL  DEFAULT    6 .rela.plt
+     5: 0000000000000418     0 SECTION LOCAL  DEFAULT    5 .rela.dyn
+     6: 0000000000000520     0 SECTION LOCAL  DEFAULT    6 .rela.plt
      7: 0000000000001000     0 SECTION LOCAL  DEFAULT    7 .init
      8: 0000000000001020     0 SECTION LOCAL  DEFAULT    8 .plt
      9: 0000000000001070     0 SECTION LOCAL  DEFAULT    9 .text
     10: 0000000000001154     0 SECTION LOCAL  DEFAULT   10 .fini
     11: 0000000000002000     0 SECTION LOCAL  DEFAULT   11 .rodata
     12: 0000000000002014     0 SECTION LOCAL  DEFAULT   12 .eh_frame_hdr
     13: 0000000000002038     0 SECTION LOCAL  DEFAULT   13 .eh_frame
@@ -43,26 +43,26 @@
     26: 00000000000010e0     0 FUNC    LOCAL  DEFAULT    9 __do_global_dtors_aux
     27: 0000000000004100     1 OBJECT  LOCAL  DEFAULT   21 completed.0
     28: 0000000000003e50     0 OBJECT  LOCAL  DEFAULT   15 __do_global_dtors_aux_fini_array_entry
     29: 0000000000001120     0 FUNC    LOCAL  DEFAULT    9 frame_dummy
     30: 0000000000003e48     0 OBJECT  LOCAL  DEFAULT   14 __frame_dummy_init_array_entry
     31: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS plutobook-module.c
     32: 0000000000001130    12 FUNC    LOCAL  DEFAULT    9 foo
-    33: 0000000000004040   112 OBJECT  LOCAL  DEFAULT   20 module
+    33: 0000000000004040   104 OBJECT  LOCAL  DEFAULT   20 module
     34: 00000000000040c0    64 OBJECT  LOCAL  DEFAULT   20 methods
     35: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
     36: 00000000000020a0     0 OBJECT  LOCAL  DEFAULT   13 __FRAME_END__
     37: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS 
     38: 0000000000003e60     0 OBJECT  LOCAL  DEFAULT   17 _DYNAMIC
     39: 0000000000004100     0 OBJECT  LOCAL  DEFAULT   20 __TMC_END__
     40: 0000000000003e58     0 OBJECT  LOCAL  DEFAULT   16 __dso_handle
     41: 0000000000002014     0 NOTYPE  LOCAL  DEFAULT   12 __GNU_EH_FRAME_HDR
     42: 0000000000004000     0 OBJECT  LOCAL  DEFAULT   19 _GLOBAL_OFFSET_TABLE_
     43: 0000000000001140    17 FUNC    GLOBAL DEFAULT    9 PyInit_plutobook
     44: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __cxa_finalize
-    45: 0000000000001000     0 FUNC    GLOBAL DEFAULT    7 _init
-    46: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
-    47: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
-    48: 0000000000001154     0 FUNC    GLOBAL DEFAULT   10 _fini
-    49: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyPyModule_Create2
-    50: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyPyUnicode_FromString
+    45: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_FromString
+    46: 0000000000001000     0 FUNC    GLOBAL DEFAULT    7 _init
+    47: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
+    48: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
+    49: 0000000000001154     0 FUNC    GLOBAL DEFAULT   10 _fini
+    50: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyModule_Create2
     51: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
```

### readelf --wide --relocs {}

```diff
@@ -1,21 +1,21 @@
 
-Relocation section '.rela.dyn' at offset 0x420 contains 11 entries:
+Relocation section '.rela.dyn' at offset 0x418 contains 11 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000003e48  0000000000000008 R_X86_64_RELATIVE                         1120
 0000000000003e50  0000000000000008 R_X86_64_RELATIVE                         10e0
 0000000000003e58  0000000000000008 R_X86_64_RELATIVE                         3e58
-0000000000004070  0000000000000008 R_X86_64_RELATIVE                         2004
-0000000000004088  0000000000000008 R_X86_64_RELATIVE                         40c0
+0000000000004068  0000000000000008 R_X86_64_RELATIVE                         2004
+0000000000004080  0000000000000008 R_X86_64_RELATIVE                         40c0
 00000000000040c0  0000000000000008 R_X86_64_RELATIVE                         200e
 00000000000040c8  0000000000000008 R_X86_64_RELATIVE                         1130
 0000000000003fe0  0000000100000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize + 0
-0000000000003fe8  0000000200000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
-0000000000003ff0  0000000300000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
+0000000000003fe8  0000000300000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
+0000000000003ff0  0000000400000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_deregisterTMCloneTable + 0
 0000000000003ff8  0000000600000006 R_X86_64_GLOB_DAT      0000000000000000 __gmon_start__ + 0
 
-Relocation section '.rela.plt' at offset 0x528 contains 4 entries:
+Relocation section '.rela.plt' at offset 0x520 contains 4 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000004018  0000000100000007 R_X86_64_JUMP_SLOT     0000000000000000 __cxa_finalize + 0
-0000000000004020  0000000400000007 R_X86_64_JUMP_SLOT     0000000000000000 PyPyModule_Create2 + 0
-0000000000004028  0000000500000007 R_X86_64_JUMP_SLOT     0000000000000000 PyPyUnicode_FromString + 0
+0000000000004020  0000000200000007 R_X86_64_JUMP_SLOT     0000000000000000 PyUnicode_FromString + 0
+0000000000004028  0000000500000007 R_X86_64_JUMP_SLOT     0000000000000000 PyModule_Create2 + 0
 0000000000004030  0000000600000007 R_X86_64_JUMP_SLOT     0000000000000000 __gmon_start__ + 0
```

### readelf --wide --dynamic {}

```diff
@@ -6,18 +6,18 @@
  0x0000000000000019 (INIT_ARRAY)         0x3e48
  0x000000000000001b (INIT_ARRAYSZ)       8 (bytes)
  0x000000000000001a (FINI_ARRAY)         0x3e50
  0x000000000000001c (FINI_ARRAYSZ)       8 (bytes)
  0x000000006ffffef5 (GNU_HASH)           0x260
  0x0000000000000005 (STRTAB)             0x380
  0x0000000000000006 (SYMTAB)             0x290
- 0x000000000000000a (STRSZ)              156 (bytes)
+ 0x000000000000000a (STRSZ)              152 (bytes)
  0x000000000000000b (SYMENT)             24 (bytes)
  0x0000000000000003 (PLTGOT)             0x4000
  0x0000000000000002 (PLTRELSZ)           96 (bytes)
  0x0000000000000014 (PLTREL)             RELA
- 0x0000000000000017 (JMPREL)             0x528
- 0x0000000000000007 (RELA)               0x420
+ 0x0000000000000017 (JMPREL)             0x520
+ 0x0000000000000007 (RELA)               0x418
  0x0000000000000008 (RELASZ)             264 (bytes)
  0x0000000000000009 (RELAENT)            24 (bytes)
  0x000000006ffffff9 (RELACOUNT)          7
  0x0000000000000000 (NULL)               0x0
```

### readelf --wide --notes {}

```diff
@@ -1,4 +1,4 @@
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 81156e3759943ddd7fa29f5d3d26ae26038e9082
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 6db04a804d2574d193ac7f11860c41f7b1a117cf
```

### strings --all --bytes=8 {}

```diff
@@ -1,14 +1,14 @@
 __gmon_start__
 _ITM_deregisterTMCloneTable
 _ITM_registerTMCloneTable
 __cxa_finalize
-PyPyUnicode_FromString
+PyUnicode_FromString
 PyInit_plutobook
-PyPyModule_Create2
+PyModule_Create2
 plutobook
 GCC: (GNU) 10.2.1 20210130 (Red Hat 10.2.1-11)
 crtstuff.c
 deregister_tm_clones
 __do_global_dtors_aux
 completed.0
 __do_global_dtors_aux_fini_array_entry
@@ -19,18 +19,18 @@
 _DYNAMIC
 __TMC_END__
 __dso_handle
 __GNU_EH_FRAME_HDR
 _GLOBAL_OFFSET_TABLE_
 PyInit_plutobook
 __cxa_finalize
+PyUnicode_FromString
 _ITM_registerTMCloneTable
 _ITM_deregisterTMCloneTable
-PyPyModule_Create2
-PyPyUnicode_FromString
+PyModule_Create2
 __gmon_start__
 .shstrtab
 .note.gnu.build-id
 .gnu.hash
 .rela.dyn
 .rela.plt
 .eh_frame_hdr
```

### readelf --wide --decompress --hex-dump=.dynstr {}

```diff
@@ -2,12 +2,12 @@
 Hex dump of section '.dynstr':
   0x00000380 005f5f67 6d6f6e5f 73746172 745f5f00 .__gmon_start__.
   0x00000390 5f696e69 74005f66 696e6900 5f49544d _init._fini._ITM
   0x000003a0 5f646572 65676973 74657254 4d436c6f _deregisterTMClo
   0x000003b0 6e655461 626c6500 5f49544d 5f726567 neTable._ITM_reg
   0x000003c0 69737465 72544d43 6c6f6e65 5461626c isterTMCloneTabl
   0x000003d0 65005f5f 6378615f 66696e61 6c697a65 e.__cxa_finalize
-  0x000003e0 00507950 79556e69 636f6465 5f46726f .PyPyUnicode_Fro
-  0x000003f0 6d537472 696e6700 5079496e 69745f70 mString.PyInit_p
-  0x00000400 6c75746f 626f6f6b 00507950 794d6f64 lutobook.PyPyMod
-  0x00000410 756c655f 43726561 74653200          ule_Create2.
+  0x000003e0 00507955 6e69636f 64655f46 726f6d53 .PyUnicode_FromS
+  0x000003f0 7472696e 67005079 496e6974 5f706c75 tring.PyInit_plu
+  0x00000400 746f626f 6f6b0050 794d6f64 756c655f tobook.PyModule_
+  0x00000410 43726561 74653200                   Create2.
```

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt {}

```diff
@@ -9,20 +9,20 @@
 	nopl   0x0(%rax)
 
 0000000000001030 <__cxa_finalize@plt>:
 	jmp    *0x2fe2(%rip)        
 	push   $0x0
 	jmp    1020 <.plt>
 
-0000000000001040 <PyPyModule_Create2@plt>:
+0000000000001040 <PyUnicode_FromString@plt>:
 	jmp    *0x2fda(%rip)        
 	push   $0x1
 	jmp    1020 <.plt>
 
-0000000000001050 <PyPyUnicode_FromString@plt>:
+0000000000001050 <PyModule_Create2@plt>:
 	jmp    *0x2fd2(%rip)        
 	push   $0x2
 	jmp    1020 <.plt>
 
 0000000000001060 <__gmon_start__@plt>:
 	jmp    *0x2fca(%rip)        
 	push   $0x3
```

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -59,15 +59,15 @@
 	jmp    10a0 <register_tm_clones>
 	cs nopw 0x0(%rax,%rax,1)
 	nop
 
 0000000000001130 <foo>:
 foo():
 	lea    0xec9(%rip),%rdi        
-	jmp    1050 <PyPyUnicode_FromString@plt>
+	jmp    1040 <PyUnicode_FromString@plt>
 	nopl   0x0(%rax)
 
 0000000000001140 <PyInit_plutobook>:
 PyInit_plutobook():
 	mov    $0x3f5,%esi
 	lea    0x2ef4(%rip),%rdi        
-	jmp    1040 <PyPyModule_Create2@plt>
+	jmp    1050 <PyModule_Create2@plt>
```

### readelf --wide --decompress --hex-dump=.data {}

```diff
@@ -1,14 +1,14 @@
 
 Hex dump of section '.data':
   0x00004040 01000000 00000000 00000000 00000000 ................
   0x00004050 00000000 00000000 00000000 00000000 ................
-  0x00004060 00000000 00000000 00000000 00000000 ................
-  0x00004070 04200000 00000000 00000000 00000000 . ..............
-  0x00004080 ffffffff ffffffff c0400000 00000000 .........@......
+  0x00004060 00000000 00000000 04200000 00000000 ......... ......
+  0x00004070 00000000 00000000 ffffffff ffffffff ................
+  0x00004080 c0400000 00000000 00000000 00000000 .@..............
   0x00004090 00000000 00000000 00000000 00000000 ................
   0x000040a0 00000000 00000000 00000000 00000000 ................
   0x000040b0 00000000 00000000 00000000 00000000 ................
   0x000040c0 0e200000 00000000 30110000 00000000 . ......0.......
   0x000040d0 04000000 00000000 00000000 00000000 ................
   0x000040e0 00000000 00000000 00000000 00000000 ................
   0x000040f0 00000000 00000000 00000000 00000000 ................
```

### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -15,16 +15,16 @@
   0x000000c0 4d455f45 4e445f5f 005f4459 4e414d49 ME_END__._DYNAMI
   0x000000d0 43005f5f 544d435f 454e445f 5f005f5f C.__TMC_END__.__
   0x000000e0 64736f5f 68616e64 6c65005f 5f474e55 dso_handle.__GNU
   0x000000f0 5f45485f 4652414d 455f4844 52005f47 _EH_FRAME_HDR._G
   0x00000100 4c4f4241 4c5f4f46 46534554 5f544142 LOBAL_OFFSET_TAB
   0x00000110 4c455f00 5079496e 69745f70 6c75746f LE_.PyInit_pluto
   0x00000120 626f6f6b 005f5f63 78615f66 696e616c book.__cxa_final
-  0x00000130 697a6500 5f696e69 74005f49 544d5f72 ize._init._ITM_r
-  0x00000140 65676973 74657254 4d436c6f 6e655461 egisterTMCloneTa
-  0x00000150 626c6500 5f49544d 5f646572 65676973 ble._ITM_deregis
-  0x00000160 74657254 4d436c6f 6e655461 626c6500 terTMCloneTable.
-  0x00000170 5f66696e 69005079 50794d6f 64756c65 _fini.PyPyModule
-  0x00000180 5f437265 61746532 00507950 79556e69 _Create2.PyPyUni
-  0x00000190 636f6465 5f46726f 6d537472 696e6700 code_FromString.
-  0x000001a0 5f5f676d 6f6e5f73 74617274 5f5f00   __gmon_start__.
+  0x00000130 697a6500 5079556e 69636f64 655f4672 ize.PyUnicode_Fr
+  0x00000140 6f6d5374 72696e67 005f696e 6974005f omString._init._
+  0x00000150 49544d5f 72656769 73746572 544d436c ITM_registerTMCl
+  0x00000160 6f6e6554 61626c65 005f4954 4d5f6465 oneTable._ITM_de
+  0x00000170 72656769 73746572 544d436c 6f6e6554 registerTMCloneT
+  0x00000180 61626c65 005f6669 6e690050 794d6f64 able._fini.PyMod
+  0x00000190 756c655f 43726561 74653200 5f5f676d ule_Create2.__gm
+  0x000001a0 6f6e5f73 74617274 5f5f00            on_start__.
```

## Comparing `plutobook-0.0.5.dist-info/LICENSE` & `plutobook-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `plutobook-0.0.5.dist-info/METADATA` & `plutobook-0.0.6.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plutobook
-Version: 0.0.5
+Version: 0.0.6
 Summary: Paged HTML rendering library
 Author-Email: Samuel Ugochukwu <sammycageagle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Samuel Ugochukwu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

