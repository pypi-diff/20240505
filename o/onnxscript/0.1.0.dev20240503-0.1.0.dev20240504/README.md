# Comparing `tmp/onnxscript-0.1.0.dev20240503.tar.gz` & `tmp/onnxscript-0.1.0.dev20240504.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-0.1.0.dev20240503.tar", last modified: Fri May  3 00:01:13 2024, max compression
+gzip compressed data, was "onnxscript-0.1.0.dev20240504.tar", last modified: Sat May  4 00:01:06 2024, max compression
```

## Comparing `onnxscript-0.1.0.dev20240503.tar` & `onnxscript-0.1.0.dev20240504.tar`

### file list

```diff
@@ -1,217 +1,217 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.848663 onnxscript-0.1.0.dev20240503/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-05-03 00:01:13.848663 onnxscript-0.1.0.dev20240503/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/VERSION
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.804663 onnxscript-0.1.0.dev20240503/onnxscript/
--rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.808663 onnxscript-0.1.0.dev20240503/onnxscript/_internal/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/_internal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/_internal/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/_internal/autocast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/_internal/deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/_internal/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/_internal/version_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.808663 onnxscript-0.1.0.dev20240503/onnxscript/_legacy_ir/
--rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/_legacy_ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/_legacy_ir/visitor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.808663 onnxscript-0.1.0.dev20240503/onnxscript/_thirdparty/
--rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/_thirdparty/asciichartpy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.808663 onnxscript-0.1.0.dev20240503/onnxscript/backend/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/backend/onnx_export.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/converter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.800663 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.812663 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/
--rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.824663 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/evaluator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.800663 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.800663 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/tools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.824663 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.824663 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/_flags.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.824663 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/graph_building/
--rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/graph_building/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28280 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
--rw-r--r--   0 vsts      (1001) docker     (127)    44452 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.828663 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/vision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/tensor_typing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.832663 onnxscript-0.1.0.dev20240503/onnxscript/ir/
--rw-r--r--   0 vsts      (1001) docker     (127)     2394 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8474 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/ir/_convenience.py
--rw-r--r--   0 vsts      (1001) docker     (127)    77357 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/ir/_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/ir/_display.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3908 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/ir/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/ir/_graph_comparison.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/ir/_invariants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/ir/_linked_list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/ir/_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/ir/_name_authority.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19570 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/ir/_protocols.py
--rw-r--r--   0 vsts      (1001) docker     (127)    47188 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/ir/serde.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.832663 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/
--rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.840663 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset20.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/onnx_types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.840663 onnxscript-0.1.0.dev20240503/onnxscript/optimizer/
--rw-r--r--   0 vsts      (1001) docker     (127)     4385 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/optimizer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10232 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/optimizer/constant_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/optimizer/evaluator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/optimizer/fold_constants_v0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/optimizer/remove_unused.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/optimizer/remove_unused_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9978 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/optimizer/simple_function_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.844663 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/_ir_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/_tape.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6405 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/broadcast_to_matmul.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1419 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/cast_constant_of_shape.py
--rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/erfgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/function_rule.py
--rw-r--r--   0 vsts      (1001) docker     (127)      747 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/gemm_to_matmul_add.py
--rw-r--r--   0 vsts      (1001) docker     (127)    35227 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/generic_pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)      832 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/no_op.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.844663 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/
--rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1257 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5196 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1824 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/softmax.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.848663 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)      602 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    29345 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)    34065 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/rewriter/pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/sourceinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/tensor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.848663 onnxscript-0.1.0.dev20240503/onnxscript/testing/
--rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/testing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/type_annotation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.848663 onnxscript-0.1.0.dev20240503/onnxscript/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/utils/evaluation_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/utils/timing_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/utils/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/onnxscript/values.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-03 00:01:13.848663 onnxscript-0.1.0.dev20240503/onnxscript.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-05-03 00:01:13.000000 onnxscript-0.1.0.dev20240503/onnxscript.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8162 2024-05-03 00:01:13.000000 onnxscript-0.1.0.dev20240503/onnxscript.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-03 00:01:13.000000 onnxscript-0.1.0.dev20240503/onnxscript.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-05-03 00:01:13.000000 onnxscript-0.1.0.dev20240503/onnxscript.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-03 00:01:13.000000 onnxscript-0.1.0.dev20240503/onnxscript.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-03 00:01:13.848663 onnxscript-0.1.0.dev20240503/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-05-03 00:00:54.000000 onnxscript-0.1.0.dev20240503/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.657064 onnxscript-0.1.0.dev20240504/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-05-04 00:01:06.657064 onnxscript-0.1.0.dev20240504/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/VERSION
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.629063 onnxscript-0.1.0.dev20240504/onnxscript/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.629063 onnxscript-0.1.0.dev20240504/onnxscript/_internal/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/_internal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/_internal/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/_internal/autocast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/_internal/deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/_internal/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/_internal/version_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.629063 onnxscript-0.1.0.dev20240504/onnxscript/_legacy_ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/_legacy_ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/_legacy_ir/visitor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.629063 onnxscript-0.1.0.dev20240504/onnxscript/_thirdparty/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/_thirdparty/asciichartpy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.629063 onnxscript-0.1.0.dev20240504/onnxscript/backend/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/converter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.625064 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.633064 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/
+-rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.637064 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/evaluator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.625064 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.625064 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/tools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.637064 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.637064 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/_flags.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.641064 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/graph_building/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/graph_building/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28280 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    44452 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.641064 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/ops/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/ops/vision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/tensor_typing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.641064 onnxscript-0.1.0.dev20240504/onnxscript/ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2394 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8474 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/ir/_convenience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    77357 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/ir/_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/ir/_display.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3908 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/ir/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/ir/_graph_comparison.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/ir/_invariants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/ir/_linked_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/ir/_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/ir/_name_authority.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19570 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/ir/_protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    47188 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/ir/serde.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.641064 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.645064 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset20.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/onnx_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.649064 onnxscript-0.1.0.dev20240504/onnxscript/optimizer/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4385 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/optimizer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10232 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/optimizer/constant_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/optimizer/evaluator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/optimizer/fold_constants_v0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/optimizer/remove_unused.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/optimizer/remove_unused_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9978 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/optimizer/simple_function_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.649064 onnxscript-0.1.0.dev20240504/onnxscript/rewriter/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/rewriter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/rewriter/_ir_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/rewriter/_tape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6405 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/rewriter/broadcast_to_matmul.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1419 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/rewriter/cast_constant_of_shape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/rewriter/erfgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/rewriter/function_rule.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      747 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/rewriter/gemm_to_matmul_add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29763 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/rewriter/generic_pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      832 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/rewriter/no_op.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.649064 onnxscript-0.1.0.dev20240504/onnxscript/rewriter/onnxruntime/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/rewriter/onnxruntime/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1257 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5196 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1824 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/rewriter/onnxruntime/softmax.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.657064 onnxscript-0.1.0.dev20240504/onnxscript/rewriter/onnxruntime/transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      602 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/rewriter/onnxruntime/transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29345 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34531 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/rewriter/pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/sourceinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/tensor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.657064 onnxscript-0.1.0.dev20240504/onnxscript/testing/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/type_annotation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.657064 onnxscript-0.1.0.dev20240504/onnxscript/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/utils/evaluation_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/utils/timing_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/utils/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/onnxscript/values.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-04 00:01:06.657064 onnxscript-0.1.0.dev20240504/onnxscript.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-05-04 00:01:06.000000 onnxscript-0.1.0.dev20240504/onnxscript.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8162 2024-05-04 00:01:06.000000 onnxscript-0.1.0.dev20240504/onnxscript.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-04 00:01:06.000000 onnxscript-0.1.0.dev20240504/onnxscript.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-05-04 00:01:06.000000 onnxscript-0.1.0.dev20240504/onnxscript.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-04 00:01:06.000000 onnxscript-0.1.0.dev20240504/onnxscript.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-04 00:01:06.657064 onnxscript-0.1.0.dev20240504/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-05-04 00:00:45.000000 onnxscript-0.1.0.dev20240504/setup.py
```

### Comparing `onnxscript-0.1.0.dev20240503/LICENSE` & `onnxscript-0.1.0.dev20240504/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/PKG-INFO` & `onnxscript-0.1.0.dev20240504/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240503
+Version: 0.1.0.dev20240504
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnxscript-0.1.0.dev20240503/README.md` & `onnxscript-0.1.0.dev20240504/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/__init__.py` & `onnxscript-0.1.0.dev20240504/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/_internal/analysis.py` & `onnxscript-0.1.0.dev20240504/onnxscript/_internal/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/_internal/ast_utils.py` & `onnxscript-0.1.0.dev20240504/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/_internal/autocast.py` & `onnxscript-0.1.0.dev20240504/onnxscript/_internal/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/_internal/deprecation.py` & `onnxscript-0.1.0.dev20240504/onnxscript/_internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/_internal/param_manipulation.py` & `onnxscript-0.1.0.dev20240504/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/_internal/runtime_typing.py` & `onnxscript-0.1.0.dev20240504/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/_internal/utils.py` & `onnxscript-0.1.0.dev20240504/onnxscript/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/_internal/version_utils.py` & `onnxscript-0.1.0.dev20240504/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/_legacy_ir/__init__.py` & `onnxscript-0.1.0.dev20240504/onnxscript/_legacy_ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/_legacy_ir/visitor.py` & `onnxscript-0.1.0.dev20240504/onnxscript/_legacy_ir/visitor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/_thirdparty/asciichartpy.py` & `onnxscript-0.1.0.dev20240504/onnxscript/_thirdparty/asciichartpy.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/backend/onnx_backend.py` & `onnxscript-0.1.0.dev20240504/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/backend/onnx_export.py` & `onnxscript-0.1.0.dev20240504/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/converter.py` & `onnxscript-0.1.0.dev20240504/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/context.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/diagnostics/infra/utils.py` & `onnxscript-0.1.0.dev20240504/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/evaluator.py` & `onnxscript-0.1.0.dev20240504/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py` & `onnxscript-0.1.0.dev20240504/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-0.1.0.dev20240504/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-0.1.0.dev20240504/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/_flags.py` & `onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/_flags.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/graph_building/__init__.py` & `onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/graph_building/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py` & `onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py` & `onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/common.py` & `onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/ops/common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/ops/vision.py` & `onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/ops/vision.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-0.1.0.dev20240504/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/ir/__init__.py` & `onnxscript-0.1.0.dev20240504/onnxscript/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/ir/_convenience.py` & `onnxscript-0.1.0.dev20240504/onnxscript/ir/_convenience.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/ir/_core.py` & `onnxscript-0.1.0.dev20240504/onnxscript/ir/_core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/ir/_display.py` & `onnxscript-0.1.0.dev20240504/onnxscript/ir/_display.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/ir/_enums.py` & `onnxscript-0.1.0.dev20240504/onnxscript/ir/_enums.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/ir/_graph_comparison.py` & `onnxscript-0.1.0.dev20240504/onnxscript/ir/_graph_comparison.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/ir/_invariants.py` & `onnxscript-0.1.0.dev20240504/onnxscript/ir/_invariants.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/ir/_linked_list.py` & `onnxscript-0.1.0.dev20240504/onnxscript/ir/_linked_list.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/ir/_metadata.py` & `onnxscript-0.1.0.dev20240504/onnxscript/ir/_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/ir/_name_authority.py` & `onnxscript-0.1.0.dev20240504/onnxscript/ir/_name_authority.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/ir/_protocols.py` & `onnxscript-0.1.0.dev20240504/onnxscript/ir/_protocols.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/ir/serde.py` & `onnxscript-0.1.0.dev20240504/onnxscript/ir/serde.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/irbuilder.py` & `onnxscript-0.1.0.dev20240504/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/main.py` & `onnxscript-0.1.0.dev20240504/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/__init__.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset20.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset20.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/onnx_types.py` & `onnxscript-0.1.0.dev20240504/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/optimizer/__init__.py` & `onnxscript-0.1.0.dev20240504/onnxscript/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/optimizer/constant_folding.py` & `onnxscript-0.1.0.dev20240504/onnxscript/optimizer/constant_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/optimizer/evaluator.py` & `onnxscript-0.1.0.dev20240504/onnxscript/optimizer/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/optimizer/fold_constants_v0.py` & `onnxscript-0.1.0.dev20240504/onnxscript/optimizer/fold_constants_v0.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/optimizer/remove_unused.py` & `onnxscript-0.1.0.dev20240504/onnxscript/optimizer/remove_unused.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/optimizer/remove_unused_function.py` & `onnxscript-0.1.0.dev20240504/onnxscript/optimizer/remove_unused_function.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/optimizer/simple_function_folding.py` & `onnxscript-0.1.0.dev20240504/onnxscript/optimizer/simple_function_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/__init__.py` & `onnxscript-0.1.0.dev20240504/onnxscript/rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/_ir_utils.py` & `onnxscript-0.1.0.dev20240504/onnxscript/rewriter/_ir_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/_tape.py` & `onnxscript-0.1.0.dev20240504/onnxscript/rewriter/_tape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/broadcast_to_matmul.py` & `onnxscript-0.1.0.dev20240504/onnxscript/rewriter/broadcast_to_matmul.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/cast_constant_of_shape.py` & `onnxscript-0.1.0.dev20240504/onnxscript/rewriter/cast_constant_of_shape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/erfgelu.py` & `onnxscript-0.1.0.dev20240504/onnxscript/rewriter/erfgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/function_rule.py` & `onnxscript-0.1.0.dev20240504/onnxscript/rewriter/function_rule.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/gemm_to_matmul_add.py` & `onnxscript-0.1.0.dev20240504/onnxscript/rewriter/gemm_to_matmul_add.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/generic_pattern.py` & `onnxscript-0.1.0.dev20240504/onnxscript/rewriter/generic_pattern.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,16 @@
 
 import collections
 import inspect
 import os
 import textwrap
 from typing import Any, Callable, Iterator, Sequence
 
-import onnx
-
-import onnxscript
 import onnxscript.rewriter.pattern as orp
 from onnxscript import ir
-from onnxscript.rewriter import _ir_utils
 
 
 class PatternMatchResult:
     """Stores information about a match if a match was successful.
 
     * pattern: the instance of :class:`GenericPattern` which found this result
     * model_nodes: matched nodes coming from the model
@@ -42,47 +38,49 @@
         self.pattern = pattern
         self.model_nodes = model_nodes
         self.pattern_nodes = pattern_nodes
         self.pattern_inputs = pattern_inputs
         self.pattern_outputs = pattern_outputs
         self.kwargs: dict[str, Any] = {}
 
-        matched_pattern_to_model_value: dict[ir.Value, ir.Value] = {}
+        matched_pattern_to_model_value: dict[str, ir.Value] = {}
         for gn, pn in zip(model_nodes, pattern_nodes):
             assert (
                 gn.op_type == pn.op_type
             ), f"Unexpected type mismatch {gn.op_type!r} != {pn.op_type!r}"
             assert len(gn.inputs) == len(
                 pn.inputs
             ), f"Unexpected number of inputs for type {gn.op_type}"
             for a, b in zip(gn.inputs, pn.inputs):
                 if b is None:
                     # optional input or not an interesting input
                     continue
-                if b in matched_pattern_to_model_value:
-                    assert matched_pattern_to_model_value[b] == a, (
-                        f"Ambiguities, pattern input {b!r} means "
-                        f"{a!r} or {matched_pattern_to_model_value[b]}"
+                b_name = b.name
+                assert b_name is not None
+                if b_name in matched_pattern_to_model_value:
+                    assert matched_pattern_to_model_value[b_name] == a, (
+                        f"Ambiguities, pattern input '{b_name}' means "
+                        f"'{a!r}' or '{matched_pattern_to_model_value[b_name]}'"
                     )
                 else:
-                    assert b is not None
-                    assert a is not None
-                    matched_pattern_to_model_value[b] = a
+                    matched_pattern_to_model_value[b_name] = a
 
             assert len(gn.outputs) == len(
                 pn.outputs
             ), f"Unexpected number of outputs for type {gn.op_type}"
             for a, b in zip(gn.outputs, pn.outputs):
-                if b in matched_pattern_to_model_value:
-                    assert matched_pattern_to_model_value[b] == a, (
-                        f"Ambiguities, pattern output {b!r} means "
-                        f"{a!r} or {matched_pattern_to_model_value[b]}"
+                b_name = b.name
+                assert b_name is not None
+                if b_name in matched_pattern_to_model_value:
+                    assert matched_pattern_to_model_value[b_name] == a, (
+                        f"Ambiguities, pattern output {b_name!r} means "
+                        f"{a!r} or {matched_pattern_to_model_value[b_name]}"
                     )
                 else:
-                    matched_pattern_to_model_value[b] = a
+                    matched_pattern_to_model_value[b_name] = a
 
         self.matched_pattern_to_model_value = matched_pattern_to_model_value
 
     def add_kwargs(self, name: str, value: Any):
         """Adds an attribute, it can be done when the match is being validated,
         this attribute can be used when building the replacement nodes.
         """
@@ -92,14 +90,29 @@
         return (
             f"{self.__class__.__name__}([{self.pattern.__class__.__name__}], "
             f"... {len(self.model_nodes)} nodes ..., {self.pattern_inputs}, "
             f"{self.pattern_outputs})"
         )
 
 
+def _to_match_result(pmr: PatternMatchResult) -> orp.MatchResult:
+    """Converts a PatternMatchResult into a MatchResult.
+
+    TODO: This is a temporary hack until MatchResult and PatternMatchResult are unified.
+    """
+    result = orp.MatchResult(success=True)
+    result.nodes.extend(pmr.model_nodes)
+    for var, val in pmr.matched_pattern_to_model_value.items():
+        result.bind(var, val)
+    result.outputs.extend(
+        [pmr.matched_pattern_to_model_value[v.name] for v in pmr.pattern_outputs]
+    )
+    return result
+
+
 class GenericRewriteRule(orp.RewriteRule):
     """
     Defines a rewriting rule.
 
         pattern: a pattern defines by :class:`GenericPattern`.
     """
 
@@ -110,51 +123,28 @@
     def matches(self, node: ir.Node, model: ir.Model) -> orp.MatchResult:
         del model
         del node
         raise RuntimeError(f"This pattern {self} is meant to replace not to only match.")
 
     def try_rewrite(
         self, model: ir.Model, graph_or_function: ir.Graph | ir.Function, node: ir.Node
-    ) -> tuple[int, list[ir.Node], list[ir.Node]] | None:
+    ) -> orp.ReplacementSubgraph | None:
         """See :meth:`RewriteRule.try_rewrite`."""
 
-        deleted_nodes: list[ir.Node] = []
-        added_nodes: list[ir.Node] = []
-        matched: set[ir.Node] = set()
-        match_count = 0
-        for match_result in self.pattern.enumerate_matches(model.graph, node):
-            conflict = False
-            for node in match_result.model_nodes:
-                if id(node) in matched:
-                    conflict = True
-                    break
-            if conflict:
-                # Some nodes are already matched as rewritten.
-                continue
-
-            # Let's build the new nodes
-            if not self.pattern.validate_mapping(model, match_result):
-                match_result._hint(
+        pattern_match_result = self.pattern.match(model.graph, node)
+        if pattern_match_result:
+            match_result = _to_match_result(pattern_match_result)
+            context = None  # TODO: create a context
+            if not self.pattern.validate_mapping(context, **match_result.bindings):
+                pattern_match_result._hint(
                     "validate_mapping", "The pattern was rejected by the validation function."
                 )
-                continue
-
-            new_nodes = self.pattern.apply(model, match_result, verbose=self.verbose)
-            assert all(
-                isinstance(i, ir.Node) for i in new_nodes
-            ), f"Unexpected types {[type(n) for n in new_nodes]}"
-
-            # Everything is good.
-            matched |= set(map(id, match_result.model_nodes))
-            added_nodes.extend(new_nodes)
-            deleted_nodes.extend(match_result.model_nodes)
-            match_count += 1
+                return None
 
-        if match_count > 0:
-            return match_count, deleted_nodes, added_nodes
+            return self.pattern.apply(model, match_result, verbose=self.verbose)
         return None
 
     def count_matches(self, model: ir.Model, *, commute: bool = False) -> int:
         """See :meth:`RewriteRule.count_matches`."""
         raise NotImplementedError("Not supported yet.")
 
     def commute(self) -> list[orp.RewriteRule]:
@@ -176,21 +166,14 @@
     * It does not compares attributes either (easy fix as well).
     """
 
     def __init__(self, verbose: int = 0):
         self.verbose = verbose
         self._cache: dict = {}
 
-    def validate_mapping(self, g: ir.Model, match_result: PatternMatchResult) -> bool:
-        """Evaluates the consistency of the replacements."""
-        raise NotImplementedError(
-            "This method could return True but it is better to let you know "
-            "that it exists. You need to overwrite it to return True."
-        )
-
     def enumerate_matches(
         self, graph: ir.Graph | ir.GraphView, node: ir.Node | None = None
     ) -> Iterator:
         """Enumerates all the matches."""
         if node is None:
             matched = []
             for node in graph:
@@ -261,76 +244,14 @@
                     msg2 = ""
                 print(
                     f"[{self.__class__.__name__}.match] NONE - line: {lineno}:"
                     f"{os.path.split(self.__class__.__module__)[-1]}, "
                     f"op_type={node.op_type}{msg}{msg2}"
                 )
 
-    @classmethod
-    def match_pattern(
-        cls,
-        g: ir.Graph,
-        *args: str,
-        **kwargs: Any,
-    ) -> Sequence[ir.Node] | None:
-        """Builds the pattern to match."""
-        raise NotImplementedError(
-            f"Class {cls.__name__!r} must overwrite method match_pattern."
-        )
-
-    def _build_pattern(
-        self,
-        func: Callable | None = None,
-        match: bool = True,
-        kwargs: dict[str, Any] | None = None,
-    ) -> ir.Graph:
-        del match
-        if func is None:
-            raise NotImplementedError(
-                f"Not implemented if func is None in class {self.__class__.__name__}"
-            )
-        if kwargs:
-            raise NotImplementedError(
-                f"Not implemented when kwargs is not empty but {kwargs} "
-                f"in class {self.__class__.__name__}"
-            )
-        kwargs = {}
-        args = []
-
-        # There should be a better way.
-        sig = inspect.signature(func)
-        for i, p in enumerate(sig.parameters.values()):
-            if i == 0:
-                continue
-            if p.default is not inspect._empty:
-                # an attribute
-                kwargs[p.name] = p.default
-            else:
-                args.append(p.name)
-
-        assert len(kwargs) == 0, f"Attributes are not supported yet but kwargs={kwargs}"
-
-        inputs = [ir.Input(name=name) for name in args]
-        builder = orp.RewriterContext()
-        outputs = func(builder, *inputs, **kwargs)
-        if isinstance(outputs, ir.Value):
-            outputs = [outputs]
-        graph = ir.Graph(inputs=inputs, outputs=outputs, nodes=builder.nodes)
-        graph.outputs[:] = outputs
-        return graph
-
-    def _get_match_pattern(self, g: ir.Graph | ir.GraphView) -> ir.Graph:
-        cache_key = 0, tuple(sorted(g.opset_imports.items()))
-        if cache_key in self._cache:
-            return self._cache[cache_key]
-
-        pat = self._build_pattern(self.match_pattern, match=True)
-        self._cache[cache_key] = pat
-        return pat
-
     def print_match(self, n1: ir.Node, n2: ir.Node) -> str:
         s1 = f"{n1.op_type}({n1.inputs})"
         s2 = f"{n2.op_type}({n2.inputs})"
         return f"match {s1} with {s2} (pattern)"
 
     def _debug_print(self) -> str:
         if not hasattr(self, "_debug"):
@@ -715,104 +636,30 @@
             self,
             matched_nodes,
             tuple(match_pattern),
             match_pattern.inputs,
             match_pattern.outputs,
         )
 
-    @classmethod
-    def apply_pattern(
-        cls,
-        g: ir.Model,
-        *args: Any,
-        **kwargs: Any,
-    ) -> Sequence[ir.Node]:
-        """Applies the replacement."""
-        raise NotImplementedError(
-            f"Class {cls.__name__!r} must overwrite method 'apply_pattern'."
-        )
-
     def apply(
         self,
         model: ir.Model,
-        match_result: PatternMatchResult,
+        match_result: orp.MatchResult,
         verbose: int = 0,
-    ) -> Sequence[ir.Node]:
-        assert isinstance(match_result, PatternMatchResult)
-        new_pattern = self._build_pattern(
-            self.apply_pattern, kwargs=match_result.kwargs, match=False
-        )
-        assert len(new_pattern.inputs) == len(match_result.pattern_inputs), (
-            f"Not the same number of inputs, "
-            f"matched inputs={len(new_pattern.inputs)}, "
-            f"got {len(match_result.pattern_inputs)} in the applied pattern."
-        )
-        assert len(new_pattern.outputs) == len(match_result.pattern_outputs), (
-            f"Not the same number of outputs, matched "
-            f"outputs={match_result.pattern_outputs}, "
-            f"got {new_pattern.outputs} in the applied pattern."
-        )
-
-        if verbose > 5:
-            print(
-                f"[GenericPattern.apply] replace {len(match_result.model_nodes)} nodes, "
-                f"applied {(self.apply_pattern)}"
-            )
-
-        # TODO: handle initializers here
-        # for name, init in pattern.initializers.items():
-        #   # We add them to the graph, they will be removed if unused.
-        #   new_name = g.make_initializer(name, init)
-        #   replacements[new_name] = name
-
-        applied_pattern_to_match_pattern: dict[ir.Value, ir.Value] = {}
-        for i, j in zip(match_result.pattern_inputs, new_pattern.inputs):
-            applied_pattern_to_match_pattern[j] = i
-        for i, j in zip(match_result.pattern_outputs, new_pattern.outputs):
-            applied_pattern_to_match_pattern[j] = i
-
-        replacements: dict[ir.Value, ir.Value] = {}
-        for k, v in applied_pattern_to_match_pattern.items():
-            replacements[k] = match_result.matched_pattern_to_model_value[v]
-
-        # Creation of the new node.
-        new_nodes: list[ir.Node] = []
-        for node in new_pattern:
-            new_inputs: list[ir.Value] = []
-            for i in node.inputs:
-                assert i in replacements, f"Unable to find {i!r} in {replacements}"
-                ni = replacements[i]
-                new_inputs.append(ni)
-            new_outputs: list[ir.Value] = []
-            for o in node.outputs:
-                if o in replacements:
-                    new_outputs.append(replacements[o])
-                else:
-                    # We give it a new name.
-                    replacements[o] = o
-                    new_outputs.append(o)
-            new_node = ir.Node(
-                domain=node.domain,
-                op_type=node.op_type,
-                inputs=new_inputs,
-                num_outputs=len(new_outputs),
-                attributes=node.attributes.values(),
-            )
-
-            for old_output, new_output in zip(node.outputs, new_node.outputs):
-                for i, graph_output in enumerate(old_output.producer().graph.outputs):
-                    if old_output is graph_output:
-                        new_output.meta[_ir_utils.GRAPH_OUTPUT_META_KEY] = i
-
-            new_nodes.append(new_node)
-
-        if verbose > 5:
-            print(f"[GenericPattern.apply] done with {len(new_nodes)} nodes")
-
-        return new_nodes
+    ) -> orp.ReplacementSubgraph | None:
+        x = orp.ReplacementPatternFunction(self.apply_pattern)
+        replacement = x.get_replacement(match_result)
+        # if replacement is not None:
+        #     TODO(Rama)
+        #     assert len(replacement.new_outputs) == len(match_result.pattern_outputs), (
+        #         f"Not the same number of outputs, matched "
+        #         f"outputs={match_result.pattern_outputs}, "
+        #         f"got {replacement.new_outputs} in the applied pattern."
+        #     )
+        return replacement
 
     def make_rule(self) -> orp.RewriteRule:
         """Creates the corresponding rule for this pattern."""
         return GenericRewriteRule(self)
 
 
 class FunctionPattern(GenericPattern):
@@ -828,73 +675,80 @@
             does not match
 
     """
 
     def __init__(
         self,
         match_pattern: ir.Function,
-        apply_pattern: ir.Function,
-        validate_mapping,
+        apply_pattern: Callable,
+        validate_mapping: Callable,
         verbose: int = 0,
     ):
         self.match_pattern = match_pattern
         self.apply_pattern = apply_pattern
         self.validate_mapping = validate_mapping
         self.verbose = verbose
 
-    def _build_pattern(self, pattern: Any, **kwargs) -> ir.Graph:
-        return pattern
-
     def _get_match_pattern(self, *_, **__):
         return self.match_pattern
 
 
+def _build_pattern(match_pattern_function: Callable) -> ir.Graph:
+    kwargs = {}
+    args = []
+
+    # There should be a better way.
+    sig = inspect.signature(match_pattern_function)
+    for i, p in enumerate(sig.parameters.values()):
+        if i == 0:
+            continue
+        if p.default is not inspect._empty:
+            # an attribute
+            kwargs[p.name] = p.default
+        else:
+            args.append(p.name)
+
+    assert len(kwargs) == 0, f"Attributes are not supported yet but kwargs={kwargs}"
+
+    inputs = [ir.Input(name=name) for name in args]
+    builder = orp.RewriterContext()
+    outputs = match_pattern_function(builder, *inputs, **kwargs)
+    if isinstance(outputs, ir.Value):
+        outputs = [outputs]
+    # TODO(Rama): Should construct a function!
+    graph = ir.Graph(inputs=inputs, outputs=outputs, nodes=builder.nodes)
+    graph.outputs[:] = outputs
+    return graph
+
+
 def make_pattern_rule(
-    match_pattern: Callable | onnx.FunctionProto,
-    apply_pattern: Callable | onnx.FunctionProto,
+    match_pattern_function: Callable,
+    apply_pattern_function: Callable,
     validate_mapping: Callable | None = None,
     verbose: int = 0,
-    opsets: dict[str, onnxscript.values.Opset] | None = None,
 ) -> orp.RewriteRule:
     """
     Creates a rewriting rule from a callable or a function proto.
 
     Args:
-        match_pattern: a function interpreted by onnx-script
-            and converted into an onnx model, this model defines the
-            nodes to be replaced
-        apply_pattern: a function interpreted by onnx-script and
-            converted into an onnx model, this model defines the new nodes
-            replacing the matched nodes
-        validate_mapping: a function validating the matching once
-            it has happened, it is not valid, the pattern is not applied,
-            if not specified, the function always return True
-        opsets: opset to consider when converting the function into ONNX,
-            if not specified, it is opset 18 for the main opset, and opset 1
-            for domain com.microsoft.
+        match_pattern_function: an onnxscript-like function that defines
+            the pattern subgraph (nodes) to be replaced
+        apply_pattern_function: an onnxscript-like function that constructs
+            the replacement subgraph (new nodes replacing the matched nodes)
+        validate_mapping: a function that validates the matching subgraph once
+            it is found. If it returns False the pattern is not applied.
+            If not specified, it is equivalent to a function that always return True
         verbose: verbosity level
 
     Returns:
         the rewriting rule
     """
 
-    if opsets is None:
-        opsets = dict(
-            op=onnxscript.opset18, msft_op=onnxscript.values.Opset("com.microsoft", 1)
-        )
-
-    if not isinstance(apply_pattern, onnx.FunctionProto):
-        apply_pattern = onnxscript.script(**opsets)(apply_pattern).to_function_proto()
-
-    if not isinstance(match_pattern, onnx.FunctionProto):
-        match_pattern = onnxscript.script(**opsets)(match_pattern).to_function_proto()
-
-    match_function = ir.serde.deserialize_function(match_pattern)
-    apply_function = ir.serde.deserialize_function(apply_pattern)
+    match_pattern_ir = _build_pattern(match_pattern_function)
 
     pat = FunctionPattern(
-        match_function,
-        apply_function,
+        match_pattern_ir,
+        apply_pattern_function,
         validate_mapping or (lambda *_, **__: True),
         verbose=verbose,
     )
     return pat.make_rule()
```

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/no_op.py` & `onnxscript-0.1.0.dev20240504/onnxscript/rewriter/no_op.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/__init__.py` & `onnxscript-0.1.0.dev20240504/onnxscript/rewriter/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py` & `onnxscript-0.1.0.dev20240504/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py` & `onnxscript-0.1.0.dev20240504/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/softmax.py` & `onnxscript-0.1.0.dev20240504/onnxscript/rewriter/onnxruntime/softmax.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/transformers/__init__.py` & `onnxscript-0.1.0.dev20240504/onnxscript/rewriter/onnxruntime/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py` & `onnxscript-0.1.0.dev20240504/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py` & `onnxscript-0.1.0.dev20240504/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/transformers/layernorm.py` & `onnxscript-0.1.0.dev20240504/onnxscript/rewriter/onnxruntime/transformers/layernorm.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py` & `onnxscript-0.1.0.dev20240504/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/rewriter/pattern.py` & `onnxscript-0.1.0.dev20240504/onnxscript/rewriter/pattern.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,14 +248,15 @@
         # These include the internal nodes of the pattern that were matched, but not
         # the leaves (sub-trees) that match against the variables in the pattern.
         # These represent the values that will be replaced by the replacement pattern.
         self.matched_nodes: MutableSequence[ir.Node] = []
         # For a successful match, bindings is a dictionary of mapping pattern-variable-names
         # to values.
         self.bindings: dict[str, Any] = {}
+        self.outputs: MutableSequence[ir.Value] = []
 
     def __bool__(self):
         return self.success
 
     @classmethod
     def FAIL(cls):
         return cls(False)
@@ -607,28 +608,36 @@
         self._tape = _tape.Tape()
         self._used_opsets: UsedOpsets = []
 
     def __getattr__(self, op_type: str) -> Any:
         return lambda *args, **kwargs: self._make_node(op_type, args, kwargs)
 
     def _make_node(self, op_type: str, inputs: Sequence[ir.Value], kwargs: dict[str, Any]):
+        # TODO(rama): some of the following logic should move into the tape.
         domain = kwargs.pop("domain", "")
         version = kwargs.pop("version", None)
         self._used_opsets.append((domain, version))
         outputs = kwargs.pop("outputs", 1)
         if isinstance(outputs, Sequence):
             num_outputs = len(outputs)
         else:
             assert isinstance(outputs, int)
             num_outputs = outputs
         if num_outputs == 1:
-            return self._tape.op(op_type, inputs=inputs, attributes=kwargs, domain=domain)
-        return self._tape.op_multi_output(
+            value = self._tape.op(op_type, inputs=inputs, attributes=kwargs, domain=domain)
+            if isinstance(outputs, Sequence):
+                value.name = outputs[0]
+            return value
+        values = self._tape.op_multi_output(
             op_type, inputs=inputs, attributes=kwargs, domain=domain, num_outputs=num_outputs
         )
+        if isinstance(outputs, Sequence):
+            for value, name in zip(values, outputs):
+                value.name = name
+        return values
 
     @property
     def nodes(self) -> Sequence[ir.Node]:
         # TODO(rama): The current tape-based implementation will not track nodes added
         # via overloaded operators, eg., `x + y`. One possible way to fix this is to
         # have values/nodes know which tape they belong to (instead of a graph/function).
         # However, it is unclear we need this feature for rewriting: we could also
@@ -730,14 +739,15 @@
         match = self._target_pattern.matches_node(node)
         if (
             self._condition_function is not None
             and match
             and not self._condition_function(**match.bindings)
         ):
             return MatchResult.FAIL()
+        match.outputs.extend(node.outputs)
         return match
 
     def try_rewrite(
         self, model: ir.Model, graph_or_function: ir.Graph | ir.Function, node: ir.Node
     ) -> ReplacementSubgraph | None:
         """If the node matches the pattern, then replace the node with the replacement pattern."""
         match = self.matches(node, model)
@@ -820,32 +830,33 @@
                     graph_or_function.outputs[index] = new_output
 
         for d in matched_nodes:
             assert d in graph_or_function
         graph_or_function.remove(matched_nodes, safe=True)
     else:
         assert isinstance(delta, ReplacementSubgraph)
-        # Replace matched nodes with new nodes.
-        last_inserted = delta.new_nodes[-1]
+        # Replace matched nodes with new nodes, matched values with new values
+        old_values = delta.match.outputs
+        new_values = delta.new_outputs
 
-        for old_value, new_value in zip(node.outputs, last_inserted.outputs):
+        for old_value, new_value in zip(old_values, new_values):
             # Propagate relevant info from old value to new value
             # TODO(Rama): Perhaps we should merge old and new types. As of now, new
             # values don't have type information. Note that this could be a problem
             # for semantics-altering rewrite-rules: we should allow users to override
             # this for such rules.
             new_value.type = old_value.type
             new_value.shape = old_value.shape
             new_value.const_value = old_value.const_value
             new_value.name = old_value.name
 
         # Reconnect the users of the deleted node to use the new outputs
-        _convenience.replace_all_uses_with(node.outputs, last_inserted.outputs)
+        _convenience.replace_all_uses_with(old_values, new_values)
         # Update graph/function outputs if the node generates output
-        replacement_mapping = dict(zip(node.outputs, last_inserted.outputs))
+        replacement_mapping = dict(zip(old_values, new_values))
         for idx, graph_or_function_output in enumerate(graph_or_function.outputs):
             if graph_or_function_output in replacement_mapping:
                 graph_or_function.outputs[idx] = replacement_mapping[graph_or_function_output]
 
         # insert new nodes after the index node
         graph_or_function.insert_after(node, delta.new_nodes)
         graph_or_function.remove(delta.match.nodes, safe=True)
```

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/sourceinfo.py` & `onnxscript-0.1.0.dev20240504/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/tensor.py` & `onnxscript-0.1.0.dev20240504/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/testing/__init__.py` & `onnxscript-0.1.0.dev20240504/onnxscript/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/type_annotation.py` & `onnxscript-0.1.0.dev20240504/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/utils/evaluation_utils.py` & `onnxscript-0.1.0.dev20240504/onnxscript/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/utils/timing_utils.py` & `onnxscript-0.1.0.dev20240504/onnxscript/utils/timing_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/utils/utils.py` & `onnxscript-0.1.0.dev20240504/onnxscript/utils/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript/values.py` & `onnxscript-0.1.0.dev20240504/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript.egg-info/PKG-INFO` & `onnxscript-0.1.0.dev20240504/onnxscript.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240503
+Version: 0.1.0.dev20240504
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnxscript-0.1.0.dev20240503/onnxscript.egg-info/SOURCES.txt` & `onnxscript-0.1.0.dev20240504/onnxscript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/pyproject.toml` & `onnxscript-0.1.0.dev20240504/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240503/setup.py` & `onnxscript-0.1.0.dev20240504/setup.py`

 * *Files identical despite different names*

