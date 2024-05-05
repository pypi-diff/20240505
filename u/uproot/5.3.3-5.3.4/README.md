# Comparing `tmp/uproot-5.3.3.tar.gz` & `tmp/uproot-5.3.4.tar.gz`

## Comparing `uproot-5.3.3.tar` & `uproot-5.3.4.tar`

### file list

```diff
@@ -1,274 +1,275 @@
--rw-r--r--   0        0        0    15427 2020-02-02 00:00:00.000000 uproot-5.3.3/.all-contributorsrc
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 uproot-5.3.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 uproot-5.3.3/.readthedocs.yml
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 uproot-5.3.3/CITATION.cff
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 uproot-5.3.3/.github/dependabot.yml
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 uproot-5.3.3/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 uproot-5.3.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 uproot-5.3.3/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 uproot-5.3.3/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 uproot-5.3.3/.github/workflows/build-distributions.yml
--rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 uproot-5.3.3/.github/workflows/build-test.yml
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 uproot-5.3.3/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 uproot-5.3.3/.github/workflows/semantic-pr-title.yml
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 uproot-5.3.3/.github/workflows/upload-nightly-wheels.yml
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 uproot-5.3.3/dev/example-objects.py
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 uproot-5.3.3/dev/make-models.py
--rw-r--r--   0        0        0    95009 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-img/diagrams/abstraction-layers.png
--rw-r--r--   0        0        0    39940 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-img/diagrams/abstraction-layers.svg
--rw-r--r--   0        0        0    49015 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-img/diagrams/example-dask-graph.png
--rw-r--r--   0        0        0    70413 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-img/diagrams/uproot-awkward-timeline.png
--rw-r--r--   0        0        0    28715 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-img/diagrams/uproot-awkward-timeline.svg
--rw-r--r--   0        0        0     6794 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-img/logo/logo-300px-white.png
--rw-r--r--   0        0        0     8489 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-img/logo/logo-600px.png
--rw-r--r--   0        0        0     7695 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-img/logo/logo.svg
--rw-r--r--   0        0        0   223219 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-img/photos/switcheroo.jpg
--rw-r--r--   0        0        0    69268 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-sphinx/basic.rst
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-sphinx/conf.py
--rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-sphinx/index.rst
--rw-r--r--   0        0        0     7841 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-sphinx/make_changelog.py
--rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-sphinx/prepare_docstrings.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-sphinx/requirements.txt
--rw-r--r--   0        0        0    22209 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-sphinx/uproot3-to-4.rst
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-sphinx/_templates/breadcrumbs.html
--rw-r--r--   0        0        0     6952 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/__init__.py
--rw-r--r--   0        0        0     9180 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/_awkwardforth.py
--rw-r--r--   0        0        0    57024 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/_dask.py
--rw-r--r--   0        0        0    34679 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/_util.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behavior.py
--rw-r--r--   0        0        0     7506 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/cache.py
--rw-r--r--   0        0        0    19158 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/compression.py
--rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/const.py
--rw-r--r--   0        0        0    64522 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/containers.py
--rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/deserialization.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/dynamic.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/exceptions.py
--rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/extras.py
--rw-r--r--   0        0        0    66033 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/model.py
--rw-r--r--   0        0        0     9625 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/pyroot.py
--rw-r--r--   0        0        0    98111 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/reading.py
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/serialization.py
--rw-r--r--   0        0        0    64326 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/streamers.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/version.py
--rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/RooCurve.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/RooHist.py
--rw-r--r--   0        0        0    10083 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TAxis.py
--rw-r--r--   0        0        0   129662 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TBranch.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TBranchElement.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TDatime.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TGraph.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TGraphAsymmErrors.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TGraphErrors.py
--rw-r--r--   0        0        0    12104 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TH1.py
--rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TH2.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TH2Poly.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TH3.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TParameter.py
--rw-r--r--   0        0        0    12480 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TProfile.py
--rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TProfile2D.py
--rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TProfile3D.py
--rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TTree.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/__init__.py
--rw-r--r--   0        0        0     8305 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/interpretation/__init__.py
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/interpretation/grouped.py
--rw-r--r--   0        0        0    41203 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/interpretation/identify.py
--rw-r--r--   0        0        0    14929 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/interpretation/jagged.py
--rw-r--r--   0        0        0    38158 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/interpretation/library.py
--rw-r--r--   0        0        0    22691 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/interpretation/numerical.py
--rw-r--r--   0        0        0    37080 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/interpretation/objects.py
--rw-r--r--   0        0        0    18832 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/interpretation/strings.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/language/__init__.py
--rw-r--r--   0        0        0    16942 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/language/python.py
--rw-r--r--   0        0        0    31247 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/RNTuple.py
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TArray.py
--rw-r--r--   0        0        0    25962 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TAtt.py
--rw-r--r--   0        0        0    11268 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TBasket.py
--rw-r--r--   0        0        0    37710 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TBranch.py
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TClonesArray.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TDatime.py
--rw-r--r--   0        0        0    35842 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TGraph.py
--rw-r--r--   0        0        0   215525 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TH.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/THashList.py
--rw-r--r--   0        0        0    34985 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TLeaf.py
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TList.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TMatrixT.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TNamed.py
--rw-r--r--   0        0        0     5879 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TObjArray.py
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TObjString.py
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TObject.py
--rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TRef.py
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TString.py
--rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TTable.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TTime.py
--rw-r--r--   0        0        0    47535 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TTree.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/__init__.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/sink/__init__.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/sink/file.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/source/__init__.py
--rw-r--r--   0        0        0    17529 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/source/chunk.py
--rw-r--r--   0        0        0    24376 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/source/cursor.py
--rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/source/file.py
--rw-r--r--   0        0        0     8185 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/source/fsspec.py
--rw-r--r--   0        0        0    15114 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/source/futures.py
--rw-r--r--   0        0        0    28139 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/source/http.py
--rw-r--r--   0        0        0     4065 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/source/object.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/source/s3.py
--rw-r--r--   0        0        0    17188 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/source/xrootd.py
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/writing/__init__.py
--rw-r--r--   0        0        0    81089 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/writing/_cascade.py
--rw-r--r--   0        0        0    31428 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/writing/_cascadentuple.py
--rw-r--r--   0        0        0    62285 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/writing/_cascadetree.py
--rw-r--r--   0        0        0     6360 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/writing/_dask_write.py
--rw-r--r--   0        0        0    82120 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/writing/identify.py
--rw-r--r--   0        0        0    80822 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/writing/writable.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/__init__.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/conftest.py
--rw-r--r--   0        0        0    17012 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0001_source_class.py
--rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0006_notify_when_downloaded.py
--rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0007_single_chunk_interface.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0008_start_interpretation.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0009_nested_directories.py
--rw-r--r--   0        0        0    29196 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0010_start_streamers.py
--rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0011_generate_classes_from_streamers.py
--rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0013_rntuple_anchor.py
--rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0014_all_ttree_versions.py
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0016_interpretations.py
--rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0017_multi_basket_multi_branch_fetch.py
--rw-r--r--   0        0        0    33935 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0018_array_fetching_interface.py
--rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0022_number_of_branches.py
--rw-r--r--   0        0        0    13960 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0023_more_interpretations_1.py
--rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0023_ttree_versions.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0028_fallback_to_read_streamer.py
--rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0029_more_string_types.py
--rw-r--r--   0        0        0    23329 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0031_test_stl_containers.py
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0033_more_interpretations_2.py
--rw-r--r--   0        0        0    46572 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0034_generic_objects_in_ttrees.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0035_datatype_generality.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0038_memberwise_serialization.py
--rw-r--r--   0        0        0     8188 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0043_iterate_function.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0044_concatenate_function.py
--rw-r--r--   0        0        0    68981 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0046_histograms_bh_hist.py
--rw-r--r--   0        0        0     8605 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0053_parents_should_not_be_bases.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0058_detach_model_objects_from_files.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0066_fix_http_fallback_freeze.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0067_common_entry_offsets.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0081_dont_parse_colons.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0087_memberwise_splitting_not_implemented_messages.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0088_read_with_http.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0099_read_from_file_object.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0112_fix_pandas_with_cut.py
--rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0118_fix_name_fetch_again.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0123_atlas_issues.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0126_turn_unknown_emptyarrays_into_known_types.py
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0167_use_the_common_histogram_interface.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0172_allow_allocators_in_vector_typenames.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0173_empty_and_multiprocessing_bugs.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0182_complain_about_missing_files.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0194_fix_lost_cuts_in_iterate.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0220_contiguous_byte_ranges_in_http.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0228_read_TProfiles.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0240_read_TGraphAsymmErrors.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0278_specializations_for_TParameter.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0302_pickle.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0303_empty_jagged_array.py
--rw-r--r--   0        0        0    14234 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0320_start_working_on_ROOT_writing.py
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0322_writablefile_infrastructure.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0329_update_existing_root_files.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0335_empty_ttree_division_by_zero.py
--rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0341_manipulate_streamer_info.py
--rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0344_writabledirectory_can_read.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0345_bulk_copy_method.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0349_write_TObjString.py
--rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0350_read_RooCurve_RooHist.py
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0351_write_TList.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0352_write_THashList.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0384_move_behavior_of_and_fix_383.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0398_dimensions_in_leaflist.py
--rw-r--r--   0        0        0    26536 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0405_write_a_histogram.py
--rw-r--r--   0        0        0    11518 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0406_write_a_ttree.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0407_read_TDatime.py
--rw-r--r--   0        0        0    17062 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0412_write_multidimensional_numpy_to_ttree.py
--rw-r--r--   0        0        0    15363 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0414_write_jagged_arrays.py
--rw-r--r--   0        0        0    26104 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0416_writing_compressed_data.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0418_read_TTable.py
--rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0420_pyroot_uproot_interoperability.py
--rw-r--r--   0        0        0    17479 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0422_hist_integration.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0430_global_index_for_tuples_of_DataFrames.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0438_TClonesArray_is_not_AsGrouped.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0439_check_awkward_before_numpy.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0442_regular_TClonesArray.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0472_tstreamerinfo_for_ttree.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0475_remember_to_update_freesegments.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0484_manually_add_model_for_TMatrixTSym_double_.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0487_implement_asdtypeinplace.py
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0498_create_leaf_branch_in_extend.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0519_remove_memmap_copy.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0520_dynamic_classes_cant_be_abc_subclasses.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0569_fBits_is_4_bytes.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0576_unicode_in_names.py
--rw-r--r--   0        0        0    25906 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0578_dask_for_numpy.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0580_round_trip_for_no_flow_histograms.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0589_explicitly_interpret_RVec_type.py
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0603_dask_delayed_open.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0609_num_enteries_func.py
--rw-r--r--   0        0        0    18214 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0610_awkward_form.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0630_rntuple_basics.py
--rw-r--r--   0        0        0   132838 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0637_setup_tests_for_AwkwardForth.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0643_reading_vector_pair_TLorentzVector_int.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0651_implement_transformed_axis.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0652_dask_for_awkward.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0662_rntuple_stl_containers.py
--rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0692_fsspec_reading.py
--rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0692_fsspec_writing.py
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0700_dask_empty_arrays.py
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0705_rntuple_writing_metadata.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0750_avoid_empty_TBasket_issue.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0755_dask_awkward_column_projection.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0791_protect_uproot_project_columns_from_dask_node_names.py
--rw-r--r--   0        0        0     4885 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0798_DAOD_PHYSLITE.py
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0808_fix_awkward_form_for_AsStridedObjects.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0816_separate_AwkwardForth_machines_by_TBranch.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0832_ak_add_doc_should_also_add_to_typetracer.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0840_support_tleafG.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0841_fix_814.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0844_fix_delete_hist_from_root.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0852_fix_strided_interp_extra_offsets.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0870_writing_arrays_of_type_unknown_fix_822.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0876_uproot_dask_blind_steps.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0886_fix_awkward_form_breadcrumbs.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0910_fix_906_members_non_numerical_branches.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0911_fix_interp_array_non_numerical_objs_issue_880.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0912_fix_pandas_and_double_nested_vectors_issue_885.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0916_read_from_s3.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0927_dont_assume_uproot_in_global_scope_in_TPython_Eval.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0930_expressions_in_pandas.py
--rw-r--r--   0        0        0     7233 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0940_feat_add_TLeafC_string_support.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0962_RNTuple_update.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0965_inverted_axes_variances_hist_888.py
--rw-r--r--   0        0        0     7389 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0976_path_object_split.py
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1000-write-TProfiles.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1043_const_std_string.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1058_dask_awkward_report.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1063_dask_distributed.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1070_pandas_dataframe_building_performance_fix.py
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1085_dask_write.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1102_any_locks_in_models_must_be_transient.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1114_fix_attempt_to_concatenate_numpy_with_awkward.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1120_check_decompression_executor_pass_for_dask.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1127_fix_allow_colon_in_key_names.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1146_split_ranges_for_large_files_over_http.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1154_classof_using_relative_path.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1160_std_string_in_TDirectory.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1180_read_free_floating_vector_issue_1179.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1181_support_for_stl_list.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1182_add_support_for_bitset.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1183_ttime_custom.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1186_dtype_might_raise_ValueError.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1189_dask_failing_on_duplicate_keys.py
--rw-r--r--   0        0        0   128147 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/samples/h_dynamic.pkl
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 uproot-5.3.3/.gitignore
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 uproot-5.3.3/LICENSE
--rw-r--r--   0        0        0    29133 2020-02-02 00:00:00.000000 uproot-5.3.3/README.md
--rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 uproot-5.3.3/pyproject.toml
--rw-r--r--   0        0        0    31907 2020-02-02 00:00:00.000000 uproot-5.3.3/PKG-INFO
+-rw-r--r--   0        0        0    15427 2020-02-02 00:00:00.000000 uproot-5.3.4/.all-contributorsrc
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 uproot-5.3.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 uproot-5.3.4/.readthedocs.yml
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 uproot-5.3.4/CITATION.cff
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 uproot-5.3.4/.github/dependabot.yml
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 uproot-5.3.4/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 uproot-5.3.4/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 uproot-5.3.4/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 uproot-5.3.4/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 uproot-5.3.4/.github/workflows/build-distributions.yml
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 uproot-5.3.4/.github/workflows/build-test.yml
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 uproot-5.3.4/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 uproot-5.3.4/.github/workflows/semantic-pr-title.yml
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 uproot-5.3.4/.github/workflows/upload-nightly-wheels.yml
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 uproot-5.3.4/dev/example-objects.py
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 uproot-5.3.4/dev/make-models.py
+-rw-r--r--   0        0        0    95009 2020-02-02 00:00:00.000000 uproot-5.3.4/docs-img/diagrams/abstraction-layers.png
+-rw-r--r--   0        0        0    39940 2020-02-02 00:00:00.000000 uproot-5.3.4/docs-img/diagrams/abstraction-layers.svg
+-rw-r--r--   0        0        0    49015 2020-02-02 00:00:00.000000 uproot-5.3.4/docs-img/diagrams/example-dask-graph.png
+-rw-r--r--   0        0        0    70413 2020-02-02 00:00:00.000000 uproot-5.3.4/docs-img/diagrams/uproot-awkward-timeline.png
+-rw-r--r--   0        0        0    28715 2020-02-02 00:00:00.000000 uproot-5.3.4/docs-img/diagrams/uproot-awkward-timeline.svg
+-rw-r--r--   0        0        0     6794 2020-02-02 00:00:00.000000 uproot-5.3.4/docs-img/logo/logo-300px-white.png
+-rw-r--r--   0        0        0     8489 2020-02-02 00:00:00.000000 uproot-5.3.4/docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 uproot-5.3.4/docs-img/logo/logo-600px.png
+-rw-r--r--   0        0        0     7695 2020-02-02 00:00:00.000000 uproot-5.3.4/docs-img/logo/logo.svg
+-rw-r--r--   0        0        0   223219 2020-02-02 00:00:00.000000 uproot-5.3.4/docs-img/photos/switcheroo.jpg
+-rw-r--r--   0        0        0    69268 2020-02-02 00:00:00.000000 uproot-5.3.4/docs-sphinx/basic.rst
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 uproot-5.3.4/docs-sphinx/conf.py
+-rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 uproot-5.3.4/docs-sphinx/index.rst
+-rw-r--r--   0        0        0     7841 2020-02-02 00:00:00.000000 uproot-5.3.4/docs-sphinx/make_changelog.py
+-rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 uproot-5.3.4/docs-sphinx/prepare_docstrings.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 uproot-5.3.4/docs-sphinx/requirements.txt
+-rw-r--r--   0        0        0    22209 2020-02-02 00:00:00.000000 uproot-5.3.4/docs-sphinx/uproot3-to-4.rst
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 uproot-5.3.4/docs-sphinx/_templates/breadcrumbs.html
+-rw-r--r--   0        0        0     6952 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/__init__.py
+-rw-r--r--   0        0        0     9180 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/_awkwardforth.py
+-rw-r--r--   0        0        0    57024 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/_dask.py
+-rw-r--r--   0        0        0    34724 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/_util.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/behavior.py
+-rw-r--r--   0        0        0     7506 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/cache.py
+-rw-r--r--   0        0        0    19158 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/compression.py
+-rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/const.py
+-rw-r--r--   0        0        0    64522 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/containers.py
+-rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/deserialization.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/dynamic.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/exceptions.py
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/extras.py
+-rw-r--r--   0        0        0    66033 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/model.py
+-rw-r--r--   0        0        0     9625 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/pyroot.py
+-rw-r--r--   0        0        0    98111 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/reading.py
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/serialization.py
+-rw-r--r--   0        0        0    64326 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/streamers.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/version.py
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/behaviors/RooCurve.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/behaviors/RooHist.py
+-rw-r--r--   0        0        0    10083 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/behaviors/TAxis.py
+-rw-r--r--   0        0        0   129724 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/behaviors/TBranch.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/behaviors/TBranchElement.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/behaviors/TDatime.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/behaviors/TGraph.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/behaviors/TGraphAsymmErrors.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/behaviors/TGraphErrors.py
+-rw-r--r--   0        0        0    12104 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/behaviors/TH1.py
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/behaviors/TH2.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/behaviors/TH2Poly.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/behaviors/TH3.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/behaviors/TParameter.py
+-rw-r--r--   0        0        0    12480 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/behaviors/TProfile.py
+-rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/behaviors/TProfile2D.py
+-rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/behaviors/TProfile3D.py
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/behaviors/TTree.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/behaviors/__init__.py
+-rw-r--r--   0        0        0     8305 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/interpretation/__init__.py
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/interpretation/grouped.py
+-rw-r--r--   0        0        0    41203 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/interpretation/identify.py
+-rw-r--r--   0        0        0    14929 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/interpretation/jagged.py
+-rw-r--r--   0        0        0    38158 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/interpretation/library.py
+-rw-r--r--   0        0        0    22691 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/interpretation/numerical.py
+-rw-r--r--   0        0        0    37599 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/interpretation/objects.py
+-rw-r--r--   0        0        0    18832 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/interpretation/strings.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/language/__init__.py
+-rw-r--r--   0        0        0    16942 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/language/python.py
+-rw-r--r--   0        0        0    32821 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/models/RNTuple.py
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/models/TArray.py
+-rw-r--r--   0        0        0    25962 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/models/TAtt.py
+-rw-r--r--   0        0        0    11268 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/models/TBasket.py
+-rw-r--r--   0        0        0    37710 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/models/TBranch.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/models/TClonesArray.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/models/TDatime.py
+-rw-r--r--   0        0        0    35842 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/models/TGraph.py
+-rw-r--r--   0        0        0   215525 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/models/TH.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/models/THashList.py
+-rw-r--r--   0        0        0    34985 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/models/TLeaf.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/models/TList.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/models/TMatrixT.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/models/TNamed.py
+-rw-r--r--   0        0        0     5879 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/models/TObjArray.py
+-rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/models/TObjString.py
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/models/TObject.py
+-rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/models/TRef.py
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/models/TString.py
+-rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/models/TTable.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/models/TTime.py
+-rw-r--r--   0        0        0    47535 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/models/TTree.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/models/__init__.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/sink/__init__.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/sink/file.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/source/__init__.py
+-rw-r--r--   0        0        0    17529 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/source/chunk.py
+-rw-r--r--   0        0        0    24376 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/source/cursor.py
+-rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/source/file.py
+-rw-r--r--   0        0        0     8185 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/source/fsspec.py
+-rw-r--r--   0        0        0    15114 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/source/futures.py
+-rw-r--r--   0        0        0    28139 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/source/http.py
+-rw-r--r--   0        0        0     4065 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/source/object.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/source/s3.py
+-rw-r--r--   0        0        0    17188 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/source/xrootd.py
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/writing/__init__.py
+-rw-r--r--   0        0        0    81089 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/writing/_cascade.py
+-rw-r--r--   0        0        0    31428 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/writing/_cascadentuple.py
+-rw-r--r--   0        0        0    62285 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/writing/_cascadetree.py
+-rw-r--r--   0        0        0     6360 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/writing/_dask_write.py
+-rw-r--r--   0        0        0    82120 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/writing/identify.py
+-rw-r--r--   0        0        0    80822 2020-02-02 00:00:00.000000 uproot-5.3.4/src/uproot/writing/writable.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/__init__.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/conftest.py
+-rw-r--r--   0        0        0    17012 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0001_source_class.py
+-rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0006_notify_when_downloaded.py
+-rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0007_single_chunk_interface.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0008_start_interpretation.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0009_nested_directories.py
+-rw-r--r--   0        0        0    29196 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0010_start_streamers.py
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0011_generate_classes_from_streamers.py
+-rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0013_rntuple_anchor.py
+-rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0014_all_ttree_versions.py
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0016_interpretations.py
+-rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0017_multi_basket_multi_branch_fetch.py
+-rw-r--r--   0        0        0    33935 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0018_array_fetching_interface.py
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0022_number_of_branches.py
+-rw-r--r--   0        0        0    13960 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0023_more_interpretations_1.py
+-rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0023_ttree_versions.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0028_fallback_to_read_streamer.py
+-rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0029_more_string_types.py
+-rw-r--r--   0        0        0    23329 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0031_test_stl_containers.py
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0033_more_interpretations_2.py
+-rw-r--r--   0        0        0    46572 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0034_generic_objects_in_ttrees.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0035_datatype_generality.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0038_memberwise_serialization.py
+-rw-r--r--   0        0        0     8188 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0043_iterate_function.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0044_concatenate_function.py
+-rw-r--r--   0        0        0    68981 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0046_histograms_bh_hist.py
+-rw-r--r--   0        0        0     8605 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0053_parents_should_not_be_bases.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0058_detach_model_objects_from_files.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0066_fix_http_fallback_freeze.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0067_common_entry_offsets.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0081_dont_parse_colons.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0087_memberwise_splitting_not_implemented_messages.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0088_read_with_http.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0099_read_from_file_object.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0112_fix_pandas_with_cut.py
+-rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0118_fix_name_fetch_again.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0123_atlas_issues.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0126_turn_unknown_emptyarrays_into_known_types.py
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0167_use_the_common_histogram_interface.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0172_allow_allocators_in_vector_typenames.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0173_empty_and_multiprocessing_bugs.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0182_complain_about_missing_files.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0194_fix_lost_cuts_in_iterate.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0220_contiguous_byte_ranges_in_http.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0228_read_TProfiles.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0240_read_TGraphAsymmErrors.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0278_specializations_for_TParameter.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0302_pickle.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0303_empty_jagged_array.py
+-rw-r--r--   0        0        0    14234 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0320_start_working_on_ROOT_writing.py
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0322_writablefile_infrastructure.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0329_update_existing_root_files.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0335_empty_ttree_division_by_zero.py
+-rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0341_manipulate_streamer_info.py
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0344_writabledirectory_can_read.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0345_bulk_copy_method.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0349_write_TObjString.py
+-rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0350_read_RooCurve_RooHist.py
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0351_write_TList.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0352_write_THashList.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0384_move_behavior_of_and_fix_383.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0398_dimensions_in_leaflist.py
+-rw-r--r--   0        0        0    26536 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0405_write_a_histogram.py
+-rw-r--r--   0        0        0    11518 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0406_write_a_ttree.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0407_read_TDatime.py
+-rw-r--r--   0        0        0    17062 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0412_write_multidimensional_numpy_to_ttree.py
+-rw-r--r--   0        0        0    15363 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0414_write_jagged_arrays.py
+-rw-r--r--   0        0        0    26706 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0416_writing_compressed_data.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0418_read_TTable.py
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0420_pyroot_uproot_interoperability.py
+-rw-r--r--   0        0        0    17479 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0422_hist_integration.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0430_global_index_for_tuples_of_DataFrames.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0438_TClonesArray_is_not_AsGrouped.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0439_check_awkward_before_numpy.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0442_regular_TClonesArray.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0472_tstreamerinfo_for_ttree.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0475_remember_to_update_freesegments.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0484_manually_add_model_for_TMatrixTSym_double_.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0487_implement_asdtypeinplace.py
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0498_create_leaf_branch_in_extend.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0519_remove_memmap_copy.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0520_dynamic_classes_cant_be_abc_subclasses.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0569_fBits_is_4_bytes.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0576_unicode_in_names.py
+-rw-r--r--   0        0        0    25906 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0578_dask_for_numpy.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0580_round_trip_for_no_flow_histograms.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0589_explicitly_interpret_RVec_type.py
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0603_dask_delayed_open.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0609_num_enteries_func.py
+-rw-r--r--   0        0        0    18214 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0610_awkward_form.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0630_rntuple_basics.py
+-rw-r--r--   0        0        0   132838 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0637_setup_tests_for_AwkwardForth.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0643_reading_vector_pair_TLorentzVector_int.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0651_implement_transformed_axis.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0652_dask_for_awkward.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0662_rntuple_stl_containers.py
+-rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0692_fsspec_reading.py
+-rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0692_fsspec_writing.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0700_dask_empty_arrays.py
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0705_rntuple_writing_metadata.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0750_avoid_empty_TBasket_issue.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0755_dask_awkward_column_projection.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0791_protect_uproot_project_columns_from_dask_node_names.py
+-rw-r--r--   0        0        0     4885 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0798_DAOD_PHYSLITE.py
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0808_fix_awkward_form_for_AsStridedObjects.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0816_separate_AwkwardForth_machines_by_TBranch.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0832_ak_add_doc_should_also_add_to_typetracer.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0840_support_tleafG.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0841_fix_814.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0844_fix_delete_hist_from_root.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0852_fix_strided_interp_extra_offsets.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0870_writing_arrays_of_type_unknown_fix_822.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0876_uproot_dask_blind_steps.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0886_fix_awkward_form_breadcrumbs.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0910_fix_906_members_non_numerical_branches.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0911_fix_interp_array_non_numerical_objs_issue_880.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0912_fix_pandas_and_double_nested_vectors_issue_885.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0916_read_from_s3.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0927_dont_assume_uproot_in_global_scope_in_TPython_Eval.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0930_expressions_in_pandas.py
+-rw-r--r--   0        0        0     7233 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0940_feat_add_TLeafC_string_support.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0962_RNTuple_update.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0965_inverted_axes_variances_hist_888.py
+-rw-r--r--   0        0        0     7389 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_0976_path_object_split.py
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_1000-write-TProfiles.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_1043_const_std_string.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_1058_dask_awkward_report.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_1063_dask_distributed.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_1070_pandas_dataframe_building_performance_fix.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_1085_dask_write.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_1102_any_locks_in_models_must_be_transient.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_1114_fix_attempt_to_concatenate_numpy_with_awkward.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_1120_check_decompression_executor_pass_for_dask.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_1127_fix_allow_colon_in_key_names.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_1146_split_ranges_for_large_files_over_http.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_1154_classof_using_relative_path.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_1160_std_string_in_TDirectory.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_1180_read_free_floating_vector_issue_1179.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_1181_support_for_stl_list.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_1182_add_support_for_bitset.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_1183_ttime_custom.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_1186_dtype_might_raise_ValueError.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_1189_dask_failing_on_duplicate_keys.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/test_1191_rntuple_fixes.py
+-rw-r--r--   0        0        0   128147 2020-02-02 00:00:00.000000 uproot-5.3.4/tests/samples/h_dynamic.pkl
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 uproot-5.3.4/.gitignore
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 uproot-5.3.4/LICENSE
+-rw-r--r--   0        0        0    29133 2020-02-02 00:00:00.000000 uproot-5.3.4/README.md
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 uproot-5.3.4/pyproject.toml
+-rw-r--r--   0        0        0    31907 2020-02-02 00:00:00.000000 uproot-5.3.4/PKG-INFO
```

### Comparing `uproot-5.3.3/.all-contributorsrc` & `uproot-5.3.4/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/.pre-commit-config.yaml` & `uproot-5.3.4/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -14,20 +14,20 @@
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: requirements-txt-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/psf/black-pre-commit-mirror
-    rev: 24.3.0
+    rev: 24.4.2
     hooks:
       - id: black
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.5
+    rev: v0.4.2
     hooks:
       - id: ruff
         args: [--fix, --show-fixes]
 
 
   - repo: https://github.com/asottile/pyupgrade
     rev: v3.15.2
```

### Comparing `uproot-5.3.3/CITATION.cff` & `uproot-5.3.4/CITATION.cff`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/.github/ISSUE_TEMPLATE/bug-report.md` & `uproot-5.3.4/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/.github/ISSUE_TEMPLATE/feature-request.md` & `uproot-5.3.4/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/.github/workflows/build-distributions.yml` & `uproot-5.3.4/.github/workflows/build-distributions.yml`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/.github/workflows/build-test.yml` & `uproot-5.3.4/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/.github/workflows/deploy.yml` & `uproot-5.3.4/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/.github/workflows/upload-nightly-wheels.yml` & `uproot-5.3.4/.github/workflows/upload-nightly-wheels.yml`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/dev/example-objects.py` & `uproot-5.3.4/dev/example-objects.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/dev/make-models.py` & `uproot-5.3.4/dev/make-models.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/docs-img/diagrams/abstraction-layers.png` & `uproot-5.3.4/docs-img/diagrams/abstraction-layers.png`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/docs-img/diagrams/abstraction-layers.svg` & `uproot-5.3.4/docs-img/diagrams/abstraction-layers.svg`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/docs-img/diagrams/example-dask-graph.png` & `uproot-5.3.4/docs-img/diagrams/example-dask-graph.png`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/docs-img/diagrams/uproot-awkward-timeline.png` & `uproot-5.3.4/docs-img/diagrams/uproot-awkward-timeline.png`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/docs-img/diagrams/uproot-awkward-timeline.svg` & `uproot-5.3.4/docs-img/diagrams/uproot-awkward-timeline.svg`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/docs-img/logo/logo-300px-white.png` & `uproot-5.3.4/docs-img/logo/logo-300px-white.png`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/docs-img/logo/logo-300px.png` & `uproot-5.3.4/docs-img/logo/logo-300px.png`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/docs-img/logo/logo-600px.png` & `uproot-5.3.4/docs-img/logo/logo-600px.png`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/docs-img/logo/logo.svg` & `uproot-5.3.4/docs-img/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/docs-img/photos/switcheroo.jpg` & `uproot-5.3.4/docs-img/photos/switcheroo.jpg`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/docs-sphinx/basic.rst` & `uproot-5.3.4/docs-sphinx/basic.rst`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/docs-sphinx/conf.py` & `uproot-5.3.4/docs-sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/docs-sphinx/index.rst` & `uproot-5.3.4/docs-sphinx/index.rst`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/docs-sphinx/make_changelog.py` & `uproot-5.3.4/docs-sphinx/make_changelog.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/docs-sphinx/prepare_docstrings.py` & `uproot-5.3.4/docs-sphinx/prepare_docstrings.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/docs-sphinx/uproot3-to-4.rst` & `uproot-5.3.4/docs-sphinx/uproot3-to-4.rst`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/__init__.py` & `uproot-5.3.4/src/uproot/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/_awkwardforth.py` & `uproot-5.3.4/src/uproot/_awkwardforth.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/_dask.py` & `uproot-5.3.4/src/uproot/_dask.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/_util.py` & `uproot-5.3.4/src/uproot/_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,28 +9,31 @@
 
 import datetime
 import glob
 import itertools
 import numbers
 import os
 import re
+import sys
 import warnings
 from collections.abc import Iterable
 from pathlib import Path
 from typing import IO
 from urllib.parse import urlparse
 
 import fsspec
 import numpy
 import packaging.version
 
 import uproot.source.chunk
 import uproot.source.fsspec
 import uproot.source.object
 
+macos = sys.platform == "darwin"
+
 
 def tobytes(array):
     """
     Calls ``array.tobytes()`` or its older equivalent, ``array.tostring()``,
     depending on what's available in this NumPy version. (tobytes added in 1.9)
     """
     if hasattr(array, "tobytes"):
```

### Comparing `uproot-5.3.3/src/uproot/behavior.py` & `uproot-5.3.4/src/uproot/behavior.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/cache.py` & `uproot-5.3.4/src/uproot/cache.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/compression.py` & `uproot-5.3.4/src/uproot/compression.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/const.py` & `uproot-5.3.4/src/uproot/const.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/containers.py` & `uproot-5.3.4/src/uproot/containers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/deserialization.py` & `uproot-5.3.4/src/uproot/deserialization.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/dynamic.py` & `uproot-5.3.4/src/uproot/dynamic.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/exceptions.py` & `uproot-5.3.4/src/uproot/exceptions.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/extras.py` & `uproot-5.3.4/src/uproot/extras.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/model.py` & `uproot-5.3.4/src/uproot/model.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/pyroot.py` & `uproot-5.3.4/src/uproot/pyroot.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/reading.py` & `uproot-5.3.4/src/uproot/reading.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/serialization.py` & `uproot-5.3.4/src/uproot/serialization.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/streamers.py` & `uproot-5.3.4/src/uproot/streamers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/behaviors/RooCurve.py` & `uproot-5.3.4/src/uproot/behaviors/RooCurve.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/behaviors/RooHist.py` & `uproot-5.3.4/src/uproot/behaviors/RooHist.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/behaviors/TAxis.py` & `uproot-5.3.4/src/uproot/behaviors/TAxis.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/behaviors/TBranch.py` & `uproot-5.3.4/src/uproot/behaviors/TBranch.py`

 * *Files 0% similar despite different names*

```diff
@@ -3003,16 +3003,18 @@
     for cache_key, interpretation in branchid_interpretation.items():
         if branchid_num_baskets[cache_key] == 0 and cache_key not in arrays:
             arrays[cache_key] = interpretation.final_array(
                 {}, 0, 0, [0], library, None, interp_options
             )
 
         # check for CannotBeAwkward errors on the main thread before reading any data
-        if isinstance(library, uproot.interpretation.library.Awkward) and isinstance(
-            interpretation, uproot.interpretation.objects.AsObjects
+        if (
+            isinstance(library, uproot.interpretation.library.Awkward)
+            and isinstance(interpretation, uproot.interpretation.objects.AsObjects)
+            and cache_key in branchid_to_branch
         ):
             branchid_to_branch[cache_key]._awkward_check(interpretation)
 
     hasbranches._file.source.chunks(ranges, notifications=notifications)
 
     def replace(ranges_or_baskets, original_index, basket):
         branch, basket_num, range_or_basket = ranges_or_baskets[original_index]
```

### Comparing `uproot-5.3.3/src/uproot/behaviors/TBranchElement.py` & `uproot-5.3.4/src/uproot/behaviors/TBranchElement.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/behaviors/TGraph.py` & `uproot-5.3.4/src/uproot/behaviors/TGraph.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/behaviors/TGraphAsymmErrors.py` & `uproot-5.3.4/src/uproot/behaviors/TGraphAsymmErrors.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/behaviors/TH1.py` & `uproot-5.3.4/src/uproot/behaviors/TH1.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/behaviors/TH2.py` & `uproot-5.3.4/src/uproot/behaviors/TH2.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/behaviors/TH2Poly.py` & `uproot-5.3.4/src/uproot/behaviors/TH2Poly.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/behaviors/TH3.py` & `uproot-5.3.4/src/uproot/behaviors/TH3.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/behaviors/TParameter.py` & `uproot-5.3.4/src/uproot/behaviors/TParameter.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/behaviors/TProfile.py` & `uproot-5.3.4/src/uproot/behaviors/TProfile.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/behaviors/TProfile2D.py` & `uproot-5.3.4/src/uproot/behaviors/TProfile2D.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/behaviors/TProfile3D.py` & `uproot-5.3.4/src/uproot/behaviors/TProfile3D.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/behaviors/TTree.py` & `uproot-5.3.4/src/uproot/behaviors/TTree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/behaviors/__init__.py` & `uproot-5.3.4/src/uproot/behaviors/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/interpretation/__init__.py` & `uproot-5.3.4/src/uproot/interpretation/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/interpretation/grouped.py` & `uproot-5.3.4/src/uproot/interpretation/grouped.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/interpretation/identify.py` & `uproot-5.3.4/src/uproot/interpretation/identify.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/interpretation/jagged.py` & `uproot-5.3.4/src/uproot/interpretation/jagged.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/interpretation/library.py` & `uproot-5.3.4/src/uproot/interpretation/library.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/interpretation/numerical.py` & `uproot-5.3.4/src/uproot/interpretation/numerical.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/interpretation/objects.py` & `uproot-5.3.4/src/uproot/interpretation/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,31 @@
         else:
             model = repr(self._model)
         return f"AsObjects({model})"
 
     def __eq__(self, other):
         return isinstance(other, AsObjects) and self._model == other._model
 
+    def __getstate__(self):
+        return {
+            k: (
+                uproot.model._LockPlaceholder()
+                if isinstance(v, uproot.model._LockPlaceholder.lock_type)
+                else v
+            )
+            for k, v in self.__dict__.items()
+        }
+
+    def __setstate__(self, state):
+        instance_data = {
+            k: threading.Lock() if isinstance(v, uproot.model._LockPlaceholder) else v
+            for k, v in state.items()
+        }
+        self.__dict__.update(instance_data)
+
     @property
     def numpy_dtype(self):
         return numpy.dtype(object)
 
     @property
     def cache_key(self):
         content_key = uproot.containers._content_cache_key(self._model)
```

### Comparing `uproot-5.3.3/src/uproot/interpretation/strings.py` & `uproot-5.3.4/src/uproot/interpretation/strings.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/language/__init__.py` & `uproot-5.3.4/src/uproot/language/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/language/python.py` & `uproot-5.3.4/src/uproot/language/python.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/models/RNTuple.py` & `uproot-5.3.4/src/uproot/models/RNTuple.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 _rntuple_cluster_group_format = struct.Struct("<qqi")
 _rntuple_locator_format = struct.Struct("<iQ")
 _rntuple_cluster_summary_format = struct.Struct("<QQ")
 _rntuple_checksum_format = struct.Struct("<Q")
 _rntuple_envlink_size_format = struct.Struct("<Q")
 _rntuple_page_num_elements_format = struct.Struct("<I")
 _rntuple_column_group_id_format = struct.Struct("<I")
+_rntuple_first_ele_index_format = struct.Struct("<I")
 
 
 def from_zigzag(n):
     return n >> 1 ^ -(n & 1)
 
 
 def _envelop_header(chunk, cursor, context):
@@ -49,15 +50,15 @@
     """
     A versionless :doc:`uproot.model.Model` for ``ROOT::Experimental::RNTuple``.
     """
 
     @property
     def _keys(self):
         keys = []
-        field_records = self.header.field_records
+        field_records = self.field_records
         for i, fr in enumerate(field_records):
             if fr.parent_field_id == i and fr.type_name != "":
                 keys.append(fr.field_name)
         return keys
 
     def keys(self):
         return self._keys
@@ -85,16 +86,21 @@
             self._members["fChecksum"],
         ) = cursor.fields(chunk, _rntuple_anchor_format, context)
 
         self._header_chunk_ready = False
         self._footer_chunk_ready = False
         self._header, self._footer = None, None
 
+        self._field_records = None
         self._field_names = None
         self._column_records = None
+        self._alias_column_records = None
+        self._alias_columns_dict_ = None
+        self._related_ids_ = None
+        self._column_records_dict_ = None
 
         self._page_list_envelopes = []
 
     def _prepare_header_chunk(self):
         context = {}
         seek, nbytes = self._members["fSeekHeader"], self._members["fNBytesHeader"]
 
@@ -148,22 +154,71 @@
 
             h = HeaderReader().read(self._header_chunk, cursor, context)
             self._header = h
 
         return self._header
 
     @property
+    def field_records(self):
+        if self._field_records is None:
+            self._field_records = list(self.header.field_records)
+            self._field_records.extend(self.footer.extension_links.field_records)
+        return self._field_records
+
+    @property
     def field_names(self):
         if self._field_names is None:
-            self._field_names = [r.field_name for r in self.header.field_records]
+            self._field_names = [r.field_name for r in self.field_records]
         return self._field_names
 
     @property
     def column_records(self):
-        return self.header.column_records
+        if self._column_records is None:
+            self._column_records = list(self.header.column_records)
+            self._column_records.extend(self.footer.extension_links.column_records)
+            for i, cr in enumerate(self._column_records):
+                cr.idx = i
+        return self._column_records
+
+    @property
+    def alias_column_records(self):
+        if self._alias_column_records is None:
+            self._alias_column_records = list(self.header.alias_column_records)
+            self._alias_column_records.extend(
+                self.footer.extension_links.alias_column_records
+            )
+        return self._alias_column_records
+
+    @property
+    def _alias_columns_dict(self):
+        if self._alias_columns_dict_ is None:
+            self._alias_columns_dict_ = {
+                el.field_id: el.physical_id for el in self.alias_column_records
+            }
+        return self._alias_columns_dict_
+
+    @property
+    def _column_records_dict(self):
+        if self._column_records_dict_ is None:
+            self._column_records_dict_ = {}
+            for cr in self.column_records:
+                if cr.field_id not in self._column_records_dict_:
+                    self._column_records_dict_[cr.field_id] = [cr]
+                else:
+                    self._column_records_dict_[cr.field_id].append(cr)
+        return self._column_records_dict_
+
+    @property
+    def _related_ids(self):
+        if self._related_ids_ is None:
+            self._related_ids_ = defaultdict(list)
+            for i, el in enumerate(self.field_records):
+                if el.parent_field_id != i:
+                    self._related_ids_[el.parent_field_id].append(i)
+        return self._related_ids_
 
     @property
     def footer(self):
         if self._footer is None:
             if not self._footer_chunk_ready:
                 self._prepare_footer_chunk()
             cursor = self._footer_cursor.copy()
@@ -214,18 +269,18 @@
                 )
                 self._page_list_envelopes = PageLink().read(
                     decomp_chunk, cursor, context
                 )
 
         return self._page_list_envelopes
 
-    def base_col_form(self, cr, col_id, parameters=None):
+    def base_col_form(self, cr, col_id, parameters=None, cardinality=False):
         ak = uproot.extras.awkward()
 
-        form_key = f"column-{col_id}"
+        form_key = f"column-{col_id}" + ("-cardinality" if cardinality else "")
         dtype_byte = cr.type
         if dtype_byte == uproot.const.rntuple_role_union:
             return form_key
         elif dtype_byte > uproot.const.rntuple_role_struct:
             dt_str = uproot.const.rntuple_col_num_to_dtype_dict[dtype_byte]
             if dt_str == "bit":
                 dt_str = "bool"
@@ -236,52 +291,50 @@
             )
         else:  # offset index column
             return form_key
 
     def col_form(self, field_id):
         ak = uproot.extras.awkward()
 
-        if field_id in self._column_records_dict:
-            rel_crs = self._column_records_dict[field_id]["rel_crs"]
-            rel_crs_idxs = self._column_records_dict[field_id]["rel_crs_idxs"]
-        elif field_id in self._alias_columns_dict:
-            rel_crs = self._column_records_dict[self._alias_columns_dict[field_id]][
-                "rel_crs"
-            ]
-            rel_crs_idxs = self._column_records_dict[
-                self._alias_columns_dict[field_id]
-            ]["rel_crs_idxs"]
-        else:
+        cfid = field_id
+        if cfid in self._alias_columns_dict:
+            cfid = self._alias_columns_dict[cfid]
+        if cfid not in self._column_records_dict:
             raise (
                 RuntimeError(
-                    f"The filed_id: {field_id} is missing both from the columns records and the alias columns."
+                    f"The field_id: {cfid} is missing from the columns records."
                 )
             )
 
+        rel_crs = self._column_records_dict[cfid]
+
         if len(rel_crs) == 1:  # base case
-            return self.base_col_form(rel_crs[0], rel_crs_idxs[0])
+            cardinality = "RNTupleCardinality" in self.field_records[field_id].type_name
+            return self.base_col_form(
+                rel_crs[0], rel_crs[0].idx, cardinality=cardinality
+            )
         elif (
-            len(rel_crs_idxs) == 2
+            len(rel_crs) == 2
             and rel_crs[1].type == uproot.const.rntuple_col_type_to_num_dict["char"]
         ):
             # string field splits->2 in col records
             inner = self.base_col_form(
-                rel_crs[1], rel_crs_idxs[-1], parameters={"__array__": "char"}
+                rel_crs[1], rel_crs[1].idx, parameters={"__array__": "char"}
             )
-            form_key = f"column-{rel_crs_idxs[0]}"
+            form_key = f"column-{rel_crs[0].idx}"
             return ak.forms.ListOffsetForm(
                 "i64", inner, form_key=form_key, parameters={"__array__": "string"}
             )
         else:
             raise (RuntimeError(f"Missing special case: {field_id}"))
 
     def field_form(self, this_id, seen):
         ak = uproot.extras.awkward()
 
-        field_records = self.header.field_records
+        field_records = self.field_records
         this_record = field_records[this_id]
         seen.add(this_id)
         structural_role = this_record.struct_role
         if (
             structural_role == uproot.const.rntuple_role_leaf
             and this_record.repetition == 0
         ):
@@ -290,22 +343,40 @@
             return self.col_form(this_id)
         elif structural_role == uproot.const.rntuple_role_leaf:
             # std::array it only has one child
             if this_id in self._related_ids:
                 child_id = self._related_ids[this_id][0]
 
             inner = self.field_form(child_id, seen)
-            return ak.forms.RegularForm(inner, this_record.repetition)
+            keyname = f"RegularForm-{this_id}"
+            return ak.forms.RegularForm(inner, this_record.repetition, form_key=keyname)
         elif structural_role == uproot.const.rntuple_role_vector:
-            keyname = f"column-{this_id}"
+            if this_id not in self._related_ids or len(self._related_ids[this_id]) != 1:
+                keyname = f"vector-{this_id}"
+                newids = self._related_ids.get(this_id, [])
+                # go find N in the rest, N is the # of fields in vector
+                recordlist = [self.field_form(i, seen) for i in newids]
+                namelist = [field_records[i].field_name for i in newids]
+                return ak.forms.RecordForm(recordlist, namelist, form_key="whatever")
+            cfid = this_id
+            if cfid in self._alias_columns_dict:
+                cfid = self._alias_columns_dict[cfid]
+            if cfid not in self._column_records_dict:
+                raise (
+                    RuntimeError(
+                        f"The field_id: {cfid} is missing from the columns records."
+                    )
+                )
+            col_id = self._column_records_dict[cfid][0].idx
+            keyname = f"column-{col_id}"
             #  this only has one child
             if this_id in self._related_ids:
                 child_id = self._related_ids[this_id][0]
             inner = self.field_form(child_id, seen)
-            return ak.forms.ListOffsetForm("u32", inner, form_key=keyname)
+            return ak.forms.ListOffsetForm("i64", inner, form_key=keyname)
         elif structural_role == uproot.const.rntuple_role_struct:
             newids = []
             if this_id in self._related_ids:
                 newids = self._related_ids[this_id]
             # go find N in the rest, N is the # of fields in struct
             recordlist = [self.field_form(i, seen) for i in newids]
             namelist = [field_records[i].field_name for i in newids]
@@ -320,21 +391,23 @@
         else:
             # everything should recurse above this branch
             raise AssertionError("this should be unreachable")
 
     def to_akform(self):
         ak = uproot.extras.awkward()
 
-        field_records = self.header.field_records
+        field_records = self.field_records
         recordlist = []
         topnames = self.keys()
         seen = set()
         for i in range(len(field_records)):
             if i not in seen:
-                recordlist.append(self.field_form(i, seen))
+                ff = self.field_form(i, seen)
+                if field_records[i].type_name != "":
+                    recordlist.append(ff)
 
         form = ak.forms.RecordForm(recordlist, topnames, form_key="toplevel")
         return form
 
     def read_pagedesc(self, destination, desc, dtype_str, dtype, nbits, split):
         loc = desc.locator
         context = {}
@@ -354,88 +427,87 @@
 
             if nbits == 16:
                 # AAAAABBBBB needs to become
                 # ABABABABAB
                 res = numpy.empty(len(content), numpy.uint8)
                 res[0::2] = content[len(res) * 0 // 2 : len(res) * 1 // 2]
                 res[1::2] = content[len(res) * 1 // 2 : len(res) * 2 // 2]
-                res = res.view(numpy.uint16)
 
             elif nbits == 32:
                 # AAAAABBBBBCCCCCDDDDD needs to become
                 # ABCDABCDABCDABCDABCD
                 res = numpy.empty(len(content), numpy.uint8)
                 res[0::4] = content[len(res) * 0 // 4 : len(res) * 1 // 4]
                 res[1::4] = content[len(res) * 1 // 4 : len(res) * 2 // 4]
                 res[2::4] = content[len(res) * 2 // 4 : len(res) * 3 // 4]
                 res[3::4] = content[len(res) * 3 // 4 : len(res) * 4 // 4]
-                res = res.view(numpy.uint32)
 
             elif nbits == 64:
                 # AAAAABBBBBCCCCCDDDDDEEEEEFFFFFGGGGGHHHHH needs to become
                 # ABCDEFGHABCDEFGHABCDEFGHABCDEFGHABCDEFGH
                 res = numpy.empty(len(content), numpy.uint8)
                 res[0::8] = content[len(res) * 0 // 8 : len(res) * 1 // 8]
                 res[1::8] = content[len(res) * 1 // 8 : len(res) * 2 // 8]
                 res[2::8] = content[len(res) * 2 // 8 : len(res) * 3 // 8]
                 res[3::8] = content[len(res) * 3 // 8 : len(res) * 4 // 8]
                 res[4::8] = content[len(res) * 4 // 8 : len(res) * 5 // 8]
                 res[5::8] = content[len(res) * 5 // 8 : len(res) * 6 // 8]
                 res[6::8] = content[len(res) * 6 // 8 : len(res) * 7 // 8]
                 res[7::8] = content[len(res) * 7 // 8 : len(res) * 8 // 8]
-                res = res.view(numpy.uint64)
 
-            content = res
+            content = res.view(dtype)
 
         if isbit:
             content = (
                 numpy.unpackbits(content.view(dtype=numpy.uint8))
                 .reshape(-1, 8)[:, ::-1]
                 .reshape(-1)
             )
 
         # needed to chop off extra bits incase we used `unpackbits`
         destination[:] = content[:num_elements]
 
-    def read_col_pages(self, ncol, cluster_range):
-        return numpy.concatenate(
+    def read_col_pages(self, ncol, cluster_range, pad_missing_ele=False):
+        res = numpy.concatenate(
             [self.read_col_page(ncol, i) for i in cluster_range], axis=0
         )
+        if pad_missing_ele:
+            first_ele_index = self.column_records[ncol].first_ele_index
+            res = numpy.pad(res, (first_ele_index, 0))
+        return res
 
     def read_col_page(self, ncol, cluster_i):
         linklist = self.page_list_envelopes.pagelinklist[cluster_i]
         pagelist = linklist[ncol]
         dtype_byte = self.column_records[ncol].type
         dtype_str = uproot.const.rntuple_col_num_to_dtype_dict[dtype_byte]
         dtype = numpy.dtype("bool") if dtype_str == "bit" else numpy.dtype(dtype_str)
 
-        # FIXME vector read
-        # n.b. it's possible pagelist is empty
-        if not pagelist:
-            return numpy.empty(0, dtype)
-        total_len = numpy.sum([desc.num_elements for desc in pagelist])
+        total_len = numpy.sum([desc.num_elements for desc in pagelist], dtype=int)
         res = numpy.empty(total_len, dtype)
-        tracker = 0
         split = 14 <= dtype_byte <= 21 or 26 <= dtype_byte <= 28
+        zigzag = 26 <= dtype_byte <= 28
+        delta = dtype_byte in (14, 15)
+        index = dtype_byte in (0, 1, 14, 15)
         nbits = uproot.const.rntuple_col_num_to_size_dict[dtype_byte]
+        tracker = 0
+        cumsum = 0
         for page_desc in pagelist:
             n_elements = page_desc.num_elements
             tracker_end = tracker + n_elements
             self.read_pagedesc(
                 res[tracker:tracker_end], page_desc, dtype_str, dtype, nbits, split
             )
+            if delta:
+                res[tracker] -= cumsum
+                cumsum += numpy.sum(res[tracker:tracker_end])
             tracker = tracker_end
 
-        if (
-            dtype_byte <= uproot.const.rntuple_col_type_to_num_dict["index32"]
-            or 14 <= dtype_byte <= 15
-        ):
+        if index:
             res = numpy.insert(res, 0, 0)  # for offsets
-        zigzag = 26 <= dtype_byte <= 28
-        delta = 14 <= dtype_byte <= 15
         if zigzag:
             res = from_zigzag(res)
         elif delta:
             res = numpy.cumsum(res)
         return res
 
     def arrays(
@@ -458,59 +530,30 @@
             numpy.searchsorted(cluster_starts, entry_start, side="right") - 1
         )
         stop_cluster_idx = numpy.searchsorted(cluster_starts, entry_stop, side="right")
         cluster_num_entries = numpy.sum(
             [c.num_entries for c in clusters[start_cluster_idx:stop_cluster_idx]]
         )
 
-        self._alias_columns_dict = {
-            el.field_id: el.physical_id for el in self.header.alias_columns
-        }
-        self._column_records_dict = {}
-        self._column_records_idx_to_id = {}
-        for i, cr in enumerate(self.header.column_records):
-            if cr.field_id not in self._column_records_dict:
-                self._column_records_dict[cr.field_id] = {
-                    "rel_crs": [cr],
-                    "rel_crs_idxs": [i],
-                }
-            else:
-                self._column_records_dict[cr.field_id]["rel_crs"].append(cr)
-                self._column_records_dict[cr.field_id]["rel_crs_idxs"].append(i)
-            self._column_records_idx_to_id[i] = cr.field_id
-
-        self._related_ids = defaultdict(list)
-        for i, el in enumerate(self.header.field_records):
-            if el.parent_field_id != i:
-                self._related_ids[el.parent_field_id].append(i)
-
         form = self.to_akform().select_columns(filter_names)
         # only read columns mentioned in the awkward form
         target_cols = []
         container_dict = {}
         _recursive_find(form, target_cols)
         for key in target_cols:
             if "column" in key:
                 key_nr = int(key.split("-")[1])
-                key_fid = self._column_records_idx_to_id[key_nr]
-                if key_fid in self._column_records_dict:
-                    id = key_fid
-                elif key_nr in self._alias_columns_dict:
-                    id = self._alias_columns_dict[key_fid]
-                else:
-                    raise (
-                        RuntimeError(
-                            f"The key: {key} is missing both from the columns records and the alias columns."
-                        )
-                    )
-
-                dtype_byte = self._column_records_dict[id]["rel_crs"][0].type
+                dtype_byte = self.column_records[key_nr].type
                 content = self.read_col_pages(
-                    key_nr, range(start_cluster_idx, stop_cluster_idx)
+                    key_nr,
+                    range(start_cluster_idx, stop_cluster_idx),
+                    pad_missing_ele=True,
                 )
+                if "cardinality" in key:
+                    content = numpy.diff(content)
                 if dtype_byte == uproot.const.rntuple_col_type_to_num_dict["switch"]:
                     kindex, tags = _split_switch_bits(content)
                     container_dict[f"{key}-index"] = kindex
                     container_dict[f"{key}-tags"] = tags
                 else:
                     # don't distinguish data and offsets
                     container_dict[f"{key}-data"] = content
@@ -663,14 +706,20 @@
 # https://github.com/root-project/root/blob/aa513463b0b512517370cb91cca025e53a8b13a2/tree/ntuple/v7/doc/specifications.md#column-description
 class ColumnRecordReader:
     def read(self, chunk, cursor, context):
         out = MetaData("ColumnRecordFrame")
         out.type, out.nbits, out.field_id, out.flags = cursor.fields(
             chunk, _rntuple_column_record_format, context
         )
+        if out.flags & 0x08:
+            out.first_ele_index = cursor.field(
+                chunk, _rntuple_first_ele_index_format, context
+            )
+        else:
+            out.first_ele_index = 0
         return out
 
 
 class AliasColumnReader:
     def read(self, chunk, cursor, context):
         out = MetaData("AliasColumn")
 
@@ -712,29 +761,22 @@
         out.feature_flag = cursor.field(chunk, _rntuple_feature_flag_format, context)
         out.name, out.ntuple_description, out.writer_identifier = (
             cursor.rntuple_string(chunk, context) for _ in range(3)
         )
 
         out.field_records = self.list_field_record_frames.read(chunk, cursor, context)
         out.column_records = self.list_column_record_frames.read(chunk, cursor, context)
-        out.alias_columns = self.list_alias_column_frames.read(chunk, cursor, context)
-        out.extra_type_infos = self.list_extra_type_info_reader.read(
+        out.alias_column_records = self.list_alias_column_frames.read(
             chunk, cursor, context
         )
-        out.checksum = cursor.field(chunk, _rntuple_checksum_format, context)
-
-        return out
-
-    def read_extension_header(self, out, chunk, cursor, context):
-        out.field_records = self.list_field_record_frames.read(chunk, cursor, context)
-        out.column_records = self.list_column_record_frames.read(chunk, cursor, context)
-        out.alias_columns = self.list_alias_column_frames.read(chunk, cursor, context)
         out.extra_type_infos = self.list_extra_type_info_reader.read(
             chunk, cursor, context
         )
+        out.checksum = cursor.field(chunk, _rntuple_checksum_format, context)
+
         return out
 
 
 class ColumnGroupIDReader:
     def read(self, chunk, cursor, context):
         out = MetaData("ColumnGroupID")
         out.col_id = cursor.field(chunk, _rntuple_column_group_id_format, context)
@@ -776,15 +818,15 @@
         assert out.size >= 0, f"size={out.size}"
         out.field_records = ListFrameReader(
             RecordFrameReader(FieldRecordReader())
         ).read(chunk, cursor, context)
         out.column_records = ListFrameReader(
             RecordFrameReader(ColumnRecordReader())
         ).read(chunk, cursor, context)
-        out.alias_records = ListFrameReader(
+        out.alias_column_records = ListFrameReader(
             RecordFrameReader(AliasColumnReader())
         ).read(chunk, cursor, context)
         out.extra_type_info = ListFrameReader(
             RecordFrameReader(ExtraTypeInfoReader())
         ).read(chunk, cursor, context)
         return out
```

### Comparing `uproot-5.3.3/src/uproot/models/TArray.py` & `uproot-5.3.4/src/uproot/models/TArray.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         return "<{}{} {} at 0x{:012x}>".format(
             self.classname,
             version,
             numpy.array2string(
                 self._data,
                 max_line_width=numpy.inf,
                 separator=", ",
-                formatter={"float": lambda x: "%g" % x},
+                formatter={"float": lambda x: f"{x:g}"},
                 threshold=6,
             ),
             id(self),
         )
 
     def tojson(self):
         return self._data.tolist()
```

### Comparing `uproot-5.3.3/src/uproot/models/TAtt.py` & `uproot-5.3.4/src/uproot/models/TAtt.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/models/TBasket.py` & `uproot-5.3.4/src/uproot/models/TBasket.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/models/TBranch.py` & `uproot-5.3.4/src/uproot/models/TBranch.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/models/TClonesArray.py` & `uproot-5.3.4/src/uproot/models/TClonesArray.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/models/TDatime.py` & `uproot-5.3.4/src/uproot/models/TDatime.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/models/TGraph.py` & `uproot-5.3.4/src/uproot/models/TGraph.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/models/TH.py` & `uproot-5.3.4/src/uproot/models/TH.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/models/THashList.py` & `uproot-5.3.4/src/uproot/models/THashList.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/models/TLeaf.py` & `uproot-5.3.4/src/uproot/models/TLeaf.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/models/TList.py` & `uproot-5.3.4/src/uproot/models/TList.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/models/TMatrixT.py` & `uproot-5.3.4/src/uproot/models/TMatrixT.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/models/TNamed.py` & `uproot-5.3.4/src/uproot/models/TNamed.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/models/TObjArray.py` & `uproot-5.3.4/src/uproot/models/TObjArray.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/models/TObjString.py` & `uproot-5.3.4/src/uproot/models/TObjString.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/models/TObject.py` & `uproot-5.3.4/src/uproot/models/TObject.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/models/TRef.py` & `uproot-5.3.4/src/uproot/models/TRef.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         return "<{}{} {} at 0x{:012x}>".format(
             self.classname,
             version,
             numpy.array2string(
                 self._data,
                 max_line_width=numpy.inf,
                 separator=", ",
-                formatter={"float": lambda x: "%g" % x},
+                formatter={"float": lambda x: f"{x:g}"},
                 threshold=6,
             ),
             id(self),
         )
 
     @classmethod
     def awkward_form(cls, file, context):
```

### Comparing `uproot-5.3.3/src/uproot/models/TString.py` & `uproot-5.3.4/src/uproot/models/TString.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/models/TTable.py` & `uproot-5.3.4/src/uproot/models/TTable.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/models/TTime.py` & `uproot-5.3.4/src/uproot/models/TTime.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/models/TTree.py` & `uproot-5.3.4/src/uproot/models/TTree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/models/__init__.py` & `uproot-5.3.4/src/uproot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/sink/__init__.py` & `uproot-5.3.4/src/uproot/sink/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/sink/file.py` & `uproot-5.3.4/src/uproot/sink/file.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/source/__init__.py` & `uproot-5.3.4/src/uproot/source/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/source/chunk.py` & `uproot-5.3.4/src/uproot/source/chunk.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/source/cursor.py` & `uproot-5.3.4/src/uproot/source/cursor.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/source/file.py` & `uproot-5.3.4/src/uproot/source/file.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/source/fsspec.py` & `uproot-5.3.4/src/uproot/source/fsspec.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/source/futures.py` & `uproot-5.3.4/src/uproot/source/futures.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/source/http.py` & `uproot-5.3.4/src/uproot/source/http.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/source/object.py` & `uproot-5.3.4/src/uproot/source/object.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/source/s3.py` & `uproot-5.3.4/src/uproot/source/s3.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/source/xrootd.py` & `uproot-5.3.4/src/uproot/source/xrootd.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/writing/__init__.py` & `uproot-5.3.4/src/uproot/writing/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/writing/_cascade.py` & `uproot-5.3.4/src/uproot/writing/_cascade.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/writing/_cascadentuple.py` & `uproot-5.3.4/src/uproot/writing/_cascadentuple.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/writing/_cascadetree.py` & `uproot-5.3.4/src/uproot/writing/_cascadetree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/writing/_dask_write.py` & `uproot-5.3.4/src/uproot/writing/_dask_write.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/writing/identify.py` & `uproot-5.3.4/src/uproot/writing/identify.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/src/uproot/writing/writable.py` & `uproot-5.3.4/src/uproot/writing/writable.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/conftest.py` & `uproot-5.3.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0001_source_class.py` & `uproot-5.3.4/tests/test_0001_source_class.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0006_notify_when_downloaded.py` & `uproot-5.3.4/tests/test_0006_notify_when_downloaded.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0007_single_chunk_interface.py` & `uproot-5.3.4/tests/test_0007_single_chunk_interface.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0008_start_interpretation.py` & `uproot-5.3.4/tests/test_0008_start_interpretation.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,15 +45,16 @@
     assert not file.is_64bit
     assert file.fNbytesInfo == 4447
     assert file.hex_uuid == "944b77d0-98ab-11e7-a769-0100007fbeef"
 
 
 @pytest.mark.parametrize("use_deflate", [False, True])
 def test_file_header(use_deflate):
-    if use_deflate:
+    # FIXME: https://github.com/dcwatson/deflate/issues/42
+    if use_deflate and not uproot._util.macos:
         pytest.importorskip("deflate")
     uproot.ZLIB.use_deflate = use_deflate
     filename = skhep_testdata.data_path("uproot-Zmumu.root")
     file = uproot.reading.ReadOnlyFile(filename)
     assert repr(file.compression) == "ZLIB(4)"
     assert not file.is_64bit
     assert file.fNbytesInfo == 4447
```

### Comparing `uproot-5.3.3/tests/test_0009_nested_directories.py` & `uproot-5.3.4/tests/test_0009_nested_directories.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0010_start_streamers.py` & `uproot-5.3.4/tests/test_0010_start_streamers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0011_generate_classes_from_streamers.py` & `uproot-5.3.4/tests/test_0011_generate_classes_from_streamers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0013_rntuple_anchor.py` & `uproot-5.3.4/tests/test_0013_rntuple_anchor.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0014_all_ttree_versions.py` & `uproot-5.3.4/tests/test_0014_all_ttree_versions.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0016_interpretations.py` & `uproot-5.3.4/tests/test_0016_interpretations.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0017_multi_basket_multi_branch_fetch.py` & `uproot-5.3.4/tests/test_0017_multi_basket_multi_branch_fetch.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0018_array_fetching_interface.py` & `uproot-5.3.4/tests/test_0018_array_fetching_interface.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0022_number_of_branches.py` & `uproot-5.3.4/tests/test_0022_number_of_branches.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0023_more_interpretations_1.py` & `uproot-5.3.4/tests/test_0023_more_interpretations_1.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0023_ttree_versions.py` & `uproot-5.3.4/tests/test_0023_ttree_versions.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0029_more_string_types.py` & `uproot-5.3.4/tests/test_0029_more_string_types.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0031_test_stl_containers.py` & `uproot-5.3.4/tests/test_0031_test_stl_containers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0033_more_interpretations_2.py` & `uproot-5.3.4/tests/test_0033_more_interpretations_2.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0034_generic_objects_in_ttrees.py` & `uproot-5.3.4/tests/test_0034_generic_objects_in_ttrees.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0035_datatype_generality.py` & `uproot-5.3.4/tests/test_0035_datatype_generality.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0038_memberwise_serialization.py` & `uproot-5.3.4/tests/test_0038_memberwise_serialization.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0043_iterate_function.py` & `uproot-5.3.4/tests/test_0043_iterate_function.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0044_concatenate_function.py` & `uproot-5.3.4/tests/test_0044_concatenate_function.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0046_histograms_bh_hist.py` & `uproot-5.3.4/tests/test_0046_histograms_bh_hist.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0053_parents_should_not_be_bases.py` & `uproot-5.3.4/tests/test_0053_parents_should_not_be_bases.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0058_detach_model_objects_from_files.py` & `uproot-5.3.4/tests/test_0058_detach_model_objects_from_files.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0067_common_entry_offsets.py` & `uproot-5.3.4/tests/test_0067_common_entry_offsets.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0081_dont_parse_colons.py` & `uproot-5.3.4/tests/test_0081_dont_parse_colons.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0087_memberwise_splitting_not_implemented_messages.py` & `uproot-5.3.4/tests/test_0087_memberwise_splitting_not_implemented_messages.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0088_read_with_http.py` & `uproot-5.3.4/tests/test_0088_read_with_http.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0099_read_from_file_object.py` & `uproot-5.3.4/tests/test_0099_read_from_file_object.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0112_fix_pandas_with_cut.py` & `uproot-5.3.4/tests/test_0112_fix_pandas_with_cut.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0118_fix_name_fetch_again.py` & `uproot-5.3.4/tests/test_0118_fix_name_fetch_again.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0167_use_the_common_histogram_interface.py` & `uproot-5.3.4/tests/test_0167_use_the_common_histogram_interface.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0173_empty_and_multiprocessing_bugs.py` & `uproot-5.3.4/tests/test_0173_empty_and_multiprocessing_bugs.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0182_complain_about_missing_files.py` & `uproot-5.3.4/tests/test_0182_complain_about_missing_files.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0220_contiguous_byte_ranges_in_http.py` & `uproot-5.3.4/tests/test_0220_contiguous_byte_ranges_in_http.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0228_read_TProfiles.py` & `uproot-5.3.4/tests/test_0228_read_TProfiles.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0240_read_TGraphAsymmErrors.py` & `uproot-5.3.4/tests/test_0240_read_TGraphAsymmErrors.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0278_specializations_for_TParameter.py` & `uproot-5.3.4/tests/test_0278_specializations_for_TParameter.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0302_pickle.py` & `uproot-5.3.4/tests/test_0302_pickle.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0303_empty_jagged_array.py` & `uproot-5.3.4/tests/test_0303_empty_jagged_array.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0320_start_working_on_ROOT_writing.py` & `uproot-5.3.4/tests/test_0320_start_working_on_ROOT_writing.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0322_writablefile_infrastructure.py` & `uproot-5.3.4/tests/test_0322_writablefile_infrastructure.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0329_update_existing_root_files.py` & `uproot-5.3.4/tests/test_0329_update_existing_root_files.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0341_manipulate_streamer_info.py` & `uproot-5.3.4/tests/test_0341_manipulate_streamer_info.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0344_writabledirectory_can_read.py` & `uproot-5.3.4/tests/test_0344_writabledirectory_can_read.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0345_bulk_copy_method.py` & `uproot-5.3.4/tests/test_0345_bulk_copy_method.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0349_write_TObjString.py` & `uproot-5.3.4/tests/test_0349_write_TObjString.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0350_read_RooCurve_RooHist.py` & `uproot-5.3.4/tests/test_0350_read_RooCurve_RooHist.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0351_write_TList.py` & `uproot-5.3.4/tests/test_0351_write_TList.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0352_write_THashList.py` & `uproot-5.3.4/tests/test_0352_write_THashList.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0384_move_behavior_of_and_fix_383.py` & `uproot-5.3.4/tests/test_0384_move_behavior_of_and_fix_383.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0398_dimensions_in_leaflist.py` & `uproot-5.3.4/tests/test_0398_dimensions_in_leaflist.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0405_write_a_histogram.py` & `uproot-5.3.4/tests/test_0405_write_a_histogram.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0406_write_a_ttree.py` & `uproot-5.3.4/tests/test_0406_write_a_ttree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0407_read_TDatime.py` & `uproot-5.3.4/tests/test_0407_read_TDatime.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0412_write_multidimensional_numpy_to_ttree.py` & `uproot-5.3.4/tests/test_0412_write_multidimensional_numpy_to_ttree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0414_write_jagged_arrays.py` & `uproot-5.3.4/tests/test_0414_write_jagged_arrays.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0416_writing_compressed_data.py` & `uproot-5.3.4/tests/test_0416_writing_compressed_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,16 @@
                 34.1444372454,
                 22.7835819537,
             ]
 
 
 @pytest.mark.parametrize("use_deflate", [False, True])
 def test_deflate(use_deflate):
-    if use_deflate:
+    # FIXME: https://github.com/dcwatson/deflate/issues/42
+    if use_deflate and not uproot._util.macos:
         pytest.importorskip("deflate")
         uproot.ZLIB.library = "deflate"
     else:
         uproot.ZLIB.library = "zlib"
 
     for _ in range(2):
         with uproot.open(skhep_testdata.data_path("uproot-Zmumu-zlib.root"))[
@@ -129,15 +130,16 @@
     assert h3.GetNbinsX() == SIZE
     assert h3.GetBinContent(SIZE) == last
     f3.Close()
 
 
 @pytest.mark.parametrize("use_deflate", [False, True])
 def test_histogram_deflate(tmp_path, use_deflate):
-    if use_deflate:
+    # FIXME: https://github.com/dcwatson/deflate/issues/42
+    if use_deflate and not uproot._util.macos:
         pytest.importorskip("deflate")
         uproot.ZLIB.library = "deflate"
     else:
         uproot.ZLIB.library = "zlib"
 
     newfile = os.path.join(tmp_path, "newfile.root")
 
@@ -587,15 +589,16 @@
     assert [x.branch1 for x in t3] == branch1.tolist()
     assert [x.branch2 for x in t3] == branch2.tolist()
     f3.Close()
 
 
 @pytest.mark.parametrize("use_deflate", [False, True])
 def test_multicompression_1_deflate(tmp_path, use_deflate):
-    if use_deflate:
+    # FIXME: https://github.com/dcwatson/deflate/issues/42
+    if use_deflate and not uproot._util.macos:
         pytest.importorskip("deflate")
         uproot.ZLIB.library = "deflate"
     else:
         uproot.ZLIB.library = "zlib"
 
     newfile = os.path.join(tmp_path, "newfile.root")
 
@@ -621,15 +624,16 @@
     assert [x.branch1 for x in t3] == branch1.tolist()
     assert [x.branch2 for x in t3] == branch2.tolist()
     f3.Close()
 
 
 @pytest.mark.parametrize("use_deflate", [False, True])
 def test_multicompression_2_deflate(tmp_path, use_deflate):
-    if use_deflate:
+    # FIXME: https://github.com/dcwatson/deflate/issues/42
+    if use_deflate and not uproot._util.macos:
         pytest.importorskip("deflate")
         uproot.ZLIB.library = "deflate"
     else:
         uproot.ZLIB.library = "zlib"
 
     newfile = os.path.join(tmp_path, "newfile.root")
 
@@ -654,15 +658,16 @@
     assert [x.branch1 for x in t3] == branch1.tolist()
     assert [x.branch2 for x in t3] == branch2.tolist()
     f3.Close()
 
 
 @pytest.mark.parametrize("use_deflate", [False, True])
 def test_multicompression_3_deflate(tmp_path, use_deflate):
-    if use_deflate:
+    # FIXME: https://github.com/dcwatson/deflate/issues/42
+    if use_deflate and not uproot._util.macos:
         pytest.importorskip("deflate")
         uproot.ZLIB.library = "deflate"
     else:
         uproot.ZLIB.library = "zlib"
 
     newfile = os.path.join(tmp_path, "newfile.root")
 
@@ -688,15 +693,16 @@
     assert [x.branch1 for x in t3] == branch1.tolist()
     assert [x.branch2 for x in t3] == branch2.tolist()
     f3.Close()
 
 
 @pytest.mark.parametrize("use_deflate", [False, True])
 def test_multicompression_4_deflate(tmp_path, use_deflate):
-    if use_deflate:
+    # FIXME: https://github.com/dcwatson/deflate/issues/42
+    if use_deflate and not uproot._util.macos:
         pytest.importorskip("deflate")
         uproot.ZLIB.library = "deflate"
     else:
         uproot.ZLIB.library = "zlib"
 
     newfile = os.path.join(tmp_path, "newfile.root")
 
@@ -720,15 +726,16 @@
     assert [x.branch1 for x in t3] == branch1.tolist()
     assert [x.branch2 for x in t3] == branch2.tolist()
     f3.Close()
 
 
 @pytest.mark.parametrize("use_deflate", [False, True])
 def test_multicompression_5_deflate(tmp_path, use_deflate):
-    if use_deflate:
+    # FIXME: https://github.com/dcwatson/deflate/issues/42
+    if use_deflate and not uproot._util.macos:
         pytest.importorskip("deflate")
         uproot.ZLIB.library = "deflate"
     else:
         uproot.ZLIB.library = "zlib"
 
     newfile = os.path.join(tmp_path, "newfile.root")
```

### Comparing `uproot-5.3.3/tests/test_0418_read_TTable.py` & `uproot-5.3.4/tests/test_0418_read_TTable.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0420_pyroot_uproot_interoperability.py` & `uproot-5.3.4/tests/test_0420_pyroot_uproot_interoperability.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0422_hist_integration.py` & `uproot-5.3.4/tests/test_0422_hist_integration.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0438_TClonesArray_is_not_AsGrouped.py` & `uproot-5.3.4/tests/test_0438_TClonesArray_is_not_AsGrouped.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0442_regular_TClonesArray.py` & `uproot-5.3.4/tests/test_0442_regular_TClonesArray.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0472_tstreamerinfo_for_ttree.py` & `uproot-5.3.4/tests/test_0472_tstreamerinfo_for_ttree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0475_remember_to_update_freesegments.py` & `uproot-5.3.4/tests/test_0475_remember_to_update_freesegments.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0487_implement_asdtypeinplace.py` & `uproot-5.3.4/tests/test_0487_implement_asdtypeinplace.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0498_create_leaf_branch_in_extend.py` & `uproot-5.3.4/tests/test_0498_create_leaf_branch_in_extend.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0576_unicode_in_names.py` & `uproot-5.3.4/tests/test_0576_unicode_in_names.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0578_dask_for_numpy.py` & `uproot-5.3.4/tests/test_0578_dask_for_numpy.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0580_round_trip_for_no_flow_histograms.py` & `uproot-5.3.4/tests/test_0580_round_trip_for_no_flow_histograms.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0589_explicitly_interpret_RVec_type.py` & `uproot-5.3.4/tests/test_0589_explicitly_interpret_RVec_type.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0603_dask_delayed_open.py` & `uproot-5.3.4/tests/test_0603_dask_delayed_open.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0609_num_enteries_func.py` & `uproot-5.3.4/tests/test_0609_num_enteries_func.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0610_awkward_form.py` & `uproot-5.3.4/tests/test_0610_awkward_form.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0630_rntuple_basics.py` & `uproot-5.3.4/tests/test_0630_rntuple_basics.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0637_setup_tests_for_AwkwardForth.py` & `uproot-5.3.4/tests/test_0637_setup_tests_for_AwkwardForth.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0643_reading_vector_pair_TLorentzVector_int.py` & `uproot-5.3.4/tests/test_0643_reading_vector_pair_TLorentzVector_int.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0651_implement_transformed_axis.py` & `uproot-5.3.4/tests/test_0651_implement_transformed_axis.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0652_dask_for_awkward.py` & `uproot-5.3.4/tests/test_0652_dask_for_awkward.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0662_rntuple_stl_containers.py` & `uproot-5.3.4/tests/test_0662_rntuple_stl_containers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0692_fsspec_reading.py` & `uproot-5.3.4/tests/test_0692_fsspec_reading.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0692_fsspec_writing.py` & `uproot-5.3.4/tests/test_0692_fsspec_writing.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0700_dask_empty_arrays.py` & `uproot-5.3.4/tests/test_0700_dask_empty_arrays.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0705_rntuple_writing_metadata.py` & `uproot-5.3.4/tests/test_0705_rntuple_writing_metadata.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0755_dask_awkward_column_projection.py` & `uproot-5.3.4/tests/test_0755_dask_awkward_column_projection.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0791_protect_uproot_project_columns_from_dask_node_names.py` & `uproot-5.3.4/tests/test_0791_protect_uproot_project_columns_from_dask_node_names.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0798_DAOD_PHYSLITE.py` & `uproot-5.3.4/tests/test_0798_DAOD_PHYSLITE.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0808_fix_awkward_form_for_AsStridedObjects.py` & `uproot-5.3.4/tests/test_0808_fix_awkward_form_for_AsStridedObjects.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0816_separate_AwkwardForth_machines_by_TBranch.py` & `uproot-5.3.4/tests/test_0816_separate_AwkwardForth_machines_by_TBranch.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0832_ak_add_doc_should_also_add_to_typetracer.py` & `uproot-5.3.4/tests/test_0832_ak_add_doc_should_also_add_to_typetracer.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0840_support_tleafG.py` & `uproot-5.3.4/tests/test_0840_support_tleafG.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0841_fix_814.py` & `uproot-5.3.4/tests/test_0841_fix_814.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0844_fix_delete_hist_from_root.py` & `uproot-5.3.4/tests/test_0844_fix_delete_hist_from_root.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0876_uproot_dask_blind_steps.py` & `uproot-5.3.4/tests/test_0876_uproot_dask_blind_steps.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0911_fix_interp_array_non_numerical_objs_issue_880.py` & `uproot-5.3.4/tests/test_0911_fix_interp_array_non_numerical_objs_issue_880.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0912_fix_pandas_and_double_nested_vectors_issue_885.py` & `uproot-5.3.4/tests/test_0912_fix_pandas_and_double_nested_vectors_issue_885.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0916_read_from_s3.py` & `uproot-5.3.4/tests/test_0916_read_from_s3.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0930_expressions_in_pandas.py` & `uproot-5.3.4/tests/test_0930_expressions_in_pandas.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0940_feat_add_TLeafC_string_support.py` & `uproot-5.3.4/tests/test_0940_feat_add_TLeafC_string_support.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0962_RNTuple_update.py` & `uproot-5.3.4/tests/test_0962_RNTuple_update.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0965_inverted_axes_variances_hist_888.py` & `uproot-5.3.4/tests/test_0965_inverted_axes_variances_hist_888.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_0976_path_object_split.py` & `uproot-5.3.4/tests/test_0976_path_object_split.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_1000-write-TProfiles.py` & `uproot-5.3.4/tests/test_1000-write-TProfiles.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_1058_dask_awkward_report.py` & `uproot-5.3.4/tests/test_1058_dask_awkward_report.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_1063_dask_distributed.py` & `uproot-5.3.4/tests/test_1063_dask_distributed.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_1085_dask_write.py` & `uproot-5.3.4/tests/test_1085_dask_write.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_1114_fix_attempt_to_concatenate_numpy_with_awkward.py` & `uproot-5.3.4/tests/test_1114_fix_attempt_to_concatenate_numpy_with_awkward.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_1120_check_decompression_executor_pass_for_dask.py` & `uproot-5.3.4/tests/test_1120_check_decompression_executor_pass_for_dask.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_1127_fix_allow_colon_in_key_names.py` & `uproot-5.3.4/tests/test_1127_fix_allow_colon_in_key_names.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_1146_split_ranges_for_large_files_over_http.py` & `uproot-5.3.4/tests/test_1146_split_ranges_for_large_files_over_http.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_1154_classof_using_relative_path.py` & `uproot-5.3.4/tests/test_1154_classof_using_relative_path.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_1160_std_string_in_TDirectory.py` & `uproot-5.3.4/tests/test_1160_std_string_in_TDirectory.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_1180_read_free_floating_vector_issue_1179.py` & `uproot-5.3.4/tests/test_1180_read_free_floating_vector_issue_1179.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_1181_support_for_stl_list.py` & `uproot-5.3.4/tests/test_1181_support_for_stl_list.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_1182_add_support_for_bitset.py` & `uproot-5.3.4/tests/test_1182_add_support_for_bitset.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_1183_ttime_custom.py` & `uproot-5.3.4/tests/test_1183_ttime_custom.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_1186_dtype_might_raise_ValueError.py` & `uproot-5.3.4/tests/test_1186_dtype_might_raise_ValueError.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/test_1189_dask_failing_on_duplicate_keys.py` & `uproot-5.3.4/tests/test_1189_dask_failing_on_duplicate_keys.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/tests/samples/h_dynamic.pkl` & `uproot-5.3.4/tests/samples/h_dynamic.pkl`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/.gitignore` & `uproot-5.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/LICENSE` & `uproot-5.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/README.md` & `uproot-5.3.4/README.md`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/pyproject.toml` & `uproot-5.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uproot-5.3.3/PKG-INFO` & `uproot-5.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: uproot
-Version: 5.3.3
+Version: 5.3.4
 Summary: ROOT I/O in pure Python and NumPy.
 Project-URL: Download, https://github.com/scikit-hep/uproot5/releases
 Project-URL: Homepage, https://github.com/scikit-hep/uproot5
 Author-email: Jim Pivarski <pivarski@princeton.edu>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
```

