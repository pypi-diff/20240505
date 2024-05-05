# Comparing `tmp/vastdb-0.1.2.tar.gz` & `tmp/vastdb-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vastdb-0.1.2.tar", last modified: Thu Apr 25 14:57:33 2024, max compression
+gzip compressed data, was "vastdb-0.1.3.tar", last modified: Sun May  5 11:44:30 2024, max compression
```

## Comparing `vastdb-0.1.2.tar` & `vastdb-0.1.3.tar`

### file list

```diff
@@ -1,197 +1,198 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.703902 vastdb-0.1.2/
--rw-rw-rw-   0 root         (0) root         (0)     3689 2024-04-25 14:01:45.000000 vastdb-0.1.2/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    11333 2024-04-25 14:01:45.000000 vastdb-0.1.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-25 14:01:45.000000 vastdb-0.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1311 2024-04-25 14:57:33.703902 vastdb-0.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5891 2024-04-25 14:01:45.000000 vastdb-0.1.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-04-25 14:01:45.000000 vastdb-0.1.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 14:57:33.703902 vastdb-0.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1702 2024-04-25 14:01:45.000000 vastdb-0.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.670903 vastdb-0.1.2/vast_flatbuf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.670903 vastdb-0.1.2/vast_flatbuf/org/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.670903 vastdb-0.1.2/vast_flatbuf/org/apache/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.670903 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.670903 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.684903 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/
--rw-rw-rw-   0 root         (0) root         (0)     5630 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py
--rw-rw-rw-   0 root         (0) root         (0)     2212 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py
--rw-rw-rw-   0 root         (0) root         (0)     2494 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)      182 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Bound.py
--rw-rw-rw-   0 root         (0) root         (0)     4434 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py
--rw-rw-rw-   0 root         (0) root         (0)     2429 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py
--rw-rw-rw-   0 root         (0) root         (0)     2520 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConcreteBoundImpl.py
--rw-rw-rw-   0 root         (0) root         (0)     3490 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py
--rw-rw-rw-   0 root         (0) root         (0)     1059 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py
--rw-rw-rw-   0 root         (0) root         (0)     1489 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     2576 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)      484 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Deref.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     2258 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py
--rw-rw-rw-   0 root         (0) root         (0)      498 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ExpressionImpl.py
--rw-rw-rw-   0 root         (0) root         (0)     1584 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py
--rw-rw-rw-   0 root         (0) root         (0)     2850 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py
--rw-rw-rw-   0 root         (0) root         (0)     3260 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py
--rw-rw-rw-   0 root         (0) root         (0)     2602 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1515 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     2130 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py
--rw-rw-rw-   0 root         (0) root         (0)      186 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Frame.py
--rw-rw-rw-   0 root         (0) root         (0)     2403 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1487 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     2139 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     2197 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py
--rw-rw-rw-   0 root         (0) root         (0)      211 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralImpl.py
--rw-rw-rw-   0 root         (0) root         (0)     1578 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py
--rw-rw-rw-   0 root         (0) root         (0)     4455 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py
--rw-rw-rw-   0 root         (0) root         (0)      230 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/JoinKind.py
--rw-rw-rw-   0 root         (0) root         (0)     2309 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py
--rw-rw-rw-   0 root         (0) root         (0)     3368 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py
--rw-rw-rw-   0 root         (0) root         (0)     2400 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     2797 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     2526 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py
--rw-rw-rw-   0 root         (0) root         (0)     3284 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py
--rw-rw-rw-   0 root         (0) root         (0)     1723 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py
--rw-rw-rw-   0 root         (0) root         (0)     2392 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     3847 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py
--rw-rw-rw-   0 root         (0) root         (0)      349 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Ordering.py
--rw-rw-rw-   0 root         (0) root         (0)     2378 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py
--rw-rw-rw-   0 root         (0) root         (0)     2130 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py
--rw-rw-rw-   0 root         (0) root         (0)     3941 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py
--rw-rw-rw-   0 root         (0) root         (0)     1526 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py
--rw-rw-rw-   0 root         (0) root         (0)     2113 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py
--rw-rw-rw-   0 root         (0) root         (0)      315 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelationImpl.py
--rw-rw-rw-   0 root         (0) root         (0)      217 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOpKind.py
--rw-rw-rw-   0 root         (0) root         (0)     3678 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py
--rw-rw-rw-   0 root         (0) root         (0)     3952 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py
--rw-rw-rw-   0 root         (0) root         (0)     2221 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py
--rw-rw-rw-   0 root         (0) root         (0)     5650 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py
--rw-rw-rw-   0 root         (0) root         (0)     1533 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1593 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py
--rw-rw-rw-   0 root         (0) root         (0)     2539 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1489 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1529 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py
--rw-rw-rw-   0 root         (0) root         (0)     7527 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.695903 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/
--rw-rw-rw-   0 root         (0) root         (0)     1026 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py
--rw-rw-rw-   0 root         (0) root         (0)     1326 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Block.py
--rw-rw-rw-   0 root         (0) root         (0)     2310 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py
--rw-rw-rw-   0 root         (0) root         (0)      836 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py
--rw-rw-rw-   0 root         (0) root         (0)      993 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py
--rw-rw-rw-   0 root         (0) root         (0)     1430 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/CompressionType.py
--rw-rw-rw-   0 root         (0) root         (0)     1760 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Date.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/DateUnit.py
--rw-rw-rw-   0 root         (0) root         (0)     2855 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py
--rw-rw-rw-   0 root         (0) root         (0)     3148 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py
--rw-rw-rw-   0 root         (0) root         (0)     4091 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py
--rw-rw-rw-   0 root         (0) root         (0)      410 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryKind.py
--rw-rw-rw-   0 root         (0) root         (0)     1456 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Endianness.py
--rw-rw-rw-   0 root         (0) root         (0)     1289 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py
--rw-rw-rw-   0 root         (0) root         (0)     7048 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Field.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py
--rw-rw-rw-   0 root         (0) root         (0)     1589 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py
--rw-rw-rw-   0 root         (0) root         (0)     1569 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py
--rw-rw-rw-   0 root         (0) root         (0)     1541 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py
--rw-rw-rw-   0 root         (0) root         (0)     6448 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py
--rw-rw-rw-   0 root         (0) root         (0)     1925 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Int.py
--rw-rw-rw-   0 root         (0) root         (0)     1456 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/IntervalUnit.py
--rw-rw-rw-   0 root         (0) root         (0)     2139 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py
--rw-rw-rw-   0 root         (0) root         (0)     1131 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py
--rw-rw-rw-   0 root         (0) root         (0)     1117 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py
--rw-rw-rw-   0 root         (0) root         (0)     1117 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py
--rw-rw-rw-   0 root         (0) root         (0)      993 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/List.py
--rw-rw-rw-   0 root         (0) root         (0)     2541 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Map.py
--rw-rw-rw-   0 root         (0) root         (0)     4486 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Message.py
--rw-rw-rw-   0 root         (0) root         (0)      671 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py
--rw-rw-rw-   0 root         (0) root         (0)      786 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py
--rw-rw-rw-   0 root         (0) root         (0)     1054 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Null.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Precision.py
--rw-rw-rw-   0 root         (0) root         (0)     5589 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py
--rw-rw-rw-   0 root         (0) root         (0)     6042 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixCompressedAxis.py
--rw-rw-rw-   0 root         (0) root         (0)     5785 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py
--rw-rw-rw-   0 root         (0) root         (0)     6091 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py
--rw-rw-rw-   0 root         (0) root         (0)      226 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndex.py
--rw-rw-rw-   0 root         (0) root         (0)     6389 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py
--rw-rw-rw-   0 root         (0) root         (0)     9409 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py
--rw-rw-rw-   0 root         (0) root         (0)     1193 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py
--rw-rw-rw-   0 root         (0) root         (0)     5767 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py
--rw-rw-rw-   0 root         (0) root         (0)     2149 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py
--rw-rw-rw-   0 root         (0) root         (0)     2639 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Time.py
--rw-rw-rw-   0 root         (0) root         (0)      191 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/TimeUnit.py
--rw-rw-rw-   0 root         (0) root         (0)     7925 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Type.py
--rw-rw-rw-   0 root         (0) root         (0)     3142 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Union.py
--rw-rw-rw-   0 root         (0) root         (0)      147 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/UnionMode.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.698902 vastdb-0.1.2/vast_flatbuf/tabular/
--rw-rw-rw-   0 root         (0) root         (0)     2114 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/AlterColumnRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     2222 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/AlterProjectionTableRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     1618 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/AlterSchemaRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     1610 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/AlterTableRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     1901 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/Column.py
--rw-rw-rw-   0 root         (0) root         (0)      151 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/ColumnType.py
--rw-rw-rw-   0 root         (0) root         (0)     2516 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/CreateProjectionRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     1626 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/CreateSchemaRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     3474 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     4655 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/GetTableStatsResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     2450 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/ImportDataRequest.py
--rw-rw-rw-   0 root         (0) root         (0)     4240 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/ListProjectionsResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     3036 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/ListSchemasResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     3550 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/ListTablesResponse.py
--rw-rw-rw-   0 root         (0) root         (0)     3589 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/ObjectDetails.py
--rw-rw-rw-   0 root         (0) root         (0)     4450 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/S3File.py
--rw-rw-rw-   0 root         (0) root         (0)     2069 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/VipRange.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:01:45.000000 vastdb-0.1.2/vast_flatbuf/tabular/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.700903 vastdb-0.1.2/vastdb/
--rw-rw-rw-   0 root         (0) root         (0)      292 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.701902 vastdb-0.1.2/vastdb/bench/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/bench/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1117 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/bench/test_perf.py
--rw-rw-rw-   0 root         (0) root         (0)     2991 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/bucket.py
--rw-rw-rw-   0 root         (0) root         (0)     2132 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3436 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/errors.py
--rw-rw-rw-   0 root         (0) root         (0)   101273 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/internal_commands.py
--rw-rw-rw-   0 root         (0) root         (0)     3324 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1718 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/session.py
--rw-rw-rw-   0 root         (0) root         (0)    20532 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.702902 vastdb-0.1.2/vastdb/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1913 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/tests/test_duckdb.py
--rw-rw-rw-   0 root         (0) root         (0)     5033 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/tests/test_imports.py
--rw-rw-rw-   0 root         (0) root         (0)      951 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/tests/test_nested.py
--rw-rw-rw-   0 root         (0) root         (0)     1255 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/tests/test_projections.py
--rw-rw-rw-   0 root         (0) root         (0)     2960 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/tests/test_sanity.py
--rw-rw-rw-   0 root         (0) root         (0)     1724 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/tests/test_schemas.py
--rw-rw-rw-   0 root         (0) root         (0)    25667 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/tests/test_tables.py
--rw-rw-rw-   0 root         (0) root         (0)      435 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/tests/util.py
--rw-rw-rw-   0 root         (0) root         (0)     2196 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/transaction.py
--rw-rw-rw-   0 root         (0) root         (0)     3022 2024-04-25 14:01:45.000000 vastdb-0.1.2/vastdb/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 14:57:33.702902 vastdb-0.1.2/vastdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1311 2024-04-25 14:57:33.000000 vastdb-0.1.2/vastdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9022 2024-04-25 14:57:33.000000 vastdb-0.1.2/vastdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 14:57:33.000000 vastdb-0.1.2/vastdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-04-25 14:57:33.000000 vastdb-0.1.2/vastdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-04-25 14:57:33.000000 vastdb-0.1.2/vastdb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.497443 vastdb-0.1.3/
+-rw-rw-rw-   0 root         (0) root         (0)     4052 2024-05-05 10:46:44.000000 vastdb-0.1.3/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    11333 2024-05-05 10:46:44.000000 vastdb-0.1.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-05 10:46:44.000000 vastdb-0.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1318 2024-05-05 11:44:30.497443 vastdb-0.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6027 2024-05-05 10:46:44.000000 vastdb-0.1.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-05-05 10:46:44.000000 vastdb-0.1.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-05 11:44:30.497443 vastdb-0.1.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1702 2024-05-05 10:46:44.000000 vastdb-0.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.463442 vastdb-0.1.3/vast_flatbuf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.463442 vastdb-0.1.3/vast_flatbuf/org/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.463442 vastdb-0.1.3/vast_flatbuf/org/apache/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.463442 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.463442 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.477443 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/
+-rw-rw-rw-   0 root         (0) root         (0)     5630 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2212 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py
+-rw-rw-rw-   0 root         (0) root         (0)     2494 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Bound.py
+-rw-rw-rw-   0 root         (0) root         (0)     4434 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py
+-rw-rw-rw-   0 root         (0) root         (0)     2520 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConcreteBoundImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)     3490 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     2576 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)      484 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Deref.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py
+-rw-rw-rw-   0 root         (0) root         (0)      498 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ExpressionImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1584 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py
+-rw-rw-rw-   0 root         (0) root         (0)     2850 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py
+-rw-rw-rw-   0 root         (0) root         (0)     3260 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2602 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1515 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2130 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py
+-rw-rw-rw-   0 root         (0) root         (0)      186 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Frame.py
+-rw-rw-rw-   0 root         (0) root         (0)     2403 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2139 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     2197 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py
+-rw-rw-rw-   0 root         (0) root         (0)      211 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1578 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py
+-rw-rw-rw-   0 root         (0) root         (0)     4455 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py
+-rw-rw-rw-   0 root         (0) root         (0)      230 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/JoinKind.py
+-rw-rw-rw-   0 root         (0) root         (0)     2309 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py
+-rw-rw-rw-   0 root         (0) root         (0)     3368 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2400 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     2797 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2526 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)     3284 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1723 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py
+-rw-rw-rw-   0 root         (0) root         (0)     2392 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     3847 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Ordering.py
+-rw-rw-rw-   0 root         (0) root         (0)     2378 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py
+-rw-rw-rw-   0 root         (0) root         (0)     2130 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py
+-rw-rw-rw-   0 root         (0) root         (0)     3941 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py
+-rw-rw-rw-   0 root         (0) root         (0)      315 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelationImpl.py
+-rw-rw-rw-   0 root         (0) root         (0)      217 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOpKind.py
+-rw-rw-rw-   0 root         (0) root         (0)     3678 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3952 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py
+-rw-rw-rw-   0 root         (0) root         (0)     2221 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py
+-rw-rw-rw-   0 root         (0) root         (0)     5650 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py
+-rw-rw-rw-   0 root         (0) root         (0)     1533 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1593 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py
+-rw-rw-rw-   0 root         (0) root         (0)     2539 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py
+-rw-rw-rw-   0 root         (0) root         (0)     7527 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.488443 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Block.py
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py
+-rw-rw-rw-   0 root         (0) root         (0)      836 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py
+-rw-rw-rw-   0 root         (0) root         (0)      993 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py
+-rw-rw-rw-   0 root         (0) root         (0)     1430 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/CompressionType.py
+-rw-rw-rw-   0 root         (0) root         (0)     1760 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Date.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/DateUnit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2855 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py
+-rw-rw-rw-   0 root         (0) root         (0)     3148 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4091 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py
+-rw-rw-rw-   0 root         (0) root         (0)      410 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryKind.py
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Endianness.py
+-rw-rw-rw-   0 root         (0) root         (0)     1289 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Field.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py
+-rw-rw-rw-   0 root         (0) root         (0)     1569 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     6448 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1925 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Int.py
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/IntervalUnit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2139 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py
+-rw-rw-rw-   0 root         (0) root         (0)      993 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/List.py
+-rw-rw-rw-   0 root         (0) root         (0)     2541 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Map.py
+-rw-rw-rw-   0 root         (0) root         (0)     4486 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Message.py
+-rw-rw-rw-   0 root         (0) root         (0)      671 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py
+-rw-rw-rw-   0 root         (0) root         (0)      786 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py
+-rw-rw-rw-   0 root         (0) root         (0)     1054 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Null.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Precision.py
+-rw-rw-rw-   0 root         (0) root         (0)     5589 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py
+-rw-rw-rw-   0 root         (0) root         (0)     6042 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixCompressedAxis.py
+-rw-rw-rw-   0 root         (0) root         (0)     5785 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py
+-rw-rw-rw-   0 root         (0) root         (0)     6091 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py
+-rw-rw-rw-   0 root         (0) root         (0)      226 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndex.py
+-rw-rw-rw-   0 root         (0) root         (0)     6389 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py
+-rw-rw-rw-   0 root         (0) root         (0)     9409 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py
+-rw-rw-rw-   0 root         (0) root         (0)     5767 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2149 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py
+-rw-rw-rw-   0 root         (0) root         (0)     2639 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Time.py
+-rw-rw-rw-   0 root         (0) root         (0)      191 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/TimeUnit.py
+-rw-rw-rw-   0 root         (0) root         (0)     7925 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Type.py
+-rw-rw-rw-   0 root         (0) root         (0)     3142 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Union.py
+-rw-rw-rw-   0 root         (0) root         (0)      147 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/UnionMode.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.491443 vastdb-0.1.3/vast_flatbuf/tabular/
+-rw-rw-rw-   0 root         (0) root         (0)     2114 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/AlterColumnRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2222 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/AlterProjectionTableRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/AlterSchemaRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1610 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/AlterTableRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1901 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/Column.py
+-rw-rw-rw-   0 root         (0) root         (0)      151 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/ColumnType.py
+-rw-rw-rw-   0 root         (0) root         (0)     2516 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/CreateProjectionRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1626 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/CreateSchemaRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3474 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     4655 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/GetTableStatsResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     2450 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/ImportDataRequest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4240 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/ListProjectionsResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/ListSchemasResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3550 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/ListTablesResponse.py
+-rw-rw-rw-   0 root         (0) root         (0)     3589 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/ObjectDetails.py
+-rw-rw-rw-   0 root         (0) root         (0)     4450 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/S3File.py
+-rw-rw-rw-   0 root         (0) root         (0)     2069 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/VipRange.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 10:46:44.000000 vastdb-0.1.3/vast_flatbuf/tabular/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.493443 vastdb-0.1.3/vastdb/
+-rw-rw-rw-   0 root         (0) root         (0)      292 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.494443 vastdb-0.1.3/vastdb/bench/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/bench/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/bench/test_perf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3566 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/bucket.py
+-rw-rw-rw-   0 root         (0) root         (0)     2132 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3793 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    99575 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/internal_commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     3346 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2323 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/session.py
+-rw-rw-rw-   0 root         (0) root         (0)    25661 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.496443 vastdb-0.1.3/vastdb/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1913 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/tests/test_duckdb.py
+-rw-rw-rw-   0 root         (0) root         (0)     5705 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/tests/test_imports.py
+-rw-rw-rw-   0 root         (0) root         (0)      951 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/tests/test_nested.py
+-rw-rw-rw-   0 root         (0) root         (0)     1255 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/tests/test_projections.py
+-rw-rw-rw-   0 root         (0) root         (0)     2960 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/tests/test_sanity.py
+-rw-rw-rw-   0 root         (0) root         (0)     1739 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/tests/test_schemas.py
+-rw-rw-rw-   0 root         (0) root         (0)    26672 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/tests/test_tables.py
+-rw-rw-rw-   0 root         (0) root         (0)     1046 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/tests/test_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      435 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/tests/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2845 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/transaction.py
+-rw-rw-rw-   0 root         (0) root         (0)     4276 2024-05-05 10:46:44.000000 vastdb-0.1.3/vastdb/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-05 11:44:30.496443 vastdb-0.1.3/vastdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1318 2024-05-05 11:44:30.000000 vastdb-0.1.3/vastdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9048 2024-05-05 11:44:30.000000 vastdb-0.1.3/vastdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-05 11:44:30.000000 vastdb-0.1.3/vastdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2024-05-05 11:44:30.000000 vastdb-0.1.3/vastdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-05 11:44:30.000000 vastdb-0.1.3/vastdb.egg-info/top_level.txt
```

### Comparing `vastdb-0.1.2/CHANGELOG.md` & `vastdb-0.1.3/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,27 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
+## [0.1.3] (2024-05-05)
+[0.1.3]: https://github.com/vast-data/vastdb_sdk/compare/v0.1.2...v0.1.3
+
+### Added
+ - Document predicate pushdown support
+ - Access imports' table (for VAST 5.2+)
+ - Support `is_in` predicate pushdown
+ - Document `table.py`
+
+### Fixed
+ - Freeze `ibis` dependency at 8.0.0
+ - Support snapshot-based access
+ - Optimize RecordBatch slicing
+
 ## [0.1.2] (2024-04-25)
 [0.1.2]: https://github.com/vast-data/vastdb_sdk/compare/v0.1.1...v0.1.2
 
 ### Added
  - Allow querying [VAST Catalog](https://www.vastdata.com/blog/vast-catalog-treat-your-file-system-like-a-database)
  - Use [mypy](https://mypy-lang.org/) for type annotation checking
```

### Comparing `vastdb-0.1.2/LICENSE` & `vastdb-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/PKG-INFO` & `vastdb-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vastdb
-Version: 0.1.2
+Version: 0.1.3
 Summary: VAST Data SDK
 Home-page: https://github.com/vast-data/vastdb_sdk
 Author: VAST DATA
 Author-email: hello@vastdata.com
 License: Copyright (C) VAST Data Ltd.
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -17,15 +17,15 @@
 Classifier: Topic :: Database :: Front-Ends
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aws-requests-auth
 Requires-Dist: boto3
 Requires-Dist: flatbuffers
-Requires-Dist: ibis-framework
+Requires-Dist: ibis-framework==8.0.0
 Requires-Dist: pyarrow
 Requires-Dist: requests
 Requires-Dist: xmltodict
 
 
 `vastdb` is a Python-based SDK designed for interacting
 with [VAST Database](https://vastdata.com/database)
```

### Comparing `vastdb-0.1.2/README.md` & `vastdb-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -173,197 +173,205 @@
 00000ac0: 0a0a 2020 2020 2320 5345 4c45 4354 202a  ..    # SELECT *
 00000ad0: 2046 524f 4d20 7420 5748 4552 4520 6333   FROM t WHERE c3
 00000ae0: 204c 494b 4520 2725 7375 6273 7472 696e   LIKE '%substrin
 00000af0: 6725 270a 2020 2020 7461 626c 652e 7365  g%'.    table.se
 00000b00: 6c65 6374 2870 7265 6469 6361 7465 3d74  lect(predicate=t
 00000b10: 6162 6c65 5b27 6333 275d 2e63 6f6e 7461  able['c3'].conta
 00000b20: 696e 7328 2773 7562 7374 7269 6e67 2729  ins('substring')
-00000b30: 290a 6060 600a 0a23 2320 496d 706f 7274  ).```..## Import
-00000b40: 2061 2073 696e 676c 6520 5061 7271 7565   a single Parque
-00000b50: 7420 6669 6c65 2076 6961 2053 3320 7072  t file via S3 pr
-00000b60: 6f74 6f63 6f6c 0a0a 4974 2069 7320 706f  otocol..It is po
-00000b70: 7373 6962 6c65 2074 6f20 6566 6669 6369  ssible to effici
-00000b80: 656e 746c 7920 6372 6561 7465 2061 2074  ently create a t
-00000b90: 6162 6c65 2066 726f 6d20 6120 5061 7271  able from a Parq
-00000ba0: 7565 7420 6669 6c65 2028 7769 7468 6f75  uet file (withou
-00000bb0: 7420 636f 7079 696e 6720 6974 2076 6961  t copying it via
-00000bc0: 2074 6865 2063 6c69 656e 7429 3a0a 0a60   the client):..`
-00000bd0: 6060 7079 7468 6f6e 0a20 2020 2077 6974  ``python.    wit
-00000be0: 6820 7465 6d70 6669 6c65 2e4e 616d 6564  h tempfile.Named
-00000bf0: 5465 6d70 6f72 6172 7946 696c 6528 2920  TemporaryFile() 
-00000c00: 6173 2066 3a0a 2020 2020 2020 2020 7061  as f:.        pa
-00000c10: 2e70 6172 7175 6574 2e77 7269 7465 5f74  .parquet.write_t
-00000c20: 6162 6c65 2861 7272 6f77 5f74 6162 6c65  able(arrow_table
-00000c30: 2c20 662e 6e61 6d65 290a 2020 2020 2020  , f.name).      
-00000c40: 2020 7333 2e70 7574 5f6f 626a 6563 7428    s3.put_object(
-00000c50: 4275 636b 6574 3d27 6275 636b 6574 2d6e  Bucket='bucket-n
-00000c60: 616d 6527 2c20 4b65 793d 2773 7461 6769  ame', Key='stagi
-00000c70: 6e67 2f66 696c 652e 7061 7271 7565 7427  ng/file.parquet'
-00000c80: 2c20 426f 6479 3d66 290a 0a20 2020 2073  , Body=f)..    s
-00000c90: 6368 656d 6120 3d20 7478 2e62 7563 6b65  chema = tx.bucke
-00000ca0: 7428 2762 7563 6b65 742d 6e61 6d65 2729  t('bucket-name')
-00000cb0: 2e73 6368 656d 6128 2773 6368 656d 612d  .schema('schema-
-00000cc0: 6e61 6d65 2729 0a20 2020 2074 6162 6c65  name').    table
-00000cd0: 203d 2075 7469 6c2e 6372 6561 7465 5f74   = util.create_t
-00000ce0: 6162 6c65 5f66 726f 6d5f 6669 6c65 7328  able_from_files(
-00000cf0: 0a20 2020 2020 2020 2073 6368 656d 613d  .        schema=
-00000d00: 7363 6865 6d61 2c20 7461 626c 655f 6e61  schema, table_na
-00000d10: 6d65 3d27 696d 706f 7274 6564 2d74 6162  me='imported-tab
-00000d20: 6c65 272c 0a20 2020 2020 2020 2070 6172  le',.        par
-00000d30: 7175 6574 5f66 696c 6573 3d5b 272f 6275  quet_files=['/bu
-00000d40: 636b 6574 2d6e 616d 652f 7374 6167 696e  cket-name/stagin
-00000d50: 672f 6669 6c65 2e70 6172 7175 6574 275d  g/file.parquet']
-00000d60: 290a 6060 600a 0a23 2320 496d 706f 7274  ).```..## Import
-00000d70: 206d 756c 7469 706c 6520 5061 7271 7565   multiple Parque
-00000d80: 7420 6669 6c65 7320 636f 6e63 7572 7265  t files concurre
-00000d90: 6e74 6c79 2076 6961 2053 3320 7072 6f74  ntly via S3 prot
-00000da0: 6f63 6f6c 0a0a 5765 2063 616e 2069 6d70  ocol..We can imp
-00000db0: 6f72 7420 6d75 6c74 6970 6c65 2066 696c  ort multiple fil
-00000dc0: 6573 2063 6f6e 6375 7272 656e 746c 7920  es concurrently 
-00000dd0: 696e 746f 2061 2074 6162 6c65 2028 6279  into a table (by
-00000de0: 2075 7469 6c69 7a69 6e67 206d 756c 7469   utilizing multi
-00000df0: 706c 6520 434e 6f64 6573 2720 636f 7265  ple CNodes' core
-00000e00: 7329 3a0a 0a60 6060 7079 7468 6f6e 0a20  s):..```python. 
-00000e10: 2020 2073 6368 656d 6120 3d20 7478 2e62     schema = tx.b
-00000e20: 7563 6b65 7428 2762 7563 6b65 742d 6e61  ucket('bucket-na
-00000e30: 6d65 2729 2e73 6368 656d 6128 2773 6368  me').schema('sch
-00000e40: 656d 612d 6e61 6d65 2729 0a20 2020 2074  ema-name').    t
-00000e50: 6162 6c65 203d 2075 7469 6c2e 6372 6561  able = util.crea
-00000e60: 7465 5f74 6162 6c65 5f66 726f 6d5f 6669  te_table_from_fi
-00000e70: 6c65 7328 0a20 2020 2020 2020 2073 6368  les(.        sch
-00000e80: 656d 613d 7363 6865 6d61 2c20 7461 626c  ema=schema, tabl
-00000e90: 655f 6e61 6d65 3d27 6c61 7267 652d 696d  e_name='large-im
-00000ea0: 706f 7274 6564 2d74 6162 6c65 272c 0a20  ported-table',. 
-00000eb0: 2020 2020 2020 2070 6172 7175 6574 5f66         parquet_f
-00000ec0: 696c 6573 3d5b 6627 2f62 7563 6b65 742d  iles=[f'/bucket-
-00000ed0: 6e61 6d65 2f73 7461 6769 6e67 2f66 696c  name/staging/fil
-00000ee0: 657b 697d 2e70 6172 7175 6574 2720 666f  e{i}.parquet' fo
-00000ef0: 7220 6920 696e 2072 616e 6765 2831 3029  r i in range(10)
-00000f00: 5d29 0a60 6060 0a0a 2323 2050 6f73 742d  ]).```..## Post-
-00000f10: 7072 6f63 6573 7369 6e67 0a0a 2323 2320  processing..### 
-00000f20: 4578 706f 7274 0a0a 6054 6162 6c65 2e73  Export..`Table.s
-00000f30: 656c 6563 7428 2960 2072 6574 7572 6e73  elect()` returns
-00000f40: 2061 2073 7472 6561 6d20 6f66 205b 5079   a stream of [Py
-00000f50: 4172 726f 7720 7265 636f 7264 2062 6174  Arrow record bat
-00000f60: 6368 6573 5d28 6874 7470 733a 2f2f 6172  ches](https://ar
-00000f70: 726f 772e 6170 6163 6865 2e6f 7267 2f64  row.apache.org/d
-00000f80: 6f63 732f 7079 7468 6f6e 2f64 6174 612e  ocs/python/data.
-00000f90: 6874 6d6c 2372 6563 6f72 642d 6261 7463  html#record-batc
-00000fa0: 6865 7329 2c20 7768 6963 6820 6361 6e20  hes), which can 
-00000fb0: 6265 2064 6972 6563 746c 7920 6578 706f  be directly expo
-00000fc0: 7274 6564 2069 6e74 6f20 6120 5061 7271  rted into a Parq
-00000fd0: 7565 7420 6669 6c65 3a0a 0a60 6060 7079  uet file:..```py
-00000fe0: 7468 6f6e 0a62 6174 6368 6573 203d 2074  thon.batches = t
-00000ff0: 6162 6c65 2e73 656c 6563 7428 290a 7769  able.select().wi
-00001000: 7468 2063 6f6e 7465 7874 6c69 622e 636c  th contextlib.cl
-00001010: 6f73 696e 6728 7061 2e70 6172 7175 6574  osing(pa.parquet
-00001020: 2e50 6172 7175 6574 5772 6974 6572 2827  .ParquetWriter('
-00001030: 2f70 6174 682f 746f 2f66 696c 652e 7061  /path/to/file.pa
-00001040: 7271 7565 7427 2c20 6261 7463 6865 732e  rquet', batches.
-00001050: 7363 6865 6d61 2929 2061 7320 7772 6974  schema)) as writ
-00001060: 6572 3a0a 2020 2020 666f 7220 6261 7463  er:.    for batc
-00001070: 6820 696e 2074 6162 6c65 5f62 6174 6368  h in table_batch
-00001080: 6573 3a0a 2020 2020 2020 2020 7772 6974  es:.        writ
-00001090: 6572 2e77 7269 7465 5f62 6174 6368 2862  er.write_batch(b
-000010a0: 6174 6368 290a 6060 600a 0a23 2323 2044  atch).```..### D
-000010b0: 7563 6b44 420a 0a57 6520 6361 6e20 7573  uckDB..We can us
-000010c0: 6520 5b44 7563 6b44 425d 2868 7474 7073  e [DuckDB](https
-000010d0: 3a2f 2f64 7563 6b64 622e 6f72 672f 646f  ://duckdb.org/do
-000010e0: 6373 2f67 7569 6465 732f 7079 7468 6f6e  cs/guides/python
-000010f0: 2f73 716c 5f6f 6e5f 6172 726f 772e 6874  /sql_on_arrow.ht
-00001100: 6d6c 2920 746f 2070 6f73 742d 7072 6f63  ml) to post-proc
-00001110: 6573 7320 7468 6520 7265 7375 6c74 696e  ess the resultin
-00001120: 6720 7374 7265 616d 206f 6620 5b50 7941  g stream of [PyA
-00001130: 7272 6f77 2072 6563 6f72 6420 6261 7463  rrow record batc
-00001140: 6865 735d 2868 7474 7073 3a2f 2f61 7272  hes](https://arr
-00001150: 6f77 2e61 7061 6368 652e 6f72 672f 646f  ow.apache.org/do
-00001160: 6373 2f70 7974 686f 6e2f 6461 7461 2e68  cs/python/data.h
-00001170: 746d 6c23 7265 636f 7264 2d62 6174 6368  tml#record-batch
-00001180: 6573 293a 0a0a 6060 6070 7974 686f 6e0a  es):..```python.
-00001190: 696d 706f 7274 2064 7563 6b64 620a 636f  import duckdb.co
-000011a0: 6e6e 203d 2064 7563 6b64 622e 636f 6e6e  nn = duckdb.conn
-000011b0: 6563 7428 290a 0a62 6174 6368 6573 203d  ect()..batches =
-000011c0: 2074 6162 6c65 2e73 656c 6563 7428 636f   table.select(co
-000011d0: 6c75 6d6e 733d 5b27 6331 275d 2c20 7072  lumns=['c1'], pr
-000011e0: 6564 6963 6174 653d 2874 6162 6c65 5b27  edicate=(table['
-000011f0: 6332 275d 203e 2032 2929 0a70 7269 6e74  c2'] > 2)).print
-00001200: 2863 6f6e 6e2e 6578 6563 7574 6528 2253  (conn.execute("S
-00001210: 454c 4543 5420 7375 6d28 6331 2920 4652  ELECT sum(c1) FR
-00001220: 4f4d 2062 6174 6368 6573 2229 2e61 7272  OM batches").arr
-00001230: 6f77 2829 290a 6060 600a 0a23 2320 5365  ow()).```..## Se
-00001240: 6d69 2d73 6f72 7465 6420 7072 6f6a 6563  mi-sorted projec
-00001250: 7469 6f6e 730a 0a57 6520 6361 6e20 6372  tions..We can cr
-00001260: 6561 7465 2c20 6c69 7374 2061 6e64 2064  eate, list and d
-00001270: 656c 6574 6520 5b61 7661 696c 6162 6c65  elete [available
-00001280: 2073 656d 692d 736f 7274 6564 2070 726f   semi-sorted pro
-00001290: 6a65 6374 696f 6e73 5d28 6874 7470 733a  jections](https:
-000012a0: 2f2f 7375 7070 6f72 742e 7661 7374 6461  //support.vastda
-000012b0: 7461 2e63 6f6d 2f73 2f61 7274 6963 6c65  ta.com/s/article
-000012c0: 2f55 5549 442d 6534 6361 3432 6162 2d64  /UUID-e4ca42ab-d
-000012d0: 3135 622d 3662 3732 2d62 6436 622d 6633  15b-6b72-bd6b-f3
-000012e0: 6337 3762 3435 3564 6534 293a 0a0a 6060  c77b455de4):..``
-000012f0: 6070 7974 686f 6e0a 7020 3d20 7461 626c  `python.p = tabl
-00001300: 652e 6372 6561 7465 5f70 726f 6a65 6374  e.create_project
-00001310: 696f 6e28 2770 726f 6a27 2c20 736f 7274  ion('proj', sort
-00001320: 6564 3d5b 2763 3327 5d2c 2075 6e73 6f72  ed=['c3'], unsor
-00001330: 7465 643d 5b27 6331 275d 290a 7072 696e  ted=['c1']).prin
-00001340: 7428 7461 626c 652e 7072 6f6a 6563 7469  t(table.projecti
-00001350: 6f6e 7328 2929 0a70 7269 6e74 2870 2e67  ons()).print(p.g
-00001360: 6574 5f73 7461 7473 2829 290a 702e 6472  et_stats()).p.dr
-00001370: 6f70 2829 0a60 6060 0a0a 2323 2053 6e61  op().```..## Sna
-00001380: 7073 686f 7473 0a0a 4974 2069 7320 706f  pshots..It is po
-00001390: 7373 6962 6c65 2074 6f20 6c69 7374 205b  ssible to list [
-000013a0: 6176 6169 6c61 626c 6520 736e 6170 7368  available snapsh
-000013b0: 6f74 735d 2868 7474 7073 3a2f 2f76 6173  ots](https://vas
-000013c0: 7464 6174 612e 636f 6d2f 626c 6f67 2f62  tdata.com/blog/b
-000013d0: 7269 6e67 696e 672d 736e 6170 7368 6f74  ringing-snapshot
-000013e0: 732d 746f 2d76 6173 7473 2d65 6c65 6d65  s-to-vasts-eleme
-000013f0: 6e74 2d73 746f 7265 293a 0a0a 6060 6070  nt-store):..```p
-00001400: 7974 686f 6e0a 7072 696e 7428 6275 636b  ython.print(buck
-00001410: 6574 2e6c 6973 745f 736e 6170 7368 6f74  et.list_snapshot
-00001420: 7328 2929 0a60 6060 0a0a 2323 2056 4153  s()).```..## VAS
-00001430: 5420 4361 7461 6c6f 670a 0a5b 5641 5354  T Catalog..[VAST
-00001440: 2043 6174 616c 6f67 5d28 6874 7470 733a   Catalog](https:
-00001450: 2f2f 7661 7374 6461 7461 2e63 6f6d 2f62  //vastdata.com/b
-00001460: 6c6f 672f 7661 7374 2d63 6174 616c 6f67  log/vast-catalog
-00001470: 2d74 7265 6174 2d79 6f75 722d 6669 6c65  -treat-your-file
-00001480: 2d73 7973 7465 6d2d 6c69 6b65 2d61 2d64  -system-like-a-d
-00001490: 6174 6162 6173 6529 2063 616e 2062 6520  atabase) can be 
-000014a0: 7175 6572 6965 6420 6173 2061 2072 6567  queried as a reg
-000014b0: 756c 6172 2074 6162 6c65 3a0a 0a60 6060  ular table:..```
-000014c0: 7079 7468 6f6e 0a74 6162 6c65 203d 2070  python.table = p
-000014d0: 612e 5461 626c 652e 6672 6f6d 5f62 6174  a.Table.from_bat
-000014e0: 6368 6573 2874 782e 6361 7461 6c6f 672e  ches(tx.catalog.
-000014f0: 7365 6c65 6374 285b 2765 6c65 6d65 6e74  select(['element
-00001500: 5f74 7970 6527 5d29 290a 6466 203d 2074  _type'])).df = t
-00001510: 6162 6c65 2e74 6f5f 7061 6e64 6173 2829  able.to_pandas()
-00001520: 0a0a 746f 7461 6c5f 656c 656d 656e 7473  ..total_elements
-00001530: 203d 206c 656e 2864 6629 0a70 7269 6e74   = len(df).print
-00001540: 2866 2254 6f74 616c 2065 6c65 6d65 6e74  (f"Total element
-00001550: 7320 696e 2074 6865 2063 6174 616c 6f67  s in the catalog
-00001560: 3a20 7b74 6f74 616c 5f65 6c65 6d65 6e74  : {total_element
-00001570: 737d 2229 0a0a 6669 6c65 5f63 6f75 6e74  s}")..file_count
-00001580: 203d 2028 6466 5b27 656c 656d 656e 745f   = (df['element_
-00001590: 7479 7065 275d 203d 3d20 2746 494c 4527  type'] == 'FILE'
-000015a0: 292e 7375 6d28 290a 7072 696e 7428 6622  ).sum().print(f"
-000015b0: 4e75 6d62 6572 206f 6620 6669 6c65 732f  Number of files/
-000015c0: 6f62 6a65 6374 733a 207b 6669 6c65 5f63  objects: {file_c
-000015d0: 6f75 6e74 7d22 290a 0a64 6973 7469 6e63  ount}")..distinc
-000015e0: 745f 656c 656d 656e 7473 203d 2064 665b  t_elements = df[
-000015f0: 2765 6c65 6d65 6e74 5f74 7970 6527 5d2e  'element_type'].
-00001600: 756e 6971 7565 2829 0a70 7269 6e74 2822  unique().print("
-00001610: 4469 7374 696e 6374 2065 6c65 6d65 6e74  Distinct element
-00001620: 2074 7970 6573 206f 6e20 7468 6520 7379   types on the sy
-00001630: 7374 656d 3a22 290a 7072 696e 7428 6469  stem:").print(di
-00001640: 7374 696e 6374 5f65 6c65 6d65 6e74 7329  stinct_elements)
-00001650: 0a60 6060 0a0a 5365 6520 7468 6520 666f  .```..See the fo
-00001660: 6c6c 6f77 696e 6720 626c 6f67 2070 6f73  llowing blog pos
-00001670: 7473 2066 6f72 206d 6f72 6520 6578 616d  ts for more exam
-00001680: 706c 6573 3a0a 0a2d 2068 7474 7073 3a2f  ples:..- https:/
-00001690: 2f76 6173 7464 6174 612e 636f 6d2f 626c  /vastdata.com/bl
-000016a0: 6f67 2f74 6865 2d76 6173 742d 6361 7461  og/the-vast-cata
-000016b0: 6c6f 672d 696e 2d61 6374 696f 6e2d 7061  log-in-action-pa
-000016c0: 7274 2d31 0a2d 2068 7474 7073 3a2f 2f76  rt-1.- https://v
-000016d0: 6173 7464 6174 612e 636f 6d2f 626c 6f67  astdata.com/blog
-000016e0: 2f74 6865 2d76 6173 742d 6361 7461 6c6f  /the-vast-catalo
-000016f0: 672d 696e 2d61 6374 696f 6e2d 7061 7274  g-in-action-part
-00001700: 2d32 0a                                  -2.
+00000b30: 290a 6060 600a 0a53 6565 205b 6865 7265  ).```..See [here
+00000b40: 2066 6f72 206d 6f72 6520 6465 7461 696c   for more detail
+00000b50: 735d 2864 6f63 732f 7072 6564 6963 6174  s](docs/predicat
+00000b60: 652e 6d64 292e 0a0a 2323 2049 6d70 6f72  e.md)...## Impor
+00000b70: 7420 6120 7369 6e67 6c65 2050 6172 7175  t a single Parqu
+00000b80: 6574 2066 696c 6520 7669 6120 5333 2070  et file via S3 p
+00000b90: 726f 746f 636f 6c0a 0a49 7420 6973 2070  rotocol..It is p
+00000ba0: 6f73 7369 626c 6520 746f 2065 6666 6963  ossible to effic
+00000bb0: 6965 6e74 6c79 2063 7265 6174 6520 6120  iently create a 
+00000bc0: 7461 626c 6520 6672 6f6d 2061 2050 6172  table from a Par
+00000bd0: 7175 6574 2066 696c 6520 2877 6974 686f  quet file (witho
+00000be0: 7574 2063 6f70 7969 6e67 2069 7420 7669  ut copying it vi
+00000bf0: 6120 7468 6520 636c 6965 6e74 293a 0a0a  a the client):..
+00000c00: 6060 6070 7974 686f 6e0a 2020 2020 7769  ```python.    wi
+00000c10: 7468 2074 656d 7066 696c 652e 4e61 6d65  th tempfile.Name
+00000c20: 6454 656d 706f 7261 7279 4669 6c65 2829  dTemporaryFile()
+00000c30: 2061 7320 663a 0a20 2020 2020 2020 2070   as f:.        p
+00000c40: 612e 7061 7271 7565 742e 7772 6974 655f  a.parquet.write_
+00000c50: 7461 626c 6528 6172 726f 775f 7461 626c  table(arrow_tabl
+00000c60: 652c 2066 2e6e 616d 6529 0a20 2020 2020  e, f.name).     
+00000c70: 2020 2073 332e 7075 745f 6f62 6a65 6374     s3.put_object
+00000c80: 2842 7563 6b65 743d 2762 7563 6b65 742d  (Bucket='bucket-
+00000c90: 6e61 6d65 272c 204b 6579 3d27 7374 6167  name', Key='stag
+00000ca0: 696e 672f 6669 6c65 2e70 6172 7175 6574  ing/file.parquet
+00000cb0: 272c 2042 6f64 793d 6629 0a0a 2020 2020  ', Body=f)..    
+00000cc0: 7363 6865 6d61 203d 2074 782e 6275 636b  schema = tx.buck
+00000cd0: 6574 2827 6275 636b 6574 2d6e 616d 6527  et('bucket-name'
+00000ce0: 292e 7363 6865 6d61 2827 7363 6865 6d61  ).schema('schema
+00000cf0: 2d6e 616d 6527 290a 2020 2020 7461 626c  -name').    tabl
+00000d00: 6520 3d20 7574 696c 2e63 7265 6174 655f  e = util.create_
+00000d10: 7461 626c 655f 6672 6f6d 5f66 696c 6573  table_from_files
+00000d20: 280a 2020 2020 2020 2020 7363 6865 6d61  (.        schema
+00000d30: 3d73 6368 656d 612c 2074 6162 6c65 5f6e  =schema, table_n
+00000d40: 616d 653d 2769 6d70 6f72 7465 642d 7461  ame='imported-ta
+00000d50: 626c 6527 2c0a 2020 2020 2020 2020 7061  ble',.        pa
+00000d60: 7271 7565 745f 6669 6c65 733d 5b27 2f62  rquet_files=['/b
+00000d70: 7563 6b65 742d 6e61 6d65 2f73 7461 6769  ucket-name/stagi
+00000d80: 6e67 2f66 696c 652e 7061 7271 7565 7427  ng/file.parquet'
+00000d90: 5d29 0a60 6060 0a0a 2323 2049 6d70 6f72  ]).```..## Impor
+00000da0: 7420 6d75 6c74 6970 6c65 2050 6172 7175  t multiple Parqu
+00000db0: 6574 2066 696c 6573 2063 6f6e 6375 7272  et files concurr
+00000dc0: 656e 746c 7920 7669 6120 5333 2070 726f  ently via S3 pro
+00000dd0: 746f 636f 6c0a 0a57 6520 6361 6e20 696d  tocol..We can im
+00000de0: 706f 7274 206d 756c 7469 706c 6520 6669  port multiple fi
+00000df0: 6c65 7320 636f 6e63 7572 7265 6e74 6c79  les concurrently
+00000e00: 2069 6e74 6f20 6120 7461 626c 6520 2862   into a table (b
+00000e10: 7920 7574 696c 697a 696e 6720 6d75 6c74  y utilizing mult
+00000e20: 6970 6c65 2043 4e6f 6465 7327 2063 6f72  iple CNodes' cor
+00000e30: 6573 293a 0a0a 6060 6070 7974 686f 6e0a  es):..```python.
+00000e40: 2020 2020 7363 6865 6d61 203d 2074 782e      schema = tx.
+00000e50: 6275 636b 6574 2827 6275 636b 6574 2d6e  bucket('bucket-n
+00000e60: 616d 6527 292e 7363 6865 6d61 2827 7363  ame').schema('sc
+00000e70: 6865 6d61 2d6e 616d 6527 290a 2020 2020  hema-name').    
+00000e80: 7461 626c 6520 3d20 7574 696c 2e63 7265  table = util.cre
+00000e90: 6174 655f 7461 626c 655f 6672 6f6d 5f66  ate_table_from_f
+00000ea0: 696c 6573 280a 2020 2020 2020 2020 7363  iles(.        sc
+00000eb0: 6865 6d61 3d73 6368 656d 612c 2074 6162  hema=schema, tab
+00000ec0: 6c65 5f6e 616d 653d 276c 6172 6765 2d69  le_name='large-i
+00000ed0: 6d70 6f72 7465 642d 7461 626c 6527 2c0a  mported-table',.
+00000ee0: 2020 2020 2020 2020 7061 7271 7565 745f          parquet_
+00000ef0: 6669 6c65 733d 5b66 272f 6275 636b 6574  files=[f'/bucket
+00000f00: 2d6e 616d 652f 7374 6167 696e 672f 6669  -name/staging/fi
+00000f10: 6c65 7b69 7d2e 7061 7271 7565 7427 2066  le{i}.parquet' f
+00000f20: 6f72 2069 2069 6e20 7261 6e67 6528 3130  or i in range(10
+00000f30: 295d 290a 6060 600a 0a23 2320 506f 7374  )]).```..## Post
+00000f40: 2d70 726f 6365 7373 696e 670a 0a23 2323  -processing..###
+00000f50: 2045 7870 6f72 740a 0a60 5461 626c 652e   Export..`Table.
+00000f60: 7365 6c65 6374 2829 6020 7265 7475 726e  select()` return
+00000f70: 7320 6120 7374 7265 616d 206f 6620 5b50  s a stream of [P
+00000f80: 7941 7272 6f77 2072 6563 6f72 6420 6261  yArrow record ba
+00000f90: 7463 6865 735d 2868 7474 7073 3a2f 2f61  tches](https://a
+00000fa0: 7272 6f77 2e61 7061 6368 652e 6f72 672f  rrow.apache.org/
+00000fb0: 646f 6373 2f70 7974 686f 6e2f 6461 7461  docs/python/data
+00000fc0: 2e68 746d 6c23 7265 636f 7264 2d62 6174  .html#record-bat
+00000fd0: 6368 6573 292c 2077 6869 6368 2063 616e  ches), which can
+00000fe0: 2062 6520 6469 7265 6374 6c79 2065 7870   be directly exp
+00000ff0: 6f72 7465 6420 696e 746f 2061 2050 6172  orted into a Par
+00001000: 7175 6574 2066 696c 653a 0a0a 6060 6070  quet file:..```p
+00001010: 7974 686f 6e0a 6261 7463 6865 7320 3d20  ython.batches = 
+00001020: 7461 626c 652e 7365 6c65 6374 2829 0a77  table.select().w
+00001030: 6974 6820 636f 6e74 6578 746c 6962 2e63  ith contextlib.c
+00001040: 6c6f 7369 6e67 2870 612e 7061 7271 7565  losing(pa.parque
+00001050: 742e 5061 7271 7565 7457 7269 7465 7228  t.ParquetWriter(
+00001060: 272f 7061 7468 2f74 6f2f 6669 6c65 2e70  '/path/to/file.p
+00001070: 6172 7175 6574 272c 2062 6174 6368 6573  arquet', batches
+00001080: 2e73 6368 656d 6129 2920 6173 2077 7269  .schema)) as wri
+00001090: 7465 723a 0a20 2020 2066 6f72 2062 6174  ter:.    for bat
+000010a0: 6368 2069 6e20 7461 626c 655f 6261 7463  ch in table_batc
+000010b0: 6865 733a 0a20 2020 2020 2020 2077 7269  hes:.        wri
+000010c0: 7465 722e 7772 6974 655f 6261 7463 6828  ter.write_batch(
+000010d0: 6261 7463 6829 0a60 6060 0a0a 2323 2320  batch).```..### 
+000010e0: 4475 636b 4442 0a0a 5765 2063 616e 2075  DuckDB..We can u
+000010f0: 7365 205b 4475 636b 4442 5d28 6874 7470  se [DuckDB](http
+00001100: 733a 2f2f 6475 636b 6462 2e6f 7267 2f64  s://duckdb.org/d
+00001110: 6f63 732f 6775 6964 6573 2f70 7974 686f  ocs/guides/pytho
+00001120: 6e2f 7371 6c5f 6f6e 5f61 7272 6f77 2e68  n/sql_on_arrow.h
+00001130: 746d 6c29 2074 6f20 706f 7374 2d70 726f  tml) to post-pro
+00001140: 6365 7373 2074 6865 2072 6573 756c 7469  cess the resulti
+00001150: 6e67 2073 7472 6561 6d20 6f66 205b 5079  ng stream of [Py
+00001160: 4172 726f 7720 7265 636f 7264 2062 6174  Arrow record bat
+00001170: 6368 6573 5d28 6874 7470 733a 2f2f 6172  ches](https://ar
+00001180: 726f 772e 6170 6163 6865 2e6f 7267 2f64  row.apache.org/d
+00001190: 6f63 732f 7079 7468 6f6e 2f64 6174 612e  ocs/python/data.
+000011a0: 6874 6d6c 2372 6563 6f72 642d 6261 7463  html#record-batc
+000011b0: 6865 7329 3a0a 0a60 6060 7079 7468 6f6e  hes):..```python
+000011c0: 0a69 6d70 6f72 7420 6475 636b 6462 0a63  .import duckdb.c
+000011d0: 6f6e 6e20 3d20 6475 636b 6462 2e63 6f6e  onn = duckdb.con
+000011e0: 6e65 6374 2829 0a0a 6261 7463 6865 7320  nect()..batches 
+000011f0: 3d20 7461 626c 652e 7365 6c65 6374 2863  = table.select(c
+00001200: 6f6c 756d 6e73 3d5b 2763 3127 5d2c 2070  olumns=['c1'], p
+00001210: 7265 6469 6361 7465 3d28 7461 626c 655b  redicate=(table[
+00001220: 2763 3227 5d20 3e20 3229 290a 7072 696e  'c2'] > 2)).prin
+00001230: 7428 636f 6e6e 2e65 7865 6375 7465 2822  t(conn.execute("
+00001240: 5345 4c45 4354 2073 756d 2863 3129 2046  SELECT sum(c1) F
+00001250: 524f 4d20 6261 7463 6865 7322 292e 6172  ROM batches").ar
+00001260: 726f 7728 2929 0a60 6060 0a0a 2323 2053  row()).```..## S
+00001270: 656d 692d 736f 7274 6564 2070 726f 6a65  emi-sorted proje
+00001280: 6374 696f 6e73 0a0a 5765 2063 616e 2063  ctions..We can c
+00001290: 7265 6174 652c 206c 6973 7420 616e 6420  reate, list and 
+000012a0: 6465 6c65 7465 205b 6176 6169 6c61 626c  delete [availabl
+000012b0: 6520 7365 6d69 2d73 6f72 7465 6420 7072  e semi-sorted pr
+000012c0: 6f6a 6563 7469 6f6e 735d 2868 7474 7073  ojections](https
+000012d0: 3a2f 2f73 7570 706f 7274 2e76 6173 7464  ://support.vastd
+000012e0: 6174 612e 636f 6d2f 732f 6172 7469 636c  ata.com/s/articl
+000012f0: 652f 5555 4944 2d65 3463 6134 3261 622d  e/UUID-e4ca42ab-
+00001300: 6431 3562 2d36 6237 322d 6264 3662 2d66  d15b-6b72-bd6b-f
+00001310: 3363 3737 6234 3535 6465 3429 3a0a 0a60  3c77b455de4):..`
+00001320: 6060 7079 7468 6f6e 0a70 203d 2074 6162  ``python.p = tab
+00001330: 6c65 2e63 7265 6174 655f 7072 6f6a 6563  le.create_projec
+00001340: 7469 6f6e 2827 7072 6f6a 272c 2073 6f72  tion('proj', sor
+00001350: 7465 643d 5b27 6333 275d 2c20 756e 736f  ted=['c3'], unso
+00001360: 7274 6564 3d5b 2763 3127 5d29 0a70 7269  rted=['c1']).pri
+00001370: 6e74 2874 6162 6c65 2e70 726f 6a65 6374  nt(table.project
+00001380: 696f 6e73 2829 290a 7072 696e 7428 702e  ions()).print(p.
+00001390: 6765 745f 7374 6174 7328 2929 0a70 2e64  get_stats()).p.d
+000013a0: 726f 7028 290a 6060 600a 0a23 2320 536e  rop().```..## Sn
+000013b0: 6170 7368 6f74 730a 0a49 7420 6973 2070  apshots..It is p
+000013c0: 6f73 7369 626c 6520 746f 2075 7365 205b  ossible to use [
+000013d0: 736e 6170 7368 6f74 735d 2868 7474 7073  snapshots](https
+000013e0: 3a2f 2f76 6173 7464 6174 612e 636f 6d2f  ://vastdata.com/
+000013f0: 626c 6f67 2f62 7269 6e67 696e 672d 736e  blog/bringing-sn
+00001400: 6170 7368 6f74 732d 746f 2d76 6173 7473  apshots-to-vasts
+00001410: 2d65 6c65 6d65 6e74 2d73 746f 7265 2920  -element-store) 
+00001420: 666f 7220 6163 6365 7373 696e 6720 7468  for accessing th
+00001430: 6520 4461 7461 6261 7365 3a0a 0a60 6060  e Database:..```
+00001440: 7079 7468 6f6e 0a73 6e61 7073 203d 2062  python.snaps = b
+00001450: 7563 6b65 742e 6c69 7374 5f73 6e61 7073  ucket.list_snaps
+00001460: 686f 7473 2829 0a62 6174 6368 6573 203d  hots().batches =
+00001470: 2073 6e61 7073 5b30 5d2e 7363 6865 6d61   snaps[0].schema
+00001480: 2827 7363 6865 6d61 2d6e 616d 6527 292e  ('schema-name').
+00001490: 7461 626c 6528 2774 6162 6c65 2d6e 616d  table('table-nam
+000014a0: 6527 292e 7365 6c65 6374 2829 0a60 6060  e').select().```
+000014b0: 0a0a 2323 2056 4153 5420 4361 7461 6c6f  ..## VAST Catalo
+000014c0: 670a 0a5b 5641 5354 2043 6174 616c 6f67  g..[VAST Catalog
+000014d0: 5d28 6874 7470 733a 2f2f 7661 7374 6461  ](https://vastda
+000014e0: 7461 2e63 6f6d 2f62 6c6f 672f 7661 7374  ta.com/blog/vast
+000014f0: 2d63 6174 616c 6f67 2d74 7265 6174 2d79  -catalog-treat-y
+00001500: 6f75 722d 6669 6c65 2d73 7973 7465 6d2d  our-file-system-
+00001510: 6c69 6b65 2d61 2d64 6174 6162 6173 6529  like-a-database)
+00001520: 2063 616e 2062 6520 7175 6572 6965 6420   can be queried 
+00001530: 6173 2061 2072 6567 756c 6172 2074 6162  as a regular tab
+00001540: 6c65 3a0a 0a60 6060 7079 7468 6f6e 0a74  le:..```python.t
+00001550: 6162 6c65 203d 2070 612e 5461 626c 652e  able = pa.Table.
+00001560: 6672 6f6d 5f62 6174 6368 6573 2874 782e  from_batches(tx.
+00001570: 6361 7461 6c6f 672e 7365 6c65 6374 285b  catalog.select([
+00001580: 2765 6c65 6d65 6e74 5f74 7970 6527 5d29  'element_type'])
+00001590: 290a 6466 203d 2074 6162 6c65 2e74 6f5f  ).df = table.to_
+000015a0: 7061 6e64 6173 2829 0a0a 746f 7461 6c5f  pandas()..total_
+000015b0: 656c 656d 656e 7473 203d 206c 656e 2864  elements = len(d
+000015c0: 6629 0a70 7269 6e74 2866 2254 6f74 616c  f).print(f"Total
+000015d0: 2065 6c65 6d65 6e74 7320 696e 2074 6865   elements in the
+000015e0: 2063 6174 616c 6f67 3a20 7b74 6f74 616c   catalog: {total
+000015f0: 5f65 6c65 6d65 6e74 737d 2229 0a0a 6669  _elements}")..fi
+00001600: 6c65 5f63 6f75 6e74 203d 2028 6466 5b27  le_count = (df['
+00001610: 656c 656d 656e 745f 7479 7065 275d 203d  element_type'] =
+00001620: 3d20 2746 494c 4527 292e 7375 6d28 290a  = 'FILE').sum().
+00001630: 7072 696e 7428 6622 4e75 6d62 6572 206f  print(f"Number o
+00001640: 6620 6669 6c65 732f 6f62 6a65 6374 733a  f files/objects:
+00001650: 207b 6669 6c65 5f63 6f75 6e74 7d22 290a   {file_count}").
+00001660: 0a64 6973 7469 6e63 745f 656c 656d 656e  .distinct_elemen
+00001670: 7473 203d 2064 665b 2765 6c65 6d65 6e74  ts = df['element
+00001680: 5f74 7970 6527 5d2e 756e 6971 7565 2829  _type'].unique()
+00001690: 0a70 7269 6e74 2822 4469 7374 696e 6374  .print("Distinct
+000016a0: 2065 6c65 6d65 6e74 2074 7970 6573 206f   element types o
+000016b0: 6e20 7468 6520 7379 7374 656d 3a22 290a  n the system:").
+000016c0: 7072 696e 7428 6469 7374 696e 6374 5f65  print(distinct_e
+000016d0: 6c65 6d65 6e74 7329 0a60 6060 0a0a 5365  lements).```..Se
+000016e0: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
+000016f0: 626c 6f67 2070 6f73 7473 2066 6f72 206d  blog posts for m
+00001700: 6f72 6520 6578 616d 706c 6573 3a0a 0a2d  ore examples:..-
+00001710: 2068 7474 7073 3a2f 2f76 6173 7464 6174   https://vastdat
+00001720: 612e 636f 6d2f 626c 6f67 2f74 6865 2d76  a.com/blog/the-v
+00001730: 6173 742d 6361 7461 6c6f 672d 696e 2d61  ast-catalog-in-a
+00001740: 6374 696f 6e2d 7061 7274 2d31 0a2d 2068  ction-part-1.- h
+00001750: 7474 7073 3a2f 2f76 6173 7464 6174 612e  ttps://vastdata.
+00001760: 636f 6d2f 626c 6f67 2f74 6865 2d76 6173  com/blog/the-vas
+00001770: 742d 6361 7461 6c6f 672d 696e 2d61 6374  t-catalog-in-act
+00001780: 696f 6e2d 7061 7274 2d32 0a              ion-part-2.
```

### Comparing `vastdb-0.1.2/setup.py` & `vastdb-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 if os.environ.get('VASTDB_APPEND_VERSION_SUFFIX'):
     suffix = _get_version_suffix()
 
 setup(
     name='vastdb',
     python_requires='>=3.9.0',
     description='VAST Data SDK',
-    version='0.1.2' + suffix,
+    version='0.1.3' + suffix,
     url='https://github.com/vast-data/vastdb_sdk',
     author='VAST DATA',
     author_email='hello@vastdata.com',
     license='Copyright (C) VAST Data Ltd.',
     packages=find_packages(),
     install_requires=open('requirements.txt').read().strip().split('\n'),
     long_description=long_description,
```

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Aggregate.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySlice.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ArraySubscript.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BinaryLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/BooleanLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Call.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CaseFragment.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Cast.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ConditionalCase.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/CurrentRow.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DateLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DecimalLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/DurationLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Expression.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldIndex.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FieldRef.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Filter.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/FixedSizeBinaryLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float16Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float32Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Float64Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Following.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Grouping.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int16Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int32Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int64Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Int8Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralDaysMilliseconds.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/IntervalLiteralMonths.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Join.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/KeyValue.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Limit.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/ListLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralColumn.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralImpl.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/LiteralRelation.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapKey.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/MapLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/OrderBy.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Plan.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Preceding.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Project.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/RelId.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Relation.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SetOperation.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SimpleCase.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/SortKey.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Source.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StringLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructField.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/StructLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimeLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/TimestampLiteral.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt16Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt32Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt64Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/UInt8Literal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/Unbounded.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/computeir/flatbuf/WindowCall.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Binary.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Block.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Block.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompression.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/BodyCompressionMethod.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Bool.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Buffer.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Date.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Date.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Decimal.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryBatch.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/DictionaryEncoding.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Duration.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Feature.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Field.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Field.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/FieldNode.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeBinary.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/FixedSizeList.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/FloatingPoint.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Footer.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Int.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Int.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Interval.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/KeyValue.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/LargeBinary.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/LargeList.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/LargeUtf8.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/List.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/List.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Map.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Map.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Message.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Message.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/MessageHeader.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/MetadataVersion.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Null.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Null.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/RecordBatch.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Schema.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseMatrixIndexCSX.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensor.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCOO.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/SparseTensorIndexCSF.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Struct_.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Tensor.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/TensorDim.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Time.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Time.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Timestamp.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Type.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Type.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Union.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Union.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py` & `vastdb-0.1.3/vast_flatbuf/org/apache/arrow/flatbuf/Utf8.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/tabular/AlterColumnRequest.py` & `vastdb-0.1.3/vast_flatbuf/tabular/AlterColumnRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/tabular/AlterProjectionTableRequest.py` & `vastdb-0.1.3/vast_flatbuf/tabular/AlterProjectionTableRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/tabular/AlterSchemaRequest.py` & `vastdb-0.1.3/vast_flatbuf/tabular/AlterSchemaRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/tabular/AlterTableRequest.py` & `vastdb-0.1.3/vast_flatbuf/tabular/AlterTableRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/tabular/Column.py` & `vastdb-0.1.3/vast_flatbuf/tabular/Column.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/tabular/CreateProjectionRequest.py` & `vastdb-0.1.3/vast_flatbuf/tabular/CreateProjectionRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/tabular/CreateSchemaRequest.py` & `vastdb-0.1.3/vast_flatbuf/tabular/CreateSchemaRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py` & `vastdb-0.1.3/vast_flatbuf/tabular/GetProjectionTableStatsResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/tabular/GetTableStatsResponse.py` & `vastdb-0.1.3/vast_flatbuf/tabular/GetTableStatsResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/tabular/ImportDataRequest.py` & `vastdb-0.1.3/vast_flatbuf/tabular/ImportDataRequest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/tabular/ListProjectionsResponse.py` & `vastdb-0.1.3/vast_flatbuf/tabular/ListProjectionsResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/tabular/ListSchemasResponse.py` & `vastdb-0.1.3/vast_flatbuf/tabular/ListSchemasResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/tabular/ListTablesResponse.py` & `vastdb-0.1.3/vast_flatbuf/tabular/ListTablesResponse.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/tabular/ObjectDetails.py` & `vastdb-0.1.3/vast_flatbuf/tabular/ObjectDetails.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/tabular/S3File.py` & `vastdb-0.1.3/vast_flatbuf/tabular/S3File.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vast_flatbuf/tabular/VipRange.py` & `vastdb-0.1.3/vast_flatbuf/tabular/VipRange.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vastdb/bench/test_perf.py` & `vastdb-0.1.3/vastdb/bench/test_perf.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vastdb/bucket.py` & `vastdb-0.1.3/vastdb/bucket.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,22 +13,14 @@
 if TYPE_CHECKING:
     from .schema import Schema
 
 log = logging.getLogger(__name__)
 
 
 @dataclass
-class Snapshot:
-    """VAST bucket-level snapshot."""
-
-    name: str
-    bucket: "Bucket"
-
-
-@dataclass
 class Bucket:
     """VAST bucket."""
 
     name: str
     tx: "transaction.Transaction"
 
     def create_schema(self, path: str, fail_if_exists=True) -> "Schema":
@@ -69,21 +61,39 @@
                 break
             schemas.extend(curr_schemas)
             if not is_truncated:
                 break
 
         return [schema.Schema(name=name, bucket=self) for name, *_ in schemas]
 
-    def snapshots(self) -> List[Snapshot]:
+    def snapshot(self, name, fail_if_missing=True) -> Optional["Bucket"]:
+        """Get snapshot by name (if exists)."""
+        snapshots, _is_truncated, _next_key = \
+            self.tx._rpc.api.list_snapshots(bucket=self.name, name_prefix=name, max_keys=1)
+
+        expected_name = f".snapshot/{name}"
+        exists = snapshots and snapshots[0] == expected_name + "/"
+        if not exists:
+            if fail_if_missing:
+                raise errors.MissingSnapshot(self.name, expected_name)
+            else:
+                return None
+
+        return Bucket(name=f'{self.name}/{expected_name}', tx=self.tx)
+
+    def snapshots(self) -> List["Bucket"]:
         """List bucket's snapshots."""
         snapshots = []
         next_key = 0
         while True:
             curr_snapshots, is_truncated, next_key = \
                 self.tx._rpc.api.list_snapshots(bucket=self.name, next_token=next_key)
             if not curr_snapshots:
                 break
             snapshots.extend(curr_snapshots)
             if not is_truncated:
                 break
 
-        return [Snapshot(name=snapshot, bucket=self) for snapshot in snapshots]
+        return [
+            Bucket(name=f'{self.name}/{snapshot.strip("/")}', tx=self.tx)
+            for snapshot in snapshots
+        ]
```

### Comparing `vastdb-0.1.2/vastdb/conftest.py` & `vastdb-0.1.3/vastdb/conftest.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vastdb/errors.py` & `vastdb-0.1.3/vastdb/errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,28 +81,42 @@
     error_dict: dict
 
 
 class InvalidArgument(Exception):
     pass
 
 
+class TooWideRow(InvalidArgument):
+    pass
+
+
 class Missing(Exception):
     pass
 
 
 class MissingTransaction(Missing):
     pass
 
 
+class NotSupported(Exception):
+    pass
+
+
 @dataclass
 class MissingBucket(Missing):
     bucket: str
 
 
 @dataclass
+class MissingSnapshot(Missing):
+    bucket: str
+    snapshot: str
+
+
+@dataclass
 class MissingSchema(Missing):
     bucket: str
     schema: str
 
 
 @dataclass
 class MissingTable(Missing):
@@ -132,14 +146,27 @@
 @dataclass
 class TableExists(Exists):
     bucket: str
     schema: str
     table: str
 
 
+@dataclass
+class NotSupportedCommand(NotSupported):
+    bucket: str
+    schema: str
+    table: str
+
+
+@dataclass
+class NotSupportedVersion(NotSupported):
+    err_msg: str
+    version: str
+
+
 ERROR_TYPES_MAP = {
     HttpStatus.BAD_REQUEST: BadRequest,
     HttpStatus.FOBIDDEN: Forbidden,
     HttpStatus.NOT_FOUND: NotFound,
     HttpStatus.METHOD_NOT_ALLOWED: MethodNotAllowed,
     HttpStatus.REQUEST_TIMEOUT: RequestTimeout,
     HttpStatus.CONFLICT: Conflict,
@@ -174,8 +201,8 @@
         url=res.request.url,
         status=res.status_code,
         headers=res.headers,
     )
     log.warning("RPC failed: %s", kwargs)
     status = HttpStatus(res.status_code)
     error_type = ERROR_TYPES_MAP.get(status, UnexpectedError)
-    raise error_type(**kwargs)
+    return error_type(**kwargs)
```

### Comparing `vastdb-0.1.2/vastdb/internal_commands.py` & `vastdb-0.1.3/vastdb/internal_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import itertools
 import json
 import logging
-import math
 import re
 import struct
 import urllib.parse
 from collections import defaultdict, namedtuple
 from enum import Enum
 from ipaddress import IPv4Address, IPv6Address
 from typing import Any, Dict, Iterator, List, Optional, Union
@@ -178,14 +177,15 @@
             TableColumn,
         )
         from ibis.expr.operations.logical import (
             And,
             Equals,
             Greater,
             GreaterEqual,
+            InValues,
             Less,
             LessEqual,
             Not,
             NotEquals,
             Or,
         )
         from ibis.expr.operations.strings import StringContains
@@ -215,48 +215,62 @@
                 or_args = list(_flatten_args(op, Or))
                 _logger.debug('OR args: %s op %s', or_args, op)
                 inner_offsets = []
 
                 prev_field_name = None
                 for inner_op in or_args:
                     _logger.debug('inner_op %s', inner_op)
-                    builder_func: Any = builder_map.get(type(inner_op))
+                    op_type = type(inner_op)
+                    builder_func: Any = builder_map.get(op_type)
                     if not builder_func:
-                        raise NotImplementedError(inner_op.name)
+                        if op_type == InValues:
+                            builder_func = self.build_equal
+                        else:
+                            raise NotImplementedError(self.expr)
 
                     if builder_func == self.build_is_null:
                         column, = inner_op.args
-                        literal = None
+                        literals = (None,)
                     elif builder_func == self.build_is_not_null:
                         not_arg, = inner_op.args
                         # currently we only support not is_null, checking we really got is_null under the not:
                         if not builder_map.get(type(not_arg)) == self.build_is_null:
-                            raise NotImplementedError(not_arg.args[0].name)
+                            raise NotImplementedError(self.expr)
                         column, = not_arg.args
-                        literal = None
+                        literals = (None,)
                     else:
-                        column, literal = inner_op.args
-                        if not isinstance(literal, Literal):
-                            raise NotImplementedError(inner_op.name)
+                        column, arg = inner_op.args
+                        if isinstance(arg, tuple):
+                            literals = arg
+                        else:
+                            literals = (arg,)
+                        for literal in literals:
+                            if not isinstance(literal, Literal):
+                                raise NotImplementedError(self.expr)
 
                     if not isinstance(column, TableColumn):
-                        raise NotImplementedError(inner_op.name)
+                        raise NotImplementedError(self.expr)
 
                     field_name = column.name
                     if prev_field_name is None:
                         prev_field_name = field_name
                     elif prev_field_name != field_name:
-                        raise NotImplementedError(op.name)
+                        raise NotImplementedError(self.expr)
 
-                    args_offsets = [self.build_column(position=positions_map[field_name])]
-                    if literal:
-                        field = self.schema.field(field_name)
-                        args_offsets.append(self.build_literal(field=field, value=literal.value))
+                    column_offset = self.build_column(position=positions_map[field_name])
+                    field = self.schema.field(field_name)
+                    for literal in literals:
+                        args_offsets = [column_offset]
+                        if literal is not None:
+                            args_offsets.append(self.build_literal(field=field, value=literal.value))
 
-                    inner_offsets.append(builder_func(*args_offsets))
+                        inner_offsets.append(builder_func(*args_offsets))
+
+                if not inner_offsets:
+                    raise NotImplementedError(self.expr)  # an empty OR is equivalent to a 'FALSE' literal
 
                 domain_offset = self.build_or(inner_offsets)
                 offsets.append(domain_offset)
 
         return self.build_and(offsets)
 
     def build_column(self, position: int):
@@ -715,28 +729,14 @@
     properties = obj.Properties().decode()
     handle = obj.Handle().decode()
     num_rows = obj.NumRows()
     used_bytes = obj.SizeInBytes()
     return TableInfo(name, properties, handle, num_rows, used_bytes)
 
 
-def build_record_batch(column_info, column_values):
-    fields = [pa.field(column_name, column_type) for column_type, column_name in column_info]
-    schema = pa.schema(fields)
-    arrays = [pa.array(column_values[column_type], type=column_type) for column_type, _ in column_info]
-    batch = pa.record_batch(arrays, schema)
-    return serialize_record_batch(batch)
-
-
-def serialize_record_batch(batch):
-    sink = pa.BufferOutputStream()
-    with pa.ipc.new_stream(sink, batch.schema) as writer:
-        writer.write(batch)
-    return sink.getvalue()
-
 # Results that returns from tablestats
 
 
 TableStatsResult = namedtuple("TableStatsResult", ["num_rows", "size_in_bytes", "is_external_rowid_alloc", "endpoints"])
 
 
 class VastdbApi:
@@ -948,34 +948,35 @@
                 schema_obj = lists.Schemas(i)
                 name = schema_obj.Name().decode()
                 properties = schema_obj.Properties().decode()
                 schemas.append([name, properties])
 
             return bucket_name, schemas, next_key, is_truncated, count
 
-    def list_snapshots(self, bucket, max_keys=1000, next_token=None, expected_retvals=None):
+    def list_snapshots(self, bucket, max_keys=1000, next_token=None, name_prefix=''):
         next_token = next_token or ''
-        expected_retvals = expected_retvals or []
-        url_params = {'list_type': '2', 'prefix': '.snapshot/', 'delimiter': '/', 'max_keys': str(max_keys)}
+        url_params = {'list_type': '2', 'prefix': '.snapshot/' + name_prefix, 'delimiter': '/', 'max_keys': str(max_keys)}
         if next_token:
             url_params['continuation-token'] = next_token
 
         res = self.session.get(self._api_prefix(bucket=bucket, command="list", url_params=url_params), headers={}, stream=True)
-        self._check_res(res, "list_snapshots", expected_retvals)
-        if res.status_code == 200:
-            out = b''.join(res.iter_content(chunk_size=128))
-            xml_str = out.decode()
-            xml_dict = xmltodict.parse(xml_str)
-            list_res = xml_dict['ListBucketResult']
-            is_truncated = list_res['IsTruncated'] == 'true'
-            marker = list_res['Marker']
-            common_prefixes = list_res['CommonPrefixes'] if 'CommonPrefixes' in list_res else []
-            snapshots = [v['Prefix'] for v in common_prefixes]
+        self._check_res(res, "list_snapshots")
 
-            return snapshots, is_truncated, marker
+        out = b''.join(res.iter_content(chunk_size=128))
+        xml_str = out.decode()
+        xml_dict = xmltodict.parse(xml_str)
+        list_res = xml_dict['ListBucketResult']
+        is_truncated = list_res['IsTruncated'] == 'true'
+        marker = list_res['Marker']
+        common_prefixes = list_res.get('CommonPrefixes', [])
+        if isinstance(common_prefixes, dict):  # in case there is a single snapshot
+            common_prefixes = [common_prefixes]
+        snapshots = [v['Prefix'] for v in common_prefixes]
+
+        return snapshots, is_truncated, marker
 
     def create_table(self, bucket, schema, name, arrow_schema, txid=0, client_tags=[], expected_retvals=[],
                      topic_partitions=0, create_imports_table=False, use_external_row_ids_allocation=False):
         """
         Create a table, use the following request
         POST /bucket/schema/table?table HTTP/1.1
 
@@ -1026,24 +1027,25 @@
             arrow_schema = parquet_ds.schema
         else:
             raise RuntimeError(f'invalid type(parquet_ds.schema) = {type(parquet_ds.schema)}')
 
         # create the table
         return self.create_table(bucket, schema, name, arrow_schema, txid, client_tags, expected_retvals)
 
-    def get_table_stats(self, bucket, schema, name, txid=0, client_tags=[], expected_retvals=[]):
+    def get_table_stats(self, bucket, schema, name, txid=0, client_tags=[], expected_retvals=[], imports_table_stats=False):
         """
         GET /mybucket/myschema/mytable?stats HTTP/1.1
         tabular-txid: TransactionId
         tabular-client-tag: ClientTag
 
         The Command will return the statistics in flatbuf format
         """
         headers = self._fill_common_headers(txid=txid, client_tags=client_tags)
-        res = self.session.get(self._api_prefix(bucket=bucket, schema=schema, table=name, command="stats"), headers=headers)
+        url_params = {'sub-table': IMPORTED_OBJECTS_TABLE_NAME} if imports_table_stats else {}
+        res = self.session.get(self._api_prefix(bucket=bucket, schema=schema, table=name, command="stats", url_params=url_params), headers=headers)
         self._check_res(res, "get_table_stats", expected_retvals)
 
         flatbuf = b''.join(res.iter_content(chunk_size=128))
         stats = get_table_stats.GetRootAs(flatbuf)
         num_rows = stats.NumRows()
         size_in_bytes = stats.SizeInBytes()
         is_external_rowid_alloc = stats.IsExternalRowidAlloc()
@@ -1523,19 +1525,26 @@
         builder.Finish(params)
         import_req = builder.Output()
 
         def iterate_over_import_data_response(response):
             if response.status_code != 200:
                 return response
 
+            ALLOWED_IMPORT_STATES = {
+                'Success',
+                'TabularInProgress',
+                'TabularAlreadyImported',
+                'TabularImportNotStarted',
+            }
+
             chunk_size = 1024
             for chunk in response.iter_content(chunk_size=chunk_size):
                 chunk_dict = json.loads(chunk)
                 _logger.debug("import data chunk=%s, result: %s", chunk_dict, chunk_dict['res'])
-                if chunk_dict['res'] != 'Success' and chunk_dict['res'] != 'TabularInProgress' and chunk_dict['res'] != 'TabularAlreadyImported':
+                if chunk_dict['res'] not in ALLOWED_IMPORT_STATES:
                     raise errors.ImportFilesError(
                         f"Encountered an error during import_data. status: {chunk_dict['res']}, "
                         f"error message: {chunk_dict['err_msg'] or 'Unexpected error'} during import of "
                         f"object name: {chunk_dict['object_name']}", chunk_dict)
                 else:
                     _logger.debug("import_data of object name '%s' is in progress. "
                                   "status: %s", chunk_dict['object_name'], chunk_dict['res'])
@@ -1551,56 +1560,14 @@
         res = self.session.post(self._api_prefix(bucket=bucket, schema=schema, table=table, command="data"),
                                 data=import_req, headers=headers, stream=True)
         if blocking:
             res = iterate_over_import_data_response(res)
 
         return self._check_res(res, "import_data", expected_retvals)
 
-    def _record_batch_slices(self, batch, rows_per_slice=None):
-        max_slice_size_in_bytes = int(0.9 * 5 * 1024 * 1024)  # 0.9 * 5MB
-        batch_len = len(batch)
-        serialized_batch = serialize_record_batch(batch)
-        batch_size_in_bytes = len(serialized_batch)
-        _logger.debug('max_slice_size_in_bytes=%d batch_len=%d batch_size_in_bytes=%d',
-                      max_slice_size_in_bytes, batch_len, batch_size_in_bytes)
-
-        if not rows_per_slice:
-            if batch_size_in_bytes < max_slice_size_in_bytes:
-                rows_per_slice = batch_len
-            else:
-                rows_per_slice = int(0.9 * batch_len * max_slice_size_in_bytes / batch_size_in_bytes)
-
-        done_slicing = False
-        while not done_slicing:
-            # Attempt slicing according to the current rows_per_slice
-            offset = 0
-            serialized_slices = []
-            for i in range(math.ceil(batch_len / rows_per_slice)):
-                offset = rows_per_slice * i
-                if offset >= batch_len:
-                    done_slicing = True
-                    break
-                slice_batch = batch.slice(offset, rows_per_slice)
-                serialized_slice_batch = serialize_record_batch(slice_batch)
-                sizeof_serialized_slice_batch = len(serialized_slice_batch)
-
-                if sizeof_serialized_slice_batch <= max_slice_size_in_bytes:
-                    serialized_slices.append(serialized_slice_batch)
-                else:
-                    _logger.info(f'Using rows_per_slice {rows_per_slice} slice {i} size {sizeof_serialized_slice_batch} exceeds {max_slice_size_in_bytes} bytes, trying smaller rows_per_slice')
-                    # We have a slice that is too large
-                    rows_per_slice = int(rows_per_slice / 2)
-                    if rows_per_slice < 1:
-                        raise ValueError('cannot decrease batch size below 1 row')
-                    break
-            else:
-                done_slicing = True
-
-        return serialized_slices
-
     def insert_rows(self, bucket, schema, table, record_batch, txid=0, client_tags=[], expected_retvals=[]):
         """
         POST /mybucket/myschema/mytable?rows HTTP/1.1
         Content-Length: ContentLength
         tabular-txid: TransactionId
         tabular-client-tag: ClientTag
```

### Comparing `vastdb-0.1.2/vastdb/schema.py` & `vastdb-0.1.3/vastdb/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,8 +83,8 @@
         self.tx._rpc.api.alter_schema(self.bucket.name, self.name, txid=self.tx.txid, new_name=new_name)
         log.info("Renamed schema: %s to %s", self.name, new_name)
         self.name = new_name
 
 
 def _parse_table_info(table_info, schema: "schema.Schema"):
     stats = table.TableStats(num_rows=table_info.num_rows, size_in_bytes=table_info.size_in_bytes)
-    return table.Table(name=table_info.name, schema=schema, handle=int(table_info.handle), stats=stats)
+    return table.Table(name=table_info.name, schema=schema, handle=int(table_info.handle), stats=stats, _imports_table=False)
```

### Comparing `vastdb-0.1.2/vastdb/table.py` & `vastdb-0.1.3/vastdb/table.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,142 +1,169 @@
+"""VAST Database table."""
+
 import concurrent.futures
 import logging
 import os
 import queue
 from dataclasses import dataclass, field
 from math import ceil
 from threading import Event
 from typing import Dict, List, Optional, Tuple, Union
 
 import ibis
 import pyarrow as pa
 
-from . import errors, internal_commands, schema
+from . import errors, internal_commands, schema, util
 
 log = logging.getLogger(__name__)
 
 
 INTERNAL_ROW_ID = "$row_id"
 MAX_ROWS_PER_BATCH = 512 * 1024
 # for insert we need a smaller limit due to response amplification
 # for example insert of 512k uint8 result in 512k*8bytes response since row_ids are uint64
 MAX_INSERT_ROWS_PER_PATCH = 512 * 1024
 
 
 @dataclass
 class TableStats:
+    """Table-related information."""
+
     num_rows: int
     size_in_bytes: int
     is_external_rowid_alloc: bool = False
     endpoints: Tuple[str, ...] = ()
 
 
 @dataclass
 class QueryConfig:
+    """Query execution configiration."""
+
     num_sub_splits: int = 4
     num_splits: int = 1
     data_endpoints: Optional[List[str]] = None
     limit_rows_per_sub_split: int = 128 * 1024
     num_row_groups_per_sub_split: int = 8
     use_semi_sorted_projections: bool = True
     rows_per_split: int = 4000000
     query_id: str = ""
 
 
 @dataclass
 class ImportConfig:
+    """Import execution configiration."""
+
     import_concurrency: int = 2
 
 
-class SelectSplitState():
+class SelectSplitState:
+    """State of a specific query split execution."""
+
     def __init__(self, query_data_request, table: "Table", split_id: int, config: QueryConfig) -> None:
+        """Initialize query split state."""
         self.split_id = split_id
         self.subsplits_state = {i: 0 for i in range(config.num_sub_splits)}
         self.config = config
         self.query_data_request = query_data_request
         self.table = table
 
     def batches(self, api: internal_commands.VastdbApi):
+        """Execute QueryData request, and yield parsed RecordBatch objects.
+
+        Can be called repeatedly, to allow pagination.
+        """
         while not self.done:
             response = api.query_data(
                             bucket=self.table.bucket.name,
                             schema=self.table.schema.name,
                             table=self.table.name,
                             params=self.query_data_request.serialized,
                             split=(self.split_id, self.config.num_splits, self.config.num_row_groups_per_sub_split),
                             num_sub_splits=self.config.num_sub_splits,
                             response_row_id=False,
                             txid=self.table.tx.txid,
                             limit_rows=self.config.limit_rows_per_sub_split,
                             sub_split_start_row_ids=self.subsplits_state.items(),
-                            enable_sorted_projections=self.config.use_semi_sorted_projections)
+                            enable_sorted_projections=self.config.use_semi_sorted_projections,
+                            query_imports_table=self.table._imports_table)
             pages_iter = internal_commands.parse_query_data_response(
                 conn=response.raw,
                 schema=self.query_data_request.response_schema,
                 start_row_ids=self.subsplits_state,
                 parser=self.query_data_request.response_parser)
 
             for page in pages_iter:
                 for batch in page.to_batches():
                     if len(batch) > 0:
                         yield batch
 
     @property
     def done(self):
+        """Returns true iff the pagination over."""
         return all(row_id == internal_commands.TABULAR_INVALID_ROW_ID for row_id in self.subsplits_state.values())
 
 
 @dataclass
 class Table:
+    """VAST Table."""
+
     name: str
     schema: "schema.Schema"
     handle: int
     stats: TableStats
-    arrow_schema: pa.Schema = field(init=False, compare=False)
-    _ibis_table: ibis.Schema = field(init=False, compare=False)
+    arrow_schema: pa.Schema = field(init=False, compare=False, repr=False)
+    _ibis_table: ibis.Schema = field(init=False, compare=False, repr=False)
+    _imports_table: bool
 
     def __post_init__(self):
+        """Also, load columns' metadata."""
         self.arrow_schema = self.columns()
 
         table_path = f'{self.schema.bucket.name}/{self.schema.name}/{self.name}'
         self._ibis_table = ibis.table(ibis.Schema.from_pyarrow(self.arrow_schema), table_path)
 
     @property
     def tx(self):
+        """Return transaction."""
         return self.schema.tx
 
     @property
     def bucket(self):
+        """Return bucket."""
         return self.schema.bucket
 
-    def __repr__(self):
-        return f"{type(self).__name__}(name={self.name})"
-
     def columns(self) -> pa.Schema:
+        """Return columns' metadata."""
         fields = []
         next_key = 0
         while True:
             cur_columns, next_key, is_truncated, _count = self.tx._rpc.api.list_columns(
-                bucket=self.bucket.name, schema=self.schema.name, table=self.name, next_key=next_key, txid=self.tx.txid)
+                bucket=self.bucket.name, schema=self.schema.name, table=self.name, next_key=next_key, txid=self.tx.txid, list_imports_table=self._imports_table)
             fields.extend(cur_columns)
             if not is_truncated:
                 break
 
         self.arrow_schema = pa.schema(fields)
         return self.arrow_schema
 
     def projection(self, name: str) -> "Projection":
+        """Get a specific semi-sorted projection of this table."""
+        if self._imports_table:
+            raise errors.NotSupportedCommand(self.bucket.name, self.schema.name, self.name)
         projs = self.projections(projection_name=name)
         if not projs:
             raise errors.MissingProjection(self.bucket.name, self.schema.name, self.name, name)
         assert len(projs) == 1, f"Expected to receive only a single projection, but got: {len(projs)}. projections: {projs}"
         log.debug("Found projection: %s", projs[0])
         return projs[0]
 
     def projections(self, projection_name=None) -> List["Projection"]:
+        """List all semi-sorted projections of this table."""
+        if self._imports_table:
+            raise errors.NotSupportedCommand(self.bucket.name, self.schema.name, self.name)
         projections = []
         next_key = 0
         name_prefix = projection_name if projection_name else ""
         exact_match = bool(projection_name)
         while True:
             _bucket_name, _schema_name, _table_name, curr_projections, next_key, is_truncated, _ = \
                 self.tx._rpc.api.list_projections(
@@ -146,22 +173,35 @@
                 break
             projections.extend(curr_projections)
             if not is_truncated:
                 break
         return [_parse_projection_info(projection, self) for projection in projections]
 
     def import_files(self, files_to_import: List[str], config: Optional[ImportConfig] = None) -> None:
+        """Import a list of Parquet files into this table.
+
+        The files must be on VAST S3 server and be accessible using current credentials.
+        """
+        if self._imports_table:
+            raise errors.NotSupportedCommand(self.bucket.name, self.schema.name, self.name)
         source_files = {}
         for f in files_to_import:
             bucket_name, object_path = _parse_bucket_and_object_names(f)
             source_files[(bucket_name, object_path)] = b''
 
         self._execute_import(source_files, config=config)
 
     def import_partitioned_files(self, files_and_partitions: Dict[str, pa.RecordBatch], config: Optional[ImportConfig] = None) -> None:
+        """Import a list of Parquet files into this table.
+
+        The files must be on VAST S3 server and be accessible using current credentials.
+        Each file must have its own partition values defined as an Arrow RecordBatch.
+        """
+        if self._imports_table:
+            raise errors.NotSupportedCommand(self.bucket.name, self.schema.name, self.name)
         source_files = {}
         for f, record_batch in files_and_partitions.items():
             bucket_name, object_path = _parse_bucket_and_object_names(f)
             serialized_batch = _serialize_record_batch(record_batch)
             source_files = {(bucket_name, object_path): serialized_batch.to_pybytes()}
 
         self._execute_import(source_files, config=config)
@@ -212,23 +252,33 @@
                 for future in concurrent.futures.as_completed(futures):
                     future.result()
             finally:
                 stop_event.set()
                 # ThreadPoolExecutor will be joined at the end of the context
 
     def get_stats(self) -> TableStats:
+        """Get the statistics of this table."""
         stats_tuple = self.tx._rpc.api.get_table_stats(
-            bucket=self.bucket.name, schema=self.schema.name, name=self.name, txid=self.tx.txid)
+            bucket=self.bucket.name, schema=self.schema.name, name=self.name, txid=self.tx.txid,
+            imports_table_stats=self._imports_table)
         return TableStats(**stats_tuple._asdict())
 
     def select(self, columns: Optional[List[str]] = None,
                predicate: ibis.expr.types.BooleanColumn = None,
                config: Optional[QueryConfig] = None,
                *,
                internal_row_id: bool = False) -> pa.RecordBatchReader:
+        """Execute a query over this table.
+
+        To read a subset of the columns, specify their names via `columns` argument. Otherwise, all columns will be read.
+
+        In order to apply a filter, a predicate can be specified. See https://github.com/vast-data/vastdb_sdk/blob/main/README.md#filters-and-projections for more details.
+
+        Query-execution configuration options can be specified via the optional `config` argument.
+        """
         if config is None:
             config = QueryConfig()
 
         # Take a snapshot of enpoints
         stats = self.get_stats()
         endpoints = stats.endpoints if config.data_endpoints is None else config.data_endpoints
 
@@ -331,111 +381,159 @@
                     stop_event.set()
                     while tasks_running > 0:
                         if record_batches_queue.get() is None:
                             tasks_running -= 1
 
         return pa.RecordBatchReader.from_batches(query_data_request.response_schema, batches_iterator())
 
-    def _combine_chunks(self, col):
-        if hasattr(col, "combine_chunks"):
-            return col.combine_chunks()
-        else:
-            return col
-
     def insert(self, rows: pa.RecordBatch) -> pa.RecordBatch:
-        serialized_slices = self.tx._rpc.api._record_batch_slices(rows, MAX_INSERT_ROWS_PER_PATCH)
+        """Insert a RecordBatch into this table."""
+        if self._imports_table:
+            raise errors.NotSupportedCommand(self.bucket.name, self.schema.name, self.name)
+        serialized_slices = util.iter_serialized_slices(rows, MAX_INSERT_ROWS_PER_PATCH)
         for slice in serialized_slices:
             self.tx._rpc.api.insert_rows(self.bucket.name, self.schema.name, self.name, record_batch=slice,
                                                txid=self.tx.txid)
 
     def update(self, rows: Union[pa.RecordBatch, pa.Table], columns: Optional[List[str]] = None) -> None:
+        """Update a subset of cells in this table.
+
+        Row IDs are specified using a special field (named "$row_id" of uint64 type).
+
+        A subset of columns to be updated can be specified via the `columns` argument.
+        """
+        if self._imports_table:
+            raise errors.NotSupportedCommand(self.bucket.name, self.schema.name, self.name)
         if columns is not None:
             update_fields = [(INTERNAL_ROW_ID, pa.uint64())]
-            update_values = [self._combine_chunks(rows[INTERNAL_ROW_ID])]
+            update_values = [_combine_chunks(rows[INTERNAL_ROW_ID])]
             for col in columns:
                 update_fields.append(rows.field(col))
-                update_values.append(self._combine_chunks(rows[col]))
+                update_values.append(_combine_chunks(rows[col]))
 
             update_rows_rb = pa.record_batch(schema=pa.schema(update_fields), data=update_values)
         else:
             update_rows_rb = rows
 
-        serialized_slices = self.tx._rpc.api._record_batch_slices(update_rows_rb, MAX_ROWS_PER_BATCH)
+        serialized_slices = util.iter_serialized_slices(update_rows_rb, MAX_ROWS_PER_BATCH)
         for slice in serialized_slices:
             self.tx._rpc.api.update_rows(self.bucket.name, self.schema.name, self.name, record_batch=slice,
                                          txid=self.tx.txid)
 
     def delete(self, rows: Union[pa.RecordBatch, pa.Table]) -> None:
+        """Delete a subset of rows in this table.
+
+        Row IDs are specified using a special field (named "$row_id" of uint64 type).
+        """
         delete_rows_rb = pa.record_batch(schema=pa.schema([(INTERNAL_ROW_ID, pa.uint64())]),
-                                         data=[self._combine_chunks(rows[INTERNAL_ROW_ID])])
+                                         data=[_combine_chunks(rows[INTERNAL_ROW_ID])])
 
-        serialized_slices = self.tx._rpc.api._record_batch_slices(delete_rows_rb, MAX_ROWS_PER_BATCH)
+        serialized_slices = util.iter_serialized_slices(delete_rows_rb, MAX_ROWS_PER_BATCH)
         for slice in serialized_slices:
             self.tx._rpc.api.delete_rows(self.bucket.name, self.schema.name, self.name, record_batch=slice,
-                                         txid=self.tx.txid)
+                                         txid=self.tx.txid, delete_from_imports_table=self._imports_table)
 
     def drop(self) -> None:
-        self.tx._rpc.api.drop_table(self.bucket.name, self.schema.name, self.name, txid=self.tx.txid)
+        """Drop this table."""
+        self.tx._rpc.api.drop_table(self.bucket.name, self.schema.name, self.name, txid=self.tx.txid, remove_imports_table=self._imports_table)
         log.info("Dropped table: %s", self.name)
 
     def rename(self, new_name) -> None:
+        """Rename this table."""
+        if self._imports_table:
+            raise errors.NotSupportedCommand(self.bucket.name, self.schema.name, self.name)
         self.tx._rpc.api.alter_table(
             self.bucket.name, self.schema.name, self.name, txid=self.tx.txid, new_name=new_name)
         log.info("Renamed table from %s to %s ", self.name, new_name)
         self.name = new_name
 
     def add_column(self, new_column: pa.Schema) -> None:
+        """Add a new column."""
+        if self._imports_table:
+            raise errors.NotSupportedCommand(self.bucket.name, self.schema.name, self.name)
         self.tx._rpc.api.add_columns(self.bucket.name, self.schema.name, self.name, new_column, txid=self.tx.txid)
         log.info("Added column(s): %s", new_column)
         self.arrow_schema = self.columns()
 
     def drop_column(self, column_to_drop: pa.Schema) -> None:
+        """Drop an existing column."""
+        if self._imports_table:
+            raise errors.NotSupported(self.bucket.name, self.schema.name, self.name)
+        if self._imports_table:
+            raise errors.NotSupportedCommand(self.bucket.name, self.schema.name, self.name)
         self.tx._rpc.api.drop_columns(self.bucket.name, self.schema.name, self.name, column_to_drop, txid=self.tx.txid)
         log.info("Dropped column(s): %s", column_to_drop)
         self.arrow_schema = self.columns()
 
     def rename_column(self, current_column_name: str, new_column_name: str) -> None:
+        """Rename an existing column."""
+        if self._imports_table:
+            raise errors.NotSupportedCommand(self.bucket.name, self.schema.name, self.name)
         self.tx._rpc.api.alter_column(self.bucket.name, self.schema.name, self.name, name=current_column_name,
                                        new_name=new_column_name, txid=self.tx.txid)
         log.info("Renamed column: %s to %s", current_column_name, new_column_name)
         self.arrow_schema = self.columns()
 
     def create_projection(self, projection_name: str, sorted_columns: List[str], unsorted_columns: List[str]) -> "Projection":
+        """Create a new semi-sorted projection."""
+        if self._imports_table:
+            raise errors.NotSupportedCommand(self.bucket.name, self.schema.name, self.name)
         columns = [(sorted_column, "Sorted") for sorted_column in sorted_columns] + [(unsorted_column, "Unorted") for unsorted_column in unsorted_columns]
         self.tx._rpc.api.create_projection(self.bucket.name, self.schema.name, self.name, projection_name, columns=columns, txid=self.tx.txid)
         log.info("Created projection: %s", projection_name)
         return self.projection(projection_name)
 
+    def create_imports_table(self, fail_if_exists=True) -> "Table":
+        """Create imports table."""
+        self.tx._rpc.features.check_imports_table()
+        empty_schema = pa.schema([])
+        self.tx._rpc.api.create_table(self.bucket.name, self.schema.name, self.name, empty_schema, txid=self.tx.txid,
+                                        create_imports_table=True)
+        log.info("Created imports table for table: %s", self.name)
+        return self.imports_table()  # type: ignore[return-value]
+
+    def imports_table(self) -> Optional["Table"]:
+        """Get the imports table under of this table."""
+        self.tx._rpc.features.check_imports_table()
+        return Table(name=self.name, schema=self.schema, handle=int(self.handle), stats=self.stats, _imports_table=True)
+
     def __getitem__(self, col_name):
+        """Allow constructing ibis-like column expressions from this table.
+
+        It is useful for constructing expressions for predicate pushdown in `Table.select()` method.
+        """
         return self._ibis_table[col_name]
 
 
 @dataclass
 class Projection:
+    """VAST semi-sorted projection."""
+
     name: str
     table: Table
     handle: int
     stats: TableStats
 
     @property
     def bucket(self):
+        """Return bucket."""
         return self.table.schema.bucket
 
     @property
     def schema(self):
+        """Return schema."""
         return self.table.schema
 
     @property
     def tx(self):
+        """Return transaction."""
         return self.table.schema.tx
 
-    def __repr__(self):
-        return f"{type(self).__name__}(name={self.name})"
-
     def columns(self) -> pa.Schema:
+        """Return this projections' columns as an Arrow schema."""
         columns = []
         next_key = 0
         while True:
             curr_columns, next_key, is_truncated, _count, _ = \
                 self.tx._rpc.api.list_projection_columns(
                     self.bucket.name, self.schema.name, self.table.name, self.name, txid=self.table.tx.txid, next_key=next_key)
             if not curr_columns:
@@ -443,20 +541,22 @@
             columns.extend(curr_columns)
             if not is_truncated:
                 break
         self.arrow_schema = pa.schema([(col[0], col[1]) for col in columns])
         return self.arrow_schema
 
     def rename(self, new_name) -> None:
+        """Rename this projection."""
         self.tx._rpc.api.alter_projection(self.bucket.name, self.schema.name,
                                                 self.table.name, self.name, txid=self.tx.txid, new_name=new_name)
         log.info("Renamed projection from %s to %s ", self.name, new_name)
         self.name = new_name
 
     def drop(self) -> None:
+        """Drop this projection."""
         self.tx._rpc.api.drop_projection(self.bucket.name, self.schema.name, self.table.name,
                                          self.name, txid=self.tx.txid)
         log.info("Dropped projection: %s", self.name)
 
 
 def _parse_projection_info(projection_info, table: "Table"):
     log.info("Projection info %s", str(projection_info))
@@ -474,7 +574,14 @@
 
 
 def _serialize_record_batch(record_batch: pa.RecordBatch) -> pa.lib.Buffer:
     sink = pa.BufferOutputStream()
     with pa.ipc.new_stream(sink, record_batch.schema) as writer:
         writer.write(record_batch)
     return sink.getvalue()
+
+
+def _combine_chunks(col):
+    if hasattr(col, "combine_chunks"):
+        return col.combine_chunks()
+    else:
+        return col
```

### Comparing `vastdb-0.1.2/vastdb/tests/test_duckdb.py` & `vastdb-0.1.3/vastdb/tests/test_duckdb.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vastdb/tests/test_imports.py` & `vastdb-0.1.3/vastdb/tests/test_imports.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from tempfile import NamedTemporaryFile
 
 import pyarrow as pa
 import pyarrow.parquet as pq
 import pytest
 
 from vastdb import util
-from vastdb.errors import ImportFilesError, InvalidArgument
+from vastdb.errors import ImportFilesError, InternalServerError, InvalidArgument
 
 log = logging.getLogger(__name__)
 
 
 def test_parallel_imports(session, clean_bucket_name, s3):
     num_rows = 1000
     num_files = 53
@@ -30,20 +30,32 @@
         s3.copy(copy_source, clean_bucket_name, f'prq{i}')
         files.append(f'/{clean_bucket_name}/prq{i}')
 
     with session.transaction() as tx:
         b = tx.bucket(clean_bucket_name)
         s = b.create_schema('s1')
         t = s.create_table('t1', pa.schema([('num', pa.int64())]))
+        with pytest.raises(InternalServerError):
+            t.create_imports_table()
         log.info("Starting import of %d files", num_files)
         t.import_files(files)
         arrow_table = pa.Table.from_batches(t.select(columns=['num']))
         assert arrow_table.num_rows == num_rows * num_files
         arrow_table = pa.Table.from_batches(t.select(columns=['num'], predicate=t['num'] == 100))
         assert arrow_table.num_rows == num_files
+        import_table = t.imports_table()
+        # checking all imports are on the imports table:
+        objects_name = pa.Table.from_batches(import_table.select(columns=["ObjectName"]))
+        objects_name = objects_name.to_pydict()
+        object_names = set(objects_name['ObjectName'])
+        prefix = 'prq'
+        numbers = set(range(53))
+        assert all(name.startswith(prefix) for name in object_names)
+        numbers.issubset(int(name.replace(prefix, '')) for name in object_names)
+        assert len(object_names) == len(objects_name['ObjectName'])
 
 
 def test_create_table_from_files(session, clean_bucket_name, s3):
     datasets = [
         {'num': [0],
          'varch': ['z']},
         {'num': [1, 2, 3, 4, 5],
```

### Comparing `vastdb-0.1.2/vastdb/tests/test_nested.py` & `vastdb-0.1.3/vastdb/tests/test_nested.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vastdb/tests/test_projections.py` & `vastdb-0.1.3/vastdb/tests/test_projections.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vastdb/tests/test_sanity.py` & `vastdb-0.1.3/vastdb/tests/test_sanity.py`

 * *Files identical despite different names*

### Comparing `vastdb-0.1.2/vastdb/tests/test_schemas.py` & `vastdb-0.1.3/vastdb/tests/test_schemas.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,9 +56,8 @@
         b = tx.bucket(clean_bucket_name)
         assert b.schemas() != []
 
 
 def test_list_snapshots(session, clean_bucket_name):
     with session.transaction() as tx:
         b = tx.bucket(clean_bucket_name)
-        s = b.snapshots()
-        assert s == []
+        b.snapshots()  # VAST Catalog may create some snapshots
```

### Comparing `vastdb-0.1.2/vastdb/tests/test_tables.py` & `vastdb-0.1.3/vastdb/tests/test_tables.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime as dt
 import decimal
 import logging
 import random
 import threading
+import time
 from contextlib import closing
 from tempfile import NamedTemporaryFile
 
 import pyarrow as pa
 import pyarrow.compute as pc
 import pyarrow.parquet as pq
 import pytest
@@ -257,15 +258,15 @@
         [111, 222, 333, 444, 555],
         [0.5, 1.5, 2.5, 3.5, 4.5],
         ['a', 'bb', 'ccc', None, 'xyz'],
     ])
 
     with prepare_data(session, clean_bucket_name, 's', 't', expected) as t:
         def select(predicate):
-            return pa.Table.from_batches(t.select(predicate=predicate))
+            return pa.Table.from_batches(t.select(predicate=predicate), t.arrow_schema)
 
         assert select(None) == expected
 
         assert select(t['a'] > 222) == expected.filter(pc.field('a') > 222)
         assert select(t['a'] < 222) == expected.filter(pc.field('a') < 222)
         assert select(t['a'] == 222) == expected.filter(pc.field('a') == 222)
         assert select(t['a'] != 222) == expected.filter(pc.field('a') != 222)
@@ -300,14 +301,21 @@
         assert select((t['s'].isnull()) | (t['s'] == 'bb'))  == expected.filter((pc.field('s').is_null()) | (pc.field('s') == 'bb'))
         assert select((t['s'].isnull()) & (t['b'] == 3.5))  == expected.filter((pc.field('s').is_null()) & (pc.field('b') == 3.5))
 
         assert select(~t['s'].isnull()) == expected.filter(~pc.field('s').is_null())
         assert select(t['s'].contains('b')) == expected.filter(pc.field('s') == 'bb')
         assert select(t['s'].contains('y')) == expected.filter(pc.field('s') == 'xyz')
 
+        assert select(t['a'].isin([555])) == expected.filter(pc.field('a').isin([555]))
+        assert select(t['a'].isin([111, 222, 999])) == expected.filter(pc.field('a').isin([111, 222, 999]))
+        assert select((t['a'] == 111) | t['a'].isin([333, 444]) | (t['a'] > 600)) == expected.filter((pc.field('a') == 111) | pc.field('a').isin([333, 444]) | (pc.field('a') > 600))
+
+        with pytest.raises(NotImplementedError):
+            select(t['a'].isin([]))
+
 
 def test_parquet_export(session, clean_bucket_name):
     with session.transaction() as tx:
         s = tx.bucket(clean_bucket_name).create_schema('s1')
         columns = pa.schema([
             ('a', pa.int16()),
             ('b', pa.float32()),
@@ -634,7 +642,24 @@
             del batches
 
     # Check that all threads were killed
     log.info("Active threads: %d", active_threads())
 
     # validate that all query threads were killed.
     assert active_threads() == 0
+
+
+def test_big_catalog_select(session, clean_bucket_name):
+    with session.transaction() as tx:
+        bc = tx.catalog()
+        actual = pa.Table.from_batches(bc.select(['name']))
+        assert actual
+        log.info("actual=%s", actual)
+
+
+def test_audit_log_select(session, clean_bucket_name):
+    with session.transaction() as tx:
+        a = tx.audit_log()
+        a.columns()
+        time.sleep(1)
+        actual = pa.Table.from_batches(a.select(), a.arrow_schema)
+        log.info("actual=%s", actual)
```

### Comparing `vastdb-0.1.2/vastdb/transaction.py` & `vastdb-0.1.3/vastdb/transaction.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,22 @@
 
 import botocore
 
 from . import bucket, errors, schema, session, table
 
 log = logging.getLogger(__name__)
 
+TABULAR_BC_BUCKET = "vast-big-catalog-bucket"
+VAST_CATALOG_SCHEMA_NAME = 'vast_big_catalog_schema'
+VAST_CATALOG_TABLE_NAME = 'vast_big_catalog_table'
+
+TABULAR_AUDERY_BUCKET = "vast-audit-log-bucket"
+AUDERY_SCHEMA_NAME = 'vast_audit_log_schema'
+AUDERY_TABLE_NAME = 'vast_audit_log_table'
+
 
 @dataclass
 class Transaction:
     """A holder of a single VAST transaction."""
 
     _rpc: "session.Session"
     txid: Optional[int] = None
@@ -40,14 +48,16 @@
             self._rpc.api.commit_transaction(txid)
         else:
             log.exception("rolling back txid=%016x due to:", txid)
             self._rpc.api.rollback_transaction(txid)
 
     def __repr__(self):
         """Don't show the session details."""
+        if self.txid is None:
+            return 'InvalidTransaction'
         return f'Transaction(id=0x{self.txid:016x})'
 
     def bucket(self, name: str) -> "bucket.Bucket":
         """Return a VAST Bucket, if exists."""
         try:
             self._rpc.s3.head_bucket(Bucket=name)
         except botocore.exceptions.ClientError as e:
@@ -55,10 +65,16 @@
             if e.response['Error']['Code'] == '404':
                 raise errors.MissingBucket(name)
             raise
         return bucket.Bucket(name, self)
 
     def catalog(self, fail_if_missing=True) -> Optional["table.Table"]:
         """Return VAST Catalog table."""
-        b = bucket.Bucket("vast-big-catalog-bucket", self)
-        s = schema.Schema("vast_big_catalog_schema", b)
-        return s.table(name="vast_big_catalog_table", fail_if_missing=fail_if_missing)
+        b = bucket.Bucket(TABULAR_BC_BUCKET, self)
+        s = schema.Schema(VAST_CATALOG_SCHEMA_NAME, b)
+        return s.table(name=VAST_CATALOG_TABLE_NAME, fail_if_missing=fail_if_missing)
+
+    def audit_log(self, fail_if_missing=True) -> Optional["table.Table"]:
+        """Return VAST AuditLog table."""
+        b = bucket.Bucket(TABULAR_AUDERY_BUCKET, self)
+        s = schema.Schema(AUDERY_SCHEMA_NAME, b)
+        return s.table(name=AUDERY_TABLE_NAME, fail_if_missing=fail_if_missing)
```

### Comparing `vastdb-0.1.2/vastdb.egg-info/PKG-INFO` & `vastdb-0.1.3/vastdb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vastdb
-Version: 0.1.2
+Version: 0.1.3
 Summary: VAST Data SDK
 Home-page: https://github.com/vast-data/vastdb_sdk
 Author: VAST DATA
 Author-email: hello@vastdata.com
 License: Copyright (C) VAST Data Ltd.
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -17,15 +17,15 @@
 Classifier: Topic :: Database :: Front-Ends
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aws-requests-auth
 Requires-Dist: boto3
 Requires-Dist: flatbuffers
-Requires-Dist: ibis-framework
+Requires-Dist: ibis-framework==8.0.0
 Requires-Dist: pyarrow
 Requires-Dist: requests
 Requires-Dist: xmltodict
 
 
 `vastdb` is a Python-based SDK designed for interacting
 with [VAST Database](https://vastdata.com/database)
```

### Comparing `vastdb-0.1.2/vastdb.egg-info/SOURCES.txt` & `vastdb-0.1.3/vastdb.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -175,8 +175,9 @@
 vastdb/tests/test_duckdb.py
 vastdb/tests/test_imports.py
 vastdb/tests/test_nested.py
 vastdb/tests/test_projections.py
 vastdb/tests/test_sanity.py
 vastdb/tests/test_schemas.py
 vastdb/tests/test_tables.py
+vastdb/tests/test_util.py
 vastdb/tests/util.py
```

