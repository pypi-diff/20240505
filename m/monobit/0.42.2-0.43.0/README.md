# Comparing `tmp/monobit-0.42.2.tar.gz` & `tmp/monobit-0.43.0.tar.gz`

## Comparing `monobit-0.42.2.tar` & `monobit-0.43.0.tar`

### file list

```diff
@@ -1,517 +1,543 @@
--rw-r--r--   0        0        0    27029 2020-02-02 00:00:00.000000 monobit-0.42.2/YAFF.md
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 monobit-0.42.2/banner.py
--rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 monobit-0.42.2/convert.py
--rwxr-xr-x   0        0        0     7145 2020-02-02 00:00:00.000000 monobit-0.42.2/explore.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/__init__.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/basetypes.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/binary.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/blocks.py
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/cachedprops.py
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/chart.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/constants.py
--rw-r--r--   0        0        0    58312 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/encoding.py
--rw-r--r--   0        0        0    48242 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/font.py
--rw-r--r--   0        0        0    34079 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/glyph.py
--rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/glyphmap.py
--rw-r--r--   0        0        0     9564 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/labels.py
--rw-r--r--   0        0        0    10129 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/magic.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/pack.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/properties.py
--rw-r--r--   0        0        0    22774 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/raster.py
--rw-r--r--   0        0        0    13332 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/renderer.py
--rw-r--r--   0        0        0    11375 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/scripting.py
--rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/storage.py
--rw-r--r--   0        0        0     7809 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/streams.py
--rw-r--r--   0        0        0     9483 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/struct.py
--rw-r--r--   0        0        0     6663 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/taggers.py
--rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/vector.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/__init__.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/adobe/ReadMe.txt
--rw-r--r--   0        0        0     8143 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/adobe/stdenc.txt
--rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/adobe/symbol.txt
--rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/adobe/zdingbat.txt
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/agl/LICENSE.md
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/agl/README.md
--rw-r--r--   0        0        0    27655 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/agl/aglfn.txt
--rw-r--r--   0        0        0    78060 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/agl/glyphlist.txt
--rw-r--r--   0        0        0    24830 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/ARABIC.TXT
--rw-r--r--   0        0        0    13008 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/CELTIC.TXT
--rw-r--r--   0        0        0    13065 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/CENTEURO.TXT
--rw-r--r--   0        0        0   197055 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/CHINSIMP.TXT
--rw-r--r--   0        0        0   323716 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/CHINTRAD.TXT
--rw-r--r--   0        0        0    26610 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/CORPCHAR.TXT
--rw-r--r--   0        0        0    13388 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/CROATIAN.TXT
--rw-r--r--   0        0        0    13497 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/CYRILLIC.TXT
--rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/DEVANAGA.TXT
--rw-r--r--   0        0        0    14320 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/DINGBATS.TXT
--rw-r--r--   0        0        0    23987 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/FARSI.TXT
--rw-r--r--   0        0        0    14055 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/GAELIC.TXT
--rw-r--r--   0        0        0    14042 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/GREEK.TXT
--rw-r--r--   0        0        0    13940 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/GUJARATI.TXT
--rw-r--r--   0        0        0    16096 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/GURMUKHI.TXT
--rw-r--r--   0        0        0    27034 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/HEBREW.TXT
--rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/ICELAND.TXT
--rw-r--r--   0        0        0    11800 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/INUIT.TXT
--rw-r--r--   0        0        0   198175 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/JAPANESE.TXT
--rw-r--r--   0        0        0    10252 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/KEYBOARD.TXT
--rw-r--r--   0        0        0   369061 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/KOREAN.TXT
--rw-r--r--   0        0        0    14385 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/ROMAN.TXT
--rw-r--r--   0        0        0    14153 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/ROMANIAN.TXT
--rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/ReadMe.txt
--rw-r--r--   0        0        0    16882 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/SYMBOL.TXT
--rw-r--r--   0        0        0    15564 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/THAI.TXT
--rw-r--r--   0        0        0    12808 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/TURKISH.TXT
--rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/apple/UKRAINE.TXT
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/czyborra/README.md
--rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/czyborra/bulgarian-mik.txt
--rw-r--r--   0        0        0     7866 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/czyborra/cp866.txt
--rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/czyborra/gost19768-87.txt
--rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/czyborra/hp-roman8.txt
--rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/czyborra/koi-0.txt
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/czyborra/koi-7.txt
--rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/czyborra/koi8-a.txt
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/czyborra/koi8-b.txt
--rw-r--r--   0        0        0     6374 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/czyborra/koi8-e.txt
--rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/czyborra/koi8-f.txt
--rw-r--r--   0        0        0     7801 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/czyborra/koi8-r.txt
--rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/czyborra/koi8-u.txt
--rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/dkuug/iso646-ca
--rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/dkuug/iso646-ca2
--rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/dkuug/iso646-cn
--rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/dkuug/iso646-cu
--rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/dkuug/iso646-de
--rw-r--r--   0        0        0    11938 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/dkuug/iso646-dk
--rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/dkuug/iso646-es
--rw-r--r--   0        0        0    11888 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/dkuug/iso646-es2
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/dkuug/iso646-fr
--rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/dkuug/iso646-gb
--rw-r--r--   0        0        0    11997 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/dkuug/iso646-hu
--rw-r--r--   0        0        0    11926 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/dkuug/iso646-it
--rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/dkuug/iso646-jp
--rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/dkuug/iso646-jp-ocr-b
--rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/dkuug/iso646-kr
--rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/dkuug/iso646-us
--rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/dkuug/iso646-yu
--rw-r--r--   0        0        0    17534 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/dkuug/jis_x0201
--rw-r--r--   0        0        0    10319 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/dkuug/x0201-7
--rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/emacs/MULE-ethiopic.map
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/emacs/MULE-ipa.map
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/emacs/MULE-is13194.map
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/emacs/MULE-lviscii.map
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/emacs/MULE-sisheng.map
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/emacs/MULE-tibetan.map
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/emacs/MULE-uviscii.map
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/emacs/README.md
--rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/evertype/ARMENIAN.TXT
--rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/evertype/GEORGIAN.TXT
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/evertype/README.md
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/1116.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/1117.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/1118.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/1119.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/1125.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/113.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/1131.ucp
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30000.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30001.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30002.ucp
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30003.ucp
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30004.ucp
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30005.ucp
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30006.ucp
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30007.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30008.ucp
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30009.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30010.ucp
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30011.ucp
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30012.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30013.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30014.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30015.ucp
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30016.ucp
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30017.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30018.ucp
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30019.ucp
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30020.ucp
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30021.ucp
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30022.ucp
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30023.ucp
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30024.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30025.ucp
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30026.ucp
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30027.ucp
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30028.ucp
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30029.ucp
--rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30030.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30031.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30032.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30033.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30034.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30039.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/30040.ucp
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/3012.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/3021.ucp
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/3845.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/3846.ucp
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/3848.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/437.ucp
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/57781.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/58152.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/58210.ucp
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/58335.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/59234.ucp
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/59829.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/60258.ucp
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/60853.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/61282.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/62306.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/667.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/668.ucp
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/737.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/770.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/771.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/772.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/773.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/774.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/775.ucp
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/777.ucp
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/778.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/790.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/808.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/848.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/849.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/850.ucp
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/851.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/852.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/853.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/855.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/856.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/857.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/858.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/859.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/860.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/861.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/862.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/863.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/864.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/865.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/866.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/867.ucp
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/869.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/872.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/895.ucp
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/899.ucp
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/991.ucp
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/README.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/freedos/__init__.py
--rw-r--r--   0        0        0     9255 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/iana/Amiga-1251
--rw-r--r--   0        0        0    13371 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/iana/PTCP154
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/iana/README.md
--rw-r--r--   0        0        0    14491 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/ibm-cdra/037B34B0.UPMAP100
--rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/ibm-cdra/038834B0.UPMAP100
--rw-r--r--   0        0        0   323573 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/ibm-cdra/039E44B0.UPMAP101
--rw-r--r--   0        0        0   973501 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/ibm-cdra/039F34B0.UPMAP100
--rw-r--r--   0        0        0    17655 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/ibm-cdra/readme.txt
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/icu/README.md
--rw-r--r--   0        0        0   177606 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/icu/aix-KSC5601.1987_0-4.3.6.ucm
--rw-r--r--   0        0        0  1348868 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/icu/cns-11643-1992.ucm
--rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/icu/ibm-1125_P100-1997.ucm
--rw-r--r--   0        0        0   433127 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/icu/ibm-1375_P100-2008.ucm
--rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/icu/ibm-720_P100-1997.ucm
--rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/icu/ibm-806_P100-1998.ucm
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/icu/ibm-851_P100-1995.ucm
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/icu/ibm-858_P100-1997.ucm
--rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/icu/ibm-868_P100-1995.ucm
--rw-r--r--   0        0        0   199596 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/icu/ibm-932_P120-1999.ucm
--rw-r--r--   0        0        0   351895 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/icu/windows-1361-2000.ucm
--rw-r--r--   0        0        0   490901 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/icu/windows-936-2000.ucm
--rw-r--r--   0        0        0     9995 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/iso-8859/8859-1.TXT
--rw-r--r--   0        0        0    10385 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/iso-8859/8859-10.TXT
--rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/iso-8859/8859-11.TXT
--rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/iso-8859/8859-13.TXT
--rw-r--r--   0        0        0    10459 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/iso-8859/8859-14.TXT
--rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/iso-8859/8859-15.TXT
--rw-r--r--   0        0        0    10390 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/iso-8859/8859-16.TXT
--rw-r--r--   0        0        0    10219 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/iso-8859/8859-2.TXT
--rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/iso-8859/8859-3.TXT
--rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/iso-8859/8859-4.TXT
--rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/iso-8859/8859-5.TXT
--rw-r--r--   0        0        0     7723 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/iso-8859/8859-6.TXT
--rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/iso-8859/8859-7.TXT
--rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/iso-8859/8859-8.TXT
--rw-r--r--   0        0        0    10030 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/iso-8859/8859-9.TXT
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/iso-8859/ReadMe.txt
--rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/ADAMOS7.TXT
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/ADAMSWTR.TXT
--rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/AMSCPC.TXT
--rw-r--r--   0        0        0    10266 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/AMSCPM.TXT
--rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/APL2ALT1.TXT
--rw-r--r--   0        0        0    10929 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/APL2ALT2.TXT
--rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/APL2ICHG.TXT
--rw-r--r--   0        0        0    11100 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/APL2PRIM.TXT
--rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/ATARI8IG.TXT
--rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/ATARI8II.TXT
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/ATARI8VG.TXT
--rw-r--r--   0        0        0    12144 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/ATARI8VI.TXT
--rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/ATARISTI.TXT
--rw-r--r--   0        0        0     9561 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/ATARISTV.TXT
--rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/C64IALT.TXT
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/C64IPRI.TXT
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/C64VALT.TXT
--rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/C64VPRI.TXT
--rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/COCOICHG.TXT
--rw-r--r--   0        0        0    11149 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/COCOSGR4.TXT
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/COCOSGR6.TXT
--rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/CPETIALT.TXT
--rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/CPETIPRI.TXT
--rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/CPETVALT.TXT
--rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/CPETVPRI.TXT
--rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/CVICIALT.TXT
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/CVICIPRI.TXT
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/CVICVALT.TXT
--rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/CVICVPRI.TXT
--rw-r--r--   0        0        0     8974 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/IBMPCICH.TXT
--rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/IBMPCVID.TXT
--rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/MINITLG0.TXT
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/MINITLG1.TXT
--rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/MSX.TXT
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/ORICG0.TXT
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/ORICG1.TXT
--rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/RISCEFF.TXT
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/RISCOSB.TXT
--rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/RISCOSI.TXT
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/RISCOSV.TXT
--rw-r--r--   0        0        0    14920 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/ReadMe.txt
--rw-r--r--   0        0        0     9603 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/SINCLRQL.TXT
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/TELTXTG0.TXT
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/TELTXTG1.TXT
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/TELTXTG2.TXT
--rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/TELTXTG3.TXT
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/TI994A.TXT
--rw-r--r--   0        0        0     5639 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM1ICH.TXT
--rw-r--r--   0        0        0     9089 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM1ORG.TXT
--rw-r--r--   0        0        0     9064 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM1REV.TXT
--rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM3IIN.TXT
--rw-r--r--   0        0        0     8497 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM3IJP.TXT
--rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM3IRV.TXT
--rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM3VIN.TXT
--rw-r--r--   0        0        0     9877 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM3VJP.TXT
--rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM3VRV.TXT
--rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM4AIA.TXT
--rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM4AIP.TXT
--rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM4AIR.TXT
--rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM4AVA.TXT
--rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM4AVP.TXT
--rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM4AVR.TXT
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/ZX80.TXT
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/ZX81.TXT
--rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/ZXDESKTP.TXT
--rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/ZXFZXKOI.TXT
--rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/ZXFZXLT1.TXT
--rw-r--r--   0        0        0     7590 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/ZXFZXLT5.TXT
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/ZXFZXPUA.TXT
--rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/ZXFZXSLT.TXT
--rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/kreativekorp/ZXSPCTRM.TXT
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/manual/c0-pictures.txt
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/manual/currency-sign-0x9c.ucp
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/manual/currency-sign-0xdb.ucp
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/manual/dec-vt100.ucp
--rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/manual/hp48.txt
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/manual/ibm897graph.ucp
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/manual/iso2047.txt
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/manual/mac-cyrillic-pre9.0.ucp
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/manual/mac-system.ucp
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/manual/mac-ukrainian-pre9.0.ucp
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/manual/ms-linedraw.txt
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/manual/russup3.ucp
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/manual/russup4ac.ucp
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/manual/russup4na.ucp
--rw-r--r--   0        0        0     7901 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/manual/windows-1.0.txt
--rw-r--r--   0        0        0     8028 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/manual/windows-2.0.txt
--rw-r--r--   0        0        0     9006 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/manual/windows-3.1.txt
--rw-r--r--   0        0        0     9000 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/EBCDIC/CP037.TXT
--rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/EBCDIC/CP1026.TXT
--rw-r--r--   0        0        0     9027 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/EBCDIC/CP500.TXT
--rw-r--r--   0        0        0     8721 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/EBCDIC/CP875.TXT
--rw-r--r--   0        0        0     9177 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/MAC/CYRILLIC.TXT
--rw-r--r--   0        0        0     9413 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/MAC/GREEK.TXT
--rw-r--r--   0        0        0     9253 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/MAC/ICELAND.TXT
--rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/MAC/LATIN2.TXT
--rw-r--r--   0        0        0     9229 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/MAC/ROMAN.TXT
--rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/MAC/TURKISH.TXT
--rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/PC/CP437.TXT
--rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/PC/CP737.TXT
--rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/PC/CP775.TXT
--rw-r--r--   0        0        0     9640 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/PC/CP850.TXT
--rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/PC/CP852.TXT
--rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/PC/CP855.TXT
--rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/PC/CP857.TXT
--rw-r--r--   0        0        0     9845 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/PC/CP860.TXT
--rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/PC/CP861.TXT
--rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/PC/CP862.TXT
--rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/PC/CP863.TXT
--rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/PC/CP864.TXT
--rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/PC/CP865.TXT
--rw-r--r--   0        0        0     9765 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/PC/CP866.TXT
--rw-r--r--   0        0        0     9318 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/PC/CP869.TXT
--rw-r--r--   0        0        0     8452 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/PC/CP874.TXT
--rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP1250.TXT
--rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP1251.TXT
--rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP1252.TXT
--rw-r--r--   0        0        0     8938 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP1253.TXT
--rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP1254.TXT
--rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP1255.TXT
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP1256.TXT
--rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP1257.TXT
--rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP1258.TXT
--rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP874.TXT
--rw-r--r--   0        0        0   295324 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP932.TXT
--rw-r--r--   0        0        0   817310 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP936.TXT
--rw-r--r--   0        0        0   790736 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP949.TXT
--rw-r--r--   0        0        0   508978 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP950.TXT
--rw-r--r--   0        0        0    11537 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/misc/APL-ISO-IR-68.TXT
--rw-r--r--   0        0        0    21171 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/misc/ATARIST.TXT
--rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/misc/CP1006.TXT
--rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/misc/CP424.TXT
--rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/misc/CP856.TXT
--rw-r--r--   0        0        0     8707 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/misc/GSM0338.TXT
--rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/misc/IBMGRAPH.TXT
--rw-r--r--   0        0        0   210734 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/misc/JIS0208.TXT
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/misc/KOI8-R.TXT
--rw-r--r--   0        0        0    11041 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/misc/KOI8-U.TXT
--rw-r--r--   0        0        0   784637 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/misc/KPS9566.TXT
--rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/misc/KZ1048.TXT
--rw-r--r--   0        0        0     7093 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/misc/NEXTSTEP.TXT
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/misc/README.md
--rw-r--r--   0        0        0    49569 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/misc/SGML.TXT
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/misc/US-ASCII-QUOTES.TXT
--rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/misc/dashen-map.txt
--rw-r--r--   0        0        0    92930 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/misc/ibm-ugl.txt
--rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/mleisher/ALTVAR.TXT
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/mleisher/ARMSCII-7.TXT
--rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/mleisher/ARMSCII-8.TXT
--rw-r--r--   0        0        0     9049 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/mleisher/ARMSCII-8A.TXT
--rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/mleisher/DECMCS.TXT
--rw-r--r--   0        0        0     9870 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/mleisher/GEO-ITA.TXT
--rw-r--r--   0        0        0     9758 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/mleisher/GEO-PS.TXT
--rw-r--r--   0        0        0    13439 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/mleisher/IRANSYSTEM.TXT
--rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/mleisher/KOI8RU.TXT
--rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/mleisher/OSNOVAR.TXT
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/mleisher/README.md
--rw-r--r--   0        0        0     9566 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/mleisher/TIS620.TXT
--rw-r--r--   0        0        0   274176 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/moztw/big5_2003-b2u.txt
--rw-r--r--   0        0        0   340277 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/moztw/eten.txt
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/moztw/url
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/python/README.md
--rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/python/TCVN5712-1.TXT
--rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/python/TCVN5712-2.TXT
--rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/python/TCVN5712-3.TXT
--rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/vietstd/unicode.html
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/vietstd/url
--rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/vietstd/viscii1.1.txt
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/wikipedia/README.md
--rw-r--r--   0        0        0   156347 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/wikipedia/abicomp.html
--rw-r--r--   0        0        0   180593 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/wikipedia/brascii.html
--rw-r--r--   0        0        0   144572 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/wikipedia/cp853.html
--rw-r--r--   0        0        0   156279 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/wikipedia/cwi2.html
--rw-r--r--   0        0        0   134679 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/wikipedia/dec-special.html
--rw-r--r--   0        0        0   153445 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/wikipedia/dec-technical.html
--rw-r--r--   0        0        0   192405 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/wikipedia/gem.html
--rw-r--r--   0        0        0   172501 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/wikipedia/kamenicky.html
--rw-r--r--   0        0        0   216297 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/wikipedia/lics.html
--rw-r--r--   0        0        0   150793 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/wikipedia/mattel-aquarius.html
--rw-r--r--   0        0        0   159296 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/wikipedia/mazovia.html
--rw-r--r--   0        0        0   167964 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/wikipedia/pascii.html
--rw-r--r--   0        0        0   217224 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/wikipedia/ventura.html
--rw-r--r--   0        0        0   254035 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/wikipedia/windows-1252.html
--rw-r--r--   0        0        0   245126 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/wikipedia/wingdings.html
--rw-r--r--   0        0        0   160779 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/wikipedia/wiscii.html
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/xfonts/README.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/xfonts/mulearabic-0.enc
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/xfonts/mulearabic-1.enc
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/xfonts/mulearabic-2.enc
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/xfonts/mulelao-1.enc
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/xfonts/suneu-greek.enc
--rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/charmaps/xfonts/viscii1.1-1.enc
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/containers/__init__.py
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/containers/compressors.py
--rw-r--r--   0        0        0     5573 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/containers/container.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/containers/directory.py
--rw-r--r--   0        0        0    11164 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/containers/mac.py
--rw-r--r--   0        0        0    15795 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/containers/source.py
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/containers/tar.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/containers/zip.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/__init__.py
--rw-r--r--   0        0        0    14368 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/amiga.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/bbc.py
--rw-r--r--   0        0        0    40817 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/bmfont.py
--rw-r--r--   0        0        0     8295 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/borland.py
--rw-r--r--   0        0        0    22580 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/cpi.py
--rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/daisydot.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/dashen.py
--rw-r--r--   0        0        0    13468 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/dec.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/dosstart.py
--rw-r--r--   0        0        0    11132 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/figlet.py
--rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/fontx.py
--rw-r--r--   0        0        0    11501 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/fzx.py
--rw-r--r--   0        0        0    26219 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/gdos.py
--rw-r--r--   0        0        0    12688 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/geos.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/hurt.py
--rw-r--r--   0        0        0    10961 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/image.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/mousegraphics.py
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/mzfon.py
--rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/nearlyraw.py
--rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/palm.py
--rw-r--r--   0        0        0    29954 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/pcl.py
--rw-r--r--   0        0        0     7579 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/pcpaint.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/pdf.py
--rw-r--r--   0        0        0    12848 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/pkfont.py
--rw-r--r--   0        0        0    10733 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/prebuilt.py
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/printshop.py
--rw-r--r--   0        0        0     5708 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/psf.py
--rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/raw.py
--rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/signum.py
--rw-r--r--   0        0        0     8488 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/svg.py
--rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/vfont.py
--rw-r--r--   0        0        0    12534 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/xerox.py
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/mac/__init__.py
--rw-r--r--   0        0        0    21417 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/mac/dfont.py
--rw-r--r--   0        0        0    29289 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/mac/fond.py
--rw-r--r--   0        0        0     5353 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/mac/iigs.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/mac/lisa.py
--rw-r--r--   0        0        0    27380 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/mac/nfnt.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/os2/__init__.py
--rw-r--r--   0        0        0    21098 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/os2/gpifont.py
--rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/os2/lx.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/os2/ne.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/sfnt/__init__.py
--rw-r--r--   0        0        0    30762 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/sfnt/sfnt.py
--rw-r--r--   0        0        0    17917 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/sfnt/sfnt_writer.py
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/sfnt/fonttools/E_B_S_C_.py
--rw-r--r--   0        0        0     6080 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/sfnt/fonttools/__init__.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/sfnt/fonttools/_b_d_a_t.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/sfnt/fonttools/_b_h_e_d.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/sfnt/fonttools/_b_l_o_c.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/text/__init__.py
--rw-r--r--   0        0        0    16750 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/text/draw.py
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/text/hex.py
--rw-r--r--   0        0        0    14764 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/text/yaff.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/windows/LICENSE.md
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/windows/__init__.py
--rw-r--r--   0        0        0    32356 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/windows/fnt.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/windows/mz.py
--rw-r--r--   0        0        0    14160 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/windows/ne.py
--rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/windows/pe.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/xlfd/__init__.py
--rw-r--r--   0        0        0    18392 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/xlfd/bdf.py
--rw-r--r--   0        0        0    18217 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/xlfd/hbf.py
--rw-r--r--   0        0        0    33895 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/xlfd/pcf.py
--rw-r--r--   0        0        0    25950 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/formats/xlfd/xlfd.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/scripts/__init__.py
--rwxr-xr-x   0        0        0     9544 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/scripts/banner.py
--rwxr-xr-x   0        0        0     3671 2020-02-02 00:00:00.000000 monobit-0.42.2/monobit/scripts/convert.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 monobit-0.42.2/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 monobit-0.42.2/LICENSE
--rw-r--r--   0        0        0    18844 2020-02-02 00:00:00.000000 monobit-0.42.2/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 monobit-0.42.2/pyproject.toml
--rw-r--r--   0        0        0    20797 2020-02-02 00:00:00.000000 monobit-0.42.2/PKG-INFO
+-rw-r--r--   0        0        0    27256 2020-02-02 00:00:00.000000 monobit-0.43.0/YAFF.md
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 monobit-0.43.0/banner.py
+-rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 monobit-0.43.0/convert.py
+-rwxr-xr-x   0        0        0     7145 2020-02-02 00:00:00.000000 monobit-0.43.0/explore.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/__init__.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/constants.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/base/__init__.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/base/basetypes.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/base/binary.py
+-rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/base/blocks.py
+-rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/base/cachedprops.py
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/base/properties.py
+-rw-r--r--   0        0        0     9488 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/base/struct.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/core/__init__.py
+-rw-r--r--   0        0        0    51020 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/core/font.py
+-rw-r--r--   0        0        0    33937 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/core/glyph.py
+-rw-r--r--   0        0        0     9420 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/core/labels.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/core/pack.py
+-rw-r--r--   0        0        0    22882 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/core/raster.py
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/core/vector.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/__init__.py
+-rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/base.py
+-rw-r--r--   0        0        0    18338 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/charmaps.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/definitions.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/indexers.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/registry.py
+-rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/taggers.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/unicode.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/__init__.py
+-rw-r--r--   0        0        0    51488 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/charmaps.json
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/adobe/README.md
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/adobe/ReadMe.txt
+-rw-r--r--   0        0        0     8143 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/adobe/stdenc.txt
+-rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/adobe/symbol.txt
+-rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/adobe/zdingbat.txt
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/agl/LICENSE.md
+-rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/agl/README.md
+-rw-r--r--   0        0        0    27655 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/agl/aglfn.txt
+-rw-r--r--   0        0        0    78060 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/agl/glyphlist.txt
+-rw-r--r--   0        0        0    24830 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/ARABIC.TXT
+-rw-r--r--   0        0        0    13008 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/CELTIC.TXT
+-rw-r--r--   0        0        0    13065 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/CENTEURO.TXT
+-rw-r--r--   0        0        0   197055 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/CHINSIMP.TXT
+-rw-r--r--   0        0        0   323716 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/CHINTRAD.TXT
+-rw-r--r--   0        0        0    26610 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/CORPCHAR.TXT
+-rw-r--r--   0        0        0    13388 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/CROATIAN.TXT
+-rw-r--r--   0        0        0    13497 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/CYRILLIC.TXT
+-rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/DEVANAGA.TXT
+-rw-r--r--   0        0        0    14320 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/DINGBATS.TXT
+-rw-r--r--   0        0        0    23987 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/FARSI.TXT
+-rw-r--r--   0        0        0    14055 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/GAELIC.TXT
+-rw-r--r--   0        0        0    14042 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/GREEK.TXT
+-rw-r--r--   0        0        0    13940 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/GUJARATI.TXT
+-rw-r--r--   0        0        0    16096 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/GURMUKHI.TXT
+-rw-r--r--   0        0        0    27034 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/HEBREW.TXT
+-rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/ICELAND.TXT
+-rw-r--r--   0        0        0    11800 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/INUIT.TXT
+-rw-r--r--   0        0        0   198175 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/JAPANESE.TXT
+-rw-r--r--   0        0        0    10252 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/KEYBOARD.TXT
+-rw-r--r--   0        0        0   369061 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/KOREAN.TXT
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/README.md
+-rw-r--r--   0        0        0    14385 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/ROMAN.TXT
+-rw-r--r--   0        0        0    14153 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/ROMANIAN.TXT
+-rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/ReadMe.txt
+-rw-r--r--   0        0        0    16882 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/SYMBOL.TXT
+-rw-r--r--   0        0        0    15564 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/THAI.TXT
+-rw-r--r--   0        0        0    12808 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/TURKISH.TXT
+-rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/UKRAINE.TXT
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/README.md
+-rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/bulgarian-mik.txt
+-rw-r--r--   0        0        0     7866 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/cp866.txt
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/gost19768-87.txt
+-rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/hp-roman8.txt
+-rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/koi-0.txt
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/koi-7.txt
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/koi8-a.txt
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/koi8-b.txt
+-rw-r--r--   0        0        0     6374 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/koi8-e.txt
+-rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/koi8-f.txt
+-rw-r--r--   0        0        0     7801 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/koi8-r.txt
+-rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/koi8-u.txt
+-rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-ca
+-rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-ca2
+-rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-cn
+-rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-cu
+-rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-de
+-rw-r--r--   0        0        0    11938 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-dk
+-rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-es
+-rw-r--r--   0        0        0    11888 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-es2
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-fr
+-rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-gb
+-rw-r--r--   0        0        0    11997 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-hu
+-rw-r--r--   0        0        0    11926 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-it
+-rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-jp
+-rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-jp-ocr-b
+-rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-kr
+-rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-us
+-rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-yu
+-rw-r--r--   0        0        0    17534 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/jis_x0201
+-rw-r--r--   0        0        0    10319 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/x0201-7
+-rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/emacs/MULE-ethiopic.map
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/emacs/MULE-ipa.map
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/emacs/MULE-is13194.map
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/emacs/MULE-lviscii.map
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/emacs/MULE-sisheng.map
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/emacs/MULE-tibetan.map
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/emacs/MULE-uviscii.map
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/emacs/README.md
+-rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/evertype/ARMENIAN.TXT
+-rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/evertype/GEORGIAN.TXT
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/evertype/README.md
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/1116.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/1117.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/1118.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/1119.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/1125.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/113.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/1131.ucp
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30000.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30001.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30002.ucp
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30003.ucp
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30004.ucp
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30005.ucp
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30006.ucp
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30007.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30008.ucp
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30009.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30010.ucp
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30011.ucp
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30012.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30013.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30014.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30015.ucp
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30016.ucp
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30017.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30018.ucp
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30019.ucp
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30020.ucp
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30021.ucp
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30022.ucp
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30023.ucp
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30024.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30025.ucp
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30026.ucp
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30027.ucp
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30028.ucp
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30029.ucp
+-rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30030.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30031.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30032.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30033.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30034.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30039.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30040.ucp
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/3012.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/3021.ucp
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/3845.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/3846.ucp
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/3848.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/437.ucp
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/57781.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/58152.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/58210.ucp
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/58335.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/59234.ucp
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/59829.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/60258.ucp
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/60853.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/61282.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/62306.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/667.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/668.ucp
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/737.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/770.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/771.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/772.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/773.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/774.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/775.ucp
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/777.ucp
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/778.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/790.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/808.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/848.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/849.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/850.ucp
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/851.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/852.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/853.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/855.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/856.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/857.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/858.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/859.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/860.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/861.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/862.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/863.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/864.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/865.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/866.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/867.ucp
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/869.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/872.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/895.ucp
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/899.ucp
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/991.ucp
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/README.md
+-rw-r--r--   0        0        0     9255 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iana/Amiga-1251
+-rw-r--r--   0        0        0    13371 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iana/PTCP154
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iana/README.md
+-rw-r--r--   0        0        0    14491 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/ibm-cdra/037B34B0.UPMAP100
+-rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/ibm-cdra/038834B0.UPMAP100
+-rw-r--r--   0        0        0   323573 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/ibm-cdra/039E44B0.UPMAP101
+-rw-r--r--   0        0        0   973501 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/ibm-cdra/039F34B0.UPMAP100
+-rw-r--r--   0        0        0    17655 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/ibm-cdra/readme.txt
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/ibm-cdra/url
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/README.md
+-rw-r--r--   0        0        0   177606 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/aix-KSC5601.1987_0-4.3.6.ucm
+-rw-r--r--   0        0        0  1348868 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/cns-11643-1992.ucm
+-rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/ibm-1125_P100-1997.ucm
+-rw-r--r--   0        0        0   433127 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/ibm-1375_P100-2008.ucm
+-rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/ibm-720_P100-1997.ucm
+-rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/ibm-806_P100-1998.ucm
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/ibm-851_P100-1995.ucm
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/ibm-858_P100-1997.ucm
+-rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/ibm-868_P100-1995.ucm
+-rw-r--r--   0        0        0   199596 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/ibm-932_P120-1999.ucm
+-rw-r--r--   0        0        0   351895 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/windows-1361-2000.ucm
+-rw-r--r--   0        0        0   490901 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/windows-936-2000.ucm
+-rw-r--r--   0        0        0     9995 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-1.TXT
+-rw-r--r--   0        0        0    10385 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-10.TXT
+-rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-11.TXT
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-13.TXT
+-rw-r--r--   0        0        0    10459 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-14.TXT
+-rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-15.TXT
+-rw-r--r--   0        0        0    10390 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-16.TXT
+-rw-r--r--   0        0        0    10219 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-2.TXT
+-rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-3.TXT
+-rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-4.TXT
+-rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-5.TXT
+-rw-r--r--   0        0        0     7723 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-6.TXT
+-rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-7.TXT
+-rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-8.TXT
+-rw-r--r--   0        0        0    10030 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-9.TXT
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/README.md
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/ReadMe.txt
+-rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ADAMOS7.TXT
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ADAMSWTR.TXT
+-rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/AMSCPC.TXT
+-rw-r--r--   0        0        0    10266 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/AMSCPM.TXT
+-rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/APL2ALT1.TXT
+-rw-r--r--   0        0        0    10929 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/APL2ALT2.TXT
+-rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/APL2ICHG.TXT
+-rw-r--r--   0        0        0    11100 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/APL2PRIM.TXT
+-rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ATARI8IG.TXT
+-rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ATARI8II.TXT
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ATARI8VG.TXT
+-rw-r--r--   0        0        0    12144 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ATARI8VI.TXT
+-rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ATARISTI.TXT
+-rw-r--r--   0        0        0     9561 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ATARISTV.TXT
+-rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/C64IALT.TXT
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/C64IPRI.TXT
+-rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/C64VALT.TXT
+-rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/C64VPRI.TXT
+-rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/COCOICHG.TXT
+-rw-r--r--   0        0        0    11149 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/COCOSGR4.TXT
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/COCOSGR6.TXT
+-rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/CPETIALT.TXT
+-rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/CPETIPRI.TXT
+-rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/CPETVALT.TXT
+-rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/CPETVPRI.TXT
+-rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/CVICIALT.TXT
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/CVICIPRI.TXT
+-rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/CVICVALT.TXT
+-rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/CVICVPRI.TXT
+-rw-r--r--   0        0        0     8974 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/IBMPCICH.TXT
+-rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/IBMPCVID.TXT
+-rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/MINITLG0.TXT
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/MINITLG1.TXT
+-rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/MSX.TXT
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ORICG0.TXT
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ORICG1.TXT
+-rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/RISCEFF.TXT
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/RISCOSB.TXT
+-rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/RISCOSI.TXT
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/RISCOSV.TXT
+-rw-r--r--   0        0        0    14920 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ReadMe.txt
+-rw-r--r--   0        0        0     9603 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/SINCLRQL.TXT
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TELTXTG0.TXT
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TELTXTG1.TXT
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TELTXTG2.TXT
+-rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TELTXTG3.TXT
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TI994A.TXT
+-rw-r--r--   0        0        0     5639 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM1ICH.TXT
+-rw-r--r--   0        0        0     9089 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM1ORG.TXT
+-rw-r--r--   0        0        0     9064 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM1REV.TXT
+-rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM3IIN.TXT
+-rw-r--r--   0        0        0     8497 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM3IJP.TXT
+-rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM3IRV.TXT
+-rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM3VIN.TXT
+-rw-r--r--   0        0        0     9877 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM3VJP.TXT
+-rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM3VRV.TXT
+-rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM4AIA.TXT
+-rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM4AIP.TXT
+-rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM4AIR.TXT
+-rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM4AVA.TXT
+-rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM4AVP.TXT
+-rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM4AVR.TXT
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZX80.TXT
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZX81.TXT
+-rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXDESKTP.TXT
+-rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXFZXKOI.TXT
+-rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXFZXLT1.TXT
+-rw-r--r--   0        0        0     7590 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXFZXLT5.TXT
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXFZXPUA.TXT
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXFZXSLT.TXT
+-rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXSPCTRM.TXT
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/README.md
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/c0-pictures.txt
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/currency-sign-0x9c.ucp
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/currency-sign-0xdb.ucp
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/dec-vt100.ucp
+-rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/hp48.txt
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/ibm897graph.ucp
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/iso2047.txt
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/mac-cyrillic-pre9.0.ucp
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/mac-system.ucp
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/mac-ukrainian-pre9.0.ucp
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/russup3.ucp
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/russup4ac.ucp
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/russup4na.ucp
+-rw-r--r--   0        0        0     7901 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/windows-1.0.txt
+-rw-r--r--   0        0        0     8028 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/windows-2.0.txt
+-rw-r--r--   0        0        0     9006 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/windows-3.1.txt
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/README.md
+-rw-r--r--   0        0        0     9000 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/EBCDIC/CP037.TXT
+-rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/EBCDIC/CP1026.TXT
+-rw-r--r--   0        0        0     9027 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/EBCDIC/CP500.TXT
+-rw-r--r--   0        0        0     8721 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/EBCDIC/CP875.TXT
+-rw-r--r--   0        0        0     9177 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/MAC/CYRILLIC.TXT
+-rw-r--r--   0        0        0     9413 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/MAC/GREEK.TXT
+-rw-r--r--   0        0        0     9253 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/MAC/ICELAND.TXT
+-rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/MAC/LATIN2.TXT
+-rw-r--r--   0        0        0     9229 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/MAC/ROMAN.TXT
+-rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/MAC/TURKISH.TXT
+-rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP437.TXT
+-rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP737.TXT
+-rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP775.TXT
+-rw-r--r--   0        0        0     9640 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP850.TXT
+-rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP852.TXT
+-rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP855.TXT
+-rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP857.TXT
+-rw-r--r--   0        0        0     9845 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP860.TXT
+-rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP861.TXT
+-rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP862.TXT
+-rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP863.TXT
+-rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP864.TXT
+-rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP865.TXT
+-rw-r--r--   0        0        0     9765 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP866.TXT
+-rw-r--r--   0        0        0     9318 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP869.TXT
+-rw-r--r--   0        0        0     8452 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP874.TXT
+-rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1250.TXT
+-rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1251.TXT
+-rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1252.TXT
+-rw-r--r--   0        0        0     8938 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1253.TXT
+-rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1254.TXT
+-rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1255.TXT
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1256.TXT
+-rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1257.TXT
+-rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1258.TXT
+-rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP874.TXT
+-rw-r--r--   0        0        0   295324 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP932.TXT
+-rw-r--r--   0        0        0   817310 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP936.TXT
+-rw-r--r--   0        0        0   790736 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP949.TXT
+-rw-r--r--   0        0        0   508978 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP950.TXT
+-rw-r--r--   0        0        0    11537 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/APL-ISO-IR-68.TXT
+-rw-r--r--   0        0        0    21171 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/ATARIST.TXT
+-rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/CP1006.TXT
+-rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/CP424.TXT
+-rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/CP856.TXT
+-rw-r--r--   0        0        0     8707 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/GSM0338.TXT
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/IBMGRAPH.TXT
+-rw-r--r--   0        0        0   210734 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/JIS0208.TXT
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/KOI8-R.TXT
+-rw-r--r--   0        0        0    11041 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/KOI8-U.TXT
+-rw-r--r--   0        0        0   784637 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/KPS9566.TXT
+-rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/KZ1048.TXT
+-rw-r--r--   0        0        0     7093 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/NEXTSTEP.TXT
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/README.md
+-rw-r--r--   0        0        0    49569 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/SGML.TXT
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/US-ASCII-QUOTES.TXT
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/dashen-map.txt
+-rw-r--r--   0        0        0    92930 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/ibm-ugl.txt
+-rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/mleisher/ALTVAR.TXT
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/mleisher/ARMSCII-7.TXT
+-rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/mleisher/ARMSCII-8.TXT
+-rw-r--r--   0        0        0     9049 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/mleisher/ARMSCII-8A.TXT
+-rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/mleisher/DECMCS.TXT
+-rw-r--r--   0        0        0     9870 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/mleisher/GEO-ITA.TXT
+-rw-r--r--   0        0        0     9758 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/mleisher/GEO-PS.TXT
+-rw-r--r--   0        0        0    13439 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/mleisher/IRANSYSTEM.TXT
+-rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/mleisher/KOI8RU.TXT
+-rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/mleisher/OSNOVAR.TXT
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/mleisher/README.md
+-rw-r--r--   0        0        0     9566 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/mleisher/TIS620.TXT
+-rw-r--r--   0        0        0   274176 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/moztw/big5_2003-b2u.txt
+-rw-r--r--   0        0        0   340277 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/moztw/eten.txt
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/moztw/url
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/python/README.md
+-rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/python/TCVN5712-1.TXT
+-rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/python/TCVN5712-2.TXT
+-rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/python/TCVN5712-3.TXT
+-rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/vietstd/unicode.html
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/vietstd/url
+-rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/vietstd/viscii1.1.txt
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/README.md
+-rw-r--r--   0        0        0   156347 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/abicomp.html
+-rw-r--r--   0        0        0   180593 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/brascii.html
+-rw-r--r--   0        0        0   144572 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/cp853.html
+-rw-r--r--   0        0        0   156279 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/cwi2.html
+-rw-r--r--   0        0        0   134679 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/dec-special.html
+-rw-r--r--   0        0        0   153445 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/dec-technical.html
+-rw-r--r--   0        0        0   192405 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/gem.html
+-rw-r--r--   0        0        0   172501 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/kamenicky.html
+-rw-r--r--   0        0        0   216297 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/lics.html
+-rw-r--r--   0        0        0   150793 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/mattel-aquarius.html
+-rw-r--r--   0        0        0   159296 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/mazovia.html
+-rw-r--r--   0        0        0   167964 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/pascii.html
+-rw-r--r--   0        0        0   217224 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/ventura.html
+-rw-r--r--   0        0        0   254035 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/windows-1252.html
+-rw-r--r--   0        0        0   245126 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/wingdings.html
+-rw-r--r--   0        0        0   160779 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/wiscii.html
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/xfonts/README.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/xfonts/mulearabic-0.enc
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/xfonts/mulearabic-1.enc
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/xfonts/mulearabic-2.enc
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/xfonts/mulelao-1.enc
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/xfonts/suneu-greek.enc
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/plumbing/__init__.py
+-rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/plumbing/args.py
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/plumbing/help.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/plumbing/history.py
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/plumbing/scripting.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/render/__init__.py
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/render/chart.py
+-rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/render/glyphmap.py
+-rw-r--r--   0        0        0    13254 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/render/renderer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/scripts/__init__.py
+-rwxr-xr-x   0        0        0     9536 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/scripts/banner.py
+-rwxr-xr-x   0        0        0     3293 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/scripts/convert.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/__init__.py
+-rw-r--r--   0        0        0    10443 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/converters.py
+-rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/magic.py
+-rw-r--r--   0        0        0     7817 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/streams.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/containers/__init__.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/containers/container.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/containers/directory.py
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/containers/tar.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/containers/zip.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/__init__.py
+-rw-r--r--   0        0        0    14372 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/amiga.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/bbc.py
+-rw-r--r--   0        0        0     9428 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/common.py
+-rw-r--r--   0        0        0    22576 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/cpi.py
+-rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/daisydot.py
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/dashen.py
+-rw-r--r--   0        0        0    13377 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/dec.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/dosstart.py
+-rw-r--r--   0        0        0    11173 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/figlet.py
+-rw-r--r--   0        0        0     6163 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fontx.py
+-rw-r--r--   0        0        0    11297 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fzx.py
+-rw-r--r--   0        0        0    25615 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/gdos.py
+-rw-r--r--   0        0        0    12651 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/geos.py
+-rw-r--r--   0        0        0    10476 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/nearlyraw.py
+-rw-r--r--   0        0        0    29873 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/pcl.py
+-rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/pcpaint.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/pdf.py
+-rw-r--r--   0        0        0    12842 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/pkfont.py
+-rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/prebuilt.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/printshop.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/psf.py
+-rw-r--r--   0        0        0     8611 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/raw.py
+-rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/signum.py
+-rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/vfont.py
+-rw-r--r--   0        0        0    12487 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/xerox.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/apple/__init__.py
+-rw-r--r--   0        0        0    21642 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/apple/dfont.py
+-rw-r--r--   0        0        0    29326 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/apple/fond.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/apple/iigs.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/apple/lisa.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/apple/mgtk.py
+-rw-r--r--   0        0        0    27670 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/apple/nfnt.py
+-rw-r--r--   0        0        0     8335 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/apple/palm.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fon/__init__.py
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fon/fon.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fon/mz.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fon/os2/__init__.py
+-rw-r--r--   0        0        0    21331 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fon/os2/gpifont.py
+-rw-r--r--   0        0        0    11075 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fon/os2/lx.py
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fon/os2/ne.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fon/windows/LICENSE.md
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fon/windows/__init__.py
+-rw-r--r--   0        0        0    25636 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fon/windows/fnt.py
+-rw-r--r--   0        0        0    14238 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fon/windows/ne.py
+-rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fon/windows/pe.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/image/__init__.py
+-rw-r--r--   0        0        0    40795 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/image/bmfont.py
+-rw-r--r--   0        0        0    10995 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/image/image.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/sfnt/__init__.py
+-rw-r--r--   0        0        0    29213 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/sfnt/sfnt.py
+-rw-r--r--   0        0        0    17626 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/sfnt/sfnt_writer.py
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/sfnt/fonttools/E_B_S_C_.py
+-rw-r--r--   0        0        0     6239 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/sfnt/fonttools/__init__.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/sfnt/fonttools/_b_d_a_t.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/sfnt/fonttools/_b_h_e_d.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/sfnt/fonttools/_b_l_o_c.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/text/__init__.py
+-rw-r--r--   0        0        0    17135 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/text/draw.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/text/edwin.py
+-rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/text/hex.py
+-rw-r--r--   0        0        0    14694 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/text/yaff.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/vector/__init__.py
+-rw-r--r--   0        0        0     8053 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/vector/borland.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/vector/hurt.py
+-rw-r--r--   0        0        0     8489 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/vector/svg.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/xlfd/__init__.py
+-rw-r--r--   0        0        0    18342 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/xlfd/bdf.py
+-rw-r--r--   0        0        0    18138 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/xlfd/hbf.py
+-rw-r--r--   0        0        0    33850 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/xlfd/pcf.py
+-rw-r--r--   0        0        0    25969 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/xlfd/xlfd.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/wrappers/__init__.py
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/wrappers/apple.py
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/wrappers/binhex.py
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/wrappers/compressors.py
+-rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/wrappers/macbinary.py
+-rw-r--r--   0        0        0    15800 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/wrappers/source.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 monobit-0.43.0/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 monobit-0.43.0/LICENSE
+-rw-r--r--   0        0        0    18929 2020-02-02 00:00:00.000000 monobit-0.43.0/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 monobit-0.43.0/pyproject.toml
+-rw-r--r--   0        0        0    20882 2020-02-02 00:00:00.000000 monobit-0.43.0/PKG-INFO
```

### Comparing `monobit-0.42.2/YAFF.md` & `monobit-0.43.0/YAFF.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,19 +51,18 @@
     notice:
         Test is the property of T€$ţ0Яζ Inc.
         It's not a very useful font.
     encoding: totally-made-up
 
     # glyph definitions follow after the global properties section
 
-    # The letter A is the first letter of the Latin alphabet.
     # We've got three kinds of labels: unicode character, codepage, and tag.
     u+0041:
     0x41:
-    latin_a:
+    "latin_a":
         ....
         .@..
         @.@.
         @@@.
         @.@.
         @.@.
 
@@ -76,44 +75,42 @@
         @@@..
         @..@.
         @@@..
 
 
     # Or for example, just a tag.
     # A glyph may contain per-glyph metrics
-    latin_c:
+    "latin_c":
         ....
         .@@.
         @..@
         @...
         @..@
         .@@.
 
-        tracking: 1
+        right-bearing: 1
 
 
     # This is a special notation for a 0x0 empty glyph, with the tag "empty".
-    empty:
+    "empty":
         -
 
-    # Multiple labels of the same type are OK. Numbers may be decimal, too.
+    # Numbers may be decimal, too.
     # Glyphs don't need to be the same width or height
-    0x01:
-    0x02:
     255:
-    smiley:
+    "smiley":
         ......
         .@..@.
         ......
         .@..@.
         ..@@..
 
     # Multiple code points may define a grapheme cluster
     u+0061, u+0300:
-    small_a_grave:
+    "small_a_grave":
         @...
         .@..
         ....
         .@@.
         @.@.
         @.@.
         .@@@
@@ -126,16 +123,15 @@
         .@.@.
         .@.@.
         @@@@@
         .@.@.
         .@.@.
         .@.@.
 
-    # While double quotes ensure a label is interpreted as a tag
-    "my_à":
+    'à':
         @...
         .@..
         ....
         .@@.
         @.@.
         @.@.
         .@@@
@@ -204,14 +200,15 @@
 A *glyph definition* consists of one or more *labels*, followed by a *glyph*. If there are multiple
 labels, all are considered to point to the glyph that follows.
 
 ##### Labels
 A *label* must be followed by a separator `:`, optional whitespace, and a line ending.
 * The label must be given at the start of the line. Leading whitespace is not allowed.
 * A label has one of three types: *character*, *codepoint*, or *tag*.
+* Multiple labels of the same type are allowed, but deprecated.
 
 If a label starts with an ASCII digit, it is a *codepoint*.
 * A codepoint label may consist of multiple elements, separated by commas and optional whitespace.
 * Each element represents an unsigned integer value.
 * If all characters in the element are digits, the element is in decimal format.
   Leading `0`s in decimals are allowed.
 * If the first two characters are `0x` or `0X`, the element is hexadecimal. All further characters
@@ -224,40 +221,48 @@
 Examples of valid codepoint labels are `32`, `0032`, `0x20`, `0o24`, (all of which refer to the same
 codepoint). Further examples are `0x120`, `0x1, 0x20`, `1, 32` (all of which are the same multi-byte
 codepoint sequence).
 
 
 If a label:
 * is enclosed by single quote characters `'`, **or**
-* starts with `u+` or `U+`, **or**
-* starts with a character that is not in 7-bit ASCII, **or**
-* consists of a single Unicode character
+* starts with `u+` or `U+`
 
 it is a *character* label, which may be a grapheme sequence consisting of multiple Unicode code points.
 * A character label may consist of multiple elements, separated by commas and optional whitespace.
 * Each element must start with `u+` or `U+` or be enclosed in single quotes.
 * If an element starts with `u+` or `U+`, it must be followed by hex digits. It represents a Unicode point in hexadecimal notation.
   The hex digits are not case sensitive.
 * If a label element starts and ends with a single-quote character `'`,
   these quotes are stripped and the element consists of everything in between.
 
-Examples of valid character labels are `A`, `À`, `安` (all of which are single characters), `ते`
+Examples of valid character labels are `'A'`, `'À'`, `'安'` (all of which are single characters), `'ते'`
 (a grapheme sequence consisting of multiple non-ASCII characters), its equivalent `u+0924, u+0947`,
- and `'ffi'` (multiple characters enclosed in single quotes).
+and `'ffi'` (multiple characters enclosed in single quotes).
+
+It is also possible, but deprecated, to create a character label as a label that:
+* starts with a character that is not in 7-bit ASCII, **or**
+* consists of a single Unicode character that is not an ASCII digit
+
+Examples of deprecated character labels are the unquoted `A`, `À`, `安` (all of which are single characters), `ते`
+(a grapheme sequence consisting of multiple non-ASCII characters)
 
 If a label:
-* is enclosed in double quote characters `"`, **or**
-* starts with an ASCII letter, is at least 2 characters long, and consists only of
-  ASCII letters, ASCII digits, the underscore `_`, the dash `-`, or the full stop `.`,
+* is enclosed in double quote characters `"`
 
 it is a *tag*.
-* Tags are case-sensitive and (if double-quoted) may contain any kind of character.
+* Tags are case-sensitive and may contain any kind of character.
 * If a label starts and ends with a double-quote character `"`,
   these quotes are stripped and the tag consists of everything in between.
 
+It is also possible, but deprecated, to create a tag as a label that
+* starts with an ASCII letter, is at least 2 characters long, and consists only of
+ASCII letters, ASCII digits, the underscore `_`, the dash `-`, or the full stop `.`,
+
+
 ##### Glyphs
 
 A *glyph* may span multiple lines.
 * The lines of a glyph must start with whitespace (the _indent_). Trailing whitespace is allowed.
 * All lines of the glyph must have identical indent.
 * If a glyph consists of the character `-` only, it is the empty glyph.
 * Otherwise, the glyph must consist of the characters `.` and `@` only.
```

### Comparing `monobit-0.42.2/explore.py` & `monobit-0.43.0/explore.py`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/basetypes.py` & `monobit-0.43.0/monobit/base/basetypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 """
-monobit.basetypes - base data types and converters
+monobit.base.basetypes - base data types and converters
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 from collections import namedtuple
 from functools import partial
 from typing import Any
 from numbers import Real
 
 
+# sentinel object
+NOT_SET = ...
+
+
 def passthrough(var):
     """Passthrough type."""
     return var
 
 def to_int(int_str):
     """Convert from int-like or string in any representation."""
     if isinstance(int_str, int):
```

### Comparing `monobit-0.42.2/monobit/binary.py` & `monobit-0.43.0/monobit/base/binary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-monobit.binary - binary utilities
+monobit.base.binary - binary utilities
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 
 def ceildiv(num, den):
```

### Comparing `monobit-0.42.2/monobit/blocks.py` & `monobit-0.43.0/monobit/base/blocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-monobit.blocks - output pixels as text using block elements
+monobit.base.blocks - output pixels as text using block elements
 
 (c) 2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from itertools import zip_longest
```

### Comparing `monobit-0.42.2/monobit/cachedprops.py` & `monobit-0.43.0/monobit/base/cachedprops.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-monobit.cachedprops - defaultable, cached property sets with type conversion
+monobit.base.cachedprops - defaultable, cached property sets with type conversion
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 
 import logging
```

### Comparing `monobit-0.42.2/monobit/chart.py` & `monobit-0.43.0/monobit/render/chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
-monobit.chart - create font chart
+monobit.render.chart - create font chart
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 from itertools import product
 
-from .binary import ceildiv
-from .properties import Props
-from .basetypes import Coord
+from ..base.binary import ceildiv
+from ..base import Props
+from ..base import Coord
 from .glyphmap import GlyphMap
 
 
 def chart(
         font,
         columns=32, margin=(0, 0), padding=(0, 0),
         order='row-major', direction=(1, -1),
```

### Comparing `monobit-0.42.2/monobit/font.py` & `monobit-0.43.0/monobit/core/font.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 """
-monobit.font - representation of font
+monobit.core.font - representation of font
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
-from functools import wraps, partial, cache
+from functools import wraps, partial, cache, cached_property
+from itertools import chain
 from pathlib import PurePath
 from unicodedata import normalize
 
-from .scripting import scriptable, get_scriptables, Any
-from .glyph import Glyph
-from .raster import turn_method, NOT_SET
-from .basetypes import Coord, Bounds
-from .basetypes import to_int
-from .encoding import charmaps, encoder, EncodingName, Encoder, Indexer
-from .taggers import tagger
-from .labels import Tag, Char, Codepoint, Label, to_label
-from .binary import ceildiv
-from .properties import extend_string
-from .cachedprops import HasProps, writable_property, checked_property
-from .taggers import tagmaps
-
+from monobit.plumbing.scripting import scriptable
+from monobit.base import Coord, Bounds, NOT_SET
+from monobit.base import to_int, Any
+from monobit.encoding import encoder, EncodingName, Encoder, Indexer, Charmap
+from monobit.base.binary import ceildiv
+from monobit.base import extend_string
+from monobit.base import HasProps, writable_property, checked_property
 
-def encoder_or_tagger(obj):
-    enc = encoder(obj)
-    if enc is None:
-        return tagger(obj)
-    return enc
+from .labels import Tag, Char, Codepoint, Label, to_label
+from .glyph import Glyph
+from .raster import turn_method
 
 
 ###############################################################################
 # font class
 
 # pylint: disable=redundant-keyword-arg, no-member
 class FontProperties:
@@ -136,15 +129,15 @@
     right_extent: int
     # horizontal distance between consecutive baselines, in pixels
     line_width: int
 
     # encoding parameters
 
     # character map, stored as normalised name
-    encoding: EncodingName
+    encoding: EncodingName = ''
     # replacement for missing glyph
     default_char: Label
     # word-break character (usually space)
     word_boundary: Label = Char(' ')
 
     # rendering hints
     # may affect rendering if effects are applied
@@ -266,21 +259,14 @@
             dpi = (72 * self.pixel_size) // self.point_size
         else:
             # default: 72 dpi; 1 point == 1 pixel
             dpi = 72
         # stretch/shrink dpi.x if aspect ratio is not square
         return Coord((dpi*self.pixel_aspect.x)//self.pixel_aspect.y, dpi)
 
-    @writable_property
-    def encoding(self):
-        """Encoding."""
-        # if we have no codepoints, we can always assume unicode encoding
-        if self.get_chars() and not self.get_codepoints():
-            return charmaps.normalise('unicode')
-        return ''
 
     ##########################################################################
     # metrics
 
     @writable_property
     def line_height(self):
         """Vertical distance between consecutive baselines, in pixels."""
@@ -654,33 +640,51 @@
 
     ###########################################################################
 
 
     def __init__(self, glyphs=(), *, comment=None, **properties):
         """Create new font."""
         super().__init__()
-        self._glyphs = tuple(glyphs)
-        # construct lookup tables
-        self._labels = {
-            _label: _index
-            for _index, _glyph in enumerate(self._glyphs)
-            for _label in _glyph.get_labels()
-        }
         # comment can be str (just global comment) or mapping of property comments
+        self._comment = {}
         if isinstance(comment, str):
-            comment = {'': comment}
-        else:
-            comment = comment or {}
+            self._comment[''] = comment
+        elif comment:
+            self._comment.update(comment)
+        self._glyphs = tuple(glyphs)
+        # update glyph list, apply globally specified metrics
         self._glyphs, properties = self._apply_metrics(self._glyphs, properties)
-        self._comment = {**comment}
         # update properties
         # NOTE - we must be careful NOT TO ACCESS CACHED PROPERTIES
         #        until the constructor is complete
         self._set_properties(properties)
 
+    @cached_property
+    def _labels(self):
+        """Label lookup table."""
+        label_map = {
+            _label: _index
+            for _index, _glyph in enumerate(self._glyphs)
+            for _label in _glyph.get_labels()
+        }
+        font_encoder = encoder(self.encoding)
+        if not font_encoder:
+            return label_map
+        char_label_map = {
+            font_encoder.char(_label): _index
+            for _label, _index in label_map.items()
+        }
+        char_label_map.pop(Char(''), None)
+        codepoint_label_map = {
+            font_encoder.codepoint(_label): _index
+            for _label, _index in label_map.items()
+        }
+        codepoint_label_map.pop(Codepoint(b''), None)
+        return char_label_map | codepoint_label_map | label_map
+
     @staticmethod
     def _apply_metrics(glyphs, props):
         """Apply globally specified glyph metrics."""
         glyph_metrics = {
             _k: props[_k]
             for _k in (
                 'shift_up', 'left_bearing', 'right_bearing',
@@ -710,15 +714,15 @@
 
     ##########################################################################
     # representation
 
     def __repr__(self):
         """Representation."""
         elements = (
-            f'glyphs=(...{len(self._glyphs)} glyphs...)' if self._glyphs else '',
+            f'glyphs=<{len(self._glyphs)} glyphs>' if self._glyphs else '',
             ',\n    '.join(
                 f'{_k}={repr(_v)}'
                 for _k, _v in self.get_properties().items()
             ),
         )
         return '{}({})'.format(
             type(self).__name__,
@@ -848,20 +852,21 @@
         indices = (self.get_index(_c) for _c in char)
         indices = tuple(indices)
         return Glyph.overlay(*(self._glyphs[_i] for _i in indices))
 
     def get_glyph(
             self, label=None, *,
             char=None, codepoint=None, tag=None,
-            missing='raise'
+            missing='raise', use_encoding=True
         ):
         """Get glyph by char, codepoint or tag; default if not present."""
         try:
             index = self.get_index(
-                label, tag=tag, char=char, codepoint=codepoint
+                label, tag=tag, char=char, codepoint=codepoint,
+                use_encoding=use_encoding,
             )
             return self.glyphs[index]
         except KeyError:
             label = to_label(label)
             # if not found and the label is a composed unicode character
             # try to compose the glyph from its elements
             if isinstance(label, Char):
@@ -877,15 +882,18 @@
                 return self.get_default_glyph()
             if missing == 'empty':
                 return self.get_empty_glyph()
             if missing is None or isinstance(missing, Glyph):
                 return missing
             raise
 
-    def get_index(self, label=None, *, char=None, codepoint=None, tag=None):
+    def get_index(
+            self, label=None, *, char=None, codepoint=None, tag=None,
+            use_encoding=True, raise_missing=True,
+        ):
         """Get index for given label, if defined."""
         if 1 != len([
                 _indexer for _indexer in (label, char, codepoint, tag)
                 if _indexer is not None
             ]):
             raise ValueError('get_index() takes exactly one parameter.')
         if char is not None:
@@ -900,15 +908,17 @@
         elif label is not None:
             # convert strings, numerics through standard rules
             label = to_label(label)
         try:
             return self._labels[label]
         except KeyError:
             pass
-        raise KeyError(f'No glyph found matching label={label}')
+        if raise_missing:
+            raise KeyError(f'No glyph found matching label={label}')
+        return -1
 
     @cache
     def get_default_glyph(self):
         """Get default glyph; empty if not defined."""
         try:
             return self.get_glyph(self.default_char, missing='raise')
         except KeyError:
@@ -947,30 +957,31 @@
     def get_tags(self):
         """Get tuple of tags covered by this font."""
         return tuple(_c for _c in self._labels if isinstance(_c, Tag))
 
     @cache
     def get_charmap(self):
         """Implied character map based on defined chars."""
-        return charmaps.create({
+        return Charmap({
             _glyph.codepoint: _glyph.char
             for _glyph in self._glyphs
             if _glyph.codepoint
             and _glyph.char
         }, name=f"implied-{self.name}")
 
 
     ##########################################################################
     # font operations
 
+
     @scriptable
     def label(
             self, *,
-            codepoint_from:encoder=NOT_SET, char_from:encoder_or_tagger=NOT_SET,
-            tag_from:tagger=NOT_SET, comment_from:tagger=NOT_SET,
+            codepoint_from:encoder=NOT_SET, char_from:encoder=NOT_SET,
+            tag_from:encoder=NOT_SET, comment_from:encoder=NOT_SET,
             overwrite:bool=False,
             match_whitespace:bool=True, match_graphical:bool=True
         ):
         """
         Add character and codepoint labels.
 
         codepoint_from: encoder registered name or filename to use to set codepoints from character labels
@@ -1003,54 +1014,137 @@
                 encoding = char_from.name
             # don't set encoding if we use an Indexer
             elif (
                 isinstance(codepoint_from, Encoder)
                 and not isinstance(codepoint_from, Indexer)
             ):
                 encoding = codepoint_from.name
-        kwargs = dict(
-            overwrite=overwrite,
-            match_whitespace=match_whitespace,
-            match_graphical=match_graphical,
-        )
-        if codepoint_from is not NOT_SET:
-            kwargs.update(dict(codepoint_from=codepoint_from))
-        elif char_from is not NOT_SET:
-            kwargs.update(dict(char_from=char_from))
-        elif tag_from is not NOT_SET:
-            kwargs.update(dict(tag_from=tag_from))
-        elif comment_from is not NOT_SET:
-            kwargs.update(dict(comment_from=comment_from))
-        else:
-            return self
-        return self.modify(encoding=encoding, glyphs=tuple(
-            _glyph.label(**kwargs)
+        glyphs = tuple(
+            _glyph.label(
+                overwrite=overwrite,
+                match_whitespace=match_whitespace,
+                match_graphical=match_graphical,
+                char_from=char_from,
+                codepoint_from=codepoint_from,
+                tag_from=tag_from,
+                comment_from=comment_from,
+            )
             for _glyph in self.glyphs
-        ))
+        )
+        glyphs, references = self._relink_glyphs(glyphs)
+        return self.modify(glyphs=glyphs, encoding=encoding, **references)
+
+
+    def _relink_glyphs(self, glyphs):
+        """Update label and kerning table references after relabelling."""
+
+        def _update_label(old_label):
+            index = self.get_index(old_label, raise_missing=False)
+            if index < 0:
+                return None
+            labels = glyphs[index].get_labels()
+            # drop references if referenced glyph has no labels
+            if not labels:
+                return None
+            return labels[0]
+
+        references = {
+            _k: _update_label(_v)
+            for _k, _v in self._props.items()
+            if isinstance(_v, Label)
+        }
+        left_kerning = (
+            {_update_label(_k): _v for _k, _v in _glyph.left_kerning.items()}
+            for _glyph in glyphs
+        )
+        right_kerning = (
+            {_update_label(_k): _v for _k, _v in _glyph.right_kerning.items()}
+            for _glyph in glyphs
+        )
+        glyphs = tuple(
+            _g.modify(left_kerning=_l, right_kerning=_r)
+            for _g, _l, _r in zip(glyphs, left_kerning, right_kerning)
+        )
+        return glyphs, references
 
     @scriptable
     def subset(
             self, labels:tuple[Label]=(), *,
             chars:tuple[Char]=(), codepoints:tuple[Codepoint]=(), tags:tuple[Tag]=(),
         ):
         """
         Return a subset of the font.
 
         labels: chars, codepoints or tags to include
         chars: chars to include
         codepoints: codepoints to include
         tags: tags to include
         """
+        labels = (
+            list(labels)
+            + [Char(_c) for _c in chars]
+            + [Codepoint(_c) for _c in codepoints]
+            + [Tag(_t) for _t in tags]
+        )
+        indices = set(
+            self.get_index(_label, raise_missing=False, use_encoding=True)
+            for _label in labels
+        )
+        glyphs = (self._glyphs[_idx] for _idx in sorted(indices) if _idx > -1)
+        return self.modify(glyphs)
+
+    @scriptable
+    def resample(
+            self, labels:tuple[Label]=(), *,
+            chars:tuple[Char]=(), codepoints:tuple[Codepoint]=(), tags:tuple[Tag]=(),
+            encoding:encoder=None, missing:Any='default',
+        ):
+        """
+        Return a (contiguous) sample of the font, filling in missing glyphs.
+        Changes the labels of the subsampled glyphs to those provided.
+
+        labels: chars, codepoints or tags to include.
+        chars: chars to include
+        codepoints: codepoints to include
+        tags: tags to include
+        encoding: encoding from which to sample all codepoints.
+        missing: how to deal with missing glyphs. 'default', 'empty', 'raise', None, or a user-defined Glyph
+        """
+        nargs = sum(
+            bool(_arg) for _arg in (labels, chars, codepoints, tags, encoding)
+        )
+        if nargs > 1:
+            raise ValueError('Can only set one of labels, chars, codepoints, tags, encoding.')
+        if encoding:
+            encoding = encoder(encoding)
+            chars = (Char(_c) for _c in encoding.mapping.values())
+        else:
+            chars = (Char(_c) for _c in chars)
+            codepoints = (Codepoint(_c) for _c in codepoints)
+            tags = (Tag(_t) for _t in tags)
+        labels = tuple(chain(labels, chars, codepoints, tags))
         glyphs = (
-            [self.get_glyph(_label, missing=None) for _label in labels]
-            + [self.get_glyph(char=_char, missing=None) for _char in chars]
-            + [self.get_glyph(codepoint=_codepoint, missing=None) for _codepoint in codepoints]
-            + [self.get_glyph(tag=_tag, missing=None) for _tag in tags]
+            self.get_glyph(_label, missing=missing, use_encoding=True)
+            for _label in labels
         )
-        return self.modify(_glyph for _glyph in glyphs if _glyph is not None)
+        glyphs, labels = zip(*(
+            (_g, _l) for _g, _l in zip(glyphs, labels) if _g is not None
+        ))
+        font = self.modify(glyphs)
+        # if missing=None, drop missing glyphs
+        glyphs = tuple(
+            _g.modify(labels=[_label])
+            for _g, _label in zip(glyphs, labels)
+        )
+        glyphs, references = font._relink_glyphs(glyphs)
+        font = font.modify(glyphs, **references)
+        if encoding:
+            font = font.label(codepoint_from=encoding, overwrite=True)
+        return font
+
 
     @scriptable
     def exclude(
             self, labels:tuple[Label]=(), *,
             chars:tuple[Char]=(), codepoints:tuple[Codepoint]=(), tags:tuple[Tag]=(),
         ):
         """
@@ -1120,30 +1214,30 @@
             return self.append(comment=comment)
         return self.modify(comment=comment)
 
 
     ##########################################################################
     # transformations
 
-    def _apply_to_all_glyphs(self, operation, **kwargs):
+    def for_all(self, operation, **kwargs):
         glyphs = tuple(
             operation(_g, **kwargs) for _g in self.glyphs
         )
         return self.modify(glyphs)
 
     # orthogonal transformations
 
     @scriptable
     def mirror(self, *, adjust_metrics:bool=True):
         """
         Reverse horizontally.
 
         adjust_metrics: also reverse metrics (default: True)
         """
-        font = self._apply_to_all_glyphs(
+        font = self.for_all(
             Glyph.mirror, adjust_metrics=adjust_metrics
         )
         if not adjust_metrics:
             return font
         return font.modify(
             direction={
                 'left-to-right': 'right-to-left',
@@ -1154,15 +1248,15 @@
     @scriptable
     def flip(self, *, adjust_metrics:bool=True):
         """
         Reverse vertically.
 
         adjust_metrics: also reverse metrics (default: True)
         """
-        font = self._apply_to_all_glyphs(
+        font = self.for_all(
             Glyph.flip, adjust_metrics=adjust_metrics
         )
         if not adjust_metrics:
             return font
         return font.modify(
             direction={
                 'top-to-bottom': 'bottom-to-top',
@@ -1173,15 +1267,15 @@
     @scriptable
     def transpose(self, *, adjust_metrics:bool=True):
         """
         Swap horizontal and vertical directions.
 
         adjust_metrics: also transpose metrics (default: True)
         """
-        font = self._apply_to_all_glyphs(
+        font = self.for_all(
             Glyph.transpose, adjust_metrics=adjust_metrics
         )
         if not adjust_metrics:
             return font
         return font.modify(
             line_height=font.line_width,
             line_width=font.line_height,
@@ -1208,15 +1302,15 @@
 
         left: number of columns to remove from left
         bottom: number of rows to remove from bottom
         right: number of columns to remove from right
         top: number of rows to remove from top
         adjust_metrics: make the operation render-invariant (default: True)
         """
-        font = self._apply_to_all_glyphs(
+        font = self.for_all(
             Glyph.crop,
             left=left, bottom=bottom, right=right, top=top, adjust_metrics=adjust_metrics
         )
         if not adjust_metrics:
             return font
         # fix line-advances to ensure they remain unchanged
         return font.modify(
@@ -1234,15 +1328,15 @@
 
         left: number of columns to add on left
         bottom: number of rows to add on bottom
         right: number of columns to add on right
         top: number of rows to add on top
         adjust_metrics: make the operation render-invariant (default: True)
         """
-        font = self._apply_to_all_glyphs(
+        font = self.for_all(
             Glyph.expand,
             left=left, bottom=bottom, right=right, top=top,
             adjust_metrics=adjust_metrics
         )
         if not adjust_metrics:
             return font
         # fix line-advances to ensure they remain unchanged
@@ -1254,15 +1348,15 @@
     @scriptable
     def reduce(self, *, adjust_metrics:bool=True):
         """
         Reduce glyphs to their bounding box.
 
         adjust_metrics: make the operation render-invariant (default: True)
         """
-        font = self._apply_to_all_glyphs(
+        font = self.for_all(
             Glyph.reduce,
             adjust_metrics=adjust_metrics,
             create_vertical_metrics=self.has_vertical_metrics(),
         )
         if not adjust_metrics:
             return font
         # fix line-advances to ensure they remain unchanged
@@ -1311,15 +1405,15 @@
 
         factor_x: number of times to repeat horizontally
         factor_y: number of times to repeat vertically
         adjust_metrics: also stretch metrics (default: True)
         """
         if (factor_x, factor_y) == (1, 1):
             return self
-        font = self._apply_to_all_glyphs(
+        font = self.for_all(
             Glyph.stretch,
             factor_x=factor_x, factor_y=factor_y,
             adjust_metrics=adjust_metrics,
         )
         if not adjust_metrics:
             return font
         # fix line-advances to ensure they remain unchanged
@@ -1338,15 +1432,15 @@
 
         factor_x: factor to shrink horizontally
         factor_y: factor to shrink vertically
         adjust_metrics: also stretch metrics (default: True)
         """
         if (factor_x, factor_y) == (1, 1):
             return self
-        font = self._apply_to_all_glyphs(
+        font = self.for_all(
             Glyph.shrink,
             factor_x=factor_x, factor_y=factor_y,
             adjust_metrics=adjust_metrics,
         )
         if not adjust_metrics:
             return font
         # fix line-advances to ensure they remain unchanged
@@ -1374,15 +1468,15 @@
         """
         if set((left, down, right, up)) == set((None,)):
             right = self.bold_smear
         right = right or 0
         left = left or 0
         down = down or 0
         up = up or 0
-        return self._apply_to_all_glyphs(
+        return self.for_all(
             Glyph.smear,
             left=left, down=down, right=right, up=up,
             adjust_metrics=adjust_metrics,
         )
 
     @scriptable
     def underline(self, descent:int=None, thickness:int=None):
@@ -1394,61 +1488,42 @@
         thickness: number of pixels the underline extends downward
                    (default: use underline-thickness value)
         """
         if descent is None:
             descent = self.underline_descent
         if thickness is None:
             thickness = self.underline_thickness
-        return self._apply_to_all_glyphs(
+        return self.for_all(
             Glyph.underline,
             descent=descent, thickness=thickness
         )
 
     @scriptable
     def shear(self, *, direction:str='right', pitch:Coord=None):
         """
-        Create a slant by dislocating diagonally, keeping
-        the horizontal baseline fixed.
+        Create a slant by dislocating diagonally, keeping the horizontal baseline fixed.
 
         direction: direction to move the top of the glyph (default: 'right').
         pitch: angle of the slant, given as (x, y) coordinate
                (default: use italic-pitch value).
         """
         if pitch is None:
             pitch = self.italic_pitch
-        return self._apply_to_all_glyphs(
+        return self.for_all(
             Glyph.shear,
             direction=direction, pitch=pitch
         )
 
     @scriptable
     def outline(self, *, thickness:int=None):
         """
         Outline glyph.
 
         thickness: number of pixels in outline in each direction
                    (default: use outline-thickness value).
         """
         if thickness is None:
             thickness = self.outline_thickness
-        return self._apply_to_all_glyphs(
+        return self.for_all(
             Glyph.outline,
             thickness = thickness
         )
-
-
-    # inject remaining Glyph transformations into Font
-
-    for _name, _func in get_scriptables(Glyph).items():
-        if _name not in locals():
-
-            @scriptable
-            @wraps(_func)
-            def _modify_glyphs(self, _func=_func, **kwargs):
-                return self._apply_to_all_glyphs(_func, **kwargs)
-
-            locals()[_name] = _modify_glyphs
-
-
-
-# scriptable font/glyph operations
-operations = get_scriptables(Font)
```

### Comparing `monobit-0.42.2/monobit/glyph.py` & `monobit-0.43.0/monobit/core/glyph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
-monobit.glyph - representation of single glyph
+monobit.core.glyph - representation of single glyph
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from functools import cache
 
-from .encoding import is_graphical, is_blank
-from .labels import Codepoint, Char, Tag, to_label
-from .raster import Raster, NOT_SET, turn_method
-from .properties import Props, extend_string
-from .cachedprops import HasProps, checked_property, writable_property
-from .basetypes import Coord, Bounds, to_number
-from .scripting import scriptable
+from monobit.encoding.unicode import is_graphical, is_blank
+from monobit.base import Props, extend_string
+from monobit.base import HasProps, checked_property, writable_property
+from monobit.base import Coord, Bounds, to_number, NOT_SET
+from monobit.plumbing.scripting import scriptable
+
+from .raster import Raster, turn_method
 from .vector import StrokePath
+from .labels import Codepoint, Char, Tag, to_label
 
 
 ##############################################################################
 # kerning table
 
 class KernTable(dict):
     """char -> int."""
@@ -301,16 +302,16 @@
             overwrite=False, match_whitespace=True, match_graphical=True,
         ):
         """
            Set labels or comment using provided encoder or tagger object.
 
            char_from: Encoder object used to set char labels
            codepoint_from: Encoder object used to set codepoint labels
-           tag_from: Tagger object used to set tag labels
-           comment_from: Tagger object used to set comment
+           tag_from: Encoder object used to set tag labels
+           comment_from: Encoder object used to set comment
            overwrite: overwrite codepoint or char if already given
            match_whitespace: do not give blank glyphs a non-whitespace char label (default: True)
            match_graphical: do not give non-blank glyphs a non-graphical label (default: True)
         """
         if sum(
                 _arg is not NOT_SET
                 for _arg in (codepoint_from, char_from, tag_from, comment_from)
@@ -339,20 +340,20 @@
                 if match_graphical and not self.is_blank() and char and not is_graphical(char):
                     return self
                 return self.modify(char=char)
         if tag_from is not NOT_SET:
             if not tag_from:
                 if overwrite:
                     return self.modify(tag=None)
-            elif overwrite or not self.tag:
+            elif overwrite or not self.tags:
                 return self.modify(tag=tag_from.tag(*labels))
         if comment_from is not NOT_SET:
             if not comment_from:
                 return self.modify(comment=None)
-            return self.modify(comment=comment_from.comment(*labels))
+            return self.modify(comment=comment_from.tag(*labels).value)
         return self
 
     def append(
             self, *,
             comment=None, **properties
         ):
         """Return a copy of the glyph with changes."""
@@ -528,15 +529,15 @@
         return self._pixels.as_blocks(resolution)
 
     def as_vector(self, ink=1, paper=0):
         """Return flat tuple of user-specified foreground and background objects."""
         return self._pixels.as_vector(ink=ink, paper=paper)
 
     def as_bits(self, ink=1, paper=0):
-        """Return flat bits as bytes string."""
+        """Return flat bits as bytes string. Ink, paper may be of type int or RGB"""
         return self._pixels.as_bits(ink=ink, paper=paper)
 
     def as_byterows(self, *, align='left'):
         """Convert glyph to rows of bytes."""
         return self._pixels.as_byterows(align=align)
 
     def as_bytes(
@@ -561,15 +562,14 @@
 
 
     ##########################################################################
     # glyph transformations
 
     # orthogonal transformations
 
-    @scriptable
     def mirror(
             self, *,
             adjust_metrics:bool=True, create_vertical_metrics:bool=False,
         ):
         """
         Reverse pixels horizontally.
 
@@ -586,15 +586,14 @@
             if create_vertical_metrics or self.has_vertical_metrics():
                 new_metrics |= dict(
                     shift_left=-self.shift_left
                     #shift_left around central axis, so should differ at most 1 pixel
                 )
         return self.modify(pixels, **new_metrics)
 
-    @scriptable
     def flip(
             self, *,
             adjust_metrics:bool=True, create_vertical_metrics:bool=False,
         ):
         """
         Reverse pixels vertically.
 
@@ -613,15 +612,14 @@
                 new_metrics |= dict(
                     top_bearing=self.bottom_bearing,
                     bottom_bearing=self.top_bearing,
                 )
         # Font should adjust ascent <-> descent and global bearings
         return self.modify(pixels, **new_metrics)
 
-    @scriptable
     def transpose(self, *, adjust_metrics:bool=True):
         """
         Transpose glyph.
 
         adjust_metrics: also transpose metrics (default: True)
         """
         pixels = self._pixels.transpose()
@@ -638,15 +636,14 @@
         return self.modify(pixels)
 
 
     turn = scriptable(turn_method)
 
     # raster resizing
 
-    @scriptable
     def crop(
             self, left:int=0, bottom:int=0, right:int=0, top:int=0,
             *, adjust_metrics:bool=True, create_vertical_metrics:bool=False,
         ):
         """
         Crop the raster.
 
@@ -676,15 +673,14 @@
                 new_metrics |= dict(
                     top_bearing=self.top_bearing + top,
                     bottom_bearing=self.bottom_bearing + bottom,
                     shift_left=self.shift_left + sign*((sign*(right-left))//2),
                 )
         return self.modify(pixels, **new_metrics)
 
-    @scriptable
     def expand(
             self, left:int=0, bottom:int=0, right:int=0, top:int=0,
             *, adjust_metrics:bool=True, create_vertical_metrics:bool=False,
         ):
         """
         Add blank space to raster.
 
@@ -715,15 +711,14 @@
                     top_bearing=self.top_bearing - top,
                     bottom_bearing=self.bottom_bearing - bottom,
                     # for shift-left, expand left is like crop right, and v.v.
                     shift_left=self.shift_left + sign*((sign*(left-right))//2),
                 )
         return self.modify(pixels, **new_metrics)
 
-    @scriptable
     def reduce(
             self, *,
             adjust_metrics:bool=True, create_vertical_metrics:bool=False,
         ):
         """
         Return a glyph reduced to the bounding box.
 
@@ -735,15 +730,14 @@
             *self.padding, adjust_metrics=adjust_metrics,
             create_vertical_metrics=create_vertical_metrics,
         )
 
 
     # scaling
 
-    @scriptable
     def stretch(
             self, factor_x:int=1, factor_y:int=1,
             *, adjust_metrics:bool=True, create_vertical_metrics:bool=False,
         ):
         """
         Stretch glyph by repeating rows and/or columns.
 
@@ -766,15 +760,14 @@
                 new_metrics |= dict(
                     top_bearing=factor_y*self.top_bearing,
                     bottom_bearing=factor_y*self.bottom_bearing,
                     shift_left=factor_x*self.shift_left,
                 )
         return self.modify(pixels, **new_metrics)
 
-    @scriptable
     def shrink(
             self, factor_x:int=1, factor_y:int=1,
             *, adjust_metrics:bool=True, create_vertical_metrics:bool=False,
         ):
         """
         Shrink by removing rows and/or columns.
 
@@ -799,15 +792,14 @@
                     bottom_bearing=self.bottom_bearing // factor_y,
                     shift_left=self.shift_left // factor_x,
                 )
         return self.modify(pixels, **new_metrics)
 
     # shear
 
-    @scriptable
     def shear(
             self, *, direction:str='right', pitch:Coord=(1, 1),
             create_vertical_metrics:bool=False,
         ):
         """
         Create a slant by dislocating diagonally, keeping
         the horizontal baseline fixed.
@@ -854,15 +846,14 @@
         pixels = work._pixels.shear(
             direction=direction, pitch=pitch, modulo=modulo,
         )
         return work.modify(pixels)
 
     # ink effects
 
-    @scriptable
     def smear(
             self, *, left:int=0, down:int=0, right:int=1, up:int=0,
             adjust_metrics:bool=True, create_vertical_metrics:bool=False,
         ):
         """
         Repeat inked pixels.
 
@@ -881,29 +872,27 @@
             adjust_metrics=adjust_metrics,
             create_vertical_metrics=create_vertical_metrics,
         )
         return work.modify(work._pixels.smear(
             left=left, right=right, up=up, down=down,
         ))
 
-    @scriptable
     def outline(self, *, thickness:int=1, create_vertical_metrics:bool=False):
         """
         Outline glyph.
 
         thickness: number of pixels in outline in each direction
         create_vertical_metrics: create vertical metrics if they don't exist (default: False)
         """
         thicker = self.smear(
             left=thickness, down=thickness, right=thickness, up=thickness,
             create_vertical_metrics=create_vertical_metrics,
         )
         return thicker.overlay(self, operator=lambda x: bool(sum(x) % 2))
 
-    @scriptable
     def underline(self, descent:int=1, thickness:int=1):
         """
         Add a line.
 
         descent: number of pixels the underline is below the baseline (default: 1)
         thickness: number of pixels the underline extends downward (default: 1)
         """
@@ -913,20 +902,18 @@
         # extend up if we get above the ratser height
         up = max(0, height-self.height+1)
         work = self.expand(bottom=down, top=up)
         top_height = height+down
         bottom_height = top_height-thickness+1
         return work.modify(work._pixels.underline(top_height, bottom_height))
 
-    @scriptable
     def invert(self):
         """Reverse video."""
         return self.modify(self._pixels.invert())
 
-    @scriptable
     def roll(self, down:int=0, right:int=0):
         """
         Cycle rows and/or columns in raster.
 
         down: number of rows to roll (down if positive, up if negative)
         right: number of columns to roll (to right if positive, to left if negative)
         """
```

### Comparing `monobit-0.42.2/monobit/glyphmap.py` & `monobit-0.43.0/monobit/render/glyphmap.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
-monobit.glyphmap - glyph maps
+monobit.render.glyphmap - glyph maps
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 try:
     from PIL import Image
 except ImportError:
     Image = None
 
-from .properties import Props
-from .raster import Raster
-from .blocks import  blockstr
+from ..base import Props
+from ..base.blocks import blockstr
+from ..core import Raster
 
 
 class GlyphMap:
 
     def __init__(self, map=()):
         self._map = list(map)
         self._turns = 0
@@ -71,28 +71,42 @@
             if entry.sheet == sheet:
                 canvas.blit(
                     entry.glyph, entry.x - min_x, entry.y - min_y, operator=max
                 )
         return canvas.stretch(self._scale_x, self._scale_y).turn(self._turns)
 
     def to_images(
-            self, *, paper, ink, border, invert_y=False,
-            transparent=True
+            self, *, paper=0, ink=255, border=0, invert_y=False,
+            transparent=True,
         ):
-        """Draw images based on shhets in glyph map."""
+        """Draw images based on sheets in glyph map."""
         if not Image:
             raise ImportError('Rendering to image requires PIL module.')
-        paper, ink, border = 0, 255, 32
+        if not(type(paper) == type(ink) == type(border)):
+            raise TypeError(
+                'paper, ink and border must be of the same type; '
+                f'got {type(paper)}, {type(ink)}, {type(border)}'
+            )
+        if isinstance(paper, int):
+            image_mode = 'L'
+        elif isinstance(paper, tuple) and len(paper) == 3:
+            image_mode = 'RGB'
+        else:
+            raise TypeError('paper, ink and border must be either int or RGB tuple')
         last, min_x, min_y, max_x, max_y = self.get_bounds()
         # no +1 as bounds are inclusive
         width, height = max_x - min_x, max_y - min_y
-        images = [Image.new('L', (width, height), border) for _ in range(last+1)]
+        images = [Image.new(image_mode, (width, height), border) for _ in range(last+1)]
         for entry in self._map:
-            charimg = Image.new('L', (entry.glyph.width, entry.glyph.height))
+            charimg = Image.new(image_mode, (entry.glyph.width, entry.glyph.height))
             data = entry.glyph.as_bits(ink, paper)
+            if image_mode == 'RGB':
+                # itertools grouper idiom, split in groups of 3 bytes
+                iterators = [iter(data)] * 3
+                data = tuple(zip(*iterators, strict=True))
             charimg.putdata(data)
             if invert_y:
                 target = (entry.x, entry.y)
             else:
                 # Image has ttb y coords, we have btt
                 # our character origin is bottom left
                 target = (entry.x-min_x, height-entry.glyph.height+min_y-entry.y)
@@ -106,15 +120,15 @@
                 .rotate(-90 * self._turns, expand=True)
             for _im in images
         )
         return images
 
     def as_image(
             self, *,
-            ink=(255, 255, 255), paper=(0, 0, 0), border=(0, 0, 0),
+            ink=255, paper=0, border=0,
             sheet=0,
         ):
         """Convert glyph map to image."""
         images = self.to_images(ink=ink, paper=paper, border=border)
         return images[sheet]
 
     def as_text(
```

### Comparing `monobit-0.42.2/monobit/labels.py` & `monobit-0.43.0/monobit/core/labels.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
-monobit.label - yaff representation of labels
+monobit.core.label - representation of labels
 
 (c) 2020--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 from string import ascii_letters, digits
 from unicodedata import normalize
 from itertools import count
 
-from .binary import ceildiv, int_to_bytes, bytes_to_int
-from .scripting import to_int
-from .basetypes import CONVERTERS
+from monobit.base.binary import ceildiv, int_to_bytes, bytes_to_int
+from monobit.base import to_int
+from monobit.base import CONVERTERS
+from monobit.encoding.unicode import is_printable
 
 
 def is_enclosed(from_str, char):
     """Check if a char occurs on both sides of a string."""
     return len(from_str) >= 2 and from_str[0] == char and from_str[-1] == char
 
 def strip_matching(from_str, char, allow_no_match=True):
@@ -120,18 +121,17 @@
 
     def __repr__(self):
         """Represent label."""
         return f"{type(self).__name__}({super().__repr__()})"
 
     def __str__(self):
         """Convert to unicode label str for yaff."""
-        return ', '.join(
-            f'u+{ord(_uc):04x}'
-            for _uc in self
-        )
+        if all(is_printable(_uc) for _uc in self):
+            return f"'{super().__str__()}'"
+        return ', '.join(f'u+{ord(_uc):04x}' for _uc in self)
 
     @property
     def value(self):
         """Get our str contents without calling __str__."""
         return ''.join(self)
 
 
@@ -166,15 +166,15 @@
         return super().__new__(cls, value)
 
     def __repr__(self):
         """Represent label."""
         return f"{type(self).__name__}({super().__repr__()})"
 
     def __str__(self):
-        """Convert codepoint label to str."""
+        """Convert codepoint label to str for yaff."""
         return '0x' + self.hex()
 
     def __lt__(self, other):
         """Order like ints."""
         return other and (not self or int(self) < int(Codepoint(other)))
 
     def __gt__(self, other):
@@ -215,33 +215,23 @@
             value = ''
         if not isinstance(value, str):
             raise ValueError(
                 f'Cannot convert value {repr(value)} of type {type(value)} to tag.'
             )
         self._value = value
 
-
     def __repr__(self):
         """Represent label."""
         return f"{type(self).__name__}({repr(self._value)})"
 
     def __str__(self):
-        """Convert tag to str."""
-        # quote otherwise ambiguous/illegal tags
+        """Convert tag to str for yaff."""
         # in particular, we need to quote 0x u+ ' ", non-ascii, and single chars
-        if (
-                len(self._value) < 2
-                or not (self._value[0] in ascii_letters)
-                or any(
-                    _c not in ascii_letters + digits + '_-.'
-                    for _c in self._value
-                )
-            ):
-            return f'"{self._value}"'
-        return self._value
+        # but we quote all as unquoted tags are deprecated
+        return f'"{self._value}"'
 
     def __hash__(self):
         """Allow use as dictionary key."""
         # make sure tag and Char don't collide
         return hash((type(self), self._value))
 
     def __eq__(self, other):
```

### Comparing `monobit-0.42.2/monobit/magic.py` & `monobit-0.43.0/monobit/storage/magic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-monobit.magic - file type recognition
+monobit.storage.magic - file type recognition
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from pathlib import Path
```

### Comparing `monobit-0.42.2/monobit/pack.py` & `monobit-0.43.0/monobit/core/pack.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
-monobit.pack - collection of fonts
+monobit.core.pack - collection of fonts
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 
+from monobit.plumbing.scripting import scriptable
 from .font import Font, FontProperties
-from .scripting import scriptable, get_scriptables
 
 
 class Pack:
     """Holds one or more potentially unrelated fonts."""
 
     def __init__(self, fonts=()):
         """Create pack from sequence of fonts."""
@@ -64,11 +64,7 @@
         """List property of fonts in collection."""
         return tuple(getattr(_font, property) for _font in self._fonts)
 
     def itergroups(self, property):
         """Iterate over subpacks with one value for a property."""
         for value in sorted(set(self.list_by(property))):
             yield value, self.select(**{property: value})
-
-
-# scriptable font/glyph operations
-operations = get_scriptables(Pack)
```

### Comparing `monobit-0.42.2/monobit/properties.py` & `monobit-0.43.0/monobit/base/properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-monobit.properties - property structures
+monobit.base.properties - property structures
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 
 import logging
```

### Comparing `monobit-0.42.2/monobit/raster.py` & `monobit-0.43.0/monobit/core/raster.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 """
-monobit.raster - bitmap raster
+monobit.core.raster - bitmap raster
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from itertools import zip_longest
 
-from .binary import ceildiv, reverse_by_group, bytes_to_bits
-from .basetypes import Bounds, Coord
-from .blocks import matrix_to_blocks, blockstr
-
-
-# sentinel object
-NOT_SET = object()
+from monobit.base.binary import ceildiv, reverse_by_group, bytes_to_bits
+from monobit.base import Bounds, Coord, NOT_SET
+from monobit.base.blocks import matrix_to_blocks, blockstr
 
 
 # turn function for Raster, Glyph and Font
 
 def _calc_turns(clockwise, anti):
     if clockwise is NOT_SET:
         if anti is NOT_SET:
@@ -230,21 +226,23 @@
         return tuple(
             ink if _c == self._1 else paper
             for _c in ''.join(self._pixels)
         )
 
     def as_bits(self, ink=1, paper=0):
         """Return flat bits as bytes string."""
+        if isinstance(ink, int) and isinstance(paper, int):
+            ink = (ink,)
+            paper = (paper,)
         return (
             ''.join(self._pixels).encode('latin-1')
-            .replace(self._1.encode('latin-1'), bytes((ink,)))
-            .replace(self._0.encode('latin-1'), bytes((paper,)))
+            .replace(self._1.encode('latin-1'), bytes(ink))
+            .replace(self._0.encode('latin-1'), bytes(paper))
         )
 
-
     @classmethod
     def from_bytes(
             cls, byteseq, width=NOT_SET, height=NOT_SET,
             *, align='left', order='row-major', stride=NOT_SET,
             byte_swap=0, bit_order='big',
             **kwargs
         ):
```

### Comparing `monobit-0.42.2/monobit/renderer.py` & `monobit-0.43.0/monobit/render/renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-monobit.renderer - render text to bitmaps using font
+monobit.render.renderer - render text to bitmaps using font
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from unicodedata import bidirectional, normalize, category
@@ -33,19 +33,19 @@
         'Module `uniseg` not found. Grapheme clusters may not render correctly.'
     )
     def grapheme_clusters(text):
         """Use NFC as poor-man's grapheme cluster. This works... sometimes."""
         for c in normalize('NFC', text):
             yield c
 
-from .binary import ceildiv
-from .labels import Char, Codepoint
-from .raster import Raster
-from .properties import Props
-from .glyph import Glyph
+from ..base.binary import ceildiv
+from ..base import Props
+from ..core import Char, Codepoint
+from ..core import Raster
+from ..core import Glyph
 from .glyphmap import GlyphMap
 
 
 DIRECTIONS = {
     'n': 'normal',
     'l': 'left-to-right',
     'r': 'right-to-left',
@@ -323,27 +323,25 @@
         tuple(_iter_labels(font, _line, missing))
         for _line in lines
     )
 
 def _iter_labels(font, text, missing='raise'):
     """Iterate over labels in text, yielding glyphs. text may be str or bytes."""
     if isinstance(text, str):
-        font = font.label()
         # split text into standard grapheme clusters
         text = tuple(grapheme_clusters(text))
         # find the longest *number of standard grapheme clusters* per label
         # this will often be 1, except when the font has defined e.g. Zł or Ft
         # as a char label for a single glyph
         labelset = font.get_chars()
         max_length = max((len(tuple(grapheme_clusters(_c))) for _c in labelset), default=0)
         # we need to combine multiple elements back into str to match a glyph
         def labeltype(seq):
             return Char(''.join(seq))
     else:
-        font = font.label(codepoint_from=font.encoding)
         labelset = font.get_codepoints()
         labeltype = Codepoint
         max_length = max((len(_c) for _c in labelset), default=0)
     remaining = text
     while remaining:
         # try multibyte/multi-grapheme cluster clusters first
         for try_len in range(max_length, 1, -1):
```

### Comparing `monobit-0.42.2/monobit/storage.py` & `monobit-0.43.0/monobit/storage/converters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """
-monobit.storage - load and save fonts
+monobit.storage.converters - load and save fonts
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import os
 import sys
 import logging
 import shlex
 from pathlib import Path
 from contextlib import contextmanager
 
-from .constants import VERSION, CONVERTER_NAME
-from .font import Font
-from .pack import Pack
+from ..constants import VERSION, CONVERTER_NAME
+from ..core import Font, Pack
+from ..base.struct import StructError
+from ..plumbing import scriptable, ARG_PREFIX, convert_arguments, check_arguments
+from ..base import Any
 from .streams import Stream, StreamBase, KeepOpen, DirectoryStream
 from .magic import MagicRegistry, FileFormatError, maybe_text
-from .struct import StructError
-from .scripting import scriptable, ScriptArgs, ARG_PREFIX
-from .basetypes import Any
 
 
 DEFAULT_TEXT_FORMAT = 'yaff'
 DEFAULT_BINARY_FORMAT = 'raw'
 
 
 @contextmanager
@@ -262,32 +261,30 @@
 # loader/saver registry
 
 class ConverterRegistry(MagicRegistry):
     """Loader/Saver registry."""
 
     def register(
             self, name='', magic=(), patterns=(),
-            linked=None, **kwargs
+            linked=None, wrapper=False,
         ):
         """
         Decorator to register font loader/saver.
 
         name: unique name of the format
         magic: magic sequences for this format (no effect for savers)
         patterns: filename patterns for this format
         linked: loader/saver linked to saver/loader
         """
         register_magic = super().register
 
         def _decorator(original_func):
-            _func = scriptable(
-                original_func,
-                record=False,
-                **kwargs
-            )
+            _func = convert_arguments(original_func)
+            if not wrapper:
+                _func = check_arguments(_func)
             # register converter
             if linked:
                 format = name or linked.format
                 _func.magic = magic or linked.magic
                 _func.patterns = patterns or linked.patterns
             else:
                 format = name
```

### Comparing `monobit-0.42.2/monobit/streams.py` & `monobit-0.43.0/monobit/storage/streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-monobit.streams - file stream tools
+monobit.storage.streams - file stream tools
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import io
 import os
```

### Comparing `monobit-0.42.2/monobit/struct.py` & `monobit-0.43.0/monobit/base/struct.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-monobit.struct - binary structures
+monobit.base.struct - binary structures
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import ctypes
```

### Comparing `monobit-0.42.2/monobit/taggers.py` & `monobit-0.43.0/monobit/encoding/taggers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,189 +1,232 @@
 """
-monobit.taggers - glyph tagging
+monobit.encoding.taggers - glyph tagging
 
 (c) 2020--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import unicodedata
-import pkgutil
 from pathlib import Path
+from importlib.resources import files
+from functools import partial, wraps, cached_property
 
-from .encoding import unicode_name, is_printable, NotFoundError
-from .labels import to_label, Tag
-from .properties import reverse_dict
+from .unicode import unicode_name, is_printable
+from ..core.labels import to_label, Tag, Char, Codepoint
+from ..base import reverse_dict
+from .base import NotFoundError, Encoder, register_reader
+from . import tables
 
 
-class Tagger:
-    """Add tags or comments to a font's glyphs."""
-
-    name = 'unknown-tagger'
-
-    def comment(self, *labels):
-        raise NotImplementedError
+def _get_label(labels, labeltype):
+    """Get first label of given type from list."""
+    for label in labels:
+        label = to_label(label)
+        if isinstance(label, labeltype):
+            return label
+    return labeltype()
 
-    def tag(self, *labels):
-        return Tag(self.comment(*labels))
+_get_char = partial(_get_label, labeltype=Char)
+_get_codepoint = partial(_get_label, labeltype=Codepoint)
+_get_tag = partial(_get_label, labeltype=Tag)
 
-    def __repr__(self):
-        """Representation."""
-        return f"{type(self).__name__}(name='{self.name}')"
 
-    def __str__(self):
-        """Yaff representation."""
-        return self.name
+class UnicodeNameTagger(Encoder):
+    """Tag with unicode name."""
 
+    def __init__(self):
+        super().__init__(name='name')
 
-def _get_char(labels):
-    """Get first char label from list."""
-    for label in labels:
-        char = to_label(label)
-        if isinstance(char, str):
-            return char
-    return ''
+    def tag(self, *labels):
+        """Get unicode glyph name."""
+        char = _get_char(labels)
+        if not char:
+            return Tag()
+        return Tag(unicode_name(char.value))
 
-def _get_codepoint(labels):
-    """Get first codepoint label from list."""
-    for label in labels:
-        cp = to_label(label)
-        if isinstance(cp, bytes):
-            return cp
-    return b''
+    def char(self, *labels):
+        """Get char from unicode glyph name."""
+        tag = _get_tag(labels)
+        elements = tag.value.split(',')
+        try:
+            return Char(''.join(
+                unicodedata.lookup(elem.strip())
+                for elem in elements
+            ))
+        except KeyError:
+            return Char()
 
 
-class UnicodeTagger(Tagger):
+class DescriptionTagger(Encoder):
     """Tag with unicode names and characters."""
 
-    def __init__(self, include_char=False):
-        self.include_char = include_char
-        if include_char:
-            self.name = 'desc'
-        else:
-            self.name = 'name'
+    def __init__(self):
+        super().__init__(name='desc')
 
-    def comment(self, *labels):
+    def tag(self, *labels):
         """Get unicode glyph name."""
         char = _get_char(labels)
         if not char:
-            return ''
+            return Tag()
         char = char.value
         name = unicode_name(char)
-        if self.include_char and is_printable(char):
-            return '[{}] {}'.format(char, name)
-        return '{}'.format(name)
+        if is_printable(char):
+            return Tag('[{}] {}'.format(char, name))
+        return Tag(name)
 
 
-class CharTagger(Tagger):
+class CharTagger(Encoder):
     """Tag with unicode characters."""
 
-    name = 'char'
+    def __init__(self):
+        super().__init__(name='char')
 
-    def comment(self, *labels):
+    def tag(self, *labels):
         """Get printable char."""
         char = _get_char(labels).value
         if is_printable(char):
-            return char
-        return ''
+            return Tag(char)
+        return Tag()
 
 
-class CodepointTagger(Tagger):
-    """Tag with codepoint numbers."""
+class FallbackTagger(Encoder):
+    """Algorithmically generate tags."""
+
+    def __init__(self, unmapped='glyph{count:04}'):
+        """Set up mapping."""
+        super().__init__(name='fallback')
+        self._pattern = unmapped
+        self._count = -1
+
+    def tag(self, *labels):
+        """Get value from tagmap."""
+        self._count += 1
+        return Tag(self._pattern.format(
+            count=self._count,
+            char=_get_char(labels),
+            codepoint=_get_codepoint(labels),
+            tag=_get_tag(labels),
+        ))
 
-    name = 'codepoint'
+
+class CodepointTagger(Encoder):
+    """Tag with codepoint numbers."""
 
     def __init__(self, prefix=''):
         """Create codepoint tagger with prefix"""
+        super().__init__(name='codepoint')
         self._prefix = prefix
 
-    def comment(self, *labels):
+    def tag(self, *labels):
         """Get codepoint string."""
         cp = _get_codepoint(labels)
         if not cp:
-            return ''
-        return f'{self._prefix}{cp}'
+            return Tag()
+        return Tag(f'{self._prefix}{cp}')
 
 
-class MappingTagger(Tagger):
+class Tagmap(Encoder):
     """Tag on the basis of a mapping table."""
 
-    def __init__(self, mapping, name=''):
+    def __init__(self, mapping, name='', fallback=None):
         """Set up mapping."""
+        super().__init__(name=name)
         self._chr2tag = mapping
-        self._tag2chr = reverse_dict(mapping)
-        self.name = name
+        self._fallback = fallback or FallbackTagger()
 
-    @classmethod
-    def load(cls, filename, *, name='', **kwargs):
-        """Create new charmap from file."""
-        try:
-            data = pkgutil.get_data(__name__, filename)
-        except EnvironmentError as exc:
-            raise NotFoundError(f'Could not load tagmap file `{filename}`: {exc}')
-        if not data:
-            raise NotFoundError(f'No data in tagmap file `{filename}`.')
-        mapping = _read_tagmap(data, **kwargs)
-        if not name:
-            name = Path(filename).stem
-        return cls(mapping, name=name)
+    @cached_property
+    def _tag2chr(self):
+        return reverse_dict(self._chr2tag)
 
-    def comment(self, *labels):
+    def tag(self, *labels):
         """Get value from tagmap."""
         char = _get_char(labels)
         try:
-            return self._chr2tag[char]
+            return Tag(self._chr2tag[char])
         except KeyError:
-            return self.get_default_tag(char)
-
-    def get_default_tag(self, char):
-        """Construct a default tag for unmapped glyphs."""
-        return ''
+            return self._fallback.tag(*labels)
 
     def char(self, *labels):
         """Get char value from tagmap."""
         for label in labels:
             if isinstance(label, Tag):
                 try:
-                    return self._tag2chr[label.value]
+                    return Char(self._tag2chr[label.value])
                 except KeyError:
                     pass
-        return ''
+        return Char()
 
+    @property
+    def mapping(self):
+        return {**self._chr2tag}
+
+    def __or__(self, other):
+        """Return encoding overlaid with all characters defined in right-hand side."""
+        return Tagmap(mapping=self._chr2tag | other._chr2tag, name=f'{self.name}')
+
+    def table(self):
+        """Mapping table"""
+        return '\n'.join(
+            f'u+{ord(_k):04X}: "{_v}"' for _k, _v in self._chr2tag.items()
+        )
 
-class AdobeTagger(MappingTagger):
+class AdobeFallbackTagger(Encoder):
+    """Fallback tagger following AGL conventions."""
 
-    name = 'adobe'
+    def __init__(self):
+        super().__init__(name='adobe-fallback')
 
-    def get_default_tag(self, char):
+    def tag(self, *labels):
         """Construct a default tag for unmapped glyphs."""
-        if not char:
-            return ''
-        cps = [ord(_c) for _c in char]
+        char = _get_char(labels)
         # following agl recommendation for naming sequences
-        return '_'.join(f'uni{_cp:04X}' if _cp < 0x10000 else f'u{_cp:06X}' for _cp in cps)
+        cps = (ord(_c) for _c in char)
+        return Tag('_'.join(
+            f'uni{_cp:04X}' if _cp < 0x10000 else f'u{_cp:06X}'
+            for _cp in cps
+        ))
 
 
-class SGMLTagger(MappingTagger):
+class SGMLFallbackTagger(Encoder):
+    """Fallback tagger following SGML conventions."""
 
-    name = 'sgml'
+    def __init__(self):
+        super().__init__(name='sgml-fallback')
 
-    def get_default_tag(self, char):
+    def tag(self, *labels):
         """Construct a default tag for unmapped glyphs."""
-        if not char:
-            return ''
-        cps = [ord(_c) for _c in char]
+        char = _get_char(labels)
+        cps = (ord(_c) for _c in char)
         # joining numeric references by semicolons
         # note that each entity should really start with & and end with ; e.g. &eacute;
-        return ';'.join(f'#{_cp:X}' for _cp in cps)
-
+        return Tag(';'.join(f'#{_cp:X}' for _cp in cps))
 
 
 ###################################################################################################
 # tag map format readers
 
+def _tagmap_loader(fn):
+    """Decorator for the shared parts of tagmap loaders."""
+
+    @wraps(fn)
+    def _load(name, path, *args, fallback, **kwargs):
+        try:
+            data = path.read_bytes()
+        except EnvironmentError as exc:
+            raise NotFoundError(f'Could not load tagmap file `{str(path)}`: {exc}')
+        if not data:
+            raise NotFoundError(f'No data in tagmap file `{str(path)}`')
+        mapping = fn(data, *args, **kwargs)
+        return Tagmap(mapping, name=name, fallback=fallback)
+
+    return _load
+
+
+@register_reader('tagmap')
+@_tagmap_loader
 def _read_tagmap(data, separator=':', comment='#', joiner=',', tag_column=0, unicode_column=1):
     """Read a tag map from file data."""
     chr2tag = {}
     for line in data.decode('utf-8').splitlines():
         if line.startswith(comment):
             continue
         columns = line.split(separator)
@@ -193,39 +236,7 @@
             try:
                 char = ''.join(chr(int(_str, 16)) for _str in unicode_str.split(joiner))
             except ValueError:
                 pass
             else:
                 chr2tag[char] = tag
     return chr2tag
-
-
-###################################################################################################
-
-# for use in function annotations
-def tagger(initialiser):
-    """Retrieve or create a tagmap from object or string."""
-    if isinstance(initialiser, Tagger):
-        return initialiser
-    if initialiser is None or not str(initialiser):
-        return None
-    initialiser = str(initialiser)
-    try:
-        return tagmaps[initialiser]
-    except KeyError:
-        pass
-    return MappingTagger.load(initialiser)
-
-
-tagmaps = {
-    'char': CharTagger(),
-    'codepoint': CodepointTagger(),
-    'name': UnicodeTagger(),
-    'desc': UnicodeTagger(include_char=True),
-    'adobe': AdobeTagger.load('charmaps/agl/aglfn.txt', name='adobe', separator=';', unicode_column=0, tag_column=1),
-    'truetype': AdobeTagger.load('charmaps/agl/aglfn.txt', name='truetype', separator=';', unicode_column=0, tag_column=1),
-    'sgml': SGMLTagger.load('charmaps/misc/SGML.TXT', name='sgml', separator='\t', unicode_column=2),
-}
-
-# truetype mapping is adobe mapping *but* with .null for NUL
-# https://developer.apple.com/fonts/TrueType-Reference-Manual/RM06/Chap6post.html
-tagmaps['truetype']._chr2tag['\0'] = '.null'
```

### Comparing `monobit-0.42.2/monobit/vector.py` & `monobit-0.43.0/monobit/core/vector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
-monobit.vector - stroke font support
+monobit.core.vector - single-stroke vector font support
 
 (c) 2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from collections import deque
 from functools import cached_property
 from itertools import accumulate
 from typing import NamedTuple
 
-from .basetypes import Coord, Bounds
+from monobit.base import Coord, Bounds
+
 from .raster import Raster
 
 
 class StrokeMove(NamedTuple):
     """Stroke path element."""
     command: str
     dx: int
```

### Comparing `monobit-0.42.2/monobit/charmaps/adobe/ReadMe.txt` & `monobit-0.43.0/monobit/encoding/tables/adobe/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/adobe/stdenc.txt` & `monobit-0.43.0/monobit/encoding/tables/adobe/stdenc.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/adobe/symbol.txt` & `monobit-0.43.0/monobit/encoding/tables/adobe/symbol.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/adobe/zdingbat.txt` & `monobit-0.43.0/monobit/encoding/tables/adobe/zdingbat.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/agl/LICENSE.md` & `monobit-0.43.0/monobit/encoding/tables/agl/LICENSE.md`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/agl/README.md` & `monobit-0.43.0/monobit/encoding/tables/agl/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/agl/aglfn.txt` & `monobit-0.43.0/monobit/encoding/tables/agl/aglfn.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/agl/glyphlist.txt` & `monobit-0.43.0/monobit/encoding/tables/agl/glyphlist.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/ARABIC.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/ARABIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/CELTIC.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/CELTIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/CENTEURO.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/CENTEURO.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/CHINSIMP.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/CHINSIMP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/CHINTRAD.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/CHINTRAD.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/CORPCHAR.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/CORPCHAR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/CROATIAN.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/CROATIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/CYRILLIC.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/CYRILLIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/DEVANAGA.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/DEVANAGA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/DINGBATS.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/DINGBATS.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/FARSI.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/FARSI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/GAELIC.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/GAELIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/GREEK.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/GREEK.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/GUJARATI.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/GUJARATI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/GURMUKHI.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/GURMUKHI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/HEBREW.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/HEBREW.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/ICELAND.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/ICELAND.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/INUIT.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/INUIT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/JAPANESE.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/JAPANESE.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/KEYBOARD.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/KEYBOARD.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/KOREAN.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/KOREAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/ROMAN.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/ROMAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/ROMANIAN.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/ROMANIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/ReadMe.txt` & `monobit-0.43.0/monobit/encoding/tables/apple/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/SYMBOL.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/SYMBOL.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/THAI.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/THAI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/TURKISH.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/TURKISH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/apple/UKRAINE.TXT` & `monobit-0.43.0/monobit/encoding/tables/apple/UKRAINE.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/czyborra/README.md` & `monobit-0.43.0/monobit/encoding/tables/czyborra/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/czyborra/bulgarian-mik.txt` & `monobit-0.43.0/monobit/encoding/tables/czyborra/bulgarian-mik.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/czyborra/cp866.txt` & `monobit-0.43.0/monobit/encoding/tables/czyborra/cp866.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/czyborra/gost19768-87.txt` & `monobit-0.43.0/monobit/encoding/tables/czyborra/gost19768-87.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/czyborra/hp-roman8.txt` & `monobit-0.43.0/monobit/encoding/tables/czyborra/hp-roman8.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/czyborra/koi-0.txt` & `monobit-0.43.0/monobit/encoding/tables/czyborra/koi-0.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/czyborra/koi-7.txt` & `monobit-0.43.0/monobit/encoding/tables/czyborra/koi-7.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/czyborra/koi8-a.txt` & `monobit-0.43.0/monobit/encoding/tables/czyborra/koi8-a.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/czyborra/koi8-b.txt` & `monobit-0.43.0/monobit/encoding/tables/czyborra/koi8-b.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/czyborra/koi8-e.txt` & `monobit-0.43.0/monobit/encoding/tables/czyborra/koi8-e.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/czyborra/koi8-f.txt` & `monobit-0.43.0/monobit/encoding/tables/czyborra/koi8-f.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/czyborra/koi8-r.txt` & `monobit-0.43.0/monobit/encoding/tables/czyborra/koi8-r.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/czyborra/koi8-u.txt` & `monobit-0.43.0/monobit/encoding/tables/czyborra/koi8-u.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/dkuug/iso646-ca` & `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-ca`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/dkuug/iso646-ca2` & `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-ca2`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/dkuug/iso646-cn` & `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-cn`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/dkuug/iso646-cu` & `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-cu`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/dkuug/iso646-de` & `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-de`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/dkuug/iso646-dk` & `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-dk`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/dkuug/iso646-es` & `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-es`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/dkuug/iso646-es2` & `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-es2`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/dkuug/iso646-fr` & `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-fr`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/dkuug/iso646-gb` & `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-gb`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/dkuug/iso646-hu` & `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-hu`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/dkuug/iso646-it` & `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-it`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/dkuug/iso646-jp` & `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-jp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/dkuug/iso646-jp-ocr-b` & `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-jp-ocr-b`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/dkuug/iso646-kr` & `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-kr`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/dkuug/iso646-us` & `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-us`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/dkuug/iso646-yu` & `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-yu`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/dkuug/jis_x0201` & `monobit-0.43.0/monobit/encoding/tables/dkuug/jis_x0201`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/dkuug/x0201-7` & `monobit-0.43.0/monobit/encoding/tables/dkuug/x0201-7`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/emacs/MULE-ethiopic.map` & `monobit-0.43.0/monobit/encoding/tables/emacs/MULE-ethiopic.map`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/emacs/MULE-ipa.map` & `monobit-0.43.0/monobit/encoding/tables/emacs/MULE-ipa.map`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/emacs/MULE-is13194.map` & `monobit-0.43.0/monobit/encoding/tables/emacs/MULE-is13194.map`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/emacs/MULE-lviscii.map` & `monobit-0.43.0/monobit/encoding/tables/emacs/MULE-lviscii.map`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/emacs/MULE-sisheng.map` & `monobit-0.43.0/monobit/encoding/tables/emacs/MULE-sisheng.map`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/emacs/MULE-tibetan.map` & `monobit-0.43.0/monobit/encoding/tables/emacs/MULE-tibetan.map`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/emacs/MULE-uviscii.map` & `monobit-0.43.0/monobit/encoding/tables/emacs/MULE-uviscii.map`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/emacs/README.md` & `monobit-0.43.0/monobit/encoding/tables/emacs/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/evertype/ARMENIAN.TXT` & `monobit-0.43.0/monobit/encoding/tables/evertype/ARMENIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/evertype/GEORGIAN.TXT` & `monobit-0.43.0/monobit/encoding/tables/evertype/GEORGIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/evertype/README.md` & `monobit-0.43.0/monobit/encoding/tables/evertype/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/1116.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/1116.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/1117.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/1117.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/1118.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/1118.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/1119.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/1119.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/1125.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/1125.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/113.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/113.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/1131.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/1131.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30000.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30000.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30001.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30001.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30002.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30002.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30003.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30003.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30004.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30004.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30005.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30005.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30006.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30006.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30007.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30007.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30008.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30008.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30009.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30009.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30010.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30010.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30011.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30011.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30012.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30012.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30013.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30013.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30014.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30014.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30015.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30015.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30016.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30016.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30017.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30017.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30018.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30018.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30019.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30019.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30020.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30020.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30021.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30021.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30022.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30022.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30023.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30023.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30024.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30024.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30025.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30025.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30026.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30026.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30027.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30027.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30028.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30028.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30029.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30029.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30030.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30030.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30031.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30031.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30032.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30032.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30033.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30033.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30034.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30034.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30039.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30039.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/30040.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/30040.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/3012.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/3012.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/3021.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/3021.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/3845.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/3845.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/3846.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/3846.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/3848.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/3848.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/437.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/437.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/57781.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/57781.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/58152.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/58152.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/58210.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/58210.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/58335.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/58335.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/59234.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/59234.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/59829.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/59829.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/60258.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/60258.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/60853.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/60853.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/61282.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/61282.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/62306.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/62306.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/667.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/667.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/668.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/668.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/737.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/737.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/770.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/770.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/771.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/771.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/772.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/772.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/773.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/773.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/774.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/774.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/775.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/775.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/777.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/777.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/778.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/778.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/790.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/790.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/808.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/808.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/848.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/848.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/849.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/849.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/850.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/850.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/851.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/851.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/852.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/852.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/853.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/853.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/855.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/855.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/856.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/856.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/857.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/857.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/858.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/858.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/859.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/859.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/860.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/860.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/861.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/861.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/862.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/862.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/863.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/863.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/864.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/864.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/865.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/865.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/866.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/866.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/867.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/867.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/869.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/869.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/872.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/872.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/895.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/895.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/899.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/899.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/991.ucp` & `monobit-0.43.0/monobit/encoding/tables/freedos/991.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/freedos/README.md` & `monobit-0.43.0/monobit/encoding/tables/freedos/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/iana/Amiga-1251` & `monobit-0.43.0/monobit/encoding/tables/iana/Amiga-1251`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/iana/PTCP154` & `monobit-0.43.0/monobit/encoding/tables/iana/PTCP154`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/ibm-cdra/037B34B0.UPMAP100` & `monobit-0.43.0/monobit/encoding/tables/ibm-cdra/037B34B0.UPMAP100`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/ibm-cdra/038834B0.UPMAP100` & `monobit-0.43.0/monobit/encoding/tables/ibm-cdra/038834B0.UPMAP100`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/ibm-cdra/039E44B0.UPMAP101` & `monobit-0.43.0/monobit/encoding/tables/ibm-cdra/039E44B0.UPMAP101`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/ibm-cdra/039F34B0.UPMAP100` & `monobit-0.43.0/monobit/encoding/tables/ibm-cdra/039F34B0.UPMAP100`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/ibm-cdra/readme.txt` & `monobit-0.43.0/monobit/encoding/tables/ibm-cdra/readme.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/icu/README.md` & `monobit-0.43.0/monobit/encoding/tables/icu/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/icu/aix-KSC5601.1987_0-4.3.6.ucm` & `monobit-0.43.0/monobit/encoding/tables/icu/aix-KSC5601.1987_0-4.3.6.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/icu/cns-11643-1992.ucm` & `monobit-0.43.0/monobit/encoding/tables/icu/cns-11643-1992.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/icu/ibm-1125_P100-1997.ucm` & `monobit-0.43.0/monobit/encoding/tables/icu/ibm-1125_P100-1997.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/icu/ibm-1375_P100-2008.ucm` & `monobit-0.43.0/monobit/encoding/tables/icu/ibm-1375_P100-2008.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/icu/ibm-720_P100-1997.ucm` & `monobit-0.43.0/monobit/encoding/tables/icu/ibm-720_P100-1997.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/icu/ibm-806_P100-1998.ucm` & `monobit-0.43.0/monobit/encoding/tables/icu/ibm-806_P100-1998.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/icu/ibm-851_P100-1995.ucm` & `monobit-0.43.0/monobit/encoding/tables/icu/ibm-851_P100-1995.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/icu/ibm-858_P100-1997.ucm` & `monobit-0.43.0/monobit/encoding/tables/icu/ibm-858_P100-1997.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/icu/ibm-868_P100-1995.ucm` & `monobit-0.43.0/monobit/encoding/tables/icu/ibm-868_P100-1995.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/icu/ibm-932_P120-1999.ucm` & `monobit-0.43.0/monobit/encoding/tables/icu/ibm-932_P120-1999.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/icu/windows-1361-2000.ucm` & `monobit-0.43.0/monobit/encoding/tables/icu/windows-1361-2000.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/icu/windows-936-2000.ucm` & `monobit-0.43.0/monobit/encoding/tables/icu/windows-936-2000.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/iso-8859/8859-1.TXT` & `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/iso-8859/8859-10.TXT` & `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-10.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/iso-8859/8859-11.TXT` & `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-11.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/iso-8859/8859-13.TXT` & `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-13.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/iso-8859/8859-14.TXT` & `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-14.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/iso-8859/8859-15.TXT` & `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-15.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/iso-8859/8859-16.TXT` & `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-16.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/iso-8859/8859-2.TXT` & `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/iso-8859/8859-3.TXT` & `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-3.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/iso-8859/8859-4.TXT` & `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-4.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/iso-8859/8859-5.TXT` & `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-5.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/iso-8859/8859-6.TXT` & `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-6.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/iso-8859/8859-7.TXT` & `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-7.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/iso-8859/8859-8.TXT` & `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-8.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/iso-8859/8859-9.TXT` & `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-9.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/iso-8859/ReadMe.txt` & `monobit-0.43.0/monobit/encoding/tables/iso-8859/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/ADAMOS7.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ADAMOS7.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/ADAMSWTR.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ADAMSWTR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/AMSCPC.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/AMSCPC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/AMSCPM.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/AMSCPM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/APL2ALT1.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/APL2ALT1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/APL2ALT2.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/APL2ALT2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/APL2ICHG.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/APL2ICHG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/APL2PRIM.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/APL2PRIM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/ATARI8IG.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ATARI8IG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/ATARI8II.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ATARI8II.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/ATARI8VG.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ATARI8VG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/ATARI8VI.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ATARI8VI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/ATARISTI.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ATARISTI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/ATARISTV.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ATARISTV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/C64IALT.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/C64IALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/C64IPRI.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/C64IPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/C64VALT.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/C64VALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/C64VPRI.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/C64VPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/COCOICHG.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/COCOICHG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/COCOSGR4.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/COCOSGR4.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/COCOSGR6.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/COCOSGR6.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/CPETIALT.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/CPETIALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/CPETIPRI.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/CPETIPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/CPETVALT.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/CPETVALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/CPETVPRI.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/CPETVPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/CVICIALT.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/CVICIALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/CVICIPRI.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/CVICIPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/CVICVALT.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/CVICVALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/CVICVPRI.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/CVICVPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/IBMPCICH.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/IBMPCICH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/IBMPCVID.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/IBMPCVID.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/MINITLG0.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/MINITLG0.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/MINITLG1.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/MINITLG1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/MSX.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/MSX.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/ORICG0.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ORICG0.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/ORICG1.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ORICG1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/RISCEFF.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/RISCEFF.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/RISCOSB.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/RISCOSB.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/RISCOSI.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/RISCOSI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/RISCOSV.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/RISCOSV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/ReadMe.txt` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/SINCLRQL.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/SINCLRQL.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/TELTXTG0.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TELTXTG0.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/TELTXTG1.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TELTXTG1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/TELTXTG2.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TELTXTG2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/TELTXTG3.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TELTXTG3.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/TI994A.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TI994A.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM1ICH.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM1ICH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM1ORG.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM1ORG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM1REV.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM1REV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM3IIN.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM3IIN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM3IJP.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM3IJP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM3IRV.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM3IRV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM3VIN.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM3VIN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM3VJP.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM3VJP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM3VRV.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM3VRV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM4AIA.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM4AIA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM4AIP.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM4AIP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM4AIR.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM4AIR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM4AVA.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM4AVA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM4AVP.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM4AVP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/TRSM4AVR.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM4AVR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/ZX80.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZX80.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/ZX81.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZX81.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/ZXDESKTP.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXDESKTP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/ZXFZXKOI.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXFZXKOI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/ZXFZXLT1.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXFZXLT1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/ZXFZXLT5.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXFZXLT5.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/ZXFZXPUA.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXFZXPUA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/ZXFZXSLT.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXFZXSLT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/kreativekorp/ZXSPCTRM.TXT` & `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXSPCTRM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/manual/dec-vt100.ucp` & `monobit-0.43.0/monobit/encoding/tables/manual/dec-vt100.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/manual/hp48.txt` & `monobit-0.43.0/monobit/encoding/tables/manual/hp48.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/manual/ibm897graph.ucp` & `monobit-0.43.0/monobit/encoding/tables/manual/ibm897graph.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/manual/iso2047.txt` & `monobit-0.43.0/monobit/encoding/tables/manual/iso2047.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/manual/mac-system.ucp` & `monobit-0.43.0/monobit/encoding/tables/manual/mac-system.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/manual/russup3.ucp` & `monobit-0.43.0/monobit/encoding/tables/manual/russup3.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/manual/russup4ac.ucp` & `monobit-0.43.0/monobit/encoding/tables/manual/russup4ac.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/manual/russup4na.ucp` & `monobit-0.43.0/monobit/encoding/tables/manual/russup4na.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/manual/windows-1.0.txt` & `monobit-0.43.0/monobit/encoding/tables/manual/windows-1.0.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/manual/windows-2.0.txt` & `monobit-0.43.0/monobit/encoding/tables/manual/windows-2.0.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/manual/windows-3.1.txt` & `monobit-0.43.0/monobit/encoding/tables/manual/windows-3.1.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/EBCDIC/CP037.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/EBCDIC/CP037.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/EBCDIC/CP1026.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/EBCDIC/CP1026.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/EBCDIC/CP500.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/EBCDIC/CP500.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/EBCDIC/CP875.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/EBCDIC/CP875.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/MAC/CYRILLIC.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/MAC/CYRILLIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/MAC/GREEK.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/MAC/GREEK.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/MAC/ICELAND.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/MAC/ICELAND.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/MAC/LATIN2.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/MAC/LATIN2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/MAC/ROMAN.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/MAC/ROMAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/MAC/TURKISH.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/MAC/TURKISH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/PC/CP437.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP437.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/PC/CP737.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP737.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/PC/CP775.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP775.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/PC/CP850.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP850.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/PC/CP852.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP852.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/PC/CP855.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP855.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/PC/CP857.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP857.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/PC/CP860.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP860.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/PC/CP861.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP861.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/PC/CP862.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP862.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/PC/CP863.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP863.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/PC/CP864.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP864.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/PC/CP865.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP865.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/PC/CP866.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP866.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/PC/CP869.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP869.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/PC/CP874.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP874.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP1250.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1250.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP1251.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1251.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP1252.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1252.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP1253.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1253.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP1254.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1254.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP1255.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1255.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP1256.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1256.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP1257.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1257.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP1258.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1258.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP874.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP874.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP932.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP932.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP936.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP936.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP949.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP949.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/microsoft/WINDOWS/CP950.TXT` & `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP950.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/misc/APL-ISO-IR-68.TXT` & `monobit-0.43.0/monobit/encoding/tables/misc/APL-ISO-IR-68.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/misc/ATARIST.TXT` & `monobit-0.43.0/monobit/encoding/tables/misc/ATARIST.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/misc/CP1006.TXT` & `monobit-0.43.0/monobit/encoding/tables/misc/CP1006.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/misc/CP424.TXT` & `monobit-0.43.0/monobit/encoding/tables/misc/CP424.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/misc/CP856.TXT` & `monobit-0.43.0/monobit/encoding/tables/misc/CP856.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/misc/GSM0338.TXT` & `monobit-0.43.0/monobit/encoding/tables/misc/GSM0338.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/misc/IBMGRAPH.TXT` & `monobit-0.43.0/monobit/encoding/tables/misc/IBMGRAPH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/misc/JIS0208.TXT` & `monobit-0.43.0/monobit/encoding/tables/misc/JIS0208.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/misc/KOI8-R.TXT` & `monobit-0.43.0/monobit/encoding/tables/misc/KOI8-R.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/misc/KOI8-U.TXT` & `monobit-0.43.0/monobit/encoding/tables/misc/KOI8-U.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/misc/KPS9566.TXT` & `monobit-0.43.0/monobit/encoding/tables/misc/KPS9566.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/misc/KZ1048.TXT` & `monobit-0.43.0/monobit/encoding/tables/misc/KZ1048.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/misc/NEXTSTEP.TXT` & `monobit-0.43.0/monobit/encoding/tables/misc/NEXTSTEP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/misc/SGML.TXT` & `monobit-0.43.0/monobit/encoding/tables/misc/SGML.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/misc/US-ASCII-QUOTES.TXT` & `monobit-0.43.0/monobit/encoding/tables/misc/US-ASCII-QUOTES.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/misc/dashen-map.txt` & `monobit-0.43.0/monobit/encoding/tables/misc/dashen-map.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/misc/ibm-ugl.txt` & `monobit-0.43.0/monobit/encoding/tables/misc/ibm-ugl.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/mleisher/ALTVAR.TXT` & `monobit-0.43.0/monobit/encoding/tables/mleisher/ALTVAR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/mleisher/ARMSCII-7.TXT` & `monobit-0.43.0/monobit/encoding/tables/mleisher/ARMSCII-7.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/mleisher/ARMSCII-8.TXT` & `monobit-0.43.0/monobit/encoding/tables/mleisher/ARMSCII-8.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/mleisher/ARMSCII-8A.TXT` & `monobit-0.43.0/monobit/encoding/tables/mleisher/ARMSCII-8A.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/mleisher/DECMCS.TXT` & `monobit-0.43.0/monobit/encoding/tables/mleisher/DECMCS.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/mleisher/GEO-ITA.TXT` & `monobit-0.43.0/monobit/encoding/tables/mleisher/GEO-ITA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/mleisher/GEO-PS.TXT` & `monobit-0.43.0/monobit/encoding/tables/mleisher/GEO-PS.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/mleisher/IRANSYSTEM.TXT` & `monobit-0.43.0/monobit/encoding/tables/mleisher/IRANSYSTEM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/mleisher/KOI8RU.TXT` & `monobit-0.43.0/monobit/encoding/tables/mleisher/KOI8RU.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/mleisher/OSNOVAR.TXT` & `monobit-0.43.0/monobit/encoding/tables/mleisher/OSNOVAR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/mleisher/README.md` & `monobit-0.43.0/monobit/encoding/tables/mleisher/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/mleisher/TIS620.TXT` & `monobit-0.43.0/monobit/encoding/tables/mleisher/TIS620.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/moztw/big5_2003-b2u.txt` & `monobit-0.43.0/monobit/encoding/tables/moztw/big5_2003-b2u.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/moztw/eten.txt` & `monobit-0.43.0/monobit/encoding/tables/moztw/eten.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/python/TCVN5712-1.TXT` & `monobit-0.43.0/monobit/encoding/tables/python/TCVN5712-1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/python/TCVN5712-2.TXT` & `monobit-0.43.0/monobit/encoding/tables/python/TCVN5712-2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/python/TCVN5712-3.TXT` & `monobit-0.43.0/monobit/encoding/tables/python/TCVN5712-3.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/vietstd/unicode.html` & `monobit-0.43.0/monobit/encoding/tables/vietstd/unicode.html`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/vietstd/viscii1.1.txt` & `monobit-0.43.0/monobit/encoding/tables/vietstd/viscii1.1.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/wikipedia/abicomp.html` & `monobit-0.43.0/monobit/encoding/tables/wikipedia/abicomp.html`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/wikipedia/brascii.html` & `monobit-0.43.0/monobit/encoding/tables/wikipedia/brascii.html`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/wikipedia/cp853.html` & `monobit-0.43.0/monobit/encoding/tables/wikipedia/cp853.html`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/wikipedia/cwi2.html` & `monobit-0.43.0/monobit/encoding/tables/wikipedia/cwi2.html`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/wikipedia/dec-special.html` & `monobit-0.43.0/monobit/encoding/tables/wikipedia/dec-special.html`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/wikipedia/dec-technical.html` & `monobit-0.43.0/monobit/encoding/tables/wikipedia/dec-technical.html`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/wikipedia/gem.html` & `monobit-0.43.0/monobit/encoding/tables/wikipedia/gem.html`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/wikipedia/kamenicky.html` & `monobit-0.43.0/monobit/encoding/tables/wikipedia/kamenicky.html`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/wikipedia/lics.html` & `monobit-0.43.0/monobit/encoding/tables/wikipedia/lics.html`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/wikipedia/mattel-aquarius.html` & `monobit-0.43.0/monobit/encoding/tables/wikipedia/mattel-aquarius.html`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/wikipedia/mazovia.html` & `monobit-0.43.0/monobit/encoding/tables/wikipedia/mazovia.html`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/wikipedia/pascii.html` & `monobit-0.43.0/monobit/encoding/tables/wikipedia/pascii.html`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/wikipedia/ventura.html` & `monobit-0.43.0/monobit/encoding/tables/wikipedia/ventura.html`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/wikipedia/windows-1252.html` & `monobit-0.43.0/monobit/encoding/tables/wikipedia/windows-1252.html`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/wikipedia/wingdings.html` & `monobit-0.43.0/monobit/encoding/tables/wikipedia/wingdings.html`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/wikipedia/wiscii.html` & `monobit-0.43.0/monobit/encoding/tables/wikipedia/wiscii.html`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/xfonts/mulearabic-1.enc` & `monobit-0.43.0/monobit/encoding/tables/xfonts/mulearabic-1.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/xfonts/mulearabic-2.enc` & `monobit-0.43.0/monobit/encoding/tables/xfonts/mulearabic-2.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/xfonts/mulelao-1.enc` & `monobit-0.43.0/monobit/encoding/tables/xfonts/mulelao-1.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/charmaps/xfonts/suneu-greek.enc` & `monobit-0.43.0/monobit/encoding/tables/xfonts/suneu-greek.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/containers/compressors.py` & `monobit-0.43.0/monobit/storage/wrappers/compressors.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
-monobit.containers.compressors - single-file compression wrappers
+monobit.storage.wrappers.compressors - single-file compression wrappers
 
 (c) 2021--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from pathlib import Path
 from contextlib import contextmanager
 from importlib import import_module
 
-from ..storage import loaders, savers, load_stream, save_stream
-from ..streams import Stream
-from ..magic import FileFormatError
+from monobit.storage import loaders, savers, load_stream, save_stream
+from monobit.storage import Stream
+from monobit.storage import FileFormatError
 
 
 class Compressor:
     """Base class for single-file compression helpers."""
 
     name = ''
     format = ''
```

### Comparing `monobit-0.42.2/monobit/containers/container.py` & `monobit-0.43.0/monobit/storage/containers/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
-monobit.containers.container - base class for containers
+monobit.storage.containers.container - base class for containers
 
 (c) 2021--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 import itertools
 from pathlib import Path
 
-from ..storage import (
+from ..converters import (
     loaders, savers, load_all, save_all, load_stream, save_stream
 )
 
 
 class Container:
     """Base class for container types."""
```

### Comparing `monobit-0.42.2/monobit/containers/directory.py` & `monobit-0.43.0/monobit/storage/containers/directory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-monobit.containers.directory - directory traversal
+monobit.storage.containers.directory - directory traversal
 
 (c) 2021--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import os
 import io
```

### Comparing `monobit-0.42.2/monobit/containers/mac.py` & `monobit-0.43.0/monobit/storage/formats/geos.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,338 +1,385 @@
 """
-monobit.containers.mac - Classic Mac OS resource & data fork containers
+monobit.storage.formats.geos - C64 GEOS font files
 
-(c) 2021--2023 Rob Hagemans
+(c) 2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
-import itertools
+from itertools import count
 
-from ..streams import Stream
-from ..storage import loaders, load_stream
-from ..magic import FileFormatError, Magic
+from monobit.storage import loaders, savers, Stream, Magic
+from monobit.core import Font, Glyph, Raster
+from monobit.base.struct import little_endian as le
+from monobit.base.binary import ceildiv, align
 
 
 @loaders.register(
-    name='binhex',
+    name='geos',
+    patterns=('*.cvt',),
     magic=(
-        b'(This file must be converted',
-        b'\r(This file must be converted',
+        Magic.offset(34) + b'formatted GEOS file',
     ),
-    patterns=('*.hqx',),
-    wrapper=True,
 )
-def load_binhex(instream, format='', **kwargs):
-    """BinHex 4.0 loader."""
-    return _load_macforks(_parse_binhex, instream, format, **kwargs)
-
+def load_geos(instream, merge_mega:bool=True):
+    """Load fonts from a GEOS ConVerT container."""
+    return _load_geos_cvt(instream, merge_mega)
 
 @loaders.register(
-    name='macbin',
-    magic=(
-        # FFILDMOV is a maybe
-        Magic.offset(65) + b'FFILDMOV',
-    ),
-    wrapper=True,
+    name='vlir',
 )
-def load_macbin(instream, format='', **kwargs):
-    """MacBinary loader."""
-    return _load_macforks(_parse_macbinary, instream, format, **kwargs)
-
+def load_geos_vlir(instream, offset:int=0):
+    """
+    Load a bare GEOS font VLIR.
+
+    offset: starting offset in bytes of the VLIR record in the file (default 0)
+    """
+    instream.seek(offset)
+    return _load_geos_vlir(instream)
 
-_APPLESINGLE_MAGIC = 0x00051600
-_APPLEDOUBLE_MAGIC = 0x00051607
 
+###############################################################################
+# GEOS font VLIR
+# https://www.lyonlabs.org/commodore/onrequest/geos/geos-fonts.html
 
-@loaders.register(
-    name='apple1',
-    magic=(
-        _APPLESINGLE_MAGIC.to_bytes(4, 'big'),
-    ),
-    patterns=('*.as',),
-    wrapper=True,
+_HEADER = le.Struct(
+    baseline='uint8',
+    stride='uint16',
+    height='uint8',
+    index_offset='uint16',
+    bitstream_offset='uint16',
 )
-def load_single(instream, format='', **kwargs):
-    """AppleSingle loader."""
-    return _load_macforks(_parse_apple_container, instream, format, **kwargs)
 
+# characters 0x20 - 0x7f
+# do we get plus one for the offset to the end?
+_OFFSETS = le.uint16.array(96)
 
-@loaders.register(
-    name='apple2',
-    magic=(
-        _APPLEDOUBLE_MAGIC.to_bytes(4, 'big'),
-    ),
-    # .adf, .rsrc - per http://fileformats.archiveteam.org/wiki/AppleDouble
-    # ._<name> is OS X representation
-    patterns=('*.adf', '*.rsrc', '._*'),
-    wrapper=True,
-)
-def load_double(instream, format='', **kwargs):
-    """AppleDouble loader."""
-    return _load_macforks(_parse_apple_container, instream, format, **kwargs)
 
-
-def _load_macforks(parser, instream, format, **kwargs):
-    """Resource and data fork loader."""
-    name, data, rsrc = parser(instream)
-    fonts = []
-    for fork in rsrc, data:
-        if fork:
-            stream = Stream.from_data(fork, mode='r', name=f'{name}')
-            try:
-                forkfonts = load_stream(stream, format=format, **kwargs)
-                fonts.extend(forkfonts)
-            except FileFormatError as e:
-                logging.debug(e)
-                pass
-    return fonts
+def _load_geos_vlir(instream):
+    """Load a bare GEOS font VLIR."""
+    header = _HEADER.read_from(instream)
+    logging.debug(header)
+    instream.seek(header.index_offset)
+    offsets = _OFFSETS.read_from(instream)
+    instream.seek(header.bitstream_offset)
+    strikebytes = instream.read(header.height * header.stride)
+    strikebytes = strikebytes.ljust(header.height * header.stride, b'\0')
+    strike = Raster.from_bytes(
+        strikebytes,
+        header.stride * 8, header.height,
+    )
+    # clip out glyphs
+    glyphs = tuple(
+        Glyph(
+            strike.crop(left=_offset, right=max(0, header.stride*8 - _next)),
+            codepoint=_cp,
+            shift_up=-(header.height-header.baseline-1)
+        )
+        for _offset, _next, _cp in zip(offsets, offsets[1:], count(0x20))
+    )
+    props = dict(
+        descent=header.height-header.baseline-1,
+        ascent=header.baseline+1,
+    )
+    return Font(glyphs, **props)
 
 
 ###############################################################################
-# BinHex 4.0 container
-# https://files.stairways.com/other/binhex-40-specs-info.txt
-
-from binascii import crc_hqx
-from itertools import zip_longest
+# CVT container
+# https://ist.uwaterloo.ca/~schepers/formats/GEOS.TXT
+# https://ist.uwaterloo.ca/~schepers/formats/CVT.TXT
+
+# the CVT contains a signature block, info block and record block, followed by
+# one or more VLIRs (whose starting sectors are given by the record block)
+# each such record is one sectore, i.e. 256 bytes.
+# However in the CVT files the two initial bytes, a linked-list pointer,
+# are left out.
+
+# https://ist.uwaterloo.ca/~schepers/formats/D64.TXT
+# > File Type
+# > $00 - Scratched (deleted file entry)
+# >  80 - DEL
+# >  81 - SEQ
+# >  82 - PRG
+# >  83 - USR
+# >  84 - REL
+_C64_FILETYPES = {
+    0x00: 'Scratched',
+    0x80: 'DEL',
+    0x81: 'SEQ',
+    0x82: 'PRG',
+    0x83: 'USR',
+    0x84: 'REL',
+}
 
-from ..struct import big_endian as be
+# > GEOS file structure
+# >   $00 - Sequential
+# >    01 - VLIR file
+_GEOS_STRUCTURES = {
+    0x00: 'Sequential',
+    0x01: 'VLIR',
+}
+# > GEOS filetype
+# >    $00 - Non-GEOS (normal C64 file)
+# >     01 - BASIC
+# >     02 - Assembler
+# >     03 - Data file
+# >     04 - System File
+# >     05 - Desk Accessory
+# >     06 - Application
+# >     07 - Application Data (user-created documents)
+# >     08 - Font File
+# >     09 - Printer Driver
+# >     0A - Input Driver
+# >     0B - Disk Driver (or Disk Device)
+# >     0C - System Boot File
+# >     0D - Temporary
+# >     0E - Auto-Execute File
+# >  0F-FF - Undefined
+_GEOS_FILETYPES = {
+    0x00: 'Non-GEOS',
+    0x01: 'BASIC',
+    0x02: 'Assembler',
+    0x03: 'Data file',
+    0x04: 'System File',
+    0x05: 'Desk Accessory',
+    0x06: 'Application',
+    0x07: 'Application Data (user-created documents)',
+    0x08: 'Font File',
+    0x09: 'Printer Driver',
+    0x0A: 'Input Driver',
+    0x0B: 'Disk Driver (or Disk Device)',
+    0x0C: 'System Boot File',
+    0x0D: 'Temporary',
+    0x0E: 'Auto-Execute File',
+}
 
+_GEOS_FONT_TYPE = 0x08
 
-_BINHEX_CODES = (
-    '''!"#$%&'()*+,-012345689@ABCDEFGHIJKLMNPQRSTUVXYZ[`abcdefhijklmpqr'''
+# 30 bytes 0x1e
+# https://ist.uwaterloo.ca/~schepers/formats/GEOS.TXT
+_DIR_BLOCK = le.Struct(
+    # > C64 filetype (see the section on D64 for an explanation)
+    # > REL files are not allowed.
+    filetype='uint8',
+    # > Starting track/sector (02/02 from above) of C64 file if GEOS
+    # > filetype is $00. If GEOS filetype is non-zero,  track/sector
+    # > of single-sector RECORD block
+    sector='uint16',
+    # > Filename (in ASCII, padded with $A0, case varies)
+    filename='16s',
+    # > Track/sector location of info block
+    info_sector='uint16',
+    # > GEOS file structure
+    geos_structure='uint8',
+    # > GEOS filetype
+    geos_filetype='uint8',
+    # > Year (1900 + value)
+    year='uint8',
+    # > Month (1-12, $01 to $0C)
+    month='uint8',
+    # > Day (1-31, $01 to $1F)
+    day='uint8',
+    # > Hour (0-23, $00 to $17) in military format
+    hour='uint8',
+    # > Minute (0-59, $00 to $3B)
+    minute='uint8',
+    # > Filesize, in sectors (low/high byte order)
+    filesize='uint16',
 )
-_BINHEX_CODEDICT = {_BINHEX_CODES[_i]: _i for _i in range(64)}
 
-_BINHEX_HEADER = be.Struct(
-    type='4s',
-    auth='4s',
-    flag='uint16',
-    dlen='uint32',
-    rlen='uint32',
-)
-_CRC = be.Struct(
-    crc='uint16',
+# https://ist.uwaterloo.ca/~schepers/formats/CVT.TXT
+_SIG_BLOCK = le.Struct(
+    # 0x1e   30
+    # b'PRG formatted GEOS file V1.0'
+    # b'SEQ formatted GEOS file V1.0'
+    signature='28s',
+    # 0x3a   58
+    notes=le.uint8.array(196),
+    # 0xfe  254
 )
 
-def _parse_binhex(stream):
-    """Parse a BinHex 4.0 file."""
-    front, binhex, *back = stream.text.read().split(':')
-    if 'BinHex 4.0' not in front:
-        logging.warning('No BinHex 4.0 signature found.')
-    back = ''.join(back).strip()
-    if back:
-        logging.warning('Additional data found after BinHex section: %r', back)
-    binhex = ''.join(binhex.split('\n'))
-    # decode into 6-bit ints
-    data = (_BINHEX_CODEDICT[_c] for _c in binhex)
-    # convert to bit sequence
-    bits = ''.join(bin(_d)[2:].zfill(6) for _d in data)
-    # group into chunks of 8
-    args = [iter(bits)] * 8
-    octets = (''.join(_t) for _t in zip_longest(*args, fillvalue='0'))
-    # convert to bytes
-    bytestr = bytes(int(_s, 2) for _s in octets)
-    # find run-length encoding marker
-    chunks = bytestr.split(b'\x90')
-    out = bytearray(chunks[0])
-    for c in chunks[1:]:
-        if c:
-            # run-length byte
-            repeat = c[0]
-        else:
-            # ...\x90\x90... -> ...', '', '...
-            repeat = 0x90
-        if not repeat:
-            # zero-byte is placeholder for just 0x90
-            out += b'\x90'
-        else:
-            # apply RLE. the last byte counts as the first of the run
-            out += out[-1:] * (repeat-1)
-        out += c[1:]
-    # decode header
-    length = out[0]
-    name = bytes(out[1:1+length]).decode('mac-roman')
-    if out[1+length] != 0:
-        logging.warning('No null byte after name')
-    header = _BINHEX_HEADER.from_bytes(out, 2+length)
-    logging.debug(header)
-    offset = 2 + length + _BINHEX_HEADER.size
-    crc_header = out[:offset]
-    hc = _CRC.from_bytes(out, offset)
-    offset += _CRC.size
-    if crc_hqx(crc_header, 0) != hc.crc:
-        logging.error('CRC fault in header')
-    data = out[offset:offset+header.dlen]
-    offset += header.dlen
-    dc = _CRC.from_bytes(out, offset)
-    offset += _CRC.size
-    rsrc = out[offset:offset+header.rlen]
-    offset += header.rlen
-    rc = _CRC.from_bytes(out, offset)
-    if crc_hqx(data, 0) != dc.crc:
-        logging.error('CRC fault in data fork')
-    if crc_hqx(rsrc, 0) != rc.crc:
-        logging.error('CRC fault in resource fork')
-    return name, data, rsrc
-
-
-##############################################################################
-# MacBinary container
-# v1: https://www.cryer.co.uk/file-types/b/bin_/original_mac_binary_format_proposal.htm
-# v2: https://files.stairways.com/other/macbinaryii-standard-info.txt
-# v2 defines additional fields inside an area zeroed in v1. we can ignore them.
-
-from ..binary import align
-
-
-_MACBINARY_HEADER = be.Struct(
-    # Offset 000-Byte, old version number, must be kept at zero for compatibility
-    old_version='byte',
-    # Offset 001-Byte, Length of filename (must be in the range 1-63)
-    filename_length='byte',
-    # Offset 002-1 to 63 chars, filename (only "length" bytes are significant).
-    filename='63s',
-    # Offset 065-Long Word, file type (normally expressed as four characters)
-    file_type='4s',
-    # Offset 069-Long Word, file creator (normally expressed as four characters)
-    file_creator='4s',
-    # Offset 073-Byte, original Finder flags
-    original_finder_flags='byte',
-    # Offset 074-Byte, zero fill, must be zero for compatibility
-    zero_0='byte',
-    # Offset 075-Word, file's vertical position within its window.
-    window_vert='word',
-    # Offset 077-Word, file's horizontal position within its window.
-    window_horiz='word',
-    # Offset 079-Word, file's window or folder ID.
-    window_id='word',
-    # Offset 081-Byte, "Protected" flag (in low order bit).
-    protected='byte',
-    # Offset 082-Byte, zero fill, must be zero for compatibility
-    zero_1='byte',
-    # Offset 083-Long Word, Data Fork length (bytes, zero if no Data Fork).
-    data_length='dword',
-    # Offset 087-Long Word, Resource Fork length (bytes, zero if no R.F.).
-    rsrc_length='dword',
-    # Offset 091-Long Word, File's creation date
-    creation_date='dword',
-    # Offset 095-Long Word, File's "last modified" date.
-    last_modified_date='dword',
-    # Offset 099-Word, length of Get Info comment to be sent after the resource
-    # fork (if implemented, see below).
-    get_info_length='word',
-    # *Offset 101-Byte, Finder Flags, bits 0-7. (Bits 8-15 are already in byte 73)
-    finder_flags='byte',
-    # *Offset 116-Long Word, Length of total files when packed files are unpacked.
-    packed_length='dword',
-    # *Offset 120-Word, Length of a secondary header.  If this is non-zero,
-    #              Skip this many bytes (rounded up to the next multiple of 128)
-    #              This is for future expansion only, when sending files with
-    #              MacBinary, this word should be zero.
-    second_header_length='dword',
-    # *Offset 122-Byte, Version number of Macbinary II that the uploading program
-    # is written for (the version begins at 129)
-    writer_version='byte',
-    # *Offset 123-Byte, Minimum MacBinary II version needed to read this file
-    # (start this value at 129 129)
-    reader_version='byte',
-    # *Offset 124-Word, CRC of previous 124 bytes
-    crc='word',
-    # from v1 desc:
-    # > 126 2 Reserved for computer type and OS ID
-    # > (this field will be zero for the current Macintosh).
-    reserved='word',
-    # *This is newly defined for MacBinary II.
-)
+# https://ist.uwaterloo.ca/~schepers/formats/GEOS.TXT
+_INFO_BLOCK = le.Struct(
+    # 0x02 / 0xfe - cvt leaves out the word-size pointer at the start
+    #        so sectors are only 254 bytes long
+    # > Information sector ID bytes (03 15 BF). The "03" is  likely
+    # > the bitmap width, and the "15" is likely the bitmap height,
+    # > but rare exceptions do exist to this!
+    id_bytes='3s', # > 03 15 bf
+    # 0x101
+    # > Icon bitmap (sprite format, 63 bytes)
+    icon=le.uint8.array(63),
+    # 0x140
+    # > C64 filetype (same as that from the directory entry)
+    filetype='uint8',
+    # > GEOS filetype (same as that from the directory entry)
+    geos_filetype='uint8',
+    # > GEOS file structure (same as that from the dir entry)
+    geos_structure='uint8',
+    # 0x143
+    # > Program load address
+    load_address='uint16',
+    # > Program end address (only with accessories)
+    end_address='uint16',
+    # > Program start address
+    start_address='uint16',
+    # 0x149
+    # > Class text (terminated with a $00)
+    class_text='20s',
+
+    # 0x61 / 0x15d
+    # > Author (with application data: name  of  application  disk,
+    # > terminated with a $00. This string may not  necessarily  be
+    # > set, or it may contain invalid data)
+    #author='20s',
+    # 0x75 / 0x171
+    # > 75-88: If a document, the name of the application that created it.
+    ##application='20s',
+    # 0x89/0x185
+    # > 89-9F: Available for applications, unreserved.
+    #unreserved='23s',
+
+    # here the font INFO section diverges from the standard one
+    # https://www.lyonlabs.org/commodore/onrequest/geos/geos-fonts.html
+    # 0x61 / 0x15d
+    O_GHSETLEN=le.uint16.array(15),
+    skip='uint8',
+    # 0x80 / 0x17c
+    O_GHFONTID='uint16',
+    # 0x82 / 0x17e
+    O_GHPTSIZES=le.uint16.array(15),
+    # 0xa0 / 0x19c
 
-def _parse_macbinary(stream):
-    """Parse a MacBinary file."""
-    data = stream.read()
-    header = _MACBINARY_HEADER.from_bytes(data)
-    ofs = 128
-    if header.old_version != 0:
-        raise FileFormatError(
-            'Not a MacBinary file: incorrect version field'
-            f' ({header.old_version}).'
-        )
-    if header.writer_version > 128:
-        ofs += align(header.second_header_length, 7)
-    data_fork = data[ofs:ofs+header.data_length]
-    ofs += align(header.data_length, 7)
-    rsrc_fork = data[ofs:ofs+header.rsrc_length]
-    name = header.filename.decode('mac-roman').strip()
-    return name, data_fork, rsrc_fork
-
-
-##############################################################################
-# AppleSingle/AppleDouble container
-# v1: see https://web.archive.org/web/20160304101440/http://kaiser-edv.de/documents/Applesingle_AppleDouble_v1.html
-# v2: https://web.archive.org/web/20160303215152/http://kaiser-edv.de/documents/AppleSingle_AppleDouble.pdf
-# the difference between v1 and v2 affects the file info sections
-# not the resource fork which is what we care about
-
-
-_APPLE_HEADER = be.Struct(
-    magic='uint32',
-    version='uint32',
-    home_fs='16s',
-    number_entities='uint16',
-)
-_APPLE_ENTRY = be.Struct(
-    entry_id='uint32',
-    offset='uint32',
-    length='uint32',
+    # > A0-FF: Description (terminated with a $00)
+    description='96s',
 )
 
-# Entry IDs
-_ID_DATA = 1
-_ID_RESOURCE = 2
-_ID_NAME = 3
-
-_APPLE_ENTRY_TYPES = {
-    1: 'data fork',
-    2: 'resource fork',
-    3: 'real name',
-    4: 'comment',
-    5: 'icon, b&w',
-    6: 'icon, color',
-    7: 'file info', # v1 only
-    8: 'file dates info', # v2
-    9: 'finder info',
-    # the following are all v2
-    10: 'macintosh file info',
-    11: 'prodos file info',
-    12: 'ms-dos file info',
-    13: 'short name',
-    14: 'afp file info',
-    15: 'directory id',
-}
+# font_id values
+# http://www.zimmers.net/geos/docs/fontfile.txt
+# 0    BSW            13   Tilden
+# 1    University     14   Evans
+# 2    California     15   Durant
+# 3    Roma           16   Telegraph
+# 4    Dwinelle       17   Superb
+# 5    Cory           18   Bowditch
+# 6    Tolman         19   Ormond
+# 7    Bubble         20   Elmwood
+# 8    Fontknox       21   Hearst
+# 9    Harmon         21   Brennens (BUG)
+# 10   Mykonos        23   Channing
+# 11   Boalt          24   Putnam
+# 12   Stadium        25   LeConte
+
+
+# >   If the file is a VLIR, then the RECORD block is of interest. This  single
+# > sector is made up of up to 127 track/sector pointers, each of  which  point
+# > to program sections (called RECORDS). VLIR files are comprised of  loadable
+# > RECORDS (overlays, if you wish to use PC terminology). The first RECORD  is
+# > what is always loaded first when you run that application. After that,  the
+# > OS loads whatever RECORD it needs.
+# >   When a T/S link of $00/$00 is encountered, we  are  at  the  end  of  the
+# > RECORD block. If the T/S  link  is  a  $00/$FF,  then  the  record  is  not
+# > available.
+
+# https://ist.uwaterloo.ca/~schepers/formats/CVT.TXT
+# >   Note that the RECORD block is modified  from  the  original  GEOS  entry.
+# > Instead of containing the track and sector  references,  we  now  have  the
+# > sector count and the size of the last sector in the chain
+_RECORD_ENTRY = le.Struct(
+    sector_count='uint8',
+    last_size='uint8',
+)
+_RECORD_BLOCK = _RECORD_ENTRY.array(127)
 
 
-def _parse_apple_container(stream):
-    """Parse an AppleSingle or AppleDouble file."""
-    data = stream.read()
-    header = _APPLE_HEADER.from_bytes(data)
-    if header.magic == _APPLESINGLE_MAGIC:
-        container = 'AppleSingle'
-    elif header.magic == _APPLEDOUBLE_MAGIC:
-        container = 'AppleDouble'
-    else:
-        raise FileFormatError('Not an AppleSingle or AppleDouble file.')
-    entry_array = _APPLE_ENTRY.array(header.number_entities)
-    entries = entry_array.from_bytes(data, _APPLE_HEADER.size)
-    name, data_fork, rsrc_fork = '', b'', b''
-    for i, entry in enumerate(entries):
-        entry_type = _APPLE_ENTRY_TYPES.get(entry.entry_id, 'unknown')
-        logging.debug(
-            '%s container: entry #%d, %s [%d]',
-            container, i, entry_type, entry.entry_id
+def _load_geos_cvt(instream, merge_mega):
+    """Load a GEOS ConVerT container."""
+    dir_entry = _DIR_BLOCK.read_from(instream)
+    sig_block = _SIG_BLOCK.read_from(instream)
+    logging.debug(
+        'filetype: %s',
+        _C64_FILETYPES.get(dir_entry.filetype, dir_entry.filetype)
+    )
+    logging.debug(
+        'GEOS structure: %s',
+        _GEOS_STRUCTURES.get(dir_entry.geos_structure, dir_entry.geos_structure)
+    )
+    logging.debug(
+        'GEOS filetype: %s',
+        _GEOS_FILETYPES.get(dir_entry.geos_filetype, dir_entry.geos_filetype)
+    )
+    logging.debug(
+        'timestamp: %02d-%02d-%02d %02d:%02d',
+        dir_entry.year, dir_entry.month, dir_entry.day,
+        dir_entry.hour, dir_entry.minute
+    )
+    logging.debug('signature: %s', bytes(sig_block.signature).decode('ascii', 'replace'))
+    info_block = _INFO_BLOCK.read_from(instream)
+    logging.debug('class: %s', info_block.class_text.decode('ascii', 'replace'))
+    icon = Raster.from_bytes(tuple(info_block.icon), width=24)
+    record_block = _RECORD_BLOCK.read_from(instream)
+    logging.debug(info_block)
+    logging.debug(list(x for x in record_block if not bytes(x) == b'\0\xff'))
+    if dir_entry.geos_filetype != _GEOS_FONT_TYPE:
+        logging.warning(
+            'Not a GEOS font file: incorrect filetype %x.',
+            dir_entry.geos_filetype
         )
-        if entry.entry_id == _ID_RESOURCE:
-            rsrc_fork = data[entry.offset:entry.offset+entry.length]
-        if entry.entry_id == _ID_DATA:
-            data_fork = data[entry.offset:entry.offset+entry.length]
-        if entry.entry_id == _ID_NAME:
-            name = data[entry.offset:entry.offset+entry.length]
-            name = name.decode('mac-roman')
-    return name, data_fork, rsrc_fork
+    comment = '\n\n'.join((
+        info_block.description.decode('ascii', 'replace').replace('\r', '\n'),
+        icon.as_text(),
+    ))
+    fonts = []
+    for data_size, ghptsize in zip(
+            info_block.O_GHSETLEN,
+            info_block.O_GHPTSIZES
+        ):
+        if not ghptsize or not data_size:
+            continue
+        # ptsize is (font_id << 6) + point_size
+        font_id, height = divmod(ghptsize, 1<<6)
+        logging.debug('Loading font id %d height %d', font_id, height)
+        anchor = instream.tell()
+        try:
+            font = _load_geos_vlir(Stream(instream, mode='r'))
+        except ValueError as e:
+            logging.warning(
+                'Could not load font id %d size %d: %s', font_id, height, e
+            )
+            # flag to skip to next sector
+            font = None
+        true_data_size = instream.tell() - anchor
+        if true_data_size != data_size:
+            logging.warning(
+                'Actual size 0x%x differs from reported size 0x%x',
+                true_data_size, data_size
+            )
+        # go to end of sector
+        # 254 bytes per sector - the cvt does not store the initial pointer
+        nxt = ceildiv(true_data_size, 254) * 254
+        instream.seek(anchor + nxt)
+        if font is not None:
+            font = font.modify(
+                family=dir_entry.filename.rstrip(b'\xa0').decode('ascii', 'replace'),
+                comment=comment,
+                font_id=font_id,
+            )
+            fonts.append(font)
+    # mega fonts: glyphs are divided over multiple strikes
+    # undefined glyphs are given as 1-pixel-wide
+    # last strike contains only empty or blank glyphs
+    last_empty = all(_g.is_blank() for _g in fonts[-1].glyphs)
+    # GHPTSIZE differs between strikes but actual pixel-size is the same
+    # sometimes the last (empty) strike has a different height
+    id_sizes = set((_f.font_id, _f.pixel_size) for _f in fonts[:-1])
+    # if all strikes have the same id and pixel_size, assume this is a mega font
+    if merge_mega and len(id_sizes) == 1 and last_empty:
+        logging.info('Mega font detected, merging.')
+        # take glyph of maximum width from each strike
+        selected = (
+            max(glyphs, key=lambda _g: _g.width)
+            for glyphs in zip(*(_f.glyphs for _f in fonts))
+        )
+        fonts = (fonts[0].modify(glyphs=selected),)
+    return fonts
```

### Comparing `monobit-0.42.2/monobit/containers/source.py` & `monobit-0.43.0/monobit/storage/wrappers/source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """
-monobit.containers.source - fonts embedded in C/Python/JS source files
+monobit.storage.wrappers.source - binary files embedded in C/Python/JS source files
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import string
 import logging
 from io import BytesIO
 
-from ..binary import ceildiv
-from ..storage import loaders, savers, load_stream, save_stream
-from ..streams import Stream
-from ..font import Font
-from ..glyph import Glyph
-from ..magic import FileFormatError
-from ..basetypes import Coord
+from monobit.base.binary import ceildiv
+from monobit.storage import loaders, savers, load_stream, save_stream
+from monobit.storage import Stream, FileFormatError
+from monobit.core import Font, Glyph
+from monobit.base import Coord
 
 
 def _int_from_c(cvalue):
     """Parse integer from C/Python/JS code."""
     cvalue = cvalue.strip()
     # C suffixes
     while cvalue[-1:].lower() in ('u', 'l'):
```

### Comparing `monobit-0.42.2/monobit/containers/tar.py` & `monobit-0.43.0/monobit/storage/containers/tar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
-monobit.containers.tar - tarfile container
+monobit.storage.containers.tar - tarfile container
 
 (c) 2021--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import io
 import time
 import tarfile
 import logging
 from pathlib import Path, PurePosixPath
 
 from .container import Container
-from ..streams import Stream, KeepOpen
+from ..streams import KeepOpen, Stream
 from ..magic import FileFormatError, Magic
 
 
 class TarContainer(Container):
     """Tar-file wrapper."""
 
     def __init__(self, file, mode='r', ignore_case=True):
```

### Comparing `monobit-0.42.2/monobit/containers/zip.py` & `monobit-0.43.0/monobit/storage/containers/zip.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-monobit.containers.zip - zipfile container
+monobit.storage.containers.zip - zipfile container
 
 (c) 2021--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import io
 import logging
```

### Comparing `monobit-0.42.2/monobit/formats/amiga.py` & `monobit-0.43.0/monobit/storage/formats/amiga.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """
-monobit.formats.amiga - Amiga font format
+monobit.storage.formats.amiga - Amiga font format
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import os
 import logging
 from pathlib import Path
 
-from ..binary import bytes_to_bits
-from ..storage import loaders, savers
-from ..magic import FileFormatError, Regex
-from ..font import Font, Coord
-from ..glyph import Glyph
-from ..struct import flag, bitfield, big_endian as be
-from ..properties import Props
+from monobit.base.binary import bytes_to_bits
+from monobit.storage import loaders, savers, FileFormatError, Regex
+from monobit.core import Font, Glyph
+from monobit.base.struct import flag, bitfield, big_endian as be
+from monobit.base import Props, Coord
 
 
 @loaders.register(
     name='amiga-fc',
     magic=(b'\x0f\0', b'\x0f\2'),
     patterns=('*.font',),
 )
```

### Comparing `monobit-0.42.2/monobit/formats/bbc.py` & `monobit-0.43.0/monobit/storage/formats/bbc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 """
-monobit.formats.bbc - Acorn BBC vfont format
+monobit.storage.formats.bbc - Acorn BBC vfont format
 
 (c) 2022--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 
-from ..properties import Props
-from ..storage import loaders, savers
-from ..font import Font
-from ..glyph import Glyph
-from ..magic import FileFormatError
+from monobit.base import Props
+from monobit.storage import loaders, savers, FileFormatError
+from monobit.core import Font, Glyph
 
 
 _BBC_VDU = b'\x17'
 
 # storable code points
 _BBC_RANGE = range(32, 256)
```

### Comparing `monobit-0.42.2/monobit/formats/bmfont.py` & `monobit-0.43.0/monobit/storage/formats/image/bmfont.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-monobit.formats.bmfont - AngelCode BMFont format
+monobit.storage.formats.bmfont - AngelCode BMFont format
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import json
 import shlex
@@ -14,29 +14,25 @@
 from itertools import zip_longest
 
 try:
     from PIL import Image
 except ImportError:
     Image = None
 
-from ..basetypes import Coord, Bounds
-from ..encoding import charmaps
-from .. import streams
-from ..magic import FileFormatError
-from ..binary import int_to_bytes, bytes_to_int, ceildiv
-from ..struct import little_endian as le
-from ..properties import Props, reverse_dict
-from ..storage import loaders, savers
-from ..font import Font, Coord
-from ..glyph import Glyph
-from ..labels import Codepoint, Char
-from ..chart import grid_map
-from ..glyphmap import GlyphMap
+from monobit.base import Coord, Bounds
+from monobit.encoding import encodings
+from monobit.storage import FileFormatError
+from monobit.base.binary import int_to_bytes, bytes_to_int, ceildiv
+from monobit.base.struct import little_endian as le
+from monobit.base import Props, reverse_dict
+from monobit.storage import loaders, savers
+from monobit.core import Font, Glyph, Codepoint, Char
+from monobit.render import GlyphMap, grid_map
 
-from .windows import CHARSET_MAP, CHARSET_REVERSE_MAP
+from ..common import CHARSET_MAP, CHARSET_REVERSE_MAP
 
 
 # text/xml/binary format: https://www.angelcode.com/products/bmfont/doc/file_format.html
 # json format: https://github.com/Jam3/load-bmfont/blob/master/json-spec.md
 
 _BMF_MAGIC = b'BMF'
 
@@ -675,15 +671,15 @@
         size, packed, grid, spacing, padding,
         image_format, descriptor,
         paper=0, ink=255, border=0,
     ):
     """Create a bmfont package."""
     # ensure codepoint/char values are set as appropriate
     encoding = font.encoding
-    if not charmaps.is_unicode(encoding):
+    if not encodings.is_unicode(encoding):
         font = font.label(codepoint_from=encoding)
     else:
         font = font.label(char_from=encoding)
     # map glyphs to image
     if grid:
         margin  = Coord(padding.left, padding.top)
         glyph_map = grid_map(
@@ -759,15 +755,15 @@
         )
         for _entry in glyph_map
         if _glyph_id(_entry.glyph, font.encoding) >= 0
     ]
     # save images; create page table
     props['pages'] = pages
     # info section
-    if not charmaps.is_unicode(font.encoding):
+    if not encodings.is_unicode(font.encoding):
         # if encoding is unknown, call it OEM
         charset = _CHARSET_STR_REVERSE_MAP.get(
             font.encoding, _CHARSET_STR_REVERSE_MAP['']
         )
     else:
         charset = ''
     props['info'] = {
@@ -782,15 +778,15 @@
         #
         # we're assuming size == pixel-size == ascent + descent
         # so it should be positive - negative means matching "cell height" (~ font.raster_size.y ?)
         'size': font.pixel_size,
         'bold': font.weight == 'bold',
         'italic': font.slant in ('italic', 'oblique'),
         'charset': charset,
-        'unicode': charmaps.is_unicode(font.encoding),
+        'unicode': encodings.is_unicode(font.encoding),
         'stretchH': 100,
         'smooth': False,
         'aa': 1,
         'padding': tuple(padding),
         'spacing': tuple(spacing),
         'outline': 0,
     }
@@ -839,15 +835,15 @@
         for _left, _right, _amount in kerningtable
         if _left >= 0 and _right >= 0
     )
     return props
 
 
 def _glyph_id(glyph, encoding):
-    if charmaps.is_unicode(encoding):
+    if encodings.is_unicode(encoding):
         char = glyph.char
         if len(char) > 1:
             logging.warning(
                 f"Can't store multi-codepoint grapheme sequence {ascii(char)}."
             )
             return -1
         if not char:
```

### Comparing `monobit-0.42.2/monobit/formats/borland.py` & `monobit-0.43.0/monobit/storage/formats/vector/borland.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """
-monobit.formats.borland - Borland Graphics Interface .CHR files
+monobit.storage.formats.vector.borland - Borland Graphics Interface .CHR files
 
 (c) 2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from itertools import accumulate
 
-from ..storage import loaders, savers
-from ..magic import FileFormatError
-from ..font import Font
-from ..glyph import Glyph
-from ..struct import little_endian as le, bitfield
-from ..vector import StrokePath, StrokeMove
+from monobit.storage import loaders, savers
+from monobit.storage import FileFormatError
+from monobit.base.struct import little_endian as le, bitfield
+from monobit.core import Font, Glyph, StrokePath, StrokeMove
 
 
 _BGI_MAGIC = b'PK\b\bBGI '
 
 @loaders.register(
     name='borland',
     magic=(_BGI_MAGIC,),
@@ -169,29 +167,19 @@
 def _convert_to_stroke_code(command, absx, absy):
     """Convert path command to two-byte stroke code."""
     return _STROKE_CODE(
         op0=-1, op1=-1 * (command==StrokePath.LINE),
         x=absx, y=absy
     )
 
-def _make_contiguous(font):
-    """Fill out a contiguous range of glyphs."""
-    # we need a contiguous range between the min and max codepoints
-    codepoints = font.get_codepoints()
-    ord_glyphs = [
-        font.get_glyph(_codepoint, missing='empty')
-        for _codepoint in range(min(codepoints)[0], max(codepoints)[0]+1)
-    ]
-    font = font.modify(ord_glyphs)
-    return font
-
-
 def _convert_to_borland(font):
     """Convert monobit Font to BGI font data."""
-    font = _make_contiguous(font)
+    min_range = int(min(font.get_codepoints()))
+    max_range = min(int(max(font.get_codepoints())), 255)
+    font = font.resample(codepoints=range(min_range, max_range+1))
     glyphbytes = []
     widths = []
     offsets = []
     for glyph in font.glyphs:
         code = []
         if glyph.path:
             path = glyph.path.as_moves()
```

### Comparing `monobit-0.42.2/monobit/formats/cpi.py` & `monobit-0.43.0/monobit/storage/formats/cpi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """
-monobit.formats.cpi - DOS Codepage Information format
+monobit.storage.formats.cpi - DOS Codepage Information format
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import os
 import string
 import logging
 from itertools import accumulate
 
-from ..binary import ceildiv
-from ..struct import little_endian as le, sizeof
-from ..storage import loaders, savers
-from ..magic import FileFormatError, Magic
-from ..font import Font
-from ..glyph import Glyph
-from ..properties import Props
+from monobit.base import Props
+from monobit.base.binary import ceildiv
+from monobit.base.struct import little_endian as le, sizeof
+from monobit.storage import loaders, savers, FileFormatError, Magic
+from monobit.core import Font, Glyph
 
 from .raw import load_bitmap
 
 
 _ID_MS = b'FONT   '
 _ID_NT = b'FONT.NT'
 _ID_DR = b'DRFONT '
@@ -81,22 +79,32 @@
         )
     _write_cp(outstream, cpdata[0], format=format)
 
 
 @savers.register(linked=load_cpi)
 def save_cpi(
         fonts, outstream,
-        version:str=_ID_MS, codepage_prefix:str='cp'
+        version:str=_ID_MS, codepage_prefix:str='cp',
+        codepages:str='',
     ):
     """
     Save character-cell fonts to Linux Keyboard Codepage (.CP) file.
 
     version: CPI format version. One of 'DRFONT', 'FONT.NT', or 'FONT' (default)
     codepage_prefix: prefix to use to find numbered codepage in encodings. Default: 'cp'.
+    codepages: codepages to resample from fonts provided
     """
+    if isinstance(codepages, str):
+        codepages = tuple(_cpg for _cpg in codepages.split(',') if _cpg)
+    if codepages:
+        fonts = tuple(
+            _f.resample(encoding=codepage_prefix+_cpg)
+            for _f in fonts
+            for _cpg in codepages
+        )
     format = version[:7].upper().ljust(7)
     if isinstance(format, str):
         format = format.encode('ascii', 'replace')
     if format in (_ID_MS, _ID_NT):
         return _save_ms_cpi(fonts, outstream, format, codepage_prefix)
     elif format == _ID_DR:
         return _save_dr_cpi(fonts, outstream, format, codepage_prefix)
@@ -413,31 +421,20 @@
         return None
     if not font.encoding.startswith(codepage_prefix):
         logging.warning(
             'CP fonts must have encoding set to a numbered codepage'
         )
         return None
     # ensure codepoint values are set, if possible
-    font = font.label(codepoint_from=font.encoding)
     # take only the glyphs that will fit
-    font = font.subset(_RANGE)
+    font = font.resample(_RANGE, missing=Glyph.blank(*font.cell_size))
     font = font.equalise_horizontal()
-    font = _fill_contiguous(font, _RANGE, Glyph.blank(*font.cell_size))
     return font
 
 
-def _fill_contiguous(font, full_range, filler):
-    """Get contiguous range, fill gaps with empties."""
-    glyphs = tuple(
-        font.get_glyph(codepoint=_cp, missing=filler).modify(codepoint=_cp)
-        for _cp in full_range
-    )
-    font = font.modify(glyphs)
-    return font
-
 def _get_consistent(fonts, property):
     """Get value for a property across fonts, or None if inconsistent."""
     values = tuple(set(
         _font.get_property(property)
         for _font in fonts
         if property in _font.get_properties()
     ))
```

### Comparing `monobit-0.42.2/monobit/formats/daisydot.py` & `monobit-0.43.0/monobit/storage/formats/daisydot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 """
-monobit.formats.daisydot - Daisy Dot II/III NLQ format
+monobit.storage.formats.daisydot - Daisy Dot II/III NLQ format
 
 (c) 2022--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from pathlib import Path
 
-from ..struct import big_endian as be
-from ..storage import loaders, savers
-from ..font import Font
-from ..glyph import Glyph
-from ..raster import Raster
-from ..magic import FileFormatError
-from ..binary import ceildiv, bytes_to_bits
+from monobit.base.struct import big_endian as be
+from monobit.base.binary import ceildiv, bytes_to_bits
+from monobit.storage import loaders, savers, FileFormatError
+from monobit.core import Font, Glyph, Raster
 
 
 # Daisy-Dot II
 _DD2_MAGIC = b'DAISY-DOT NLQ FONT\x9b'
 # Daisy-Dot III
 _DD3_MAGIC = b'3\x9b'
 # Daisy-Dot III Magnified
```

### Comparing `monobit-0.42.2/monobit/formats/dashen.py` & `monobit-0.43.0/monobit/storage/formats/dashen.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 """
-monobit.formats.dashen - Dashen font
+monobit.storage.formats.dashen - Dashen font
 
 (c) 2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 
-from ..binary import ceildiv
-from ..struct import little_endian as le
-from ..properties import Props
-from ..storage import loaders, savers
-from ..font import Font
-from ..glyph import Glyph
-from ..raster import Raster
-from ..properties import Props
-from ..magic import Magic, FileFormatError
+from monobit.base.binary import ceildiv
+from monobit.base.struct import little_endian as le
+from monobit.base import Props
+from monobit.storage import loaders, savers, Magic, FileFormatError
+from monobit.core import Font, Glyph, Raster
 
 from .pcl import load_hppcl
 
 
 @loaders.register(
     name='dashen',
     patterns=('*.pft',),
```

### Comparing `monobit-0.42.2/monobit/formats/dec.py` & `monobit-0.43.0/monobit/storage/formats/dec.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 """
-monobit.formats.dec - DEC Dynamically Redefined Character Set
+monobit.storage.formats.dec - DEC Dynamically Redefined Character Set
 
 (c) 2022--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 # DRCS format documentation
 # https://vt100.net/dec/vt320/soft_characters
 # https://vt100.net/docs/vt510-rm/DECDLD
 
 
 import shlex
 import logging
 
-from ..storage import loaders, savers
-from ..magic import FileFormatError
-from ..font import Font
-from ..glyph import Glyph
-from ..binary import ceildiv
-from ..basetypes import Coord
-from ..properties import reverse_dict
+from monobit.storage import loaders, savers, FileFormatError
+from monobit.core import Font, Raster, Glyph
+from monobit.base.binary import ceildiv
+from monobit.base import Coord
+from monobit.base import reverse_dict
 
 
 @loaders.register(
     name='dec',
     magic=(b'\x90', b'\x1bP'),
 )
 def load_dec_drcs(instream):
@@ -43,16 +41,14 @@
         raise FileFormatError('Can only save one font to dec-drcs file.')
         # check if font is fixed-width and fixed-height
     font, = fonts
     if font.spacing != 'character-cell':
         raise FileFormatError(
             'This format only supports character-cell fonts.'
         )
-    # ensure codepoint values are set if possible
-    font = font.label(codepoint_from=font.encoding)
     # fill out bearings and equalise heights
     font = font.equalise_horizontal()
     # upper size limits vary by device, not enforced.
     # lower sizes would conflict with vt200 size values
     if font.raster_size.x < 5 or font.raster_size.y < 1:
         raise FileFormatError(
             'This format only supports fonts of 5px or wider and 1px or taller.'
@@ -263,22 +259,22 @@
         for _block in glyphdef.split(b'/')
     )
     glyphbytes = zip(*glyphbytes)
     glyphstrs = tuple(
         ''.join(f'{_b:06b}' for _b in _pair[::-1])
         for _pair in glyphbytes
     )
-    glyph = Glyph(glyphstrs, _0='0', _1='1')
+    raster = Raster(glyphstrs, _0='0', _1='1')
     # pylint: disable=unexpected-keyword-arg
-    glyph = glyph.turn(anti=1)
-    glyph = glyph.crop(
-        right=glyph.width-raster_size.x,
-        bottom=glyph.height-raster_size.y
+    raster = raster.turn(anti=1)
+    raster = raster.crop(
+        right=max(0, raster.width-raster_size.x),
+        bottom=max(0, raster.height-raster_size.y),
     )
-    return glyph
+    return Glyph(raster)
 
 
 def _parse_drcs_glyphs(glyphdefs, props, first_codepoint):
     """Convert DRCS glyphs to monobit glyphs."""
     glyphs = (
         _convert_drcs_glyph(_g, Coord(*props['raster_size']))
         for _g in glyphdefs
@@ -334,20 +330,18 @@
     return props, count, first_codepoint
 
 ##########################################################################
 
 def _write_dec_drcs(font, outstream, use_8bit=False):
     """Write a font to a DRCS file."""
     esc = not use_8bit
-    # we can onl store the printable ascii range
+    # we can only store the printable ascii range
     ascii = tuple(chr(_b) for _b in range(0x20, 0x80))
-    glyphs = tuple(
-        font.get_glyph(char=_c, missing='empty')
-        for _c in ascii
-    )
+    font = font.resample(ascii, missing='empty')
+    glyphs = font.glyphs
     # write 96 glyphs?
     is_big = not glyphs[0].is_blank() or not glyphs[-1].is_blank()
     if not is_big:
         glyphs = glyphs[1:-1]
     dec_props = _convert_to_drcs_props(font, is_big)
     outstream.write(_ESC_START[esc])
     outstream.write(b';'.join(
```

### Comparing `monobit-0.42.2/monobit/formats/dosstart.py` & `monobit-0.43.0/monobit/storage/formats/dosstart.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 """
-monobit.formats.dosstart - DosStart! format
+monobit.storage.formats.dosstart - DosStart! format
 
 (c) 2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 import string
 from io import StringIO
 
-from ..storage import loaders, savers
-from ..magic import FileFormatError
-from ..font import Font
-from ..glyph import Glyph
-from ..raster import Raster
-from ..vector import StrokePath
+from monobit.storage import loaders, savers, FileFormatError
+from monobit.core import Font, Glyph, Raster, StrokePath
 
 
 @loaders.register(
     name='dosstart',
     magic=(b'DosStartFont',),
     patterns=('*.dsf',),
 )
```

### Comparing `monobit-0.42.2/monobit/formats/figlet.py` & `monobit-0.43.0/monobit/storage/formats/figlet.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """
-monobit.formats.figlet - FIGlet .flf format
+monobit.storage.formats.figlet - FIGlet .flf format
 
 (c) 2021--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from typing import NamedTuple
 
-from ..storage import loaders, savers
-from ..magic import FileFormatError
-from ..font import Font
-from ..glyph import Glyph
-from ..properties import Props, reverse_dict, extend_string
-from ..taggers import tagmaps
+from monobit.storage import loaders, savers, FileFormatError
+from monobit.base import Props, reverse_dict, extend_string
+from monobit.core import Font, Glyph
+from monobit.encoding import encodings
 
 
 # note that we won't be able to use the "subcharacters" that are the defining feature of FIGlet
 # as we only work with monochrome bitmaps
 
 
 ##############################################################################
@@ -206,23 +204,22 @@
 
 ##############################################################################
 # saver
 
 def _convert_to_flf(font, hardblank='$'):
     """Convert monobit glyphs and properties to figlet."""
     # ensure we have unicode labels where possible
-    font = font.label()
+    if not font.get_chars():
+        raise FileFormatError('No figlet-storable codepoints in font.')
     # count glyphs outside the default set
     # we can only encode glyphs that have chars
     # latin-1 codepoints, so we can just use chr()
     flf_chars = tuple(chr(_cp) for _cp in _CODEPOINTS)
     # exclude NULL which is used for the default char
     coded_chars = set(font.get_chars()) - set(flf_chars) - set('\0')
-    if not font.get_chars():
-        raise FileFormatError('No figlet-storable codepoints in font.')
     # construct flf properties
     props = Props(
         signature_hardblank=_SIGNATURE + hardblank,
         height=font.line_height,
         baseline=font.ascent,
         # > The Max_Length parameter is the maximum length of any line describing a
         # > FIGcharacter.  This is usually the width of the widest FIGcharacter, plus 2
@@ -242,17 +239,22 @@
         figprops = {_k: _v for _k, _, _v in propsplit}
     else:
         figprops = {}
     props.old_layout = figprops.get('old_layout', 0)
     props.full_layout = figprops.get('full_layout', 0)
     # first get glyphs in default repertoire
     # fill missing glyphs with empties
-    glyphs = [font.get_glyph(_chr, missing='empty') for _chr in flf_chars]
+    glyphs = [
+        font.get_glyph(_chr, missing='empty').modify(char=_chr)
+        for _chr in flf_chars
+    ]
     # code-tagged glyphs
-    glyphs.extend(font.get_glyph(_chr) for _chr in sorted(coded_chars))
+    glyphs.extend(
+        font.get_glyph(_chr).modify(char=_chr) for _chr in sorted(coded_chars)
+    )
     # map default glyph to codepoint zero
     # > If a FIGcharacter with code 0 is present, it is treated
     # > specially.  It is a FIGfont's "missing character".  Whenever
     # > the FIGdriver is told to print a character which doesn't exist
     # > in the current FIGfont, it will print FIGcharacter 0.  If there
     # > is no FIGcharacter 0, nothing will be printed.
     glyphs.append(font.get_default_glyph().modify(char='\0'))
@@ -273,15 +275,15 @@
     if comments:
         outstream.write(comments + '\n')
     # use hardblank for space char (first char)
     outstream.write(_format_glyph(flf_glyphs[0], ink=ink, paper=hardblank))
     for glyph in flf_glyphs[1:len(_CODEPOINTS)]:
         outstream.write(_format_glyph(glyph, ink=ink, paper=paper))
     for glyph in flf_glyphs[len(_CODEPOINTS):]:
-        tag = glyph.tags[0] if glyph.tags else tagmaps['name'].tag(*glyph.get_labels()).value
+        tag = glyph.tags[0] if glyph.tags else encodings['name'].tag(*glyph.get_labels()).value
         if glyph.char > chr(255):
             outstream.write(f'{ord(glyph.char):#04x} {tag}\n')
         else:
             outstream.write(f'{ord(glyph.char)} {tag}\n')
         outstream.write(_format_glyph(glyph, ink=ink, paper=paper))
```

### Comparing `monobit-0.42.2/monobit/formats/fontx.py` & `monobit-0.43.0/monobit/storage/formats/fontx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-"""
-monobit.formats.fontx - DOS/V FONTX2 format
+f"""
+monobit.storage.formats.fontx - DOS/V FONTX2 format
 
 (c) 2022--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from itertools import accumulate
 
-from ..struct import bitfield, little_endian as le
-from ..properties import Props
-from ..storage import loaders, savers
-from ..font import Font
-from ..glyph import Glyph
-from ..magic import FileFormatError
-from ..binary import ceildiv
+from monobit.base.struct import bitfield, little_endian as le
+from monobit.base.binary import ceildiv
+from monobit.base import Props
+from monobit.storage import loaders, savers, FileFormatError
+from monobit.core import Font, Glyph
 
 from .raw import load_bitmap
 
 
 _FONTX_MAGIC = b'FONTX2'
 
 
@@ -142,17 +140,14 @@
     if font.spacing != 'character-cell':
         raise FileFormatError(
             'FONTX2 format can only store character-cell fonts.'
         )
     # inflate glyphs to fill positive horizontal bearings
     font = font.equalise_horizontal()
     blank = Glyph.blank(*font.raster_size)
-    # ensure codepoint values are set if possible
-    if font.encoding:
-        font = font.label(codepoint_from=font.encoding)
     props = Props(
         code_flag=len(max(font.get_codepoints())) > 1,
         name=font.name[:8].encode('ascii', 'replace'),
         width=font.cell_size.x,
         height=font.cell_size.y,
     )
     if not props.code_flag:
@@ -172,20 +167,17 @@
             for _hi in range(256)
         )
         # skip empty ranges
         blocks = tuple(
             range(min(_page), max(_page)+1)
             for _page in pages if _page
         )
-    glyphs = tuple(
-        font.get_glyph(codepoint=_cp, missing=blank).modify(codepoint=_cp)
-        for _range in blocks
-        for _cp in _range
-    )
-    return props, blocks, glyphs
+    codepoints = (_cp for _range in blocks for _cp in _range)
+    font = font.resample(codepoints=codepoints, missing=blank)
+    return props, blocks, font.glyphs
 
 def _write_fontx(outstream, props, blocks, glyphs):
     """Write fontx properties and glyphs to binary file."""
     glyph_bytes = tuple(_g.as_bytes() for _g in glyphs)
     bitmap = b''.join(glyph_bytes)
     offsets = (0,) + tuple(accumulate(len(_g) for _g in glyph_bytes))
     sbcs_header = _SBCS_HEADER(
```

### Comparing `monobit-0.42.2/monobit/formats/fzx.py` & `monobit-0.43.0/monobit/storage/formats/fzx.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """
-monobit.formats.fzx - FZX format
+monobit.storage.formats.fzx - FZX format
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from itertools import accumulate
 
-from ..binary import ceildiv
-from ..struct import bitfield, little_endian as le
-from ..properties import Props
-from ..storage import loaders, savers
-from ..font import Font
-from ..glyph import Glyph
-from ..magic import FileFormatError
+from monobit.base.binary import ceildiv
+from monobit.base.struct import bitfield, little_endian as le
+from monobit.base import Props
+from monobit.storage import loaders, savers, FileFormatError
+from monobit.core import Font, Glyph
 
 
 # beyond ASCII, multiple encodings are in use - set these manually after extraction
 _FZX_RANGE = range(32, 256)
 
 
 @loaders.register(
@@ -231,25 +229,20 @@
         right_bearing=fzx_props.tracking,
     )
     return properties, glyphs
 
 
 def _convert_to_fzx(font):
     """Convert monobit font to FZX properties and glyphs."""
-    # ensure codepoint values are set if possible
-    font = font.label(codepoint_from=font.encoding)
     # select glyphs that can be included
     # only codepoints 32--255 inclusive
     # on extraction 32--127 will be assumed to be ASCII
-    includable = font.subset(codepoints=set(_FZX_RANGE))
     # get contiguous range, fill gaps with empties
-    glyphs = tuple(
-        includable.get_glyph(codepoint=_cp, missing='empty').modify(codepoint=_cp)
-        for _cp in _FZX_RANGE
-    )
+    font = font.resample(codepoints=_FZX_RANGE, missing='empty')
+    glyphs = font.glyphs
     # remove empties at end
     while glyphs and glyphs[-1].is_blank() and not glyphs[-1].advance_width:
         glyphs = glyphs[:-1]
     if not glyphs:
         raise FileFormatError(
             'FZX format: no glyphs in storable codepoint range 32--255.'
         )
```

### Comparing `monobit-0.42.2/monobit/formats/gdos.py` & `monobit-0.43.0/monobit/storage/formats/gdos.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 """
-monobit.formats.gdos - Atari GDOS/GEM format
+monobit.storage.formats.gdos - Atari GDOS/GEM format
 
 (c) 2022--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from itertools import accumulate
 
-from ..struct import bitfield, little_endian as le, big_endian as be, sizeof
-from ..properties import Props
-from ..storage import loaders, savers
-from ..font import Font
-from ..glyph import Glyph
-from ..magic import FileFormatError, Magic
-from ..binary import bytes_to_bits, ceildiv
-from ..raster import Raster
+from monobit.base.struct import bitfield, little_endian as le, big_endian as be, sizeof
+from monobit.base.binary import bytes_to_bits, ceildiv
+from monobit.base import Props
+from monobit.storage import loaders, savers, FileFormatError, Magic
+from monobit.core import Font, Glyph, Raster
 
 
 @loaders.register(
     name='gdos',
     patterns=('*.fnt', '*.gft', '*.[cev]ga'),
     # maybe - this is the usual value for 'lighten' and 'skew'
     magic=(Magic.offset(62) + b'UUUU',),
@@ -554,17 +551,17 @@
 
 ################################################################################
 # GDOS writer
 
 def _convert_to_gdos(font, endianness):
     """Convert monobit font to GDOS properties and glyphs."""
     # ensure codepoint values are set if possible
-    font = font.label(codepoint_from=font.encoding)
-    font = font.subset(_GDOS_RANGE)
-    font = _make_contiguous(font)
+    min_range = max(int(min(font.get_codepoints())), min(_GDOS_RANGE))
+    max_range = min(int(max(font.get_codepoints())), max(_GDOS_RANGE))
+    font = font.resample(codepoints=range(min_range, max_range+1))
     # bring to padded normal form with equalised upshifts
     font = font.equalise_horizontal()
     upshifts = set(_g.shift_up for _g in font.glyphs)
     shift_up, *remainder = upshifts
     assert not remainder
     # check glyph dimensions / bitfield ranges
     if any(_g.left_bearing < -127 or _g.right_bearing < -127 for _g in font.glyphs):
@@ -587,16 +584,16 @@
         dbcs_flag=0,
         use_full_id=0,
     )
     header = _FNT_HEADER[endian](
         font_id=add_props.get('font-id', 255),
         point=font.point_size,
         name=font.name.encode('ascii', 'replace')[:32],
-        first_ade=int(min(font.get_codepoints())),
-        last_ade=int(max(font.get_codepoints())),
+        first_ade=min_range,
+        last_ade=max_range,
         # common shift up must be negative as we brought to padded normal form
         top=font.raster_size.y + shift_up,
         ascent=font.ascent-1,
         # Half line distance expressed as a positive offset from baseline.
         # interpreting as x-height
         half=font.x_height,
         descent=font.descent,
@@ -616,33 +613,14 @@
         skew=add_props.get('skew_mask', 0x5555),
         flags=flags,
         #hor_table, off_table, dat_table, form_width, form_height
     )
     return header, font.glyphs
 
 
-def _make_contiguous(font):
-    """Get contiguous range, fill gaps with empties."""
-    glyphs = tuple(
-        font.get_glyph(codepoint=_cp, missing='empty').modify(codepoint=_cp)
-        for _cp in range(
-            int(min(font.get_codepoints())),
-            int(max(font.get_codepoints()))+1
-        )
-    )
-    # remove empties at end
-    while glyphs and glyphs[-1].is_blank() and not glyphs[-1].advance_width:
-        glyphs = glyphs[:-1]
-    if not glyphs:
-        raise FileFormatError(
-            'Output format: no glyphs in storable codepoint range 0--255.'
-        )
-    font = font.modify(glyphs)
-    return font
-
 def _generate_bitmap_strike(glyphs):
     """Generate horizontal bitmap strike."""
     # all glyphs have been brought to the same height previously
     matrices = tuple(_g.as_matrix() for _g in glyphs)
     strike = tuple(
         sum((_m[_row] for _m in matrices), ())
         for _row in range(glyphs[0].height)
```

### Comparing `monobit-0.42.2/monobit/formats/hurt.py` & `monobit-0.43.0/monobit/storage/formats/vector/hurt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """
-monobit.formats.hurt - read Hershey fonts in Jim Hurt's format
+monobit.storage.formats.vector.hurt - read Hershey fonts in Jim Hurt's format
 
 (c) 2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 
-from ..storage import loaders, savers
-from ..font import Font
-from ..glyph import Glyph
-from ..struct import big_endian as be, bitfield
-from ..properties import Props
-from ..vector import StrokePath
+from monobit.storage import loaders, savers
+from monobit.core import Font, Glyph, StrokePath
+from monobit.base.struct import big_endian as be, bitfield
+from monobit.base import Props
 
 
 @loaders.register(
     name='hurt',
     patterns=('*.jhf',),
 )
 def load_hurt(
@@ -36,15 +34,15 @@
     font = _convert_hurt(jhf_data, baseline, top, bottom)
     return font
 
 
 ###############################################################################
 # the distribution format is described in the accompanying usenet messages
 # https://web.mit.edu/ghostscript/www/Hershey.htm
-# the format brings too mind FORTRAN77 and punch cards
+# the format brings to mind FORTRAN77 and punch cards
 # https://hackaday.com/2021/03/30/hershey-fonts-not-chocolate-the-origin-of-vector-lettering/
 # the *original* NTIS format seems to have been spelled-out numbers in a book
 
 
 _LINEHEADER = be.Struct(
     number='5s',
     datasize='3s',
```

### Comparing `monobit-0.42.2/monobit/formats/image.py` & `monobit-0.43.0/monobit/storage/formats/image/image.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 """
-monobit.formats.image - fonts stored in image files
+monobit.storage.formats.image.image - fonts stored in image files
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from collections import Counter
 from pathlib import Path
 
 try:
     from PIL import Image
 except ImportError:
     Image = None
 
-from ..basetypes import Coord, RGB
-from ..binary import ceildiv
-from ..storage import loaders, savers
-from ..magic import FileFormatError
-from ..font import Font
-from ..glyph import Glyph
-from ..chart import chart, grid_traverser
+from monobit.base import Coord, RGB
+from monobit.base.binary import ceildiv
+from monobit.storage import loaders, savers
+from monobit.storage import FileFormatError
+from monobit.core import Font, Glyph
+from monobit.render import chart, grid_traverser
 
 
 DEFAULT_IMAGE_FORMAT = 'png'
 
 
 # available background policies
 # -----------------------------
```

### Comparing `monobit-0.42.2/monobit/formats/mousegraphics.py` & `monobit-0.43.0/monobit/storage/formats/apple/mgtk.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """
-monobit.formats.mousegraphics - Apple II MouseGraphics ToolKit Font Format
+monobit.storage.formats.apple.mgtk - Apple II MouseGraphics ToolKit Font Format
 
 (c) 2023 Kelvin Sherlock
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 
-from ..storage import loaders, savers
-from ..font import Font
-from ..glyph import Glyph
-from ..labels import Char
-from ..struct import little_endian as le
-from ..binary import bytes_to_bits
+from monobit.storage import loaders, savers
+from monobit.core import Font, Glyph, Char
+from monobit.base.struct import little_endian as le
+from monobit.base.binary import bytes_to_bits
 
 
 @loaders.register(
     name='mgtk'
 )
 def load_mgtk_fnt(instream):
     """Load font from a MouseGraphics ToolKit font file"""
```

### Comparing `monobit-0.42.2/monobit/formats/mzfon.py` & `monobit-0.43.0/monobit/storage/formats/fon/fon.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """
-monobit.formats.mzfon - Windows and OS/2 FON files
+monobit.storage.formats.fon.fon - Windows and OS/2 FON files
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 
-from ..storage import loaders, savers
-from ..streams import Stream
-from ..magic import FileFormatError
+from monobit.storage import loaders, savers
+from monobit.storage import Stream
+from monobit.storage import FileFormatError
 
-from .windows.mz import MZ_HEADER, create_mz_stub
+from monobit.storage.formats.sfnt import load_sfnt, SFNT_MAGIC
+
+from .mz import MZ_HEADER, create_mz_stub
 from .windows.ne import create_ne, read_ne, NE_HEADER
 from .windows.pe import read_pe
 from .windows.fnt import (
     convert_win_fnt_resource,
     FNT_MAGIC_1, FNT_MAGIC_2, FNT_MAGIC_3
 )
 from .os2.lx import read_lx
 from .os2.ne import read_os2_ne
 from .os2.gpifont import convert_os2_font_resource, GPI_MAGIC
-from .sfnt import load_sfnt, SFNT_MAGIC
 
 
 @loaders.register(
     name='mzfon',
     magic=(b'MZ', b'LX', b'LE', b'NE', b'PE'),
     patterns=('*.fon', '*.exe', '*.dll'),
 )
```

### Comparing `monobit-0.42.2/monobit/formats/nearlyraw.py` & `monobit-0.43.0/monobit/storage/formats/nearlyraw.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """
-monobit.formats.nearlyraw - almost raw binary font files
+monobit.storage.formats.nearlyraw - almost raw binary font files
 
 (c) 2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
-from ..storage import loaders, savers
-from ..glyph import Glyph
-from ..font import Font
-from ..struct import little_endian as le, bitfield
-from ..magic import Magic, FileFormatError
+
+from monobit.storage import loaders, savers, Magic, FileFormatError
+from monobit.core import Glyph, Font
+from monobit.base.struct import little_endian as le, bitfield
 
 from .raw import load_bitmap, save_bitmap
 
 
 ###############################################################################
 # OPTIKS PCR - near-raw format
 # http://fileformats.archiveteam.org/wiki/PCR_font
@@ -270,21 +269,23 @@
 
 
 @savers.register(linked=load_xbin)
 def save_xbin(fonts, outstream):
     """Save an XBIN font."""
     font, *extra = fonts
     if extra:
-        raise FileFormatError('Can only save a single font to an XBIN file')
+        raise ValueError('Can only save a single font to an XBIN file')
     if font.spacing != 'character-cell' or font.cell_size.x != 8:
-        raise FileFormatError(
+        raise ValueError(
             'This format can only store 8xN character-cell fonts'
         )
-    font = font.label(codepoint_from=font.encoding)
-    max_cp = max(int(_cp) for _cp in font.get_codepoints())
+    codepoints = font.get_codepoints()
+    if not codepoints:
+        raise ValueError('No storable codepoints found in font.')
+    max_cp = max(int(_cp) for _cp in codepoints)
     if max_cp >= 512:
         logging.warning('Glyphs above codepoint 512 will not be stored.')
     blank = Glyph.blank(width=8, height=font.cell_size.y)
     if max_cp >= 256:
         count = 512
     else:
         count = 256
```

### Comparing `monobit-0.42.2/monobit/formats/palm.py` & `monobit-0.43.0/monobit/storage/formats/apple/palm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
-monobit.formats.palm - Palm OS databases and font resources
+monobit.storage.formats.apple.palm - Palm OS databases and NFNT font resources
 
 (c) 2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 
-from ..struct import big_endian as be
-from ..properties import Props
-from ..storage import loaders, savers
-from ..font import Font
-from ..magic import FileFormatError, Magic
+from monobit.base.struct import big_endian as be
+from monobit.base import Props
+from monobit.storage import loaders, savers
+from monobit.core import Font
+from monobit.storage import FileFormatError, Magic
 
-from .mac.nfnt import extract_nfnt, convert_nfnt
+from .nfnt import extract_nfnt, convert_nfnt
 
 
 # offset magic: b'FontFont' at offset 0x3c (type, creator fields)
 @loaders.register(
     name='palm',
     magic=(Magic.offset(0x3c) + b'FontFont',),
     patterns=('*.pdb',),
```

### Comparing `monobit-0.42.2/monobit/formats/pcl.py` & `monobit-0.43.0/monobit/storage/formats/pcl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 """
-monobit.formats.pcl - HP PCL soft fonts
+monobit.storage.formats.pcl - HP PCL soft fonts
 
 (c) 2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from io import BytesIO
 
-from ..storage import loaders, savers
-from ..magic import FileFormatError, Magic
-from ..struct import big_endian as be, bitfield
-from ..glyph import Glyph
-from ..raster import Raster
-from ..font import Font
-from ..properties import Props, reverse_dict
-from ..encoding import charmaps
+from monobit.storage import loaders, savers, FileFormatError, Magic
+from monobit.base.struct import big_endian as be, bitfield
+from monobit.core import Glyph, Raster, Font
+from monobit.base import Props, reverse_dict
+from monobit.encoding import EncodingName
 
 
 @loaders.register(
     name='hppcl',
     magic=(
         b'\x1b)s' + Magic.offset(2) + b'W',
         b'\x1b)s' + Magic.offset(3) + b'W',
@@ -54,15 +51,14 @@
     if orientation.lower().startswith('p'):
         orientation = 0
     elif orientation.lower().startswith('l'):
         orientation = 1
     else:
         raise ValueError(f"orientation must be one of 'portrait' or 'landscape', not {orientation}")
     # get storable glyphs (8-bit bound)
-    font = font.label(codepoint_from=font.encoding)
     font = font.subset(codepoints=range(256))
     # convert
     fontdef, copyright = _convert_to_hppcl_props(font, orientation)
     glyphdefs = (
         _convert_to_hppcl_glyph(glyph, orientation)
         for glyph in font.glyphs
     )
@@ -492,15 +488,15 @@
     # '0B': 'pcl-linedraw-7', # == pcl-linedraw-71
     # '0L': 'pcl-linedraw-7',
     # '14L': # pcl itc zapf dingbats
     # '5M': # pcl ps math symbol set
     # '19M': # pcl math symbol set
 }
 _REV_SYMBOL_SETS = {
-    charmaps.normalise(_k): _v
+    EncodingName(_k): _v
     for _k, _v in reverse_dict(_SYMBOL_SETS).items()
 }
 
 
 ###############################################################################
 # converter
 
@@ -800,15 +796,15 @@
         chardef.character_height = glyph.width
     return int(glyph.codepoint), chardef, glyphbytes
 
 
 def _symbol_set_from_encoding(encoding):
     """Convert encoding to symbol set code."""
     try:
-        code = _REV_SYMBOL_SETS[charmaps.normalise(encoding)]
+        code = _REV_SYMBOL_SETS[EncodingName(encoding)]
     except KeyError:
         if not encoding.startswith('pcl-'):
             return 0
         code = encoding.removeprefix('pcl-')
     if not len(code) == 2 or not code[0].isdigit():
         return 0
     num, lett = code
```

### Comparing `monobit-0.42.2/monobit/formats/pcpaint.py` & `monobit-0.43.0/monobit/storage/formats/pcpaint.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """
-monobit.formats.pcpaint - ChiWriter, GRASP, PCPaint, FONTRIX (for IBM) font files
+monobit.storage.formats.pcpaint - ChiWriter, GRASP, PCPaint, FONTRIX (for IBM) font files
 
 (c) 2022--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 
-from ..storage import loaders, savers
-from ..font import Font
-from ..glyph import Glyph
-from ..raster import Raster
-from ..struct import little_endian as le
-from ..binary import ceildiv
-from ..magic import FileFormatError
+from monobit.storage import loaders, savers, FileFormatError
+from monobit.core import Font, Glyph, Raster
+from monobit.base.struct import little_endian as le
+from monobit.base.binary import ceildiv
+
 from .raw import load_bitmap
 
 
 ###############################################################################
 # font formats claiming descent from/compatibility with FONTRIX for IBM
 # I have only found FONTRIX and its fonts for the Apple II
 # and they are similar but incompatible (header offsets are different)
```

### Comparing `monobit-0.42.2/monobit/formats/pdf.py` & `monobit-0.43.0/monobit/storage/formats/pdf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """
-monobit.formats.pdf - pdf chart output
+monobit.storage.formats.pdf - pdf chart output
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 
 try:
     import reportlab
     from reportlab.lib.units import mm
     from reportlab.pdfgen.canvas import Canvas
 except ImportError:
     reportlab = None
 
-from ..storage import savers
-from ..magic import FileFormatError
+from monobit.storage import savers, FileFormatError
 
 
 if reportlab:
 
     @savers.register(
         name='pdf',
         patterns=('*.pdf',),
```

### Comparing `monobit-0.42.2/monobit/formats/pkfont.py` & `monobit-0.43.0/monobit/storage/formats/pkfont.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 """
-monobit.formats.pkfont - TeX packed font font files
+monobit.storage.formats.pkfont - TeX packed font font files
 
 (c) 2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from itertools import count
 
-from ..storage import loaders, savers
-from ..font import Font
-from ..glyph import Glyph
-from ..raster import Raster
-from .. import struct
-from ..struct import big_endian as be, bitfield, sizeof
-from ..binary import ceildiv, align
-from ..properties import Props
-from ..magic import Regex
+from monobit.storage import loaders, savers, Regex
+from monobit.core import Font, Glyph, Raster
+from monobit.base import Props
+from monobit.base import struct
+from monobit.base.struct import big_endian as be, bitfield, sizeof
+from monobit.base.binary import ceildiv, align
 
 
 @loaders.register(
     name='pkfont',
     magic=(b'\xf7\x59',),
     # file name pattern is '{name}.{dpi}PK'
     patterns=(Regex(r'.+\.\d+pk'),),
```

### Comparing `monobit-0.42.2/monobit/formats/prebuilt.py` & `monobit-0.43.0/monobit/storage/formats/prebuilt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """
-monobit.formats.prebuilt - Adobe BE/LE Prebuilt Format
+monobit.storage.formats.prebuilt - Adobe BE/LE Prebuilt Format
 
 (c) 2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from itertools import cycle
 
-from ..struct import bitfield, little_endian as le, big_endian as be
-from ..properties import Props
-from ..storage import loaders, savers
-from ..font import Font
-from ..glyph import Glyph
-from ..magic import FileFormatError
-from ..taggers import tagmaps
+from monobit.base.struct import bitfield, little_endian as le, big_endian as be
+from monobit.base import Props
+from monobit.storage import loaders, savers, FileFormatError
+from monobit.core import Font, Glyph
+from monobit.encoding import encodings
 
 
 @loaders.register(
     name='prebuilt',
     patterns=('*.bepf', '*.lepf'),
 )
 def load_pf(instream):
@@ -292,11 +290,11 @@
             #  matrix.d / fixedScale == bdf SIZE.PointSize * (75 dpi) / SIZE.Yres
             # however the pf file doesn't include the point size or xres/yres separately
             # if we assume Yres == 75 dpi by definition,
             # d becomes point size and a gives us aspect ratio
             dpi=(75 * _matrix.a / _matrix.d, 75),
             point_size=_matrix.d / _FIXEDSCALE,
             encoding='latin-1' if pf_props.characterSetName == b'ISOLatin1CharacterSet' else '',
-        ).label(char_from=tagmaps['adobe'])
+        ).label(char_from=encodings['adobe'])
         for _matrix, _glyphs in zip(pf_props.matrices, strikes)
     )
     return fonts
```

### Comparing `monobit-0.42.2/monobit/formats/printshop.py` & `monobit-0.43.0/monobit/storage/formats/printshop.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 """
-monobit.formats.printshop - Broderbund's The Print Shop font files
+monobit.storage.formats.printshop - Broderbund's The Print Shop font files
 
 (c) 2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from itertools import count
 
-from ..storage import loaders, savers
-from ..font import Font
-from ..glyph import Glyph
-from ..raster import Raster
-from .. import struct
-from ..struct import little_endian as le
-from ..binary import ceildiv
+from monobit.storage import loaders, savers
+from monobit.core import Font, Glyph, Raster
+from monobit.base import struct
+from monobit.base.struct import little_endian as le
+from monobit.base.binary import ceildiv
 
 # offset 0
 _HEADER = le.Struct(
     bbx_width='uint8',
     bbx_height='uint8',
     unused='uint16',
 )
```

### Comparing `monobit-0.42.2/monobit/formats/psf.py` & `monobit-0.43.0/monobit/storage/formats/psf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """
-monobit.formats.psf - PC Screen Font format
+monobit.storage.formats.psf - PC Screen Font format
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 
-from ..binary import ceildiv
-from ..struct import bitfield, flag, little_endian as le
-from ..storage import loaders, savers
-from ..font import Font
-from ..glyph import Glyph
-from ..magic import FileFormatError
+from monobit.base.binary import ceildiv
+from monobit.base.struct import bitfield, flag, little_endian as le
+from monobit.storage import loaders, savers, FileFormatError
+from monobit.core import Font, Glyph
 
 from .raw import load_bitmap
 
 
 # PSF formats:
 # https://www.win.tue.nl/~aeb/linux/kbd/font-formats-1.html
```

### Comparing `monobit-0.42.2/monobit/formats/raw.py` & `monobit-0.43.0/monobit/storage/formats/raw.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """
-monobit.formats.raw - raw binary font files
+monobit.storage.formats.raw - raw binary font files
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from itertools import zip_longest
 from pathlib import PurePath
 
-from ..binary import ceildiv, bytes_to_bits
-from ..storage import loaders, savers
-from ..font import Font
-from ..glyph import Glyph
-from ..raster import Raster, NOT_SET
-from ..magic import FileFormatError, Regex, Glob
-from ..basetypes import Coord
+from monobit.base.binary import ceildiv, bytes_to_bits
+from monobit.storage import loaders, savers
+from monobit.storage import FileFormatError, Regex, Glob
+from monobit.core import Font, Glyph, Raster
+from monobit.base import Coord, NOT_SET
+
 
 # patterns
 
 # CHET .814 - http://fileformats.archiveteam.org/wiki/CHET_font
 
 # .udg: https://www.seasip.info/Unix/PSF/Amstrad/UDG/index.html
 
@@ -46,28 +45,29 @@
     patterns=('*.814', '.car', '*.64c', '*.udg', '*.ch8', _FXX),
 )
 def load_binary(
         instream, *,
         cell:Coord=NOT_SET, count:int=-1, offset:int=0, padding:int=0,
         align:str='left', byte_order:str='row-major',
         strike_count:int=1, strike_bytes:int=-1,
-        first_codepoint:int=0
+        first_codepoint:int=0, invert:bool=False
     ):
     """
     Load character-cell font from binary bitmap.
 
     cell: size X,Y of character cell (default: 8x8 or determine from filename)
     offset: number of bytes in file before bitmap starts (default: 0)
     padding: number of bytes between encoded glyph rows (default: 0)
     count: number of glyphs to extract (<= 0 means all; default: all)
     strike_count: number of glyphs in glyph row (<=0 for all; default: 1)
     strike_bytes: strike width in bytes (<=0 means as many as needed to fit the glyphs; default: as needed)
     align: alignment of strike row ('left' for most-, 'right' for least-significant; 'bit' for bit-aligned; default: 'left')
     byte_order: 'row-major' (default) or 'column-major' byte order (affect cell sizes wider than 8 pixels)
     first_codepoint: first code point in bitmap (default: 0)
+    invert: use 0-bits as ink, 1-bits as paper (default: False)
     """
     # determine cell size from filename, if not given
     if cell is NOT_SET:
         if Glob('*.814').fits(instream):
             width, height = 8, 14
         elif Glob('*.car').fits(instream):
             width, height = 16, 16
@@ -86,15 +86,15 @@
     else:
         width, height = cell
     # get through the offset
     instream.read(offset)
     return load_bitmap(
         instream, width, height, count, padding, align,
         strike_count, strike_bytes, first_codepoint,
-        byte_order=byte_order
+        byte_order=byte_order, invert=invert
     )
 
 @savers.register(linked=load_binary)
 def save_binary(
         fonts, outstream, *,
         strike_count:int=1, align:str='left', padding:int=0,
     ):
@@ -114,31 +114,33 @@
 
 ###############################################################################
 # bitmap reader
 
 def load_bitmap(
         instream, width, height, count=-1, padding=0, align='left',
         strike_count=1, strike_bytes=-1, first_codepoint=0, *,
-        byte_order='row-major',
+        byte_order='row-major', invert=False,
     ):
     """Load fixed-width font from bitmap."""
     data, count, cells_per_row, bytes_per_row, nrows = _extract_data_and_geometry(
         instream, width, height, count, padding, strike_count, strike_bytes,
     )
     cells = _extract_cells(
         data, width, height, align, cells_per_row, bytes_per_row, nrows,
         byte_order=byte_order,
     )
     # reduce to given count, if exceeded
     cells = cells[:count]
     # assign codepoints
-    glyphs = tuple(
+    glyphs = (
         Glyph(_cell, codepoint=_index)
         for _index, _cell in enumerate(cells, first_codepoint)
     )
+    if invert:
+        glyphs = (_g.invert() for _g in glyphs)
     return Font(glyphs)
 
 
 def _extract_data_and_geometry(
         instream, width, height, count=-1, padding=0,
         strike_count=1, strike_bytes=-1,
     ):
```

### Comparing `monobit-0.42.2/monobit/formats/signum.py` & `monobit-0.43.0/monobit/storage/formats/signum.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 """
-monobit.formats.signum - Signum! 2 editor and printer font formats
+monobit.storage.formats.signum - Signum! 2 editor and printer font formats
 
 (c) 2022--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from pathlib import Path
 
-from ..struct import big_endian as be
-from ..storage import loaders, savers
-from ..font import Font
-from ..glyph import Glyph
-from ..raster import Raster
-from ..magic import FileFormatError
-from ..binary import ceildiv, bytes_to_bits
+from monobit.base.struct import big_endian as be
+from monobit.storage import loaders, savers, FileFormatError
+from monobit.core import Font, Glyph, Raster
+from monobit.base.binary import ceildiv, bytes_to_bits
 
 
 # editor font
 _E24_MAGIC = b'eset0001'
 # printer fonts
 _L30_MAGIC = b'ls300001'
 _P24_MAGIC = b'ps240001'
```

### Comparing `monobit-0.42.2/monobit/formats/svg.py` & `monobit-0.43.0/monobit/storage/formats/vector/svg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 """
-monobit.formats.svg - svg writer for vector fonts
+monobit.storage.formats.vector.svg - svg writer for vector fonts
 
 (c) 2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import re
 import logging
 from math import ceil
 import xml.etree.ElementTree as etree
 
-from ..storage import loaders, savers
-from ..magic import FileFormatError
-from ..vector import StrokePath
-from ..font import Font
-from ..glyph import Glyph
-from ..properties import Props, reverse_dict
-from .windows import WEIGHT_MAP, WEIGHT_REVERSE_MAP
+from monobit.storage import loaders, savers, FileFormatError
+from monobit.base import Props, reverse_dict
+from monobit.core import Font, Glyph, StrokePath
+
+from ..common import WEIGHT_MAP, WEIGHT_REVERSE_MAP
 
 
 _STYLE_MAP = {
     'normal': 'roman',
     'italic': 'italic',
     'oblique': 'oblique'
 }
 _STYLE_REVERSE_MAP = reverse_dict(_STYLE_MAP)
 
+# tag used for 'missing' glyph
 DEFAULT_NAME = 'missing'
 
 
 @loaders.register(
     name='svg',
     patterns=('*.svg',),
     magic=(
```

### Comparing `monobit-0.42.2/monobit/formats/vfont.py` & `monobit-0.43.0/monobit/storage/formats/vfont.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """
-monobit.formats.vfont - BSD/SunOS vfont format
+monobit.storage.formats.vfont - BSD/SunOS vfont format
 
 (c) 2022--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from itertools import accumulate
 
-from ..struct import bitfield, little_endian as le, big_endian as be
-from ..properties import Props
-from ..storage import loaders, savers
-from ..font import Font
-from ..glyph import Glyph
-from ..magic import FileFormatError
+from monobit.base.struct import bitfield, little_endian as le, big_endian as be
+from monobit.base import Props
+from monobit.storage import loaders, savers, FileFormatError
+from monobit.core import Font, Glyph
 
 
 @loaders.register(
     name='vfont',
     magic=(b'\x01\x1e', b'\x1e\x01'),
     patterns=('*.vfont',),
 )
@@ -163,17 +161,15 @@
 
 ###############################################################################
 # writer
 
 def _convert_to_vfont(font):
     """Convert monobit font to vfont properties and glyphs."""
     # ensure codepoint values are set if possible
-    font = font.label(codepoint_from=font.encoding)
-    font = font.subset(_VFONT_RANGE)
-    font = _make_contiguous(font)
+    font = font.resample(_VFONT_RANGE, missing='empty')
     # set glyph properties
     glyphs = tuple(
         _glyph.modify(
             vfont=dict(
                 left=-_glyph.left_bearing,
                 right=_glyph.width+_glyph.left_bearing,
                 down=-_glyph.shift_up,
@@ -209,17 +205,7 @@
         **vfont_props
     )
     outstream.write(
         bytes(header)
         + bytes(dispatch)
         + bitmap
     )
-
-
-def _make_contiguous(font):
-    """Get contiguous range, fill gaps with empties."""
-    glyphs = tuple(
-        font.get_glyph(codepoint=_cp, missing='empty').modify(codepoint=_cp)
-        for _cp in _VFONT_RANGE
-    )
-    font = font.modify(glyphs)
-    return font
```

### Comparing `monobit-0.42.2/monobit/formats/xerox.py` & `monobit-0.43.0/monobit/storage/formats/xerox.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 """
-monobit.formats.alto - Xerox Alto .AL screen font format
+monobit.storage.formats.alto - Xerox Alto .AL screen font format
 
 (c) 2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from itertools import count
 
-from ..struct import bitfield, flag, big_endian as be
-from ..storage import loaders, savers
-from ..magic import FileFormatError
-from ..properties import Props
-from ..font import Font
-from ..glyph import Glyph
-from ..raster import Raster
-from ..labels import Tag
+from monobit.base.struct import bitfield, flag, big_endian as be
+from monobit.storage import loaders, savers, FileFormatError
+from monobit.base import Props
+from monobit.core import Font, Glyph, Raster, Tag
 
 
 @loaders.register(
     name='alto',
     patterns=('*.al',),
 )
 def load_alto(instream):
```

### Comparing `monobit-0.42.2/monobit/formats/mac/__init__.py` & `monobit-0.43.0/monobit/storage/formats/apple/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 """
-monobit.formats.mac - Mac OS fonts
+monobit.storage.formats.apple - Mac OS and other Apple font formats
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 
-from ...storage import loaders, savers
+from monobit.storage import loaders, savers
+from monobit.encoding import EncodingName
+from monobit.base import NOT_SET
+from monobit.base import import_all
+
+import_all(__name__)
 
 from .dfont import parse_resource_fork, save_dfont
 from .nfnt import extract_nfnt, convert_nfnt, create_nfnt
 from .lisa import _load_lisa
 from .iigs import _load_iigs, _save_iigs
 
 
@@ -24,20 +29,24 @@
 def load_mac_dfont(instream):
     """Load font from MacOS resource fork or data-fork resource."""
     data = instream.read()
     return parse_resource_fork(data)
 
 
 @savers.register(linked=load_mac_dfont)
-def save_mac_dfont(fonts, outstream, resource_type:str='NFNT', family_id:int=None):
+def save_mac_dfont(
+        fonts, outstream, resource_type:str='NFNT', family_id:int=None,
+        resample_encoding:EncodingName=NOT_SET,
+    ):
     """Save font to MacOS resource fork or data-fork resource.
 
     resource_type: type of resource to store font in. One of `sfnt`, `NFNT`.
+    resample_encoding: encoding to use for NFNT resources. Must be one of the `mac-` encodings. Default: use font's encoding.
     """
-    save_dfont(fonts, outstream, resource_type)
+    save_dfont(fonts, outstream, resource_type, resample_encoding)
 
 
 @loaders.register(
     name='nfnt',
     # \x90\0 is not a formal signature, but the most common set of FONT_TYPE flags
     # the \x80 sigs are LISA compressed NFNTs
     magic=(b'\x90\0', b'\xb0\0', b'\x90\x80', b'\xb0\x80'),
@@ -67,40 +76,48 @@
 )
 def load_iigs(instream):
     """Load a IIgs font."""
     return _load_iigs(instream)
 
 
 @savers.register(linked=load_iigs)
-def save_iigs(fonts, outstream, version:int=None):
+def save_iigs(
+        fonts, outstream, version:int=None, resample_encoding:EncodingName=NOT_SET,
+    ):
     """
     Write font to a IIgs font file.
 
     version: IIgs font format version (0x101, 0x105). Default: 0x101 unless needed for bitmap size.
+    resample_encoding: encoding to use for NFNT resources. Must be one of the `mac-` encodings. Default: use font's encoding.
     """
     if len(fonts) > 1:
         logging.warning('IIgs font file can only store one font.')
     font = fonts[0]
-    _save_iigs(outstream, font, version=version)
+    _save_iigs(
+        outstream, font, version=version, resample_encoding=resample_encoding
+    )
 
 
 @savers.register(linked=load_nfnt)
 def save_nfnt(
         fonts, outstream,
         create_width_table:bool=True,
         create_height_table:bool=False,
+        resample_encoding:EncodingName=NOT_SET,
     ):
     """
     Write font to a bare FONT/NFNT resource.
 
     create_width_table: include a fractional glyph-width table in the resource (default: True)
     create_height_table: include an image-height table in the resource (default: False)
+    resample_encoding: encoding to use for NFNT resources. Must be one of the `mac-` encodings. Default: use font's encoding.
     """
     if len(fonts) > 1:
         logging.warning('NFNT resource can only store one font.')
     font = fonts[0]
     data, _, _ = create_nfnt(
         font, endian='big', ndescent_is_high=True,
         create_width_table=create_width_table,
         create_height_table=create_height_table,
+        resample_encoding=resample_encoding,
     )
     outstream.write(data)
```

### Comparing `monobit-0.42.2/monobit/formats/mac/dfont.py` & `monobit-0.43.0/monobit/storage/formats/apple/dfont.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """
-monobit.formats.mac.dfont - MacOS suitcases and resources
+monobit.storage.formats.apple.dfont - MacOS suitcases and resources
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from collections import Counter
 from itertools import accumulate
 from io import BytesIO
 
-from ...struct import big_endian as be
-from ...magic import FileFormatError
-from ...streams import Stream
-from ...properties import Props, reverse_dict
-from ...pack import Pack
+from monobit.base.struct import big_endian as be
+from monobit.storage import FileFormatError
+from monobit.storage import Stream
+from monobit.base import Props, reverse_dict
+from monobit.core import Pack
 
-from ..sfnt import load_sfnt, save_sfnt, MAC_ENCODING, STYLE_MAP
+from ..common import MAC_ENCODING, STYLE_MAP
+from ..sfnt import load_sfnt, save_sfnt
 from .nfnt import (
     extract_nfnt, convert_nfnt,
     subset_for_nfnt, convert_to_nfnt, nfnt_data_to_bytes, generate_nfnt_header
 )
 from .fond import extract_fond, convert_fond, create_fond
 
 
@@ -316,19 +317,20 @@
 # > (truetype) resource in the ‘bloc’ and ‘bdat’ tables. When this happens there are
 # > a series of dummy ‘NFNT’ resources in the resource file, one for each strike.
 # > Each resource is 26 bytes long (which means they contain the FontRec structure
 # > but no data tables) and are flagged by having rowWords set to 0. (I have
 # > determined this empirically, I have seen no documentation on the subject)
 
 
-def save_dfont(fonts, outstream, resource_type):
+def save_dfont(fonts, outstream, resource_type, resample_encoding):
     """
     Save font to MacOS resource fork or data-fork resource.
 
     resource_type: type of resource to store font in. One of `sfnt`, `NFNT`.
+    resample_encoding: encoding to use for NFNT resources. Must be one of the `mac-` encodings. Default: use font's encoding.
     """
     resource_type = resource_type.lower()
     if resource_type not in ('sfnt', 'nfnt'):
         raise ValueError(
             'Only saving to sfnt or NFNT resource currently supported'
         )
     resources = []
@@ -338,15 +340,15 @@
         font, *_ = fonts
         family_id = _get_family_id(font.family, font.encoding)
         resources.append(
             Props(type=b'sfnt', id=family_id, name='', data=sfnt_io.getvalue()),
         )
     # reduce fonts to what's storable in (stub) FOND/NFNT
     # we need a Pack for _group_families
-    fonts = Pack(subset_for_nfnt(_f) for _f in fonts)
+    fonts = Pack(subset_for_nfnt(_f, resample_encoding) for _f in fonts)
     for family_id, style_group in _group_families(fonts):
         i = 0
         for style_id, size_group in style_group:
             for font in size_group:
                 if resource_type == 'sfnt':
                     # create stub NFNT if the bitmaps are in an sfnt
                     nfnt_data = generate_nfnt_header(font, endian='big')
@@ -374,15 +376,15 @@
             ),
         )
     _write_resource_fork(outstream, resources)
 
 
 def _get_family_id(name, encoding):
     """Generate a resource id based on the font's properties."""
-    script_code = reverse_dict(MAC_ENCODING).get(encoding, _FALLBACK_ENCODING)
+    script_code = reverse_dict(MAC_ENCODING).get(str(encoding), _FALLBACK_ENCODING)
     return _hash_to_id(name, script=script_code)
 
 
 def _write_resource_fork(outstream, resources):
     """
     Write a Mac dfont/resource fork.
```

### Comparing `monobit-0.42.2/monobit/formats/mac/fond.py` & `monobit-0.43.0/monobit/storage/formats/apple/fond.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
-monobit.formats.mac.fond - Mac FOND font directory
+monobit.storage.formats.apple.fond - Mac FOND font directory
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from itertools import accumulate
 
-from ..sfnt import MAC_ENCODING, mac_style_name, to_postscript_name
-from ...binary import bytes_to_bits, align
-from ...struct import bitfield, big_endian as be, sizeof
-from ...glyph import Glyph
+from monobit.base.binary import bytes_to_bits, align
+from monobit.base.struct import bitfield, big_endian as be, sizeof
+from monobit.core import Glyph
+
+from ..common import MAC_ENCODING, mac_style_name, to_postscript_name
 
 
 ##############################################################################
 # FOND resource
 # https://developer.apple.com/library/archive/documentation/mac/Text/Text-269.html#MARKER-2-525
 
 _FFLAGS = be.Struct(
```

### Comparing `monobit-0.42.2/monobit/formats/mac/iigs.py` & `monobit-0.43.0/monobit/storage/formats/apple/iigs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
-monobit.formats.mac.iigs - Apple IIgs font file
+monobit.storage.formats.apple.iigs - Apple IIgs font file
 
 (c) 2023 Kelvin Sherlock
 licence: https://opensource.org/licenses/MIT
 
 modifications (c) 2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import io
 import logging
 
-from ...binary import bytes_to_bits, align
-from ...struct import bitfield, little_endian as le
-from ... import struct
-from ...storage import loaders, savers
-from ...font import Font, Coord
-from ...glyph import Glyph, KernTable
-from ...magic import FileFormatError
+from monobit.base.binary import bytes_to_bits, align
+from monobit.base.struct import bitfield, little_endian as le
+from monobit.base import struct
+from monobit.base import Coord
+from monobit.storage import loaders, savers
+from monobit.storage import FileFormatError
+from monobit.core import Font, Glyph, KernTable
 
 from .nfnt import convert_nfnt, extract_nfnt, create_nfnt
 from .dfont import NON_ROMAN_NAMES
 
 
 # IIgs font file is essentially a little-endian MacOS FONT resource,
 # without the resource, plus an extra header.
@@ -109,19 +109,20 @@
         decoration.append('outline')
     if header.style.shadow:
         decoration.append('shadow')
     properties['decoration'] = ' '.join(decoration);
     return font.modify(**properties).label()
 
 
-def _save_iigs(outstream, font, version=None):
+def _save_iigs(outstream, font, version, resample_encoding):
     """Save an Apple IIgs font file."""
     nfnt, owt_loc_high, fbr_extent = create_nfnt(
         font, endian='little', ndescent_is_high=False,
         create_width_table=False, create_height_table=False,
+        resample_encoding=resample_encoding,
     )
     # if offset > 32 bits, need to use iigs format v1.05
     if version is None:
         if owt_loc_high:
             version = 0x0105
         else:
             version = 0x0101
```

### Comparing `monobit-0.42.2/monobit/formats/mac/lisa.py` & `monobit-0.43.0/monobit/storage/formats/apple/lisa.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
-monobit.formats.mac.lisa - Apple Lisa fonts
+monobit.storage.formats.apple.lisa - Apple Lisa fonts
 
 (c) 2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 
-from ...struct import big_endian as be
-from ...binary import align
-from ...magic import FileFormatError
+from monobit.base.struct import big_endian as be
+from monobit.base.binary import align
+from monobit.storage import FileFormatError
 
 from .nfnt import extract_nfnt, convert_nfnt
 
 
 # https://www.kreativekorp.com/swdownload/lisa/AppleLisaFontFormat.pdf
 
 _LISA_HEADER = be.Struct(
```

### Comparing `monobit-0.42.2/monobit/formats/mac/nfnt.py` & `monobit-0.43.0/monobit/storage/formats/apple/nfnt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 """
-monobit.formats.mac.nfnt - Mac FONT/NFNT fonts
+monobit.storage.formats.apple.nfnt - Mac FONT/NFNT fonts
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 
 NFNT writer based on the Apple IIgs writer
 (c) 2023 Kelvin Sherlock
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from itertools import chain, accumulate
 
-from ...binary import bytes_to_bits
-from ...struct import bitfield, big_endian as be, little_endian as le
-from ...font import Font
-from ...glyph import Glyph, KernTable
-from ...magic import FileFormatError
-from ...labels import Char
-from ...encoding import charmaps
-from ...raster import Raster
-from ...properties import Props
+from monobit.base.binary import bytes_to_bits
+from monobit.base.struct import bitfield, big_endian as be, little_endian as le
+from monobit.core import Font, Glyph, KernTable, Char, Raster
+from monobit.storage import FileFormatError
+from monobit.encoding import EncodingName
+from monobit.base import Props
+from monobit.base import NOT_SET
 
 from .fond import fixed_to_float
+from ..common import MAC_ENCODING
 
 
+# normalised names so we can test with `in`
+MAC_ENCODING_NAMES = tuple(str(EncodingName(_name) for _name in MAC_ENCODING))
+
+# tag used for the 'missing' glyph
+MISSING_TAG = 'missing'
+
 ##############################################################################
 # NFNT/FONT resource
 
 # the Font Type Element
 # https://developer.apple.com/library/archive/documentation/mac/Text/Text-251.html#MARKER-9-442
 def font_type_struct(base):
     return base.Struct(
@@ -350,15 +355,15 @@
         )
     # codepoint labels
     labelled = [
         _glyph.modify(codepoint=(_codepoint,))
         for _codepoint, _glyph in enumerate(glyphs[:-1], start=fontrec.firstChar)
     ]
     # last glyph is the "missing" glyph
-    labelled.append(glyphs[-1].modify(tag='missing'))
+    labelled.append(glyphs[-1].modify(tag=MISSING_TAG))
     # drop undefined glyphs & their labels, so long as they're empty
     glyphs = tuple(
         _glyph for _glyph in labelled
         if (_glyph.wo_width != 0xff and _glyph.wo_offset != 0xff) or (_glyph.width and _glyph.height)
     )
     # drop mac glyph metrics
     # keep scalable_width
@@ -390,15 +395,15 @@
             }))
             for _glyph in glyphs
         )
     # store properties
     properties.update({
         # not overridable; also seems incorrect for system fonts
         #'spacing': 'monospace' if fontrec.fontType.fixed_width else 'proportional',
-        'default_char': 'missing',
+        'default_char': MISSING_TAG,
         'ascent': fontrec.ascent,
         'descent': fontrec.descent,
         'line_height': fontrec.ascent + fontrec.descent + fontrec.leading,
         'shift_up': -fontrec.descent,
         # remove the kerning table and encoding table now stored in glyphs
         'kerning_table': None,
         'encoding_table': None,
@@ -408,50 +413,52 @@
 
 
 
 ###############################################################################
 # NFNT writer
 
 def create_nfnt(
-        font, endian, ndescent_is_high, create_width_table, create_height_table
+        font, endian, ndescent_is_high, create_width_table, create_height_table,
+        resample_encoding,
     ):
     """Create NFNT/FONT resource."""
     # subset to characters storable in NFNT
-    font = subset_for_nfnt(font)
+    font = subset_for_nfnt(font, resample_encoding)
     nfnt_data = convert_to_nfnt(
         font, endian, ndescent_is_high, create_width_table, create_height_table
     )
     data = nfnt_data_to_bytes(nfnt_data)
     return data, nfnt_data.owt_loc_high, nfnt_data.fbr_extent
 
 
-def subset_for_nfnt(font):
+def subset_for_nfnt(font, resample_encoding):
     """Subset to glyphs storable in NFNT and append default glyph."""
-    font = font.label(codepoint_from=font.encoding)
-    resample = False
-    if font.encoding.startswith('mac') or font.encoding in ('raw', '', None):
+    default = font.get_default_glyph().modify(labels=(), tag=MISSING_TAG)
+    is_mac_encoding = str(EncodingName(font.encoding)) in MAC_ENCODING_NAMES
+    if (
+            resample_encoding is NOT_SET
+            and font.encoding and not is_mac_encoding
+            and not font.encoding in ('raw', 'ascii')
+        ):
+        resample_encoding = 'mac-roman'
+    if resample_encoding:
+        # NFNT can only store encodings from a pre-defined list of 'scripts'
+        # for fonts with other encodings, get glyphs corresponding to mac-roman
+        font = font.resample(encoding=resample_encoding, missing=None)
+    if font.encoding == 'ascii':
+        font = font.subset(range(0, 128))
+    else:
         # it's not clear to me if/how NFNT resources are used for MBCS
         # currently we just use the single-byte sector
         # this affects mac-japanese, mac-korean which have multibyte codepoints
-        labels = tuple(range(0, 256))
-    elif font.encoding == 'ascii':
-        labels = tuple(range(0, 128))
-    else:
-        resample = True
-        # NFNT can only store encodings from a pre-defined list of 'scripts'
-        # for fonts with other encodings, get glyphs corresponding to mac-roman
-        font = font.label()
-        labels = tuple(Char(_c) for _i, _c in sorted(charmaps['mac-roman'].mapping.items()))
-    subfont = font.subset(labels=labels)
-    if not subfont.glyphs:
+        font = font.subset(range(0, 256))
+    if not font.glyphs:
         raise FileFormatError('No suitable characters for NFNT font')
-    glyphs = [*subfont.glyphs, font.get_default_glyph().modify(labels=(), tag='missing')]
-    font = font.modify(glyphs, encoding=None)
-    if resample:
-        font = font.label(codepoint_from='mac-roman', overwrite=True)
+    # add the default glyph at the end
+    font = font.append(glyphs=(default,))
     return font
 
 
 def _normalize_glyph(g, ink_bounds):
     """
     Trim the horizontal to glyph's ink bounds
     and expand the vertical to font's ink bounds
```

### Comparing `monobit-0.42.2/monobit/formats/os2/gpifont.py` & `monobit-0.43.0/monobit/storage/formats/fon/os2/gpifont.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-monobit.formats.os2.gpifont - OS/2 GPI font resource parser
+monobit.storage.formats.fon.os2.gpifont - OS/2 GPI font resource parser
 
 (c) 2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 
 
 this is mostly ported code from gpifont.c and gpifont.h
 - http://www.altsan.org/programming/os2font_src.zip
@@ -14,20 +14,19 @@
 >  (C) 2012 Alexander Taylor
 >  This code is placed in the public domain.
 >
 """
 
 import logging
 
-from ...magic import FileFormatError
-from ...glyph import Glyph
-from ...font import Font
-from ...properties import Props
-from ...struct import little_endian as le, bitfield
-from ...binary import ceildiv
+from monobit.storage import FileFormatError
+from monobit.core import Font, Glyph
+from monobit.base import Props
+from monobit.base.struct import little_endian as le, bitfield
+from monobit.base.binary import ceildiv
 
 
 GPI_MAGIC = b'\xfe\xff\xff\xff'
 
 
 # Text signatures for standard OS/2 bitmap fonts.
 OS2FNT_SIGNATURE = "OS/2 FONT"
@@ -458,37 +457,40 @@
         b'' if not _c.ulOffset else pBuffer[_c.ulOffset : _c.ulOffset+_uw*cy]
         for _c, _uw in zip(pFont.pChars, usWidths)
     )
     #
     # read optional tables (kerning, panose)
     #
     ofs += pFont.pFontDef.ulSize
-    pRecord = GENERICRECORD.from_bytes(pBuffer, ofs)
-    if pFont.pMetrics.usKerningPairs and pRecord.Identity == SIG_OS2KERN:
-        pFont.pKerning = OS2KERNPAIRTABLE.from_bytes(pBuffer, ofs)
-        # Advance to the next record (whether OS2ADDMETRICS or OS2FONTEND).
-        # This is a guess; since the actual format, and thus size, of the
-        # kerning information is unclear (see remarks in gpifont.h), there is
-        # no guarantee this will work.  Fortunately, we've already parsed the
-        # important stuff.
-        ofs += (
-            OS2KERNPAIRTABLE.size
-            + pFont.pMetrics.usKerningPairs * OS2KERNINGPAIRS.size
-        )
-        pRecord = GENERICRECORD.from_bytes(pBuffer, ofs)
-    if pRecord.Identity == SIG_OS2ADDMETRICS:
-        pFont.pPanose = OS2ADDMETRICS.from_bytes(pBuffer, ofs)
-        ofs += pRecord.ulSize
+    if ofs >= len(pBuffer):
+        logging.debug('Offset to optional kerning table exceeds buffer length')
+    else:
         pRecord = GENERICRECORD.from_bytes(pBuffer, ofs)
-    # We set the pointer to the end signature, but there's really no need to
-    # use it for anything.  We check the Identity field to make sure it's
-    # valid (if we did miscalculate the kern table size above, then it could
-    # well be wrong) before setting the pointer.
-    if pRecord.Identity == SIG_OS2FONTEND:
-        pFont.pEnd = OS2FONTEND.from_bytes(pBuffer, ofs)
+        if pFont.pMetrics.usKerningPairs and pRecord.Identity == SIG_OS2KERN:
+            pFont.pKerning = OS2KERNPAIRTABLE.from_bytes(pBuffer, ofs)
+            # Advance to the next record (whether OS2ADDMETRICS or OS2FONTEND).
+            # This is a guess; since the actual format, and thus size, of the
+            # kerning information is unclear (see remarks in gpifont.h), there is
+            # no guarantee this will work.  Fortunately, we've already parsed the
+            # important stuff.
+            ofs += (
+                OS2KERNPAIRTABLE.size
+                + pFont.pMetrics.usKerningPairs * OS2KERNINGPAIRS.size
+            )
+            pRecord = GENERICRECORD.from_bytes(pBuffer, ofs)
+        if pRecord.Identity == SIG_OS2ADDMETRICS:
+            pFont.pPanose = OS2ADDMETRICS.from_bytes(pBuffer, ofs)
+            ofs += pRecord.ulSize
+            pRecord = GENERICRECORD.from_bytes(pBuffer, ofs)
+        # We set the pointer to the end signature, but there's really no need to
+        # use it for anything.  We check the Identity field to make sure it's
+        # valid (if we did miscalculate the kern table size above, then it could
+        # well be wrong) before setting the pointer.
+        if pRecord.Identity == SIG_OS2FONTEND:
+            pFont.pEnd = OS2FONTEND.from_bytes(pBuffer, ofs)
     return pFont
 
 
 def parse_os2_font_directory(data):
     """
     Parse a font directory resource, return as font directory entries.
     Return an empty tuple if parsing failed.
```

### Comparing `monobit-0.42.2/monobit/formats/os2/lx.py` & `monobit-0.43.0/monobit/storage/formats/fon/os2/lx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-monobit.formats.os2.lx - read OS/2 LX containers
+monobit.storage.formats.fon.os2.lx - read OS/2 LX containers
 
 (c) 2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 
 
 this is mostly ported code from gpifont.c and os2res.h
 - http://www.altsan.org/programming/os2font_src.zip
@@ -14,16 +14,16 @@
 >  (C) 2012 Alexander Taylor
 >  This code is placed in the public domain.
 >
 """
 
 import logging
 
-from ...magic import FileFormatError
-from ...struct import little_endian as le
+from monobit.storage import FileFormatError
+from monobit.base.struct import little_endian as le
 
 from .gpifont import parse_os2_font_directory
 
 
 # from os2res.h
 
 # OS/2 resource types that we're interested in.
@@ -205,15 +205,15 @@
 
     This algorithm was derived from public-domain Pascal code by Veit
     Kannegieser (based on previous work by Max Alekseyev).
     """
     cbPage = len(pBuf)
     if cbPage > 4096:
         return pBuf
-    ofIn  = 0;
+    ofIn = 0
     abOut = bytearray()
     while True:
         usReps = pBuf[ofIn] | (pBuf[ofIn+1] << 8)
         if not usReps:
             break
         ofIn += 2
         usLen = pBuf[ofIn] | (pBuf[ofIn+1] << 8)
@@ -236,15 +236,15 @@
 
     This algorithm was derived from public-domain Pascal-and-x86-assembly
     code by Veit Kannegieser (based on previous work by Max Alekseyev).
     """
     cbPage = len(pBuf)
     if cbPage > 4096:
         return pBuf
-    ofIn  = 0
+    ofIn = 0
     abOut = bytearray()
     while True:
         ulControl = int(le.uint16.from_bytes(pBuf, ofIn))
         # Bits 1 & 0 hold the case flag (0-3); the interpretation of the
         # remaining bits depend on the flag value.
         case_flag = ulControl & 0x3
         if case_flag == 0:
@@ -278,35 +278,35 @@
             ulLen = (( ulControl >> 4 ) & 0x7 ) + 3
             _copy_byte_seq(abOut, -((ulControl >> 7) & 0x1FF), ulLen)
         elif case_flag == 2:
             # bits 15.. 4     = backwards reference
             # bits  3.. 2  +3 = length
             ulLen = (( ulControl >> 2 ) & 0x3 ) + 3
             _copy_byte_seq(abOut, -((ulControl >> 4) & 0xFFF), ulLen)
-            ofIn  += 2
+            ofIn += 2
         elif case_flag == 3:
             ulControl = int(le.uint32.from_bytes(pBuf, ofIn))
             # bits 23..21  = ?
             # bits 20..12  = backwards reference
             # bits 11.. 6  = length2
             # bits  5.. 2  = length1
             # block copy (length1) bytes
             ulLen = (ulControl >> 2) & 0xF
             # memcpy( abOut + ofOut, pBuf + ofIn + 3, ulLen );
             abOut.extend(pBuf[ofIn+3 : ofIn+3+ulLen])
-            ofIn  += ulLen + 3
+            ofIn += ulLen + 3
             # copy (length2) bytes from previously-unpacked data
             ulLen = (ulControl >> 6) & 0x3F
             _copy_byte_seq(abOut, -((ulControl >> 12) & 0xFFF), ulLen)
         if ofIn >= cbPage:
             break
     # It seems that the unpacked data will always be 4096 bytes, except for
     # the final page (which will be taken care of when the caller uses the
     # total object length to read the concatenated buffer).
-    return bytes(abOut)
+    return bytes(abOut).ljust(4096, b'\0')
 
 
 def _copy_byte_seq(target, source_offset, count):
     """
     Perform a byte-over-byte iterative copy from one byte array into another,
     or from one point to another within the same array.  Used by LXUnpack2().
     Note that memcpy() does not work for this purpose, because the source and
```

### Comparing `monobit-0.42.2/monobit/formats/os2/ne.py` & `monobit-0.43.0/monobit/storage/formats/fon/os2/ne.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
-monobit.formats.os2.ne - read OS/2 NE containers
+monobit.storage.formats.fon.os2.ne - read OS/2 NE containers
 
 (c) 2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 
-from ...magic import FileFormatError
-from ...struct import little_endian as le
+from monobit.storage import FileFormatError
+from monobit.base.struct import little_endian as le
+
 from ..windows.ne import NE_HEADER
 from .gpifont import parse_os2_font_directory
 
 # resource ids
 OS2RES_FONTDIR = 6
 OS2RES_FONTFACE = 7
```

### Comparing `monobit-0.42.2/monobit/formats/sfnt/sfnt.py` & `monobit-0.43.0/monobit/storage/formats/sfnt/sfnt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 """
-monobit.formats.sfnt - TrueType/OpenType and related formats
+monobit.storage.formats.sfnt - TrueType/OpenType and related formats
 
 (c) 2022--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import sys
 import logging
 import json
 import math
 import re
 from unicodedata import bidirectional
 
+from monobit.base import Props
+from monobit.core import Font, Glyph, Raster, Tag, Char, Codepoint
+from monobit.storage import loaders, savers
+from monobit.storage import FileFormatError
+
 from . import fonttools
 from .fonttools import check_fonttools
-
-from ...properties import Props
-from ...font import Font
-from ...glyph import Glyph
-from ...raster import Raster
-from ...labels import Tag, Char, Codepoint
-from ...storage import loaders, savers
-from ...magic import FileFormatError
-from ..windows import WEIGHT_MAP, CHARSET_MAP
+from ..common import WEIGHT_MAP, CHARSET_MAP, MAC_ENCODING, STYLE_MAP, mac_style_name
 
 
 # errors that invalidate only one strike or resource, not the whole file
 
 class ResourceFormatError(FileFormatError):
     """Unsupported parameters in resource."""
 
@@ -113,55 +110,14 @@
     load_sfnt = check_fonttools
     load_collection = check_fonttools
 
 
 ###############################################################################
 # common encoding tables
 
-# shared with mac
-
-# based on:
-# [1] Apple Technotes (As of 2002)/te/te_02.html
-# [2] https://developer.apple.com/library/archive/documentation/mac/Text/Text-367.html#HEADING367-0
-MAC_ENCODING = {
-    0: 'mac-roman',
-    1: 'mac-japanese',
-    2: 'mac-trad-chinese',
-    3: 'mac-korean',
-    4: 'mac-arabic',
-    5: 'mac-hebrew',
-    6: 'mac-greek',
-    7: 'mac-cyrillic', # [1] russian
-    # 8: [2] right-to-left symbols
-    9: 'mac-devanagari',
-    10: 'mac-gurmukhi',
-    11: 'mac-gujarati',
-    12: 'mac-oriya',
-    13: 'mac-bengali',
-    14: 'mac-tamil',
-    15: 'mac-telugu',
-    16: 'mac-kannada',
-    17: 'mac-malayalam',
-    18: 'mac-sinhalese',
-    19: 'mac-burmese',
-    20: 'mac-khmer',
-    21: 'mac-thai',
-    22: 'mac-laotian',
-    23: 'mac-georgian',
-    24: 'mac-armenian',
-    25: 'mac-simp-chinese', # [1] maldivian
-    26: 'mac-tibetan',
-    27: 'mac-mongolian',
-    28: 'mac-ethiopic', # [2] == geez
-    29: 'mac-centraleurope', # [1] non-cyrillic slavic
-    30: 'mac-vietnamese',
-    31: 'mac-sindhi', # [2] == ext-arabic
-    #32: [1] [2] 'uninterpreted symbols'
-}
-
 WIN_ENCODING = {
     # Symbol, but apparently not windows-symbol but any undefined encoding
     0: '',
     1: 'utf-16le', # unicode bmp
     2: 'ms932', # shift-jis
     3: 'ms936', # PRC
     4: 'ms950', # Big-5
@@ -188,14 +144,16 @@
     # legacy windows charset value
     4: CHARSET_MAP,
 }
 
 ###############################################################################
 # sfnt resource reader
 
+NOTDEF_NAME = '.notdef'
+
 # tags we will decompile and process
 _TAGS = (
     # check `maxp` first to catch any assertion errors on decompile
     'maxp',
     # core bitmap tables
     'head', 'bhed',
     'EBLC', 'bloc',
@@ -341,23 +299,23 @@
         try:
             props = _convert_props(sfnt, i_strike)
             glyphs = _convert_glyphs(
                 sfnt, i_strike, props._hfupp, props._vfupp, unitable, enctable
             )
             del props._hfupp
             del props._vfupp
-            # disabled - if we remove tags we break kerning (can label() adjust kerning too?)
-            # # remove temporary names created by fontTools
-            # # if there's no post table or it is empty
-            # if not sfnt.post or sfnt.post.formatType == 3.0:
-            #     glyphs = (_g.modify(tag=None) if _g.char else _g for _g in glyphs)
-            fonts.append(Font(
+            font = Font(
                 glyphs, source_format=source_format, encoding=encoding or None,
                 **vars(props)
-            ))
+            )
+            # remove temporary names created by fontTools
+            # if there's no post table or it is empty
+            if not sfnt.post or sfnt.post.formatType == 3.0:
+                font = font.label(tag_from=None)
+            fonts.append(font)
         except StrikeFormatError:
             pass
     return fonts
 
 
 def _convert_props(sfnt, i_strike):
     """Build font properties from sfnt data."""
@@ -693,31 +651,14 @@
     # anyway, which way is the 'ascent', left or right?
     return props
 
 
 ###############################################################################
 # 'head' or 'bhed' table
 
-# interpretation of head.macStyle flags
-STYLE_MAP = {
-    0: 'bold',
-    1: 'italic',
-    2: 'underline',
-    3: 'outline',
-    4: 'shadow',
-    5: 'condensed',
-    6: 'extended',
-}
-
-def mac_style_name(font_style):
-    """Get human-readable representation of font style."""
-    return ' '.join(
-        _tag for _bit, _tag in STYLE_MAP.items() if font_style & (1 << _bit)
-    )
-
 def _convert_head_props(head):
     """Convert font properties from head/bhed table."""
     if not head:
         return Props()
     props = Props(
         revision=head.fontRevision,
         style=mac_style_name(head.macStyle) or None,
@@ -899,15 +840,15 @@
             word_boundary=Char(chr(os_2.usBreakChar)),
         )
         # > This is the Unicode code point, in UTF-16 encoding, of a character
         # > that can be used for a default glyph if a requested character is not
         # > supported in the font. If the value of this field is zero,
         # > glyph ID 0 is to be used for the default character.
         if props.default_char == Char('\0'):
-            props.default_char = Tag('.notdef')
+            props.default_char = Tag(NOTDEF_NAME)
     return props
 
 
 ###############################################################################
 # 'post' table
 
 def _convert_post_props(post, vert_fu_p_pix):
```

### Comparing `monobit-0.42.2/monobit/formats/sfnt/sfnt_writer.py` & `monobit-0.43.0/monobit/storage/formats/sfnt/sfnt_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
-monobit.formats.sfnt_writer - TrueType/OpenType and related formats (writer)
+monobit.storageformats.sfnt_writer - TrueType/OpenType and related formats (writer)
 
 (c) 2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 
-from ...glyph import Glyph
-from ...binary import ceildiv
-from ...storage import loaders, savers
-from ...properties import reverse_dict
-from .sfnt import WEIGHT_MAP, SETWIDTH_MAP, check_fonttools
+from monobit.core import Glyph
+from monobit.core import Tag
+from monobit.base.binary import ceildiv
+from monobit.storage import loaders, savers
+from monobit.base import reverse_dict
+from monobit.base import to_number
+
+from .sfnt import WEIGHT_MAP, SETWIDTH_MAP, NOTDEF_NAME, check_fonttools
 from .sfnt import load_sfnt, load_collection
-from ...labels import Tag
-from ...taggers import CodepointTagger
-from ...basetypes import to_number
+from ..common import to_postscript_name
 
 from . import fonttools
 from .fonttools import check_fonttools
 
 if fonttools.loaded:
     from .fonttools import (
         _setup_kern_table,
@@ -88,15 +89,15 @@
 EBSC_SIZES = (*range(8, 26), 30, 32, 33, 40)
 
 
 def _label_to_utf16(font, label, default):
     """Convert a glyph label to a UTF-16 codepoint, if possible; 0 if not."""
     try:
         utf16 = ord(font.get_glyph(label).char)
-    except KeyError:
+    except (KeyError, TypeError):
         utf16 = default
     else:
         if utf16 > 0x1000:
             utf16 = default
     return utf16
 
 
@@ -138,25 +139,14 @@
         usBreakChar=_label_to_utf16(font, font.word_boundary, 0x20),
         # vendor ID - can be left blank (four spaces)
         achVendID=b'    ',
     )
     return props
 
 
-def to_postscript_name(name):
-    """Postscript name must be printable ascii, no [](){}<>/%, max 63 chars."""
-    ps_name = ''.join(
-        _c if _c.isalnum() and _c.isascii() else '-'
-        for _c in name
-    )
-    ps_name = ps_name[:63]
-    # expected to be Title-Cased (at least on Mac, see FontForge code comments)
-    return ps_name.title()
-
-
 def _convert_to_name_props(font):
     """Convert font properties to `name` table."""
     # `name` table should only store x.y version numbers
     # while font.revision could be any string
     try:
         version_number = to_number(font.revision)
         extra = ''
@@ -241,15 +231,15 @@
 
 def _convert_to_cmap_props(glyphs):
     """Convert glyph properties to `cmap` table."""
     return {
         ord(_g.char): _name
         for _name, _g in glyphs.items()
         # .notdef should not be mapped  in cmap
-        if _g.char and _name != '.notdef'
+        if _g.char and _name != NOTDEF_NAME
     }
 
 
 def _convert_to_kern_props(font, glyphs, _to_funits):
     """Convert kerning values to `kern` table."""
     kern_table = {}
     for tag, glyph in glyphs.items():
@@ -423,15 +413,15 @@
     # note that x and y ppem are equal - if not, fontforge rejects the bitmap
     def _to_funits(pixel_amount):
         return ceildiv(pixel_amount * funits_per_em, font.pixel_size)
 
     check_fonttools()
     font, default = _prepare_for_sfnt(font, glyph_names)
     # get the storable glyphs
-    glyphnames = ('.notdef', *(_t.value for _t in font.get_tags()))
+    glyphnames = (NOTDEF_NAME, *(_t.value for _t in font.get_tags()))
     glyphs = {
         _name: font.get_glyph(tag=_name, missing=default)
         for _name in glyphnames
     }
     # build font object
     fb = fonttools.FontBuilder(funits_per_em, isTTF=True)
     fb.setupGlyphOrder(glyphnames)
```

### Comparing `monobit-0.42.2/monobit/formats/sfnt/fonttools/E_B_S_C_.py` & `monobit-0.43.0/monobit/storage/formats/sfnt/fonttools/E_B_S_C_.py`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/monobit/formats/sfnt/fonttools/__init__.py` & `monobit-0.43.0/monobit/storage/formats/sfnt/fonttools/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,25 @@
+"""
+monobit.storage.formats.sfnt.fonttools - fontTools interface and extensions
+
+(c) 2023 Rob Hagemans
+licence: https://opensource.org/licenses/MIT
+"""
+
 from importlib.resources import files
 from pathlib import Path
 
 try:
     from fontTools import ttLib
     loaded = True
 except ImportError:
     ttLib = None
     loaded = False
 
-from ....magic import FileFormatError
+from monobit.storage import FileFormatError
 
 
 def register_extensions():
     """Register extension tables"""
     for file in files(__name__).iterdir():
         name = Path(file.name).stem
         if name.startswith('__'):
```

### Comparing `monobit-0.42.2/monobit/formats/text/draw.py` & `monobit-0.43.0/monobit/storage/formats/text/draw.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 """
-monobit.formats.text.draw - visual-text formats
+monobit.storage.formats.text.draw - visual-text formats
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 import string
 
-from ...storage import loaders, savers
-from ...font import Font
-from ...glyph import Glyph
-from ...labels import Tag, Char
-from ...magic import FileFormatError
-from ...encoding import charmaps
-from ...binary import align
+from monobit.storage import loaders, savers, FileFormatError
+from monobit.core import Font, Glyph, Tag, Char
+from monobit.encoding import encodings
+from monobit.base.binary import align
 
 
 ##############################################################################
 # hexdraw
 
 @loaders.register(
     name='hexdraw',
     patterns=('*.draw',),
 )
-def load_hexdraw(instream, ink:str='#', paper:str='-', unicode:bool=True):
+def load_hexdraw(
+        instream, ink:str='#', paper:str='-', unicode:bool=True, base:int=16,
+    ):
     """
-    Load font from a hexdraw file.
+    Load font from a hexdraw or similar text-based file.
 
     ink: character used for inked/foreground pixels (default #)
     paper: character used for uninked/background pixels (default -)
     unicode: interpret codepoint as Unicode (default: True)
+    base: representational base for codepoint (default: 16 for hexadecimal)
     """
-    DrawGlyph.ink = ink
-    DrawGlyph.paper = paper
+    class CustomGlyph(DrawGlyph): pass
+    CustomGlyph.ink = ink
+    CustomGlyph.paper = paper
+    CustomGlyph.base = base
     return load_draw(
-        instream.text, blocktypes=(DrawGlyph, DrawComment, Empty),
+        instream.text, blocktypes=(CustomGlyph, DrawComment, Empty),
         unicode=unicode
     )
 
 
 @savers.register(linked=load_hexdraw)
 def save_hexdraw(fonts, outstream, ink:str='#', paper:str='-', unicode:bool=True):
     """
@@ -74,24 +76,27 @@
             glyphs.append(block.get_value().modify(
                 comment='\n\n'.join(current_comment),
             ))
             current_comment = []
         elif isinstance(block, Unparsed):
             logging.debug('Unparsed lines: %s', block.get_value())
     font_comments.extend(current_comment)
-    if not unicode:
+    if unicode:
+        encoding = 'unicode'
+    else:
+        encoding = ''
         glyphs = tuple(
-            _g.label(codepoint_from=charmaps['unicode']).modify(char=None)
+            _g.label(codepoint_from=encodings['unicode']).modify(char=None)
             for _g in glyphs
         )
     font = Font(
         glyphs,
+        encoding=encoding,
         comment='\n\n'.join(font_comments)
     )
-
     return font
 
 
 # write hexdraw file
 
 def _save_draw(font, outstream, *, ink, paper, unicode):
     """Write one font to a plaintext stream as hexdraw."""
@@ -135,16 +140,16 @@
         for _line in comments.splitlines()
     )
 
 
 ###############################################################################
 # mkwinfon .fd
 
-from ...properties import Props
-from ..windows import WEIGHT_MAP, CHARSET_MAP
+from monobit.base import Props
+from ..common import WEIGHT_MAP, CHARSET_MAP
 
 
 FD_KEYS = {
     'facename',
     'copyright',
     'height',
     'ascent',
@@ -230,15 +235,15 @@
     return Font(glyphs, **mb_props).label()
 
 
 ###############################################################################
 # consoleet / vfontas / hxtools
 
 from pathlib import Path
-from ...containers.directory import Directory
+from monobit.storage.containers.directory import Directory
 
 @loaders.register(
     name='consoleet',
 )
 def load_clt(instream):
     """Load font from consoleet files."""
     # this format consists of separate image files, without a manifest
@@ -453,14 +458,17 @@
     return None
 
 
 class DrawGlyph(NonEmptyBlock):
     paper = '-'
     ink = '#'
 
+    # base for codepoint. default: hexadecimal
+    base = 16
+
     def starts(self, line):
         return line and line[:1] in string.hexdigits
 
     def ends(self, line):
         # empty or non-indented
         return not line[:1] in string.whitespace
 
@@ -472,20 +480,23 @@
             lines = [value] + lines
         lines = tuple(_l.strip() for _l in lines)
         return Glyph(
             lines, _0=self.paper, _1=self.ink,
             labels=(self.convert_key(key),),
         )
 
-    @staticmethod
-    def convert_key(key):
+    @classmethod
+    def convert_key(cls, key):
         """Convert keys on input from .draw."""
         key = key.strip()
         try:
-            return Char(''.join(chr(int(_key, 16)) for _key in key.split(',')))
+            return Char(''.join(
+                chr(int(_key, cls.base))
+                for _key in key.split(',')
+            ))
         except (TypeError, ValueError):
             return Tag(key)
 
 
 # mkwinfont block readers
 
 class MWFGlyph(NonEmptyBlock):
```

### Comparing `monobit-0.42.2/monobit/formats/text/hex.py` & `monobit-0.43.0/monobit/storage/formats/text/hex.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """
-monobit.formats.text.hex - Unifont Hex format
+monobit.storage.formats.text.hex - Unifont Hex format
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 # HEX format documentation
 # http://czyborra.com/unifont/
 
 import logging
 import string
 
-from ...storage import loaders, savers
-from ...magic import FileFormatError
-from ...font import Font
-from ...glyph import Glyph
+from monobit.storage import loaders, savers, FileFormatError
+from monobit.core import Font, Glyph
+
 from .draw import load_draw, DrawGlyph, DrawComment, Empty
 
 
 @loaders.register(name='pcbasic',)
 def load_hext(instream):
     """Load 8xN multi-cell font from PC-BASIC extended .HEX file."""
     return _load_hex(instream)
```

### Comparing `monobit-0.42.2/monobit/formats/text/yaff.py` & `monobit-0.43.0/monobit/storage/formats/text/yaff.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """
-monobit.formats.text.yaff - monobit-yaff format
+monobit.storage.formats.text.yaff - monobit-yaff format
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 import string
 from dataclasses import dataclass, field
 from itertools import count, zip_longest
 from collections import deque
 from functools import cached_property
 
-from ...storage import loaders, savers
-from ...encoding import charmaps
-from ...magic import FileFormatError
-from ...font import Font, FontProperties
-from ...glyph import Glyph
-from ...raster import Raster
-from ...labels import Label, strip_matching
-from ...properties import Props
-from ...basetypes import Coord, passthrough
+from monobit.storage import loaders, savers
+from monobit.storage import FileFormatError
+from monobit.core import Font, FontProperties, Glyph, Raster, Label, strip_matching
+from monobit.base import Props
+from monobit.base import Coord, passthrough
+
 from .draw import NonEmptyBlock, DrawComment, Empty, Unparsed, iter_blocks
 from .draw import format_comment
 
 
 ##############################################################################
 # interface
```

### Comparing `monobit-0.42.2/monobit/formats/windows/LICENSE.md` & `monobit-0.43.0/monobit/storage/formats/fon/windows/LICENSE.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Copyright
 ---------
-`monobit.formats.windows` is copyright 2019--2023 Rob Hagemans  
+`monobit.storage.formats.fon.windows` is copyright 2019--2023 Rob Hagemans  
 `mkwinfont` is copyright 2001 Simon Tatham. All rights reserved.  
 `dewinfont` is copyright 2001,2017 Simon Tatham. All rights reserved.  
 
 
 License
 -------
 Permission is hereby granted, free of charge, to any person
```

### Comparing `monobit-0.42.2/monobit/formats/windows/__init__.py` & `monobit-0.43.0/monobit/storage/formats/fon/windows/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """
-monobit.formats.windows - Windows FON and FNT files
+monobit.storage.formats.fon.windows - Windows FON and FNT files
 
-`monobit.formats.windows` is copyright 2019--2023 Rob Hagemans
+`monobit.storage.formats.windows` is copyright 2019--2023 Rob Hagemans
 `mkwinfont` is copyright 2001 Simon Tatham. All rights reserved.
 `dewinfont` is copyright 2001,2017 Simon Tatham. All rights reserved.
 
 See `LICENSE.md` in this package's directory.
 """
 
 import logging
 
-from ...storage import loaders, savers
-from ...magic import FileFormatError
+from monobit.storage import loaders, savers
+from monobit.storage import FileFormatError
+
 from .fnt import create_fnt
 from .fnt import convert_win_fnt_resource, FNT_MAGIC_1, FNT_MAGIC_2, FNT_MAGIC_3
 
-# used by other formats
-from .fnt import WEIGHT_MAP, WEIGHT_REVERSE_MAP, CHARSET_MAP, CHARSET_REVERSE_MAP
-
 
 @loaders.register(
     name='win',
     magic=(FNT_MAGIC_1, FNT_MAGIC_2, FNT_MAGIC_3),
     patterns=('*.fnt',),
 )
 def load_win_fnt(instream):
```

### Comparing `monobit-0.42.2/monobit/formats/windows/fnt.py` & `monobit-0.43.0/monobit/storage/formats/fon/windows/fnt.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 """
-monobit.formats.windows.fnt - Windows FNT resource
+monobit.storage.formats.fon.windows.fnt - Windows FNT resource
 
-`monobit.formats.windows` is copyright 2019--2023 Rob Hagemans
+`monobit.storage.formats.fon.windows` is copyright 2019--2023 Rob Hagemans
 `mkwinfont` is copyright 2001 Simon Tatham. All rights reserved.
 `dewinfont` is copyright 2001,2017 Simon Tatham. All rights reserved.
 
 See `LICENSE.md` in this package's directory.
 """
 
 
 import io
 import string
 import logging
 import itertools
 from types import SimpleNamespace
 
-from ...binary import bytes_to_bits, ceildiv, align
-from ...struct import little_endian as le
-from ...properties import reverse_dict
-from ...magic import FileFormatError
-from ...properties import Props
-from ...font import Font
-from ...glyph import Glyph
-from ...raster import Raster
-from ...vector import StrokePath
+from monobit.base.binary import bytes_to_bits, ceildiv, align
+from monobit.base.struct import little_endian as le
+from monobit.base import reverse_dict
+from monobit.storage import FileFormatError
+from monobit.base import Props
+from monobit.core import Font, Glyph, Raster, StrokePath
+
+# tables used by other formats
+from ...common import (
+    WEIGHT_MAP, WEIGHT_REVERSE_MAP,
+    CHARSET_MAP, CHARSET_REVERSE_MAP
+)
+
 
 FNT_MAGIC_1 = b'\0\1'
 FNT_MAGIC_2 = b'\0\2'
 FNT_MAGIC_3 = b'\0\3'
 
 
 ##############################################################################
@@ -47,170 +51,14 @@
 _FALLBACK_BREAK = 0x20
 
 # despite the presence of MBCS character set codes,
 # FNT can only hold single-byte codepoints
 # as firstChar and lastChar are byte-sized
 _FNT_RANGE = range(256)
 
-# official but vague documentation:
-# https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-wmf/0d0b32ac-a836-4bd2-a112-b6000a1b4fc9
-#
-# The CharacterSet Enumeration defines the possible sets of character glyphs that are defined in fonts for graphics output.
-#      typedef  enum
-#      {
-#        ANSI_CHARSET = 0x00000000,
-#        DEFAULT_CHARSET = 0x00000001,
-#        SYMBOL_CHARSET = 0x00000002,
-#        MAC_CHARSET = 0x0000004D,
-#        SHIFTJIS_CHARSET = 0x00000080,
-#        HANGUL_CHARSET = 0x00000081,
-#        JOHAB_CHARSET = 0x00000082,
-#        GB2312_CHARSET = 0x00000086,
-#        CHINESEBIG5_CHARSET = 0x00000088,
-#        GREEK_CHARSET = 0x000000A1,
-#        TURKISH_CHARSET = 0x000000A2,
-#        VIETNAMESE_CHARSET = 0x000000A3,
-#        HEBREW_CHARSET = 0x000000B1,
-#        ARABIC_CHARSET = 0x000000B2,
-#        BALTIC_CHARSET = 0x000000BA,
-#        RUSSIAN_CHARSET = 0x000000CC,
-#        THAI_CHARSET = 0x000000DE,
-#        EASTEUROPE_CHARSET = 0x000000EE,
-#        OEM_CHARSET = 0x000000FF
-#      } CharacterSet;
-#
-# ANSI_CHARSET: Specifies the English character set.
-# DEFAULT_CHARSET: Specifies a character set based on the current system locale; for example, when the system locale is United States English, the default character set is ANSI_CHARSET.
-# SYMBOL_CHARSET: Specifies a character set of symbols.
-# MAC_CHARSET: Specifies the Apple Macintosh character set.<6>
-# SHIFTJIS_CHARSET: Specifies the Japanese character set.
-# HANGUL_CHARSET: Also spelled "Hangeul". Specifies the Hangul Korean character set.
-# JOHAB_CHARSET: Also spelled "Johap". Specifies the Johab Korean character set.
-# GB2312_CHARSET: Specifies the "simplified" Chinese character set for People's Republic of China.
-# CHINESEBIG5_CHARSET: Specifies the "traditional" Chinese character set, used mostly in Taiwan and in the Hong Kong and Macao Special Administrative Regions.
-# GREEK_CHARSET: Specifies the Greek character set.
-# TURKISH_CHARSET: Specifies the Turkish character set.
-# VIETNAMESE_CHARSET: Specifies the Vietnamese character set.
-# HEBREW_CHARSET: Specifies the Hebrew character set
-# ARABIC_CHARSET: Specifies the Arabic character set
-# BALTIC_CHARSET: Specifies the Baltic (Northeastern European) character set
-# RUSSIAN_CHARSET: Specifies the Russian Cyrillic character set.
-# THAI_CHARSET: Specifies the Thai character set.
-# EASTEUROPE_CHARSET: Specifies a Eastern European character set.
-# OEM_CHARSET: Specifies a mapping to one of the OEM code pages, according to the current system locale setting.
-
-# MS Windows SDK 1.03 Programmer's reference, Appendix C Font Files, p. 427:
-#   "One byte specifying the character set defined by this font. The IBM@ PC hardware font has been
-#   assigned the designation 377 octal (FF hexadecimal or 255 decimal)."
-
-# below we follow the more useful info at https://www.freetype.org/freetype2/docs/reference/ft2-winfnt_fonts.html
-# from freetype freetype/ftwinfnt.h:
-#define FT_WinFNT_ID_CP1252    0
-#define FT_WinFNT_ID_DEFAULT   1
-#define FT_WinFNT_ID_SYMBOL    2
-#define FT_WinFNT_ID_MAC      77
-#define FT_WinFNT_ID_CP932   128
-#define FT_WinFNT_ID_CP949   129
-#define FT_WinFNT_ID_CP1361  130
-#define FT_WinFNT_ID_CP936   134
-#define FT_WinFNT_ID_CP950   136
-#define FT_WinFNT_ID_CP1253  161
-#define FT_WinFNT_ID_CP1254  162
-#define FT_WinFNT_ID_CP1258  163
-#define FT_WinFNT_ID_CP1255  177
-#define FT_WinFNT_ID_CP1256  178
-#define FT_WinFNT_ID_CP1257  186
-#define FT_WinFNT_ID_CP1251  204
-#define FT_WinFNT_ID_CP874   222
-#define FT_WinFNT_ID_CP1250  238
-#define FT_WinFNT_ID_OEM     255
-# some of their notes:
-#   SYMBOL - There is no known mapping table available.
-#   OEM - as opposed to ANSI, denotes the second default codepage that most international versions of Windows have.
-#         It is one of the OEM codepages from https://docs.microsoft.com/en-us/windows/desktop/intl/code-page-identifiers
-#   DEFAULT	- This is used for font enumeration and font creation as a ‘don't care’ value. Valid font files don't contain this value.
-#   Exact mapping tables for the various ‘cpXXXX’ encodings (except for ‘cp1361’) can be found at
-#   ‘ftp://ftp.unicode.org/Public/’ in the MAPPINGS/VENDORS/MICSFT/WINDOWS subdirectory.
-#   ‘cp1361’ is roughly a superset of MAPPINGS/OBSOLETE/EASTASIA/KSC/JOHAB.TXT.
-#
-CHARSET_MAP = {
-    0x00: 'windows-1252',
-    # no codepage
-    0x01: '',
-    0x02: 'windows-symbol',
-    0x4d: 'mac-roman',
-    0x80: 'windows-932',
-    0x81: 'windows-949',
-    0x82: 'windows-1361',
-    0x86: 'windows-936',
-    0x88: 'windows-950',
-    0xa1: 'windows-1253',
-    0xa2: 'windows-1254',
-    0xa3: 'windows-1258',
-    0xb1: 'windows-1255',
-    0xb2: 'windows-1256',
-    0xba: 'windows-1257',
-    0xcc: 'windows-1251',
-    0xde: 'windows-874',
-    0xee: 'windows-1250',
-    # could be any OEM codepage
-    0xff: '',
-}
-CHARSET_REVERSE_MAP = reverse_dict(CHARSET_MAP)
-CHARSET_REVERSE_MAP.update({
-    # different windows versions used different definitions of windows-1252
-    # see https://www.aivosto.com/articles/charsets-codepages-windows.html
-    'windows-ansi-1.0': 0x00,
-    'windows-ansi-2.0': 0x00,
-    'windows-ansi-3.1': 0x00,
-    'windows-1252': 0x00,
-    # windows-1252 agrees with iso-8859-1 (u+0000--u+00ff) except for controls 0x7F-0x9F
-    # furthermore, often the control range 0x00-0x19 is set to IBM graphics in windows-1252
-    'latin-1': 0x00,
-    'unicode': 0x00,
-    # use OEM as fallback for undefined as "valid font files don't contain 0x01"
-    '': 0xff,
-})
-
-# https://web.archive.org/web/20120215123301/http://support.microsoft.com/kb/65123
-# dfWeight: 2 bytes specifying the weight of the characters in the character definition data, on a scale of 1 to 1000.
-# A dfWeight of 400 specifies a regular weight.
-#
-# https://docs.microsoft.com/en-gb/windows/desktop/api/wingdi/ns-wingdi-taglogfonta
-# The weight of the font in the range 0 through 1000. For example, 400 is normal and 700 is bold.
-# If this value is zero, a default weight is used.
-# Value	Weight
-# FW_DONTCARE	0
-# FW_THIN	100
-# FW_EXTRALIGHT	200
-# FW_ULTRALIGHT	200
-# FW_LIGHT	300
-# FW_NORMAL	400
-# FW_REGULAR	400
-# FW_MEDIUM	500
-# FW_SEMIBOLD	600
-# FW_DEMIBOLD	600
-# FW_BOLD	700
-# FW_EXTRABOLD	800
-# FW_ULTRABOLD	800
-# FW_HEAVY	900
-# FW_BLACK	900
-WEIGHT_MAP = {
-    0: '', # undefined/unknown
-    100: 'thin', # bdf 'ultra-light' is windows' 'thin'
-    200: 'extra-light', # windows 'ultralight' equals 'extralight'
-    300: 'light',
-    400: 'regular', # 'regular' is 'normal' but less than 'medium' :/ ... bdf has a semi-light here
-    500: 'medium',
-    600: 'semi-bold',
-    700: 'bold',
-    800: 'extra-bold', # windows 'ultrabold' equals 'extrabold'
-    900: 'heavy', # bdf 'ultra-bold' is 'heavy'
-}
-WEIGHT_REVERSE_MAP = reverse_dict(WEIGHT_MAP)
 
 # pitch and family
 # low bit: 1 - proportional 0 - monospace
 # upper bits: family (like bdf add_style_name)
 #
 # Don't care or don't know.
 _FF_DONTCARE = 0<<4
@@ -615,32 +463,27 @@
     """Fill out a contiguous range of glyphs."""
     # x_width should equal average width
     # this is 0 for proportional fonts
     pix_width = font.cell_size.x
     # blank glyph of standard size
     blank = Glyph.blank(pix_width, font.raster_size.y)
     # char table; we need a contiguous range between the min and max codepoints
-    codepoints = font.get_codepoints()
-    ord_glyphs = [
-        font.get_glyph(_codepoint, missing=blank)
-        for _codepoint in range(min(codepoints)[0], max(codepoints)[0]+1)
-    ]
+    min_range = max(int(min(font.get_codepoints())), min(_FNT_RANGE))
+    max_range = min(int(max(font.get_codepoints())), max(_FNT_RANGE))
+    font = font.resample(codepoints=range(min_range, max_range+1), missing=blank)
     # add the guaranteed-blank glyph
-    ord_glyphs.append(blank)
-    font = font.modify(ord_glyphs)
+    font = font.modify(font.glyphs + (blank,))
     return font
 
 
 def create_fnt(font, version=0x200, vector=False):
     """Create .FNT from monobit font."""
     # ensure codepoint values are set, if possible
-    font = font.label(codepoint_from=font.encoding)
     # only include single-byte encoded glyphs
     # as firstChar and lastChar are byte-sized
-    font = font.subset(codepoints=_FNT_RANGE)
     font = _make_contiguous(font)
     # bring to equal-height, equal-upshift, padded normal form
     font = font.equalise_horizontal()
     bitmaps, char_table, offset_bitmaps, byte_width = _convert_to_fnt_glyphs(
         font, version, vector
     )
     bitmap_size = sum(len(_b) for _b in bitmaps)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `monobit-0.42.2/monobit/formats/windows/mz.py` & `monobit-0.43.0/monobit/storage/formats/fon/mz.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 """
-monobit.formats.windows.mz - DOS MZ executable header
+monobit.storage.formats.fon.windows.mz - DOS MZ executable header
 
-`monobit.formats.windows` is copyright 2019--2023 Rob Hagemans
-`mkwinfont` is copyright 2001 Simon Tatham. All rights reserved.
-`dewinfont` is copyright 2001,2017 Simon Tatham. All rights reserved.
-
-See `LICENSE.md` in this package's directory.
+(c) 2019--2023 Rob Hagemans
+with code from `mkwinfon`, copyright 2001 Simon Tatham. All rights reserved.
+licence: https://opensource.org/licenses/MIT
 """
 
-from ...struct import little_endian as le
-from ...binary import ceildiv, align
-
+from monobit.base.struct import little_endian as le
+from monobit.base.binary import ceildiv, align
 
-# MZ header:
-#   http://www.delorie.com/djgpp/doc/exe/
-#   https://wiki.osdev.org/MZ
 
 _STUB_MSG = b'This is a Windows font file.\r\n'
 
-# stub 16-bit DOS executable
+# stub 16-bit DOS executable from `mkwinfon`
 _STUB_CODE = bytes((
     0xBA, 0x0E, 0x00, # mov dx,0xe
     0x0E,             # push cs
     0x1F,             # pop ds
     0xB4, 0x09,       # mov ah,0x9
     0xCD, 0x21,       # int 0x21
     0xB8, 0x01, 0x4C, # mov ax,0x4c01
     0xCD, 0x21        # int 0x21
 ))
 
 # align on 16-byte (1<<4) boundaries
 ALIGN_SHIFT = 4
 
 # DOS executable (MZ) header
+#   http://www.delorie.com/djgpp/doc/exe/
+#   https://wiki.osdev.org/MZ
 # 40h size of structure
 MZ_HEADER = le.Struct(
     # 00 Magic number
     # EXE signature, 'MZ' or 'ZM'
     e_magic='2s',
     # 02 Bytes on last page of file
     # number of bytes in last 512-byte page of executable
```

### Comparing `monobit-0.42.2/monobit/formats/windows/ne.py` & `monobit-0.43.0/monobit/storage/formats/fon/windows/ne.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """
-monobit.formats.windows.ne - Windows 16-bit NE executable header
+monobit.storage.formats.fon.windows.ne - Windows 16-bit NE executable header
 
-`monobit.formats.windows` is copyright 2019--2023 Rob Hagemans
+`monobit.storage.formats.fon.windows` is copyright 2019--2023 Rob Hagemans
 `mkwinfont` is copyright 2001 Simon Tatham. All rights reserved.
 `dewinfont` is copyright 2001,2017 Simon Tatham. All rights reserved.
 
 See `LICENSE.md` in this package's directory.
 """
 
 import string
 import logging
 
-from ...binary import align
-from ...struct import little_endian as le
-from ...magic import FileFormatError
-from .mz import ALIGN_SHIFT
+from monobit.base.binary import align
+from monobit.base.struct import little_endian as le
+from monobit.storage import FileFormatError
+
 from .fnt import create_fnt
 
+# align on 16-byte (1<<4) boundaries
+ALIGN_SHIFT = 4
+
 
 ##############################################################################
 # NE (16-bit) executable structures
 
 # NE format:
 #   http://www.csn.ul.ie/~caolan/pub/winresdump/winresdump/doc/winexe.txt
 #   http://www.fileformat.info/format/exe/corion-ne.htm
```

### Comparing `monobit-0.42.2/monobit/formats/windows/pe.py` & `monobit-0.43.0/monobit/storage/formats/fon/windows/pe.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
-monobit.formats.windows.pe - Windows 32-bit PE executable header
+monobit.storage.formats.fon.windows.pe - Windows 32-bit PE executable header
 
-`monobit.formats.windows` is copyright 2019--2023 Rob Hagemans
+`monobit.storage.formats.fon.windows` is copyright 2019--2023 Rob Hagemans
 `mkwinfont` is copyright 2001 Simon Tatham. All rights reserved.
 `dewinfont` is copyright 2001,2017 Simon Tatham. All rights reserved.
 
 See `LICENSE.md` in this package's directory.
 """
 
 import logging
 
-from ...struct import little_endian as le
-from ...magic import FileFormatError
+from monobit.base.struct import little_endian as le
+from monobit.storage import FileFormatError
 
 
 ##############################################################################
 # PE (32-bit) executable structures
 
 # https://docs.microsoft.com/en-gb/windows/desktop/Debug/pe-format
 # https://github.com/deptofdefense/SalSA/wiki/PE-File-Format
```

### Comparing `monobit-0.42.2/monobit/formats/xlfd/bdf.py` & `monobit-0.43.0/monobit/storage/formats/xlfd/bdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 """
-monobit.formats.xlfd.bdf - Adobe Glyph Bitmap Distribution Format
+monobit.storage.formats.xlfd.bdf - Adobe Glyph Bitmap Distribution Format
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 
-from ...binary import ceildiv
-from ...storage import loaders, savers
-from ...magic import FileFormatError
-from ...font import Font, Coord
-from ...raster import Raster
-from ...glyph import Glyph
-from ...encoding import charmaps, NotFoundError
-from ...taggers import tagmaps
-from ...labels import Char, Codepoint, Tag
+from monobit.base.binary import ceildiv
+from monobit.storage import loaders, savers, FileFormatError
+from monobit.base import Coord
+from monobit.core import Font, Raster, Glyph, Char, Codepoint, Tag
+from monobit.encoding import encodings, NotFoundError
 
 from .xlfd import parse_xlfd_properties, create_xlfd_properties
 from .xlfd import create_xlfd_name, CUSTOM_PROP
 
 
 @loaders.register(
     name='bdf',
@@ -40,15 +36,15 @@
         logging.info('    %s: %s', name, value)
     bdf_glyphs = _read_bdf_glyphs(instream)
     glyphs, properties = _convert_from_bdf(bdf_glyphs, bdf_props, x_props)
     font = Font(glyphs, comment=comments, **properties)
     # create char labels, if encoding recognised
     font = font.label()
     # store labels as char only if we're working in unicode
-    if charmaps.is_unicode(font.encoding):
+    if encodings.is_unicode(font.encoding):
         font = font.label(codepoint_from=None)
     return font
 
 
 @savers.register(linked=load_bdf)
 def save_bdf(fonts, outstream):
     """
@@ -364,15 +360,15 @@
     xlfd_props = create_xlfd_properties(font)
     xlfd_name = create_xlfd_name(xlfd_props)
     bdf_props = _convert_to_bdf_properties(font, xlfd_name)
     # minimize glyphs to ink-bounds (BBX) before storing, except "cell" fonts
     if font.spacing not in ('character-cell', 'multi-cell'):
         font = font.reduce()
     # ensure character labels exist if needed
-    if charmaps.is_unicode(font.encoding):
+    if encodings.is_unicode(font.encoding):
         font = font.label(match_whitespace=False, match_graphical=False)
     glyphs = tuple(
         _convert_to_bdf_glyph(glyph, font)
         for glyph in font.glyphs
     )
     # write out
     for key, value in bdf_props:
@@ -438,29 +434,29 @@
             name = tag.value.encode('ascii').decode()
             if all(_c.isalnum() for _c in name):
                 break
         except UnicodeError:
             pass
     else:
         # look up in adobe glyph list if character available
-        name = tagmaps['adobe'].tag(*glyph.get_labels()).value
+        name = encodings['adobe'].tag(*glyph.get_labels()).value
         # otherwise, use encoding value if available
         if not name and encoding != -1:
             name = f'char{encoding:02X}'
         if not name:
             logging.warning(
                 f'Multi-codepoint glyph {glyph.codepoint}'
                 "can't be stored as no name or character available."
             )
     return encoding, name
 
 
 def _convert_to_bdf_glyph(glyph, font):
     encoding, name = _get_glyph_encvalue(
-        glyph, charmaps.is_unicode(font.encoding)
+        glyph, encodings.is_unicode(font.encoding)
     )
     swidth_y, dwidth_y = 0, 0
     # SWIDTH = DWIDTH / ( points/1000 * dpi / 72 )
     # DWIDTH specifies the widths in x and y, dwx0 and dwy0, in device pixels.
     # Like SWIDTH , this width information is a vector indicating the position of
     # the next glyph’s origin relative to the origin of this glyph.
     dwidth_x = glyph.advance_width
```

### Comparing `monobit-0.42.2/monobit/formats/xlfd/hbf.py` & `monobit-0.43.0/monobit/storage/formats/xlfd/hbf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """
-monobit.formats.xlfd.hbf - Hanzi Bitmap File Format
+monobit.storage.formats.xlfd.hbf - Hanzi Bitmap File Format
 
 (c) 2022--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from pathlib import Path
 
-from ...storage import loaders, savers
-from ...magic import FileFormatError
-from ...font import Font, Coord
-from ...glyph import Glyph
-from ...binary import ceildiv
+from monobit.storage import loaders, savers, FileFormatError
+from monobit.base import Coord
+from monobit.core import Font, Glyph
+from monobit.base.binary import ceildiv
 
 from .bdf import read_props
-from .xlfd import parse_xlfd_properties, create_xlfd_properties
+from .xlfd import parse_xlfd_properties, create_xlfd_properties, CUSTOM_PROP
 from .xlfd import create_xlfd_name
 from ..text.yaff import globalise_glyph_metrics
 
 
 @loaders.register(
     name='hbf',
     magic=(b'HBF_START_FONT ',),
@@ -175,39 +174,36 @@
         if not keyword or keyword == end:
             return props, comments
         sec_props, sec_comments = _read_section(
             instream, subsections=(), end=keyword.replace('START', 'END')
         )
         props.append((keyword, sec_props))
         # we're combining all comments in one block
-        comments.append('')
-        comments.extend(sec_comments)
+        if sec_comments:
+            comments.append('')
+            comments.extend(sec_comments)
 
 def indexer(plane, code_range, b2_ranges, b3_ranges):
     """Generator to run through code range keeping to allowed low-bytes."""
     if not code_range:
         return
     n_bytes = 3 if b3_ranges else 2
-    planeshift = 8 * n_bytes
-    hishift = 8 * (n_bytes-1)
-    loshift = 8 * (n_bytes-2)
-    himask = (1 << hishift) - 1
-    lomask = (1 << loshift) - 1
     for codepoint in code_range:
-        byte2 = (codepoint & himask) >> loshift
+        codebytes = tuple(codepoint.to_bytes(n_bytes, 'big'))
+        byte2 = codebytes[1]
         if all(byte2 not in _range for _range in b2_ranges):
             continue
         if n_bytes == 3:
-            byte3 = codepoint & lomask
+            byte3 = codebytes[2]
             if all(byte3 not in _range for _range in b3_ranges):
                 continue
         if plane is None:
             yield codepoint
         else:
-            yield ((0x80 + plane) << planeshift) + codepoint
+            yield int.from_bytes((plane, *codebytes), 'big')
 
 def _convert_ranges(b2_ranges):
     """Convert range descriptors to ranges."""
     b2_ranges = tuple(
         _split_hbf_ints(_range, sep='-')
         for _, _range in b2_ranges
     )
@@ -266,15 +262,15 @@
     # parse meaningful metadata
     properties, unparsed, plane = _parse_hbf_properties(hbf_props)
     # the FONT field *may* conform to xlfd but doesn't have to. don't parse it
     xlfd_props = parse_xlfd_properties(x_props, xlfd_name='', to_int=hbf_int)
     for key, value in unparsed.items():
         logging.info(f'Unrecognised HBF property {key}={value}')
         # preserve as property
-        properties[key] = value
+        properties[f'{CUSTOM_PROP}.{key}'] = value
     for key, value in xlfd_props.items():
         if key in properties and properties[key] != value:
             logging.debug(
                 'Inconsistency between HBF and XLFD properties: '
                 '%s=%s (from XLFD) but %s=%s (from HBF). Taking HBF property.',
                 key, value, key, properties[key]
             )
@@ -322,14 +318,15 @@
     code_scheme = hbf_props.pop('HBF_CODE_SCHEME')
     properties['encoding'], plane = _map_code_scheme(code_scheme)
     logging.debug(
         'Interpreting code scheme `%s` as encoding `%s` %s',
         code_scheme, properties['encoding'],
         f'plane {plane}' if plane is not None else ''
     )
+    hbf_props.pop('CHARS', None)
     hbf_props.pop('HBF_END_FONT', None)
     # keep unparsed hbf props
     return properties, hbf_props, plane
 
 
 ##############################################################################
 # hbf writer
@@ -345,16 +342,14 @@
             binfile.write(bitmap)
     for name, value in hbf_props:
         outstream.write(f'{name} {value}\n')
 
 
 def _convert_to_hbf(font, bitmap_name, code_scheme):
     """Convert to HBF properties."""
-    # set codepoints
-    font = font.label(codepoint_from=font.encoding)
     # get ranges
     cps, cranges, b2ranges, b3ranges = _get_code_ranges(font)
     font = font.subset(cps)
     # check if the remaining glyphs mae for a cell font
     if font.spacing != 'character-cell':
         raise FileFormatError(
             'Only character-cell fonts can be stored in HBF format.'
```

### Comparing `monobit-0.42.2/monobit/formats/xlfd/pcf.py` & `monobit-0.43.0/monobit/storage/formats/xlfd/pcf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 """
-monobit.formats.xlfd.pcf - X11 portable compiled format
+monobit.storage.formats.xlfd.pcf - X11 portable compiled format
 
 (c) 2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 from itertools import accumulate
 
-from ...struct import big_endian as be, little_endian as le
-from ...storage import loaders, savers
-from ...magic import FileFormatError
-from ...properties import Props
-from ...font import Font
-from ...glyph import Glyph
-from ...raster import Raster
-from ...labels import Tag, Codepoint
-from ...binary import align, ceildiv
+from monobit.base.struct import big_endian as be, little_endian as le
+from monobit.storage import loaders, savers, FileFormatError
+from monobit.base import Props
+from monobit.core import Font, Glyph, Raster, Tag, Codepoint
+from monobit.base.binary import align, ceildiv
 
 from .bdf import swidth_to_pixel, pixel_to_swidth
 from .xlfd import (
     parse_xlfd_properties, create_xlfd_properties, create_xlfd_name,
     from_quoted_string
 )
```

### Comparing `monobit-0.42.2/monobit/formats/xlfd/xlfd.py` & `monobit-0.43.0/monobit/storage/formats/xlfd/xlfd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
-monobit.formats.xlfd.xlfd - X11 Logical Font Description
+monobit.storage.formats.xlfd.xlfd - X11 Logical Font Description
 
 (c) 2019--2023 Rob Hagemans
 licence: https://opensource.org/licenses/MIT
 """
 
 import logging
 
-from ...encoding import charmaps
-from ...labels import Char
+from monobit.encoding import encodings
+from monobit.core import Char
 
 
 # dot property namespace for unrecognised properties
 CUSTOM_PROP = 'custom'
 
 
 ##############################################################################
@@ -569,15 +569,15 @@
         properties['encoding'] = registry
     elif encoding != '0':
         properties['encoding'] = encoding
     if properties['encoding'] in _UNDEFINED_ENCODINGS:
         properties['encoding'] = ''
     if 'DEFAULT_CHAR' in x_props:
         default_ord = to_int(x_props.pop('DEFAULT_CHAR', None))
-        if charmaps.is_unicode(properties['encoding']):
+        if encodings.is_unicode(properties['encoding']):
             properties['default_char'] = Char(chr(default_ord))
         else:
             properties['default_char'] = default_ord
     # keep original FontName if invalid or conflicting
     if not xlfd_name_props:
         if not properties['family']:
             properties['family'] = xlfd_name
@@ -676,15 +676,15 @@
         'MIN_SPACE': font.get_defined('min_word_space'),
         'NORM_SPACE': font.get_defined('word_space'),
         'MAX_SPACE': font.get_defined('max_word_space'),
         'END_SPACE': font.get_defined('sentence_space'),
     }
     # encoding dependent values
     default_glyph = font.get_default_glyph()
-    if charmaps.is_unicode(font.encoding):
+    if encodings.is_unicode(font.encoding):
         if default_glyph.char:
             default_codepoint = tuple(ord(_c) for _c in default_glyph.char)
         else:
             default_codepoint = default_glyph.codepoint
         if not len(default_codepoint):
             logging.debug('Cannot store default glyph in BDF without character or codepoint label.')
         elif len(default_codepoint) > 1:
```

### Comparing `monobit-0.42.2/monobit/scripts/banner.py` & `monobit-0.43.0/monobit/scripts/banner.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 import sys
 import argparse
 import logging
 import codecs
 from codecs import escape_decode
 
 import monobit
-from monobit.scripting import wrap_main
-from monobit.basetypes import Coord, RGB
-from monobit.renderer import render
-from monobit.font import Font
+from monobit.plumbing import wrap_main
+from monobit.base import Coord, RGB
+from monobit.render import render
+from monobit.core import Font
 
 
 def unescape(text):
     """Interpolate escape sequences."""
     # escape_decode is undocumented/unsupported and will leave \u escapes untouched
     # simpler variant - using documented/supported codecs
     #   raw-unicode-escape encodes to latin-1, leaves existing backslashes untouched but escapes non-latin-1
```

### Comparing `monobit-0.42.2/monobit/scripts/convert.py` & `monobit-0.43.0/monobit/scripts/convert.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,23 +5,22 @@
 
 import sys
 import logging
 from types import SimpleNamespace as Namespace
 from pathlib import Path
 
 import monobit
-from monobit.scripting import (
-    wrap_main, parse_subcommands, print_help, argrecord, GLOBAL_ARG_PREFIX
+from monobit.plumbing import (
+    wrap_main, parse_subcommands, argrecord, GLOBAL_ARG_PREFIX
 )
+from monobit.plumbing.help import get_context_func, print_help
 
 script_name = Path(sys.argv[0]).name
 
 operations = {
-    'load': monobit.load,
-    'save': monobit.save,
     'to': monobit.save,
     **monobit.operations
 }
 
 global_options = {
     'help': (bool, 'Print a help message and exit.'),
     'version': (bool, 'Show monobit version and exit.'),
@@ -32,38 +31,26 @@
     f'usage: {script_name} '
     + '[INFILE] [LOAD-OPTIONS] '
     + ' '.join(f'[{GLOBAL_ARG_PREFIX}{_op}]' for _op in global_options)
     + ' [COMMAND [OPTION...]] ...'
     + ' [to [OUTFILE] [SAVE-OPTIONS]]'
 )
 
-def _get_context_help(rec):
-    if rec.args:
-        file = rec.args[0]
-    else:
-        file = rec.kwargs.get('infile', '')
-    format = rec.kwargs.get('format', '')
-    if rec.command == 'load':
-        func, *_ = monobit.loaders.get_for(format=format)
-    else:
-        func, *_ = monobit.savers.get_for(format=format)
-    if func:
-        return func.script_args
-    return None
 
 def help(command_args):
     """Print the usage help message."""
     context_help = {
-        _rec.command: _get_context_help(_rec)
+        _rec.command: get_context_func(**vars(_rec))
         for _rec in command_args
         if _rec.command in ('load', 'save', 'to')
     }
     context_help = {_k: _v for _k, _v in context_help.items() if _v}
     print_help(command_args, usage, operations, global_options, context_help)
 
+
 def version():
     """Print the version string."""
     print(f'monobit v{monobit.__version__}')
 
 
 def main():
     command_args, global_args = parse_subcommands(operations, global_options=global_options)
```

### Comparing `monobit-0.42.2/LICENSE` & `monobit-0.43.0/LICENSE`

 * *Files identical despite different names*

### Comparing `monobit-0.42.2/README.md` & `monobit-0.43.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,15 @@
 | Raw binary            | `raw`      | `.fnt` `.rom` [*]           |&check;|&check;|
 | Codepage Information  | `cpi`      | `.cpi`                      |&check;|&check;|
 | Consoleet / vfontas   | `consoleet`| `.txt`                      |&check;|       |
 | Daisy-Dot             | `daisy`    | `.nlq` `.nl2` `.nl3` `.nl4` |&check;|       |
 | Dashen                | `dashen`   | `.pft`                      |&check;|       |
 | DEC DRCS soft font    | `dec`      |                             |&check;|&check;|
 | DosStart!             | `dosstart` | `.dsf`                      |&check;|       |
+| EDWIN bitmap font     | `edwin`    | `.fnt`                      |&check;|&check;|
 | FZX font              | `fzx`      | `.fzx`                      |&check;|&check;|
 | Figlet font           | `figlet`   | `.flf`                      |&check;|&check;|
 | Windows or OS/2 font  | `mzfon`    | `.fon` `.exe` `.dll`        |&check;|&check; (16-bit Windows) |
 | FONTX2                | `fontx`    | `.fnt`                      |&check;|&check;|
 | FONTEDIT              | `fontedit` | `.com`                      |&check;|       |
 | Fontraption           | `frapt`    | `.com`                      |&check;|       |
 | Fontraption TSR       | `frapt-tsr`| `.com`                      |&check;|       |
```

### Comparing `monobit-0.42.2/pyproject.toml` & `monobit-0.43.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "monobit"
-version = "0.42.2"
+version = "0.43.0"
 authors = [
     { name = "Rob Hagemans", email = "rob.hagemans@hotmail.com" },
 ]
 description = "Tools for working with monochrome bitmap fonts."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `monobit-0.42.2/PKG-INFO` & `monobit-0.43.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: monobit
-Version: 0.42.2
+Version: 0.43.0
 Summary: Tools for working with monochrome bitmap fonts.
 Project-URL: Homepage, https://github.com/robhagemans/monobit
 Author-email: Rob Hagemans <rob.hagemans@hotmail.com>
 License: MIT License
         
         Copyright (c) 2019--2023 Rob Hagemans
         
@@ -141,14 +141,15 @@
 | Raw binary            | `raw`      | `.fnt` `.rom` [*]           |&check;|&check;|
 | Codepage Information  | `cpi`      | `.cpi`                      |&check;|&check;|
 | Consoleet / vfontas   | `consoleet`| `.txt`                      |&check;|       |
 | Daisy-Dot             | `daisy`    | `.nlq` `.nl2` `.nl3` `.nl4` |&check;|       |
 | Dashen                | `dashen`   | `.pft`                      |&check;|       |
 | DEC DRCS soft font    | `dec`      |                             |&check;|&check;|
 | DosStart!             | `dosstart` | `.dsf`                      |&check;|       |
+| EDWIN bitmap font     | `edwin`    | `.fnt`                      |&check;|&check;|
 | FZX font              | `fzx`      | `.fzx`                      |&check;|&check;|
 | Figlet font           | `figlet`   | `.flf`                      |&check;|&check;|
 | Windows or OS/2 font  | `mzfon`    | `.fon` `.exe` `.dll`        |&check;|&check; (16-bit Windows) |
 | FONTX2                | `fontx`    | `.fnt`                      |&check;|&check;|
 | FONTEDIT              | `fontedit` | `.com`                      |&check;|       |
 | Fontraption           | `frapt`    | `.com`                      |&check;|       |
 | Fontraption TSR       | `frapt-tsr`| `.com`                      |&check;|       |
```

